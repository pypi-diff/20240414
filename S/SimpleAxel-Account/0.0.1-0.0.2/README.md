# Comparing `tmp/simpleaxel_account-0.0.1.tar.gz` & `tmp/simpleaxel_account-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleaxel_account-0.0.1.tar", last modified: Sat Apr 13 22:57:02 2024, max compression
+gzip compressed data, was "simpleaxel_account-0.0.2.tar", last modified: Sat Apr 13 23:05:07 2024, max compression
```

## Comparing `simpleaxel_account-0.0.1.tar` & `simpleaxel_account-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:57:02.752792 simpleaxel_account-0.0.1/
--rw-r--r--   0 naiel      (501) staff       (20)     1063 2024-04-13 22:52:31.000000 simpleaxel_account-0.0.1/LICENSE
--rw-r--r--   0 naiel      (501) staff       (20)      459 2024-04-13 22:57:02.752501 simpleaxel_account-0.0.1/PKG-INFO
--rw-r--r--   0 naiel      (501) staff       (20)       79 2024-04-13 22:54:45.000000 simpleaxel_account-0.0.1/README.md
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:57:02.752274 simpleaxel_account-0.0.1/SimpleAxel_Account.egg-info/
--rw-r--r--   0 naiel      (501) staff       (20)      459 2024-04-13 22:57:02.000000 simpleaxel_account-0.0.1/SimpleAxel_Account.egg-info/PKG-INFO
--rw-r--r--   0 naiel      (501) staff       (20)      230 2024-04-13 22:57:02.000000 simpleaxel_account-0.0.1/SimpleAxel_Account.egg-info/SOURCES.txt
--rw-r--r--   0 naiel      (501) staff       (20)        1 2024-04-13 22:57:02.000000 simpleaxel_account-0.0.1/SimpleAxel_Account.egg-info/dependency_links.txt
--rw-r--r--   0 naiel      (501) staff       (20)        8 2024-04-13 22:57:02.000000 simpleaxel_account-0.0.1/SimpleAxel_Account.egg-info/top_level.txt
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:57:02.751952 simpleaxel_account-0.0.1/account/
--rw-r--r--   0 naiel      (501) staff       (20)       35 2024-04-13 22:04:30.000000 simpleaxel_account-0.0.1/account/__init__.py
--rw-r--r--   0 naiel      (501) staff       (20)     1560 2024-04-13 22:25:26.000000 simpleaxel_account-0.0.1/account/main.py
--rw-r--r--   0 naiel      (501) staff       (20)       38 2024-04-13 22:57:02.752835 simpleaxel_account-0.0.1/setup.cfg
--rw-r--r--   0 naiel      (501) staff       (20)      744 2024-04-13 22:56:49.000000 simpleaxel_account-0.0.1/setup.py
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 23:05:07.606164 simpleaxel_account-0.0.2/
+-rw-r--r--   0 naiel      (501) staff       (20)     1063 2024-04-13 22:52:31.000000 simpleaxel_account-0.0.2/LICENSE
+-rw-r--r--   0 naiel      (501) staff       (20)      463 2024-04-13 23:05:07.605906 simpleaxel_account-0.0.2/PKG-INFO
+-rw-r--r--   0 naiel      (501) staff       (20)       79 2024-04-13 22:54:45.000000 simpleaxel_account-0.0.2/README.md
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 23:05:07.605705 simpleaxel_account-0.0.2/SimpleAxel_Account.egg-info/
+-rw-r--r--   0 naiel      (501) staff       (20)      463 2024-04-13 23:05:07.000000 simpleaxel_account-0.0.2/SimpleAxel_Account.egg-info/PKG-INFO
+-rw-r--r--   0 naiel      (501) staff       (20)      230 2024-04-13 23:05:07.000000 simpleaxel_account-0.0.2/SimpleAxel_Account.egg-info/SOURCES.txt
+-rw-r--r--   0 naiel      (501) staff       (20)        1 2024-04-13 23:05:07.000000 simpleaxel_account-0.0.2/SimpleAxel_Account.egg-info/dependency_links.txt
+-rw-r--r--   0 naiel      (501) staff       (20)        8 2024-04-13 23:05:07.000000 simpleaxel_account-0.0.2/SimpleAxel_Account.egg-info/top_level.txt
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 23:05:07.605530 simpleaxel_account-0.0.2/account/
+-rw-r--r--   0 naiel      (501) staff       (20)       35 2024-04-13 22:04:30.000000 simpleaxel_account-0.0.2/account/__init__.py
+-rw-r--r--   0 naiel      (501) staff       (20)     1564 2024-04-13 23:03:58.000000 simpleaxel_account-0.0.2/account/main.py
+-rw-r--r--   0 naiel      (501) staff       (20)       38 2024-04-13 23:05:07.606205 simpleaxel_account-0.0.2/setup.cfg
+-rw-r--r--   0 naiel      (501) staff       (20)      748 2024-04-13 23:04:14.000000 simpleaxel_account-0.0.2/setup.py
```

### Comparing `simpleaxel_account-0.0.1/LICENSE` & `simpleaxel_account-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleaxel_account-0.0.1/account/main.py` & `simpleaxel_account-0.0.2/account/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from flask import Blueprint, render_template, redirect, request
 from simplesdk.internal import AlphacrmSDK, AulaSDK
 from os import environ
 from dotenv import load_dotenv
 from simplesdk.translations import translation, language
 
+load_dotenv()
 loc = translation(
-    environ["ET_TRANSLATIONS"]
+    environ.get("ET_TRANSLATIONS")
     or "https://git.tech.eus/EuskadiTech/Translations/raw/branch/main/SimpleAxel.json"
 )
 
-load_dotenv()
 
 app = Blueprint("account", __name__, url_prefix="/account", template_folder="templates")
 client = AlphacrmSDK(environ["ET_USER"], environ["ET_PASSWORD"], environ["ET_BASEURL"])
 client2 = AulaSDK(environ["ET_USER"], environ["ET_PASSWORD"], environ["ET_BASEURL"])
 
 
 def login_session():
```

### Comparing `simpleaxel_account-0.0.1/setup.py` & `simpleaxel_account-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup  # type: ignore
 
 __project__ = "SimpleAxel-Account"
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 __description__ = (
-    "Pay blueprint for SimpleAxel (https://git.tech.eus/EuskadiTech/Simple-Account)"
+    "Account blueprint for SimpleAxel (https://git.tech.eus/EuskadiTech/Simple-Account)"
 )
 __packages__ = ["account"]
 __url__ = "https://git.tech.eus/EuskadiTech/Simple-Account"
 __author__ = "EuskadiTech"
 __classifiers__ = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

