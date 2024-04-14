# Comparing `tmp/librecell-common-0.0.8.tar.gz` & `tmp/librecell-common-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/librecell-common-0.0.8.tar", last modified: Wed Dec 30 17:35:42 2020, max compression
+gzip compressed data, was "dist/librecell-common-0.0.9.tar", last modified: Wed Dec 30 17:45:38 2020, max compression
```

## Comparing `librecell-common-0.0.8.tar` & `librecell-common-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:35:42.000000 librecell-common-0.0.8/
--rw-r--r--   0 kramert   (1000) kramert   (1000)      736 2020-12-30 17:35:42.000000 librecell-common-0.0.8/PKG-INFO
--rw-r--r--   0 kramert   (1000) kramert   (1000)       97 2019-10-05 16:43:05.000000 librecell-common-0.0.8/README.md
-drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:35:42.000000 librecell-common-0.0.8/lccommon/
--rw-r--r--   0 kramert   (1000) kramert   (1000)       17 2019-10-05 16:43:05.000000 librecell-common-0.0.8/lccommon/__init__.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     6721 2020-12-30 16:48:52.000000 librecell-common-0.0.8/lccommon/net_util.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     7495 2020-04-23 08:46:45.000000 librecell-common-0.0.8/lccommon/net_util_BACKUP_4.py
--rw-------   0 kramert   (1000) kramert   (1000)     5366 2020-04-23 08:46:53.000000 librecell-common-0.0.8/lccommon/net_util_BASE_4.py
--rw-------   0 kramert   (1000) kramert   (1000)     5365 2020-04-23 08:46:53.000000 librecell-common-0.0.8/lccommon/net_util_LOCAL_4.py
--rw-------   0 kramert   (1000) kramert   (1000)     6615 2020-04-23 08:46:53.000000 librecell-common-0.0.8/lccommon/net_util_REMOTE_4.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     5767 2019-10-05 16:43:05.000000 librecell-common-0.0.8/lccommon/spice_parser.py
-drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:35:42.000000 librecell-common-0.0.8/librecell_common.egg-info/
--rw-r--r--   0 kramert   (1000) kramert   (1000)      736 2020-12-30 17:35:42.000000 librecell-common-0.0.8/librecell_common.egg-info/PKG-INFO
--rw-r--r--   0 kramert   (1000) kramert   (1000)      440 2020-12-30 17:35:42.000000 librecell-common-0.0.8/librecell_common.egg-info/SOURCES.txt
--rw-r--r--   0 kramert   (1000) kramert   (1000)        1 2020-12-30 17:35:42.000000 librecell-common-0.0.8/librecell_common.egg-info/dependency_links.txt
--rw-r--r--   0 kramert   (1000) kramert   (1000)        1 2019-10-11 19:52:12.000000 librecell-common-0.0.8/librecell_common.egg-info/not-zip-safe
--rw-r--r--   0 kramert   (1000) kramert   (1000)       29 2020-12-30 17:35:42.000000 librecell-common-0.0.8/librecell_common.egg-info/requires.txt
--rw-r--r--   0 kramert   (1000) kramert   (1000)        9 2020-12-30 17:35:42.000000 librecell-common-0.0.8/librecell_common.egg-info/top_level.txt
--rw-r--r--   0 kramert   (1000) kramert   (1000)       38 2020-12-30 17:35:42.000000 librecell-common-0.0.8/setup.cfg
--rw-r--r--   0 kramert   (1000) kramert   (1000)     1001 2020-12-30 17:33:04.000000 librecell-common-0.0.8/setup.py
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:45:38.000000 librecell-common-0.0.9/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      736 2020-12-30 17:45:38.000000 librecell-common-0.0.9/PKG-INFO
+-rw-r--r--   0 kramert   (1000) kramert   (1000)       97 2019-10-05 16:43:05.000000 librecell-common-0.0.9/README.md
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:45:38.000000 librecell-common-0.0.9/lccommon/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)       17 2019-10-05 16:43:05.000000 librecell-common-0.0.9/lccommon/__init__.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     6721 2020-12-30 16:48:52.000000 librecell-common-0.0.9/lccommon/net_util.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     7495 2020-04-23 08:46:45.000000 librecell-common-0.0.9/lccommon/net_util_BACKUP_4.py
+-rw-------   0 kramert   (1000) kramert   (1000)     5366 2020-04-23 08:46:53.000000 librecell-common-0.0.9/lccommon/net_util_BASE_4.py
+-rw-------   0 kramert   (1000) kramert   (1000)     5365 2020-04-23 08:46:53.000000 librecell-common-0.0.9/lccommon/net_util_LOCAL_4.py
+-rw-------   0 kramert   (1000) kramert   (1000)     6615 2020-04-23 08:46:53.000000 librecell-common-0.0.9/lccommon/net_util_REMOTE_4.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     5767 2019-10-05 16:43:05.000000 librecell-common-0.0.9/lccommon/spice_parser.py
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:45:38.000000 librecell-common-0.0.9/librecell_common.egg-info/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      736 2020-12-30 17:45:38.000000 librecell-common-0.0.9/librecell_common.egg-info/PKG-INFO
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      440 2020-12-30 17:45:38.000000 librecell-common-0.0.9/librecell_common.egg-info/SOURCES.txt
+-rw-r--r--   0 kramert   (1000) kramert   (1000)        1 2020-12-30 17:45:38.000000 librecell-common-0.0.9/librecell_common.egg-info/dependency_links.txt
+-rw-r--r--   0 kramert   (1000) kramert   (1000)        1 2019-10-11 19:52:12.000000 librecell-common-0.0.9/librecell_common.egg-info/not-zip-safe
+-rw-r--r--   0 kramert   (1000) kramert   (1000)       29 2020-12-30 17:45:38.000000 librecell-common-0.0.9/librecell_common.egg-info/requires.txt
+-rw-r--r--   0 kramert   (1000) kramert   (1000)        9 2020-12-30 17:45:38.000000 librecell-common-0.0.9/librecell_common.egg-info/top_level.txt
+-rw-r--r--   0 kramert   (1000) kramert   (1000)       38 2020-12-30 17:45:38.000000 librecell-common-0.0.9/setup.cfg
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     1001 2020-12-30 17:44:21.000000 librecell-common-0.0.9/setup.py
```

### Comparing `librecell-common-0.0.8/PKG-INFO` & `librecell-common-0.0.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: librecell-common
-Version: 0.0.8
+Version: 0.0.9
 Summary: Common utility functions for LibreCell suite.
 Home-page: https://codeberg.org/tok/librecell
 Author: T. Kramer
 Author-email: code@tkramer.ch
 License: GPLv3
 Description: # LibreCell - Common
         This project contains code that is used across different LibreCell projects.
