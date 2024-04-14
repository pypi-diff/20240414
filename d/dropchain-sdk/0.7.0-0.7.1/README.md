# Comparing `tmp/dropchain-sdk-0.7.0.tar.gz` & `tmp/dropchain-sdk-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dropchain-sdk-0.7.0.tar", last modified: Thu Mar 21 01:45:30 2024, max compression
+gzip compressed data, was "dropchain-sdk-0.7.1.tar", last modified: Sun Apr 14 00:24:49 2024, max compression
```

## Comparing `dropchain-sdk-0.7.0.tar` & `dropchain-sdk-0.7.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 crazink    (501) staff       (20)        0 2024-03-21 01:45:30.951174 dropchain-sdk-0.7.0/
--rw-r--r--   0 crazink    (501) staff       (20)     1069 2023-03-03 02:58:53.000000 dropchain-sdk-0.7.0/LICENSE.md
--rw-r--r--   0 crazink    (501) staff       (20)      935 2024-03-21 01:45:30.950927 dropchain-sdk-0.7.0/PKG-INFO
--rw-r--r--   0 crazink    (501) staff       (20)      436 2023-03-04 00:06:46.000000 dropchain-sdk-0.7.0/README.md
-drwxr-xr-x   0 crazink    (501) staff       (20)        0 2024-03-21 01:45:30.943976 dropchain-sdk-0.7.0/dropchain_sdk/
--rw-r--r--   0 crazink    (501) staff       (20)    32271 2024-03-21 01:42:16.000000 dropchain-sdk-0.7.0/dropchain_sdk/__init__.py
-drwxr-xr-x   0 crazink    (501) staff       (20)        0 2024-03-21 01:45:30.950526 dropchain-sdk-0.7.0/dropchain_sdk.egg-info/
--rw-r--r--   0 crazink    (501) staff       (20)      935 2024-03-21 01:45:30.000000 dropchain-sdk-0.7.0/dropchain_sdk.egg-info/PKG-INFO
--rw-r--r--   0 crazink    (501) staff       (20)      239 2024-03-21 01:45:30.000000 dropchain-sdk-0.7.0/dropchain_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 crazink    (501) staff       (20)        1 2024-03-21 01:45:30.000000 dropchain-sdk-0.7.0/dropchain_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 crazink    (501) staff       (20)        9 2024-03-21 01:45:30.000000 dropchain-sdk-0.7.0/dropchain_sdk.egg-info/requires.txt
--rw-r--r--   0 crazink    (501) staff       (20)       14 2024-03-21 01:45:30.000000 dropchain-sdk-0.7.0/dropchain_sdk.egg-info/top_level.txt
--rw-r--r--   0 crazink    (501) staff       (20)       38 2024-03-21 01:45:30.951259 dropchain-sdk-0.7.0/setup.cfg
--rw-r--r--   0 crazink    (501) staff       (20)      580 2024-03-21 01:44:36.000000 dropchain-sdk-0.7.0/setup.py
+drwxr-xr-x   0 crazink    (501) staff       (20)        0 2024-04-14 00:24:49.814333 dropchain-sdk-0.7.1/
+-rw-r--r--   0 crazink    (501) staff       (20)     1069 2023-03-03 02:58:53.000000 dropchain-sdk-0.7.1/LICENSE.md
+-rw-r--r--   0 crazink    (501) staff       (20)      935 2024-04-14 00:24:49.814162 dropchain-sdk-0.7.1/PKG-INFO
+-rw-r--r--   0 crazink    (501) staff       (20)      436 2023-03-04 00:06:46.000000 dropchain-sdk-0.7.1/README.md
+drwxr-xr-x   0 crazink    (501) staff       (20)        0 2024-04-14 00:24:49.813273 dropchain-sdk-0.7.1/dropchain_sdk/
+-rw-r--r--   0 crazink    (501) staff       (20)    33401 2024-04-14 00:03:00.000000 dropchain-sdk-0.7.1/dropchain_sdk/__init__.py
+drwxr-xr-x   0 crazink    (501) staff       (20)        0 2024-04-14 00:24:49.813943 dropchain-sdk-0.7.1/dropchain_sdk.egg-info/
+-rw-r--r--   0 crazink    (501) staff       (20)      935 2024-04-14 00:24:49.000000 dropchain-sdk-0.7.1/dropchain_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 crazink    (501) staff       (20)      239 2024-04-14 00:24:49.000000 dropchain-sdk-0.7.1/dropchain_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 crazink    (501) staff       (20)        1 2024-04-14 00:24:49.000000 dropchain-sdk-0.7.1/dropchain_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 crazink    (501) staff       (20)        9 2024-04-14 00:24:49.000000 dropchain-sdk-0.7.1/dropchain_sdk.egg-info/requires.txt
+-rw-r--r--   0 crazink    (501) staff       (20)       14 2024-04-14 00:24:49.000000 dropchain-sdk-0.7.1/dropchain_sdk.egg-info/top_level.txt
+-rw-r--r--   0 crazink    (501) staff       (20)       38 2024-04-14 00:24:49.814391 dropchain-sdk-0.7.1/setup.cfg
+-rw-r--r--   0 crazink    (501) staff       (20)      580 2024-04-14 00:24:12.000000 dropchain-sdk-0.7.1/setup.py
```

### Comparing `dropchain-sdk-0.7.0/LICENSE.md` & `dropchain-sdk-0.7.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dropchain-sdk-0.7.0/PKG-INFO` & `dropchain-sdk-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dropchain-sdk
-Version: 0.7.0
+Version: 0.7.1
 Summary: Build robust web3 applications seamlessly using Python with existing frameworks.
 Home-page: https://github.com/cRazink/py_dropchain_sdk
 Author: DropChain Inc
 Author-email: carter@dropchain.network
 License: MIT
 Description: # Python DropChain SDK
