# Comparing `tmp/openapi_service_client-0.0.5.tar.gz` & `tmp/openapi_service_client-0.0.6.tar.gz`

## Comparing `openapi_service_client-0.0.5.tar` & `openapi_service_client-0.0.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/.github/workflows/pypi_release.yml
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/.github/workflows/tests.yml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/__init__.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/client.py
--rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/client_configuration.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/config/__init__.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/config/auth_strategy.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/config/configuration.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/http_client/__init__.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/http_client/client.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/providers/__init__.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/providers/anthropic.py
--rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/providers/cohere.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/providers/converter.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/providers/llm_provider.py
--rw-r--r--   0        0        0     7295 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/providers/openai.py
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/providers/payload_extractor.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/request_builder/__init__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/request_builder/builder.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/spec/__init__.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/spec/open_api_spec.py
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/src/openapi_service_client/spec/operation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/__init__.py
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_client.py
--rw-r--r--   0        0        0     9768 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_client_auth.py
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_client_complex_request_body.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_client_complex_request_body_mixed.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_client_edge_cases.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_client_error_handling.py
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_client_live.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_client_live_anthropic.py
--rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_client_live_cohere.py
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_client_live_openai.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_cohere_conversion.py
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/client/test_openai_conversion.py
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/test_files/complex_types_openapi_service.json
--rw-r--r--   0        0        0    12430 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/test_files/github_compare.yml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/test_files/openapi_edge_cases.yml
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/test_files/openapi_error_handling.yml
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/test_files/openapi_greeting_service.yml
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/test_files/openapi_order_service.json
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/test_files/openapi_order_service.yml
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/tests/test_files/serper.yaml
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/LICENSE
--rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/README.md
--rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 openapi_service_client-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/.github/workflows/pypi_release.yml
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/__init__.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/client.py
+-rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/client_configuration.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/config/__init__.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/config/auth_strategy.py
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/config/configuration.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/http_client/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/http_client/client.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/providers/__init__.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/providers/anthropic.py
+-rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/providers/cohere.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/providers/converter.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/providers/llm_provider.py
+-rw-r--r--   0        0        0     7295 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/providers/openai.py
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/providers/payload_extractor.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/request_builder/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/request_builder/builder.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/spec/__init__.py
+-rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/spec/open_api_spec.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/src/openapi_service_client/spec/operation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/__init__.py
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_client.py
+-rw-r--r--   0        0        0     9768 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_client_auth.py
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_client_complex_request_body.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_client_complex_request_body_mixed.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_client_edge_cases.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_client_error_handling.py
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_client_live.py
+-rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_client_live_anthropic.py
+-rw-r--r--   0        0        0     2807 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_client_live_cohere.py
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_client_live_openai.py
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_cohere_conversion.py
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/client/test_openai_conversion.py
+-rw-r--r--   0        0        0     2782 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/test_files/complex_types_openapi_service.json
+-rw-r--r--   0        0        0    12430 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/test_files/github_compare.yml
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/test_files/openapi_edge_cases.yml
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/test_files/openapi_error_handling.yml
+-rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/test_files/openapi_greeting_service.yml
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/test_files/openapi_order_service.json
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/test_files/openapi_order_service.yml
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/tests/test_files/serper.yaml
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/LICENSE
+-rw-r--r--   0        0        0     7889 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/README.md
+-rw-r--r--   0        0        0     3931 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     8836 2020-02-02 00:00:00.000000 openapi_service_client-0.0.6/PKG-INFO
```

### Comparing `openapi_service_client-0.0.5/.github/workflows/tests.yml` & `openapi_service_client-0.0.6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/src/openapi_service_client/client.py` & `openapi_service_client-0.0.6/src/openapi_service_client/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,23 @@
 from typing import Any, Dict
 
 from openapi_service_client.client_configuration import ClientConfiguration
-from openapi_service_client.http_client import VALID_HTTP_METHODS
 from openapi_service_client.request_builder import RequestBuilder
