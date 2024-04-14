# Comparing `tmp/dtrc-0.0.8.tar.gz` & `tmp/dtrc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtrc-0.0.8.tar", last modified: Sat Apr  6 19:33:13 2024, max compression
+gzip compressed data, was "dtrc-0.0.9.tar", last modified: Sat Apr  6 19:59:16 2024, max compression
```

## Comparing `dtrc-0.0.8.tar` & `dtrc-0.0.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 19:33:13.478735 dtrc-0.0.8/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2023-11-17 13:08:05.000000 dtrc-0.0.8/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2023-11-17 13:08:05.000000 dtrc-0.0.8/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     3895 2024-04-06 19:33:13.478489 dtrc-0.0.8/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     2720 2023-12-22 19:25:54.000000 dtrc-0.0.8/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 19:33:13.476136 dtrc-0.0.8/dtrc/
--rw-r--r--   0 solst      (501) staff       (20)      641 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     8241 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)      626 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/atyp.py
--rw-r--r--   0 solst      (501) staff       (20)     3885 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/cats.py
--rw-r--r--   0 solst      (501) staff       (20)      589 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/cons.py
--rw-r--r--   0 solst      (501) staff       (20)     4674 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/data.py
--rw-r--r--   0 solst      (501) staff       (20)     6105 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/dmod.py
--rw-r--r--   0 solst      (501) staff       (20)     3889 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/dset.py
--rw-r--r--   0 solst      (501) staff       (20)      498 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/enum.py
--rw-r--r--   0 solst      (501) staff       (20)    16565 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/make.py
--rw-r--r--   0 solst      (501) staff       (20)     4791 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/poly.py
--rw-r--r--   0 solst      (501) staff       (20)     5350 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/trig.py
--rw-r--r--   0 solst      (501) staff       (20)     2548 2024-04-06 19:33:05.000000 dtrc-0.0.8/dtrc/util.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 19:33:13.477471 dtrc-0.0.8/dtrc.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     3895 2024-04-06 19:33:13.000000 dtrc-0.0.8/dtrc.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      424 2024-04-06 19:33:13.000000 dtrc-0.0.8/dtrc.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-06 19:33:13.000000 dtrc-0.0.8/dtrc.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-06 19:33:13.000000 dtrc-0.0.8/dtrc.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-24 17:50:00.000000 dtrc-0.0.8/dtrc.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)      154 2024-04-06 19:33:13.000000 dtrc-0.0.8/dtrc.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-06 19:33:13.000000 dtrc-0.0.8/dtrc.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      929 2024-04-06 19:33:03.000000 dtrc-0.0.8/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-06 19:33:13.478774 dtrc-0.0.8/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2585 2023-11-17 13:08:05.000000 dtrc-0.0.8/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 19:59:16.429796 dtrc-0.0.9/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2023-11-17 13:08:05.000000 dtrc-0.0.9/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2023-11-17 13:08:05.000000 dtrc-0.0.9/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     3895 2024-04-06 19:59:16.429550 dtrc-0.0.9/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     2720 2023-12-22 19:25:54.000000 dtrc-0.0.9/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 19:59:16.427519 dtrc-0.0.9/dtrc/
+-rw-r--r--   0 solst      (501) staff       (20)      641 2024-04-06 19:59:07.000000 dtrc-0.0.9/dtrc/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     8241 2024-04-06 19:59:07.000000 dtrc-0.0.9/dtrc/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)      626 2024-04-06 19:59:07.000000 dtrc-0.0.9/dtrc/atyp.py
+-rw-r--r--   0 solst      (501) staff       (20)     3885 2024-04-06 19:59:07.000000 dtrc-0.0.9/dtrc/cats.py
+-rw-r--r--   0 solst      (501) staff       (20)      589 2024-04-06 19:59:07.000000 dtrc-0.0.9/dtrc/cons.py
+-rw-r--r--   0 solst      (501) staff       (20)     4674 2024-04-06 19:59:07.000000 dtrc-0.0.9/dtrc/data.py
+-rw-r--r--   0 solst      (501) staff       (20)     6105 2024-04-06 19:59:07.000000 dtrc-0.0.9/dtrc/dmod.py
+-rw-r--r--   0 solst      (501) staff       (20)     3906 2024-04-06 19:59:07.000000 dtrc-0.0.9/dtrc/dset.py
+-rw-r--r--   0 solst      (501) staff       (20)      498 2024-04-06 19:59:07.000000 dtrc-0.0.9/dtrc/enum.py
+-rw-r--r--   0 solst      (501) staff       (20)    16565 2024-04-06 19:59:07.000000 dtrc-0.0.9/dtrc/make.py
+-rw-r--r--   0 solst      (501) staff       (20)     4791 2024-04-06 19:59:07.000000 dtrc-0.0.9/dtrc/poly.py
+-rw-r--r--   0 solst      (501) staff       (20)     5350 2024-04-06 19:59:07.000000 dtrc-0.0.9/dtrc/trig.py
+-rw-r--r--   0 solst      (501) staff       (20)     2548 2024-04-06 19:59:07.000000 dtrc-0.0.9/dtrc/util.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 19:59:16.428555 dtrc-0.0.9/dtrc.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     3895 2024-04-06 19:59:16.000000 dtrc-0.0.9/dtrc.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      424 2024-04-06 19:59:16.000000 dtrc-0.0.9/dtrc.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-06 19:59:16.000000 dtrc-0.0.9/dtrc.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-06 19:59:16.000000 dtrc-0.0.9/dtrc.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-24 17:50:00.000000 dtrc-0.0.9/dtrc.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)      154 2024-04-06 19:59:16.000000 dtrc-0.0.9/dtrc.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-06 19:59:16.000000 dtrc-0.0.9/dtrc.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      929 2024-04-06 19:33:57.000000 dtrc-0.0.9/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-06 19:59:16.429836 dtrc-0.0.9/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2585 2023-11-17 13:08:05.000000 dtrc-0.0.9/setup.py
```

### Comparing `dtrc-0.0.8/LICENSE` & `dtrc-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dtrc-0.0.8/PKG-INFO` & `dtrc-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtrc
-Version: 0.0.8
+Version: 0.0.9
 Summary: data torch
 Home-page: https://github.com/dsm-72/dtrc
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: dtrc data pytorch torch trc
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dtrc-0.0.8/README.md` & `dtrc-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dtrc-0.0.8/dtrc/__init__.py` & `dtrc-0.0.9/dtrc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00__init__.ipynb.
 
 # %% auto 0
 __all__ = []
 
 # %% ../nbs/00__init__.ipynb 3
 from itertools import chain
