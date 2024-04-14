# Comparing `tmp/rtorrent_rpc-0.2.2.tar.gz` & `tmp/rtorrent_rpc-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtorrent_rpc-0.2.2.tar", max compression
+gzip compressed data, was "rtorrent_rpc-0.2.3.tar", max compression
```

## Comparing `rtorrent_rpc-0.2.2.tar` & `rtorrent_rpc-0.2.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1084 2024-04-14 11:22:29.741783 rtorrent_rpc-0.2.2/LICENSE
--rw-r--r--   0        0        0     2449 2024-04-14 11:22:29.741783 rtorrent_rpc-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1077 2024-04-14 11:22:29.741783 rtorrent_rpc-0.2.2/readme.md
--rw-r--r--   0        0        0    27945 2024-04-14 11:22:29.741783 rtorrent_rpc-0.2.2/rtorrent_rpc/__init__.py
--rw-r--r--   0        0        0     2668 2024-04-14 11:22:29.741783 rtorrent_rpc-0.2.2/rtorrent_rpc/helper.py
--rw-r--r--   0        0        0        0 2024-04-14 11:22:29.741783 rtorrent_rpc-0.2.2/rtorrent_rpc/py.typed
--rw-r--r--   0        0        0     3889 2024-04-14 11:22:29.741783 rtorrent_rpc-0.2.2/rtorrent_rpc/scgi.py
--rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 rtorrent_rpc-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2024-04-14 19:12:13.766070 rtorrent_rpc-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2466 2024-04-14 19:12:13.766070 rtorrent_rpc-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1077 2024-04-14 19:12:13.766070 rtorrent_rpc-0.2.3/readme.md
+-rw-r--r--   0        0        0    27945 2024-04-14 19:12:13.766070 rtorrent_rpc-0.2.3/rtorrent_rpc/__init__.py
+-rw-r--r--   0        0        0     2665 2024-04-14 19:12:13.766070 rtorrent_rpc-0.2.3/rtorrent_rpc/helper.py
+-rw-r--r--   0        0        0        0 2024-04-14 19:12:13.766070 rtorrent_rpc-0.2.3/rtorrent_rpc/py.typed
+-rw-r--r--   0        0        0     3889 2024-04-14 19:12:13.766070 rtorrent_rpc-0.2.3/rtorrent_rpc/scgi.py
+-rw-r--r--   0        0        0     1905 1970-01-01 00:00:00.000000 rtorrent_rpc-0.2.3/PKG-INFO
```

### Comparing `rtorrent_rpc-0.2.2/LICENSE` & `rtorrent_rpc-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.2.2/pyproject.toml` & `rtorrent_rpc-0.2.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "rtorrent-rpc"
-version = "0.2.2"
+version = "0.2.3"
 description = "Typed rtorrent rpc client"
 authors = ["Trim21 <i@trim21.me>"]
 readme = 'readme.md'
 repository = 'https://github.com/trim21/rtorrent-rpc'
 license = 'MIT'
 packages = [{ include = 'rtorrent_rpc' }]
 keywords = ['rtorrent', 'rpc']
@@ -36,15 +36,15 @@
 pytest = "==8.1.1"
 pytest-github-actions-annotate-failures = "==0.2.0"
 coverage = "==7.4.4"
 
 # linter and formatter
 pre-commit = { version = "==3.7.0", markers = "implementation_name != 'pypy'", python = "^3.9" }
 #mypy = { version = "==1.4.1", markers = "implementation_name != 'pypy'", python = "^3.9" }
-ruff = "0.3.4"
+ruff = "0.3.7"
 sphinx-autobuild = "2024.2.4"
 mypy = "1.9.0"
 
 [tool.poetry-plugin-bump]
 commit_msg = 'bump: v{version}'
 
 [tool.pytest.ini_options]
@@ -60,14 +60,17 @@
 
 platform = 'unix'
 
 [tool.black]
 target-version = ['py310']
 
 [tool.ruff]
+target-version = "py310"
+
+[tool.ruff.lint]
 select = [
     "B",
     "C",
     "E",
     "F",
     "G",
     "I",
@@ -125,9 +128,7 @@
     'TRY201',
     'TRY301',
     'PLR0912',
     'PLR0915',
     'PLR2004',
     'PGH003',
 ]
-
-target-version = "py310"
```

### Comparing `rtorrent_rpc-0.2.2/readme.md` & `rtorrent_rpc-0.2.3/readme.md`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.2.2/rtorrent_rpc/__init__.py` & `rtorrent_rpc-0.2.3/rtorrent_rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.2.2/rtorrent_rpc/helper.py` & `rtorrent_rpc-0.2.3/rtorrent_rpc/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,29 +39,29 @@
 def add_completed_resume_file(base_save_path: Path, torrent_content: bytes) -> bytes:
     """update torrent content, add resume data to torrent.
 
     based on [rtorrent_fast_resume.pl](https://github.com/rakshasa/rtorrent/blob/master/doc/rtorrent_fast_resume.pl)
     """
     data: dict[str, Any] = bencode2.bdecode(torrent_content, str_key=True)
 
-    piece_length = data["info"][b"piece length"]
+    piece_length = data["info"]["piece length"]
     files = []
 
     t_files = data["info"].get("files")
 
     piece_count = int(len(data["info"]["pieces"]) / 20)
     if t_files:
         for file in t_files:
-            file_path = base_save_path.joinpath(*[p.decode() for p in file[b"path"]])
+            file_path = base_save_path.joinpath(*[p.decode() for p in file["path"]])
             if not file_path.exists():
                 files.append({"complete": 0, "mtime": 0, "priority": 0})
                 continue
 
             stat = file_path.lstat()
-            if stat.st_size == file[b"length"]:
+            if stat.st_size == file["length"]:
                 files.append(
                     {
                         "complete": int(file["length"] / piece_length),
                         "mtime": int(stat.st_mtime),
                         "priority": 1,
                     }
                 )
```

### Comparing `rtorrent_rpc-0.2.2/rtorrent_rpc/scgi.py` & `rtorrent_rpc-0.2.3/rtorrent_rpc/scgi.py`

 * *Files identical despite different names*

### Comparing `rtorrent_rpc-0.2.2/PKG-INFO` & `rtorrent_rpc-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtorrent-rpc
-Version: 0.2.2
+Version: 0.2.3
 Summary: Typed rtorrent rpc client
 Home-page: https://github.com/trim21/rtorrent-rpc
 License: MIT
 Keywords: rtorrent,rpc
 Author: Trim21
 Author-email: i@trim21.me
 Requires-Python: >=3.10,<4.0
```

