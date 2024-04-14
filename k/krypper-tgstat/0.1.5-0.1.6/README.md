# Comparing `tmp/krypper_tgstat-0.1.5.tar.gz` & `tmp/krypper_tgstat-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krypper_tgstat-0.1.5.tar", last modified: Sun Apr 14 20:53:15 2024, max compression
+gzip compressed data, was "krypper_tgstat-0.1.6.tar", last modified: Sun Apr 14 20:56:04 2024, max compression
```

## Comparing `krypper_tgstat-0.1.5.tar` & `krypper_tgstat-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-14 20:53:15.538766 krypper_tgstat-0.1.5/
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)     1063 2024-04-13 08:38:04.000000 krypper_tgstat-0.1.5/LICENSE
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      914 2024-04-14 20:53:15.538766 krypper_tgstat-0.1.5/PKG-INFO
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      103 2024-04-13 08:55:13.000000 krypper_tgstat-0.1.5/README.md
-drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-14 20:53:15.537766 krypper_tgstat-0.1.5/krypper_tgstat/
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      238 2024-04-14 19:03:04.000000 krypper_tgstat-0.1.5/krypper_tgstat/__init__.py
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)     9194 2024-04-14 20:50:02.000000 krypper_tgstat-0.1.5/krypper_tgstat/classes.py
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)     2906 2024-04-14 19:03:04.000000 krypper_tgstat-0.1.5/krypper_tgstat/enums.py
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      661 2024-04-14 19:01:40.000000 krypper_tgstat-0.1.5/krypper_tgstat/exceptions.py
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)     7611 2024-04-14 20:50:23.000000 krypper_tgstat-0.1.5/krypper_tgstat/tg_stat.py
-drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-14 20:53:15.537766 krypper_tgstat-0.1.5/krypper_tgstat.egg-info/
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      914 2024-04-14 20:53:15.000000 krypper_tgstat-0.1.5/krypper_tgstat.egg-info/PKG-INFO
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)      382 2024-04-14 20:53:15.000000 krypper_tgstat-0.1.5/krypper_tgstat.egg-info/SOURCES.txt
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)        1 2024-04-14 20:53:15.000000 krypper_tgstat-0.1.5/krypper_tgstat.egg-info/dependency_links.txt
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)       17 2024-04-14 20:53:15.000000 krypper_tgstat-0.1.5/krypper_tgstat.egg-info/requires.txt
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)       15 2024-04-14 20:53:15.000000 krypper_tgstat-0.1.5/krypper_tgstat.egg-info/top_level.txt
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)       38 2024-04-14 20:53:15.539766 krypper_tgstat-0.1.5/setup.cfg
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)     1293 2024-04-14 20:53:09.000000 krypper_tgstat-0.1.5/setup.py
-drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-14 20:53:15.538766 krypper_tgstat-0.1.5/tests/
--rw-r--r--   0 krymmy    (1000) krymmy    (1000)    36813 2024-04-14 20:46:26.000000 krypper_tgstat-0.1.5/tests/test_TGStatSync.py
+drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-14 20:56:04.029566 krypper_tgstat-0.1.6/
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)     1063 2024-04-13 08:38:04.000000 krypper_tgstat-0.1.6/LICENSE
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      908 2024-04-14 20:56:04.029566 krypper_tgstat-0.1.6/PKG-INFO
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      103 2024-04-13 08:55:13.000000 krypper_tgstat-0.1.6/README.md
+drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-14 20:56:04.028566 krypper_tgstat-0.1.6/krypper_tgstat/
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      238 2024-04-14 19:03:04.000000 krypper_tgstat-0.1.6/krypper_tgstat/__init__.py
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)     9194 2024-04-14 20:50:02.000000 krypper_tgstat-0.1.6/krypper_tgstat/classes.py
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)     2906 2024-04-14 19:03:04.000000 krypper_tgstat-0.1.6/krypper_tgstat/enums.py
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      661 2024-04-14 19:01:40.000000 krypper_tgstat-0.1.6/krypper_tgstat/exceptions.py
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)     7611 2024-04-14 20:50:23.000000 krypper_tgstat-0.1.6/krypper_tgstat/tg_stat.py
+drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-14 20:56:04.028566 krypper_tgstat-0.1.6/krypper_tgstat.egg-info/
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      908 2024-04-14 20:56:03.000000 krypper_tgstat-0.1.6/krypper_tgstat.egg-info/PKG-INFO
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)      382 2024-04-14 20:56:03.000000 krypper_tgstat-0.1.6/krypper_tgstat.egg-info/SOURCES.txt
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)        1 2024-04-14 20:56:03.000000 krypper_tgstat-0.1.6/krypper_tgstat.egg-info/dependency_links.txt
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)       17 2024-04-14 20:56:03.000000 krypper_tgstat-0.1.6/krypper_tgstat.egg-info/requires.txt
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)       15 2024-04-14 20:56:03.000000 krypper_tgstat-0.1.6/krypper_tgstat.egg-info/top_level.txt
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)       38 2024-04-14 20:56:04.029566 krypper_tgstat-0.1.6/setup.cfg
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)     1287 2024-04-14 20:55:52.000000 krypper_tgstat-0.1.6/setup.py
+drwxr-xr-x   0 krymmy    (1000) krymmy    (1000)        0 2024-04-14 20:56:04.029566 krypper_tgstat-0.1.6/tests/
+-rw-r--r--   0 krymmy    (1000) krymmy    (1000)    36813 2024-04-14 20:46:26.000000 krypper_tgstat-0.1.6/tests/test_TGStatSync.py
```

### Comparing `krypper_tgstat-0.1.5/LICENSE` & `krypper_tgstat-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `krypper_tgstat-0.1.5/PKG-INFO` & `krypper_tgstat-0.1.6/krypper_tgstat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: krypper_tgstat
-Version: 0.1.5
+Name: krypper-tgstat
+Version: 0.1.6
 Summary: Wrapper for TG Stat API writing on Python
-Home-page: https://github.com/KrymmyEM/PyrapperTGStatAPI
-Download-URL: https://github.com/KrymmyEM/PyrapperTGStatAPI/archive/main.zip
+Home-page: https://github.com/KrymmyEM/krypper_tgstat
+Download-URL: https://github.com/KrymmyEM/krypper_tgstat/archive/main.zip
 Author: Evgeny Momotov (KrymmyEM)
 Author-email: evgeny.momotov@gmail.com
 License: MIT License. See LICENSE file
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `krypper_tgstat-0.1.5/krypper_tgstat/classes.py` & `krypper_tgstat-0.1.6/krypper_tgstat/classes.py`

 * *Files identical despite different names*

### Comparing `krypper_tgstat-0.1.5/krypper_tgstat/enums.py` & `krypper_tgstat-0.1.6/krypper_tgstat/enums.py`

 * *Files identical despite different names*

### Comparing `krypper_tgstat-0.1.5/krypper_tgstat/exceptions.py` & `krypper_tgstat-0.1.6/krypper_tgstat/exceptions.py`

 * *Files identical despite different names*

### Comparing `krypper_tgstat-0.1.5/krypper_tgstat/tg_stat.py` & `krypper_tgstat-0.1.6/krypper_tgstat/tg_stat.py`

 * *Files identical despite different names*

### Comparing `krypper_tgstat-0.1.5/krypper_tgstat.egg-info/PKG-INFO` & `krypper_tgstat-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: krypper-tgstat
-Version: 0.1.5
+Name: krypper_tgstat
+Version: 0.1.6
 Summary: Wrapper for TG Stat API writing on Python
