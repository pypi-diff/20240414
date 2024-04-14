# Comparing `tmp/archerdfu_bmp-1.0.0.tar.gz` & `tmp/archerdfu_bmp-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "archerdfu_bmp-1.0.0.tar", last modified: Sun Apr 14 13:51:52 2024, max compression
+gzip compressed data, was "archerdfu_bmp-1.0.1.tar", last modified: Sun Apr 14 14:33:32 2024, max compression
```

## Comparing `archerdfu_bmp-1.0.0.tar` & `archerdfu_bmp-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:51:52.490401 archerdfu_bmp-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-14 13:51:46.000000 archerdfu_bmp-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-14 13:51:46.000000 archerdfu_bmp-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    41757 2024-04-14 13:51:52.486401 archerdfu_bmp-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-14 13:51:46.000000 archerdfu_bmp-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:51:52.482401 archerdfu_bmp-1.0.0/archerdfu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:51:52.486401 archerdfu_bmp-1.0.0/archerdfu/bmp/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-14 13:51:46.000000 archerdfu_bmp-1.0.0/archerdfu/bmp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:51:52.486401 archerdfu_bmp-1.0.0/archerdfu/bmp/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-14 13:51:46.000000 archerdfu_bmp-1.0.0/archerdfu/bmp/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-14 13:51:46.000000 archerdfu_bmp-1.0.0/archerdfu/bmp/__pyinstaller/hook-archerdfu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-14 13:51:46.000000 archerdfu_bmp-1.0.0/archerdfu/bmp/caliber_icons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:51:52.486401 archerdfu_bmp-1.0.0/archerdfu/bmp/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-04-14 13:51:46.000000 archerdfu_bmp-1.0.0/archerdfu/bmp/fonts/default.flf
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-14 13:51:46.000000 archerdfu_bmp-1.0.0/archerdfu/bmp/fonts/pixel.flf
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-14 13:51:46.000000 archerdfu_bmp-1.0.0/archerdfu/bmp/processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:51:52.486401 archerdfu_bmp-1.0.0/archerdfu.bmp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    41757 2024-04-14 13:51:52.000000 archerdfu_bmp-1.0.0/archerdfu.bmp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-14 13:51:52.000000 archerdfu_bmp-1.0.0/archerdfu.bmp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 13:51:52.000000 archerdfu_bmp-1.0.0/archerdfu.bmp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-14 13:51:52.000000 archerdfu_bmp-1.0.0/archerdfu.bmp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 13:51:52.000000 archerdfu_bmp-1.0.0/archerdfu.bmp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-14 13:51:46.000000 archerdfu_bmp-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 13:51:52.490401 archerdfu_bmp-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 13:51:46.000000 archerdfu_bmp-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:51:52.486401 archerdfu_bmp-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-14 13:51:46.000000 archerdfu_bmp-1.0.0/tests/test_caliber_icons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:33:32.392895 archerdfu_bmp-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-14 14:33:23.000000 archerdfu_bmp-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-14 14:33:23.000000 archerdfu_bmp-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    41757 2024-04-14 14:33:32.392895 archerdfu_bmp-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-14 14:33:23.000000 archerdfu_bmp-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:33:32.388895 archerdfu_bmp-1.0.1/archerdfu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:33:32.392895 archerdfu_bmp-1.0.1/archerdfu/bmp/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-14 14:33:23.000000 archerdfu_bmp-1.0.1/archerdfu/bmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-14 14:33:23.000000 archerdfu_bmp-1.0.1/archerdfu/bmp/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:33:32.392895 archerdfu_bmp-1.0.1/archerdfu/bmp/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-14 14:33:23.000000 archerdfu_bmp-1.0.1/archerdfu/bmp/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-14 14:33:23.000000 archerdfu_bmp-1.0.1/archerdfu/bmp/__pyinstaller/hook-archerdfu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-14 14:33:23.000000 archerdfu_bmp-1.0.1/archerdfu/bmp/caliber_icons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:33:32.392895 archerdfu_bmp-1.0.1/archerdfu/bmp/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    10742 2024-04-14 14:33:23.000000 archerdfu_bmp-1.0.1/archerdfu/bmp/fonts/default.flf
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-14 14:33:23.000000 archerdfu_bmp-1.0.1/archerdfu/bmp/fonts/pixel.flf
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-14 14:33:23.000000 archerdfu_bmp-1.0.1/archerdfu/bmp/processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:33:32.392895 archerdfu_bmp-1.0.1/archerdfu.bmp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41757 2024-04-14 14:33:32.000000 archerdfu_bmp-1.0.1/archerdfu.bmp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-14 14:33:32.000000 archerdfu_bmp-1.0.1/archerdfu.bmp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 14:33:32.000000 archerdfu_bmp-1.0.1/archerdfu.bmp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-14 14:33:32.000000 archerdfu_bmp-1.0.1/archerdfu.bmp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-14 14:33:32.000000 archerdfu_bmp-1.0.1/archerdfu.bmp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 14:33:32.000000 archerdfu_bmp-1.0.1/archerdfu.bmp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-14 14:33:23.000000 archerdfu_bmp-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 14:33:32.392895 archerdfu_bmp-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 14:33:23.000000 archerdfu_bmp-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:33:32.392895 archerdfu_bmp-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-14 14:33:23.000000 archerdfu_bmp-1.0.1/tests/test_caliber_icons.py
```

### Comparing `archerdfu_bmp-1.0.0/LICENSE` & `archerdfu_bmp-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `archerdfu_bmp-1.0.0/PKG-INFO` & `archerdfu_bmp-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archerdfu.bmp
-Version: 1.0.0
+Version: 1.0.1
 Summary: PyDfuUtil binds for archerdfu library
 Author: o-murphy
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `archerdfu_bmp-1.0.0/archerdfu/bmp/caliber_icons.py` & `archerdfu_bmp-1.0.1/archerdfu/bmp/caliber_icons.py`

 * *Files identical despite different names*

### Comparing `archerdfu_bmp-1.0.0/archerdfu/bmp/fonts/default.flf` & `archerdfu_bmp-1.0.1/archerdfu/bmp/fonts/default.flf`

 * *Files identical despite different names*

### Comparing `archerdfu_bmp-1.0.0/archerdfu/bmp/fonts/pixel.flf` & `archerdfu_bmp-1.0.1/archerdfu/bmp/fonts/pixel.flf`

 * *Files identical despite different names*

### Comparing `archerdfu_bmp-1.0.0/archerdfu/bmp/processing.py` & `archerdfu_bmp-1.0.1/archerdfu/bmp/processing.py`

 * *Files identical despite different names*

### Comparing `archerdfu_bmp-1.0.0/archerdfu.bmp.egg-info/PKG-INFO` & `archerdfu_bmp-1.0.1/archerdfu.bmp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: archerdfu.bmp
-Version: 1.0.0
+Version: 1.0.1
 Summary: PyDfuUtil binds for archerdfu library
 Author: o-murphy
 License:  GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `archerdfu_bmp-1.0.0/pyproject.toml` & `archerdfu_bmp-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "archerdfu.bmp"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
     { name="o-murphy" },
 ]
 
 description = "PyDfuUtil binds for archerdfu library"
 readme = "README.md"
 requires-python = ">=3.9"
@@ -41,8 +41,11 @@
 
 [tool.setuptools]
 py-modules = ["archerdfu.bmp"]
 
 
 [tool.setuptools.packages.find]
 where = ["."]
-include = ["archerdfu*"]
+include = ["archerdfu*"]
+
+[project.scripts]
+archerdfu-icon = "archerdfu.bmp.__main__:main"
```

### Comparing `archerdfu_bmp-1.0.0/tests/test_caliber_icons.py` & `archerdfu_bmp-1.0.1/tests/test_caliber_icons.py`

 * *Files identical despite different names*

