# Comparing `tmp/htagui-0.3.0.tar.gz` & `tmp/htagui-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htagui-0.3.0.tar", max compression
+gzip compressed data, was "htagui-0.3.1.tar", max compression
```

## Comparing `htagui-0.3.0.tar` & `htagui-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1065 2024-04-13 15:43:21.596339 htagui-0.3.0/LICENSE
--rw-r--r--   0        0        0     6761 2024-04-13 15:43:21.596339 htagui-0.3.0/README.md
--rw-r--r--   0        0        0      330 2024-04-13 15:43:21.840338 htagui-0.3.0/htagui/__init__.py
--rw-r--r--   0        0        0     1080 2024-04-13 15:43:21.596339 htagui-0.3.0/htagui/basics/__init__.py
--rw-r--r--   0        0        0     6073 2024-04-13 15:43:21.596339 htagui-0.3.0/htagui/basics/bases/__init__.py
--rw-r--r--   0        0        0     1081 2024-04-13 15:43:21.596339 htagui-0.3.0/htagui/bulma/__init__.py
--rw-r--r--   0        0        0   652848 2024-04-13 15:43:21.600339 htagui-0.3.0/htagui/bulma/bases/__init__.py
--rw-r--r--   0        0        0     3215 2024-04-13 15:43:21.600339 htagui-0.3.0/htagui/common.py
--rw-r--r--   0        0        0     3828 2024-04-13 15:43:21.600339 htagui-0.3.0/htagui/dialog.py
--rw-r--r--   0        0        0     1856 2024-04-13 15:43:21.600339 htagui-0.3.0/htagui/flex.py
--rw-r--r--   0        0        0      758 2024-04-13 15:43:21.600339 htagui-0.3.0/htagui/form.py
--rw-r--r--   0        0        0     1616 2024-04-13 15:43:21.600339 htagui-0.3.0/htagui/shoelace/__init__.py
--rw-r--r--   0        0        0     5968 2024-04-13 15:43:21.600339 htagui-0.3.0/htagui/shoelace/bases/__init__.py
--rw-r--r--   0        0        0     8884 2024-04-13 15:43:21.600339 htagui-0.3.0/htagui/splitters.py
--rw-r--r--   0        0        0     2023 2024-04-13 15:43:21.600339 htagui-0.3.0/htagui/tabs.py
--rw-r--r--   0        0        0     1069 2024-04-13 15:43:21.840338 htagui-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     7994 1970-01-01 00:00:00.000000 htagui-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-14 09:09:03.980268 htagui-0.3.1/LICENSE
+-rw-r--r--   0        0        0     6828 2024-04-14 09:09:03.980268 htagui-0.3.1/README.md
+-rw-r--r--   0        0        0      330 2024-04-14 09:09:04.228270 htagui-0.3.1/htagui/__init__.py
+-rw-r--r--   0        0        0     1080 2024-04-14 09:09:03.980268 htagui-0.3.1/htagui/basics/__init__.py
+-rw-r--r--   0        0        0     6073 2024-04-14 09:09:03.984269 htagui-0.3.1/htagui/basics/bases/__init__.py
+-rw-r--r--   0        0        0     1081 2024-04-14 09:09:03.984269 htagui-0.3.1/htagui/bulma/__init__.py
+-rw-r--r--   0        0        0   652848 2024-04-14 09:09:03.984269 htagui-0.3.1/htagui/bulma/bases/__init__.py
+-rw-r--r--   0        0        0     3215 2024-04-14 09:09:03.984269 htagui-0.3.1/htagui/common.py
+-rw-r--r--   0        0        0     4047 2024-04-14 09:09:03.984269 htagui-0.3.1/htagui/dialog.py
+-rw-r--r--   0        0        0     1856 2024-04-14 09:09:03.984269 htagui-0.3.1/htagui/flex.py
+-rw-r--r--   0        0        0      758 2024-04-14 09:09:03.984269 htagui-0.3.1/htagui/form.py
+-rw-r--r--   0        0        0     1616 2024-04-14 09:09:03.984269 htagui-0.3.1/htagui/shoelace/__init__.py
+-rw-r--r--   0        0        0     5968 2024-04-14 09:09:03.984269 htagui-0.3.1/htagui/shoelace/bases/__init__.py
+-rw-r--r--   0        0        0     8884 2024-04-14 09:09:03.984269 htagui-0.3.1/htagui/splitters.py
+-rw-r--r--   0        0        0     2023 2024-04-14 09:09:03.984269 htagui-0.3.1/htagui/tabs.py
+-rw-r--r--   0        0        0     1069 2024-04-14 09:09:04.228270 htagui-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8061 1970-01-01 00:00:00.000000 htagui-0.3.1/PKG-INFO
```

### Comparing `htagui-0.3.0/LICENSE` & `htagui-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `htagui-0.3.0/README.md` & `htagui-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -208,14 +208,18 @@
 
 Display a modal dialog box containing the object 'obj'. But the dialog is not closable, so be sure to provide a way to close it.
 
 ### method dialog.close()
 
 Close programatically, the current ui dialog.
 
+### method clipboard_copy(txt:str)
+
+Copy the txt in the clipboard
+
 ## Object HSplit (& VSplit)
 
 A Tag object to use "SplitJS" (currently only in horizontal form)
 
 ```python
 import htagui as ui
 self <= ui.HSplit( Tag.div(1), Tag.div(2), sizes=[60,40], minSize=100, _style="border:2px solid red;height:100px" )
