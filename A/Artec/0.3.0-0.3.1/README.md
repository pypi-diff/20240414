# Comparing `tmp/Artec-0.3.0.tar.gz` & `tmp/artec-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Artec-0.3.0.tar", last modified: Sun Aug  6 10:42:43 2023, max compression
+gzip compressed data, was "artec-0.3.1.tar", last modified: Sun Apr 14 17:04:45 2024, max compression
```

## Comparing `Artec-0.3.0.tar` & `artec-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:42:43.295436 Artec-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:42:43.291436 Artec-0.3.0/Artec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    47094 2023-08-06 10:42:43.000000 Artec-0.3.0/Artec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-06 10:42:43.000000 Artec-0.3.0/Artec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 10:42:43.000000 Artec-0.3.0/Artec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-06 10:42:43.000000 Artec-0.3.0/Artec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-06 10:42:43.000000 Artec-0.3.0/Artec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-06 10:42:43.000000 Artec-0.3.0/Artec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-08-06 10:42:33.000000 Artec-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    47094 2023-08-06 10:42:43.291436 Artec-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-08-06 10:42:33.000000 Artec-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:42:43.291436 Artec-0.3.0/artec/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-08-06 10:42:33.000000 Artec-0.3.0/artec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-06 10:42:33.000000 Artec-0.3.0/artec/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-08-06 10:42:33.000000 Artec-0.3.0/artec/argparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-08-06 10:42:33.000000 Artec-0.3.0/artec/boiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-08-06 10:42:33.000000 Artec-0.3.0/artec/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-08-06 10:42:33.000000 Artec-0.3.0/artec/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-08-06 10:42:33.000000 Artec-0.3.0/artec/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-06 10:42:33.000000 Artec-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 10:42:43.295436 Artec-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 10:42:33.000000 Artec-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 10:42:43.291436 Artec-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-08-06 10:42:33.000000 Artec-0.3.0/test/test_boiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-08-06 10:42:33.000000 Artec-0.3.0/test/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-08-06 10:42:33.000000 Artec-0.3.0/test/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:04:45.325901 artec-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:04:45.325901 artec-0.3.1/Artec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    43765 2024-04-14 17:04:45.000000 artec-0.3.1/Artec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-14 17:04:45.000000 artec-0.3.1/Artec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 17:04:45.000000 artec-0.3.1/Artec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-14 17:04:45.000000 artec-0.3.1/Artec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-14 17:04:45.000000 artec-0.3.1/Artec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 17:04:45.000000 artec-0.3.1/Artec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-04-14 17:04:36.000000 artec-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    43765 2024-04-14 17:04:45.325901 artec-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-14 17:04:36.000000 artec-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:04:45.325901 artec-0.3.1/artec/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-14 17:04:36.000000 artec-0.3.1/artec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-14 17:04:36.000000 artec-0.3.1/artec/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-14 17:04:36.000000 artec-0.3.1/artec/argparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-14 17:04:36.000000 artec-0.3.1/artec/boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-14 17:04:36.000000 artec-0.3.1/artec/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-14 17:04:36.000000 artec-0.3.1/artec/repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:04:45.325901 artec-0.3.1/artec/temp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-14 17:04:36.000000 artec-0.3.1/artec/temp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-14 17:04:36.000000 artec-0.3.1/artec/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-14 17:04:36.000000 artec-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 17:04:45.325901 artec-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 17:04:36.000000 artec-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:04:45.325901 artec-0.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-14 17:04:36.000000 artec-0.3.1/test/test_boiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-04-14 17:04:36.000000 artec-0.3.1/test/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-14 17:04:36.000000 artec-0.3.1/test/test_parser.py
```

### Comparing `Artec-0.3.0/Artec.egg-info/PKG-INFO` & `artec-0.3.1/Artec.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Artec
-Version: 0.3.0
+Version: 0.3.1
 Summary: Creates a configurable python project template in a given directory.
 Author-email: HushmKun <HushmKun@outlook.com>, Link- <bsm.dgdy@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -682,17 +682,21 @@
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: GitPython
 Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest; extra == "test"
 
 ![Logo](img/Artec.png)
 # Artec
 A python application that creates a configurable python project template in a given directory.<br>
 _It's a maintained version of PyBoiler_
 
 ## Installation
