# Comparing `tmp/headline-gen-2.4.tar.gz` & `tmp/headline-gen-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "headline-gen-2.4.tar", last modified: Sun Apr 14 04:38:18 2024, max compression
+gzip compressed data, was "headline-gen-2.5.tar", last modified: Sun Apr 14 04:45:30 2024, max compression
```

## Comparing `headline-gen-2.4.tar` & `headline-gen-2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:38:18.303922 headline-gen-2.4/
--rw-r--r--   0 root         (0) root         (0)     1817 2024-04-14 04:38:18.303922 headline-gen-2.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1560 2024-04-14 04:32:29.000000 headline-gen-2.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:38:18.301921 headline-gen-2.4/headline_gen/
--rw-r--r--   0 root         (0) root         (0)    13480 2024-04-14 04:03:22.000000 headline-gen-2.4/headline_gen/Control.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 04:02:19.000000 headline-gen-2.4/headline_gen/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:38:18.302922 headline-gen-2.4/headline_gen.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1817 2024-04-14 04:38:18.000000 headline-gen-2.4/headline_gen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      246 2024-04-14 04:38:18.000000 headline-gen-2.4/headline_gen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 04:38:18.000000 headline-gen-2.4/headline_gen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      148 2024-04-14 04:38:18.000000 headline-gen-2.4/headline_gen.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-14 04:38:18.000000 headline-gen-2.4/headline_gen.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-14 04:38:18.303922 headline-gen-2.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      812 2024-04-14 04:37:39.000000 headline-gen-2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:45:30.488473 headline-gen-2.5/
+-rw-r--r--   0 root         (0) root         (0)     1817 2024-04-14 04:45:30.488473 headline-gen-2.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-04-14 04:44:46.000000 headline-gen-2.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:45:30.487473 headline-gen-2.5/headline_gen/
+-rw-r--r--   0 root         (0) root         (0)    13480 2024-04-14 04:03:22.000000 headline-gen-2.5/headline_gen/Control.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 04:02:19.000000 headline-gen-2.5/headline_gen/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:45:30.488473 headline-gen-2.5/headline_gen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1817 2024-04-14 04:45:30.000000 headline-gen-2.5/headline_gen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      246 2024-04-14 04:45:30.000000 headline-gen-2.5/headline_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 04:45:30.000000 headline-gen-2.5/headline_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2024-04-14 04:45:30.000000 headline-gen-2.5/headline_gen.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-14 04:45:30.000000 headline-gen-2.5/headline_gen.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-14 04:45:30.488473 headline-gen-2.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      747 2024-04-14 04:44:17.000000 headline-gen-2.5/setup.py
```

### Comparing `headline-gen-2.4/PKG-INFO` & `headline-gen-2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: headline-gen
-Version: 2.4
+Version: 2.5
 Summary: Provides functionality to generate headlines from articles using natural language processing techniques.
 Author: venkatchoudharyala
 Author-email: venkatchoudhary.ala@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 
@@ -43,13 +43,13 @@
 ## Usage Instructions
 
 1. Import the `ServerCntrl` and `Generate` functions from the `Control` module.
 2. Start the server using `ServerCntrl("Start")`. This only needs to be done once.
 3. Generate headlines using the `Generate` function, passing the article text as an argument.
 4. Stop the server when done using `ServerCntrl("Stop", Server)`.
 
-## New Release Features (v2.4) and Bug Fixes
+## New Release Features (v2.5) and Bug Fixes
 
 1. Fixed a corner case issue causing a ZeroDivisionError when processing irregular parameters for phrase extraction. The package now gracefully handles such scenarios without disrupting functionality.
 2. Renamed the function `ServerInit` to `ServerCntrl` for improved clarity and consistency within the codebase.
 3. Additionally, streamlined the dependency management by directly including `en_core_web_sm` in the downloader module.
 4. Output made more Comprehensive.
```

### Comparing `headline-gen-2.4/README.md` & `headline-gen-2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -34,13 +34,13 @@
 ## Usage Instructions
 
 1. Import the `ServerCntrl` and `Generate` functions from the `Control` module.
 2. Start the server using `ServerCntrl("Start")`. This only needs to be done once.
 3. Generate headlines using the `Generate` function, passing the article text as an argument.
 4. Stop the server when done using `ServerCntrl("Stop", Server)`.
 
-## New Release Features (v2.4) and Bug Fixes
+## New Release Features (v2.5) and Bug Fixes
 
 1. Fixed a corner case issue causing a ZeroDivisionError when processing irregular parameters for phrase extraction. The package now gracefully handles such scenarios without disrupting functionality.
 2. Renamed the function `ServerInit` to `ServerCntrl` for improved clarity and consistency within the codebase.
 3. Additionally, streamlined the dependency management by directly including `en_core_web_sm` in the downloader module.
 4. Output made more Comprehensive.
```

### Comparing `headline-gen-2.4/headline_gen/Control.py` & `headline-gen-2.5/headline_gen/Control.py`

 * *Files identical despite different names*

### Comparing `headline-gen-2.4/headline_gen.egg-info/PKG-INFO` & `headline-gen-2.5/headline_gen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: headline-gen
-Version: 2.4
+Version: 2.5
 Summary: Provides functionality to generate headlines from articles using natural language processing techniques.
 Author: venkatchoudharyala
 Author-email: venkatchoudhary.ala@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 
@@ -43,13 +43,13 @@
 ## Usage Instructions
 
 1. Import the `ServerCntrl` and `Generate` functions from the `Control` module.
 2. Start the server using `ServerCntrl("Start")`. This only needs to be done once.
 3. Generate headlines using the `Generate` function, passing the article text as an argument.
 4. Stop the server when done using `ServerCntrl("Stop", Server)`.
 
-## New Release Features (v2.4) and Bug Fixes
+## New Release Features (v2.5) and Bug Fixes
 
 1. Fixed a corner case issue causing a ZeroDivisionError when processing irregular parameters for phrase extraction. The package now gracefully handles such scenarios without disrupting functionality.
 2. Renamed the function `ServerInit` to `ServerCntrl` for improved clarity and consistency within the codebase.
 3. Additionally, streamlined the dependency management by directly including `en_core_web_sm` in the downloader module.
 4. Output made more Comprehensive.
```

### Comparing `headline-gen-2.4/setup.py` & `headline-gen-2.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name='headline-gen',
-    version='2.4',
+    version='2.5',
     author='venkatchoudharyala',
     author_email='venkatchoudhary.ala@gmail.com',
     description='Provides functionality to generate headlines from articles using natural language processing techniques.',
     long_description=open('README.md').read(),  # Read the contents of README.md
     long_description_content_type='text/markdown',  # Specify the content type of the l
     install_requires=[
-        'requests==2.31.0',
-        'nltk==3.8.1',
-        'numpy==1.26.4',
+        'requests',
+        'nltk',
+        'numpy',
         'scipy==1.12.0',
-        'gensim==4.3.2',
-        'networkx==3.3',
-        'textacy==0.13.0',
-        'transformers==4.39.3',
-        'torch==2.2.2',
-        'spacy==3.7.4'
+        'gensim',
+        'networkx',
+        'textacy',
+        'transformers',
+        'torch',
+        'spacy'
     ],
     python_requires='>=3.6',
 )
```

