# Comparing `tmp/chipmunkdb_python_client-2.0.8.tar.gz` & `tmp/chipmunkdb_python_client-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chipmunkdb_python_client-2.0.8.tar", last modified: Fri Dec 29 09:13:04 2023, max compression
+gzip compressed data, was "dist/chipmunkdb_python_client-2.0.9.tar", last modified: Fri Dec 29 09:52:14 2023, max compression
```

## Comparing `chipmunkdb_python_client-2.0.8.tar` & `chipmunkdb_python_client-2.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-29 09:13:04.055423 chipmunkdb_python_client-2.0.8/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-29 09:12:52.000000 chipmunkdb_python_client-2.0.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-12-29 09:12:51.000000 chipmunkdb_python_client-2.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1555 2023-12-29 09:13:04.055423 chipmunkdb_python_client-2.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      210 2023-12-29 09:12:51.000000 chipmunkdb_python_client-2.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-29 09:13:04.051423 chipmunkdb_python_client-2.0.8/chipmunkdb/
--rw-rw-rw-   0 root         (0) root         (0)     3070 2023-12-29 09:12:51.000000 chipmunkdb_python_client-2.0.8/chipmunkdb/ChipmunkConnection.py
--rw-rw-rw-   0 root         (0) root         (0)     6483 2023-12-29 09:12:51.000000 chipmunkdb_python_client-2.0.8/chipmunkdb/ChipmunkDb.py
--rw-rw-rw-   0 root         (0) root         (0)     2548 2023-12-29 09:12:51.000000 chipmunkdb_python_client-2.0.8/chipmunkdb/ChipmunkDialect.py
--rw-rw-rw-   0 root         (0) root         (0)      124 2023-12-29 09:12:51.000000 chipmunkdb_python_client-2.0.8/chipmunkdb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-29 09:12:52.000000 chipmunkdb_python_client-2.0.8/chipmunkdb/config.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-29 09:13:04.055423 chipmunkdb_python_client-2.0.8/chipmunkdb_python_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1555 2023-12-29 09:13:04.000000 chipmunkdb_python_client-2.0.8/chipmunkdb_python_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      676 2023-12-29 09:13:04.000000 chipmunkdb_python_client-2.0.8/chipmunkdb_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-29 09:13:04.000000 chipmunkdb_python_client-2.0.8/chipmunkdb_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       72 2023-12-29 09:13:04.000000 chipmunkdb_python_client-2.0.8/chipmunkdb_python_client.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-12-29 09:13:04.000000 chipmunkdb_python_client-2.0.8/chipmunkdb_python_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-12-29 09:13:04.000000 chipmunkdb_python_client-2.0.8/chipmunkdb_python_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-29 09:13:04.056423 chipmunkdb_python_client-2.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1168 2023-12-29 09:12:51.000000 chipmunkdb_python_client-2.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-29 09:13:04.055423 chipmunkdb_python_client-2.0.8/test/
--rw-rw-rw-   0 root         (0) root         (0)     2495 2023-12-29 09:12:51.000000 chipmunkdb_python_client-2.0.8/test/test.py
--rw-rw-rw-   0 root         (0) root         (0)      331 2023-12-29 09:12:51.000000 chipmunkdb_python_client-2.0.8/test/testDelete.py
--rw-rw-rw-   0 root         (0) root         (0)     3536 2023-12-29 09:12:51.000000 chipmunkdb_python_client-2.0.8/test/testDomain.py
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-12-29 09:12:51.000000 chipmunkdb_python_client-2.0.8/test/testStorage.py
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-12-29 09:12:51.000000 chipmunkdb_python_client-2.0.8/test/testdocument.py
--rw-rw-rw-   0 root         (0) root         (0)      558 2023-12-29 09:12:51.000000 chipmunkdb_python_client-2.0.8/test/testduck_multiindex.py
--rw-rw-rw-   0 root         (0) root         (0)      162 2023-12-29 09:12:51.000000 chipmunkdb_python_client-2.0.8/test/testmultiindex_save_load.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2023-12-29 09:12:51.000000 chipmunkdb_python_client-2.0.8/test/testmultiples.py
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-12-29 09:12:51.000000 chipmunkdb_python_client-2.0.8/test/testsize.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2023-12-29 09:12:51.000000 chipmunkdb_python_client-2.0.8/test/testsuperlarge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-29 09:52:14.426153 chipmunkdb_python_client-2.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-29 09:52:01.000000 chipmunkdb_python_client-2.0.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-12-29 09:52:01.000000 chipmunkdb_python_client-2.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-12-29 09:52:14.426153 chipmunkdb_python_client-2.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      210 2023-12-29 09:52:01.000000 chipmunkdb_python_client-2.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-29 09:52:14.421153 chipmunkdb_python_client-2.0.9/chipmunkdb/
+-rw-rw-rw-   0 root         (0) root         (0)     3070 2023-12-29 09:52:01.000000 chipmunkdb_python_client-2.0.9/chipmunkdb/ChipmunkConnection.py
+-rw-rw-rw-   0 root         (0) root         (0)     6483 2023-12-29 09:52:01.000000 chipmunkdb_python_client-2.0.9/chipmunkdb/ChipmunkDb.py
+-rw-rw-rw-   0 root         (0) root         (0)     2548 2023-12-29 09:52:01.000000 chipmunkdb_python_client-2.0.9/chipmunkdb/ChipmunkDialect.py
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-12-29 09:52:01.000000 chipmunkdb_python_client-2.0.9/chipmunkdb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-12-29 09:52:01.000000 chipmunkdb_python_client-2.0.9/chipmunkdb/config.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-29 09:52:14.425153 chipmunkdb_python_client-2.0.9/chipmunkdb_python_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-12-29 09:52:14.000000 chipmunkdb_python_client-2.0.9/chipmunkdb_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      676 2023-12-29 09:52:14.000000 chipmunkdb_python_client-2.0.9/chipmunkdb_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-29 09:52:14.000000 chipmunkdb_python_client-2.0.9/chipmunkdb_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-12-29 09:52:14.000000 chipmunkdb_python_client-2.0.9/chipmunkdb_python_client.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-12-29 09:52:14.000000 chipmunkdb_python_client-2.0.9/chipmunkdb_python_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-12-29 09:52:14.000000 chipmunkdb_python_client-2.0.9/chipmunkdb_python_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-12-29 09:52:14.426153 chipmunkdb_python_client-2.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1218 2023-12-29 09:52:01.000000 chipmunkdb_python_client-2.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-29 09:52:14.425153 chipmunkdb_python_client-2.0.9/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2495 2023-12-29 09:52:01.000000 chipmunkdb_python_client-2.0.9/test/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      331 2023-12-29 09:52:01.000000 chipmunkdb_python_client-2.0.9/test/testDelete.py
+-rw-rw-rw-   0 root         (0) root         (0)     3536 2023-12-29 09:52:01.000000 chipmunkdb_python_client-2.0.9/test/testDomain.py
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-12-29 09:52:01.000000 chipmunkdb_python_client-2.0.9/test/testStorage.py
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-12-29 09:52:01.000000 chipmunkdb_python_client-2.0.9/test/testdocument.py
+-rw-rw-rw-   0 root         (0) root         (0)      558 2023-12-29 09:52:01.000000 chipmunkdb_python_client-2.0.9/test/testduck_multiindex.py
+-rw-rw-rw-   0 root         (0) root         (0)      162 2023-12-29 09:52:01.000000 chipmunkdb_python_client-2.0.9/test/testmultiindex_save_load.py
+-rw-rw-rw-   0 root         (0) root         (0)      348 2023-12-29 09:52:01.000000 chipmunkdb_python_client-2.0.9/test/testmultiples.py
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-12-29 09:52:01.000000 chipmunkdb_python_client-2.0.9/test/testsize.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-12-29 09:52:01.000000 chipmunkdb_python_client-2.0.9/test/testsuperlarge.py
```

### Comparing `chipmunkdb_python_client-2.0.8/PKG-INFO` & `chipmunkdb_python_client-2.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: chipmunkdb_python_client
-Version: 2.0.8
+Version: 2.0.9
 Summary: Read and Write Dataframes and Data to a chipmunkdb
 Home-page: https://gitlab.com/coindeck/chipmunkdb-python-client
 Author: coindeck
 Author-email: donnercody86@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
