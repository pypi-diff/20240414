# Comparing `tmp/piwiPre-0.8.4.tar.gz` & `tmp/piwiPre-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piwiPre-0.8.4.tar", last modified: Fri Sep 29 17:10:59 2023, max compression
+gzip compressed data, was "piwiPre-0.8.5.tar", last modified: Fri Sep 29 17:12:37 2023, max compression
```

## Comparing `piwiPre-0.8.4.tar` & `piwiPre-0.8.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-09-29 17:10:59.247941 piwiPre-0.8.4/
--rw-rw-rw-   0        0        0    14408 2023-03-13 18:23:44.000000 piwiPre-0.8.4/LICENCE
--rw-rw-rw-   0        0        0     4308 2023-09-29 17:10:59.245949 piwiPre-0.8.4/PKG-INFO
--rw-rw-rw-   0        0        0     3624 2023-09-26 20:41:01.000000 piwiPre-0.8.4/README.md
-drwxrwxrwx   0        0        0        0 2023-09-29 17:10:59.198604 piwiPre-0.8.4/piwiPre/
--rw-rw-rw-   0        0        0      499 2023-07-15 16:43:15.000000 piwiPre-0.8.4/piwiPre/__init__.py
--rw-rw-rw-   0        0        0      500 2023-09-09 18:17:08.000000 piwiPre-0.8.4/piwiPre/__main__.py
--rw-rw-rw-   0        0        0    23841 2023-09-29 14:15:21.000000 piwiPre-0.8.4/piwiPre/pwpActor.py
--rw-rw-rw-   0        0        0    15128 2023-09-20 21:48:43.000000 piwiPre-0.8.4/piwiPre/pwpArgsIni.py
--rw-rw-rw-   0        0        0    10347 2023-09-26 15:35:46.000000 piwiPre-0.8.4/piwiPre/pwpConfig.py
--rw-rw-rw-   0        0        0     5016 2023-09-26 15:19:34.000000 piwiPre-0.8.4/piwiPre/pwpErrors.py
--rw-rw-rw-   0        0        0    17338 2023-09-29 13:58:18.000000 piwiPre-0.8.4/piwiPre/pwpJpg.py
--rw-rw-rw-   0        0        0    20412 2023-08-16 21:01:03.000000 piwiPre-0.8.4/piwiPre/pwpLicence.py
--rw-rw-rw-   0        0        0    39454 2023-09-29 14:01:26.000000 piwiPre-0.8.4/piwiPre/pwpMain.py
--rw-rw-rw-   0        0        0    15037 2023-09-26 15:45:44.000000 piwiPre-0.8.4/piwiPre/pwpMp4.py
--rw-rw-rw-   0        0        0    29901 2023-09-26 15:19:34.000000 piwiPre-0.8.4/piwiPre/pwpParser.py
--rw-rw-rw-   0        0        0    13878 2023-09-29 17:08:20.000000 piwiPre-0.8.4/piwiPre/pwpPatcher.py
--rw-rw-rw-   0        0        0      602 2023-09-29 17:10:21.000000 piwiPre-0.8.4/piwiPre/pwpVersion.py
-drwxrwxrwx   0        0        0        0 2023-09-29 17:10:59.237960 piwiPre-0.8.4/piwiPre.egg-info/
--rw-rw-rw-   0        0        0     4308 2023-09-29 17:10:59.000000 piwiPre-0.8.4/piwiPre.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-09-29 17:10:59.000000 piwiPre-0.8.4/piwiPre.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-29 17:10:59.000000 piwiPre-0.8.4/piwiPre.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-09-29 17:10:59.000000 piwiPre-0.8.4/piwiPre.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2023-09-29 17:10:59.000000 piwiPre-0.8.4/piwiPre.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-09-29 17:10:59.247941 piwiPre-0.8.4/setup.cfg
--rw-rw-rw-   0        0        0     1365 2023-07-16 19:31:34.000000 piwiPre-0.8.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-09-29 17:10:59.241444 piwiPre-0.8.4/tests/
--rw-rw-rw-   0        0        0    95055 2023-09-29 15:31:53.000000 piwiPre-0.8.4/tests/test_pwp.py
+drwxrwxrwx   0        0        0        0 2023-09-29 17:12:37.715041 piwiPre-0.8.5/
+-rw-rw-rw-   0        0        0    14408 2023-03-13 18:23:44.000000 piwiPre-0.8.5/LICENCE
+-rw-rw-rw-   0        0        0     4308 2023-09-29 17:12:37.713036 piwiPre-0.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3624 2023-09-26 20:41:01.000000 piwiPre-0.8.5/README.md
+drwxrwxrwx   0        0        0        0 2023-09-29 17:12:37.663227 piwiPre-0.8.5/piwiPre/
+-rw-rw-rw-   0        0        0      499 2023-07-15 16:43:15.000000 piwiPre-0.8.5/piwiPre/__init__.py
+-rw-rw-rw-   0        0        0      500 2023-09-09 18:17:08.000000 piwiPre-0.8.5/piwiPre/__main__.py
+-rw-rw-rw-   0        0        0    23841 2023-09-29 14:15:21.000000 piwiPre-0.8.5/piwiPre/pwpActor.py
+-rw-rw-rw-   0        0        0    15128 2023-09-20 21:48:43.000000 piwiPre-0.8.5/piwiPre/pwpArgsIni.py
+-rw-rw-rw-   0        0        0    10347 2023-09-26 15:35:46.000000 piwiPre-0.8.5/piwiPre/pwpConfig.py
+-rw-rw-rw-   0        0        0     5016 2023-09-26 15:19:34.000000 piwiPre-0.8.5/piwiPre/pwpErrors.py
+-rw-rw-rw-   0        0        0    17338 2023-09-29 13:58:18.000000 piwiPre-0.8.5/piwiPre/pwpJpg.py
+-rw-rw-rw-   0        0        0    20412 2023-08-16 21:01:03.000000 piwiPre-0.8.5/piwiPre/pwpLicence.py
+-rw-rw-rw-   0        0        0    39454 2023-09-29 14:01:26.000000 piwiPre-0.8.5/piwiPre/pwpMain.py
+-rw-rw-rw-   0        0        0    15037 2023-09-26 15:45:44.000000 piwiPre-0.8.5/piwiPre/pwpMp4.py
+-rw-rw-rw-   0        0        0    29901 2023-09-26 15:19:34.000000 piwiPre-0.8.5/piwiPre/pwpParser.py
+-rw-rw-rw-   0        0        0    13878 2023-09-29 17:08:20.000000 piwiPre-0.8.5/piwiPre/pwpPatcher.py
+-rw-rw-rw-   0        0        0      602 2023-09-29 17:12:01.000000 piwiPre-0.8.5/piwiPre/pwpVersion.py
+drwxrwxrwx   0        0        0        0 2023-09-29 17:12:37.704940 piwiPre-0.8.5/piwiPre.egg-info/
+-rw-rw-rw-   0        0        0     4308 2023-09-29 17:12:37.000000 piwiPre-0.8.5/piwiPre.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2023-09-29 17:12:37.000000 piwiPre-0.8.5/piwiPre.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-09-29 17:12:37.000000 piwiPre-0.8.5/piwiPre.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-09-29 17:12:37.000000 piwiPre-0.8.5/piwiPre.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2023-09-29 17:12:37.000000 piwiPre-0.8.5/piwiPre.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-09-29 17:12:37.715041 piwiPre-0.8.5/setup.cfg
+-rw-rw-rw-   0        0        0     1365 2023-07-16 19:31:34.000000 piwiPre-0.8.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-09-29 17:12:37.707917 piwiPre-0.8.5/tests/
+-rw-rw-rw-   0        0        0    95055 2023-09-29 15:31:53.000000 piwiPre-0.8.5/tests/test_pwp.py
```

### Comparing `piwiPre-0.8.4/LICENCE` & `piwiPre-0.8.5/LICENCE`

 * *Files identical despite different names*

### Comparing `piwiPre-0.8.4/PKG-INFO` & `piwiPre-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwiPre
-Version: 0.8.4
+Version: 0.8.5
 Summary: piwigo picture preparation tool
 Home-page: https://gitlab.com/fabien.battini/piwipre
 Author: Fabien BATTINI
 Author-email: fabien.battini@gmail.com
 Keywords: piwigo images pictures
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
```

### Comparing `piwiPre-0.8.4/README.md` & `piwiPre-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `piwiPre-0.8.4/piwiPre/pwpActor.py` & `piwiPre-0.8.5/piwiPre/pwpActor.py`

 * *Files identical despite different names*

