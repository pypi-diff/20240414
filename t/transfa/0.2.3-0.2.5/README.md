# Comparing `tmp/transfa-0.2.3.tar.gz` & `tmp/transfa-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transfa-0.2.3.tar", last modified: Mon Apr 24 14:17:16 2023, max compression
+gzip compressed data, was "transfa-0.2.5.tar", last modified: Sun Apr 14 16:30:45 2024, max compression
```

## Comparing `transfa-0.2.3.tar` & `transfa-0.2.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:17:16.721100 transfa-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-24 14:17:00.000000 transfa-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-24 14:17:16.721100 transfa-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-04-24 14:17:00.000000 transfa-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-24 14:17:00.000000 transfa-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-04-24 14:17:16.721100 transfa-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:17:00.000000 transfa-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:17:16.717100 transfa-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-04-24 14:17:00.000000 transfa-0.2.3/tests/test_payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-04-24 14:17:00.000000 transfa-0.2.3/tests/test_webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:17:16.717100 transfa-0.2.3/transfa/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-24 14:17:00.000000 transfa-0.2.3/transfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-24 14:17:00.000000 transfa-0.2.3/transfa/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:17:16.721100 transfa-0.2.3/transfa/api_resources/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-24 14:17:00.000000 transfa-0.2.3/transfa/api_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-24 14:17:00.000000 transfa-0.2.3/transfa/api_resources/payments.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-04-24 14:17:00.000000 transfa-0.2.3/transfa/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-24 14:17:00.000000 transfa-0.2.3/transfa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-24 14:17:00.000000 transfa-0.2.3/transfa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-04-24 14:17:00.000000 transfa-0.2.3/transfa/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:17:16.721100 transfa-0.2.3/transfa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-04-24 14:17:16.000000 transfa-0.2.3/transfa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-24 14:17:16.000000 transfa-0.2.3/transfa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:17:16.000000 transfa-0.2.3/transfa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:17:16.000000 transfa-0.2.3/transfa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 14:17:16.000000 transfa-0.2.3/transfa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 14:17:16.000000 transfa-0.2.3/transfa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:30:45.172134 transfa-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-14 16:30:41.000000 transfa-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-14 16:30:45.172134 transfa-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-04-14 16:30:41.000000 transfa-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-14 16:30:41.000000 transfa-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-14 16:30:45.176133 transfa-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 16:30:41.000000 transfa-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:30:45.172134 transfa-0.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-04-14 16:30:41.000000 transfa-0.2.5/tests/test_payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-14 16:30:41.000000 transfa-0.2.5/tests/test_webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:30:45.172134 transfa-0.2.5/transfa/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-14 16:30:41.000000 transfa-0.2.5/transfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-14 16:30:41.000000 transfa-0.2.5/transfa/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:30:45.172134 transfa-0.2.5/transfa/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-14 16:30:41.000000 transfa-0.2.5/transfa/api_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-14 16:30:41.000000 transfa-0.2.5/transfa/api_resources/payments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-14 16:30:41.000000 transfa-0.2.5/transfa/api_resources/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:30:45.172134 transfa-0.2.5/transfa/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 16:30:41.000000 transfa-0.2.5/transfa/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-14 16:30:41.000000 transfa-0.2.5/transfa/configs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 16:30:45.172134 transfa-0.2.5/transfa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-14 16:30:45.000000 transfa-0.2.5/transfa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-14 16:30:45.000000 transfa-0.2.5/transfa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 16:30:45.000000 transfa-0.2.5/transfa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 16:30:44.000000 transfa-0.2.5/transfa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-14 16:30:45.000000 transfa-0.2.5/transfa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 16:30:45.000000 transfa-0.2.5/transfa.egg-info/top_level.txt
```

### Comparing `transfa-0.2.3/LICENSE` & `transfa-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `transfa-0.2.3/PKG-INFO` & `transfa-0.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transfa
-Version: 0.2.3
+Version: 0.2.5
 Summary: This is the official python SDK for the Transfa API.
 Home-page: https://transfapp.com
 Author: Kolawole Mangabo
 Author-email: kolawole.mangabo@transfapp.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -13,16 +13,20 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: requests>=2.20
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: responses; extra == "test"
+Requires-Dist: coverage; extra == "test"
 
 # Transfa Python SDK
 
 The Transfa Python SDK provides methods and resources to the Transfa API for applications written in Python. 
 
 ## Documentation
```

