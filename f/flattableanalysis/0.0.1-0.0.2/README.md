# Comparing `tmp/flattableanalysis-0.0.1.tar.gz` & `tmp/flattableanalysis-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flattableanalysis-0.0.1.tar", max compression
+gzip compressed data, was "flattableanalysis-0.0.2.tar", max compression
```

## Comparing `flattableanalysis-0.0.1.tar` & `flattableanalysis-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2024-03-24 16:40:25.606567 flattableanalysis-0.0.1/LICENSE
--rw-r--r--   0        0        0       51 2024-03-24 16:40:25.606567 flattableanalysis-0.0.1/flattableanalysis/__init__.py
--rw-r--r--   0        0        0    15417 2024-03-24 16:40:25.606567 flattableanalysis-0.0.1/flattableanalysis/flat_table_analysis.py
--rw-r--r--   0        0        0      219 2024-03-24 16:40:25.606567 flattableanalysis-0.0.1/flattableanalysis/utils.py
--rw-r--r--   0        0        0      433 2024-03-24 16:40:35.122654 flattableanalysis-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 flattableanalysis-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-14 18:45:26.625920 flattableanalysis-0.0.2/LICENSE
+-rw-r--r--   0        0        0       51 2024-04-14 18:45:26.625920 flattableanalysis-0.0.2/flattableanalysis/__init__.py
+-rw-r--r--   0        0        0    20278 2024-04-14 18:45:26.625920 flattableanalysis-0.0.2/flattableanalysis/flat_table_analysis.py
+-rw-r--r--   0        0        0     2314 2024-04-14 18:45:26.625920 flattableanalysis-0.0.2/flattableanalysis/utils.py
+-rw-r--r--   0        0        0      433 2024-04-14 18:45:36.185990 flattableanalysis-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      674 1970-01-01 00:00:00.000000 flattableanalysis-0.0.2/PKG-INFO
```

### Comparing `flattableanalysis-0.0.1/LICENSE` & `flattableanalysis-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flattableanalysis-0.0.1/flattableanalysis/flat_table_analysis.py` & `flattableanalysis-0.0.2/flattableanalysis/flat_table_analysis.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import numpy as np
 import pandas as pd
 
 import itertools as it
-import more_itertools as mit
 
 import networkx as nx
 import graphviz
-import igraph as ig
 
 import math
 from collections.abc import Iterable
 from collections import Counter
-from typing import Union, Optional
+from typing import Union, Optional, Tuple, List
 from IPython.display import display
 from tqdm.notebook import tqdm
 
 from .utils import wrap_text
 
 
 class FlatTableAnalysis:
     def __repr__(self) -> str:
         return f"FlatTableAnalysis instance\ndf.shape = {self.df.shape}"
 
     def __init__(
         self,
         df: pd.DataFrame,
+        remove_constant_columns: bool = True,
+        remove_all_unique_columns: bool = True,
+        remove_one_one_relations: bool = True,
     ) -> None:
         r"""
         check df for basic validity
         modify df to internal representation (factorize, unify nan, ...)
         convert dtypes for speedup
         """
         if not isinstance(df.columns, pd.core.indexes.base.Index):
@@ -37,45 +38,53 @@
         if not df.columns.is_unique:
             raise ValueError("DataFrame columns must be unique")
 
         if any(df.columns.isna()):
             raise ValueError("DataFrame columns must not contain NaN values")
 
         self.df = (
-            df.copy()
-            .replace(["None", "none", "nan", ""], [np.nan] * 4)
+            df.replace(["None", "none", "nan", ""], [np.nan] * 4)
             .fillna(np.nan)
             .rename(str, axis=1)
             .reset_index(drop=True)
         )
+
         # utils mappings
         self.col_pos = {col: pos for pos, col in enumerate(self.df)}.get
         self.col_to_unique = {
             col: self.df.loc[:, col].drop_duplicates().shape[0] for col in self.df
         }.get
 
