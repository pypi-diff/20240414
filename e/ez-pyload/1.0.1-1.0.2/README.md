# Comparing `tmp/ez_pyload-1.0.1.tar.gz` & `tmp/ez_pyload-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez_pyload-1.0.1.tar", max compression
+gzip compressed data, was "ez_pyload-1.0.2.tar", max compression
```

## Comparing `ez_pyload-1.0.1.tar` & `ez_pyload-1.0.2.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1356 2024-04-13 06:43:40.913054 ez_pyload-1.0.1/README.md
--rw-r--r--   0        0        0       39 2024-04-13 06:43:40.913054 ez_pyload-1.0.1/ez_pyload/__init__.py
--rw-r--r--   0        0        0      613 2024-04-13 06:43:40.913054 ez_pyload-1.0.1/ez_pyload/__main__.py
--rw-r--r--   0        0        0     3128 2024-04-13 06:43:40.913054 ez_pyload-1.0.1/ez_pyload/download.py
--rw-r--r--   0        0        0      451 2024-04-13 06:43:40.913054 ez_pyload-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2142 1970-01-01 00:00:00.000000 ez_pyload-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1356 2024-04-14 16:49:11.900468 ez_pyload-1.0.2/README.md
+-rw-r--r--   0        0        0       39 2024-04-14 16:49:11.900468 ez_pyload-1.0.2/ez_pyload/__init__.py
+-rw-r--r--   0        0        0      613 2024-04-14 16:49:11.900468 ez_pyload-1.0.2/ez_pyload/__main__.py
+-rw-r--r--   0        0        0     2852 2024-04-14 16:49:11.900468 ez_pyload-1.0.2/ez_pyload/download.py
+-rw-r--r--   0        0        0     1125 2024-04-14 16:49:11.900468 ez_pyload-1.0.2/ez_pyload/patches.py
+-rw-r--r--   0        0        0      451 2024-04-14 16:49:11.904468 ez_pyload-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2142 1970-01-01 00:00:00.000000 ez_pyload-1.0.2/PKG-INFO
```

### Comparing `ez_pyload-1.0.1/README.md` & `ez_pyload-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ez_pyload-1.0.1/ez_pyload/__main__.py` & `ez_pyload-1.0.2/ez_pyload/__main__.py`

 * *Files identical despite different names*

### Comparing `ez_pyload-1.0.1/ez_pyload/download.py` & `ez_pyload-1.0.2/ez_pyload/download.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,21 @@
 import logging
 import os
 import shutil
-import sys
 from pathlib import Path
 
 cwd = os.getcwd() # pyload messes with cwd
 
 from pyload.core import Core
 from pyload.core.datatypes.pyfile import PyFile
-from pyload.core.log_factory import LogFactory
 from pyload.core.threads.download_thread import DownloadThread
 
-os.chdir(cwd)
+from .patches import logger
 
-logger = logging.getLogger("pyload")
-consoleform = logging.Formatter(
-    LogFactory.LINEFORMAT, LogFactory.DATEFORMAT, LogFactory.LINESTYLE
-)
-consolehdlr = logging.StreamHandler(sys.stdout)
-consolehdlr.setFormatter(consoleform)
-logger.addHandler(consolehdlr)
-def new_get_logger(self, name: str):
-    return logger
-LogFactory.get_logger = new_get_logger
+os.chdir(cwd)
 
 import tempfile
 
 
 def _download(pyload: Core, url: str, pkg_name: str = "unknown", pkg_dir: str = "unknown") -> bool:
     urls = [url]
     data = pyload.plugin_manager.parse_urls(urls)
@@ -69,22 +58,25 @@
     Returns:
         Path: Path to downloaded file/folder
     """
     download_dir = Path(download_dir)
     debug = loglevel == logging.DEBUG
     logger.setLevel(loglevel)
     tmp = "."
-    with tempfile.TemporaryDirectory(".ez-pyload", ignore_cleanup_errors=True) as tmp:
+    with tempfile.TemporaryDirectory(".ez-pyload") as tmp:
         pyload = Core(tmp, "tmpdir", "storage", debug)
         is_dir = _download(pyload, url)
         src_path = next((Path(tmp) / "data" / "storage" / "unknown").glob("*"))
         name = src_path.name
         dst_path = download_dir / name
         # pyload messes with cwd again
         os.chdir(cwd)
         if is_dir:
             shutil.copytree(src_path, dst_path)
         else:
             shutil.copy(src_path, dst_path)
-        pyload.stop()
-        pyload.db.shutdown()
+        # don't care about corrupting data,
+        # just need to release connections NOW
+        # so we can clean up tempdir
+        pyload.db.c.close()
+        pyload.db.conn.close()
         return dst_path
```

### Comparing `ez_pyload-1.0.1/PKG-INFO` & `ez_pyload-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez-pyload
-Version: 1.0.1
+Version: 1.0.2
 Summary: Wrapper for pyLoad to allow downloading files through Python (no webserver). Includes CLI
 License: MIT
 Author: 7x11x13
 Author-email: x7x11x13@gmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

