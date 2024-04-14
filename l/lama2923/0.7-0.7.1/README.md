# Comparing `tmp/lama2923-0.7.tar.gz` & `tmp/lama2923-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lama2923-0.7.tar", last modified: Sat Apr 13 22:27:17 2024, max compression
+gzip compressed data, was "lama2923-0.7.1.tar", last modified: Sat Apr 13 23:44:49 2024, max compression
```

## Comparing `lama2923-0.7.tar` & `lama2923-0.7.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 22:27:17.612657 lama2923-0.7/
--rw-rw-rw-   0        0        0      941 2024-04-13 22:27:17.610244 lama2923-0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-13 22:27:17.593610 lama2923-0.7/lama2923/
--rw-rw-rw-   0        0        0    23634 2024-04-13 22:25:42.000000 lama2923-0.7/lama2923/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 22:27:17.608662 lama2923-0.7/lama2923.egg-info/
--rw-rw-rw-   0        0        0      941 2024-04-13 22:27:17.000000 lama2923-0.7/lama2923.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-04-13 22:27:17.000000 lama2923-0.7/lama2923.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 22:27:17.000000 lama2923-0.7/lama2923.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-13 22:27:17.000000 lama2923-0.7/lama2923.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-13 22:27:17.000000 lama2923-0.7/lama2923.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-13 22:27:17.613174 lama2923-0.7/setup.cfg
--rw-rw-rw-   0        0        0     1279 2024-04-13 22:26:44.000000 lama2923-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 23:44:49.982944 lama2923-0.7.1/
+-rw-rw-rw-   0        0        0      943 2024-04-13 23:44:49.980412 lama2923-0.7.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-13 23:44:49.940686 lama2923-0.7.1/lama2923/
+-rw-rw-rw-   0        0        0    23730 2024-04-13 23:30:52.000000 lama2923-0.7.1/lama2923/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 23:44:49.974851 lama2923-0.7.1/lama2923.egg-info/
+-rw-rw-rw-   0        0        0      943 2024-04-13 23:44:49.000000 lama2923-0.7.1/lama2923.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-04-13 23:44:49.000000 lama2923-0.7.1/lama2923.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 23:44:49.000000 lama2923-0.7.1/lama2923.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-13 23:44:49.000000 lama2923-0.7.1/lama2923.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-13 23:44:49.000000 lama2923-0.7.1/lama2923.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-13 23:44:49.983944 lama2923-0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1281 2024-04-13 23:44:27.000000 lama2923-0.7.1/setup.py
```

### Comparing `lama2923-0.7/PKG-INFO` & `lama2923-0.7.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lama2923
-Version: 0.7
+Version: 0.7.1
 Summary: Sikimsonik bir kütüphane
 Author: lama2923
 Author-email: lama2923.v2@gmail.com
 Keywords: example project setuptools development discord lama2923
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lama2923-0.7/lama2923/__init__.py` & `lama2923-0.7.1/lama2923/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -441,15 +441,15 @@
         
         def send_reply_message(self, Channel_id, Message, Message_id):
             payload = {'content': str(Message), 'message_reference': {'message_id': Message_id}}
             headers = {'Authorization': str(self.token)}
             response = requests.post(f'https://discord.com/api/v9/channels/{Channel_id}/messages', data=payload, headers=headers)
             return response.status_code
         
-        def change_nickname(self, Guild_id, Nickname):
+        def change_user_nickname(self, Guild_id, Nickname):
             headers = {'Authorization': str(self.token)}
             payload = {'nick': str(Nickname)}
             response = requests.patch(f'https://discord.com/api/v9/guilds/{Guild_id}/members/@me/nick', json=payload, headers=headers)
             return response.status_code
 
         def get_user_info(self, User_id):
             headers = {'Authorization': str(self.token)}
@@ -480,18 +480,19 @@
             
         def kick_member(self, Guild_id, Member_id):
             headers = {'Authorization': str(self.token)}
             url = f'https://discord.com/api/v9/guilds/{Guild_id}/members/{Member_id}'
             response = requests.delete(url, headers=headers)
             return response.status_code
         
-        def ban_member(self, Guild_id, Member_id):
+        def ban_member(self, Guild_id, Member_id, delete_message_days=0):
             headers = {'Authorization': str(self.token)}
             url = f'https://discord.com/api/v9/guilds/{Guild_id}/bans/{Member_id}'
-            response = requests.put(url, headers=headers)
+            data = {'delete_message_days': delete_message_days}
+            response = requests.put(url, headers=headers, json=data)
             return response.status_code
         
         def unban_member(self, Guild_id, Member_id):
             headers = {'Authorization': str(self.token)}
             url = f'https://discord.com/api/v9/guilds/{Guild_id}/bans/{Member_id}'
             response = requests.delete(url, headers=headers)
             return response.status_code
@@ -521,15 +522,15 @@
             return response.status_code
         
         def delete_guild_role(self, Guild_id, Role_id):
             headers = {'Authorization': str(self.token)}
             response = requests.delete(f'https://discord.com/api/v9/guilds/{Guild_id}/roles/{Role_id}', headers=headers)
             return response.status_code
         
-        
+
 
     class Webhook:
         def __init__(self, webhook_url):
             self.WebhookUrl = str(webhook_url)
             
         def send_webhook(self, Content='', embed=None, files=None):
             def format_embed(embed):
```

### Comparing `lama2923-0.7/lama2923.egg-info/PKG-INFO` & `lama2923-0.7.1/lama2923.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lama2923
-Version: 0.7
+Version: 0.7.1
 Summary: Sikimsonik bir kütüphane
 Author: lama2923
 Author-email: lama2923.v2@gmail.com
 Keywords: example project setuptools development discord lama2923
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lama2923-0.7/setup.py` & `lama2923-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Komutlar.txt dosyasından komutlar ile terminalde setup dosyasını çalıştırım upload edebilirsin.
 
 setup(
     name='lama2923',
-    version='0.7',
+    version='0.7.1',
     description='Sikimsonik bir kütüphane',
     long_description="Discord Apı ile işlemler, Webhook ile işlemler, lprint, linput gibi güzel görünümlü yazılar... kısacası projenizde kullanabilceğiniz tasarım olarak ve sistem olarak kullanabilceğiniz bir kütüphane, ayrıca bu kütüphanenin ana dili Türkçe.",
     author='lama2923',
     author_email='lama2923.v2@gmail.com',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
```

