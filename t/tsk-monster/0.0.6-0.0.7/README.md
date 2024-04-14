# Comparing `tmp/tsk_monster-0.0.6.tar.gz` & `tmp/tsk_monster-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsk_monster-0.0.6.tar", max compression
+gzip compressed data, was "tsk_monster-0.0.7.tar", max compression
```

## Comparing `tsk_monster-0.0.6.tar` & `tsk_monster-0.0.7.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      363 2024-04-13 17:57:20.490880 tsk_monster-0.0.6/README.md
--rw-r--r--   0        0        0      583 2024-04-13 17:57:32.498649 tsk_monster-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3424 2024-04-13 17:23:43.548774 tsk_monster-0.0.6/tsk_monster/__init__.py
--rw-r--r--   0        0        0      801 1970-01-01 00:00:00.000000 tsk_monster-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      363 2024-04-13 17:57:20.490880 tsk_monster-0.0.7/README.md
+-rw-r--r--   0        0        0      583 2024-04-13 17:57:55.078214 tsk_monster-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3424 2024-04-13 17:23:43.548774 tsk_monster-0.0.7/tsk_monster/__init__.py
+-rw-r--r--   0        0        0      801 1970-01-01 00:00:00.000000 tsk_monster-0.0.7/PKG-INFO
```

### Comparing `tsk_monster-0.0.6/pyproject.toml` & `tsk_monster-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tsk-monster"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 authors = ["Gilad Kutiel <giladk@mobileye.com>"]
 readme = "README.md"
 
 [tool.poetry.urls]
 Homepage = "https://tsk.monster"
 Documentation = "https://tsk.monster"
```

### Comparing `tsk_monster-0.0.6/tsk_monster/__init__.py` & `tsk_monster-0.0.7/tsk_monster/__init__.py`

 * *Files identical despite different names*

### Comparing `tsk_monster-0.0.6/PKG-INFO` & `tsk_monster-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsk-monster
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Author: Gilad Kutiel
 Author-email: giladk@mobileye.com
 Requires-Python: ==3.10.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Project-URL: Documentation, https://tsk.monster
```

