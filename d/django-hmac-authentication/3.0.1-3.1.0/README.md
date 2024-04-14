# Comparing `tmp/django_hmac_authentication-3.0.1.tar.gz` & `tmp/django_hmac_authentication-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_hmac_authentication-3.0.1.tar", last modified: Mon Jan 22 01:54:24 2024, max compression
+gzip compressed data, was "django_hmac_authentication-3.1.0.tar", last modified: Sun Apr 14 00:05:14 2024, max compression
```

## Comparing `django_hmac_authentication-3.0.1.tar` & `django_hmac_authentication-3.1.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 01:54:24.920302 django_hmac_authentication-3.0.1/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-04 10:27:36.000000 django_hmac_authentication-3.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9605 2024-01-22 01:54:24.920302 django_hmac_authentication-3.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     8949 2024-01-22 01:41:40.000000 django_hmac_authentication-3.0.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      840 2024-01-22 01:47:29.000000 django_hmac_authentication-3.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-22 01:54:24.920302 django_hmac_authentication-3.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 01:54:24.908302 django_hmac_authentication-3.0.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 01:54:24.916302 django_hmac_authentication-3.0.1/src/django_hmac_authentication/
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-01-22 01:47:29.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1187 2023-12-14 12:51:24.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      455 2023-07-09 03:21:53.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/apps.py
--rw-rw-rw-   0 root         (0) root         (0)     4149 2023-12-14 12:51:24.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)     5293 2023-09-16 08:55:34.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/checks.py
--rw-rw-rw-   0 root         (0) root         (0)     2817 2023-06-04 10:27:36.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/client_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 01:54:24.916302 django_hmac_authentication-3.0.1/src/django_hmac_authentication/crypt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 01:53:42.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/crypt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-12-14 12:51:24.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/crypt/aes.py
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-12-14 12:51:24.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/crypt/camellia.py
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-12-14 12:51:24.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/crypt/settings.py
--rw-rw-rw-   0 root         (0) root         (0)     1664 2023-09-12 04:34:53.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 01:54:24.916302 django_hmac_authentication-3.0.1/src/django_hmac_authentication/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 01:53:42.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 01:54:24.916302 django_hmac_authentication-3.0.1/src/django_hmac_authentication/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 01:53:42.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1282 2023-06-04 10:27:36.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/management/commands/create_hmac_for_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 01:54:24.920302 django_hmac_authentication-3.0.1/src/django_hmac_authentication/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1776 2023-06-04 10:27:36.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      494 2023-06-04 10:27:36.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/migrations/0002_apihmackey_failed_attempts.py
--rw-rw-rw-   0 root         (0) root         (0)      586 2023-06-05 22:40:36.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py
--rw-rw-rw-   0 root         (0) root         (0)      952 2023-09-16 08:55:34.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/migrations/0004_apihmackey_throttle_rate.py
--rw-rw-rw-   0 root         (0) root         (0)      965 2023-12-14 12:51:24.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/migrations/0005_alter_apihmackey_throttle_rate.py
--rw-rw-rw-   0 root         (0) root         (0)      576 2023-12-14 12:51:24.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/migrations/0006_apihmackey_cipher_algorithm.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-01-22 01:53:42.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1916 2023-12-14 12:51:24.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/models.py
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-06-04 10:27:36.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/padding.py
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-06-04 10:27:36.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     4580 2023-12-14 12:51:24.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/server_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2023-09-12 04:34:53.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-08-25 23:45:01.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/signals.py
--rw-rw-rw-   0 root         (0) root         (0)     2466 2023-09-16 08:55:34.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/throttling.py
--rw-rw-rw-   0 root         (0) root         (0)      813 2023-06-04 10:27:36.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 01:54:24.920302 django_hmac_authentication-3.0.1/src/django_hmac_authentication.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9605 2024-01-22 01:54:24.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1829 2024-01-22 01:54:24.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-22 01:54:24.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2024-01-22 01:54:24.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2024-01-22 01:54:24.000000 django_hmac_authentication-3.0.1/src/django_hmac_authentication.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 00:05:14.382516 django_hmac_authentication-3.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2023-06-04 10:27:36.000000 django_hmac_authentication-3.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9605 2024-04-14 00:05:14.382516 django_hmac_authentication-3.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8949 2024-01-22 01:41:40.000000 django_hmac_authentication-3.1.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      840 2024-04-13 23:56:17.000000 django_hmac_authentication-3.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-14 00:05:14.382516 django_hmac_authentication-3.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 00:05:14.370516 django_hmac_authentication-3.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 00:05:14.378516 django_hmac_authentication-3.1.0/src/django_hmac_authentication/
+-rw-rw-rw-   0 root         (0) root         (0)      140 2024-04-13 23:56:17.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1187 2023-12-14 12:51:24.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      455 2023-07-09 03:21:53.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)     4149 2023-12-14 12:51:24.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)     5293 2023-09-16 08:55:34.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/checks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2817 2023-06-04 10:27:36.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/client_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 00:05:14.382516 django_hmac_authentication-3.1.0/src/django_hmac_authentication/crypt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-14 00:04:26.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/crypt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2024-04-13 23:56:17.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/crypt/aes.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-04-13 23:56:17.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/crypt/camellia.py
+-rw-rw-rw-   0 root         (0) root         (0)      192 2024-04-13 23:56:17.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/crypt/padding.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-12-14 12:51:24.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/crypt/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     1664 2023-09-12 04:34:53.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 00:05:14.382516 django_hmac_authentication-3.1.0/src/django_hmac_authentication/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-14 00:04:26.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 00:05:14.382516 django_hmac_authentication-3.1.0/src/django_hmac_authentication/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-14 00:04:26.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2023-06-04 10:27:36.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/management/commands/create_hmac_for_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 00:05:14.382516 django_hmac_authentication-3.1.0/src/django_hmac_authentication/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1776 2023-06-04 10:27:36.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      494 2023-06-04 10:27:36.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/migrations/0002_apihmackey_failed_attempts.py
+-rw-rw-rw-   0 root         (0) root         (0)      586 2023-06-05 22:40:36.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2023-09-16 08:55:34.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/migrations/0004_apihmackey_throttle_rate.py
+-rw-rw-rw-   0 root         (0) root         (0)      965 2023-12-14 12:51:24.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/migrations/0005_alter_apihmackey_throttle_rate.py
+-rw-rw-rw-   0 root         (0) root         (0)      576 2023-12-14 12:51:24.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/migrations/0006_apihmackey_cipher_algorithm.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-14 00:04:26.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1916 2023-12-14 12:51:24.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-06-04 10:27:36.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4580 2023-12-14 12:51:24.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/server_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-09-12 04:34:53.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-08-25 23:45:01.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/signals.py
+-rw-rw-rw-   0 root         (0) root         (0)     2466 2023-09-16 08:55:34.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/throttling.py
+-rw-rw-rw-   0 root         (0) root         (0)      813 2023-06-04 10:27:36.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 00:05:14.382516 django_hmac_authentication-3.1.0/src/django_hmac_authentication.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9605 2024-04-14 00:05:14.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1835 2024-04-14 00:05:14.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 00:05:14.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2024-04-14 00:05:14.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2024-04-14 00:05:14.000000 django_hmac_authentication-3.1.0/src/django_hmac_authentication.egg-info/top_level.txt
```

### Comparing `django_hmac_authentication-3.0.1/LICENSE` & `django_hmac_authentication-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-3.0.1/PKG-INFO` & `django_hmac_authentication-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_hmac_authentication
-Version: 3.0.1
+Version: 3.1.0
 Summary: Django HMAC authentication using shared secret
 Author-email: "Harisankar Krishna Swamy @ Vevde" <harisankar.krishna@outlook.com>
 Project-URL: Homepage, https://github.com/harisankar-krishna-swamy/django_hmac_authentication
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.2
```

### Comparing `django_hmac_authentication-3.0.1/README.md` & `django_hmac_authentication-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-3.0.1/pyproject.toml` & `django_hmac_authentication-3.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["django_hmac_authentication*"]
 namespaces = false
 
 [project]
 name = "django_hmac_authentication"
