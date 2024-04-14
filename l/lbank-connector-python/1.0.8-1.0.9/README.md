# Comparing `tmp/lbank-connector-python-1.0.8.tar.gz` & `tmp/lbank-connector-python-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lbank-connector-python-1.0.8.tar", last modified: Fri Mar 22 07:43:03 2024, max compression
+gzip compressed data, was "lbank-connector-python-1.0.9.tar", last modified: Fri Mar 22 08:14:42 2024, max compression
```

## Comparing `lbank-connector-python-1.0.8.tar` & `lbank-connector-python-1.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 zhangweijia   (502) staff       (20)        0 2024-03-22 07:43:03.262764 lbank-connector-python-1.0.8/
--rw-r--r--   0 zhangweijia   (502) staff       (20)     1066 2024-02-20 07:45:40.000000 lbank-connector-python-1.0.8/LICENSE.md
--rw-r--r--   0 zhangweijia   (502) staff       (20)      609 2024-03-22 07:43:03.262610 lbank-connector-python-1.0.8/PKG-INFO
--rw-r--r--   0 zhangweijia   (502) staff       (20)        0 2024-01-04 06:51:23.000000 lbank-connector-python-1.0.8/README.md
-drwxr-xr-x   0 zhangweijia   (502) staff       (20)        0 2024-03-22 07:43:03.259063 lbank-connector-python-1.0.8/lbank/
--rw-r--r--   0 zhangweijia   (502) staff       (20)        0 2024-01-04 06:51:23.000000 lbank-connector-python-1.0.8/lbank/__init__.py
--rw-r--r--   0 zhangweijia   (502) staff       (20)       22 2024-03-22 07:42:13.000000 lbank-connector-python-1.0.8/lbank/__version__.py
--rw-r--r--   0 zhangweijia   (502) staff       (20)     5895 2024-03-22 07:41:26.000000 lbank-connector-python-1.0.8/lbank/api.py
--rw-r--r--   0 zhangweijia   (502) staff       (20)     1042 2024-03-21 11:52:02.000000 lbank-connector-python-1.0.8/lbank/error.py
--rw-r--r--   0 zhangweijia   (502) staff       (20)     5464 2024-03-22 07:40:46.000000 lbank-connector-python-1.0.8/lbank/old_api.py
-drwxr-xr-x   0 zhangweijia   (502) staff       (20)        0 2024-03-22 07:43:03.261003 lbank-connector-python-1.0.8/lbank/spot/
--rw-r--r--   0 zhangweijia   (502) staff       (20)      699 2024-02-23 06:39:03.000000 lbank-connector-python-1.0.8/lbank/spot/__init__.py
--rw-r--r--   0 zhangweijia   (502) staff       (20)     2497 2024-02-28 10:15:56.000000 lbank-connector-python-1.0.8/lbank/spot/_account.py
--rw-r--r--   0 zhangweijia   (502) staff       (20)     3771 2024-02-28 10:21:04.000000 lbank-connector-python-1.0.8/lbank/spot/_base_data.py
--rw-r--r--   0 zhangweijia   (502) staff       (20)     1462 2024-02-28 10:21:25.000000 lbank-connector-python-1.0.8/lbank/spot/_market.py
--rw-r--r--   0 zhangweijia   (502) staff       (20)     6569 2024-02-28 10:22:59.000000 lbank-connector-python-1.0.8/lbank/spot/_order.py
--rw-r--r--   0 zhangweijia   (502) staff       (20)     6603 2024-02-28 10:24:37.000000 lbank-connector-python-1.0.8/lbank/spot/_trade.py
--rw-r--r--   0 zhangweijia   (502) staff       (20)     3078 2024-02-28 10:25:44.000000 lbank-connector-python-1.0.8/lbank/spot/_wallet.py
--rw-r--r--   0 zhangweijia   (502) staff       (20)     2637 2024-02-28 10:26:22.000000 lbank-connector-python-1.0.8/lbank/spot/_withdraw.py
--rw-r--r--   0 zhangweijia   (502) staff       (20)     1136 2024-03-22 07:38:22.000000 lbank-connector-python-1.0.8/lbank/utils.py
-drwxr-xr-x   0 zhangweijia   (502) staff       (20)        0 2024-03-22 07:43:03.261681 lbank-connector-python-1.0.8/lbank/websocket/
--rw-r--r--   0 zhangweijia   (502) staff       (20)        0 2024-03-20 09:12:01.000000 lbank-connector-python-1.0.8/lbank/websocket/__init__.py
--rw-r--r--   0 zhangweijia   (502) staff       (20)     3402 2024-03-20 10:12:37.000000 lbank-connector-python-1.0.8/lbank/websocket/base_lbank_socket.py
--rw-r--r--   0 zhangweijia   (502) staff       (20)     1521 2024-03-20 10:12:15.000000 lbank-connector-python-1.0.8/lbank/websocket/websocket_client.py
-drwxr-xr-x   0 zhangweijia   (502) staff       (20)        0 2024-03-22 07:43:03.262416 lbank-connector-python-1.0.8/lbank_connector_python.egg-info/
--rw-r--r--   0 zhangweijia   (502) staff       (20)      609 2024-03-22 07:43:03.000000 lbank-connector-python-1.0.8/lbank_connector_python.egg-info/PKG-INFO
--rw-r--r--   0 zhangweijia   (502) staff       (20)      639 2024-03-22 07:43:03.000000 lbank-connector-python-1.0.8/lbank_connector_python.egg-info/SOURCES.txt
--rw-r--r--   0 zhangweijia   (502) staff       (20)        1 2024-03-22 07:43:03.000000 lbank-connector-python-1.0.8/lbank_connector_python.egg-info/dependency_links.txt
--rw-r--r--   0 zhangweijia   (502) staff       (20)      245 2024-03-22 07:43:03.000000 lbank-connector-python-1.0.8/lbank_connector_python.egg-info/requires.txt
--rw-r--r--   0 zhangweijia   (502) staff       (20)        6 2024-03-22 07:43:03.000000 lbank-connector-python-1.0.8/lbank_connector_python.egg-info/top_level.txt
--rw-r--r--   0 zhangweijia   (502) staff       (20)       38 2024-03-22 07:43:03.262804 lbank-connector-python-1.0.8/setup.cfg
--rw-r--r--   0 zhangweijia   (502) staff       (20)     1396 2024-03-20 09:08:49.000000 lbank-connector-python-1.0.8/setup.py
+drwxr-xr-x   0 zhangweijia   (502) staff       (20)        0 2024-03-22 08:14:42.853413 lbank-connector-python-1.0.9/
+-rw-r--r--   0 zhangweijia   (502) staff       (20)     1066 2024-02-20 07:45:40.000000 lbank-connector-python-1.0.9/LICENSE.md
+-rw-r--r--   0 zhangweijia   (502) staff       (20)     1402 2024-03-22 08:14:42.853269 lbank-connector-python-1.0.9/PKG-INFO
+-rw-r--r--   0 zhangweijia   (502) staff       (20)      791 2024-03-22 08:12:57.000000 lbank-connector-python-1.0.9/README.md
+drwxr-xr-x   0 zhangweijia   (502) staff       (20)        0 2024-03-22 08:14:42.849473 lbank-connector-python-1.0.9/lbank/
+-rw-r--r--   0 zhangweijia   (502) staff       (20)        0 2024-01-04 06:51:23.000000 lbank-connector-python-1.0.9/lbank/__init__.py
+-rw-r--r--   0 zhangweijia   (502) staff       (20)       22 2024-03-22 08:02:58.000000 lbank-connector-python-1.0.9/lbank/__version__.py
+-rw-r--r--   0 zhangweijia   (502) staff       (20)     6002 2024-03-22 08:05:04.000000 lbank-connector-python-1.0.9/lbank/api.py
+-rw-r--r--   0 zhangweijia   (502) staff       (20)     1042 2024-03-21 11:52:02.000000 lbank-connector-python-1.0.9/lbank/error.py
+-rw-r--r--   0 zhangweijia   (502) staff       (20)     5568 2024-03-22 08:02:22.000000 lbank-connector-python-1.0.9/lbank/old_api.py
+drwxr-xr-x   0 zhangweijia   (502) staff       (20)        0 2024-03-22 08:14:42.851759 lbank-connector-python-1.0.9/lbank/spot/
+-rw-r--r--   0 zhangweijia   (502) staff       (20)      699 2024-02-23 06:39:03.000000 lbank-connector-python-1.0.9/lbank/spot/__init__.py
+-rw-r--r--   0 zhangweijia   (502) staff       (20)     2497 2024-02-28 10:15:56.000000 lbank-connector-python-1.0.9/lbank/spot/_account.py
+-rw-r--r--   0 zhangweijia   (502) staff       (20)     3771 2024-02-28 10:21:04.000000 lbank-connector-python-1.0.9/lbank/spot/_base_data.py
+-rw-r--r--   0 zhangweijia   (502) staff       (20)     1462 2024-02-28 10:21:25.000000 lbank-connector-python-1.0.9/lbank/spot/_market.py
+-rw-r--r--   0 zhangweijia   (502) staff       (20)     6569 2024-02-28 10:22:59.000000 lbank-connector-python-1.0.9/lbank/spot/_order.py
+-rw-r--r--   0 zhangweijia   (502) staff       (20)     6603 2024-02-28 10:24:37.000000 lbank-connector-python-1.0.9/lbank/spot/_trade.py
+-rw-r--r--   0 zhangweijia   (502) staff       (20)     3078 2024-02-28 10:25:44.000000 lbank-connector-python-1.0.9/lbank/spot/_wallet.py
+-rw-r--r--   0 zhangweijia   (502) staff       (20)     2637 2024-02-28 10:26:22.000000 lbank-connector-python-1.0.9/lbank/spot/_withdraw.py
+-rw-r--r--   0 zhangweijia   (502) staff       (20)     1012 2024-03-22 08:02:46.000000 lbank-connector-python-1.0.9/lbank/utils.py
+drwxr-xr-x   0 zhangweijia   (502) staff       (20)        0 2024-03-22 08:14:42.852371 lbank-connector-python-1.0.9/lbank/websocket/
+-rw-r--r--   0 zhangweijia   (502) staff       (20)        0 2024-03-20 09:12:01.000000 lbank-connector-python-1.0.9/lbank/websocket/__init__.py
+-rw-r--r--   0 zhangweijia   (502) staff       (20)     3402 2024-03-20 10:12:37.000000 lbank-connector-python-1.0.9/lbank/websocket/base_lbank_socket.py
+-rw-r--r--   0 zhangweijia   (502) staff       (20)     1521 2024-03-20 10:12:15.000000 lbank-connector-python-1.0.9/lbank/websocket/websocket_client.py
+drwxr-xr-x   0 zhangweijia   (502) staff       (20)        0 2024-03-22 08:14:42.853080 lbank-connector-python-1.0.9/lbank_connector_python.egg-info/
+-rw-r--r--   0 zhangweijia   (502) staff       (20)     1402 2024-03-22 08:14:42.000000 lbank-connector-python-1.0.9/lbank_connector_python.egg-info/PKG-INFO
+-rw-r--r--   0 zhangweijia   (502) staff       (20)      639 2024-03-22 08:14:42.000000 lbank-connector-python-1.0.9/lbank_connector_python.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangweijia   (502) staff       (20)        1 2024-03-22 08:14:42.000000 lbank-connector-python-1.0.9/lbank_connector_python.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangweijia   (502) staff       (20)      245 2024-03-22 08:14:42.000000 lbank-connector-python-1.0.9/lbank_connector_python.egg-info/requires.txt
+-rw-r--r--   0 zhangweijia   (502) staff       (20)        6 2024-03-22 08:14:42.000000 lbank-connector-python-1.0.9/lbank_connector_python.egg-info/top_level.txt
+-rw-r--r--   0 zhangweijia   (502) staff       (20)       38 2024-03-22 08:14:42.853453 lbank-connector-python-1.0.9/setup.cfg
+-rw-r--r--   0 zhangweijia   (502) staff       (20)     1396 2024-03-20 09:08:49.000000 lbank-connector-python-1.0.9/setup.py
```

### Comparing `lbank-connector-python-1.0.8/LICENSE.md` & `lbank-connector-python-1.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lbank-connector-python-1.0.8/lbank/api.py` & `lbank-connector-python-1.0.9/lbank/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from lbank import __version__
 from lbank.error import ServerError, CommonError
 from lbank.utils import (
     RSA_STR,
     HMACSHA256_STR,
     ALLOW_METHOD,
+    API_HMACSHA,
     get_timestamp,
     random_str,
     build_md5,
 )
 
 
 class HttpClient:
