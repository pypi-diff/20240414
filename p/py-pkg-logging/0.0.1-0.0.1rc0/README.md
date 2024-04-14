# Comparing `tmp/py_pkg_logging-0.0.1.tar.gz` & `tmp/py_pkg_logging-0.0.1rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_pkg_logging-0.0.1.tar", last modified: Sun Apr 14 18:17:47 2024, max compression
+gzip compressed data, was "py_pkg_logging-0.0.1rc0.tar", last modified: Sun Apr 14 18:14:27 2024, max compression
```

## Comparing `py_pkg_logging-0.0.1.tar` & `py_pkg_logging-0.0.1rc0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:17:47.349908 py_pkg_logging-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-14 18:17:47.349908 py_pkg_logging-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-14 18:17:38.000000 py_pkg_logging-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:17:47.349908 py_pkg_logging-0.0.1/py_pkg_logging/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-14 18:17:38.000000 py_pkg_logging-0.0.1/py_pkg_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-14 18:17:38.000000 py_pkg_logging-0.0.1/py_pkg_logging/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-14 18:17:38.000000 py_pkg_logging-0.0.1/py_pkg_logging/_log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-14 18:17:38.000000 py_pkg_logging-0.0.1/py_pkg_logging/_log_function_call.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:17:47.349908 py_pkg_logging-0.0.1/py_pkg_logging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-14 18:17:47.000000 py_pkg_logging-0.0.1/py_pkg_logging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-14 18:17:47.000000 py_pkg_logging-0.0.1/py_pkg_logging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 18:17:47.000000 py_pkg_logging-0.0.1/py_pkg_logging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-14 18:17:47.000000 py_pkg_logging-0.0.1/py_pkg_logging.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 18:17:47.349908 py_pkg_logging-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-14 18:17:38.000000 py_pkg_logging-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:14:27.385337 py_pkg_logging-0.0.1rc0/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-14 18:14:27.385337 py_pkg_logging-0.0.1rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-14 18:14:17.000000 py_pkg_logging-0.0.1rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:14:27.385337 py_pkg_logging-0.0.1rc0/py_pkg_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-14 18:14:17.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-14 18:14:17.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-04-14 18:14:17.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging/_log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-14 18:14:17.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging/_log_function_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:14:27.385337 py_pkg_logging-0.0.1rc0/py_pkg_logging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-14 18:14:27.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-14 18:14:27.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 18:14:27.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-14 18:14:27.000000 py_pkg_logging-0.0.1rc0/py_pkg_logging.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 18:14:27.389337 py_pkg_logging-0.0.1rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-14 18:14:17.000000 py_pkg_logging-0.0.1rc0/setup.py
```

### Comparing `py_pkg_logging-0.0.1/PKG-INFO` & `py_pkg_logging-0.0.1rc0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_pkg_logging
-Version: 0.0.1
+Version: 0.0.1rc0
 Summary: Python Package Logging Assistant.
 Home-page: https://github.com/mvinyard/py-pkg-logging
 Author: Michael E. Vinyard
 Author-email: mvinyard.ai@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `py_pkg_logging-0.0.1/py_pkg_logging/_log_config.py` & `py_pkg_logging-0.0.1rc0/py_pkg_logging/_log_config.py`

 * *Files identical despite different names*

### Comparing `py_pkg_logging-0.0.1/py_pkg_logging/_log_function_call.py` & `py_pkg_logging-0.0.1rc0/py_pkg_logging/_log_function_call.py`

 * *Files identical despite different names*

### Comparing `py_pkg_logging-0.0.1/py_pkg_logging.egg-info/PKG-INFO` & `py_pkg_logging-0.0.1rc0/py_pkg_logging.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_pkg_logging
-Version: 0.0.1
+Version: 0.0.1rc0
 Summary: Python Package Logging Assistant.
 Home-page: https://github.com/mvinyard/py-pkg-logging
 Author: Michael E. Vinyard
 Author-email: mvinyard.ai@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `py_pkg_logging-0.0.1/setup.py` & `py_pkg_logging-0.0.1rc0/setup.py`

 * *Files identical despite different names*

