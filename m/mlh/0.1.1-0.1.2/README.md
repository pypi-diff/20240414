# Comparing `tmp/mlh-0.1.1.tar.gz` & `tmp/mlh-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlh-0.1.1.tar", last modified: Mon Jan  8 18:28:17 2024, max compression
+gzip compressed data, was "mlh-0.1.2.tar", last modified: Sun Apr 14 15:27:55 2024, max compression
```

## Comparing `mlh-0.1.1.tar` & `mlh-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-01-08 18:28:17.845015 mlh-0.1.1/
--rw-rw-rw-   0        0        0     3157 2024-01-08 18:28:17.842945 mlh-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2582 2023-08-02 05:28:22.000000 mlh-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-01-08 18:28:17.815458 mlh-0.1.1/mlh/
--rw-rw-rw-   0        0        0      269 2023-08-02 06:21:43.000000 mlh-0.1.1/mlh/__init__.py
--rw-rw-rw-   0        0        0     6954 2023-08-04 04:57:16.000000 mlh-0.1.1/mlh/common_utils.py
--rw-rw-rw-   0        0        0     7958 2024-01-08 17:56:03.000000 mlh-0.1.1/mlh/data_from_parquet.py
--rw-rw-rw-   0        0        0     5936 2023-08-02 05:28:22.000000 mlh-0.1.1/mlh/s3_connect.py
--rw-rw-rw-   0        0        0    13968 2023-09-01 10:16:16.000000 mlh-0.1.1/mlh/snowflake_connect.py
--rw-rw-rw-   0        0        0     9675 2023-08-02 06:44:38.000000 mlh-0.1.1/mlh/sqlite_functions.py
--rw-rw-rw-   0        0        0    15538 2023-09-01 10:03:58.000000 mlh-0.1.1/mlh/support.py
--rw-rw-rw-   0        0        0    21100 2023-08-02 07:02:13.000000 mlh-0.1.1/mlh/woe.py
-drwxrwxrwx   0        0        0        0 2024-01-08 18:28:17.840762 mlh-0.1.1/mlh.egg-info/
--rw-rw-rw-   0        0        0     3157 2024-01-08 18:28:17.000000 mlh-0.1.1/mlh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2024-01-08 18:28:17.000000 mlh-0.1.1/mlh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-08 18:28:17.000000 mlh-0.1.1/mlh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2024-01-08 18:28:17.000000 mlh-0.1.1/mlh.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-01-08 18:28:17.000000 mlh-0.1.1/mlh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-08 18:28:17.845015 mlh-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      845 2024-01-08 17:48:07.000000 mlh-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:27:55.144111 mlh-0.1.2/
+-rw-rw-rw-   0        0        0     3157 2024-04-14 15:27:55.144111 mlh-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2582 2023-08-02 05:28:22.000000 mlh-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 15:27:55.064735 mlh-0.1.2/mlh/
+-rw-rw-rw-   0        0        0      269 2023-08-02 06:21:43.000000 mlh-0.1.2/mlh/__init__.py
+-rw-rw-rw-   0        0        0     6954 2023-08-04 04:57:16.000000 mlh-0.1.2/mlh/common_utils.py
+-rw-rw-rw-   0        0        0     7958 2024-01-08 17:56:03.000000 mlh-0.1.2/mlh/data_from_parquet.py
+-rw-rw-rw-   0        0        0     5936 2023-08-02 05:28:22.000000 mlh-0.1.2/mlh/s3_connect.py
+-rw-rw-rw-   0        0        0    13968 2023-09-01 10:16:16.000000 mlh-0.1.2/mlh/snowflake_connect.py
+-rw-rw-rw-   0        0        0     9675 2023-08-02 06:44:38.000000 mlh-0.1.2/mlh/sqlite_functions.py
+-rw-rw-rw-   0        0        0    15539 2024-04-14 15:25:07.000000 mlh-0.1.2/mlh/support.py
+-rw-rw-rw-   0        0        0    21100 2023-08-02 07:02:13.000000 mlh-0.1.2/mlh/woe.py
+drwxrwxrwx   0        0        0        0 2024-04-14 15:27:55.128068 mlh-0.1.2/mlh.egg-info/
+-rw-rw-rw-   0        0        0     3157 2024-04-14 15:27:54.000000 mlh-0.1.2/mlh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-04-14 15:27:54.000000 mlh-0.1.2/mlh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 15:27:54.000000 mlh-0.1.2/mlh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2024-04-14 15:27:54.000000 mlh-0.1.2/mlh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-14 15:27:54.000000 mlh-0.1.2/mlh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 15:27:55.144111 mlh-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      835 2024-04-14 15:26:06.000000 mlh-0.1.2/setup.py
```

### Comparing `mlh-0.1.1/PKG-INFO` & `mlh-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlh
-Version: 0.1.1
+Version: 0.1.2
 Summary: This package provides helper utilities for machine learning tasks. One major utility is calculation of weight of evidence
 Home-page: https://github.com/devsahu99/mlh
 Author: Devendra Kumar Sahu
 Author-email: devsahu99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mlh-0.1.1/README.md` & `mlh-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mlh-0.1.1/mlh/common_utils.py` & `mlh-0.1.2/mlh/common_utils.py`

 * *Files identical despite different names*

### Comparing `mlh-0.1.1/mlh/data_from_parquet.py` & `mlh-0.1.2/mlh/data_from_parquet.py`

 * *Files identical despite different names*

### Comparing `mlh-0.1.1/mlh/s3_connect.py` & `mlh-0.1.2/mlh/s3_connect.py`

 * *Files identical despite different names*

### Comparing `mlh-0.1.1/mlh/snowflake_connect.py` & `mlh-0.1.2/mlh/snowflake_connect.py`

 * *Files identical despite different names*

### Comparing `mlh-0.1.1/mlh/sqlite_functions.py` & `mlh-0.1.2/mlh/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `mlh-0.1.1/mlh/support.py` & `mlh-0.1.2/mlh/support.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas as pd
 import pandas.core.algorithms as algos
 import scipy.stats.stats as stats
 import re
 from pandas import Series
 import numpy as np
 import random
-from IPython.display import display, HTML, Markdown
+#from IPython.display import display, HTML, Markdown
 import matplotlib.pyplot as plt
 from sklearn.model_selection import GridSearchCV, StratifiedKFold, RandomizedSearchCV, train_test_split
 from sklearn.metrics import accuracy_score,classification_report,confusion_matrix,roc_curve,auc,precision_recall_curve,make_scorer,recall_score,precision_score
 
 class support:
     #!/usr/bin/env python
     # -*- coding: utf-8 -*-
```

