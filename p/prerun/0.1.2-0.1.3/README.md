# Comparing `tmp/prerun-0.1.2.tar.gz` & `tmp/prerun-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prerun-0.1.2.tar", last modified: Sun Apr 14 07:54:12 2024, max compression
+gzip compressed data, was "prerun-0.1.3.tar", last modified: Sun Apr 14 09:28:51 2024, max compression
```

## Comparing `prerun-0.1.2.tar` & `prerun-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:54:12.636061 prerun-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-14 07:54:07.000000 prerun-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-14 07:54:12.636061 prerun-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 07:54:07.000000 prerun-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-14 07:54:07.000000 prerun-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 07:54:12.636061 prerun-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:54:12.632061 prerun-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:54:12.632061 prerun-0.1.2/src/prerun/
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-14 07:54:07.000000 prerun-0.1.2/src/prerun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-14 07:54:07.000000 prerun-0.1.2/src/prerun/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:54:12.636061 prerun-0.1.2/src/prerun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-14 07:54:12.000000 prerun-0.1.2/src/prerun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-14 07:54:12.000000 prerun-0.1.2/src/prerun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 07:54:12.000000 prerun-0.1.2/src/prerun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-14 07:54:12.000000 prerun-0.1.2/src/prerun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-14 07:54:12.000000 prerun-0.1.2/src/prerun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 07:54:12.000000 prerun-0.1.2/src/prerun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:28:51.264696 prerun-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-14 09:28:46.000000 prerun-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-14 09:28:51.264696 prerun-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 09:28:46.000000 prerun-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-14 09:28:46.000000 prerun-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 09:28:51.264696 prerun-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:28:51.260696 prerun-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:28:51.264696 prerun-0.1.3/src/prerun/
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-04-14 09:28:46.000000 prerun-0.1.3/src/prerun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-14 09:28:46.000000 prerun-0.1.3/src/prerun/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:28:51.264696 prerun-0.1.3/src/prerun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-14 09:28:51.000000 prerun-0.1.3/src/prerun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-14 09:28:51.000000 prerun-0.1.3/src/prerun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 09:28:51.000000 prerun-0.1.3/src/prerun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-14 09:28:51.000000 prerun-0.1.3/src/prerun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-14 09:28:51.000000 prerun-0.1.3/src/prerun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 09:28:51.000000 prerun-0.1.3/src/prerun.egg-info/top_level.txt
```

### Comparing `prerun-0.1.2/LICENSE` & `prerun-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prerun-0.1.2/PKG-INFO` & `prerun-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prerun
-Version: 0.1.2
+Version: 0.1.3
 Summary: Prerun
 License: Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `prerun-0.1.2/pyproject.toml` & `prerun-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "prerun"
-version = "0.1.2"
+version = "0.1.3"
 description = "Prerun"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 keywords = ["development"]
 classifiers = [
   "Development Status :: 3 - Alpha",
```

### Comparing `prerun-0.1.2/src/prerun/__init__.py` & `prerun-0.1.3/src/prerun/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import multiprocessing
 import os
 import readline
 import runpy
 import shlex
 import signal
 import sys
 from multiprocessing import Pipe, Process
@@ -11,14 +12,15 @@
 
 def sigint_once_handler(signum, frame):
     signal.signal(signal.SIGINT, signal.SIG_IGN)
     return signal.default_int_handler(signum, frame)
 
 
 def run(stdio, preloader, conn):
+    multiprocessing.set_start_method(None, force=True)
     os.setpgid(0, 0)
     os.dup2(sys.stdin.fileno(), 0, inheritable=True)
     signal.signal(signal.SIGINT, signal.default_int_handler)
 
     runpy.run_path(preloader)
 
     runner = conn.recv()
@@ -108,14 +110,16 @@
                 except ProcessLookupError:
                     pass
                 proc.kill()
         os._exit(0)
 
 
 def main():
+    multiprocessing.set_start_method("fork")
+
     signal.signal(signal.SIGINT, signal.SIG_IGN)
     stdio = [os.dup(0)]
     os.set_inheritable(stdio[0], True)
 
     p = Process(target=real_main, args=(stdio,))
     p.start()
     p.join()
```

### Comparing `prerun-0.1.2/src/prerun.egg-info/PKG-INFO` & `prerun-0.1.3/src/prerun.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prerun
-Version: 0.1.2
+Version: 0.1.3
 Summary: Prerun
 License: Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

