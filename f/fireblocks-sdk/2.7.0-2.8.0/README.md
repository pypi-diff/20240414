# Comparing `tmp/fireblocks_sdk-2.7.0.tar.gz` & `tmp/fireblocks_sdk-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fireblocks_sdk-2.7.0.tar", last modified: Mon Mar 18 07:09:05 2024, max compression
+gzip compressed data, was "fireblocks_sdk-2.8.0.tar", last modified: Sun Apr 14 11:56:05 2024, max compression
```

## Comparing `fireblocks_sdk-2.7.0.tar` & `fireblocks_sdk-2.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 07:09:05.875700 fireblocks_sdk-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-18 07:08:58.000000 fireblocks_sdk-2.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-18 07:09:05.875700 fireblocks_sdk-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-03-18 07:08:58.000000 fireblocks_sdk-2.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 07:09:05.875700 fireblocks_sdk-2.7.0/fireblocks_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-03-18 07:08:58.000000 fireblocks_sdk-2.7.0/fireblocks_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23580 2024-03-18 07:08:58.000000 fireblocks_sdk-2.7.0/fireblocks_sdk/api_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-03-18 07:08:58.000000 fireblocks_sdk-2.7.0/fireblocks_sdk/ncw_sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)   105294 2024-03-18 07:08:58.000000 fireblocks_sdk-2.7.0/fireblocks_sdk/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-18 07:08:58.000000 fireblocks_sdk-2.7.0/fireblocks_sdk/sdk_token_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-03-18 07:08:58.000000 fireblocks_sdk-2.7.0/fireblocks_sdk/tokenization_api_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 07:09:05.875700 fireblocks_sdk-2.7.0/fireblocks_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-18 07:09:05.000000 fireblocks_sdk-2.7.0/fireblocks_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-18 07:09:05.000000 fireblocks_sdk-2.7.0/fireblocks_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 07:09:05.000000 fireblocks_sdk-2.7.0/fireblocks_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-18 07:09:05.000000 fireblocks_sdk-2.7.0/fireblocks_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-18 07:09:05.000000 fireblocks_sdk-2.7.0/fireblocks_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-18 07:09:05.875700 fireblocks_sdk-2.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-18 07:09:02.000000 fireblocks_sdk-2.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:56:05.642354 fireblocks_sdk-2.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-14 11:55:58.000000 fireblocks_sdk-2.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-14 11:56:05.642354 fireblocks_sdk-2.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-14 11:55:58.000000 fireblocks_sdk-2.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:56:05.642354 fireblocks_sdk-2.8.0/fireblocks_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-14 11:55:58.000000 fireblocks_sdk-2.8.0/fireblocks_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23580 2024-04-14 11:55:58.000000 fireblocks_sdk-2.8.0/fireblocks_sdk/api_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-14 11:55:58.000000 fireblocks_sdk-2.8.0/fireblocks_sdk/ncw_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105849 2024-04-14 11:55:58.000000 fireblocks_sdk-2.8.0/fireblocks_sdk/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-14 11:55:58.000000 fireblocks_sdk-2.8.0/fireblocks_sdk/sdk_token_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-04-14 11:55:58.000000 fireblocks_sdk-2.8.0/fireblocks_sdk/tokenization_api_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:56:05.642354 fireblocks_sdk-2.8.0/fireblocks_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-14 11:56:05.000000 fireblocks_sdk-2.8.0/fireblocks_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-14 11:56:05.000000 fireblocks_sdk-2.8.0/fireblocks_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 11:56:05.000000 fireblocks_sdk-2.8.0/fireblocks_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-14 11:56:05.000000 fireblocks_sdk-2.8.0/fireblocks_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-14 11:56:05.000000 fireblocks_sdk-2.8.0/fireblocks_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-14 11:56:05.642354 fireblocks_sdk-2.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-14 11:56:02.000000 fireblocks_sdk-2.8.0/setup.py
```

### Comparing `fireblocks_sdk-2.7.0/LICENSE.txt` & `fireblocks_sdk-2.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fireblocks_sdk-2.7.0/PKG-INFO` & `fireblocks_sdk-2.8.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fireblocks_sdk
-Version: 2.7.0
+Version: 2.8.0
 Summary: Fireblocks python SDK
 Home-page: https://github.com/fireblocks/fireblocks-sdk-py
