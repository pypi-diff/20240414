# Comparing `tmp/chromastone-0.1.7.tar.gz` & `tmp/chromastone-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromastone-0.1.7.tar", last modified: Sat Mar 30 16:05:26 2024, max compression
+gzip compressed data, was "chromastone-0.1.8.tar", last modified: Sat Apr 13 21:14:12 2024, max compression
```

## Comparing `chromastone-0.1.7.tar` & `chromastone-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-03-30 16:05:26.424225 chromastone-0.1.7/
--rw-r--r--   0 lordskyzw   (501) staff       (20)     1082 2024-03-29 23:18:58.000000 chromastone-0.1.7/LICENSE
--rw-r--r--   0 lordskyzw   (501) staff       (20)     2595 2024-03-30 16:05:26.423846 chromastone-0.1.7/PKG-INFO
-drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-03-30 16:05:26.417220 chromastone-0.1.7/chromastone/
--rw-r--r--   0 lordskyzw   (501) staff       (20)     3131 2024-03-30 07:25:12.000000 chromastone-0.1.7/chromastone/__init__.py
--rw-r--r--   0 lordskyzw   (501) staff       (20)     3259 2024-03-30 16:04:27.000000 chromastone-0.1.7/chromastone/chromastone.py
-drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-03-30 16:05:26.423107 chromastone-0.1.7/chromastone.egg-info/
--rw-r--r--   0 lordskyzw   (501) staff       (20)     2595 2024-03-30 16:05:26.000000 chromastone-0.1.7/chromastone.egg-info/PKG-INFO
--rw-r--r--   0 lordskyzw   (501) staff       (20)      241 2024-03-30 16:05:26.000000 chromastone-0.1.7/chromastone.egg-info/SOURCES.txt
--rw-r--r--   0 lordskyzw   (501) staff       (20)        1 2024-03-30 16:05:26.000000 chromastone-0.1.7/chromastone.egg-info/dependency_links.txt
--rw-r--r--   0 lordskyzw   (501) staff       (20)       18 2024-03-30 16:05:26.000000 chromastone-0.1.7/chromastone.egg-info/requires.txt
--rw-r--r--   0 lordskyzw   (501) staff       (20)       12 2024-03-30 16:05:26.000000 chromastone-0.1.7/chromastone.egg-info/top_level.txt
--rw-r--r--   0 lordskyzw   (501) staff       (20)       38 2024-03-30 16:05:26.424402 chromastone-0.1.7/setup.cfg
--rw-r--r--   0 lordskyzw   (501) staff       (20)      795 2024-03-30 16:05:18.000000 chromastone-0.1.7/setup.py
+drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-13 21:14:12.784772 chromastone-0.1.8/
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     1082 2024-03-29 23:18:58.000000 chromastone-0.1.8/LICENSE
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     2595 2024-04-13 21:14:12.784371 chromastone-0.1.8/PKG-INFO
+drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-13 21:14:12.778479 chromastone-0.1.8/chromastone/
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     4719 2024-04-13 21:06:06.000000 chromastone-0.1.8/chromastone/__init__.py
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     5151 2024-04-13 21:07:48.000000 chromastone-0.1.8/chromastone/chromastone.py
+drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-13 21:14:12.783668 chromastone-0.1.8/chromastone.egg-info/
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     2595 2024-04-13 21:14:12.000000 chromastone-0.1.8/chromastone.egg-info/PKG-INFO
+-rw-r--r--   0 lordskyzw   (501) staff       (20)      241 2024-04-13 21:14:12.000000 chromastone-0.1.8/chromastone.egg-info/SOURCES.txt
+-rw-r--r--   0 lordskyzw   (501) staff       (20)        1 2024-04-13 21:14:12.000000 chromastone-0.1.8/chromastone.egg-info/dependency_links.txt
+-rw-r--r--   0 lordskyzw   (501) staff       (20)       18 2024-04-13 21:14:12.000000 chromastone-0.1.8/chromastone.egg-info/requires.txt
+-rw-r--r--   0 lordskyzw   (501) staff       (20)       12 2024-04-13 21:14:12.000000 chromastone-0.1.8/chromastone.egg-info/top_level.txt
+-rw-r--r--   0 lordskyzw   (501) staff       (20)       38 2024-04-13 21:14:12.784913 chromastone-0.1.8/setup.cfg
+-rw-r--r--   0 lordskyzw   (501) staff       (20)      795 2024-04-13 21:09:01.000000 chromastone-0.1.8/setup.py
```

### Comparing `chromastone-0.1.7/LICENSE` & `chromastone-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chromastone-0.1.7/PKG-INFO` & `chromastone-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromastone
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python application for powering other python applications to send SMS messages globally with number validation and restrictions by Tarmica Chiwara
 Home-page: https://github.com/lordskyzw/chromastone
 Author: Tarmica Chiwara
 Author-email: lilskyforever@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chromastone-0.1.7/chromastone/__init__.py` & `chromastone-0.1.8/chromastone/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import requests
 from pydantic import BaseModel, ValidationError, validator
+from typing import Optional
 
 class SMSModel(BaseModel):
-    source_number: str
+    # source number is optional because it is not required for sending SMS
+    source_number: Optional[str]
     destination_number: str
     message: str
 
     @validator('destination_number')
     def validate_destination_number(cls, v):
         if not v.isdigit():
             raise ValueError('Destination number must contain only digits')
         if len(v) < 10 or len(v) > 15:
             raise ValueError('Destination number length must be between 10 and 15 digits')
         return v
 
     @validator('message')
     def validate_message_length(cls, v):
