# Comparing `tmp/MMLToolbox-1.0.8.tar.gz` & `tmp/MMLToolbox-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MMLToolbox-1.0.8.tar", last modified: Fri Mar 22 11:55:02 2024, max compression
+gzip compressed data, was "MMLToolbox-1.0.9.tar", last modified: Sun Mar 24 14:11:08 2024, max compression
```

## Comparing `MMLToolbox-1.0.8.tar` & `MMLToolbox-1.0.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 eliali    (1000) eliali    (1000)        0 2024-03-22 11:55:02.814512 MMLToolbox-1.0.8/
--rw-rw-r--   0 eliali    (1000) eliali    (1000)     1060 2023-12-18 14:54:35.000000 MMLToolbox-1.0.8/LICENSE
--rw-rw-r--   0 eliali    (1000) eliali    (1000)       18 2024-03-15 10:36:05.000000 MMLToolbox-1.0.8/MANIFEST.in
-drwxrwxr-x   0 eliali    (1000) eliali    (1000)        0 2024-03-22 11:55:02.810507 MMLToolbox-1.0.8/MMLToolbox/
--rw-rw-r--   0 eliali    (1000) eliali    (1000)       20 2023-12-18 14:54:35.000000 MMLToolbox-1.0.8/MMLToolbox/MML.py
--rw-rw-r--   0 eliali    (1000) eliali    (1000)       21 2023-12-18 14:54:35.000000 MMLToolbox-1.0.8/MMLToolbox/__init__.py
-drwxrwxr-x   0 eliali    (1000) eliali    (1000)        0 2024-03-22 11:55:02.810507 MMLToolbox-1.0.8/MMLToolbox/coord/
--rw-rw-r--   0 eliali    (1000) eliali    (1000)     8228 2024-03-15 11:24:48.000000 MMLToolbox-1.0.8/MMLToolbox/coord/Coord.py
--rw-rw-r--   0 eliali    (1000) eliali    (1000)     1290 2024-02-20 08:09:15.000000 MMLToolbox-1.0.8/MMLToolbox/coord/WASDHandle.py
--rw-rw-r--   0 eliali    (1000) eliali    (1000)       24 2023-12-18 14:54:35.000000 MMLToolbox-1.0.8/MMLToolbox/coord/__init__.py
-drwxrwxr-x   0 eliali    (1000) eliali    (1000)        0 2024-03-22 11:55:02.814512 MMLToolbox-1.0.8/MMLToolbox/optic/
--rw-rw-r--   0 eliali    (1000) eliali    (1000)       21 2023-12-18 14:54:35.000000 MMLToolbox-1.0.8/MMLToolbox/optic/Optic.py
--rw-rw-r--   0 eliali    (1000) eliali    (1000)       24 2023-12-18 14:54:35.000000 MMLToolbox-1.0.8/MMLToolbox/optic/__init__.py
-drwxrwxr-x   0 eliali    (1000) eliali    (1000)        0 2024-03-22 11:55:02.814512 MMLToolbox-1.0.8/MMLToolbox/pxi/
--rw-rw-r--   0 eliali    (1000) eliali    (1000)    22746 2024-02-20 09:03:02.000000 MMLToolbox-1.0.8/MMLToolbox/pxi/PXIControl.py
--rw-rw-r--   0 eliali    (1000) eliali    (1000)     4732 2024-02-18 11:32:52.000000 MMLToolbox-1.0.8/MMLToolbox/pxi/PXIPostProcessing.py
--rw-rw-r--   0 eliali    (1000) eliali    (1000)     2589 2023-12-18 14:54:35.000000 MMLToolbox-1.0.8/MMLToolbox/pxi/PXIPreProcessing.py
--rw-rw-r--   0 eliali    (1000) eliali    (1000)    16061 2024-03-22 11:54:42.000000 MMLToolbox-1.0.8/MMLToolbox/pxi/StoreSetup.py
--rw-rw-r--   0 eliali    (1000) eliali    (1000)      114 2023-12-18 14:54:35.000000 MMLToolbox-1.0.8/MMLToolbox/pxi/__init__.py
-drwxrwxr-x   0 eliali    (1000) eliali    (1000)        0 2024-03-22 11:55:02.814512 MMLToolbox-1.0.8/MMLToolbox/util/
--rw-rw-r--   0 eliali    (1000) eliali    (1000)     3059 2024-02-29 07:32:48.000000 MMLToolbox-1.0.8/MMLToolbox/util/StoreH5.py
--rw-rw-r--   0 eliali    (1000) eliali    (1000)       68 2023-12-18 14:54:35.000000 MMLToolbox-1.0.8/MMLToolbox/util/__init__.py
--rw-rw-r--   0 eliali    (1000) eliali    (1000)      115 2023-12-18 14:54:35.000000 MMLToolbox-1.0.8/MMLToolbox/util/types.py
--rw-rw-r--   0 eliali    (1000) eliali    (1000)        0 2023-12-18 14:54:35.000000 MMLToolbox-1.0.8/MMLToolbox/util/util.py
-drwxrwxr-x   0 eliali    (1000) eliali    (1000)        0 2024-03-22 11:55:02.814512 MMLToolbox-1.0.8/MMLToolbox.egg-info/
--rw-r--r--   0 eliali    (1000) eliali    (1000)     2879 2024-03-22 11:55:02.000000 MMLToolbox-1.0.8/MMLToolbox.egg-info/PKG-INFO
--rw-rw-r--   0 eliali    (1000) eliali    (1000)      660 2024-03-22 11:55:02.000000 MMLToolbox-1.0.8/MMLToolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 eliali    (1000) eliali    (1000)        1 2024-03-22 11:55:02.000000 MMLToolbox-1.0.8/MMLToolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 eliali    (1000) eliali    (1000)        6 2024-03-22 11:55:02.000000 MMLToolbox-1.0.8/MMLToolbox.egg-info/requires.txt
--rw-rw-r--   0 eliali    (1000) eliali    (1000)       11 2024-03-22 11:55:02.000000 MMLToolbox-1.0.8/MMLToolbox.egg-info/top_level.txt
--rw-r--r--   0 eliali    (1000) eliali    (1000)     2879 2024-03-22 11:55:02.814512 MMLToolbox-1.0.8/PKG-INFO
--rw-rw-r--   0 eliali    (1000) eliali    (1000)     2334 2024-03-17 18:58:33.000000 MMLToolbox-1.0.8/README.rst
--rw-rw-r--   0 eliali    (1000) eliali    (1000)       80 2024-03-22 11:55:02.814512 MMLToolbox-1.0.8/setup.cfg
--rw-rw-r--   0 eliali    (1000) eliali    (1000)     1127 2024-03-22 11:54:38.000000 MMLToolbox-1.0.8/setup.py
+drwxrwxr-x   0 eliali    (1000) eliali    (1000)        0 2024-03-24 14:11:08.832420 MMLToolbox-1.0.9/
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)     1060 2023-12-18 14:54:35.000000 MMLToolbox-1.0.9/LICENSE
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)       18 2024-03-15 10:36:05.000000 MMLToolbox-1.0.9/MANIFEST.in
+drwxrwxr-x   0 eliali    (1000) eliali    (1000)        0 2024-03-24 14:11:08.824420 MMLToolbox-1.0.9/MMLToolbox/
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)       20 2023-12-18 14:54:35.000000 MMLToolbox-1.0.9/MMLToolbox/MML.py
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)       21 2023-12-18 14:54:35.000000 MMLToolbox-1.0.9/MMLToolbox/__init__.py
+drwxrwxr-x   0 eliali    (1000) eliali    (1000)        0 2024-03-24 14:11:08.824420 MMLToolbox-1.0.9/MMLToolbox/coord/
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)     8228 2024-03-15 11:24:48.000000 MMLToolbox-1.0.9/MMLToolbox/coord/Coord.py
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)     1290 2024-02-20 08:09:15.000000 MMLToolbox-1.0.9/MMLToolbox/coord/WASDHandle.py
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)       24 2023-12-18 14:54:35.000000 MMLToolbox-1.0.9/MMLToolbox/coord/__init__.py
+drwxrwxr-x   0 eliali    (1000) eliali    (1000)        0 2024-03-24 14:11:08.828420 MMLToolbox-1.0.9/MMLToolbox/optic/
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)       21 2023-12-18 14:54:35.000000 MMLToolbox-1.0.9/MMLToolbox/optic/Optic.py
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)       24 2023-12-18 14:54:35.000000 MMLToolbox-1.0.9/MMLToolbox/optic/__init__.py
+drwxrwxr-x   0 eliali    (1000) eliali    (1000)        0 2024-03-24 14:11:08.828420 MMLToolbox-1.0.9/MMLToolbox/pxi/
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)    22746 2024-02-20 09:03:02.000000 MMLToolbox-1.0.9/MMLToolbox/pxi/PXIControl.py
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)     4732 2024-02-18 11:32:52.000000 MMLToolbox-1.0.9/MMLToolbox/pxi/PXIPostProcessing.py
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)     2589 2023-12-18 14:54:35.000000 MMLToolbox-1.0.9/MMLToolbox/pxi/PXIPreProcessing.py
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)    16061 2024-03-22 11:54:42.000000 MMLToolbox-1.0.9/MMLToolbox/pxi/StoreSetup.py
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)      114 2023-12-18 14:54:35.000000 MMLToolbox-1.0.9/MMLToolbox/pxi/__init__.py
+drwxrwxr-x   0 eliali    (1000) eliali    (1000)        0 2024-03-24 14:11:08.828420 MMLToolbox-1.0.9/MMLToolbox/util/
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)     3059 2024-02-29 07:32:48.000000 MMLToolbox-1.0.9/MMLToolbox/util/StoreH5.py
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)       68 2023-12-18 14:54:35.000000 MMLToolbox-1.0.9/MMLToolbox/util/__init__.py
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)      115 2023-12-18 14:54:35.000000 MMLToolbox-1.0.9/MMLToolbox/util/types.py
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)        0 2023-12-18 14:54:35.000000 MMLToolbox-1.0.9/MMLToolbox/util/util.py
+drwxrwxr-x   0 eliali    (1000) eliali    (1000)        0 2024-03-24 14:11:08.828420 MMLToolbox-1.0.9/MMLToolbox.egg-info/
+-rw-r--r--   0 eliali    (1000) eliali    (1000)    29242 2024-03-24 14:11:08.000000 MMLToolbox-1.0.9/MMLToolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)      660 2024-03-24 14:11:08.000000 MMLToolbox-1.0.9/MMLToolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)        1 2024-03-24 14:11:08.000000 MMLToolbox-1.0.9/MMLToolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)        6 2024-03-24 14:11:08.000000 MMLToolbox-1.0.9/MMLToolbox.egg-info/requires.txt
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)       11 2024-03-24 14:11:08.000000 MMLToolbox-1.0.9/MMLToolbox.egg-info/top_level.txt
+-rw-r--r--   0 eliali    (1000) eliali    (1000)    29242 2024-03-24 14:11:08.832420 MMLToolbox-1.0.9/PKG-INFO
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)    28696 2024-03-24 14:05:46.000000 MMLToolbox-1.0.9/README.rst
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)       80 2024-03-24 14:11:08.832420 MMLToolbox-1.0.9/setup.cfg
+-rw-rw-r--   0 eliali    (1000) eliali    (1000)     1127 2024-03-24 14:10:57.000000 MMLToolbox-1.0.9/setup.py
```

### Comparing `MMLToolbox-1.0.8/LICENSE` & `MMLToolbox-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `MMLToolbox-1.0.8/MMLToolbox/coord/Coord.py` & `MMLToolbox-1.0.9/MMLToolbox/coord/Coord.py`

 * *Files identical despite different names*

