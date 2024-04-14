# Comparing `tmp/chromastone-0.2.0.tar.gz` & `tmp/chromastone-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromastone-0.2.0.tar", last modified: Sun Apr 14 07:03:03 2024, max compression
+gzip compressed data, was "chromastone-0.2.1.tar", last modified: Sun Apr 14 07:07:09 2024, max compression
```

## Comparing `chromastone-0.2.0.tar` & `chromastone-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 07:03:03.941292 chromastone-0.2.0/
--rw-r--r--   0 lordskyzw   (501) staff       (20)     1082 2024-03-29 23:18:58.000000 chromastone-0.2.0/LICENSE
--rw-r--r--   0 lordskyzw   (501) staff       (20)     2595 2024-04-14 07:03:03.940722 chromastone-0.2.0/PKG-INFO
-drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 07:03:03.935427 chromastone-0.2.0/chromastone/
--rw-r--r--   0 lordskyzw   (501) staff       (20)     4719 2024-04-13 21:06:06.000000 chromastone-0.2.0/chromastone/__init__.py
--rw-r--r--   0 lordskyzw   (501) staff       (20)     6551 2024-04-14 07:02:07.000000 chromastone-0.2.0/chromastone/chromastone.py
-drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 07:03:03.939821 chromastone-0.2.0/chromastone.egg-info/
--rw-r--r--   0 lordskyzw   (501) staff       (20)     2595 2024-04-14 07:03:03.000000 chromastone-0.2.0/chromastone.egg-info/PKG-INFO
--rw-r--r--   0 lordskyzw   (501) staff       (20)      241 2024-04-14 07:03:03.000000 chromastone-0.2.0/chromastone.egg-info/SOURCES.txt
--rw-r--r--   0 lordskyzw   (501) staff       (20)        1 2024-04-14 07:03:03.000000 chromastone-0.2.0/chromastone.egg-info/dependency_links.txt
--rw-r--r--   0 lordskyzw   (501) staff       (20)       18 2024-04-14 07:03:03.000000 chromastone-0.2.0/chromastone.egg-info/requires.txt
--rw-r--r--   0 lordskyzw   (501) staff       (20)       12 2024-04-14 07:03:03.000000 chromastone-0.2.0/chromastone.egg-info/top_level.txt
--rw-r--r--   0 lordskyzw   (501) staff       (20)       38 2024-04-14 07:03:03.941508 chromastone-0.2.0/setup.cfg
--rw-r--r--   0 lordskyzw   (501) staff       (20)      795 2024-04-14 07:02:56.000000 chromastone-0.2.0/setup.py
+drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 07:07:09.868939 chromastone-0.2.1/
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     1082 2024-03-29 23:18:58.000000 chromastone-0.2.1/LICENSE
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     2595 2024-04-14 07:07:09.868338 chromastone-0.2.1/PKG-INFO
+drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 07:07:09.863283 chromastone-0.2.1/chromastone/
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     4768 2024-04-14 07:06:37.000000 chromastone-0.2.1/chromastone/__init__.py
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     6600 2024-04-14 07:06:42.000000 chromastone-0.2.1/chromastone/chromastone.py
+drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 07:07:09.867355 chromastone-0.2.1/chromastone.egg-info/
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     2595 2024-04-14 07:07:09.000000 chromastone-0.2.1/chromastone.egg-info/PKG-INFO
+-rw-r--r--   0 lordskyzw   (501) staff       (20)      241 2024-04-14 07:07:09.000000 chromastone-0.2.1/chromastone.egg-info/SOURCES.txt
+-rw-r--r--   0 lordskyzw   (501) staff       (20)        1 2024-04-14 07:07:09.000000 chromastone-0.2.1/chromastone.egg-info/dependency_links.txt
+-rw-r--r--   0 lordskyzw   (501) staff       (20)       18 2024-04-14 07:07:09.000000 chromastone-0.2.1/chromastone.egg-info/requires.txt
+-rw-r--r--   0 lordskyzw   (501) staff       (20)       12 2024-04-14 07:07:09.000000 chromastone-0.2.1/chromastone.egg-info/top_level.txt
+-rw-r--r--   0 lordskyzw   (501) staff       (20)       38 2024-04-14 07:07:09.869127 chromastone-0.2.1/setup.cfg
+-rw-r--r--   0 lordskyzw   (501) staff       (20)      795 2024-04-14 07:06:51.000000 chromastone-0.2.1/setup.py
```

### Comparing `chromastone-0.2.0/LICENSE` & `chromastone-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chromastone-0.2.0/PKG-INFO` & `chromastone-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromastone
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python application for powering other python applications to send SMS messages globally with number validation and restrictions by Tarmica Chiwara
 Home-page: https://github.com/lordskyzw/chromastone
 Author: Tarmica Chiwara
 Author-email: lilskyforever@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chromastone-0.2.0/chromastone/__init__.py` & `chromastone-0.2.1/chromastone/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,27 +73,27 @@
                     return 'Failed to send SMS'
             except ValidationError as e:
                 print(e.json())
                 return f"Failed to send SMS, {e.json()}"
         else:
             return 'You do not have enough balance to send the SMS'
         
