# Comparing `tmp/totemlib-0.1.0.8.tar.gz` & `tmp/totemlib-0.1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "totemlib-0.1.0.8.tar", last modified: Thu Sep  7 02:58:21 2023, max compression
+gzip compressed data, was "totemlib-0.1.0.9.tar", last modified: Sat Sep  9 00:43:38 2023, max compression
```

## Comparing `totemlib-0.1.0.8.tar` & `totemlib-0.1.0.9.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 lau        (501) staff       (20)        0 2023-09-07 02:58:21.209823 totemlib-0.1.0.8/
--rw-r--r--   0 lau        (501) staff       (20)        6 2023-08-26 15:31:59.000000 totemlib-0.1.0.8/LICENSE
--rw-r--r--   0 lau        (501) staff       (20)      167 2023-09-07 02:58:21.209630 totemlib-0.1.0.8/PKG-INFO
--rw-r--r--   0 lau        (501) staff       (20)        6 2023-08-26 15:31:47.000000 totemlib-0.1.0.8/README.md
--rw-r--r--   0 lau        (501) staff       (20)       38 2023-09-07 02:58:21.210023 totemlib-0.1.0.8/setup.cfg
--rw-r--r--   0 lau        (501) staff       (20)      333 2023-09-07 02:56:36.000000 totemlib-0.1.0.8/setup.py
-drwxr-xr-x   0 lau        (501) staff       (20)        0 2023-09-07 02:58:21.202242 totemlib-0.1.0.8/totemlib/
--rw-r--r--   0 lau        (501) staff       (20)       60 2023-09-07 02:56:27.000000 totemlib-0.1.0.8/totemlib/__init__.py
-drwxr-xr-x   0 lau        (501) staff       (20)        0 2023-09-07 02:58:21.205101 totemlib-0.1.0.8/totemlib/data/
--rw-r--r--   0 lau        (501) staff       (20)        0 2023-08-26 16:45:41.000000 totemlib-0.1.0.8/totemlib/data/__init__.py
--rw-r--r--   0 lau        (501) staff       (20)      811 2023-08-28 20:10:53.000000 totemlib-0.1.0.8/totemlib/data/conectDB.py
--rw-r--r--   0 lau        (501) staff       (20)     9832 2023-08-28 23:46:56.000000 totemlib-0.1.0.8/totemlib/data/datamanager.py
-drwxr-xr-x   0 lau        (501) staff       (20)        0 2023-09-07 02:58:21.206713 totemlib-0.1.0.8/totemlib/security/
--rw-r--r--   0 lau        (501) staff       (20)       59 2023-09-07 02:56:04.000000 totemlib-0.1.0.8/totemlib/security/__init__.py
--rw-r--r--   0 lau        (501) staff       (20)     1150 2023-08-26 18:18:06.000000 totemlib-0.1.0.8/totemlib/security/auth.py
--rw-r--r--   0 lau        (501) staff       (20)     4403 2023-09-05 13:35:57.000000 totemlib-0.1.0.8/totemlib/security/response_manager.py
--rw-r--r--   0 lau        (501) staff       (20)     1480 2023-09-06 20:54:14.000000 totemlib-0.1.0.8/totemlib/security/validations.py
-drwxr-xr-x   0 lau        (501) staff       (20)        0 2023-09-07 02:58:21.208891 totemlib-0.1.0.8/totemlib/utils/
--rw-r--r--   0 lau        (501) staff       (20)       67 2023-08-26 20:42:48.000000 totemlib-0.1.0.8/totemlib/utils/__init__.py
--rw-r--r--   0 lau        (501) staff       (20)      834 2023-08-26 20:01:18.000000 totemlib-0.1.0.8/totemlib/utils/encrypter.py
--rw-r--r--   0 lau        (501) staff       (20)     1689 2023-08-26 21:44:30.000000 totemlib-0.1.0.8/totemlib/utils/logger.py
--rw-r--r--   0 lau        (501) staff       (20)      559 2023-08-26 21:39:51.000000 totemlib-0.1.0.8/totemlib/utils/privproperties.py
-drwxr-xr-x   0 lau        (501) staff       (20)        0 2023-09-07 02:58:21.204438 totemlib-0.1.0.8/totemlib.egg-info/
--rw-r--r--   0 lau        (501) staff       (20)      167 2023-09-07 02:58:21.000000 totemlib-0.1.0.8/totemlib.egg-info/PKG-INFO
--rw-r--r--   0 lau        (501) staff       (20)      527 2023-09-07 02:58:21.000000 totemlib-0.1.0.8/totemlib.egg-info/SOURCES.txt
--rw-r--r--   0 lau        (501) staff       (20)        1 2023-09-07 02:58:21.000000 totemlib-0.1.0.8/totemlib.egg-info/dependency_links.txt
--rw-r--r--   0 lau        (501) staff       (20)       19 2023-09-07 02:58:21.000000 totemlib-0.1.0.8/totemlib.egg-info/requires.txt
--rw-r--r--   0 lau        (501) staff       (20)        9 2023-09-07 02:58:21.000000 totemlib-0.1.0.8/totemlib.egg-info/top_level.txt
+drwxr-xr-x   0 lau        (501) staff       (20)        0 2023-09-09 00:43:38.204862 totemlib-0.1.0.9/
+-rw-r--r--   0 lau        (501) staff       (20)        6 2023-08-26 15:31:59.000000 totemlib-0.1.0.9/LICENSE
+-rw-r--r--   0 lau        (501) staff       (20)      167 2023-09-09 00:43:38.204681 totemlib-0.1.0.9/PKG-INFO
+-rw-r--r--   0 lau        (501) staff       (20)        6 2023-08-26 15:31:47.000000 totemlib-0.1.0.9/README.md
+-rw-r--r--   0 lau        (501) staff       (20)       38 2023-09-09 00:43:38.204926 totemlib-0.1.0.9/setup.cfg
+-rw-r--r--   0 lau        (501) staff       (20)      333 2023-09-09 00:43:08.000000 totemlib-0.1.0.9/setup.py
+drwxr-xr-x   0 lau        (501) staff       (20)        0 2023-09-09 00:43:38.199814 totemlib-0.1.0.9/totemlib/
+-rw-r--r--   0 lau        (501) staff       (20)       60 2023-09-07 02:56:27.000000 totemlib-0.1.0.9/totemlib/__init__.py
+drwxr-xr-x   0 lau        (501) staff       (20)        0 2023-09-09 00:43:38.201285 totemlib-0.1.0.9/totemlib/data/
+-rw-r--r--   0 lau        (501) staff       (20)        0 2023-08-26 16:45:41.000000 totemlib-0.1.0.9/totemlib/data/__init__.py
+-rw-r--r--   0 lau        (501) staff       (20)      811 2023-08-28 20:10:53.000000 totemlib-0.1.0.9/totemlib/data/conectDB.py
+-rw-r--r--   0 lau        (501) staff       (20)     9832 2023-08-28 23:46:56.000000 totemlib-0.1.0.9/totemlib/data/datamanager.py
+-rw-r--r--   0 lau        (501) staff       (20)     1741 2023-09-09 00:39:56.000000 totemlib-0.1.0.9/totemlib/data/transform.py
+drwxr-xr-x   0 lau        (501) staff       (20)        0 2023-09-09 00:43:38.202720 totemlib-0.1.0.9/totemlib/security/
+-rw-r--r--   0 lau        (501) staff       (20)       59 2023-09-07 02:56:04.000000 totemlib-0.1.0.9/totemlib/security/__init__.py
+-rw-r--r--   0 lau        (501) staff       (20)     1150 2023-08-26 18:18:06.000000 totemlib-0.1.0.9/totemlib/security/auth.py
+-rw-r--r--   0 lau        (501) staff       (20)     4403 2023-09-05 13:35:57.000000 totemlib-0.1.0.9/totemlib/security/response_manager.py
+-rw-r--r--   0 lau        (501) staff       (20)     1480 2023-09-06 20:54:14.000000 totemlib-0.1.0.9/totemlib/security/validations.py
+drwxr-xr-x   0 lau        (501) staff       (20)        0 2023-09-09 00:43:38.204226 totemlib-0.1.0.9/totemlib/utils/
+-rw-r--r--   0 lau        (501) staff       (20)       67 2023-08-26 20:42:48.000000 totemlib-0.1.0.9/totemlib/utils/__init__.py
+-rw-r--r--   0 lau        (501) staff       (20)      834 2023-08-26 20:01:18.000000 totemlib-0.1.0.9/totemlib/utils/encrypter.py
+-rw-r--r--   0 lau        (501) staff       (20)     1689 2023-08-26 21:44:30.000000 totemlib-0.1.0.9/totemlib/utils/logger.py
+-rw-r--r--   0 lau        (501) staff       (20)      559 2023-08-26 21:39:51.000000 totemlib-0.1.0.9/totemlib/utils/privproperties.py
+drwxr-xr-x   0 lau        (501) staff       (20)        0 2023-09-09 00:43:38.200511 totemlib-0.1.0.9/totemlib.egg-info/
+-rw-r--r--   0 lau        (501) staff       (20)      167 2023-09-09 00:43:38.000000 totemlib-0.1.0.9/totemlib.egg-info/PKG-INFO
+-rw-r--r--   0 lau        (501) staff       (20)      554 2023-09-09 00:43:38.000000 totemlib-0.1.0.9/totemlib.egg-info/SOURCES.txt
+-rw-r--r--   0 lau        (501) staff       (20)        1 2023-09-09 00:43:38.000000 totemlib-0.1.0.9/totemlib.egg-info/dependency_links.txt
+-rw-r--r--   0 lau        (501) staff       (20)       19 2023-09-09 00:43:38.000000 totemlib-0.1.0.9/totemlib.egg-info/requires.txt
+-rw-r--r--   0 lau        (501) staff       (20)        9 2023-09-09 00:43:38.000000 totemlib-0.1.0.9/totemlib.egg-info/top_level.txt
```

### Comparing `totemlib-0.1.0.8/totemlib/data/conectDB.py` & `totemlib-0.1.0.9/totemlib/data/conectDB.py`

 * *Files identical despite different names*

### Comparing `totemlib-0.1.0.8/totemlib/data/datamanager.py` & `totemlib-0.1.0.9/totemlib/data/datamanager.py`

 * *Files identical despite different names*

### Comparing `totemlib-0.1.0.8/totemlib/security/auth.py` & `totemlib-0.1.0.9/totemlib/security/auth.py`

 * *Files identical despite different names*

### Comparing `totemlib-0.1.0.8/totemlib/security/response_manager.py` & `totemlib-0.1.0.9/totemlib/security/response_manager.py`

 * *Files identical despite different names*

### Comparing `totemlib-0.1.0.8/totemlib/security/validations.py` & `totemlib-0.1.0.9/totemlib/security/validations.py`

 * *Files identical despite different names*

### Comparing `totemlib-0.1.0.8/totemlib/utils/encrypter.py` & `totemlib-0.1.0.9/totemlib/utils/encrypter.py`

 * *Files identical despite different names*

### Comparing `totemlib-0.1.0.8/totemlib/utils/logger.py` & `totemlib-0.1.0.9/totemlib/utils/logger.py`

 * *Files identical despite different names*

### Comparing `totemlib-0.1.0.8/totemlib/utils/privproperties.py` & `totemlib-0.1.0.9/totemlib/utils/privproperties.py`

 * *Files identical despite different names*

### Comparing `totemlib-0.1.0.8/totemlib.egg-info/SOURCES.txt` & `totemlib-0.1.0.9/totemlib.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 totemlib.egg-info/SOURCES.txt
 totemlib.egg-info/dependency_links.txt
 totemlib.egg-info/requires.txt
 totemlib.egg-info/top_level.txt
 totemlib/data/__init__.py
 totemlib/data/conectDB.py
 totemlib/data/datamanager.py
+totemlib/data/transform.py
 totemlib/security/__init__.py
 totemlib/security/auth.py
 totemlib/security/response_manager.py
 totemlib/security/validations.py
 totemlib/utils/__init__.py
 totemlib/utils/encrypter.py
 totemlib/utils/logger.py
```

