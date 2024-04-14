# Comparing `tmp/ipgogogo-1.0.3.tar.gz` & `tmp/ipgogogo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipgogogo-1.0.3.tar", last modified: Sun Apr 14 10:00:17 2024, max compression
+gzip compressed data, was "ipgogogo-1.1.0.tar", last modified: Sun Apr 14 10:57:04 2024, max compression
```

## Comparing `ipgogogo-1.0.3.tar` & `ipgogogo-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 10:00:17.730069 ipgogogo-1.0.3/
--rw-rw-rw-   0        0        0    11558 2024-04-14 09:26:15.000000 ipgogogo-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     1480 2024-04-14 10:00:17.729069 ipgogogo-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      403 2024-04-14 09:57:36.000000 ipgogogo-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 10:00:17.715065 ipgogogo-1.0.3/ipgogogo/
--rw-rw-rw-   0        0        0     1394 2024-04-14 09:51:21.000000 ipgogogo-1.0.3/ipgogogo/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 10:00:17.724071 ipgogogo-1.0.3/ipgogogo/core/
--rw-rw-rw-   0        0        0        0 2024-04-14 07:49:39.000000 ipgogogo-1.0.3/ipgogogo/core/__init__.py
--rw-rw-rw-   0        0        0      968 2024-04-14 09:52:53.000000 ipgogogo-1.0.3/ipgogogo/core/core.py
--rw-rw-rw-   0        0        0     1088 2024-04-14 09:06:32.000000 ipgogogo-1.0.3/ipgogogo/core/rcore.py
--rw-rw-rw-   0        0        0      933 2024-04-14 09:06:30.000000 ipgogogo-1.0.3/ipgogogo/core/wcore.py
-drwxrwxrwx   0        0        0        0 2024-04-14 10:00:17.726070 ipgogogo-1.0.3/ipgogogo/model/
--rw-rw-rw-   0        0        0        0 2024-04-14 08:36:47.000000 ipgogogo-1.0.3/ipgogogo/model/__init__.py
--rw-rw-rw-   0        0        0     1614 2024-04-14 09:53:07.000000 ipgogogo-1.0.3/ipgogogo/model/state.py
--rw-rw-rw-   0        0        0     1825 2024-04-14 09:23:38.000000 ipgogogo-1.0.3/ipgogogo/run.py
-drwxrwxrwx   0        0        0        0 2024-04-14 10:00:17.728066 ipgogogo-1.0.3/ipgogogo/utils/
--rw-rw-rw-   0        0        0        0 2024-04-14 08:10:33.000000 ipgogogo-1.0.3/ipgogogo/utils/__init__.py
--rw-rw-rw-   0        0        0      720 2024-04-14 09:06:41.000000 ipgogogo-1.0.3/ipgogogo/utils/checkdir.py
--rw-rw-rw-   0        0        0      552 2024-04-14 09:21:24.000000 ipgogogo-1.0.3/ipgogogo/utils/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-14 10:00:17.729069 ipgogogo-1.0.3/ipgogogo.egg-info/
--rw-rw-rw-   0        0        0     1480 2024-04-14 10:00:17.000000 ipgogogo-1.0.3/ipgogogo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      446 2024-04-14 10:00:17.000000 ipgogogo-1.0.3/ipgogogo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 10:00:17.000000 ipgogogo-1.0.3/ipgogogo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-14 10:00:17.000000 ipgogogo-1.0.3/ipgogogo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-14 10:00:17.000000 ipgogogo-1.0.3/ipgogogo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 10:00:17.730069 ipgogogo-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     4349 2024-04-14 09:58:58.000000 ipgogogo-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 10:57:04.921513 ipgogogo-1.1.0/
+-rw-rw-rw-   0        0        0    11558 2024-04-14 09:26:15.000000 ipgogogo-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1503 2024-04-14 10:57:04.921005 ipgogogo-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2024-04-14 10:56:10.000000 ipgogogo-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 10:57:04.876446 ipgogogo-1.1.0/ipgogogo/
+-rw-rw-rw-   0        0        0     1445 2024-04-14 10:56:10.000000 ipgogogo-1.1.0/ipgogogo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 10:57:04.916543 ipgogogo-1.1.0/ipgogogo/core/
+-rw-rw-rw-   0        0        0        0 2024-04-14 07:49:39.000000 ipgogogo-1.1.0/ipgogogo/core/__init__.py
+-rw-rw-rw-   0        0        0      975 2024-04-14 10:56:10.000000 ipgogogo-1.1.0/ipgogogo/core/core.py
+-rw-rw-rw-   0        0        0     1088 2024-04-14 09:06:32.000000 ipgogogo-1.1.0/ipgogogo/core/rcore.py
+-rw-rw-rw-   0        0        0      933 2024-04-14 09:06:30.000000 ipgogogo-1.1.0/ipgogogo/core/wcore.py
+drwxrwxrwx   0        0        0        0 2024-04-14 10:57:04.917559 ipgogogo-1.1.0/ipgogogo/model/
+-rw-rw-rw-   0        0        0        0 2024-04-14 08:36:47.000000 ipgogogo-1.1.0/ipgogogo/model/__init__.py
+-rw-rw-rw-   0        0        0     1614 2024-04-14 09:53:07.000000 ipgogogo-1.1.0/ipgogogo/model/state.py
+-rw-rw-rw-   0        0        0     1825 2024-04-14 10:50:59.000000 ipgogogo-1.1.0/ipgogogo/run.py
+-rw-rw-rw-   0        0        0     2500 2024-04-14 10:56:10.000000 ipgogogo-1.1.0/ipgogogo/ui.py
+drwxrwxrwx   0        0        0        0 2024-04-14 10:57:04.920000 ipgogogo-1.1.0/ipgogogo/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-14 08:10:33.000000 ipgogogo-1.1.0/ipgogogo/utils/__init__.py
+-rw-rw-rw-   0        0        0      720 2024-04-14 09:06:41.000000 ipgogogo-1.1.0/ipgogogo/utils/checkdir.py
+-rw-rw-rw-   0        0        0      552 2024-04-14 09:21:24.000000 ipgogogo-1.1.0/ipgogogo/utils/logger.py
+drwxrwxrwx   0        0        0        0 2024-04-14 10:57:04.920000 ipgogogo-1.1.0/ipgogogo.egg-info/
+-rw-rw-rw-   0        0        0     1503 2024-04-14 10:57:04.000000 ipgogogo-1.1.0/ipgogogo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2024-04-14 10:57:04.000000 ipgogogo-1.1.0/ipgogogo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 10:57:04.000000 ipgogogo-1.1.0/ipgogogo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-14 10:57:04.000000 ipgogogo-1.1.0/ipgogogo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-14 10:57:04.000000 ipgogogo-1.1.0/ipgogogo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 10:57:04.921513 ipgogogo-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     4349 2024-04-14 10:56:43.000000 ipgogogo-1.1.0/setup.py
```

### Comparing `ipgogogo-1.0.3/LICENSE` & `ipgogogo-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipgogogo-1.0.3/PKG-INFO` & `ipgogogo-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipgogogo
-Version: 1.0.3
+Version: 1.1.0
 Summary: I(mage) to P(df) Go Go Go!
 Home-page: https://github.com/keyork/ipgogogo
 Author: Keyork
 Author-email: chengky18@icloud.com
 License: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -50,7 +50,11 @@
 ```
 
 ### for source code
 
 ```shell
 python ipgogogo/run.py -i {input files dir path} -o {output files dir path} -l {log level}
 ```
+
+## TODO
+
+- [x] ui
```

