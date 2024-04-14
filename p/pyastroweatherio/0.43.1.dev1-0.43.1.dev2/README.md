# Comparing `tmp/pyastroweatherio-0.43.1.dev1.tar.gz` & `tmp/pyastroweatherio-0.43.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastroweatherio-0.43.1.dev1.tar", last modified: Thu Apr  4 15:29:42 2024, max compression
+gzip compressed data, was "pyastroweatherio-0.43.1.dev2.tar", last modified: Sun Apr 14 12:26:18 2024, max compression
```

## Comparing `pyastroweatherio-0.43.1.dev1.tar` & `pyastroweatherio-0.43.1.dev2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-04 15:29:42.766053 pyastroweatherio-0.43.1.dev1/
--rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev1/LICENSE
--rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-04 15:29:42.766053 pyastroweatherio-0.43.1.dev1/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.43.1.dev1/README.md
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-04 15:29:42.758052 pyastroweatherio-0.43.1.dev1/pyastroweatherio/
--rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev1/pyastroweatherio/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    32176 2024-04-04 13:56:28.000000 pyastroweatherio-0.43.1.dev1/pyastroweatherio/client.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     3638 2024-04-04 14:01:19.000000 pyastroweatherio-0.43.1.dev1/pyastroweatherio/const.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    20083 2024-04-04 14:08:15.000000 pyastroweatherio-0.43.1.dev1/pyastroweatherio/dataclasses.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.43.1.dev1/pyastroweatherio/errors.py
--rw-rw-r--   0 markus    (1000) markus    (1000)    32312 2023-11-12 10:53:43.000000 pyastroweatherio-0.43.1.dev1/pyastroweatherio/helper_functions.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-04 15:29:42.766053 pyastroweatherio-0.43.1.dev1/pyastroweatherio.egg-info/
--rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-04 15:29:42.000000 pyastroweatherio-0.43.1.dev1/pyastroweatherio.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-04-04 15:29:42.000000 pyastroweatherio-0.43.1.dev1/pyastroweatherio.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-04-04 15:29:42.000000 pyastroweatherio-0.43.1.dev1/pyastroweatherio.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-04-04 15:29:42.000000 pyastroweatherio-0.43.1.dev1/pyastroweatherio.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-04-04 15:29:42.000000 pyastroweatherio-0.43.1.dev1/pyastroweatherio.egg-info/top_level.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-04-04 15:29:42.766053 pyastroweatherio-0.43.1.dev1/setup.cfg
--rw-rw-r--   0 markus    (1000) markus    (1000)     1340 2024-04-04 15:28:31.000000 pyastroweatherio-0.43.1.dev1/setup.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-14 12:26:18.910754 pyastroweatherio-0.43.1.dev2/
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1071 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev2/LICENSE
+-rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-14 12:26:18.910754 pyastroweatherio-0.43.1.dev2/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1576 2023-10-06 18:49:53.000000 pyastroweatherio-0.43.1.dev2/README.md
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-14 12:26:18.906754 pyastroweatherio-0.43.1.dev2/pyastroweatherio/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-04-10 18:40:11.000000 pyastroweatherio-0.43.1.dev2/pyastroweatherio/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    32176 2024-04-04 13:56:28.000000 pyastroweatherio-0.43.1.dev2/pyastroweatherio/client.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     3638 2024-04-04 14:01:19.000000 pyastroweatherio-0.43.1.dev2/pyastroweatherio/const.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    20074 2024-04-14 12:24:57.000000 pyastroweatherio-0.43.1.dev2/pyastroweatherio/dataclasses.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      337 2023-11-05 13:15:24.000000 pyastroweatherio-0.43.1.dev2/pyastroweatherio/errors.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    32312 2023-11-12 10:53:43.000000 pyastroweatherio-0.43.1.dev2/pyastroweatherio/helper_functions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2024-04-14 12:26:18.910754 pyastroweatherio-0.43.1.dev2/pyastroweatherio.egg-info/
+-rw-r--r--   0 markus    (1000) markus    (1000)     1042 2024-04-14 12:26:18.000000 pyastroweatherio-0.43.1.dev2/pyastroweatherio.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      413 2024-04-14 12:26:18.000000 pyastroweatherio-0.43.1.dev2/pyastroweatherio.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2024-04-14 12:26:18.000000 pyastroweatherio-0.43.1.dev2/pyastroweatherio.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       16 2024-04-14 12:26:18.000000 pyastroweatherio-0.43.1.dev2/pyastroweatherio.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       17 2024-04-14 12:26:18.000000 pyastroweatherio-0.43.1.dev2/pyastroweatherio.egg-info/top_level.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       79 2024-04-14 12:26:18.910754 pyastroweatherio-0.43.1.dev2/setup.cfg
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1340 2024-04-14 12:26:13.000000 pyastroweatherio-0.43.1.dev2/setup.py
```

### Comparing `pyastroweatherio-0.43.1.dev1/LICENSE` & `pyastroweatherio-0.43.1.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev1/PKG-INFO` & `pyastroweatherio-0.43.1.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.43.1.dev1
+Version: 0.43.1.dev2
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.43.1.dev1/README.md` & `pyastroweatherio-0.43.1.dev2/README.md`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev1/pyastroweatherio/client.py` & `pyastroweatherio-0.43.1.dev2/pyastroweatherio/client.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev1/pyastroweatherio/const.py` & `pyastroweatherio-0.43.1.dev2/pyastroweatherio/const.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev1/pyastroweatherio/dataclasses.py` & `pyastroweatherio-0.43.1.dev2/pyastroweatherio/dataclasses.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 
     @property
     def wind10m_speed(self) -> float:
         """Return 10m Wind Speed."""
         return self._wind_speed
 
     @property
-    def wind10m_speed_percentage(self) -> int:
+    def calm_percentage(self) -> int:
         """Return 10m Wind Speed."""
         return int((100 + 100 / 7 - self._wind_speed * 100 / 7))
     
     @property
     def wind10m_direction(self) -> str:
         """Return 10m Wind Direction."""
         direction = self._wind_from_direction
```

### Comparing `pyastroweatherio-0.43.1.dev1/pyastroweatherio/helper_functions.py` & `pyastroweatherio-0.43.1.dev2/pyastroweatherio/helper_functions.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.43.1.dev1/pyastroweatherio.egg-info/PKG-INFO` & `pyastroweatherio-0.43.1.dev2/pyastroweatherio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.43.1.dev1
+Version: 0.43.1.dev2
 Summary: Python Wrapper for 7Timer and Met.no REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Met.no,Python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyastroweatherio-0.43.1.dev1/setup.py` & `pyastroweatherio-0.43.1.dev2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="pyastroweatherio",
     packages=["pyastroweatherio"],
-    version="0.43.1.dev1",
+    version="0.43.1.dev2",
     license="MIT",
     description="Python Wrapper for 7Timer and Met.no REST API",
     long_description=" ".join(
         [
             "Lightweight Python 3 module to receive data via",
             "REST API from 7Timer and Met.no.",
         ],
```

