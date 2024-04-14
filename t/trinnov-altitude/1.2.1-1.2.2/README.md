# Comparing `tmp/trinnov_altitude-1.2.1.tar.gz` & `tmp/trinnov_altitude-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trinnov_altitude-1.2.1.tar", last modified: Sat Apr 13 19:14:31 2024, max compression
+gzip compressed data, was "trinnov_altitude-1.2.2.tar", last modified: Sat Apr 13 19:30:42 2024, max compression
```

## Comparing `trinnov_altitude-1.2.1.tar` & `trinnov_altitude-1.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:14:31.572385 trinnov_altitude-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-04-13 19:14:31.572385 trinnov_altitude-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-13 19:14:31.572385 trinnov_altitude-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:14:31.568385 trinnov_altitude-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/tests/test_trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:14:31.568385 trinnov_altitude-1.2.1/trinnov_altitude/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/trinnov_altitude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/trinnov_altitude/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/trinnov_altitude/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/trinnov_altitude/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/trinnov_altitude/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    26143 2024-04-13 19:14:27.000000 trinnov_altitude-1.2.1/trinnov_altitude/trinnov_altitude.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:14:31.572385 trinnov_altitude-1.2.1/trinnov_altitude.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-04-13 19:14:31.000000 trinnov_altitude-1.2.1/trinnov_altitude.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-13 19:14:31.000000 trinnov_altitude-1.2.1/trinnov_altitude.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 19:14:31.000000 trinnov_altitude-1.2.1/trinnov_altitude.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 19:14:31.000000 trinnov_altitude-1.2.1/trinnov_altitude.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-13 19:14:31.000000 trinnov_altitude-1.2.1/trinnov_altitude.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:30:42.219280 trinnov_altitude-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-04-13 19:30:42.219280 trinnov_altitude-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-13 19:30:42.219280 trinnov_altitude-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:30:42.219280 trinnov_altitude-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/tests/test_trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:30:42.219280 trinnov_altitude-1.2.2/trinnov_altitude/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/trinnov_altitude/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/trinnov_altitude/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/trinnov_altitude/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/trinnov_altitude/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7531 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/trinnov_altitude/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26189 2024-04-13 19:30:37.000000 trinnov_altitude-1.2.2/trinnov_altitude/trinnov_altitude.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 19:30:42.219280 trinnov_altitude-1.2.2/trinnov_altitude.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-04-13 19:30:42.000000 trinnov_altitude-1.2.2/trinnov_altitude.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-13 19:30:42.000000 trinnov_altitude-1.2.2/trinnov_altitude.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 19:30:42.000000 trinnov_altitude-1.2.2/trinnov_altitude.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-13 19:30:42.000000 trinnov_altitude-1.2.2/trinnov_altitude.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-13 19:30:42.000000 trinnov_altitude-1.2.2/trinnov_altitude.egg-info/top_level.txt
```

### Comparing `trinnov_altitude-1.2.1/LICENSE` & `trinnov_altitude-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.2.1/PKG-INFO` & `trinnov_altitude-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trinnov-altitude
-Version: 1.2.1
+Version: 1.2.2
 Summary: "Python client for interfacing with the Trinnov Altitude processor."
 Home-page: https://github.com/binarylogic/py-trinnov-altitude
 Author: Ben Johnson
 Author-email: ben@binarylogic.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trinnov_altitude-1.2.1/README.md` & `trinnov_altitude-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.2.1/setup.cfg` & `trinnov_altitude-1.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.2.1/tests/test_trinnov_altitude.py` & `trinnov_altitude-1.2.2/tests/test_trinnov_altitude.py`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.2.1/trinnov_altitude/const.py` & `trinnov_altitude-1.2.2/trinnov_altitude/const.py`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.2.1/trinnov_altitude/exceptions.py` & `trinnov_altitude-1.2.2/trinnov_altitude/exceptions.py`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.2.1/trinnov_altitude/messages.py` & `trinnov_altitude-1.2.2/trinnov_altitude/messages.py`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.2.1/trinnov_altitude/mocks.py` & `trinnov_altitude-1.2.2/trinnov_altitude/mocks.py`

 * *Files identical despite different names*

### Comparing `trinnov_altitude-1.2.1/trinnov_altitude/trinnov_altitude.py` & `trinnov_altitude-1.2.2/trinnov_altitude/trinnov_altitude.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,14 +83,15 @@
         self.decoder: str | None = None
         self.dim: bool | None = None
         self.id: str | None = None
         self.mute: bool | None = None
         self.preset: str | None = None
         self.presets: dict[int, str] = {}
         self.source: str | None = None
+        self.source_format: str | None = None
         self.sources: dict[int, str] = {}
         self.upmixer: str | None = None
         self.version: str | None = None
         self.volume: float | None = None
 
         # Utility
         self._callbacks: set[Callback] = set()
```

### Comparing `trinnov_altitude-1.2.1/trinnov_altitude.egg-info/PKG-INFO` & `trinnov_altitude-1.2.2/trinnov_altitude.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trinnov-altitude
-Version: 1.2.1
+Version: 1.2.2
 Summary: "Python client for interfacing with the Trinnov Altitude processor."
 Home-page: https://github.com/binarylogic/py-trinnov-altitude
 Author: Ben Johnson
 Author-email: ben@binarylogic.com
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