### Comparing `ipgogogo-1.0.3/ipgogogo/__init__.py` & `ipgogogo-1.1.0/ipgogogo/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 
 from .core.core import Core
 from .model.state import CoreState
 from .utils.checkdir import is_bottom_dir
 from .utils.logger import init_logger
+from .ui import run
 
 
 class IPGoGoGo:
 
     def __init__(self, input_path: str, output_path: str, loglevel: str = "INFO"):
         self.input_path = input_path
         self.output_path = output_path
@@ -35,7 +36,11 @@
 
     def run(self):
         self.core_state.init_input_path(self.input_path)
         self.core_state.init_output_path(self.output_path)
         self.logger = init_logger(self.loglevel)
         self.core_state.init_logger(self.logger)
         self.run_multi()
+
+
+def run_ui():
+    run()
```

### Comparing `ipgogogo-1.0.3/ipgogogo/core/core.py` & `ipgogogo-1.1.0/ipgogogo/core/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 @ Author         :  Keyork
 @ Version        :  0.1
 @ Contact        :  chengky18@icloud.com
 @ Description    :  None
 @ History        :  0.1(2024/04/14) - None(Keyork)
 """
 
-from ..model.state import CoreState
+from ipgogogo.model.state import CoreState
 
 from .rcore import RCore
 from .wcore import WCore
 
 
 class Core:
```

### Comparing `ipgogogo-1.0.3/ipgogogo/core/rcore.py` & `ipgogogo-1.1.0/ipgogogo/core/rcore.py`

 * *Files identical despite different names*

### Comparing `ipgogogo-1.0.3/ipgogogo/core/wcore.py` & `ipgogogo-1.1.0/ipgogogo/core/wcore.py`

 * *Files identical despite different names*

### Comparing `ipgogogo-1.0.3/ipgogogo/model/state.py` & `ipgogogo-1.1.0/ipgogogo/model/state.py`

 * *Files identical despite different names*

### Comparing `ipgogogo-1.0.3/ipgogogo/run.py` & `ipgogogo-1.1.0/ipgogogo/run.py`

 * *Files identical despite different names*

### Comparing `ipgogogo-1.0.3/ipgogogo/utils/checkdir.py` & `ipgogogo-1.1.0/ipgogogo/utils/checkdir.py`

 * *Files identical despite different names*

### Comparing `ipgogogo-1.0.3/ipgogogo/utils/logger.py` & `ipgogogo-1.1.0/ipgogogo/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ipgogogo-1.0.3/ipgogogo.egg-info/PKG-INFO` & `ipgogogo-1.1.0/ipgogogo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipgogogo
-Version: 1.0.3
+Version: 1.1.0
 Summary: I(mage) to P(df) Go Go Go!
 Home-page: https://github.com/keyork/ipgogogo
 Author: Keyork
 Author-email: chengky18@icloud.com
 License: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -50,7 +50,11 @@
 ```
 
 ### for source code
 
 ```shell
 python ipgogogo/run.py -i {input files dir path} -o {output files dir path} -l {log level}
 ```
+
+## TODO
+
+- [x] ui
```

### Comparing `ipgogogo-1.0.3/setup.py` & `ipgogogo-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # Package meta-data.
 NAME = "ipgogogo"
 DESCRIPTION = "I(mage) to P(df) Go Go Go!"
 URL = "https://github.com/keyork/ipgogogo"
 EMAIL = "chengky18@icloud.com"
 AUTHOR = "Keyork"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "1.0.3"
+VERSION = "1.1.0"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "pillow",
     "loguru",
 ]
```

