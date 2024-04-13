# Comparing `tmp/retried-7.4.0.tar.gz` & `tmp/retried-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retried-7.4.0.tar", last modified: Sat Apr 13 09:49:55 2024, max compression
+gzip compressed data, was "retried-8.0.0.tar", last modified: Sat Apr 13 23:13:20 2024, max compression
```

## Comparing `retried-7.4.0.tar` & `retried-8.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      102 2024-04-13 09:49:39.913796 retried-7.4.0/README.md
--rw-r--r--   0        0        0     1061 2024-04-13 09:49:55.653736 retried-7.4.0/pyproject.toml
--rw-r--r--   0        0        0      224 2024-04-13 09:49:39.917796 retried-7.4.0/src/retried/__init__.py
--rw-r--r--   0        0        0       18 2024-04-13 09:49:39.917796 retried-7.4.0/src/retried/__version__.py
--rw-r--r--   0        0        0     2290 2024-04-13 09:49:39.917796 retried-7.4.0/src/retried/aretry.py
--rw-r--r--   0        0        0     4052 2024-04-13 09:49:39.917796 retried-7.4.0/src/retried/retry.py
--rw-r--r--   0        0        0      189 2024-04-13 09:49:39.917796 retried-7.4.0/src/retried/utils.py
--rw-r--r--   0        0        0        0 2024-04-13 09:49:39.917796 retried-7.4.0/tests/__init__.py
--rw-r--r--   0        0        0      657 2024-04-13 09:49:39.917796 retried-7.4.0/tests/test_aretry.py
--rw-r--r--   0        0        0      276 1970-01-01 00:00:00.000000 retried-7.4.0/PKG-INFO
+-rw-r--r--   0        0        0      102 2024-04-13 23:13:03.933806 retried-8.0.0/README.md
+-rw-r--r--   0        0        0     1061 2024-04-13 23:13:20.734152 retried-8.0.0/pyproject.toml
+-rw-r--r--   0        0        0      224 2024-04-13 23:13:03.933806 retried-8.0.0/src/retried/__init__.py
+-rw-r--r--   0        0        0       18 2024-04-13 23:13:03.933806 retried-8.0.0/src/retried/__version__.py
+-rw-r--r--   0        0        0     2290 2024-04-13 23:13:03.933806 retried-8.0.0/src/retried/aretry.py
+-rw-r--r--   0        0        0     4018 2024-04-13 23:13:03.933806 retried-8.0.0/src/retried/retry.py
+-rw-r--r--   0        0        0      189 2024-04-13 23:13:03.933806 retried-8.0.0/src/retried/utils.py
+-rw-r--r--   0        0        0        0 2024-04-13 23:13:03.933806 retried-8.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      657 2024-04-13 23:13:03.933806 retried-8.0.0/tests/test_aretry.py
+-rw-r--r--   0        0        0      276 1970-01-01 00:00:00.000000 retried-8.0.0/PKG-INFO
```

### Comparing `retried-7.4.0/pyproject.toml` & `retried-8.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "retried"
-version = "7.4.0"
+version = "8.0.0"
 requires-python = ">=3.9"
 description = "A simple and powerful retrying library for Python"
 readme = "README.md"
 dependencies = []
 
 [build-system]
 requires = [
```

### Comparing `retried-7.4.0/src/retried/aretry.py` & `retried-8.0.0/src/retried/aretry.py`

 * *Files identical despite different names*

### Comparing `retried-7.4.0/src/retried/retry.py` & `retried-8.0.0/src/retried/retry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from functools import partial
 from functools import wraps
 from itertools import cycle
 from itertools import repeat
+from itertools import tee
 import logging
 import time
 import typing as t
 
 from .utils import relative_to_cwd
 
 
@@ -62,30 +63,33 @@
             return f(*args, **kwds)
 
         return wrapper
 
     return decorator
 
 
+def _fork_delays(delays: SingleOrIterable[DelayT]):
+    if not isinstance(delays, t.Iterable):
+        delays = repeat(delays)
+    delays, delays_ = tee(delays)
+    delays_ = cycle(delays_)
+    return delays, delays_
+
+
 def retry(
     retries: RetriesT = None,
     *,
     exceptions: SingleOrTuple[t.Type[Exception]] = Exception,
     error_callback: t.Optional[t.Callable[[int, Exception, DelayT, RetriesT, FuncT], None]] = None,
     sleep: SleepT = time.sleep,
     delays: SingleOrIterable[DelayT] = 0,
     first_delay: t.Optional[DelayT] = None,
     chain_exception: bool = False,
     logger: t.Union[logging.Logger, LogfT] = logger,
 ):
-    if not isinstance(delays, t.Iterable):
-        delays = repeat(delays)
-    delays = cycle(delays)
-    if first_delay is None:
-        first_delay = next(delays)
     if not isinstance(logger, logging.Logger):
         logger = DummyLogger(logger)
 
     def _default_error_callback(i: int, e: Exception, d: DelayT, r: RetriesT, f: FuncT):
         log_prefix = (
             f'{f.__qualname__} tried {i} of {r}:'
             f' '
@@ -105,36 +109,32 @@
         error_callback(i, e, d, r, f)
         if i != r:
             sleep(d)
 
     def decorator(f):
         @wraps(f)
         def wrapper(*args, **kwargs):
+            nonlocal delays
+            delays, delays_ = _fork_delays(delays)
             function_retrying = partial(f, *args, **kwargs)
             try:
-                # execute once
                 result = function_retrying()
             except exceptions as e:
-                # start retrying
                 i = 0
-                callback(i, e, first_delay, retries, f)
-                # retrying
+                callback(i, e, first_delay or next(delays_), retries, f)
                 while True:
                     try:
                         result = function_retrying()
                     except exceptions as e:
-                        # check if should retry
                         if i == retries:
                             if chain_exception:
                                 raise
                             raise e from None
-                        # then ++
                         i += 1
-                        delay = next(delays)
-                        callback(i, e, delay, retries, f)
+                        callback(i, e, next(delays_), retries, f)
                     else:
                         return result
             else:
                 return result
 
         return wrapper
```

### Comparing `retried-7.4.0/tests/test_aretry.py` & `retried-8.0.0/tests/test_aretry.py`

 * *Files identical despite different names*

