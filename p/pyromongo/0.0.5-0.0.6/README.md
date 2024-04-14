# Comparing `tmp/pyromongo-0.0.5.tar.gz` & `tmp/pyromongo-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyromongo-0.0.5.tar", last modified: Tue May 30 10:29:04 2023, max compression
+gzip compressed data, was "pyromongo-0.0.6.tar", last modified: Sun Apr 14 06:04:37 2024, max compression
```

## Comparing `pyromongo-0.0.5.tar` & `pyromongo-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwx------   0 u0_a268  (10268) u0_a268  (10268)        0 2023-05-30 10:29:04.051613 pyromongo-0.0.5/
--rw-------   0 u0_a268  (10268) u0_a268  (10268)     1070 2023-05-28 06:21:34.000000 pyromongo-0.0.5/LICENSE
--rw-------   0 u0_a268  (10268) u0_a268  (10268)     2252 2023-05-30 10:29:04.051613 pyromongo-0.0.5/PKG-INFO
--rw-------   0 u0_a268  (10268) u0_a268  (10268)     1271 2023-05-28 07:10:04.000000 pyromongo-0.0.5/README.md
-drwx------   0 u0_a268  (10268) u0_a268  (10268)        0 2023-05-30 10:29:04.051613 pyromongo-0.0.5/pyromongo/
--rw-------   0 u0_a268  (10268) u0_a268  (10268)     4950 2023-05-24 14:19:41.000000 pyromongo-0.0.5/pyromongo/__init__.py
-drwx------   0 u0_a268  (10268) u0_a268  (10268)        0 2023-05-30 10:29:04.051613 pyromongo-0.0.5/pyromongo.egg-info/
--rw-------   0 u0_a268  (10268) u0_a268  (10268)     2252 2023-05-30 10:29:03.000000 pyromongo-0.0.5/pyromongo.egg-info/PKG-INFO
--rw-------   0 u0_a268  (10268) u0_a268  (10268)      212 2023-05-30 10:29:03.000000 pyromongo-0.0.5/pyromongo.egg-info/SOURCES.txt
--rw-------   0 u0_a268  (10268) u0_a268  (10268)        1 2023-05-30 10:29:03.000000 pyromongo-0.0.5/pyromongo.egg-info/dependency_links.txt
--rw-------   0 u0_a268  (10268) u0_a268  (10268)      179 2023-05-30 10:29:03.000000 pyromongo-0.0.5/pyromongo.egg-info/requires.txt
--rw-------   0 u0_a268  (10268) u0_a268  (10268)       10 2023-05-30 10:29:03.000000 pyromongo-0.0.5/pyromongo.egg-info/top_level.txt
--rw-------   0 u0_a268  (10268) u0_a268  (10268)       38 2023-05-30 10:29:04.051613 pyromongo-0.0.5/setup.cfg
--rw-------   0 u0_a268  (10268) u0_a268  (10268)     1426 2023-05-30 10:26:46.000000 pyromongo-0.0.5/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-14 06:04:37.120772 pyromongo-0.0.6/
+-rw-r--r--   0 user      (1000) user      (1000)     1070 2024-04-14 05:14:58.000000 pyromongo-0.0.6/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)     2303 2024-04-14 06:04:37.120772 pyromongo-0.0.6/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     1271 2024-04-14 05:14:58.000000 pyromongo-0.0.6/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-14 06:04:37.120772 pyromongo-0.0.6/pyromongo/
+-rw-r--r--   0 user      (1000) user      (1000)     4950 2024-04-14 05:14:58.000000 pyromongo-0.0.6/pyromongo/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-14 06:04:37.120772 pyromongo-0.0.6/pyromongo.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     2303 2024-04-14 06:04:37.000000 pyromongo-0.0.6/pyromongo.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      212 2024-04-14 06:04:37.000000 pyromongo-0.0.6/pyromongo.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-04-14 06:04:37.000000 pyromongo-0.0.6/pyromongo.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)      179 2024-04-14 06:04:37.000000 pyromongo-0.0.6/pyromongo.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       10 2024-04-14 06:04:37.000000 pyromongo-0.0.6/pyromongo.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2024-04-14 06:04:37.120772 pyromongo-0.0.6/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     1476 2024-04-14 06:04:07.000000 pyromongo-0.0.6/setup.py
```

### Comparing `pyromongo-0.0.5/LICENSE` & `pyromongo-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyromongo-0.0.5/PKG-INFO` & `pyromongo-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pyromongo
-Version: 0.0.5
+Version: 0.0.6
 Summary: Mongo Session Storage for pyrogram
 Home-page: https://github.com/animeshxd/pyromongo
 Author: Animesh Murmu
 Author-email: am2646374@gmail.com
 License: MIT
 Keywords: async mongo session storage pyrogram
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: encryption
```

### Comparing `pyromongo-0.0.5/README.md` & `pyromongo-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyromongo-0.0.5/pyromongo/__init__.py` & `pyromongo-0.0.6/pyromongo/__init__.py`

 * *Files identical despite different names*

### Comparing `pyromongo-0.0.5/pyromongo.egg-info/PKG-INFO` & `pyromongo-0.0.6/pyromongo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: pyromongo
-Version: 0.0.5
+Version: 0.0.6
 Summary: Mongo Session Storage for pyrogram
 Home-page: https://github.com/animeshxd/pyromongo
 Author: Animesh Murmu
 Author-email: am2646374@gmail.com
 License: MIT
 Keywords: async mongo session storage pyrogram
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: encryption
```

### Comparing `pyromongo-0.0.5/setup.py` & `pyromongo-0.0.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 with open("requirements.txt", encoding="utf-8") as r:
     requires = [i.strip() for i in r]
 
 setup(
     name="pyromongo",
-    version="0.0.5",
+    version="0.0.6",
     description="Mongo Session Storage for pyrogram",
     long_description=readme,
     long_description_content_type="text/markdown",
 
     packages=["pyromongo"],
 
     url="https://github.com/animeshxd/pyromongo",
@@ -21,14 +21,15 @@
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Unix",
         "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python",
     ],
 
     keywords="async mongo session storage pyrogram",
```

