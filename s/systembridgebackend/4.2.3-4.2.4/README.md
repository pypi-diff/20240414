# Comparing `tmp/systembridgebackend-4.2.3.tar.gz` & `tmp/systembridgebackend-4.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgebackend-4.2.3.tar", last modified: Wed Apr 10 01:03:46 2024, max compression
+gzip compressed data, was "systembridgebackend-4.2.4.tar", last modified: Sun Apr 14 12:23:05 2024, max compression
```

## Comparing `systembridgebackend-4.2.3.tar` & `systembridgebackend-4.2.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:03:46.754522 systembridgebackend-4.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-10 01:03:46.754522 systembridgebackend-4.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 01:03:46.754522 systembridgebackend-4.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:03:46.746523 systembridgebackend-4.2.3/systembridgebackend/
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-10 01:03:44.000000 systembridgebackend-4.2.3/systembridgebackend/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:03:46.746523 systembridgebackend-4.2.3/systembridgebackend/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/keyboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:03:46.746523 systembridgebackend-4.2.3/systembridgebackend/handlers/media/
--rw-r--r--   0 runner    (1001) docker     (127)    16367 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/media/windows.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/open.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/power.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:03:46.750522 systembridgebackend-4.2.3/systembridgebackend/handlers/threads/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/threads/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/threads/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/threads/update.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/handlers/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:03:46.750522 systembridgebackend-4.2.3/systembridgebackend/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/disks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/displays.py
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/gpus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/listeners.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/modules/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:03:46.750522 systembridgebackend-4.2.3/systembridgebackend/server/
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/server/mdns.py
--rw-r--r--   0 runner    (1001) docker     (127)    36941 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/systembridgebackend/server/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:03:46.754522 systembridgebackend-4.2.3/systembridgebackend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-10 01:03:46.000000 systembridgebackend-4.2.3/systembridgebackend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-10 01:03:46.000000 systembridgebackend-4.2.3/systembridgebackend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 01:03:46.000000 systembridgebackend-4.2.3/systembridgebackend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-10 01:03:46.000000 systembridgebackend-4.2.3/systembridgebackend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-10 01:03:46.000000 systembridgebackend-4.2.3/systembridgebackend.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:03:46.750522 systembridgebackend-4.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-10 01:00:58.000000 systembridgebackend-4.2.3/tests/test__version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:23:05.046157 systembridgebackend-4.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-14 12:23:05.046157 systembridgebackend-4.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 12:23:05.046157 systembridgebackend-4.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:23:05.038157 systembridgebackend-4.2.4/systembridgebackend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-14 12:23:02.000000 systembridgebackend-4.2.4/systembridgebackend/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:23:05.042158 systembridgebackend-4.2.4/systembridgebackend/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/keyboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:23:05.042158 systembridgebackend-4.2.4/systembridgebackend/handlers/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    16367 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/media/windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/power.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:23:05.042158 systembridgebackend-4.2.4/systembridgebackend/handlers/threads/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/threads/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/threads/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/threads/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/handlers/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:23:05.046157 systembridgebackend-4.2.4/systembridgebackend/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14935 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/disks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/displays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/gpus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8535 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13679 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/modules/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:23:05.046157 systembridgebackend-4.2.4/systembridgebackend/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/server/mdns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36941 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/systembridgebackend/server/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:23:05.046157 systembridgebackend-4.2.4/systembridgebackend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-14 12:23:04.000000 systembridgebackend-4.2.4/systembridgebackend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-14 12:23:05.000000 systembridgebackend-4.2.4/systembridgebackend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 12:23:04.000000 systembridgebackend-4.2.4/systembridgebackend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-14 12:23:04.000000 systembridgebackend-4.2.4/systembridgebackend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-14 12:23:04.000000 systembridgebackend-4.2.4/systembridgebackend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:23:05.046157 systembridgebackend-4.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-14 12:20:09.000000 systembridgebackend-4.2.4/tests/test__version.py
```

### Comparing `systembridgebackend-4.2.3/LICENSE` & `systembridgebackend-4.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/PKG-INFO` & `systembridgebackend-4.2.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: systembridgebackend
-Version: 4.2.3
+Version: 4.2.4
 Summary: System Bridge Backend
 Home-page: https://github.com/timmo001/system-bridge-backend
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiofiles==23.2.1
+Requires-Dist: aiohttp>=3.9.0b0
 Requires-Dist: fastapi==0.110.1
 Requires-Dist: incremental==22.10.0
 Requires-Dist: keyboard==0.13.5
 Requires-Dist: mutagen==1.47.0
 Requires-Dist: packaging>=24.0
 Requires-Dist: plyer==2.1.0
 Requires-Dist: psutil==5.9.8
