# Comparing `tmp/ombott-2.0rc1.tar.gz` & `tmp/ombott-2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\_MyPy\ombott\dist\.tmp-mzrkqplm\ombott-2.0rc1.tar", last modified: Fri Dec  8 21:37:13 2023, max compression
+gzip compressed data, was "D:\_MyPy\ombott\dist\.tmp-qv6_v0ro\ombott-2.0rc2.tar", last modified: Sat Dec  9 22:52:00 2023, max compression
```

## Comparing `ombott-2.0rc1.tar` & `ombott-2.0rc2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-12-08 21:37:13.964807 ombott-2.0rc1/
--rw-rw-rw-   0        0        0     1138 2021-08-02 22:15:45.000000 ombott-2.0rc1/LICENSE
--rw-rw-rw-   0        0        0      976 2023-12-08 21:37:13.963805 ombott-2.0rc1/PKG-INFO
--rw-rw-rw-   0        0        0       80 2021-08-02 21:55:10.000000 ombott-2.0rc1/README.md
-drwxrwxrwx   0        0        0        0 2023-12-08 21:37:13.923805 ombott-2.0rc1/ombott/
--rw-rw-rw-   0        0        0      785 2023-12-07 16:58:37.000000 ombott-2.0rc1/ombott/__init__.py
--rw-rw-rw-   0        0        0    10855 2023-12-07 16:58:37.000000 ombott-2.0rc1/ombott/common_helpers.py
--rw-rw-rw-   0        0        0      692 2021-08-28 23:59:49.000000 ombott-2.0rc1/ombott/error.html
--rw-rw-rw-   0        0        0     1163 2021-08-29 00:12:13.000000 ombott-2.0rc1/ombott/error_render.py
--rw-rw-rw-   0        0        0      146 2021-08-27 13:59:22.000000 ombott-2.0rc1/ombott/errors.py
--rw-rw-rw-   0        0        0     2848 2023-12-07 16:58:37.000000 ombott-2.0rc1/ombott/mixable.py
--rw-rw-rw-   0        0        0    16987 2023-12-08 21:10:16.000000 ombott-2.0rc1/ombott/ombott.py
-drwxrwxrwx   0        0        0        0 2023-12-08 21:37:13.940806 ombott-2.0rc1/ombott/request_pkg/
--rw-rw-rw-   0        0        0       52 2023-12-07 16:58:37.000000 ombott-2.0rc1/ombott/request_pkg/__init__.py
--rw-rw-rw-   0        0        0     9881 2023-12-08 20:38:40.000000 ombott-2.0rc1/ombott/request_pkg/body_mixin.py
--rw-rw-rw-   0        0        0      187 2023-12-07 16:58:37.000000 ombott-2.0rc1/ombott/request_pkg/errors.py
--rw-rw-rw-   0        0        0    11938 2023-12-07 16:58:37.000000 ombott-2.0rc1/ombott/request_pkg/helpers.py
--rw-rw-rw-   0        0        0    16055 2023-12-08 21:20:49.000000 ombott-2.0rc1/ombott/request_pkg/multipart.py
--rw-rw-rw-   0        0        0     8668 2023-12-07 16:58:37.000000 ombott-2.0rc1/ombott/request_pkg/props_mixin.py
--rw-rw-rw-   0        0        0     4560 2023-12-07 16:58:37.000000 ombott-2.0rc1/ombott/request_pkg/request.py
--rw-rw-rw-   0        0        0    11323 2023-12-07 16:58:37.000000 ombott-2.0rc1/ombott/response.py
-drwxrwxrwx   0        0        0        0 2023-12-08 21:37:13.947806 ombott-2.0rc1/ombott/router/
--rw-rw-rw-   0        0        0       65 2021-08-17 10:58:08.000000 ombott-2.0rc1/ombott/router/__init__.py
--rw-rw-rw-   0        0        0      544 2021-08-17 05:45:18.000000 ombott-2.0rc1/ombott/router/errors.py
--rw-rw-rw-   0        0        0     2612 2023-12-07 16:58:37.000000 ombott-2.0rc1/ombott/router/filter_factory.py
--rw-rw-rw-   0        0        0     4518 2023-12-07 16:58:37.000000 ombott-2.0rc1/ombott/router/parser.py
--rw-rw-rw-   0        0        0    17991 2023-12-07 16:58:37.000000 ombott-2.0rc1/ombott/router/radidict.py
--rw-rw-rw-   0        0        0    14037 2023-12-07 16:58:37.000000 ombott-2.0rc1/ombott/router/radirouter.py
--rw-rw-rw-   0        0        0     2445 2023-12-07 16:58:37.000000 ombott-2.0rc1/ombott/router/sym_stream.py
--rw-rw-rw-   0        0        0     9875 2023-12-07 16:58:37.000000 ombott-2.0rc1/ombott/server_adapters.py
--rw-rw-rw-   0        0        0     4942 2023-12-07 16:58:37.000000 ombott-2.0rc1/ombott/static_stream.py
-drwxrwxrwx   0        0        0        0 2023-12-08 21:37:13.962806 ombott-2.0rc1/ombott.egg-info/
--rw-rw-rw-   0        0        0      976 2023-12-08 21:37:13.000000 ombott-2.0rc1/ombott.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1192 2023-12-08 21:37:13.000000 ombott-2.0rc1/ombott.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-08 21:37:13.000000 ombott-2.0rc1/ombott.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-12-08 21:37:13.000000 ombott-2.0rc1/ombott.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-08 21:37:13.964807 ombott-2.0rc1/setup.cfg
--rw-rw-rw-   0        0        0     1150 2023-12-07 16:58:37.000000 ombott-2.0rc1/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-08 21:37:13.949805 ombott-2.0rc1/tests/
--rw-rw-rw-   0        0        0        0 2023-12-07 22:20:45.000000 ombott-2.0rc1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-08 21:37:13.956806 ombott-2.0rc1/tests/request/
--rw-rw-rw-   0        0        0        0 2021-08-16 22:37:23.000000 ombott-2.0rc1/tests/request/__init__.py
--rw-rw-rw-   0        0        0     1824 2023-12-07 16:58:37.000000 ombott-2.0rc1/tests/request/test_body_read.py
--rw-rw-rw-   0        0        0     1517 2023-12-07 16:58:37.000000 ombott-2.0rc1/tests/request/test_helpers.py
--rw-rw-rw-   0        0        0     2955 2023-12-08 21:24:23.000000 ombott-2.0rc1/tests/request/test_multipart.py
--rw-rw-rw-   0        0        0     3778 2023-12-07 16:58:37.000000 ombott-2.0rc1/tests/request/test_props.py
--rw-rw-rw-   0        0        0     1563 2023-12-07 16:58:37.000000 ombott-2.0rc1/tests/request/test_thread.py
--rw-rw-rw-   0        0        0     1327 2021-08-30 10:38:28.000000 ombott-2.0rc1/tests/request/test_thread_crossref.py
-drwxrwxrwx   0        0        0        0 2023-12-08 21:37:13.958806 ombott-2.0rc1/tests/response/
--rw-rw-rw-   0        0        0        0 2021-08-16 22:37:23.000000 ombott-2.0rc1/tests/response/__init__.py
--rw-rw-rw-   0        0        0     3085 2021-08-27 22:57:54.000000 ombott-2.0rc1/tests/response/test_static_file.py
--rw-rw-rw-   0        0        0     2285 2021-08-16 23:13:20.000000 ombott-2.0rc1/tests/response/test_thread.py
-drwxrwxrwx   0        0        0        0 2023-12-08 21:37:13.961805 ombott-2.0rc1/tests/router/
--rw-rw-rw-   0        0        0        0 2021-08-16 22:37:23.000000 ombott-2.0rc1/tests/router/__init__.py
--rw-rw-rw-   0        0        0     1276 2023-12-07 16:58:37.000000 ombott-2.0rc1/tests/router/test_route.py
--rw-rw-rw-   0        0        0     5133 2023-12-07 16:58:37.000000 ombott-2.0rc1/tests/router/test_router.py
--rw-rw-rw-   0        0        0     1409 2021-08-29 22:38:33.000000 ombott-2.0rc1/tests/test_simple_config.py
+drwxrwxrwx   0        0        0        0 2023-12-09 22:52:00.556393 ombott-2.0rc2/
+-rw-rw-rw-   0        0        0     1138 2021-08-02 22:15:45.000000 ombott-2.0rc2/LICENSE
+-rw-rw-rw-   0        0        0      976 2023-12-09 22:52:00.555423 ombott-2.0rc2/PKG-INFO
+-rw-rw-rw-   0        0        0       80 2021-08-02 21:55:10.000000 ombott-2.0rc2/README.md
+drwxrwxrwx   0        0        0        0 2023-12-09 22:52:00.517132 ombott-2.0rc2/ombott/
+-rw-rw-rw-   0        0        0      785 2023-12-07 16:58:37.000000 ombott-2.0rc2/ombott/__init__.py
+-rw-rw-rw-   0        0        0    10855 2023-12-07 16:58:37.000000 ombott-2.0rc2/ombott/common_helpers.py
+-rw-rw-rw-   0        0        0      692 2021-08-28 23:59:49.000000 ombott-2.0rc2/ombott/error.html
+-rw-rw-rw-   0        0        0     1163 2021-08-29 00:12:13.000000 ombott-2.0rc2/ombott/error_render.py
+-rw-rw-rw-   0        0        0      146 2021-08-27 13:59:22.000000 ombott-2.0rc2/ombott/errors.py
+-rw-rw-rw-   0        0        0     2848 2023-12-07 16:58:37.000000 ombott-2.0rc2/ombott/mixable.py
+-rw-rw-rw-   0        0        0    16987 2023-12-09 22:49:02.000000 ombott-2.0rc2/ombott/ombott.py
+drwxrwxrwx   0        0        0        0 2023-12-09 22:52:00.531004 ombott-2.0rc2/ombott/request_pkg/
+-rw-rw-rw-   0        0        0       52 2023-12-07 16:58:37.000000 ombott-2.0rc2/ombott/request_pkg/__init__.py
+-rw-rw-rw-   0        0        0     9881 2023-12-09 00:00:10.000000 ombott-2.0rc2/ombott/request_pkg/body_mixin.py
+-rw-rw-rw-   0        0        0      187 2023-12-07 16:58:37.000000 ombott-2.0rc2/ombott/request_pkg/errors.py
+-rw-rw-rw-   0        0        0    11938 2023-12-07 16:58:37.000000 ombott-2.0rc2/ombott/request_pkg/helpers.py
+-rw-rw-rw-   0        0        0    16232 2023-12-09 22:45:10.000000 ombott-2.0rc2/ombott/request_pkg/multipart.py
+-rw-rw-rw-   0        0        0     8668 2023-12-07 16:58:37.000000 ombott-2.0rc2/ombott/request_pkg/props_mixin.py
+-rw-rw-rw-   0        0        0     4560 2023-12-07 16:58:37.000000 ombott-2.0rc2/ombott/request_pkg/request.py
+-rw-rw-rw-   0        0        0    11323 2023-12-07 16:58:37.000000 ombott-2.0rc2/ombott/response.py
+drwxrwxrwx   0        0        0        0 2023-12-09 22:52:00.539384 ombott-2.0rc2/ombott/router/
+-rw-rw-rw-   0        0        0       65 2021-08-17 10:58:08.000000 ombott-2.0rc2/ombott/router/__init__.py
+-rw-rw-rw-   0        0        0      544 2021-08-17 05:45:18.000000 ombott-2.0rc2/ombott/router/errors.py
+-rw-rw-rw-   0        0        0     2612 2023-12-07 16:58:37.000000 ombott-2.0rc2/ombott/router/filter_factory.py
+-rw-rw-rw-   0        0        0     4518 2023-12-07 16:58:37.000000 ombott-2.0rc2/ombott/router/parser.py
+-rw-rw-rw-   0        0        0    17991 2023-12-07 16:58:37.000000 ombott-2.0rc2/ombott/router/radidict.py
+-rw-rw-rw-   0        0        0    14037 2023-12-07 16:58:37.000000 ombott-2.0rc2/ombott/router/radirouter.py
+-rw-rw-rw-   0        0        0     2445 2023-12-07 16:58:37.000000 ombott-2.0rc2/ombott/router/sym_stream.py
+-rw-rw-rw-   0        0        0     9875 2023-12-07 16:58:37.000000 ombott-2.0rc2/ombott/server_adapters.py
+-rw-rw-rw-   0        0        0     4942 2023-12-07 16:58:37.000000 ombott-2.0rc2/ombott/static_stream.py
+drwxrwxrwx   0        0        0        0 2023-12-09 22:52:00.554394 ombott-2.0rc2/ombott.egg-info/
+-rw-rw-rw-   0        0        0      976 2023-12-09 22:52:00.000000 ombott-2.0rc2/ombott.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1192 2023-12-09 22:52:00.000000 ombott-2.0rc2/ombott.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-09 22:52:00.000000 ombott-2.0rc2/ombott.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-12-09 22:52:00.000000 ombott-2.0rc2/ombott.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-12-09 22:52:00.556393 ombott-2.0rc2/setup.cfg
+-rw-rw-rw-   0        0        0     1150 2023-12-07 16:58:37.000000 ombott-2.0rc2/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-09 22:52:00.540392 ombott-2.0rc2/tests/
+-rw-rw-rw-   0        0        0        0 2023-12-07 22:20:45.000000 ombott-2.0rc2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-09 22:52:00.547392 ombott-2.0rc2/tests/request/
+-rw-rw-rw-   0        0        0        0 2021-08-16 22:37:23.000000 ombott-2.0rc2/tests/request/__init__.py
+-rw-rw-rw-   0        0        0     1824 2023-12-07 16:58:37.000000 ombott-2.0rc2/tests/request/test_body_read.py
+-rw-rw-rw-   0        0        0     1517 2023-12-07 16:58:37.000000 ombott-2.0rc2/tests/request/test_helpers.py
+-rw-rw-rw-   0        0        0     2955 2023-12-08 21:24:23.000000 ombott-2.0rc2/tests/request/test_multipart.py
+-rw-rw-rw-   0        0        0     3778 2023-12-07 16:58:37.000000 ombott-2.0rc2/tests/request/test_props.py
+-rw-rw-rw-   0        0        0     1563 2023-12-07 16:58:37.000000 ombott-2.0rc2/tests/request/test_thread.py
+-rw-rw-rw-   0        0        0     1327 2021-08-30 10:38:28.000000 ombott-2.0rc2/tests/request/test_thread_crossref.py
+drwxrwxrwx   0        0        0        0 2023-12-09 22:52:00.550393 ombott-2.0rc2/tests/response/
+-rw-rw-rw-   0        0        0        0 2021-08-16 22:37:23.000000 ombott-2.0rc2/tests/response/__init__.py
+-rw-rw-rw-   0        0        0     3085 2021-08-27 22:57:54.000000 ombott-2.0rc2/tests/response/test_static_file.py
+-rw-rw-rw-   0        0        0     2285 2021-08-16 23:13:20.000000 ombott-2.0rc2/tests/response/test_thread.py
+drwxrwxrwx   0        0        0        0 2023-12-09 22:52:00.553419 ombott-2.0rc2/tests/router/
+-rw-rw-rw-   0        0        0        0 2021-08-16 22:37:23.000000 ombott-2.0rc2/tests/router/__init__.py
+-rw-rw-rw-   0        0        0     1276 2023-12-07 16:58:37.000000 ombott-2.0rc2/tests/router/test_route.py
+-rw-rw-rw-   0        0        0     5133 2023-12-07 16:58:37.000000 ombott-2.0rc2/tests/router/test_router.py
+-rw-rw-rw-   0        0        0     1409 2021-08-29 22:38:33.000000 ombott-2.0rc2/tests/test_simple_config.py
```

### Comparing `ombott-2.0rc1/LICENSE` & `ombott-2.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/PKG-INFO` & `ombott-2.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ombott
-Version: 2.0rc1
+Version: 2.0rc2
 Summary: One More BOTTle
 Home-page: https://github.com/valq7711/ombott
 Author: Valery Kucherov <valq7711@gmail.com>
 Author-email: valq7711@gmail.com
 Maintainer: Valery Kucherov <valq7711@gmail.com>
 Maintainer-email: valq7711@gmail.com
 License: MIT
