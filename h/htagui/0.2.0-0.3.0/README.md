# Comparing `tmp/htagui-0.2.0.tar.gz` & `tmp/htagui-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagui-0.2.0.tar", max compression
+gzip compressed data, was "htagui-0.3.0.tar", max compression
```

## Comparing `htagui-0.2.0.tar` & `htagui-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,17 @@
--rw-r--r--   0        0        0     1065 2024-04-12 11:14:52.129510 htagui-0.2.0/LICENSE
--rw-r--r--   0        0        0     6761 2024-04-12 11:14:52.129510 htagui-0.2.0/README.md
--rw-r--r--   0        0        0     1113 2024-04-12 11:14:52.657509 htagui-0.2.0/htagui/__init__.py
--rw-r--r--   0        0        0     3549 2024-04-12 11:14:52.129510 htagui-0.2.0/htagui/basics/__init__.py
--rw-r--r--   0        0        0     3215 2024-04-12 11:14:52.129510 htagui-0.2.0/htagui/common.py
--rw-r--r--   0        0        0     5598 2024-04-12 11:14:52.129510 htagui-0.2.0/htagui/dialog.py
--rw-r--r--   0        0        0     1856 2024-04-12 11:14:52.129510 htagui-0.2.0/htagui/flex.py
--rw-r--r--   0        0        0      758 2024-04-12 11:14:52.129510 htagui-0.2.0/htagui/form.py
--rw-r--r--   0        0        0     8884 2024-04-12 11:14:52.129510 htagui-0.2.0/htagui/splitters.py
--rw-r--r--   0        0        0     2023 2024-04-12 11:14:52.129510 htagui-0.2.0/htagui/tabs.py
--rw-r--r--   0        0        0     1069 2024-04-12 11:14:52.657509 htagui-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     7994 1970-01-01 00:00:00.000000 htagui-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-13 15:43:21.596339 htagui-0.3.0/LICENSE
+-rw-r--r--   0        0        0     6761 2024-04-13 15:43:21.596339 htagui-0.3.0/README.md
+-rw-r--r--   0        0        0      330 2024-04-13 15:43:21.840338 htagui-0.3.0/htagui/__init__.py
+-rw-r--r--   0        0        0     1080 2024-04-13 15:43:21.596339 htagui-0.3.0/htagui/basics/__init__.py
+-rw-r--r--   0        0        0     6073 2024-04-13 15:43:21.596339 htagui-0.3.0/htagui/basics/bases/__init__.py
+-rw-r--r--   0        0        0     1081 2024-04-13 15:43:21.596339 htagui-0.3.0/htagui/bulma/__init__.py
+-rw-r--r--   0        0        0   652848 2024-04-13 15:43:21.600339 htagui-0.3.0/htagui/bulma/bases/__init__.py
+-rw-r--r--   0        0        0     3215 2024-04-13 15:43:21.600339 htagui-0.3.0/htagui/common.py
+-rw-r--r--   0        0        0     3828 2024-04-13 15:43:21.600339 htagui-0.3.0/htagui/dialog.py
+-rw-r--r--   0        0        0     1856 2024-04-13 15:43:21.600339 htagui-0.3.0/htagui/flex.py
+-rw-r--r--   0        0        0      758 2024-04-13 15:43:21.600339 htagui-0.3.0/htagui/form.py
+-rw-r--r--   0        0        0     1616 2024-04-13 15:43:21.600339 htagui-0.3.0/htagui/shoelace/__init__.py
+-rw-r--r--   0        0        0     5968 2024-04-13 15:43:21.600339 htagui-0.3.0/htagui/shoelace/bases/__init__.py
+-rw-r--r--   0        0        0     8884 2024-04-13 15:43:21.600339 htagui-0.3.0/htagui/splitters.py
+-rw-r--r--   0        0        0     2023 2024-04-13 15:43:21.600339 htagui-0.3.0/htagui/tabs.py
+-rw-r--r--   0        0        0     1069 2024-04-13 15:43:21.840338 htagui-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7994 1970-01-01 00:00:00.000000 htagui-0.3.0/PKG-INFO
```

### Comparing `htagui-0.2.0/LICENSE` & `htagui-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `htagui-0.2.0/README.md` & `htagui-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `htagui-0.2.0/htagui/__init__.py` & `htagui-0.3.0/htagui/bulma/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 # Copyright (C) 2024 manatlan manatlan[at]gmail(dot)com
 #
 # MIT licence
 #
 # https://github.com/manatlan/htag
 # #############################################################################
 