-        if len(v) > 100:
+        if len(v) > 120:
             raise ValueError('Message must not exceed 100 characters')
         return v
 
 class Chromastone:
     def __init__(self, api_key) -> None:
         self.api_key = api_key
         self.base_url = 'https://chromastone-production.up.railway.app'
@@ -57,20 +59,48 @@
         if balance == 'Failed to check balance, check your api key or internet connection':
             raise Exception('Failed to check balance, check your api key or internet connection')
         else:
             balance = int(balance)
         if balance > 0:
             try:
                 sms = SMSModel(source_number=source_number, destination_number=destination_number, message=message)
-                sms_data = sms.model_dump_json()
+                sms_data = sms.dict()
                 response = requests.post(url=full_url, data=sms_data, headers=headers)
                 if response.status_code == 200:
                     print('SMS sent successfully, remaining balance:', response.json()['balance'])
                     return 'SMS sent successfully'
                 else:
                     print('Failed to send SMS, status code:', response.status_code)
                     return 'Failed to send SMS'
             except ValidationError as e:
                 print(e.json())
+                return f"Failed to send SMS, {e.json()}"
+        else:
+            return 'You do not have enough balance to send the SMS'
+        
+    def send_innbucks(self, destination_number: str, message: str):
+        full_url = self.base_url + '/send_innbucks'
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
+                sms = SMSModel(destination_number=destination_number, message=message)
+                sms_data = sms.dict()
+                response = requests.post(url=full_url, data=sms_data, headers=headers)
+                if response.status_code == 200:
+                    print('Innbucks sent successfully, remaining balance:', response.json()['balance'])
+                    return 'Innbucks sent successfully'
+                else:
+                    print('Failed to send Innbucks, status code:', response.status_code)
+                    return 'Failed to send Innbucks'
+            except ValidationError as e:
+                print(e.json())
+                return f"Failed to send Innbucks, {e.json()}"
```

### Comparing `chromastone-0.1.7/chromastone/chromastone.py` & `chromastone-0.1.8/chromastone/chromastone.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import requests
 from pydantic import BaseModel, ValidationError, validator
+from typing import Optional
 
 class SMSModel(BaseModel):
-    source_number: str
+    # source number is optional because it is not required for sending SMS
+    source_number: Optional[str]
     destination_number: str
     message: str
 
     @validator('destination_number')
     def validate_destination_number(cls, v):
         if not v.isdigit():
             raise ValueError('Destination number must contain only digits')
         if len(v) < 10 or len(v) > 15:
             raise ValueError('Destination number length must be between 10 and 15 digits')
         return v
 
     @validator('message')
     def validate_message_length(cls, v):
-        if len(v) > 100:
+        if len(v) > 120:
             raise ValueError('Message must not exceed 100 characters')
         return v
 
 class Chromastone:
     def __init__(self, api_key) -> None:
         self.api_key = api_key
         self.base_url = 'https://chromastone-production.up.railway.app'
@@ -45,14 +47,15 @@
     def buy_sms(self, amount: int) -> None:
         '''this function will be used to buy more sms but it is not implemented yet,'''
 
         return 'This function is not implemented yet'
         
 
     def send_sms(self, source_number: str, destination_number: str, message: str):
+        '''destination_number must be of the form 263xxxxxxxxx, message must not exceed 120 characters, source_number is optional, it is the number that will be displayed as the sender of the SMS, it must be of the form 263xxxxxxxxx, if it is not provided, the default sender number will be used.'''
         full_url = self.base_url + '/send_sms'
         headers = {'Authorization': f'Bearer {self.api_key}',
                    'Content-Type': 'application/json'}
         # check if the user has enough balance to send the SMS
         balance = self.check_balance()
         if balance == 'Failed to check balance, check your api key or internet connection':
             raise Exception('Failed to check balance, check your api key or internet connection')
@@ -70,10 +73,36 @@
                     print('Failed to send SMS, status code:', response.status_code)
                     return 'Failed to send SMS'
             except ValidationError as e:
                 print(e.json())
                 return f"Failed to send SMS, {e.json()}"
         else:
             return 'You do not have enough balance to send the SMS'
+        
+    def send_innbucks(self, destination_number: str, message: str):
+        '''send InnBucks to a user, destination_number must be of the form 263xxxxxxxxx, message must not exceed 120 characters.'''
+        full_url = self.base_url + '/send_innbucks'
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
+                sms = SMSModel(destination_number=destination_number, message=message)
+                sms_data = sms.dict()
+                response = requests.post(url=full_url, data=sms_data, headers=headers)
+                if response.status_code == 200:
+                    print('Innbucks sent successfully, remaining balance:', response.json()['balance'])
+                    return 'Innbucks sent successfully'
+                else:
+                    print('Failed to send Innbucks, status code:', response.status_code)
+                    return 'Failed to send Innbucks'
+            except ValidationError as e:
+                print(e.json())
+                return f"Failed to send Innbucks, {e.json()}"
```

### Comparing `chromastone-0.1.7/chromastone.egg-info/PKG-INFO` & `chromastone-0.1.8/chromastone.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromastone
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python application for powering other python applications to send SMS messages globally with number validation and restrictions by Tarmica Chiwara
 Home-page: https://github.com/lordskyzw/chromastone
 Author: Tarmica Chiwara
 Author-email: lilskyforever@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chromastone-0.1.7/setup.py` & `chromastone-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='chromastone', 
-    version='0.1.7',
+    version='0.1.8',
     author='Tarmica Chiwara',  
     author_email='lilskyforever@gmail.com',  
     description='A Python application for powering other python applications to send SMS messages globally with number validation and restrictions by Tarmica Chiwara',
     long_description=open('readme.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/lordskyzw/chromastone', 
     packages=find_packages(),
```

