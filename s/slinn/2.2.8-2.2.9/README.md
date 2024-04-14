# Comparing `tmp/slinn-2.2.8.tar.gz` & `tmp/slinn-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slinn-2.2.8.tar", last modified: Thu Apr 11 17:22:14 2024, max compression
+gzip compressed data, was "slinn-2.2.9.tar", last modified: Thu Apr 11 17:29:39 2024, max compression
```

## Comparing `slinn-2.2.8.tar` & `slinn-2.2.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:22:14.387385 slinn-2.2.8/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1052 2024-04-11 12:51:31.000000 slinn-2.2.8/LICENSE
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     6649 2024-04-11 17:22:14.387385 slinn-2.2.8/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     6385 2024-04-11 15:56:10.000000 slinn-2.2.8/README.md
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2024-04-11 17:22:14.387385 slinn-2.2.8/setup.cfg
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      763 2024-04-11 13:09:34.000000 slinn-2.2.8/setup.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:22:14.384052 slinn-2.2.8/slinn/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      579 2024-04-11 12:51:31.000000 slinn-2.2.8/slinn/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     4383 2024-04-07 11:26:11.000000 slinn-2.2.8/slinn/__main__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      349 2024-04-07 20:45:27.000000 slinn-2.2.8/slinn/address.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       58 2024-04-07 11:26:11.000000 slinn-2.2.8/slinn/any_filter.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:22:14.384052 slinn-2.2.8/slinn/default/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       35 2024-03-28 20:36:39.000000 slinn-2.2.8/slinn/default/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)    12696 2024-04-11 12:51:31.000000 slinn-2.2.8/slinn/default/manage.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      261 2024-04-07 20:24:45.000000 slinn-2.2.8/slinn/default/project.json
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      312 2024-04-11 12:51:31.000000 slinn-2.2.8/slinn/dispatcher.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      156 2024-03-28 20:39:01.000000 slinn-2.2.8/slinn/file.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      667 2024-04-07 11:26:11.000000 slinn-2.2.8/slinn/filter.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:22:14.384052 slinn-2.2.8/slinn/guides/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       56 2024-03-28 20:36:39.000000 slinn-2.2.8/slinn/guides/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      586 2024-04-11 16:03:48.000000 slinn-2.2.8/slinn/guides/migration1xx2xx.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      612 2024-04-07 11:26:11.000000 slinn-2.2.8/slinn/http_api_response.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      363 2024-04-07 11:26:11.000000 slinn-2.2.8/slinn/http_json_api_response.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      466 2024-04-07 11:26:11.000000 slinn-2.2.8/slinn/http_json_response.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      183 2024-03-28 20:36:39.000000 slinn-2.2.8/slinn/http_redirect.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      752 2024-04-07 14:32:49.000000 slinn-2.2.8/slinn/http_response.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      251 2024-04-07 11:26:11.000000 slinn-2.2.8/slinn/link_filter.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     3096 2024-04-07 14:32:49.000000 slinn-2.2.8/slinn/request.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     4785 2024-04-11 15:57:31.000000 slinn-2.2.8/slinn/server.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:22:14.384052 slinn-2.2.8/slinn/templates/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       23 2024-03-28 20:36:39.000000 slinn-2.2.8/slinn/templates/__init__.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:22:14.387385 slinn-2.2.8/slinn/templates/example/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      159 2024-03-28 20:36:39.000000 slinn-2.2.8/slinn/templates/example/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      277 2024-03-28 20:36:39.000000 slinn-2.2.8/slinn/templates/example/app.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       22 2024-03-28 20:36:39.000000 slinn-2.2.8/slinn/templates/example/config.json
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:22:14.387385 slinn-2.2.8/slinn/templates/firstrun/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      162 2024-03-28 20:36:39.000000 slinn-2.2.8/slinn/templates/firstrun/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      549 2024-04-11 16:01:12.000000 slinn-2.2.8/slinn/templates/firstrun/app.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       21 2024-03-28 20:36:39.000000 slinn-2.2.8/slinn/templates/firstrun/config.json
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:22:14.387385 slinn-2.2.8/slinn/templates/firstrun/data/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2199 2024-03-28 20:36:39.000000 slinn-2.2.8/slinn/templates/firstrun/data/slinn.html
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      543 2024-03-28 20:36:39.000000 slinn-2.2.8/slinn/templates/firstrun/data/styles.css
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1191 2024-04-07 15:10:25.000000 slinn-2.2.8/slinn/utils.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:22:14.387385 slinn-2.2.8/slinn.egg-info/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     6649 2024-04-11 17:22:14.000000 slinn-2.2.8/slinn.egg-info/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      944 2024-04-11 17:22:14.000000 slinn-2.2.8/slinn.egg-info/SOURCES.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2024-04-11 17:22:14.000000 slinn-2.2.8/slinn.egg-info/dependency_links.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        6 2024-04-11 17:22:14.000000 slinn-2.2.8/slinn.egg-info/top_level.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2024-04-07 11:02:22.000000 slinn-2.2.8/slinn.egg-info/zip-safe
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:29:39.935950 slinn-2.2.9/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1052 2024-04-11 12:51:31.000000 slinn-2.2.9/LICENSE
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     6649 2024-04-11 17:29:39.935950 slinn-2.2.9/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     6385 2024-04-11 15:56:10.000000 slinn-2.2.9/README.md
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2024-04-11 17:29:39.935950 slinn-2.2.9/setup.cfg
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      763 2024-04-11 17:29:22.000000 slinn-2.2.9/setup.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:29:39.935950 slinn-2.2.9/slinn/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      579 2024-04-11 17:28:58.000000 slinn-2.2.9/slinn/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     4383 2024-04-07 11:26:11.000000 slinn-2.2.9/slinn/__main__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      349 2024-04-11 17:28:26.000000 slinn-2.2.9/slinn/address.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       58 2024-04-07 11:26:11.000000 slinn-2.2.9/slinn/any_filter.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:29:39.935950 slinn-2.2.9/slinn/default/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       35 2024-03-28 20:36:39.000000 slinn-2.2.9/slinn/default/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)    12696 2024-04-11 12:51:31.000000 slinn-2.2.9/slinn/default/manage.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      261 2024-04-07 20:24:45.000000 slinn-2.2.9/slinn/default/project.json
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      312 2024-04-11 12:51:31.000000 slinn-2.2.9/slinn/dispatcher.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      156 2024-03-28 20:39:01.000000 slinn-2.2.9/slinn/file.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      667 2024-04-07 11:26:11.000000 slinn-2.2.9/slinn/filter.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:29:39.935950 slinn-2.2.9/slinn/guides/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       56 2024-03-28 20:36:39.000000 slinn-2.2.9/slinn/guides/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      586 2024-04-11 16:03:48.000000 slinn-2.2.9/slinn/guides/migration1xx2xx.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      612 2024-04-07 11:26:11.000000 slinn-2.2.9/slinn/http_api_response.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      363 2024-04-07 11:26:11.000000 slinn-2.2.9/slinn/http_json_api_response.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      466 2024-04-07 11:26:11.000000 slinn-2.2.9/slinn/http_json_response.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      183 2024-03-28 20:36:39.000000 slinn-2.2.9/slinn/http_redirect.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      752 2024-04-07 14:32:49.000000 slinn-2.2.9/slinn/http_response.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      251 2024-04-07 11:26:11.000000 slinn-2.2.9/slinn/link_filter.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     3096 2024-04-07 14:32:49.000000 slinn-2.2.9/slinn/request.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     4785 2024-04-11 15:57:31.000000 slinn-2.2.9/slinn/server.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:29:39.935950 slinn-2.2.9/slinn/templates/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       23 2024-03-28 20:36:39.000000 slinn-2.2.9/slinn/templates/__init__.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:29:39.935950 slinn-2.2.9/slinn/templates/example/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      159 2024-03-28 20:36:39.000000 slinn-2.2.9/slinn/templates/example/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      277 2024-03-28 20:36:39.000000 slinn-2.2.9/slinn/templates/example/app.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       22 2024-03-28 20:36:39.000000 slinn-2.2.9/slinn/templates/example/config.json
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:29:39.935950 slinn-2.2.9/slinn/templates/firstrun/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      162 2024-03-28 20:36:39.000000 slinn-2.2.9/slinn/templates/firstrun/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      549 2024-04-11 16:01:12.000000 slinn-2.2.9/slinn/templates/firstrun/app.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       21 2024-03-28 20:36:39.000000 slinn-2.2.9/slinn/templates/firstrun/config.json
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:29:39.935950 slinn-2.2.9/slinn/templates/firstrun/data/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2199 2024-03-28 20:36:39.000000 slinn-2.2.9/slinn/templates/firstrun/data/slinn.html
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      543 2024-03-28 20:36:39.000000 slinn-2.2.9/slinn/templates/firstrun/data/styles.css
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1191 2024-04-07 15:10:25.000000 slinn-2.2.9/slinn/utils.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-11 17:29:39.935950 slinn-2.2.9/slinn.egg-info/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     6649 2024-04-11 17:29:39.000000 slinn-2.2.9/slinn.egg-info/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      944 2024-04-11 17:29:39.000000 slinn-2.2.9/slinn.egg-info/SOURCES.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2024-04-11 17:29:39.000000 slinn-2.2.9/slinn.egg-info/dependency_links.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        6 2024-04-11 17:29:39.000000 slinn-2.2.9/slinn.egg-info/top_level.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2024-04-07 11:02:22.000000 slinn-2.2.9/slinn.egg-info/zip-safe
```

### Comparing `slinn-2.2.8/LICENSE` & `slinn-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `slinn-2.2.8/PKG-INFO` & `slinn-2.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slinn
-Version: 2.2.8
+Version: 2.2.9
 Summary: A HTTPS and HTTP server framework
 Home-page: https://slinn.miotp.ru/
 Author: Mark Radin
 Author-email: mrybs2@gmail.com
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `slinn-2.2.8/README.md` & `slinn-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `slinn-2.2.8/setup.py` & `slinn-2.2.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     with open('README.md', 'r') as f:
         return f.read()
     
 templates = ['firstrun', 'example']
 
 
 setup(name='slinn',
-      version='2.2.8',
+      version='2.2.9',
       description='A HTTPS and HTTP server framework',
       packages=['slinn', 'slinn.templates', 'slinn.guides'] + ['slinn.templates.' + template for template in templates],
       package_data={'slinn': ['default/*.*']} | {'slinn.templates.' + template: ['data/*.css', 'data/*.html', 'config.json'] for template in templates},
       author='Mark Radin',
       author_email='mrybs2@gmail.com',
       url='https://slinn.miotp.ru/',
       long_description=readme(),
```

