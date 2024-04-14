# Comparing `tmp/nacl_middleware-0.0.4.tar.gz` & `tmp/nacl_middleware-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nacl_middleware-0.0.4.tar", last modified: Sun Apr 14 02:26:10 2024, max compression
+gzip compressed data, was "nacl_middleware-0.0.5.tar", last modified: Sun Apr 14 02:38:48 2024, max compression
```

## Comparing `nacl_middleware-0.0.4.tar` & `nacl_middleware-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-14 02:26:10.545922 nacl_middleware-0.0.4/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8627 2024-04-14 02:26:10.545922 nacl_middleware-0.0.4/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7010 2024-04-14 02:25:08.000000 nacl_middleware-0.0.4/README.rst
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-14 02:26:10.545922 nacl_middleware-0.0.4/nacl_middleware/
--rw-r--r--   0 daniel    (1000) daniel    (1000)      113 2024-04-13 19:29:25.000000 nacl_middleware-0.0.4/nacl_middleware/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     5014 2024-04-14 00:46:30.000000 nacl_middleware-0.0.4/nacl_middleware/nacl_middleware.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     2999 2024-04-14 00:46:30.000000 nacl_middleware-0.0.4/nacl_middleware/nacl_utils.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)      570 2024-04-14 00:46:30.000000 nacl_middleware-0.0.4/nacl_middleware/utils.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-14 02:26:10.545922 nacl_middleware-0.0.4/nacl_middleware.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     8627 2024-04-14 02:26:10.000000 nacl_middleware-0.0.4/nacl_middleware.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      358 2024-04-14 02:26:10.000000 nacl_middleware-0.0.4/nacl_middleware.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2024-04-14 02:26:10.000000 nacl_middleware-0.0.4/nacl_middleware.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)      211 2024-04-14 02:26:10.000000 nacl_middleware-0.0.4/nacl_middleware.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       16 2024-04-14 02:26:10.000000 nacl_middleware-0.0.4/nacl_middleware.egg-info/top_level.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1361 2024-04-14 02:26:01.000000 nacl_middleware-0.0.4/pyproject.toml
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2024-04-14 02:26:10.545922 nacl_middleware-0.0.4/setup.cfg
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-14 02:26:10.545922 nacl_middleware-0.0.4/tests/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1698 2024-04-14 00:46:30.000000 nacl_middleware-0.0.4/tests/test_server.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-14 02:38:48.565902 nacl_middleware-0.0.5/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8629 2024-04-14 02:38:48.565902 nacl_middleware-0.0.5/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7012 2024-04-14 02:37:43.000000 nacl_middleware-0.0.5/README.rst
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-14 02:38:48.555902 nacl_middleware-0.0.5/nacl_middleware/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      113 2024-04-13 19:29:25.000000 nacl_middleware-0.0.5/nacl_middleware/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     5014 2024-04-14 00:46:30.000000 nacl_middleware-0.0.5/nacl_middleware/nacl_middleware.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     2999 2024-04-14 00:46:30.000000 nacl_middleware-0.0.5/nacl_middleware/nacl_utils.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      570 2024-04-14 00:46:30.000000 nacl_middleware-0.0.5/nacl_middleware/utils.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-14 02:38:48.565902 nacl_middleware-0.0.5/nacl_middleware.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     8629 2024-04-14 02:38:48.000000 nacl_middleware-0.0.5/nacl_middleware.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      358 2024-04-14 02:38:48.000000 nacl_middleware-0.0.5/nacl_middleware.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2024-04-14 02:38:48.000000 nacl_middleware-0.0.5/nacl_middleware.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      211 2024-04-14 02:38:48.000000 nacl_middleware-0.0.5/nacl_middleware.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       16 2024-04-14 02:38:48.000000 nacl_middleware-0.0.5/nacl_middleware.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1361 2024-04-14 02:38:39.000000 nacl_middleware-0.0.5/pyproject.toml
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2024-04-14 02:38:48.565902 nacl_middleware-0.0.5/setup.cfg
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2024-04-14 02:38:48.565902 nacl_middleware-0.0.5/tests/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1698 2024-04-14 00:46:30.000000 nacl_middleware-0.0.5/tests/test_server.py
```

### Comparing `nacl_middleware-0.0.4/PKG-INFO` & `nacl_middleware-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nacl_middleware
-Version: 0.0.4
+Version: 0.0.5
 Summary: aiohttp compatible pynacl middleware
 License: GNU General Public License v3 or later (GPLv3+)
 Keywords: pynacle,middleware,aiohttp
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -148,15 +148,15 @@
         ], exclude_routes=['/get_public_key'])
 
         async def thanks_handler(request):
             decrypted_message = request['decrypted_message']
             mail_box = request['mail_box']
             if decrypted_message == 'Thank you!':
                 return json_response(mail_box.box('You are welcome!'))
