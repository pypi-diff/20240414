# Comparing `tmp/tendril-config-0.3.5.tar.gz` & `tmp/tendril-config-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tendril-config-0.3.5.tar", last modified: Sun Sep 17 09:12:29 2023, max compression
+gzip compressed data, was "tendril-config-0.3.6.tar", last modified: Sun Apr 14 10:52:08 2024, max compression
```

## Comparing `tendril-config-0.3.5.tar` & `tendril-config-0.3.6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-17 09:12:29.317880 tendril-config-0.3.5/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2020-08-18 06:57:00.000000 tendril-config-0.3.5/.gitignore
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2020-08-18 06:57:00.000000 tendril-config-0.3.5/.readthedocs.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2020-08-18 06:57:00.000000 tendril-config-0.3.5/.travis.yml
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:00.000000 tendril-config-0.3.5/CHANGELOG.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2020-08-18 06:57:00.000000 tendril-config-0.3.5/LICENSE
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2020-08-18 06:57:00.000000 tendril-config-0.3.5/MANIFEST.in
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3455 2023-09-17 09:12:29.317880 tendril-config-0.3.5/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2176 2020-08-18 06:57:00.000000 tendril-config-0.3.5/README.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-17 09:12:29.313880 tendril-config-0.3.5/docs/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2020-08-18 06:57:00.000000 tendril-config-0.3.5/docs/Makefile
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-17 09:12:29.313880 tendril-config-0.3.5/docs/_static/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2020-08-18 06:57:00.000000 tendril-config-0.3.5/docs/_static/custom.css
--rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2020-08-18 06:57:00.000000 tendril-config-0.3.5/docs/_static/favicon.ico
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2020-08-18 06:57:00.000000 tendril-config-0.3.5/docs/_static/logo.png
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2020-08-18 06:57:00.000000 tendril-config-0.3.5/docs/_static/logo_packed.png
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-17 09:12:29.313880 tendril-config-0.3.5/docs/_templates/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-08-18 06:57:00.000000 tendril-config-0.3.5/docs/_templates/about.html
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-17 09:12:29.313880 tendril-config-0.3.5/docs/api/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      367 2020-08-18 06:57:00.000000 tendril-config-0.3.5/docs/api/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       94 2020-08-18 06:57:00.000000 tendril-config-0.3.5/docs/api/tendril.config.core.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       97 2020-08-18 06:57:00.000000 tendril-config-0.3.5/docs/api/tendril.config.legacy.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       95 2020-08-18 06:57:00.000000 tendril-config-0.3.5/docs/api/tendril.config.paths.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    13489 2020-08-18 06:57:00.000000 tendril-config-0.3.5/docs/conf.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      865 2020-08-18 06:57:00.000000 tendril-config-0.3.5/docs/index.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1559 2020-08-18 06:57:00.000000 tendril-config-0.3.5/docs/installation.rst
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-17 09:12:29.313880 tendril-config-0.3.5/docs/usage/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2020-08-18 06:57:00.000000 tendril-config-0.3.5/docs/usage/standalone.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2020-08-18 06:57:00.000000 tendril-config-0.3.5/docs/usage/tendril.rst
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2023-09-17 09:12:29.317880 tendril-config-0.3.5/setup.cfg
--rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3252 2022-11-22 10:36:33.000000 tendril-config-0.3.5/setup.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-17 09:12:29.309880 tendril-config-0.3.5/src/
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-17 09:12:29.313880 tendril-config-0.3.5/src/tendril/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:49:28.000000 tendril-config-0.3.5/src/tendril/__init__.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-17 09:12:29.313880 tendril-config-0.3.5/src/tendril/config/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:00.000000 tendril-config-0.3.5/src/tendril/config/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1100 2023-03-16 04:48:21.000000 tendril-config-0.3.5/src/tendril/config/core.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2216 2023-09-06 12:49:59.000000 tendril-config-0.3.5/src/tendril/config/coremeta.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)    17818 2021-03-14 15:58:14.000000 tendril-config-0.3.5/src/tendril/config/legacy.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3541 2023-09-17 06:27:52.000000 tendril-config-0.3.5/src/tendril/config/log.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2101 2021-03-14 15:56:54.000000 tendril-config-0.3.5/src/tendril/config/mail.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     2882 2020-08-18 06:57:00.000000 tendril-config-0.3.5/src/tendril/config/paths.py
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-17 09:12:29.313880 tendril-config-0.3.5/src/tendril_config.egg-info/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     3455 2023-09-17 09:12:29.000000 tendril-config-0.3.5/src/tendril_config.egg-info/PKG-INFO
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      941 2023-09-17 09:12:29.000000 tendril-config-0.3.5/src/tendril_config.egg-info/SOURCES.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2023-09-17 09:12:29.000000 tendril-config-0.3.5/src/tendril_config.egg-info/dependency_links.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      690 2023-09-17 09:12:29.000000 tendril-config-0.3.5/src/tendril_config.egg-info/requires.txt
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2023-09-17 09:12:29.000000 tendril-config-0.3.5/src/tendril_config.egg-info/top_level.txt
-drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2023-09-17 09:12:29.317880 tendril-config-0.3.5/tests/
--rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:00.000000 tendril-config-0.3.5/tests/__init__.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2020-08-18 06:57:00.000000 tendril-config-0.3.5/tests/coveralls.py
--rw-rw-r--   0 chintal   (1000) chintal   (1000)      826 2020-08-18 06:57:00.000000 tendril-config-0.3.5/tox.ini
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 10:52:08.406477 tendril-config-0.3.6/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2122 2020-08-18 06:57:00.000000 tendril-config-0.3.6/.gitignore
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      638 2020-08-18 06:57:00.000000 tendril-config-0.3.6/.readthedocs.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      629 2020-08-18 06:57:00.000000 tendril-config-0.3.6/.travis.yml
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:00.000000 tendril-config-0.3.6/CHANGELOG.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    34520 2020-08-18 06:57:00.000000 tendril-config-0.3.6/LICENSE
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      173 2020-08-18 06:57:00.000000 tendril-config-0.3.6/MANIFEST.in
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3455 2024-04-14 10:52:08.406477 tendril-config-0.3.6/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2176 2020-08-18 06:57:00.000000 tendril-config-0.3.6/README.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 10:52:08.398476 tendril-config-0.3.6/docs/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     7660 2020-08-18 06:57:00.000000 tendril-config-0.3.6/docs/Makefile
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 10:52:08.402477 tendril-config-0.3.6/docs/_static/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2727 2020-08-18 06:57:00.000000 tendril-config-0.3.6/docs/_static/custom.css
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)   128918 2020-08-18 06:57:00.000000 tendril-config-0.3.6/docs/_static/favicon.ico
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    96804 2020-08-18 06:57:00.000000 tendril-config-0.3.6/docs/_static/logo.png
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     9889 2020-08-18 06:57:00.000000 tendril-config-0.3.6/docs/_static/logo_packed.png
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 10:52:08.402477 tendril-config-0.3.6/docs/_templates/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1713 2020-08-18 06:57:00.000000 tendril-config-0.3.6/docs/_templates/about.html
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 10:52:08.402477 tendril-config-0.3.6/docs/api/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      367 2020-08-18 06:57:00.000000 tendril-config-0.3.6/docs/api/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       94 2020-08-18 06:57:00.000000 tendril-config-0.3.6/docs/api/tendril.config.core.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       97 2020-08-18 06:57:00.000000 tendril-config-0.3.6/docs/api/tendril.config.legacy.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       95 2020-08-18 06:57:00.000000 tendril-config-0.3.6/docs/api/tendril.config.paths.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    13489 2020-08-18 06:57:00.000000 tendril-config-0.3.6/docs/conf.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      865 2020-08-18 06:57:00.000000 tendril-config-0.3.6/docs/index.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1559 2020-08-18 06:57:00.000000 tendril-config-0.3.6/docs/installation.rst
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 10:52:08.402477 tendril-config-0.3.6/docs/usage/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       35 2020-08-18 06:57:00.000000 tendril-config-0.3.6/docs/usage/standalone.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       49 2020-08-18 06:57:00.000000 tendril-config-0.3.6/docs/usage/tendril.rst
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      131 2024-04-14 10:52:08.406477 tendril-config-0.3.6/setup.cfg
+-rwxrwxr-x   0 chintal   (1000) chintal   (1000)     3252 2022-11-22 10:36:33.000000 tendril-config-0.3.6/setup.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 10:52:08.398476 tendril-config-0.3.6/src/
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 10:52:08.402477 tendril-config-0.3.6/src/tendril/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)       65 2020-11-29 17:49:28.000000 tendril-config-0.3.6/src/tendril/__init__.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 10:52:08.402477 tendril-config-0.3.6/src/tendril/config/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1112 2020-08-18 06:57:00.000000 tendril-config-0.3.6/src/tendril/config/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1100 2023-03-16 04:48:21.000000 tendril-config-0.3.6/src/tendril/config/core.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2216 2023-09-06 12:49:59.000000 tendril-config-0.3.6/src/tendril/config/coremeta.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)    17818 2021-03-14 15:58:14.000000 tendril-config-0.3.6/src/tendril/config/legacy.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3541 2023-09-17 06:27:52.000000 tendril-config-0.3.6/src/tendril/config/log.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2101 2021-03-14 15:56:54.000000 tendril-config-0.3.6/src/tendril/config/mail.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     2882 2020-08-18 06:57:00.000000 tendril-config-0.3.6/src/tendril/config/paths.py
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 10:52:08.406477 tendril-config-0.3.6/src/tendril_config.egg-info/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     3455 2024-04-14 10:52:08.000000 tendril-config-0.3.6/src/tendril_config.egg-info/PKG-INFO
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      941 2024-04-14 10:52:08.000000 tendril-config-0.3.6/src/tendril_config.egg-info/SOURCES.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        1 2024-04-14 10:52:08.000000 tendril-config-0.3.6/src/tendril_config.egg-info/dependency_links.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      690 2024-04-14 10:52:08.000000 tendril-config-0.3.6/src/tendril_config.egg-info/requires.txt
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        8 2024-04-14 10:52:08.000000 tendril-config-0.3.6/src/tendril_config.egg-info/top_level.txt
+drwxrwxr-x   0 chintal   (1000) chintal   (1000)        0 2024-04-14 10:52:08.406477 tendril-config-0.3.6/tests/
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)        0 2020-08-18 06:57:00.000000 tendril-config-0.3.6/tests/__init__.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)     1060 2020-08-18 06:57:00.000000 tendril-config-0.3.6/tests/coveralls.py
+-rw-rw-r--   0 chintal   (1000) chintal   (1000)      826 2020-08-18 06:57:00.000000 tendril-config-0.3.6/tox.ini
```

### Comparing `tendril-config-0.3.5/.gitignore` & `tendril-config-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/.readthedocs.yml` & `tendril-config-0.3.6/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/.travis.yml` & `tendril-config-0.3.6/.travis.yml`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/LICENSE` & `tendril-config-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/PKG-INFO` & `tendril-config-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-config
-Version: 0.3.5
+Version: 0.3.6
 Summary: Tendril Config Infrastructure
 Home-page: https://github.com/tendril-framework/tendril-config
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-config.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-config/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-config
```