@@ -31,14 +32,16 @@
         api_secret: str = None,
         private_key: str = None,
         base_url: str = "",
     ):
         sign_method = sign_method.upper()
         if sign_method not in ALLOW_METHOD:
             raise CommonError(f"{sign_method} sign method is not supported!")
+        if sign_method == HMACSHA256_STR:
+            sign_method = API_HMACSHA
         self.api_key = api_key
         self.api_secret = api_secret
         self.base_url = base_url
         self.sign_method = sign_method
         self.private_key = private_key
         self.random_str = None
         self.timestamp = None
@@ -101,15 +104,15 @@
             "Content-Type": "application/json",
             "signature_method": self.sign_method,
             "User-Agent": "lbank-connector-python/" + __version__.__version__,
             "timestamp": self.timestamp,
             "echostr": self.random_str,
         }
 
-    def build_rsasignv2(self, payload: dict) -> bytes:
+    def build_rsasignv2(self, payload: dict) -> str:
         """
         build the sign
         """
         if self.private_key is None:
             raise Exception("private key is empty!")
 
         msg = build_md5(payload)
@@ -117,15 +120,15 @@
             "-----BEGIN RSA PRIVATE KEY-----\n"
             + self.private_key
             + "\n-----END RSA PRIVATE KEY-----"
         )
         pri_key = PKCS1_v1_5.new(RSA.importKey(private_key))
         digest = SHA256.new(msg.encode("utf8"))
         sign = b64encode(pri_key.sign(digest))
