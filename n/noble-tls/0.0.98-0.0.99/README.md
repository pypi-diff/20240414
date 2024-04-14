# Comparing `tmp/noble_tls-0.0.98.tar.gz` & `tmp/noble_tls-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noble_tls-0.0.98.tar", last modified: Wed Jan 10 10:26:38 2024, max compression
+gzip compressed data, was "noble_tls-0.0.99.tar", last modified: Wed Jan 10 10:33:37 2024, max compression
```

## Comparing `noble_tls-0.0.98.tar` & `noble_tls-0.0.99.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-10 10:26:38.402100 noble_tls-0.0.98/
--rw-r--r--   0 runner     (501) staff       (20)     1070 2024-01-10 10:26:29.000000 noble_tls-0.0.98/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)     7125 2024-01-10 10:26:38.401666 noble_tls-0.0.98/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     6466 2024-01-10 10:26:29.000000 noble_tls-0.0.98/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-10 10:26:38.391821 noble_tls-0.0.98/noble_tls/
--rw-r--r--   0 runner     (501) staff       (20)      490 2024-01-10 10:26:29.000000 noble_tls-0.0.98/noble_tls/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      159 2024-01-10 10:26:29.000000 noble_tls-0.0.98/noble_tls/__version__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-10 10:26:38.394170 noble_tls-0.0.98/noble_tls/c/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-01-10 10:26:29.000000 noble_tls-0.0.98/noble_tls/c/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2994 2024-01-10 10:26:29.000000 noble_tls-0.0.98/noble_tls/c/cffi.py
--rw-r--r--   0 runner     (501) staff       (20)    15419 2024-01-10 10:26:29.000000 noble_tls-0.0.98/noble_tls/cookies.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-10 10:26:38.394849 noble_tls-0.0.98/noble_tls/exceptions/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-01-10 10:26:29.000000 noble_tls-0.0.98/noble_tls/exceptions/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       79 2024-01-10 10:26:29.000000 noble_tls-0.0.98/noble_tls/exceptions/exceptions.py
--rw-r--r--   0 runner     (501) staff       (20)     2354 2024-01-10 10:26:29.000000 noble_tls-0.0.98/noble_tls/response.py
--rw-r--r--   0 runner     (501) staff       (20)    18093 2024-01-10 10:26:29.000000 noble_tls-0.0.98/noble_tls/sessions.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-10 10:26:38.397679 noble_tls-0.0.98/noble_tls/tests/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-01-10 10:26:29.000000 noble_tls-0.0.98/noble_tls/tests/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2664 2024-01-10 10:26:29.000000 noble_tls-0.0.98/noble_tls/tests/test_asset.py
--rw-r--r--   0 runner     (501) staff       (20)     2404 2024-01-10 10:26:29.000000 noble_tls-0.0.98/noble_tls/tests/test_cffi.py
--rw-r--r--   0 runner     (501) staff       (20)      310 2024-01-10 10:26:29.000000 noble_tls-0.0.98/noble_tls/tests/test_exceptions.py
--rw-r--r--   0 runner     (501) staff       (20)     2362 2024-01-10 10:26:29.000000 noble_tls-0.0.98/noble_tls/tests/test_file_fetch.py
--rw-r--r--   0 runner     (501) staff       (20)     1821 2024-01-10 10:26:29.000000 noble_tls-0.0.98/noble_tls/tests/test_response.py
--rw-r--r--   0 runner     (501) staff       (20)     1683 2024-01-10 10:26:29.000000 noble_tls-0.0.98/noble_tls/tests/test_sessions.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-10 10:26:38.398383 noble_tls-0.0.98/noble_tls/updater/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-01-10 10:26:29.000000 noble_tls-0.0.98/noble_tls/updater/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4099 2024-01-10 10:26:29.000000 noble_tls-0.0.98/noble_tls/updater/file_fetch.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-10 10:26:38.400447 noble_tls-0.0.98/noble_tls/utils/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-01-10 10:26:29.000000 noble_tls-0.0.98/noble_tls/utils/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2261 2024-01-10 10:26:29.000000 noble_tls-0.0.98/noble_tls/utils/asset.py
--rw-r--r--   0 runner     (501) staff       (20)     1972 2024-01-10 10:26:29.000000 noble_tls-0.0.98/noble_tls/utils/identifiers.py
--rw-r--r--   0 runner     (501) staff       (20)       74 2024-01-10 10:26:29.000000 noble_tls-0.0.98/noble_tls/utils/session_utils.py
--rw-r--r--   0 runner     (501) staff       (20)     2443 2024-01-10 10:26:29.000000 noble_tls-0.0.98/noble_tls/utils/structures.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-10 10:26:38.401209 noble_tls-0.0.98/noble_tls.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     7125 2024-01-10 10:26:38.000000 noble_tls-0.0.98/noble_tls.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)      814 2024-01-10 10:26:38.000000 noble_tls-0.0.98/noble_tls.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-01-10 10:26:38.000000 noble_tls-0.0.98/noble_tls.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       10 2024-01-10 10:26:38.000000 noble_tls-0.0.98/noble_tls.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-01-10 10:26:38.402188 noble_tls-0.0.98/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)     1111 2024-01-10 10:26:29.000000 noble_tls-0.0.98/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-10 10:33:37.109127 noble_tls-0.0.99/
+-rw-r--r--   0 runner     (501) staff       (20)     1070 2024-01-10 10:33:19.000000 noble_tls-0.0.99/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)     7177 2024-01-10 10:33:37.108501 noble_tls-0.0.99/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     6466 2024-01-10 10:33:19.000000 noble_tls-0.0.99/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-10 10:33:37.094048 noble_tls-0.0.99/noble_tls/
+-rw-r--r--   0 runner     (501) staff       (20)      490 2024-01-10 10:33:19.000000 noble_tls-0.0.99/noble_tls/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      159 2024-01-10 10:33:19.000000 noble_tls-0.0.99/noble_tls/__version__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-10 10:33:37.098727 noble_tls-0.0.99/noble_tls/c/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-01-10 10:33:19.000000 noble_tls-0.0.99/noble_tls/c/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2994 2024-01-10 10:33:19.000000 noble_tls-0.0.99/noble_tls/c/cffi.py
+-rw-r--r--   0 runner     (501) staff       (20)    15419 2024-01-10 10:33:19.000000 noble_tls-0.0.99/noble_tls/cookies.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-10 10:33:37.099605 noble_tls-0.0.99/noble_tls/exceptions/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-01-10 10:33:19.000000 noble_tls-0.0.99/noble_tls/exceptions/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       79 2024-01-10 10:33:19.000000 noble_tls-0.0.99/noble_tls/exceptions/exceptions.py
+-rw-r--r--   0 runner     (501) staff       (20)     2354 2024-01-10 10:33:19.000000 noble_tls-0.0.99/noble_tls/response.py
+-rw-r--r--   0 runner     (501) staff       (20)    18093 2024-01-10 10:33:19.000000 noble_tls-0.0.99/noble_tls/sessions.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-10 10:33:37.103555 noble_tls-0.0.99/noble_tls/tests/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-01-10 10:33:19.000000 noble_tls-0.0.99/noble_tls/tests/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2664 2024-01-10 10:33:19.000000 noble_tls-0.0.99/noble_tls/tests/test_asset.py
+-rw-r--r--   0 runner     (501) staff       (20)     2404 2024-01-10 10:33:19.000000 noble_tls-0.0.99/noble_tls/tests/test_cffi.py
+-rw-r--r--   0 runner     (501) staff       (20)      310 2024-01-10 10:33:19.000000 noble_tls-0.0.99/noble_tls/tests/test_exceptions.py
+-rw-r--r--   0 runner     (501) staff       (20)     2362 2024-01-10 10:33:19.000000 noble_tls-0.0.99/noble_tls/tests/test_file_fetch.py
+-rw-r--r--   0 runner     (501) staff       (20)     1821 2024-01-10 10:33:19.000000 noble_tls-0.0.99/noble_tls/tests/test_response.py
+-rw-r--r--   0 runner     (501) staff       (20)     1683 2024-01-10 10:33:19.000000 noble_tls-0.0.99/noble_tls/tests/test_sessions.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-10 10:33:37.104492 noble_tls-0.0.99/noble_tls/updater/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-01-10 10:33:19.000000 noble_tls-0.0.99/noble_tls/updater/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4099 2024-01-10 10:33:19.000000 noble_tls-0.0.99/noble_tls/updater/file_fetch.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-10 10:33:37.107224 noble_tls-0.0.99/noble_tls/utils/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-01-10 10:33:19.000000 noble_tls-0.0.99/noble_tls/utils/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2261 2024-01-10 10:33:19.000000 noble_tls-0.0.99/noble_tls/utils/asset.py
+-rw-r--r--   0 runner     (501) staff       (20)     1972 2024-01-10 10:33:19.000000 noble_tls-0.0.99/noble_tls/utils/identifiers.py
+-rw-r--r--   0 runner     (501) staff       (20)       74 2024-01-10 10:33:19.000000 noble_tls-0.0.99/noble_tls/utils/session_utils.py
+-rw-r--r--   0 runner     (501) staff       (20)     2443 2024-01-10 10:33:19.000000 noble_tls-0.0.99/noble_tls/utils/structures.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-01-10 10:33:37.107866 noble_tls-0.0.99/noble_tls.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     7177 2024-01-10 10:33:37.000000 noble_tls-0.0.99/noble_tls.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)      814 2024-01-10 10:33:37.000000 noble_tls-0.0.99/noble_tls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-01-10 10:33:37.000000 noble_tls-0.0.99/noble_tls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       10 2024-01-10 10:33:37.000000 noble_tls-0.0.99/noble_tls.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-01-10 10:33:37.109243 noble_tls-0.0.99/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)     1157 2024-01-10 10:33:19.000000 noble_tls-0.0.99/setup.py
```

### Comparing `noble_tls-0.0.98/LICENSE` & `noble_tls-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `noble_tls-0.0.98/PKG-INFO` & `noble_tls-0.0.99/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: noble_tls
-Version: 0.0.98
+Version: 0.0.99
 Summary: Advanced TLS/SSL wrapper for Python
 Author: Rawand Ahmed Shaswar
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
+Requires: httpx
+Requires: distro
+Requires: requests
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🔥 Noble TLS
 
 [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-310/)
```