```

### Comparing `dropchain-sdk-0.7.0/dropchain_sdk/__init__.py` & `dropchain-sdk-0.7.1/dropchain_sdk/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -764,116 +764,134 @@
         if session1_token is not None:
             payload["session1_token"] = session1_token
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
-    def asset_optin_algorand_mainnet(self, asset1_id, session1_token, user1_uid):
+    def asset_optin_algorand_mainnet(self, asset1_id, session1_token, user1_uid, self_custody_signing_request_bool):
         url = "https://api.dropchain.network/v1/asset_optin_algorand_mainnet"
 
         payload = {
             "app_id": self.app_id,
             "asset1_id": asset1_id,
             "user1_uid": user1_uid
         }
 
         if session1_token is not None:
             payload["session1_token"] = session1_token
 
+        if self_custody_signing_request_bool is not None:
+            payload["self_custody_signing_request_bool"] = self_custody_signing_request_bool
+
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
-    def send_algo_algorand_mainnet(self, asset1_amount_int, receiver1_address, transaction1_note, session1_token, user1_uid): 
+    def send_algo_algorand_mainnet(self, asset1_amount_int, receiver1_address, transaction1_note, session1_token, user1_uid, self_custody_signing_request_bool): 
         url = "https://api.dropchain.network/v1/send_algo_algorand_mainnet"
 
         payload = {
             "app_id": self.app_id,
             "ALGO_amount": asset1_amount_int,
             "receiver1_address": receiver1_address,
             "note": transaction1_note,
             "user1_uid": user1_uid
         }
 
         if session1_token is not None:
             payload["session1_token"] = session1_token
 
+        if self_custody_signing_request_bool is not None:
+            payload["self_custody_signing_request_bool"] = self_custody_signing_request_bool
+
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
-    def send_asset_algorand_mainnet(self, asset1_amount_int, asset1_id, receiver1_address, transaction1_note, session1_token, user1_uid): 
+    def send_asset_algorand_mainnet(self, asset1_amount_int, asset1_id, receiver1_address, transaction1_note, session1_token, user1_uid, self_custody_signing_request_bool): 
         url = "https://api.dropchain.network/v1/send_asset_algorand_mainnet"
 
         payload = {
             "app_id": self.app_id,
             "asset_amount_int": asset1_amount_int,
             "asset1_id": asset1_id,
             "receiver1_address": receiver1_address,
             "note": transaction1_note,
             "user1_uid": user1_uid
         }
 
         if session1_token is not None:
             payload["session1_token"] = session1_token
 