+Requires-Dist: sqlalchemy
 Requires-Dist: pandas
 Requires-Dist: influxdb
 Requires-Dist: importlib_resources
 Requires-Dist: typing
 
 
 # chipmunkdb :chipmunk: python-client
```

### Comparing `chipmunkdb_python_client-2.0.8/chipmunkdb/ChipmunkConnection.py` & `chipmunkdb_python_client-2.0.9/chipmunkdb/ChipmunkConnection.py`

 * *Files identical despite different names*

### Comparing `chipmunkdb_python_client-2.0.8/chipmunkdb/ChipmunkDb.py` & `chipmunkdb_python_client-2.0.9/chipmunkdb/ChipmunkDb.py`

 * *Files identical despite different names*

### Comparing `chipmunkdb_python_client-2.0.8/chipmunkdb/ChipmunkDialect.py` & `chipmunkdb_python_client-2.0.9/chipmunkdb/ChipmunkDialect.py`

 * *Files identical despite different names*

### Comparing `chipmunkdb_python_client-2.0.8/chipmunkdb_python_client.egg-info/PKG-INFO` & `chipmunkdb_python_client-2.0.9/chipmunkdb_python_client.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: chipmunkdb_python_client
-Version: 2.0.8
+Version: 2.0.9
 Summary: Read and Write Dataframes and Data to a chipmunkdb
 Home-page: https://gitlab.com/coindeck/chipmunkdb-python-client
 Author: coindeck
 Author-email: donnercody86@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