-from openapi_service_client.spec import Operation
 
 
 class OpenAPIServiceClient:
     def __init__(
         self,
         client_config: ClientConfiguration,
     ):
         self.openapi_spec = client_config.get_openapi_spec()
         self.http_client = client_config.get_http_client()
         self.request_builder = RequestBuilder(client_config)
         self.payload_extractor = client_config.get_payload_extractor()
 
-    def get_operations(self) -> Dict[str, Dict[str, Operation]]:
-        operations: Dict[str, Dict[str, Operation]] = {}
-        for path, path_item in self.openapi_spec.get_paths().items():
-            operations[path] = {}
-            for method, operation in path_item.items():
-                if method in VALID_HTTP_METHODS:
-                    operations[path][method] = operation
-        return operations
-
     def invoke(self, function_payload: Dict[str, Any]) -> Any:
         fn_invocation_payload = self.payload_extractor.extract_function_invocation(function_payload)
         if not fn_invocation_payload:
             raise OpenAPIClientError(
                 f"Failed to extract function invocation payload from {function_payload} using "
                 f"{self.payload_extractor.__class__.__name__}. Ensure the payload format matches the expected "
                 "structure for the designated LLM extractor."
```

### Comparing `openapi_service_client-0.0.5/src/openapi_service_client/client_configuration.py` & `openapi_service_client-0.0.6/src/openapi_service_client/client_configuration.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Protocol, Union
+from urllib.parse import urlparse
 
 from openapi_service_client.config import (
     ApiKeyAuthentication,
     AuthenticationStrategy,
     HTTPAuthentication,
     HttpClientConfig,
     OAuthAuthentication,
@@ -47,14 +48,19 @@
         http_client_config: Optional[HttpClientConfig] = None,
         provider: Optional[LLMProvider] = None,
     ):
         if isinstance(openapi_spec, (str, Path)) and os.path.isfile(openapi_spec):
             self.openapi_spec = OpenAPISpecification.from_file(openapi_spec)
         elif isinstance(openapi_spec, dict):
             self.openapi_spec = OpenAPISpecification.from_dict(openapi_spec)
+        elif isinstance(openapi_spec, str):
+            if self.is_valid_http_url(openapi_spec):
+                self.openapi_spec = OpenAPISpecification.from_url(openapi_spec)
+            else:
+                self.openapi_spec = OpenAPISpecification.from_str(openapi_spec)
         else:
             raise ValueError("Invalid OpenAPI specification format. Expected file path or dictionary.")
 
         self.credentials = credentials
         self.http_client = http_client or RequestsHttpClient(http_client_config)
         self.http_client_config = http_client_config or HttpClientConfig()
         self.provider = provider or OpenAILLMProvider()
@@ -111,14 +117,19 @@
             return HTTPAuthentication(token=credentials["token"])
         elif "access_token" in credentials:
             token_type = credentials.get("token_type", "Bearer")
             return OAuthAuthentication(access_token=credentials["access_token"], token_type=token_type)
         else:
             raise ValueError("Unable to create authentication from provided credentials: {credentials}")
 
+    def is_valid_http_url(self, url: str) -> bool:
+        """Check if a URL is a valid HTTP/HTTPS URL."""
+        r = urlparse(url)
+        return all([r.scheme in ["http", "https"], r.netloc])
+
 
 class ClientConfigurationBuilder:
     def __init__(self):
         self._openapi_spec: Union[str, Path, None] = None
         self._credentials: Optional[Union[str, Dict[str, Any], AuthenticationStrategy]] = None
         self._http_client: Optional[AbstractHttpClient] = None
         self._http_client_config: Optional[HttpClientConfig] = None
```

### Comparing `openapi_service_client-0.0.5/src/openapi_service_client/config/configuration.py` & `openapi_service_client-0.0.6/src/openapi_service_client/config/configuration.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/src/openapi_service_client/http_client/client.py` & `openapi_service_client-0.0.6/src/openapi_service_client/http_client/client.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/src/openapi_service_client/providers/__init__.py` & `openapi_service_client-0.0.6/src/openapi_service_client/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/src/openapi_service_client/providers/anthropic.py` & `openapi_service_client-0.0.6/src/openapi_service_client/providers/anthropic.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/src/openapi_service_client/providers/cohere.py` & `openapi_service_client-0.0.6/src/openapi_service_client/providers/cohere.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/src/openapi_service_client/providers/openai.py` & `openapi_service_client-0.0.6/src/openapi_service_client/providers/openai.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/src/openapi_service_client/providers/payload_extractor.py` & `openapi_service_client-0.0.6/src/openapi_service_client/providers/payload_extractor.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/src/openapi_service_client/request_builder/builder.py` & `openapi_service_client-0.0.6/src/openapi_service_client/request_builder/builder.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/src/openapi_service_client/spec/open_api_spec.py` & `openapi_service_client-0.0.6/src/openapi_service_client/spec/open_api_spec.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import logging
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
+import requests
 import yaml
 
 from openapi_service_client.http_client import VALID_HTTP_METHODS
 from openapi_service_client.spec.operation import Operation
 
 logger = logging.getLogger(__name__)
 
@@ -18,28 +19,46 @@
     @classmethod
     def from_dict(cls, spec_dict: Dict[str, Any]) -> "OpenAPISpecification":
         parser = cls({})
         parser.spec_dict = spec_dict
         return parser
 
     @classmethod
-    def from_file(cls, spec_file: Union[str, Path]) -> "OpenAPISpecification":
-        loaded_spec: Dict[str, Any]
-        with open(spec_file, encoding="utf-8") as file:
-            content = file.read()
+    def from_str(cls, content: str) -> "OpenAPISpecification":
+        if not isinstance(content, str):
+            raise ValueError(f"Invalid schema {content}. Provide a valid OpenAPI schema.")
+        if "openapi" not in content or "paths" not in content or "servers" not in content:
+            raise ValueError(
+                "Invalid OpenAPI specification format. See https://swagger.io/specification/ for details.", content
+            )
         try:
             loaded_spec = json.loads(content)
         except json.JSONDecodeError:
             try:
                 loaded_spec = yaml.safe_load(content)
             except yaml.YAMLError as e:
-                raise ValueError("File cannot be decoded as JSON or YAML: " + str(e)) from e
-
+                raise ValueError("Content cannot be decoded as JSON or YAML: " + str(e)) from e
         return cls(loaded_spec)
 
+    @classmethod
+    def from_file(cls, spec_file: Union[str, Path]) -> "OpenAPISpecification":
+        with open(spec_file, encoding="utf-8") as file:
+            content = file.read()
+        return cls.from_str(content)
+
+    @classmethod
+    def from_url(cls, url: str) -> "OpenAPISpecification":
+        try:
+            response = requests.get(url, timeout=10)
+            response.raise_for_status()
+            content = response.text
+        except requests.RequestException as e:
+            raise ConnectionError(f"Failed to fetch the specification from URL: {url}. {e!s}") from e
+        return cls.from_str(content)
+
     def get_paths(self) -> Dict[str, Dict[str, Any]]:
         return self.spec_dict.get("paths", {})
 
     def get_operation(self, path: str, method: Optional[str] = None) -> Operation:
         path_item = self.get_paths().get(path, {})
         return self.get_operation_item(path, path_item, method)
```

### Comparing `openapi_service_client-0.0.5/src/openapi_service_client/spec/operation.py` & `openapi_service_client-0.0.6/src/openapi_service_client/spec/operation.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/tests/conftest.py` & `openapi_service_client-0.0.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/tests/client/test_client.py` & `openapi_service_client-0.0.6/tests/client/test_client.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/tests/client/test_client_auth.py` & `openapi_service_client-0.0.6/tests/client/test_client_auth.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/tests/client/test_client_complex_request_body.py` & `openapi_service_client-0.0.6/tests/client/test_client_complex_request_body.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/tests/client/test_client_complex_request_body_mixed.py` & `openapi_service_client-0.0.6/tests/client/test_client_complex_request_body_mixed.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/tests/client/test_client_edge_cases.py` & `openapi_service_client-0.0.6/tests/client/test_client_edge_cases.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/tests/client/test_client_error_handling.py` & `openapi_service_client-0.0.6/tests/client/test_client_error_handling.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/tests/client/test_client_live.py` & `openapi_service_client-0.0.6/tests/client/test_client_live.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/tests/client/test_client_live_anthropic.py` & `openapi_service_client-0.0.6/tests/client/test_client_live_anthropic.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 from openapi_service_client.providers import AnthropicLLMProvider
 
 
 class TestClientLiveAnthropic:
 
     @pytest.mark.skipif("SERPERDEV_API_KEY" not in os.environ, reason="SERPERDEV_API_KEY not set")
     @pytest.mark.skipif("ANTHROPIC_API_KEY" not in os.environ, reason="ANTHROPIC_API_KEY not set")
-    def test_serperdev(self, test_files_path):
+    def test_serperdev(self):
         builder = ClientConfigurationBuilder()
         config = (
-            builder.with_openapi_spec(test_files_path / "serper.yaml")
+            builder.with_openapi_spec("https://bit.ly/serper_dev_spec_yaml")
             .with_credentials(os.getenv("SERPERDEV_API_KEY"))
             .with_provider(AnthropicLLMProvider())
             .build()
         )
         client = anthropic.Anthropic(api_key=os.getenv("ANTHROPIC_API_KEY"))
         tool_choice = config.get_tools_definitions()
         response = client.beta.tools.messages.create(
```

### Comparing `openapi_service_client-0.0.5/tests/client/test_client_live_cohere.py` & `openapi_service_client-0.0.6/tests/client/test_client_live_cohere.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/tests/client/test_client_live_openai.py` & `openapi_service_client-0.0.6/tests/client/test_client_live_openai.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 from openapi_service_client.client_configuration import ClientConfigurationBuilder
 
 
 class TestClientLiveOpenAPI:
 
     @pytest.mark.skipif("SERPERDEV_API_KEY" not in os.environ, reason="SERPERDEV_API_KEY not set")
     @pytest.mark.skipif("OPENAI_API_KEY" not in os.environ, reason="OPENAI_API_KEY not set")
-    def test_serperdev(self, test_files_path):
+    def test_serperdev(self):
         builder = ClientConfigurationBuilder()
         config = (
-            builder.with_openapi_spec(test_files_path / "serper.yaml")
+            builder.with_openapi_spec("https://bit.ly/serper_dev_spec_yaml")
             .with_credentials(os.getenv("SERPERDEV_API_KEY"))
             .build()
         )
         client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))
         tool_choice = config.get_tools_definitions()
         response = client.chat.completions.create(
             model="gpt-3.5-turbo",
```

### Comparing `openapi_service_client-0.0.5/tests/client/test_cohere_conversion.py` & `openapi_service_client-0.0.6/tests/client/test_cohere_conversion.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/tests/client/test_openai_conversion.py` & `openapi_service_client-0.0.6/tests/client/test_openai_conversion.py`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/tests/test_files/complex_types_openapi_service.json` & `openapi_service_client-0.0.6/tests/test_files/complex_types_openapi_service.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.95%*

 * *Differences: {"'servers'": "{0: {'url': 'http://localhost'}}"}*

```diff
@@ -93,11 +93,11 @@
                 },
                 "summary": "Process a new payment"
             }
         }
     },
     "servers": [
         {
-            "url": "http://localhost:8080"
+            "url": "http://localhost"
         }
     ]
 }
