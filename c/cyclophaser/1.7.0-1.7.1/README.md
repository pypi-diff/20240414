# Comparing `tmp/cyclophaser-1.7.0.tar.gz` & `tmp/cyclophaser-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclophaser-1.7.0.tar", last modified: Thu Apr 11 23:09:34 2024, max compression
+gzip compressed data, was "cyclophaser-1.7.1.tar", last modified: Sat Apr 13 21:13:20 2024, max compression
```

## Comparing `cyclophaser-1.7.0.tar` & `cyclophaser-1.7.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-11 23:09:34.721340 cyclophaser-1.7.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1783 2024-04-11 23:09:34.721340 cyclophaser-1.7.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-11 23:09:34.721340 cyclophaser-1.7.0/cyclophaser/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/cyclophaser/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17593 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/cyclophaser/determine_periods.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12997 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/cyclophaser/find_stages.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1981 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/cyclophaser/lanczos_filter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12837 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/cyclophaser/plots.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-11 23:09:34.721340 cyclophaser-1.7.0/cyclophaser.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1783 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/cyclophaser.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      343 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/cyclophaser.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/cyclophaser.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/cyclophaser.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-11 23:09:34.721340 cyclophaser-1.7.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-11 23:09:34.721340 cyclophaser-1.7.0/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1901 2024-04-11 23:09:34.000000 cyclophaser-1.7.0/tests/test_determine_periods.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-13 21:13:20.780402 cyclophaser-1.7.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1783 2024-04-13 21:13:20.780402 cyclophaser-1.7.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2024-04-13 21:13:20.000000 cyclophaser-1.7.1/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-13 21:13:20.780402 cyclophaser-1.7.1/cyclophaser/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       48 2024-04-13 21:13:20.000000 cyclophaser-1.7.1/cyclophaser/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17569 2024-04-13 21:13:20.000000 cyclophaser-1.7.1/cyclophaser/determine_periods.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12997 2024-04-13 21:13:20.000000 cyclophaser-1.7.1/cyclophaser/find_stages.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1981 2024-04-13 21:13:20.000000 cyclophaser-1.7.1/cyclophaser/lanczos_filter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12837 2024-04-13 21:13:20.000000 cyclophaser-1.7.1/cyclophaser/plots.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-13 21:13:20.780402 cyclophaser-1.7.1/cyclophaser.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1783 2024-04-13 21:13:20.000000 cyclophaser-1.7.1/cyclophaser.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      343 2024-04-13 21:13:20.000000 cyclophaser-1.7.1/cyclophaser.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-13 21:13:20.000000 cyclophaser-1.7.1/cyclophaser.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2024-04-13 21:13:20.000000 cyclophaser-1.7.1/cyclophaser.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-13 21:13:20.780402 cyclophaser-1.7.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1264 2024-04-13 21:13:20.000000 cyclophaser-1.7.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-13 21:13:20.780402 cyclophaser-1.7.1/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-13 21:13:20.000000 cyclophaser-1.7.1/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1901 2024-04-13 21:13:20.000000 cyclophaser-1.7.1/tests/test_determine_periods.py
```

### Comparing `cyclophaser-1.7.0/PKG-INFO` & `cyclophaser-1.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclophaser
-Version: 1.7.0
+Version: 1.7.1
 Summary: Determine phases from extratropical cyclone life cycle
 Author: Danilo Couto de Souza
 Author-email: danilo.oceano@gmail.com
 License: MIT
 Project-URL: Documentation, https://yourproject.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/daniloceano/CycloPhaser
 Project-URL: Issue Tracker, https://readthedocs.org/projects/cyclophaser/
```

### Comparing `cyclophaser-1.7.0/README.md` & `cyclophaser-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `cyclophaser-1.7.0/cyclophaser/determine_periods.py` & `cyclophaser-1.7.1/cyclophaser/determine_periods.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #                                                                              #
 #                                                         :::      ::::::::    #
 #    determine_periods.py                               :+:      :+:    :+:    #
 #                                                     +:+ +:+         +:+      #
 #    By: daniloceano <danilo.oceano@gmail.com>      +#+  +:+       +#+         #
 #                                                 +#+#+#+#+#+   +#+            #
 #    Created: 2023/05/19 19:06:47 by danilocs          #+#    #+#              #
-#    Updated: 2024/04/11 19:59:55 by daniloceano      ###   ########.fr        #
+#    Updated: 2024/04/13 17:37:13 by daniloceano      ###   ########.fr        #
 #                                                                              #
 # **************************************************************************** #
 
 import os
 import csv
 
 import xarray as xr
@@ -391,22 +391,22 @@
     # Testing options
     process_vorticity_args = {
             "use_filter": False,
             "use_smoothing_twice": False
         }
 
     periods_args= {
-        'threshold_intensification_length': 0.10,  # Decreased threshold
-        'threshold_intensification_gap': 0.05,
-        'threshold_mature_distance': 0.10,
-        'threshold_mature_length': 0.02,
-        'threshold_decay_length': 0.06,
-        'threshold_decay_gap': 0.06,
-        'threshold_incipient_length': 0.35
-        }
+        'threshold_intensification_length': 0.25,
+        'threshold_intensification_gap': 0.075,
+        'threshold_mature_distance': 0.125,
+        'threshold_mature_length': 0.03,
+        'threshold_decay_length': 0.075,
+        'threshold_decay_gap': 0.075,
+        'threshold_incipient_length': 0.4
+    }
 
     # Test the determine_periods function
     result = determine_periods(series,
             x=x,
             plot="test",
             plot_steps="test_steps",
             export_dict=False,
```

### Comparing `cyclophaser-1.7.0/cyclophaser/find_stages.py` & `cyclophaser-1.7.1/cyclophaser/find_stages.py`

 * *Files identical despite different names*

### Comparing `cyclophaser-1.7.0/cyclophaser/lanczos_filter.py` & `cyclophaser-1.7.1/cyclophaser/lanczos_filter.py`

 * *Files identical despite different names*

### Comparing `cyclophaser-1.7.0/cyclophaser/plots.py` & `cyclophaser-1.7.1/cyclophaser/plots.py`

 * *Files identical despite different names*

### Comparing `cyclophaser-1.7.0/cyclophaser.egg-info/PKG-INFO` & `cyclophaser-1.7.1/cyclophaser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclophaser
-Version: 1.7.0
+Version: 1.7.1
 Summary: Determine phases from extratropical cyclone life cycle
 Author: Danilo Couto de Souza
 Author-email: danilo.oceano@gmail.com
 License: MIT
 Project-URL: Documentation, https://yourproject.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/daniloceano/CycloPhaser
 Project-URL: Issue Tracker, https://readthedocs.org/projects/cyclophaser/
```

### Comparing `cyclophaser-1.7.0/setup.py` & `cyclophaser-1.7.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
-VERSION = '1.7.0'
+VERSION = '1.7.1'
 DESCRIPTION = 'Determine phases from extratropical cyclone life cycle'
 # LONG_DESCRIPTION = 'This script processes vorticity data, identifies different phases of the cyclone \
     # and plots the identified periods on periods.png and periods_didatic.png'
 
 setup(
     name="cyclophaser",
     version=VERSION,
```

### Comparing `cyclophaser-1.7.0/tests/test_determine_periods.py` & `cyclophaser-1.7.1/tests/test_determine_periods.py`

 * *Files identical despite different names*