-    def send_innbucks(self, destination_number: str, message: str):
+    def send_innbucks(self, destination_number: str, message: str, source_number=None):
         full_url = self.base_url + '/send_innbucks'
         headers = {'Authorization': f'Bearer {self.api_key}',
                    'Content-Type': 'application/json'}
         # check if the user has enough balance to send the SMS
         balance = self.check_balance()
         if balance == 'Failed to check balance, check your api key or internet connection':
             raise Exception('Failed to check balance, check your api key or internet connection')
         else:
             balance = int(balance)
         if balance > 0:
             try:
-                sms = SMSModel(destination_number=destination_number, message=message)
+                sms = SMSModel(source_number=source_number, destination_number=destination_number, message=message)
                 sms_data = sms.dict()
                 response = requests.post(url=full_url, data=sms_data, headers=headers)
                 if response.status_code == 200:
                     print('Innbucks sent successfully, remaining balance:', response.json()['balance'])
                     return 'Innbucks sent successfully'
                 else:
                     print('Failed to send Innbucks, status code:', response.status_code)
```

### Comparing `chromastone-0.2.0/chromastone/chromastone.py` & `chromastone-0.2.1/chromastone/chromastone.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,28 +74,28 @@
                     return 'Failed to send SMS'
             except ValidationError as e:
                 print(e.json())
                 return f"Failed to send SMS, {e.json()}"
         else:
             return 'You do not have enough balance to send the SMS'
         
-    def send_innbucks(self, destination_number: str, message: str):
+    def send_innbucks(self, destination_number: str, message: str, source_number=None):
         '''send InnBucks to a user, destination_number must be of the form 263xxxxxxxxx, message must not exceed 120 characters.'''
         full_url = self.base_url + '/send_innbucks'
         headers = {'Authorization': f'Bearer {self.api_key}',
                    'Content-Type': 'application/json'}
         # check if the user has enough balance to send the SMS
         balance = self.check_balance()
         if balance == 'Failed to check balance, check your api key or internet connection':
             raise Exception('Failed to check balance, check your api key or internet connection')
         else:
             balance = int(balance)
         if balance > 0:
             try:
-                sms = SMSModel(destination_number=destination_number, message=message)
+                sms = SMSModel(source_number=source_number, destination_number=destination_number, message=message)
                 sms_data = sms.dict()
                 response = requests.post(url=full_url, data=sms_data, headers=headers)
                 if response.status_code == 200:
                     print('Innbucks sent successfully, remaining balance:', response.json()['balance'])
                     return 'Innbucks sent successfully'
                 else:
                     print('Failed to send Innbucks, status code:', response.status_code)
```

### Comparing `chromastone-0.2.0/chromastone.egg-info/PKG-INFO` & `chromastone-0.2.1/chromastone.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromastone
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python application for powering other python applications to send SMS messages globally with number validation and restrictions by Tarmica Chiwara
 Home-page: https://github.com/lordskyzw/chromastone
 Author: Tarmica Chiwara
 Author-email: lilskyforever@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chromastone-0.2.0/setup.py` & `chromastone-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='chromastone', 
-    version='0.2.0',
+    version='0.2.1',
     author='Tarmica Chiwara',  
     author_email='lilskyforever@gmail.com',  
     description='A Python application for powering other python applications to send SMS messages globally with number validation and restrictions by Tarmica Chiwara',
     long_description=open('readme.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/lordskyzw/chromastone', 
     packages=find_packages(),
```

