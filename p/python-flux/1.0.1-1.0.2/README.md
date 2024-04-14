# Comparing `tmp/python_flux-1.0.1.tar.gz` & `tmp/python_flux-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_flux-1.0.1.tar", max compression
+gzip compressed data, was "python_flux-1.0.2.tar", max compression
```

## Comparing `python_flux-1.0.1.tar` & `python_flux-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      719 2024-04-14 03:28:17.857340 python_flux-1.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.0.1/python_flux/__init__.py
--rw-r--r--   0        0        0    15039 2024-04-14 03:28:17.497346 python_flux-1.0.1/python_flux/flux.py
--rw-r--r--   0        0        0      703 2024-04-14 03:28:17.497751 python_flux-1.0.1/python_flux/flux_utilis.py
--rw-r--r--   0        0        0     1532 2024-04-14 03:28:17.498041 python_flux-1.0.1/python_flux/producers.py
--rw-r--r--   0        0        0     1246 2024-04-14 03:28:17.498326 python_flux-1.0.1/python_flux/subscribers.py
--rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 python_flux-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      719 2024-04-14 04:36:38.278239 python_flux-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.0.2/python_flux/__init__.py
+-rw-r--r--   0        0        0    15039 2024-04-14 03:28:17.497346 python_flux-1.0.2/python_flux/flux.py
+-rw-r--r--   0        0        0      703 2024-04-14 03:28:17.497751 python_flux-1.0.2/python_flux/flux_utilis.py
+-rw-r--r--   0        0        0     1596 2024-04-14 04:36:37.930223 python_flux-1.0.2/python_flux/producers.py
+-rw-r--r--   0        0        0     1246 2024-04-14 03:28:17.498326 python_flux-1.0.2/python_flux/subscribers.py
+-rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 python_flux-1.0.2/PKG-INFO
```

### Comparing `python_flux-1.0.1/pyproject.toml` & `python_flux-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-flux"
-version = "1.0.1"
+version = "1.0.2"
 description = "Librería que utiliza generadores de python para simular procesamiento de flujo de datos"
 authors = ["Juan Pablo Bochard <jbochard@gmail.com>"]
 license = "GPL-3.0-or-later"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
```

### Comparing `python_flux-1.0.1/python_flux/flux.py` & `python_flux-1.0.2/python_flux/flux.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.0.1/python_flux/flux_utilis.py` & `python_flux-1.0.2/python_flux/flux_utilis.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.0.1/python_flux/producers.py` & `python_flux-1.0.2/python_flux/producers.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,19 +17,21 @@
     def prepare_next(self):
         self.value = None
 
     def get_value(self):
         return self.value
 
     def next(self, context):
-        if self.value is None:
-            v, e = self._next(context)
-            if e is None:
-                self.value = v
-        return self.value, e, context
+        if self.value is not None:
+            return self.value, None, context
+        v, e = self._next(context)
+        if e is None:
+            self.value = v
+            return self.value, None, context
+        return None, e, context
 
     def _next(self, context):
         return None, None
 
 
 class PFromIterator(Producer):
     def __init__(self, iterator):
@@ -40,15 +42,15 @@
             raise e
 
     def _next(self, context):
         try:
             v = next(self.iterator)
             return v, None
         except Exception as ex:
-            return self.value, ex
+            return None, ex
 
 
 class PFromGenerator(Producer):
     def __init__(self, function_gen):
         super(PFromGenerator, self).__init__()
         self.function_gen = function_gen
         self.generator = None
@@ -56,8 +58,8 @@
     def _next(self, context):
         if self.generator is None:
             self.generator = self.function_gen(context)
         try:
             v = next(self.generator)
             return v, None
         except Exception as ex:
-            return self.value, ex
+            return None, ex
```

### Comparing `python_flux-1.0.1/python_flux/subscribers.py` & `python_flux-1.0.2/python_flux/subscribers.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.0.1/PKG-INFO` & `python_flux-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-flux
-Version: 1.0.1
+Version: 1.0.2
 Summary: Librería que utiliza generadores de python para simular procesamiento de flujo de datos
 License: GPL-3.0-or-later
 Author: Juan Pablo Bochard
 Author-email: jbochard@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