```

### Comparing `dtrc-0.0.8/dtrc/_modidx.py` & `dtrc-0.0.9/dtrc/_modidx.py`

 * *Files identical despite different names*

### Comparing `dtrc-0.0.8/dtrc/atyp.py` & `dtrc-0.0.9/dtrc/atyp.py`

 * *Files identical despite different names*

### Comparing `dtrc-0.0.8/dtrc/cats.py` & `dtrc-0.0.9/dtrc/cats.py`

 * *Files identical despite different names*

### Comparing `dtrc-0.0.8/dtrc/cons.py` & `dtrc-0.0.9/dtrc/cons.py`

 * *Files identical despite different names*

### Comparing `dtrc-0.0.8/dtrc/data.py` & `dtrc-0.0.9/dtrc/data.py`

 * *Files identical despite different names*

### Comparing `dtrc-0.0.8/dtrc/dmod.py` & `dtrc-0.0.9/dtrc/dmod.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 
 # %% ../nbs/60_dmod.ipynb 19
 from .cons import DATASET_CLS, DATAFRAME_FN
 from .util import DataSplits
 from .make import diamonds
 from .dset import PandasDataset, PandasCategoricalDataset, PandasTimeSeriesDataset
 
-# %% ../nbs/60_dmod.ipynb 26
+# %% ../nbs/60_dmod.ipynb 22
 class PandasDataModule(LightningDataModule):
     dl_kwargs: dict = dict(drop_last=True)
     batch_size: int = 32
     collate_fn: FunctionType | None
     dataframe_fn: FunctionType | None = diamonds
     splits: DataSplits = DataSplits(.7, .2, .1, .0)
     dataset_cls: FunctionType | None = PandasDataset
@@ -146,32 +146,32 @@
         return DataLoader(self.test_ds, **self.dl_kwargs)
 
     def predict_dataloader(self) -> DataLoader:      
         return DataLoader(self.pred_ds, **self.dl_kwargs)
 
     def teardown(self, stage: str | Stage): ...
 
-# %% ../nbs/60_dmod.ipynb 28
+# %% ../nbs/60_dmod.ipynb 24
 class PandasCategoricalDataModule(PandasDataModule):
     collate_fn = PandasCategoricalDataset.collate_fn
     dataset_cls: FunctionType | None = PandasCategoricalDataset
     
     def __init__(self, df: pd.DataFrame, col: str = LABEL, device: str = MPS, *args: P.args, **kwargs: P.kwargs):
         super().__init__(df, col, device, *args, **kwargs)
         self.n_cats = len(self.labels)
         
     def __len__(self) -> int:
         return min(grouplens(self.df, self.column))
 