-        # delete columns
-        to_delete = list(self.df.columns[self.df.columns.map(self.col_to_unique) == 1])
-        print("remove constants columns: ", to_delete)
-        self.df = self.df.loc[:, lambda df: df.columns.difference(to_delete)]
-
-        to_delete = list(
-            self.df.columns[self.df.columns.map(self.col_to_unique) == df.shape[0]]
-        )
-        print("remove all unique columns: ", to_delete)
-        self.df = self.df.loc[:, lambda df: df.columns.difference(to_delete)]
-
-        self.df = self._delete_one_one_relations(self.df)
-
-        self._df = (
-            self.df
-        )  # save df version without factorize, need for self.show_header_info()
+        # remove columns
+        if remove_constant_columns:
+            to_delete = list(
+                self.df.columns[self.df.columns.map(self.col_to_unique) == 1]
+            )
+            self.df = self.df.loc[:, lambda df: df.columns.difference(to_delete)]
+            print("remove_constant_columns: ", to_delete)
+        if remove_all_unique_columns:
+            to_delete = list(
+                self.df.columns[self.df.columns.map(self.col_to_unique) == df.shape[0]]
+            )
+            self.df = self.df.loc[:, lambda df: df.columns.difference(to_delete)]
+            print("remove_all_unique_columns: ", to_delete)
+        if remove_one_one_relations:
+            self.df = self._delete_one_one_relations(self.df)
+
+        if self.df.empty:
+            raise Exception("removed all columns during preprocessing")
+
+        self._make_header_info()  # store info befor factorize erase it
+
+        # final processing
         self.df = (
             self.df.drop_duplicates()
-            .apply(lambda ser: ser.factorize()[0])
+            .apply(
+                lambda ser: ser.factorize()[0]
+            )  # sentinel -1 will be used for NaN values
             .pipe(lambda obj: obj if isinstance(obj, pd.DataFrame) else obj.to_frame())
             .assign(
                 **{
                     col: lambda df, col=col: df[col].astype("category")
                     for col in self.df
                 }
             )
@@ -95,106 +104,143 @@
             if (
                 self.col_to_unique(cols[0])
                 == self.col_to_unique(cols[1])
                 == df.loc[:, cols].drop_duplicates().shape[0]
             ):
                 edge_list.append(cols)
 
-        # if e.g. 4 cols have one-to-one relations between them -> need do delete all but one from them
+        # e.g. 4 cols have one-to-one relations between them -> we delete all but one
         G = nx.Graph()
         G.add_edges_from(edge_list)
-        to_delete = [
-            sorted(cc, key=self.col_pos)[1:] for cc in nx.connected_components(G)
-        ]
+        ccs = [sorted(cc, key=self.col_pos) for cc in nx.connected_components(G)]
+        to_delete = [cc[1:] for cc in ccs]
         to_delete = list(it.chain.from_iterable(to_delete))
         if to_delete:
-            print("deleted one-one relations", to_delete)
+            print("remove_one_one_relations: ", to_delete)
+            print(
+                "    found these sets of one-one relations, keep only 1st item from each: ",
+                ccs,
+            )
             return df.drop(to_delete, axis=1)
         else:
             return df
 
+    def _make_header_info(self) -> None:
+        r"""
+        prepare header info and store it on instance variable
+        """
+        col_name_width = min(max(len(c) for c in self.df) + 5, 35)
+        self.header_info = {}
+        d = {}
+        d["idx"] = "idx".ljust(5)
+        d["col name"] = "col name".ljust(col_name_width)
+        d["unique count"] = "unique count".ljust(15)
+        d["nan count"] = "nan count".ljust(15)
+        d["dtype"] = "dtype".ljust(15)
+        d["examples"] = "examples".ljust(15)
+        self.header_info["header"] = d
+        for idx, col in enumerate(self.df):
+            d = {}
+            d["idx"] = f"{idx:<5}"
+            d["col name"] = col[: col_name_width - 3].ljust(col_name_width)
+            d["unique count"] = f"{self.col_to_unique(col):<15_}"
+            d["nan count"] = f"{sum(self.df[col].isna()):<15_}"
+            d["dtype"] = str(self.df[col].dtype).ljust(15)
+            d["examples"] = str(list(self.df[col].dropna().unique()[:5]))[:70]
+            self.header_info[col] = d
+
     def show_header_info(self) -> None:
         r"""
         print header and relevant info about each columns. useful for analysis overview
         """
-        print(
-            f'{"idx":<5}',
-            f'{"col name":<15}',
-            f'{"unique count":<15}',
-            f'{"nan count":<15}',
-            f'{"dtype":<15}',
-            f'{"examples":<15}',
-        )
-        for idx, col in enumerate(self.df):
+        for _, header_info in self.header_info.items():
             print(
-                f"{idx:<5}",
-                f"{col:<20}"[:18],
-                f"{self.col_to_unique(col):<15_}",
-                f"{sum(self._df[col].isna()):<15_}",
-                f"{str(self._df[col].dtype):<15}",
-                f"{str(list(self._df[col].unique()[:5])):<15}"[:50],
+                header_info["idx"],
+                header_info["col name"],
+                header_info["unique count"],
+                header_info["nan count"],
+                header_info["dtype"],
+                header_info["examples"],
             )
         print(f"total rows: {self.df.shape[0]:_}")
 
     def get_candidate_keys(
         self,
-        col_nums: Optional[Union[int, Iterable[int]]] = None,
+        col_nums: int = 1,
     ) -> pd.DataFrame:
         r"""
         calculate cardinality for all sets of cols with given lengths
         sort them to show bigger cardinality and smaller sets of cols
         """
-        col_nums = col_nums or 1
-        col_nums = list(col_nums) if isinstance(col_nums, Iterable) else [col_nums]
-        if max(col_nums) > self.df.shape[1]:
-            raise ValueError("Maximum number of columns specified is larger than the number of DataFrame columns")
-        if min(col_nums) <= 0:
-            raise ValueError("Minimum number of columns must be greater than 0")
+        if col_nums > self.df.shape[1]:
+            raise ValueError(
+                "number of columns specified is larger than the number of DataFrame columns"
+            )
+        if col_nums <= 0:
+            raise ValueError("number of columns must be greater than 0")
 
         pbar = tqdm(
-            total=sum(math.comb(self.df.shape[1], col_num) for col_num in col_nums)
+            total=sum(
+                math.comb(self.df.shape[1], col_num)
+                for col_num in range(1, col_nums + 1)
+            )
         )
-        result = []
-        for col_num in col_nums:
+        candidates = []
+        for col_num in range(1, col_nums + 1):
             for col_names in it.combinations(self.df, r=col_num):
-                result.append(
-                    [col_names, self.df.loc[:, col_names].drop_duplicates().shape[0]]
-                )
+                unique_n = sum(~self.df.duplicated(subset=col_names))
+                col_names_set = set(col_names)
+
+                flag = True
+                for candidate in candidates:
+                    if col_names_set > candidate[0] and unique_n <= candidate[1]:
+                        flag = False
+                        break
+
+                if flag:
+                    candidates.append((col_names_set, unique_n))
                 pbar.update(1)
         pbar.close()
 
         return (
-            pd.DataFrame(result, columns=["col_names", "uniques"])
+            pd.DataFrame(candidates, columns=["col_names", "uniques"])
+            .assign(
+                col_names=lambda df: df["col_names"].map(
+                    lambda el: tuple(sorted(el, key=self.col_pos))
+                )
+            )
             .assign(total_rows=self.df.shape[0])
+            .assign(col_names_len=lambda df: df["col_names"].str.len())
             .assign(uniques_frac=lambda df: df["uniques"] / df["total_rows"])
-            .pipe(
-                lambda df: df.insert(1, "col_names_len", df["col_names"].str.len())
-                or df
+            .assign(
+                col_names_pos=lambda df: df["col_names"].map(
+                    lambda el: tuple(map(self.col_pos, el))
+                )  # for sorting only
             )
-            .sort_values(["uniques_frac", "col_names_len"], ascending=[False, True])
-            .reset_index(drop=True)
-            .pipe(
-                lambda df: df.assign(
-                    col_names=lambda df: df["col_names"].map(
-                        lambda el: tuple(sorted(el, key=self.col_pos))
-                    )
-                )
+            .sort_values(
+                ["uniques_frac", "col_names_len", "col_names_pos"],
+                ascending=[False, True, True],
             )
+            .drop("col_names_pos", axis=1)
+            .reset_index(drop=True)
+            .loc[
+                :,
+                ["col_names", "col_names_len", "uniques", "total_rows", "uniques_frac"],
+            ]
         )
 
     def show_fd_graph(
         self,
         threshold: Optional[Union[float, int]] = 1,
-    ) -> graphviz.Digraph:
+    ) -> Union[graphviz.Digraph, nx.classes.digraph.DiGraph]:
         r"""
         draw graph with functional dependancies (fds) as edges (between each pair of columns)
         fds may be not strict (threshold level)
-        for better visualization we remove transitive dependancies
         """
-        if not (0 < threshold <= 1):
+        if not 0 < threshold <= 1:
             raise ValueError("Threshold should be in the left-open interval (0, 1]")
 
         table = []
         for cols in it.combinations(self.df, r=2):
             table.append(
                 (cols[0], cols[1], self.df.loc[:, cols].drop_duplicates().shape[0])
             )
@@ -212,30 +258,47 @@
             if frac_L >= threshold:
                 edge_list.append((col_L, col_R, {"weight": round(frac_L, 2)}))
             if frac_R >= threshold:
                 edge_list.append((col_R, col_L, {"weight": round(frac_R, 2)}))
 
         G = nx.DiGraph()
         G.add_edges_from(edge_list)
-        if mit.first(nx.simple_cycles(G), False):  # if at leaste one cycle exists
-            H = ig.Graph.from_networkx(G)
-            edges_to_remove = H.feedback_arc_set()
-            H.delete_edges(edges_to_remove)
-            print(f"simple cylces removed {len(edges_to_remove)}")
-            G = H.to_networkx()
-        G_tr = nx.transitive_reduction(G)
-        G_tr.add_nodes_from(G.nodes(data=True))
-        G_tr.add_edges_from((u, v, G.edges[u, v]) for u, v in G.edges)
-
-        K = graphviz.Digraph(node_attr={"shape": "box"})
+        if threshold == 1:
+            G_tr = nx.transitive_reduction(G)
+            # need to copy data for nodes and edges manually
+            G_tr.add_nodes_from(G.nodes(data=True))
+            G_tr.add_edges_from((u, v, G.edges[u, v]) for u, v in G_tr.edges)
+            G = G_tr
+
+        K = graphviz.Digraph()
+        K.attr(
+            nodesep=".3",
+            ranksep=".3",
+            # size='8.5',
+            # ration='1',
+            rankdir="TB",
+            # ordering='out',
+            # splines='polyline',
+            bgcolor="antiquewhite",
+            fontsize="10",
+        )
+        K.attr(
+            "node",
+            shape="box",
+            style="filled",
+            color="lightblue2",
+            #    fontname='Helvetica',
+        )
+        # g.attr('edge', fontname='Helvetica')
         for col in self.df:
             K.node(wrap_text(col))
         for L, R, data in G.edges(data=True):
             K.edge(wrap_text(L), wrap_text(R), label=str(data["weight"]))
-        return K
+        K = K.unflatten(stagger=3, fanout=True, chain=5)
+        return K, G
 
     def get_density_table(self) -> pd.DataFrame:
         r"""
         applied to all columns pairs
         pair consists two columns
         main info: count of links compared to min and max possible (density)
         """
@@ -258,33 +321,50 @@
             .reset_index(drop=True)
         )
 
     def show_set_relation(
         self,
         L: Optional[Union[str, Iterable[str]]] = None,
         R: Optional[Union[str, Iterable[str]]] = None,
+        level: int = 1,
     ) -> None:
         r"""
         deep analysis of pair
         pair consists of two objects. each object may be one column or set of columns
         main info: types of connected components and their count
 
         additionaly shows tails types (nan, blanks, void) for each side of pair
         """
         L = L or self.df.columns[0]
         R = R or self.df.columns[1]
         L = [L] if isinstance(L, str) else list(L)
         R = [R] if isinstance(R, str) else list(R)
 
-        L_n, R_n = len(L), len(R)
+        subdf = self.df.loc[:, L + R].drop_duplicates()
+        total = subdf.shape[0]
+        L_one_nodes = sum(~subdf.loc[:, L].duplicated(keep=False))
+        R_one_nodes = sum(~subdf.loc[:, R].duplicated(keep=False))
+        L_nodes = sum(~subdf.loc[:, L].duplicated(keep="first"))
+        R_nodes = sum(~subdf.loc[:, R].duplicated(keep="first"))
+        LR_frac_edges = L_one_nodes / total
+        RL_frac_edges = R_one_nodes / total
+        LR_frac_nodes = L_one_nodes / L_nodes
+        RL_frac_nodes = R_one_nodes / R_nodes
+        print(
+            f"left unique {L_nodes:_}, right unique {R_nodes:_}, edges {total:_} ({total / (L_nodes * R_nodes):.5f}%)"
+        )
+        print(f"nodes: left fd -> {LR_frac_nodes:.5f}, right fd -> {RL_frac_nodes:.5f}")
+        print(f"edges: left fd -> {LR_frac_edges:.5f}, right fd -> {RL_frac_edges:.5f}")
+        if level == 1:
+            return
 
         G = nx.Graph()
-        L = self.df.loc[:, L].values.tolist()
-        R = self.df.loc[:, R].values.tolist()
-        for L_tup, R_tup in zip(L, R):
+        L_list = self.df.loc[:, L].values.tolist()
+        R_list = self.df.loc[:, R].values.tolist()
+        for L_tup, R_tup in zip(L_list, R_list):
             L_tup = (0,) + tuple(L_tup)
             R_tup = (1,) + tuple(R_tup)
             G.add_edge(L_tup, R_tup)
 
         CC_type = Counter()
         CC_all = []
         for cc in nx.connected_components(G):
@@ -297,53 +377,83 @@
             elif L_count > 1:
                 CC_type["many_one"] += 1
             elif R_count > 1:
                 CC_type["one_many"] += 1
             elif L_count == 1 and R_count == 1:
                 CC_type["one_one"] += 1
 
-        result = pd.Series(CC_type).reset_index().set_axis(["CC_type", "count"], axis=1)
+        result = (
+            pd.Series(CC_type)
+            .reset_index()
+            .set_axis(["CC_type", "count"], axis=1)
+            .sort_values("CC_type")
+        )
+        display(result)
+        if level == 2:
+            return
 
         CC_all = (
             sorted(CC_all, key=lambda el: el[0], reverse=True)[:20]
             + (["..."] if len(CC_all) > 20 else [])
             + sorted(CC_all, key=lambda el: el[1], reverse=True)[:20]
             + (["..."] if len(CC_all) > 20 else [])
         )
 
         zero_symbol = -1
         try:
-            L_nan_cc = nx.node_connected_component(G, tuple([0] + [zero_symbol] * L_n))
+            L_nan_cc = nx.node_connected_component(
+                G, tuple([0] + [zero_symbol] * len(L))
+            )
         except KeyError:
             L_nan_cc = []
         cc_flag = [node[0] for node in L_nan_cc]
         L_nan_L_count = cc_flag.count(0)
         L_nan_R_count = cc_flag.count(1)
 
         try:
-            R_nan_cc = nx.node_connected_component(G, tuple([1] + [zero_symbol] * R_n))
+            R_nan_cc = nx.node_connected_component(
+                G, tuple([1] + [zero_symbol] * len(R))
+            )
         except KeyError:
             R_nan_cc = []
         cc_flag = [node[0] for node in R_nan_cc]
         R_nan_L_count = cc_flag.count(0)
         R_nan_R_count = cc_flag.count(1)
 
-        display(result)
         print("_" * 50)
         display(CC_all)
         print("_" * 50)
         display(
             (
                 L_nan_L_count,
                 L_nan_R_count,
                 R_nan_L_count,
                 R_nan_R_count,
                 L_nan_cc == R_nan_cc,
             )
         )
+        if level == 3:
+            return
+
+    def fds(self, data: Iterable[Iterable[Iterable[str]]]) -> List[Tuple[bool, bool]]:
+        """
+        take list of pairs. Each pair include left columns set and right columns set
+        determine if fd exists (left->right and right->left)
+        method is intended for fast functional dependancy calculations
+        """
+        rv = []
+        for L, R in tqdm(data):
+            subdf = self.df.loc[:, L + R].drop_duplicates()
+            rv.append(
+                (
+                    any(subdf.loc[:, L].duplicated()),
+                    any(subdf.loc[:, R].duplicated()),
+                )
+            )
+        return rv
 
     def show_opposite_count(
         self,
         L: Optional[Union[str, Iterable[str]]] = None,
         R: Optional[Union[str, Iterable[str]]] = None,
     ) -> None:
         r"""
@@ -377,44 +487,74 @@
         )
         display(L_df)
         display(R_df)
 
     def get_cols_determinants(
         self,
         target: Optional[Union[str, Iterable[str]]] = None,
-        col_nums: Optional[Union[int, Iterable[int]]] = 1,
+        max_cols: int = 1,
     ) -> pd.DataFrame:
         r"""
         deep analysis of possible determinants of the object
         object may be one columns or set of columns
         determinants may be one column or set of columns
         main info: what columns defines object the best
         """
         target = target or [self.df.columns[0]]
         target = (str(target),) if isinstance(target, (int, str)) else tuple(target)
 
-        col_nums = [col_nums] if isinstance(col_nums, int) else list(col_nums)
-        if max(col_nums) > self.df.shape[1] - len(target):
-            raise ValueError("Maximum number of columns specified is larger than the number of available DataFrame columns")
-        if min(col_nums) <= 0:
+        if max_cols + len(target) > self.df.shape[1]:
+            raise ValueError(
+                "Maximum number of columns specified is larger than the number of available DataFrame columns"
+            )
+        if max_cols <= 0:
             raise ValueError("Minimum number of columns must be greater than 0")
 
         other_cols = list(self.df.columns.difference(target))
 
         pbar = tqdm(
-            total=sum(math.comb(len(other_cols), col_num) for col_num in col_nums)
+            total=sum(
+                math.comb(len(other_cols), col_num)
+                for col_num in range(1, max_cols + 1)
+            )
         )
-        result = []
-        for col_num in col_nums:
+
+        determinants = []
+        for col_num in range(1, max_cols + 1):
             for source in it.combinations(other_cols, r=col_num):
-                sub_df = self.df.loc[:, source + target].drop_duplicates()
-                LR_unique = sub_df.loc[:, source + target].drop_duplicates().shape[0]
-                L_unique = sub_df.loc[:, source].drop_duplicates().shape[0]
-                result.append((source, L_unique / LR_unique))
+                subdf = self.df.loc[:, source + target].drop_duplicates()
+                unique_n = sum(~subdf.loc[:, source].duplicated(keep=False))
+                frac = unique_n / subdf.shape[0]
+                source_set = set(source)
+
+                flag = True
+                for determinant in determinants:
+                    if source_set > determinant[0] and frac <= determinant[1]:
+                        flag = False
+                        break
+
+                if flag:
+                    determinants.append((source_set, frac))
                 pbar.update(1)
-        pbar.close
+        pbar.close()
 
         return (
-            pd.DataFrame(result, columns=["cols", "ratio"])
-            .sort_values("ratio", ascending=False)
+            pd.DataFrame(determinants, columns=["col_names", "frac"])
+            .assign(
+                col_names=lambda df: df["col_names"].map(
+                    lambda el: tuple(sorted(el, key=self.col_pos))
+                )
+            )
+            .assign(col_names_len=lambda df: df["col_names"].str.len())
+            .loc[:, ["col_names", "col_names_len", "frac"]]
+            .assign(
+                col_names_pos=lambda df: df["col_names"].map(
+                    lambda el: tuple(map(self.col_pos, el))
+                )  # for sorting only
+            )
+            .sort_values(
+                ["frac", "col_names_len", "col_names_pos"],
+                ascending=[False, True, True],
+            )
+            .drop("col_names_pos", axis=1)
             .reset_index(drop=True)
         )
```

### Comparing `flattableanalysis-0.0.1/PKG-INFO` & `flattableanalysis-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flattableanalysis
-Version: 0.0.1
+Version: 0.0.2
 Summary: Architectural analysis of a flat table. Discovering data from technical point of view.
 Author: Grigory T
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

