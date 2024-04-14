# Comparing `tmp/potaahto-0.1.1.tar.gz` & `tmp/potaahto-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "potaahto-0.1.1.tar", last modified: Sun Jan 30 23:36:38 2022, max compression
+gzip compressed data, was "potaahto-0.1.2.tar", last modified: Sun Apr 14 13:36:14 2024, max compression
```

## Comparing `potaahto-0.1.1.tar` & `potaahto-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-01-30 23:36:38.655591 potaahto-0.1.1/
--rw-r--r--   0 lash      (1000) lash      (1000)      498 2021-10-31 05:57:02.000000 potaahto-0.1.1/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)      664 2022-01-30 23:36:38.655591 potaahto-0.1.1/PKG-INFO
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-01-30 23:36:38.655591 potaahto-0.1.1/potaahto/
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-04-14 11:47:32.000000 potaahto-0.1.1/potaahto/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1225 2022-01-28 03:43:34.000000 potaahto-0.1.1/potaahto/symbols.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-01-30 23:36:38.655591 potaahto-0.1.1/potaahto.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      664 2022-01-30 23:36:38.000000 potaahto-0.1.1/potaahto.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      195 2022-01-30 23:36:38.000000 potaahto-0.1.1/potaahto.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2022-01-30 23:36:38.000000 potaahto-0.1.1/potaahto.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        9 2022-01-30 23:36:38.000000 potaahto-0.1.1/potaahto.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      662 2022-01-30 23:36:38.655591 potaahto-0.1.1/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      508 2021-04-14 11:58:40.000000 potaahto-0.1.1/setup.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-14 13:36:14.156644 potaahto-0.1.2/
+-rw-r--r--   0 lash      (1000) lash      (1000)      498 2021-10-31 05:57:02.000000 potaahto-0.1.2/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)      636 2024-04-14 13:36:14.156644 potaahto-0.1.2/PKG-INFO
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-14 13:36:14.156644 potaahto-0.1.2/potaahto/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-04-14 11:47:32.000000 potaahto-0.1.2/potaahto/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1737 2024-04-14 13:34:54.000000 potaahto-0.1.2/potaahto/symbols.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-14 13:36:14.156644 potaahto-0.1.2/potaahto.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      636 2024-04-14 13:36:14.000000 potaahto-0.1.2/potaahto.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      215 2024-04-14 13:36:14.000000 potaahto-0.1.2/potaahto.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2024-04-14 13:36:14.000000 potaahto-0.1.2/potaahto.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2024-04-14 13:36:14.000000 potaahto-0.1.2/potaahto.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      662 2024-04-14 13:36:14.156644 potaahto-0.1.2/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      508 2021-04-14 11:58:40.000000 potaahto-0.1.2/setup.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-14 13:36:14.156644 potaahto-0.1.2/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2356 2024-04-14 13:34:54.000000 potaahto-0.1.2/tests/test_basic.py
```

### Comparing `potaahto-0.1.1/PKG-INFO` & `potaahto-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: potaahto
-Version: 0.1.1
+Version: 0.1.2
 Summary: Conversions and redundancy for poor data formatting choices
 Home-page: https://gitlab.com/nolash/chainlib
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: WTFPL
 Keywords: lint,code,formatting
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.6
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `potaahto-0.1.1/potaahto.egg-info/PKG-INFO` & `potaahto-0.1.2/potaahto.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: potaahto
-Version: 0.1.1
+Version: 0.1.2
 Summary: Conversions and redundancy for poor data formatting choices
 Home-page: https://gitlab.com/nolash/chainlib
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: WTFPL
 Keywords: lint,code,formatting
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.6
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `potaahto-0.1.1/setup.cfg` & `potaahto-0.1.2/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = potaahto
-version = 0.1.1
+version = 0.1.2
 description = Conversions and redundancy for poor data formatting choices
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://gitlab.com/nolash/chainlib
 keywords = 
 	lint
 	code
```

