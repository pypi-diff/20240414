# Comparing `tmp/mfoci-0.1.4.tar.gz` & `tmp/mfoci-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfoci-0.1.4.tar", max compression
+gzip compressed data, was "mfoci-0.1.5.tar", max compression
```

## Comparing `mfoci-0.1.4.tar` & `mfoci-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      466 2024-04-07 13:43:46.157714 mfoci-0.1.4/mfoci/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 12:30:19.184929 mfoci-0.1.4/mfoci/factors/__init__.py
--rw-r--r--   0        0        0     2087 2024-04-07 12:37:06.216614 mfoci-0.1.4/mfoci/factors/esg_factors.py
--rw-r--r--   0        0        0      706 2024-04-07 13:13:28.373738 mfoci-0.1.4/mfoci/factors/fama_french.py
--rw-r--r--   0        0        0        0 2024-04-07 13:23:36.730502 mfoci-0.1.4/mfoci/helpers/__init__.py
--rw-r--r--   0        0        0      712 2024-04-07 13:30:58.556054 mfoci-0.1.4/mfoci/helpers/filterer.py
--rw-r--r--   0        0        0      957 2024-04-07 13:53:49.215591 mfoci-0.1.4/mfoci/methods/__init__.py
--rw-r--r--   0        0        0     1089 2024-04-07 13:53:46.987093 mfoci-0.1.4/mfoci/methods/kfoci.py
--rw-r--r--   0        0        0      668 2024-04-07 14:53:14.996525 mfoci-0.1.4/mfoci/methods/kfoci.R
--rw-r--r--   0        0        0     1146 2024-04-07 13:43:46.148861 mfoci-0.1.4/mfoci/methods/lasso.py
--rw-r--r--   0        0        0     2195 2024-04-07 14:59:32.883423 mfoci-0.1.4/mfoci/methods/mfoci_func.py
--rw-r--r--   0        0        0     2347 2024-04-07 12:47:46.625086 mfoci-0.1.4/mfoci/methods/multivar_chatterjee.py
--rw-r--r--   0        0        0        0 2024-04-07 12:31:23.708556 mfoci-0.1.4/mfoci/response_vars/__init__.py
--rw-r--r--   0        0        0      732 2024-04-07 12:37:06.222288 mfoci-0.1.4/mfoci/response_vars/etf_vars.py
--rw-r--r--   0        0        0      501 2024-04-07 14:49:03.295227 mfoci-0.1.4/mfoci/response_vars/stock_return_vars.py
--rw-r--r--   0        0        0      440 2024-04-07 14:24:51.227734 mfoci-0.1.4/mfoci/response_vars/volatility_vars.py
--rw-r--r--   0        0        0      613 2024-04-07 15:00:20.491543 mfoci-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2090 2024-04-07 14:46:22.936777 mfoci-0.1.4/README.md
--rw-r--r--   0        0        0     2809 1970-01-01 00:00:00.000000 mfoci-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      466 2024-04-07 13:43:46.157714 mfoci-0.1.5/mfoci/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 12:30:19.184929 mfoci-0.1.5/mfoci/factors/__init__.py
+-rw-r--r--   0        0        0     2087 2024-04-07 12:37:06.216614 mfoci-0.1.5/mfoci/factors/esg_factors.py
+-rw-r--r--   0        0        0      852 2024-04-11 06:52:49.858567 mfoci-0.1.5/mfoci/factors/fama_french.py
+-rw-r--r--   0        0        0        0 2024-04-07 13:23:36.730502 mfoci-0.1.5/mfoci/helpers/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-08 21:30:34.540726 mfoci-0.1.5/mfoci/helpers/filterer.py
+-rw-r--r--   0        0        0     1124 2024-04-13 09:24:17.156185 mfoci-0.1.5/mfoci/methods/__init__.py
+-rw-r--r--   0        0        0      972 2024-04-13 09:23:06.286866 mfoci-0.1.5/mfoci/methods/kfoci.py
+-rw-r--r--   0        0        0      761 2024-04-13 09:52:03.463824 mfoci-0.1.5/mfoci/methods/kfoci.R
+-rw-r--r--   0        0        0     1214 2024-04-08 21:39:16.466477 mfoci-0.1.5/mfoci/methods/lasso.py
+-rw-r--r--   0        0        0     2377 2024-04-11 09:52:16.793180 mfoci-0.1.5/mfoci/methods/mfoci_func.py
+-rw-r--r--   0        0        0     2347 2024-04-07 12:47:46.625086 mfoci-0.1.5/mfoci/methods/multivar_chatterjee.py
+-rw-r--r--   0        0        0        0 2024-04-07 12:31:23.708556 mfoci-0.1.5/mfoci/response_vars/__init__.py
+-rw-r--r--   0        0        0      732 2024-04-07 12:37:06.222288 mfoci-0.1.5/mfoci/response_vars/etf_vars.py
+-rw-r--r--   0        0        0      501 2024-04-07 14:49:03.295227 mfoci-0.1.5/mfoci/response_vars/stock_return_vars.py
+-rw-r--r--   0        0        0      438 2024-04-08 19:25:40.201137 mfoci-0.1.5/mfoci/response_vars/volatility_vars.py
+-rw-r--r--   0        0        0      613 2024-04-14 09:58:09.847416 mfoci-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2199 2024-04-14 09:58:09.851417 mfoci-0.1.5/README.md
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 mfoci-0.1.5/PKG-INFO
```

### Comparing `mfoci-0.1.4/mfoci/factors/esg_factors.py` & `mfoci-0.1.5/mfoci/factors/esg_factors.py`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.4/mfoci/factors/fama_french.py` & `mfoci-0.1.5/mfoci/factors/fama_french.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,12 +11,16 @@
     :return: pd.DataFrame
     """
     dataset_name = "F-F_Research_Data_5_Factors_2x3_daily"
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         ff5_data = pdr.get_data_famafrench(dataset_name, start=start_date, end=end_date)
     ff5 = ff5_data[0].reset_index().dropna()
-    ff5["placebo"] = np.random.rand(len(ff5))
+    # set seed
+    np.random.seed(1)
+    ff5["PLA-Unif"] = np.random.rand(len(ff5))
+    ff5["PLA-Gauss"] = np.random.randn(len(ff5))
+    ff5["PLA-Exp"] = np.exp(np.random.randn(len(ff5)))
     # ff5["Date"] = ff5["Date"].dt.strftime("%Y-%m-%d")
     ff5.set_index("Date", inplace=True)
     del ff5["RF"]
     return ff5
```

