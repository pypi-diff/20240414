# Comparing `tmp/rtorrent_rpc-0.2.1.tar.gz` & `tmp/rtorrent_rpc-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtorrent_rpc-0.2.1.tar", max compression
+gzip compressed data, was "rtorrent_rpc-0.2.2.tar", max compression
```

## Comparing `rtorrent_rpc-0.2.1.tar` & `rtorrent_rpc-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1084 2024-04-14 10:35:37.157762 rtorrent_rpc-0.2.1/LICENSE
--rw-r--r--   0        0        0     2445 2024-04-14 10:35:37.157762 rtorrent_rpc-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1077 2024-04-14 10:35:37.157762 rtorrent_rpc-0.2.1/readme.md
--rw-r--r--   0        0        0    27945 2024-04-14 10:35:37.157762 rtorrent_rpc-0.2.1/rtorrent_rpc/__init__.py
--rw-r--r--   0        0        0     2668 2024-04-14 10:35:37.157762 rtorrent_rpc-0.2.1/rtorrent_rpc/helper.py
--rw-r--r--   0        0        0        0 2024-04-14 10:35:37.157762 rtorrent_rpc-0.2.1/rtorrent_rpc/py.typed
--rw-r--r--   0        0        0     3889 2024-04-14 10:35:37.157762 rtorrent_rpc-0.2.1/rtorrent_rpc/scgi.py
--rw-r--r--   0        0        0     1909 1970-01-01 00:00:00.000000 rtorrent_rpc-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-04-14 11:22:29.741783 rtorrent_rpc-0.2.2/LICENSE
+-rw-r--r--   0        0        0     2449 2024-04-14 11:22:29.741783 rtorrent_rpc-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1077 2024-04-14 11:22:29.741783 rtorrent_rpc-0.2.2/readme.md
+-rw-r--r--   0        0        0    27945 2024-04-14 11:22:29.741783 rtorrent_rpc-0.2.2/rtorrent_rpc/__init__.py
+-rw-r--r--   0        0        0     2668 2024-04-14 11:22:29.741783 rtorrent_rpc-0.2.2/rtorrent_rpc/helper.py
+-rw-r--r--   0        0        0        0 2024-04-14 11:22:29.741783 rtorrent_rpc-0.2.2/rtorrent_rpc/py.typed
+-rw-r--r--   0        0        0     3889 2024-04-14 11:22:29.741783 rtorrent_rpc-0.2.2/rtorrent_rpc/scgi.py
+-rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 rtorrent_rpc-0.2.2/PKG-INFO
```

### Comparing `rtorrent_rpc-0.2.1/LICENSE` & `rtorrent_rpc-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.2.1/pyproject.toml` & `rtorrent_rpc-0.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rtorrent-rpc"
-version = "0.2.1"
+version = "0.2.2"
 description = "Typed rtorrent rpc client"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'readme.md'
 repository = 'https://github.com/trim21/rtorrent-rpc'
 license = 'MIT'
 packages = [{ include = 'rtorrent_rpc' }]
 keywords = ['rtorrent', 'rpc']
@@ -21,15 +21,15 @@
     'Programming Language :: Python :: 3.11',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 # dependencies
 typing-extensions = ">=4.7.1"
-bencode2 = "^0.0.6"
+bencode2 = ">=0.0.6,<1"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = { version = "^7.0.0", python = "^3.9" }
 furo = { version = "^2024.0.0", python = "^3.9" }
 
 [tool.poetry.group.dev.dependencies]
 # tests
```

### Comparing `rtorrent_rpc-0.2.1/readme.md` & `rtorrent_rpc-0.2.2/readme.md`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.2.1/rtorrent_rpc/__init__.py` & `rtorrent_rpc-0.2.2/rtorrent_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.2.1/rtorrent_rpc/helper.py` & `rtorrent_rpc-0.2.2/rtorrent_rpc/helper.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.2.1/rtorrent_rpc/scgi.py` & `rtorrent_rpc-0.2.2/rtorrent_rpc/scgi.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.2.1/PKG-INFO` & `rtorrent_rpc-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtorrent-rpc
-Version: 0.2.1
+Version: 0.2.2
 Summary: Typed rtorrent rpc client
 Home-page: https://github.com/trim21/rtorrent-rpc
 License: MIT
 Keywords: rtorrent,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.10,<4.0
@@ -12,15 +12,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Dist: bencode2 (>=0.0.6,<0.0.7)
+Requires-Dist: bencode2 (>=0.0.6,<1)
 Requires-Dist: typing-extensions (>=4.7.1)
 Project-URL: Repository, https://github.com/trim21/rtorrent-rpc
 Description-Content-Type: text/markdown
 
 # Typed rtorrent rpc client
 
 [![PyPI](https://img.shields.io/pypi/v/rtorrent-rpc)](https://pypi.org/project/rtorrent-rpc/)
```

