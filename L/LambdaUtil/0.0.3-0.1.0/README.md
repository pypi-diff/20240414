# Comparing `tmp/LambdaUtil-0.0.3.tar.gz` & `tmp/LambdaUtil-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LambdaUtil-0.0.3.tar", last modified: Tue Jan 23 19:13:19 2024, max compression
+gzip compressed data, was "LambdaUtil-0.1.0.tar", last modified: Sun Apr 14 03:39:21 2024, max compression
```

## Comparing `LambdaUtil-0.0.3.tar` & `LambdaUtil-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 duket     (1001) duket     (1001)        0 2024-01-23 19:13:19.017918 LambdaUtil-0.0.3/
-drwxrwxr-x   0 duket     (1001) duket     (1001)        0 2024-01-23 19:13:19.017918 LambdaUtil-0.0.3/LambdaUtil.egg-info/
--rw-rw-r--   0 duket     (1001) duket     (1001)      194 2024-01-23 19:13:18.000000 LambdaUtil-0.0.3/LambdaUtil.egg-info/PKG-INFO
--rw-rw-r--   0 duket     (1001) duket     (1001)      581 2024-01-23 19:13:18.000000 LambdaUtil-0.0.3/LambdaUtil.egg-info/SOURCES.txt
--rw-rw-r--   0 duket     (1001) duket     (1001)        1 2024-01-23 19:13:18.000000 LambdaUtil-0.0.3/LambdaUtil.egg-info/dependency_links.txt
--rw-rw-r--   0 duket     (1001) duket     (1001)       54 2024-01-23 19:13:18.000000 LambdaUtil-0.0.3/LambdaUtil.egg-info/entry_points.txt
--rw-rw-r--   0 duket     (1001) duket     (1001)       28 2024-01-23 19:13:18.000000 LambdaUtil-0.0.3/LambdaUtil.egg-info/requires.txt
--rw-rw-r--   0 duket     (1001) duket     (1001)       11 2024-01-23 19:13:18.000000 LambdaUtil-0.0.3/LambdaUtil.egg-info/top_level.txt
--rw-rw-r--   0 duket     (1001) duket     (1001)      194 2024-01-23 19:13:19.017918 LambdaUtil-0.0.3/PKG-INFO
--rw-rw-r--   0 duket     (1001) duket     (1001)        6 2024-01-23 19:00:29.000000 LambdaUtil-0.0.3/README.md
-drwxrwxr-x   0 duket     (1001) duket     (1001)        0 2024-01-23 19:13:19.017918 LambdaUtil-0.0.3/lambdautil/
--rw-rw-r--   0 duket     (1001) duket     (1001)     1895 2024-01-23 19:00:29.000000 LambdaUtil-0.0.3/lambdautil/__init__.py
--rw-rw-r--   0 duket     (1001) duket     (1001)      907 2024-01-23 18:51:22.000000 LambdaUtil-0.0.3/lambdautil/aws_clients.py
--rw-rw-r--   0 duket     (1001) duket     (1001)      322 2024-01-23 18:51:22.000000 LambdaUtil-0.0.3/lambdautil/cfg.py
--rw-rw-r--   0 duket     (1001) duket     (1001)     2711 2024-01-23 19:00:29.000000 LambdaUtil-0.0.3/lambdautil/command.py
-drwxrwxr-x   0 duket     (1001) duket     (1001)        0 2024-01-23 19:13:19.017918 LambdaUtil-0.0.3/lambdautil/config_parser/
--rw-rw-r--   0 duket     (1001) duket     (1001)      149 2024-01-23 18:51:22.000000 LambdaUtil-0.0.3/lambdautil/config_parser/__init__.py
--rw-rw-r--   0 duket     (1001) duket     (1001)     5702 2024-01-23 19:00:29.000000 LambdaUtil-0.0.3/lambdautil/creator.py
--rw-rw-r--   0 duket     (1001) duket     (1001)    18670 2024-01-23 18:51:22.000000 LambdaUtil-0.0.3/lambdautil/deployer.py
-drwxrwxr-x   0 duket     (1001) duket     (1001)        0 2024-01-23 19:13:19.017918 LambdaUtil-0.0.3/lambdautil/parts/
--rw-rw-r--   0 duket     (1001) duket     (1001)        0 2024-01-23 18:51:22.000000 LambdaUtil-0.0.3/lambdautil/parts/__init__.py
-drwxrwxr-x   0 duket     (1001) duket     (1001)        0 2024-01-23 19:13:19.017918 LambdaUtil-0.0.3/lambdautil/parts/service/
--rw-rw-r--   0 duket     (1001) duket     (1001)     2451 2024-01-23 18:51:22.000000 LambdaUtil-0.0.3/lambdautil/parts/service/__init__.py
-drwxrwxr-x   0 duket     (1001) duket     (1001)        0 2024-01-23 19:13:19.017918 LambdaUtil-0.0.3/lambdautil/parts/simple/
--rw-rw-r--   0 duket     (1001) duket     (1001)     1577 2024-01-23 18:51:22.000000 LambdaUtil-0.0.3/lambdautil/parts/simple/__init__.py
--rw-rw-r--   0 duket     (1001) duket     (1001)     9965 2024-01-23 18:51:22.000000 LambdaUtil-0.0.3/lambdautil/stack.py
-drwxrwxr-x   0 duket     (1001) duket     (1001)        0 2024-01-23 19:13:19.017918 LambdaUtil-0.0.3/lambdautil/template/
--rw-rw-r--   0 duket     (1001) duket     (1001)    11752 2024-01-23 18:51:22.000000 LambdaUtil-0.0.3/lambdautil/template/__init__.py
--rw-rw-r--   0 duket     (1001) duket     (1001)      400 2024-01-23 18:51:22.000000 LambdaUtil-0.0.3/lambdautil/utility.py
--rw-rw-r--   0 duket     (1001) duket     (1001)      406 2024-01-23 19:13:19.021918 LambdaUtil-0.0.3/setup.cfg
--rw-rw-r--   0 duket     (1001) duket     (1001)      447 2024-01-23 19:00:29.000000 LambdaUtil-0.0.3/setup.py
+drwxrwxr-x   0 duket     (1001) duket     (1001)        0 2024-04-14 03:39:21.200179 LambdaUtil-0.1.0/
+drwxrwxr-x   0 duket     (1001) duket     (1001)        0 2024-04-14 03:39:21.196179 LambdaUtil-0.1.0/LambdaUtil.egg-info/
+-rw-rw-r--   0 duket     (1001) duket     (1001)      194 2024-04-14 03:39:21.000000 LambdaUtil-0.1.0/LambdaUtil.egg-info/PKG-INFO
+-rw-rw-r--   0 duket     (1001) duket     (1001)      581 2024-04-14 03:39:21.000000 LambdaUtil-0.1.0/LambdaUtil.egg-info/SOURCES.txt
+-rw-rw-r--   0 duket     (1001) duket     (1001)        1 2024-04-14 03:39:21.000000 LambdaUtil-0.1.0/LambdaUtil.egg-info/dependency_links.txt
+-rw-rw-r--   0 duket     (1001) duket     (1001)       54 2024-04-14 03:39:21.000000 LambdaUtil-0.1.0/LambdaUtil.egg-info/entry_points.txt
+-rw-rw-r--   0 duket     (1001) duket     (1001)       28 2024-04-14 03:39:21.000000 LambdaUtil-0.1.0/LambdaUtil.egg-info/requires.txt
+-rw-rw-r--   0 duket     (1001) duket     (1001)       11 2024-04-14 03:39:21.000000 LambdaUtil-0.1.0/LambdaUtil.egg-info/top_level.txt
+-rw-rw-r--   0 duket     (1001) duket     (1001)      194 2024-04-14 03:39:21.200179 LambdaUtil-0.1.0/PKG-INFO
+-rw-rw-r--   0 duket     (1001) duket     (1001)        6 2024-04-14 03:39:12.000000 LambdaUtil-0.1.0/README.md
+drwxrwxr-x   0 duket     (1001) duket     (1001)        0 2024-04-14 03:39:21.196179 LambdaUtil-0.1.0/lambdautil/
+-rw-rw-r--   0 duket     (1001) duket     (1001)     1895 2024-04-14 03:39:12.000000 LambdaUtil-0.1.0/lambdautil/__init__.py
+-rw-rw-r--   0 duket     (1001) duket     (1001)      907 2024-01-23 18:51:22.000000 LambdaUtil-0.1.0/lambdautil/aws_clients.py
+-rw-rw-r--   0 duket     (1001) duket     (1001)      322 2024-01-23 18:51:22.000000 LambdaUtil-0.1.0/lambdautil/cfg.py
+-rw-rw-r--   0 duket     (1001) duket     (1001)     2711 2024-04-14 03:39:12.000000 LambdaUtil-0.1.0/lambdautil/command.py
+drwxrwxr-x   0 duket     (1001) duket     (1001)        0 2024-04-14 03:39:21.196179 LambdaUtil-0.1.0/lambdautil/config_parser/
+-rw-rw-r--   0 duket     (1001) duket     (1001)      149 2024-01-23 18:51:22.000000 LambdaUtil-0.1.0/lambdautil/config_parser/__init__.py
+-rw-rw-r--   0 duket     (1001) duket     (1001)     5660 2024-04-14 03:39:12.000000 LambdaUtil-0.1.0/lambdautil/creator.py
+-rw-rw-r--   0 duket     (1001) duket     (1001)    19385 2024-04-14 03:39:12.000000 LambdaUtil-0.1.0/lambdautil/deployer.py
+drwxrwxr-x   0 duket     (1001) duket     (1001)        0 2024-04-14 03:39:21.196179 LambdaUtil-0.1.0/lambdautil/parts/
+-rw-rw-r--   0 duket     (1001) duket     (1001)        0 2024-01-23 18:51:22.000000 LambdaUtil-0.1.0/lambdautil/parts/__init__.py
+drwxrwxr-x   0 duket     (1001) duket     (1001)        0 2024-04-14 03:39:21.196179 LambdaUtil-0.1.0/lambdautil/parts/service/
+-rw-rw-r--   0 duket     (1001) duket     (1001)     2451 2024-01-23 18:51:22.000000 LambdaUtil-0.1.0/lambdautil/parts/service/__init__.py
+drwxrwxr-x   0 duket     (1001) duket     (1001)        0 2024-04-14 03:39:21.200179 LambdaUtil-0.1.0/lambdautil/parts/simple/
+-rw-rw-r--   0 duket     (1001) duket     (1001)     1577 2024-01-23 18:51:22.000000 LambdaUtil-0.1.0/lambdautil/parts/simple/__init__.py
+-rw-rw-r--   0 duket     (1001) duket     (1001)    10060 2024-04-14 03:39:12.000000 LambdaUtil-0.1.0/lambdautil/stack.py
+drwxrwxr-x   0 duket     (1001) duket     (1001)        0 2024-04-14 03:39:21.200179 LambdaUtil-0.1.0/lambdautil/template/
+-rw-rw-r--   0 duket     (1001) duket     (1001)    12304 2024-04-14 03:39:12.000000 LambdaUtil-0.1.0/lambdautil/template/__init__.py
+-rw-rw-r--   0 duket     (1001) duket     (1001)      400 2024-01-23 18:51:22.000000 LambdaUtil-0.1.0/lambdautil/utility.py
+-rw-rw-r--   0 duket     (1001) duket     (1001)      406 2024-04-14 03:39:21.200179 LambdaUtil-0.1.0/setup.cfg
+-rw-rw-r--   0 duket     (1001) duket     (1001)      447 2024-04-14 03:39:12.000000 LambdaUtil-0.1.0/setup.py
```

### Comparing `LambdaUtil-0.0.3/LambdaUtil.egg-info/SOURCES.txt` & `LambdaUtil-0.1.0/LambdaUtil.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LambdaUtil-0.0.3/lambdautil/__init__.py` & `LambdaUtil-0.1.0/lambdautil/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from datetime import datetime
 
 __title__ = 'lambdatool'