-Home-page: https://github.com/KrymmyEM/PyrapperTGStatAPI
-Download-URL: https://github.com/KrymmyEM/PyrapperTGStatAPI/archive/main.zip
+Home-page: https://github.com/KrymmyEM/krypper_tgstat
+Download-URL: https://github.com/KrymmyEM/krypper_tgstat/archive/main.zip
 Author: Evgeny Momotov (KrymmyEM)
 Author-email: evgeny.momotov@gmail.com
 License: MIT License. See LICENSE file
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
```

### Comparing `krypper_tgstat-0.1.5/setup.py` & `krypper_tgstat-0.1.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 
 """
 :authors: Evgeny Momotov (KrymmyEM)
 :license: MIT License
 Copyright: (c) 2024 Evgeny
 """
 
-version = "0.1.5"
+version = "0.1.6"
 
 long_description = ""
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name = "krypper_tgstat",
     version = version,
     description = "Wrapper for TG Stat API writing on Python\nTGStat (https://tgstat.ru API wrapper)",
     long_description = long_description,
 
     author = "Evgeny Momotov (KrymmyEM)",
     author_email = "evgeny.momotov@gmail.com",
-    url = "https://github.com/KrymmyEM/PyrapperTGStatAPI",
-    download_url = "https://github.com/KrymmyEM/PyrapperTGStatAPI/archive/main.zip",
+    url = "https://github.com/KrymmyEM/krypper_tgstat",
+    download_url = "https://github.com/KrymmyEM/krypper_tgstat/archive/main.zip",
 
     license = "MIT License. See LICENSE file",
     packages = ["krypper_tgstat"],
     install_requires=[
         "requests",
         "aiohttp"
     ],
```

### Comparing `krypper_tgstat-0.1.5/tests/test_TGStatSync.py` & `krypper_tgstat-0.1.6/tests/test_TGStatSync.py`

 * *Files identical despite different names*

