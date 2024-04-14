# Comparing `tmp/rtorrent_rpc-0.2.0.tar.gz` & `tmp/rtorrent_rpc-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtorrent_rpc-0.2.0.tar", max compression
+gzip compressed data, was "rtorrent_rpc-0.2.1.tar", max compression
```

## Comparing `rtorrent_rpc-0.2.0.tar` & `rtorrent_rpc-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1084 2023-11-08 17:16:23.690656 rtorrent_rpc-0.2.0/LICENSE
--rw-r--r--   0        0        0     2449 2023-11-08 17:16:23.690656 rtorrent_rpc-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1077 2023-11-08 17:16:23.690656 rtorrent_rpc-0.2.0/readme.md
--rw-r--r--   0        0        0    27948 2023-11-08 17:16:23.690656 rtorrent_rpc-0.2.0/rtorrent_rpc/__init__.py
--rw-r--r--   0        0        0     2688 2023-11-08 17:16:23.690656 rtorrent_rpc-0.2.0/rtorrent_rpc/helper.py
--rw-r--r--   0        0        0        0 2023-11-08 17:16:23.690656 rtorrent_rpc-0.2.0/rtorrent_rpc/py.typed
--rw-r--r--   0        0        0     3889 2023-11-08 17:16:23.690656 rtorrent_rpc-0.2.0/rtorrent_rpc/scgi.py
--rw-r--r--   0        0        0     1911 1970-01-01 00:00:00.000000 rtorrent_rpc-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-04-14 10:35:37.157762 rtorrent_rpc-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2445 2024-04-14 10:35:37.157762 rtorrent_rpc-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1077 2024-04-14 10:35:37.157762 rtorrent_rpc-0.2.1/readme.md
+-rw-r--r--   0        0        0    27945 2024-04-14 10:35:37.157762 rtorrent_rpc-0.2.1/rtorrent_rpc/__init__.py
+-rw-r--r--   0        0        0     2668 2024-04-14 10:35:37.157762 rtorrent_rpc-0.2.1/rtorrent_rpc/helper.py
+-rw-r--r--   0        0        0        0 2024-04-14 10:35:37.157762 rtorrent_rpc-0.2.1/rtorrent_rpc/py.typed
+-rw-r--r--   0        0        0     3889 2024-04-14 10:35:37.157762 rtorrent_rpc-0.2.1/rtorrent_rpc/scgi.py
+-rw-r--r--   0        0        0     1909 1970-01-01 00:00:00.000000 rtorrent_rpc-0.2.1/PKG-INFO
```

### Comparing `rtorrent_rpc-0.2.0/LICENSE` & `rtorrent_rpc-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.2.0/pyproject.toml` & `rtorrent_rpc-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rtorrent-rpc"
-version = "0.2.0"
+version = "0.2.1"
 description = "Typed rtorrent rpc client"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'readme.md'
 repository = 'https://github.com/trim21/rtorrent-rpc'
 license = 'MIT'
 packages = [{ include = 'rtorrent_rpc' }]
 keywords = ['rtorrent', 'rpc']
@@ -21,32 +21,32 @@
     'Programming Language :: Python :: 3.11',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 # dependencies
 typing-extensions = ">=4.7.1"
-bencode-py = "^4.0.0"
+bencode2 = "^0.0.6"
 
 [tool.poetry.group.docs.dependencies]
 sphinx = { version = "^7.0.0", python = "^3.9" }
-furo = { version = "^2023.5.20", python = "^3.9" }
+furo = { version = "^2024.0.0", python = "^3.9" }
 
 [tool.poetry.group.dev.dependencies]
 # tests
-pytest = "==7.4.3"
+pytest = "==8.1.1"
 pytest-github-actions-annotate-failures = "==0.2.0"
-coverage = "==7.3.2"
+coverage = "==7.4.4"
 
 # linter and formatter
-pre-commit = { version = "==3.5.0", markers = "implementation_name != 'pypy'", python = "^3.9" }
+pre-commit = { version = "==3.7.0", markers = "implementation_name != 'pypy'", python = "^3.9" }
 #mypy = { version = "==1.4.1", markers = "implementation_name != 'pypy'", python = "^3.9" }
-ruff = "0.1.4"
-sphinx-autobuild = "2021.3.14"
-mypy = "1.6.1"
+ruff = "0.3.4"
+sphinx-autobuild = "2024.2.4"
+mypy = "1.9.0"
 
 [tool.poetry-plugin-bump]
 commit_msg = 'bump: v{version}'
 
 [tool.pytest.ini_options]
 addopts = '-rav -Werror'
```

### Comparing `rtorrent_rpc-0.2.0/readme.md` & `rtorrent_rpc-0.2.1/readme.md`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.2.0/rtorrent_rpc/__init__.py` & `rtorrent_rpc-0.2.1/rtorrent_rpc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import time
 import urllib.parse
 import xmlrpc.client
 from collections.abc import Iterable
 from typing import Any, Literal, Protocol, TypeAlias, TypedDict
 from urllib.parse import quote
 
-import bencodepy
+import bencode2
 from typing_extensions import NotRequired
 
 from .scgi import SCGIServerProxy
 
 __all__ = ["RTorrent", "MultiCall"]
 
 Unknown: TypeAlias = Any
@@ -155,16 +155,16 @@
             f"d.custom.set=addtime,{int(time.time())}",
         ]
 
         if tags:
             params.append(f'd.custom1.set="{_encode_tags(tags)}"')
 
         if self.rutorrent_compatibility:
-            t = bencodepy.bdecode(content)
-            if b"comment" in t:
+            t = bencode2.bdecode(content)
+            if "comment" in t:
                 params.append(
                     f'd.custom2.set="VRS24mrker{quote(t[b"comment"].decode().strip())}"'
                 )
 
         self.rpc.load.raw_start_verbose(*params)  # type: ignore
 
     def stop_torrent(self, info_hash: str) -> None:
```

