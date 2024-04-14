# Comparing `tmp/pynonymizer-2.1.1.tar.gz` & `tmp/pynonymizer-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynonymizer-2.1.1.tar", last modified: Sat Apr  6 14:12:39 2024, max compression
+gzip compressed data, was "pynonymizer-2.2.0.tar", last modified: Sun Apr 14 16:33:37 2024, max compression
```

## Comparing `pynonymizer-2.1.1.tar` & `pynonymizer-2.2.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:12:39.825706 pynonymizer-2.1.1/
--rw-r--r--   0 root         (0) root         (0)     1050 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6537 2024-04-06 14:12:39.825706 pynonymizer-2.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5684 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:12:39.817706 pynonymizer-2.1.1/pynonymizer/
--rw-r--r--   0 root         (0) root         (0)       76 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/__main__.py
--rw-r--r--   0 root         (0) root         (0)     9811 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:12:39.821706 pynonymizer-2.1.1/pynonymizer/database/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/__init__.py
--rw-r--r--   0 root         (0) root         (0)      934 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2791 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:12:39.821706 pynonymizer-2.1.1/pynonymizer/database/mssql/
--rw-r--r--   0 root         (0) root         (0)    16622 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/mssql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8518 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/mssql/connectionstring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:12:39.821706 pynonymizer-2.1.1/pynonymizer/database/mysql/
--rw-r--r--   0 root         (0) root         (0)     7478 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/mysql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5214 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/mysql/execution.py
--rw-r--r--   0 root         (0) root         (0)     4560 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/mysql/query_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:12:39.821706 pynonymizer-2.1.1/pynonymizer/database/postgres/
--rw-r--r--   0 root         (0) root         (0)     7321 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/postgres/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4305 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/postgres/execution.py
--rw-r--r--   0 root         (0) root         (0)     5252 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/postgres/query_factory.py
--rw-r--r--   0 root         (0) root         (0)       48 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/database/provider.py
--rw-r--r--   0 root         (0) root         (0)      317 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:12:39.821706 pynonymizer-2.1.1/pynonymizer/fake/
--rw-r--r--   0 root         (0) root         (0)     3823 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/fake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3848 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/process_steps.py
--rw-r--r--   0 root         (0) root         (0)     4750 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/pynonymize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:12:39.825706 pynonymizer-2.1.1/pynonymizer/strategy/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/strategy/__init__.py
--rw-r--r--   0 root         (0) root         (0)      543 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/strategy/config.py
--rw-r--r--   0 root         (0) root         (0)     1910 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/strategy/database.py
--rw-r--r--   0 root         (0) root         (0)      797 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/strategy/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     8132 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/strategy/parser.py
--rw-r--r--   0 root         (0) root         (0)     1951 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/strategy/table.py
--rw-r--r--   0 root         (0) root         (0)     3283 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/pynonymizer/strategy/update_column.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:12:39.825706 pynonymizer-2.1.1/pynonymizer.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6537 2024-04-06 14:12:39.000000 pynonymizer-2.1.1/pynonymizer.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1144 2024-04-06 14:12:39.000000 pynonymizer-2.1.1/pynonymizer.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 14:12:39.000000 pynonymizer-2.1.1/pynonymizer.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-06 14:12:39.000000 pynonymizer-2.1.1/pynonymizer.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2024-04-06 14:12:39.000000 pynonymizer-2.1.1/pynonymizer.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-06 14:12:39.000000 pynonymizer-2.1.1/pynonymizer.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      122 2024-04-06 14:12:39.825706 pynonymizer-2.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1235 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:12:39.825706 pynonymizer-2.1.1/tests/
--rw-r--r--   0 root         (0) root         (0)      462 2024-04-06 14:12:32.000000 pynonymizer-2.1.1/tests/test_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 16:33:37.302275 pynonymizer-2.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1050 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6537 2024-04-14 16:33:37.302275 pynonymizer-2.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5684 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 16:33:37.294275 pynonymizer-2.2.0/pynonymizer/
+-rw-r--r--   0 root         (0) root         (0)       76 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 16:33:37.294275 pynonymizer-2.2.0/pynonymizer/database/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      934 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 16:33:37.298275 pynonymizer-2.2.0/pynonymizer/database/mssql/
+-rw-r--r--   0 root         (0) root         (0)    16778 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/mssql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8518 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/mssql/connectionstring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 16:33:37.298275 pynonymizer-2.2.0/pynonymizer/database/mysql/
+-rw-r--r--   0 root         (0) root         (0)     7478 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/mysql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5214 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/mysql/execution.py
+-rw-r--r--   0 root         (0) root         (0)     4560 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/mysql/query_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 16:33:37.298275 pynonymizer-2.2.0/pynonymizer/database/postgres/
+-rw-r--r--   0 root         (0) root         (0)     7321 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/postgres/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4305 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/postgres/execution.py
+-rw-r--r--   0 root         (0) root         (0)     5252 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/postgres/query_factory.py
+-rw-r--r--   0 root         (0) root         (0)       48 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/database/provider.py
+-rw-r--r--   0 root         (0) root         (0)      317 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 16:33:37.298275 pynonymizer-2.2.0/pynonymizer/fake/
+-rw-r--r--   0 root         (0) root         (0)     3823 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/fake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3848 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/process_steps.py
+-rw-r--r--   0 root         (0) root         (0)     4750 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/pynonymize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 16:33:37.298275 pynonymizer-2.2.0/pynonymizer/strategy/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/strategy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      543 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/strategy/config.py
+-rw-r--r--   0 root         (0) root         (0)     1910 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/strategy/database.py
+-rw-r--r--   0 root         (0) root         (0)      797 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/strategy/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     8132 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/strategy/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1951 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/strategy/table.py
+-rw-r--r--   0 root         (0) root         (0)     3283 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/pynonymizer/strategy/update_column.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 16:33:37.298275 pynonymizer-2.2.0/pynonymizer.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6537 2024-04-14 16:33:37.000000 pynonymizer-2.2.0/pynonymizer.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1144 2024-04-14 16:33:37.000000 pynonymizer-2.2.0/pynonymizer.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 16:33:37.000000 pynonymizer-2.2.0/pynonymizer.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-14 16:33:37.000000 pynonymizer-2.2.0/pynonymizer.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-14 16:33:37.000000 pynonymizer-2.2.0/pynonymizer.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-14 16:33:37.000000 pynonymizer-2.2.0/pynonymizer.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      122 2024-04-14 16:33:37.302275 pynonymizer-2.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1235 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 16:33:37.298275 pynonymizer-2.2.0/tests/
+-rw-r--r--   0 root         (0) root         (0)      462 2024-04-14 16:33:29.000000 pynonymizer-2.2.0/tests/test_meta.py
```

### Comparing `pynonymizer-2.1.1/LICENSE` & `pynonymizer-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.1/PKG-INFO` & `pynonymizer-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynonymizer
-Version: 2.1.1
+Version: 2.2.0
 Summary: An anonymization tool for production databases
 Home-page: https://github.com/rwnx/pynonymizer
 Author: Rowan Twell
 Author-email: rowantwell@gmail.com
 License: MIT
 Keywords: anonymization gdpr database mysql
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pynonymizer-2.1.1/README.md` & `pynonymizer-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.1/pynonymizer/cli.py` & `pynonymizer-2.2.0/pynonymizer/cli.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.1/pynonymizer/database/exceptions.py` & `pynonymizer-2.2.0/pynonymizer/database/exceptions.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.1/pynonymizer/database/io.py` & `pynonymizer-2.2.0/pynonymizer/database/io.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.1/pynonymizer/database/mssql/__init__.py` & `pynonymizer-2.2.0/pynonymizer/database/mssql/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,17 @@
         ansi_warnings_off=True,
     ):
         # import here for fast-failiness
         import pyodbc
 
         self.connnectionstr = ConnectionString.from_string(connection_string or "")
 
