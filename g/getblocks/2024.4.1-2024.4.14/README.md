# Comparing `tmp/getblocks-2024.4.1.tar.gz` & `tmp/getblocks-2024.4.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getblocks-2024.4.1.tar", last modified: Wed Apr  3 23:45:56 2024, max compression
+gzip compressed data, was "getblocks-2024.4.14.tar", last modified: Sun Apr 14 13:07:12 2024, max compression
```

## Comparing `getblocks-2024.4.1.tar` & `getblocks-2024.4.14.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:45:56.589134 getblocks-2024.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 23:45:52.000000 getblocks-2024.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-03 23:45:56.589134 getblocks-2024.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-03 23:45:52.000000 getblocks-2024.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:45:56.589134 getblocks-2024.4.1/getblocks/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 23:45:52.000000 getblocks-2024.4.1/getblocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-03 23:45:52.000000 getblocks-2024.4.1/getblocks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-04-03 23:45:52.000000 getblocks-2024.4.1/getblocks/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 23:45:56.589134 getblocks-2024.4.1/getblocks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-03 23:45:56.000000 getblocks-2024.4.1/getblocks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-03 23:45:56.000000 getblocks-2024.4.1/getblocks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:45:56.000000 getblocks-2024.4.1/getblocks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 23:45:56.000000 getblocks-2024.4.1/getblocks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 23:45:56.000000 getblocks-2024.4.1/getblocks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 23:45:56.000000 getblocks-2024.4.1/getblocks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 23:45:56.000000 getblocks-2024.4.1/getblocks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 23:45:56.589134 getblocks-2024.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-03 23:45:52.000000 getblocks-2024.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:07:12.687512 getblocks-2024.4.14/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-14 13:07:08.000000 getblocks-2024.4.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-14 13:07:12.687512 getblocks-2024.4.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-14 13:07:08.000000 getblocks-2024.4.14/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:07:12.683512 getblocks-2024.4.14/getblocks/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-14 13:07:08.000000 getblocks-2024.4.14/getblocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-14 13:07:08.000000 getblocks-2024.4.14/getblocks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8566 2024-04-14 13:07:08.000000 getblocks-2024.4.14/getblocks/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:07:12.687512 getblocks-2024.4.14/getblocks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-14 13:07:12.000000 getblocks-2024.4.14/getblocks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-14 13:07:12.000000 getblocks-2024.4.14/getblocks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 13:07:12.000000 getblocks-2024.4.14/getblocks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-14 13:07:12.000000 getblocks-2024.4.14/getblocks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 13:07:12.000000 getblocks-2024.4.14/getblocks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-14 13:07:12.000000 getblocks-2024.4.14/getblocks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 13:07:12.000000 getblocks-2024.4.14/getblocks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 13:07:12.687512 getblocks-2024.4.14/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-14 13:07:08.000000 getblocks-2024.4.14/setup.py
```

### Comparing `getblocks-2024.4.1/LICENSE` & `getblocks-2024.4.14/LICENSE`

 * *Files identical despite different names*

### Comparing `getblocks-2024.4.1/PKG-INFO` & `getblocks-2024.4.14/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getblocks
-Version: 2024.4.1
+Version: 2024.4.14
 Summary: Down to the smallest sector detail!
 Home-page: https://github.com/jblukach/getblocks
 Author: John Lukach
 Author-email: hello@lukach.io
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -87,7 +87,11 @@
 ```
 
 ### DEVELOPMENT
 
 ```
 python setup.py install --user
 ```
+
+### META INFORMATION
+
+![Meta Information](images/metainfo.png)
```

### Comparing `getblocks-2024.4.1/README.md` & `getblocks-2024.4.14/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -72,8 +72,12 @@
 pip install getblocks
 ```
 
 ### DEVELOPMENT
 
 ```
 python setup.py install --user
-```
+```
+
+### META INFORMATION
+
+![Meta Information](images/metainfo.png)
```

### Comparing `getblocks-2024.4.1/getblocks/cli.py` & `getblocks-2024.4.14/getblocks/cli.py`

 * *Files identical despite different names*

### Comparing `getblocks-2024.4.1/getblocks.egg-info/PKG-INFO` & `getblocks-2024.4.14/getblocks.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: getblocks
-Version: 2024.4.1
+Version: 2024.4.14
 Summary: Down to the smallest sector detail!
 Home-page: https://github.com/jblukach/getblocks
 Author: John Lukach
 Author-email: hello@lukach.io
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -87,7 +87,11 @@
 ```
 
 ### DEVELOPMENT
 
 ```
 python setup.py install --user
 ```
+
+### META INFORMATION
+
+![Meta Information](images/metainfo.png)
```

### Comparing `getblocks-2024.4.1/setup.py` & `getblocks-2024.4.14/setup.py`

 * *Files identical despite different names*