```

### Comparing `librecell-common-0.0.8/lccommon/net_util.py` & `librecell-common-0.0.9/lccommon/net_util.py`

 * *Files identical despite different names*

### Comparing `librecell-common-0.0.8/lccommon/net_util_BACKUP_4.py` & `librecell-common-0.0.9/lccommon/net_util_BACKUP_4.py`

 * *Files identical despite different names*

### Comparing `librecell-common-0.0.8/lccommon/net_util_BASE_4.py` & `librecell-common-0.0.9/lccommon/net_util_BASE_4.py`

 * *Files identical despite different names*

### Comparing `librecell-common-0.0.8/lccommon/net_util_LOCAL_4.py` & `librecell-common-0.0.9/lccommon/net_util_LOCAL_4.py`

 * *Files identical despite different names*

### Comparing `librecell-common-0.0.8/lccommon/net_util_REMOTE_4.py` & `librecell-common-0.0.9/lccommon/net_util_REMOTE_4.py`

 * *Files identical despite different names*

### Comparing `librecell-common-0.0.8/lccommon/spice_parser.py` & `librecell-common-0.0.9/lccommon/spice_parser.py`

 * *Files identical despite different names*

### Comparing `librecell-common-0.0.8/librecell_common.egg-info/PKG-INFO` & `librecell-common-0.0.9/librecell_common.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: librecell-common
-Version: 0.0.8
+Version: 0.0.9
 Summary: Common utility functions for LibreCell suite.
 Home-page: https://codeberg.org/tok/librecell
 Author: T. Kramer
 Author-email: code@tkramer.ch
 License: GPLv3
 Description: # LibreCell - Common
         This project contains code that is used across different LibreCell projects.
```

### Comparing `librecell-common-0.0.8/setup.py` & `librecell-common-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
     with open("README.md", "r") as f:
         return f.read()
 
 
 setup(name='librecell-common',
-      version='0.0.8',
+      version='0.0.9',
       description='Common utility functions for LibreCell suite.',
       long_description=readme(),
       long_description_content_type="text/markdown",
       keywords='cmos cell vlsi asic',
       classifiers=[
           'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
           'Development Status :: 3 - Alpha',
```

