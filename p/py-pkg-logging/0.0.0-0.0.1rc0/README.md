# Comparing `tmp/py_pkg_logging-0.0.0.tar.gz` & `tmp/py_pkg_logging-0.0.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_pkg_logging-0.0.0.tar", last modified: Wed Feb 21 22:00:33 2024, max compression
+gzip compressed data, was "py_pkg_logging-0.0.1rc0.tar", last modified: Sun Apr 14 18:14:27 2024, max compression
```

## Comparing `py_pkg_logging-0.0.0.tar` & `py_pkg_logging-0.0.1rc0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:00:33.350411 py_pkg_logging-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-02-21 22:00:33.350411 py_pkg_logging-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-21 22:00:21.000000 py_pkg_logging-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:00:33.350411 py_pkg_logging-0.0.0/py_pkg_logging/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-21 22:00:21.000000 py_pkg_logging-0.0.0/py_pkg_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-21 22:00:21.000000 py_pkg_logging-0.0.0/py_pkg_logging/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-02-21 22:00:21.000000 py_pkg_logging-0.0.0/py_pkg_logging/_log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-02-21 22:00:21.000000 py_pkg_logging-0.0.0/py_pkg_logging/_log_function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 22:00:33.350411 py_pkg_logging-0.0.0/py_pkg_logging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-02-21 22:00:33.000000 py_pkg_logging-0.0.0/py_pkg_logging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-21 22:00:33.000000 py_pkg_logging-0.0.0/py_pkg_logging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 22:00:33.000000 py_pkg_logging-0.0.0/py_pkg_logging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-21 22:00:33.000000 py_pkg_logging-0.0.0/py_pkg_logging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 22:00:33.350411 py_pkg_logging-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-02-21 22:00:21.000000 py_pkg_logging-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:14:27.385337 py_pkg_logging-0.0.1rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-14 18:14:27.385337 py_pkg_logging-0.0.1rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-14 18:14:17.000000 py_pkg_logging-0.0.1rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:14:27.385337 py_pkg_logging-0.0.1rc0/py_pkg_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-14 18:14:17.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-14 18:14:17.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-14 18:14:17.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging/_log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-14 18:14:17.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging/_log_function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:14:27.385337 py_pkg_logging-0.0.1rc0/py_pkg_logging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-14 18:14:27.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-14 18:14:27.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 18:14:27.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-14 18:14:27.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 18:14:27.389337 py_pkg_logging-0.0.1rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-14 18:14:17.000000 py_pkg_logging-0.0.1rc0/setup.py
```

### Comparing `py_pkg_logging-0.0.0/PKG-INFO` & `py_pkg_logging-0.0.1rc0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_pkg_logging
-Version: 0.0.0
+Version: 0.0.1rc0
 Summary: Python Package Logging Assistant.
 Home-page: https://github.com/mvinyard/py-pkg-logging
 Author: Michael E. Vinyard
 Author-email: mvinyard.ai@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `py_pkg_logging-0.0.0/py_pkg_logging/_log_config.py` & `py_pkg_logging-0.0.1rc0/py_pkg_logging/_log_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 import logging
 import pathlib
 
 
 class LogConfig(ABCParse.ABCParse):
     def __init__(
         self,
+        name: str = "pypkg_logger",
         log_file="log.log",
         log_dir = pathlib.os.getcwd(),
         dirname = ".log_cache",
-        name: str = "cell_neighbors",
         file_level=logging.DEBUG,
-        console_level=logging.WARNING,
+        console_level=logging.INFO,
         *args,
         **kwargs
     ):
         """"""
         self.__parse__(locals())
         
         if not self.log_dir.exists():
```

### Comparing `py_pkg_logging-0.0.0/py_pkg_logging/_log_function_call.py` & `py_pkg_logging-0.0.1rc0/py_pkg_logging/_log_function_call.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,89 +1,72 @@
 
 import ABCParse
 import inspect
 from functools import wraps
 import logging
