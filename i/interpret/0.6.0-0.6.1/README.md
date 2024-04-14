# Comparing `tmp/interpret-0.6.0.tar.gz` & `tmp/interpret-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interpret-0.6.0.tar", last modified: Sat Mar 16 09:08:38 2024, max compression
+gzip compressed data, was "interpret-0.6.1.tar", last modified: Sun Apr 14 03:54:59 2024, max compression
```

## Comparing `interpret-0.6.0.tar` & `interpret-0.6.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-16 09:08:38.161015 interpret-0.6.0/
--rw-r--r--   0 vsts      (1001) docker     (127)     1067 2024-03-16 09:08:38.161015 interpret-0.6.0/PKG-INFO
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-03-16 09:08:38.161015 interpret-0.6.0/interpret.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1067 2024-03-16 09:08:38.000000 interpret-0.6.0/interpret.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      172 2024-03-16 09:08:38.000000 interpret-0.6.0/interpret.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-16 09:08:38.000000 interpret-0.6.0/interpret.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       74 2024-03-16 09:08:38.000000 interpret-0.6.0/interpret.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-03-16 09:08:38.000000 interpret-0.6.0/interpret.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-03-16 09:08:38.161015 interpret-0.6.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)     1695 2024-03-16 09:03:47.000000 interpret-0.6.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-14 03:54:59.107388 interpret-0.6.1/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1067 2024-04-14 03:54:59.107388 interpret-0.6.1/PKG-INFO
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-14 03:54:59.107388 interpret-0.6.1/interpret.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1067 2024-04-14 03:54:59.000000 interpret-0.6.1/interpret.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      172 2024-04-14 03:54:59.000000 interpret-0.6.1/interpret.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-14 03:54:59.000000 interpret-0.6.1/interpret.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       74 2024-04-14 03:54:59.000000 interpret-0.6.1/interpret.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-14 03:54:59.000000 interpret-0.6.1/interpret.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-14 03:54:59.107388 interpret-0.6.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     1695 2024-04-14 03:49:18.000000 interpret-0.6.1/setup.py
```

### Comparing `interpret-0.6.0/PKG-INFO` & `interpret-0.6.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpret
-Version: 0.6.0
+Version: 0.6.1
 Summary: Fit interpretable models. Explain blackbox machine learning.
 Home-page: https://github.com/interpretml/interpret
 Author: The InterpretML Contributors
 Author-email: interpret@microsoft.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Dist: interpret-core[dash,debug,linear,notebook,plotly,sensitivity,shap]==0.6.0
+Requires-Dist: interpret-core[dash,debug,linear,notebook,plotly,sensitivity,shap]==0.6.1
 
 
 In the beginning machines learned in darkness, and data scientists struggled in the void to explain them.
 
 Let there be light.
 
 https://github.com/interpretml/interpret
```

### Comparing `interpret-0.6.0/interpret.egg-info/PKG-INFO` & `interpret-0.6.1/interpret.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interpret
-Version: 0.6.0
+Version: 0.6.1
 Summary: Fit interpretable models. Explain blackbox machine learning.
 Home-page: https://github.com/interpretml/interpret
 Author: The InterpretML Contributors
 Author-email: interpret@microsoft.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Dist: interpret-core[dash,debug,linear,notebook,plotly,sensitivity,shap]==0.6.0
+Requires-Dist: interpret-core[dash,debug,linear,notebook,plotly,sensitivity,shap]==0.6.1
 
 
 In the beginning machines learned in darkness, and data scientists struggled in the void to explain them.
 
 Let there be light.
 
 https://github.com/interpretml/interpret
```

### Comparing `interpret-0.6.0/setup.py` & `interpret-0.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) 2023 The InterpretML Contributors
 # Distributed under the MIT software license
 
 from setuptools import setup, find_packages
 
 name = "interpret"
 # NOTE: Version is replaced by a regex script.
-version = "0.6.0"
+version = "0.6.1"
 long_description = """
 In the beginning machines learned in darkness, and data scientists struggled in the void to explain them.
 
 Let there be light.
 
 https://github.com/interpretml/interpret
 """
```