-__version__ = '0.0.3'
+__version__ = '0.1.0'
 __author__ = 'Duke P. Takle'
 __author_email__ = 'duke.takle@gmail.com'
 __license__ = '''MIT License
 
 Copyright (c) 2023 Duke Takle
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `LambdaUtil-0.0.3/lambdautil/aws_clients.py` & `LambdaUtil-0.1.0/lambdautil/aws_clients.py`

 * *Files identical despite different names*

### Comparing `LambdaUtil-0.0.3/lambdautil/command.py` & `LambdaUtil-0.1.0/lambdautil/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 Develop the lambda function as needed then you can deploy it with:
 lambdatool deploy. The lambda has been started in main.py.
 '''
 
 
 @click.group()
-@click.version_option(version='0.0.3')
+@click.version_option(version='0.1.0')
 def cli():
     pass
 
 
 @cli.command()
 @click.option('-n', '--name', help='name of the new lambda skeleton', required=True)
 @click.option('-d', '--directory', help='target directory for new Lambda, defaults to current directory')
```

### Comparing `LambdaUtil-0.0.3/lambdautil/creator.py` & `LambdaUtil-0.1.0/lambdautil/creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import json
 import time
 
 from lambdautil.parts.simple import main_code as simple_main_code
 from lambdautil.parts.simple import requirements_txt as simple_requirements_txt
 from lambdautil.parts.service import main_code as service_main_code
 from lambdautil.parts.service import requirements_txt as service_requirements_txt
