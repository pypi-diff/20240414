# Comparing `tmp/dtaas_cli-0.1.2.tar.gz` & `tmp/dtaas_cli-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtaas_cli-0.1.2.tar", max compression
+gzip compressed data, was "dtaas_cli-0.1.3.tar", max compression
```

## Comparing `dtaas_cli-0.1.2.tar` & `dtaas_cli-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0        0 2024-03-24 11:06:51.522935 dtaas_cli-0.1.2/README.md
--rw-r--r--   0        0        0      423 2024-04-10 16:30:28.567515 dtaas_cli-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-31 06:33:13.786621 dtaas_cli-0.1.2/src/__init__.py
--rw-r--r--   0        0        0     1231 2024-03-27 14:51:32.151684 dtaas_cli-0.1.2/src/cmd.py
--rw-r--r--   0        0        0     2888 2024-03-31 07:23:34.069695 dtaas_cli-0.1.2/src/pkg/config.py
--rw-r--r--   0        0        0     3922 2024-04-10 16:19:14.359580 dtaas_cli-0.1.2/src/pkg/users.py
--rw-r--r--   0        0        0     2227 2024-04-10 16:02:20.456118 dtaas_cli-0.1.2/src/pkg/utils.py
--rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 dtaas_cli-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-24 11:06:51.522935 dtaas_cli-0.1.3/README.md
+-rw-r--r--   0        0        0      423 2024-04-13 12:32:19.841573 dtaas_cli-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-31 06:33:13.786621 dtaas_cli-0.1.3/src/__init__.py
+-rw-r--r--   0        0        0     1231 2024-03-27 14:51:32.151684 dtaas_cli-0.1.3/src/cmd.py
+-rw-r--r--   0        0        0     2938 2024-04-13 11:40:13.263651 dtaas_cli-0.1.3/src/pkg/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0        0        0     3309 2024-04-13 12:09:17.233572 dtaas_cli-0.1.3/src/pkg/__pycache__/users.cpython-310.pyc
+-rw-r--r--   0        0        0     2472 2024-04-13 11:40:13.263651 dtaas_cli-0.1.3/src/pkg/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0        0        0     2888 2024-03-31 07:23:34.069695 dtaas_cli-0.1.3/src/pkg/config.py
+-rw-r--r--   0        0        0     4254 2024-04-13 11:51:15.012495 dtaas_cli-0.1.3/src/pkg/users.py
+-rw-r--r--   0        0        0     2319 2024-04-13 11:31:54.941367 dtaas_cli-0.1.3/src/pkg/utils.py
+-rw-r--r--   0        0        0      714 1970-01-01 00:00:00.000000 dtaas_cli-0.1.3/PKG-INFO
```

### Comparing `dtaas_cli-0.1.2/src/cmd.py` & `dtaas_cli-0.1.3/src/cmd.py`

 * *Files identical despite different names*

### Comparing `dtaas_cli-0.1.2/src/pkg/config.py` & `dtaas_cli-0.1.3/src/pkg/config.py`

 * *Files identical despite different names*

### Comparing `dtaas_cli-0.1.2/src/pkg/users.py` & `dtaas_cli-0.1.3/src/pkg/users.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This file has functions that handle the user cli commands"""
 
 import subprocess
+import shutil
 from src.pkg import utils
 
 def getComposeConfig(username, server, path):
     """Makes and returns the config for the user"""
 
     template = {}
     mapping = {
@@ -24,14 +25,19 @@
         config, err = utils.replaceAll(template, mapping)
         utils.checkError(err)
     except Exception as e:
         return e
 
     return config, None
 
+def createUserFiles(users, filePath):
+    """Creates all the users' workspace directories"""
+    for username in users:
+        shutil.copytree(filePath+'/template', filePath+'/'+username, dirs_exist_ok=True)
+
 def addUsersToCompose(users, compose, server, path):
     """Adds all the users config to the compose dictionary"""
     for username in users:
         config, err = getComposeConfig(username, server, path)
         if err is not None:
             return err
         compose['services'][username] = config
@@ -61,15 +67,15 @@
     result = subprocess.run(cmdStr, shell=True, check=False)
     if result.returncode != 0:
         return Exception("failed to stop containers")
     return None
 
 def addUsers(configObj):
     """add cli command handler"""
-
+    print("hi")
     try:
         compose, err = utils.importYaml('compose.users.yml')
         utils.checkError(err)
         userList, err = configObj.getAddUsersList()
         utils.checkError(err)
         server, err= configObj.getServerDNS()
         utils.checkError(err)
@@ -89,14 +95,16 @@
             'users': {
                 'name': 'dtaas-users',
                 'external': True
             }
         }
 
     try:
+        err = createUserFiles(userList, path+'/files')
+        utils.checkError(err)
         err = addUsersToCompose(userList, compose, server, path)
         utils.checkError(err)
         err = utils.exportYaml(compose, 'compose.users.yml')
         utils.checkError(err)
         err = startUserContainers(userList)
         utils.checkError(err)
     except Exception as e:
```

### Comparing `dtaas_cli-0.1.2/src/pkg/utils.py` & `dtaas_cli-0.1.3/src/pkg/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,38 +34,40 @@
     except Exception as err:
         return None, Exception(f"Error while getting toml file: {filename}, " + str(err))
     return config, None
 
 def replaceAll(obj, mapping):
     """This function is used to replace all placeholders with values in a nested object"""
     if isinstance(obj,str):
-
-        for key in mapping:
-            obj = obj.replace(key, mapping[key])
-        return obj, None
+        obj, err = replaceString(obj,mapping)
+        return obj, err
 
     if isinstance(obj,list):
 
         for ind, val in enumerate(obj):
             obj[ind], err = replaceAll(val, mapping)
             if err is not None:
                 return None, err
-
         return obj, None
 
     if isinstance(obj,dict):
 
         for key in obj:
             if not isinstance(key,str):
                 return None, Exception("Config substitution failed: Key is not a string")
-
             obj[key], err = replaceAll(obj[key], mapping)
             if err is not None:
                 return None, err
-
         return obj, None
 
     return None, Exception("Config substition failed: Object format not valid")
 
+def replaceString(obj, mapping):
+    for key in mapping:
+        obj = obj.replace(key, mapping[key])
+    return obj, None
+
+
+
 def checkError(err):
     if err is not None:
         raise err
```

### Comparing `dtaas_cli-0.1.2/PKG-INFO` & `dtaas_cli-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtaas-cli
-Version: 0.1.2
+Version: 0.1.3
 Summary: DTaaS CLI
 License: INTO-CPS-Association
 Author: Astitva Sehgal
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