@@ -711,25 +715,29 @@
 ```
 ## Usage
 Create a JSON file to match the folder structure you desire
 ```
 $ vim structure.json 
     
 # Paste the below into your file and modify as you desire
-[
-    {"folder": "{}"},           # Use '{}' to be replaced with project name.
-    {"file": "{}/__init__.py"},
-    {"folder": "test"},
-    {"file": "test/__init__.py"},
-    {"file": "README.md"},
-    {"file": "LICENSE"},
-    {"file": "setup.py"},
-    {"file": "setup.cfg"},
-    {"file": "pyproject.toml"},
-]
+{
+    "folders": [
+        "{}",
+        "test"
+    ], 
+    "files": [
+        "{}/__init__.py",
+        "test/__init__.py",
+        "README.md",
+        "LICENSE",
+        "setup.py",
+        "pyproject.toml"
+    ]
+}
+
 ```
 How to execute
 ```
 $ artec -h
 usage: artec [OPTIONS] -o [DEST] 
 
 Artec is a python application that creates a configurable python project template in a given directory.
@@ -752,149 +760,22 @@
         artec -o dest
         artec -o dest -t python
         artec -o dest -s structure.json
         artec -o dest -s structure.json -v
 ```
 
 ## Templates
-<details>
-<summary> Python </summary>
-
-Project Named Artec 
-```
-artec
-├── artec
-│   └── __main__.py
-├── test
-│   └── __init__.py
-├── LICENSE
-├── pyproject.toml
-├── README.md
-├── setup.cfg
-└── setup.py
- 
-2 directories, 7 files
-```
-</details>
-
-<details>
-<summary> Flask </summary>
-
-Project Named flaskr 
-```
-flaskr
-.
-├── flaskr
-│   ├── auth.py
-│   ├── blog
-│   │   ├── create.html
-│   │   ├── index.html
-│   │   └── update.html
-│   ├── blog.py
-│   ├── db.py
-│   ├── __init__.py
-│   ├── schema.py
-│   ├── static
-│   │   └── style.css
-│   └── templates
-│       ├── auth
-│       │   ├── login.html
-│       │   └── register.html
-│       └── base.html
-├── LICENSE
-├── pyproject.toml
-├── README.md
-├── setup.py
-└── test
-    ├── conftest.py
-    ├── data.sql
-    ├── __init__.py
-    ├── test_auth.py
-    ├── test_blog.py
-    └── test_db.py
-
-7 directories, 22 files
-```
-</details>
-<details>
-<summary> Node.Js </summary>
-
-Project Named Node 
-```
-Node
-├── LICENSE
-├── package.json
-├── package-lock.json
-├── README.md
-└── src
-    ├── api
-    │   ├── controllers
-    │   │   └── user
-    │   │       ├── auth
-    │   │       │   ├── forgot-password.js
-    │   │       │   ├── login.js
-    │   │       │   ├── logout.js
-    │   │       │   ├── refresh-token.js
-    │   │       │   ├── register.js
-    │   │       │   ├── send-verification-code.js
-    │   │       │   └── verify-email.js
-    │   │       ├── delete-user.js
-    │   │       ├── edit
-    │   │       │   ├── change-password.js
-    │   │       │   └── edit-user.js
-    │   │       ├── get-user.js
-    │   │       └── index.js
-    │   ├── middlewares
-    │   │   ├── auth
-    │   │   │   ├── check-auth.js
-    │   │   │   └── check-authority.js
-    │   │   ├── image-upload.js
-    │   │   ├── index.js
-    │   │   ├── object-id-control.js
-    │   │   └── rate-limiter.js
-    │   ├── routes
-    │   │   ├── index.js
-    │   │   └── user.js
-    │   └── validators
-    │       ├── index.js
-    │       └── user.validator.js
-    ├── app.js
-    ├── config
-    │   └── index.js
-    ├── loaders
-    │   ├── express.js
-    │   ├── index.js
-    │   └── mongoose.js
-    ├── models
-    │   ├── index.js
-    │   ├── log.js
-    │   ├── token.js
-    │   └── user.js
-    └── utils
-        ├── helpers
-        │   ├── error-helper.js
-        │   ├── generate-random-code.js
-        │   ├── ip-helper.js
-        │   ├── jwt-token-helper.js
-        │   └── local-text-helper.js
-        ├── index.js
-        ├── lang
-        │   ├── en.json
-        │   ├── get-text.json
-        │   └── tr.json
-        ├── logger.js
-        └── send-code-to-email.js
-
-17 directories, 46 files
-```
-</details>
+- Python
+- Flask 
+- Node.Js
+- Data_Science
 
 ## Version
 
-    0.3.0
+    0.3.1
 
 ## Contributing
 Please refer to [Here](CONTRIBUTING.md) for contributing.
 Any help that can contribute to the templates will be really appreciated.
 
 * Big Thanks to [Link-](https://github.com/Link-) for jump starting the project.
 * Thanks for [Narayandas Akhil Achary](https://github.com/0018akhil) for various fixes & features.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Artec-0.3.0/LICENSE` & `artec-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Artec-0.3.0/PKG-INFO` & `artec-0.3.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Artec
-Version: 0.3.0
+Version: 0.3.1
 Summary: Creates a configurable python project template in a given directory.
 Author-email: HushmKun <HushmKun@outlook.com>, Link- <bsm.dgdy@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -682,17 +682,21 @@
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Build Tools
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: GitPython
 Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: flake8; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest; extra == "test"
 
 ![Logo](img/Artec.png)
 # Artec
 A python application that creates a configurable python project template in a given directory.<br>
 _It's a maintained version of PyBoiler_
 
 ## Installation
@@ -711,25 +715,29 @@
 ```
 ## Usage
 Create a JSON file to match the folder structure you desire
 ```
 $ vim structure.json 
     
 # Paste the below into your file and modify as you desire
-[
-    {"folder": "{}"},           # Use '{}' to be replaced with project name.
-    {"file": "{}/__init__.py"},
-    {"folder": "test"},
-    {"file": "test/__init__.py"},
-    {"file": "README.md"},
-    {"file": "LICENSE"},
-    {"file": "setup.py"},
-    {"file": "setup.cfg"},
-    {"file": "pyproject.toml"},
-]
+{
+    "folders": [
+        "{}",
+        "test"
+    ], 
+    "files": [
+        "{}/__init__.py",
+        "test/__init__.py",
+        "README.md",
+        "LICENSE",
+        "setup.py",
+        "pyproject.toml"
+    ]
+}
+
 ```
 How to execute
 ```
 $ artec -h
 usage: artec [OPTIONS] -o [DEST] 
 
 Artec is a python application that creates a configurable python project template in a given directory.
@@ -752,149 +760,22 @@
         artec -o dest
         artec -o dest -t python
         artec -o dest -s structure.json
         artec -o dest -s structure.json -v
 ```
 
 ## Templates