```

### Comparing `openapi_service_client-0.0.5/tests/test_files/github_compare.yml` & `openapi_service_client-0.0.6/tests/test_files/github_compare.yml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/tests/test_files/openapi_greeting_service.yml` & `openapi_service_client-0.0.6/tests/test_files/openapi_greeting_service.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 openapi: 3.0.0
 info:
   title: Greeting Service
   version: 1.0.0
-
+servers:
+  - url: http://localhost # not used anyway
 paths:
   /greet/{name}:
     post:
       operationId: greet
       parameters:
         - name: name
           in: path
```

### Comparing `openapi_service_client-0.0.5/tests/test_files/openapi_order_service.json` & `openapi_service_client-0.0.6/tests/test_files/openapi_order_service.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'servers'": "[OrderedDict([('url', 'http://localhost')])]"}*

```diff
@@ -100,9 +100,14 @@
                         },
                         "description": "Created"
                     }
                 },
                 "summary": "Create a new order"
             }
         }
-    }
+    },
+    "servers": [
+        {
+            "url": "http://localhost"
+        }
+    ]
 }
```

### Comparing `openapi_service_client-0.0.5/tests/test_files/openapi_order_service.yml` & `openapi_service_client-0.0.6/tests/test_files/openapi_order_service.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 openapi: 3.0.0
 info:
   title: Order Service
   version: 1.0.0
