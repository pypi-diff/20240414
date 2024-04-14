# Comparing `tmp/swpclib-4.3.1.tar.gz` & `tmp/swpclib-4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swpclib-4.3.1.tar", last modified: Sun Apr 14 21:20:22 2024, max compression
+gzip compressed data, was "swpclib-4.3.2.tar", last modified: Sun Apr 14 21:35:19 2024, max compression
```

## Comparing `swpclib-4.3.1.tar` & `swpclib-4.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:20:22.005495 swpclib-4.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-14 21:20:11.000000 swpclib-4.3.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-14 21:20:11.000000 swpclib-4.3.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-14 21:20:11.000000 swpclib-4.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-14 21:20:11.000000 swpclib-4.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-14 21:20:22.005495 swpclib-4.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-14 21:20:11.000000 swpclib-4.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:20:22.001495 swpclib-4.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-14 21:20:11.000000 swpclib-4.3.1/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)     4835 2024-04-14 21:20:11.000000 swpclib-4.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-14 21:20:11.000000 swpclib-4.3.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-14 21:20:11.000000 swpclib-4.3.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-14 21:20:11.000000 swpclib-4.3.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-14 21:20:11.000000 swpclib-4.3.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-14 21:20:11.000000 swpclib-4.3.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-14 21:20:11.000000 swpclib-4.3.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-14 21:20:11.000000 swpclib-4.3.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-14 21:20:11.000000 swpclib-4.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-14 21:20:22.005495 swpclib-4.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-14 21:20:11.000000 swpclib-4.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:20:22.001495 swpclib-4.3.1/swpclib/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-14 21:20:11.000000 swpclib-4.3.1/swpclib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-04-14 21:20:11.000000 swpclib-4.3.1/swpclib/alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-14 21:20:11.000000 swpclib-4.3.1/swpclib/animate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-14 21:20:11.000000 swpclib-4.3.1/swpclib/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8167 2024-04-14 21:20:11.000000 swpclib-4.3.1/swpclib/swpclib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:20:22.005495 swpclib-4.3.1/swpclib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-14 21:20:21.000000 swpclib-4.3.1/swpclib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-14 21:20:21.000000 swpclib-4.3.1/swpclib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:20:21.000000 swpclib-4.3.1/swpclib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-14 21:20:21.000000 swpclib-4.3.1/swpclib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-14 21:20:21.000000 swpclib-4.3.1/swpclib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 21:20:21.000000 swpclib-4.3.1/swpclib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:20:22.001495 swpclib-4.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-14 21:20:11.000000 swpclib-4.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-14 21:20:11.000000 swpclib-4.3.1/tests/test_swpclib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:35:19.948348 swpclib-4.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-14 21:35:05.000000 swpclib-4.3.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-14 21:35:05.000000 swpclib-4.3.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-14 21:35:05.000000 swpclib-4.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-14 21:35:05.000000 swpclib-4.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-14 21:35:19.948348 swpclib-4.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-14 21:35:05.000000 swpclib-4.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:35:19.944348 swpclib-4.3.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-14 21:35:05.000000 swpclib-4.3.2/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4835 2024-04-14 21:35:05.000000 swpclib-4.3.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-14 21:35:05.000000 swpclib-4.3.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-14 21:35:05.000000 swpclib-4.3.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-14 21:35:05.000000 swpclib-4.3.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-14 21:35:05.000000 swpclib-4.3.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-14 21:35:05.000000 swpclib-4.3.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-14 21:35:05.000000 swpclib-4.3.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-14 21:35:05.000000 swpclib-4.3.2/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-14 21:35:05.000000 swpclib-4.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-14 21:35:19.948348 swpclib-4.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-14 21:35:05.000000 swpclib-4.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:35:19.948348 swpclib-4.3.2/swpclib/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-14 21:35:05.000000 swpclib-4.3.2/swpclib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-04-14 21:35:05.000000 swpclib-4.3.2/swpclib/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-14 21:35:05.000000 swpclib-4.3.2/swpclib/animate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-14 21:35:05.000000 swpclib-4.3.2/swpclib/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8167 2024-04-14 21:35:05.000000 swpclib-4.3.2/swpclib/swpclib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:35:19.948348 swpclib-4.3.2/swpclib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-14 21:35:19.000000 swpclib-4.3.2/swpclib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-14 21:35:19.000000 swpclib-4.3.2/swpclib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:35:19.000000 swpclib-4.3.2/swpclib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-14 21:35:19.000000 swpclib-4.3.2/swpclib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-14 21:35:19.000000 swpclib-4.3.2/swpclib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 21:35:19.000000 swpclib-4.3.2/swpclib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:35:19.948348 swpclib-4.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-14 21:35:05.000000 swpclib-4.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-14 21:35:05.000000 swpclib-4.3.2/tests/test_swpclib.py
```

### Comparing `swpclib-4.3.1/CONTRIBUTING.rst` & `swpclib-4.3.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.1/LICENSE` & `swpclib-4.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.1/docs/Makefile` & `swpclib-4.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.1/docs/conf.py` & `swpclib-4.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.1/docs/installation.rst` & `swpclib-4.3.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.1/docs/make.bat` & `swpclib-4.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.1/setup.cfg` & `swpclib-4.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.1/setup.py` & `swpclib-4.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.1/swpclib/alerts.py` & `swpclib-4.3.2/swpclib/alerts.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.1/swpclib/animate.py` & `swpclib-4.3.2/swpclib/animate.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.1/swpclib/cli.py` & `swpclib-4.3.2/swpclib/cli.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.1/swpclib/swpclib.py` & `swpclib-4.3.2/swpclib/swpclib.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.1/swpclib.egg-info/SOURCES.txt` & `swpclib-4.3.2/swpclib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swpclib-4.3.1/tests/test_swpclib.py` & `swpclib-4.3.2/tests/test_swpclib.py`

 * *Files identical despite different names*

