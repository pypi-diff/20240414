# Comparing `tmp/genflowly_lambda_utils-0.0.5.tar.gz` & `tmp/genflowly_lambda_utils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genflowly_lambda_utils-0.0.5.tar", last modified: Sun Apr 14 21:15:02 2024, max compression
+gzip compressed data, was "genflowly_lambda_utils-0.0.6.tar", last modified: Sun Apr 14 21:38:25 2024, max compression
```

## Comparing `genflowly_lambda_utils-0.0.5.tar` & `genflowly_lambda_utils-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:15:02.593548 genflowly_lambda_utils-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-14 21:15:02.593548 genflowly_lambda_utils-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:15:02.589547 genflowly_lambda_utils-0.0.5/genflowly_lambda_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-14 21:15:02.000000 genflowly_lambda_utils-0.0.5/genflowly_lambda_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-14 21:15:02.000000 genflowly_lambda_utils-0.0.5/genflowly_lambda_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:15:02.000000 genflowly_lambda_utils-0.0.5/genflowly_lambda_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-14 21:15:02.000000 genflowly_lambda_utils-0.0.5/genflowly_lambda_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 21:15:02.000000 genflowly_lambda_utils-0.0.5/genflowly_lambda_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 21:15:02.593548 genflowly_lambda_utils-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:15:02.589547 genflowly_lambda_utils-0.0.5/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/utils/aws_dynamodb_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/utils/aws_s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/utils/aws_secrets_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/utils/aws_sns_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/utils/aws_sqs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/utils/aws_step_functions_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/utils/contants.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/utils/hashing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/utils/jwt_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:38:25.249218 genflowly_lambda_utils-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-14 21:38:25.249218 genflowly_lambda_utils-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:38:25.249218 genflowly_lambda_utils-0.0.6/genflowly_lambda_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-14 21:38:25.000000 genflowly_lambda_utils-0.0.6/genflowly_lambda_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-14 21:38:25.000000 genflowly_lambda_utils-0.0.6/genflowly_lambda_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:38:25.000000 genflowly_lambda_utils-0.0.6/genflowly_lambda_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-14 21:38:25.000000 genflowly_lambda_utils-0.0.6/genflowly_lambda_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 21:38:25.000000 genflowly_lambda_utils-0.0.6/genflowly_lambda_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 21:38:25.249218 genflowly_lambda_utils-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:38:25.249218 genflowly_lambda_utils-0.0.6/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/utils/aws_dynamodb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/utils/aws_s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/utils/aws_secrets_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/utils/aws_sns_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/utils/aws_sqs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/utils/aws_step_functions_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/utils/contants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/utils/hashing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2705 2024-04-14 21:37:59.000000 genflowly_lambda_utils-0.0.6/utils/jwt_utils.py
```

### Comparing `genflowly_lambda_utils-0.0.5/PKG-INFO` & `genflowly_lambda_utils-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genflowly-lambda-utils
-Version: 0.0.5
+Version: 0.0.6
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: aiosignal
 Requires-Dist: async-timeout
 Requires-Dist: attrs
 Requires-Dist: bardapi
 Requires-Dist: boto3
```

### Comparing `genflowly_lambda_utils-0.0.5/README.md` & `genflowly_lambda_utils-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `genflowly_lambda_utils-0.0.5/genflowly_lambda_utils.egg-info/PKG-INFO` & `genflowly_lambda_utils-0.0.6/genflowly_lambda_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genflowly-lambda-utils
-Version: 0.0.5
+Version: 0.0.6
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: aiosignal
 Requires-Dist: async-timeout
 Requires-Dist: attrs
 Requires-Dist: bardapi
 Requires-Dist: boto3
```

### Comparing `genflowly_lambda_utils-0.0.5/genflowly_lambda_utils.egg-info/requires.txt` & `genflowly_lambda_utils-0.0.6/genflowly_lambda_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `genflowly_lambda_utils-0.0.5/setup.py` & `genflowly_lambda_utils-0.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="genflowly-lambda-utils",
-    version="0.0.5",
+    version="0.0.6",
     packages=find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         "aiohttp",
         "aiosignal",
         "async-timeout",
```

### Comparing `genflowly_lambda_utils-0.0.5/utils/aws_dynamodb_utils.py` & `genflowly_lambda_utils-0.0.6/utils/aws_dynamodb_utils.py`

 * *Files identical despite different names*

### Comparing `genflowly_lambda_utils-0.0.5/utils/aws_secrets_utils.py` & `genflowly_lambda_utils-0.0.6/utils/aws_secrets_utils.py`

 * *Files identical despite different names*

### Comparing `genflowly_lambda_utils-0.0.5/utils/aws_sns_utils.py` & `genflowly_lambda_utils-0.0.6/utils/aws_sns_utils.py`

 * *Files identical despite different names*

### Comparing `genflowly_lambda_utils-0.0.5/utils/aws_step_functions_utils.py` & `genflowly_lambda_utils-0.0.6/utils/aws_step_functions_utils.py`

 * *Files identical despite different names*

### Comparing `genflowly_lambda_utils-0.0.5/utils/jwt_utils.py` & `genflowly_lambda_utils-0.0.6/utils/jwt_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import base64
 import json
 
+import jwt
+
 
 def extract_field_from_jwt(jwt: str, field: str) -> str:
     """
     Extracts a specified field from a JWT
 
     Parameters:
     - jwt (str): The JWT by OAUTH provider to extract the information.
@@ -79,7 +81,22 @@
     Returns:
     - str: The extracted email if available.
 
     Raises:
     - ValueError: If the JWT is invalid or the email is not present.
     """
     return extract_field_from_jwt(jwt, 'email')
+
+
+def create_jwt(payload: dict, secret: str, algorithm: str = 'HS256') -> str:
+    """
+    Creates a JWT from given payload and secret
+
+    Parameters:
+    - payload (dict): The payload to create the JWT
+    - secret (str): The secret to encrypt the payload
+    - algorithm (str): The algorithm to use for the JWT
+
+    Returns:
+    - str: The generated JWT
+    """
+    return jwt.encode(payload, secret, algorithm=algorithm)
```