### Comparing `mlh-0.1.1/mlh/woe.py` & `mlh-0.1.2/mlh/woe.py`

 * *Files identical despite different names*

### Comparing `mlh-0.1.1/mlh.egg-info/PKG-INFO` & `mlh-0.1.2/mlh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlh
-Version: 0.1.1
+Version: 0.1.2
 Summary: This package provides helper utilities for machine learning tasks. One major utility is calculation of weight of evidence
 Home-page: https://github.com/devsahu99/mlh
 Author: Devendra Kumar Sahu
 Author-email: devsahu99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mlh-0.1.1/setup.py` & `mlh-0.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mlh",
-    version = '0.1.1',
+    version = '0.1.2',
     author="Devendra Kumar Sahu",
     author_email="devsahu99@gmail.com",
     description="This package provides helper utilities for machine learning tasks. One major utility is calculation of weight of evidence",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/devsahu99/mlh",
     packages=['mlh'],
     install_requires=[
-        'pandas','scipy','IPython','matplotlib', 'snowflake-connector-python[pandas]', 's3fs', 'boto3', 'openpyxl', 'xlsxwriter'
+        'pandas','scipy','matplotlib', 'snowflake-connector-python[pandas]', 's3fs', 'boto3', 'openpyxl', 'xlsxwriter'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

