# Comparing `tmp/ccnuacm_datamocker-0.0.4.tar.gz` & `tmp/ccnuacm_datamocker-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccnuacm_datamocker-0.0.4.tar", last modified: Sun Apr 14 15:39:28 2024, max compression
+gzip compressed data, was "ccnuacm_datamocker-0.0.5.tar", last modified: Sun Apr 14 15:39:29 2024, max compression
```

## Comparing `ccnuacm_datamocker-0.0.4.tar` & `ccnuacm_datamocker-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:39:28.483724 ccnuacm_datamocker-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-14 15:39:24.000000 ccnuacm_datamocker-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-14 15:39:28.483724 ccnuacm_datamocker-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-14 15:39:24.000000 ccnuacm_datamocker-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:39:28.483724 ccnuacm_datamocker-0.0.4/ccnuacm_datamocker/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-14 15:39:24.000000 ccnuacm_datamocker-0.0.4/ccnuacm_datamocker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:39:28.483724 ccnuacm_datamocker-0.0.4/ccnuacm_datamocker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-14 15:39:28.000000 ccnuacm_datamocker-0.0.4/ccnuacm_datamocker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-14 15:39:28.000000 ccnuacm_datamocker-0.0.4/ccnuacm_datamocker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 15:39:28.000000 ccnuacm_datamocker-0.0.4/ccnuacm_datamocker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-14 15:39:28.000000 ccnuacm_datamocker-0.0.4/ccnuacm_datamocker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-14 15:39:28.000000 ccnuacm_datamocker-0.0.4/ccnuacm_datamocker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 15:39:28.483724 ccnuacm_datamocker-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-14 15:39:24.000000 ccnuacm_datamocker-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:39:29.695345 ccnuacm_datamocker-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-14 15:39:25.000000 ccnuacm_datamocker-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-14 15:39:29.691346 ccnuacm_datamocker-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-14 15:39:25.000000 ccnuacm_datamocker-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:39:29.691346 ccnuacm_datamocker-0.0.5/ccnuacm_datamocker/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-14 15:39:25.000000 ccnuacm_datamocker-0.0.5/ccnuacm_datamocker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:39:29.691346 ccnuacm_datamocker-0.0.5/ccnuacm_datamocker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-14 15:39:29.000000 ccnuacm_datamocker-0.0.5/ccnuacm_datamocker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-14 15:39:29.000000 ccnuacm_datamocker-0.0.5/ccnuacm_datamocker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 15:39:29.000000 ccnuacm_datamocker-0.0.5/ccnuacm_datamocker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-14 15:39:29.000000 ccnuacm_datamocker-0.0.5/ccnuacm_datamocker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-14 15:39:29.000000 ccnuacm_datamocker-0.0.5/ccnuacm_datamocker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 15:39:29.695345 ccnuacm_datamocker-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-14 15:39:25.000000 ccnuacm_datamocker-0.0.5/setup.py
```

### Comparing `ccnuacm_datamocker-0.0.4/LICENSE` & `ccnuacm_datamocker-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ccnuacm_datamocker-0.0.4/PKG-INFO` & `ccnuacm_datamocker-0.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccnuacm_datamocker
-Version: 0.0.4
+Version: 0.0.5
 Summary: A data mocking library for CCNU ACM
 Home-page: https://github.com/CCNU-ACM-Official/CCNUACM_DataMocker.git
 Author: JixiangXiong
 Author-email: xiongjx751@qq.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -28,15 +28,15 @@
 
 ```bash
 pip3 install ccnuacm-datamocker -U
 ```
 
 ## Usage
 
-Following is a basic example of how to use the data mocker. More examples are avaliable [here](https://github.com/CCNU-ACM-Official/CCNUACM_DataMocker/tree/578ac35f3dbea1733bbbed94b38e8669b26bd4dc/examples).
+Following is a basic example of how to use the data mocker. More examples are avaliable [here](examples).
 
 ```python
 import ccnuacm_datamocker as dm
 from ccnuacm_datamocker.data_model import *
 import os
 
 dm.set_seed(0)
```

### Comparing `ccnuacm_datamocker-0.0.4/README.md` & `ccnuacm_datamocker-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 ```bash
 pip3 install ccnuacm-datamocker -U
 ```
 
 ## Usage
 
-Following is a basic example of how to use the data mocker. More examples are avaliable [here](https://github.com/CCNU-ACM-Official/CCNUACM_DataMocker/tree/578ac35f3dbea1733bbbed94b38e8669b26bd4dc/examples).
+Following is a basic example of how to use the data mocker. More examples are avaliable [here](examples).
 
 ```python
 import ccnuacm_datamocker as dm
 from ccnuacm_datamocker.data_model import *
 import os
 
 dm.set_seed(0)
```

### Comparing `ccnuacm_datamocker-0.0.4/ccnuacm_datamocker.egg-info/PKG-INFO` & `ccnuacm_datamocker-0.0.5/ccnuacm_datamocker.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccnuacm_datamocker
-Version: 0.0.4
+Version: 0.0.5
 Summary: A data mocking library for CCNU ACM
 Home-page: https://github.com/CCNU-ACM-Official/CCNUACM_DataMocker.git
 Author: JixiangXiong
 Author-email: xiongjx751@qq.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -28,15 +28,15 @@
 
 ```bash
 pip3 install ccnuacm-datamocker -U
 ```
 
 ## Usage
 
-Following is a basic example of how to use the data mocker. More examples are avaliable [here](https://github.com/CCNU-ACM-Official/CCNUACM_DataMocker/tree/578ac35f3dbea1733bbbed94b38e8669b26bd4dc/examples).
+Following is a basic example of how to use the data mocker. More examples are avaliable [here](examples).
 
 ```python
 import ccnuacm_datamocker as dm
 from ccnuacm_datamocker.data_model import *
 import os
 
 dm.set_seed(0)
```

### Comparing `ccnuacm_datamocker-0.0.4/setup.py` & `ccnuacm_datamocker-0.0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="ccnuacm_datamocker",
-    version="0.0.4",
+    version="0.0.5",
     description="A data mocking library for CCNU ACM",
     author="JixiangXiong",
     author_email="xiongjx751@qq.com",
     url="https://github.com/CCNU-ACM-Official/CCNUACM_DataMocker.git",
     packages=["ccnuacm_datamocker"],
     install_requires=[
         "numpy",
```

