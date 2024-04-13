# Comparing `tmp/lama2923-0.6.tar.gz` & `tmp/lama2923-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lama2923-0.6.tar", last modified: Sat Apr 13 18:04:56 2024, max compression
+gzip compressed data, was "lama2923-0.7.tar", last modified: Sat Apr 13 22:27:17 2024, max compression
```

## Comparing `lama2923-0.6.tar` & `lama2923-0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 18:04:56.499534 lama2923-0.6/
--rw-rw-rw-   0        0        0      895 2024-04-13 18:04:56.497835 lama2923-0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-13 18:04:56.478834 lama2923-0.6/lama2923/
--rw-rw-rw-   0        0        0    19506 2024-04-13 18:04:10.000000 lama2923-0.6/lama2923/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 18:04:56.494798 lama2923-0.6/lama2923.egg-info/
--rw-rw-rw-   0        0        0      895 2024-04-13 18:04:56.000000 lama2923-0.6/lama2923.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-04-13 18:04:56.000000 lama2923-0.6/lama2923.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 18:04:56.000000 lama2923-0.6/lama2923.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-13 18:04:56.000000 lama2923-0.6/lama2923.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-13 18:04:56.000000 lama2923-0.6/lama2923.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-13 18:04:56.500049 lama2923-0.6/setup.cfg
--rw-rw-rw-   0        0        0     1233 2024-04-13 18:04:36.000000 lama2923-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 22:27:17.612657 lama2923-0.7/
+-rw-rw-rw-   0        0        0      941 2024-04-13 22:27:17.610244 lama2923-0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-13 22:27:17.593610 lama2923-0.7/lama2923/
+-rw-rw-rw-   0        0        0    23634 2024-04-13 22:25:42.000000 lama2923-0.7/lama2923/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 22:27:17.608662 lama2923-0.7/lama2923.egg-info/
+-rw-rw-rw-   0        0        0      941 2024-04-13 22:27:17.000000 lama2923-0.7/lama2923.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-04-13 22:27:17.000000 lama2923-0.7/lama2923.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 22:27:17.000000 lama2923-0.7/lama2923.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-13 22:27:17.000000 lama2923-0.7/lama2923.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-13 22:27:17.000000 lama2923-0.7/lama2923.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-13 22:27:17.613174 lama2923-0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1279 2024-04-13 22:26:44.000000 lama2923-0.7/setup.py
```

### Comparing `lama2923-0.6/PKG-INFO` & `lama2923-0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lama2923
-Version: 0.6
+Version: 0.7
 Summary: Sikimsonik bir kütüphane
 Author: lama2923
 Author-email: lama2923.v2@gmail.com
 Keywords: example project setuptools development discord lama2923
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -12,8 +12,8 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 
-Discord Apı ile işlemler, Webhook ile işlemler, lprint, linput gibi güzel görünümlü yazılar... kısacası projenizde kullanabilceğiniz tasarım olarak ve sistem olarak kullanabilceğiniz bir kütüphane
+Discord Apı ile işlemler, Webhook ile işlemler, lprint, linput gibi güzel görünümlü yazılar... kısacası projenizde kullanabilceğiniz tasarım olarak ve sistem olarak kullanabilceğiniz bir kütüphane, ayrıca bu kütüphanenin ana dili Türkçe.
```

### Comparing `lama2923-0.6/lama2923/__init__.py` & `lama2923-0.7/lama2923/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -374,44 +374,27 @@
                 response = requests.post(f'https://discord.com/api/v9/channels/{Channel_id}/messages', data=payload, files=files_data, headers=headers)
             else:
                 response = requests.post(f'https://discord.com/api/v9/channels/{Channel_id}/messages', data=payload, headers=headers)
                 
             return response.status_code
         
         def delete_message(self, Channel_id, Message_id):
-            headers = {
-                'Authorization': str(self.token)
-            }
-    
-    
+            headers = {'Authorization': str(self.token)}
             r = requests.delete(f'https://discord.com/api/v9/channels/{Channel_id}/messages/{Message_id}', headers=headers)
-            
             return r.status_code
         
         def edit_message(self, Channel_id, Message_id, Message_Content):
-            headers = {
-                'Authorization': str(self.token)
-            }
-            
-            payload = {
-                'content': str(Message_Content)
-            }
-            
+            headers = {'Authorization': str(self.token)}
+            payload = {'content': str(Message_Content)}
             r = requests.patch(f'https://discord.com/api/v9/channels/{Channel_id}/messages/{Message_id}', json=payload, headers=headers)
-            
             return r.status_code
         
         def get_channel_message(self, Channel_id):
-            
-            headers = {
-                'Authorization': str(self.token)
-            }
-            
+            headers = {'Authorization': str(self.token)}
             r = requests.get(f'https://discord.com/api/v9/channels/{Channel_id}/messages', headers=headers)
-            
             if r.status_code == 200:
                 messages = r.json()
                 return [r.status_code, messages]
             else:
                 return r.status_code
             
         def get_specific_message(self, Channel_id, Message_id):
@@ -452,17 +435,102 @@
 
         def send_tts_message(self, Channel_id, Message):
             payload = {'content': str(Message), 'tts': True}
             headers = {'Authorization': str(self.token)}
             response = requests.post(f'https://discord.com/api/v9/channels/{Channel_id}/messages', data=payload, headers=headers)
             return response.status_code
         