### Comparing `transfa-0.2.3/README.md` & `transfa-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `transfa-0.2.3/setup.cfg` & `transfa-0.2.5/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [bumpversion]
-current_version = 0.2.3
+current_version = 0.2.5
 commit = True
 tag = True
 
 [bumpversion:file:pyproject.toml]
 search = version = "{current_version}"
 replace = version = "{new_version}"
 
-[bumpversion:file:transfa/version.py]
+[bumpversion:file:transfa/configs/version.py]
 search = VERSION = "{current_version}"
 replace = VERSION = "{new_version}"
 
 [bumpversion:file:CHANGELOG.md]
 search = 
 	[Unreleased]
 	------------
```

### Comparing `transfa-0.2.3/tests/test_payment.py` & `transfa-0.2.5/tests/test_payment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import uuid
 from http import HTTPStatus
 
 import responses
 from responses import matchers
 
-from transfa import default_auth_header_bearer
-
 from transfa.api_client import client
-from transfa.version import VERSION
+from transfa.configs.version import VERSION
 
 client.api_key = "ak_live_123"
 API_URL = "https://api.transfapp.com/api/v1/optimus/payment/"
 
 
 def paginator_response(data):
     return {"count": len(data), "results": data}
@@ -28,15 +26,15 @@
         responses.POST,
         API_URL,
         json=payment,
         status=HTTPStatus.CREATED,
         match=[
             matchers.header_matcher(
                 {
-                    "Authorization": f"{default_auth_header_bearer} {client.api_key}",
+                    "Authorization": f"{client.api_key}",
                     "accept": "application/json",
                     "content-type": "application/json;charset=utf-8",
                     "Idempotency-Key": idempotency_key,
                     "user-agent": "Transfa API SDK-Python/%s" % VERSION,
                 }
             )
         ],
@@ -64,15 +62,15 @@
         responses.GET,
         API_URL,
         json=paginator_response(payments),
         status=HTTPStatus.OK,
         match=[
             matchers.header_matcher(
                 {
-                    "Authorization": f"{default_auth_header_bearer} {client.api_key}",
+                    "Authorization": f"{client.api_key}",
                     "user-agent": "Transfa API SDK-Python/%s" % VERSION,
                 }
             )
         ],
     )
 
     response = client.Payment.list()
@@ -93,15 +91,15 @@
         responses.GET,
         f"{API_URL}{payment['id']}/",
         json=payment,
         status=HTTPStatus.OK,
         match=[
             matchers.header_matcher(
                 {
-                    "Authorization": f"{default_auth_header_bearer} {client.api_key}",
+                    "Authorization": f"{client.api_key}",
                     "user-agent": "Transfa API SDK-Python/%s" % VERSION,
                 }
             ),
             matchers.query_param_matcher({}),
         ],
     )
 
@@ -123,15 +121,15 @@
         responses.POST,
         f"{API_URL}{payment['id']}/refund/",
         json=payment,
         status=HTTPStatus.OK,
         match=[
             matchers.header_matcher(
                 {
-                    "Authorization": f"{default_auth_header_bearer} {client.api_key}",
+                    "Authorization": f"{client.api_key}",
                     "user-agent": "Transfa API SDK-Python/%s" % VERSION,
                 }
             )
         ],
     )
 
     response = client.Payment.refund(payment["id"])
```

### Comparing `transfa-0.2.3/tests/test_webhook.py` & `transfa-0.2.5/tests/test_webhook.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import hmac
 import hashlib
 import json
 
-from transfa.webhook import Webhook
-from transfa.utils import get_random_string
+from transfa.api_resources.webhook import WebhookResource
+from transfa.utils.helpers import get_random_string
 
 
 class WebhookData:
