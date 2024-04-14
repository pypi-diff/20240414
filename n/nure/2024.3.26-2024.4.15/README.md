# Comparing `tmp/nure-2024.3.26.tar.gz` & `tmp/nure-2024.4.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nure-2024.3.26.tar", last modified: Tue Mar 26 08:05:56 2024, max compression
+gzip compressed data, was "nure-2024.4.15.tar", last modified: Sun Apr 14 17:03:02 2024, max compression
```

## Comparing `nure-2024.3.26.tar` & `nure-2024.4.15.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 trungtran   (502) staff       (20)        0 2024-03-26 08:05:56.151270 nure-2024.3.26/
--rw-r--r--   0 trungtran   (502) staff       (20)    35149 2024-03-26 07:11:04.000000 nure-2024.3.26/LICENSE
--rw-r--r--   0 trungtran   (502) staff       (20)      993 2024-03-26 08:05:56.151014 nure-2024.3.26/PKG-INFO
--rw-r--r--   0 trungtran   (502) staff       (20)       30 2024-03-26 07:11:04.000000 nure-2024.3.26/README.md
-drwxr-xr-x   0 trungtran   (502) staff       (20)        0 2024-03-26 08:05:56.136811 nure-2024.3.26/nure/
--rw-r--r--   0 trungtran   (502) staff       (20)        0 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/__init__.py
--rw-r--r--   0 trungtran   (502) staff       (20)     2523 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/archive.py
--rw-r--r--   0 trungtran   (502) staff       (20)     2379 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/array.py
-drwxr-xr-x   0 trungtran   (502) staff       (20)        0 2024-03-26 08:05:56.137281 nure-2024.3.26/nure/code/
--rw-r--r--   0 trungtran   (502) staff       (20)       62 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/code/__init__.py
--rw-r--r--   0 trungtran   (502) staff       (20)     1353 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/code/label_coder.py
--rw-r--r--   0 trungtran   (502) staff       (20)     4912 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/dataframe.py
--rw-r--r--   0 trungtran   (502) staff       (20)     1263 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/datetime.py
--rw-r--r--   0 trungtran   (502) staff       (20)      106 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/debug.py
--rw-r--r--   0 trungtran   (502) staff       (20)     1416 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/dict.py
--rw-r--r--   0 trungtran   (502) staff       (20)      487 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/func.py
-drwxr-xr-x   0 trungtran   (502) staff       (20)        0 2024-03-26 08:05:56.138293 nure-2024.3.26/nure/image/
--rw-r--r--   0 trungtran   (502) staff       (20)        0 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/image/__init__.py
--rw-r--r--   0 trungtran   (502) staff       (20)    10325 2024-03-26 07:21:02.000000 nure-2024.3.26/nure/image/annotate.py
--rw-r--r--   0 trungtran   (502) staff       (20)     6438 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/image/func.py
--rw-r--r--   0 trungtran   (502) staff       (20)     6667 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/image/pil.py
--rw-r--r--   0 trungtran   (502) staff       (20)     1457 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/meta.py
--rw-r--r--   0 trungtran   (502) staff       (20)      445 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/path.py
-drwxr-xr-x   0 trungtran   (502) staff       (20)        0 2024-03-26 08:05:56.139636 nure-2024.3.26/nure/sync/
--rw-r--r--   0 trungtran   (502) staff       (20)        0 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/sync/__init__.py
--rw-r--r--   0 trungtran   (502) staff       (20)      457 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/sync/bigquery.py
--rw-r--r--   0 trungtran   (502) staff       (20)     1628 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/sync/cache.py
--rw-r--r--   0 trungtran   (502) staff       (20)     3249 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/sync/googlesheet.py
--rw-r--r--   0 trungtran   (502) staff       (20)      706 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/sync/postgre.py
--rw-r--r--   0 trungtran   (502) staff       (20)     3481 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/sync/s3.py
--rw-r--r--   0 trungtran   (502) staff       (20)     1806 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/sync/sql.py
--rw-r--r--   0 trungtran   (502) staff       (20)     1450 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/sync/suffix.py
--rw-r--r--   0 trungtran   (502) staff       (20)     2872 2024-03-26 07:11:04.000000 nure-2024.3.26/nure/volatitle.py
-drwxr-xr-x   0 trungtran   (502) staff       (20)        0 2024-03-26 08:05:56.150355 nure-2024.3.26/nure.egg-info/
--rw-r--r--   0 trungtran   (502) staff       (20)      993 2024-03-26 08:05:56.000000 nure-2024.3.26/nure.egg-info/PKG-INFO
--rw-r--r--   0 trungtran   (502) staff       (20)      842 2024-03-26 08:05:56.000000 nure-2024.3.26/nure.egg-info/SOURCES.txt
--rw-r--r--   0 trungtran   (502) staff       (20)        1 2024-03-26 08:05:56.000000 nure-2024.3.26/nure.egg-info/dependency_links.txt
--rw-r--r--   0 trungtran   (502) staff       (20)      154 2024-03-26 08:05:56.000000 nure-2024.3.26/nure.egg-info/requires.txt
--rw-r--r--   0 trungtran   (502) staff       (20)        5 2024-03-26 08:05:56.000000 nure-2024.3.26/nure.egg-info/top_level.txt
--rw-r--r--   0 trungtran   (502) staff       (20)      103 2024-03-26 07:11:04.000000 nure-2024.3.26/pyproject.toml
--rw-r--r--   0 trungtran   (502) staff       (20)      858 2024-03-26 08:05:56.151662 nure-2024.3.26/setup.cfg
-drwxr-xr-x   0 trungtran   (502) staff       (20)        0 2024-03-26 08:05:56.147961 nure-2024.3.26/tests/
--rw-r--r--   0 trungtran   (502) staff       (20)     1011 2024-03-26 07:11:04.000000 nure-2024.3.26/tests/test_archive.py
--rw-r--r--   0 trungtran   (502) staff       (20)     1225 2024-03-26 07:11:04.000000 nure-2024.3.26/tests/test_bigquery.py
--rw-r--r--   0 trungtran   (502) staff       (20)     2890 2024-03-26 07:11:04.000000 nure-2024.3.26/tests/test_coder.py
--rw-r--r--   0 trungtran   (502) staff       (20)      792 2024-03-26 07:11:04.000000 nure-2024.3.26/tests/test_googlesheet.py
--rw-r--r--   0 trungtran   (502) staff       (20)     3698 2024-03-26 07:11:04.000000 nure-2024.3.26/tests/test_parallel.py
--rw-r--r--   0 trungtran   (502) staff       (20)      708 2024-03-26 07:11:04.000000 nure-2024.3.26/tests/test_postgre.py
--rw-r--r--   0 trungtran   (502) staff       (20)      655 2024-03-26 07:11:04.000000 nure-2024.3.26/tests/test_s3.py
+drwxr-xr-x   0 trungtran   (502) staff       (20)        0 2024-04-14 17:03:02.317737 nure-2024.4.15/
+-rw-r--r--   0 trungtran   (502) staff       (20)    35149 2024-03-26 07:11:04.000000 nure-2024.4.15/LICENSE
+-rw-r--r--   0 trungtran   (502) staff       (20)      993 2024-04-14 17:03:02.317657 nure-2024.4.15/PKG-INFO
+-rw-r--r--   0 trungtran   (502) staff       (20)       30 2024-03-26 07:11:04.000000 nure-2024.4.15/README.md
+drwxr-xr-x   0 trungtran   (502) staff       (20)        0 2024-04-14 17:03:02.311763 nure-2024.4.15/nure/
+-rw-r--r--   0 trungtran   (502) staff       (20)        0 2024-03-26 07:11:04.000000 nure-2024.4.15/nure/__init__.py
+-rw-r--r--   0 trungtran   (502) staff       (20)     2523 2024-03-26 07:11:04.000000 nure-2024.4.15/nure/archive.py
+-rw-r--r--   0 trungtran   (502) staff       (20)     3637 2024-04-14 17:01:53.000000 nure-2024.4.15/nure/array.py
+drwxr-xr-x   0 trungtran   (502) staff       (20)        0 2024-04-14 17:03:02.312141 nure-2024.4.15/nure/code/
+-rw-r--r--   0 trungtran   (502) staff       (20)       62 2024-03-26 07:11:04.000000 nure-2024.4.15/nure/code/__init__.py
+-rw-r--r--   0 trungtran   (502) staff       (20)     1576 2024-04-14 16:57:47.000000 nure-2024.4.15/nure/code/label_coder.py
+-rw-r--r--   0 trungtran   (502) staff       (20)     4912 2024-03-26 07:11:04.000000 nure-2024.4.15/nure/dataframe.py
+-rw-r--r--   0 trungtran   (502) staff       (20)     1263 2024-03-26 07:11:04.000000 nure-2024.4.15/nure/datetime.py
+-rw-r--r--   0 trungtran   (502) staff       (20)      106 2024-03-26 07:11:04.000000 nure-2024.4.15/nure/debug.py
+-rw-r--r--   0 trungtran   (502) staff       (20)     1416 2024-03-26 07:11:04.000000 nure-2024.4.15/nure/dict.py
+-rw-r--r--   0 trungtran   (502) staff       (20)      487 2024-03-26 07:11:04.000000 nure-2024.4.15/nure/func.py
+drwxr-xr-x   0 trungtran   (502) staff       (20)        0 2024-04-14 17:03:02.313150 nure-2024.4.15/nure/image/
+-rw-r--r--   0 trungtran   (502) staff       (20)        0 2024-03-26 07:11:04.000000 nure-2024.4.15/nure/image/__init__.py
+-rw-r--r--   0 trungtran   (502) staff       (20)    10325 2024-03-26 07:21:02.000000 nure-2024.4.15/nure/image/annotate.py
+-rw-r--r--   0 trungtran   (502) staff       (20)     6438 2024-03-26 07:11:04.000000 nure-2024.4.15/nure/image/func.py
+-rw-r--r--   0 trungtran   (502) staff       (20)     6667 2024-03-26 07:11:04.000000 nure-2024.4.15/nure/image/pil.py
+-rw-r--r--   0 trungtran   (502) staff       (20)     1457 2024-03-26 07:11:04.000000 nure-2024.4.15/nure/meta.py
+-rw-r--r--   0 trungtran   (502) staff       (20)      445 2024-03-26 07:11:04.000000 nure-2024.4.15/nure/path.py
+drwxr-xr-x   0 trungtran   (502) staff       (20)        0 2024-04-14 17:03:02.314449 nure-2024.4.15/nure/sync/
+-rw-r--r--   0 trungtran   (502) staff       (20)        0 2024-03-26 07:11:04.000000 nure-2024.4.15/nure/sync/__init__.py
+-rw-r--r--   0 trungtran   (502) staff       (20)      457 2024-03-26 07:11:04.000000 nure-2024.4.15/nure/sync/bigquery.py
+-rw-r--r--   0 trungtran   (502) staff       (20)     1628 2024-03-26 07:11:04.000000 nure-2024.4.15/nure/sync/cache.py
+-rw-r--r--   0 trungtran   (502) staff       (20)     3249 2024-03-26 07:11:04.000000 nure-2024.4.15/nure/sync/googlesheet.py
+-rw-r--r--   0 trungtran   (502) staff       (20)      706 2024-03-26 07:11:04.000000 nure-2024.4.15/nure/sync/postgre.py
+-rw-r--r--   0 trungtran   (502) staff       (20)     3481 2024-03-26 07:11:04.000000 nure-2024.4.15/nure/sync/s3.py
+-rw-r--r--   0 trungtran   (502) staff       (20)     1806 2024-03-26 07:11:04.000000 nure-2024.4.15/nure/sync/sql.py
+-rw-r--r--   0 trungtran   (502) staff       (20)     1450 2024-03-26 07:11:04.000000 nure-2024.4.15/nure/sync/suffix.py
+-rw-r--r--   0 trungtran   (502) staff       (20)     2872 2024-03-26 07:11:04.000000 nure-2024.4.15/nure/volatitle.py
+drwxr-xr-x   0 trungtran   (502) staff       (20)        0 2024-04-14 17:03:02.317151 nure-2024.4.15/nure.egg-info/
+-rw-r--r--   0 trungtran   (502) staff       (20)      993 2024-04-14 17:03:02.000000 nure-2024.4.15/nure.egg-info/PKG-INFO
+-rw-r--r--   0 trungtran   (502) staff       (20)      842 2024-04-14 17:03:02.000000 nure-2024.4.15/nure.egg-info/SOURCES.txt
+-rw-r--r--   0 trungtran   (502) staff       (20)        1 2024-04-14 17:03:02.000000 nure-2024.4.15/nure.egg-info/dependency_links.txt
+-rw-r--r--   0 trungtran   (502) staff       (20)      154 2024-04-14 17:03:02.000000 nure-2024.4.15/nure.egg-info/requires.txt
+-rw-r--r--   0 trungtran   (502) staff       (20)        5 2024-04-14 17:03:02.000000 nure-2024.4.15/nure.egg-info/top_level.txt
+-rw-r--r--   0 trungtran   (502) staff       (20)      103 2024-03-26 07:11:04.000000 nure-2024.4.15/pyproject.toml
+-rw-r--r--   0 trungtran   (502) staff       (20)      858 2024-04-14 17:03:02.318015 nure-2024.4.15/setup.cfg
+drwxr-xr-x   0 trungtran   (502) staff       (20)        0 2024-04-14 17:03:02.316687 nure-2024.4.15/tests/
+-rw-r--r--   0 trungtran   (502) staff       (20)     1011 2024-03-26 07:11:04.000000 nure-2024.4.15/tests/test_archive.py
+-rw-r--r--   0 trungtran   (502) staff       (20)     1225 2024-03-26 07:11:04.000000 nure-2024.4.15/tests/test_bigquery.py
+-rw-r--r--   0 trungtran   (502) staff       (20)     2890 2024-03-26 07:11:04.000000 nure-2024.4.15/tests/test_coder.py
+-rw-r--r--   0 trungtran   (502) staff       (20)      792 2024-03-26 07:11:04.000000 nure-2024.4.15/tests/test_googlesheet.py
+-rw-r--r--   0 trungtran   (502) staff       (20)     3698 2024-03-26 07:11:04.000000 nure-2024.4.15/tests/test_parallel.py
+-rw-r--r--   0 trungtran   (502) staff       (20)      708 2024-03-26 07:11:04.000000 nure-2024.4.15/tests/test_postgre.py
+-rw-r--r--   0 trungtran   (502) staff       (20)      655 2024-03-26 07:11:04.000000 nure-2024.4.15/tests/test_s3.py
```

### Comparing `nure-2024.3.26/LICENSE` & `nure-2024.4.15/LICENSE`

 * *Files identical despite different names*

### Comparing `nure-2024.3.26/PKG-INFO` & `nure-2024.4.15/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nure
-Version: 2024.3.26
+Version: 2024.4.15
 Summary: Data Science Utilities
 Home-page: https://github.com/tranduytrung/nure
 Author: Trung Tran
 Author-email: tranduytrung@outlook.com
 Project-URL: Bug Tracker, https://github.com/tranduytrung/nure/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `nure-2024.3.26/nure/archive.py` & `nure-2024.4.15/nure/archive.py`

 * *Files identical despite different names*

