# Comparing `tmp/pynovnc-1.1.1.tar.gz` & `tmp/pynovnc-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynovnc-1.1.1.tar", last modified: Sat Apr 13 08:30:02 2024, max compression
+gzip compressed data, was "pynovnc-1.1.2.tar", last modified: Sat Apr 13 08:39:57 2024, max compression
```

## Comparing `pynovnc-1.1.1.tar` & `pynovnc-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:30:02.867399 pynovnc-1.1.1/
--rw-r--r--   0 root         (0) root         (0)     1125 2024-04-13 08:30:02.866399 pynovnc-1.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      733 2024-04-13 08:29:54.000000 pynovnc-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:30:02.864399 pynovnc-1.1.1/pynovnc/
--rw-rw-rw-   0 root         (0) root         (0)      348 2024-04-13 08:29:54.000000 pynovnc-1.1.1/pynovnc/Main.py
--rw-rw-rw-   0 root         (0) root         (0)     2918 2024-04-13 08:29:54.000000 pynovnc-1.1.1/pynovnc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:30:02.866399 pynovnc-1.1.1/pynovnc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1125 2024-04-13 08:30:02.000000 pynovnc-1.1.1/pynovnc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      242 2024-04-13 08:30:02.000000 pynovnc-1.1.1/pynovnc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 08:30:02.000000 pynovnc-1.1.1/pynovnc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2024-04-13 08:30:02.000000 pynovnc-1.1.1/pynovnc.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-13 08:30:02.000000 pynovnc-1.1.1/pynovnc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-13 08:30:02.000000 pynovnc-1.1.1/pynovnc.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 08:30:02.867399 pynovnc-1.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3019 2024-04-13 08:29:54.000000 pynovnc-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:39:57.444763 pynovnc-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-13 08:39:57.444763 pynovnc-1.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      733 2024-04-13 08:39:48.000000 pynovnc-1.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:39:57.442763 pynovnc-1.1.2/pynovnc/
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-04-13 08:39:48.000000 pynovnc-1.1.2/pynovnc/Main.py
+-rw-rw-rw-   0 root         (0) root         (0)     2918 2024-04-13 08:39:48.000000 pynovnc-1.1.2/pynovnc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 08:39:57.443763 pynovnc-1.1.2/pynovnc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-04-13 08:39:57.000000 pynovnc-1.1.2/pynovnc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      242 2024-04-13 08:39:57.000000 pynovnc-1.1.2/pynovnc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 08:39:57.000000 pynovnc-1.1.2/pynovnc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-04-13 08:39:57.000000 pynovnc-1.1.2/pynovnc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-13 08:39:57.000000 pynovnc-1.1.2/pynovnc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-13 08:39:57.000000 pynovnc-1.1.2/pynovnc.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 08:39:57.444763 pynovnc-1.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3019 2024-04-13 08:39:48.000000 pynovnc-1.1.2/setup.py
```

### Comparing `pynovnc-1.1.1/PKG-INFO` & `pynovnc-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynovnc
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python Package made by Mhadhbi Issam . 
 Home-page: https://gitlab.com/isampypi/pynovnc
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pynovnc Version: 1.1.1 Summary: Python Package made
+Metadata-Version: 2.1 Name: pynovnc Version: 1.1.2 Summary: Python Package made
 by Mhadhbi Issam . Home-page: https://gitlab.com/isampypi/pynovnc Author:
 Mhadhbi Issam Author-email: mhadhbixissam@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown Requires-Dist: bashi # pynovnc _C_o_l_a_b ## Install Requiements : ```bash
 apt install -y --fix-missing xserver-xephyr x11vnc xvfb novnc net-tools x11-
 apps x11-xkb-utils gedit tightvncserver x11-utils gnumeric ``` ## Installation
```

### Comparing `pynovnc-1.1.1/README.md` & `pynovnc-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pynovnc-1.1.1/pynovnc/__init__.py` & `pynovnc-1.1.2/pynovnc/__init__.py`

 * *Files identical despite different names*

### Comparing `pynovnc-1.1.1/pynovnc.egg-info/PKG-INFO` & `pynovnc-1.1.2/pynovnc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynovnc
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python Package made by Mhadhbi Issam . 
 Home-page: https://gitlab.com/isampypi/pynovnc
 Author: Mhadhbi Issam
 Author-email: mhadhbixissam@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pynovnc Version: 1.1.1 Summary: Python Package made
+Metadata-Version: 2.1 Name: pynovnc Version: 1.1.2 Summary: Python Package made
 by Mhadhbi Issam . Home-page: https://gitlab.com/isampypi/pynovnc Author:
 Mhadhbi Issam Author-email: mhadhbixissam@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown Requires-Dist: bashi # pynovnc _C_o_l_a_b ## Install Requiements : ```bash
 apt install -y --fix-missing xserver-xephyr x11vnc xvfb novnc net-tools x11-
 apps x11-xkb-utils gedit tightvncserver x11-utils gnumeric ``` ## Installation
```

### Comparing `pynovnc-1.1.1/setup.py` & `pynovnc-1.1.2/setup.py`

 * *Files identical despite different names*

