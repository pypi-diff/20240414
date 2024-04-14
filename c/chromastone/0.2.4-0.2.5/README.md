# Comparing `tmp/chromastone-0.2.4.tar.gz` & `tmp/chromastone-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromastone-0.2.4.tar", last modified: Sun Apr 14 11:31:52 2024, max compression
+gzip compressed data, was "chromastone-0.2.5.tar", last modified: Sun Apr 14 16:19:07 2024, max compression
```

## Comparing `chromastone-0.2.4.tar` & `chromastone-0.2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 11:31:52.419134 chromastone-0.2.4/
--rw-r--r--   0 lordskyzw   (501) staff       (20)     1082 2024-03-29 23:18:58.000000 chromastone-0.2.4/LICENSE
--rw-r--r--   0 lordskyzw   (501) staff       (20)     2595 2024-04-14 11:31:52.418777 chromastone-0.2.4/PKG-INFO
-drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 11:31:52.413375 chromastone-0.2.4/chromastone/
--rw-r--r--   0 lordskyzw   (501) staff       (20)     4768 2024-04-14 11:13:49.000000 chromastone-0.2.4/chromastone/__init__.py
--rw-r--r--   0 lordskyzw   (501) staff       (20)     6611 2024-04-14 11:31:22.000000 chromastone-0.2.4/chromastone/chromastone.py
-drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 11:31:52.418151 chromastone-0.2.4/chromastone.egg-info/
--rw-r--r--   0 lordskyzw   (501) staff       (20)     2595 2024-04-14 11:31:52.000000 chromastone-0.2.4/chromastone.egg-info/PKG-INFO
--rw-r--r--   0 lordskyzw   (501) staff       (20)      241 2024-04-14 11:31:52.000000 chromastone-0.2.4/chromastone.egg-info/SOURCES.txt
--rw-r--r--   0 lordskyzw   (501) staff       (20)        1 2024-04-14 11:31:52.000000 chromastone-0.2.4/chromastone.egg-info/dependency_links.txt
--rw-r--r--   0 lordskyzw   (501) staff       (20)       18 2024-04-14 11:31:52.000000 chromastone-0.2.4/chromastone.egg-info/requires.txt
--rw-r--r--   0 lordskyzw   (501) staff       (20)       12 2024-04-14 11:31:52.000000 chromastone-0.2.4/chromastone.egg-info/top_level.txt
--rw-r--r--   0 lordskyzw   (501) staff       (20)       38 2024-04-14 11:31:52.419256 chromastone-0.2.4/setup.cfg
--rw-r--r--   0 lordskyzw   (501) staff       (20)      795 2024-04-14 11:31:44.000000 chromastone-0.2.4/setup.py
+drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 16:19:07.829417 chromastone-0.2.5/
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     1082 2024-03-29 23:18:58.000000 chromastone-0.2.5/LICENSE
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     2595 2024-04-14 16:19:07.829024 chromastone-0.2.5/PKG-INFO
+drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 16:19:07.823143 chromastone-0.2.5/chromastone/
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     6192 2024-04-14 16:16:28.000000 chromastone-0.2.5/chromastone/__init__.py
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     6633 2024-04-14 15:08:39.000000 chromastone-0.2.5/chromastone/chromastone.py
+drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 16:19:07.828270 chromastone-0.2.5/chromastone.egg-info/
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     2595 2024-04-14 16:19:07.000000 chromastone-0.2.5/chromastone.egg-info/PKG-INFO
+-rw-r--r--   0 lordskyzw   (501) staff       (20)      241 2024-04-14 16:19:07.000000 chromastone-0.2.5/chromastone.egg-info/SOURCES.txt
+-rw-r--r--   0 lordskyzw   (501) staff       (20)        1 2024-04-14 16:19:07.000000 chromastone-0.2.5/chromastone.egg-info/dependency_links.txt
+-rw-r--r--   0 lordskyzw   (501) staff       (20)       18 2024-04-14 16:19:07.000000 chromastone-0.2.5/chromastone.egg-info/requires.txt
+-rw-r--r--   0 lordskyzw   (501) staff       (20)       12 2024-04-14 16:19:07.000000 chromastone-0.2.5/chromastone.egg-info/top_level.txt
+-rw-r--r--   0 lordskyzw   (501) staff       (20)       38 2024-04-14 16:19:07.829602 chromastone-0.2.5/setup.cfg
+-rw-r--r--   0 lordskyzw   (501) staff       (20)      795 2024-04-14 16:19:00.000000 chromastone-0.2.5/setup.py
```

### Comparing `chromastone-0.2.4/LICENSE` & `chromastone-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `chromastone-0.2.4/PKG-INFO` & `chromastone-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromastone
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python application for powering other python applications to send SMS messages globally with number validation and restrictions by Tarmica Chiwara
 Home-page: https://github.com/lordskyzw/chromastone
 Author: Tarmica Chiwara
 Author-email: lilskyforever@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chromastone-0.2.4/chromastone/__init__.py` & `chromastone-0.2.5/chromastone/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         if balance == 'Failed to check balance, check your api key or internet connection':
             raise Exception('Failed to check balance, check your api key or internet connection')
         else:
             balance = int(balance)
         if balance > 0:
             try:
                 sms = SMSModel(source_number=source_number, destination_number=destination_number, message=message)
-                sms_data = sms.dict()
+                sms_data = sms.model_dump_json()
                 response = requests.post(url=full_url, json=sms_data, headers=headers)
                 if response.status_code == 200:
                     print('SMS sent successfully, remaining balance:', response.json()['balance'])
                     return 'SMS sent successfully'
                 else:
                     print('Failed to send SMS, status code:', response.status_code)
                     return 'Failed to send SMS'
@@ -86,21 +86,47 @@
         if balance == 'Failed to check balance, check your api key or internet connection':
             raise Exception('Failed to check balance, check your api key or internet connection')
         else:
             balance = int(balance)
         if balance > 0:
             try:
                 sms = SMSModel(source_number=source_number, destination_number=destination_number, message=message)
-                sms_data = sms.dict()
+                sms_data = sms.model_dump_json()
                 response = requests.post(url=full_url, json=sms_data, headers=headers)
                 if response.status_code == 200:
                     print('Innbucks sent successfully, remaining balance:', response.json()['balance'])
                     return 'Innbucks sent successfully'
                 else:
                     print('Failed to send Innbucks, status code:', response.status_code)
                     return 'Failed to send Innbucks'
             except ValidationError as e:
                 print(e.json())
                 return f"Failed to send Innbucks, {e.json()}"
+            
+
+    def send_mukuru(self, destination_number: str, message: str, source_number='mukuru'):
+        full_url = self.base_url + '/send_mukuru'
+        headers = {'Authorization': f'Bearer {self.api_key}',
+                   'Content-Type': 'application/json'}
+        # check if the user has enough balance to send the SMS
+        balance = self.check_balance()
+        if balance == 'Failed to check balance, check your api key or internet connection':
+            raise Exception('Failed to check balance, check your api key or internet connection')
+        else:
+            balance = int(balance)
+        if balance > 0:
+            try:
+                sms = SMSModel(source_number=source_number, destination_number=destination_number, message=message)
+                sms_data = sms.model_dump_json()
+                response = requests.post(url=full_url, json=sms_data, headers=headers)
+                if response.status_code == 200:
+                    print('mukuru sent successfully, remaining balance:', response.json()['balance'])
+                    return 'mukuru sent successfully'
+                else:
+                    print('Failed to send mukuru, status code:', response.status_code)
+                    return 'Failed to send mukuru'
+            except ValidationError as e:
+                print(e.json())
+                return f"Failed to send mukuru, {e.json()}"
```

