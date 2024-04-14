# Comparing `tmp/sshared-0.2.0.tar.gz` & `tmp/sshared-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sshared-0.2.0.tar", max compression
+gzip compressed data, was "sshared-0.3.0.tar", max compression
```

## Comparing `sshared-0.2.0.tar` & `sshared-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,13 @@
--rw-r--r--   0        0        0     1063 2024-03-31 00:23:56.619435 sshared-0.2.0/LICENSE
--rw-r--r--   0        0        0        0 2024-03-31 00:23:56.619435 sshared-0.2.0/README.md
--rw-r--r--   0        0        0     1106 2024-03-31 00:23:56.619435 sshared-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-03-31 00:23:56.619435 sshared-0.2.0/sshared/__init__.py
--rw-r--r--   0        0        0       74 2024-03-31 00:23:56.619435 sshared-0.2.0/sshared/mongo/__init__.py
--rw-r--r--   0        0        0     7113 2024-03-31 00:23:56.619435 sshared-0.2.0/sshared/mongo/document.py
--rw-r--r--   0        0        0      263 2024-03-31 00:23:56.619435 sshared-0.2.0/sshared/mongo/meta.py
--rw-r--r--   0        0        0      249 2024-03-31 00:23:56.619435 sshared-0.2.0/sshared/struct.py
--rw-r--r--   0        0        0      139 2024-03-31 00:23:56.623435 sshared-0.2.0/sshared/time.py
--rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 sshared-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-14 00:41:51.517836 sshared-0.3.0/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-14 00:41:51.517836 sshared-0.3.0/README.md
+-rw-r--r--   0        0        0     1111 2024-04-14 00:41:51.517836 sshared-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-14 00:41:51.517836 sshared-0.3.0/sshared/__init__.py
+-rw-r--r--   0        0        0       74 2024-04-14 00:41:51.517836 sshared-0.3.0/sshared/mongo/__init__.py
+-rw-r--r--   0        0        0     5962 2024-04-14 00:41:51.517836 sshared-0.3.0/sshared/mongo/document.py
+-rw-r--r--   0        0        0      263 2024-04-14 00:41:51.517836 sshared-0.3.0/sshared/mongo/meta.py
+-rw-r--r--   0        0        0     1687 2024-04-14 00:41:51.517836 sshared-0.3.0/sshared/retry/asyncio.py
+-rw-r--r--   0        0        0      229 2024-04-14 00:41:51.517836 sshared-0.3.0/sshared/retry/event.py
+-rw-r--r--   0        0        0     1660 2024-04-14 00:41:51.517836 sshared-0.3.0/sshared/retry/sync.py
+-rw-r--r--   0        0        0      249 2024-04-14 00:41:51.517836 sshared-0.3.0/sshared/struct.py
+-rw-r--r--   0        0        0      139 2024-04-14 00:41:51.517836 sshared-0.3.0/sshared/time.py
+-rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 sshared-0.3.0/PKG-INFO
```

### Comparing `sshared-0.2.0/LICENSE` & `sshared-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sshared-0.2.0/pyproject.toml` & `sshared-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sshared"
-version = "0.2.0"
+version = "0.3.0"
 description = "后端共享组件"
 authors = ["yezi <yehaowei20060411@qq.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/FHU-yezi/sshared"
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -40,10 +40,10 @@
     "ICN", "ISC", "N", "PERF", "PIE",
     "PT", "Q", "RET", "RSE", "RUF",
     "S", "SIM", "SLOT", "TCH", "UP",
     "W"
 ]
 lint.ignore = ["ANN101", "ANN102", "ISC001", "RUF001", "RUF002", "RUF003"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 
 "__init__.py" = ["F401"]
```

### Comparing `sshared-0.2.0/PKG-INFO` & `sshared-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sshared
-Version: 0.2.0
+Version: 0.3.0
 Summary: 后端共享组件
 Home-page: https://github.com/FHU-yezi/sshared
 License: MIT
 Author: yezi
 Author-email: yehaowei20060411@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