```

### Comparing `systembridgebackend-4.2.3/pyproject.toml` & `systembridgebackend-4.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/setup.py` & `systembridgebackend-4.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/__init__.py` & `systembridgebackend-4.2.4/systembridgebackend/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/__main__.py` & `systembridgebackend-4.2.4/systembridgebackend/__main__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/handlers/action.py` & `systembridgebackend-4.2.4/systembridgebackend/handlers/action.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/handlers/data.py` & `systembridgebackend-4.2.4/systembridgebackend/handlers/data.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/handlers/keyboard.py` & `systembridgebackend-4.2.4/systembridgebackend/handlers/keyboard.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/handlers/media/__init__.py` & `systembridgebackend-4.2.4/systembridgebackend/handlers/media/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/handlers/media/windows.py` & `systembridgebackend-4.2.4/systembridgebackend/handlers/media/windows.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/handlers/power.py` & `systembridgebackend-4.2.4/systembridgebackend/handlers/power.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/handlers/threads/__init__.py` & `systembridgebackend-4.2.4/systembridgebackend/handlers/threads/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/handlers/threads/data.py` & `systembridgebackend-4.2.4/systembridgebackend/handlers/threads/data.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/handlers/threads/media.py` & `systembridgebackend-4.2.4/systembridgebackend/handlers/threads/media.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/handlers/threads/update.py` & `systembridgebackend-4.2.4/systembridgebackend/handlers/threads/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/modules/__init__.py` & `systembridgebackend-4.2.4/systembridgebackend/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/modules/battery.py` & `systembridgebackend-4.2.4/systembridgebackend/modules/battery.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/modules/cpu.py` & `systembridgebackend-4.2.4/systembridgebackend/modules/cpu.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     cpu_freq,
     cpu_percent,
     cpu_stats,
     cpu_times,
     cpu_times_percent,
     getloadavg,
 )
-from psutil._common import pcputimes, scpufreq, scpustats
+from psutil._common import pcputimes, scpufreq, scpustats, shwtemp
 
 from systembridgemodels.modules.cpu import CPU, CPUFrequency, CPUStats, CPUTimes, PerCPU
 from systembridgemodels.modules.sensors import Sensors
 
 from .base import ModuleUpdateBase
 
 
@@ -121,40 +121,65 @@
 
     async def _get_stats(self) -> scpustats:
         """CPU stats."""
         return cpu_stats()
 
     async def _get_temperature(self) -> float | None:
         """CPU temperature."""
-        if (
-            self.sensors is None
-            or self.sensors.windows_sensors is None
-            or self.sensors.windows_sensors.hardware is None
-        ):
-            return None
-        for hardware in self.sensors.windows_sensors.hardware:
-            # Find type "CPU"
-            if "CPU" not in hardware.type.upper():
-                continue
-            for sensor in hardware.sensors:
-                name = sensor.name.upper()
-                # Find type "TEMPERATURE" and name "PACKAGE" or "AVERAGE"
-                if (
-                    "TEMPERATURE" in sensor.type.upper()
-                    and ("PACKAGE" in name or "AVERAGE" in name)
-                    and sensor.value is not None
-                ):
-                    self._logger.debug(
-                        "Found CPU temperature: %s = %s", sensor.name, sensor.value
-                    )
-                    return (
-                        float(sensor.value)
-                        if isinstance(sensor.value, (int, float, str))
-                        else None
-                    )
+        if self.sensors is not None:
+            if self.sensors.temperatures is not None:
+                temperatures: dict[str, list[shwtemp]] = self.sensors.temperatures
+                if "k10temp" in temperatures:
+                    for sensor in self.sensors.temperatures["k10temp"]:
+                        self._logger.debug("k10temp: %s", sensor)
+                        if "Tdie" in sensor or "Tctl" in sensor or "Tccd1" in sensor:
+                            self._logger.debug(
+                                "Found CPU temperature (k10temp): %s",
+                                sensor,
+                            )
+                            return sensor.current
+                if "coretemp" in self.sensors.temperatures:
+                    for sensor in self.sensors.temperatures["coretemp"]:
+                        self._logger.debug("coretemp: %s", sensor)
+                        if (
+                            "Package id 0" in sensor
+                            or "Physical id 0" in sensor
+                            or "Core 0" in sensor
+                        ):
+                            self._logger.debug(
+                                "Found CPU temperature (coretemp): %s",
+                                sensor,
+                            )
+                            return sensor.current
+            if (
+                self.sensors.windows_sensors is not None
+                and self.sensors.windows_sensors.hardware is not None
+            ):
+                for hardware in self.sensors.windows_sensors.hardware:
+                    # Find type "CPU"
+                    if "CPU" not in hardware.type.upper():
+                        continue
+                    for sensor in hardware.sensors:
+                        name = sensor.name.upper()
+                        # Find type "TEMPERATURE" and name "PACKAGE" or "AVERAGE"
+                        if (
+                            "TEMPERATURE" in sensor.type.upper()
+                            and ("PACKAGE" in name or "AVERAGE" in name)
+                            and sensor.value is not None
+                        ):
+                            self._logger.debug(
+                                "Found CPU temperature: %s = %s",
+                                sensor.name,
+                                sensor.value,
+                            )
+                            return (
+                                float(sensor.value)
+                                if isinstance(sensor.value, (int, float, str))
+                                else None
+                            )
         return None
 
     async def _get_times(self) -> pcputimes:
         """CPU times."""
         return cpu_times(percpu=False)
 
     async def _get_times_percent(self) -> pcputimes:
```

### Comparing `systembridgebackend-4.2.3/systembridgebackend/modules/disks.py` & `systembridgebackend-4.2.4/systembridgebackend/modules/disks.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/modules/displays.py` & `systembridgebackend-4.2.4/systembridgebackend/modules/displays.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/modules/gpus.py` & `systembridgebackend-4.2.4/systembridgebackend/modules/gpus.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/modules/listeners.py` & `systembridgebackend-4.2.4/systembridgebackend/modules/listeners.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/modules/media.py` & `systembridgebackend-4.2.4/systembridgebackend/modules/media.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/modules/memory.py` & `systembridgebackend-4.2.4/systembridgebackend/modules/memory.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/modules/networks.py` & `systembridgebackend-4.2.4/systembridgebackend/modules/networks.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/modules/processes.py` & `systembridgebackend-4.2.4/systembridgebackend/modules/processes.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/modules/sensors.py` & `systembridgebackend-4.2.4/systembridgebackend/modules/sensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Sensors."""
 
 import asyncio
 import json
 import subprocess
 import sys
-from typing import Any
 
 import psutil
+from psutil._common import sfan, shwtemp
 
 from systembridgemodels.modules.sensors import (
     Sensors,
     SensorsNVIDIA,
     SensorsNVIDIAChipset,
     SensorsNVIDIADisplay,
     SensorsNVIDIADriver,
@@ -22,25 +22,25 @@
 
 from .base import ModuleUpdateBase
 
 
 class SensorsUpdate(ModuleUpdateBase):
     """Sensors Update."""
 
-    async def _get_fans(self) -> Any | None:
+    async def _get_fans(self) -> dict[str, list[sfan]] | None:
         """Get fans."""
         if not hasattr(psutil, "sensors_fans"):
             return None
         return psutil.sensors_fans()  # type: ignore
 
-    async def _get_temperatures(self) -> Any | None:
+    async def _get_temperatures(self) -> dict[str, list[shwtemp]] | None:
         """Get temperatures."""
         if not hasattr(psutil, "sensors_temperatures"):
             return None
-        return psutil.sensors_temperatures()  # type: ignore
+        return psutil.sensors_temperatures(fahrenheit=False)  # type: ignore
 
     async def _get_windows_sensors(self) -> dict | None:
         """Get windows sensors."""
         if sys.platform != "win32":
             return None
 
         try:
```

### Comparing `systembridgebackend-4.2.3/systembridgebackend/modules/system.py` & `systembridgebackend-4.2.4/systembridgebackend/modules/system.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/server/__init__.py` & `systembridgebackend-4.2.4/systembridgebackend/server/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/server/api.py` & `systembridgebackend-4.2.4/systembridgebackend/server/api.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/server/mdns.py` & `systembridgebackend-4.2.4/systembridgebackend/server/mdns.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend/server/websocket.py` & `systembridgebackend-4.2.4/systembridgebackend/server/websocket.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.3/systembridgebackend.egg-info/PKG-INFO` & `systembridgebackend-4.2.4/systembridgebackend.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: systembridgebackend
-Version: 4.2.3
+Version: 4.2.4
 Summary: System Bridge Backend
 Home-page: https://github.com/timmo001/system-bridge-backend
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiofiles==23.2.1
+Requires-Dist: aiohttp>=3.9.0b0
 Requires-Dist: fastapi==0.110.1
 Requires-Dist: incremental==22.10.0
 Requires-Dist: keyboard==0.13.5
 Requires-Dist: mutagen==1.47.0
 Requires-Dist: packaging>=24.0
 Requires-Dist: plyer==2.1.0
 Requires-Dist: psutil==5.9.8
```

### Comparing `systembridgebackend-4.2.3/systembridgebackend.egg-info/SOURCES.txt` & `systembridgebackend-4.2.4/systembridgebackend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

