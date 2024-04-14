# Comparing `tmp/libreppc-0.1.3.tar.gz` & `tmp/libreppc-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreppc-0.1.3.tar", last modified: Sun Apr 14 17:32:30 2024, max compression
+gzip compressed data, was "libreppc-0.1.4.tar", last modified: Sun Apr 14 19:48:43 2024, max compression
```

## Comparing `libreppc-0.1.3.tar` & `libreppc-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 17:32:30.261845 libreppc-0.1.3/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1096 2024-02-23 10:09:06.000000 libreppc-0.1.3/LICENSE
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-14 17:32:30.261845 libreppc-0.1.3/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1500 2024-04-14 17:20:23.000000 libreppc-0.1.3/README.md
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 17:32:30.261845 libreppc-0.1.3/libreppc/
--rw-r--r--   0 warlock   (1000) warlock   (1000)       48 2024-04-14 17:31:42.000000 libreppc-0.1.3/libreppc/__init__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)      705 2024-04-14 17:18:08.000000 libreppc-0.1.3/libreppc/__main__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     5555 2024-04-14 17:31:16.000000 libreppc-0.1.3/libreppc/libreppc.py
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 17:32:30.261845 libreppc-0.1.3/libreppc.egg-info/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-14 17:32:30.000000 libreppc-0.1.3/libreppc.egg-info/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)      248 2024-04-14 17:32:30.000000 libreppc-0.1.3/libreppc.egg-info/SOURCES.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-04-14 17:32:30.000000 libreppc-0.1.3/libreppc.egg-info/dependency_links.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       28 2024-04-14 17:32:30.000000 libreppc-0.1.3/libreppc.egg-info/requires.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        9 2024-04-14 17:32:30.000000 libreppc-0.1.3/libreppc.egg-info/top_level.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-04-14 17:32:30.261845 libreppc-0.1.3/setup.cfg
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1070 2024-04-14 16:02:17.000000 libreppc-0.1.3/setup.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 19:48:43.771888 libreppc-0.1.4/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1096 2024-02-23 10:09:06.000000 libreppc-0.1.4/LICENSE
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-14 19:48:43.771888 libreppc-0.1.4/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1500 2024-04-14 17:20:23.000000 libreppc-0.1.4/README.md
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 19:48:43.771888 libreppc-0.1.4/libreppc/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       48 2024-04-14 19:47:57.000000 libreppc-0.1.4/libreppc/__init__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      705 2024-04-14 17:18:08.000000 libreppc-0.1.4/libreppc/__main__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     5555 2024-04-14 17:31:16.000000 libreppc-0.1.4/libreppc/libreppc.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 19:48:43.771888 libreppc-0.1.4/libreppc.egg-info/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-14 19:48:43.000000 libreppc-0.1.4/libreppc.egg-info/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      248 2024-04-14 19:48:43.000000 libreppc-0.1.4/libreppc.egg-info/SOURCES.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-04-14 19:48:43.000000 libreppc-0.1.4/libreppc.egg-info/dependency_links.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       28 2024-04-14 19:48:43.000000 libreppc-0.1.4/libreppc.egg-info/requires.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        9 2024-04-14 19:48:43.000000 libreppc-0.1.4/libreppc.egg-info/top_level.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-04-14 19:48:43.771888 libreppc-0.1.4/setup.cfg
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1070 2024-04-14 16:02:17.000000 libreppc-0.1.4/setup.py
```

### Comparing `libreppc-0.1.3/LICENSE` & `libreppc-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.3/PKG-INFO` & `libreppc-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreppc
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple profile page creator.
 Home-page: https://codeberg.org/librehub/libreppc
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,profile,html,css,markdown,profile page,page,site,personal page
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `libreppc-0.1.3/README.md` & `libreppc-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.3/libreppc/__main__.py` & `libreppc-0.1.4/libreppc/__main__.py`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.3/libreppc/libreppc.py` & `libreppc-0.1.4/libreppc/libreppc.py`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.3/libreppc.egg-info/PKG-INFO` & `libreppc-0.1.4/libreppc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreppc
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple profile page creator.
 Home-page: https://codeberg.org/librehub/libreppc
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,profile,html,css,markdown,profile page,page,site,personal page
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `libreppc-0.1.3/setup.py` & `libreppc-0.1.4/setup.py`

 * *Files identical despite different names*