-__version__ = "0.2.0" # auto updated
 
 from htag import Tag
+
 ########################################################################################
-from .basics import Button,Input,Menu,Spinner,Select
+from .bases import Button,Input,Menu,Spinner,Select
 ########################################################################################
-from .form import Form
-from .tabs import Tabs
-from .dialog import Dialog
-from .splitters import HSplit #VSplit
-from .flex import hflex,vflex  # utilities (Htag contructor methods)
+from ..form import Form
+from ..tabs import Tabs
+from ..dialog import Dialog
+from ..splitters import HSplit #VSplit
+from ..flex import hflex,vflex  # utilities (Htag contructor methods)
 
 class App(Tag.body):
     _ui=None
     
     @property
     def ui(self):
         if self._ui is None:
```

### Comparing `htagui-0.2.0/htagui/common.py` & `htagui-0.3.0/htagui/common.py`

 * *Files identical despite different names*

### Comparing `htagui-0.2.0/htagui/flex.py` & `htagui-0.3.0/htagui/flex.py`

 * *Files identical despite different names*

### Comparing `htagui-0.2.0/htagui/form.py` & `htagui-0.3.0/htagui/form.py`

 * *Files identical despite different names*

### Comparing `htagui-0.2.0/htagui/splitters.py` & `htagui-0.3.0/htagui/splitters.py`

 * *Files identical despite different names*

### Comparing `htagui-0.2.0/htagui/tabs.py` & `htagui-0.3.0/htagui/tabs.py`

 * *Files identical despite different names*

### Comparing `htagui-0.2.0/pyproject.toml` & `htagui-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagui"
-version = "0.2.0" # auto-updated
+version = "0.3.0" # auto-updated
 description = "GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','gui', 'electron', "cef", "asyncio", "guy", "desktop", "web", "mobile", "http", "websocket", "html", "pyscript"]
 homepage = "https://github.com/manatlan/htagui"
 repository = "https://github.com/manatlan/htagui"
@@ -15,15 +15,15 @@
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: Apache Software License",
 ]
 
 [tool.poetry.dependencies]
 # https://python-poetry.org/docs/dependency-specification/
 python = "^3.7"
-htag = ">= 0.102"
+htag = ">= 0.103"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6"
 pytest-cov = "^2.6"
 
 [build-system]
 requires = ["poetry>=0.12"]
```

### Comparing `htagui-0.2.0/PKG-INFO` & `htagui-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagui
-Version: 0.2.0
+Version: 0.3.0
 Summary: GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase
 Home-page: https://github.com/manatlan/htagui
 License: MIT
 Keywords: htag,gui,electron,cef,asyncio,guy,desktop,web,mobile,http,websocket,html,pyscript
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: htag (>=0.102)
+Requires-Dist: htag (>=0.103)
 Project-URL: Documentation, https://github.com/manatlan/htagui
 Project-URL: Repository, https://github.com/manatlan/htagui
 Description-Content-Type: text/markdown
 
 # htagUI
 
 This is a (basic) UI toolkit for [htag](https://github.com/manatlan/htag) apps. Contrario to [htbulma](https://github.com/manatlan/htbulma), this one is a minimal toolkit, providing only useful and solid widgets, and will be maintained (you can use it ;-)).
```

