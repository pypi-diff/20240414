# Comparing `tmp/Flask-Docs-0.7.5.tar.gz` & `tmp/flask_docs-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Docs-0.7.5.tar", last modified: Fri Feb 23 09:49:16 2024, max compression
+gzip compressed data, was "flask_docs-0.7.6.tar", last modified: Sun Apr 14 07:07:47 2024, max compression
```

## Comparing `Flask-Docs-0.7.5.tar` & `flask_docs-0.7.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:49:16.008695 Flask-Docs-0.7.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:49:16.008695 Flask-Docs-0.7.5/Flask_Docs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9071 2024-02-23 09:49:15.000000 Flask-Docs-0.7.5/Flask_Docs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-02-23 09:49:15.000000 Flask-Docs-0.7.5/Flask_Docs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 09:49:15.000000 Flask-Docs-0.7.5/Flask_Docs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 09:49:15.000000 Flask-Docs-0.7.5/Flask_Docs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-23 09:49:15.000000 Flask-Docs-0.7.5/Flask_Docs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-23 09:49:15.000000 Flask-Docs-0.7.5/Flask_Docs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9071 2024-02-23 09:49:16.008695 Flask-Docs-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:49:16.000695 Flask-Docs-0.7.5/flask_docs/
--rw-r--r--   0 runner    (1001) docker     (127)    22910 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:49:16.000695 Flask-Docs-0.7.5/flask_docs/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    23712 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/assets/debugger.png
--rw-r--r--   0 runner    (1001) docker     (127)    34650 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/assets/sample_app_add.png
--rw-r--r--   0 runner    (1001) docker     (127)    35046 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/assets/sample_app_delete.png
--rw-r--r--   0 runner    (1001) docker     (127)    31682 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/assets/sample_app_get.png
--rw-r--r--   0 runner    (1001) docker     (127)    31719 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/assets/sample_app_restful_get.png
--rw-r--r--   0 runner    (1001) docker     (127)    31881 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/assets/sample_app_restful_post.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:49:15.996694 Flask-Docs-0.7.5/flask_docs/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:49:16.000695 Flask-Docs-0.7.5/flask_docs/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)   238602 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/static/css/element-ui-2.15.6.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:49:16.000695 Flask-Docs-0.7.5/flask_docs/static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    55956 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/static/css/fonts/element-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    28200 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/static/css/fonts/element-icons.woff
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/static/css/github-11.2.0.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    14182 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/static/css/github-markdown-1.0.0.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:49:16.000695 Flask-Docs-0.7.5/flask_docs/static/icon/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/static/icon/book.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:49:16.004695 Flask-Docs-0.7.5/flask_docs/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/static/js/FileSaver-2.0.5.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    17816 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/static/js/axios-0.22.0.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    48316 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/static/js/crypto-js-4.1.1.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   580859 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/static/js/element-ui-2.15.6.min.js
--rw-r--r--   0 runner    (1001) docker     (127)   109006 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/static/js/highlight-11.2.0.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    46590 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/static/js/marked-3.0.7.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    94151 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/static/js/vue-2.6.14.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    27424 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/static/js/vue-i18n-8.26.5.min.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:49:16.004695 Flask-Docs-0.7.5/flask_docs/static/locale/
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/static/locale/zh.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:49:16.004695 Flask-Docs-0.7.5/flask_docs/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/templates/css_template_cdn.html
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/templates/css_template_local.html
--rw-r--r--   0 runner    (1001) docker     (127)    38913 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/templates/js_template_cdn.html
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/templates/js_template_local.html
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/flask_docs/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 09:49:16.008695 Flask-Docs-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 09:49:16.008695 Flask-Docs-0.7.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8025 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/tests/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/tests/test_case_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/tests/test_case_config_fail.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-02-23 09:48:53.000000 Flask-Docs-0.7.5/tests/test_case_disable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:47.750582 flask_docs-0.7.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:47.750582 flask_docs-0.7.6/Flask_Docs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-14 07:07:47.000000 flask_docs-0.7.6/Flask_Docs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-04-14 07:07:47.000000 flask_docs-0.7.6/Flask_Docs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 07:07:47.000000 flask_docs-0.7.6/Flask_Docs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 07:07:47.000000 flask_docs-0.7.6/Flask_Docs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 07:07:47.000000 flask_docs-0.7.6/Flask_Docs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-14 07:07:47.000000 flask_docs-0.7.6/Flask_Docs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-14 07:07:28.000000 flask_docs-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-14 07:07:28.000000 flask_docs-0.7.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-14 07:07:47.750582 flask_docs-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-04-14 07:07:28.000000 flask_docs-0.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:47.742581 flask_docs-0.7.6/flask_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    22910 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:47.746582 flask_docs-0.7.6/flask_docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    23712 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/assets/debugger.png
+-rw-r--r--   0 runner    (1001) docker     (127)    34650 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/assets/sample_app_add.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35046 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/assets/sample_app_delete.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31682 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/assets/sample_app_get.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31719 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/assets/sample_app_restful_get.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31881 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/assets/sample_app_restful_post.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:47.742581 flask_docs-0.7.6/flask_docs/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:47.746582 flask_docs-0.7.6/flask_docs/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   238602 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/static/css/element-ui-2.15.6.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:47.746582 flask_docs-0.7.6/flask_docs/static/css/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    55956 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/static/css/fonts/element-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    28200 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/static/css/fonts/element-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/static/css/github-11.2.0.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    14182 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/static/css/github-markdown-1.0.0.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:47.746582 flask_docs-0.7.6/flask_docs/static/icon/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/static/icon/book.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:47.750582 flask_docs-0.7.6/flask_docs/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/static/js/FileSaver-2.0.5.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17816 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/static/js/axios-0.22.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    48316 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/static/js/crypto-js-4.1.1.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   580859 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/static/js/element-ui-2.15.6.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   109006 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/static/js/highlight-11.2.0.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    46590 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/static/js/marked-3.0.7.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    94151 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/static/js/vue-2.6.14.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    27424 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/static/js/vue-i18n-8.26.5.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:47.750582 flask_docs-0.7.6/flask_docs/static/locale/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/static/locale/zh.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:47.750582 flask_docs-0.7.6/flask_docs/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/templates/css_template_cdn.html
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/templates/css_template_local.html
+-rw-r--r--   0 runner    (1001) docker     (127)    38913 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/templates/js_template_cdn.html
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/templates/js_template_local.html
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-14 07:07:28.000000 flask_docs-0.7.6/flask_docs/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 07:07:47.750582 flask_docs-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-14 07:07:28.000000 flask_docs-0.7.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 07:07:47.750582 flask_docs-0.7.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8025 2024-04-14 07:07:28.000000 flask_docs-0.7.6/tests/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-04-14 07:07:28.000000 flask_docs-0.7.6/tests/test_case_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-14 07:07:28.000000 flask_docs-0.7.6/tests/test_case_config_fail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-14 07:07:28.000000 flask_docs-0.7.6/tests/test_case_disable.py
```

### Comparing `Flask-Docs-0.7.5/Flask_Docs.egg-info/PKG-INFO` & `flask_docs-0.7.6/Flask_Docs.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Docs
-Version: 0.7.5
+Version: 0.7.6
 Summary: Adds Docs support to Flask.
 Home-page: https://github.com/kwkwc/flask-docs
 Author: kwkw
 Author-email: 
 License: MIT
 Keywords: flask,api,apidoc,doc,docs,documentation,md,markdown,RESTful,auto
 Platform: any
