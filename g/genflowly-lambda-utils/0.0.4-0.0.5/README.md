# Comparing `tmp/genflowly-lambda-utils-0.0.4.tar.gz` & `tmp/genflowly_lambda_utils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genflowly-lambda-utils-0.0.4.tar", last modified: Sun Apr  7 14:46:39 2024, max compression
+gzip compressed data, was "genflowly_lambda_utils-0.0.5.tar", last modified: Sun Apr 14 21:15:02 2024, max compression
```

## Comparing `genflowly-lambda-utils-0.0.4.tar` & `genflowly_lambda_utils-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:46:39.905788 genflowly-lambda-utils-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-07 14:46:39.905788 genflowly-lambda-utils-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:46:39.905788 genflowly-lambda-utils-0.0.4/genflowly_lambda_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-07 14:46:39.000000 genflowly-lambda-utils-0.0.4/genflowly_lambda_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-07 14:46:39.000000 genflowly-lambda-utils-0.0.4/genflowly_lambda_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:46:39.000000 genflowly-lambda-utils-0.0.4/genflowly_lambda_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-07 14:46:39.000000 genflowly-lambda-utils-0.0.4/genflowly_lambda_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 14:46:39.000000 genflowly-lambda-utils-0.0.4/genflowly_lambda_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 14:46:39.905788 genflowly-lambda-utils-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:46:39.905788 genflowly-lambda-utils-0.0.4/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/utils/aws_dynamodb_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/utils/aws_s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/utils/aws_secrets_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/utils/aws_sns_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/utils/aws_sqs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/utils/aws_step_functions_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/utils/contants.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/utils/hashing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/utils/jwt_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:15:02.593548 genflowly_lambda_utils-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-14 21:15:02.593548 genflowly_lambda_utils-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:15:02.589547 genflowly_lambda_utils-0.0.5/genflowly_lambda_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-14 21:15:02.000000 genflowly_lambda_utils-0.0.5/genflowly_lambda_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-14 21:15:02.000000 genflowly_lambda_utils-0.0.5/genflowly_lambda_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:15:02.000000 genflowly_lambda_utils-0.0.5/genflowly_lambda_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-14 21:15:02.000000 genflowly_lambda_utils-0.0.5/genflowly_lambda_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 21:15:02.000000 genflowly_lambda_utils-0.0.5/genflowly_lambda_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 21:15:02.593548 genflowly_lambda_utils-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:15:02.589547 genflowly_lambda_utils-0.0.5/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/utils/aws_dynamodb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/utils/aws_s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/utils/aws_secrets_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/utils/aws_sns_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/utils/aws_sqs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/utils/aws_step_functions_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/utils/contants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/utils/hashing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-14 21:14:31.000000 genflowly_lambda_utils-0.0.5/utils/jwt_utils.py
```

### Comparing `genflowly-lambda-utils-0.0.4/PKG-INFO` & `genflowly_lambda_utils-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genflowly-lambda-utils
-Version: 0.0.4
+Version: 0.0.5
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: aiosignal
 Requires-Dist: async-timeout
 Requires-Dist: attrs
 Requires-Dist: bardapi
 Requires-Dist: boto3
```

### Comparing `genflowly-lambda-utils-0.0.4/README.md` & `genflowly_lambda_utils-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `genflowly-lambda-utils-0.0.4/genflowly_lambda_utils.egg-info/PKG-INFO` & `genflowly_lambda_utils-0.0.5/genflowly_lambda_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genflowly-lambda-utils
-Version: 0.0.4
+Version: 0.0.5
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: aiosignal
 Requires-Dist: async-timeout
 Requires-Dist: attrs
 Requires-Dist: bardapi
 Requires-Dist: boto3
```

### Comparing `genflowly-lambda-utils-0.0.4/genflowly_lambda_utils.egg-info/requires.txt` & `genflowly_lambda_utils-0.0.5/genflowly_lambda_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `genflowly-lambda-utils-0.0.4/setup.py` & `genflowly_lambda_utils-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="genflowly-lambda-utils",
-    version="0.0.4",
+    version="0.0.5",
     packages=find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         "aiohttp",
         "aiosignal",
         "async-timeout",
```

### Comparing `genflowly-lambda-utils-0.0.4/utils/aws_dynamodb_utils.py` & `genflowly_lambda_utils-0.0.5/utils/aws_dynamodb_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 
 def save_to_dynamodb(table_name: str, data: dict, aws_region: str = AWS_DEFAULT_REGION) -> dict:
     logger.info("Received data object: %s", data)
     dynamodb = boto3.resource('dynamodb', region_name=aws_region)
     response = {}
     try:
         table = dynamodb.Table(table_name)
-        print("Received item_data : %s", data)
         response = table.put_item(Item=data)  # putItem expects a dict object
         logger.info("Saved data object: %s", str(response))
+        return {"status": 200, "response": response}
     except Exception as e:
         logger.error("Save to DynamoDB failed: %s", e)
-    return response
+        return {"status": 500, "response": e}
 
 
 def read_from_dynamodb(table_name: str, key: dict, aws_region: str = AWS_DEFAULT_REGION) -> dict:
     dynamodb = boto3.resource('dynamodb', region_name=aws_region)
     logger.error(dynamodb)
     try:
         table = dynamodb.Table(table_name)
```

### Comparing `genflowly-lambda-utils-0.0.4/utils/aws_secrets_utils.py` & `genflowly_lambda_utils-0.0.5/utils/aws_secrets_utils.py`

 * *Files identical despite different names*

### Comparing `genflowly-lambda-utils-0.0.4/utils/aws_sns_utils.py` & `genflowly_lambda_utils-0.0.5/utils/aws_sns_utils.py`

 * *Files identical despite different names*

### Comparing `genflowly-lambda-utils-0.0.4/utils/aws_step_functions_utils.py` & `genflowly_lambda_utils-0.0.5/utils/aws_step_functions_utils.py`

 * *Files identical despite different names*

### Comparing `genflowly-lambda-utils-0.0.4/utils/jwt_utils.py` & `genflowly_lambda_utils-0.0.5/utils/jwt_utils.py`

 * *Files identical despite different names*

