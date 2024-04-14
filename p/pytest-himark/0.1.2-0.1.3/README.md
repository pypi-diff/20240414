# Comparing `tmp/pytest-himark-0.1.2.tar.gz` & `tmp/pytest_himark-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-himark-0.1.2.tar", last modified: Sun Apr  7 21:16:07 2024, max compression
+gzip compressed data, was "pytest_himark-0.1.3.tar", last modified: Sun Apr 14 08:19:54 2024, max compression
```

## Comparing `pytest-himark-0.1.2.tar` & `pytest_himark-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 21:16:07.767127 pytest-himark-0.1.2/
--rw-rw-rw-   0        0        0     1111 2024-04-07 10:46:35.000000 pytest-himark-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     5852 2024-04-07 21:16:07.766122 pytest-himark-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3158 2024-04-07 21:14:15.000000 pytest-himark-0.1.2/README.rst
--rw-rw-rw-   0        0        0     1579 2024-04-07 21:10:16.000000 pytest-himark-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-07 21:16:07.767127 pytest-himark-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-07 21:16:07.753383 pytest-himark-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-07 21:16:07.759477 pytest-himark-0.1.2/src/pytest_himark/
--rw-rw-rw-   0        0        0        0 2024-04-07 10:46:35.000000 pytest-himark-0.1.2/src/pytest_himark/__init__.py
--rw-rw-rw-   0        0        0     1747 2024-04-07 21:08:47.000000 pytest-himark-0.1.2/src/pytest_himark/plugin.py
-drwxrwxrwx   0        0        0        0 2024-04-07 21:16:07.766122 pytest-himark-0.1.2/src/pytest_himark.egg-info/
--rw-rw-rw-   0        0        0     5852 2024-04-07 21:16:07.000000 pytest-himark-0.1.2/src/pytest_himark.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2024-04-07 21:16:07.000000 pytest-himark-0.1.2/src/pytest_himark.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 21:16:07.000000 pytest-himark-0.1.2/src/pytest_himark.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-04-07 21:16:07.000000 pytest-himark-0.1.2/src/pytest_himark.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-04-07 21:16:07.000000 pytest-himark-0.1.2/src/pytest_himark.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-07 21:16:07.000000 pytest-himark-0.1.2/src/pytest_himark.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-07 21:16:07.765121 pytest-himark-0.1.2/tests/
--rw-rw-rw-   0        0        0     5074 2024-04-07 21:08:47.000000 pytest-himark-0.1.2/tests/test_himark.py
+drwxrwxrwx   0        0        0        0 2024-04-14 08:19:54.229738 pytest_himark-0.1.3/
+-rw-rw-rw-   0        0        0     1111 2024-04-07 10:46:35.000000 pytest_himark-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     5990 2024-04-14 08:19:54.229738 pytest_himark-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3233 2024-04-14 08:04:14.000000 pytest_himark-0.1.3/README.rst
+-rw-rw-rw-   0        0        0     1642 2024-04-14 08:13:12.000000 pytest_himark-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-14 08:19:54.229738 pytest_himark-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-14 08:19:54.206738 pytest_himark-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-14 08:19:54.213737 pytest_himark-0.1.3/src/pytest_himark/
+-rw-rw-rw-   0        0        0        0 2024-04-07 10:46:35.000000 pytest_himark-0.1.3/src/pytest_himark/__init__.py
+-rw-rw-rw-   0        0        0     1747 2024-04-07 21:08:47.000000 pytest_himark-0.1.3/src/pytest_himark/plugin.py
+drwxrwxrwx   0        0        0        0 2024-04-14 08:19:54.228736 pytest_himark-0.1.3/src/pytest_himark.egg-info/
+-rw-rw-rw-   0        0        0     5990 2024-04-14 08:19:54.000000 pytest_himark-0.1.3/src/pytest_himark.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2024-04-14 08:19:54.000000 pytest_himark-0.1.3/src/pytest_himark.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 08:19:54.000000 pytest_himark-0.1.3/src/pytest_himark.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-04-14 08:19:54.000000 pytest_himark-0.1.3/src/pytest_himark.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-04-14 08:19:54.000000 pytest_himark-0.1.3/src/pytest_himark.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-14 08:19:54.000000 pytest_himark-0.1.3/src/pytest_himark.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-14 08:19:54.227736 pytest_himark-0.1.3/tests/
+-rw-rw-rw-   0        0        0     5074 2024-04-07 21:08:47.000000 pytest_himark-0.1.3/tests/test_himark.py
```

### Comparing `pytest-himark-0.1.2/LICENSE` & `pytest_himark-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-himark-0.1.2/PKG-INFO` & `pytest_himark-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pytest-himark
-Version: 0.1.2
-Summary: A plugin that reads a config.json file in your test root directory, searches the 'markers' key, lists the markers declared as 'true' as enabled markers and automatically adds -m option to the command line with an OR on the enabled markers.
+Version: 0.1.3
+Summary: A plugin that will filter pytest's test collection using a json file. It will read a json file provided with a --json argument in pytest command line (or in pytest.ini), search the markers key and automatically add -m option to the command line for filtering out the tests marked with disabled markers.
 Author-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
 Maintainer-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
 License: 
         The MIT License (MIT)
         
         Copyright (c) 2024 Rodolphe Mete Soyding
         