-version = "3.0.1"
+version = "3.1.0"
 authors = [
   { name="Harisankar Krishna Swamy @ Vevde", email="harisankar.krishna@outlook.com" },
 ]
 description = "Django HMAC authentication using shared secret"
 readme = "README.md"
 requires-python = ">=3.9.2"
 dependencies = [
```

### Comparing `django_hmac_authentication-3.0.1/src/django_hmac_authentication/admin.py` & `django_hmac_authentication-3.1.0/src/django_hmac_authentication/admin.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-3.0.1/src/django_hmac_authentication/authentication.py` & `django_hmac_authentication-3.1.0/src/django_hmac_authentication/authentication.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-3.0.1/src/django_hmac_authentication/checks.py` & `django_hmac_authentication-3.1.0/src/django_hmac_authentication/checks.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-3.0.1/src/django_hmac_authentication/client_utils.py` & `django_hmac_authentication-3.1.0/src/django_hmac_authentication/client_utils.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-3.0.1/src/django_hmac_authentication/crypt/aes.py` & `django_hmac_authentication-3.1.0/src/django_hmac_authentication/crypt/aes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 
-from django_hmac_authentication.padding import pad, unpad
+from django_hmac_authentication.crypt.padding import pad, unpad
 
 block_size = 128
 
 
 def aes_crypt(msg: bytes, key: bytes, iv: bytes, encrypt: bool = True):
     backend = default_backend()
     cipher = Cipher(algorithms.AES(key), modes.CBC(iv), backend=backend)
```

### Comparing `django_hmac_authentication-3.0.1/src/django_hmac_authentication/crypt/camellia.py` & `django_hmac_authentication-3.1.0/src/django_hmac_authentication/crypt/camellia.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 
-from django_hmac_authentication.padding import pad, unpad
+from django_hmac_authentication.crypt.padding import pad, unpad
 
 block_size = 128
 
 
 def camellia_crypt(msg: bytes, key: bytes, iv: bytes, encrypt: bool = True):
     backend = default_backend()
     cipher = Cipher(algorithms.Camellia(key), modes.CBC(iv), backend=backend)
```

### Comparing `django_hmac_authentication-3.0.1/src/django_hmac_authentication/exceptions.py` & `django_hmac_authentication-3.1.0/src/django_hmac_authentication/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-3.0.1/src/django_hmac_authentication/management/commands/create_hmac_for_user.py` & `django_hmac_authentication-3.1.0/src/django_hmac_authentication/management/commands/create_hmac_for_user.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-3.0.1/src/django_hmac_authentication/migrations/0001_initial.py` & `django_hmac_authentication-3.1.0/src/django_hmac_authentication/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-3.0.1/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py` & `django_hmac_authentication-3.1.0/src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-3.0.1/src/django_hmac_authentication/migrations/0004_apihmackey_throttle_rate.py` & `django_hmac_authentication-3.1.0/src/django_hmac_authentication/migrations/0004_apihmackey_throttle_rate.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-3.0.1/src/django_hmac_authentication/migrations/0005_alter_apihmackey_throttle_rate.py` & `django_hmac_authentication-3.1.0/src/django_hmac_authentication/migrations/0005_alter_apihmackey_throttle_rate.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-3.0.1/src/django_hmac_authentication/migrations/0006_apihmackey_cipher_algorithm.py` & `django_hmac_authentication-3.1.0/src/django_hmac_authentication/migrations/0006_apihmackey_cipher_algorithm.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-3.0.1/src/django_hmac_authentication/models.py` & `django_hmac_authentication-3.1.0/src/django_hmac_authentication/models.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-3.0.1/src/django_hmac_authentication/server_utils.py` & `django_hmac_authentication-3.1.0/src/django_hmac_authentication/server_utils.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-3.0.1/src/django_hmac_authentication/settings.py` & `django_hmac_authentication-3.1.0/src/django_hmac_authentication/settings.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-3.0.1/src/django_hmac_authentication/throttling.py` & `django_hmac_authentication-3.1.0/src/django_hmac_authentication/throttling.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-3.0.1/src/django_hmac_authentication/views.py` & `django_hmac_authentication-3.1.0/src/django_hmac_authentication/views.py`

 * *Files identical despite different names*

### Comparing `django_hmac_authentication-3.0.1/src/django_hmac_authentication.egg-info/PKG-INFO` & `django_hmac_authentication-3.1.0/src/django_hmac_authentication.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_hmac_authentication
-Version: 3.0.1
+Version: 3.1.0
 Summary: Django HMAC authentication using shared secret
 Author-email: "Harisankar Krishna Swamy @ Vevde" <harisankar.krishna@outlook.com>
 Project-URL: Homepage, https://github.com/harisankar-krishna-swamy/django_hmac_authentication
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9.2
```

### Comparing `django_hmac_authentication-3.0.1/src/django_hmac_authentication.egg-info/SOURCES.txt` & `django_hmac_authentication-3.1.0/src/django_hmac_authentication.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 src/django_hmac_authentication/admin.py
 src/django_hmac_authentication/apps.py
 src/django_hmac_authentication/authentication.py
 src/django_hmac_authentication/checks.py
 src/django_hmac_authentication/client_utils.py
 src/django_hmac_authentication/exceptions.py
 src/django_hmac_authentication/models.py
-src/django_hmac_authentication/padding.py
 src/django_hmac_authentication/serializers.py
 src/django_hmac_authentication/server_utils.py
 src/django_hmac_authentication/settings.py
 src/django_hmac_authentication/signals.py
 src/django_hmac_authentication/throttling.py
 src/django_hmac_authentication/views.py
 src/django_hmac_authentication.egg-info/PKG-INFO
 src/django_hmac_authentication.egg-info/SOURCES.txt
 src/django_hmac_authentication.egg-info/dependency_links.txt
 src/django_hmac_authentication.egg-info/requires.txt
 src/django_hmac_authentication.egg-info/top_level.txt
 src/django_hmac_authentication/crypt/__init__.py
 src/django_hmac_authentication/crypt/aes.py
 src/django_hmac_authentication/crypt/camellia.py
+src/django_hmac_authentication/crypt/padding.py
 src/django_hmac_authentication/crypt/settings.py
 src/django_hmac_authentication/management/__init__.py
 src/django_hmac_authentication/management/commands/__init__.py
 src/django_hmac_authentication/management/commands/create_hmac_for_user.py
 src/django_hmac_authentication/migrations/0001_initial.py
 src/django_hmac_authentication/migrations/0002_apihmackey_failed_attempts.py
 src/django_hmac_authentication/migrations/0003_apihmackey_expires_at.py
```

