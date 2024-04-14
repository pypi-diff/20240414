# Comparing `tmp/colcon-meson-0.4.4.tar.gz` & `tmp/colcon-meson-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colcon-meson-0.4.4.tar", last modified: Wed Apr 10 17:06:04 2024, max compression
+gzip compressed data, was "colcon-meson-0.4.5.tar", last modified: Sun Apr 14 18:42:47 2024, max compression
```

## Comparing `colcon-meson-0.4.4.tar` & `colcon-meson-0.4.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-04-10 17:06:04.465613 colcon-meson-0.4.4/
--rw-rw-r--   0 christian  (1000) christian  (1000)    11357 2024-03-31 16:27:09.000000 colcon-meson-0.4.4/LICENSE
--rw-rw-r--   0 christian  (1000) christian  (1000)     1094 2024-04-10 17:06:04.469612 colcon-meson-0.4.4/PKG-INFO
--rw-rw-r--   0 christian  (1000) christian  (1000)      630 2024-03-31 16:27:09.000000 colcon-meson-0.4.4/README.md
-drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-04-10 17:06:04.465613 colcon-meson-0.4.4/colcon_meson/
--rw-rw-r--   0 christian  (1000) christian  (1000)        0 2024-03-31 16:27:09.000000 colcon-meson-0.4.4/colcon_meson/__init__.py
--rw-rw-r--   0 christian  (1000) christian  (1000)    10717 2024-04-08 20:24:44.000000 colcon-meson-0.4.4/colcon_meson/build.py
--rw-rw-r--   0 christian  (1000) christian  (1000)     4737 2024-04-10 17:04:02.000000 colcon-meson-0.4.4/colcon_meson/identification.py
-drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-04-10 17:06:04.465613 colcon-meson-0.4.4/colcon_meson.egg-info/
--rw-rw-r--   0 christian  (1000) christian  (1000)     1094 2024-04-10 17:06:04.000000 colcon-meson-0.4.4/colcon_meson.egg-info/PKG-INFO
--rw-rw-r--   0 christian  (1000) christian  (1000)      436 2024-04-10 17:06:04.000000 colcon-meson-0.4.4/colcon_meson.egg-info/SOURCES.txt
--rw-rw-r--   0 christian  (1000) christian  (1000)        1 2024-04-10 17:06:04.000000 colcon-meson-0.4.4/colcon_meson.egg-info/dependency_links.txt
--rw-rw-r--   0 christian  (1000) christian  (1000)      217 2024-04-10 17:06:04.000000 colcon-meson-0.4.4/colcon_meson.egg-info/entry_points.txt
--rw-rw-r--   0 christian  (1000) christian  (1000)      280 2024-04-10 17:06:04.000000 colcon-meson-0.4.4/colcon_meson.egg-info/requires.txt
--rw-rw-r--   0 christian  (1000) christian  (1000)       13 2024-04-10 17:06:04.000000 colcon-meson-0.4.4/colcon_meson.egg-info/top_level.txt
--rw-rw-r--   0 christian  (1000) christian  (1000)     1278 2024-04-10 17:06:04.469612 colcon-meson-0.4.4/setup.cfg
--rw-rw-r--   0 christian  (1000) christian  (1000)      121 2024-04-08 20:24:44.000000 colcon-meson-0.4.4/setup.py
-drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-04-10 17:06:04.465613 colcon-meson-0.4.4/test/
--rw-rw-r--   0 christian  (1000) christian  (1000)     1339 2024-04-08 20:24:44.000000 colcon-meson-0.4.4/test/test_copyright_license.py
--rw-rw-r--   0 christian  (1000) christian  (1000)     1899 2024-04-08 20:24:44.000000 colcon-meson-0.4.4/test/test_flake8.py
--rw-rw-r--   0 christian  (1000) christian  (1000)      549 2024-04-10 17:04:02.000000 colcon-meson-0.4.4/test/test_identification.py
--rw-rw-r--   0 christian  (1000) christian  (1000)     1929 2024-04-08 20:24:44.000000 colcon-meson-0.4.4/test/test_spell_check.py
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-04-14 18:42:47.005812 colcon-meson-0.4.5/
+-rw-rw-r--   0 christian  (1000) christian  (1000)    11357 2024-03-31 16:27:09.000000 colcon-meson-0.4.5/LICENSE
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1094 2024-04-14 18:42:47.005812 colcon-meson-0.4.5/PKG-INFO
+-rw-rw-r--   0 christian  (1000) christian  (1000)      630 2024-03-31 16:27:09.000000 colcon-meson-0.4.5/README.md
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-04-14 18:42:47.001811 colcon-meson-0.4.5/colcon_meson/
+-rw-rw-r--   0 christian  (1000) christian  (1000)        0 2024-03-31 16:27:09.000000 colcon-meson-0.4.5/colcon_meson/__init__.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)    10741 2024-04-14 18:41:26.000000 colcon-meson-0.4.5/colcon_meson/build.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     4737 2024-04-12 19:26:29.000000 colcon-meson-0.4.5/colcon_meson/identification.py
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-04-14 18:42:47.005812 colcon-meson-0.4.5/colcon_meson.egg-info/
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1094 2024-04-14 18:42:46.000000 colcon-meson-0.4.5/colcon_meson.egg-info/PKG-INFO
+-rw-rw-r--   0 christian  (1000) christian  (1000)      436 2024-04-14 18:42:46.000000 colcon-meson-0.4.5/colcon_meson.egg-info/SOURCES.txt
+-rw-rw-r--   0 christian  (1000) christian  (1000)        1 2024-04-14 18:42:46.000000 colcon-meson-0.4.5/colcon_meson.egg-info/dependency_links.txt
+-rw-rw-r--   0 christian  (1000) christian  (1000)      217 2024-04-14 18:42:46.000000 colcon-meson-0.4.5/colcon_meson.egg-info/entry_points.txt
+-rw-rw-r--   0 christian  (1000) christian  (1000)      280 2024-04-14 18:42:46.000000 colcon-meson-0.4.5/colcon_meson.egg-info/requires.txt
+-rw-rw-r--   0 christian  (1000) christian  (1000)       13 2024-04-14 18:42:46.000000 colcon-meson-0.4.5/colcon_meson.egg-info/top_level.txt
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1278 2024-04-14 18:42:47.005812 colcon-meson-0.4.5/setup.cfg
+-rw-rw-r--   0 christian  (1000) christian  (1000)      121 2024-04-08 20:24:44.000000 colcon-meson-0.4.5/setup.py
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-04-14 18:42:47.005812 colcon-meson-0.4.5/test/
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1339 2024-04-08 20:24:44.000000 colcon-meson-0.4.5/test/test_copyright_license.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1899 2024-04-08 20:24:44.000000 colcon-meson-0.4.5/test/test_flake8.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)      549 2024-04-10 17:04:02.000000 colcon-meson-0.4.5/test/test_identification.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1929 2024-04-08 20:24:44.000000 colcon-meson-0.4.5/test/test_spell_check.py
```

### Comparing `colcon-meson-0.4.4/LICENSE` & `colcon-meson-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `colcon-meson-0.4.4/PKG-INFO` & `colcon-meson-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colcon-meson
-Version: 0.4.4
+Version: 0.4.5
 Summary: Extension for colcon to support Meson packages.
 Author: Christian Rauch
 Author-email: Rauch.Christian@gmx.de
 Maintainer: Christian Rauch
 Maintainer-email: Rauch.Christian@gmx.de
 License: Apache License, Version 2.0
 Project-URL: GitHub, https://github.com/colcon/colcon-meson
```