-
+servers:
+  - url: http://localhost # not used anyway
 paths:
   /orders:
     post:
       summary: Create a new order
       operationId: createOrder
       requestBody:
         required: true
```

### Comparing `openapi_service_client-0.0.5/tests/test_files/serper.yaml` & `openapi_service_client-0.0.6/tests/test_files/serper.yaml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/.gitignore` & `openapi_service_client-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/LICENSE` & `openapi_service_client-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/pyproject.toml` & `openapi_service_client-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openapi_service_client-0.0.5/PKG-INFO` & `openapi_service_client-0.0.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.3
-Name: openapi-service-client
-Version: 0.0.5
-Summary: A client library for invoking APIs based on provided OpenAPI specifications
-Project-URL: Documentation, https://github.com/vblagoje/openapi-service-client/blob/main/README.md
-Project-URL: Issues, https://github.com/vblagoje/openapi-service-client/issues
-Project-URL: Source, https://github.com/vblagoje/openapi-service-client
-Author-email: Vladimir Blagojevic <dovlex@gmail.com>
-License-Expression: Apache-2.0
-License-File: LICENSE
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8
-Requires-Dist: jsonref
-Requires-Dist: pyyaml
-Requires-Dist: requests
-Description-Content-Type: text/markdown
-
 # OpenAPI Service Client
 [![PyPI - Version](https://img.shields.io/pypi/v/openapi-service-client.svg)](https://pypi.org/project/openapi-service-client)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openapi-service-client.svg)](https://pypi.org/project/openapi-service-client)
 
 
 OpenAPI Service Client is a Python library that enables effortless integration between Large Language Models (LLMs) and services defined by OpenAPI specifications. It provides a simple and intuitive way to invoke REST services using the function-calling JSON format, making it easy to integrate with LLM-generated function calls.
 
@@ -49,27 +27,33 @@
 
 ```shell
 pip install openapi-service-client
 ```
 
 ## Usage
 
-To effectively use the `OpenAPIServiceClient`, follow these steps to configure and invoke operations on your target API defined by an OpenAPI specification.
+To use `OpenAPIServiceClient`, follow these steps to configure and invoke operations on your target API (aka tool/service) defined by an OpenAPI specification.
 
 ### OpenAI Example
 
+To run the OpenAI example below, you need:
+1) Install openai package (`pip install openai`)
+2) OpenAI API key. You can obtain an OpenAI API key by signing up for an account on the OpenAI platform. See https://platform.openai.com/ for more details.
+3) SerperDev API key. This api key is required to access the SerperDev Google search engine API. See https://serper.dev/ for a quick signup and free credits. 
+
+
 ```python
 import os
 from openai import OpenAI
 from openapi_service_client.client import OpenAPIServiceClient
 from openapi_service_client.client_configuration import ClientConfigurationBuilder
 
 builder = ClientConfigurationBuilder()
 config = (
-    builder.with_openapi_spec("path/to/serper.yaml")
+    builder.with_openapi_spec("https://bit.ly/serper_dev_spec_yaml")
     .with_credentials(os.getenv("SERPERDEV_API_KEY"))
     .build()
 )
 
 client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))
 tool_choice = config.get_tools_definitions()
 response = client.chat.completions.create(
@@ -78,31 +62,37 @@
     tools=[{"type": "function", "function": tool_choice[0]}],
     tool_choice={"type": "function", "function": {"name": tool_choice[0]["name"]}},
 )
 
 tool_payloads = response.choices[0].message.tool_calls
 serper_api = OpenAPIServiceClient(config)
 response = serper_api.invoke(tool_payloads[0].to_dict())
-
-assert "inventions" in str(response)
+print(response)
 ```
 
 ### Anthropic Example
 
