# Comparing `tmp/indexify-0.0.8.tar.gz` & `tmp/indexify-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indexify-0.0.8.tar", max compression
+gzip compressed data, was "indexify-0.0.9.tar", max compression
```

## Comparing `indexify-0.0.8.tar` & `indexify-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2024-02-16 20:50:49.845214 indexify-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0     1056 2024-02-16 20:50:49.845214 indexify-0.0.8/README.md
--rw-r--r--   0        0        0      290 2024-02-16 20:50:49.849214 indexify-0.0.8/indexify/__init__.py
--rw-r--r--   0        0        0    12910 2024-02-16 20:50:49.849214 indexify-0.0.8/indexify/client.py
--rw-r--r--   0        0        0      690 2024-02-16 20:50:49.849214 indexify-0.0.8/indexify/data_containers.py
--rw-r--r--   0        0        0      111 2024-02-16 20:50:49.849214 indexify-0.0.8/indexify/exceptions.py
--rw-r--r--   0        0        0     1130 2024-02-16 20:50:49.849214 indexify-0.0.8/indexify/extractor.py
--rw-r--r--   0        0        0      721 2024-02-16 20:50:49.849214 indexify-0.0.8/indexify/extractor_binding.py
--rw-r--r--   0        0        0      517 2024-02-16 20:50:49.849214 indexify-0.0.8/indexify/index.py
--rw-r--r--   0        0        0       46 2024-02-16 20:50:49.849214 indexify-0.0.8/indexify/settings.py
--rw-r--r--   0        0        0      282 2024-02-16 20:50:49.849214 indexify-0.0.8/indexify/utils.py
--rw-r--r--   0        0        0      688 2024-02-16 20:50:49.849214 indexify-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1713 1970-01-01 00:00:00.000000 indexify-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-17 20:26:27.020300 indexify-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0     1056 2024-02-17 20:26:27.020300 indexify-0.0.9/README.md
+-rw-r--r--   0        0        0      251 2024-02-17 20:26:27.020300 indexify-0.0.9/indexify/__init__.py
+-rw-r--r--   0        0        0    12999 2024-02-17 20:26:27.020300 indexify-0.0.9/indexify/client.py
+-rw-r--r--   0        0        0      361 2024-02-17 20:26:27.020300 indexify-0.0.9/indexify/data_containers.py
+-rw-r--r--   0        0        0      111 2024-02-17 20:26:27.020300 indexify-0.0.9/indexify/exceptions.py
+-rw-r--r--   0        0        0      721 2024-02-17 20:26:27.020300 indexify-0.0.9/indexify/extraction_policy.py
+-rw-r--r--   0        0        0     1130 2024-02-17 20:26:27.020300 indexify-0.0.9/indexify/extractor.py
+-rw-r--r--   0        0        0      504 2024-02-17 20:26:27.020300 indexify-0.0.9/indexify/index.py
+-rw-r--r--   0        0        0       46 2024-02-17 20:26:27.020300 indexify-0.0.9/indexify/settings.py
+-rw-r--r--   0        0        0      125 2024-02-17 20:26:27.020300 indexify-0.0.9/indexify/utils.py
+-rw-r--r--   0        0        0      688 2024-02-17 20:26:27.024300 indexify-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1713 1970-01-01 00:00:00.000000 indexify-0.0.9/PKG-INFO
```

### Comparing `indexify-0.0.8/LICENSE.txt` & `indexify-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `indexify-0.0.8/README.md` & `indexify-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `indexify-0.0.8/indexify/client.py` & `indexify-0.0.9/indexify/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import httpx
 import json
 from collections import namedtuple
 from .settings import DEFAULT_SERVICE_URL
 from .extractor import Extractor
-from .extractor_binding import ExtractorBinding
+from .extraction_policy import ExtractionPolicy
 from .index import Index
 from .utils import json_set_default
 from .data_containers import TextChunk
 from indexify.exceptions import ApiException
 
 from typing import List, Optional, Union
 
@@ -37,26 +37,26 @@
         self,
         service_url: str = DEFAULT_SERVICE_URL,
         namespace: str = "default",
         *args,
         **kwargs,
     ):
         self.namespace: str = namespace
-        self.extractor_bindings: List[ExtractorBinding] = []
+        self.extraction_policies: List[ExtractionPolicy] = []
         self.labels: dict = {}
         self._service_url = service_url
         self._client = httpx.Client(*args, **kwargs)
 
         # get namespace data
         response = self.get(f"namespaces/{self.namespace}")
         response.raise_for_status()
         resp_json = response.json()
         # initialize extractor_bindings
