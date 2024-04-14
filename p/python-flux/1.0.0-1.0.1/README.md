# Comparing `tmp/python_flux-1.0.0.tar.gz` & `tmp/python_flux-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_flux-1.0.0.tar", max compression
+gzip compressed data, was "python_flux-1.0.1.tar", max compression
```

## Comparing `python_flux-1.0.0.tar` & `python_flux-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      719 2024-04-13 23:26:20.252584 python_flux-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.0.0/python_flux/__init__.py
--rw-r--r--   0        0        0    14870 2024-04-14 00:16:09.911500 python_flux-1.0.0/python_flux/flux.py
--rw-r--r--   0        0        0      736 2024-04-13 23:50:57.491246 python_flux-1.0.0/python_flux/flux_utilis.py
--rw-r--r--   0        0        0     1522 2024-04-13 21:23:45.466753 python_flux-1.0.0/python_flux/producers.py
--rw-r--r--   0        0        0     1248 2024-04-13 22:38:54.621949 python_flux-1.0.0/python_flux/subscribers.py
--rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 python_flux-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      719 2024-04-14 03:28:17.857340 python_flux-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.0.1/python_flux/__init__.py
+-rw-r--r--   0        0        0    15039 2024-04-14 03:28:17.497346 python_flux-1.0.1/python_flux/flux.py
+-rw-r--r--   0        0        0      703 2024-04-14 03:28:17.497751 python_flux-1.0.1/python_flux/flux_utilis.py
+-rw-r--r--   0        0        0     1532 2024-04-14 03:28:17.498041 python_flux-1.0.1/python_flux/producers.py
+-rw-r--r--   0        0        0     1246 2024-04-14 03:28:17.498326 python_flux-1.0.1/python_flux/subscribers.py
+-rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 python_flux-1.0.1/PKG-INFO
```

### Comparing `python_flux-1.0.0/pyproject.toml` & `python_flux-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-flux"
-version = "1.0.0"
+version = "1.0.1"
 description = "Librería que utiliza generadores de python para simular procesamiento de flujo de datos"
 authors = ["Juan Pablo Bochard <jbochard@gmail.com>"]
 license = "GPL-3.0-or-later"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
```

### Comparing `python_flux-1.0.0/python_flux/flux.py` & `python_flux-1.0.1/python_flux/flux.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     def filter(self, predicate, on_mismatch=fu.default_action):
         """
         Permite filtrar un flujo perimtiendo continuar a aquellos valores que cumplen con el
         predicado que se indica.
         Si no se cumple el predicado opcionalmente se puede indicar una función que dado el valor y el contexto acutal
         retorna el valor que se enviará al flujo.
 
-        :param predicte: función(valor, contexto) que retorna un booleano
-        :param on_mismath: función(valor, contexto) que retorna un valor alternativo al testeado originalmente
+        :param predicate: función(valor, contexto) que retorna un booleano
+        :param on_mismatch: función(valor, contexto) que retorna un valor alternativo al testeado originalmente
         """
         return FFilter(predicate, on_mismatch, self)
 
     def map(self, map_function):
         """
         Permite modificar el valor de un flujo.
         Recibe una función(valor, contexto) que se evaluará para cada elemento del flujo y se substiuirá en el mismo
@@ -145,19 +145,29 @@
         return SSubscribe(context, self)
 
     def foreach(self, on_success=fu.default_success, on_error=fu.default_error, context={}):
         """
         Itera sobre los elementos del flujo e invoca a funciones on_success y on_error dependiendo
         el estado del flujo.
         :param on_success: función(valor, contexto) se invoca si el flujo procesa correctamente un valor