+To run the Anthropic Claude Opus example below, you need:
+
+1) Install anthropic package (`pip install anthropic`)
+2) Anthropic API key. You can obtain an Anthropic API key by signing up for an account on the Anthropic platform. See https://www.anthropic.com/ for more details.
+3) SerperDev API key. This api key is required to access the SerperDev Google search engine API. See https://serper.dev/ for a quick signup and free credits. 
+
+
 ```python
 import os
 import anthropic
 from openapi_service_client.client import OpenAPIServiceClient
 from openapi_service_client.client_configuration import ClientConfigurationBuilder
 from openapi_service_client.providers import AnthropicLLMProvider
 
 
 builder = ClientConfigurationBuilder()
 config = (
-    builder.with_openapi_spec("path/to/serper.yaml")
+    builder.with_openapi_spec("https://bit.ly/serper_dev_spec_yaml")
     .with_credentials(os.getenv("SERPERDEV_API_KEY"))
     .with_provider(AnthropicLLMProvider())
     .build()
 )
 
 client = anthropic.Anthropic(api_key=os.getenv("ANTHROPIC_API_KEY"))
 tool_choice = config.get_tools_definitions()
@@ -113,29 +103,35 @@
     tools=[tool_choice[0]],
     messages=[{"role": "user", "content": "Do a google search: Who was Nikola Tesla?"}],
 )
 
 tool_payload = response.content[1].to_dict()
 serper_api = OpenAPIServiceClient(config)
 response = serper_api.invoke(tool_payload)
-
-assert "inventions" in str(response)
+print(response)
 ```
 ### Cohere Example
 
