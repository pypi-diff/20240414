# Comparing `tmp/gbnf-0.0.1.tar.gz` & `tmp/gbnf-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gbnf-0.0.1.tar", last modified: Sun Apr 14 10:04:04 2024, max compression
+gzip compressed data, was "gbnf-0.0.2.tar", last modified: Sun Apr 14 10:15:21 2024, max compression
```

## Comparing `gbnf-0.0.1.tar` & `gbnf-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 thekevinscott   (501) staff       (20)        0 2024-04-14 10:04:04.657349 gbnf-0.0.1/
--rw-r--r--   0 thekevinscott   (501) staff       (20)     1068 2024-04-14 10:02:45.000000 gbnf-0.0.1/LICENSE
--rw-r--r--   0 thekevinscott   (501) staff       (20)       55 2024-04-14 10:02:27.000000 gbnf-0.0.1/MANIFEST.in
--rw-r--r--   0 thekevinscott   (501) staff       (20)     3168 2024-04-14 10:04:04.657118 gbnf-0.0.1/PKG-INFO
--rw-r--r--   0 thekevinscott   (501) staff       (20)     2667 2024-04-14 10:02:45.000000 gbnf-0.0.1/README.md
-drwxr-xr-x   0 thekevinscott   (501) staff       (20)        0 2024-04-14 10:04:04.656249 gbnf-0.0.1/gbnf/
--rw-r--r--   0 thekevinscott   (501) staff       (20)       21 2024-04-14 09:58:10.000000 gbnf-0.0.1/gbnf/__init__.py
--rw-r--r--   0 thekevinscott   (501) staff       (20)       25 2024-04-14 09:58:10.000000 gbnf-0.0.1/gbnf/foo_test.py
-drwxr-xr-x   0 thekevinscott   (501) staff       (20)        0 2024-04-14 10:04:04.656922 gbnf-0.0.1/gbnf.egg-info/
--rw-r--r--   0 thekevinscott   (501) staff       (20)     3168 2024-04-14 10:04:04.000000 gbnf-0.0.1/gbnf.egg-info/PKG-INFO
--rw-r--r--   0 thekevinscott   (501) staff       (20)      190 2024-04-14 10:04:04.000000 gbnf-0.0.1/gbnf.egg-info/SOURCES.txt
--rw-r--r--   0 thekevinscott   (501) staff       (20)        1 2024-04-14 10:04:04.000000 gbnf-0.0.1/gbnf.egg-info/dependency_links.txt
--rw-r--r--   0 thekevinscott   (501) staff       (20)        5 2024-04-14 10:04:04.000000 gbnf-0.0.1/gbnf.egg-info/top_level.txt
--rw-r--r--   0 thekevinscott   (501) staff       (20)     1733 2024-04-14 09:58:10.000000 gbnf-0.0.1/pyproject.toml
--rw-r--r--   0 thekevinscott   (501) staff       (20)       38 2024-04-14 10:04:04.657390 gbnf-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:15:21.339844 gbnf-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-14 10:15:19.000000 gbnf-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-14 10:15:10.000000 gbnf-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-14 10:15:21.339844 gbnf-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-14 10:15:19.000000 gbnf-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:15:21.339844 gbnf-0.0.2/gbnf/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-14 10:15:10.000000 gbnf-0.0.2/gbnf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-14 10:15:10.000000 gbnf-0.0.2/gbnf/foo_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:15:21.339844 gbnf-0.0.2/gbnf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-14 10:15:21.000000 gbnf-0.0.2/gbnf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-14 10:15:21.000000 gbnf-0.0.2/gbnf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 10:15:21.000000 gbnf-0.0.2/gbnf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-14 10:15:21.000000 gbnf-0.0.2/gbnf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-14 10:15:10.000000 gbnf-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 10:15:21.339844 gbnf-0.0.2/setup.cfg
```

### Comparing `gbnf-0.0.1/LICENSE` & `gbnf-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gbnf-0.0.1/PKG-INFO` & `gbnf-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbnf
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for parsing GBNF grammars
 Author-email: Kevin Scott <kevin@gbnf.dev>
 Project-URL: Homepage, https://github.com/thekevinscott/gbnf
 Project-URL: Bug Tracker, https://github.com/thekevinscott/gbnf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gbnf-0.0.1/README.md` & `gbnf-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `gbnf-0.0.1/gbnf.egg-info/PKG-INFO` & `gbnf-0.0.2/gbnf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gbnf
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for parsing GBNF grammars
 Author-email: Kevin Scott <kevin@gbnf.dev>
 Project-URL: Homepage, https://github.com/thekevinscott/gbnf
 Project-URL: Bug Tracker, https://github.com/thekevinscott/gbnf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gbnf-0.0.1/pyproject.toml` & `gbnf-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gbnf"
-version = "0.0.1"
+version = "0.0.2"
 # Notes
 authors = [{ name = "Kevin Scott", email = "kevin@gbnf.dev" }]
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
 ]
 description = "A library for parsing GBNF grammars"
```

