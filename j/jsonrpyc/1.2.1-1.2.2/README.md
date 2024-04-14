# Comparing `tmp/jsonrpyc-1.2.1.tar.gz` & `tmp/jsonrpyc-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonrpyc-1.2.1.tar", last modified: Wed Nov 22 18:07:49 2023, max compression
+gzip compressed data, was "jsonrpyc-1.2.2.tar", last modified: Sun Apr 14 11:42:15 2024, max compression
```

## Comparing `jsonrpyc-1.2.1.tar` & `jsonrpyc-1.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 18:07:49.404395 jsonrpyc-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2023-11-22 18:07:34.000000 jsonrpyc-1.2.1/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2023-11-22 18:07:34.000000 jsonrpyc-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-11-22 18:07:34.000000 jsonrpyc-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6611 2023-11-22 18:07:49.404395 jsonrpyc-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2023-11-22 18:07:34.000000 jsonrpyc-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 18:07:49.400395 jsonrpyc-1.2.1/jsonrpyc/
--rw-r--r--   0 runner    (1001) docker     (127)    20199 2023-11-22 18:07:34.000000 jsonrpyc-1.2.1/jsonrpyc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2023-11-22 18:07:34.000000 jsonrpyc-1.2.1/jsonrpyc/__meta__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 18:07:49.404395 jsonrpyc-1.2.1/jsonrpyc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6611 2023-11-22 18:07:49.000000 jsonrpyc-1.2.1/jsonrpyc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      328 2023-11-22 18:07:49.000000 jsonrpyc-1.2.1/jsonrpyc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-22 18:07:49.000000 jsonrpyc-1.2.1/jsonrpyc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       89 2023-11-22 18:07:49.000000 jsonrpyc-1.2.1/jsonrpyc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-22 18:07:49.000000 jsonrpyc-1.2.1/jsonrpyc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2023-11-22 18:07:34.000000 jsonrpyc-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-22 18:07:34.000000 jsonrpyc-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-11-22 18:07:34.000000 jsonrpyc-1.2.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-22 18:07:49.404395 jsonrpyc-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-22 18:07:49.400395 jsonrpyc-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2023-11-22 18:07:34.000000 jsonrpyc-1.2.1/tests/test_rpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2023-11-22 18:07:34.000000 jsonrpyc-1.2.1/tests/test_spec.py
+drwxr-xr-x   0 marcel     (501) staff       (20)        0 2024-04-14 11:42:15.691522 jsonrpyc-1.2.2/
+-rw-r--r--   0 marcel     (501) staff       (20)      165 2023-11-22 17:53:22.000000 jsonrpyc-1.2.2/.flake8
+-rw-r--r--   0 marcel     (501) staff       (20)     1496 2024-04-14 08:52:12.000000 jsonrpyc-1.2.2/LICENSE
+-rw-r--r--   0 marcel     (501) staff       (20)      133 2023-11-22 17:53:22.000000 jsonrpyc-1.2.2/MANIFEST.in
+-rw-r--r--   0 marcel     (501) staff       (20)     7021 2024-04-14 11:42:15.691238 jsonrpyc-1.2.2/PKG-INFO
+-rw-r--r--   0 marcel     (501) staff       (20)     3446 2024-04-14 11:41:27.000000 jsonrpyc-1.2.2/README.md
+drwxr-xr-x   0 marcel     (501) staff       (20)        0 2024-04-14 11:42:15.688385 jsonrpyc-1.2.2/jsonrpyc/
+-rw-r--r--   0 marcel     (501) staff       (20)    21472 2024-04-14 11:41:27.000000 jsonrpyc-1.2.2/jsonrpyc/__init__.py
+-rw-r--r--   0 marcel     (501) staff       (20)      430 2024-04-14 11:41:27.000000 jsonrpyc-1.2.2/jsonrpyc/__meta__.py
+drwxr-xr-x   0 marcel     (501) staff       (20)        0 2024-04-14 11:42:15.689998 jsonrpyc-1.2.2/jsonrpyc.egg-info/
+-rw-r--r--   0 marcel     (501) staff       (20)     7021 2024-04-14 11:42:15.000000 jsonrpyc-1.2.2/jsonrpyc.egg-info/PKG-INFO
+-rw-r--r--   0 marcel     (501) staff       (20)      328 2024-04-14 11:42:15.000000 jsonrpyc-1.2.2/jsonrpyc.egg-info/SOURCES.txt
+-rw-r--r--   0 marcel     (501) staff       (20)        1 2024-04-14 11:42:15.000000 jsonrpyc-1.2.2/jsonrpyc.egg-info/dependency_links.txt
+-rw-r--r--   0 marcel     (501) staff       (20)      240 2024-04-14 11:42:15.000000 jsonrpyc-1.2.2/jsonrpyc.egg-info/requires.txt
+-rw-r--r--   0 marcel     (501) staff       (20)        9 2024-04-14 11:42:15.000000 jsonrpyc-1.2.2/jsonrpyc.egg-info/top_level.txt
+-rw-r--r--   0 marcel     (501) staff       (20)     1687 2024-04-14 11:41:27.000000 jsonrpyc-1.2.2/pyproject.toml
+-rw-r--r--   0 marcel     (501) staff       (20)        0 2024-04-14 11:41:27.000000 jsonrpyc-1.2.2/requirements.txt
+-rw-r--r--   0 marcel     (501) staff       (20)      301 2024-04-14 11:41:27.000000 jsonrpyc-1.2.2/requirements_dev.txt
+-rw-r--r--   0 marcel     (501) staff       (20)       38 2024-04-14 11:42:15.691579 jsonrpyc-1.2.2/setup.cfg
+drwxr-xr-x   0 marcel     (501) staff       (20)        0 2024-04-14 11:42:15.689569 jsonrpyc-1.2.2/tests/
+-rw-r--r--   0 marcel     (501) staff       (20)     1932 2023-11-22 17:53:22.000000 jsonrpyc-1.2.2/tests/test_rpc.py
+-rw-r--r--   0 marcel     (501) staff       (20)     1839 2023-11-22 17:53:22.000000 jsonrpyc-1.2.2/tests/test_spec.py
```

### Comparing `jsonrpyc-1.2.1/LICENSE` & `jsonrpyc-1.2.2/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2016-2023, Marcel Rieger
+Copyright (c) 2016-2024, Marcel Rieger
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `jsonrpyc-1.2.1/PKG-INFO` & `jsonrpyc-1.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: jsonrpyc
-Version: 1.2.1
+Version: 1.2.2
 Summary: Minimal python RPC implementation in a single file based on the JSON-RPC 2.0 specs from http://www.jsonrpc.org/specification.
 Author-email: Marcel Rieger <github.riga@icloud.com>
-License: Copyright (c) 2016-2023, Marcel Rieger
+License: Copyright (c) 2016-2024, Marcel Rieger
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         * Redistributions of source code must retain the above copyright notice, this
           list of conditions and the following disclaimer.
@@ -48,19 +48,24 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
-Requires-Dist: flake8~=5.0; extra == "dev"
-Requires-Dist: flake8-commas~=2.1; extra == "dev"
-Requires-Dist: flake8-quotes~=3.3; extra == "dev"
-Requires-Dist: pytest~=7.4.0; extra == "dev"
+Requires-Dist: mypy~=1.9.0; python_version >= "3.8" and extra == "dev"
+Requires-Dist: mypy~=1.4.1; python_version < "3.8" and extra == "dev"
+Requires-Dist: flake8~=7.0.0; python_version >= "3.8" and extra == "dev"
+Requires-Dist: flake8~=5.0.0; python_version < "3.8" and extra == "dev"
+Requires-Dist: flake8-commas~=2.1.0; extra == "dev"
+Requires-Dist: flake8-quotes~=3.3.2; extra == "dev"
+Requires-Dist: pytest~=7.4.4; extra == "dev"
 Requires-Dist: pytest-cov~=4.1.0; extra == "dev"
+Requires-Dist: types-docutils~=0.20.0; python_version >= "3.8" and extra == "dev"
+Requires-Dist: types-docutils~=0.20.0; python_version < "3.8" and extra == "dev"
 
 <!-- marker-before-logo -->
 
 <p align="center">
   <img src="https://media.githubusercontent.com/media/riga/jsonrpyc/master/assets/logo.png" width="400" />
 </p>
```

