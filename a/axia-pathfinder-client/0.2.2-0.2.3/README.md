# Comparing `tmp/axia_pathfinder_client-0.2.2.tar.gz` & `tmp/axia_pathfinder_client-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axia_pathfinder_client-0.2.2.tar", max compression
+gzip compressed data, was "axia_pathfinder_client-0.2.3.tar", max compression
```

## Comparing `axia_pathfinder_client-0.2.2.tar` & `axia_pathfinder_client-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    34523 2023-11-26 14:35:57.991379 axia_pathfinder_client-0.2.2/LICENSE
--rw-r--r--   0        0        0     1803 2023-11-26 14:35:57.991379 axia_pathfinder_client-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-11-26 14:35:57.991379 axia_pathfinder_client-0.2.2/pathfinder/__init__.py
--rw-r--r--   0        0        0        0 2023-11-26 14:35:57.991379 axia_pathfinder_client-0.2.2/pathfinder/operators/__init__.py
--rw-r--r--   0        0        0      333 2023-11-26 14:35:57.991379 axia_pathfinder_client-0.2.2/pathfinder/operators/base.py
--rw-r--r--   0        0        0      679 2023-11-26 14:35:57.991379 axia_pathfinder_client-0.2.2/pathfinder/operators/get.py
--rw-r--r--   0        0        0      683 2023-11-26 14:35:57.991379 axia_pathfinder_client-0.2.2/pathfinder/operators/gpo.py
--rw-r--r--   0        0        0      860 2023-11-26 14:35:57.991379 axia_pathfinder_client-0.2.2/pathfinder/operators/login.py
--rw-r--r--   0        0        0      387 2023-11-26 14:35:57.991379 axia_pathfinder_client-0.2.2/pathfinder/operators/sub.py
--rw-r--r--   0        0        0     1366 2023-11-26 14:35:57.991379 axia_pathfinder_client-0.2.2/pathfinder/parser.py
--rw-r--r--   0        0        0     1179 2023-11-26 14:35:57.991379 axia_pathfinder_client-0.2.2/pathfinder/telnet.py
--rw-r--r--   0        0        0     1058 2023-11-26 14:36:17.583419 axia_pathfinder_client-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2290 1970-01-01 00:00:00.000000 axia_pathfinder_client-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-14 19:36:38.684850 axia_pathfinder_client-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1803 2024-04-14 19:36:38.684850 axia_pathfinder_client-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-14 19:36:38.684850 axia_pathfinder_client-0.2.3/pathfinder/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 19:36:38.684850 axia_pathfinder_client-0.2.3/pathfinder/operators/__init__.py
+-rw-r--r--   0        0        0      333 2024-04-14 19:36:38.684850 axia_pathfinder_client-0.2.3/pathfinder/operators/base.py
+-rw-r--r--   0        0        0      679 2024-04-14 19:36:38.684850 axia_pathfinder_client-0.2.3/pathfinder/operators/get.py
+-rw-r--r--   0        0        0      683 2024-04-14 19:36:38.684850 axia_pathfinder_client-0.2.3/pathfinder/operators/gpo.py
+-rw-r--r--   0        0        0      860 2024-04-14 19:36:38.684850 axia_pathfinder_client-0.2.3/pathfinder/operators/login.py
+-rw-r--r--   0        0        0      388 2024-04-14 19:36:38.684850 axia_pathfinder_client-0.2.3/pathfinder/operators/sub.py
+-rw-r--r--   0        0        0     1366 2024-04-14 19:36:38.684850 axia_pathfinder_client-0.2.3/pathfinder/parser.py
+-rw-r--r--   0        0        0     1178 2024-04-14 19:36:38.684850 axia_pathfinder_client-0.2.3/pathfinder/telnet.py
+-rw-r--r--   0        0        0     1075 2024-04-14 19:36:54.908888 axia_pathfinder_client-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2290 1970-01-01 00:00:00.000000 axia_pathfinder_client-0.2.3/PKG-INFO
```

### Comparing `axia_pathfinder_client-0.2.2/LICENSE` & `axia_pathfinder_client-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `axia_pathfinder_client-0.2.2/README.md` & `axia_pathfinder_client-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `axia_pathfinder_client-0.2.2/pathfinder/operators/get.py` & `axia_pathfinder_client-0.2.3/pathfinder/operators/get.py`

 * *Files identical despite different names*

### Comparing `axia_pathfinder_client-0.2.2/pathfinder/operators/gpo.py` & `axia_pathfinder_client-0.2.3/pathfinder/operators/gpo.py`

 * *Files identical despite different names*

### Comparing `axia_pathfinder_client-0.2.2/pathfinder/operators/login.py` & `axia_pathfinder_client-0.2.3/pathfinder/operators/login.py`

 * *Files identical despite different names*

### Comparing `axia_pathfinder_client-0.2.2/pathfinder/parser.py` & `axia_pathfinder_client-0.2.3/pathfinder/parser.py`

 * *Files identical despite different names*

### Comparing `axia_pathfinder_client-0.2.2/pathfinder/telnet.py` & `axia_pathfinder_client-0.2.3/pathfinder/telnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 >>> from pathfinder.telnet import TelnetClient
 >>> tc = TelnetClient()
 >>> tc.connect()
 >>> tc.disconnect()
 """
 
-
 import logging
 import telnetlib
 
 logger = logging.getLogger(__name__)
 
 
 class TelnetClientException(Exception):
```

### Comparing `axia_pathfinder_client-0.2.2/pyproject.toml` & `axia_pathfinder_client-0.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "axia-pathfinder-client"
-version = "v0.2.2"
+version = "v0.2.3"
 description = "Proof of concept Axia Pathfinder API/SDK."
 authors = ["RaBe IT-Reaktion <it@rabe.ch>"]
 license = "AGPLv3"
 readme = "README.md"
 packages = [{include = "pathfinder"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 parsy = "^2.1"
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.3.0"
-pytest = "^7.3.2"
-pytest-cov = "^4.0.0"
+black = ">=23.3,<25.0"
+pytest = ">=7.3.2,<9.0.0"
+pytest-cov = ">=4,<6"
 pytest-random-order = "^1.1.0"
-pytest-ruff = ">=0.1,<0.3"
-ruff = ">=0.0.272,<0.1.7"
+pytest-ruff = ">=0.1,<0.4"
+ruff = ">=0.0.272,<0.3.8"
 isort = "^5.12.0"
-pytest-isort = "^3.1.0"
+pytest-isort = ">=3.1,<5.0"
 mkdocs = "^1.4.3"
 mkdocs-gen-files = "^0.5.0"
 mkdocs-literate-nav = "^0.6.0"
 mkdocs-section-index = "^0.3.5"
 mkdocs-material = "^9.1.16"
 mkdocstrings = {extras = ["python"], version = ">=0.22,<0.25"}
```

### Comparing `axia_pathfinder_client-0.2.2/PKG-INFO` & `axia_pathfinder_client-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axia-pathfinder-client
-Version: 0.2.2
+Version: 0.2.3
 Summary: Proof of concept Axia Pathfinder API/SDK.
 License: AGPLv3
 Author: RaBe IT-Reaktion
 Author-email: it@rabe.ch
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

