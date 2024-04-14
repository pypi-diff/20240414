# Comparing `tmp/hundred_x-0.1.7.tar.gz` & `tmp/hundred_x-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hundred_x-0.1.7.tar", max compression
+gzip compressed data, was "hundred_x-0.1.8.tar", max compression
```

## Comparing `hundred_x-0.1.7.tar` & `hundred_x-0.1.8.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      221 2024-04-14 10:28:47.990690 hundred_x-0.1.7/README.md
--rw-r--r--   0        0        0     4841 2024-04-14 10:28:47.990690 hundred_x-0.1.7/hundred_x/abis/erc20.json
--rw-r--r--   0        0        0    12590 2024-04-14 10:28:47.990690 hundred_x-0.1.7/hundred_x/abis/protocol.json
--rw-r--r--   0        0        0    14160 2024-04-14 10:28:47.990690 hundred_x-0.1.7/hundred_x/client.py
--rw-r--r--   0        0        0     1403 2024-04-14 10:28:47.990690 hundred_x-0.1.7/hundred_x/constants.py
--rw-r--r--   0        0        0      896 2024-04-14 10:28:47.990690 hundred_x-0.1.7/hundred_x/eip_712.py
--rw-r--r--   0        0        0      750 2024-04-14 10:28:47.990690 hundred_x-0.1.7/hundred_x/enums.py
--rw-r--r--   0        0        0      834 2024-04-14 10:28:47.990690 hundred_x-0.1.7/hundred_x/utils.py
--rw-r--r--   0        0        0     1069 2024-04-14 10:28:47.990690 hundred_x-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 hundred_x-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      221 2024-04-14 10:31:31.922080 hundred_x-0.1.8/README.md
+-rw-r--r--   0        0        0     4841 2024-04-14 10:31:31.922080 hundred_x-0.1.8/hundred_x/abis/erc20.json
+-rw-r--r--   0        0        0    12590 2024-04-14 10:31:31.922080 hundred_x-0.1.8/hundred_x/abis/protocol.json
+-rw-r--r--   0        0        0    14160 2024-04-14 10:31:31.922080 hundred_x-0.1.8/hundred_x/client.py
+-rw-r--r--   0        0        0     1403 2024-04-14 10:31:31.922080 hundred_x-0.1.8/hundred_x/constants.py
+-rw-r--r--   0        0        0      896 2024-04-14 10:31:31.922080 hundred_x-0.1.8/hundred_x/eip_712.py
+-rw-r--r--   0        0        0      750 2024-04-14 10:31:31.922080 hundred_x-0.1.8/hundred_x/enums.py
+-rw-r--r--   0        0        0      834 2024-04-14 10:31:31.922080 hundred_x-0.1.8/hundred_x/utils.py
+-rw-r--r--   0        0        0     1076 2024-04-14 10:31:31.922080 hundred_x-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 hundred_x-0.1.8/PKG-INFO
```

### Comparing `hundred_x-0.1.7/hundred_x/abis/erc20.json` & `hundred_x-0.1.8/hundred_x/abis/erc20.json`

 * *Files identical despite different names*

### Comparing `hundred_x-0.1.7/hundred_x/abis/protocol.json` & `hundred_x-0.1.8/hundred_x/abis/protocol.json`

 * *Files identical despite different names*

### Comparing `hundred_x-0.1.7/hundred_x/client.py` & `hundred_x-0.1.8/hundred_x/client.py`

 * *Files identical despite different names*

### Comparing `hundred_x-0.1.7/hundred_x/constants.py` & `hundred_x-0.1.8/hundred_x/constants.py`

 * *Files identical despite different names*

### Comparing `hundred_x-0.1.7/hundred_x/eip_712.py` & `hundred_x-0.1.8/hundred_x/eip_712.py`

 * *Files identical despite different names*

### Comparing `hundred_x-0.1.7/hundred_x/enums.py` & `hundred_x-0.1.8/hundred_x/enums.py`

 * *Files identical despite different names*

### Comparing `hundred_x-0.1.7/hundred_x/utils.py` & `hundred_x-0.1.8/hundred_x/utils.py`

 * *Files identical despite different names*

### Comparing `hundred_x-0.1.7/pyproject.toml` & `hundred_x-0.1.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "hundred-x"
-version = "0.1.7"
+version = "0.1.8"
 description = "# hundred_x"
 authors = ["8baller <8ball030@gmail.com>"]
 readme = "README.md"
 packages = [{include = "hundred_x"}]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.9,<=3.11"
 requests = "^2.31.0"
 eth-account = "^0.11.0"
 eip712-structs = "^1.1.0"
 web3 = "^6.15.1"
 
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `hundred_x-0.1.7/PKG-INFO` & `hundred_x-0.1.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: hundred-x
-Version: 0.1.7
+Version: 0.1.8
 Summary: # hundred_x
 Author: 8baller
 Author-email: 8ball030@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<=3.11
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: eip712-structs (>=1.1.0,<2.0.0)
 Requires-Dist: eth-account (>=0.11.0,<0.12.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: web3 (>=6.15.1,<7.0.0)
 Description-Content-Type: text/markdown
 
 # 100x Python Client
```