```

### Comparing `ombott-2.0rc1/ombott/__init__.py` & `ombott-2.0rc2/ombott/__init__.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/ombott/common_helpers.py` & `ombott-2.0rc2/ombott/common_helpers.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/ombott/error.html` & `ombott-2.0rc2/ombott/error.html`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/ombott/error_render.py` & `ombott-2.0rc2/ombott/error_render.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/ombott/mixable.py` & `ombott-2.0rc2/ombott/mixable.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/ombott/ombott.py` & `ombott-2.0rc2/ombott/ombott.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 )
 from .router import HookTypes, RadiRouter
 from .request_pkg import Request, errors as request_errors
 from .response import Response, HTTPResponse, HTTPError
 from . import server_adapters
 from . import error_render
 
-__version__ = "2.0rc1"
+__version__ = "2.0rc2"
 
 HTTP_METHODS = 'DELETE GET HEAD OPTIONS PATCH POST PUT'.split()
 
 
 @SimpleConfig.keys_holder
 class DefaultConfig(SimpleConfig):
     catchall = True
```

### Comparing `ombott-2.0rc1/ombott/request_pkg/body_mixin.py` & `ombott-2.0rc2/ombott/request_pkg/body_mixin.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/ombott/request_pkg/helpers.py` & `ombott-2.0rc2/ombott/request_pkg/helpers.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/ombott/request_pkg/multipart.py` & `ombott-2.0rc2/ombott/request_pkg/multipart.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Optional, Iterable, Union, Tuple, Dict
 from types import SimpleNamespace
 from collections import defaultdict
 from io import BytesIO
 import re
 