-        :param on_error:  función(ex, contexto) se invoca si hay un error en el flujo. Esto no corta el procesamiento
+        :param on_error:  función(ex, contexto) se invoca si hay un error en el flujo.
+                          Esto no corta el procesamiento a menos que se lance una excepción en el método
         :param context: Contexto inicial para el flujo
         """
-        for _ in SForeach(on_success, on_error, context, self):
-            pass
+        flux = self.subscribe(context)
+        while True:
+            try:
+                value = next(flux)
+                fu.try_or(partial(on_success), value, context)
+            except StopIteration:
+                return
+            except Exception as ex:
+                _, e = fu.try_or(partial(on_error), ex, context)
+                if e is not None:
+                    raise e
 
     def to_list(self, context={}):
         """
         Itera sobre los elementos del flujo y los retorna todos dentro de una lista.
         :param context: contexto inicial para el flujo
         :return: Lista de elementos
         """
@@ -170,17 +180,23 @@
         se invoca la función reduce(valor, acumulador) que procesa el valor y retorna un nuevo valor del acumulador.
         :param init: función(contexto) Retorna valor inicial del acumulador
         :param reduce: funcón(valor, acumulador) Dados el nuevo valor y el acumulador retorna un nuevo valor de acumulador.
         :param context: Contexto inicial para el flujo
         :return: Acumulador
         """
         acum = init(context)
-        for v in SSubscribe(context, self):
-            acum = reduce(v, acum)
-        return acum
+        flux = self.subscribe(context)
+        while True:
+            try:
+                value = next(flux)
+                acum = reduce(value, acum)
+            except StopIteration:
+                return
+            except Exception as ex:
+                raise ex
 
 
 class Stream(Flux):
     def __init__(self, up):
         super(Stream, self).__init__()
         self.upstream = up
 
@@ -201,14 +217,16 @@
     def next(self, context):
         value, e, ctx = super(FFilter, self).next(context)
         if e is not None:
             return value, e, ctx
         valid, e = fu.try_or(partial(self.predicate), value, context)
         while e is None and not valid:
             _, e = fu.try_or(partial(self.on_mismatch), value, context)
+            if e is not None:
+                return value, e, ctx
             super(FFilter, self).prepare_next()
             value, e, ctx = super(FFilter, self).next(context)
             if e is not None:
                 return value, e, ctx
             valid, e = fu.try_or(partial(self.predicate), value, context)
         return value, e, ctx
 
@@ -253,66 +271,50 @@
         super().__init__(flux)
         self.delay = delay
         self.predicate = predicate
 
     def next(self, context):
         value, e, ctx = super(FDelayMs, self).next(context)
         if e is not None:
-            return None, e, ctx
+            return value, e, ctx
         valid, e = fu.try_or(partial(self.predicate), value, context)
         if e is not None:
             return value, e, ctx
         if valid:
             time.sleep(self.delay / 1000)
         return value, e, ctx
 
 
-class FDelayConditional(Stream):
-    def __init__(self, delay, predicate, flux):
-        super().__init__(flux)
-        self.delay = delay
-        self.predicate = predicate
-
-    def next(self, context):
-        value, e, ctx = super(FDelayConditional, self).next(context)
-        valid, e = fu.try_or(partial(self.predicate), e, value, context)
-        if e is not None:
-            return value, e, ctx
-
-        time.sleep(self.delay)
-        return value, e, ctx
-
-
 class FMap(Stream):
     def __init__(self, func, flux):
         super().__init__(flux)
         self.function = func
 
     def next(self, context):
         value, e, ctx = super(FMap, self).next(context)
         if e is not None:
-            return None, e, ctx
+            return value, e, ctx
         mapped_value, e = fu.try_or(partial(self.function), value, ctx.copy())
         if e is not None:
-            return None, e, ctx
+            return value, e, ctx
         return mapped_value, e, ctx
 
 
 class FMapContext(Stream):
     def __init__(self, func, flux):
         super().__init__(flux)
         self.function = func
 
     def next(self, context):
         value, e, ctx = super(FMapContext, self).next(context)
         if e is not None:
-            return None, e, ctx
+            return value, e, ctx
         mapped_context, e = fu.try_or(partial(self.function), value, ctx.copy())
         if e is not None:
-            return None, e, ctx
+            return value, e, ctx
         return value, e, merge(ctx, mapped_context)
 
 
 class FFlatMap(Stream):
     def __init__(self, func, flux):
         super().__init__(flux)
         self.function = func