### Comparing `piwiPre-0.8.4/piwiPre/pwpArgsIni.py` & `piwiPre-0.8.5/piwiPre/pwpArgsIni.py`

 * *Files identical despite different names*

### Comparing `piwiPre-0.8.4/piwiPre/pwpConfig.py` & `piwiPre-0.8.5/piwiPre/pwpConfig.py`

 * *Files identical despite different names*

### Comparing `piwiPre-0.8.4/piwiPre/pwpErrors.py` & `piwiPre-0.8.5/piwiPre/pwpErrors.py`

 * *Files identical despite different names*

### Comparing `piwiPre-0.8.4/piwiPre/pwpJpg.py` & `piwiPre-0.8.5/piwiPre/pwpJpg.py`

 * *Files identical despite different names*

### Comparing `piwiPre-0.8.4/piwiPre/pwpLicence.py` & `piwiPre-0.8.5/piwiPre/pwpLicence.py`

 * *Files identical despite different names*

### Comparing `piwiPre-0.8.4/piwiPre/pwpMain.py` & `piwiPre-0.8.5/piwiPre/pwpMain.py`

 * *Files identical despite different names*

### Comparing `piwiPre-0.8.4/piwiPre/pwpMp4.py` & `piwiPre-0.8.5/piwiPre/pwpMp4.py`

 * *Files identical despite different names*

