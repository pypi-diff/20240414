# Comparing `tmp/swpclib-4.2.0.tar.gz` & `tmp/swpclib-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swpclib-4.2.0.tar", last modified: Sat Apr  6 04:33:35 2024, max compression
+gzip compressed data, was "swpclib-4.3.0.tar", last modified: Sun Apr 14 21:16:59 2024, max compression
```

## Comparing `swpclib-4.2.0.tar` & `swpclib-4.3.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:33:35.356449 swpclib-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-06 04:33:26.000000 swpclib-4.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-06 04:33:26.000000 swpclib-4.2.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-06 04:33:26.000000 swpclib-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-06 04:33:26.000000 swpclib-4.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-06 04:33:35.356449 swpclib-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-06 04:33:26.000000 swpclib-4.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:33:35.352449 swpclib-4.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-06 04:33:26.000000 swpclib-4.2.0/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (127)     4835 2024-04-06 04:33:26.000000 swpclib-4.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-06 04:33:26.000000 swpclib-4.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-06 04:33:26.000000 swpclib-4.2.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-06 04:33:26.000000 swpclib-4.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-06 04:33:26.000000 swpclib-4.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-06 04:33:26.000000 swpclib-4.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-06 04:33:26.000000 swpclib-4.2.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-06 04:33:26.000000 swpclib-4.2.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-06 04:33:26.000000 swpclib-4.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-06 04:33:35.356449 swpclib-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-06 04:33:26.000000 swpclib-4.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:33:35.352449 swpclib-4.2.0/swpclib/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-06 04:33:26.000000 swpclib-4.2.0/swpclib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-04-06 04:33:26.000000 swpclib-4.2.0/swpclib/alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-06 04:33:26.000000 swpclib-4.2.0/swpclib/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-04-06 04:33:26.000000 swpclib-4.2.0/swpclib/swpclib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:33:35.356449 swpclib-4.2.0/swpclib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-06 04:33:35.000000 swpclib-4.2.0/swpclib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-06 04:33:35.000000 swpclib-4.2.0/swpclib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 04:33:35.000000 swpclib-4.2.0/swpclib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-06 04:33:35.000000 swpclib-4.2.0/swpclib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-06 04:33:35.000000 swpclib-4.2.0/swpclib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 04:33:35.000000 swpclib-4.2.0/swpclib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 04:33:35.356449 swpclib-4.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-06 04:33:26.000000 swpclib-4.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-06 04:33:26.000000 swpclib-4.2.0/tests/test_swpclib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:16:59.206661 swpclib-4.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-14 21:16:48.000000 swpclib-4.3.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-14 21:16:48.000000 swpclib-4.3.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-14 21:16:48.000000 swpclib-4.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-14 21:16:48.000000 swpclib-4.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-14 21:16:59.206661 swpclib-4.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-14 21:16:48.000000 swpclib-4.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:16:59.202661 swpclib-4.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-14 21:16:48.000000 swpclib-4.3.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4835 2024-04-14 21:16:48.000000 swpclib-4.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-14 21:16:48.000000 swpclib-4.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-14 21:16:48.000000 swpclib-4.3.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-14 21:16:48.000000 swpclib-4.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-14 21:16:48.000000 swpclib-4.3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-14 21:16:48.000000 swpclib-4.3.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-14 21:16:48.000000 swpclib-4.3.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-14 21:16:48.000000 swpclib-4.3.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-14 21:16:48.000000 swpclib-4.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-14 21:16:59.206661 swpclib-4.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-14 21:16:48.000000 swpclib-4.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:16:59.202661 swpclib-4.3.0/swpclib/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-14 21:16:48.000000 swpclib-4.3.0/swpclib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-04-14 21:16:48.000000 swpclib-4.3.0/swpclib/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-14 21:16:48.000000 swpclib-4.3.0/swpclib/animate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-04-14 21:16:48.000000 swpclib-4.3.0/swpclib/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8167 2024-04-14 21:16:48.000000 swpclib-4.3.0/swpclib/swpclib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:16:59.206661 swpclib-4.3.0/swpclib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-14 21:16:59.000000 swpclib-4.3.0/swpclib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-14 21:16:59.000000 swpclib-4.3.0/swpclib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:16:59.000000 swpclib-4.3.0/swpclib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-14 21:16:59.000000 swpclib-4.3.0/swpclib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-14 21:16:59.000000 swpclib-4.3.0/swpclib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 21:16:59.000000 swpclib-4.3.0/swpclib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:16:59.206661 swpclib-4.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-14 21:16:48.000000 swpclib-4.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-14 21:16:48.000000 swpclib-4.3.0/tests/test_swpclib.py
```

### Comparing `swpclib-4.2.0/CONTRIBUTING.rst` & `swpclib-4.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `swpclib-4.2.0/LICENSE` & `swpclib-4.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swpclib-4.2.0/docs/Makefile` & `swpclib-4.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `swpclib-4.2.0/docs/conf.py` & `swpclib-4.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.2.0/docs/installation.rst` & `swpclib-4.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `swpclib-4.2.0/docs/make.bat` & `swpclib-4.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `swpclib-4.2.0/swpclib/alerts.py` & `swpclib-4.3.0/swpclib/alerts.py`

 * *Files identical despite different names*

### Comparing `swpclib-4.2.0/swpclib.egg-info/SOURCES.txt` & `swpclib-4.3.0/swpclib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/readme.rst
 docs/usage.rst
 swpclib/__init__.py
 swpclib/alerts.py
+swpclib/animate.py
 swpclib/cli.py
 swpclib/swpclib.py
 swpclib.egg-info/PKG-INFO
 swpclib.egg-info/SOURCES.txt
 swpclib.egg-info/dependency_links.txt
 swpclib.egg-info/entry_points.txt
 swpclib.egg-info/requires.txt
```

### Comparing `swpclib-4.2.0/tests/test_swpclib.py` & `swpclib-4.3.0/tests/test_swpclib.py`

 * *Files identical despite different names*

