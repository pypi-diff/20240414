# Comparing `tmp/most_sdk-0.1.0.tar.gz` & `tmp/most_sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "most_sdk-0.1.0.tar", max compression
+gzip compressed data, was "most_sdk-0.1.1.tar", max compression
```

## Comparing `most_sdk-0.1.0.tar` & `most_sdk-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       35 2024-01-09 15:26:54.578945 most_sdk-0.1.0/most_sdk/__init__.py
--rw-r--r--   0        0        0     2207 2024-02-20 16:04:07.220701 most_sdk-0.1.0/most_sdk/client.py
--rw-r--r--   0        0        0      748 2024-01-09 15:26:54.582945 most_sdk-0.1.0/most_sdk/exceptions.py
--rw-r--r--   0        0        0     1103 2024-02-20 16:02:04.138355 most_sdk-0.1.0/most_sdk/routes.py
--rw-r--r--   0        0        0     1219 2024-02-20 15:35:25.407324 most_sdk-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      527 1970-01-01 00:00:00.000000 most_sdk-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       35 2024-01-09 15:26:54.578945 most_sdk-0.1.1/most_sdk/__init__.py
+-rw-r--r--   0        0        0     2207 2024-04-14 19:14:05.599602 most_sdk-0.1.1/most_sdk/client.py
+-rw-r--r--   0        0        0      748 2024-01-09 15:26:54.582945 most_sdk-0.1.1/most_sdk/exceptions.py
+-rw-r--r--   0        0        0     1223 2024-04-14 19:14:22.032931 most_sdk-0.1.1/most_sdk/routes.py
+-rw-r--r--   0        0        0     1219 2024-04-14 19:14:22.032931 most_sdk-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      527 1970-01-01 00:00:00.000000 most_sdk-0.1.1/PKG-INFO
```

### Comparing `most_sdk-0.1.0/most_sdk/client.py` & `most_sdk-0.1.1/most_sdk/client.py`

 * *Files identical despite different names*

### Comparing `most_sdk-0.1.0/most_sdk/exceptions.py` & `most_sdk-0.1.1/most_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `most_sdk-0.1.0/most_sdk/routes.py` & `most_sdk-0.1.1/most_sdk/routes.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,27 +4,30 @@
         :param most_sdk.client.Client client: MOST SDK client
         :rtype: most_sdk.routes.Enrichment
         """
 
         self.client = client
         self.domain = 'big-data/enrichment'
 
-    def base(self, path: str, query: str, cpf: str, birthdate: str) -> dict:
+    def base(self, path: str, query: str, cpf: str, birthdate: str, webhook: dict = None) -> dict:
         data = {
             'query': query,
             'parameters': {'cpf': cpf, 'data_nascimento': birthdate},
         }
 
+        if webhook:
+            data['webhook'] = webhook
+
         return self.client.post(path=f'{self.domain}/{path}', original_data=data)
 
     def query(self, query: str, cpf: str, birthdate: str) -> dict:
         return self.base(path='', query=query, cpf=cpf, birthdate=birthdate)
 
-    def send(self, query: str, cpf: str, birthdate: str) -> dict:
-        return self.base(path='async', query=query, cpf=cpf, birthdate=birthdate)
+    def send(self, query: str, cpf: str, birthdate: str, webhook: dict = None) -> dict:
+        return self.base(path='async', query=query, cpf=cpf, birthdate=birthdate, webhook=webhook)
 
     def get(
         self,
         protocol: str = '',
     ) -> dict:
         path = 'async/status'
```

### Comparing `most_sdk-0.1.0/pyproject.toml` & `most_sdk-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "most_sdk"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Tecnologia BYX <tecnologia@grupobyx.com.br>"]
 packages = [{include = "most_sdk"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 six = "^1.16.0"
```

### Comparing `most_sdk-0.1.0/PKG-INFO` & `most_sdk-0.1.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: most_sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Tecnologia BYX
 Author-email: tecnologia@grupobyx.com.br
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

