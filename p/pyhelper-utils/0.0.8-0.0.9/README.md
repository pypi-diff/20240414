# Comparing `tmp/pyhelper_utils-0.0.8.tar.gz` & `tmp/pyhelper_utils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhelper_utils-0.0.8.tar", max compression
+gzip compressed data, was "pyhelper_utils-0.0.9.tar", max compression
```

## Comparing `pyhelper_utils-0.0.8.tar` & `pyhelper_utils-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2024-04-10 11:34:42.614458 pyhelper_utils-0.0.8/LICENSE
--rw-r--r--   0        0        0      680 2024-04-10 11:34:42.615458 pyhelper_utils-0.0.8/README.md
--rw-r--r--   0        0        0        0 2024-04-10 11:34:42.620458 pyhelper_utils-0.0.8/pyhelper_utils/__init__.py
--rw-r--r--   0        0        0     1871 2024-04-10 11:34:42.620458 pyhelper_utils-0.0.8/pyhelper_utils/general.py
--rw-r--r--   0        0        0     1455 2024-04-10 11:34:42.620458 pyhelper_utils-0.0.8/pyhelper_utils/notifications.py
--rw-r--r--   0        0        0     1624 2024-04-10 11:34:42.620458 pyhelper_utils-0.0.8/pyhelper_utils/runners.py
--rw-r--r--   0        0        0     2324 2024-04-10 11:34:42.620458 pyhelper_utils-0.0.8/pyhelper_utils/shell.py
--rw-r--r--   0        0        0     1549 2024-04-10 11:34:46.935428 pyhelper_utils-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1737 1970-01-01 00:00:00.000000 pyhelper_utils-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-14 13:36:00.090263 pyhelper_utils-0.0.9/LICENSE
+-rw-r--r--   0        0        0      680 2024-04-14 13:36:00.090263 pyhelper_utils-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2024-04-14 13:36:00.096263 pyhelper_utils-0.0.9/pyhelper_utils/__init__.py
+-rw-r--r--   0        0        0     2193 2024-04-14 13:36:00.096263 pyhelper_utils-0.0.9/pyhelper_utils/general.py
+-rw-r--r--   0        0        0     1455 2024-04-14 13:36:00.096263 pyhelper_utils-0.0.9/pyhelper_utils/notifications.py
+-rw-r--r--   0        0        0     1624 2024-04-14 13:36:00.096263 pyhelper_utils-0.0.9/pyhelper_utils/runners.py
+-rw-r--r--   0        0        0     2324 2024-04-14 13:36:00.096263 pyhelper_utils-0.0.9/pyhelper_utils/shell.py
+-rw-r--r--   0        0        0     1549 2024-04-14 13:36:04.126225 pyhelper_utils-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1737 1970-01-01 00:00:00.000000 pyhelper_utils-0.0.9/PKG-INFO
```

### Comparing `pyhelper_utils-0.0.8/LICENSE` & `pyhelper_utils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.8/README.md` & `pyhelper_utils-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.8/pyhelper_utils/general.py` & `pyhelper_utils-0.0.9/pyhelper_utils/general.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from __future__ import annotations
 import re
 from time import sleep
 from functools import wraps
 from logging import Logger
-from typing import Any, Optional
+from typing import Any
 
 
 def tts(ts: Any) -> int:
     """
     Convert time string to seconds.
 
     Args:
@@ -35,39 +36,48 @@
         return _time * 60
     elif _unit == "h":
         return _time * 60 * 60
     else:
         return int(ts)
 
 
-def ignore_exceptions(logger: Optional[Logger] = None, retry: int = 0) -> Any:
+def ignore_exceptions(
+    retry: int = 0,
+    retry_interval: int = 1,
+    return_on_error: Any = None,
+    logger: Logger | None = None,
+) -> Any:
     """
     Decorator to ignore exceptions with support for retry.
 
     Args:
-        logger (Logger): logger to use, if not passed no logs will be displayed.
         retry (int): Number of retry if the underline function throw exception.
+        retry_interval (int): Number of seconds to wait between retries.
+        return_on_error (Any): Return value if the underline function throw exception.
+        logger (Logger): logger to use, if not passed no logs will be displayed.
+
 
     Returns:
         any: the underline function return value.
     """
 
     def wrapper(func):
         @wraps(func)
         def inner(*args, **kwargs):
             try:
                 return func(*args, **kwargs)
             except Exception as ex:
                 if retry:
+                    sleep(retry_interval)
                     for _ in range(0, retry):
                         try:
                             return func(*args, **kwargs)
                         except Exception:
-                            sleep(1)
+                            sleep(retry_interval)
 
                 if logger:
                     logger.info(f"{func.__name__} error: {ex}")
-                return None
+                return return_on_error
 
         return inner
 
     return wrapper
```

### Comparing `pyhelper_utils-0.0.8/pyhelper_utils/notifications.py` & `pyhelper_utils-0.0.9/pyhelper_utils/notifications.py`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.8/pyhelper_utils/runners.py` & `pyhelper_utils-0.0.9/pyhelper_utils/runners.py`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.8/pyhelper_utils/shell.py` & `pyhelper_utils-0.0.9/pyhelper_utils/shell.py`

 * *Files identical despite different names*

### Comparing `pyhelper_utils-0.0.8/pyproject.toml` & `pyhelper_utils-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 output-format = "grouped"
 
 [tool.ruff.format]
 exclude = [".git", ".venv", ".mypy_cache", ".tox", "__pycache__"]
 
 [tool.poetry]
 name = "pyhelper-utils"
-version = "0.0.8"
+version = "0.0.9"
 description = "Collective utility functions for python projects"
 readme = "README.md"
 repository = "https://github.com/RedHatQE/pyhelper-utils"
 authors = [
   "Meni Yakove <myakove@gmail.com>",
   "Ruth Netser <rnetser@gmail.com>",
   "Debarati Basu-Nag <dbasunag@redhat.com>",
```

### Comparing `pyhelper_utils-0.0.8/PKG-INFO` & `pyhelper_utils-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhelper-utils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Collective utility functions for python projects
 Home-page: https://github.com/RedHatQE/pyhelper-utils
 License: Apache-2.0
 Author: Meni Yakove
 Author-email: myakove@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