### Comparing `nure-2024.3.26/nure/dataframe.py` & `nure-2024.4.15/nure/dataframe.py`

 * *Files identical despite different names*

### Comparing `nure-2024.3.26/nure/datetime.py` & `nure-2024.4.15/nure/datetime.py`

 * *Files identical despite different names*

### Comparing `nure-2024.3.26/nure/dict.py` & `nure-2024.4.15/nure/dict.py`

 * *Files identical despite different names*

### Comparing `nure-2024.3.26/nure/image/annotate.py` & `nure-2024.4.15/nure/image/annotate.py`

 * *Files identical despite different names*

### Comparing `nure-2024.3.26/nure/image/func.py` & `nure-2024.4.15/nure/image/func.py`

 * *Files identical despite different names*

### Comparing `nure-2024.3.26/nure/image/pil.py` & `nure-2024.4.15/nure/image/pil.py`

 * *Files identical despite different names*

### Comparing `nure-2024.3.26/nure/meta.py` & `nure-2024.4.15/nure/meta.py`

 * *Files identical despite different names*

### Comparing `nure-2024.3.26/nure/sync/cache.py` & `nure-2024.4.15/nure/sync/cache.py`

 * *Files identical despite different names*

### Comparing `nure-2024.3.26/nure/sync/googlesheet.py` & `nure-2024.4.15/nure/sync/googlesheet.py`

 * *Files identical despite different names*

