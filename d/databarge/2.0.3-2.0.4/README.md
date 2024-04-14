# Comparing `tmp/databarge-2.0.3.tar.gz` & `tmp/databarge-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "databarge-2.0.3.tar", last modified: Mon Apr  8 11:38:29 2024, max compression
+gzip compressed data, was "databarge-2.0.4.tar", last modified: Sun Apr 14 12:10:54 2024, max compression
```

## Comparing `databarge-2.0.3.tar` & `databarge-2.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 11:38:29.822093 databarge-2.0.3/
--rw-rw-rw-   0        0        0     1092 2024-03-27 12:25:58.000000 databarge-2.0.3/LICENSE
--rw-rw-rw-   0        0        0     4598 2024-04-08 11:38:29.820696 databarge-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4001 2024-04-04 18:13:36.000000 databarge-2.0.3/README.md
--rw-rw-rw-   0        0        0      708 2024-04-08 11:37:19.000000 databarge-2.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-08 11:38:29.822093 databarge-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0      426 2024-04-08 11:37:12.000000 databarge-2.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-08 11:38:29.785656 databarge-2.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-08 11:38:29.804823 databarge-2.0.3/src/databarge/
--rw-rw-rw-   0        0        0      241 2024-04-04 18:50:47.000000 databarge-2.0.3/src/databarge/__init__.py
--rw-rw-rw-   0        0        0     2764 2024-03-31 16:37:11.000000 databarge-2.0.3/src/databarge/connections.py
--rw-rw-rw-   0        0        0     2400 2024-03-31 16:37:55.000000 databarge-2.0.3/src/databarge/dimensions.py
--rw-rw-rw-   0        0        0     3718 2024-03-31 16:37:47.000000 databarge-2.0.3/src/databarge/execution.py
--rw-rw-rw-   0        0        0      371 2024-03-27 12:34:35.000000 databarge-2.0.3/src/databarge/functions.py
--rw-rw-rw-   0        0        0    16160 2024-04-01 19:36:55.000000 databarge-2.0.3/src/databarge/transfers.py
-drwxrwxrwx   0        0        0        0 2024-04-08 11:38:29.819253 databarge-2.0.3/src/databarge.egg-info/
--rw-rw-rw-   0        0        0     4598 2024-04-08 11:38:29.000000 databarge-2.0.3/src/databarge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2024-04-08 11:38:29.000000 databarge-2.0.3/src/databarge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 11:38:29.000000 databarge-2.0.3/src/databarge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-08 11:38:29.000000 databarge-2.0.3/src/databarge.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 12:10:54.800332 databarge-2.0.4/
+-rw-rw-rw-   0        0        0     1092 2024-03-27 12:25:58.000000 databarge-2.0.4/LICENSE
+-rw-rw-rw-   0        0        0     4598 2024-04-14 12:10:54.797824 databarge-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4001 2024-04-04 18:13:36.000000 databarge-2.0.4/README.md
+-rw-rw-rw-   0        0        0      708 2024-04-14 12:08:47.000000 databarge-2.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-14 12:10:54.800958 databarge-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      426 2024-04-14 12:09:06.000000 databarge-2.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 12:10:54.755112 databarge-2.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-14 12:10:54.786903 databarge-2.0.4/src/databarge/
+-rw-rw-rw-   0        0        0      312 2024-04-14 12:07:48.000000 databarge-2.0.4/src/databarge/__init__.py
+-rw-rw-rw-   0        0        0     2764 2024-03-31 16:37:11.000000 databarge-2.0.4/src/databarge/connections.py
+-rw-rw-rw-   0        0        0     2400 2024-03-31 16:37:55.000000 databarge-2.0.4/src/databarge/dimensions.py
+-rw-rw-rw-   0        0        0     3720 2024-04-14 12:03:35.000000 databarge-2.0.4/src/databarge/execution.py
+-rw-rw-rw-   0        0        0      371 2024-03-27 12:34:35.000000 databarge-2.0.4/src/databarge/functions.py
+-rw-rw-rw-   0        0        0    16160 2024-04-01 19:36:55.000000 databarge-2.0.4/src/databarge/transfers.py
+drwxrwxrwx   0        0        0        0 2024-04-14 12:10:54.794968 databarge-2.0.4/src/databarge.egg-info/
+-rw-rw-rw-   0        0        0     4598 2024-04-14 12:10:54.000000 databarge-2.0.4/src/databarge.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2024-04-14 12:10:54.000000 databarge-2.0.4/src/databarge.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 12:10:54.000000 databarge-2.0.4/src/databarge.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-14 12:10:54.000000 databarge-2.0.4/src/databarge.egg-info/top_level.txt
```

### Comparing `databarge-2.0.3/LICENSE` & `databarge-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `databarge-2.0.3/PKG-INFO` & `databarge-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databarge
-Version: 2.0.3
+Version: 2.0.4
 Summary: Simple ETL tools for SQL Server
 Home-page: https://github.com/porteverte/databarge
 Author: Porte Verte
 Author-email: Port Verte <porte_verte@outlook.com>
 Project-URL: Homepage, https://github.com/porteverte/databarge
 Project-URL: Issues, https://github.com/porteverte/databarge/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `databarge-2.0.3/README.md` & `databarge-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `databarge-2.0.3/pyproject.toml` & `databarge-2.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "databarge"
-version = "2.0.3"
+version = "2.0.4"
 authors = [
   { name="Port Verte", email="porte_verte@outlook.com" },
 ]
 description = "Simple ETL tools for SQL Server"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `databarge-2.0.3/src/databarge/connections.py` & `databarge-2.0.4/src/databarge/connections.py`

 * *Files identical despite different names*

### Comparing `databarge-2.0.3/src/databarge/dimensions.py` & `databarge-2.0.4/src/databarge/dimensions.py`

 * *Files identical despite different names*

### Comparing `databarge-2.0.3/src/databarge/execution.py` & `databarge-2.0.4/src/databarge/execution.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # ===================================================================================================
 # EXECUTE CODE
 # ===================================================================================================
 
 def run_sql_server_code(my_conn, my_db, my_code, log_path):
     
     import sys
-    from gen_mods.misc_fns import write_to_log
+    # from gen_mods.misc_fns import write_to_log
     
     if log_path != None and len(log_path) > 0:
         write_to_log(log_path, 'code execution started: ' + my_code)
 
     my_cursor = my_conn.connection.cursor()
     my_cursor.execute("USE " + my_db)
```

### Comparing `databarge-2.0.3/src/databarge/transfers.py` & `databarge-2.0.4/src/databarge/transfers.py`

 * *Files identical despite different names*

### Comparing `databarge-2.0.3/src/databarge.egg-info/PKG-INFO` & `databarge-2.0.4/src/databarge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databarge
-Version: 2.0.3
+Version: 2.0.4
 Summary: Simple ETL tools for SQL Server
 Home-page: https://github.com/porteverte/databarge
 Author: Porte Verte
 Author-email: Port Verte <porte_verte@outlook.com>
 Project-URL: Homepage, https://github.com/porteverte/databarge
 Project-URL: Issues, https://github.com/porteverte/databarge/issues
 Classifier: Programming Language :: Python :: 3
```