### Comparing `tendril-config-0.3.5/README.rst` & `tendril-config-0.3.6/README.rst`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/docs/Makefile` & `tendril-config-0.3.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/docs/_static/custom.css` & `tendril-config-0.3.6/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/docs/_static/favicon.ico` & `tendril-config-0.3.6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/docs/_static/logo.png` & `tendril-config-0.3.6/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/docs/_static/logo_packed.png` & `tendril-config-0.3.6/docs/_static/logo_packed.png`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/docs/_templates/about.html` & `tendril-config-0.3.6/docs/_templates/about.html`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/docs/conf.py` & `tendril-config-0.3.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/docs/index.rst` & `tendril-config-0.3.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/docs/installation.rst` & `tendril-config-0.3.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/setup.py` & `tendril-config-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/src/tendril/config/__init__.py` & `tendril-config-0.3.6/src/tendril/config/__init__.py`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/src/tendril/config/core.py` & `tendril-config-0.3.6/src/tendril/config/core.py`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/src/tendril/config/coremeta.py` & `tendril-config-0.3.6/src/tendril/config/coremeta.py`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/src/tendril/config/legacy.py` & `tendril-config-0.3.6/src/tendril/config/legacy.py`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/src/tendril/config/log.py` & `tendril-config-0.3.6/src/tendril/config/log.py`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/src/tendril/config/mail.py` & `tendril-config-0.3.6/src/tendril/config/mail.py`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/src/tendril/config/paths.py` & `tendril-config-0.3.6/src/tendril/config/paths.py`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/src/tendril_config.egg-info/PKG-INFO` & `tendril-config-0.3.6/src/tendril_config.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tendril-config
-Version: 0.3.5
+Version: 0.3.6
 Summary: Tendril Config Infrastructure
 Home-page: https://github.com/tendril-framework/tendril-config
 Author: Chintalagiri Shashank
 Author-email: shashank@chintal.in
 Project-URL: Documentation, https://tendril-config.readthedocs.io/en/latest
 Project-URL: Bug Tracker, https://github.com/tendril-framework/tendril-config/issues
 Project-URL: Source Repository, https://github.com/tendril-framework/tendril-config
```

### Comparing `tendril-config-0.3.5/src/tendril_config.egg-info/SOURCES.txt` & `tendril-config-0.3.6/src/tendril_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/src/tendril_config.egg-info/requires.txt` & `tendril-config-0.3.6/src/tendril_config.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/tests/coveralls.py` & `tendril-config-0.3.6/tests/coveralls.py`

 * *Files identical despite different names*

### Comparing `tendril-config-0.3.5/tox.ini` & `tendril-config-0.3.6/tox.ini`

 * *Files identical despite different names*

