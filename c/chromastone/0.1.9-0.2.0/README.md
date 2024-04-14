# Comparing `tmp/chromastone-0.1.9.tar.gz` & `tmp/chromastone-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromastone-0.1.9.tar", last modified: Sun Apr 14 06:52:29 2024, max compression
+gzip compressed data, was "chromastone-0.2.0.tar", last modified: Sun Apr 14 07:03:03 2024, max compression
```

## Comparing `chromastone-0.1.9.tar` & `chromastone-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 06:52:29.109852 chromastone-0.1.9/
--rw-r--r--   0 lordskyzw   (501) staff       (20)     1082 2024-03-29 23:18:58.000000 chromastone-0.1.9/LICENSE
--rw-r--r--   0 lordskyzw   (501) staff       (20)     2595 2024-04-14 06:52:29.109401 chromastone-0.1.9/PKG-INFO
-drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 06:52:29.103586 chromastone-0.1.9/chromastone/
--rw-r--r--   0 lordskyzw   (501) staff       (20)     4719 2024-04-13 21:06:06.000000 chromastone-0.1.9/chromastone/__init__.py
--rw-r--r--   0 lordskyzw   (501) staff       (20)     6585 2024-04-14 06:44:32.000000 chromastone-0.1.9/chromastone/chromastone.py
-drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 06:52:29.108452 chromastone-0.1.9/chromastone.egg-info/
--rw-r--r--   0 lordskyzw   (501) staff       (20)     2595 2024-04-14 06:52:28.000000 chromastone-0.1.9/chromastone.egg-info/PKG-INFO
--rw-r--r--   0 lordskyzw   (501) staff       (20)      241 2024-04-14 06:52:29.000000 chromastone-0.1.9/chromastone.egg-info/SOURCES.txt
--rw-r--r--   0 lordskyzw   (501) staff       (20)        1 2024-04-14 06:52:28.000000 chromastone-0.1.9/chromastone.egg-info/dependency_links.txt
--rw-r--r--   0 lordskyzw   (501) staff       (20)       18 2024-04-14 06:52:28.000000 chromastone-0.1.9/chromastone.egg-info/requires.txt
--rw-r--r--   0 lordskyzw   (501) staff       (20)       12 2024-04-14 06:52:28.000000 chromastone-0.1.9/chromastone.egg-info/top_level.txt
--rw-r--r--   0 lordskyzw   (501) staff       (20)       38 2024-04-14 06:52:29.110093 chromastone-0.1.9/setup.cfg
--rw-r--r--   0 lordskyzw   (501) staff       (20)      795 2024-04-14 06:52:00.000000 chromastone-0.1.9/setup.py
+drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 07:03:03.941292 chromastone-0.2.0/
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     1082 2024-03-29 23:18:58.000000 chromastone-0.2.0/LICENSE
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     2595 2024-04-14 07:03:03.940722 chromastone-0.2.0/PKG-INFO
+drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 07:03:03.935427 chromastone-0.2.0/chromastone/
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     4719 2024-04-13 21:06:06.000000 chromastone-0.2.0/chromastone/__init__.py
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     6551 2024-04-14 07:02:07.000000 chromastone-0.2.0/chromastone/chromastone.py
+drwxr-xr-x   0 lordskyzw   (501) staff       (20)        0 2024-04-14 07:03:03.939821 chromastone-0.2.0/chromastone.egg-info/
+-rw-r--r--   0 lordskyzw   (501) staff       (20)     2595 2024-04-14 07:03:03.000000 chromastone-0.2.0/chromastone.egg-info/PKG-INFO
+-rw-r--r--   0 lordskyzw   (501) staff       (20)      241 2024-04-14 07:03:03.000000 chromastone-0.2.0/chromastone.egg-info/SOURCES.txt
+-rw-r--r--   0 lordskyzw   (501) staff       (20)        1 2024-04-14 07:03:03.000000 chromastone-0.2.0/chromastone.egg-info/dependency_links.txt
+-rw-r--r--   0 lordskyzw   (501) staff       (20)       18 2024-04-14 07:03:03.000000 chromastone-0.2.0/chromastone.egg-info/requires.txt
+-rw-r--r--   0 lordskyzw   (501) staff       (20)       12 2024-04-14 07:03:03.000000 chromastone-0.2.0/chromastone.egg-info/top_level.txt
+-rw-r--r--   0 lordskyzw   (501) staff       (20)       38 2024-04-14 07:03:03.941508 chromastone-0.2.0/setup.cfg
+-rw-r--r--   0 lordskyzw   (501) staff       (20)      795 2024-04-14 07:02:56.000000 chromastone-0.2.0/setup.py
```

### Comparing `chromastone-0.1.9/LICENSE` & `chromastone-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chromastone-0.1.9/PKG-INFO` & `chromastone-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromastone
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python application for powering other python applications to send SMS messages globally with number validation and restrictions by Tarmica Chiwara
 Home-page: https://github.com/lordskyzw/chromastone
 Author: Tarmica Chiwara
 Author-email: lilskyforever@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chromastone-0.1.9/chromastone/__init__.py` & `chromastone-0.2.0/chromastone/__init__.py`

 * *Files identical despite different names*

### Comparing `chromastone-0.1.9/chromastone/chromastone.py` & `chromastone-0.2.0/chromastone/chromastone.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import requests
 from pydantic import BaseModel, ValidationError, validator
 from typing import Optional
 
+
 class SMSModel(BaseModel):
-    # source number is optional because it is not required for sending SMS
     destination_number: str
     message: str
+    source_number: Optional[str] = None
 
     @validator('destination_number')
     def validate_destination_number(cls, v):
         if not v.isdigit():
             raise ValueError('Destination number must contain only digits')
         if len(v) < 10 or len(v) > 15:
             raise ValueError('Destination number length must be between 10 and 15 digits')
```

### Comparing `chromastone-0.1.9/chromastone.egg-info/PKG-INFO` & `chromastone-0.2.0/chromastone.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chromastone
-Version: 0.1.9
+Version: 0.2.0
 Summary: A Python application for powering other python applications to send SMS messages globally with number validation and restrictions by Tarmica Chiwara
 Home-page: https://github.com/lordskyzw/chromastone
 Author: Tarmica Chiwara
 Author-email: lilskyforever@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chromastone-0.1.9/setup.py` & `chromastone-0.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='chromastone', 
-    version='0.1.9',
+    version='0.2.0',
     author='Tarmica Chiwara',  
     author_email='lilskyforever@gmail.com',  
     description='A Python application for powering other python applications to send SMS messages globally with number validation and restrictions by Tarmica Chiwara',
     long_description=open('readme.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/lordskyzw/chromastone', 
     packages=find_packages(),
```