-
+import numpy as np
 
 from typing import Callable
 
 
-
 class FunctionCallLogger(ABCParse.ABCParse):
-    def __init__(self):
+    def __init__(self, logger):
         """"""
         self.__parse__(locals())
-        
-    @property
-    def arg_names(self):
-        return inspect.getfullargspec(self._func).args
+        self._ARGS_IGNORE = ['self']
 
     @property
     def arg_values(self):
-        return self._args
+        return self.bound.arguments
 
     @property
     def cls_method(self):
-        return "self" in self.all_args
+        return self._args and hasattr(self._args[0], self._func.__name__)
 
     @property
-    def func_name(self):
+    def bound(self):
         if self.cls_method:
-            cls = self.all_args.pop("self").__class__.__name__
+            self._bound = inspect.signature(self._func).bind(*self._args, **self._kwargs)
+        else:
+            self._bound = inspect.signature(self._func).bind_partial(*self._args, **self._kwargs)
+        self._bound.apply_defaults()
+        return self._bound
+
+    @property
+    def func_name(self):
+        if "self" in self.arg_values:
+            cls = self.arg_values.pop("self").__class__.__name__
             return f"{cls}.{self._func.__name__}"
         return self._func.__name__
     
     @property
     def _arg_message(self):
         return_str = ""
-        for key, val in self.all_args.items():
-            return_str += f"{key}={val}, "
+        for key, val in self.arg_values.items():
+            if not key in self._ARGS_IGNORE:
+                if isinstance(val, np.ndarray):
+                    val = f"np.ndarray of shape: {val.shape}"
+                return_str += f"{key}={val}, "
         return return_str[:-2] # rm final comma
     
     @property
     def log_message(self):
-        return print(f"Called: {self.func_name} with args: {self._arg_message}")
+        return f"Called: {self.func_name} with args: {self._arg_message}"
 
 
     def __call__(self, func, *args, **kwargs):
-        
+        """ """
         self.__update__(locals())
-        
-        self.all_args = dict(zip(self.arg_names, self.arg_values))
-        self.all_args.update(kwargs.items())
-        
-        logger.debug(self.log_message)
+        self._logger.debug(self.log_message)
 
 
-def log_function_call(func: Callable, *args, **kwargs):
-    
-    """
-    Args:
-        func (Callable)
-        
-        
-    Example:
-
-        ```python
-
-        class MyClass:
-            def __init__(self, *args, **kwargs):
-                """"""
-            @log_function_call
-            def special_func(self, a: float, b: float):
-                return a + b
-
-        my_cls = MyClass()
-        my_cls.special_func(2, 4)
-        ```
-        >>> Called: MyClass.special_func with args: a=2, b=4
-        >>> 6
-        """
-
-    @wraps(func)
-    def wrapper(*args, **kwargs):
-        function_call_logger = FunctionCallLogger()
-        function_call_logger(func, *args, **kwargs)
-        return func(*args, **kwargs)
-
-    return wrapper
+def log_function_call(logger):
+    def decorator(func: Callable):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            
+            function_call_logger = FunctionCallLogger(logger = logger)
+            function_call_logger(func, *args, **kwargs)
+            
+            return func(*args, **kwargs)
+        return wrapper
+    return decorator
```

### Comparing `py_pkg_logging-0.0.0/py_pkg_logging.egg-info/PKG-INFO` & `py_pkg_logging-0.0.1rc0/py_pkg_logging.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_pkg_logging
-Version: 0.0.0
+Version: 0.0.1rc0
 Summary: Python Package Logging Assistant.
 Home-page: https://github.com/mvinyard/py-pkg-logging
 Author: Michael E. Vinyard
 Author-email: mvinyard.ai@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `py_pkg_logging-0.0.0/setup.py` & `py_pkg_logging-0.0.1rc0/setup.py`

 * *Files identical despite different names*

