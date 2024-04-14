# Comparing `tmp/ipgogogo-1.0.0.tar.gz` & `tmp/ipgogogo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipgogogo-1.0.0.tar", last modified: Sun Apr 14 09:48:35 2024, max compression
+gzip compressed data, was "ipgogogo-1.0.1.tar", last modified: Sun Apr 14 09:52:03 2024, max compression
```

## Comparing `ipgogogo-1.0.0.tar` & `ipgogogo-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 09:48:35.433437 ipgogogo-1.0.0/
--rw-rw-rw-   0        0        0    11558 2024-04-14 09:26:15.000000 ipgogogo-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1331 2024-04-14 09:48:35.432439 ipgogogo-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      254 2024-04-14 09:23:42.000000 ipgogogo-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 09:48:35.410001 ipgogogo-1.0.0/ipgogogo/
--rw-rw-rw-   0        0        0     1390 2024-04-14 09:31:36.000000 ipgogogo-1.0.0/ipgogogo/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 09:48:35.427084 ipgogogo-1.0.0/ipgogogo/core/
--rw-rw-rw-   0        0        0        0 2024-04-14 07:49:39.000000 ipgogogo-1.0.0/ipgogogo/core/__init__.py
--rw-rw-rw-   0        0        0      966 2024-04-14 09:15:49.000000 ipgogogo-1.0.0/ipgogogo/core/core.py
--rw-rw-rw-   0        0        0     1088 2024-04-14 09:06:32.000000 ipgogogo-1.0.0/ipgogogo/core/rcore.py
--rw-rw-rw-   0        0        0      933 2024-04-14 09:06:30.000000 ipgogogo-1.0.0/ipgogogo/core/wcore.py
-drwxrwxrwx   0        0        0        0 2024-04-14 09:48:35.429433 ipgogogo-1.0.0/ipgogogo/model/
--rw-rw-rw-   0        0        0        0 2024-04-14 08:36:47.000000 ipgogogo-1.0.0/ipgogogo/model/__init__.py
--rw-rw-rw-   0        0        0     1614 2024-04-14 09:13:46.000000 ipgogogo-1.0.0/ipgogogo/model/state.py
--rw-rw-rw-   0        0        0     1825 2024-04-14 09:23:38.000000 ipgogogo-1.0.0/ipgogogo/run.py
-drwxrwxrwx   0        0        0        0 2024-04-14 09:48:35.430435 ipgogogo-1.0.0/ipgogogo/utils/
--rw-rw-rw-   0        0        0        0 2024-04-14 08:10:33.000000 ipgogogo-1.0.0/ipgogogo/utils/__init__.py
--rw-rw-rw-   0        0        0      720 2024-04-14 09:06:41.000000 ipgogogo-1.0.0/ipgogogo/utils/checkdir.py
--rw-rw-rw-   0        0        0      552 2024-04-14 09:21:24.000000 ipgogogo-1.0.0/ipgogogo/utils/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-14 09:48:35.431434 ipgogogo-1.0.0/ipgogogo.egg-info/
--rw-rw-rw-   0        0        0     1331 2024-04-14 09:48:35.000000 ipgogogo-1.0.0/ipgogogo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2024-04-14 09:48:35.000000 ipgogogo-1.0.0/ipgogogo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 09:48:35.000000 ipgogogo-1.0.0/ipgogogo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-14 09:48:35.000000 ipgogogo-1.0.0/ipgogogo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-14 09:48:35.000000 ipgogogo-1.0.0/ipgogogo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 09:48:35.433437 ipgogogo-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     4349 2024-04-14 09:47:58.000000 ipgogogo-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 09:52:03.280948 ipgogogo-1.0.1/
+-rw-rw-rw-   0        0        0    11558 2024-04-14 09:26:15.000000 ipgogogo-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1331 2024-04-14 09:52:03.279944 ipgogogo-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2024-04-14 09:23:42.000000 ipgogogo-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 09:52:03.256333 ipgogogo-1.0.1/ipgogogo/
+-rw-rw-rw-   0        0        0     1394 2024-04-14 09:51:21.000000 ipgogogo-1.0.1/ipgogogo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 09:52:03.275860 ipgogogo-1.0.1/ipgogogo/core/
+-rw-rw-rw-   0        0        0        0 2024-04-14 07:49:39.000000 ipgogogo-1.0.1/ipgogogo/core/__init__.py
+-rw-rw-rw-   0        0        0      966 2024-04-14 09:15:49.000000 ipgogogo-1.0.1/ipgogogo/core/core.py
+-rw-rw-rw-   0        0        0     1088 2024-04-14 09:06:32.000000 ipgogogo-1.0.1/ipgogogo/core/rcore.py
+-rw-rw-rw-   0        0        0      933 2024-04-14 09:06:30.000000 ipgogogo-1.0.1/ipgogogo/core/wcore.py
+drwxrwxrwx   0        0        0        0 2024-04-14 09:52:03.276940 ipgogogo-1.0.1/ipgogogo/model/
+-rw-rw-rw-   0        0        0        0 2024-04-14 08:36:47.000000 ipgogogo-1.0.1/ipgogogo/model/__init__.py
+-rw-rw-rw-   0        0        0     1614 2024-04-14 09:13:46.000000 ipgogogo-1.0.1/ipgogogo/model/state.py
+-rw-rw-rw-   0        0        0     1825 2024-04-14 09:23:38.000000 ipgogogo-1.0.1/ipgogogo/run.py
+drwxrwxrwx   0        0        0        0 2024-04-14 09:52:03.278943 ipgogogo-1.0.1/ipgogogo/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-14 08:10:33.000000 ipgogogo-1.0.1/ipgogogo/utils/__init__.py
+-rw-rw-rw-   0        0        0      720 2024-04-14 09:06:41.000000 ipgogogo-1.0.1/ipgogogo/utils/checkdir.py
+-rw-rw-rw-   0        0        0      552 2024-04-14 09:21:24.000000 ipgogogo-1.0.1/ipgogogo/utils/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-14 09:52:03.279944 ipgogogo-1.0.1/ipgogogo.egg-info/
+-rw-rw-rw-   0        0        0     1331 2024-04-14 09:52:03.000000 ipgogogo-1.0.1/ipgogogo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2024-04-14 09:52:03.000000 ipgogogo-1.0.1/ipgogogo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 09:52:03.000000 ipgogogo-1.0.1/ipgogogo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-14 09:52:03.000000 ipgogogo-1.0.1/ipgogogo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-14 09:52:03.000000 ipgogogo-1.0.1/ipgogogo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 09:52:03.281943 ipgogogo-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     4349 2024-04-14 09:51:31.000000 ipgogogo-1.0.1/setup.py
```

### Comparing `ipgogogo-1.0.0/LICENSE` & `ipgogogo-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipgogogo-1.0.0/PKG-INFO` & `ipgogogo-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipgogogo
-Version: 1.0.0
+Version: 1.0.1
 Summary: I(mage) to P(df) Go Go Go!
 Home-page: https://github.com/keyork/ipgogogo
 Author: Keyork
 Author-email: chengky18@icloud.com
 License: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `ipgogogo-1.0.0/ipgogogo/__init__.py` & `ipgogogo-1.0.1/ipgogogo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
-from core.core import Core
-from model.state import CoreState
-from utils.checkdir import is_bottom_dir
-from utils.logger import init_logger
+from .core.core import Core
+from .model.state import CoreState
+from .utils.checkdir import is_bottom_dir
+from .utils.logger import init_logger
 
 
 class IPGoGoGo:
 
     def __init__(self, input_path: str, output_path: str, loglevel: str = "INFO"):
         self.input_path = input_path
         self.output_path = output_path
```

