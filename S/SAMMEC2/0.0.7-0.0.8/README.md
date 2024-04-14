# Comparing `tmp/SAMMEC2-0.0.7.tar.gz` & `tmp/SAMMEC2-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAMMEC2-0.0.7.tar", last modified: Sat Apr 13 14:22:50 2024, max compression
+gzip compressed data, was "SAMMEC2-0.0.8.tar", last modified: Sat Apr 13 23:56:30 2024, max compression
```

## Comparing `SAMMEC2-0.0.7.tar` & `SAMMEC2-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-13 14:22:50.681892 SAMMEC2-0.0.7/
--rw-r--r--   0 bso2     (1724916894) 285334988      380 2024-04-13 14:22:50.681258 SAMMEC2-0.0.7/PKG-INFO
--rw-r--r--   0 bso2     (1724916894) 285334988        7 2024-04-11 13:08:29.000000 SAMMEC2-0.0.7/README
-drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-13 14:22:50.677786 SAMMEC2-0.0.7/SAMMEC2/
--rw-r--r--   0 bso2     (1724916894) 285334988     5980 2024-04-13 14:20:59.000000 SAMMEC2-0.0.7/SAMMEC2/GA.py
--rw-r--r--   0 bso2     (1724916894) 285334988     3491 2024-04-11 14:27:13.000000 SAMMEC2-0.0.7/SAMMEC2/SAMMEC2.py
--rw-r--r--   0 bso2     (1724916894) 285334988       40 2024-04-12 10:44:38.000000 SAMMEC2-0.0.7/SAMMEC2/__init__.py
-drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-13 14:22:50.680655 SAMMEC2-0.0.7/SAMMEC2.egg-info/
--rw-r--r--   0 bso2     (1724916894) 285334988      380 2024-04-13 14:22:50.000000 SAMMEC2-0.0.7/SAMMEC2.egg-info/PKG-INFO
--rw-r--r--   0 bso2     (1724916894) 285334988      192 2024-04-13 14:22:50.000000 SAMMEC2-0.0.7/SAMMEC2.egg-info/SOURCES.txt
--rw-r--r--   0 bso2     (1724916894) 285334988        1 2024-04-13 14:22:50.000000 SAMMEC2-0.0.7/SAMMEC2.egg-info/dependency_links.txt
--rw-r--r--   0 bso2     (1724916894) 285334988        8 2024-04-13 14:22:50.000000 SAMMEC2-0.0.7/SAMMEC2.egg-info/top_level.txt
--rw-r--r--   0 bso2     (1724916894) 285334988       38 2024-04-13 14:22:50.682024 SAMMEC2-0.0.7/setup.cfg
--rw-r--r--   0 bso2     (1724916894) 285334988      648 2024-04-13 14:16:54.000000 SAMMEC2-0.0.7/setup.py
+drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-13 23:56:30.847172 SAMMEC2-0.0.8/
+-rw-r--r--   0 bso2     (1724916894) 285334988      380 2024-04-13 23:56:30.846731 SAMMEC2-0.0.8/PKG-INFO
+-rw-r--r--   0 bso2     (1724916894) 285334988        7 2024-04-11 13:08:29.000000 SAMMEC2-0.0.8/README
+drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-13 23:56:30.844528 SAMMEC2-0.0.8/SAMMEC2/
+-rw-r--r--   0 bso2     (1724916894) 285334988     6001 2024-04-13 14:51:00.000000 SAMMEC2-0.0.8/SAMMEC2/GA.py
+-rw-r--r--   0 bso2     (1724916894) 285334988     3491 2024-04-11 14:27:13.000000 SAMMEC2-0.0.8/SAMMEC2/SAMMEC2.py
+-rw-r--r--   0 bso2     (1724916894) 285334988       71 2024-04-13 14:50:23.000000 SAMMEC2-0.0.8/SAMMEC2/__init__.py
+drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-13 23:56:30.846315 SAMMEC2-0.0.8/SAMMEC2.egg-info/
+-rw-r--r--   0 bso2     (1724916894) 285334988      380 2024-04-13 23:56:30.000000 SAMMEC2-0.0.8/SAMMEC2.egg-info/PKG-INFO
+-rw-r--r--   0 bso2     (1724916894) 285334988      192 2024-04-13 23:56:30.000000 SAMMEC2-0.0.8/SAMMEC2.egg-info/SOURCES.txt
+-rw-r--r--   0 bso2     (1724916894) 285334988        1 2024-04-13 23:56:30.000000 SAMMEC2-0.0.8/SAMMEC2.egg-info/dependency_links.txt
+-rw-r--r--   0 bso2     (1724916894) 285334988        8 2024-04-13 23:56:30.000000 SAMMEC2-0.0.8/SAMMEC2.egg-info/top_level.txt
+-rw-r--r--   0 bso2     (1724916894) 285334988       38 2024-04-13 23:56:30.847254 SAMMEC2-0.0.8/setup.cfg
+-rw-r--r--   0 bso2     (1724916894) 285334988      648 2024-04-13 23:56:09.000000 SAMMEC2-0.0.8/setup.py
```

### Comparing `SAMMEC2-0.0.7/SAMMEC2/GA.py` & `SAMMEC2-0.0.8/SAMMEC2/GA.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from imblearn.metrics import geometric_mean_score
 from sklearn.metrics import accuracy_score, matthews_corrcoef
-import SAMMEC2
+from SAMMEC2 import AdaBoostClassifier_C2V2
 import operator
 
 class GA_SAMMEC2():
     def __init__(self, cost=None, n_class=3, lim=0.9, err=0.005, size=10, generations=5, n_estimators=200,
                  random_state=None):
         self.n_class = n_class
         self.size = size
@@ -42,15 +42,15 @@
                     c = vvv
                 v.reverse()
                 population.append(v)
         return population
 
     def apply_function(self, Xtrain, Xtest, ytrain, ytest, individual):
 
-        SAMME_C2 = SAMMEC2.AdaBoostClassifier_C2V2(n_estimators=self.n_estimators,
+        SAMME_C2 = AdaBoostClassifier_C2V2(n_estimators=self.n_estimators,
                                                    random_state=self.random_state, cost=individual)
         SAMME_C2.fit = SAMME_C2.fit(Xtrain, ytrain)
         y_pred_SAMMEC2 = SAMME_C2.fit.predict(Xtest)
         return geometric_mean_score(ytest, y_pred_SAMMEC2, correction=0.0001), accuracy_score(ytest, y_pred_SAMMEC2)
         # return matthews_corrcoef(ytest, y_pred_SAMMEC2), accuracy_score(ytest, y_pred_SAMMEC2)
 
     # sorted_population, fitness_sum
```

### Comparing `SAMMEC2-0.0.7/SAMMEC2/SAMMEC2.py` & `SAMMEC2-0.0.8/SAMMEC2/SAMMEC2.py`

 * *Files identical despite different names*

### Comparing `SAMMEC2-0.0.7/setup.py` & `SAMMEC2-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SAMMEC2", # Replace with your own PyPI username(id)
-    version="0.0.7",
+    version="0.0.8",
     author="Banghee So",
     author_email="bso@towson.edu",
     description="SAMMEC2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bheeso/SAMME.C2",
     packages=setuptools.find_packages(),
```