-        return sign
+        return sign.decode("utf8")
 
     def build_hmacsha256(self, payload: dict) -> str:
         """
         build the signature of the HmacSHA256
         """
         msg = build_md5(payload)
         api_secret = bytes(self.api_secret, encoding="utf8")
@@ -145,15 +148,15 @@
         payload["api_key"] = self.api_key
         payload["timestamp"] = self.timestamp
         payload["signature_method"] = self.sign_method
         payload["echostr"] = self.random_str
 
         if self.sign_method == RSA_STR:
             payload["sign"] = self.build_rsasignv2(payload)
-        elif self.sign_method == HMACSHA256_STR:
+        elif self.sign_method == API_HMACSHA:
             payload["sign"] = self.build_hmacsha256(payload)
         else:
             raise CommonError(
                 f"{self.sign_method} sign method is not supported!")
         return payload
 
     async def http_request(self, method, path, payload: dict = None, **kwargs):
```

### Comparing `lbank-connector-python-1.0.8/lbank/error.py` & `lbank-connector-python-1.0.9/lbank/error.py`

 * *Files identical despite different names*

### Comparing `lbank-connector-python-1.0.8/lbank/old_api.py` & `lbank-connector-python-1.0.9/lbank/old_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 
 from lbank import __version__
 from lbank.error import ServerError, CommonError
 from lbank.utils import (
     RSA_STR,
     HMACSHA256_STR,
     ALLOW_METHOD,
+    API_HMACSHA,
     get_timestamp,
     random_str,
-    build_md5
+    build_md5,
 )
 
 
 class BlockHttpClient:
 
     def __init__(
         self,
@@ -30,14 +31,16 @@
         api_key: str = None,
         api_secret: str = None,
         base_url: str = "",
     ):
         sign_method = sign_method.upper()
         if sign_method not in ALLOW_METHOD:
             raise CommonError(f"{sign_method} sign method is not supported!")