-from .errors import BodyParsingError, BodySizeError
+from ombott.request_pkg.errors import BodyParsingError, BodySizeError
 
 
 class BaseMarkupException(BodyParsingError):
     pass
 
 
 class InvalidBoundaryError(BaseMarkupException):
@@ -29,27 +29,27 @@
 
 class MatchTail:
     def __init__(self, token: bytes):
         self.token = token
         self.len = len(token)
         self.idx = idx = defaultdict(list)   # 1-based indices for each token symbol
         for i, c in enumerate(token, start=1):
-            idx[c].append(i)
+            idx[c].append([i, token[:i]])
 
-    def match_tail(self, s: bytes) -> Optional[int]:
-        slen = len(s)
-        assert slen <= self.len
-        idxs = self.idx.get(s[-1])
+    def match_tail(self, s: bytes, start: int, end: int) -> Optional[int]:
+        idxs = self.idx.get(s[end - 1])
         if idxs is None:
             return
-        token = self.token
-        for i in idxs:  # idxs is 1-based index, so 'abc'[:i] returns 'a', if i == 1
-            if slen < i:
+        slen = end - start
+        assert slen <= self.len
+        for i, thead in idxs:  # idxs is 1-based index
+            search_pos = slen - i
+            if search_pos < 0:
                 return
