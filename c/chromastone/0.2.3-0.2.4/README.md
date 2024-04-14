# Comparing `tmp/chromastone-0.2.3.tar.gz` & `tmp/chromastone-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromastone-0.2.3.tar", last modified: Sun Apr 14 11:18:37 2024, max compression
+gzip compressed data, was "chromastone-0.2.4.tar", last modified: Sun Apr 14 11:31:52 2024, max compression
```

## Comparing `chromastone-0.2.3.tar` & `chromastone-0.2.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 11:18:37.474460 chromastone-0.2.3/
--rw-r--r--   0 lordskyzw   (501) staff       (20)     1082 2024-03-29 23:18:58.000000 chromastone-0.2.3/LICENSE
--rw-r--r--   0 lordskyzw   (501) staff       (20)     2595 2024-04-14 11:18:37.473976 chromastone-0.2.3/PKG-INFO
-drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 11:18:37.469704 chromastone-0.2.3/chromastone/
--rw-r--r--   0 lordskyzw   (501) staff       (20)     4768 2024-04-14 11:13:49.000000 chromastone-0.2.3/chromastone/__init__.py
--rw-r--r--   0 lordskyzw   (501) staff       (20)     6600 2024-04-14 11:18:03.000000 chromastone-0.2.3/chromastone/chromastone.py
-drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 11:18:37.473276 chromastone-0.2.3/chromastone.egg-info/
--rw-r--r--   0 lordskyzw   (501) staff       (20)     2595 2024-04-14 11:18:37.000000 chromastone-0.2.3/chromastone.egg-info/PKG-INFO
--rw-r--r--   0 lordskyzw   (501) staff       (20)      241 2024-04-14 11:18:37.000000 chromastone-0.2.3/chromastone.egg-info/SOURCES.txt
--rw-r--r--   0 lordskyzw   (501) staff       (20)        1 2024-04-14 11:18:37.000000 chromastone-0.2.3/chromastone.egg-info/dependency_links.txt
--rw-r--r--   0 lordskyzw   (501) staff       (20)       18 2024-04-14 11:18:37.000000 chromastone-0.2.3/chromastone.egg-info/requires.txt
--rw-r--r--   0 lordskyzw   (501) staff       (20)       12 2024-04-14 11:18:37.000000 chromastone-0.2.3/chromastone.egg-info/top_level.txt
--rw-r--r--   0 lordskyzw   (501) staff       (20)       38 2024-04-14 11:18:37.474679 chromastone-0.2.3/setup.cfg
--rw-r--r--   0 lordskyzw   (501) staff       (20)      795 2024-04-14 11:18:21.000000 chromastone-0.2.3/setup.py
+drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 11:31:52.419134 chromastone-0.2.4/
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     1082 2024-03-29 23:18:58.000000 chromastone-0.2.4/LICENSE
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     2595 2024-04-14 11:31:52.418777 chromastone-0.2.4/PKG-INFO
+drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 11:31:52.413375 chromastone-0.2.4/chromastone/
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     4768 2024-04-14 11:13:49.000000 chromastone-0.2.4/chromastone/__init__.py
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     6611 2024-04-14 11:31:22.000000 chromastone-0.2.4/chromastone/chromastone.py
+drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 11:31:52.418151 chromastone-0.2.4/chromastone.egg-info/
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     2595 2024-04-14 11:31:52.000000 chromastone-0.2.4/chromastone.egg-info/PKG-INFO
+-rw-r--r--   0 lordskyzw   (501) staff       (20)      241 2024-04-14 11:31:52.000000 chromastone-0.2.4/chromastone.egg-info/SOURCES.txt
+-rw-r--r--   0 lordskyzw   (501) staff       (20)        1 2024-04-14 11:31:52.000000 chromastone-0.2.4/chromastone.egg-info/dependency_links.txt
+-rw-r--r--   0 lordskyzw   (501) staff       (20)       18 2024-04-14 11:31:52.000000 chromastone-0.2.4/chromastone.egg-info/requires.txt
+-rw-r--r--   0 lordskyzw   (501) staff       (20)       12 2024-04-14 11:31:52.000000 chromastone-0.2.4/chromastone.egg-info/top_level.txt
+-rw-r--r--   0 lordskyzw   (501) staff       (20)       38 2024-04-14 11:31:52.419256 chromastone-0.2.4/setup.cfg
+-rw-r--r--   0 lordskyzw   (501) staff       (20)      795 2024-04-14 11:31:44.000000 chromastone-0.2.4/setup.py
```

### Comparing `chromastone-0.2.3/LICENSE` & `chromastone-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `chromastone-0.2.3/PKG-INFO` & `chromastone-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromastone
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python application for powering other python applications to send SMS messages globally with number validation and restrictions by Tarmica Chiwara
 Home-page: https://github.com/lordskyzw/chromastone
 Author: Tarmica Chiwara
 Author-email: lilskyforever@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chromastone-0.2.3/chromastone/__init__.py` & `chromastone-0.2.4/chromastone/__init__.py`

 * *Files identical despite different names*

### Comparing `chromastone-0.2.3/chromastone/chromastone.py` & `chromastone-0.2.4/chromastone/chromastone.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
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
```

### Comparing `chromastone-0.2.3/chromastone.egg-info/PKG-INFO` & `chromastone-0.2.4/chromastone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromastone
-Version: 0.2.3
+Version: 0.2.4
 Summary: A Python application for powering other python applications to send SMS messages globally with number validation and restrictions by Tarmica Chiwara
 Home-page: https://github.com/lordskyzw/chromastone
 Author: Tarmica Chiwara
 Author-email: lilskyforever@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chromastone-0.2.3/setup.py` & `chromastone-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='chromastone', 
-    version='0.2.3',
+    version='0.2.4',
     author='Tarmica Chiwara',  
     author_email='lilskyforever@gmail.com',  
     description='A Python application for powering other python applications to send SMS messages globally with number validation and restrictions by Tarmica Chiwara',
     long_description=open('readme.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/lordskyzw/chromastone', 
     packages=find_packages(),
```

