# Comparing `tmp/mlh-0.1.2.tar.gz` & `tmp/mlh-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlh-0.1.2.tar", last modified: Sun Apr 14 15:27:55 2024, max compression
+gzip compressed data, was "mlh-0.1.3.tar", last modified: Sun Apr 14 16:29:10 2024, max compression
```

## Comparing `mlh-0.1.2.tar` & `mlh-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 15:27:55.144111 mlh-0.1.2/
--rw-rw-rw-   0        0        0     3157 2024-04-14 15:27:55.144111 mlh-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2582 2023-08-02 05:28:22.000000 mlh-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 15:27:55.064735 mlh-0.1.2/mlh/
--rw-rw-rw-   0        0        0      269 2023-08-02 06:21:43.000000 mlh-0.1.2/mlh/__init__.py
--rw-rw-rw-   0        0        0     6954 2023-08-04 04:57:16.000000 mlh-0.1.2/mlh/common_utils.py
--rw-rw-rw-   0        0        0     7958 2024-01-08 17:56:03.000000 mlh-0.1.2/mlh/data_from_parquet.py
--rw-rw-rw-   0        0        0     5936 2023-08-02 05:28:22.000000 mlh-0.1.2/mlh/s3_connect.py
--rw-rw-rw-   0        0        0    13968 2023-09-01 10:16:16.000000 mlh-0.1.2/mlh/snowflake_connect.py
--rw-rw-rw-   0        0        0     9675 2023-08-02 06:44:38.000000 mlh-0.1.2/mlh/sqlite_functions.py
--rw-rw-rw-   0        0        0    15539 2024-04-14 15:25:07.000000 mlh-0.1.2/mlh/support.py
--rw-rw-rw-   0        0        0    21100 2023-08-02 07:02:13.000000 mlh-0.1.2/mlh/woe.py
-drwxrwxrwx   0        0        0        0 2024-04-14 15:27:55.128068 mlh-0.1.2/mlh.egg-info/
--rw-rw-rw-   0        0        0     3157 2024-04-14 15:27:54.000000 mlh-0.1.2/mlh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2024-04-14 15:27:54.000000 mlh-0.1.2/mlh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 15:27:54.000000 mlh-0.1.2/mlh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2024-04-14 15:27:54.000000 mlh-0.1.2/mlh.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-14 15:27:54.000000 mlh-0.1.2/mlh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 15:27:55.144111 mlh-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      835 2024-04-14 15:26:06.000000 mlh-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 16:29:10.841057 mlh-0.1.3/
+-rw-rw-rw-   0        0        0     3157 2024-04-14 16:29:10.837210 mlh-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2582 2023-08-02 05:28:22.000000 mlh-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 16:29:10.758093 mlh-0.1.3/mlh/
+-rw-rw-rw-   0        0        0      270 2024-04-14 16:26:08.000000 mlh-0.1.3/mlh/__init__.py
+-rw-rw-rw-   0        0        0     6954 2023-08-04 04:57:16.000000 mlh-0.1.3/mlh/common_utils.py
+-rw-rw-rw-   0        0        0     7958 2024-01-08 17:56:03.000000 mlh-0.1.3/mlh/data_from_parquet.py
+-rw-rw-rw-   0        0        0     5936 2023-08-02 05:28:22.000000 mlh-0.1.3/mlh/s3_connect.py
+-rw-rw-rw-   0        0        0    13968 2023-09-01 10:16:16.000000 mlh-0.1.3/mlh/snowflake_connect.py
+-rw-rw-rw-   0        0        0     9675 2023-08-02 06:44:38.000000 mlh-0.1.3/mlh/sqlite_functions.py
+-rw-rw-rw-   0        0        0    15539 2024-04-14 15:25:07.000000 mlh-0.1.3/mlh/support.py
+-rw-rw-rw-   0        0        0    21100 2023-08-02 07:02:13.000000 mlh-0.1.3/mlh/woe.py
+drwxrwxrwx   0        0        0        0 2024-04-14 16:29:10.827113 mlh-0.1.3/mlh.egg-info/
+-rw-rw-rw-   0        0        0     3157 2024-04-14 16:29:10.000000 mlh-0.1.3/mlh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-04-14 16:29:10.000000 mlh-0.1.3/mlh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 16:29:10.000000 mlh-0.1.3/mlh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2024-04-14 16:29:10.000000 mlh-0.1.3/mlh.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-14 16:29:10.000000 mlh-0.1.3/mlh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 16:29:10.841643 mlh-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      835 2024-04-14 16:28:20.000000 mlh-0.1.3/setup.py
```

### Comparing `mlh-0.1.2/PKG-INFO` & `mlh-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlh
-Version: 0.1.2
+Version: 0.1.3
 Summary: This package provides helper utilities for machine learning tasks. One major utility is calculation of weight of evidence
 Home-page: https://github.com/devsahu99/mlh
 Author: Devendra Kumar Sahu
 Author-email: devsahu99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mlh-0.1.2/README.md` & `mlh-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mlh-0.1.2/mlh/common_utils.py` & `mlh-0.1.3/mlh/common_utils.py`

 * *Files identical despite different names*

### Comparing `mlh-0.1.2/mlh/data_from_parquet.py` & `mlh-0.1.3/mlh/data_from_parquet.py`

 * *Files identical despite different names*

### Comparing `mlh-0.1.2/mlh/s3_connect.py` & `mlh-0.1.3/mlh/s3_connect.py`

 * *Files identical despite different names*

### Comparing `mlh-0.1.2/mlh/snowflake_connect.py` & `mlh-0.1.3/mlh/snowflake_connect.py`

 * *Files identical despite different names*

### Comparing `mlh-0.1.2/mlh/sqlite_functions.py` & `mlh-0.1.3/mlh/sqlite_functions.py`

 * *Files identical despite different names*

### Comparing `mlh-0.1.2/mlh/support.py` & `mlh-0.1.3/mlh/support.py`

 * *Files identical despite different names*

### Comparing `mlh-0.1.2/mlh/woe.py` & `mlh-0.1.3/mlh/woe.py`

 * *Files identical despite different names*

### Comparing `mlh-0.1.2/mlh.egg-info/PKG-INFO` & `mlh-0.1.3/mlh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlh
-Version: 0.1.2
+Version: 0.1.3
 Summary: This package provides helper utilities for machine learning tasks. One major utility is calculation of weight of evidence
 Home-page: https://github.com/devsahu99/mlh
 Author: Devendra Kumar Sahu
 Author-email: devsahu99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mlh-0.1.2/setup.py` & `mlh-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mlh",
-    version = '0.1.2',
+    version = '0.1.3',
     author="Devendra Kumar Sahu",
     author_email="devsahu99@gmail.com",
     description="This package provides helper utilities for machine learning tasks. One major utility is calculation of weight of evidence",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/devsahu99/mlh",
     packages=['mlh'],
```