### Comparing `mfoci-0.1.4/mfoci/helpers/filterer.py` & `mfoci-0.1.5/mfoci/helpers/filterer.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,8 +9,9 @@
     filtered_factors = factors.loc[common_idx]
     n_response_dropped = response_vars.shape[0] - filtered_response_vars.shape[0]
     n_factors_dropped = factors.shape[0] - filtered_factors.shape[0]
     if n_response_dropped > 0:
         log.warning(f"Dropped {n_response_dropped} rows from response variables.")
     if n_factors_dropped > 0:
         log.warning(f"Dropped {n_factors_dropped} rows from factors.")
+    log.info(f"Response variables shape: {filtered_response_vars.shape}")
     return filtered_factors, filtered_response_vars
```

### Comparing `mfoci-0.1.4/mfoci/methods/__init__.py` & `mfoci-0.1.5/mfoci/methods/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,19 +10,23 @@
     :param factors: pd.DataFrame
     :param response_vars: pd.DataFrame
     :param method: str
 
     :return: list
     """
     if method == "mfoci":
-        return mfoci(factors, response_vars)
+        if "shuffle" not in kwargs:
+            kwargs["shuffle"] = True
+        return mfoci(factors, response_vars, shuffle=kwargs["shuffle"])
     elif method == "kfoci":
         if "r_path" not in kwargs:
             raise ValueError(
                 "R path must be specified for kfoci method, "
                 "e.g. 'C:/Program Files/R/R-4.3.3/bin/x64/Rscript'."
             )
-        return kfoci(factors, response_vars, kwargs["r_path"])
+        r_path = kwargs["r_path"]
+        del kwargs["r_path"]
+        return kfoci(factors, response_vars, r_path, **kwargs)
     elif method == "lasso":
         return select_indicators_with_lasso(factors, response_vars)
     else:
         raise ValueError(f"Method {method} not implemented.")
```

### Comparing `mfoci-0.1.4/mfoci/methods/mfoci_func.py` & `mfoci-0.1.5/mfoci/methods/mfoci_func.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,64 +5,69 @@
 
 from mfoci.methods.multivar_chatterjee import xi_q_n_calculate
 
 
 log = logging.getLogger(__name__)
 
 
-def mfoci(factors, response_vars, report_insignificant=False):
+def mfoci(factors, response_vars, report_insignificant=False, shuffle=True):
     """
     Multivariate FOCI - implements slide 31 from Jonathan's presentation
 
     :param factors: pd.DataFrame
     :param response_vars: pd.DataFrame
