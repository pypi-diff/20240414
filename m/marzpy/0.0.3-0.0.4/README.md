# Comparing `tmp/marzpy-0.0.3.tar.gz` & `tmp/marzpy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marzpy-0.0.3.tar", last modified: Thu Apr  4 23:20:32 2024, max compression
+gzip compressed data, was "marzpy-0.0.4.tar", last modified: Sun Apr 14 13:52:45 2024, max compression
```

## Comparing `marzpy-0.0.3.tar` & `marzpy-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:20:32.092160 marzpy-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-04 23:20:28.000000 marzpy-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-04 23:20:32.092160 marzpy-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-04-04 23:20:28.000000 marzpy-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:20:32.088160 marzpy-0.0.3/marzpy/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-04 23:20:28.000000 marzpy-0.0.3/marzpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:20:32.092160 marzpy-0.0.3/marzpy/api/
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-04 23:20:28.000000 marzpy-0.0.3/marzpy/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-04-04 23:20:28.000000 marzpy-0.0.3/marzpy/api/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-04 23:20:28.000000 marzpy-0.0.3/marzpy/api/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-04-04 23:20:28.000000 marzpy-0.0.3/marzpy/api/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-04 23:20:28.000000 marzpy-0.0.3/marzpy/api/send_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-04 23:20:28.000000 marzpy-0.0.3/marzpy/api/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-04 23:20:28.000000 marzpy-0.0.3/marzpy/api/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-04 23:20:28.000000 marzpy-0.0.3/marzpy/api/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-04 23:20:28.000000 marzpy-0.0.3/marzpy/api/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-04 23:20:28.000000 marzpy-0.0.3/marzpy/marzban.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:20:32.092160 marzpy-0.0.3/marzpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-04 23:20:32.000000 marzpy-0.0.3/marzpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-04 23:20:32.000000 marzpy-0.0.3/marzpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:20:32.000000 marzpy-0.0.3/marzpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 23:20:32.000000 marzpy-0.0.3/marzpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 23:20:32.092160 marzpy-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-04 23:20:28.000000 marzpy-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:52:45.113135 marzpy-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 13:52:39.000000 marzpy-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-14 13:52:45.113135 marzpy-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10493 2024-04-14 13:52:39.000000 marzpy-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:52:45.113135 marzpy-0.0.4/marzpy/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-14 13:52:39.000000 marzpy-0.0.4/marzpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:52:45.113135 marzpy-0.0.4/marzpy/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-14 13:52:39.000000 marzpy-0.0.4/marzpy/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-14 13:52:39.000000 marzpy-0.0.4/marzpy/api/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-14 13:52:39.000000 marzpy-0.0.4/marzpy/api/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-14 13:52:39.000000 marzpy-0.0.4/marzpy/api/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-14 13:52:39.000000 marzpy-0.0.4/marzpy/api/send_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-14 13:52:39.000000 marzpy-0.0.4/marzpy/api/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-14 13:52:39.000000 marzpy-0.0.4/marzpy/api/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-14 13:52:39.000000 marzpy-0.0.4/marzpy/api/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-04-14 13:52:39.000000 marzpy-0.0.4/marzpy/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-14 13:52:39.000000 marzpy-0.0.4/marzpy/marzban.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:52:45.113135 marzpy-0.0.4/marzpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-14 13:52:45.000000 marzpy-0.0.4/marzpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-14 13:52:45.000000 marzpy-0.0.4/marzpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 13:52:45.000000 marzpy-0.0.4/marzpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 13:52:45.000000 marzpy-0.0.4/marzpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 13:52:45.113135 marzpy-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-14 13:52:39.000000 marzpy-0.0.4/setup.py
```

### Comparing `marzpy-0.0.3/LICENSE` & `marzpy-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `marzpy-0.0.3/README.md` & `marzpy-0.0.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # marzpy
 A Python library that helps you easily use [Marzban](https://github.com/Gozargah/Marzban)'s API panel
+>[!IMPORTANT]
+>**Status:** Working on new update 🔥
 ## installation
 ```shell
 pip install marzpy
 ```
-requirements : ```requests```
+requirements : ```aiohttp```
 # How To Use
 ```python
 from marzpy import Marzban
+import asyncio
+        
+async def main():
+    panel = Marzban("username","password","https://example.com")
+    token = await await panel.get_token()
+    #await await panel.anyfunction(token)
 
-panel = Marzban("username","password","https://example.com")
-
-mytoken = panel.get_token()
-
-# panel.anyfunction()
+asyncio.run(main())
 
 ```
 # Features
 
 - Admin
     - [get token](#get-token)
     - [get admin](#get-current-admin)
@@ -70,72 +74,72 @@
 ### Get Token
 ```python
 
 from marzpy import Marzban
 
 panel = Marzban("username","password","https://example.com")
 