+Requires-Dist: sqlalchemy
 Requires-Dist: pandas
 Requires-Dist: influxdb
 Requires-Dist: importlib_resources
 Requires-Dist: typing
 
 
 # chipmunkdb :chipmunk: python-client
```

### Comparing `chipmunkdb_python_client-2.0.8/chipmunkdb_python_client.egg-info/SOURCES.txt` & `chipmunkdb_python_client-2.0.9/chipmunkdb_python_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chipmunkdb_python_client-2.0.8/setup.py` & `chipmunkdb_python_client-2.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # The text of the README file
 with open(os.path.join(HERE, "README_pip.md")) as fid:
     README = fid.read()
 
 # This call to setup() does all the work
 setup(
     name="chipmunkdb_python_client",
-    version="2.0.8",
+    version="2.0.9",
     description="Read and Write Dataframes and Data to a chipmunkdb",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/coindeck/chipmunkdb-python-client",
     author="coindeck",
     author_email="donnercody86@gmail.com",
     license="MIT",
@@ -26,11 +26,15 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
     ],
     packages=["chipmunkdb"],
     include_package_data=True,
     install_requires=[
-        "requests", "pandas", "influxdb", "importlib_resources", "typing"
+        "requests",  "sqlalchemy", "pandas", "influxdb", "importlib_resources", "typing"
     ],
-    entry_points={"console_scripts": ["chipmunkdb_python_client=chipmunkdb.ChipmunkDb:main"]},
+    entry_points={
+          'sqlalchemy.dialects': [
+              'chipmunkdb = chipmunkdb:ChipmunkDialect'
+          ]
+      }
 )
```

### Comparing `chipmunkdb_python_client-2.0.8/test/test.py` & `chipmunkdb_python_client-2.0.9/test/test.py`

 * *Files identical despite different names*

### Comparing `chipmunkdb_python_client-2.0.8/test/testDomain.py` & `chipmunkdb_python_client-2.0.9/test/testDomain.py`

 * *Files identical despite different names*

### Comparing `chipmunkdb_python_client-2.0.8/test/testStorage.py` & `chipmunkdb_python_client-2.0.9/test/testStorage.py`

 * *Files identical despite different names*

### Comparing `chipmunkdb_python_client-2.0.8/test/testduck_multiindex.py` & `chipmunkdb_python_client-2.0.9/test/testduck_multiindex.py`

 * *Files identical despite different names*

### Comparing `chipmunkdb_python_client-2.0.8/test/testsuperlarge.py` & `chipmunkdb_python_client-2.0.9/test/testsuperlarge.py`

 * *Files identical despite different names*