-from lambdautil.cfg import LAMBDAUTIL_TMP
 from lambdautil.cfg import LAMBDAUTIL_BUCKET
 from lambdautil.cfg import LAMBDAUTIL_ROLE
 
 DEFAULT_STAGE = 'dev'
 DEFAULT_TIMEOUT = 60
 DEFAULT_MEMORY = 512
 
@@ -81,15 +80,15 @@
                 if self.service:
                     f.write(service_requirements_txt)
                 else:
                     f.write(simple_requirements_txt)
 
             with open(f'{self.directory}/.lambdautil', 'w') as f:
                 msg = {
-                    'tool-version': '0.0.3',
+                    'tool-version': '0.1.0',
                     'init-time': int(time.time())
                 }
                 f.write(json.dumps(msg, indent=2))
 
             logger.info('LambdaCreator successfully created source files.')
 
             if self._create_config():
@@ -143,15 +142,15 @@
                 f.write(f'role = {role_arn}\n\n')
 
                 f.write('[network]\n')
                 f.write('; security_group = ; TODO: ask for security_group\n')
                 f.write('; subnets =        ; TODO: ask for subnets\n\n')
 
                 f.write('[tags]\n')
-                f.write(f'tool = LambdaUtil 0.0.3\n\n')
+                f.write(f'tool = LambdaUtil 0.1.0\n\n')
 
                 f.write('[parameters]\n')
                 f.write('ANSWER = 42')
                 return True
         except Exception as wtf:
             logger.error(wtf, exc_info=self.verbose)
             logger.error('LambdaCreator failed to create config file.')
