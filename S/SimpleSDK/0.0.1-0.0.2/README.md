# Comparing `tmp/simplesdk-0.0.1.tar.gz` & `tmp/simplesdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplesdk-0.0.1.tar", last modified: Sat Apr 13 22:01:12 2024, max compression
+gzip compressed data, was "simplesdk-0.0.2.tar", last modified: Sat Apr 13 22:14:46 2024, max compression
```

## Comparing `simplesdk-0.0.1.tar` & `simplesdk-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:01:12.160388 simplesdk-0.0.1/
--rw-r--r--   0 naiel      (501) staff       (20)     1063 2024-04-13 21:41:46.000000 simplesdk-0.0.1/LICENSE
--rw-r--r--   0 naiel      (501) staff       (20)      392 2024-04-13 22:01:12.160176 simplesdk-0.0.1/PKG-INFO
--rw-r--r--   0 naiel      (501) staff       (20)       53 2024-04-13 21:41:46.000000 simplesdk-0.0.1/README.md
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:01:12.159911 simplesdk-0.0.1/SimpleSDK.egg-info/
--rw-r--r--   0 naiel      (501) staff       (20)      392 2024-04-13 22:01:12.000000 simplesdk-0.0.1/SimpleSDK.egg-info/PKG-INFO
--rw-r--r--   0 naiel      (501) staff       (20)      202 2024-04-13 22:01:12.000000 simplesdk-0.0.1/SimpleSDK.egg-info/SOURCES.txt
--rw-r--r--   0 naiel      (501) staff       (20)        1 2024-04-13 22:01:12.000000 simplesdk-0.0.1/SimpleSDK.egg-info/dependency_links.txt
--rw-r--r--   0 naiel      (501) staff       (20)       10 2024-04-13 22:01:12.000000 simplesdk-0.0.1/SimpleSDK.egg-info/top_level.txt
--rw-r--r--   0 naiel      (501) staff       (20)       38 2024-04-13 22:01:12.160461 simplesdk-0.0.1/setup.cfg
--rw-r--r--   0 naiel      (501) staff       (20)      700 2024-04-13 21:55:52.000000 simplesdk-0.0.1/setup.py
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:01:12.159502 simplesdk-0.0.1/simplesdk/
--rw-r--r--   0 naiel      (501) staff       (20)       23 2024-04-13 21:56:32.000000 simplesdk-0.0.1/simplesdk/__init__.py
--rw-r--r--   0 naiel      (501) staff       (20)    11876 2024-04-13 21:46:58.000000 simplesdk-0.0.1/simplesdk/internal.py
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:14:46.579743 simplesdk-0.0.2/
+-rw-r--r--   0 naiel      (501) staff       (20)     1063 2024-04-13 21:41:46.000000 simplesdk-0.0.2/LICENSE
+-rw-r--r--   0 naiel      (501) staff       (20)      392 2024-04-13 22:14:46.579391 simplesdk-0.0.2/PKG-INFO
+-rw-r--r--   0 naiel      (501) staff       (20)       53 2024-04-13 21:41:46.000000 simplesdk-0.0.2/README.md
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:14:46.579151 simplesdk-0.0.2/SimpleSDK.egg-info/
+-rw-r--r--   0 naiel      (501) staff       (20)      392 2024-04-13 22:14:46.000000 simplesdk-0.0.2/SimpleSDK.egg-info/PKG-INFO
+-rw-r--r--   0 naiel      (501) staff       (20)      227 2024-04-13 22:14:46.000000 simplesdk-0.0.2/SimpleSDK.egg-info/SOURCES.txt
+-rw-r--r--   0 naiel      (501) staff       (20)        1 2024-04-13 22:14:46.000000 simplesdk-0.0.2/SimpleSDK.egg-info/dependency_links.txt
+-rw-r--r--   0 naiel      (501) staff       (20)       10 2024-04-13 22:14:46.000000 simplesdk-0.0.2/SimpleSDK.egg-info/top_level.txt
+-rw-r--r--   0 naiel      (501) staff       (20)       38 2024-04-13 22:14:46.579787 simplesdk-0.0.2/setup.cfg
+-rw-r--r--   0 naiel      (501) staff       (20)      700 2024-04-13 22:14:44.000000 simplesdk-0.0.2/setup.py
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:14:46.578781 simplesdk-0.0.2/simplesdk/
+-rw-r--r--   0 naiel      (501) staff       (20)       23 2024-04-13 21:56:32.000000 simplesdk-0.0.2/simplesdk/__init__.py
+-rw-r--r--   0 naiel      (501) staff       (20)    11876 2024-04-13 21:46:58.000000 simplesdk-0.0.2/simplesdk/internal.py
+-rw-r--r--   0 naiel      (501) staff       (20)      270 2024-04-13 22:13:55.000000 simplesdk-0.0.2/simplesdk/translatons.py
```

### Comparing `simplesdk-0.0.1/LICENSE` & `simplesdk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simplesdk-0.0.1/setup.py` & `simplesdk-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup  # type: ignore
 
 __project__ = "SimpleSDK"
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 __description__ = (
     "SDK for EuskadiTech's Simple Axel (https://git.tech.eus/EuskadiTech/SimpleSDK)"
 )
 __packages__ = ["simplesdk"]
 __url__ = "https://git.tech.eus/EuskadiTech/SimpleSDK"
 __author__ = "EuskadiTech"
 __classifiers__ = [
```

### Comparing `simplesdk-0.0.1/simplesdk/internal.py` & `simplesdk-0.0.2/simplesdk/internal.py`

 * *Files identical despite different names*