### Comparing `colcon-meson-0.4.4/README.md` & `colcon-meson-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `colcon-meson-0.4.4/colcon_meson/build.py` & `colcon-meson-0.4.5/colcon_meson/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # Licensed under the Apache License, Version 2.0
 
 from argparse import ArgumentParser, Namespace
 import json
 import os
 from pathlib import Path
 import shutil
+from typing import List
 
 # colcon
 from colcon_core.environment import create_environment_scripts
 from colcon_core.logging import colcon_logger
 from colcon_core.shell import get_command_environment
 from colcon_core.task import run
 from colcon_core.task import TaskExtensionPoint
@@ -90,15 +91,15 @@
         """
         parser.add_argument('--meson-args',
                             nargs='*', metavar='*',
                             type=str.lstrip, default=[],
                             help="Pass 'setup' arguments to Meson projects.",
                             )
 
-    def get_default_args(self, args: Namespace) -> list[str]:
+    def get_default_args(self, args: Namespace) -> List[str]:
         """Get default Meson arguments.
 
         Args:
             args (Namespace): parse arguments from an ArgumentParser
 
         Returns:
             list: list of command line arguments for meson
@@ -117,28 +118,28 @@
 
         # positional arguments for 'builddir' and 'sourcedir'
         margs += [args.build_base]
         margs += [args.path]
 
         return margs
 