+To run the Cohere Command-R example below, you need:
+
+1) Install cohere package (`pip install cohere`)
+2) Cohere API key. You can obtain Cohere API key by signing up for an account on the Cohere platform. See https://cohere.ai/ for more details.
+3) SerperDev API key. This api key is required to access the SerperDev Google search engine API. See https://serper.dev/ for a quick signup and free credits. 
+
+
 ```python
 import os
 import cohere
 from openapi_service_client.client import OpenAPIServiceClient
 from openapi_service_client.client_configuration import ClientConfigurationBuilder
 from openapi_service_client.providers import CohereLLMProvider
 
 builder = ClientConfigurationBuilder()
 config = (
-    builder.with_openapi_spec("path/to/serper.yaml")
+    builder.with_openapi_spec("https://bit.ly/serper_dev_spec_yaml")
     .with_credentials(os.getenv("SERPERDEV_API_KEY"))
     .with_provider(CohereLLMProvider())
     .build()
 )
 
 client = cohere.Client(api_key=os.getenv("COHERE_API_KEY"))
 tool_choices = config.get_tools_definitions()
@@ -146,16 +142,15 @@
     tools=tool_choices,
     message="Do a google search: Who was Nikola Tesla?",
 )
 
 tool_payload = response.tool_calls[0].dict()
 serper_api = OpenAPIServiceClient(config)
 response = serper_api.invoke(tool_payload)
-
-assert "inventions" in str(response)
+print(response)
 ```
 
 ## How It Works
 `OpenAPIServiceClient` simplifies the process of invoking REST services defined by OpenAPI specifications. It takes care of the complexities involved in making HTTP requests, handling authentication, and processing responses.
 
 When you provide an OpenAPI specification file to the client, it parses the specification and sets up the necessary request payloads and configurations to interact with the API based on the provided specification. You can then invoke specific operations using the OpenAI function-calling JSON format, which specifies the operation name and its arguments.
```

