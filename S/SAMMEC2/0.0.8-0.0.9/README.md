# Comparing `tmp/SAMMEC2-0.0.8.tar.gz` & `tmp/SAMMEC2-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SAMMEC2-0.0.8.tar", last modified: Sat Apr 13 23:56:30 2024, max compression
+gzip compressed data, was "SAMMEC2-0.0.9.tar", last modified: Sun Apr 14 00:01:58 2024, max compression
```

## Comparing `SAMMEC2-0.0.8.tar` & `SAMMEC2-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-13 23:56:30.847172 SAMMEC2-0.0.8/
--rw-r--r--   0 bso2     (1724916894) 285334988      380 2024-04-13 23:56:30.846731 SAMMEC2-0.0.8/PKG-INFO
--rw-r--r--   0 bso2     (1724916894) 285334988        7 2024-04-11 13:08:29.000000 SAMMEC2-0.0.8/README
-drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-13 23:56:30.844528 SAMMEC2-0.0.8/SAMMEC2/
--rw-r--r--   0 bso2     (1724916894) 285334988     6001 2024-04-13 14:51:00.000000 SAMMEC2-0.0.8/SAMMEC2/GA.py
--rw-r--r--   0 bso2     (1724916894) 285334988     3491 2024-04-11 14:27:13.000000 SAMMEC2-0.0.8/SAMMEC2/SAMMEC2.py
--rw-r--r--   0 bso2     (1724916894) 285334988       71 2024-04-13 14:50:23.000000 SAMMEC2-0.0.8/SAMMEC2/__init__.py
-drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-13 23:56:30.846315 SAMMEC2-0.0.8/SAMMEC2.egg-info/
--rw-r--r--   0 bso2     (1724916894) 285334988      380 2024-04-13 23:56:30.000000 SAMMEC2-0.0.8/SAMMEC2.egg-info/PKG-INFO
--rw-r--r--   0 bso2     (1724916894) 285334988      192 2024-04-13 23:56:30.000000 SAMMEC2-0.0.8/SAMMEC2.egg-info/SOURCES.txt
--rw-r--r--   0 bso2     (1724916894) 285334988        1 2024-04-13 23:56:30.000000 SAMMEC2-0.0.8/SAMMEC2.egg-info/dependency_links.txt
--rw-r--r--   0 bso2     (1724916894) 285334988        8 2024-04-13 23:56:30.000000 SAMMEC2-0.0.8/SAMMEC2.egg-info/top_level.txt
--rw-r--r--   0 bso2     (1724916894) 285334988       38 2024-04-13 23:56:30.847254 SAMMEC2-0.0.8/setup.cfg
--rw-r--r--   0 bso2     (1724916894) 285334988      648 2024-04-13 23:56:09.000000 SAMMEC2-0.0.8/setup.py
+drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-14 00:01:58.730751 SAMMEC2-0.0.9/
+-rw-r--r--   0 bso2     (1724916894) 285334988      380 2024-04-14 00:01:58.730344 SAMMEC2-0.0.9/PKG-INFO
+-rw-r--r--   0 bso2     (1724916894) 285334988        7 2024-04-11 13:08:29.000000 SAMMEC2-0.0.9/README
+drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-14 00:01:58.728613 SAMMEC2-0.0.9/SAMMEC2/
+-rw-r--r--   0 bso2     (1724916894) 285334988     5472 2024-04-14 00:00:57.000000 SAMMEC2-0.0.9/SAMMEC2/GA.py
+-rw-r--r--   0 bso2     (1724916894) 285334988     3491 2024-04-11 14:27:13.000000 SAMMEC2-0.0.9/SAMMEC2/SAMMEC2.py
+-rw-r--r--   0 bso2     (1724916894) 285334988       71 2024-04-13 14:50:23.000000 SAMMEC2-0.0.9/SAMMEC2/__init__.py
+drwxr-xr-x   0 bso2     (1724916894) 285334988        0 2024-04-14 00:01:58.729985 SAMMEC2-0.0.9/SAMMEC2.egg-info/
+-rw-r--r--   0 bso2     (1724916894) 285334988      380 2024-04-14 00:01:58.000000 SAMMEC2-0.0.9/SAMMEC2.egg-info/PKG-INFO
+-rw-r--r--   0 bso2     (1724916894) 285334988      192 2024-04-14 00:01:58.000000 SAMMEC2-0.0.9/SAMMEC2.egg-info/SOURCES.txt
+-rw-r--r--   0 bso2     (1724916894) 285334988        1 2024-04-14 00:01:58.000000 SAMMEC2-0.0.9/SAMMEC2.egg-info/dependency_links.txt
+-rw-r--r--   0 bso2     (1724916894) 285334988        8 2024-04-14 00:01:58.000000 SAMMEC2-0.0.9/SAMMEC2.egg-info/top_level.txt
+-rw-r--r--   0 bso2     (1724916894) 285334988       38 2024-04-14 00:01:58.730828 SAMMEC2-0.0.9/setup.cfg
+-rw-r--r--   0 bso2     (1724916894) 285334988      648 2024-04-14 00:01:46.000000 SAMMEC2-0.0.9/setup.py
```

### Comparing `SAMMEC2-0.0.8/SAMMEC2/GA.py` & `SAMMEC2-0.0.9/SAMMEC2/GA.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,16 +136,7 @@
             population = self.make_next_generation(function)
 
         best_individual = self.sort_population_by_fitness(function)[-1][0]
         print("\n🔬 FINAL RESULT")
         print(best_individual, self.apply_function(Xtrain, Xtest, ytrain, ytest, best_individual))
 
 
-from sklearn.datasets import make_classification
-from sklearn.model_selection import train_test_split
-
-X,y = make_classification(n_samples=10000, n_features=50, n_informative=50, n_redundant=0, n_repeated=0, n_classes=3,
-                          n_clusters_per_class=2,class_sep=2,flip_y=0,weights=[0.96,0.035,0.005], random_state=16)
-
-X_train,X_test,y_train,y_test=train_test_split(X,y,random_state=1)
-
-GA_SAMMEC2(n_class=3, err=0.01, size=1, generations=2, n_estimators=200, random_state=50).fit(X_train,y_train,X_test,y_test)
```

### Comparing `SAMMEC2-0.0.8/SAMMEC2/SAMMEC2.py` & `SAMMEC2-0.0.9/SAMMEC2/SAMMEC2.py`

 * *Files identical despite different names*

### Comparing `SAMMEC2-0.0.8/setup.py` & `SAMMEC2-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SAMMEC2", # Replace with your own PyPI username(id)
-    version="0.0.8",
+    version="0.0.9",
     author="Banghee So",
     author_email="bso@towson.edu",
     description="SAMMEC2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bheeso/SAMME.C2",
     packages=setuptools.find_packages(),
```