+    :param report_insignificant: bool
+    :param shuffle: bool
 
     :return: list
     """
     q = response_vars.shape[1]
     p = factors.shape[1]
     selected_factors = []
     max_t = 0
     max_ts = []
     n_selected = 0
     print(
         f"Starting MFOCI factor selection with {p} factors and {q} response variables. "
         f"Depending on the number of selected factors "
         f"there can be up to {p} iterations."
     )
+    y_order_range = range(q) if shuffle else range(1)
     for i in range(p):
         print(f"\nIteration {i + 1}:")
         t_js = []
         for j in tqdm(range(p)):
             if j in selected_factors:
                 t_js.append(0)
                 continue
             t_ks = []
-            k_range = range(q)
-            for k in k_range:  # shuffle y order to see effect on T^q
+            for k in y_order_range:  # shuffle y order to see effect on T^q
                 shuffled_y = pd.concat(
                     [response_vars.iloc[:, k:], response_vars.iloc[:, :k]], axis=1
                 )
                 t_k = xi_q_n_calculate(
                     factors.iloc[:, selected_factors + [j]], shuffled_y
                 )
                 t_ks.append(t_k)
-            t_j = sum(t_ks) / len(k_range)  # average over different orders of y
+            t_j = sum(t_ks) / len(y_order_range)  # average over different orders of y
             t_js.append(t_j)
         if max(t_js) <= max_t and n_selected == 0:
             n_selected = i
             if not report_insignificant:
                 break
         max_t = max(t_js)
         argmax = t_js.index(max_t)
         selected_factors.append(argmax)
         max_ts.append(max_t)
 
     t = [str(round(i, 3)) for i in max_ts]
     print("\nMFOCI results:")
     ind_str = ", ".join(factors.columns[selected_factors])
-    print(f"Predictive indicators are (in this order) {ind_str}")
+    print(
+        f"Predictive indicators for {', '.join(response_vars.columns)}"
+        f" are (in this order) {ind_str}"
+    )
     print(f"The corresponding T's are {' '.join(t)}")
     print(f"Number of selected variables is {n_selected}.")
     print("Done!")
 
     return selected_factors, max_ts
```

### Comparing `mfoci-0.1.4/mfoci/methods/multivar_chatterjee.py` & `mfoci-0.1.5/mfoci/methods/multivar_chatterjee.py`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.4/mfoci/response_vars/etf_vars.py` & `mfoci-0.1.5/mfoci/response_vars/etf_vars.py`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.4/pyproject.toml` & `mfoci-0.1.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mfoci"
-version = "0.1.4"
+version = "0.1.5"
 description = ""
 authors = ["Marcus Rockel <corram@outlook.de>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 # stock_loader = {path = "../../finadvisor/stock-loader", develop = true}
```

### Comparing `mfoci-0.1.4/README.md` & `mfoci-0.1.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -48,14 +48,17 @@
 factors, response_vars = filter_for_common_indices(factors, response_vars)
 
 # Factor selection using LASSO
 lasso_selected, coef = select_factors(factors, response_vars, "lasso")
 
 # KFOCI factor selection (ensure Rscript is installed and path is set)
 r_path = "C:/Program Files/R/R-4.3.3/bin/x64/Rscript"
-kfoci_linear_selected, kfoci_gaussian_selected = select_factors(
-    factors, response_vars, "kfoci", r_path=r_path
+kfoci_gauss_selected = select_factors(
+    factors, response_vars, "kfoci", r_path=r_path, kernel="rbfdot"
+)
+kfoci_laplace_selected = select_factors(
+    factors, response_vars, "kfoci", r_path=r_path, kernel="laplacedot"
 )
 
 # MFOCI factor selection
 mfoci_selected, t_values = select_factors(factors, response_vars, "mfoci")
 ```
```

### Comparing `mfoci-0.1.4/PKG-INFO` & `mfoci-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfoci
-Version: 0.1.4
+Version: 0.1.5
 Summary: 
 Author: Marcus Rockel
 Author-email: corram@outlook.de
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -71,15 +71,18 @@
 factors, response_vars = filter_for_common_indices(factors, response_vars)
 
 # Factor selection using LASSO
 lasso_selected, coef = select_factors(factors, response_vars, "lasso")
 
 # KFOCI factor selection (ensure Rscript is installed and path is set)
 r_path = "C:/Program Files/R/R-4.3.3/bin/x64/Rscript"
-kfoci_linear_selected, kfoci_gaussian_selected = select_factors(
-    factors, response_vars, "kfoci", r_path=r_path
+kfoci_gauss_selected = select_factors(
+    factors, response_vars, "kfoci", r_path=r_path, kernel="rbfdot"
+)
+kfoci_laplace_selected = select_factors(
+    factors, response_vars, "kfoci", r_path=r_path, kernel="laplacedot"
 )
 
 # MFOCI factor selection
 mfoci_selected, t_values = select_factors(factors, response_vars, "mfoci")
 ```
```