-<details>
-<summary> Python </summary>
-
-Project Named Artec 
-```
-artec
-├── artec
-│   └── __main__.py
-├── test
-│   └── __init__.py
-├── LICENSE
-├── pyproject.toml
-├── README.md
-├── setup.cfg
-└── setup.py
- 
-2 directories, 7 files
-```
-</details>
-
-<details>
-<summary> Flask </summary>
-
-Project Named flaskr 
-```
-flaskr
-.
-├── flaskr
-│   ├── auth.py
-│   ├── blog
-│   │   ├── create.html
-│   │   ├── index.html
-│   │   └── update.html
-│   ├── blog.py
-│   ├── db.py
-│   ├── __init__.py
-│   ├── schema.py
-│   ├── static
-│   │   └── style.css
-│   └── templates
-│       ├── auth
-│       │   ├── login.html
-│       │   └── register.html
-│       └── base.html
-├── LICENSE
-├── pyproject.toml
-├── README.md
-├── setup.py
-└── test
-    ├── conftest.py
-    ├── data.sql
-    ├── __init__.py
-    ├── test_auth.py
-    ├── test_blog.py
-    └── test_db.py
-
-7 directories, 22 files
-```
-</details>
-<details>
-<summary> Node.Js </summary>
-
-Project Named Node 
-```
-Node
-├── LICENSE
-├── package.json
-├── package-lock.json
-├── README.md
-└── src
-    ├── api
-    │   ├── controllers
-    │   │   └── user
-    │   │       ├── auth
-    │   │       │   ├── forgot-password.js
-    │   │       │   ├── login.js
-    │   │       │   ├── logout.js
-    │   │       │   ├── refresh-token.js
-    │   │       │   ├── register.js
-    │   │       │   ├── send-verification-code.js
-    │   │       │   └── verify-email.js
-    │   │       ├── delete-user.js
-    │   │       ├── edit
-    │   │       │   ├── change-password.js
-    │   │       │   └── edit-user.js
-    │   │       ├── get-user.js
-    │   │       └── index.js
-    │   ├── middlewares
-    │   │   ├── auth
-    │   │   │   ├── check-auth.js
-    │   │   │   └── check-authority.js
-    │   │   ├── image-upload.js
-    │   │   ├── index.js
-    │   │   ├── object-id-control.js
-    │   │   └── rate-limiter.js
-    │   ├── routes
-    │   │   ├── index.js
-    │   │   └── user.js
-    │   └── validators
-    │       ├── index.js
-    │       └── user.validator.js
-    ├── app.js
-    ├── config
-    │   └── index.js
-    ├── loaders
-    │   ├── express.js
-    │   ├── index.js
-    │   └── mongoose.js
-    ├── models
-    │   ├── index.js
-    │   ├── log.js
-    │   ├── token.js
-    │   └── user.js
-    └── utils
-        ├── helpers
-        │   ├── error-helper.js
-        │   ├── generate-random-code.js
-        │   ├── ip-helper.js
-        │   ├── jwt-token-helper.js
-        │   └── local-text-helper.js
-        ├── index.js
-        ├── lang
-        │   ├── en.json
-        │   ├── get-text.json
-        │   └── tr.json
-        ├── logger.js
-        └── send-code-to-email.js
-
-17 directories, 46 files
-```
-</details>
+- Python
+- Flask 
+- Node.Js
+- Data_Science
 
 ## Version
 