### Comparing `ipgogogo-1.0.0/ipgogogo/core/core.py` & `ipgogogo-1.0.1/ipgogogo/core/core.py`

 * *Files identical despite different names*

### Comparing `ipgogogo-1.0.0/ipgogogo/core/rcore.py` & `ipgogogo-1.0.1/ipgogogo/core/rcore.py`

 * *Files identical despite different names*

### Comparing `ipgogogo-1.0.0/ipgogogo/core/wcore.py` & `ipgogogo-1.0.1/ipgogogo/core/wcore.py`

 * *Files identical despite different names*

### Comparing `ipgogogo-1.0.0/ipgogogo/model/state.py` & `ipgogogo-1.0.1/ipgogogo/model/state.py`

 * *Files identical despite different names*

### Comparing `ipgogogo-1.0.0/ipgogogo/run.py` & `ipgogogo-1.0.1/ipgogogo/run.py`

 * *Files identical despite different names*

### Comparing `ipgogogo-1.0.0/ipgogogo/utils/checkdir.py` & `ipgogogo-1.0.1/ipgogogo/utils/checkdir.py`

 * *Files identical despite different names*

### Comparing `ipgogogo-1.0.0/ipgogogo/utils/logger.py` & `ipgogogo-1.0.1/ipgogogo/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ipgogogo-1.0.0/ipgogogo.egg-info/PKG-INFO` & `ipgogogo-1.0.1/ipgogogo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipgogogo
-Version: 1.0.0
+Version: 1.0.1
 Summary: I(mage) to P(df) Go Go Go!
 Home-page: https://github.com/keyork/ipgogogo
 Author: Keyork
 Author-email: chengky18@icloud.com
 License: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `ipgogogo-1.0.0/setup.py` & `ipgogogo-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # Package meta-data.
 NAME = "ipgogogo"
 DESCRIPTION = "I(mage) to P(df) Go Go Go!"
 URL = "https://github.com/keyork/ipgogogo"
 EMAIL = "chengky18@icloud.com"
 AUTHOR = "Keyork"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "pillow",
     "loguru",
 ]
```

