# Comparing `tmp/SecLoadSDK-0.0.2.tar.gz` & `tmp/secloadsdk-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SecLoadSDK-0.0.2.tar", last modified: Sun Apr 14 07:39:09 2024, max compression
+gzip compressed data, was "secloadsdk-0.0.3.tar", last modified: Sun Apr 14 19:20:48 2024, max compression
```

## Comparing `SecLoadSDK-0.0.2.tar` & `secloadsdk-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-14 07:39:09.612368 SecLoadSDK-0.0.2/
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      303 2024-04-14 07:39:09.612368 SecLoadSDK-0.0.2/PKG-INFO
-drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-14 07:39:09.612368 SecLoadSDK-0.0.2/SecLoad/
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)     1137 2024-04-11 03:23:37.000000 SecLoadSDK-0.0.2/SecLoad/__init__.py
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)     4829 2024-04-14 07:39:03.000000 SecLoadSDK-0.0.2/SecLoad/apihandlers.py
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      127 2024-04-10 22:20:59.000000 SecLoadSDK-0.0.2/SecLoad/enums.py
-drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-14 07:39:09.612368 SecLoadSDK-0.0.2/SecLoadSDK.egg-info/
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      303 2024-04-14 07:39:09.000000 SecLoadSDK-0.0.2/SecLoadSDK.egg-info/PKG-INFO
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      237 2024-04-14 07:39:09.000000 SecLoadSDK-0.0.2/SecLoadSDK.egg-info/SOURCES.txt
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)        1 2024-04-14 07:39:09.000000 SecLoadSDK-0.0.2/SecLoadSDK.egg-info/dependency_links.txt
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)       30 2024-04-14 07:39:09.000000 SecLoadSDK-0.0.2/SecLoadSDK.egg-info/requires.txt
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)        8 2024-04-14 07:39:09.000000 SecLoadSDK-0.0.2/SecLoadSDK.egg-info/top_level.txt
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)       38 2024-04-14 07:39:09.612368 SecLoadSDK-0.0.2/setup.cfg
--rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      531 2024-04-14 07:38:54.000000 SecLoadSDK-0.0.2/setup.py
+drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-14 19:20:48.314607 secloadsdk-0.0.3/
+-rw-r--r--   0 equsjd    (1000) equsjd    (1000)      299 2024-04-14 19:20:48.314607 secloadsdk-0.0.3/PKG-INFO
+drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-14 19:20:48.310607 secloadsdk-0.0.3/SecLoad/
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)     1137 2024-04-11 03:23:37.000000 secloadsdk-0.0.3/SecLoad/__init__.py
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)     4864 2024-04-14 19:18:22.000000 secloadsdk-0.0.3/SecLoad/apihandlers.py
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      127 2024-04-10 22:20:59.000000 secloadsdk-0.0.3/SecLoad/enums.py
+drwxrwxr-x   0 equsjd    (1000) equsjd    (1000)        0 2024-04-14 19:20:48.314607 secloadsdk-0.0.3/SecLoadSDK.egg-info/
+-rw-r--r--   0 equsjd    (1000) equsjd    (1000)      299 2024-04-14 19:20:48.000000 secloadsdk-0.0.3/SecLoadSDK.egg-info/PKG-INFO
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      237 2024-04-14 19:20:48.000000 secloadsdk-0.0.3/SecLoadSDK.egg-info/SOURCES.txt
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)        1 2024-04-14 19:20:48.000000 secloadsdk-0.0.3/SecLoadSDK.egg-info/dependency_links.txt
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)       30 2024-04-14 19:20:48.000000 secloadsdk-0.0.3/SecLoadSDK.egg-info/requires.txt
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)        8 2024-04-14 19:20:48.000000 secloadsdk-0.0.3/SecLoadSDK.egg-info/top_level.txt
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)       38 2024-04-14 19:20:48.314607 secloadsdk-0.0.3/setup.cfg
+-rw-rw-r--   0 equsjd    (1000) equsjd    (1000)      531 2024-04-14 19:19:42.000000 secloadsdk-0.0.3/setup.py
```

### Comparing `SecLoadSDK-0.0.2/SecLoad/__init__.py` & `secloadsdk-0.0.3/SecLoad/__init__.py`

 * *Files identical despite different names*

### Comparing `SecLoadSDK-0.0.2/SecLoad/apihandlers.py` & `secloadsdk-0.0.3/SecLoad/apihandlers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,117 +1,118 @@
 from .enums import *
 from requests_html import HTMLSession
 import os
+import ast
 
-class SecLoad:
-    def __init__(self, APIKey: str):
-        self.APIKey = APIKey
-        self.URL = "https://secload.scriptlang.com"
+class secload:
+    def __init__(self, apiKey: str):
+        self.apiKey = apiKey
+        self.url = "https://secload.scriptlang.com"
         self.session = HTMLSession()
         
-    def CreateScript(self, script_name: str, source: str, sourcetype: ScriptType):
-        if self.APIKey:
+    def createScript(self, script_name: str, source: str, source_type: ScriptType):
+        if self.apiKey:
             data={
-                "Key": self.APIKey,
+                "Key": self.apiKey,
                 "ScriptName": script_name
             }