-mytoken = panel.get_token()
+mytoken = await panel.get_token()
 
 ```
 ### Get Current admin
 ```python
-admin = panel.get_current_admin(token=mytoken)
+admin = await panel.get_current_admin(token=mytoken)
 print(admin) #output: {'username': 'admin', 'is_sudo': True}
 ```
 ### Create Admin
 ```python
 info = {'username':'test','password':'pasword','is_sudo':False}
-rsault = panel.create_admin(token=mytoken,data=info)
+rsault = await panel.create_admin(token=mytoken,data=info)
 print(result) #output: success
 ```
 ### Modify Admin
 ```python
 target_admin = "test"
 info = {'password':'newpassword','is_sudo':False}
-result = panel.change_admin_password(username=target_admin,token=mytoken,data=info)
+result = await panel.change_admin_password(username=target_admin,token=mytoken,data=info)
 print(result) #output: success
 ```
 ### Remove Admin
 ```python
 target_admin = "test"
-result = panel.delete_admin(username=target_admin,token=mytoken)
+result = await panel.delete_admin(username=target_admin,token=mytoken)
 print(result) #output: success
 ```
 ### Get All Admins
 ```python
-result = panel.get_all_admins(token=mytoken)
+result = await panel.get_all_admins(token=mytoken)
 print(result) 
 #output: [{'username': 'test', 'is_sudo': True}, {'username': 'test1', 'is_sudo': False}]
 ```
 ### User Subscription
 ```python
 subscription_url = "https://sub.yourdomain.com/sub/eyJhbGciOiJIUzI8NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiJNbWRDcmFaeSIsImFjY2VzcyI8InN1YnNjcmlwdGlvbiIsImlhdCI1MTY5NDk1NTkxMH0.o75ML5835SPXpVPKXcvEIUxMTwSy-4XGS9NIdWOAmXY"
-result = panel.get_subscription(subscription_url)
+result = await panel.get_subscription(subscription_url)
 print(result) #output: Configs
 ```
 ### User Subscription info
 ```python
 subscription_url =  "https://sub.yourdomain.com/sub/eyJhbGciOiJIUzI8NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiJNbWRDcmFaeSIsImFjY2VzcyI8InN1YnNjcmlwdGlvbiIsImlhdCI1MTY5NDk1NTkxMH0.o75ML5835SPXpVPKXcvEIUxMTwSy-4XGS9NIdWOAmXY"
-result = panel.get_subscription_info(subscription_url)
+result = await panel.get_subscription_info(subscription_url)
 print(result) #output: User information (usage,links,inbounds,....)
 ```
 ### Get System Stats
 ```python
-result = panel.get_system_stats(token=mytoken)
+result = await panel.get_system_stats(token=mytoken)
 print(result) #output: system stats Memory & CPU usage ...
 ```
 ### Get Inbounds
 ```python
-result = panel.get_inbounds(token=mytoken)
+result = await panel.get_inbounds(token=mytoken)
 print(result) #output: list of inbounds
 ```
 ### Get Hosts
 ```python
-result = panel.get_hosts(token=mytoken)
+result = await panel.get_hosts(token=mytoken)
 print(result) #output: list of hosts
 ```
 ### Modify Hosts
 ```python
 hosts = {
   "VMess TCP": [
     {
@@ -147,38 +151,38 @@
       "security": "inbound_default",
       "alpn": "",
       "fingerprint": ""
     }
   ]
 }
 # **Backup first**
-result = panel.modify_hosts(token=mytoken,data=hosts)
+result = await panel.modify_hosts(token=mytoken,data=hosts)
 print(result) #output: hosts
 ```
 ### Get Core Stats
 ```python
-result = panel.get_xray_core(token=mytoken)
+result = await panel.get_xray_core(token=mytoken)
 print(result)
  #output: {'version': '1.8.1', 'started': True, 'logs_websocket': '/api/core/logs'}
 ```
 ### Restart Core
 ```python
-result = panel.restart_xray_core(token=mytoken)
+result = await panel.restart_xray_core(token=mytoken)
 print(result)
  #output: success
 ```
 ### Get Core Config
 ```python
-result = panel.get_xray_config(token=mytoken)
+result = await panel.get_xray_config(token=mytoken)
 print(result) #output: your xray core config
 ```
 ### Modify Core Config
 ```python
 new_config={"your config"}
-result = panel.modify_xray_config(token=mytoken,config=new_config)
+result = await panel.modify_xray_config(token=mytoken,config=new_config)
 print(result) #output: success
 ```
 ### Add User
 ```python
 from marzpy.api.user import User
 
 user = User(
@@ -188,21 +192,21 @@
         "vless": {"id": "35e7e39c-7d5c-1f4b-8b71-508e4f37ff53"},
     },
     inbounds={"vmess": ["VMess TCP"], "vless": ["VLESS TCP REALITY"]},
     expire=0,
     data_limit=0,
     data_limit_reset_strategy="no_reset",
 )