+        if sign_method == HMACSHA256_STR:
+            sign_method = API_HMACSHA
         self.api_key = api_key
         self.api_secret = api_secret
         self.base_url = base_url
         self.sign_method = sign_method
         self.random_str = None
         self.timestamp = None
         self.session = requests.Session()
@@ -68,15 +71,16 @@
             # 判断请求是否成功
             if response.status_code != 200:
                 raise ServerError(response.status_code, response.reason)
             try:
                 data = response.json()
             except JSONDecodeError:
                 raise CommonError(
-                    f"response is not json format response is {response.text}")
+                    f"response is not json format response is {response.text}"
+                )
             # code = data.get("error_code", 0)
             # if code is None or code != 200:
             #     msg = data.get("msg", "")
             #     raise ClientError(
             #         response.status_code,
             #         code,
             #         msg
@@ -96,15 +100,15 @@
             "Content-Type": "application/json",
             "signature_method": self.sign_method,
             "User-Agent": "lbank-connector-python/" + __version__.__version__,
             "timestamp": self.timestamp,
             "echostr": self.random_str,
         }
 
-    def build_rsasignv2(self, payload: dict) -> bytes:
+    def build_rsasignv2(self, payload: dict) -> str:
         """
         build the sign
         """
         if self.api_secret is None:
             raise Exception("private key is empty!")
 
         msg = build_md5(payload)
@@ -123,16 +127,16 @@
         build the signature of the HmacSHA256
         """
         msg = build_md5(payload)
         api_secret = bytes(self.api_secret, encoding="utf8")
         payload = bytes(msg, encoding="utf8")
         signature = (
             hmac.new(
-                api_secret, payload, digestmod=hashlib.sha256
-            ).hexdigest().lower()
+                api_secret,
+                payload, digestmod=hashlib.sha256).hexdigest().lower()
         )
         return signature
 
     def build_payload(self, payload: dict) -> dict:
         """
         @param payload: request form
         @return:
@@ -140,15 +144,15 @@
         payload["api_key"] = self.api_key
         payload["timestamp"] = self.timestamp
         payload["signature_method"] = self.sign_method
         payload["echostr"] = self.random_str
 
         if self.sign_method == RSA_STR:
             payload["sign"] = self.build_rsasignv2(payload)
-        elif self.sign_method == HMACSHA256_STR:
+        elif self.sign_method == API_HMACSHA:
             payload["sign"] = self.build_hmacsha256(payload)
         else:
             raise CommonError(
                 f"{self.sign_method} sign method is not supported!")
         return payload
 
     def http_request(self, method, path, payload: dict = None, **kwargs):
@@ -170,13 +174,12 @@
         if "signature_method" in payload:
             del payload["signature_method"]
         if "echostr" in payload:
             del payload["echostr"]
         if "timestamp" in payload:
             del payload["timestamp"]
         res = self.request(
-            method=method, path=path, headers=headers, json=payload
-        )
+            method=method, path=path, headers=headers, json=payload)
         return res
 
     def close(self):
         self.session.close()
```

### Comparing `lbank-connector-python-1.0.8/lbank/spot/__init__.py` & `lbank-connector-python-1.0.9/lbank/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `lbank-connector-python-1.0.8/lbank/spot/_account.py` & `lbank-connector-python-1.0.9/lbank/spot/_account.py`

 * *Files identical despite different names*

### Comparing `lbank-connector-python-1.0.8/lbank/spot/_base_data.py` & `lbank-connector-python-1.0.9/lbank/spot/_base_data.py`

 * *Files identical despite different names*

### Comparing `lbank-connector-python-1.0.8/lbank/spot/_market.py` & `lbank-connector-python-1.0.9/lbank/spot/_market.py`

 * *Files identical despite different names*

### Comparing `lbank-connector-python-1.0.8/lbank/spot/_order.py` & `lbank-connector-python-1.0.9/lbank/spot/_order.py`

 * *Files identical despite different names*

### Comparing `lbank-connector-python-1.0.8/lbank/spot/_trade.py` & `lbank-connector-python-1.0.9/lbank/spot/_trade.py`

 * *Files identical despite different names*

### Comparing `lbank-connector-python-1.0.8/lbank/spot/_wallet.py` & `lbank-connector-python-1.0.9/lbank/spot/_wallet.py`

 * *Files identical despite different names*

### Comparing `lbank-connector-python-1.0.8/lbank/spot/_withdraw.py` & `lbank-connector-python-1.0.9/lbank/spot/_withdraw.py`

 * *Files identical despite different names*

### Comparing `lbank-connector-python-1.0.8/lbank/utils.py` & `lbank-connector-python-1.0.9/lbank/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import random
 import string
 import time
 
 
 RSA_STR = "RSA"
 HMACSHA256_STR = "HMACSHA256"
+API_HMACSHA = "HmacSHA256"
 ALLOW_METHOD = [
     RSA_STR,
     HMACSHA256_STR,
 ]
 
 
 def get_timestamp() -> str:
@@ -34,12 +35,10 @@
 
 
 def init_logger(level, log_file: str = None):
     logging.Formatter.converter = time.gmtime  # date time in GMT/UTC
     logging.basicConfig(
         level=level,
         filename=log_file,
-        # format="[%(asctime)s] %(process)d %(thread)d {%(name)s} %(levelname)s [%(module)s:%(lineno)s:%(funcName)s] %("
-        #        "message)s",
         format="[%(asctime)s.%(msecs)03d] UTC %(levelname)s %(name)s: %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
     )
```

### Comparing `lbank-connector-python-1.0.8/lbank/websocket/base_lbank_socket.py` & `lbank-connector-python-1.0.9/lbank/websocket/base_lbank_socket.py`

 * *Files identical despite different names*

### Comparing `lbank-connector-python-1.0.8/lbank/websocket/websocket_client.py` & `lbank-connector-python-1.0.9/lbank/websocket/websocket_client.py`

 * *Files identical despite different names*

### Comparing `lbank-connector-python-1.0.8/lbank_connector_python.egg-info/SOURCES.txt` & `lbank-connector-python-1.0.9/lbank_connector_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lbank-connector-python-1.0.8/setup.py` & `lbank-connector-python-1.0.9/setup.py`

 * *Files identical despite different names*