```

### Comparing `LambdaUtil-0.0.3/lambdautil/deployer.py` & `LambdaUtil-0.1.0/lambdautil/deployer.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from lambdautil.aws_clients import get_api_client
 from lambdautil.template import starter
 from lambdautil.template import lambda_schedule
 from lambdautil.template import trusted_service
 from lambdautil.template import the_api
 from lambdautil.template import the_deployment
 from lambdautil.template import the_outputs
+from lambdautil.template import white_list
 
 from lambdautil.stack import StackUtility 
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 
 TOOL_FILE = '.lambdautil'
@@ -205,14 +206,22 @@
 
     def _read_network_info(self):
         try:
             self._add_vpc_config = False
             subnets = self.config.get('network', {}).get('subnets')
             security_group = self.config.get('network', {}).get('security_group')
 
+            whitelist = self.config.get('network', {}).get('whitelist')
+            if whitelist:
+                self.whitelist = [wrk.strip() for wrk in whitelist.split(',')]
+                logger.info('adding CIDR whitelist to deployment')
+            else:
+                self.whitelist = None
+                logger.debug('not adding CIDR whitelist to deployment')
+
             if subnets is None and security_group is None:
                 return True
             elif None in [subnets, security_group]:
                 logger.error('network section requires both "subnets" and "security_group"')
                 sys.exit(1)
             else:
                 logger.info('adding VPC configuration to deployment')