-Download-URL: https://github.com/fireblocks/fireblocks-sdk-py/archive/v2.7.0.tar.gz
+Download-URL: https://github.com/fireblocks/fireblocks-sdk-py/archive/v2.8.0.tar.gz
 License: MIT
 Keywords: Fireblocks,SDK
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: PyJWT>=2.7.0
+Requires-Dist: PyJWT>=2.8.0
 Requires-Dist: cryptography>=2.7
 Requires-Dist: requests>=2.22.0
 
 Fireblocks python SDK
```

### Comparing `fireblocks_sdk-2.7.0/README.md` & `fireblocks_sdk-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `fireblocks_sdk-2.7.0/fireblocks_sdk/api_types.py` & `fireblocks_sdk-2.8.0/fireblocks_sdk/api_types.py`

 * *Files identical despite different names*

### Comparing `fireblocks_sdk-2.7.0/fireblocks_sdk/ncw_sdk.py` & `fireblocks_sdk-2.8.0/fireblocks_sdk/ncw_sdk.py`

 * *Files identical despite different names*

### Comparing `fireblocks_sdk-2.7.0/fireblocks_sdk/sdk.py` & `fireblocks_sdk-2.8.0/fireblocks_sdk/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1322,14 +1322,31 @@
         """
         body = {
             "name": name,
         }
 
         return self._put_request(f"/v1/vault/accounts/{vault_account_id}", body)
 
+    def register_new_asset(self, blockchainId, address, symbol=None, idempotency_key=None):
+        """Registers new asset
+
+        Args:
+            blockchainId (str): Native asset of blockchain
+            address (str): Asset contract address
+            symbol (str) optional: Asset symbol
+            idempotency_key (str, optional)
+        """
+        body = {
+            "blockchainId": blockchainId,
+            "address": address,
+            "symbol": symbol,
+        }
+
+        return self._post_request("/v1/assets", body, idempotency_key)
+
     def create_vault_asset(self, vault_account_id, asset_id, idempotency_key=None):
         """Creates a new asset within an existing vault account
 
         Args:
             vault_account_id (str): The vault account Id
             asset_id (str): The symbol of the asset to add (e.g BTC, ETH)
             idempotency_key (str, optional)
```

### Comparing `fireblocks_sdk-2.7.0/fireblocks_sdk/sdk_token_provider.py` & `fireblocks_sdk-2.8.0/fireblocks_sdk/sdk_token_provider.py`

 * *Files identical despite different names*

### Comparing `fireblocks_sdk-2.7.0/fireblocks_sdk/tokenization_api_types.py` & `fireblocks_sdk-2.8.0/fireblocks_sdk/tokenization_api_types.py`

 * *Files identical despite different names*

### Comparing `fireblocks_sdk-2.7.0/fireblocks_sdk.egg-info/PKG-INFO` & `fireblocks_sdk-2.8.0/fireblocks_sdk.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fireblocks_sdk
-Version: 2.7.0
+Version: 2.8.0
 Summary: Fireblocks python SDK
 Home-page: https://github.com/fireblocks/fireblocks-sdk-py
-Download-URL: https://github.com/fireblocks/fireblocks-sdk-py/archive/v2.7.0.tar.gz
+Download-URL: https://github.com/fireblocks/fireblocks-sdk-py/archive/v2.8.0.tar.gz
 License: MIT
 Keywords: Fireblocks,SDK
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: PyJWT>=2.7.0
+Requires-Dist: PyJWT>=2.8.0
 Requires-Dist: cryptography>=2.7
 Requires-Dist: requests>=2.22.0
 
 Fireblocks python SDK
```