### Comparing `piwiPre-0.8.4/piwiPre/pwpParser.py` & `piwiPre-0.8.5/piwiPre/pwpParser.py`

 * *Files identical despite different names*

### Comparing `piwiPre-0.8.4/piwiPre/pwpPatcher.py` & `piwiPre-0.8.5/piwiPre/pwpPatcher.py`

 * *Files identical despite different names*

### Comparing `piwiPre-0.8.4/piwiPre/pwpVersion.py` & `piwiPre-0.8.5/piwiPre/pwpVersion.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # piwiPre project
 # This program and library is licenced under the European Union Public Licence v1.2 (see LICENCE)
 # developed by fabien.battini(at)gmail.com
 # ---------------------------------------------------------------------------------------------------------------
 
 
 class PwpVersion:
-    help = '0.8.4 at 09/29/2023 19:10:21'
-    spec = '0.8.4'
+    help = '0.8.5 at 09/29/2023 19:12:01'
+    spec = '0.8.5'
     release = 0
     version = 8
-    patch = 4
-    date = '09/29/2023 19:10:21'
+    patch = 5
+    date = '09/29/2023 19:12:01'
 
     def __init__(self):
         pass
```

### Comparing `piwiPre-0.8.4/piwiPre.egg-info/PKG-INFO` & `piwiPre-0.8.5/piwiPre.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwiPre
-Version: 0.8.4
+Version: 0.8.5
 Summary: piwigo picture preparation tool
 Home-page: https://gitlab.com/fabien.battini/piwipre
 Author: Fabien BATTINI
 Author-email: fabien.battini@gmail.com
 Keywords: piwigo images pictures
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
```

### Comparing `piwiPre-0.8.4/setup.py` & `piwiPre-0.8.5/setup.py`

 * *Files identical despite different names*

### Comparing `piwiPre-0.8.4/tests/test_pwp.py` & `piwiPre-0.8.5/tests/test_pwp.py`

 * *Files identical despite different names*

