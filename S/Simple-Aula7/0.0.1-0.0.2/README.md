# Comparing `tmp/simple_aula7-0.0.1.tar.gz` & `tmp/simple_aula7-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_aula7-0.0.1.tar", last modified: Sat Apr 13 22:34:23 2024, max compression
+gzip compressed data, was "simple_aula7-0.0.2.tar", last modified: Sat Apr 13 22:37:08 2024, max compression
```

## Comparing `simple_aula7-0.0.1.tar` & `simple_aula7-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:34:23.488421 simple_aula7-0.0.1/
--rw-r--r--   0 naiel      (501) staff       (20)     1068 2024-04-13 22:29:46.000000 simple_aula7-0.0.1/LICENSE
--rw-r--r--   0 naiel      (501) staff       (20)      398 2024-04-13 22:34:23.488118 simple_aula7-0.0.1/PKG-INFO
--rw-r--r--   0 naiel      (501) staff       (20)       36 2024-04-13 22:29:46.000000 simple_aula7-0.0.1/README.md
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:34:23.487896 simple_aula7-0.0.1/Simple_Aula7.egg-info/
--rw-r--r--   0 naiel      (501) staff       (20)      398 2024-04-13 22:34:23.000000 simple_aula7-0.0.1/Simple_Aula7.egg-info/PKG-INFO
--rw-r--r--   0 naiel      (501) staff       (20)      202 2024-04-13 22:34:23.000000 simple_aula7-0.0.1/Simple_Aula7.egg-info/SOURCES.txt
--rw-r--r--   0 naiel      (501) staff       (20)        1 2024-04-13 22:34:23.000000 simple_aula7-0.0.1/Simple_Aula7.egg-info/dependency_links.txt
--rw-r--r--   0 naiel      (501) staff       (20)        6 2024-04-13 22:34:23.000000 simple_aula7-0.0.1/Simple_Aula7.egg-info/top_level.txt
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:34:23.487509 simple_aula7-0.0.1/aula7/
--rw-r--r--   0 naiel      (501) staff       (20)       33 2024-04-13 22:04:30.000000 simple_aula7-0.0.1/aula7/__init__.py
--rw-r--r--   0 naiel      (501) staff       (20)     7889 2024-04-13 22:21:53.000000 simple_aula7-0.0.1/aula7/main.py
--rw-r--r--   0 naiel      (501) staff       (20)       38 2024-04-13 22:34:23.488462 simple_aula7-0.0.1/setup.cfg
--rw-r--r--   0 naiel      (501) staff       (20)      702 2024-04-13 22:33:51.000000 simple_aula7-0.0.1/setup.py
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:37:08.895920 simple_aula7-0.0.2/
+-rw-r--r--   0 naiel      (501) staff       (20)     1068 2024-04-13 22:29:46.000000 simple_aula7-0.0.2/LICENSE
+-rw-r--r--   0 naiel      (501) staff       (20)      398 2024-04-13 22:37:08.895576 simple_aula7-0.0.2/PKG-INFO
+-rw-r--r--   0 naiel      (501) staff       (20)       36 2024-04-13 22:29:46.000000 simple_aula7-0.0.2/README.md
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:37:08.895334 simple_aula7-0.0.2/Simple_Aula7.egg-info/
+-rw-r--r--   0 naiel      (501) staff       (20)      398 2024-04-13 22:37:08.000000 simple_aula7-0.0.2/Simple_Aula7.egg-info/PKG-INFO
+-rw-r--r--   0 naiel      (501) staff       (20)      202 2024-04-13 22:37:08.000000 simple_aula7-0.0.2/Simple_Aula7.egg-info/SOURCES.txt
+-rw-r--r--   0 naiel      (501) staff       (20)        1 2024-04-13 22:37:08.000000 simple_aula7-0.0.2/Simple_Aula7.egg-info/dependency_links.txt
+-rw-r--r--   0 naiel      (501) staff       (20)        6 2024-04-13 22:37:08.000000 simple_aula7-0.0.2/Simple_Aula7.egg-info/top_level.txt
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:37:08.895026 simple_aula7-0.0.2/aula7/
+-rw-r--r--   0 naiel      (501) staff       (20)       33 2024-04-13 22:04:30.000000 simple_aula7-0.0.2/aula7/__init__.py
+-rw-r--r--   0 naiel      (501) staff       (20)     7889 2024-04-13 22:21:53.000000 simple_aula7-0.0.2/aula7/main.py
+-rw-r--r--   0 naiel      (501) staff       (20)       38 2024-04-13 22:37:08.895966 simple_aula7-0.0.2/setup.cfg
+-rw-r--r--   0 naiel      (501) staff       (20)      702 2024-04-13 22:36:56.000000 simple_aula7-0.0.2/setup.py
```

### Comparing `simple_aula7-0.0.1/LICENSE` & `simple_aula7-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_aula7-0.0.1/aula7/main.py` & `simple_aula7-0.0.2/aula7/main.py`

 * *Files identical despite different names*

### Comparing `simple_aula7-0.0.1/setup.py` & `simple_aula7-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup  # type: ignore
 
 __project__ = "Simple-Aula7"
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 __description__ = (
     "Aula7 blueprint for SimpleAxel (https://git.tech.eus/EuskadiTech/Simple-Aula7)"
 )
 __packages__ = ["aula7"]
 __url__ = "https://git.tech.eus/EuskadiTech/Simple-Aula7"
 __author__ = "EuskadiTech"
 __classifiers__ = [
```