-            if sourcetype.value == 1:
+            if source_type.value == 1:
                 data["Source"] = source
             else:
                 if os.path.exists(source):
                     with open(source) as file:
                         data["Source"] = file.read()
                 else:
                     raise Exception(f"File '{source}' does not exist.")
             
-            response = self.session.post(self.URL+"/secload/publicapi/CreateScript", json=data)
+            response = self.session.post(self.url+"/secload/publicapi/CreateScript", json=data)
             if response.status_code == 200:
                 return response.text
             else:
                 raise Exception(f"ERROR {response.status_code} - {response.text}")
         else:
             raise Exception("API Key has not been defined. Create a new API key at https://secload.scriptlang.com/docs")
         
-    def RemoveScript(self, script_name: str):
-        if self.APIKey:
-            response = self.session.post(self.URL+"/secload/publicapi/RemoveScript", json={
-                "Key": self.APIKey,
+    def removeScript(self, script_name: str):
+        if self.apiKey:
+            response = self.session.post(self.url+"/secload/publicapi/RemoveScript", json={
+                "Key": self.apiKey,
                 "ScriptName": script_name,
             })
             
             if response.status_code == 200:
                 return response.text
             else:
                 raise Exception(f"ERROR {response.status_code} - {response.text}")
         else:
             raise Exception("API Key has not been defined. Create a new API key at https://secload.scriptlang.com/docs")
         
-    def OverwriteScript(self, script_name: str, source: str, sourcetype: ScriptType):
-        if self.APIKey:
+    def overwriteScript(self, script_name: str, source: str, source_type: ScriptType):
+        if self.apiKey:
             data={
-                "Key": self.APIKey,
+                "Key": self.apiKey,
                 "ScriptName": script_name
             }
-            if sourcetype.value == 1:
+            if source_type.value == 1:
                 data["Source"] = source
             else:
                 if os.path.exists(source):
                     with open(source) as file:
                         data["Source"] = file.read()
                 else:
                     raise Exception(f"File '{source}' does not exist.")
                 
-            response = self.session.post(self.URL+"/secload/publicapi/OverwriteScript", json=data)
+            response = self.session.post(self.url+"/secload/publicapi/OverwriteScript", json=data)
             if response.status_code == 200:
                 return response.text
             else:
                 raise Exception(f"ERROR {response.status_code} - {response.text}")
         else:
             raise Exception("API Key has not been defined. Create a new API key at https://secload.scriptlang.com/docs")
         
-    def ListScripts(self):
-        if self.APIKey:
-            response = self.session.post(self.URL+"/secload/publicapi/ListScripts", json={
-                "Key": self.APIKey,
+    def listScripts(self):
+        if self.apiKey:
+            response = self.session.post(self.url+"/secload/publicapi/ListScripts", json={
+                "Key": self.apiKey,
             })
             
             if response.status_code == 200:
-                return response.text
+                return ast.literal_eval(response.text)
             else:
                 raise Exception(f"ERROR {response.status_code} - {response.text}")
         else:
             raise Exception("API Key has not been defined. Create a new API key at https://secload.scriptlang.com/docs")
         
-    def GenerateKey(self, script_name: str, username: str="username", time: int=5):
-        if self.APIKey:
-            response = self.session.post(self.URL+"/secload/publicapi/GenerateKey", json={
-                "Key": self.APIKey,
+    def generateKey(self, script_name: str, username: str="username", time: int=5):
+        if self.apiKey:
+            response = self.session.post(self.url+"/secload/publicapi/GenerateKey", json={
+                "Key": self.apiKey,
                 "ScriptName": script_name,
                 "Username": username,
                 "Time": time
             })
             
             if response.status_code == 200:
                 return response.text
             else:
                 raise Exception(f"ERROR {response.status_code} - {response.text}")
         else:
             raise Exception("API Key has not been defined. Create a new API key at https://secload.scriptlang.com/docs")
         
-    def GetScriptSource(self, script_name: str, sourcetype: ScriptType):
-        if self.APIKey:
+    def getScriptSource(self, script_name: str, source_type: ScriptType):
+        if self.apiKey:
             data={
-                "Key": self.APIKey,
+                "Key": self.apiKey,
                 "ScriptName": script_name
             }
-            if sourcetype.value == 1:
+            if source_type.value == 1:
                 data["Type"] = "text"
             else:
                 data["Type"] = "file"
                 
-            response = self.session.post(self.URL+"/secload/publicapi/GetScriptSource", json=data)
+            response = self.session.post(self.url+"/secload/publicapi/GetScriptSource", json=data)
             if response.status_code == 200:
                 return response.text
             else:
                 raise Exception(f"ERROR {response.status_code} - {response.text}")
         else:
             raise Exception("API Key has not been defined. Create a new API key at https://secload.scriptlang.com/docs")
```

### Comparing `SecLoadSDK-0.0.2/setup.py` & `secloadsdk-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2' 
+VERSION = '0.0.3' 
 DESCRIPTION = 'SecLoad SDK package for Roblox Script Builder APIs.'
 
 # Setting up
 setup(
         name="SecLoadSDK", 
         version=VERSION,
         author="equsjd",
```

