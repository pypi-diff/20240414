# Comparing `tmp/prerun-0.1.3.tar.gz` & `tmp/prerun-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prerun-0.1.3.tar", last modified: Sun Apr 14 09:28:51 2024, max compression
+gzip compressed data, was "prerun-0.1.4.tar", last modified: Sun Apr 14 09:37:34 2024, max compression
```

## Comparing `prerun-0.1.3.tar` & `prerun-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:28:51.264696 prerun-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-14 09:28:46.000000 prerun-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-14 09:28:51.264696 prerun-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 09:28:46.000000 prerun-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-14 09:28:46.000000 prerun-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 09:28:51.264696 prerun-0.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:28:51.260696 prerun-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:28:51.264696 prerun-0.1.3/src/prerun/
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-14 09:28:46.000000 prerun-0.1.3/src/prerun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-14 09:28:46.000000 prerun-0.1.3/src/prerun/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:28:51.264696 prerun-0.1.3/src/prerun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-14 09:28:51.000000 prerun-0.1.3/src/prerun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-14 09:28:51.000000 prerun-0.1.3/src/prerun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 09:28:51.000000 prerun-0.1.3/src/prerun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-14 09:28:51.000000 prerun-0.1.3/src/prerun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-14 09:28:51.000000 prerun-0.1.3/src/prerun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 09:28:51.000000 prerun-0.1.3/src/prerun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:37:34.139468 prerun-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-14 09:37:23.000000 prerun-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-14 09:37:34.139468 prerun-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 09:37:23.000000 prerun-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-14 09:37:23.000000 prerun-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 09:37:34.139468 prerun-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:37:34.135468 prerun-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:37:34.135468 prerun-0.1.4/src/prerun/
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-04-14 09:37:23.000000 prerun-0.1.4/src/prerun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-14 09:37:23.000000 prerun-0.1.4/src/prerun/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:37:34.139468 prerun-0.1.4/src/prerun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-14 09:37:34.000000 prerun-0.1.4/src/prerun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-14 09:37:34.000000 prerun-0.1.4/src/prerun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 09:37:34.000000 prerun-0.1.4/src/prerun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-14 09:37:34.000000 prerun-0.1.4/src/prerun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-14 09:37:34.000000 prerun-0.1.4/src/prerun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 09:37:34.000000 prerun-0.1.4/src/prerun.egg-info/top_level.txt
```

### Comparing `prerun-0.1.3/LICENSE` & `prerun-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prerun-0.1.3/PKG-INFO` & `prerun-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prerun
-Version: 0.1.3
+Version: 0.1.4
 Summary: Prerun
 License: Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `prerun-0.1.3/pyproject.toml` & `prerun-0.1.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "prerun"
-version = "0.1.3"
+version = "0.1.4"
 description = "Prerun"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["development"]
 classifiers = [
   "Development Status :: 3 - Alpha",
```

### Comparing `prerun-0.1.3/src/prerun/__init__.py` & `prerun-0.1.4/src/prerun/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 def run(stdio, preloader, conn):
     multiprocessing.set_start_method(None, force=True)
     os.setpgid(0, 0)
     os.dup2(sys.stdin.fileno(), 0, inheritable=True)
     signal.signal(signal.SIGINT, signal.default_int_handler)
 
+    sys.argv = [preloader]
     runpy.run_path(preloader)
 
     runner = conn.recv()
 
     os.dup2(stdio[0], 0, inheritable=True)
     os.close(stdio[0])
     sys.stdin.close()
```

### Comparing `prerun-0.1.3/src/prerun.egg-info/PKG-INFO` & `prerun-0.1.4/src/prerun.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prerun
-Version: 0.1.3
+Version: 0.1.4
 Summary: Prerun
 License: Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

