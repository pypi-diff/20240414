# Comparing `tmp/simple_aula7-0.0.3.tar.gz` & `tmp/simple_aula7-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_aula7-0.0.3.tar", last modified: Sat Apr 13 22:44:17 2024, max compression
+gzip compressed data, was "simple_aula7-0.0.4.tar", last modified: Sat Apr 13 23:06:23 2024, max compression
```

## Comparing `simple_aula7-0.0.3.tar` & `simple_aula7-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:44:17.801768 simple_aula7-0.0.3/
--rw-r--r--   0 naiel      (501) staff       (20)     1068 2024-04-13 22:29:46.000000 simple_aula7-0.0.3/LICENSE
--rw-r--r--   0 naiel      (501) staff       (20)      451 2024-04-13 22:44:17.801515 simple_aula7-0.0.3/PKG-INFO
--rw-r--r--   0 naiel      (501) staff       (20)       36 2024-04-13 22:29:46.000000 simple_aula7-0.0.3/README.md
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:44:17.801322 simple_aula7-0.0.3/Simple_Aula7.egg-info/
--rw-r--r--   0 naiel      (501) staff       (20)      451 2024-04-13 22:44:17.000000 simple_aula7-0.0.3/Simple_Aula7.egg-info/PKG-INFO
--rw-r--r--   0 naiel      (501) staff       (20)      202 2024-04-13 22:44:17.000000 simple_aula7-0.0.3/Simple_Aula7.egg-info/SOURCES.txt
--rw-r--r--   0 naiel      (501) staff       (20)        1 2024-04-13 22:44:17.000000 simple_aula7-0.0.3/Simple_Aula7.egg-info/dependency_links.txt
--rw-r--r--   0 naiel      (501) staff       (20)        6 2024-04-13 22:44:17.000000 simple_aula7-0.0.3/Simple_Aula7.egg-info/top_level.txt
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:44:17.801045 simple_aula7-0.0.3/aula7/
--rw-r--r--   0 naiel      (501) staff       (20)       33 2024-04-13 22:04:30.000000 simple_aula7-0.0.3/aula7/__init__.py
--rw-r--r--   0 naiel      (501) staff       (20)     7889 2024-04-13 22:21:53.000000 simple_aula7-0.0.3/aula7/main.py
--rw-r--r--   0 naiel      (501) staff       (20)       38 2024-04-13 22:44:17.801811 simple_aula7-0.0.3/setup.cfg
--rw-r--r--   0 naiel      (501) staff       (20)      734 2024-04-13 22:44:07.000000 simple_aula7-0.0.3/setup.py
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 23:06:23.505159 simple_aula7-0.0.4/
+-rw-r--r--   0 naiel      (501) staff       (20)     1068 2024-04-13 22:29:46.000000 simple_aula7-0.0.4/LICENSE
+-rw-r--r--   0 naiel      (501) staff       (20)      451 2024-04-13 23:06:23.504800 simple_aula7-0.0.4/PKG-INFO
+-rw-r--r--   0 naiel      (501) staff       (20)       36 2024-04-13 22:29:46.000000 simple_aula7-0.0.4/README.md
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 23:06:23.504538 simple_aula7-0.0.4/Simple_Aula7.egg-info/
+-rw-r--r--   0 naiel      (501) staff       (20)      451 2024-04-13 23:06:23.000000 simple_aula7-0.0.4/Simple_Aula7.egg-info/PKG-INFO
+-rw-r--r--   0 naiel      (501) staff       (20)      202 2024-04-13 23:06:23.000000 simple_aula7-0.0.4/Simple_Aula7.egg-info/SOURCES.txt
+-rw-r--r--   0 naiel      (501) staff       (20)        1 2024-04-13 23:06:23.000000 simple_aula7-0.0.4/Simple_Aula7.egg-info/dependency_links.txt
+-rw-r--r--   0 naiel      (501) staff       (20)        6 2024-04-13 23:06:23.000000 simple_aula7-0.0.4/Simple_Aula7.egg-info/top_level.txt
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 23:06:23.504225 simple_aula7-0.0.4/aula7/
+-rw-r--r--   0 naiel      (501) staff       (20)       33 2024-04-13 22:04:30.000000 simple_aula7-0.0.4/aula7/__init__.py
+-rw-r--r--   0 naiel      (501) staff       (20)     7893 2024-04-13 23:03:16.000000 simple_aula7-0.0.4/aula7/main.py
+-rw-r--r--   0 naiel      (501) staff       (20)       38 2024-04-13 23:06:23.505203 simple_aula7-0.0.4/setup.cfg
+-rw-r--r--   0 naiel      (501) staff       (20)      734 2024-04-13 23:06:13.000000 simple_aula7-0.0.4/setup.py
```

### Comparing `simple_aula7-0.0.3/LICENSE` & `simple_aula7-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_aula7-0.0.3/aula7/main.py` & `simple_aula7-0.0.4/aula7/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from flask import Blueprint, render_template, redirect, request
 from simplesdk.internal import AulaSDK, AulaData, AlphacrmSDK
 from os import environ
 from dotenv import load_dotenv
 from urllib.parse import urlparse
 from simplesdk.translations import translation, language
 
+load_dotenv()
 loc = translation(
-    environ["ET_TRANSLATIONS"]
+    environ.get("ET_TRANSLATIONS")
     or "https://git.tech.eus/EuskadiTech/Translations/raw/branch/main/SimpleAxel.json"
 )
 
-load_dotenv()
 
 app = Blueprint("aula7", __name__, url_prefix="/aula7", template_folder="templates")
 client = AulaSDK(environ["ET_USER"], environ["ET_PASSWORD"], environ["ET_BASEURL"])
 client2 = AlphacrmSDK(environ["ET_USER"], environ["ET_PASSWORD"], environ["ET_BASEURL"])
 
 
 def login_session():
```

### Comparing `simple_aula7-0.0.3/setup.py` & `simple_aula7-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup  # type: ignore
 
 __project__ = "Simple-Aula7"
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 __description__ = (
     "Aula7 blueprint for SimpleAxel (https://git.tech.eus/EuskadiTech/Simple-Aula7)"
 )
 __packages__ = ["aula7"]
 __url__ = "https://git.tech.eus/EuskadiTech/Simple-Aula7"
 __author__ = "EuskadiTech"
 __classifiers__ = [
```