-            if token[:i] == s[-i:]:  # if token_head == s_tail
+            if s[start + search_pos:end] == thead:  # if s_tail == token_head
                 return i
 
 
 HYPHEN = b'-'
 HYPHENx2 = HYPHEN * 2
 CR = b'\r'
 LF = b'\n'
@@ -256,43 +256,45 @@
             self.trest_len = len(boundary)
 
         end_section = self._eat_data(chunk, base)
         if end_section is not None:
             return end_section
 
     def _eat_data(self, chunk: bytes, base: int):
+        chunk_len = len(chunk)
         token, tlen, trest, trest_len = self.token, self.tlen, self.trest, self.trest_len
         start = base
         mt = self.mt
+        part = None
         while True:
             end = start + tlen
-            part = chunk[start:end]
-            if len(part) < tlen:
+            if end > chunk_len:
+                part = chunk[start:]
                 break
             if trest is not None:
-                if part.startswith(trest):
+                if chunk[start:start + trest_len] == trest:   # part.startswith(trest):
                     data_end = start + trest_len - tlen
                     self.trest_len = self.trest = None
                     return data_end
                 else:
                     trest_len = trest = None
-            matched_len = mt.match_tail(part)
+            matched_len = mt.match_tail(chunk, start, end)
             if matched_len is not None:
                 if matched_len == tlen:
                     self.trest_len = self.trest = None
                     return start
                 else:
                     trest_len, trest = tlen - matched_len, token[matched_len:]
 
             start += tlen
 
         # process the tail of the chunk
         if part:
