# Comparing `tmp/movoid_threading-1.0.1.tar.gz` & `tmp/movoid_threading-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_threading-1.0.1.tar", last modified: Thu Apr 11 15:53:21 2024, max compression
+gzip compressed data, was "movoid_threading-1.0.2.tar", last modified: Sun Apr 14 08:14:19 2024, max compression
```

## Comparing `movoid_threading-1.0.1.tar` & `movoid_threading-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 15:53:21.064358 movoid_threading-1.0.1/
--rw-rw-rw-   0        0        0       14 2024-04-11 15:52:26.000000 movoid_threading-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      214 2024-04-11 15:53:21.062339 movoid_threading-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_threading-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 15:53:21.049529 movoid_threading-1.0.1/movoid_threading/
--rw-rw-rw-   0        0        0      278 2024-04-11 15:47:15.000000 movoid_threading-1.0.1/movoid_threading/__init__.py
--rw-rw-rw-   0        0        0     6634 2024-04-11 15:47:15.000000 movoid_threading-1.0.1/movoid_threading/thread.py
-drwxrwxrwx   0        0        0        0 2024-04-11 15:53:21.056752 movoid_threading-1.0.1/movoid_threading.egg-info/
--rw-rw-rw-   0        0        0      214 2024-04-11 15:53:21.000000 movoid_threading-1.0.1/movoid_threading.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-11 15:53:21.000000 movoid_threading-1.0.1/movoid_threading.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 15:53:21.000000 movoid_threading-1.0.1/movoid_threading.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-11 15:53:21.000000 movoid_threading-1.0.1/movoid_threading.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 15:53:21.064358 movoid_threading-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      463 2024-04-11 15:53:17.000000 movoid_threading-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 08:14:19.172645 movoid_threading-1.0.2/
+-rw-rw-rw-   0        0        0       14 2024-04-11 15:52:26.000000 movoid_threading-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      246 2024-04-14 08:14:19.171629 movoid_threading-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_threading-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 08:14:19.161785 movoid_threading-1.0.2/movoid_threading/
+-rw-rw-rw-   0        0        0      279 2024-04-13 08:34:36.000000 movoid_threading-1.0.2/movoid_threading/__init__.py
+-rw-rw-rw-   0        0        0     5847 2024-04-14 08:13:10.000000 movoid_threading-1.0.2/movoid_threading/thread.py
+drwxrwxrwx   0        0        0        0 2024-04-14 08:14:19.170591 movoid_threading-1.0.2/movoid_threading.egg-info/
+-rw-rw-rw-   0        0        0      246 2024-04-14 08:14:19.000000 movoid_threading-1.0.2/movoid_threading.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2024-04-14 08:14:19.000000 movoid_threading-1.0.2/movoid_threading.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 08:14:19.000000 movoid_threading-1.0.2/movoid_threading.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-14 08:14:19.000000 movoid_threading-1.0.2/movoid_threading.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-14 08:14:19.000000 movoid_threading-1.0.2/movoid_threading.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 08:14:19.172645 movoid_threading-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      480 2024-04-14 08:14:00.000000 movoid_threading-1.0.2/setup.py
```

### Comparing `movoid_threading-1.0.1/movoid_threading/thread.py` & `movoid_threading-1.0.2/movoid_threading/thread.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,48 +7,24 @@
 # Description   : 
 """
 import ctypes
 import threading
 import time
 from typing import Union, Dict
 
-
-class ThreadFunction:
-    def __init__(self, func=None, args=None, kwargs=None):
-        self._func = None
-        self._args = None
-        self._kwargs = None
-        if isinstance(func, (list, tuple)):
-            self.init(*func)
-        elif isinstance(func, dict):
-            self.init(**func)
-        elif isinstance(func, ThreadFunction):
-            self.init(func._func, func._args, func._kwargs)
-        else:
-            self.init(func, args, kwargs)
-
-    def init(self, func=None, args=None, kwargs=None):
-        self._func = func
-        self._args = args if args else ()
-        self._kwargs = kwargs if kwargs else {}
-
-    def __call__(self):
-        if self._func:
-            return self._func(*self._args, **self._kwargs)
-        else:
-            return None
+from movoid_function import Function
 
 
 class Thread:
     def __init__(self, target, name: str, args: Union[list, tuple] = None, kwargs: dict = None, loop: int = 1, init=None, end=None, *, start: bool = True, daemon: bool = False, thread_dict: dict):
-        self._target = ThreadFunction(target, args, kwargs)
+        self._target = Function(target, args, kwargs)
         self._name: str = str(name)
         self._loop: int = int(loop)
-        self._init = ThreadFunction(init)
-        self._end = ThreadFunction(end)
+        self._init = Function(init)
+        self._end = Function(end)
         self._daemon: bool = bool(daemon)
         self._thread_dict: dict = thread_dict
 
         self._ident = None
         self._start: bool = False
         self._pause: bool = False
         self._stop: bool = False
```

