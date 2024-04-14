# Comparing `tmp/vomero-0.1.5.tar.gz` & `tmp/vomero-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vomero-0.1.5.tar", max compression
+gzip compressed data, was "vomero-0.1.6.tar", max compression
```

## Comparing `vomero-0.1.5.tar` & `vomero-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2024-04-10 20:57:16.728973 vomero-0.1.5/LICENSE
--rw-r--r--   0        0        0     2605 2024-04-10 20:57:16.728973 vomero-0.1.5/README.md
--rw-r--r--   0        0        0      537 2024-04-10 20:57:16.728973 vomero-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       88 2024-04-10 20:57:16.728973 vomero-0.1.5/src/vomero/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 20:57:16.728973 vomero-0.1.5/src/vomero/py.typed
--rw-r--r--   0        0        0     5641 2024-04-10 20:57:16.728973 vomero-0.1.5/src/vomero/streams.py
--rw-r--r--   0        0        0      357 2024-04-10 20:57:16.728973 vomero-0.1.5/src/vomero/types.py
--rw-r--r--   0        0        0      996 2024-04-10 20:57:16.728973 vomero-0.1.5/src/vomero/worker.py
--rw-r--r--   0        0        0     3155 1970-01-01 00:00:00.000000 vomero-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-14 13:36:36.862376 vomero-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2605 2024-04-14 13:36:36.862376 vomero-0.1.6/README.md
+-rw-r--r--   0        0        0      537 2024-04-14 13:36:36.862376 vomero-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       88 2024-04-14 13:36:36.862376 vomero-0.1.6/src/vomero/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 13:36:36.862376 vomero-0.1.6/src/vomero/py.typed
+-rw-r--r--   0        0        0     5941 2024-04-14 13:36:36.862376 vomero-0.1.6/src/vomero/streams.py
+-rw-r--r--   0        0        0      357 2024-04-14 13:36:36.862376 vomero-0.1.6/src/vomero/types.py
+-rw-r--r--   0        0        0      996 2024-04-14 13:36:36.862376 vomero-0.1.6/src/vomero/worker.py
+-rw-r--r--   0        0        0     3155 1970-01-01 00:00:00.000000 vomero-0.1.6/PKG-INFO
```

### Comparing `vomero-0.1.5/LICENSE` & `vomero-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vomero-0.1.5/README.md` & `vomero-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `vomero-0.1.5/pyproject.toml` & `vomero-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vomero"
-version = "0.1.5"
+version = "0.1.6"
 description = "Event processing library for Python based on Redis Streams"
 authors = ["Marcin Sawicki <marcin.z.sawicki@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/mzsawicki/vomero"
 
 [tool.poetry.dependencies]
```

### Comparing `vomero-0.1.5/src/vomero/streams.py` & `vomero-0.1.6/src/vomero/streams.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,19 +39,27 @@
 
         return wrapper_decorator
 
     def consumer(
         self,
         stream: str,
         consumer_group: str,
-        consumer: str,
         block: int = 0,
         auto_claim: bool = False,
         auto_claim_timeout: int = AUTO_CLAIM_TIMEOUT_DEFAULT,
+        consumer: typing.Optional[str] = None,
+        consumer_factory: typing.Optional[typing.Callable[..., str]] = None,
     ) -> typing.Callable[[ConsumerCoro], ConsumerCoro]:
+
+        if consumer_factory is not None:
+            consumer = consumer_factory()
+
+        if consumer is None:
+            raise ValueError("Either consumer or consumer_factory must be defined")
+
         def wrapper_decorator(consumer_coro: ConsumerCoro) -> ConsumerCoro:
             @functools.wraps(consumer_coro)
             async def wrapper_consumer(
                 *args: typing.Any, **kwargs: typing.Any
             ) -> typing.Any:
                 id_, event = None, None
                 if auto_claim:
```

### Comparing `vomero-0.1.5/src/vomero/worker.py` & `vomero-0.1.6/src/vomero/worker.py`

 * *Files identical despite different names*

### Comparing `vomero-0.1.5/PKG-INFO` & `vomero-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vomero
-Version: 0.1.5
+Version: 0.1.6
 Summary: Event processing library for Python based on Redis Streams
 Home-page: https://github.com/mzsawicki/vomero
 License: MIT
 Author: Marcin Sawicki
 Author-email: marcin.z.sawicki@protonmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