### Comparing `MMLToolbox-1.0.8/MMLToolbox/coord/WASDHandle.py` & `MMLToolbox-1.0.9/MMLToolbox/coord/WASDHandle.py`

 * *Files identical despite different names*

### Comparing `MMLToolbox-1.0.8/MMLToolbox/pxi/PXIControl.py` & `MMLToolbox-1.0.9/MMLToolbox/pxi/PXIControl.py`

 * *Files identical despite different names*

### Comparing `MMLToolbox-1.0.8/MMLToolbox/pxi/PXIPostProcessing.py` & `MMLToolbox-1.0.9/MMLToolbox/pxi/PXIPostProcessing.py`

 * *Files identical despite different names*

### Comparing `MMLToolbox-1.0.8/MMLToolbox/pxi/PXIPreProcessing.py` & `MMLToolbox-1.0.9/MMLToolbox/pxi/PXIPreProcessing.py`

 * *Files identical despite different names*

### Comparing `MMLToolbox-1.0.8/MMLToolbox/pxi/StoreSetup.py` & `MMLToolbox-1.0.9/MMLToolbox/pxi/StoreSetup.py`

 * *Files identical despite different names*

### Comparing `MMLToolbox-1.0.8/MMLToolbox/util/StoreH5.py` & `MMLToolbox-1.0.9/MMLToolbox/util/StoreH5.py`

 * *Files identical despite different names*

### Comparing `MMLToolbox-1.0.8/MMLToolbox.egg-info/SOURCES.txt` & `MMLToolbox-1.0.9/MMLToolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MMLToolbox-1.0.8/setup.py` & `MMLToolbox-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 setup(
     name="MMLToolbox",
     description="",
     long_description_content_type= 'text/x-rst',
     long_description=readme,
     #long_description_content_type='text/markdown',
-    version="1.0.8",
+    version="1.0.9",
     author="IGTE",  
     author_email="andreas.gschwentner@tugraz.at",
     url="https://www.tugraz.at/institute/igte/home/",
     packages=["MMLToolbox", "MMLToolbox.util", "MMLToolbox.coord", "MMLToolbox.optic", "MMLToolbox.pxi"],
     # include_package_data=True,
     # scripts=["bin/generate-ex"],
     keywords=["parameter", "identification", "measurements", "optimization"],
```