-result = panel.add_user(user=user, token=token) #return new User object
+result = await panel.add_user(user=user, token=token) #return new User object
 
 print(result.username) #-> Mewhrzad, #user.proxies, #user.inbounds, #user.expire, #user.data_limit, #userdata_limit_reset_strategy, #user.status, #user.used_traffic, #user.lifetime_used_traffic, #user.created_at, #user.links, #user.subscription_url, #user.excluded_inbounds
 ```
 ### Get User
 ```python
-result = panel.get_user("Mewhrzad",token=mytoken) #return User object
+result = await panel.get_user("Mewhrzad",token=mytoken) #return User object
 print(result.subscription_url)
 ```
 ### Modify User
 ```python
 new_user = User(
     username="test",
     proxies={
@@ -211,48 +215,48 @@
     },
     inbounds={"vmess": ["VMess TCP"], "vless": ["VLESS TCP REALITY"]},
     expire=0,
     data_limit=0,
     data_limit_reset_strategy="no_reset",
     status="active",
 )
-result = panel.modify_user("Mewhrzad", token=mytoken, user=new_user)
+result = await panel.modify_user("Mewhrzad", token=mytoken, user=new_user)
 print(result.subscription_url) #output: modified user object
 ```
 ### Remove User
 ```python
-result = panel.delete_user("test", token=mytoken)
+result = await panel.delete_user("test", token=mytoken)
 print(result) #output: success
 ```
 ### Reset User Data Usage
 ```python
-result = panel.reset_user_traffic("test", token=mytoken)
+result = await panel.reset_user_traffic("test", token=mytoken)
 print(result) #output: success
 ```
 ### Reset All Users Data Usage
 ```python
-result = panel.reset_all_users_traffic(token=mytoken)
+result = await panel.reset_all_users_traffic(token=mytoken)
 print(result) #output: success
 ```
 ### Get All Users
 ```python
-result = panel.get_all_users(token=mytoken) #return list of users
+result = await panel.get_all_users(token=mytoken) #return list of users
 for user in result:
     print(user.username) 
 ```
 ### Get User Usage
 ```python
-result = panel.get_user_usage("mewhrzad",token=mytoken)
+result = await panel.get_user_usage("mewhrzad",token=mytoken)
 print(result) 
 #output: [{'node_id': None, 'node_name': 'MTN', 'used_traffic': 0}, 
 #{'node_id': 1, 'node_name': 'MCI', 'used_traffic': 0}]
 ```
 ### Get All User Templates
 ```python
-result = panel.get_all_templates(token=mytoken) #return template list object
+result = await panel.get_all_templates(token=mytoken) #return template list object
 for template in result:
     print(template.name)
 ```
 ### Add User Template
 ```python
 from marzpy.api.template import Template
 
@@ -260,42 +264,42 @@
     name="new_template",
     inbounds={"vmess": ["VMESS TCP"], "vless": ["VLESS TCP REALITY"]},
     data_limit=0,
     expire_duration=0,
     username_prefix=None,
     username_suffix=None,
 )
-result = panel.add_template(token=mytoken, template=temp)  # return new Template object
+result = await panel.add_template(token=mytoken, template=temp)  # return new Template object
 print(result.name) #output: new_template
 ```
 ### Get User Template
 ```python
 template_id = 11
-result = panel.get_template_by_id(token=mytoken, id=template_id) # return Template object
+result = await panel.get_template_by_id(token=mytoken, id=template_id) # return Template object
 print(result.name) #output: new_template
 ```
 ### Modify User Template
 ```python
 from marzpy.api.template import Template
 
 temp = Template(
     name="new_template2",
     inbounds={"vmess": ["VMESS TCP"], "vless": ["VLESS TCP REALITY"]},
     data_limit=0,
     expire_duration=0,
     username_prefix=None,
     username_suffix=None,
 )