+        def send_reply_message(self, Channel_id, Message, Message_id):
+            payload = {'content': str(Message), 'message_reference': {'message_id': Message_id}}
+            headers = {'Authorization': str(self.token)}
+            response = requests.post(f'https://discord.com/api/v9/channels/{Channel_id}/messages', data=payload, headers=headers)
+            return response.status_code
+        
+        def change_nickname(self, Guild_id, Nickname):
+            headers = {'Authorization': str(self.token)}
+            payload = {'nick': str(Nickname)}
+            response = requests.patch(f'https://discord.com/api/v9/guilds/{Guild_id}/members/@me/nick', json=payload, headers=headers)
+            return response.status_code
+
+        def get_user_info(self, User_id):
+            headers = {'Authorization': str(self.token)}
+            url = f'https://discord.com/api/v9/users/{User_id}'
+            response = requests.get(url, headers=headers)
+            if response.status_code == 200:
+                return [response.status_code, response.json()]
+            else:
+                return response.status_code
+
+        def get_all_guilds(self):
+            headers = {'Authorization': str(self.token)}
+            url = 'https://discord.com/api/v9/users/@me/guilds'
+            response = requests.get(url, headers=headers)
+            if response.status_code == 200:
+                return [response.status_code, response.json()]
+            else:
+                return response.status_code
+        
+        def get_spesific_guild(self, Guild_id):
+            headers = {'Authorization': str(self.token)}
+            url = f'https://discord.com/api/v9/guilds/{Guild_id}'
+            response = requests.get(url, headers=headers)
+            if response.status_code == 200:
+                return [response.status_code, response.json()]
+            else:
+                return response.status_code
+            
+        def kick_member(self, Guild_id, Member_id):
+            headers = {'Authorization': str(self.token)}
+            url = f'https://discord.com/api/v9/guilds/{Guild_id}/members/{Member_id}'
+            response = requests.delete(url, headers=headers)
+            return response.status_code
+        
+        def ban_member(self, Guild_id, Member_id):
+            headers = {'Authorization': str(self.token)}
+            url = f'https://discord.com/api/v9/guilds/{Guild_id}/bans/{Member_id}'
+            response = requests.put(url, headers=headers)
+            return response.status_code
+        
+        def unban_member(self, Guild_id, Member_id):
+            headers = {'Authorization': str(self.token)}
+            url = f'https://discord.com/api/v9/guilds/{Guild_id}/bans/{Member_id}'
+            response = requests.delete(url, headers=headers)
+            return response.status_code
+        
+        def get_guild_members(self, Guild_id):
+            headers = {'Authorization': str(self.token)}
+            url = f'https://discord.com/api/v9/guilds/{Guild_id}/members'
+            response = requests.get(url, headers=headers)
+            if response.status_code == 200:
+                return [response.status_code, response.json()]
+            else:
+                return response.status_code
+            
+        def get_guild_roles(self, Guild_id):
+            headers = {'Authorization': str(self.token)}
+            url = f'https://discord.com/api/v9/guilds/{Guild_id}/roles'
+            response = requests.get(url, headers=headers)
+            if response.status_code == 200:
+                return [response.status_code, response.json()]
+            else:
+                return response.status_code
+            
+        def create_guild_role(self, Guild_id, Role_name):
+            headers = {'Authorization': str(self.token)}
+            payload = {'name': str(Role_name)}
+            response = requests.post(f'https://discord.com/api/v9/guilds/{Guild_id}/roles', json=payload, headers=headers)
+            return response.status_code
+        
+        def delete_guild_role(self, Guild_id, Role_id):
+            headers = {'Authorization': str(self.token)}
+            response = requests.delete(f'https://discord.com/api/v9/guilds/{Guild_id}/roles/{Role_id}', headers=headers)
+            return response.status_code
+        
         
 
-    
     class Webhook:
         def __init__(self, webhook_url):
             self.WebhookUrl = str(webhook_url)
             
         def send_webhook(self, Content='', embed=None, files=None):
             def format_embed(embed):
                 formatted_embed = {}
```

### Comparing `lama2923-0.6/lama2923.egg-info/PKG-INFO` & `lama2923-0.7/lama2923.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lama2923
-Version: 0.6
+Version: 0.7
 Summary: Sikimsonik bir kütüphane
 Author: lama2923
 Author-email: lama2923.v2@gmail.com
 Keywords: example project setuptools development discord lama2923
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -12,8 +12,8 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 
-Discord Apı ile işlemler, Webhook ile işlemler, lprint, linput gibi güzel görünümlü yazılar... kısacası projenizde kullanabilceğiniz tasarım olarak ve sistem olarak kullanabilceğiniz bir kütüphane
+Discord Apı ile işlemler, Webhook ile işlemler, lprint, linput gibi güzel görünümlü yazılar... kısacası projenizde kullanabilceğiniz tasarım olarak ve sistem olarak kullanabilceğiniz bir kütüphane, ayrıca bu kütüphanenin ana dili Türkçe.
```

### Comparing `lama2923-0.6/setup.py` & `lama2923-0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 # Komutlar.txt dosyasından komutlar ile terminalde setup dosyasını çalıştırım upload edebilirsin.
 
 setup(
     name='lama2923',
-    version='0.6',
+    version='0.7',
     description='Sikimsonik bir kütüphane',
-    long_description="Discord Apı ile işlemler, Webhook ile işlemler, lprint, linput gibi güzel görünümlü yazılar... kısacası projenizde kullanabilceğiniz tasarım olarak ve sistem olarak kullanabilceğiniz bir kütüphane",
+    long_description="Discord Apı ile işlemler, Webhook ile işlemler, lprint, linput gibi güzel görünümlü yazılar... kısacası projenizde kullanabilceğiniz tasarım olarak ve sistem olarak kullanabilceğiniz bir kütüphane, ayrıca bu kütüphanenin ana dili Türkçe.",
     author='lama2923',
     author_email='lama2923.v2@gmail.com',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
```