@@ -18,21 +18,22 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Flask
 
 # Flask-Docs
 
-[![build](https://github.com/kwkwc/flask-docs/actions/workflows/python-build.yml/badge.svg)](https://github.com/kwkwc/flask-docs/actions/workflows/python-build.yml)
-[![test](https://github.com/kwkwc/flask-docs/actions/workflows/python-test.yml/badge.svg)](https://github.com/kwkwc/flask-docs/actions/workflows/python-test.yml)
+[![test](https://github.com/kwkwc/flask-docs/actions/workflows/test.yml/badge.svg)](https://github.com/kwkwc/flask-docs/actions/workflows/test.yml)
+[![publish](https://github.com/kwkwc/flask-docs/actions/workflows/publish.yml/badge.svg)](https://github.com/kwkwc/flask-docs/actions/workflows/publish.yml)
 [![codecov](https://codecov.io/gh/kwkwc/flask-docs/branch/master/graph/badge.svg?token=EV69K9WPJ0)](https://codecov.io/gh/kwkwc/flask-docs)
-[![license](https://img.shields.io/github/license/kwkwc/flask-docs)](https://github.com/kwkwc/flask-docs/blob/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/Flask-Docs)](https://pypi.org/project/Flask-Docs/)
 [![Python](https://img.shields.io/pypi/pyversions/flask-docs)](https://pypi.org/project/Flask-Docs/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+![GitHub release (with filter)](https://img.shields.io/github/v/release/kwkwc/flask-docs)
+[![license](https://img.shields.io/github/license/kwkwc/flask-docs)](https://github.com/kwkwc/flask-docs/blob/master/LICENSE)
 
 > Adds Docs support to Flask.
 
 English | [简体中文](README.zh-CN.md)
 
 ## Features
```

### Comparing `Flask-Docs-0.7.5/Flask_Docs.egg-info/SOURCES.txt` & `flask_docs-0.7.6/Flask_Docs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/LICENSE` & `flask_docs-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/PKG-INFO` & `flask_docs-0.7.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Docs
-Version: 0.7.5
+Version: 0.7.6
 Summary: Adds Docs support to Flask.
 Home-page: https://github.com/kwkwc/flask-docs
 Author: kwkw
 Author-email: 
 License: MIT
 Keywords: flask,api,apidoc,doc,docs,documentation,md,markdown,RESTful,auto
 Platform: any
@@ -18,21 +18,22 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Flask
 
 # Flask-Docs
 
-[![build](https://github.com/kwkwc/flask-docs/actions/workflows/python-build.yml/badge.svg)](https://github.com/kwkwc/flask-docs/actions/workflows/python-build.yml)
-[![test](https://github.com/kwkwc/flask-docs/actions/workflows/python-test.yml/badge.svg)](https://github.com/kwkwc/flask-docs/actions/workflows/python-test.yml)
+[![test](https://github.com/kwkwc/flask-docs/actions/workflows/test.yml/badge.svg)](https://github.com/kwkwc/flask-docs/actions/workflows/test.yml)
+[![publish](https://github.com/kwkwc/flask-docs/actions/workflows/publish.yml/badge.svg)](https://github.com/kwkwc/flask-docs/actions/workflows/publish.yml)
 [![codecov](https://codecov.io/gh/kwkwc/flask-docs/branch/master/graph/badge.svg?token=EV69K9WPJ0)](https://codecov.io/gh/kwkwc/flask-docs)
-[![license](https://img.shields.io/github/license/kwkwc/flask-docs)](https://github.com/kwkwc/flask-docs/blob/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/Flask-Docs)](https://pypi.org/project/Flask-Docs/)
 [![Python](https://img.shields.io/pypi/pyversions/flask-docs)](https://pypi.org/project/Flask-Docs/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+![GitHub release (with filter)](https://img.shields.io/github/v/release/kwkwc/flask-docs)
+[![license](https://img.shields.io/github/license/kwkwc/flask-docs)](https://github.com/kwkwc/flask-docs/blob/master/LICENSE)
 
 > Adds Docs support to Flask.
 
 English | [简体中文](README.zh-CN.md)
 
 ## Features
```

### Comparing `Flask-Docs-0.7.5/README.md` & `flask_docs-0.7.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Flask-Docs
 
-[![build](https://github.com/kwkwc/flask-docs/actions/workflows/python-build.yml/badge.svg)](https://github.com/kwkwc/flask-docs/actions/workflows/python-build.yml)
-[![test](https://github.com/kwkwc/flask-docs/actions/workflows/python-test.yml/badge.svg)](https://github.com/kwkwc/flask-docs/actions/workflows/python-test.yml)
+[![test](https://github.com/kwkwc/flask-docs/actions/workflows/test.yml/badge.svg)](https://github.com/kwkwc/flask-docs/actions/workflows/test.yml)
+[![publish](https://github.com/kwkwc/flask-docs/actions/workflows/publish.yml/badge.svg)](https://github.com/kwkwc/flask-docs/actions/workflows/publish.yml)
 [![codecov](https://codecov.io/gh/kwkwc/flask-docs/branch/master/graph/badge.svg?token=EV69K9WPJ0)](https://codecov.io/gh/kwkwc/flask-docs)
-[![license](https://img.shields.io/github/license/kwkwc/flask-docs)](https://github.com/kwkwc/flask-docs/blob/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/Flask-Docs)](https://pypi.org/project/Flask-Docs/)
 [![Python](https://img.shields.io/pypi/pyversions/flask-docs)](https://pypi.org/project/Flask-Docs/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+![GitHub release (with filter)](https://img.shields.io/github/v/release/kwkwc/flask-docs)
+[![license](https://img.shields.io/github/license/kwkwc/flask-docs)](https://github.com/kwkwc/flask-docs/blob/master/LICENSE)
 
 > Adds Docs support to Flask.
 
 English | [简体中文](README.zh-CN.md)
 
 ## Features
```

### Comparing `Flask-Docs-0.7.5/flask_docs/__init__.py` & `flask_docs-0.7.6/flask_docs/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/flask_docs/assets/debugger.png` & `flask_docs-0.7.6/flask_docs/assets/debugger.png`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/flask_docs/assets/sample_app_add.png` & `flask_docs-0.7.6/flask_docs/assets/sample_app_add.png`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/flask_docs/assets/sample_app_delete.png` & `flask_docs-0.7.6/flask_docs/assets/sample_app_delete.png`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/flask_docs/assets/sample_app_get.png` & `flask_docs-0.7.6/flask_docs/assets/sample_app_get.png`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/flask_docs/assets/sample_app_restful_get.png` & `flask_docs-0.7.6/flask_docs/assets/sample_app_restful_get.png`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/flask_docs/assets/sample_app_restful_post.png` & `flask_docs-0.7.6/flask_docs/assets/sample_app_restful_post.png`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/flask_docs/static/css/element-ui-2.15.6.min.css` & `flask_docs-0.7.6/flask_docs/static/css/element-ui-2.15.6.min.css`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/flask_docs/static/css/fonts/element-icons.ttf` & `flask_docs-0.7.6/flask_docs/static/css/fonts/element-icons.ttf`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/flask_docs/static/css/fonts/element-icons.woff` & `flask_docs-0.7.6/flask_docs/static/css/fonts/element-icons.woff`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/flask_docs/static/css/github-11.2.0.min.css` & `flask_docs-0.7.6/flask_docs/static/css/github-11.2.0.min.css`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/flask_docs/static/css/github-markdown-1.0.0.min.css` & `flask_docs-0.7.6/flask_docs/static/css/github-markdown-1.0.0.min.css`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/flask_docs/static/js/FileSaver-2.0.5.min.js` & `flask_docs-0.7.6/flask_docs/static/js/FileSaver-2.0.5.min.js`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/flask_docs/static/js/axios-0.22.0.min.js` & `flask_docs-0.7.6/flask_docs/static/js/axios-0.22.0.min.js`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/flask_docs/static/js/crypto-js-4.1.1.min.js` & `flask_docs-0.7.6/flask_docs/static/js/crypto-js-4.1.1.min.js`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/flask_docs/static/js/element-ui-2.15.6.min.js` & `flask_docs-0.7.6/flask_docs/static/js/element-ui-2.15.6.min.js`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/flask_docs/static/js/highlight-11.2.0.min.js` & `flask_docs-0.7.6/flask_docs/static/js/highlight-11.2.0.min.js`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/flask_docs/static/js/marked-3.0.7.min.js` & `flask_docs-0.7.6/flask_docs/static/js/marked-3.0.7.min.js`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/flask_docs/static/js/vue-2.6.14.min.js` & `flask_docs-0.7.6/flask_docs/static/js/vue-2.6.14.min.js`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/flask_docs/static/js/vue-i18n-8.26.5.min.js` & `flask_docs-0.7.6/flask_docs/static/js/vue-i18n-8.26.5.min.js`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/flask_docs/static/locale/zh.js` & `flask_docs-0.7.6/flask_docs/static/locale/zh.js`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/flask_docs/templates/index.html` & `flask_docs-0.7.6/flask_docs/templates/index.html`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/flask_docs/templates/js_template_cdn.html` & `flask_docs-0.7.6/flask_docs/templates/js_template_cdn.html`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/setup.py` & `flask_docs-0.7.6/setup.py`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/tests/test_case.py` & `flask_docs-0.7.6/tests/test_case.py`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/tests/test_case_config.py` & `flask_docs-0.7.6/tests/test_case_config.py`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/tests/test_case_config_fail.py` & `flask_docs-0.7.6/tests/test_case_config_fail.py`

 * *Files identical despite different names*

### Comparing `Flask-Docs-0.7.5/tests/test_case_disable.py` & `flask_docs-0.7.6/tests/test_case_disable.py`

 * *Files identical despite different names*