-            return json_response(mail_box.box("Alright!"))
+            return json_response(mail_box.box("Pardon me?"))
 
         app.router.add_get('/handle_thanks', thanks_handler)
 
         async def get_public_key(request):
             decoded_public_key = Nacl(private_key).decodedPublicKey()
             return json_response(decoded_public_key)
```

### Comparing `nacl_middleware-0.0.4/README.rst` & `nacl_middleware-0.0.5/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         ], exclude_routes=['/get_public_key'])
 
         async def thanks_handler(request):
             decrypted_message = request['decrypted_message']
             mail_box = request['mail_box']
             if decrypted_message == 'Thank you!':
                 return json_response(mail_box.box('You are welcome!'))
-            return json_response(mail_box.box("Alright!"))
+            return json_response(mail_box.box("Pardon me?"))
 
         app.router.add_get('/handle_thanks', thanks_handler)
 
         async def get_public_key(request):
             decoded_public_key = Nacl(private_key).decodedPublicKey()
             return json_response(decoded_public_key)
```

### Comparing `nacl_middleware-0.0.4/nacl_middleware/nacl_middleware.py` & `nacl_middleware-0.0.5/nacl_middleware/nacl_middleware.py`

 * *Files identical despite different names*

### Comparing `nacl_middleware-0.0.4/nacl_middleware/nacl_utils.py` & `nacl_middleware-0.0.5/nacl_middleware/nacl_utils.py`

 * *Files identical despite different names*

### Comparing `nacl_middleware-0.0.4/nacl_middleware/utils.py` & `nacl_middleware-0.0.5/nacl_middleware/utils.py`

 * *Files identical despite different names*

### Comparing `nacl_middleware-0.0.4/nacl_middleware.egg-info/PKG-INFO` & `nacl_middleware-0.0.5/nacl_middleware.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nacl_middleware
-Version: 0.0.4
+Version: 0.0.5
 Summary: aiohttp compatible pynacl middleware
 License: GNU General Public License v3 or later (GPLv3+)
 Keywords: pynacle,middleware,aiohttp
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -148,15 +148,15 @@
         ], exclude_routes=['/get_public_key'])
 
         async def thanks_handler(request):
             decrypted_message = request['decrypted_message']
             mail_box = request['mail_box']
             if decrypted_message == 'Thank you!':
                 return json_response(mail_box.box('You are welcome!'))
-            return json_response(mail_box.box("Alright!"))
+            return json_response(mail_box.box("Pardon me?"))
 
         app.router.add_get('/handle_thanks', thanks_handler)
 
         async def get_public_key(request):
             decoded_public_key = Nacl(private_key).decodedPublicKey()
             return json_response(decoded_public_key)
```

### Comparing `nacl_middleware-0.0.4/pyproject.toml` & `nacl_middleware-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Declare the build backend (required)
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools"]
 
 [project]
 name = "nacl_middleware"
-version = "0.0.4"
+version = "0.0.5"
 description = "aiohttp compatible pynacl middleware"
 license = { text = "GNU General Public License v3 or later (GPLv3+)" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Plugins",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
```

### Comparing `nacl_middleware-0.0.4/tests/test_server.py` & `nacl_middleware-0.0.5/tests/test_server.py`

 * *Files identical despite different names*

