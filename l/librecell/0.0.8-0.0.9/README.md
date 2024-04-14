# Comparing `tmp/librecell-0.0.8.tar.gz` & `tmp/librecell-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/librecell-0.0.8.tar", last modified: Wed Dec 30 17:35:43 2020, max compression
+gzip compressed data, was "dist/librecell-0.0.9.tar", last modified: Wed Dec 30 17:45:39 2020, max compression
```

## Comparing `librecell-0.0.8.tar` & `librecell-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:35:43.000000 librecell-0.0.8/
--rw-r--r--   0 kramert   (1000) kramert   (1000)      773 2020-12-30 17:35:43.000000 librecell-0.0.8/PKG-INFO
--rw-r--r--   0 kramert   (1000) kramert   (1000)      168 2019-10-05 16:43:05.000000 librecell-0.0.8/README.md
-drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:35:43.000000 librecell-0.0.8/librecell.egg-info/
--rw-r--r--   0 kramert   (1000) kramert   (1000)      773 2020-12-30 17:35:43.000000 librecell-0.0.8/librecell.egg-info/PKG-INFO
--rw-r--r--   0 kramert   (1000) kramert   (1000)      214 2020-12-30 17:35:43.000000 librecell-0.0.8/librecell.egg-info/SOURCES.txt
--rw-r--r--   0 kramert   (1000) kramert   (1000)        1 2020-12-30 17:35:43.000000 librecell-0.0.8/librecell.egg-info/dependency_links.txt
--rw-r--r--   0 kramert   (1000) kramert   (1000)        1 2020-12-30 09:39:08.000000 librecell-0.0.8/librecell.egg-info/not-zip-safe
--rw-r--r--   0 kramert   (1000) kramert   (1000)       69 2020-12-30 17:35:43.000000 librecell-0.0.8/librecell.egg-info/requires.txt
--rw-r--r--   0 kramert   (1000) kramert   (1000)        1 2020-12-30 17:35:43.000000 librecell-0.0.8/librecell.egg-info/top_level.txt
--rw-r--r--   0 kramert   (1000) kramert   (1000)       38 2020-12-30 17:35:43.000000 librecell-0.0.8/setup.cfg
--rw-r--r--   0 kramert   (1000) kramert   (1000)      924 2020-12-30 17:34:52.000000 librecell-0.0.8/setup.py
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:45:39.000000 librecell-0.0.9/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      773 2020-12-30 17:45:39.000000 librecell-0.0.9/PKG-INFO
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      168 2019-10-05 16:43:05.000000 librecell-0.0.9/README.md
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:45:39.000000 librecell-0.0.9/librecell.egg-info/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      773 2020-12-30 17:45:39.000000 librecell-0.0.9/librecell.egg-info/PKG-INFO
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      214 2020-12-30 17:45:39.000000 librecell-0.0.9/librecell.egg-info/SOURCES.txt
+-rw-r--r--   0 kramert   (1000) kramert   (1000)        1 2020-12-30 17:45:39.000000 librecell-0.0.9/librecell.egg-info/dependency_links.txt
+-rw-r--r--   0 kramert   (1000) kramert   (1000)        1 2020-12-30 09:39:08.000000 librecell-0.0.9/librecell.egg-info/not-zip-safe
+-rw-r--r--   0 kramert   (1000) kramert   (1000)       69 2020-12-30 17:45:39.000000 librecell-0.0.9/librecell.egg-info/requires.txt
+-rw-r--r--   0 kramert   (1000) kramert   (1000)        1 2020-12-30 17:45:39.000000 librecell-0.0.9/librecell.egg-info/top_level.txt
+-rw-r--r--   0 kramert   (1000) kramert   (1000)       38 2020-12-30 17:45:39.000000 librecell-0.0.9/setup.cfg
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      924 2020-12-30 17:43:51.000000 librecell-0.0.9/setup.py
```

### Comparing `librecell-0.0.8/PKG-INFO` & `librecell-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: librecell
-Version: 0.0.8
+Version: 0.0.9
 Summary: Meta-package for the LibreCell suite.
 Home-page: https://codeberg.org/tok/librecell
 Author: T. Kramer
 Author-email: code@tkramer.ch
 License: UNKNOWN
 Description: # LibreCell Meta
         This is a meta-package containing no code but just references to sub-packages.
```

### Comparing `librecell-0.0.8/librecell.egg-info/PKG-INFO` & `librecell-0.0.9/librecell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: librecell
-Version: 0.0.8
+Version: 0.0.9
 Summary: Meta-package for the LibreCell suite.
 Home-page: https://codeberg.org/tok/librecell
 Author: T. Kramer
 Author-email: code@tkramer.ch
 License: UNKNOWN
 Description: # LibreCell Meta
         This is a meta-package containing no code but just references to sub-packages.
```

### Comparing `librecell-0.0.8/setup.py` & `librecell-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
     with open("README.md", "r") as f:
         return f.read()
 
 
 setup(name='librecell',
-      version='0.0.8',
+      version='0.0.9',
       description='Meta-package for the LibreCell suite.',
       long_description=readme(),
       long_description_content_type="text/markdown",
       keywords='cmos cell generator layout characterization vlsi asic',
       classifiers=[
           'Development Status :: 3 - Alpha',
           'Topic :: Scientific/Engineering',
@@ -19,12 +19,12 @@
           'Programming Language :: Python :: 3'
       ],
       url='https://codeberg.org/tok/librecell',
       author='T. Kramer',
       author_email='code@tkramer.ch',
       license='',  # ???
       install_requires=[
-          'librecell-common==0.0.8',
-          'librecell-layout==0.0.8',
-          'librecell-lib==0.0.8',
+          'librecell-common==0.0.9',
+          'librecell-layout==0.0.9',
+          'librecell-lib==0.0.9',
       ],
       zip_safe=False)
```

