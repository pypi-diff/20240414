# Comparing `tmp/prerun-0.1.0.tar.gz` & `tmp/prerun-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prerun-0.1.0.tar", last modified: Sun Apr 14 05:35:34 2024, max compression
+gzip compressed data, was "prerun-0.1.1.tar", last modified: Sun Apr 14 05:44:51 2024, max compression
```

## Comparing `prerun-0.1.0.tar` & `prerun-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:35:34.109922 prerun-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-14 05:35:24.000000 prerun-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-14 05:35:34.109922 prerun-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 05:35:24.000000 prerun-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-14 05:35:24.000000 prerun-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 05:35:34.109922 prerun-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:35:34.109922 prerun-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:35:34.109922 prerun-0.1.0/src/prerun/
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-04-14 05:35:24.000000 prerun-0.1.0/src/prerun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-14 05:35:24.000000 prerun-0.1.0/src/prerun/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:35:34.109922 prerun-0.1.0/src/prerun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-04-14 05:35:34.000000 prerun-0.1.0/src/prerun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-14 05:35:34.000000 prerun-0.1.0/src/prerun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 05:35:34.000000 prerun-0.1.0/src/prerun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-14 05:35:34.000000 prerun-0.1.0/src/prerun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 05:35:34.000000 prerun-0.1.0/src/prerun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:44:51.613665 prerun-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-14 05:44:46.000000 prerun-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-14 05:44:51.613665 prerun-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 05:44:46.000000 prerun-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-14 05:44:46.000000 prerun-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 05:44:51.613665 prerun-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:44:51.609665 prerun-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:44:51.609665 prerun-0.1.1/src/prerun/
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-04-14 05:44:46.000000 prerun-0.1.1/src/prerun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-14 05:44:46.000000 prerun-0.1.1/src/prerun/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:44:51.613665 prerun-0.1.1/src/prerun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-14 05:44:51.000000 prerun-0.1.1/src/prerun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-14 05:44:51.000000 prerun-0.1.1/src/prerun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 05:44:51.000000 prerun-0.1.1/src/prerun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-14 05:44:51.000000 prerun-0.1.1/src/prerun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-14 05:44:51.000000 prerun-0.1.1/src/prerun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 05:44:51.000000 prerun-0.1.1/src/prerun.egg-info/top_level.txt
```

### Comparing `prerun-0.1.0/LICENSE` & `prerun-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prerun-0.1.0/PKG-INFO` & `prerun-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prerun
-Version: 0.1.0
+Version: 0.1.1
 Summary: Prerun
 License: Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -26,9 +26,10 @@
 Keywords: development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: psutil>=5.9.0
 
 # Prerun
```

### Comparing `prerun-0.1.0/pyproject.toml` & `prerun-0.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "prerun"
-version = "0.1.0"
+version = "0.1.1"
 description = "Prerun"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["development"]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
 ]
-dependencies = []
+dependencies = [
+  "psutil>=5.9.0",
+]
 
 [project.urls]
 "Homepage" = "https://github.com/sfanxiang/prerun"
 
 [project.scripts]
 prerun = "prerun:main"
```

### Comparing `prerun-0.1.0/src/prerun/__init__.py` & `prerun-0.1.1/src/prerun/__init__.py`

 * *Files identical despite different names*

### Comparing `prerun-0.1.0/src/prerun.egg-info/PKG-INFO` & `prerun-0.1.1/src/prerun.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prerun
-Version: 0.1.0
+Version: 0.1.1
 Summary: Prerun
 License: Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
@@ -26,9 +26,10 @@
 Keywords: development
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: psutil>=5.9.0
 
 # Prerun
```