-        for eb in resp_json["namespace"]["extractor_bindings"]:
-            self.extractor_bindings.append(ExtractorBinding.from_dict(eb))
+        for eb in resp_json["namespace"]["extraction_policies"]:
+            self.extraction_policies.append(ExtractionPolicy.from_dict(eb))
 
     @classmethod
     def with_mtls(
         cls,
         cert_path: str,
         key_path: str,
         ca_bundle_path: Optional[str] = None,
@@ -185,32 +185,32 @@
             namespaces.append(item["name"])
         return namespaces
 
     @classmethod
     def create_namespace(
         self,
         namespace: str,
-        extractor_bindings: list = [],
+        extraction_policies: list = [],
         labels: dict = {},
     ) -> "IndexifyClient":
         """
         Create a new namespace.
 
         Returns:
             IndexifyClient: a new client with the given namespace
         """
-        bindings = []
-        for bd in extractor_bindings:
-            if isinstance(bd, ExtractorBinding):
-                bindings.append(bd.to_dict())
+        extraction_policies = []
+        for bd in extraction_policies:
+            if isinstance(bd, ExtractionPolicy):
+                extraction_policies.append(bd.to_dict())
             else:
-                bindings.append(bd)
+                extraction_policies.append(bd)
         req = {
             "name": namespace,
-            "extractor_bindings": bindings,
+            "extraction_policies": extraction_policies,
             "labels": labels,
         }
 
         client = IndexifyClient(namespace=namespace)
         client.post(f"namespaces", json=req)
         return client
 
@@ -235,70 +235,70 @@
         response = self.get(f"extractors")
         extractors_dict = response.json()["extractors"]
         extractors = []
         for ed in extractors_dict:
             extractors.append(Extractor.from_dict(ed))
         return extractors
 
-    def get_extractor_bindings(self):
+    def get_extraction_policies(self):
         """
-        Retrieve and update the list of extractor bindings for the current namespace.
+        Retrieve and update the list of extraction policies for the current namespace.
         """
         response = self.get(f"namespaces/{self.namespace}")
         response.raise_for_status()
 
-        self.extractor_bindings = []
-        for eb in response.json()["namespace"]["extractor_bindings"]:
-            self.extractor_bindings.append(ExtractorBinding.from_dict(eb))
-        return self.extractor_bindings
+        self.extraction_policies = []
+        for eb in response.json()["namespace"]["extraction_policies"]:
+            self.extraction_policies.append(ExtractionPolicy.from_dict(eb))
+        return self.extraction_policies
 
-    def bind_extractor(
+    def add_extraction_policy(
         self,
         extractor: str,
         name: str,
         input_params: dict = {},
         labels_eq: str = None,
         content_source="ingestion",
     ) -> dict:
-        """Bind an extractor.
+        """Add a new extraction policy.
 
         Args:
             - extractor (str): Name of the extractor
             - name (str): Name for this instance
             - input_params (dict): Dictionary containing extractor input params
             - filter (Filter): Optional filter for this extractor
 
         Returns:
             dict: response payload
 
         Examples:
-            >>> repo.bind_extractor("EfficientNet", "efficientnet")
+            >>> repo.add_extraction_policy("EfficientNet", "efficientnet")
 
-            >>> repo.bind_extractor("MiniLML6", "minilm")
+            >>> repo.add_extraction_policy("MiniLML6", "minilm")
 
         """
         req = {
             "extractor": extractor,
             "name": name,
             "input_params": input_params,
             "filters_eq": labels_eq,
             "content_source": content_source,
         }
         if req["filters_eq"] == None:
             del req["filters_eq"]
 
         request_body = json.dumps(req, default=json_set_default)
         response = self.post(
-            f"namespaces/{self.namespace}/extractor_bindings",
+            f"namespaces/{self.namespace}/extraction_policies",
             data=request_body,
             headers={"Content-Type": "application/json"},
         )
 
         # update self.extractor_bindings
-        self.get_extractor_bindings()
+        self.get_extraction_policies()
 
         try:
             response.raise_for_status()
         except httpx.HTTPStatusError as exc:
             raise ApiException(exc.response.text)
         return
```

### Comparing `indexify-0.0.8/indexify/extractor.py` & `indexify-0.0.9/indexify/extractor.py`

 * *Files identical despite different names*

### Comparing `indexify-0.0.8/indexify/extractor_binding.py` & `indexify-0.0.9/indexify/extraction_policy.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from dataclasses import dataclass, asdict
 from typing import Optional
 
 
 @dataclass
-class ExtractorBinding:
+class ExtractionPolicy:
     extractor: str
     name: str
     content_source: str
     input_params: dict
     labels_eq: Optional[str] = None
 
     def __repr__(self) -> str:
-        return f"ExtractorBinding(name={self.name} extractor={self.extractor})"
+        return f"ExtractionPolicy(name={self.name} extractor={self.extractor})"
 
     def __str__(self) -> str:
         return self.__repr__()
 
     def to_dict(self) -> dict:
         filtered_dict = {k: v for k, v in asdict(self).items() if v is not None}
         return filtered_dict
 
     @classmethod
     def from_dict(cls, json: dict):
         if "filters_eq" in json:
             json["labels_eq"] = json.pop("filters_eq")
-        return ExtractorBinding(**json)
+        return ExtractionPolicy(**json)
```

### Comparing `indexify-0.0.8/pyproject.toml` & `indexify-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "indexify"
-version = "0.0.8"
+version = "0.0.9"
 description = "Python Client for Indexify"
 authors = ["Diptanu Gon Choudhury <diptanuc@gmail.com>", "Vijay Parthasarathy <vijay2win@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 homepage = "https://github.com/tensorlakeai/indexify"
 repository = "https://github.com/tensorlakeai/indexify"
```

### Comparing `indexify-0.0.8/PKG-INFO` & `indexify-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indexify
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python Client for Indexify
 Home-page: https://github.com/tensorlakeai/indexify
 License: Apache 2.0
 Author: Diptanu Gon Choudhury
 Author-email: diptanuc@gmail.com
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: License :: Other/Proprietary License
```

