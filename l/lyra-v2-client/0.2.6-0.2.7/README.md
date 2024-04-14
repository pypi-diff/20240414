# Comparing `tmp/lyra_v2_client-0.2.6.tar.gz` & `tmp/lyra_v2_client-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyra_v2_client-0.2.6.tar", max compression
+gzip compressed data, was "lyra_v2_client-0.2.7.tar", max compression
```

## Comparing `lyra_v2_client-0.2.6.tar` & `lyra_v2_client-0.2.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      814 2024-03-19 12:52:12.055076 lyra_v2_client-0.2.6/README.md
--rw-r--r--   0        0        0       74 2024-03-19 12:52:12.059076 lyra_v2_client-0.2.6/lyra/__init__.py
--rw-r--r--   0        0        0     1715 2024-03-19 12:52:12.059076 lyra_v2_client-0.2.6/lyra/analyser.py
--rw-r--r--   0        0        0     6515 2024-03-19 12:52:12.059076 lyra_v2_client-0.2.6/lyra/async_client.py
--rw-r--r--   0        0        0    29083 2024-03-19 12:52:12.059076 lyra_v2_client-0.2.6/lyra/base_client.py
--rw-r--r--   0        0        0    13530 2024-03-19 12:52:12.059076 lyra_v2_client-0.2.6/lyra/cli.py
--rw-r--r--   0        0        0     2806 2024-03-19 12:52:12.059076 lyra_v2_client-0.2.6/lyra/constants.py
--rw-r--r--   0        0        0     1224 2024-03-19 12:52:12.059076 lyra_v2_client-0.2.6/lyra/enums.py
--rw-r--r--   0        0        0      637 2024-03-19 12:52:12.059076 lyra_v2_client-0.2.6/lyra/http_client.py
--rw-r--r--   0        0        0      770 2024-03-19 12:52:12.059076 lyra_v2_client-0.2.6/lyra/lyra.py
--rw-r--r--   0        0        0      762 2024-03-19 12:52:12.059076 lyra_v2_client-0.2.6/lyra/utils.py
--rw-r--r--   0        0        0      645 2024-03-19 12:52:12.059076 lyra_v2_client-0.2.6/lyra/ws_client.py
--rw-r--r--   0        0        0     1208 2024-03-19 12:52:12.063076 lyra_v2_client-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     1491 1970-01-01 00:00:00.000000 lyra_v2_client-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      814 2024-04-14 10:02:57.595758 lyra_v2_client-0.2.7/README.md
+-rw-r--r--   0        0        0       74 2024-04-14 10:02:57.595758 lyra_v2_client-0.2.7/lyra/__init__.py
+-rw-r--r--   0        0        0     1715 2024-04-14 10:02:57.595758 lyra_v2_client-0.2.7/lyra/analyser.py
+-rw-r--r--   0        0        0    10384 2024-04-14 10:02:57.595758 lyra_v2_client-0.2.7/lyra/async_client.py
+-rw-r--r--   0        0        0    29084 2024-04-14 10:02:57.595758 lyra_v2_client-0.2.7/lyra/base_client.py
+-rw-r--r--   0        0        0    13530 2024-04-14 10:02:57.595758 lyra_v2_client-0.2.7/lyra/cli.py
+-rw-r--r--   0        0        0     2806 2024-04-14 10:02:57.595758 lyra_v2_client-0.2.7/lyra/constants.py
+-rw-r--r--   0        0        0     1224 2024-04-14 10:02:57.595758 lyra_v2_client-0.2.7/lyra/enums.py
+-rw-r--r--   0        0        0      637 2024-04-14 10:02:57.595758 lyra_v2_client-0.2.7/lyra/http_client.py
+-rw-r--r--   0        0        0      713 2024-04-14 10:02:57.595758 lyra_v2_client-0.2.7/lyra/lyra.py
+-rw-r--r--   0        0        0      762 2024-04-14 10:02:57.595758 lyra_v2_client-0.2.7/lyra/utils.py
+-rw-r--r--   0        0        0      645 2024-04-14 10:02:57.595758 lyra_v2_client-0.2.7/lyra/ws_client.py
+-rw-r--r--   0        0        0     1481 2024-04-14 10:02:57.599758 lyra_v2_client-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     1590 1970-01-01 00:00:00.000000 lyra_v2_client-0.2.7/PKG-INFO
```

### Comparing `lyra_v2_client-0.2.6/README.md` & `lyra_v2_client-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `lyra_v2_client-0.2.6/lyra/analyser.py` & `lyra_v2_client-0.2.7/lyra/analyser.py`

 * *Files identical despite different names*

### Comparing `lyra_v2_client-0.2.6/lyra/base_client.py` & `lyra_v2_client-0.2.7/lyra/base_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,16 +56,14 @@
         if wallet:
             print(f"Using wallet: {wallet}")
         if not subaccount_id:
             self.subaccount_id = self.fetch_subaccounts()['subaccount_ids'][0]
         else:
             self.subaccount_id = subaccount_id
         print(f"Using subaccount id: {self.subaccount_id}")
