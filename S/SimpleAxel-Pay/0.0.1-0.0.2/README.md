# Comparing `tmp/simpleaxel_pay-0.0.1.tar.gz` & `tmp/simpleaxel_pay-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpleaxel_pay-0.0.1.tar", last modified: Sat Apr 13 22:50:22 2024, max compression
+gzip compressed data, was "simpleaxel_pay-0.0.2.tar", last modified: Sat Apr 13 23:05:33 2024, max compression
```

## Comparing `simpleaxel_pay-0.0.1.tar` & `simpleaxel_pay-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:50:22.553312 simpleaxel_pay-0.0.1/
--rw-r--r--   0 naiel      (501) staff       (20)     1068 2024-04-13 22:48:25.000000 simpleaxel_pay-0.0.1/LICENSE
--rw-r--r--   0 naiel      (501) staff       (20)      455 2024-04-13 22:50:22.553025 simpleaxel_pay-0.0.1/PKG-INFO
--rw-r--r--   0 naiel      (501) staff       (20)       18 2024-04-13 22:48:25.000000 simpleaxel_pay-0.0.1/README.md
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:50:22.552811 simpleaxel_pay-0.0.1/SimpleAxel_Pay.egg-info/
--rw-r--r--   0 naiel      (501) staff       (20)      455 2024-04-13 22:50:22.000000 simpleaxel_pay-0.0.1/SimpleAxel_Pay.egg-info/PKG-INFO
--rw-r--r--   0 naiel      (501) staff       (20)      206 2024-04-13 22:50:22.000000 simpleaxel_pay-0.0.1/SimpleAxel_Pay.egg-info/SOURCES.txt
--rw-r--r--   0 naiel      (501) staff       (20)        1 2024-04-13 22:50:22.000000 simpleaxel_pay-0.0.1/SimpleAxel_Pay.egg-info/dependency_links.txt
--rw-r--r--   0 naiel      (501) staff       (20)        4 2024-04-13 22:50:22.000000 simpleaxel_pay-0.0.1/SimpleAxel_Pay.egg-info/top_level.txt
-drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 22:50:22.552636 simpleaxel_pay-0.0.1/pay/
--rw-r--r--   0 naiel      (501) staff       (20)       31 2024-04-13 22:04:30.000000 simpleaxel_pay-0.0.1/pay/__init__.py
--rw-r--r--   0 naiel      (501) staff       (20)     2757 2024-04-13 22:22:48.000000 simpleaxel_pay-0.0.1/pay/main.py
--rw-r--r--   0 naiel      (501) staff       (20)       38 2024-04-13 22:50:22.553351 simpleaxel_pay-0.0.1/setup.cfg
--rw-r--r--   0 naiel      (501) staff       (20)      736 2024-04-13 22:50:21.000000 simpleaxel_pay-0.0.1/setup.py
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 23:05:33.911178 simpleaxel_pay-0.0.2/
+-rw-r--r--   0 naiel      (501) staff       (20)     1068 2024-04-13 22:48:25.000000 simpleaxel_pay-0.0.2/LICENSE
+-rw-r--r--   0 naiel      (501) staff       (20)      455 2024-04-13 23:05:33.910835 simpleaxel_pay-0.0.2/PKG-INFO
+-rw-r--r--   0 naiel      (501) staff       (20)       18 2024-04-13 22:48:25.000000 simpleaxel_pay-0.0.2/README.md
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 23:05:33.910568 simpleaxel_pay-0.0.2/SimpleAxel_Pay.egg-info/
+-rw-r--r--   0 naiel      (501) staff       (20)      455 2024-04-13 23:05:33.000000 simpleaxel_pay-0.0.2/SimpleAxel_Pay.egg-info/PKG-INFO
+-rw-r--r--   0 naiel      (501) staff       (20)      206 2024-04-13 23:05:33.000000 simpleaxel_pay-0.0.2/SimpleAxel_Pay.egg-info/SOURCES.txt
+-rw-r--r--   0 naiel      (501) staff       (20)        1 2024-04-13 23:05:33.000000 simpleaxel_pay-0.0.2/SimpleAxel_Pay.egg-info/dependency_links.txt
+-rw-r--r--   0 naiel      (501) staff       (20)        4 2024-04-13 23:05:33.000000 simpleaxel_pay-0.0.2/SimpleAxel_Pay.egg-info/top_level.txt
+drwxr-xr-x   0 naiel      (501) staff       (20)        0 2024-04-13 23:05:33.910276 simpleaxel_pay-0.0.2/pay/
+-rw-r--r--   0 naiel      (501) staff       (20)       31 2024-04-13 22:04:30.000000 simpleaxel_pay-0.0.2/pay/__init__.py
+-rw-r--r--   0 naiel      (501) staff       (20)     2760 2024-04-13 23:04:06.000000 simpleaxel_pay-0.0.2/pay/main.py
+-rw-r--r--   0 naiel      (501) staff       (20)       38 2024-04-13 23:05:33.911222 simpleaxel_pay-0.0.2/setup.cfg
+-rw-r--r--   0 naiel      (501) staff       (20)      736 2024-04-13 23:05:29.000000 simpleaxel_pay-0.0.2/setup.py
```

### Comparing `simpleaxel_pay-0.0.1/LICENSE` & `simpleaxel_pay-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simpleaxel_pay-0.0.1/pay/main.py` & `simpleaxel_pay-0.0.2/pay/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from flask import Blueprint, redirect, request
 from simplesdk.internal import AlphacrmSDK, AulaSDK
 from os import environ
 from dotenv import load_dotenv
 import stripe
 from simplesdk.translations import translation, language
 
+load_dotenv()
 loc = translation(
-    environ["ET_TRANSLATIONS"]
+    environ.get("ET_TRANSLATIONS")
     or "https://git.tech.eus/EuskadiTech/Translations/raw/branch/main/SimpleAxel.json"
 )
 
 stripe.api_key = environ["ET_STRIPE_API_KEY"]
 
 
-load_dotenv()
-
 app = Blueprint("pay", __name__, url_prefix="/pay", template_folder="templates")
 client = AlphacrmSDK(environ["ET_USER"], environ["ET_PASSWORD"], environ["ET_BASEURL"])
 client2 = AulaSDK(environ["ET_USER"], environ["ET_PASSWORD"], environ["ET_BASEURL"])
 
 
 def login_session():
     user = client.login_with_session(request.cookies.get("et_auth_session"))
```

### Comparing `simpleaxel_pay-0.0.1/setup.py` & `simpleaxel_pay-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup  # type: ignore
 
 __project__ = "SimpleAxel-Pay"
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 __description__ = (
     "Pay blueprint for SimpleAxel (https://git.tech.eus/EuskadiTech/SimpleAxel-Pay)"
 )
 __packages__ = ["pay"]
 __url__ = "https://git.tech.eus/EuskadiTech/SimpleAxel-Pay"
 __author__ = "EuskadiTech"
 __classifiers__ = [
```

