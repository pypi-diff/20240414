# Comparing `tmp/lama2923-0.7.1.tar.gz` & `tmp/lama2923-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lama2923-0.7.1.tar", last modified: Sat Apr 13 23:44:49 2024, max compression
+gzip compressed data, was "lama2923-0.7.2.tar", last modified: Sun Apr 14 00:52:22 2024, max compression
```

## Comparing `lama2923-0.7.1.tar` & `lama2923-0.7.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 23:44:49.982944 lama2923-0.7.1/
--rw-rw-rw-   0        0        0      943 2024-04-13 23:44:49.980412 lama2923-0.7.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-13 23:44:49.940686 lama2923-0.7.1/lama2923/
--rw-rw-rw-   0        0        0    23730 2024-04-13 23:30:52.000000 lama2923-0.7.1/lama2923/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-13 23:44:49.974851 lama2923-0.7.1/lama2923.egg-info/
--rw-rw-rw-   0        0        0      943 2024-04-13 23:44:49.000000 lama2923-0.7.1/lama2923.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-04-13 23:44:49.000000 lama2923-0.7.1/lama2923.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 23:44:49.000000 lama2923-0.7.1/lama2923.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-13 23:44:49.000000 lama2923-0.7.1/lama2923.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-13 23:44:49.000000 lama2923-0.7.1/lama2923.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-13 23:44:49.983944 lama2923-0.7.1/setup.cfg
--rw-rw-rw-   0        0        0     1281 2024-04-13 23:44:27.000000 lama2923-0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 00:52:22.272061 lama2923-0.7.2/
+-rw-rw-rw-   0        0        0      943 2024-04-14 00:52:22.270596 lama2923-0.7.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-14 00:52:22.253584 lama2923-0.7.2/lama2923/
+-rw-rw-rw-   0        0        0    24142 2024-04-14 00:51:37.000000 lama2923-0.7.2/lama2923/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 00:52:22.268049 lama2923-0.7.2/lama2923.egg-info/
+-rw-rw-rw-   0        0        0      943 2024-04-14 00:52:21.000000 lama2923-0.7.2/lama2923.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-04-14 00:52:22.000000 lama2923-0.7.2/lama2923.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 00:52:21.000000 lama2923-0.7.2/lama2923.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-14 00:52:21.000000 lama2923-0.7.2/lama2923.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-14 00:52:21.000000 lama2923-0.7.2/lama2923.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 00:52:22.272061 lama2923-0.7.2/setup.cfg
+-rw-rw-rw-   0        0        0     1281 2024-04-14 00:52:11.000000 lama2923-0.7.2/setup.py
```

### Comparing `lama2923-0.7.1/PKG-INFO` & `lama2923-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lama2923
-Version: 0.7.1
+Version: 0.7.2
 Summary: Sikimsonik bir kütüphane
 Author: lama2923
 Author-email: lama2923.v2@gmail.com
 Keywords: example project setuptools development discord lama2923
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lama2923-0.7.1/lama2923/__init__.py` & `lama2923-0.7.2/lama2923/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -409,14 +409,21 @@
 
         def add_reaction(self, Channel_id, Message_id, emoji):
             headers = {'Authorization': str(self.token)}
             emoji = requests.utils.quote(emoji)
             url = f'https://discord.com/api/v9/channels/{Channel_id}/messages/{Message_id}/reactions/{emoji}/@me'
             response = requests.put(url, headers=headers)
             return response.status_code
+        
+        def remove_reaction(self, Channel_id, Message_id, emoji):
+            headers = {'Authorization': str(self.token)}
+            emoji = requests.utils.quote(emoji)
+            url = f'https://discord.com/api/v9/channels/{Channel_id}/messages/{Message_id}/reactions/{emoji}/@me'
+            response = requests.delete(url, headers=headers)
+            return response.status_code
 
 
         def get_channel_info(self, Channel_id):
             headers = {'Authorization': str(self.token)}
             url = f'https://discord.com/api/v9/channels/{Channel_id}'
             response = requests.get(url, headers=headers)
             if response.status_code == 200:
@@ -522,14 +529,15 @@
             return response.status_code
         
         def delete_guild_role(self, Guild_id, Role_id):
             headers = {'Authorization': str(self.token)}
             response = requests.delete(f'https://discord.com/api/v9/guilds/{Guild_id}/roles/{Role_id}', headers=headers)
             return response.status_code
         
+        
 
 
     class Webhook:
         def __init__(self, webhook_url):
             self.WebhookUrl = str(webhook_url)
             
         def send_webhook(self, Content='', embed=None, files=None):
```

### Comparing `lama2923-0.7.1/lama2923.egg-info/PKG-INFO` & `lama2923-0.7.2/lama2923.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lama2923
-Version: 0.7.1
+Version: 0.7.2
 Summary: Sikimsonik bir kütüphane
 Author: lama2923
 Author-email: lama2923.v2@gmail.com
 Keywords: example project setuptools development discord lama2923
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lama2923-0.7.1/setup.py` & `lama2923-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Komutlar.txt dosyasından komutlar ile terminalde setup dosyasını çalıştırım upload edebilirsin.
 
 setup(
     name='lama2923',
-    version='0.7.1',
+    version='0.7.2',
     description='Sikimsonik bir kütüphane',
     long_description="Discord Apı ile işlemler, Webhook ile işlemler, lprint, linput gibi güzel görünümlü yazılar... kısacası projenizde kullanabilceğiniz tasarım olarak ve sistem olarak kullanabilceğiniz bir kütüphane, ayrıca bu kütüphanenin ana dili Türkçe.",
     author='lama2923',
     author_email='lama2923.v2@gmail.com',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
```