@@ -60,15 +60,18 @@
     :target: https://pypi.org/project/pytest-himark
     :alt: Python versions
 
 .. image:: https://github.com/supermete/pytest-himark/actions/workflows/main.yml/badge.svg
     :target: https://github.com/supermete/pytest-himark/actions/workflows/main.yml
     :alt: See Build Status on GitHub Actions
 
-A plugin that reads a json file in your test root directory, searches the 'markers' key, lists the markers declared as 'true' as enabled markers and automatically adds -m option to the command line with an OR on the enabled markers.
+A plugin that will filter pytest's test collection using a json file.
+It will read a json file provided with a --json argument in pytest command line
+(or in pytest.ini), search the 'markers' key and automatically add -m option to
+the command line for filtering out the tests marked with disabled markers.
 
 ----
 
 This `pytest`_ plugin was generated with `Cookiecutter`_ along with `@hackebrot`_'s `cookiecutter-pytest-plugin`_ template.
 
 
 Requirements
```

### Comparing `pytest-himark-0.1.2/README.rst` & `pytest_himark-0.1.3/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,18 @@
     :target: https://pypi.org/project/pytest-himark
     :alt: Python versions
 
 .. image:: https://github.com/supermete/pytest-himark/actions/workflows/main.yml/badge.svg
     :target: https://github.com/supermete/pytest-himark/actions/workflows/main.yml
     :alt: See Build Status on GitHub Actions
 
-A plugin that reads a json file in your test root directory, searches the 'markers' key, lists the markers declared as 'true' as enabled markers and automatically adds -m option to the command line with an OR on the enabled markers.
+A plugin that will filter pytest's test collection using a json file.
+It will read a json file provided with a --json argument in pytest command line
+(or in pytest.ini), search the 'markers' key and automatically add -m option to
+the command line for filtering out the tests marked with disabled markers.
 
 ----
 
 This `pytest`_ plugin was generated with `Cookiecutter`_ along with `@hackebrot`_'s `cookiecutter-pytest-plugin`_ template.
 
 
 Requirements
```

### Comparing `pytest-himark-0.1.2/pyproject.toml` & `pytest_himark-0.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 requires = [
   "setuptools>=61.0.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytest-himark"
-description = "A plugin that reads a config.json file in your test root directory, searches the 'markers' key, lists the markers declared as 'true' as enabled markers and automatically adds -m option to the command line with an OR on the enabled markers."
-version = "0.1.2"
+description = "A plugin that will filter pytest's test collection using a json file. It will read a json file provided with a --json argument in pytest command line (or in pytest.ini), search the markers key and automatically add -m option to the command line for filtering out the tests marked with disabled markers."
+version = "0.1.3"
 readme = "README.rst"
 requires-python = ">=3.8"
 authors = [
     { name = "Rodolphe Mete Soyding", email = "r.soyding@gmail.com" },
 ]
 maintainers = [
     { name = "Rodolphe Mete Soyding", email = "r.soyding@gmail.com" },
```

### Comparing `pytest-himark-0.1.2/src/pytest_himark/plugin.py` & `pytest_himark-0.1.3/src/pytest_himark/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-himark-0.1.2/src/pytest_himark.egg-info/PKG-INFO` & `pytest_himark-0.1.3/src/pytest_himark.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pytest-himark
-Version: 0.1.2
-Summary: A plugin that reads a config.json file in your test root directory, searches the 'markers' key, lists the markers declared as 'true' as enabled markers and automatically adds -m option to the command line with an OR on the enabled markers.
+Version: 0.1.3
+Summary: A plugin that will filter pytest's test collection using a json file. It will read a json file provided with a --json argument in pytest command line (or in pytest.ini), search the markers key and automatically add -m option to the command line for filtering out the tests marked with disabled markers.
 Author-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
 Maintainer-email: Rodolphe Mete Soyding <r.soyding@gmail.com>
 License: 
         The MIT License (MIT)
         
         Copyright (c) 2024 Rodolphe Mete Soyding
         
@@ -60,15 +60,18 @@
     :target: https://pypi.org/project/pytest-himark
     :alt: Python versions
 
 .. image:: https://github.com/supermete/pytest-himark/actions/workflows/main.yml/badge.svg
     :target: https://github.com/supermete/pytest-himark/actions/workflows/main.yml
     :alt: See Build Status on GitHub Actions
 
-A plugin that reads a json file in your test root directory, searches the 'markers' key, lists the markers declared as 'true' as enabled markers and automatically adds -m option to the command line with an OR on the enabled markers.
+A plugin that will filter pytest's test collection using a json file.
+It will read a json file provided with a --json argument in pytest command line
+(or in pytest.ini), search the 'markers' key and automatically add -m option to
+the command line for filtering out the tests marked with disabled markers.
 
 ----
 
 This `pytest`_ plugin was generated with `Cookiecutter`_ along with `@hackebrot`_'s `cookiecutter-pytest-plugin`_ template.
 
 
 Requirements
```

### Comparing `pytest-himark-0.1.2/tests/test_himark.py` & `pytest_himark-0.1.3/tests/test_himark.py`

 * *Files identical despite different names*

