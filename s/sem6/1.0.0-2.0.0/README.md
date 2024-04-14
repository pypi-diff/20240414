# Comparing `tmp/sem6-1.0.0.tar.gz` & `tmp/sem6-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sem6-1.0.0.tar", last modified: Sat Apr 13 13:10:03 2024, max compression
+gzip compressed data, was "sem6-2.0.0.tar", last modified: Sun Apr 14 15:07:10 2024, max compression
```

## Comparing `sem6-1.0.0.tar` & `sem6-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 13:10:03.334805 sem6-1.0.0/
--rw-rw-rw-   0        0        0       51 2024-04-13 13:10:03.334805 sem6-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-13 13:10:03.319250 sem6-1.0.0/sem6/
--rw-rw-rw-   0        0        0        0 2024-04-13 12:06:54.000000 sem6-1.0.0/sem6/__init__.py
--rw-rw-rw-   0        0        0     1712 2024-04-13 12:00:16.000000 sem6-1.0.0/sem6/adaboost.py
--rw-rw-rw-   0        0        0     5768 2024-04-13 12:00:38.000000 sem6-1.0.0/sem6/clustering.py
--rw-rw-rw-   0        0        0     3096 2024-04-13 12:04:00.000000 sem6-1.0.0/sem6/ensemble_classification.py
--rw-rw-rw-   0        0        0     2193 2024-04-13 12:00:57.000000 sem6-1.0.0/sem6/ensemble_regression.py
-drwxrwxrwx   0        0        0        0 2024-04-13 13:10:03.334805 sem6-1.0.0/sem6.egg-info/
--rw-rw-rw-   0        0        0       51 2024-04-13 13:10:03.000000 sem6-1.0.0/sem6.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2024-04-13 13:10:03.000000 sem6-1.0.0/sem6.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 13:10:03.000000 sem6-1.0.0/sem6.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-04-13 13:10:03.000000 sem6-1.0.0/sem6.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-13 13:10:03.000000 sem6-1.0.0/sem6.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-13 13:10:03.334805 sem6-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      235 2024-04-13 13:09:31.000000 sem6-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:07:10.219230 sem6-2.0.0/
+-rw-rw-rw-   0        0        0       51 2024-04-14 15:07:10.219230 sem6-2.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-14 15:07:10.158338 sem6-2.0.0/sem6/
+-rw-rw-rw-   0        0        0        0 2024-04-13 12:06:54.000000 sem6-2.0.0/sem6/__init__.py
+-rw-rw-rw-   0        0        0     1712 2024-04-13 12:00:16.000000 sem6-2.0.0/sem6/adaboost.py
+-rw-rw-rw-   0        0        0     5770 2024-04-13 13:17:40.000000 sem6-2.0.0/sem6/clustering.py
+-rw-rw-rw-   0        0        0     3604 2024-04-14 14:55:04.000000 sem6-2.0.0/sem6/decisiontree.py
+-rw-rw-rw-   0        0        0     3100 2024-04-14 15:02:18.000000 sem6-2.0.0/sem6/ensemble_classification.py
+-rw-rw-rw-   0        0        0     2193 2024-04-13 12:00:57.000000 sem6-2.0.0/sem6/ensemble_regression.py
+-rw-rw-rw-   0        0        0     3263 2024-04-14 14:55:06.000000 sem6-2.0.0/sem6/gradientboosting.py
+-rw-rw-rw-   0        0        0     3418 2024-04-14 14:55:07.000000 sem6-2.0.0/sem6/lightgbm.py
+-rw-rw-rw-   0        0        0     3314 2024-04-14 14:55:09.000000 sem6-2.0.0/sem6/linearreg.py
+-rw-rw-rw-   0        0        0     3315 2024-04-14 14:55:10.000000 sem6-2.0.0/sem6/logisticreg.py
+-rw-rw-rw-   0        0        0     3666 2024-04-14 14:55:12.000000 sem6-2.0.0/sem6/randomforest.py
+-rw-rw-rw-   0        0        0     4379 2024-04-14 14:55:14.000000 sem6-2.0.0/sem6/svm.py
+-rw-rw-rw-   0        0        0     3441 2024-04-14 15:03:40.000000 sem6-2.0.0/sem6/xgb.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:07:10.213037 sem6-2.0.0/sem6.egg-info/
+-rw-rw-rw-   0        0        0       51 2024-04-14 15:07:09.000000 sem6-2.0.0/sem6.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2024-04-14 15:07:09.000000 sem6-2.0.0/sem6.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 15:07:09.000000 sem6-2.0.0/sem6.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-04-14 15:07:09.000000 sem6-2.0.0/sem6.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-14 15:07:09.000000 sem6-2.0.0/sem6.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 15:07:10.219230 sem6-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      235 2024-04-14 14:59:21.000000 sem6-2.0.0/setup.py
```

### Comparing `sem6-1.0.0/sem6/adaboost.py` & `sem6-2.0.0/sem6/adaboost.py`

 * *Files identical despite different names*

### Comparing `sem6-1.0.0/sem6/clustering.py` & `sem6-2.0.0/sem6/clustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     plt.show()
     """
     print(code)
 
 
 
 
-def hierarical():
+def hierarchical():
     code = """
 
     import matplotlib.pyplot as plt
     import pandas as pd
     import numpy as np
     import scipy.cluster.hierarchy as shc
     from sklearn.cluster import AgglomerativeClustering
```

### Comparing `sem6-1.0.0/sem6/ensemble_classification.py` & `sem6-2.0.0/sem6/ensemble_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-def ensemble_classifier():
+def ensemble_classification():
     code = """
 
     import numpy as np
     import pandas as pd
     import os
     from sklearn.preprocessing import LabelEncoder
     import seaborn as sns
```

### Comparing `sem6-1.0.0/sem6/ensemble_regression.py` & `sem6-2.0.0/sem6/ensemble_regression.py`

 * *Files identical despite different names*

