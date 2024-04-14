# Comparing `tmp/monisha-0.0.41.tar.gz` & `tmp/monisha-0.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monisha-0.0.41.tar", last modified: Fri Apr 12 07:22:44 2024, max compression
+gzip compressed data, was "monisha-0.0.42.tar", last modified: Sun Apr 14 02:37:17 2024, max compression
```

## Comparing `monisha-0.0.41.tar` & `monisha-0.0.42.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:22:44.626558 monisha-0.0.41/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-12 07:22:38.000000 monisha-0.0.41/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:22:44.622558 monisha-0.0.41/Monisha/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:22:44.626558 monisha-0.0.41/Monisha/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function01.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function02.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function03.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function04.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function05.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function06.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function07.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function08.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function09.py
--rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function10.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function11.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function12.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/functions/function13.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:22:44.626558 monisha-0.0.41/Monisha/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-12 07:22:38.000000 monisha-0.0.41/Monisha/scripts/es.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-12 07:22:44.626558 monisha-0.0.41/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-04-12 07:22:38.000000 monisha-0.0.41/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 07:22:44.626558 monisha-0.0.41/monisha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-12 07:22:44.000000 monisha-0.0.41/monisha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-12 07:22:44.000000 monisha-0.0.41/monisha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 07:22:44.000000 monisha-0.0.41/monisha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 07:22:44.000000 monisha-0.0.41/monisha.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-12 07:22:44.000000 monisha-0.0.41/monisha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 07:22:44.626558 monisha-0.0.41/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-12 07:22:38.000000 monisha-0.0.41/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:37:17.595572 monisha-0.0.42/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-14 02:37:11.000000 monisha-0.0.42/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:37:17.587572 monisha-0.0.42/Monisha/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 02:37:11.000000 monisha-0.0.42/Monisha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:37:17.591572 monisha-0.0.42/Monisha/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-14 02:37:11.000000 monisha-0.0.42/Monisha/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-04-14 02:37:11.000000 monisha-0.0.42/Monisha/functions/function01.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-14 02:37:11.000000 monisha-0.0.42/Monisha/functions/function02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-14 02:37:11.000000 monisha-0.0.42/Monisha/functions/function03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-14 02:37:11.000000 monisha-0.0.42/Monisha/functions/function04.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-14 02:37:11.000000 monisha-0.0.42/Monisha/functions/function05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-14 02:37:11.000000 monisha-0.0.42/Monisha/functions/function06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-14 02:37:11.000000 monisha-0.0.42/Monisha/functions/function07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-14 02:37:11.000000 monisha-0.0.42/Monisha/functions/function08.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-14 02:37:11.000000 monisha-0.0.42/Monisha/functions/function09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60105 2024-04-14 02:37:11.000000 monisha-0.0.42/Monisha/functions/function10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-14 02:37:11.000000 monisha-0.0.42/Monisha/functions/function11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-14 02:37:11.000000 monisha-0.0.42/Monisha/functions/function12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-14 02:37:11.000000 monisha-0.0.42/Monisha/functions/function13.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-14 02:37:11.000000 monisha-0.0.42/Monisha/functions/function14.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:37:17.591572 monisha-0.0.42/Monisha/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-14 02:37:11.000000 monisha-0.0.42/Monisha/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-14 02:37:11.000000 monisha-0.0.42/Monisha/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-14 02:37:11.000000 monisha-0.0.42/Monisha/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-14 02:37:11.000000 monisha-0.0.42/Monisha/scripts/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-14 02:37:17.595572 monisha-0.0.42/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-14 02:37:11.000000 monisha-0.0.42/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 02:37:17.595572 monisha-0.0.42/monisha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-14 02:37:17.000000 monisha-0.0.42/monisha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-14 02:37:17.000000 monisha-0.0.42/monisha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 02:37:17.000000 monisha-0.0.42/monisha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 02:37:17.000000 monisha-0.0.42/monisha.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-14 02:37:17.000000 monisha-0.0.42/monisha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 02:37:17.595572 monisha-0.0.42/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-14 02:37:11.000000 monisha-0.0.42/setup.py
```

### Comparing `monisha-0.0.41/LICENSE` & `monisha-0.0.42/LICENSE`

 * *Files identical despite different names*

### Comparing `monisha-0.0.41/Monisha/functions/function01.py` & `monisha-0.0.42/Monisha/functions/function01.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.41/Monisha/functions/function02.py` & `monisha-0.0.42/Monisha/functions/function02.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.41/Monisha/functions/function03.py` & `monisha-0.0.42/Monisha/functions/function03.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.41/Monisha/functions/function04.py` & `monisha-0.0.42/Monisha/functions/function04.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.41/Monisha/functions/function06.py` & `monisha-0.0.42/Monisha/functions/function06.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.41/Monisha/functions/function07.py` & `monisha-0.0.42/Monisha/functions/function07.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.41/Monisha/functions/function10.py` & `monisha-0.0.42/Monisha/functions/function10.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.41/monisha.egg-info/SOURCES.txt` & `monisha-0.0.42/monisha.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 Monisha/functions/function07.py
 Monisha/functions/function08.py
 Monisha/functions/function09.py
 Monisha/functions/function10.py
 Monisha/functions/function11.py
 Monisha/functions/function12.py
 Monisha/functions/function13.py
+Monisha/functions/function14.py
 Monisha/scripts/__init__.py
 Monisha/scripts/en.py
 Monisha/scripts/eo.py
 Monisha/scripts/es.py
 monisha.egg-info/PKG-INFO
 monisha.egg-info/SOURCES.txt
 monisha.egg-info/dependency_links.txt
```

### Comparing `monisha-0.0.41/setup.py` & `monisha-0.0.42/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         'Topic :: Software Development :: Libraries :: Python Modules',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)']
 
 setup(
     name='monisha',
     license='MIT',
     zip_safe=False,
-    version='0.0.41',
+    version='0.0.42',
     classifiers=DATA02,
     author_email=DATA01,
     python_requires='~=3.8',
     packages=find_packages(),
     author='Clinton-Abraham',
     long_description=long_description,
     description='python helper modules',
```