-
     def __init__(self):
         self.valid_webhook_token = get_random_string(64)
         self.invalid_webhook_token = get_random_string(64)
 
     def generate_signature(self, body, webhook_token, algorithm=hashlib.sha512):
         body = json.dumps(body)
         secret = webhook_token.encode("utf-8")
@@ -22,55 +21,71 @@
         signature = hmac.new(secret, body, digestmod=algorithm)
 
         return signature.hexdigest()
 
 
 def test_valid_webhook_signature(valid_webhook_payload):
     webhook_data = WebhookData()
-    signature = webhook_data.generate_signature(valid_webhook_payload, webhook_data.valid_webhook_token)
-
-    webhook = Webhook(webhook_token=webhook_data.valid_webhook_token, body=valid_webhook_payload, headers={
-        "X-Webhook-Transfa-Signature": signature
-    })
+    signature = webhook_data.generate_signature(
+        valid_webhook_payload, webhook_data.valid_webhook_token
+    )
+
+    webhook = WebhookResource(
+        webhook_token=webhook_data.valid_webhook_token,
+        body=valid_webhook_payload,
+        headers={"X-Webhook-Transfa-Signature": signature},
+    )
 
     verified = webhook.verify()
 
     assert verified == valid_webhook_payload
 
 
 def test_invalid_webhook_signature(valid_webhook_payload, invalid_webhook_payload):
     webhook_data = WebhookData()
-    invalid_signature = webhook_data.generate_signature(invalid_webhook_payload, webhook_data.valid_webhook_token)
-
-    webhook = Webhook(webhook_token=webhook_data.valid_webhook_token, body=valid_webhook_payload, headers={
-        "X-Webhook-Transfa-Signature": invalid_signature
-    })
+    invalid_signature = webhook_data.generate_signature(
+        invalid_webhook_payload, webhook_data.valid_webhook_token
+    )
+
+    webhook = WebhookResource(
+        webhook_token=webhook_data.valid_webhook_token,
+        body=valid_webhook_payload,
+        headers={"X-Webhook-Transfa-Signature": invalid_signature},
+    )
 
     verified = webhook.verify()
 
     assert not verified
 
 
 def test_valid_webhook_token(valid_webhook_payload):
     webhook_data = WebhookData()
-    valid_signature = webhook_data.generate_signature(valid_webhook_payload, webhook_data.valid_webhook_token)
-
-    webhook = Webhook(webhook_token=webhook_data.valid_webhook_token, body=valid_webhook_payload, headers={
-        "X-Webhook-Transfa-Signature": valid_signature
-    })
+    valid_signature = webhook_data.generate_signature(
+        valid_webhook_payload, webhook_data.valid_webhook_token
+    )
+
+    webhook = WebhookResource(
+        webhook_token=webhook_data.valid_webhook_token,
+        body=valid_webhook_payload,
+        headers={"X-Webhook-Transfa-Signature": valid_signature},
+    )
 
     verified = webhook.verify()
 
     assert verified == valid_webhook_payload
 
 
 def test_invalid_webhook_token(valid_webhook_payload):
     webhook_data = WebhookData()
-    valid_signature = webhook_data.generate_signature(valid_webhook_payload, webhook_data.valid_webhook_token)
-
-    webhook = Webhook(webhook_token=webhook_data.invalid_webhook_token, body=valid_webhook_payload, headers={
-        "X-Webhook-Transfa-Signature": valid_signature
-    })
+    valid_signature = webhook_data.generate_signature(
+        valid_webhook_payload, webhook_data.valid_webhook_token
+    )
+
+    webhook = WebhookResource(
+        webhook_token=webhook_data.invalid_webhook_token,
+        body=valid_webhook_payload,
+        headers={"X-Webhook-Transfa-Signature": valid_signature},
+    )
 
     verified = webhook.verify()
 
     assert not verified
```

### Comparing `transfa-0.2.3/transfa/api_client.py` & `transfa-0.2.5/transfa/api_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import json
 
 from requests import request
 
-from transfa import api_key, api_base, default_auth_header_bearer
+from transfa import api_key, api_base
 from transfa.api_resources.payments import PaymentResource
 