+            part_len = len(part)
             if trest is not None:
-                part_len = len(part)
                 if part_len < trest_len:
                     if trest.startswith(part):
                         trest_len -= part_len
                         trest = trest[part_len:]
                         part = None
                     else:
                         trest_len = trest = None
@@ -301,15 +303,15 @@
                         data_end = start + trest_len - tlen
                         self.trest_len = self.trest = None
                         return data_end
                     trest_len = trest = None
 
             if part is not None:
                 assert trest is None
-                matched_len = mt.match_tail(part)
+                matched_len = mt.match_tail(part, 0, part_len)
                 if matched_len is not None:
                     trest_len, trest = tlen - matched_len, token[matched_len:]
 
         self.trest_len, self.trest = trest_len, trest
 
 
 class MultipartMarkup:
@@ -482,9 +484,7 @@
             field = cls()
             has_read = field.read(src, headers_slice, data_slice, max_read=max_read)
             max_read -= has_read
             yield field
 
             headers = next(iter_markup, None)
             data = next(iter_markup, None)
-
-
```

### Comparing `ombott-2.0rc1/ombott/request_pkg/props_mixin.py` & `ombott-2.0rc2/ombott/request_pkg/props_mixin.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/ombott/request_pkg/request.py` & `ombott-2.0rc2/ombott/request_pkg/request.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/ombott/response.py` & `ombott-2.0rc2/ombott/response.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/ombott/router/errors.py` & `ombott-2.0rc2/ombott/router/errors.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/ombott/router/filter_factory.py` & `ombott-2.0rc2/ombott/router/filter_factory.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/ombott/router/parser.py` & `ombott-2.0rc2/ombott/router/parser.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/ombott/router/radidict.py` & `ombott-2.0rc2/ombott/router/radidict.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/ombott/router/radirouter.py` & `ombott-2.0rc2/ombott/router/radirouter.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/ombott/router/sym_stream.py` & `ombott-2.0rc2/ombott/router/sym_stream.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/ombott/server_adapters.py` & `ombott-2.0rc2/ombott/server_adapters.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/ombott/static_stream.py` & `ombott-2.0rc2/ombott/static_stream.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/ombott.egg-info/PKG-INFO` & `ombott-2.0rc2/ombott.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ombott
-Version: 2.0rc1
+Version: 2.0rc2
 Summary: One More BOTTle
 Home-page: https://github.com/valq7711/ombott
 Author: Valery Kucherov <valq7711@gmail.com>
 Author-email: valq7711@gmail.com
 Maintainer: Valery Kucherov <valq7711@gmail.com>
 Maintainer-email: valq7711@gmail.com
 License: MIT
