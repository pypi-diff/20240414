# Comparing `tmp/icodes-0.1.0.tar.gz` & `tmp/icodes-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icodes-0.1.0.tar", max compression
+gzip compressed data, was "icodes-0.1.1.tar", max compression
```

## Comparing `icodes-0.1.0.tar` & `icodes-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,11 @@
--rw-r--r--   0        0        0     7048 2024-03-31 18:37:25.121754 icodes-0.1.0/LICENSE
--rw-r--r--   0        0        0     2885 2024-04-14 10:09:51.204558 icodes-0.1.0/README.md
--rw-r--r--   0        0        0     4495 2024-04-14 09:52:31.214089 icodes-0.1.0/icodes.py
--rw-r--r--   0        0        0     1136 2024-04-14 10:12:52.961322 icodes-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4019 1970-01-01 00:00:00.000000 icodes-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7048 2024-03-31 18:37:25.121754 icodes-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2883 2024-04-14 10:21:32.481639 icodes-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-06 19:55:00.301396 icodes-0.1.1/icds/__init__.py
+-rw-r--r--   0        0        0     1935 2024-04-14 09:52:58.273822 icodes-0.1.1/icds/data.py
+-rw-r--r--   0        0        0     1285 2024-04-14 09:43:58.775498 icodes-0.1.1/icds/git_helpers.py
+-rw-r--r--   0        0        0     3124 2024-04-06 19:55:00.301396 icodes-0.1.1/icds/llm_interface.py
+-rw-r--r--   0        0        0      797 2024-04-14 09:43:58.775498 icodes-0.1.1/icds/models.py
+-rw-r--r--   0        0        0      241 2024-04-06 19:55:00.301396 icodes-0.1.1/icds/settings.py
+-rw-r--r--   0        0        0     4495 2024-04-14 09:52:31.214089 icodes-0.1.1/icodes.py
+-rw-r--r--   0        0        0     1145 2024-04-14 11:23:28.352088 icodes-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3941 1970-01-01 00:00:00.000000 icodes-0.1.1/PKG-INFO
```

### Comparing `icodes-0.1.0/LICENSE` & `icodes-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `icodes-0.1.0/README.md` & `icodes-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 * Insight extraction to identify trends and patterns in code evolution
 * CLI and web-based UI (comming soon)
 
 ## Installation
 
 iCODES requires Python 3.11 or higher. 
 
-    `pip install icodes`
+    pip install icodes
 
 ### Alternative installation 
 
 Or clone the repo:
 
     git clone https://github.com/a115/iCODES.git
```

### Comparing `icodes-0.1.0/icodes.py` & `icodes-0.1.1/icodes.py`

 * *Files identical despite different names*

### Comparing `icodes-0.1.0/pyproject.toml` & `icodes-0.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 [tool.poetry]
 name = "icodes"
-version = "0.1.0"
+version = "0.1.1"
 description = "LLM-powered Git archeology tool (a.k.a. Intelligent Commit Ontology Distiller and Enhanced Search)"
 authors = ["Jordan Dimov <jdimov@a115.co.uk>", "Bayo Ade <bayo.300@gmail.com>"]
 license = "CC0-1.0"
 readme = "README.md"
+packages = [
+    { include = "icodes.py" },
+    { include = "icds/**/*.py" },
+]
 repository = "https://github.com/a115/iCODES"
 homepage = "https://github.com/a115/iCODES"
 documentation = "https://github.com/a115/iCODES"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.11",
-    "License :: OSI Approved :: Creative Commons Zero v1.0 Universal",
     "Operating System :: OS Independent",
 ]
 keywords = ["git", "llm", "archeology", "commit", "search"]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 typer = "^0.12.0"
```

### Comparing `icodes-0.1.0/PKG-INFO` & `icodes-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: icodes
-Version: 0.1.0
+Version: 0.1.1
 Summary: LLM-powered Git archeology tool (a.k.a. Intelligent Commit Ontology Distiller and Enhanced Search)
 Home-page: https://github.com/a115/iCODES
 License: CC0-1.0
 Keywords: git,llm,archeology,commit,search
 Author: Jordan Dimov
 Author-email: jdimov@a115.co.uk
 Requires-Python: >=3.11,<4.0
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Classifier: License :: OSI Approved :: Creative Commons Zero v1.0 Universal
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: gitpython (>=3.1.43,<4.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: openai (>=1.14.3,<2.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
@@ -39,15 +38,15 @@
 * Insight extraction to identify trends and patterns in code evolution
 * CLI and web-based UI (comming soon)
 
 ## Installation
 
 iCODES requires Python 3.11 or higher. 
 
-    `pip install icodes`
+    pip install icodes
 
 ### Alternative installation 
 
 Or clone the repo:
 
     git clone https://github.com/a115/iCODES.git
```