+        if self_custody_signing_request_bool is not None:
+            payload["self_custody_signing_request_bool"] = self_custody_signing_request_bool
+
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
-    def unfreeze_asset_algorand_mainnet(self, asset1_id, receiver_frozen_address, session1_token, user1_uid):
+    def unfreeze_asset_algorand_mainnet(self, asset1_id, receiver_frozen_address, session1_token, user1_uid, self_custody_signing_request_bool):
         url = "https://api.dropchain.network/v1/unfreeze_asset_algorand_mainnet"
 
         payload = {
             "app_id": self.app_id,
             "asset1_id": asset1_id,
             "receiver_frozen_address": receiver_frozen_address,
             "user1_uid": user1_uid
         }
 
         if session1_token is not None:
             payload["session1_token"] = session1_token
 
+        if self_custody_signing_request_bool is not None:
+            payload["self_custody_signing_request_bool"] = self_custody_signing_request_bool
+
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
-    def freeze_asset_algorand_mainnet(self, asset1_id, receiver_frozen_address, session1_token, user1_uid):
+    def freeze_asset_algorand_mainnet(self, asset1_id, receiver_frozen_address, session1_token, user1_uid, self_custody_signing_request_bool):
         url = "https://api.dropchain.network/v1/freeze_asset_algorand_mainnet"
 
         payload = {
             "app_id": self.app_id,
             "asset1_id": asset1_id,
             "receiver_frozen_address": receiver_frozen_address,
             "user1_uid": user1_uid
         }
 
         if session1_token is not None:
             payload["session1_token"] = session1_token
 
+        if self_custody_signing_request_bool is not None:
+            payload["self_custody_signing_request_bool"] = self_custody_signing_request_bool
+
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
-    def asset_mint_algorand_mainnet(self, created_asset_amount_int, created_asset_decimals, created_asset_name, created_asset_unit_name, created_asset_url, session1_token, user1_uid):
+    def asset_mint_algorand_mainnet(self, created_asset_amount_int, created_asset_decimals, created_asset_name, created_asset_unit_name, created_asset_url, session1_token, user1_uid, self_custody_signing_request_bool):
         url = "https://api.dropchain.network/v1/asset_mint_algorand_mainnet"
 
         payload = {
             "app_id": self.app_id,
             "total_nfts_exist": created_asset_amount_int,
             "asset_decimals": created_asset_decimals,
             "nft_asset_name": created_asset_name,
             "nft_unit_name": created_asset_unit_name,
             "created_asset_url": created_asset_url,
             "user1_uid": user1_uid
         }
 
         if session1_token is not None:
             payload["session1_token"] = session1_token
+        
+        if self_custody_signing_request_bool is not None:
+            payload["self_custody_signing_request_bool"] = self_custody_signing_request_bool
 
         response = requests.post(url, json=payload, headers=self.headers, timeout=30)
 
         return response.json()
 
     def grab_user_linked_wallets(self, lookup_uid, session1_token, user1_uid):
         url = "https://api.dropchain.network/v1/grab_user_linked_wallets"
```

### Comparing `dropchain-sdk-0.7.0/dropchain_sdk.egg-info/PKG-INFO` & `dropchain-sdk-0.7.1/dropchain_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dropchain-sdk
-Version: 0.7.0
+Version: 0.7.1
 Summary: Build robust web3 applications seamlessly using Python with existing frameworks.
 Home-page: https://github.com/cRazink/py_dropchain_sdk
 Author: DropChain Inc
 Author-email: carter@dropchain.network
 License: MIT
 Description: # Python DropChain SDK
```

### Comparing `dropchain-sdk-0.7.0/setup.py` & `dropchain-sdk-0.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
   
 with open("README.md", "r") as fh:
     description = fh.read()
   
 setuptools.setup(
     name="dropchain-sdk",
-    version="0.7.0",
+    version="0.7.1",
     author="DropChain Inc",
     author_email="carter@dropchain.network",
     packages=["dropchain_sdk"],
     description="Build robust web3 applications seamlessly using Python with existing frameworks.",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/cRazink/py_dropchain_sdk",
```