-# %% ../nbs/60_dmod.ipynb 30
+# %% ../nbs/60_dmod.ipynb 26
 class PandasTimeSeriesDataModule(PandasCategoricalDataModule):
     collate_fn = PandasCategoricalDataset.collate_fn
     
     dataset_cls: FunctionType | None = PandasTimeSeriesDataset
     def __init__(self, df: pd.DataFrame, col: str = LABEL, device: str = MPS, *args: P.args, **kwargs: P.kwargs):
         super().__init__(df, col, device, *args, **kwargs)
         self.t_dict = dict(enumerate(self.labels))
         self.t_step = torch.linspace(0, self.n_cats - 1, self.n_cats)
 
-# %% ../nbs/60_dmod.ipynb 39
+# %% ../nbs/60_dmod.ipynb 38
 #| export
```

### Comparing `dtrc-0.0.8/dtrc/dset.py` & `dtrc-0.0.9/dtrc/dset.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 from etrc import Stage, BatchReturn, DataFormat
 
 # %% ../nbs/50_dset.ipynb 19
 from .make import diamonds
 from .util import DataSplits
 from .cats import torch_categorical_sample, categorical_collate_fn
 
-# %% ../nbs/50_dset.ipynb 25
+# %% ../nbs/50_dset.ipynb 22
 class PandasDataset(Dataset):
     def __init__(
         self, 
         df: pd.DataFrame, 
         col: str = LABEL, 
         device: str = MPS, 
         *args: P.args, 
@@ -81,48 +81,49 @@
         self.n_feat = len(df.columns) - (1 if col in df.columns else 0)
         self.device = device
         self.replace = replace
         
     def __len__(self) -> int:
         return self.df.shape[0]
 
-# %% ../nbs/50_dset.ipynb 27
+# %% ../nbs/50_dset.ipynb 24
 class PandasCategoricalDataset(PandasDataset):
     def __init__(
         self, df: pd.DataFrame, col: str = LABEL, device: str = MPS, *args: P.args, 
         replace: bool = False, 
         labels: pd.Series | None = None, 
         **kwargs: P.kwargs
     ):
         super().__init__(df, col, device, *args, replace=replace, labels=labels, **kwargs)
         self.n_cats = len(self.labels)
 
     def __len__(self) -> int:
         return min(grouplens(self.df, self.column))
     
+    @classmethod
     def collate_fn(cls, xys: tuple[tuple[torch.Tensor, torch.Tensor], ...]):
         return categorical_collate_fn(xys)
         xs = torch.concat(tuple(x for x, _ in xys), dim=1)
         ys = torch.concat(tuple(y for _, y in xys), dim=1)
         return (xs, ys)
 
     def __getitem__(self, idx):
         n = len(slice2range(idx)) if isslice(idx) else 1
         samples, labels = torch_categorical_sample(
             df=self.df, col=self.column, n=n, replace=self.replace, device=self.device)
         return samples, labels
 
-# %% ../nbs/50_dset.ipynb 28
+# %% ../nbs/50_dset.ipynb 25
 class PandasTimeSeriesDataset(PandasCategoricalDataset):
     def __init__(
         self, df: pd.DataFrame, col: str = LABEL, device: str = MPS, *args: P.args, 
         replace: bool = False, 
         labels: pd.Series | None = None, 
         **kwargs: P.kwargs
     ):
         super().__init__(df, col, device, *args, replace=replace, labels=labels, **kwargs)
         self.t_dict = dict(enumerate(self.labels))
         self.t_step = torch.linspace(0, self.n_cats - 1, self.n_cats)
 
-# %% ../nbs/50_dset.ipynb 33
+# %% ../nbs/50_dset.ipynb 32
 #| export
```

### Comparing `dtrc-0.0.8/dtrc/make.py` & `dtrc-0.0.9/dtrc/make.py`

 * *Files identical despite different names*

### Comparing `dtrc-0.0.8/dtrc/poly.py` & `dtrc-0.0.9/dtrc/poly.py`

 * *Files identical despite different names*

### Comparing `dtrc-0.0.8/dtrc/trig.py` & `dtrc-0.0.9/dtrc/trig.py`

 * *Files identical despite different names*

### Comparing `dtrc-0.0.8/dtrc/util.py` & `dtrc-0.0.9/dtrc/util.py`

 * *Files identical despite different names*

### Comparing `dtrc-0.0.8/dtrc.egg-info/PKG-INFO` & `dtrc-0.0.9/dtrc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtrc
-Version: 0.0.8
+Version: 0.0.9
 Summary: data torch
 Home-page: https://github.com/dsm-72/dtrc
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: dtrc data pytorch torch trc
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dtrc-0.0.8/settings.ini` & `dtrc-0.0.9/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = dtrc
 lib_name = dtrc
-version = 0.0.8
+version = 0.0.9
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = dtrc
 nbs_path = nbs
 recursive = True
```

### Comparing `dtrc-0.0.8/setup.py` & `dtrc-0.0.9/setup.py`

 * *Files identical despite different names*

