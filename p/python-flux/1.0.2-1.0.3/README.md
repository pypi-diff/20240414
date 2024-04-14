# Comparing `tmp/python_flux-1.0.2.tar.gz` & `tmp/python_flux-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_flux-1.0.2.tar", max compression
+gzip compressed data, was "python_flux-1.0.3.tar", max compression
```

## Comparing `python_flux-1.0.2.tar` & `python_flux-1.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      719 2024-04-14 04:36:38.278239 python_flux-1.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.0.2/python_flux/__init__.py
--rw-r--r--   0        0        0    15039 2024-04-14 03:28:17.497346 python_flux-1.0.2/python_flux/flux.py
--rw-r--r--   0        0        0      703 2024-04-14 03:28:17.497751 python_flux-1.0.2/python_flux/flux_utilis.py
--rw-r--r--   0        0        0     1596 2024-04-14 04:36:37.930223 python_flux-1.0.2/python_flux/producers.py
--rw-r--r--   0        0        0     1246 2024-04-14 03:28:17.498326 python_flux-1.0.2/python_flux/subscribers.py
--rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 python_flux-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      719 2024-04-14 14:08:00.699756 python_flux-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.0.3/python_flux/__init__.py
+-rw-r--r--   0        0        0    15271 2024-04-14 14:19:20.119928 python_flux-1.0.3/python_flux/flux.py
+-rw-r--r--   0        0        0      703 2024-04-14 03:28:17.497751 python_flux-1.0.3/python_flux/flux_utilis.py
+-rw-r--r--   0        0        0     1596 2024-04-14 04:36:37.930223 python_flux-1.0.3/python_flux/producers.py
+-rw-r--r--   0        0        0     1246 2024-04-14 03:28:17.498326 python_flux-1.0.3/python_flux/subscribers.py
+-rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 python_flux-1.0.3/PKG-INFO
```

### Comparing `python_flux-1.0.2/pyproject.toml` & `python_flux-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-flux"
-version = "1.0.2"
+version = "1.0.3"
 description = "Librería que utiliza generadores de python para simular procesamiento de flujo de datos"
 authors = ["Juan Pablo Bochard <jbochard@gmail.com>"]
 license = "GPL-3.0-or-later"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
```

### Comparing `python_flux-1.0.2/python_flux/flux.py` & `python_flux-1.0.3/python_flux/flux.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,17 +41,17 @@
 
         :param map_context_function: función(valor, contexto) desde donde se obtendrá el contexto a subsituir.
         """
         return FMapContext(map_context_function, self)
 
     def flat_map(self, flatmap_function):
         """
-        Permite modificar el valor de un flujo por lo elementos de otro flujo.
-        Recibe una función(valor, contexto) que se evaluará para cada elemento del flujo y retornará un flujo
-        cuyos elementos se usarán como nuevo flujo de datos.
+        Permite sustituir el valor de un flujo por elementos de otro flujo.
+        Recibe una función(valor, contexto) que se evaluará para cada elemento del flujo original y retornará un
+        flujo cuyos elementos se usarán como nuevo origen del flujo de datos.
 
         flatmap_function: función(valor, contexto) desde donde se obtendrá el valor a subsituir.
         """
         return FFlatMap(flatmap_function, self)
 
     def do_on_next(self, on_next):
         """
@@ -316,37 +316,44 @@
 
 class FFlatMap(Stream):
     def __init__(self, func, flux):
         super().__init__(flux)
         self.function = func
         self.current = None
 
+    def prepare_next(self):
+        if self.current is None:
+            super(FFlatMap, self).prepare_next()
+        else:
+            self.current.prepare_next()
+
     def next(self, context):
         ctx = context.copy()
         while True:
             while self.current is None:
                 value, e, ctx = super(FFlatMap, self).next(ctx)
                 if e is not None:
                     return None, e, ctx
                 func, e = fu.try_or(partial(self.function), value, ctx)
                 if e is not None:
                     return None, e, ctx
+                fgen = func
                 if isinstance(func, types.GeneratorType):
                     from python_flux.producers import PFromGenerator
                     fgen = PFromGenerator(func)
-                else:
-                    fgen = func
-                self.current = fgen.subscribe(ctx)
-            try:
-                v = next(self.current)
-                return v, None, ctx
-            except StopIteration:
+                self.current = fgen
+                self.current.prepare_next()
+
+            cur_value, cur_e, cur_ctx = self.current.next(ctx)
+            if cur_e is None:
+                return cur_value, cur_e, cur_ctx
+
+            if isinstance(cur_e, StopIteration):
                 self.current = None
-            except Exception as ex:
-                return None, ex, ctx
+                super(FFlatMap, self).prepare_next()
 
 
 class FOnErrorResume(Stream):
     def __init__(self, f, exceptions, flux):
         super().__init__(flux)
         self.on_error_resume = f
         self.exceptions = exceptions
```

### Comparing `python_flux-1.0.2/python_flux/flux_utilis.py` & `python_flux-1.0.3/python_flux/flux_utilis.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.0.2/python_flux/producers.py` & `python_flux-1.0.3/python_flux/producers.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.0.2/python_flux/subscribers.py` & `python_flux-1.0.3/python_flux/subscribers.py`

 * *Files identical despite different names*

### Comparing `python_flux-1.0.2/PKG-INFO` & `python_flux-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-flux
-Version: 1.0.2
+Version: 1.0.3
 Summary: Librería que utiliza generadores de python para simular procesamiento de flujo de datos
 License: GPL-3.0-or-later
 Author: Juan Pablo Bochard
 Author-email: jbochard@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