### Comparing `slinn-2.2.8/slinn/__init__.py` & `slinn-2.2.9/slinn/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 from slinn.http_api_response import HttpAPIResponse
 from slinn.http_json_response import HttpJSONResponse
 from slinn.http_json_api_response import HttpJSONAPIResponse
 from slinn.server import Server
 from slinn.dispatcher import Dispatcher
 
 
-version = 'Slinn Murega v2.2.8 110424A'
+version = 'Slinn Murega v2.2.9 110424B'
```

### Comparing `slinn-2.2.8/slinn/__main__.py` & `slinn-2.2.9/slinn/__main__.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.8/slinn/default/manage.py` & `slinn-2.2.9/slinn/default/manage.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.8/slinn/filter.py` & `slinn-2.2.9/slinn/filter.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.8/slinn/guides/migration1xx2xx.py` & `slinn-2.2.9/slinn/guides/migration1xx2xx.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.8/slinn/http_api_response.py` & `slinn-2.2.9/slinn/http_api_response.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.8/slinn/http_response.py` & `slinn-2.2.9/slinn/http_response.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.8/slinn/request.py` & `slinn-2.2.9/slinn/request.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.8/slinn/server.py` & `slinn-2.2.9/slinn/server.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.8/slinn/templates/firstrun/app.py` & `slinn-2.2.9/slinn/templates/firstrun/app.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.8/slinn/templates/firstrun/data/slinn.html` & `slinn-2.2.9/slinn/templates/firstrun/data/slinn.html`

 * *Files identical despite different names*

### Comparing `slinn-2.2.8/slinn/templates/firstrun/data/styles.css` & `slinn-2.2.9/slinn/templates/firstrun/data/styles.css`

 * *Files identical despite different names*

### Comparing `slinn-2.2.8/slinn/utils.py` & `slinn-2.2.9/slinn/utils.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.8/slinn.egg-info/PKG-INFO` & `slinn-2.2.9/slinn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slinn
-Version: 2.2.8
+Version: 2.2.9
 Summary: A HTTPS and HTTP server framework
 Home-page: https://slinn.miotp.ru/
 Author: Mark Radin
 Author-email: mrybs2@gmail.com
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `slinn-2.2.8/slinn.egg-info/SOURCES.txt` & `slinn-2.2.9/slinn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

