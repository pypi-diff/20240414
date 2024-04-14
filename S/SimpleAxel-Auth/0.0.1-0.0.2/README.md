# Comparing `tmp/simpleaxel_auth-0.0.1.tar.gz` & `tmp/simpleaxel_auth-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleaxel_auth-0.0.1.tar", last modified: Sat Apr 13 22:45:09 2024, max compression
+gzip compressed data, was "simpleaxel_auth-0.0.2.tar", last modified: Sat Apr 13 23:05:58 2024, max compression
```

## Comparing `simpleaxel_auth-0.0.1.tar` & `simpleaxel_auth-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:45:09.578104 simpleaxel_auth-0.0.1/
--rw-r--r--   0 naiel      (501) staff       (20)     1068 2024-04-13 22:39:42.000000 simpleaxel_auth-0.0.1/LICENSE
--rw-r--r--   0 naiel      (501) staff       (20)      451 2024-04-13 22:45:09.577783 simpleaxel_auth-0.0.1/PKG-INFO
--rw-r--r--   0 naiel      (501) staff       (20)       15 2024-04-13 22:39:42.000000 simpleaxel_auth-0.0.1/README.md
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:45:09.577544 simpleaxel_auth-0.0.1/SimpleAxel_Auth.egg-info/
--rw-r--r--   0 naiel      (501) staff       (20)      451 2024-04-13 22:45:09.000000 simpleaxel_auth-0.0.1/SimpleAxel_Auth.egg-info/PKG-INFO
--rw-r--r--   0 naiel      (501) staff       (20)      212 2024-04-13 22:45:09.000000 simpleaxel_auth-0.0.1/SimpleAxel_Auth.egg-info/SOURCES.txt
--rw-r--r--   0 naiel      (501) staff       (20)        1 2024-04-13 22:45:09.000000 simpleaxel_auth-0.0.1/SimpleAxel_Auth.egg-info/dependency_links.txt
--rw-r--r--   0 naiel      (501) staff       (20)        5 2024-04-13 22:45:09.000000 simpleaxel_auth-0.0.1/SimpleAxel_Auth.egg-info/top_level.txt
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:45:09.577230 simpleaxel_auth-0.0.1/auth/
--rw-r--r--   0 naiel      (501) staff       (20)       32 2024-04-13 22:04:30.000000 simpleaxel_auth-0.0.1/auth/__init__.py
--rw-r--r--   0 naiel      (501) staff       (20)     3046 2024-04-13 22:25:32.000000 simpleaxel_auth-0.0.1/auth/main.py
--rw-r--r--   0 naiel      (501) staff       (20)       38 2024-04-13 22:45:09.578150 simpleaxel_auth-0.0.1/setup.cfg
--rw-r--r--   0 naiel      (501) staff       (20)      733 2024-04-13 22:44:55.000000 simpleaxel_auth-0.0.1/setup.py
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 23:05:58.683004 simpleaxel_auth-0.0.2/
+-rw-r--r--   0 naiel      (501) staff       (20)     1068 2024-04-13 22:39:42.000000 simpleaxel_auth-0.0.2/LICENSE
+-rw-r--r--   0 naiel      (501) staff       (20)      451 2024-04-13 23:05:58.682726 simpleaxel_auth-0.0.2/PKG-INFO
+-rw-r--r--   0 naiel      (501) staff       (20)       73 2024-04-13 22:46:19.000000 simpleaxel_auth-0.0.2/README.md
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 23:05:58.682507 simpleaxel_auth-0.0.2/SimpleAxel_Auth.egg-info/
+-rw-r--r--   0 naiel      (501) staff       (20)      451 2024-04-13 23:05:58.000000 simpleaxel_auth-0.0.2/SimpleAxel_Auth.egg-info/PKG-INFO
+-rw-r--r--   0 naiel      (501) staff       (20)      212 2024-04-13 23:05:58.000000 simpleaxel_auth-0.0.2/SimpleAxel_Auth.egg-info/SOURCES.txt
+-rw-r--r--   0 naiel      (501) staff       (20)        1 2024-04-13 23:05:58.000000 simpleaxel_auth-0.0.2/SimpleAxel_Auth.egg-info/dependency_links.txt
+-rw-r--r--   0 naiel      (501) staff       (20)        5 2024-04-13 23:05:58.000000 simpleaxel_auth-0.0.2/SimpleAxel_Auth.egg-info/top_level.txt
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 23:05:58.682241 simpleaxel_auth-0.0.2/auth/
+-rw-r--r--   0 naiel      (501) staff       (20)       32 2024-04-13 22:04:30.000000 simpleaxel_auth-0.0.2/auth/__init__.py
+-rw-r--r--   0 naiel      (501) staff       (20)     3050 2024-04-13 23:03:34.000000 simpleaxel_auth-0.0.2/auth/main.py
+-rw-r--r--   0 naiel      (501) staff       (20)       38 2024-04-13 23:05:58.683051 simpleaxel_auth-0.0.2/setup.cfg
+-rw-r--r--   0 naiel      (501) staff       (20)      733 2024-04-13 23:05:56.000000 simpleaxel_auth-0.0.2/setup.py
```

### Comparing `simpleaxel_auth-0.0.1/LICENSE` & `simpleaxel_auth-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleaxel_auth-0.0.1/auth/main.py` & `simpleaxel_auth-0.0.2/auth/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 from simplesdk.internal import AlphacrmSDK, safe_hash, uuid4
 from os import environ
 from dotenv import load_dotenv
 from datetime import datetime, timedelta
 from random import randrange
 from simplesdk.translations import translation, language
 
+load_dotenv()
 loc = translation(
-    environ["ET_TRANSLATIONS"]
+    environ.get("ET_TRANSLATIONS")
     or "https://git.tech.eus/EuskadiTech/Translations/raw/branch/main/SimpleAxel.json"
 )
 
-load_dotenv()
 
 app = Blueprint("auth", __name__, url_prefix="/auth", template_folder="templates")
 client = AlphacrmSDK(environ["ET_USER"], environ["ET_PASSWORD"], environ["ET_BASEURL"])
 
 
 def login_session():
     user = client.login_with_session(request.cookies.get("et_auth_session"))
```

### Comparing `simpleaxel_auth-0.0.1/setup.py` & `simpleaxel_auth-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup  # type: ignore
 
 __project__ = "SimpleAxel-Auth"
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 __description__ = (
     "Auth blueprint for SimpleAxel (https://git.tech.eus/EuskadiTech/Simple-Auth)"
 )
 __packages__ = ["auth"]
 __url__ = "https://git.tech.eus/EuskadiTech/Simple-Auth"
 __author__ = "EuskadiTech"
 __classifiers__ = [
```