### Comparing `noble_tls-0.0.98/README.md` & `noble_tls-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `noble_tls-0.0.98/noble_tls/c/cffi.py` & `noble_tls-0.0.99/noble_tls/c/cffi.py`

 * *Files identical despite different names*

### Comparing `noble_tls-0.0.98/noble_tls/cookies.py` & `noble_tls-0.0.99/noble_tls/cookies.py`

 * *Files identical despite different names*

### Comparing `noble_tls-0.0.98/noble_tls/response.py` & `noble_tls-0.0.99/noble_tls/response.py`

 * *Files identical despite different names*

### Comparing `noble_tls-0.0.98/noble_tls/sessions.py` & `noble_tls-0.0.99/noble_tls/sessions.py`

 * *Files identical despite different names*

### Comparing `noble_tls-0.0.98/noble_tls/tests/test_asset.py` & `noble_tls-0.0.99/noble_tls/tests/test_asset.py`

 * *Files identical despite different names*

### Comparing `noble_tls-0.0.98/noble_tls/tests/test_cffi.py` & `noble_tls-0.0.99/noble_tls/tests/test_cffi.py`

 * *Files identical despite different names*

### Comparing `noble_tls-0.0.98/noble_tls/tests/test_file_fetch.py` & `noble_tls-0.0.99/noble_tls/tests/test_file_fetch.py`

 * *Files identical despite different names*