-        self.ws = self.connect_ws()
-        self.login_client()
 
     def sign_authentication_header(self):
         timestamp = str(int(time.time() * 1000))
         msg = encode_defunct(
             text=timestamp,
         )
         signature = self.web3_client.eth.account.sign_message(
@@ -74,15 +72,15 @@
         return {
             'wallet': self.wallet,
             'timestamp': str(timestamp),
             'signature': signature,
         }
 
     def connect_ws(self):
-        ws = create_connection(self.contracts['WS_ADDRESS'])
+        ws = create_connection(self.contracts['WS_ADDRESS'], enable_multithread=True, timeout=60)
         return ws
 
     def create_account(self, wallet):
         """Call the create account endpoint."""
         payload = {"wallet": wallet}
         url = f"{self.contracts['BASE_URL']}/public/create_account"
         result = requests.post(
@@ -360,14 +358,15 @@
 
     def cancel_all(self):
         """
         Cancel all orders
         """
         id = str(int(time.time()))
         payload = {"subaccount_id": self.subaccount_id}
+        self.login_client()
         self.ws.send(json.dumps({'method': 'private/cancel_all', 'params': payload, 'id': id}))
         while True:
             message = json.loads(self.ws.recv())
             if message['id'] == id:
                 return message['result']
 
     def get_positions(self):
```

### Comparing `lyra_v2_client-0.2.6/lyra/cli.py` & `lyra_v2_client-0.2.7/lyra/cli.py`

 * *Files identical despite different names*

### Comparing `lyra_v2_client-0.2.6/lyra/constants.py` & `lyra_v2_client-0.2.7/lyra/constants.py`

 * *Files identical despite different names*

### Comparing `lyra_v2_client-0.2.6/lyra/enums.py` & `lyra_v2_client-0.2.7/lyra/enums.py`

 * *Files identical despite different names*

### Comparing `lyra_v2_client-0.2.6/lyra/http_client.py` & `lyra_v2_client-0.2.7/lyra/http_client.py`

 * *Files identical despite different names*

### Comparing `lyra_v2_client-0.2.6/lyra/lyra.py` & `lyra_v2_client-0.2.7/lyra/lyra.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,19 +15,15 @@
 def to_32byte_hex(val):
     return Web3.to_hex(Web3.to_bytes(val).rjust(32, b"\0"))
 
 
 class LyraClient(BaseClient):
     """Client for the lyra dex."""
 
-    http_client: HttpClient
-
     def _create_signature_headers(self):
         """Generate the signature headers."""
-        return self.http_client._create_signature_headers()
+        return HttpClient._create_signature_headers(self)
 
     def __init__(self, *args, **kwargs):
-        self.http_client = HttpClient(
-            *args,
-            **kwargs,
-        )
         super().__init__(*args, **kwargs)
+        self.ws = self.connect_ws()
+        self.login_client()
```

### Comparing `lyra_v2_client-0.2.6/lyra/utils.py` & `lyra_v2_client-0.2.7/lyra/utils.py`

 * *Files identical despite different names*

### Comparing `lyra_v2_client-0.2.6/lyra/ws_client.py` & `lyra_v2_client-0.2.7/lyra/ws_client.py`

 * *Files identical despite different names*

### Comparing `lyra_v2_client-0.2.6/pyproject.toml` & `lyra_v2_client-0.2.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "lyra-v2-client"
-version = "0.2.6"
+version = "0.2.7"
 description = ""
 authors = ["8baller <8ball030@gmail.com>"]
 readme = "README.md"
 packages = [{include = "lyra"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<=3.11.7"
 requests = "^2.31.0"
 web3 = "^5"
 websocket-client = ">=0.32.0,<1"
 setuptools = "^68.2.2"
 rich-click = "^1.7.1"
 python-dotenv = ">=0.14.0,<0.18.0"
 pandas = "~1"
+websockets = "9.1"
+python-socketio = {extras = ["asyncio-client"], version = "^5.11.2"}
 
 
 [tool.poetry.scripts]
 lyra= "lyra.cli:cli"
 
 
 [tool.poetry.group.dev.dependencies]
@@ -26,19 +28,26 @@
 black = "^23.10.1"
 isort = "^5.12.0"
 flake8 = "^6.1.0"
 tbump = "^6.11.0"
 pytest-rerunfailures = "^13.0"
 semver = ">=2.9.1,<3.0.0"
 
+mkdocs = "^1.3.1"
+mkdocs-include-markdown-plugin = "^3.6.1"
+mkdocs-material = "^8.4.0"
+mkdocs-material-extensions = "^1.0.3"
+mkdocs-autorefs = "^0.4.1"
+mkdocstrings-python = "^0.10.0"
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
+
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
 ensure_newline_before_comments = true
 line_length = 120
```

### Comparing `lyra_v2_client-0.2.6/PKG-INFO` & `lyra_v2_client-0.2.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: lyra-v2-client
-Version: 0.2.6
+Version: 0.2.7
 Summary: 
 Author: 8baller
 Author-email: 8ball030@gmail.com
 Requires-Python: >=3.8.1,<=3.11.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=1,<2)
 Requires-Dist: python-dotenv (>=0.14.0,<0.18.0)
+Requires-Dist: python-socketio[asyncio-client] (>=5.11.2,<6.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich-click (>=1.7.1,<2.0.0)
 Requires-Dist: setuptools (>=68.2.2,<69.0.0)
 Requires-Dist: web3 (>=5,<6)
 Requires-Dist: websocket-client (>=0.32.0,<1)
+Requires-Dist: websockets (==9.1)
 Description-Content-Type: text/markdown
 
 # Lyra V2 Python Client.
 
 This repo provides a unified interface for the Lyra V2 Exchange.
 
 Please checkout the [examples](./examples) directory for usage.
```