```

### Comparing `ombott-2.0rc1/ombott.egg-info/SOURCES.txt` & `ombott-2.0rc2/ombott.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/setup.py` & `ombott-2.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/tests/request/test_body_read.py` & `ombott-2.0rc2/tests/request/test_body_read.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/tests/request/test_helpers.py` & `ombott-2.0rc2/tests/request/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/tests/request/test_multipart.py` & `ombott-2.0rc2/tests/request/test_multipart.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/tests/request/test_props.py` & `ombott-2.0rc2/tests/request/test_props.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/tests/request/test_thread.py` & `ombott-2.0rc2/tests/request/test_thread.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/tests/request/test_thread_crossref.py` & `ombott-2.0rc2/tests/request/test_thread_crossref.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/tests/response/test_static_file.py` & `ombott-2.0rc2/tests/response/test_static_file.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/tests/response/test_thread.py` & `ombott-2.0rc2/tests/response/test_thread.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/tests/router/test_route.py` & `ombott-2.0rc2/tests/router/test_route.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/tests/router/test_router.py` & `ombott-2.0rc2/tests/router/test_router.py`

 * *Files identical despite different names*

### Comparing `ombott-2.0rc1/tests/test_simple_config.py` & `ombott-2.0rc2/tests/test_simple_config.py`

 * *Files identical despite different names*

