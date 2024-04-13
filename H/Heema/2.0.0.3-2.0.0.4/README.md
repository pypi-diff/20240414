# Comparing `tmp/Heema-2.0.0.3.tar.gz` & `tmp/Heema-2.0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Heema-2.0.0.3.tar", last modified: Sat Apr 13 22:36:55 2024, max compression
+gzip compressed data, was "Heema-2.0.0.4.tar", last modified: Sat Apr 13 23:16:21 2024, max compression
```

## Comparing `Heema-2.0.0.3.tar` & `Heema-2.0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 22:36:55.446342 Heema-2.0.0.3/
-drwxrwxrwx   0        0        0        0 2024-04-13 22:36:55.430717 Heema-2.0.0.3/Heema.egg-info/
--rw-rw-rw-   0        0        0     5582 2024-04-13 22:36:55.000000 Heema-2.0.0.3/Heema.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2024-04-13 22:36:55.000000 Heema-2.0.0.3/Heema.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 22:36:55.000000 Heema-2.0.0.3/Heema.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-13 22:36:55.000000 Heema-2.0.0.3/Heema.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 22:36:55.000000 Heema-2.0.0.3/Heema.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1111 2024-04-13 22:15:45.000000 Heema-2.0.0.3/LICENSE
--rw-rw-rw-   0        0        0     5582 2024-04-13 22:36:55.446342 Heema-2.0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4689 2024-04-13 22:15:45.000000 Heema-2.0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-13 22:36:55.446342 Heema-2.0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1170 2024-04-13 22:36:42.000000 Heema-2.0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-13 22:36:55.430717 Heema-2.0.0.3/tests/
--rw-rw-rw-   0        0        0     3705 2024-04-13 22:15:45.000000 Heema-2.0.0.3/tests/test.py
--rw-rw-rw-   0        0        0    14787 2024-04-13 22:15:45.000000 Heema-2.0.0.3/tests/test2.py
+drwxrwxrwx   0        0        0        0 2024-04-13 23:16:21.224110 Heema-2.0.0.4/
+drwxrwxrwx   0        0        0        0 2024-04-13 23:16:21.224110 Heema-2.0.0.4/Heema.egg-info/
+-rw-rw-rw-   0        0        0     5582 2024-04-13 23:16:21.000000 Heema-2.0.0.4/Heema.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2024-04-13 23:16:21.000000 Heema-2.0.0.4/Heema.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 23:16:21.000000 Heema-2.0.0.4/Heema.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-13 23:16:21.000000 Heema-2.0.0.4/Heema.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 23:16:21.000000 Heema-2.0.0.4/Heema.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1111 2024-04-13 23:00:55.000000 Heema-2.0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     5582 2024-04-13 23:16:21.224110 Heema-2.0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4689 2024-04-13 23:00:55.000000 Heema-2.0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-13 23:16:21.224110 Heema-2.0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1170 2024-04-13 23:10:05.000000 Heema-2.0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 23:16:21.224110 Heema-2.0.0.4/tests/
+-rw-rw-rw-   0        0        0     3705 2024-04-13 23:00:55.000000 Heema-2.0.0.4/tests/test.py
+-rw-rw-rw-   0        0        0    14787 2024-04-13 23:00:55.000000 Heema-2.0.0.4/tests/test2.py
```

### Comparing `Heema-2.0.0.3/Heema.egg-info/PKG-INFO` & `Heema-2.0.0.4/Heema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Heema
-Version: 2.0.0.3
+Version: 2.0.0.4
 Summary: A GUI framework built on top of tkinter, with new features.
 Author: Федор Глеб | Abhay Gaur
 Author-email: <abhay.12104531@gmail.com>
 Keywords: Heema,heema,heema gui,HEEMA,heemagui,python,tkinter,modern,gui,tkintergui,browser
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Heema-2.0.0.3/LICENSE` & `Heema-2.0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Heema-2.0.0.3/PKG-INFO` & `Heema-2.0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Heema
-Version: 2.0.0.3
+Version: 2.0.0.4
 Summary: A GUI framework built on top of tkinter, with new features.
 Author: Федор Глеб | Abhay Gaur
 Author-email: <abhay.12104531@gmail.com>
 Keywords: Heema,heema,heema gui,HEEMA,heemagui,python,tkinter,modern,gui,tkintergui,browser
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Heema-2.0.0.3/README.md` & `Heema-2.0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `Heema-2.0.0.3/setup.py` & `Heema-2.0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "2.0.0.3"
+VERSION = "2.0.0.4"
 DESCRIPTION = 'A GUI framework built on top of tkinter, with new features.'
 LONG_DESCRIPTION = ''
 
 # Setting up
 setup(
     name="Heema",
     version=VERSION,
```

### Comparing `Heema-2.0.0.3/tests/test.py` & `Heema-2.0.0.4/tests/test.py`

 * *Files identical despite different names*

### Comparing `Heema-2.0.0.3/tests/test2.py` & `Heema-2.0.0.4/tests/test2.py`

 * *Files identical despite different names*

