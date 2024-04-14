# Comparing `tmp/tulona-0.5.1.tar.gz` & `tmp/tulona-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulona-0.5.1.tar", last modified: Sat Apr 13 15:32:54 2024, max compression
+gzip compressed data, was "tulona-0.5.2.tar", last modified: Sun Apr 14 04:04:58 2024, max compression
```

## Comparing `tulona-0.5.1.tar` & `tulona-0.5.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:32:54.002933 tulona-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-13 15:32:45.000000 tulona-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-04-13 15:32:54.002933 tulona-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-04-13 15:32:45.000000 tulona-0.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:32:53.994933 tulona-0.5.1/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:32:53.998933 tulona-0.5.1/core/tulona/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:32:53.998933 tulona-0.5.1/core/tulona/adapter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:32:53.998933 tulona-0.5.1/core/tulona/adapter/base/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/adapter/base/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/adapter/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/adapter/mssql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/adapter/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/adapter/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/adapter/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:32:53.998933 tulona-0.5.1/core/tulona/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     9753 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/cli/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:32:53.998933 tulona-0.5.1/core/tulona/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/config/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:32:54.002933 tulona-0.5.1/core/tulona/task/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/task/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17335 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/task/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/task/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/task/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/task/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/task/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:32:54.002933 tulona-0.5.1/core/tulona/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/util/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/util/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/util/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/util/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/util/profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/util/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-13 15:32:45.000000 tulona-0.5.1/core/tulona/util/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 15:32:54.002933 tulona-0.5.1/core/tulona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-04-13 15:32:53.000000 tulona-0.5.1/core/tulona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-13 15:32:53.000000 tulona-0.5.1/core/tulona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 15:32:53.000000 tulona-0.5.1/core/tulona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-13 15:32:53.000000 tulona-0.5.1/core/tulona.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-13 15:32:53.000000 tulona-0.5.1/core/tulona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-13 15:32:53.000000 tulona-0.5.1/core/tulona.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-13 15:32:45.000000 tulona-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 15:32:54.002933 tulona-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:04:58.667181 tulona-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-14 04:04:46.000000 tulona-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-04-14 04:04:58.667181 tulona-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-04-14 04:04:46.000000 tulona-0.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:04:58.659181 tulona-0.5.2/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:04:58.663181 tulona-0.5.2/core/tulona/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:04:58.663181 tulona-0.5.2/core/tulona/adapter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:04:58.663181 tulona-0.5.2/core/tulona/adapter/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/adapter/base/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/adapter/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/adapter/mssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/adapter/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/adapter/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/adapter/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:04:58.663181 tulona-0.5.2/core/tulona/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     9753 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/cli/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:04:58.663181 tulona-0.5.2/core/tulona/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:04:58.667181 tulona-0.5.2/core/tulona/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17335 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/task/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/task/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/task/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/task/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/task/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:04:58.667181 tulona-0.5.2/core/tulona/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/util/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/util/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/util/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/util/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/util/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5304 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/util/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-14 04:04:46.000000 tulona-0.5.2/core/tulona/util/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 04:04:58.667181 tulona-0.5.2/core/tulona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10305 2024-04-14 04:04:58.000000 tulona-0.5.2/core/tulona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-14 04:04:58.000000 tulona-0.5.2/core/tulona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 04:04:58.000000 tulona-0.5.2/core/tulona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-14 04:04:58.000000 tulona-0.5.2/core/tulona.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-14 04:04:58.000000 tulona-0.5.2/core/tulona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 04:04:58.000000 tulona-0.5.2/core/tulona.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-14 04:04:46.000000 tulona-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 04:04:58.667181 tulona-0.5.2/setup.cfg
```

### Comparing `tulona-0.5.1/LICENSE` & `tulona-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/PKG-INFO` & `tulona-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.5.1
+Version: 0.5.2
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
```

### Comparing `tulona-0.5.1/README.rst` & `tulona-0.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/core/tulona/adapter/connection.py` & `tulona-0.5.2/core/tulona/adapter/connection.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/core/tulona/adapter/mssql.py` & `tulona-0.5.2/core/tulona/adapter/mssql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/core/tulona/adapter/mysql.py` & `tulona-0.5.2/core/tulona/adapter/mysql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/core/tulona/adapter/postgres.py` & `tulona-0.5.2/core/tulona/adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/core/tulona/adapter/snowflake.py` & `tulona-0.5.2/core/tulona/adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/core/tulona/cli/base.py` & `tulona-0.5.2/core/tulona/cli/base.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/core/tulona/cli/params.py` & `tulona-0.5.2/core/tulona/cli/params.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/core/tulona/config/profile.py` & `tulona-0.5.2/core/tulona/config/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/core/tulona/config/project.py` & `tulona-0.5.2/core/tulona/config/project.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/core/tulona/exceptions.py` & `tulona-0.5.2/core/tulona/exceptions.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/core/tulona/task/base.py` & `tulona-0.5.2/core/tulona/task/base.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/core/tulona/task/compare.py` & `tulona-0.5.2/core/tulona/task/compare.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/core/tulona/task/helper.py` & `tulona-0.5.2/core/tulona/task/helper.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/core/tulona/task/ping.py` & `tulona-0.5.2/core/tulona/task/ping.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/core/tulona/task/profile.py` & `tulona-0.5.2/core/tulona/task/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/core/tulona/task/scan.py` & `tulona-0.5.2/core/tulona/task/scan.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/core/tulona/util/database.py` & `tulona-0.5.2/core/tulona/util/database.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/core/tulona/util/dataframe.py` & `tulona-0.5.2/core/tulona/util/dataframe.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/core/tulona/util/excel.py` & `tulona-0.5.2/core/tulona/util/excel.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/core/tulona/util/filesystem.py` & `tulona-0.5.2/core/tulona/util/filesystem.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/core/tulona/util/profiles.py` & `tulona-0.5.2/core/tulona/util/profiles.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/core/tulona/util/sql.py` & `tulona-0.5.2/core/tulona/util/sql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/core/tulona.egg-info/PKG-INFO` & `tulona-0.5.2/core/tulona.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.5.1
+Version: 0.5.2
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
```

### Comparing `tulona-0.5.1/core/tulona.egg-info/SOURCES.txt` & `tulona-0.5.2/core/tulona.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tulona-0.5.1/pyproject.toml` & `tulona-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tulona"
-version = "0.5.1"
+version = "0.5.2"
 description = "A tool to compare data from different sources."
 dependencies = [
   "click~=8.1",
   "ruamel.yaml~=0.18",
   "psycopg2-binary~=2.9",
   "pymysql~=1.1",
   "cryptography~=42.0",
@@ -110,15 +110,15 @@
 
 [tool.isort]
 profile = "black"
 line_length = 90
 skip = [".gitignore"]
 
 [tool.bumpversion]
-current_version = "0.5.1"
+current_version = "0.5.2"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
 tag = false
```