### Comparing `jsonrpyc-1.2.1/README.md` & `jsonrpyc-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `jsonrpyc-1.2.1/jsonrpyc/__init__.py` & `jsonrpyc-1.2.2/jsonrpyc/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 import sys
 import json
 import io
 import time
 import threading
-from typing import Any, Callable
+from typing import Any, Callable, Type
 
 # package infos
 from jsonrpyc.__meta__ import (  # noqa
     __doc__,
     __author__,
     __email__,
     __copyright__,
@@ -60,19 +60,18 @@
 
     @classmethod
     def check_code(cls, code: int) -> None:
         """
         Value check for *code* entries. Raises a *TypeError* when *code* is not an integer, or a
         *KeyError* when there is no :py:class:`RPCError` subclass registered for that *code*.
         """
-        if not isinstance(code, int):
-            raise TypeError(f"code must be an integer, got {code} ({type(code)})")
-
-        if not get_error(code):
-            raise ValueError(f"unknown code, got {code} ({type(code)})")
+        try:
+            get_error(code)
+        except:
+            raise TypeError(f"invalid error code, got {code} ({type(code)})")
 
     @classmethod
     def request(
         cls,
         method: str,
         id: str | int | None = None,
         params: dict[str, Any] | None = None,
@@ -130,28 +129,33 @@
             res = f"{{\"jsonrpc\":\"2.0\",\"id\":{id},\"result\":{json.dumps(result)}}}"
         except Exception as e:
             raise RPCParseError(str(e))
 
         return res
 
     @classmethod
-    def error(cls, id: str | int | None, code: int, data: dict | None = None) -> str:
+    def error(
+        cls,
+        id: str | int | None,
+        code: int,
+        data: Any | None = None,
+    ) -> str:
         """
         Creates the string representation of an error that occured while processing a request with
         *id*. *code* must lead to a registered :py:class:`RPCError`. *data* might contain
         additional, detailed error information and is encoded by ``json.dumps`` when set.
         """
         try:
             cls.check_id(id)
             cls.check_code(code)
         except Exception as e:
             raise RPCInvalidRequest(str(e))
 
         # build the inner error data
-        message = get_error(code).title
+        message = get_error(code).title  # type: ignore[union-attr]
         err_data = f"{{\"code\":{code},\"message\":\"{message}\""
 
         # insert data when given
         if data is not None:
             try:
                 err_data += f",\"data\":{json.dumps(data)}}}"
             except Exception as e:
@@ -240,80 +244,91 @@
 
         The :py:class:`Watchdog` instance that optionally watches *stdin* and dispatches incoming
         requests.
     """
 
     EMPTY_RESULT = object()
 
+    # TODO: use protocol instead of discouraged hints
     def __init__(
-        self: RPC,
+        self,
         target: Any | None = None,
         stdin: io.TextIOBase | None = None,
         stdout: io.TextIOBase | None = None,
         watch: bool = True,
         **kwargs,
     ) -> None:
         super().__init__()
 
         # the wrapped target object
         self.target = target
 
         # open streams
-        stdin = sys.stdin if stdin is None else stdin
-        stdout = sys.stdout if stdout is None else stdout
-        self.stdin = io.open(stdin.fileno(), "rb")
-        self.stdout = io.open(stdout.fileno(), "wb")
+        _stdin = sys.stdin if stdin is None else stdin  # type: ignore[assignment]
+        _stdout = sys.stdout if stdout is None else stdout  # type: ignore[assignment]
+        self.stdin = io.open(_stdin.fileno(), "rb")  # type: ignore[attr-defined]
+        self.stdout = io.open(_stdout.fileno(), "wb")  # type: ignore[attr-defined]
+        self.original_stdin = _stdin
+        self.original_stdout = _stdout
 
         # other attributes
         self._i = -1
-        self._callbacks = {}
-        self._results = {}
+        self._callbacks: dict[int, Callable] = {}
+        self._results: dict[int, Any] = {}
 
         # create and optionall start the watchdog
         kwargs["start"] = watch
         kwargs.setdefault("daemon", target is None)
         self.watchdog = Watchdog(self, **kwargs)
 
-    def __del__(self: RPC) -> None:
+    def __del__(self) -> None:
         watchdog = getattr(self, "watchdog", None)
         if watchdog:
             watchdog.stop()
 
-    def __call__(self: RPC, *args, **kwargs) -> None:
+    def __call__(self, *args, **kwargs) -> None:
         """
         Shorthand for :py:meth:`call`.
         """
         return self.call(*args, **kwargs)
 
     def call(
-        self: RPC,
+        self,
         method: str,
-        args: tuple[Any] = (),
+        args: tuple[Any, ...] = (),
         kwargs: dict | None = None,
         callback: Callable | None = None,
         block: int = 0,
+        timeout: float | int = 0,
     ) -> None:
         """
         Performs an actual remote procedure call by writing a request representation (a string) to
         the output stream. The remote RPC instance uses *method* to route to the actual method to
-        call with *args* and *kwargs*. When *callback* is set, it will be called with the result of
-        the remote call. When *block* is larger than *0*, the calling thread is blocked until the
-        result is received. In this case, *block* will be the poll interval, emulating synchronuous
-        return value behavior. When both *callback* is *None* and *block* is *0* or smaller, the
-        request is considered a notification and the remote RPC instance will not send a response.
+        call with *args* and *kwargs*.
+
+        When *callback* is set, it will be called with the result of the remote call. When *block*
+        is larger than *0*, the calling thread is blocked until the result is received. In this
+        case, *block* will be the poll interval, emulating synchronuous return value behavior.
+        When both *callback* is *None* and *block* is *0* or smaller, the request is considered a
+        notification and the remote RPC instance will not send a response.
+
+        If *timeout* is not zero, raise TimeoutError after *timeout* seconds with no response.
         """
+        starting_time = time.monotonic()
+
         # default kwargs
         if kwargs is None:
             kwargs = {}
 
         # check if the call is a notification
         is_notification = callback is None and block <= 0
 
         # create a new id for requests expecting a response
-        id = None
+        # TODO: simplify case when id is (not) needed
+        id = -1
         if not is_notification:
             self._i += 1
             id = self._i
 
         # register the callback
         if callback is not None:
             self._callbacks[id] = callback
@@ -332,17 +347,23 @@
             while True:
                 if self._results[id] != self.EMPTY_RESULT:
                     result = self._results[id]
                     del self._results[id]
                     if isinstance(result, Exception):
                         raise result
                     return result
+
+                if timeout:
+                    elapsed = time.monotonic() - starting_time
+                    if elapsed > timeout:
+                        raise TimeoutError("RPC Request timed out")
+
                 time.sleep(block)
 
-    def _handle(self: RPC, line: str) -> None:
+    def _handle(self, line: str) -> None:
         """
         Handles an incoming *line* and dispatches the parsed object to the request, response, or
         error handlers.
         """
         obj = json.loads(line)
 
         # dispatch to the correct handler
@@ -352,15 +373,15 @@
         elif "error" not in obj:
             # response
             self._handle_response(obj)
         else:
             # error
             self._handle_error(obj)
 
-    def _handle_request(self: RPC, req: dict[str, Any]) -> None:
+    def _handle_request(self, req: dict[str, Any]) -> None:
         """
         Handles an incoming request *req*. When it containes an id, a response or error is sent
         back.
         """
         try:
             method = self._route(req["method"])
             result = method(*req["params"]["args"], **req["params"]["kwargs"])
@@ -371,30 +392,30 @@
             if "id" in req:
                 if isinstance(e, RPCError):
                     err = Spec.error(req["id"], e.code, e.data)
                 else:
                     err = Spec.error(req["id"], -32603, str(e))
                 self._write(err)
 
-    def _handle_response(self: RPC, res: dict[str, Any]) -> None:
+    def _handle_response(self, res: dict[str, Any]) -> None:
         """
         Handles an incoming successful response *res*. Blocking calls are resolved and registered
         callbacks are invoked with the first error argument being set to *None*.
         """
         # set the result
         if res["id"] in self._results:
             self._results[res["id"]] = res["result"]
 
         # lookup and invoke the callback
         if res["id"] in self._callbacks:
             callback = self._callbacks[res["id"]]
             del self._callbacks[res["id"]]
             callback(None, res["result"])
 
-    def _handle_error(self: RPC, res: dict[str, Any]) -> None:
+    def _handle_error(self, res: dict[str, Any]) -> None:
         """
         Handles an incoming failed response *res*. Blocking calls throw an exception and
         registered callbacks are invoked with an exception and the second result argument set to
         *None*.
         """
         # extract the error and create an actual error instance to raise
         err = res["error"]
@@ -406,15 +427,15 @@
 
         # lookup and invoke the callback
         if res["id"] in self._callbacks:
             callback = self._callbacks[res["id"]]
             del self._callbacks[res["id"]]
             callback(error, None)
 
-    def _route(self: RPC, method: str) -> Any:
+    def _route(self, method: str) -> Any:
         """
         Returnes the method of the wrapped target object to be called when *method* is requested.
         Example:
 
         .. code-block:: python
 
             MyClassB(object):
@@ -443,19 +464,19 @@
                 break
             obj = getattr(obj, part)
         else:
             return obj
 
         raise RPCMethodNotFound(data=method)
 
-    def _write(self: RPC, s: str) -> None:
+    def _write(self, s: str) -> None:
         """
         Writes a string *s* to the output stream.
         """
-        self.stdout.write(bytearray(s + "\n", "utf-8"))
+        self.stdout.write(bytearray(f"{s}\n", "utf-8"))
         self.stdout.flush()
 
 
 class Watchdog(threading.Thread):
     """
     This class represents a thread that watches the input stream of an :py:class:`RPC` instance for
     incoming content and dispatches requests to it.
@@ -474,18 +495,18 @@
 
     .. py:attribute:: daemon
 
         The thread's daemon flag.
     """
 
     def __init__(
-        self: Watchdog,
+        self,
         rpc: RPC,
         name: str = "watchdog",
-        interval: float = 0.1,
+        interval: float | int = 0.1,
         daemon: bool = False,
         start: bool = True,
     ) -> None:
         super().__init__()
 
         # store attributes
         self.rpc = rpc
@@ -495,27 +516,27 @@
 
         # register a stop event
         self._stop = threading.Event()
 
         if start:
             self.start()
 
-    def start(self: Watchdog) -> None:
+    def start(self) -> None:
         """
-        Starts with thread's activity.
+        Starts the thread's activity.
         """
         super().start()
 
-    def stop(self: Watchdog) -> None:
+    def stop(self) -> None:
         """
-        Stops with thread's activity.
+        Stops the thread's activity.
         """
         self._stop.set()
 
-    def run(self: Watchdog) -> None:
+    def run(self) -> None:
         # reset the stop event
         self._stop.clear()
 
         # stop here when stdin is not set or closed
         if not self.rpc.stdin or self.rpc.stdin.closed:
             return
 
@@ -524,14 +545,18 @@
         while not self._stop.is_set():
             lines = None
 
             # stop when stdin is closed
             if self.rpc.stdin.closed:
                 break
 
+            # Keep linter happy
+            if self.rpc.original_stdin and self.rpc.original_stdin.closed:  # type: ignore[attr-defined] # noqa
+                break
+
             # read from stdin depending on whether it is a tty or not
             if self.rpc.stdin.isatty():
                 cur_pos = self.rpc.stdin.tell()
                 if cur_pos != last_pos:
                     self.rpc.stdin.seek(last_pos)
                     lines = self.rpc.stdin.readlines()
                     last_pos = self.rpc.stdin.tell()
@@ -541,16 +566,16 @@
                     lines = [self.rpc.stdin.readline()]
                 except IOError:
                     # prevent residual race conditions occurring when stdin is closed externally
                     pass
 
             # handle new lines if any
             if lines:
-                for line in lines:
-                    line = line.decode("utf-8").strip()
+                for b_line in lines:
+                    line = b_line.decode("utf-8").strip()
                     if line:
                         self.rpc._handle(line)
             else:
                 self._stop.wait(self.interval)
 
 
 class RPCError(Exception):
@@ -563,125 +588,130 @@
 
     .. py:attribute:: data
 
         Additional data of this error. Setting the data attribute will also change the message
         attribute.
     """
 
-    def __init__(self: RPCError, data: str | None = None) -> None:
+    code_range: tuple[int, int]
+    code: int
+    title: str
+
+    @classmethod
+    def is_code_range(cls, code: Any) -> bool:
+        return (
+            isinstance(code, tuple) and
+            len(code) == 2 and
+            all(isinstance(i, int) for i in code) and
+            code[0] <= code[1]
+        )
+
+    def __init__(self, data: str | None = None) -> None:
         # build the error message
         message = f"{self.title} ({self.code})"
         if data is not None:
             message += f", data: {data}"
         self.message = message
 
         super().__init__(message)
 
         self.data = data
 
     def __str__(self):
         return self.message
 
 
-error_map_distinct = {}
-error_map_range = {}
-
+error_map_code: dict[int, Type[RPCError]] = {}
+error_map_code_range: dict[tuple[int, int], Type[RPCError]] = {}
 
-def is_range(code: Any) -> bool:
-    return (
-        isinstance(code, tuple) and
-        len(code) == 2 and
-        all(isinstance(i, int) for i in code) and
-        code[0] < code[1]
-    )
 
-
-def register_error(cls: type) -> type:
+def register_error(cls: Type[RPCError]) -> Type[RPCError]:
     """
     Decorator that registers a new RPC error derived from :py:class:`RPCError`. The purpose of
     error registration is to have a mapping of error codes/code ranges to error classes for faster
     lookups during error creation.
 
     .. code-block:: python
 
         @register_error
         class MyCustomRPCError(RPCError):
-            code = ...
+            code_range = (lower_bound, upper_bound)  # both inclusive
+            code = code_range[0]  # default code when used as is
             title = "My custom error"
     """
-    # it would be much cleaner to add a meta class to RPCError as a registry for codes
-    # but in CPython 2 exceptions aren't types, so simply provide a registry mechanism here
     if not issubclass(cls, RPCError):
         raise TypeError(f"'{cls}' is not a subclass of RPCError")
 
-    code = cls.code
-
-    if isinstance(code, int):
-        error_map = error_map_distinct
-    elif is_range(code):
-        error_map = error_map_range
-    else:
-        raise TypeError(f"invalid RPC error code {code}")
-
-    if code in error_map:
-        raise AttributeError(f"duplicate RPC error code {code}")
-
-    error_map[code] = cls
+    # check duplicates
+    if cls.code in error_map_code:
+        raise AttributeError(f"duplicate RPC error code {cls.code}")
+    if cls.code_range in error_map_code_range:
+        raise AttributeError(f"duplicate RPC error code range {cls.code_range}")
+
+    # register
+    error_map_code[cls.code] = cls
+    error_map_code_range[cls.code_range] = cls
 
     return cls
 
 
-def get_error(code: int) -> type | None:
+def get_error(code: int) -> Type[RPCError]:
     """
-    Returns the RPC error class that was previously registered to *code*. *None* is returned when no
-    class could be found.
+    Returns the RPC error class that was previously registered to *code*. A ``ValueError`` is raised
+    if no error class was found for *code*.
     """
-    if code in error_map_distinct:
-        return error_map_distinct[code]
+    if code in error_map_code:
+        return error_map_code[code]
 
-    for (lower, upper), cls in error_map_range.items():
+    for (lower, upper), cls in error_map_code_range.items():
         if lower <= code <= upper:
             return cls
 
-    return None
+    raise ValueError(f"unknown error code '{code}' ({type(code)})")
 
 
 @register_error
 class RPCParseError(RPCError):
 
-    code = -32700
+    code_range = (-32700, -32700)
+    code = code_range[0]
     title = "Parse error"
 
 
 @register_error
 class RPCInvalidRequest(RPCError):
 
-    code = -32600
+    code_range = (-32600, -32600)
+    code = code_range[0]
     title = "Invalid Request"
 
 
 @register_error
 class RPCMethodNotFound(RPCError):
 
-    code = -32601
+    code_range = (-32601, -32601)
+    code = code_range[0]
     title = "Method not found"
 
 
 @register_error
 class RPCInvalidParams(RPCError):
 
-    code = -32602
+    code_range = (-32602, -32602)
+    code = code_range[0]
     title = "Invalid params"
 
 
 @register_error
 class RPCInternalError(RPCError):
 
-    code = -32603
+    code_range = (-32603, -32603)
+    code = code_range[0]
     title = "Internal error"
 
 
 @register_error
 class RPCServerError(RPCError):
 
-    code = (-32099, -32000)
+    code_range = (-32099, -32000)
+    code = code_range[0]  # default code when used as is
     title = "Server error"
```

### Comparing `jsonrpyc-1.2.1/jsonrpyc.egg-info/PKG-INFO` & `jsonrpyc-1.2.2/jsonrpyc.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: jsonrpyc
-Version: 1.2.1
+Version: 1.2.2
 Summary: Minimal python RPC implementation in a single file based on the JSON-RPC 2.0 specs from http://www.jsonrpc.org/specification.
 Author-email: Marcel Rieger <github.riga@icloud.com>
-License: Copyright (c) 2016-2023, Marcel Rieger
+License: Copyright (c) 2016-2024, Marcel Rieger
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         * Redistributions of source code must retain the above copyright notice, this
           list of conditions and the following disclaimer.
@@ -48,19 +48,24 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
-Requires-Dist: flake8~=5.0; extra == "dev"
-Requires-Dist: flake8-commas~=2.1; extra == "dev"
-Requires-Dist: flake8-quotes~=3.3; extra == "dev"
-Requires-Dist: pytest~=7.4.0; extra == "dev"
+Requires-Dist: mypy~=1.9.0; python_version >= "3.8" and extra == "dev"
+Requires-Dist: mypy~=1.4.1; python_version < "3.8" and extra == "dev"
+Requires-Dist: flake8~=7.0.0; python_version >= "3.8" and extra == "dev"
+Requires-Dist: flake8~=5.0.0; python_version < "3.8" and extra == "dev"
+Requires-Dist: flake8-commas~=2.1.0; extra == "dev"
+Requires-Dist: flake8-quotes~=3.3.2; extra == "dev"
+Requires-Dist: pytest~=7.4.4; extra == "dev"
 Requires-Dist: pytest-cov~=4.1.0; extra == "dev"
+Requires-Dist: types-docutils~=0.20.0; python_version >= "3.8" and extra == "dev"
+Requires-Dist: types-docutils~=0.20.0; python_version < "3.8" and extra == "dev"
 
 <!-- marker-before-logo -->
 
 <p align="center">
   <img src="https://media.githubusercontent.com/media/riga/jsonrpyc/master/assets/logo.png" width="400" />
 </p>
```

### Comparing `jsonrpyc-1.2.1/pyproject.toml` & `jsonrpyc-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jsonrpyc-1.2.1/tests/test_rpc.py` & `jsonrpyc-1.2.2/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `jsonrpyc-1.2.1/tests/test_spec.py` & `jsonrpyc-1.2.2/tests/test_spec.py`

 * *Files identical despite different names*