@@ -300,14 +309,19 @@
                 api_part['Properties']['Body']['paths']['/']['x-amazon-apigateway-any-method']['x-amazon-apigateway-integration']['uri'] = self.uri
                 api_part['Properties']['Body']['paths']['/{proxy+}']['x-amazon-apigateway-any-method']['x-amazon-apigateway-integration']['uri'] = self.uri
 
                 deployment_part = copy.deepcopy(the_deployment)
                 deployment_part['Properties']['Description'] = self.stage
                 deployment_part['Properties']['StageName'] = self.stage
 
+                if self.whitelist:
+                    whitelist_part = copy.deepcopy(white_list)
+                    whitelist_part['Policy']['Statement'][0]['Condition']['IpAddress']['aws:SourceIp'] = self.whitelist
+                    api_part['Properties']['Policy'] = whitelist_part['Policy']
+
                 self.template['Resources']['theAPI'] = api_part
                 self.template['Resources']['theDeployment'] = deployment_part
                 self._trust_service('apigateway.amazonaws.com')
 
             if self._add_vpc_config:
                 self.template['Resources']['LambdaFunction']['Properties']['VpcConfig'] = {}
                 self.template['Resources']['LambdaFunction']['Properties']['VpcConfig']['SecurityGroupIds'] = self.security_group
```

### Comparing `LambdaUtil-0.0.3/lambdautil/parts/service/__init__.py` & `LambdaUtil-0.1.0/lambdautil/parts/service/__init__.py`

 * *Files identical despite different names*

### Comparing `LambdaUtil-0.0.3/lambdautil/parts/simple/__init__.py` & `LambdaUtil-0.1.0/lambdautil/parts/simple/__init__.py`

 * *Files identical despite different names*

### Comparing `LambdaUtil-0.0.3/lambdautil/stack.py` & `LambdaUtil-0.1.0/lambdautil/stack.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 
 complete_states = [
     'CREATE_COMPLETE',
     'UPDATE_COMPLETE',
     'UPDATE_ROLLBACK_COMPLETE'
 ]
 
+successful_states = [
+    'CREATE_COMPLETE',
+    'UPDATE_COMPLETE',
+    'DELETE_COMPLETE'
+]
+
 try:
     POLL_INTERVAL = int(os.environ.get('CSU_POLL_INTERVAL', 30))
 except:
     POLL_INTERVAL = 30
 
 class StackUtility:
     def __init__(self, **kwargs):
@@ -135,15 +141,15 @@
         while True:
             try:
                 response = self.cf_client.describe_stacks(StackName=stack_name)
                 stack = response['Stacks'][0]
                 current_status = stack['StackStatus']
                 logger.info(f'current status of {stack_name}: {current_status}')
                 if current_status.endswith('COMPLETE') or current_status.endswith('FAILED'):
-                    if current_status in complete_states:
+                    if current_status in successful_states:
                         return True
                     else:
                         return False
 
                 time.sleep(POLL_INTERVAL)
             except ClientError as wtf:
                 if str(wtf).find('does not exist') == -1:
```

### Comparing `LambdaUtil-0.0.3/lambdautil/template/__init__.py` & `LambdaUtil-0.1.0/lambdautil/template/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,14 +123,37 @@
         "Principal": {
             "Ref": "trustedService"
         }
     }
 }  # wrk['Properties']['Principal']
 
 '''
+aws:SourceIp is a list of CIDR blocks to let in. Sibling of
+Properties.Body in the_api
+'''
+white_list = {
+    "Policy": {
+        "Version": "2012-10-17",
+        "Statement": [
+            {
+                "Effect": "Allow",
+                "Principal": "*",
+                "Action": "execute-api:Invoke",
+                "Resource": "arn:aws:execute-api:*:*:*",
+                "Condition": {
+                    "IpAddress": {
+                        "aws:SourceIp": []
+                    }
+                }
+            }
+        ]
+    }
+}
+
+'''
 Path: Properties|Body|info|title - value: xxx-title
 Path: Properties|Body|basePath - value: xxx-base-path
 Path: Properties|Body|paths|/|x-amazon-apigateway-any-method|x-amazon-apigateway-integration|uri - value: xxx-uri0
 Path: Properties|Body|paths|/{proxy+}|x-amazon-apigateway-any-method|x-amazon-apigateway-integration|uri - value: xxx-uri1
 '''
 the_api = {
     "Type": "AWS::ApiGateway::RestApi",
```

