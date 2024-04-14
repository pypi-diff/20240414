# Comparing `tmp/mcnets-2.0.6.tar.gz` & `tmp/mcnets-2.0.7.tar.gz`

## Comparing `mcnets-2.0.6.tar` & `mcnets-2.0.7.tar`

### file list

```diff
@@ -1,15 +1,11 @@
--rw-r--r--   0        0        0   129361 2020-02-02 00:00:00.000000 mcnets-2.0.6/src/mcnets/__deprecated.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mcnets-2.0.6/src/mcnets/__init__.py
--rw-r--r--   0        0        0    38662 2020-02-02 00:00:00.000000 mcnets-2.0.6/src/mcnets/_experimental.py
--rw-r--r--   0        0        0    14864 2020-02-02 00:00:00.000000 mcnets-2.0.6/src/mcnets/_nlp_tools.py
--rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 mcnets-2.0.6/src/mcnets/activations.py
--rw-r--r--   0        0        0    37101 2020-02-02 00:00:00.000000 mcnets-2.0.6/src/mcnets/main.py
--rw-r--r--   0        0        0    14837 2020-02-02 00:00:00.000000 mcnets-2.0.6/src/mcnets/tools.py
--rw-r--r--   0        0        0   792684 2020-02-02 00:00:00.000000 mcnets-2.0.6/stock tests/spy
--rw-r--r--   0        0        0    68789 2020-02-02 00:00:00.000000 mcnets-2.0.6/stock tests/stocks.xlsx
--rw-r--r--   0        0        0     3098 2020-02-02 00:00:00.000000 mcnets-2.0.6/stock tests/top500tickers_list
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 mcnets-2.0.6/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 mcnets-2.0.6/LICENSE
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 mcnets-2.0.6/README.md
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 mcnets-2.0.6/pyproject.toml
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 mcnets-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0   129361 2020-02-02 00:00:00.000000 mcnets-2.0.7/src/mcnets/__deprecated.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mcnets-2.0.7/src/mcnets/__init__.py
+-rw-r--r--   0        0        0    38662 2020-02-02 00:00:00.000000 mcnets-2.0.7/src/mcnets/_experimental.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 mcnets-2.0.7/src/mcnets/activations.py
+-rw-r--r--   0        0        0    37108 2020-02-02 00:00:00.000000 mcnets-2.0.7/src/mcnets/main.py
+-rw-r--r--   0        0        0    14926 2020-02-02 00:00:00.000000 mcnets-2.0.7/src/mcnets/tools.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 mcnets-2.0.7/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 mcnets-2.0.7/LICENSE
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 mcnets-2.0.7/README.md
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 mcnets-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 mcnets-2.0.7/PKG-INFO
```

### Comparing `mcnets-2.0.6/src/mcnets/__deprecated.py` & `mcnets-2.0.7/src/mcnets/__deprecated.py`

 * *Files identical despite different names*

### Comparing `mcnets-2.0.6/src/mcnets/_experimental.py` & `mcnets-2.0.7/src/mcnets/_experimental.py`

 * *Files identical despite different names*

### Comparing `mcnets-2.0.6/src/mcnets/activations.py` & `mcnets-2.0.7/src/mcnets/activations.py`

 * *Files identical despite different names*

### Comparing `mcnets-2.0.6/src/mcnets/main.py` & `mcnets-2.0.7/src/mcnets/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MCNet Dependancies
 from mcnets.activations import *
-from tools import *
+from mcnets.tools import *
 
 # Early Fitting - Ignore polynomial rank warnings
 import warnings
 warnings.simplefilter('ignore', np.RankWarning)
 
 
 ## =================== Models ==================== ##
```

### Comparing `mcnets-2.0.6/src/mcnets/tools.py` & `mcnets-2.0.7/src/mcnets/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,29 +343,30 @@
     """
 
     # Get locations of zeros and all else
     zeroLocs = np.where(yTrue == 0)
     nonZeroLocs = np.where(yTrue != 0)
 
     # Get scores form zero locations and non-zero locations
-    if len(zeroLocs[0]) > 0:
-        score_zeros = np.mean(np.abs(yPred[zeroLocs]))
-    else:
-        score_zeros = 0
-
-    if len(nonZeroLocs[0]) > 0:
-        score_nonzeros = np.mean(np.abs(yTrue[nonZeroLocs] - yPred[nonZeroLocs]) / np.abs(yTrue[nonZeroLocs]))
-    else:
-        score_nonzeros = 0
+    # if len(zeroLocs[0]) > 0:
+    #     score_zeros = np.mean(np.abs(yPred[zeroLocs]))
+    # else:
+    #     score_zeros = 0
+
+    # if len(nonZeroLocs[0]) > 0:
+    #     score_nonzeros = np.mean(np.abs(yTrue[nonZeroLocs] - yPred[nonZeroLocs]) / np.abs(yTrue[nonZeroLocs]))
+    # else:
+    #     score_nonzeros = 0
 
     # Get score average
-    avgScore = (score_zeros + score_nonzeros) / 2
+    # avgScore = (score_zeros + score_nonzeros) / 2
+    avg_score = np.mean(np.abs(yTrue - yPred) / (np.abs(yTrue) + 1))
 
     # Get/return RAE
-    return np.e ** (-avgScore)
+    return np.e ** (-avg_score)
 
 def normalize(array:np.ndarray):
     """
     ## Function
 
     Normalizes a given array (per col.) such that each point is the z-score for the given 
     columns mean and standard deviation. The returned array is a copy.
```

### Comparing `mcnets-2.0.6/LICENSE` & `mcnets-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mcnets-2.0.6/README.md` & `mcnets-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `mcnets-2.0.6/pyproject.toml` & `mcnets-2.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "numpy", "joblib"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mcnets"
-version = "2.0.6"
+version = "2.0.7"
 authors = [
   { name="Sean", email="svs.2k15@gmail.com" },
 ]
 description = "Lightweight Machine Learning package with models that train using simple Monte Carlo-like methods."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `mcnets-2.0.6/PKG-INFO` & `mcnets-2.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mcnets
-Version: 2.0.6
+Version: 2.0.7
 Summary: Lightweight Machine Learning package with models that train using simple Monte Carlo-like methods.
 Project-URL: Homepage, https://github.com/SciCapt/Monte-Carlo-Neural-Nets
 Project-URL: Bug Tracker, https://github.com/SciCapt/Monte-Carlo-Neural-Nets/issues
 Author-email: Sean <svs.2k15@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