-from transfa.version import VERSION
+from transfa.configs.version import VERSION
 
 
 class TransfaAPIClient:
     _base_url = api_base
-    auth_header_prefix = default_auth_header_bearer
     __version__ = VERSION
 
     def __init__(
         self,
         timeout=5,
         verify_ssl=True,
     ):
@@ -40,15 +39,15 @@
         if params is None:
             params = {}
 
         url = self._get_url(endpoint)
         headers = {
             "user-agent": "Transfa API SDK-Python/%s" % self.__version__,
             "accept": "application/json",
-            "Authorization": f"{self.auth_header_prefix} {self.api_key}",
+            "Authorization": f"{self.api_key}",
         }
 
         if "headers" in kwargs:
             headers = {**kwargs.pop("headers"), **headers}
 
         if data is not None:
             data = json.dumps(data, ensure_ascii=False).encode("utf-8")
```

### Comparing `transfa-0.2.3/transfa/api_resources/payments.py` & `transfa-0.2.5/transfa/api_resources/payments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import uuid
 
-from transfa.enums import PaymentTypeEnum
-from transfa.utils import get_default_error_log_message
+from transfa.types.enums import PaymentTypeEnum
+from transfa.utils.helpers import get_default_error_log_message
 
 
 class PaymentResource:
     """
     This class contains methods and utils used for interacting with the payment API.
     """
 
@@ -74,14 +74,14 @@
         if response.status_code != 200:
             logging.error(get_default_error_log_message(response))
 
         response_data = response.json()
 
         status_data = {
             "status": response_data.get("status"),
-            "financial_status": response_data.get("financial_status")
-        } 
+            "financial_status": response_data.get("financial_status"),
+        }
 
         return status_data
 
 
 Payment = PaymentResource
```

### Comparing `transfa-0.2.3/transfa/webhook.py` & `transfa-0.2.5/transfa/api_resources/webhook.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 import hmac
 import hashlib
 import json
 
 from transfa import private_secret
-from transfa.enums import TransfaHeadersIdentifiers
+from transfa.types.enums import TransfaHeadersIdentifiers
 
 
-class Webhook:
+class WebhookResource:
     def __init__(self, webhook_token=private_secret, body=None, headers=None):
         if webhook_token is None:
             raise NotImplementedError(
                 "Can't work without private secret for security reasons."
             )
 
         if body is None:
-            raise NotImplementedError(
-                "Can't work without the body of the request."
-            )
+            raise NotImplementedError("Can't work without the body of the request.")
 
         if headers is None:
-            raise NotImplementedError(
-                "Can't work without the headers."
-            )
+            raise NotImplementedError("Can't work without the headers.")
 
         if isinstance(body, bytes):
             body = body.decode("utf-8")
             body = json.loads(body)
 
         self.webhook_token = webhook_token
         self.headers = headers
@@ -38,15 +34,14 @@
             body = body.encode("utf-8")
 
         signature = hmac.new(secret, body, digestmod=algorithm)
 
         return signature.hexdigest()
 
     def has_data_not_tempered(self, body, transfa_api_signature):
-
         if isinstance(body, dict):
             body = json.dumps(body)
 
         signature = self.sign_body(body)
         return signature == transfa_api_signature
 
     def verify(self):
```

### Comparing `transfa-0.2.3/transfa.egg-info/PKG-INFO` & `transfa-0.2.5/transfa.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transfa
-Version: 0.2.3
+Version: 0.2.5
 Summary: This is the official python SDK for the Transfa API.
 Home-page: https://transfapp.com
 Author: Kolawole Mangabo
 Author-email: kolawole.mangabo@transfapp.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -13,16 +13,20 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
-Provides-Extra: test
 License-File: LICENSE
+Requires-Dist: requests>=2.20
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: responses; extra == "test"
+Requires-Dist: coverage; extra == "test"
 
 # Transfa Python SDK
 
 The Transfa Python SDK provides methods and resources to the Transfa API for applications written in Python. 
 
 ## Documentation
```

