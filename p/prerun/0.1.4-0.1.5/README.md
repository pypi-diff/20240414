# Comparing `tmp/prerun-0.1.4.tar.gz` & `tmp/prerun-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prerun-0.1.4.tar", last modified: Sun Apr 14 09:37:34 2024, max compression
+gzip compressed data, was "prerun-0.1.5.tar", last modified: Sun Apr 14 09:52:29 2024, max compression
```

## Comparing `prerun-0.1.4.tar` & `prerun-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:37:34.139468 prerun-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-14 09:37:23.000000 prerun-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-14 09:37:34.139468 prerun-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 09:37:23.000000 prerun-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-14 09:37:23.000000 prerun-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 09:37:34.139468 prerun-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:37:34.135468 prerun-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:37:34.135468 prerun-0.1.4/src/prerun/
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-04-14 09:37:23.000000 prerun-0.1.4/src/prerun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-14 09:37:23.000000 prerun-0.1.4/src/prerun/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:37:34.139468 prerun-0.1.4/src/prerun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-14 09:37:34.000000 prerun-0.1.4/src/prerun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-14 09:37:34.000000 prerun-0.1.4/src/prerun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 09:37:34.000000 prerun-0.1.4/src/prerun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-14 09:37:34.000000 prerun-0.1.4/src/prerun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-14 09:37:34.000000 prerun-0.1.4/src/prerun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 09:37:34.000000 prerun-0.1.4/src/prerun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:52:29.673138 prerun-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-14 09:52:24.000000 prerun-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-14 09:52:29.673138 prerun-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 09:52:24.000000 prerun-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-14 09:52:24.000000 prerun-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 09:52:29.673138 prerun-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:52:29.669138 prerun-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:52:29.669138 prerun-0.1.5/src/prerun/
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-14 09:52:24.000000 prerun-0.1.5/src/prerun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-14 09:52:24.000000 prerun-0.1.5/src/prerun/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:52:29.669138 prerun-0.1.5/src/prerun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-14 09:52:29.000000 prerun-0.1.5/src/prerun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-14 09:52:29.000000 prerun-0.1.5/src/prerun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 09:52:29.000000 prerun-0.1.5/src/prerun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-14 09:52:29.000000 prerun-0.1.5/src/prerun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-14 09:52:29.000000 prerun-0.1.5/src/prerun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 09:52:29.000000 prerun-0.1.5/src/prerun.egg-info/top_level.txt
```

### Comparing `prerun-0.1.4/LICENSE` & `prerun-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `prerun-0.1.4/PKG-INFO` & `prerun-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prerun
-Version: 0.1.4
+Version: 0.1.5
 Summary: Prerun
 License: Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `prerun-0.1.4/pyproject.toml` & `prerun-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "prerun"
-version = "0.1.4"
+version = "0.1.5"
 description = "Prerun"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["development"]
 classifiers = [
   "Development Status :: 3 - Alpha",
```

### Comparing `prerun-0.1.4/src/prerun/__init__.py` & `prerun-0.1.5/src/prerun/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,15 +86,20 @@
             try:
                 signal.signal(signal.SIGINT, sigint_once_handler)
                 conn.send(runner)
                 proc.join()
                 signal.signal(signal.SIGINT, signal.SIG_IGN)
             except KeyboardInterrupt:
                 if proc.exitcode is None:
-                    proc.join(0.5)
+                    try:
+                        signal.signal(signal.SIGINT, sigint_once_handler)
+                        proc.join()
+                        signal.signal(signal.SIGINT, signal.SIG_IGN)
+                    except KeyboardInterrupt:
+                        pass
 
             if proc.exitcode is None:
                 parent = psutil.Process(proc.pid)
                 for child in parent.children(recursive=True):
                     child.kill()
                 parent.kill()
```

### Comparing `prerun-0.1.4/src/prerun.egg-info/PKG-INFO` & `prerun-0.1.5/src/prerun.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prerun
-Version: 0.1.4
+Version: 0.1.5
 Summary: Prerun
 License: Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