-    def meson_parse_cmdline(self, cmdline: list[str]) -> Namespace:
+    def meson_parse_cmdline(self, cmdline: List[str]) -> Namespace:
         """Parse command line arguments with the Meson arg parser.
 
         Args:
             cmdline (list): command line arguments
 
         Returns:
             Namespace: parse args
         """
         args = self.parser_setup.parse_args(cmdline)
         coredata.parse_cmd_line_options(args)
         return args
 
-    def meson_format_cmdline(self, cmdline: list[str]):
+    def meson_format_cmdline(self, cmdline: List[str]):
         """Convert Meson args from command line.
 
         Args:
             cmdline (list): command line arguments
 
         Returns:
             dict: converted key-value pairs
```

### Comparing `colcon-meson-0.4.4/colcon_meson/identification.py` & `colcon-meson-0.4.5/colcon_meson/identification.py`

 * *Files identical despite different names*

### Comparing `colcon-meson-0.4.4/colcon_meson.egg-info/PKG-INFO` & `colcon-meson-0.4.5/colcon_meson.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colcon-meson
-Version: 0.4.4
+Version: 0.4.5
 Summary: Extension for colcon to support Meson packages.
 Author: Christian Rauch
 Author-email: Rauch.Christian@gmx.de
 Maintainer: Christian Rauch
 Maintainer-email: Rauch.Christian@gmx.de
 License: Apache License, Version 2.0
 Project-URL: GitHub, https://github.com/colcon/colcon-meson
```

### Comparing `colcon-meson-0.4.4/setup.cfg` & `colcon-meson-0.4.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = colcon-meson
-version = 0.4.4
+version = 0.4.5
 project_urls = 
 	GitHub = https://github.com/colcon/colcon-meson
 author = Christian Rauch
 author_email = Rauch.Christian@gmx.de
 maintainer = Christian Rauch
 maintainer_email = Rauch.Christian@gmx.de
 license = Apache License, Version 2.0
```

### Comparing `colcon-meson-0.4.4/test/test_copyright_license.py` & `colcon-meson-0.4.5/test/test_copyright_license.py`

 * *Files identical despite different names*

### Comparing `colcon-meson-0.4.4/test/test_flake8.py` & `colcon-meson-0.4.5/test/test_flake8.py`

 * *Files identical despite different names*

### Comparing `colcon-meson-0.4.4/test/test_identification.py` & `colcon-meson-0.4.5/test/test_identification.py`

 * *Files identical despite different names*

### Comparing `colcon-meson-0.4.4/test/test_spell_check.py` & `colcon-meson-0.4.5/test/test_spell_check.py`

 * *Files identical despite different names*