```

### Comparing `htagui-0.3.0/htagui/basics/__init__.py` & `htagui-0.3.1/htagui/basics/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.3.0/htagui/basics/bases/__init__.py` & `htagui-0.3.1/htagui/basics/bases/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.3.0/htagui/bulma/__init__.py` & `htagui-0.3.1/htagui/bulma/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.3.0/htagui/bulma/bases/__init__.py` & `htagui-0.3.1/htagui/bulma/bases/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.3.0/htagui/common.py` & `htagui-0.3.1/htagui/common.py`

 * *Files identical despite different names*

### Comparing `htagui-0.3.0/htagui/dialog.py` & `htagui-0.3.1/htagui/dialog.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,24 @@
         self["info"]="UI.current object"
         self._toasts = Tag.div(_info="UI.toasts objects")
         self._previous=None
         parent += self  # auto add
         parent += self._toasts  # add a personnal place for toasts
         TagStep.init(self)
 
+    def clipboard_copy(self,txt:str):
+        self.call(f"""
+let ta = document.createElement('textarea');
+ta.value = `{txt}`;
+self.appendChild(ta);
+ta.select();
+document.execCommand('copy');
+self.removeChild(ta);
+""")
+
     def alert(self,obj):
         self.step( alert = obj )
 
     def box(self,obj,size:float=0.5):
         self.step( box = obj, size=50 - size*50 )
         
     def confirm(self,obj,cbresponse=lambda bool:bool):
```

### Comparing `htagui-0.3.0/htagui/flex.py` & `htagui-0.3.1/htagui/flex.py`

 * *Files identical despite different names*

### Comparing `htagui-0.3.0/htagui/form.py` & `htagui-0.3.1/htagui/form.py`

 * *Files identical despite different names*

### Comparing `htagui-0.3.0/htagui/shoelace/__init__.py` & `htagui-0.3.1/htagui/shoelace/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.3.0/htagui/shoelace/bases/__init__.py` & `htagui-0.3.1/htagui/shoelace/bases/__init__.py`

 * *Files identical despite different names*

### Comparing `htagui-0.3.0/htagui/splitters.py` & `htagui-0.3.1/htagui/splitters.py`

 * *Files identical despite different names*

### Comparing `htagui-0.3.0/htagui/tabs.py` & `htagui-0.3.1/htagui/tabs.py`

 * *Files identical despite different names*

### Comparing `htagui-0.3.0/pyproject.toml` & `htagui-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "htagui"
-version = "0.3.0" # auto-updated
+version = "0.3.1" # auto-updated
 description = "GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase"
 authors = ["manatlan <manatlan@gmail.com>"]
 readme = 'README.md'
 license="MIT"
 keywords=['htag','gui', 'electron', "cef", "asyncio", "guy", "desktop", "web", "mobile", "http", "websocket", "html", "pyscript"]
 homepage = "https://github.com/manatlan/htagui"
 repository = "https://github.com/manatlan/htagui"
```

### Comparing `htagui-0.3.0/PKG-INFO` & `htagui-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: htagui
-Version: 0.3.0
+Version: 0.3.1
 Summary: GUI toolkit for creating beautiful applications for mobile, web, and desktop from a single python3 codebase
 Home-page: https://github.com/manatlan/htagui
 License: MIT
 Keywords: htag,gui,electron,cef,asyncio,guy,desktop,web,mobile,http,websocket,html,pyscript
 Author: manatlan
 Author-email: manatlan@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -235,14 +235,18 @@
 
 Display a modal dialog box containing the object 'obj'. But the dialog is not closable, so be sure to provide a way to close it.
 
 ### method dialog.close()
 
 Close programatically, the current ui dialog.
 
+### method clipboard_copy(txt:str)
+
+Copy the txt in the clipboard
+
 ## Object HSplit (& VSplit)
 
 A Tag object to use "SplitJS" (currently only in horizontal form)
 
 ```python
 import htagui as ui
 self <= ui.HSplit( Tag.div(1), Tag.div(2), sizes=[60,40], minSize=100, _style="border:2px solid red;height:100px" )
```

