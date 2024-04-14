# Comparing `tmp/pyslth-0.0.2.tar.gz` & `tmp/pyslth-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.0.2.tar", last modified: Sun Apr 14 18:34:43 2024, max compression
+gzip compressed data, was "pyslth-0.0.3.tar", last modified: Sun Apr 14 18:50:47 2024, max compression
```

## Comparing `pyslth-0.0.2.tar` & `pyslth-0.0.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:34:43.496286 pyslth-0.0.2/
--rw-r--r--   0 breno      (501) staff       (20)       59 2024-04-13 21:50:18.000000 pyslth-0.0.2/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-14 18:34:43.496125 pyslth-0.0.2/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:34:43.485700 pyslth-0.0.2/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-14 18:34:43.000000 pyslth-0.0.2/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)      845 2024-04-14 18:34:43.000000 pyslth-0.0.2/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-14 18:34:43.000000 pyslth-0.0.2/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      126 2024-04-14 18:34:43.000000 pyslth-0.0.2/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-14 18:34:43.000000 pyslth-0.0.2/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      118 2024-04-14 17:58:42.000000 pyslth-0.0.2/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-14 18:34:43.496328 pyslth-0.0.2/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-14 18:33:33.000000 pyslth-0.0.2/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:34:43.490697 pyslth-0.0.2/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3610 2024-04-09 12:56:09.000000 pyslth-0.0.2/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6707 2024-04-12 02:17:46.000000 pyslth-0.0.2/slth/components.py
--rw-r--r--   0 breno      (501) staff       (20)     2217 2024-04-13 03:34:53.000000 pyslth-0.0.2/slth/conf.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:34:43.493201 pyslth-0.0.2/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)      168 2024-04-09 12:56:09.000000 pyslth-0.0.2/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     2916 2024-04-09 12:56:09.000000 pyslth-0.0.2/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    16159 2024-04-14 02:11:34.000000 pyslth-0.0.2/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.0.2/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)    21877 2024-04-13 11:26:17.000000 pyslth-0.0.2/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:34:43.494130 pyslth-0.0.2/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.2/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:34:43.494612 pyslth-0.0.2/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.2/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.0.2/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.0.2/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:34:43.495221 pyslth-0.0.2/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.0.2/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3577 2024-04-09 12:56:09.000000 pyslth-0.0.2/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.2/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     5256 2024-04-09 12:56:09.000000 pyslth-0.0.2/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.0.2/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.0.2/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    16142 2024-04-13 11:45:38.000000 pyslth-0.0.2/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-09 12:56:09.000000 pyslth-0.0.2/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:34:43.495563 pyslth-0.0.2/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     8995 2024-04-14 00:29:15.000000 pyslth-0.0.2/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    10955 2024-04-14 10:37:29.000000 pyslth-0.0.2/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    12970 2024-04-12 02:20:59.000000 pyslth-0.0.2/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:34:43.484655 pyslth-0.0.2/slth/static/
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:34:43.495802 pyslth-0.0.2/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.0.2/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.0.2/slth/statistics.py
--rw-r--r--   0 breno      (501) staff       (20)     5356 2024-04-09 12:56:09.000000 pyslth-0.0.2/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      893 2024-04-12 02:07:28.000000 pyslth-0.0.2/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)      940 2024-04-09 12:56:09.000000 pyslth-0.0.2/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     1838 2024-04-13 11:39:20.000000 pyslth-0.0.2/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:50:47.128871 pyslth-0.0.3/
+-rw-r--r--   0 breno      (501) staff       (20)       59 2024-04-13 21:50:18.000000 pyslth-0.0.3/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-14 18:50:47.128670 pyslth-0.0.3/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:50:47.117308 pyslth-0.0.3/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-04-14 18:50:47.000000 pyslth-0.0.3/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)      845 2024-04-14 18:50:47.000000 pyslth-0.0.3/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-04-14 18:50:47.000000 pyslth-0.0.3/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      139 2024-04-14 18:50:47.000000 pyslth-0.0.3/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-04-14 18:50:47.000000 pyslth-0.0.3/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      131 2024-04-14 18:49:27.000000 pyslth-0.0.3/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-04-14 18:50:47.129611 pyslth-0.0.3/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-04-14 18:50:41.000000 pyslth-0.0.3/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:50:47.122110 pyslth-0.0.3/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3610 2024-04-09 12:56:09.000000 pyslth-0.0.3/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6707 2024-04-12 02:17:46.000000 pyslth-0.0.3/slth/components.py
+-rw-r--r--   0 breno      (501) staff       (20)     2217 2024-04-13 03:34:53.000000 pyslth-0.0.3/slth/conf.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:50:47.122651 pyslth-0.0.3/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)      168 2024-04-09 12:56:09.000000 pyslth-0.0.3/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     2916 2024-04-09 12:56:09.000000 pyslth-0.0.3/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    16159 2024-04-14 02:11:34.000000 pyslth-0.0.3/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.0.3/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)    21877 2024-04-13 11:26:17.000000 pyslth-0.0.3/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:50:47.123123 pyslth-0.0.3/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.3/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:50:47.123778 pyslth-0.0.3/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.3/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.0.3/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.0.3/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:50:47.125362 pyslth-0.0.3/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1396 2024-04-09 12:56:09.000000 pyslth-0.0.3/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3577 2024-04-09 12:56:09.000000 pyslth-0.0.3/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.0.3/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     5256 2024-04-09 12:56:09.000000 pyslth-0.0.3/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      394 2024-04-13 09:58:46.000000 pyslth-0.0.3/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-04-09 12:56:09.000000 pyslth-0.0.3/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    16142 2024-04-13 11:45:38.000000 pyslth-0.0.3/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-09 12:56:09.000000 pyslth-0.0.3/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:50:47.125887 pyslth-0.0.3/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     8995 2024-04-14 00:29:15.000000 pyslth-0.0.3/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    10955 2024-04-14 10:37:29.000000 pyslth-0.0.3/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    12970 2024-04-12 02:20:59.000000 pyslth-0.0.3/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:50:47.116387 pyslth-0.0.3/slth/static/
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-04-14 18:50:47.126907 pyslth-0.0.3/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.0.3/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)     6319 2024-04-09 12:56:09.000000 pyslth-0.0.3/slth/statistics.py
+-rw-r--r--   0 breno      (501) staff       (20)     5356 2024-04-09 12:56:09.000000 pyslth-0.0.3/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      893 2024-04-12 02:07:28.000000 pyslth-0.0.3/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)      940 2024-04-09 12:56:09.000000 pyslth-0.0.3/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     1838 2024-04-13 11:39:20.000000 pyslth-0.0.3/slth/views.py
```

### Comparing `pyslth-0.0.2/PKG-INFO` & `pyslth-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.0.2
+Version: 0.0.3
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.0.2/pyslth.egg-info/PKG-INFO` & `pyslth-0.0.3/pyslth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.0.2
+Version: 0.0.3
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.0.2/pyslth.egg-info/SOURCES.txt` & `pyslth-0.0.3/pyslth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.2/setup.py` & `pyslth-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.0.2/slth/__init__.py` & `pyslth-0.0.3/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.2/slth/components.py` & `pyslth-0.0.3/slth/components.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.2/slth/conf.py` & `pyslth-0.0.3/slth/conf.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.2/slth/db/models.py` & `pyslth-0.0.3/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.2/slth/endpoints.py` & `pyslth-0.0.3/slth/endpoints.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.2/slth/forms.py` & `pyslth-0.0.3/slth/forms.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.2/slth/management/commands/integration_test.py` & `pyslth-0.0.3/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.2/slth/management/commands/sync.py` & `pyslth-0.0.3/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.2/slth/migrations/0001_initial.py` & `pyslth-0.0.3/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.2/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.0.3/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.2/slth/models.py` & `pyslth-0.0.3/slth/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.2/slth/permissions.py` & `pyslth-0.0.3/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.2/slth/queryset.py` & `pyslth-0.0.3/slth/queryset.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.2/slth/roles.py` & `pyslth-0.0.3/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.2/slth/selenium/__init__.py` & `pyslth-0.0.3/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.2/slth/selenium/browser.py` & `pyslth-0.0.3/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.2/slth/serializer.py` & `pyslth-0.0.3/slth/serializer.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.2/slth/static/images/logo.svg` & `pyslth-0.0.3/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.2/slth/statistics.py` & `pyslth-0.0.3/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.2/slth/tests.py` & `pyslth-0.0.3/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.2/slth/urls.py` & `pyslth-0.0.3/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.2/slth/utils.py` & `pyslth-0.0.3/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.0.2/slth/views.py` & `pyslth-0.0.3/slth/views.py`

 * *Files identical despite different names*