-    0.3.0
+    0.3.1
 
 ## Contributing
 Please refer to [Here](CONTRIBUTING.md) for contributing.
 Any help that can contribute to the templates will be really appreciated.
 
 * Big Thanks to [Link-](https://github.com/Link-) for jump starting the project.
 * Thanks for [Narayandas Akhil Achary](https://github.com/0018akhil) for various fixes & features.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `Artec-0.3.0/artec/__init__.py` & `artec-0.3.1/artec/__init__.py`

 * *Files identical despite different names*

### Comparing `Artec-0.3.0/artec/__main__.py` & `artec-0.3.1/artec/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from . import argparser as parser
 from . import boiler
 from . import logging, console_handler
+from .temp import * 
 
 __app_name__ = "Artec"
-__version__ = "0.3.0"
+__version__ = "0.3.1"
 __desc__ = "Creates a configurable python project \
     template in a given directory."
 
 ERROR_LOGING = {
     0: logging.FATAL,
     1: logging.ERROR,
     2: logging.WARN,
@@ -15,17 +16,17 @@
 }
 
 
 def main():
     args = parser.main_args(__version__)
 
     console_handler.setLevel(ERROR_LOGING[args.verbose])
-
     builder = boiler.boiler_builder(
         args.source, args.target, args.template, args.git
     )
 
     builder.build()
 
 
 if __name__ == "__main__":
     main()
+
```

### Comparing `Artec-0.3.0/artec/argparser.py` & `artec-0.3.1/artec/argparser.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,26 +3,23 @@
 """
 from argparse import (
     ArgumentParser,
     Namespace,
     RawTextHelpFormatter,
     _VersionAction,
 )
-from .templates import templates
+from .temp import *
 import sys
 
 
 class list_templates(_VersionAction):
     def __call__(self, parser: ArgumentParser, *args, **kwargs) -> None:
         formatter = parser._get_formatter()
         formatter.add_text(
-            "".join(
-                "Available templates\n\n",
-                "\n".join([f"> {key.title()}\t" for key in templates.keys()]),
-            )
+            list_available_templates()
         )
         parser._print_message(formatter.format_help(), sys.stdout)
         parser.exit()
 
 
 class Parser(ArgumentParser):
     def __init__(self, appVersion):
@@ -39,14 +36,15 @@
             description,
             epilog,
             formatter_class=RawTextHelpFormatter,
         )
 
     def setup(self):
         group = self.add_mutually_exclusive_group()
+        
         group.add_argument(
             "-s",
             "--source-file",
             dest="source",
             help="Source JSON file containing structure to be created",
             type=str,
             required=False,
@@ -56,21 +54,29 @@
             "-t",
             "--template",
             dest="template",
             help="Uses ready-made templates.",
             required=False,
         )
 
+
         self.add_argument(
             "-o",
             "--output-directory",
             dest="target",
             help="Target output path where the structure will be created",
             type=str,
-            required=True,
+        )
+
+        self.add_argument(
+            "-i",
+            "--interactuve",
+            dest="interactive",
+            help="Runs artec in interactive mode.",
+            action="store_true",
         )
 
         self.add_argument(
             "-ls",
             "--list-template",
             help="lists all ready-made templates.",
             action=list_templates,
@@ -103,12 +109,20 @@
             version=f"{self.prog} {self.appVersion}",
         )
 
 
 def main_args(appVersion) -> Namespace:
     parser = Parser(appVersion)
     parser.setup()
-    return parser.parse_args()
+    args = parser.parse_args()
+
+    if args.interactive:
+        print("Running Artec in interactive mode ....")  
+    else:
+        if not args.target:
+            parser.error("The '-o' argument is required when not in interactive mode.")
+
+    return args
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `Artec-0.3.0/artec/boiler.py` & `artec-0.3.1/artec/boiler.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 	Main module core.
 	#3 Step
 """
 import json
 import os
 from pathlib import Path
 from . import exceptions as ex
-from . import templates as temps
+from .temp import *
 from . import repo 
 from . import logger 
 
+
 class boiler_builder:
     def __init__(
         self,
         source: str = None,
         target: str = None,
         template: str = None,
         git=False,
@@ -25,69 +26,66 @@
         if template is None:
             self.structure = self._source(source)
         else:
             self.structure = self._source_temp(template.lower())
 
     def _source_temp(self, template) -> list[dict[str, str]]:
         try:
-            if template in temps.templates:
-                structure = temps.templates[template].format(self.target)
+            if template in templates:
+                structure = format_project_structure(templates[template], self.target)
+
             else:
                 raise ex.InValidTemplate()
 
         except ex.InValidTemplate:
-            structure = temps.templates["python"].format(self.target)
+            structure = format_project_structure(templates["python"], self.target)
         return structure
 
     def _source(self, source) -> list[dict[str, str]]:
         try:
             if source is None:
                 raise ex.NoSource()
             if os.path.isfile(source) and source.endswith(".json"):
                 with open(source, "rt", encoding="utf-8") as file_data:
-                    structure = temps.static_list(json.load(file_data)).format(
+                    structure = format_project_structure(json.load(file_data),
                         self.target
                     )
             else:
                 raise ex.NotJsonFile()
 
         except Exception:
-            structure = temps.templates["python"].format(self.target)
+            structure = format_project_structure(templates["python"], self.target)
 
         return structure
 
     def build(self):
         print("> Creating folder structure: {}\n".format(self.target))
 
-        for entry in self.structure:
-            for _type, name in entry.items():
-                try:
-                    joined = Path(os.path.join(self.target, name))
-                    if "folder" in _type:
-                        self._make_folder(joined)
-                    elif "file" in _type:
-                        self._make_file(joined)
-                    else:
-                        raise ex.NotValidJson()
-                    print("Created: %s" % joined)
-                except Exception:
-                    pass
+        for folder in self.structure['folders']:
+            folder_path = os.path.join(self.target, folder)
+            self._make_folder(folder_path)
+            print("Created: {}".format(folder_path))
+
+        for file_path in self.structure['files']:
+            file_path = os.path.join(self.target, file_path)
+            self._make_file(file_path)
+            print("Created: {}".format(file_path))
+
         print()
 
         if self.git:
             try:
                 Repo = repo.repository(os.path.join(self.home_dir, self.target), self.target)
                 Repo.add()
                     
             except Exception as e :
                 ex.GitError(e)
 
     def _make_file(self, path):
         """Create an empty file in a given directory"""
-        path.parent.mkdir(parents=True, exist_ok=True)
         open(path, "a").close()
 
     def _make_folder(self, path):
         """Create an empty directory"""
         os.makedirs(path, exist_ok=True)
```

### Comparing `Artec-0.3.0/artec/exceptions.py` & `artec-0.3.1/artec/exceptions.py`

 * *Files identical despite different names*

### Comparing `Artec-0.3.0/artec/repo.py` & `artec-0.3.1/artec/repo.py`

 * *Files identical despite different names*

### Comparing `Artec-0.3.0/artec/templates.py` & `artec-0.3.1/artec/templates.py`

 * *Files identical despite different names*

### Comparing `Artec-0.3.0/pyproject.toml` & `artec-0.3.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 [tool.setuptools.packages.find]
 include = ["artec*"]
 exclude = ["img*"]
 
 [project]
 name = "Artec"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
   { name="HushmKun", email="HushmKun@outlook.com" },
   { name="Link-", email="bsm.dgdy@gmail.com" },
 ]
 description = "Creates a configurable python project template in a given directory."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `Artec-0.3.0/test/test_boiler.py` & `artec-0.3.1/test/test_boiler.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import unittest
 import json
 import git
 from pathlib import Path
 from artec.boiler import boiler_builder
-from artec.templates import static_list, templates
+
+from artec.temp import *
 
 VAILD_JSON = Path("./test/resources/structure.json")
 INVAILD_JSON = Path("./test/resources/structure.txt")
 
 
 class TestBoilerBuilder(unittest.TestCase):
     def test_init(self):
         builder = boiler_builder(
             source="structure.json", target="target"
         )
         self.assertEqual(builder.target, "target")
-        self.assertIsInstance(builder.structure, list)
+        self.assertIsInstance(builder.structure, dict)
 
     def test_source_temp(self):
         builder = boiler_builder(
             template="python", target="target"
         )
         self.assertEqual(
-            builder.structure, templates["python"].format("target")
+            builder.structure, format_project_structure(templates["python"], "target")
         )
 
     def test_source(self):
         with open(VAILD_JSON, "rt", encoding="utf-8") as file_data:
-            structure = static_list(json.load(file_data)).format("target")
+            structure = format_project_structure(json.load(file_data),"target")
         builder = boiler_builder(
             source=VAILD_JSON, target="target"
         )
         self.assertEqual(builder.structure, structure)
 
     def test_build(self):
         builder = boiler_builder(
@@ -52,26 +53,26 @@
 
 
     def test_exception_handling(self):
         builder = boiler_builder(
             source=INVAILD_JSON, target="target"
         )
         self.assertEqual(
-            builder.structure, templates["python"].format("target")
+            builder.structure, format_project_structure(templates["python"],"target")
         )
 
         builder = boiler_builder(
             template="invalid", target="target"
         )
         self.assertEqual(
-            builder.structure, templates["python"].format("target")
+            builder.structure, format_project_structure(templates["python"],"target")
         )
 
         builder = boiler_builder(target="target")
         self.assertEqual(
-            builder.structure, templates["python"].format("target")
+            builder.structure, format_project_structure(templates["python"],"target")
         )
 
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `Artec-0.3.0/test/test_exceptions.py` & `artec-0.3.1/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `Artec-0.3.0/test/test_parser.py` & `artec-0.3.1/test/test_parser.py`

 * *Files identical despite different names*

