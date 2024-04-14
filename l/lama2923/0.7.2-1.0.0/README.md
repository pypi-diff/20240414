# Comparing `tmp/lama2923-0.7.2.tar.gz` & `tmp/lama2923-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lama2923-0.7.2.tar", last modified: Sun Apr 14 00:52:22 2024, max compression
+gzip compressed data, was "lama2923-1.0.0.tar", last modified: Sun Apr 14 02:17:50 2024, max compression
```

## Comparing `lama2923-0.7.2.tar` & `lama2923-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 00:52:22.272061 lama2923-0.7.2/
--rw-rw-rw-   0        0        0      943 2024-04-14 00:52:22.270596 lama2923-0.7.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-14 00:52:22.253584 lama2923-0.7.2/lama2923/
--rw-rw-rw-   0        0        0    24142 2024-04-14 00:51:37.000000 lama2923-0.7.2/lama2923/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:52:22.268049 lama2923-0.7.2/lama2923.egg-info/
--rw-rw-rw-   0        0        0      943 2024-04-14 00:52:21.000000 lama2923-0.7.2/lama2923.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-04-14 00:52:22.000000 lama2923-0.7.2/lama2923.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 00:52:21.000000 lama2923-0.7.2/lama2923.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-14 00:52:21.000000 lama2923-0.7.2/lama2923.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-14 00:52:21.000000 lama2923-0.7.2/lama2923.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 00:52:22.272061 lama2923-0.7.2/setup.cfg
--rw-rw-rw-   0        0        0     1281 2024-04-14 00:52:11.000000 lama2923-0.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 02:17:50.045637 lama2923-1.0.0/
+-rw-rw-rw-   0        0        0      956 2024-04-14 02:17:50.044135 lama2923-1.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-14 02:17:50.026034 lama2923-1.0.0/lama2923/
+-rw-rw-rw-   0        0        0    26157 2024-04-14 02:17:30.000000 lama2923-1.0.0/lama2923/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 02:17:50.041133 lama2923-1.0.0/lama2923.egg-info/
+-rw-rw-rw-   0        0        0      956 2024-04-14 02:17:49.000000 lama2923-1.0.0/lama2923.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-04-14 02:17:49.000000 lama2923-1.0.0/lama2923.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 02:17:49.000000 lama2923-1.0.0/lama2923.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-14 02:17:49.000000 lama2923-1.0.0/lama2923.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-14 02:17:49.000000 lama2923-1.0.0/lama2923.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 02:17:50.045637 lama2923-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1294 2024-04-14 02:17:22.000000 lama2923-1.0.0/setup.py
```

### Comparing `lama2923-0.7.2/PKG-INFO` & `lama2923-1.0.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: lama2923
-Version: 0.7.2
+Version: 1.0.0
 Summary: Sikimsonik bir kütüphane
 Author: lama2923
 Author-email: lama2923.v2@gmail.com
 Keywords: example project setuptools development discord lama2923
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `lama2923-0.7.2/lama2923/__init__.py` & `lama2923-1.0.0/lama2923/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # python version = 3.11
 import os
 import time
 import socket
 from colorama import Fore, Style, init
 import requests
 import msvcrt
+import requests
+import os
+import requests
 
 
 def ekran_temizle():
     if os.name == 'posix':
         os.system('clear')
     elif os.name == 'nt':
         os.system('cls')
@@ -442,16 +445,16 @@
 
         def send_tts_message(self, Channel_id, Message):
             payload = {'content': str(Message), 'tts': True}
             headers = {'Authorization': str(self.token)}
             response = requests.post(f'https://discord.com/api/v9/channels/{Channel_id}/messages', data=payload, headers=headers)
             return response.status_code
         
-        def send_reply_message(self, Channel_id, Message, Message_id):
-            payload = {'content': str(Message), 'message_reference': {'message_id': Message_id}}
+        def send_reply_message(self, Channel_id, Message, ReplyMessage_id):
+            payload = {'content': str(Message), 'message_reference': {'message_id': ReplyMessage_id}}
             headers = {'Authorization': str(self.token)}
             response = requests.post(f'https://discord.com/api/v9/channels/{Channel_id}/messages', data=payload, headers=headers)
             return response.status_code
         
         def change_user_nickname(self, Guild_id, Nickname):
             headers = {'Authorization': str(self.token)}
             payload = {'nick': str(Nickname)}
@@ -500,14 +503,36 @@
         
         def unban_member(self, Guild_id, Member_id):
             headers = {'Authorization': str(self.token)}
             url = f'https://discord.com/api/v9/guilds/{Guild_id}/bans/{Member_id}'
             response = requests.delete(url, headers=headers)
             return response.status_code
         
+
+
+        
+        def get_guild_bans(self, Guild_id):
+            headers = {'Authorization': str(self.token)}
+            url = f'https://discord.com/api/v9/guilds/{Guild_id}/bans'
+            response = requests.get(url, headers=headers)
+            if response.status_code == 200:
+                return [response.status_code, response.json()]
+            else:
+                return response.status_code
+            
+        
+        def get_guild_channels(self, Guild_id):
+            headers = {'Authorization': str(self.token)}
+            url = f'https://discord.com/api/v9/guilds/{Guild_id}/channels'
+            response = requests.get(url, headers=headers)
+            if response.status_code == 200:
+                return [response.status_code, response.json()]
+            else:
+                return response.status_code
+        
         def get_guild_members(self, Guild_id):
             headers = {'Authorization': str(self.token)}
             url = f'https://discord.com/api/v9/guilds/{Guild_id}/members'
             response = requests.get(url, headers=headers)
             if response.status_code == 200:
                 return [response.status_code, response.json()]
             else:
@@ -528,16 +553,14 @@
             response = requests.post(f'https://discord.com/api/v9/guilds/{Guild_id}/roles', json=payload, headers=headers)
             return response.status_code
         
         def delete_guild_role(self, Guild_id, Role_id):
             headers = {'Authorization': str(self.token)}
             response = requests.delete(f'https://discord.com/api/v9/guilds/{Guild_id}/roles/{Role_id}', headers=headers)
             return response.status_code
-        
-        
 
 
     class Webhook:
         def __init__(self, webhook_url):
             self.WebhookUrl = str(webhook_url)
             
         def send_webhook(self, Content='', embed=None, files=None):
@@ -610,13 +633,40 @@
                     return [response, response2]
                 else:
                     
                     response = requests.post(self.WebhookUrl, json=data)
                 
                     return response.status_code
                 
+        def delete_specific_message(self, Message_id):
+            response = requests.delete(f'{self.WebhookUrl}/messages/{Message_id}')
+            return response.status_code
+        
+        def get_specific_message(self, Message_id):
+            response = requests.get(f'{self.WebhookUrl}/messages/{Message_id}')
+            if response.status_code == 200:
+                return [response.status_code, response.json()]
+            else:
+                return response.status_code
+            
+        def get_webhook_info(self):
+            response = requests.get(self.WebhookUrl)
+            if response.status_code == 200:
+                return [response.status_code, response.json()]
+            else:
+                return response.status_code
+                
+                
+        def get_messages(self):
+            response = requests.get(f'{self.WebhookUrl}/messages')
+            if response.status_code == 200:
+                return [response.status_code, response.json()]
+            else:
+                return response.status_code
+            
+
```

### Comparing `lama2923-0.7.2/lama2923.egg-info/PKG-INFO` & `lama2923-1.0.0/lama2923.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: lama2923
-Version: 0.7.2
+Version: 1.0.0
 Summary: Sikimsonik bir kütüphane
 Author: lama2923
 Author-email: lama2923.v2@gmail.com
 Keywords: example project setuptools development discord lama2923
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `lama2923-0.7.2/setup.py` & `lama2923-1.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 # Komutlar.txt dosyasından komutlar ile terminalde setup dosyasını çalıştırım upload edebilirsin.
 
 setup(
     name='lama2923',
-    version='0.7.2',
+    version='1.0.0',
     description='Sikimsonik bir kütüphane',
     long_description="Discord Apı ile işlemler, Webhook ile işlemler, lprint, linput gibi güzel görünümlü yazılar... kısacası projenizde kullanabilceğiniz tasarım olarak ve sistem olarak kullanabilceğiniz bir kütüphane, ayrıca bu kütüphanenin ana dili Türkçe.",
     author='lama2923',
     author_email='lama2923.v2@gmail.com',
     classifiers=[
-        'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
```