### Comparing `chromastone-0.2.4/chromastone/chromastone.py` & `chromastone-0.2.5/chromastone/chromastone.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         if balance == 'Failed to check balance, check your api key or internet connection':
             raise Exception('Failed to check balance, check your api key or internet connection')
         else:
             balance = int(balance)
         if balance > 0:
             try:
                 sms = SMSModel(source_number=source_number, destination_number=destination_number, message=message)
-                sms_data = sms.dict()
+                sms_data = sms.model_dump_json()
                 response = requests.post(url=full_url, json=sms_data, headers=headers)
                 if response.status_code == 200:
                     print('Innbucks sent successfully, remaining balance:', response.json()['balance'])
                     return 'Innbucks sent successfully'
                 else:
                     print('Failed to send Innbucks, status code:', response.status_code)
                     return 'Failed to send Innbucks'
@@ -114,16 +114,16 @@
         if balance == 'Failed to check balance, check your api key or internet connection':
             raise Exception('Failed to check balance, check your api key or internet connection')
         else:
             balance = int(balance)
         if balance > 0:
             try:
                 sms = SMSModel(destination_number=destination_number, message=message)
-                sms_data = sms.dict()
-                response = requests.post(url=full_url, data=sms_data, headers=headers)
+                sms_data = sms.model_dump_json()
+                response = requests.post(url=full_url, json=sms_data, headers=headers)
                 if response.status_code == 200:
                     print('mukuru sent successfully, remaining balance:', response.json()['balance'])
                     return 'mukuru sent successfully'
                 else:
                     print('Failed to send mukuru, status code:', response.status_code)
                     return 'Failed to send mukuru'
             except ValidationError as e:
```

### Comparing `chromastone-0.2.4/chromastone.egg-info/PKG-INFO` & `chromastone-0.2.5/chromastone.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromastone
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Python application for powering other python applications to send SMS messages globally with number validation and restrictions by Tarmica Chiwara
 Home-page: https://github.com/lordskyzw/chromastone
 Author: Tarmica Chiwara
 Author-email: lilskyforever@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chromastone-0.2.4/setup.py` & `chromastone-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='chromastone', 
-    version='0.2.4',
+    version='0.2.5',
     author='Tarmica Chiwara',  
     author_email='lilskyforever@gmail.com',  
     description='A Python application for powering other python applications to send SMS messages globally with number validation and restrictions by Tarmica Chiwara',
     long_description=open('readme.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/lordskyzw/chromastone', 
     packages=find_packages(),
```

