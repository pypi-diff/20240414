# Comparing `tmp/tsk_monster-0.0.7.tar.gz` & `tmp/tsk_monster-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tsk_monster-0.0.7.tar", max compression
+gzip compressed data, was "tsk_monster-0.0.8.tar", max compression
```

## Comparing `tsk_monster-0.0.7.tar` & `tsk_monster-0.0.8.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      363 2024-04-13 17:57:20.490880 tsk_monster-0.0.7/README.md
--rw-r--r--   0        0        0      583 2024-04-13 17:57:55.078214 tsk_monster-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3424 2024-04-13 17:23:43.548774 tsk_monster-0.0.7/tsk_monster/__init__.py
--rw-r--r--   0        0        0      801 1970-01-01 00:00:00.000000 tsk_monster-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      363 2024-04-14 06:48:06.638346 tsk_monster-0.0.8/README.md
+-rw-r--r--   0        0        0      753 2024-04-14 12:37:29.439176 tsk_monster-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5853 2024-04-14 12:36:51.019552 tsk_monster-0.0.8/tsk_monster/__init__.py
+-rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 tsk_monster-0.0.8/PKG-INFO
```

### Comparing `tsk_monster-0.0.7/pyproject.toml` & `tsk_monster-0.0.8/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tsk-monster"
-version = "0.0.7"
+version = "0.0.8"
 description = ""
 authors = ["Gilad Kutiel <giladk@mobileye.com>"]
 readme = "README.md"
 
 [tool.poetry.urls]
 Homepage = "https://tsk.monster"
 Documentation = "https://tsk.monster"
@@ -19,10 +19,18 @@
 ruff = "^0.3.5"
 rope = "^1.13.0"
 autopep8 = "^2.1.0"
 isort = "^5.13.2"
 pytest = "^8.1.1"
 pyright = "^1.1.357"
 pre-commit = "^3.7.0"
+mkdocs = "^1.5.3"
+mkdocstrings = {extras = ["python"], version = "^0.24.3"}
+mkdocs-material = "^9.5.17"
 
 [tool.poetry.dependencies]
 python = "3.10.*"
+typer = "^0.12.3"
+
+
+[tool.poetry.scripts]
+tsk = "tsk_monster:main"
```

### Comparing `tsk_monster-0.0.7/PKG-INFO` & `tsk_monster-0.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: tsk-monster
-Version: 0.0.7
+Version: 0.0.8
 Summary: 
 Author: Gilad Kutiel
 Author-email: giladk@mobileye.com
 Requires-Python: ==3.10.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: typer (>=0.12.3,<0.13.0)
 Project-URL: Documentation, https://tsk.monster
 Project-URL: Homepage, https://tsk.monster
 Project-URL: Repository, https://github.com/tsk-monster/tsk
 Description-Content-Type: text/markdown
 
 # tsk.monster
 ## A cute little task runner.
```