### Comparing `nure-2024.3.26/nure/sync/postgre.py` & `nure-2024.4.15/nure/sync/postgre.py`

 * *Files identical despite different names*

### Comparing `nure-2024.3.26/nure/sync/s3.py` & `nure-2024.4.15/nure/sync/s3.py`

 * *Files identical despite different names*

### Comparing `nure-2024.3.26/nure/sync/sql.py` & `nure-2024.4.15/nure/sync/sql.py`

 * *Files identical despite different names*

### Comparing `nure-2024.3.26/nure/sync/suffix.py` & `nure-2024.4.15/nure/sync/suffix.py`

 * *Files identical despite different names*

### Comparing `nure-2024.3.26/nure/volatitle.py` & `nure-2024.4.15/nure/volatitle.py`

 * *Files identical despite different names*

### Comparing `nure-2024.3.26/nure.egg-info/PKG-INFO` & `nure-2024.4.15/nure.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nure
-Version: 2024.3.26
+Version: 2024.4.15
 Summary: Data Science Utilities
 Home-page: https://github.com/tranduytrung/nure
 Author: Trung Tran
 Author-email: tranduytrung@outlook.com
 Project-URL: Bug Tracker, https://github.com/tranduytrung/nure/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `nure-2024.3.26/nure.egg-info/SOURCES.txt` & `nure-2024.4.15/nure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nure-2024.3.26/setup.cfg` & `nure-2024.4.15/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nure
-version = 2024.03.26
+version = 2024.04.15
 author = Trung Tran
 author_email = tranduytrung@outlook.com
 description = Data Science Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tranduytrung/nure
 project_urls =
```

### Comparing `nure-2024.3.26/tests/test_archive.py` & `nure-2024.4.15/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `nure-2024.3.26/tests/test_bigquery.py` & `nure-2024.4.15/tests/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `nure-2024.3.26/tests/test_coder.py` & `nure-2024.4.15/tests/test_coder.py`

 * *Files identical despite different names*

### Comparing `nure-2024.3.26/tests/test_googlesheet.py` & `nure-2024.4.15/tests/test_googlesheet.py`

 * *Files identical despite different names*

### Comparing `nure-2024.3.26/tests/test_parallel.py` & `nure-2024.4.15/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `nure-2024.3.26/tests/test_postgre.py` & `nure-2024.4.15/tests/test_postgre.py`

 * *Files identical despite different names*

### Comparing `nure-2024.3.26/tests/test_s3.py` & `nure-2024.4.15/tests/test_s3.py`

 * *Files identical despite different names*

