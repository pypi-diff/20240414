# Comparing `tmp/libreppc-0.1.0.tar.gz` & `tmp/libreppc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreppc-0.1.0.tar", last modified: Sun Apr 14 16:03:52 2024, max compression
+gzip compressed data, was "libreppc-0.1.1.tar", last modified: Sun Apr 14 16:07:30 2024, max compression
```

## Comparing `libreppc-0.1.0.tar` & `libreppc-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 16:03:52.883189 libreppc-0.1.0/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1096 2024-02-23 10:09:06.000000 libreppc-0.1.0/LICENSE
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2261 2024-04-14 16:03:52.883189 libreppc-0.1.0/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1552 2024-02-23 13:06:45.000000 libreppc-0.1.0/README.md
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 16:03:52.883189 libreppc-0.1.0/libreppc/
--rw-r--r--   0 warlock   (1000) warlock   (1000)       48 2024-04-14 16:01:45.000000 libreppc-0.1.0/libreppc/__init__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)      705 2024-04-14 15:53:52.000000 libreppc-0.1.0/libreppc/__main__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     5427 2024-04-14 15:58:57.000000 libreppc-0.1.0/libreppc/libreppc.py
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 16:03:52.883189 libreppc-0.1.0/libreppc.egg-info/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2261 2024-04-14 16:03:52.000000 libreppc-0.1.0/libreppc.egg-info/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)      248 2024-04-14 16:03:52.000000 libreppc-0.1.0/libreppc.egg-info/SOURCES.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-04-14 16:03:52.000000 libreppc-0.1.0/libreppc.egg-info/dependency_links.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       28 2024-04-14 16:03:52.000000 libreppc-0.1.0/libreppc.egg-info/requires.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        9 2024-04-14 16:03:52.000000 libreppc-0.1.0/libreppc.egg-info/top_level.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-04-14 16:03:52.883189 libreppc-0.1.0/setup.cfg
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1070 2024-04-14 16:02:17.000000 libreppc-0.1.0/setup.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 16:07:30.342728 libreppc-0.1.1/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1096 2024-02-23 10:09:06.000000 libreppc-0.1.1/LICENSE
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2164 2024-04-14 16:07:30.342728 libreppc-0.1.1/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1455 2024-04-14 16:06:12.000000 libreppc-0.1.1/README.md
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 16:07:30.339395 libreppc-0.1.1/libreppc/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       48 2024-04-14 16:06:37.000000 libreppc-0.1.1/libreppc/__init__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      705 2024-04-14 15:53:52.000000 libreppc-0.1.1/libreppc/__main__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     5427 2024-04-14 15:58:57.000000 libreppc-0.1.1/libreppc/libreppc.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 16:07:30.339395 libreppc-0.1.1/libreppc.egg-info/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2164 2024-04-14 16:07:30.000000 libreppc-0.1.1/libreppc.egg-info/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      248 2024-04-14 16:07:30.000000 libreppc-0.1.1/libreppc.egg-info/SOURCES.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-04-14 16:07:30.000000 libreppc-0.1.1/libreppc.egg-info/dependency_links.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       28 2024-04-14 16:07:30.000000 libreppc-0.1.1/libreppc.egg-info/requires.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        9 2024-04-14 16:07:30.000000 libreppc-0.1.1/libreppc.egg-info/top_level.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-04-14 16:07:30.342728 libreppc-0.1.1/setup.cfg
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1070 2024-04-14 16:02:17.000000 libreppc-0.1.1/setup.py
```

### Comparing `libreppc-0.1.0/LICENSE` & `libreppc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.0/PKG-INFO` & `libreppc-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreppc
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple profile page creator.
 Home-page: https://codeberg.org/librehub/libreppc
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,profile,html,css,markdown,profile page,page,site,personal page
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -15,27 +15,26 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: flask
 Requires-Dist: markdown
 Requires-Dist: feedgen
 Requires-Dist: pytz
 
-# profiler 
+# libreppc 
 
-A simple profile page creator. 
+A simple profile page creator.
 
-![example](resources/profiler-example.png "Profile example")
+![example](resources/example.png "Profile example")
 
 ## Installation
 
 ```sh
-$ git clone https://codeberg.org/librehub/profiler
-$ cd profiler
-$ python main.py --serve
-```
+$ pip install libreppc
+$ python -m libreppc --serve
+``
 
 ## Getting started
 
 You need to create `config.json`:
 
 **config.json** structure
 ```json
@@ -73,20 +72,22 @@
         }
     ]
 }
 ```
 
 Then you need to build site with:
 
-```
-$ python main.py --build
+```sh
+$ python -m libreppc --build
 ```
 
 ## Contacts
 
 | Contact                                               | Description       |
 | :---:                                                 | :---              |
 | [`Matrix`](https://matrix.to/#/#librehub:matrix.org)  | Matrix server     |
 
-## Donates
-**Monero/XMR:** `47KkgEb3agJJjSpeW1LpVi1M8fsCfREhnBCb1yib5KQgCxwb6j47XBQAamueByrLUceRinJqveZ82UCbrGqrsY9oNuZ97xN`
+## Support
+
+You can support us [here](https://warlock.codeberg.page).
+
```

### Comparing `libreppc-0.1.0/libreppc/__main__.py` & `libreppc-0.1.1/libreppc/__main__.py`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.0/libreppc/libreppc.py` & `libreppc-0.1.1/libreppc/libreppc.py`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.0/libreppc.egg-info/PKG-INFO` & `libreppc-0.1.1/libreppc.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreppc
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple profile page creator.
 Home-page: https://codeberg.org/librehub/libreppc
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,profile,html,css,markdown,profile page,page,site,personal page
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -15,27 +15,26 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: flask
 Requires-Dist: markdown
 Requires-Dist: feedgen
 Requires-Dist: pytz
 
-# profiler 
+# libreppc 
 
-A simple profile page creator. 
+A simple profile page creator.
 
-![example](resources/profiler-example.png "Profile example")
+![example](resources/example.png "Profile example")
 
 ## Installation
 
 ```sh
-$ git clone https://codeberg.org/librehub/profiler
-$ cd profiler
-$ python main.py --serve
-```
+$ pip install libreppc
+$ python -m libreppc --serve
+``
 
 ## Getting started
 
 You need to create `config.json`:
 
 **config.json** structure
 ```json
@@ -73,20 +72,22 @@
         }
     ]
 }
 ```
 
 Then you need to build site with:
 
-```
-$ python main.py --build
+```sh
+$ python -m libreppc --build
 ```
 
 ## Contacts
 
 | Contact                                               | Description       |
 | :---:                                                 | :---              |
 | [`Matrix`](https://matrix.to/#/#librehub:matrix.org)  | Matrix server     |
 
-## Donates
-**Monero/XMR:** `47KkgEb3agJJjSpeW1LpVi1M8fsCfREhnBCb1yib5KQgCxwb6j47XBQAamueByrLUceRinJqveZ82UCbrGqrsY9oNuZ97xN`
+## Support
+
+You can support us [here](https://warlock.codeberg.page).
+
```

### Comparing `libreppc-0.1.0/setup.py` & `libreppc-0.1.1/setup.py`

 * *Files identical despite different names*