@@ -354,15 +356,15 @@
         if e is None:
             return value, e, ctx
         if isinstance(e, StopIteration):
             return None, e, ctx
         if any([isinstance(e, ex) for ex in self.exceptions]):
             v, e = fu.try_or(partial(self.on_error_resume), e, ctx)
             if e is not None:
-                return None, e, ctx
+                return value, e, ctx
             value = v
         return value, None, ctx
 
 
 class FOnErrorRetry(Stream):
     def __init__(self, retries, exceptions, delay_ms, flux):
         super().__init__(flux)
```

### Comparing `python_flux-1.0.0/python_flux/flux_utilis.py` & `python_flux-1.0.1/python_flux/flux_utilis.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 
     @staticmethod
     def default_success(value, context):
         pass
 
     @staticmethod
     def default_error(e, context):
-        if not isinstance(e, StopIteration):
-            traceback.print_exception(type(e), e, e.__traceback__)
+        traceback.print_exception(type(e), e, e.__traceback__)
+        raise e
 
     @staticmethod
     def try_or(statement, value, ctx) -> (object, Exception):
         try:
             v = statement(value, ctx)
             return v, None
         except Exception as ex:
```

### Comparing `python_flux-1.0.0/python_flux/producers.py` & `python_flux-1.0.1/python_flux/producers.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,52 +8,56 @@
 def from_iterator(iterator):
     return PFromIterator(iterator)
 
 
 class Producer(Flux):
     def __init__(self):
         super(Producer, self).__init__()
+        self.value = None
+
+    def prepare_next(self):
+        self.value = None
+
+    def get_value(self):
+        return self.value
 
     def next(self, context):
-        return None, None, context
+        if self.value is None:
+            v, e = self._next(context)
+            if e is None:
+                self.value = v
+        return self.value, e, context
+
+    def _next(self, context):
+        return None, None
 
 
 class PFromIterator(Producer):
     def __init__(self, iterator):
         super(PFromIterator, self).__init__()
-        self.value = None
         try:
             self.iterator = iterator if type(iterator) is iter else iter(iterator)
         except TypeError as e:
             raise e
 
-    def prepare_next(self):
-        self.value = None
-
-    def next(self, context):
+    def _next(self, context):
         try:
-            if self.value is None:
-                self.value = next(self.iterator)
-            return self.value, None, context
+            v = next(self.iterator)
+            return v, None
         except Exception as ex:
-            return self.value, ex, context
+            return self.value, ex
 
 
 class PFromGenerator(Producer):
     def __init__(self, function_gen):
         super(PFromGenerator, self).__init__()
         self.function_gen = function_gen
         self.generator = None
-        self.value = None
 
-    def prepare_next(self):
-        self.value = None
-
-    def next(self, context):
+    def _next(self, context):
         if self.generator is None:
             self.generator = self.function_gen(context)
         try:
-            if self.value is None:
-                self.value = next(self.generator)
-            return self.value, None, context
+            v = next(self.generator)
+            return v, None
         except Exception as ex:
-            return self.value, ex, context
+            return self.value, ex
```

### Comparing `python_flux-1.0.0/python_flux/subscribers.py` & `python_flux-1.0.1/python_flux/subscribers.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,19 +20,20 @@
         value, e, ctx = self.flux.next(self.context)
         if e is not None:
             raise e
         self.context = merge(self.context, ctx)
         return value
 
 
-class SForeach(SSubscribe):
+class SForeach(object):
     def __init__(self, on_success, on_error, ctx, f):
-        super(SForeach, self).__init__(ctx, f)
         self.on_success = on_success
         self.on_error = on_error
+        self.context = ctx
+        self.flux = f
 
     def __next__(self):
         while True:
             self.flux.prepare_next()
             value, e, ctx = self.flux.next(self.context)
             if e is not None and isinstance(e, StopIteration):
                 raise e
```

### Comparing `python_flux-1.0.0/PKG-INFO` & `python_flux-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-flux
-Version: 1.0.0
+Version: 1.0.1
 Summary: Librería que utiliza generadores de python para simular procesamiento de flujo de datos
 License: GPL-3.0-or-later
 Author: Juan Pablo Bochard
 Author-email: jbochard@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