### Comparing `rtorrent_rpc-0.2.0/rtorrent_rpc/helper.py` & `rtorrent_rpc-0.2.1/rtorrent_rpc/helper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import hashlib
 from pathlib import Path
 from typing import Any
 from urllib.parse import unquote
 
-import bencodepy
+import bencode2
 
 __all__ = [
     "add_completed_resume_file",
     "get_torrent_info_hash",
     "parse_tags",
     "parse_comment",
 ]
@@ -28,61 +28,61 @@
     if s.startswith("VRS24mrker"):
         return unquote(s.removeprefix("VRS24mrker"))
     return s
 
 
 def get_torrent_info_hash(content: bytes) -> str:
     """get torrent info_hash in low case string"""
-    data = bencodepy.bdecode(content)
-    return hashlib.sha1(bencodepy.bencode(data[b"info"])).hexdigest()
+    data = bencode2.bdecode(content)
+    return hashlib.sha1(bencode2.bencode(data[b"info"])).hexdigest()
 
 
 def add_completed_resume_file(base_save_path: Path, torrent_content: bytes) -> bytes:
     """update torrent content, add resume data to torrent.
 
     based on [rtorrent_fast_resume.pl](https://github.com/rakshasa/rtorrent/blob/master/doc/rtorrent_fast_resume.pl)
     """
-    data: dict[bytes, Any] = bencodepy.bdecode(torrent_content)
+    data: dict[str, Any] = bencode2.bdecode(torrent_content, str_key=True)
 
-    piece_length = data[b"info"][b"piece length"]
+    piece_length = data["info"][b"piece length"]
     files = []
 
-    t_files = data[b"info"].get(b"files")
+    t_files = data["info"].get("files")
 
-    piece_count = int(len(data[b"info"][b"pieces"]) / 20)
+    piece_count = int(len(data["info"]["pieces"]) / 20)
     if t_files:
         for file in t_files:
             file_path = base_save_path.joinpath(*[p.decode() for p in file[b"path"]])
             if not file_path.exists():
-                files.append({b"complete": 0, b"mtime": 0, b"priority": 0})
+                files.append({"complete": 0, "mtime": 0, "priority": 0})
                 continue
 
             stat = file_path.lstat()
             if stat.st_size == file[b"length"]:
                 files.append(
                     {
-                        b"complete": int(file[b"length"] / piece_length),
-                        b"mtime": int(stat.st_mtime),
-                        b"priority": 1,
+                        "complete": int(file["length"] / piece_length),
+                        "mtime": int(stat.st_mtime),
+                        "priority": 1,
                     }
                 )
             else:
-                files.append({b"complete": 0, b"mtime": 0, b"priority": 1})
+                files.append({"complete": 0, "mtime": 0, "priority": 1})
     else:
         try:
-            stat = base_save_path.joinpath(data[b"info"][b"name"].decode()).lstat()
+            stat = base_save_path.joinpath(data["info"]["name"].decode()).lstat()
         except FileNotFoundError:
             return torrent_content
 
-        if stat.st_size == data[b"info"][b"length"]:
+        if stat.st_size == data["info"]["length"]:
             files.append(
-                {b"complete": piece_count, b"mtime": int(stat.st_mtime), b"priority": 1}
+                {"complete": piece_count, "mtime": int(stat.st_mtime), "priority": 1}
             )
         else:
             return torrent_content
 
-    data[b"rtorrent"] = None
-    del data[b"rtorrent"]
+    data["rtorrent"] = None
+    del data["rtorrent"]
 
-    data[b"libtorrent_resume"] = {b"bitfield": piece_count, b"files": files}
+    data["libtorrent_resume"] = {"bitfield": piece_count, "files": files}
 
-    return bencodepy.bencode(data)
+    return bencode2.bencode(data)
```

### Comparing `rtorrent_rpc-0.2.0/rtorrent_rpc/scgi.py` & `rtorrent_rpc-0.2.1/rtorrent_rpc/scgi.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.2.0/PKG-INFO` & `rtorrent_rpc-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtorrent-rpc
-Version: 0.2.0
+Version: 0.2.1
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
-Requires-Dist: bencode-py (>=4.0.0,<5.0.0)
+Requires-Dist: bencode2 (>=0.0.6,<0.0.7)
 Requires-Dist: typing-extensions (>=4.7.1)
 Project-URL: Repository, https://github.com/trim21/rtorrent-rpc
 Description-Content-Type: text/markdown
 
 # Typed rtorrent rpc client
 
 [![PyPI](https://img.shields.io/pypi/v/rtorrent-rpc)](https://pypi.org/project/rtorrent-rpc/)
```