+        # Allow multiple results sets as this can cause connection busy when using multiple threads
+        self.connnectionstr["MARS_Connection"] = "yes"
+
         if db_name is None:
             raise ValueError("db_name is required")
         else:
             self.db_name = db_name
 
         if db_host and db_host.startswith(r"(local)\\"):
             self.connnectionstr["server"] = db_host
```

### Comparing `pynonymizer-2.1.1/pynonymizer/database/mssql/connectionstring.py` & `pynonymizer-2.2.0/pynonymizer/database/mssql/connectionstring.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.1/pynonymizer/database/mysql/__init__.py` & `pynonymizer-2.2.0/pynonymizer/database/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.1/pynonymizer/database/mysql/execution.py` & `pynonymizer-2.2.0/pynonymizer/database/mysql/execution.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.1/pynonymizer/database/mysql/query_factory.py` & `pynonymizer-2.2.0/pynonymizer/database/mysql/query_factory.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.1/pynonymizer/database/postgres/__init__.py` & `pynonymizer-2.2.0/pynonymizer/database/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.1/pynonymizer/database/postgres/execution.py` & `pynonymizer-2.2.0/pynonymizer/database/postgres/execution.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.1/pynonymizer/database/postgres/query_factory.py` & `pynonymizer-2.2.0/pynonymizer/database/postgres/query_factory.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.1/pynonymizer/fake/__init__.py` & `pynonymizer-2.2.0/pynonymizer/fake/__init__.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.1/pynonymizer/process_steps.py` & `pynonymizer-2.2.0/pynonymizer/process_steps.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.1/pynonymizer/pynonymize.py` & `pynonymizer-2.2.0/pynonymizer/pynonymize.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.1/pynonymizer/strategy/config.py` & `pynonymizer-2.2.0/pynonymizer/strategy/config.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.1/pynonymizer/strategy/database.py` & `pynonymizer-2.2.0/pynonymizer/strategy/database.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.1/pynonymizer/strategy/exceptions.py` & `pynonymizer-2.2.0/pynonymizer/strategy/exceptions.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.1/pynonymizer/strategy/parser.py` & `pynonymizer-2.2.0/pynonymizer/strategy/parser.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.1/pynonymizer/strategy/table.py` & `pynonymizer-2.2.0/pynonymizer/strategy/table.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.1/pynonymizer/strategy/update_column.py` & `pynonymizer-2.2.0/pynonymizer/strategy/update_column.py`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.1/pynonymizer.egg-info/PKG-INFO` & `pynonymizer-2.2.0/pynonymizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynonymizer
-Version: 2.1.1
+Version: 2.2.0
 Summary: An anonymization tool for production databases
 Home-page: https://github.com/rwnx/pynonymizer
 Author: Rowan Twell
 Author-email: rowantwell@gmail.com
 License: MIT
 Keywords: anonymization gdpr database mysql
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pynonymizer-2.1.1/pynonymizer.egg-info/SOURCES.txt` & `pynonymizer-2.2.0/pynonymizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynonymizer-2.1.1/setup.py` & `pynonymizer-2.2.0/setup.py`

 * *Files identical despite different names*

