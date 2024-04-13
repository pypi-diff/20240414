# Comparing `tmp/easyencryption-0.2.0.1.tar.gz` & `tmp/easyencryption-0.2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyencryption-0.2.0.1.tar", last modified: Sat Apr 13 12:25:32 2024, max compression
+gzip compressed data, was "easyencryption-0.2.0.2.tar", last modified: Sat Apr 13 12:38:28 2024, max compression
```

## Comparing `easyencryption-0.2.0.1.tar` & `easyencryption-0.2.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:25:32.741778 easyencryption-0.2.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-13 12:25:32.741778 easyencryption-0.2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-13 12:25:32.741778 easyencryption-0.2.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:25:32.737778 easyencryption-0.2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:25:32.737778 easyencryption-0.2.0.1/src/easyencryption/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/src/easyencryption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/src/easyencryption/aes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/src/easyencryption/ascii.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/src/easyencryption/blake.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/src/easyencryption/ecc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/src/easyencryption/fernet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/src/easyencryption/rsa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/src/easyencryption/sha.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/src/easyencryption/shake.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/src/easyencryption/test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-13 12:25:24.000000 easyencryption-0.2.0.1/src/easyencryption/xor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:25:32.741778 easyencryption-0.2.0.1/src/easyencryption.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-13 12:25:32.000000 easyencryption-0.2.0.1/src/easyencryption.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-13 12:25:32.000000 easyencryption-0.2.0.1/src/easyencryption.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 12:25:32.000000 easyencryption-0.2.0.1/src/easyencryption.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-13 12:25:32.000000 easyencryption-0.2.0.1/src/easyencryption.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 12:25:32.000000 easyencryption-0.2.0.1/src/easyencryption.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:38:28.131899 easyencryption-0.2.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-13 12:38:28.131899 easyencryption-0.2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-13 12:38:24.000000 easyencryption-0.2.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-13 12:38:28.131899 easyencryption-0.2.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-13 12:38:24.000000 easyencryption-0.2.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:38:28.127899 easyencryption-0.2.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:38:28.131899 easyencryption-0.2.0.2/src/easyencryption/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-13 12:38:24.000000 easyencryption-0.2.0.2/src/easyencryption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-13 12:38:24.000000 easyencryption-0.2.0.2/src/easyencryption/aes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-13 12:38:24.000000 easyencryption-0.2.0.2/src/easyencryption/ascii.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-13 12:38:24.000000 easyencryption-0.2.0.2/src/easyencryption/blake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-13 12:38:24.000000 easyencryption-0.2.0.2/src/easyencryption/ecc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-13 12:38:24.000000 easyencryption-0.2.0.2/src/easyencryption/fernet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-13 12:38:24.000000 easyencryption-0.2.0.2/src/easyencryption/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2037 2024-04-13 12:38:24.000000 easyencryption-0.2.0.2/src/easyencryption/sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-13 12:38:24.000000 easyencryption-0.2.0.2/src/easyencryption/shake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-13 12:38:24.000000 easyencryption-0.2.0.2/src/easyencryption/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-13 12:38:24.000000 easyencryption-0.2.0.2/src/easyencryption/xor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 12:38:28.131899 easyencryption-0.2.0.2/src/easyencryption.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-04-13 12:38:28.000000 easyencryption-0.2.0.2/src/easyencryption.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-13 12:38:28.000000 easyencryption-0.2.0.2/src/easyencryption.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 12:38:28.000000 easyencryption-0.2.0.2/src/easyencryption.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-13 12:38:28.000000 easyencryption-0.2.0.2/src/easyencryption.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 12:38:28.000000 easyencryption-0.2.0.2/src/easyencryption.egg-info/top_level.txt
```

### Comparing `easyencryption-0.2.0.1/PKG-INFO` & `easyencryption-0.2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.2.0.1
+Version: 0.2.0.2
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: setuptools>=42
 Requires-Dist: cryptography
 Requires-Dist: pycryptodomex
 Requires-Dist: pycryptodome
 Requires-Dist: wheel
 Requires-Dist: eciespy
```

### Comparing `easyencryption-0.2.0.1/README.md` & `easyencryption-0.2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `easyencryption-0.2.0.1/setup.cfg` & `easyencryption-0.2.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `easyencryption-0.2.0.1/setup.py` & `easyencryption-0.2.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_desc = open("README.md", "r")
 long_description = long_desc.read()
-version = "0.2.0.1"
+version = "0.2.0.2"
 
 setup(
     name='easyencryption',
     version=version,
     description='A very easy way to encrypt data.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     url='https://github.com/BlazenBoi/easyencryption/issues',
     author='Blazen',
     author_email='contact@fireballbot.com',
     keywords='',
     packages=find_packages(include=['easyencryption']),
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     install_requires=[
     "setuptools>=42",
     "cryptography",
     "pycryptodomex",
     "pycryptodome",
     "wheel",
     "eciespy",
```

### Comparing `easyencryption-0.2.0.1/src/easyencryption/__init__.py` & `easyencryption-0.2.0.2/src/easyencryption/__init__.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.2.0.1/src/easyencryption/aes.py` & `easyencryption-0.2.0.2/src/easyencryption/aes.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.2.0.1/src/easyencryption/ascii.py` & `easyencryption-0.2.0.2/src/easyencryption/ascii.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.2.0.1/src/easyencryption/blake.py` & `easyencryption-0.2.0.2/src/easyencryption/blake.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.2.0.1/src/easyencryption/ecc.py` & `easyencryption-0.2.0.2/src/easyencryption/ecc.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.2.0.1/src/easyencryption/fernet.py` & `easyencryption-0.2.0.2/src/easyencryption/fernet.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.2.0.1/src/easyencryption/rsa.py` & `easyencryption-0.2.0.2/src/easyencryption/rsa.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.2.0.1/src/easyencryption/sha.py` & `easyencryption-0.2.0.2/src/easyencryption/sha.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.2.0.1/src/easyencryption/shake.py` & `easyencryption-0.2.0.2/src/easyencryption/shake.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.2.0.1/src/easyencryption/test_all.py` & `easyencryption-0.2.0.2/src/easyencryption/test_all.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.2.0.1/src/easyencryption/xor.py` & `easyencryption-0.2.0.2/src/easyencryption/xor.py`

 * *Files identical despite different names*

### Comparing `easyencryption-0.2.0.1/src/easyencryption.egg-info/PKG-INFO` & `easyencryption-0.2.0.2/src/easyencryption.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyencryption
-Version: 0.2.0.1
+Version: 0.2.0.2
 Summary: A very easy way to encrypt data.
 Home-page: https://github.com/BlazenBoi/easyencryption/issues
 Author: Blazen
 Author-email: contact@fireballbot.com
 License: MIT
 Project-URL: Discord Server, https://discord.com/invite/mPU3HybBs9
 Project-URL: Bug Tracker, https://github.com/BlazenBoi/easyencryption/issues
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: setuptools>=42
 Requires-Dist: cryptography
 Requires-Dist: pycryptodomex
 Requires-Dist: pycryptodome
 Requires-Dist: wheel
 Requires-Dist: eciespy
```

### Comparing `easyencryption-0.2.0.1/src/easyencryption.egg-info/SOURCES.txt` & `easyencryption-0.2.0.2/src/easyencryption.egg-info/SOURCES.txt`

 * *Files identical despite different names*

