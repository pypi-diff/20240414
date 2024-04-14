# Comparing `tmp/calibrated_explanations-0.3.1a0.tar.gz` & `tmp/calibrated_explanations-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calibrated_explanations-0.3.1a0.tar", last modified: Fri Feb 23 17:39:38 2024, max compression
+gzip compressed data, was "calibrated_explanations-0.3.2.tar", last modified: Sun Apr 14 00:06:14 2024, max compression
```

## Comparing `calibrated_explanations-0.3.1a0.tar` & `calibrated_explanations-0.3.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-02-23 17:39:38.975140 calibrated_explanations-0.3.1a0/
--rw-rw-rw-   0        0        0     1532 2023-12-07 10:33:41.000000 calibrated_explanations-0.3.1a0/LICENSE
--rw-rw-rw-   0        0        0    20522 2024-02-23 17:39:38.971140 calibrated_explanations-0.3.1a0/PKG-INFO
--rw-rw-rw-   0        0        0    19642 2024-02-23 16:56:59.000000 calibrated_explanations-0.3.1a0/README.md
--rw-rw-rw-   0        0        0      971 2024-02-23 17:38:39.000000 calibrated_explanations-0.3.1a0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-23 17:39:38.975140 calibrated_explanations-0.3.1a0/setup.cfg
--rw-rw-rw-   0        0        0      226 2023-12-07 10:33:43.000000 calibrated_explanations-0.3.1a0/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-23 17:39:38.891824 calibrated_explanations-0.3.1a0/src/
-drwxrwxrwx   0        0        0        0 2024-02-23 17:39:38.926017 calibrated_explanations-0.3.1a0/src/calibrated_explanations/
--rw-rw-rw-   0        0        0     5321 2024-02-22 18:47:07.000000 calibrated_explanations-0.3.1a0/src/calibrated_explanations/VennAbers.py
--rw-rw-rw-   0        0        0      808 2024-01-17 09:22:57.000000 calibrated_explanations-0.3.1a0/src/calibrated_explanations/__init__.py
--rw-rw-rw-   0        0        0     7827 2024-01-18 08:04:34.000000 calibrated_explanations-0.3.1a0/src/calibrated_explanations/_discretizers.py
--rw-rw-rw-   0        0        0    93051 2024-02-23 16:42:28.000000 calibrated_explanations-0.3.1a0/src/calibrated_explanations/_explanations.py
--rw-rw-rw-   0        0        0    10362 2024-02-22 18:45:13.000000 calibrated_explanations-0.3.1a0/src/calibrated_explanations/_interval_regressor.py
--rw-rw-rw-   0        0        0    56762 2024-02-23 17:20:54.000000 calibrated_explanations-0.3.1a0/src/calibrated_explanations/core.py
--rw-rw-rw-   0        0        0     8105 2024-02-21 11:41:35.000000 calibrated_explanations-0.3.1a0/src/calibrated_explanations/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-23 17:39:38.968966 calibrated_explanations-0.3.1a0/src/calibrated_explanations.egg-info/
--rw-rw-rw-   0        0        0    20522 2024-02-23 17:39:38.000000 calibrated_explanations-0.3.1a0/src/calibrated_explanations.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      644 2024-02-23 17:39:38.000000 calibrated_explanations-0.3.1a0/src/calibrated_explanations.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-23 17:39:38.000000 calibrated_explanations-0.3.1a0/src/calibrated_explanations.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-02-23 17:39:38.000000 calibrated_explanations-0.3.1a0/src/calibrated_explanations.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-02-23 17:39:38.000000 calibrated_explanations-0.3.1a0/src/calibrated_explanations.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-23 17:39:38.964959 calibrated_explanations-0.3.1a0/tests/
--rw-rw-rw-   0        0        0     8311 2023-12-07 10:33:43.000000 calibrated_explanations-0.3.1a0/tests/test_classification.py
--rw-rw-rw-   0        0        0    16212 2024-02-23 17:32:40.000000 calibrated_explanations-0.3.1a0/tests/test_regression.py
+drwxrwxrwx   0        0        0        0 2024-04-14 00:06:14.966813 calibrated_explanations-0.3.2/
+-rw-rw-rw-   0        0        0     1532 2023-12-07 10:33:41.000000 calibrated_explanations-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0    20514 2024-04-14 00:06:14.963811 calibrated_explanations-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0    19636 2024-04-14 00:01:31.000000 calibrated_explanations-0.3.2/README.md
+-rw-rw-rw-   0        0        0     1023 2024-04-14 00:01:31.000000 calibrated_explanations-0.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-14 00:06:14.966813 calibrated_explanations-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      226 2023-12-07 10:33:43.000000 calibrated_explanations-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 00:06:14.894489 calibrated_explanations-0.3.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-14 00:06:14.919388 calibrated_explanations-0.3.2/src/calibrated_explanations/
+-rw-rw-rw-   0        0        0     6977 2024-04-11 08:56:51.000000 calibrated_explanations-0.3.2/src/calibrated_explanations/VennAbers.py
+-rw-rw-rw-   0        0        0      808 2024-01-17 09:22:57.000000 calibrated_explanations-0.3.2/src/calibrated_explanations/__init__.py
+-rw-rw-rw-   0        0        0     7827 2024-01-18 08:04:34.000000 calibrated_explanations-0.3.2/src/calibrated_explanations/_discretizers.py
+-rw-rw-rw-   0        0        0    93400 2024-04-11 17:11:56.000000 calibrated_explanations-0.3.2/src/calibrated_explanations/_explanations.py
+-rw-rw-rw-   0        0        0    10362 2024-02-22 18:45:13.000000 calibrated_explanations-0.3.2/src/calibrated_explanations/_interval_regressor.py
+-rw-rw-rw-   0        0        0    57289 2024-04-14 00:01:31.000000 calibrated_explanations-0.3.2/src/calibrated_explanations/core.py
+-rw-rw-rw-   0        0        0     8105 2024-02-21 11:41:35.000000 calibrated_explanations-0.3.2/src/calibrated_explanations/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-14 00:06:14.961810 calibrated_explanations-0.3.2/src/calibrated_explanations.egg-info/
+-rw-rw-rw-   0        0        0    20514 2024-04-14 00:06:14.000000 calibrated_explanations-0.3.2/src/calibrated_explanations.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2024-04-14 00:06:14.000000 calibrated_explanations-0.3.2/src/calibrated_explanations.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 00:06:14.000000 calibrated_explanations-0.3.2/src/calibrated_explanations.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-04-14 00:06:14.000000 calibrated_explanations-0.3.2/src/calibrated_explanations.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-14 00:06:14.000000 calibrated_explanations-0.3.2/src/calibrated_explanations.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 00:06:14.958387 calibrated_explanations-0.3.2/tests/
+-rw-rw-rw-   0        0        0     8311 2023-12-07 10:33:43.000000 calibrated_explanations-0.3.2/tests/test_classification.py
+-rw-rw-rw-   0        0        0    16212 2024-03-23 16:22:05.000000 calibrated_explanations-0.3.2/tests/test_regression.py
```

### Comparing `calibrated_explanations-0.3.1a0/LICENSE` & `calibrated_explanations-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.3.1a0/PKG-INFO` & `calibrated_explanations-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibrated_explanations
-Version: 0.3.1a0
+Version: 0.3.2
 Summary: Extract calibrated explanations from machine learning models.
 Author-email: Helena Löfström <helena.lofstrom@ju.se>, Tuwe Löfström <tuwe.lofstrom@ju.se>
 Project-URL: Homepage, https://github.com/Moffran/calibrated_explanations
 Project-URL: Bug Tracker, https://github.com/Moffran/calibrated_explanations/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -28,15 +28,15 @@
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/calibrated-explanations.svg)](https://anaconda.org/conda-forge/calibrated-explanations)
 [![GitHub (Pre-)Release Date](https://img.shields.io/github/release-date-pre/Moffran/calibrated_explanations)](https://github.com/Moffran/calibrated_explanations/blob/main/CHANGELOG.md)
 [![Documentation Status](https://readthedocs.org/projects/calibrated-explanations/badge/?version=latest)](https://calibrated-explanations.readthedocs.io/en/latest/?badge=latest)
 [![Build Status for Calibrated Explanations][build-status]][build-log]
 [![Lint Status for Calibrated Explanations][lint-status]][lint-log]
 [![License](https://badgen.net/github/license/moffran/calibrated_explanations)](https://github.com/moffran/calibrated_explanations/blob/main/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/calibrated-explanations)](https://pepy.tech/project/calibrated-explanations)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Moffran/calibrated_explanations/v0.3.1)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Moffran/calibrated_explanations/v0.3.2)
 
 `calibrated-explanations` is a Python package for the local feature importance explanation method called Calibrated Explanations, supporting both classification and regression.
 The proposed method is based on Venn-Abers (classification & regression) and Conformal Predictive Systems (regression) and has the following characteristics:
 * Fast, reliable, stable and robust feature importance explanations.
 * Calibration of the underlying model to ensure that predictions reflect reality.
 * Uncertainty quantification of the prediction from the underlying model and the feature importance weights. 
 * Rules with straightforward interpretation in relation to the feature weights.
@@ -219,15 +219,15 @@
 #### Additional Regression Use Cases
 Regression offers many more options and to learn more about them, see the [demo_regression](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_regression.ipynb) or the [demo_probabilistic_regression](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_probabilistic_regression.ipynb) notebooks.
 
 [Top](#calibrated-explanations-documentation)
 
 Known Limitations
 -----------------
-The implementation currently only support numerical input. Use the `utils.transform_to_numeric` (not yet in any  released version) to transform a `DataFrame` with text data into numerical form and at the same time extracting `categorical_features`, `categorical_labels`, `target_labels` (if text labels) and `mappings` (used to apply the same mappings to new data) to be used as input to the `CalibratedExplainer`. The algorithm does not currently support image data.
+The implementation currently only support numerical input. Use the `utils.transform_to_numeric` (released in version v0.3.2) to transform a `DataFrame` with text data into numerical form and at the same time extracting `categorical_features`, `categorical_labels`, `target_labels` (if text labels) and `mappings` (used to apply the same mappings to new data) to be used as input to the `CalibratedExplainer`. The algorithm does not currently support image data.
 
 [Top](#calibrated-explanations-documentation)
 
 Install
 -------
 
 `calibrated-explanations` is implemented in Python, so you need a Python environment.
@@ -320,15 +320,15 @@
 
 ```bibtex
 @software{Lofstrom_Calibrated_Explanations_2024,
 	author = 	{Löfström, Helena and Löfström, Tuwe and Johansson, Ulf and Sönströd, Cecilia and Matela, Rudy},
 	license = 	{BSD-3-Clause},
 	title = 	{Calibrated Explanations},
 	url = 		{https://github.com/Moffran/calibrated_explanations},
-	version = 	{v0.3.1},
+	version = 	{v0.3.2},
 	month = 	Feb,
 	year = 		{2024}
 }
 ```
   
 [Top](#calibrated-explanations-documentation)
```

### Comparing `calibrated_explanations-0.3.1a0/README.md` & `calibrated_explanations-0.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/calibrated-explanations.svg)](https://anaconda.org/conda-forge/calibrated-explanations)
 [![GitHub (Pre-)Release Date](https://img.shields.io/github/release-date-pre/Moffran/calibrated_explanations)](https://github.com/Moffran/calibrated_explanations/blob/main/CHANGELOG.md)
 [![Documentation Status](https://readthedocs.org/projects/calibrated-explanations/badge/?version=latest)](https://calibrated-explanations.readthedocs.io/en/latest/?badge=latest)
 [![Build Status for Calibrated Explanations][build-status]][build-log]
 [![Lint Status for Calibrated Explanations][lint-status]][lint-log]
 [![License](https://badgen.net/github/license/moffran/calibrated_explanations)](https://github.com/moffran/calibrated_explanations/blob/main/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/calibrated-explanations)](https://pepy.tech/project/calibrated-explanations)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Moffran/calibrated_explanations/v0.3.1)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Moffran/calibrated_explanations/v0.3.2)
 
 `calibrated-explanations` is a Python package for the local feature importance explanation method called Calibrated Explanations, supporting both classification and regression.
 The proposed method is based on Venn-Abers (classification & regression) and Conformal Predictive Systems (regression) and has the following characteristics:
 * Fast, reliable, stable and robust feature importance explanations.
 * Calibration of the underlying model to ensure that predictions reflect reality.
 * Uncertainty quantification of the prediction from the underlying model and the feature importance weights. 
 * Rules with straightforward interpretation in relation to the feature weights.
@@ -196,15 +196,15 @@
 #### Additional Regression Use Cases
 Regression offers many more options and to learn more about them, see the [demo_regression](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_regression.ipynb) or the [demo_probabilistic_regression](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_probabilistic_regression.ipynb) notebooks.
 
 [Top](#calibrated-explanations-documentation)
 
 Known Limitations
 -----------------
-The implementation currently only support numerical input. Use the `utils.transform_to_numeric` (not yet in any  released version) to transform a `DataFrame` with text data into numerical form and at the same time extracting `categorical_features`, `categorical_labels`, `target_labels` (if text labels) and `mappings` (used to apply the same mappings to new data) to be used as input to the `CalibratedExplainer`. The algorithm does not currently support image data.
+The implementation currently only support numerical input. Use the `utils.transform_to_numeric` (released in version v0.3.2) to transform a `DataFrame` with text data into numerical form and at the same time extracting `categorical_features`, `categorical_labels`, `target_labels` (if text labels) and `mappings` (used to apply the same mappings to new data) to be used as input to the `CalibratedExplainer`. The algorithm does not currently support image data.
 
 [Top](#calibrated-explanations-documentation)
 
 Install
 -------
 
 `calibrated-explanations` is implemented in Python, so you need a Python environment.
@@ -297,15 +297,15 @@
 
 ```bibtex
 @software{Lofstrom_Calibrated_Explanations_2024,
 	author = 	{Löfström, Helena and Löfström, Tuwe and Johansson, Ulf and Sönströd, Cecilia and Matela, Rudy},
 	license = 	{BSD-3-Clause},
 	title = 	{Calibrated Explanations},
 	url = 		{https://github.com/Moffran/calibrated_explanations},
-	version = 	{v0.3.1},
+	version = 	{v0.3.2},
 	month = 	Feb,
 	year = 		{2024}
 }
 ```
   
 [Top](#calibrated-explanations-documentation)
```

### Comparing `calibrated_explanations-0.3.1a0/pyproject.toml` & `calibrated_explanations-0.3.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "calibrated_explanations"
-version = "0.3.1a"
+version = "0.3.2"
 authors = [
   { name="Helena Löfström", email="helena.lofstrom@ju.se" },
   { name="Tuwe Löfström", email="tuwe.lofstrom@ju.se" },
 ]
 description = "Extract calibrated explanations from machine learning models."
 readme = "README.md"
 requires-python = ">=3.8"
@@ -29,9 +29,12 @@
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage"    = "https://github.com/Moffran/calibrated_explanations"
 "Bug Tracker" = "https://github.com/Moffran/calibrated_explanations/issues"
 
+[tool.pytest.ini_options]
+pythonpath = ["src"]
+
 [tool.setuptools.packages.find]
-where = ["src"]
+where = ["src"]
```

### Comparing `calibrated_explanations-0.3.1a0/src/calibrated_explanations/VennAbers.py` & `calibrated_explanations-0.3.2/src/calibrated_explanations/VennAbers.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,29 +5,49 @@
 # flake8: noqa: E501
 import numpy as np
 import venn_abers as va
 
 class VennAbers:
     """a class to calibrate the predictions of a model using the VennABERS method
     """
-    def __init__(self, cal_probs, cal_y, model, bins=None):
-        self.cprobs = cal_probs
+    def __init__(self, cprobs, cal_y, model, bins=None):
+        self.cprobs = cprobs
         self.ctargets = cal_y
         self.model = model
         self.bins = bins
-        cprobs, predict = self.get_p_value(self.cprobs)
         if self.is_mondrian():
-            self.va = []
-            for b in np.unique(self.bins):
-                va_bin = va.VennAbers()
-                va_bin.fit(cprobs[self.bins == b,:], np.multiply(predict[self.bins == b] == self.ctargets[self.bins == b], 1) if self.is_multiclass() else self.ctargets[self.bins == b], precision=4)
-                self.va.append((va_bin, b))
+            self.va = {}
+            if self.is_multiclass():
+                tmp_probs = np.zeros((cprobs.shape[0],2))
+                for c in np.unique(self.ctargets):
+                    self.va[c] = {}
+                    tmp_probs[:,0] = 1 - cprobs[:,c]
+                    tmp_probs[:,1] = cprobs[:,c]
+                    for b in np.unique(self.bins):
+                        va_class_bin = va.VennAbers()
+                        va_class_bin.fit(tmp_probs[self.bins == b,:], np.multiply(c == self.ctargets[self.bins == b], 1), precision=4)
+                        self.va[c][b] = va_class_bin
+            else:
+                for b in np.unique(self.bins):
+                    va_bin = va.VennAbers()
+                    va_bin.fit(cprobs[self.bins == b,:], self.ctargets[self.bins == b], precision=4)
+                    self.va[b] = va_bin
         else:
-            self.va = va.VennAbers()
-            self.va.fit(cprobs, np.multiply(predict == self.ctargets, 1) if self.is_multiclass() else self.ctargets, precision=4)
+            if self.is_multiclass():
+                self.va = {}
+                tmp_probs = np.zeros((cprobs.shape[0],2))
+                for c in np.unique(self.ctargets):
+                    tmp_probs[:,0] = 1 - cprobs[:,c]
+                    tmp_probs[:,1] = cprobs[:,c]
+                    va_class = va.VennAbers()
+                    va_class.fit(tmp_probs, np.multiply(c == self.ctargets, 1), precision=4)
+                    self.va[c] = va_class
+            else:
+                self.va = va.VennAbers()
+                self.va.fit(cprobs, self.ctargets, precision=4)
 
     def predict(self, test_X, bins=None):
         """a function to predict the class of the test samples
 
         Args:
             test_X (n_test_samples, n_features): test samples
             bins (array-like of shape (n_samples,), optional): Mondrian categories
@@ -40,20 +60,22 @@
         #     p0p1 = np.zeros((tprobs.shape[0],2))
         #     for va_bin, b in self.va:
         #         p0p1[bins == b,:] = va_bin.predict_proba(tprobs[bins == b,:])[1]
         # else:
         #     _, p0p1 = self.va.predict_proba(tprobs)
         # low, high = p0p1[:,0], p0p1[:,1]
         # tmp = high / (1-low + high)
+
         if self.is_multiclass():
             tmp, _ = self.predict_proba(test_X, bins=bins)
             return np.asarray(np.round(tmp[:,1]))
         tmp = self.predict_proba(test_X, bins=bins)[:,1]
         return np.asarray(np.round(tmp))
 
+    # pylint: disable=too-many-locals, too-many-branches
     def predict_proba(self, test_X, output_interval=False, classes=None, bins=None):
         """a function to predict the probabilities of the test samples, optionally outputting the VennABERS interval
 
         Args:
             testX (n_test_samples, n_features): test samples
             output_interval (bool, optional): if true, the VennAbers intervals are outputted. Defaults to False.
             classes ((n_test_samples,), optional): a list of predicted classes. Defaults to None.
@@ -62,50 +84,61 @@
         Returns:
             proba (n_test_samples,2): regularized VennABERS probabilities for the test samples. 
             if output_interval is true, the VennABERS intervals are also returned:
                 low (n_test_samples,): lower bounds of the VennABERS interval for each test sample
                 high (n_test_samples,): upper bounds of the VennABERS interval for each test sample
         """
         if 'bins' in self.model.predict_proba.__code__.co_varnames:
-            va_proba = self.model.predict_proba(test_X, bins=bins)
+            tprobs = self.model.predict_proba(test_X, bins=bins)
         else:
-            va_proba = self.model.predict_proba(test_X)
-        tprobs, classes = self.get_p_value(va_proba, classes)
+            tprobs = self.model.predict_proba(test_X)
+        p0p1 = np.zeros((tprobs.shape[0],2))
+        va_proba = np.zeros(tprobs.shape)
+
+        if self.is_multiclass():
+            low, high = np.zeros(tprobs.shape), np.zeros(tprobs.shape)
+            tmp_probs = np.zeros((tprobs.shape[0],2))
+            for c, va_class in self.va.items():
+                tmp_probs[:,0] = 1 - tprobs[:,c]
+                tmp_probs[:,1] = tprobs[:,c]
+                if self.is_mondrian():
+                    assert bins is not None, "bins must be provided if Mondrian"
+                    for b, va_class_bin in va_class.items():
+                        p0p1[bins == b,:] = va_class_bin.predict_proba(tmp_probs[bins == b,:])[1]
+                else:
+                    p0p1 = va_class.predict_proba(tmp_probs)[1]
+                low[:,c], high[:,c] = p0p1[:,0], p0p1[:,1]
+                tmp = high[:,c] / (1-low[:,c] + high[:,c])
+                va_proba[:,c] = tmp
+            if classes is not None:
+                if type(classes) not in (list, np.ndarray):
+                    classes = [classes]
+                if output_interval:
+                    return np.asarray(va_proba), [low[i,c] for i,c in enumerate(classes)], [high[i,c] for i,c in enumerate(classes)], classes
+                return np.asarray(va_proba), classes
+            classes = np.argmax(va_proba, axis=1)
+            if output_interval:
+                return np.asarray(va_proba), low, high, classes
+            return np.asarray(va_proba), classes
+
         if self.is_mondrian():
             assert bins is not None, "bins must be provided if Mondrian"
-            p0p1 = np.zeros((tprobs.shape[0],2))
-            for va_bin, b in self.va:
+            for b, va_bin in self.va.items():
                 p0p1[bins == b,:] = va_bin.predict_proba(tprobs[bins == b,:])[1]
         else:
             _, p0p1 = self.va.predict_proba(tprobs)
         low, high = p0p1[:,0], p0p1[:,1]
         tmp = high / (1-low + high)
         va_proba[:,0] = 1-tmp
         va_proba[:,1] = tmp
-        if self.is_multiclass():
-            va_proba = va_proba[:,:2]
-            if output_interval:
-                return np.asarray(va_proba), low, high, classes
-            return np.asarray(va_proba), classes
         # binary
         if output_interval:
             return np.asarray(va_proba), low, high
         return np.asarray(va_proba)
 
-    def get_p_value(self, proba, classes=None):
-        """return probability for the positive class when binary classification and for the most 
-        probable class otherwise
-        """
-        if classes is None:
-            return proba, np.argmax(proba, axis=1)
-        proba_2 = np.zeros((proba.shape[0], 2))
-        proba_2[:,1] = proba[:,classes]
-        proba_2[:,0] = 1 - proba[:,classes]
-        return proba_2, classes
-
     def is_multiclass(self) -> bool:
         """returns true if more than two classes
 
         Returns:
             bool: true if more than two classes
         """
         return len(self.cprobs[0,:]) > 2
```

### Comparing `calibrated_explanations-0.3.1a0/src/calibrated_explanations/__init__.py` & `calibrated_explanations-0.3.2/src/calibrated_explanations/__init__.py`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.3.1a0/src/calibrated_explanations/_discretizers.py` & `calibrated_explanations-0.3.2/src/calibrated_explanations/_discretizers.py`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.3.1a0/src/calibrated_explanations/_explanations.py` & `calibrated_explanations-0.3.2/src/calibrated_explanations/_explanations.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """contains the CalibratedExplanations class created by the CalibratedExplainer class
 """
 import os
 # from pyexpat import features
 import warnings
 from copy import deepcopy
 from abc import ABC, abstractmethod
+from time import time
 import numpy as np
 import matplotlib.pyplot as plt
 from ._discretizers import BinaryEntropyDiscretizer, EntropyDiscretizer, RegressorDiscretizer, BinaryRegressorDiscretizer
 from .utils import make_directory #, is_notebook, safe_import
 
 class CalibratedExplanations: # pylint: disable=too-many-instance-attributes
     """
@@ -22,14 +23,15 @@
         self.y_threshold = y_threshold
         self.low_high_percentiles = None
         self.explanations = []
         self.start_index = 0
         self.current_index = self.start_index
         self.end_index = len(test_objects[:,0])
         self.bins = bins
+        self.total_explain_time = None
 
     def __iter__(self):
         self.current_index = self.start_index
         return self
     
     def __next__(self):
         if self.current_index >= self.end_index:
@@ -85,26 +87,27 @@
     def get_high_percentile(self) -> float:
         """get the high percentile of the explanation
         """
         return self.low_high_percentiles[1] # pylint: disable=unsubscriptable-object
 
 
 
-
-    def _finalize(self, binned, feature_weights, feature_predict, prediction) -> None:
+    # pylint: disable=too-many-arguments
+    def _finalize(self, binned, feature_weights, feature_predict, prediction, instance_time=None, total_time=None) -> None:
         # """finalize the explanation by adding the binned data and the feature weights
         # """
         for i, instance in enumerate(self.test_objects):
             instance_bin = self.bins[i] if self.bins is not None else None
             if self._is_counterfactual():
                 explanation = CounterfactualExplanation(self, i, instance, binned, feature_weights, feature_predict, prediction, self.y_threshold, instance_bin=instance_bin)
             else:
                 explanation = FactualExplanation(self, i, instance, binned, feature_weights, feature_predict, prediction, self.y_threshold, instance_bin=instance_bin)
+            explanation.explain_time = instance_time[i] if instance_time is not None else None
             self.explanations.append(explanation)
-        self.calibrated_explainer._set_latest_explanation(self) # pylint: disable=protected-access
+        self.total_explain_time = time() - total_time if total_time is not None else None
         
             
 
 
 
     def _get_explainer(self):
         # """get the explainer object
@@ -388,14 +391,15 @@
 
         self.conditions = []
         self.rules = []
         self.conjunctive_rules = []
         self._has_rules = False
         self._has_conjunctive_rules = False
         self.bin = [instance_bin] if instance_bin is not None else None
+        self.explain_time = None
         
     def _get_explainer(self):
         return self.calibrated_explanations._get_explainer() # pylint: disable=protected-access
 
     def _rank_features(self, feature_weights, width=None, num_to_show=None):
         if num_to_show is None or num_to_show > len(feature_weights):
             num_to_show = len(feature_weights)
@@ -491,15 +495,15 @@
                             predicted_class, bins=None):
         # """support function to calculate the prediction for a conjunctive rule
         # """
         rule_predict, rule_low, rule_high, rule_count = 0,0,0,0
         if len(original_features) == 2:
             of1, of2 = original_features[0], original_features[1]
             rule_value1, rule_value2 = rule_value_set[0], rule_value_set[1]
-        elif len(original_features) == 3:
+        elif len(original_features) >= 3:
             of1, of2, of3 = original_features[0], original_features[1], original_features[2]
             rule_value1, rule_value2, rule_value3 = rule_value_set[0], rule_value_set[1], rule_value_set[2]  
         for value_1 in rule_value1:
             perturbed[of1] = value_1
             for value_2 in rule_value2:
                 perturbed[of2] = value_2
                 if len(original_features) >= 3:
@@ -1451,15 +1455,16 @@
                     continue
                 covered_combinations.append(np.sort(original_features))
 
                 rule_predict, rule_low, rule_high = self._predict_conjunctive(rule_values,
                                                                         original_features,
                                                                         deepcopy(x_original),
                                                                         threshold,
-                                                                        predicted_class)
+                                                                        predicted_class,
+                                                                        bins=self.bin)
                 conjunctive['predict'].append(rule_predict)
                 conjunctive['predict_low'].append(rule_low)
                 conjunctive['predict_high'].append(rule_high)
                 conjunctive['weight'].append(rule_predict - self.prediction['predict'])
                 conjunctive['weight_low'].append(rule_low - self.prediction['predict'] \
                         if rule_low != -np.inf else -np.inf)
                 conjunctive['weight_high'].append(rule_high - self.prediction['predict'] \
```

### Comparing `calibrated_explanations-0.3.1a0/src/calibrated_explanations/_interval_regressor.py` & `calibrated_explanations-0.3.2/src/calibrated_explanations/_interval_regressor.py`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.3.1a0/src/calibrated_explanations/core.py` & `calibrated_explanations-0.3.2/src/calibrated_explanations/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,28 @@
 using Venn-Abers predictors (classification) or 
 conformal predictive systems (regression).
 """
 # pylint: disable=invalid-name, line-too-long, too-many-lines
 # flake8: noqa: E501
 import copy
 import warnings
+from time import time
 import numpy as np
 
 from lime.lime_tabular import LimeTabularExplainer
 
 from ._explanations import CalibratedExplanations
 from ._discretizers import BinaryDiscretizer, BinaryEntropyDiscretizer, \
                 DecileDiscretizer, QuartileDiscretizer, EntropyDiscretizer, \
                 RegressorDiscretizer, BinaryRegressorDiscretizer
 from .VennAbers import VennAbers
 from ._interval_regressor import IntervalRegressor
 from .utils import safe_isinstance, safe_import, check_is_fitted
 
-__version__ = 'v0.3.1'
+__version__ = 'v0.3.2'
 
 
 
 class CalibratedExplainer:
     """The CalibratedExplainer class is used for explaining machine learning models with calibrated
     predictions.
 
@@ -106,14 +107,15 @@
             execution of the code. If set to False, it will not print out any additional information.
         
         Return
         ------
         CalibratedExplainer : A CalibratedExplainer object that can be used to explain predictions from a predictive model.
         
         '''
+        init_time = time()
         self.__initialized = False
         if safe_isinstance(cal_X, "pandas.core.frame.DataFrame"):
             self.cal_X = cal_X.values  # pylint: disable=invalid-name
         else:
             self.cal_X = cal_X
         if safe_isinstance(cal_y, "pandas.core.frame.DataFrame"):
             self.cal_y = cal_y.values  # pylint: disable=invalid-name
@@ -155,21 +157,25 @@
         self.__shap_enabled = False
         self.__lime_enabled = False
         self.lime = None
         self.lime_exp = None
         self.shap = None
         self.shap_exp = None
 
+        self.init_time = time() - init_time
+
 
     def __repr__(self):
         disp_str = f"CalibratedExplainer:\n\t\
                 mode={self.mode}\n\t\
                 {f'mondrian={self.bins is not None}'}\n\t\
                 discretizer={self.discretizer.__class__}\n\t\
                 model={self.model}\n\t\
+                init_time={self.init_time}\n\t\
+                {f'total_explain_time={self.latest_explanation.total_explain_time}' if self.latest_explanation is not None else 'latest_explanation is None'}\n\t\
                 {f'difficulty_estimator={self.difficulty_estimator}' if self.mode == 'regression' else ''}"
         if self.verbose:
             disp_str += f"\n\tsample_percentiles={self.sample_percentiles}\
                         \n\trandom_state={self.random_state}\
                         \n\tverbose={self.verbose}"
             if self.feature_names is not None:
                 disp_str += f"\n\tfeature_names={self.feature_names}"
@@ -231,16 +237,18 @@
         if self.mode == 'classification':
             if self._is_multiclass():
                 predict, low, high, new_classes = self.interval_model.predict_proba(test_X,
                                                                                     output_interval=True,
                                                                                     classes=classes,
                                                                                     bins=bins)
                 if classes is None:
-                    return predict[:,1], low, high, new_classes
-                return predict[:,1], low, high, None
+                    return [predict[i,c] for i,c in enumerate(new_classes)], [low[i,c] for i,c in enumerate(new_classes)], [high[i,c] for i,c in enumerate(new_classes)], new_classes
+                if type(classes) not in (list, np.ndarray):
+                    classes = [classes]
+                return [predict[i,c] for i,c in enumerate(classes)], low, high, None
 
             predict, low, high = self.interval_model.predict_proba(test_X, output_interval=True, bins=bins)
             return predict[:,1], low, high, None
         if 'regression' in self.mode:
             # pylint: disable=unexpected-keyword-arg, no-value-for-parameter
             if threshold is None: # normal regression
                 assert low_high_percentiles[0] <= low_high_percentiles[1], \
@@ -349,14 +357,16 @@
                 bins = None,
                 ) -> CalibratedExplanations:
         """
         Calling self as a function creates a CalibratedExplanations object for the test data with the 
         already assigned discretizer. Called by the `explain_factual` and `explain_counterfactual` methods. 
         See their documentation for further information.
         """
+        total_time = time()
+        instance_time = []
         if safe_isinstance(testX, "pandas.core.frame.DataFrame"):
             testX = testX.values  # pylint: disable=invalid-name
         if len(testX.shape) == 1:
             testX = testX.reshape(1, -1)
         if testX.shape[1] != self.cal_X.shape[1]:
             raise ValueError("The number of features in the test data must be the same as in the \
                             calibration data.")
@@ -381,14 +391,16 @@
 
         feature_weights =  {'predict': [],'low': [],'high': [],}
         feature_predict =  {'predict': [],'low': [],'high': [],}
         prediction =  {'predict': [],'low': [],'high': [], 'classes': []}
         binned_predict =  {'predict': [],'low': [],'high': [],'current_bin': [],'rule_values': [], 'counts': [], 'fractions': []}
 
         for i, x in enumerate(testX):
+            instance_time.append(time())
+
             bin_x = [bins[i]] if bins is not None else None
 
             if threshold is not None and not np.isscalar(explanation.y_threshold):
                 threshold = float(explanation.y_threshold[i])
             predict, low, high, predicted_class = self._predict(x.reshape(1,-1), threshold=threshold, low_high_percentiles=low_high_percentiles, bins=bin_x)
             prediction['predict'].append(predict[0])
             prediction['low'].append(low[0])
@@ -530,16 +542,18 @@
             feature_weights['predict'].append(instance_weights['predict'])
             feature_weights['low'].append(instance_weights['low'])
             feature_weights['high'].append(instance_weights['high'])
 
             feature_predict['predict'].append(instance_predict['predict'])
             feature_predict['low'].append(instance_predict['low'])
             feature_predict['high'].append(instance_predict['high'])
+            instance_time[-1] = time() - instance_time[-1]
 
-        explanation._finalize(binned_predict, feature_weights, feature_predict, prediction)
+        explanation._finalize(binned_predict, feature_weights, feature_predict, prediction, instance_time=instance_time, total_time=total_time)
+        self.latest_explanation = explanation
         return explanation
 
 
 
     def _assign_weight(self, instance_predict, prediction, is_probabilistic):
         if is_probabilistic:
             return prediction - instance_predict # probabilistic regression
@@ -795,25 +809,14 @@
             values, frequencies = map(list, zip(*(sorted(feature_count.items()))))
 
             self.feature_values[feature] = values
             self.feature_frequencies[feature] = (np.array(frequencies) /
                                                  float(sum(frequencies)))
 
 
-
-    def _set_latest_explanation(self, explanation) -> None:
-        # """assigns the latest explanation to the explainer
-
-        # Args:
-        #     explanation (CalibratedExplanations): the latest created explanation
-        # """
-        self.latest_explanation = explanation
-
-
-
     def _is_mondrian(self):
         # """returns whether the explainer is a Mondrian explainer
 
         # Returns:
         #     bool: True if Mondrian
         # """
         return self.bins is not None
```

### Comparing `calibrated_explanations-0.3.1a0/src/calibrated_explanations/utils.py` & `calibrated_explanations-0.3.2/src/calibrated_explanations/utils.py`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.3.1a0/src/calibrated_explanations.egg-info/PKG-INFO` & `calibrated_explanations-0.3.2/src/calibrated_explanations.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calibrated_explanations
-Version: 0.3.1a0
+Version: 0.3.2
 Summary: Extract calibrated explanations from machine learning models.
 Author-email: Helena Löfström <helena.lofstrom@ju.se>, Tuwe Löfström <tuwe.lofstrom@ju.se>
 Project-URL: Homepage, https://github.com/Moffran/calibrated_explanations
 Project-URL: Bug Tracker, https://github.com/Moffran/calibrated_explanations/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -28,15 +28,15 @@
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/calibrated-explanations.svg)](https://anaconda.org/conda-forge/calibrated-explanations)
 [![GitHub (Pre-)Release Date](https://img.shields.io/github/release-date-pre/Moffran/calibrated_explanations)](https://github.com/Moffran/calibrated_explanations/blob/main/CHANGELOG.md)
 [![Documentation Status](https://readthedocs.org/projects/calibrated-explanations/badge/?version=latest)](https://calibrated-explanations.readthedocs.io/en/latest/?badge=latest)
 [![Build Status for Calibrated Explanations][build-status]][build-log]
 [![Lint Status for Calibrated Explanations][lint-status]][lint-log]
 [![License](https://badgen.net/github/license/moffran/calibrated_explanations)](https://github.com/moffran/calibrated_explanations/blob/main/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/calibrated-explanations)](https://pepy.tech/project/calibrated-explanations)
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Moffran/calibrated_explanations/v0.3.1)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Moffran/calibrated_explanations/v0.3.2)
 
 `calibrated-explanations` is a Python package for the local feature importance explanation method called Calibrated Explanations, supporting both classification and regression.
 The proposed method is based on Venn-Abers (classification & regression) and Conformal Predictive Systems (regression) and has the following characteristics:
 * Fast, reliable, stable and robust feature importance explanations.
 * Calibration of the underlying model to ensure that predictions reflect reality.
 * Uncertainty quantification of the prediction from the underlying model and the feature importance weights. 
 * Rules with straightforward interpretation in relation to the feature weights.
@@ -219,15 +219,15 @@
 #### Additional Regression Use Cases
 Regression offers many more options and to learn more about them, see the [demo_regression](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_regression.ipynb) or the [demo_probabilistic_regression](https://github.com/Moffran/calibrated_explanations/blob/main/notebooks/demo_probabilistic_regression.ipynb) notebooks.
 
 [Top](#calibrated-explanations-documentation)
 
 Known Limitations
 -----------------
-The implementation currently only support numerical input. Use the `utils.transform_to_numeric` (not yet in any  released version) to transform a `DataFrame` with text data into numerical form and at the same time extracting `categorical_features`, `categorical_labels`, `target_labels` (if text labels) and `mappings` (used to apply the same mappings to new data) to be used as input to the `CalibratedExplainer`. The algorithm does not currently support image data.
+The implementation currently only support numerical input. Use the `utils.transform_to_numeric` (released in version v0.3.2) to transform a `DataFrame` with text data into numerical form and at the same time extracting `categorical_features`, `categorical_labels`, `target_labels` (if text labels) and `mappings` (used to apply the same mappings to new data) to be used as input to the `CalibratedExplainer`. The algorithm does not currently support image data.
 
 [Top](#calibrated-explanations-documentation)
 
 Install
 -------
 
 `calibrated-explanations` is implemented in Python, so you need a Python environment.
@@ -320,15 +320,15 @@
 
 ```bibtex
 @software{Lofstrom_Calibrated_Explanations_2024,
 	author = 	{Löfström, Helena and Löfström, Tuwe and Johansson, Ulf and Sönströd, Cecilia and Matela, Rudy},
 	license = 	{BSD-3-Clause},
 	title = 	{Calibrated Explanations},
 	url = 		{https://github.com/Moffran/calibrated_explanations},
-	version = 	{v0.3.1},
+	version = 	{v0.3.2},
 	month = 	Feb,
 	year = 		{2024}
 }
 ```
   
 [Top](#calibrated-explanations-documentation)
```

### Comparing `calibrated_explanations-0.3.1a0/src/calibrated_explanations.egg-info/SOURCES.txt` & `calibrated_explanations-0.3.2/src/calibrated_explanations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.3.1a0/tests/test_classification.py` & `calibrated_explanations-0.3.2/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `calibrated_explanations-0.3.1a0/tests/test_regression.py` & `calibrated_explanations-0.3.2/tests/test_regression.py`

 * *Files identical despite different names*