-result = panel.modify_template_by_id(
+result = await panel.modify_template_by_id(
     id=1, token=mytoken, template=temp)  # return Modified Template object
 print(result.name) #output: new_template2
 ```
 ### Remove User Template
 ```python
-result = panel.delete_template_by_id(id=1, token=mytoken)
+result = await panel.delete_template_by_id(id=1, token=mytoken)
 print(result) #output: success
 ```
 ### Add Node
 ```python
 from marzpy.api.node import Node
 
 my_node = Node(
@@ -306,20 +310,20 @@
     certificate="your_cert",
     id=4,
     xray_version="1.8.1",
     status="connected",
     message="string",
 )
 
-result = panel.add_node(token=mytoken, node=my_node)  # return new Node object
+result = await panel.add_node(token=mytoken, node=my_node)  # return new Node object
 print(result.address)
 ```
 ### Get Node
 ```python
-result = panel.get_node_by_id(id=1, token=mytoken)  # return exist Node object
+result = await panel.get_node_by_id(id=1, token=mytoken)  # return exist Node object
 print(result.address) #output: address of node 1
 ```
 ### Modify Node
 ```python
 from marzpy.api.node import Node
 
 my_node = Node(
@@ -330,34 +334,34 @@
     certificate="your_cert",
     id=4,
     xray_version="1.8.1",
     status="connected",
     message="string",
 )
 
-result = panel.modify_node_by_id(id=1, token=mytoken,node=my_node)  # return modified Node object
+result = await panel.modify_node_by_id(id=1, token=mytoken,node=my_node)  # return modified Node object
 print(result.address) #output:test.example.com
 ```
 ### Remove Node
 ```python
-result = panel.delete_node(id=1, token=mytoken)
+result = await panel.delete_node(id=1, token=mytoken)
 print(result) #output: success
 ```
 ### Get All Nodes
 ```python
-result = panel.get_all_nodes(token=mytoken)  # return List of Node object
+result = await panel.get_all_nodes(token=mytoken)  # return List of Node object
 for node in result:
     print(node.address)
 ```
 ### Reconenct Node
 ```python
-result = panel.reconnect_node(id=1,token=mytoken)
+result = await panel.reconnect_node(id=1,token=mytoken)
 print(result) #output: success
 ```
 ### Get Node Usage
 ```python
-result = panel.get_nodes_usage(token=mytoken)
+result = await panel.get_nodes_usage(token=mytoken)
 for node in result:
     print(node)
 #output:{'node_id': 1, 'node_name': 'N1', 'uplink': 1000000000000, 'downlink': 1000000000000}
 # {'node_id': 2, 'node_name': 'N2', 'uplink': 1000000000000, 'downlink': 1000000000000}
-```
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `marzpy-0.0.3/marzpy/api/admin.py` & `marzpy-0.0.4/marzpy/api/admin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,105 +1,99 @@
 from .send_requests import *
-
+import aiohttp,json
 
 class Admin:
     def __init__(self, username: str, password: str, panel_address: str):
         self.username = username
         self.password = password
         self.panel_address = panel_address
 
-    def get_token(self):
+    async def get_token(self):
         """login for Authorization token
 
         Returns: `~dict`: Authorization token
         """
         try:
-            request_address = f"{self.panel_address}/api/admin/token"
-            payload = {"username": self.username, "password": self.password}
-            response = requests.post(
-                request_address,
-                data=payload,
-                timeout=3000,
-                headers={
-                    "Accept": "application/json",
-                    "Content-Type": "application/x-www-form-urlencoded",
-                },
-            )
-            response.raise_for_status()  # Raise an exception for non-200 status codes
-            result = json.loads(response.content)
-            result["panel_address"] = self.panel_address
-            return result
-        except requests.exceptions.RequestException as ex:
+            async with aiohttp.request(
+                "post",
+                url = f"{self.panel_address}/api/admin/token",
+                data = {"username": self.username, "password": self.password},
+                ) as response :
+                # response.raise_for_status()  # Raise an exception for non-200 status codes
+                result = await response.json()
+                result["panel_address"] = self.panel_address
+                return result
+        except aiohttp.exceptions.RequestException as ex:
             print(f"Request Exception: {ex}")
             return None
         except json.JSONDecodeError as ex:
             print(f"JSON Decode Error: {ex}")
             return None
 
-    def get_current_admin(self, token: dict):
+    async def get_current_admin(self, token: dict):
         """get current admin who has logged in.
 
         Parameters:
             token (``dict``) : Authorization token
 
         Returns:
         `~dict`: {"username": "str" , "is_sudo": true}
         """
-        return send_request(endpoint="admin", token=token, method="get")
+        return await send_request(endpoint="admin", token=token, method="get")
 
-    def create_admin(self, token: dict, data: dict):
+    async def create_admin(self, token: dict, data: dict):
         """add new admin.
 
         Parameters:
             token (``dict``) : Authorization token
             data (``dict``) : information of new admin
 
         Returns:
         `~dict`: username && is_sudo
         """
-        send_request(endpoint="admin", token=token, method="post", data=data)
+        await send_request(endpoint="admin", token=token, method="post", data=data)
         return "success"
 
-    def change_admin_password(self, username: str, token: dict, data: dict):
+    async def change_admin_password(self, username: str, token: dict, data: dict):
         """change exist admins password.
 
         *you cant modify sudo admins password*
 
         Parameters:
             username (``str``) : username of admin
             token (``dict``) : Authorization token
             data (``dict``) : information of new admin
 
         Returns:
         `~dict`: username && is_sudo
         """
-        send_request(
+        await send_request(
             endpoint=f"admin/{username}",
             token=token,
             method="put",
             data=data,
         )
         return "success"
 
-    def delete_admin(self, username: str, token: dict):
+    async def delete_admin(self, username: str, token: dict):
         """delete admin.
 
         Parameters:
             username (``str``) : username of admin
             token (``dict``) : Authorization token
 
         Returns:
         `~str`: success
         """
-        send_request(endpoint=f"admin/{username}", token=token, method="delete")
+        await send_request(endpoint=f"admin/{username}", token=token, method="delete")
         return "success"
 
-    def get_all_admins(self, token: dict):
+    async def get_all_admins(self, token: dict):
         """get all admins.
 
         Parameters:
             token (``dict``) : Authorization token
 
         Returns:
         `~list`: [{username && is_sudo}]
         """
-        return send_request(endpoint=f"admins", token=token, method="get")
+        return await send_request(endpoint=f"admins", token=token, method="get")
```

### Comparing `marzpy-0.0.3/marzpy/api/core.py` & `marzpy-0.0.4/marzpy/api/core.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 from .send_requests import *
 
 
 class Core:
     def __init__(self) -> None:
         pass
 
-    def get_xray_core(self, token: dict):
+    async def get_xray_core(self, token: dict):
         """get xray core.
 
         Parameters:
             token (``dict``): Authorization token
 
         Returns:
             `~dict`: xray core
         """
-        return send_request(endpoint="core", token=token, method="get")
+        return await send_request(endpoint="core", token=token, method="get")
 
-    def restart_xray_core(self, token: dict):
+    async def restart_xray_core(self, token: dict):
         """restart xray core.
 
         Parameters:
             token (``dict``): Authorization token
 
         Returns:
             `~str`: success
         """
-        send_request(endpoint="core/restart", token=token, method="post")
+        await send_request(endpoint="core/restart", token=token, method="post")
         return "success"
 
-    def get_xray_config(self, token: dict):
+    async def get_xray_config(self, token: dict):
         """get xray config.
 
         Parameters:
             token (``dict``): Authorization token
 
         Returns:
             `~dict`: xray config
         """
-        return send_request(endpoint="core/config", token=token, method="get")
+        return await send_request(endpoint="core/config", token=token, method="get")
 
-    def modify_xray_config(self, token: dict, config: json):
+    async def modify_xray_config(self, token: dict, config: json):
         """edit xray config.
 
         Parameters:
             token (``dict``): Authorization token
             config (``json``): json of new config
 
         Returns:
             `~str`: success
         """
-        send_request(endpoint="core/config", token=token, method="put", data=config)
-        return "success"
+        await send_request(endpoint="core/config", token=token, method="put", data=config)
+        return "success"
```

### Comparing `marzpy-0.0.3/marzpy/api/node.py` & `marzpy-0.0.4/marzpy/api/node.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,113 +25,113 @@
         self.message = message
 
 
 class NodeMethods:
     def __init__(self) -> None:
         pass
 
-    def add_node(self, token: dict, node: Node):
+    async def add_node(self, token: dict, node: Node):
         """add new node.
 
         Parameters:
             token (``dict``): Authorization token
 
             node (``api.Node``): node object
 
         Returns:
             `~object`: information of new node
         """
         return Node(
-            **send_request(
+            **await send_request(
                 endpoint="node", token=token, method="post", data=node.__dict__
             )
         )
 
-    def get_node_by_id(self, id: int, token: dict):
+    async def get_node_by_id(self, id: int, token: dict):
         """get exist node from id.
 
         Parameters:
             id (``int``): id of node
 
             token (``dict``): Authorization token
 
         Returns:
             `~object`: information of new node
         """
-        return Node(**send_request(endpoint=f"node/{id}", token=token, method="get"))
+        return Node(**await send_request(endpoint=f"node/{id}", token=token, method="get"))
 
-    def modify_node_by_id(self, id: int, token: dict, node: object):
+    async def modify_node_by_id(self, id: int, token: dict, node: object):
         """edit exist node from id.
 
         Parameters:
             id (``int``): id of node
 
             token (``dict``): Authorization token
 
             node (``api.Node``): node object
 
         Returns:
             `~object`: information of new node
         """
-        request = send_request(
+        request = await send_request(
             endpoint=f"node/{id}", token=token, method="put", data=node.__dict__
         )
         return Node(**request)
 
-    def delete_node(self, id: int, token: dict):
+    async def delete_node(self, id: int, token: dict):
         """delete node from id.
 
         Parameters:
             id (``int``): id of node
 
             token (``dict``): Authorization token
 
         Returns:
             `~str`: success
         """
-        send_request(endpoint=f"node/{id}", token=token, method="delete")
+        await send_request(endpoint=f"node/{id}", token=token, method="delete")
         return "success"
 
-    def get_all_nodes(self, token: dict):
+    async def get_all_nodes(self, token: dict):
         """get all nodes.
 
         Parameters:
             token (``dict``): Authorization token
 
         Returns:
             `~list of objects`: [Node]
         """
-        request = send_request(endpoint="nodes", token=token, method="get")
+        request = await send_request(endpoint="nodes", token=token, method="get")
         node_list = [Node()]
         for node in request:
             node_list.append(Node(**node))
         del node_list[0]
         return node_list
 
-    def reconnect_node(self, id: int, token: dict):
+    async def reconnect_node(self, id: int, token: dict):
         """reconnect from id.
 
         Parameters:
             id (``int``): id of node
 
             token (``dict``): Authorization token
 
         Returns:
             `~str`: success
         """
-        request = send_request(
+        request = await send_request(
             endpoint=f"node/{id}/reconnect", token=token, method="post"
         )
 
         return "success"
 
-    def get_nodes_usage(self, token: dict):
+    async def get_nodes_usage(self, token: dict):
         """get all nodes usage.
 
         Parameters:
             token (``dict``): Authorization token
 
         Returns:
             `~dict`: "usage" : []
         """
-        request = send_request(endpoint="nodes/usage", token=token, method="get")
-        return request["usages"]
+        request = await send_request(endpoint="nodes/usage", token=token, method="get")
+        return request["usages"]
```

### Comparing `marzpy-0.0.3/marzpy/api/subscription.py` & `marzpy-0.0.4/marzpy/api/subscription.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-import requests, json, base64
+import aiohttp, json, base64
 
 
 class Subscription:
     def __init__(self) -> None:
         pass
 
-    def subsend_request(sub_link: str, endpoint: str):
+    async def subsend_request(sub_link: str, endpoint: str):
         try:
-            request_address = f"{sub_link}/{endpoint}"
-            headers = {
-                "Accept": "application/json",
-            }
-            response = requests.request("get", request_address, headers=headers)
-            response.raise_for_status()  # Raise an exception for non-200 status codes
-            result = response.content
+            async with aiohttp.request(
+                method="get",
+                url = f"{sub_link}/{endpoint}",
+                headers={"Accept": "application/json"}
+                ) as response :
+                await response.raise_for_status()  # Raise an exception for non-200 status codes
+                result = await response.content
             if endpoint:
-                return json.loads(response.content)
+                return await response.json
             else:
                 return base64.b64decode(result).decode("utf-8")
-        except requests.exceptions.RequestException as ex:
+        except aiohttp.exceptions.RequestException as ex:
             print(f"Request Exception: {ex}")
             return None
 
-    def get_subscription(self, sub_link: str):
+    async def get_subscription(self, sub_link: str):
         """Unknow usage!"""
-        return Subscription.subsend_request(sub_link, "")
+        return await Subscription.subsend_request(sub_link, "")
 
-    def get_subscription_info(self, sub_link: str):
+    async def get_subscription_info(self, sub_link: str):
         """get user information.
 
         Parameters:
             token (``dict``): subscription token
 
         Returns:
             `~dict`: information of user
         """
-        return Subscription.subsend_request(sub_link, "info")
+        return await Subscription.subsend_request(sub_link, "info")
```

### Comparing `marzpy-0.0.3/marzpy/api/system.py` & `marzpy-0.0.4/marzpy/api/system.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 from .send_requests import send_request
 
 
 class System:
     def __init__(self) -> None:
         pass
 
-    def get_system_stats(self, token: dict):
+    async def get_system_stats(self, token: dict):
         """get server stats.
 
         Parameters:
             token (``dict``): Authorization token
 
         Returns:
             `~dict`: server stats
         """
-        return send_request(endpoint="system", token=token, method="get")
+        return await send_request(endpoint="system", token=token, method="get")
 
-    def get_inbounds(self, token: dict):
+    async def get_inbounds(self, token: dict):
         """get server inbounds.
 
         Parameters:
             token (``dict``): Authorization token
 
         Returns:
             `~dict`: server inbounds
         """
-        return send_request(endpoint="inbounds", token=token, method="get")
+        return await send_request(endpoint="inbounds", token=token, method="get")
 
-    def get_hosts(self, token: dict):
+    async def get_hosts(self, token: dict):
         """get server hosts.
 
         Parameters:
             token (``dict``): Authorization token
 
         Returns:
             `~dict`: server hosts
         """
-        return send_request(endpoint="hosts", token=token, method="get")
+        return await send_request(endpoint="hosts", token=token, method="get")
 
-    def modify_hosts(self, token: dict, data: dict):
+    async def modify_hosts(self, token: dict, data: dict):
         """get server hosts.
 
         Parameters:
             token (``dict``): Authorization token
             data (``dict``) : new hosts data
         Returns:
             `~dict`: server hosts
         """
-        return send_request(endpoint="hosts", token=token, method="put", data=data)
+        return await send_request(endpoint="hosts", token=token, method="put", data=data)
```

### Comparing `marzpy-0.0.3/marzpy/api/template.py` & `marzpy-0.0.4/marzpy/api/template.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,82 +18,82 @@
         self.expire_duration = expire_duration
         self.username_prefix = username_prefix
         self.username_suffix = username_suffix
         self.id = id
 
 
 class TemplateMethods:
-    def get_all_templates(self, token: dict):
+    async def get_all_templates(self, token: dict):
         """get all templates list.
 
         Parameters:
             token (``dict``) : Authorization token
 
         Returns:
             `~list`: list of templates
         """
-        request = send_request(endpoint="user_template", token=token, method="get")
+        request = await send_request(endpoint="user_template", token=token, method="get")
         template_list = [Template()]
         for user in request:
             template_list.append(Template(**user))
         del template_list[0]
         return template_list
 
-    def add_template(self, template: Template, token: dict):
+    async def add_template(self, template: Template, token: dict):
         """add new template.
 
         Parameters:
             token (``dict``) : Authorization token
             template (``api.template object``) : template
 
         Returns:
             `~object`: information of new template
         """
-        request = send_request(
+        request = await send_request(
             endpoint="user_template", token=token, method="post", data=template.__dict__
         )
         return Template(**request)
 
-    def get_template_by_id(self, id: int, token: dict):
+    async def get_template_by_id(self, id: int, token: dict):
         """get exist template from id.
 
         Parameters:
             id (``id``) : template id
             token (``dict``) : Authorization token
         Returns:
             `~object`: information of template
         """
-        request = send_request(
+        request = await send_request(
             endpoint=f"user_template/{id}", token=token, method="get"
         )
 
         return Template(**request)
 
-    def modify_template_by_id(self, id: int, token: dict, template: Template):
+    async def modify_template_by_id(self, id: int, token: dict, template: Template):
         """edit exist template from id.
 
         Parameters:
             id (``id``) : template id
             token (``dict``) : Authorization token
             template (``object``) template
         Returns:
             `~object`: information of edited template
         """
-        request = send_request(
+        request = await send_request(
             endpoint=f"user_template/{id}",
             token=token,
             method="put",
             data=template.__dict__,
         )
         return Template(**request)
 
-    def delete_template_by_id(self, id: int, token: dict):
+    async def delete_template_by_id(self, id: int, token: dict):
         """delete template from id.
 
         Parameters:
             id (``id``) : template id
             token (``dict``) : Authorization token
         Returns:
             `~str`: success
         """
-        send_request(endpoint=f"user_template/{id}", token=token, method="delete")
-        return "success"
+        await send_request(endpoint=f"user_template/{id}", token=token, method="delete")
+        return "success"
```

### Comparing `marzpy-0.0.3/marzpy/api/user.py` & `marzpy-0.0.4/marzpy/api/user.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .send_requests import *
 
-def delete_if_exist(dic,keys:list):
+async def delete_if_exist(dic,keys:list):
     for key in keys:
         if key in dic:
             del dic[key]
     return dic
+
 class User:
     def __init__(
         self,
         username: str,
         proxies: dict,
         inbounds: dict,  
         data_limit: float,
@@ -44,100 +45,100 @@
         self.note = note
         self.on_hold_timeout = on_hold_timeout
         self.on_hold_expire_duration = on_hold_expire_duration
         self.sub_last_user_agent = sub_last_user_agent
         self.online_at = online_at
         self.sub_updated_at = sub_updated_at
 class UserMethods:
-    def add_user(self, user: User, token: dict):
+    async def add_user(self, user: User, token: dict):
         """add new user.
 
         Parameters:
             user (``api.User``) : User Object
 
             token (``dict``) : Authorization token
 
         Returns: `~User`: api.User object
         """
         user.status = "active"
         if user.on_hold_expire_duration:
             user.status = "on_hold"
-        request = send_request(
+        request = await send_request(
             endpoint="user", token=token, method="post", data=user.__dict__
         )
         return User(**request)
 
-    def get_user(self, user_username: str, token: dict):
+    async def get_user(self, user_username: str, token: dict):
         """get exist user information by username.
 
         Parameters:
             user_username (``str``) : username of user
 
             token (``dict``) : Authorization token
 
         Returns: `~User`: api.User object
         """
-        request = send_request(f"user/{user_username}", token=token, method="get")
+        request = await send_request(f"user/{user_username}", token=token, method="get")
         return User(**request)
 
-    def modify_user(self, user_username: str, token: dict, user: object):
+    async def modify_user(self, user_username: str, token: dict, user: object):
         """edit exist user by username.
 
         Parameters:
             user_username (``str``) : username of user
 
             token (``dict``) : Authorization token
 
             user (``api.User``) : User Object
 
         Returns: `~User`: api.User object
         """
-        request = send_request(f"user/{user_username}", token, "put", user.__dict__)
+        request = await send_request(f"user/{user_username}", token, "put", user.__dict__)
         return User(**request)
 
-    def delete_user(self, user_username: str, token: dict):
+    async def delete_user(self, user_username: str, token: dict):
         """delete exist user by username.
 
         Parameters:
             user_username (``str``) : username of user
 
             token (``dict``) : Authorization token
 
         Returns: `~str`: success
         """
-        send_request(f"user/{user_username}", token, "delete")
+        await send_request(f"user/{user_username}", token, "delete")
         return "success"
 
-    def reset_user_traffic(self, user_username: str, token: dict):
+    async def reset_user_traffic(self, user_username: str, token: dict):
         """reset exist user traffic by username.
 
         Parameters:
             user_username (``str``) : username of user
 
             token (``dict``) : Authorization token
 
         Returns: `~str`: success
         """
-        send_request(f"user/{user_username}/reset", token, "post")
+        await send_request(f"user/{user_username}/reset", token, "post")
         return "success"
     
-    def revoke_sub(self, user_username: str, token: dict):
+    async def revoke_sub(self, user_username: str, token: dict):
         """Revoke users subscription (Subscription link and proxies) traffic by username.
 
         Parameters:
             user_username (``str``) : username of user
 
             token (``dict``) : Authorization token
 
         Returns: `~str`: success
         """
-        request = send_request(f"user/{user_username}/revoke_sub", token, "post")
+        request = await send_request(f"user/{user_username}/revoke_sub", token, "post")
         return User(**request)
     
-    def get_all_users(self, token: dict, username=None, status=None):
+    async def get_all_users(self, token: dict, username=None, status=None):
         """get all users list.
 
         Parameters:
             token (``dict``) : Authorization token
 
         Returns:
             `~list`: list of users
@@ -146,15 +147,15 @@
         if username:
             endpoint += f"?username={username}"
         if status:
             if "?" in endpoint:
                 endpoint += f"&status={status}"
             else:
                 endpoint += f"?status={status}"
-        request = send_request(endpoint, token, "get")
+        request = await send_request(endpoint, token, "get")
         user_list = [
             User(
                 username="",
                 proxies={},
                 inbounds={},
                 expire=0,
                 data_limit=0,
@@ -162,40 +163,39 @@
             )
         ]
         for user in request["users"]:
             user_list.append(User(**user))
         del user_list[0]
         return user_list
 
-    def reset_all_users_traffic(self, token: dict):
+    async def reset_all_users_traffic(self, token: dict):
         """reset all users traffic.
 
         Parameters:
             token (``dict``) : Authorization token
 
         Returns: `~str`: success
         """
-        send_request("users/reset", token, "post")
+        await send_request("users/reset", token, "post")
         return "success"
 
-    def get_user_usage(self, user_username: str, token: dict):
+    async def get_user_usage(self, user_username: str, token: dict):
         """get user usage by username.
 
         Parameters:
             user_username (``str``) : username of user
 
             token (``dict``) : Authorization token
 
         Returns: `~dict`: dict of user usage
         """
-        return send_request(f"user/{user_username}/usage", token, "get")["usages"]
+        return await end_request(f"user/{user_username}/usage", token, "get")["usages"]
 
-    def get_all_users_count(self, token: dict):
+    async def get_all_users_count(self, token: dict):
         """get all users count.
 
         Parameters:
             token (``dict``) : Authorization token
 
         Returns: `~int`: count of users
         """
-        return self.get_all_users(token)["content"]["total"]
-
+        return await self.get_all_users(token)["content"]["total"]
```

### Comparing `marzpy-0.0.3/setup.py` & `marzpy-0.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as file:
     readme = file.read()
 
 setup(
     name="marzpy",
-    version="0.0.3",
+    version="0.0.4",
     author="Mewhrzad",
     description="a simple application with python to manage Marzban panel",
     long_description="text/markdown",
     url="https://github.com/Mewhrzad/marzpy",
     keywords=["marzpy", "Marzban", "Gozargah", "Marzban python", "Marzban API"],
     packages=find_packages(),
-    ins=["requests"],
+    ins=["aiohttp"],
     classifiers=["Programming Language :: Python :: 3"],
 )
```

