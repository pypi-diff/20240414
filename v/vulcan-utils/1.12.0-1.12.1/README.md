# Comparing `tmp/vulcan-utils-1.12.0.tar.gz` & `tmp/vulcan-utils-1.12.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-utils-1.12.0.tar", last modified: Fri Apr 12 23:30:33 2024, max compression
+gzip compressed data, was "vulcan-utils-1.12.1.tar", last modified: Fri Apr 12 23:36:11 2024, max compression
```

## Comparing `vulcan-utils-1.12.0.tar` & `vulcan-utils-1.12.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:30:33.217128 vulcan-utils-1.12.0/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-12 23:30:33.217128 vulcan-utils-1.12.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 23:30:33.217128 vulcan-utils-1.12.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      384 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:30:33.217128 vulcan-utils-1.12.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/tests/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/tests/test_formatter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8171 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/tests/test_printable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:30:33.217128 vulcan-utils-1.12.0/vulcan_utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)       99 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/vulcan_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/vulcan_utils/cache.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9539 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/vulcan_utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/vulcan_utils/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/vulcan_utils/formatter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9285 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/vulcan_utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-12 23:30:25.000000 vulcan-utils-1.12.0/vulcan_utils/printable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:30:33.217128 vulcan-utils-1.12.0/vulcan_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-12 23:30:33.000000 vulcan-utils-1.12.0/vulcan_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-12 23:30:33.000000 vulcan-utils-1.12.0/vulcan_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 23:30:33.000000 vulcan-utils-1.12.0/vulcan_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 23:30:33.000000 vulcan-utils-1.12.0/vulcan_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 23:30:33.000000 vulcan-utils-1.12.0/vulcan_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:36:11.489630 vulcan-utils-1.12.1/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-12 23:36:11.489630 vulcan-utils-1.12.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 23:36:11.489630 vulcan-utils-1.12.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      384 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:36:11.485630 vulcan-utils-1.12.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8337 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/tests/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/tests/test_formatter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8171 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/tests/test_printable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:36:11.489630 vulcan-utils-1.12.1/vulcan_utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       99 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/vulcan_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/vulcan_utils/cache.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9539 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/vulcan_utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/vulcan_utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/vulcan_utils/formatter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9285 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/vulcan_utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-12 23:36:03.000000 vulcan-utils-1.12.1/vulcan_utils/printable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:36:11.489630 vulcan-utils-1.12.1/vulcan_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-04-12 23:36:11.000000 vulcan-utils-1.12.1/vulcan_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-12 23:36:11.000000 vulcan-utils-1.12.1/vulcan_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 23:36:11.000000 vulcan-utils-1.12.1/vulcan_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 23:36:11.000000 vulcan-utils-1.12.1/vulcan_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 23:36:11.000000 vulcan-utils-1.12.1/vulcan_utils.egg-info/top_level.txt
```

### Comparing `vulcan-utils-1.12.0/LICENSE` & `vulcan-utils-1.12.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan-utils-1.12.0/PKG-INFO` & `vulcan-utils-1.12.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-utils
-Version: 1.12.0
+Version: 1.12.1
 Summary: A utility package for Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 <!-- docs/README.md -->
 # Vulcan Utils
```

### Comparing `vulcan-utils-1.12.0/tests/test_cache.py` & `vulcan-utils-1.12.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `vulcan-utils-1.12.0/tests/test_decorator.py` & `vulcan-utils-1.12.1/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan-utils-1.12.0/tests/test_encoder.py` & `vulcan-utils-1.12.1/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan-utils-1.12.0/tests/test_formatter.py` & `vulcan-utils-1.12.1/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `vulcan-utils-1.12.0/tests/test_logger.py` & `vulcan-utils-1.12.1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `vulcan-utils-1.12.0/tests/test_printable.py` & `vulcan-utils-1.12.1/tests/test_printable.py`

 * *Files identical despite different names*

### Comparing `vulcan-utils-1.12.0/vulcan_utils/cache.py` & `vulcan-utils-1.12.1/vulcan_utils/cache.py`

 * *Files identical despite different names*

### Comparing `vulcan-utils-1.12.0/vulcan_utils/decorator.py` & `vulcan-utils-1.12.1/vulcan_utils/decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan-utils-1.12.0/vulcan_utils/encoder.py` & `vulcan-utils-1.12.1/vulcan_utils/encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan-utils-1.12.0/vulcan_utils/formatter.py` & `vulcan-utils-1.12.1/vulcan_utils/formatter.py`

 * *Files identical despite different names*

### Comparing `vulcan-utils-1.12.0/vulcan_utils/logger.py` & `vulcan-utils-1.12.1/vulcan_utils/logger.py`

 * *Files identical despite different names*

### Comparing `vulcan-utils-1.12.0/vulcan_utils/printable.py` & `vulcan-utils-1.12.1/vulcan_utils/printable.py`

 * *Files identical despite different names*

### Comparing `vulcan-utils-1.12.0/vulcan_utils.egg-info/PKG-INFO` & `vulcan-utils-1.12.1/vulcan_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-utils
-Version: 1.12.0
+Version: 1.12.1
 Summary: A utility package for Python
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 <!-- docs/README.md -->
 # Vulcan Utils
```

### Comparing `vulcan-utils-1.12.0/vulcan_utils.egg-info/SOURCES.txt` & `vulcan-utils-1.12.1/vulcan_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

