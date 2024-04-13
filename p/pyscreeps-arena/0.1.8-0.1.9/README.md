# Comparing `tmp/pyscreeps-arena-0.1.8.tar.gz` & `tmp/pyscreeps-arena-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscreeps-arena-0.1.8.tar", last modified: Wed Apr  3 05:37:14 2024, max compression
+gzip compressed data, was "pyscreeps-arena-0.1.9.tar", last modified: Wed Apr  3 12:34:42 2024, max compression
```

## Comparing `pyscreeps-arena-0.1.8.tar` & `pyscreeps-arena-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 05:37:14.760000 pyscreeps-arena-0.1.8/
--rw-rw-rw-   0        0        0      672 2024-04-03 05:37:16.000000 pyscreeps-arena-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-03 05:37:14.770000 pyscreeps-arena-0.1.8/pyscreeps_arena/
--rw-rw-rw-   0        0        0      749 2024-04-03 05:19:58.000000 pyscreeps-arena-0.1.8/pyscreeps_arena/__init__.py
--rw-rw-rw-   0        0        0    20454 2024-04-03 02:55:00.000000 pyscreeps-arena-0.1.8/pyscreeps_arena/build.py
--rw-rw-rw-   0        0        0    30232 2024-04-03 05:36:36.000000 pyscreeps-arena-0.1.8/pyscreeps_arena/project.7z
-drwxrwxrwx   0        0        0        0 2024-04-03 05:37:14.780000 pyscreeps-arena-0.1.8/pyscreeps_arena.egg-info/
--rw-rw-rw-   0        0        0      672 2024-04-03 05:37:16.000000 pyscreeps-arena-0.1.8/pyscreeps_arena.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2024-04-03 05:37:16.000000 pyscreeps-arena-0.1.8/pyscreeps_arena.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 05:37:16.000000 pyscreeps-arena-0.1.8/pyscreeps_arena.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-04-03 05:37:16.000000 pyscreeps-arena-0.1.8/pyscreeps_arena.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       87 2024-04-03 05:37:16.000000 pyscreeps-arena-0.1.8/pyscreeps_arena.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-03 05:37:16.000000 pyscreeps-arena-0.1.8/pyscreeps_arena.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 05:37:16.000000 pyscreeps-arena-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1230 2024-04-03 05:37:02.000000 pyscreeps-arena-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:34:42.390000 pyscreeps-arena-0.1.9/
+-rw-rw-rw-   0        0        0      672 2024-04-03 12:34:44.000000 pyscreeps-arena-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-03 12:34:42.390000 pyscreeps-arena-0.1.9/pyscreeps_arena/
+-rw-rw-rw-   0        0        0      749 2024-04-03 05:44:56.000000 pyscreeps-arena-0.1.9/pyscreeps_arena/__init__.py
+-rw-rw-rw-   0        0        0    30454 2024-04-03 12:33:18.000000 pyscreeps-arena-0.1.9/pyscreeps_arena/project.7z
+drwxrwxrwx   0        0        0        0 2024-04-03 12:34:42.400000 pyscreeps-arena-0.1.9/pyscreeps_arena.egg-info/
+-rw-rw-rw-   0        0        0      672 2024-04-03 12:34:44.000000 pyscreeps-arena-0.1.9/pyscreeps_arena.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2024-04-03 12:34:44.000000 pyscreeps-arena-0.1.9/pyscreeps_arena.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 12:34:44.000000 pyscreeps-arena-0.1.9/pyscreeps_arena.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-03 12:34:44.000000 pyscreeps-arena-0.1.9/pyscreeps_arena.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       87 2024-04-03 12:34:44.000000 pyscreeps-arena-0.1.9/pyscreeps_arena.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-04-03 12:34:44.000000 pyscreeps-arena-0.1.9/pyscreeps_arena.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 12:34:44.000000 pyscreeps-arena-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1230 2024-04-03 12:34:32.000000 pyscreeps-arena-0.1.9/setup.py
```

### Comparing `pyscreeps-arena-0.1.8/PKG-INFO` & `pyscreeps-arena-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscreeps-arena
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python api|interface to play steam game: Screeps: Arena.
 Author-email: 2229066748@qq.com
 Maintainer: Eagle'sBaby
 Maintainer-email: 2229066748@qq.com
 License: Apache Licence 2.0
 Keywords: python,screeps:arena,screeps
 Classifier: Programming Language :: Python
```

### Comparing `pyscreeps-arena-0.1.8/pyscreeps_arena/__init__.py` & `pyscreeps-arena-0.1.9/pyscreeps_arena/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscreeps-arena-0.1.8/pyscreeps_arena.egg-info/PKG-INFO` & `pyscreeps-arena-0.1.9/pyscreeps_arena.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscreeps-arena
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python api|interface to play steam game: Screeps: Arena.
 Author-email: 2229066748@qq.com
 Maintainer: Eagle'sBaby
 Maintainer-email: 2229066748@qq.com
 License: Apache Licence 2.0
 Keywords: python,screeps:arena,screeps
 Classifier: Programming Language :: Python
```

### Comparing `pyscreeps-arena-0.1.8/setup.py` & `pyscreeps-arena-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 from setuptools import setup, find_packages
 
 with open(r"T:\New_PC\Import_Project\uploads\pyscreeps-arena_upload\pyscreeps-arena.md", 'r') as f:
     long_description = f.read()
 setup(
     name='pyscreeps-arena',
-    version='0.1.8',
+    version='0.1.9',
     description='Python api|interface to play steam game: Screeps: Arena.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author_email='2229066748@qq.com',
     maintainer="Eagle'sBaby",
     maintainer_email='2229066748@qq.com',
     packages=find_packages(),
```