### Comparing `noble_tls-0.0.98/noble_tls/tests/test_response.py` & `noble_tls-0.0.99/noble_tls/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `noble_tls-0.0.98/noble_tls/tests/test_sessions.py` & `noble_tls-0.0.99/noble_tls/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `noble_tls-0.0.98/noble_tls/updater/file_fetch.py` & `noble_tls-0.0.99/noble_tls/updater/file_fetch.py`

 * *Files identical despite different names*

### Comparing `noble_tls-0.0.98/noble_tls/utils/asset.py` & `noble_tls-0.0.99/noble_tls/utils/asset.py`

 * *Files identical despite different names*

### Comparing `noble_tls-0.0.98/noble_tls/utils/identifiers.py` & `noble_tls-0.0.99/noble_tls/utils/identifiers.py`

 * *Files identical despite different names*

### Comparing `noble_tls-0.0.98/noble_tls/utils/structures.py` & `noble_tls-0.0.99/noble_tls/utils/structures.py`

 * *Files identical despite different names*

### Comparing `noble_tls-0.0.98/noble_tls.egg-info/PKG-INFO` & `noble_tls-0.0.99/noble_tls.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: noble_tls
-Version: 0.0.98
+Version: 0.0.99
 Summary: Advanced TLS/SSL wrapper for Python
 Author: Rawand Ahmed Shaswar
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries
+Requires: httpx
+Requires: distro
+Requires: requests
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # 🔥 Noble TLS
 
 [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-310/)
```

### Comparing `noble_tls-0.0.98/noble_tls.egg-info/SOURCES.txt` & `noble_tls-0.0.99/noble_tls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `noble_tls-0.0.98/setup.py` & `noble_tls-0.0.99/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     version=about["__version__"],
     author=about["__author__"],
     description=about["__description__"],
     license=about["__license__"],
     long_description=readme,
     long_description_content_type="text/markdown",
     packages=find_packages(exclude=["tests"]),
+    requires=["httpx", "distro", "requests"],
     classifiers=[
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

