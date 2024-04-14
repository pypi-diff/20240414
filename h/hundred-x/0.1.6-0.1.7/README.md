# Comparing `tmp/hundred_x-0.1.6.tar.gz` & `tmp/hundred_x-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hundred_x-0.1.6.tar", max compression
+gzip compressed data, was "hundred_x-0.1.7.tar", max compression
```

## Comparing `hundred_x-0.1.6.tar` & `hundred_x-0.1.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      221 2024-04-01 14:03:52.380935 hundred_x-0.1.6/README.md
--rw-r--r--   0        0        0     4841 2024-04-01 14:03:52.380935 hundred_x-0.1.6/hundred_x/abis/erc20.json
--rw-r--r--   0        0        0    12590 2024-04-01 14:03:52.380935 hundred_x-0.1.6/hundred_x/abis/protocol.json
--rw-r--r--   0        0        0    14232 2024-04-01 14:03:52.380935 hundred_x-0.1.6/hundred_x/client.py
--rw-r--r--   0        0        0      569 2024-04-01 14:03:52.380935 hundred_x-0.1.6/hundred_x/constants.py
--rw-r--r--   0        0        0      896 2024-04-01 14:03:52.380935 hundred_x-0.1.6/hundred_x/eip_712.py
--rw-r--r--   0        0        0      636 2024-04-01 14:03:52.380935 hundred_x-0.1.6/hundred_x/enums.py
--rw-r--r--   0        0        0      834 2024-04-01 14:03:52.380935 hundred_x-0.1.6/hundred_x/utils.py
--rw-r--r--   0        0        0     1069 2024-04-01 14:03:52.380935 hundred_x-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 hundred_x-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      221 2024-04-14 10:28:47.990690 hundred_x-0.1.7/README.md
+-rw-r--r--   0        0        0     4841 2024-04-14 10:28:47.990690 hundred_x-0.1.7/hundred_x/abis/erc20.json
+-rw-r--r--   0        0        0    12590 2024-04-14 10:28:47.990690 hundred_x-0.1.7/hundred_x/abis/protocol.json
+-rw-r--r--   0        0        0    14160 2024-04-14 10:28:47.990690 hundred_x-0.1.7/hundred_x/client.py
+-rw-r--r--   0        0        0     1403 2024-04-14 10:28:47.990690 hundred_x-0.1.7/hundred_x/constants.py
+-rw-r--r--   0        0        0      896 2024-04-14 10:28:47.990690 hundred_x-0.1.7/hundred_x/eip_712.py
+-rw-r--r--   0        0        0      750 2024-04-14 10:28:47.990690 hundred_x-0.1.7/hundred_x/enums.py
+-rw-r--r--   0        0        0      834 2024-04-14 10:28:47.990690 hundred_x-0.1.7/hundred_x/utils.py
+-rw-r--r--   0        0        0     1069 2024-04-14 10:28:47.990690 hundred_x-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 hundred_x-0.1.7/PKG-INFO
```

### Comparing `hundred_x-0.1.6/hundred_x/abis/erc20.json` & `hundred_x-0.1.7/hundred_x/abis/erc20.json`

 * *Files identical despite different names*

### Comparing `hundred_x-0.1.6/hundred_x/abis/protocol.json` & `hundred_x-0.1.7/hundred_x/abis/protocol.json`

 * *Files identical despite different names*

### Comparing `hundred_x-0.1.6/hundred_x/client.py` & `hundred_x-0.1.7/hundred_x/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,58 +9,53 @@
 import eth_account
 import requests
 from eip712_structs import make_domain
 from eth_account.messages import encode_structured_data
 from web3 import Web3
 from web3.exceptions import TransactionNotFound
 
-from hundred_x.constants import CONTRACTS, ENV_TO_BASE_URL, ENV_TO_WEBSOCKET_URL, LOGIN_MESSAGE
+from hundred_x.constants import APIS, CONTRACTS, LOGIN_MESSAGE
 from hundred_x.eip_712 import CancelOrder, CancelOrders, LoginMessage, Order, Withdraw
-from hundred_x.enums import Environment, OrderSide, OrderType, TimeInForce
+from hundred_x.enums import ApiType, Environment, OrderSide, OrderType, TimeInForce
 from hundred_x.utils import from_message_to_payload, get_abi
 
 headers = {
     "Accept": "application/json",
     "Content-Type": "application/json",
 }
 
 
 PROTOCOL_ABI = get_abi("protocol")
 ERC_20_ABI = get_abi("erc20")
 
 
-VERIFYING_CONTRACT = "0x65CbB566D1A6E60107c0c7888761de1AdFa1ccC0"
-CHAIN_ID = 168587773
-
-
 class HundredXClient:
-
     def __init__(
         self,
         env: Environment = Environment.TESTNET,
         private_key: str = None,
         subaccount_id: int = 0,
     ):
         """
         Initialize the client with the given environment.
         """
-        self.domain = make_domain(
-            name="100x",
-            version="0.0.0",
-            chainId=CHAIN_ID,
-            verifyingContract=VERIFYING_CONTRACT,
-        )
         self.env = env
-        self.rest_url = ENV_TO_BASE_URL[env]
-        self.websocket_url = ENV_TO_WEBSOCKET_URL[env]
+        self.rest_url = APIS[env][ApiType.REST]
+        self.websocket_url = APIS[env][ApiType.WEBSOCKET]
         self.wallet = eth_account.Account.from_key(private_key)
         self.public_key = self.wallet.address
         self.subaccount_id = subaccount_id
         self.session_cookie = {}
         self.web3 = Web3(Web3.HTTPProvider("https://sepolia.blast.io"))
+        self.domain = make_domain(
+            name="100x",
+            version="0.0.0",
+            chainId=CONTRACTS[env]["CHAIN_ID"],
+            verifyingContract=CONTRACTS[env]["VERIFYING_CONTRACT"],
+        )
 
     def _current_timestamp(self):
         timestamp_ms = int(time.time() * 1000)
         return timestamp_ms
 
     def generate_and_sign_message(self, message_class, **kwargs):
         """
```

### Comparing `hundred_x-0.1.6/hundred_x/eip_712.py` & `hundred_x-0.1.7/hundred_x/eip_712.py`

 * *Files identical despite different names*

### Comparing `hundred_x-0.1.6/hundred_x/enums.py` & `hundred_x-0.1.7/hundred_x/enums.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 """
 Enmum for the hundred_x package
 """
 
 from enum import Enum
 
 
+class ApiType(Enum):
+    """
+    Enum for the API type.
+    """
+
+    REST = "REST"
+    WEBSOCKET = "WEBSOCKET"
+
+
 class Environment(Enum):
     """
     Enum for the environment of the client.
     """
 
     PROD = "prod"
     TESTNET = "testnet"
-    LOCAL = "local"
+    DEVNET = "local"
 
 
 class OrderType(Enum):
     """
     Enum for the order type.
     """
```

### Comparing `hundred_x-0.1.6/hundred_x/utils.py` & `hundred_x-0.1.7/hundred_x/utils.py`

 * *Files identical despite different names*

### Comparing `hundred_x-0.1.6/pyproject.toml` & `hundred_x-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hundred-x"
-version = "0.1.6"
+version = "0.1.7"
 description = "# hundred_x"
 authors = ["8baller <8ball030@gmail.com>"]
 readme = "README.md"
 packages = [{include = "hundred_x"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `hundred_x-0.1.6/PKG-INFO` & `hundred_x-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hundred-x
-Version: 0.1.6
+Version: 0.1.7
 Summary: # hundred_x
 Author: 8baller
 Author-email: 8ball030@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

