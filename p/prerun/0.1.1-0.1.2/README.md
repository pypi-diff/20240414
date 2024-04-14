# Comparing `tmp/prerun-0.1.1.tar.gz` & `tmp/prerun-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prerun-0.1.1.tar", last modified: Sun Apr 14 05:44:51 2024, max compression
+gzip compressed data, was "prerun-0.1.2.tar", last modified: Sun Apr 14 07:54:12 2024, max compression
```

## Comparing `prerun-0.1.1.tar` & `prerun-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:44:51.613665 prerun-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-14 05:44:46.000000 prerun-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-14 05:44:51.613665 prerun-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 05:44:46.000000 prerun-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-14 05:44:46.000000 prerun-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 05:44:51.613665 prerun-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:44:51.609665 prerun-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:44:51.609665 prerun-0.1.1/src/prerun/
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-04-14 05:44:46.000000 prerun-0.1.1/src/prerun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-14 05:44:46.000000 prerun-0.1.1/src/prerun/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:44:51.613665 prerun-0.1.1/src/prerun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-14 05:44:51.000000 prerun-0.1.1/src/prerun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-14 05:44:51.000000 prerun-0.1.1/src/prerun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 05:44:51.000000 prerun-0.1.1/src/prerun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-14 05:44:51.000000 prerun-0.1.1/src/prerun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-14 05:44:51.000000 prerun-0.1.1/src/prerun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 05:44:51.000000 prerun-0.1.1/src/prerun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:54:12.636061 prerun-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-14 07:54:07.000000 prerun-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-14 07:54:12.636061 prerun-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 07:54:07.000000 prerun-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-14 07:54:07.000000 prerun-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 07:54:12.636061 prerun-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:54:12.632061 prerun-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:54:12.632061 prerun-0.1.2/src/prerun/
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-14 07:54:07.000000 prerun-0.1.2/src/prerun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-14 07:54:07.000000 prerun-0.1.2/src/prerun/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:54:12.636061 prerun-0.1.2/src/prerun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-14 07:54:12.000000 prerun-0.1.2/src/prerun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-14 07:54:12.000000 prerun-0.1.2/src/prerun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 07:54:12.000000 prerun-0.1.2/src/prerun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-14 07:54:12.000000 prerun-0.1.2/src/prerun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-14 07:54:12.000000 prerun-0.1.2/src/prerun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 07:54:12.000000 prerun-0.1.2/src/prerun.egg-info/top_level.txt
```

### Comparing `prerun-0.1.1/LICENSE` & `prerun-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prerun-0.1.1/PKG-INFO` & `prerun-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prerun
-Version: 0.1.1
+Version: 0.1.2
 Summary: Prerun
 License: Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `prerun-0.1.1/src/prerun/__init__.py` & `prerun-0.1.2/src/prerun/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,17 +5,23 @@
 import signal
 import sys
 from multiprocessing import Pipe, Process
 
 import psutil
 
 
+def sigint_once_handler(signum, frame):
+    signal.signal(signal.SIGINT, signal.SIG_IGN)
+    return signal.default_int_handler(signum, frame)
+
+
 def run(stdio, preloader, conn):
     os.setpgid(0, 0)
     os.dup2(sys.stdin.fileno(), 0, inheritable=True)
+    signal.signal(signal.SIGINT, signal.default_int_handler)
 
     runpy.run_path(preloader)
 
     runner = conn.recv()
 
     os.dup2(stdio[0], 0, inheritable=True)
     os.close(stdio[0])
@@ -30,14 +36,16 @@
     c1, c2 = Pipe(duplex=True)
     p = Process(target=run, args=(stdio, preloader, c2))
     p.start()
     return p, c1
 
 
 def real_main(stdio):
+    signal.signal(signal.SIGINT, signal.SIG_IGN)
+
     os.dup2(stdio[0], 0, inheritable=True)
     sys.stdin.close()
     sys.stdin = open(0, closefd=False)
 
     preloader, num_proc, runner = sys.argv[1], int(sys.argv[2]), sys.argv[3:]
 
     processes = []
@@ -47,38 +55,42 @@
     if runner:
         readline.add_history(shlex.join(runner))
 
     try:
         while True:
             while not runner:
                 try:
-                    s = input("Next task > ")
-                    runner = shlex.split(s)
-                except ValueError as e:
-                    sys.stderr.write("Error: " + str(e) + "\n")
-                    continue
-                except EOFError:
-                    return
+                    signal.signal(signal.SIGINT, sigint_once_handler)
+                    try:
+                        s = input("Next task > ")
+                    except EOFError:
+                        signal.signal(signal.SIGINT, signal.SIG_IGN)
+                        return
+                    signal.signal(signal.SIGINT, signal.SIG_IGN)
+                    try:
+                        runner = shlex.split(s)
+                    except ValueError as e:
+                        sys.stderr.write("Error: " + str(e) + "\n")
+                        continue
                 except KeyboardInterrupt:
                     print("^C")
-                    pass
 
             proc, conn = processes[0]
             processes.append(launch_process(stdio, preloader))
 
+            if proc.exitcode is None:
+                os.setpgid(proc.pid, os.getpgid(0))
+
             try:
+                signal.signal(signal.SIGINT, sigint_once_handler)
                 conn.send(runner)
                 proc.join()
+                signal.signal(signal.SIGINT, signal.SIG_IGN)
             except KeyboardInterrupt:
                 if proc.exitcode is None:
-                    parent = psutil.Process(proc.pid)
-                    for child in parent.children(recursive=True):
-                        child.send_signal(signal.SIGINT)
-                    parent.send_signal(signal.SIGINT)
-
                     proc.join(0.5)
 
             if proc.exitcode is None:
                 parent = psutil.Process(proc.pid)
                 for child in parent.children(recursive=True):
                     child.kill()
                 parent.kill()
@@ -96,19 +108,15 @@
                 except ProcessLookupError:
                     pass
                 proc.kill()
         os._exit(0)
 
 
 def main():
+    signal.signal(signal.SIGINT, signal.SIG_IGN)
     stdio = [os.dup(0)]
     os.set_inheritable(stdio[0], True)
 
     p = Process(target=real_main, args=(stdio,))
     p.start()
-    while True:
-        try:
-            p.join()
-            break
-        except KeyboardInterrupt:
-            pass
+    p.join()
     p.close()
```

### Comparing `prerun-0.1.1/src/prerun.egg-info/PKG-INFO` & `prerun-0.1.2/src/prerun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prerun
-Version: 0.1.1
+Version: 0.1.2
 Summary: Prerun
 License: Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

