# Comparing `tmp/types-uWSGI-2.0.0.20240311.tar.gz` & `tmp/types-uWSGI-2.0.0.20240414.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-uWSGI-2.0.0.20240311.tar", last modified: Mon Mar 11 02:15:35 2024, max compression
+gzip compressed data, was "types-uWSGI-2.0.0.20240414.tar", last modified: Sun Apr 14 03:12:24 2024, max compression
```

## Comparing `types-uWSGI-2.0.0.20240311.tar` & `types-uWSGI-2.0.0.20240414.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:15:35.009679 types-uWSGI-2.0.0.20240311/
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-03-11 02:15:34.000000 types-uWSGI-2.0.0.20240311/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-11 02:15:34.000000 types-uWSGI-2.0.0.20240311/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-11 02:15:35.009679 types-uWSGI-2.0.0.20240311/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 02:15:35.009679 types-uWSGI-2.0.0.20240311/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-03-11 02:15:34.000000 types-uWSGI-2.0.0.20240311/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:15:35.009679 types-uWSGI-2.0.0.20240311/types_uWSGI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-11 02:15:34.000000 types-uWSGI-2.0.0.20240311/types_uWSGI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-11 02:15:34.000000 types-uWSGI-2.0.0.20240311/types_uWSGI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 02:15:34.000000 types-uWSGI-2.0.0.20240311/types_uWSGI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-11 02:15:34.000000 types-uWSGI-2.0.0.20240311/types_uWSGI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:15:35.009679 types-uWSGI-2.0.0.20240311/uwsgi-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-11 02:15:34.000000 types-uWSGI-2.0.0.20240311/uwsgi-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)    11898 2024-03-11 02:15:34.000000 types-uWSGI-2.0.0.20240311/uwsgi-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 02:15:35.009679 types-uWSGI-2.0.0.20240311/uwsgidecorators-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-11 02:15:34.000000 types-uWSGI-2.0.0.20240311/uwsgidecorators-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-03-11 02:15:34.000000 types-uWSGI-2.0.0.20240311/uwsgidecorators-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 03:12:24.792696 types-uWSGI-2.0.0.20240414/
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-14 03:12:22.000000 types-uWSGI-2.0.0.20240414/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-14 03:12:22.000000 types-uWSGI-2.0.0.20240414/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-14 03:12:24.792696 types-uWSGI-2.0.0.20240414/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 03:12:24.792696 types-uWSGI-2.0.0.20240414/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-14 03:12:22.000000 types-uWSGI-2.0.0.20240414/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 03:12:24.792696 types-uWSGI-2.0.0.20240414/types_uWSGI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-14 03:12:24.000000 types-uWSGI-2.0.0.20240414/types_uWSGI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-14 03:12:24.000000 types-uWSGI-2.0.0.20240414/types_uWSGI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 03:12:24.000000 types-uWSGI-2.0.0.20240414/types_uWSGI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-14 03:12:24.000000 types-uWSGI-2.0.0.20240414/types_uWSGI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 03:12:24.792696 types-uWSGI-2.0.0.20240414/uwsgi-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-14 03:12:22.000000 types-uWSGI-2.0.0.20240414/uwsgi-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)    11898 2024-04-14 03:12:22.000000 types-uWSGI-2.0.0.20240414/uwsgi-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 03:12:22.000000 types-uWSGI-2.0.0.20240414/uwsgi-stubs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 03:12:24.792696 types-uWSGI-2.0.0.20240414/uwsgidecorators-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-14 03:12:22.000000 types-uWSGI-2.0.0.20240414/uwsgidecorators-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-04-14 03:12:22.000000 types-uWSGI-2.0.0.20240414/uwsgidecorators-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 03:12:22.000000 types-uWSGI-2.0.0.20240414/uwsgidecorators-stubs/py.typed
```

### Comparing `types-uWSGI-2.0.0.20240311/PKG-INFO` & `types-uWSGI-2.0.0.20240414/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-uWSGI
-Version: 2.0.0.20240311
+Version: 2.0.0.20240414
 Summary: Typing stubs for uWSGI
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/uWSGI.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -30,10 +30,10 @@
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/uWSGI. All fixes for
 types and metadata should be contributed there.
 
 Type hints for uWSGI's [Python API](https://uwsgi-docs.readthedocs.io/en/latest/PythonModule.html). Note that this API is available only when running Python code inside a uWSGI process and some parts of the API are only present when corresponding configuration options have been enabled.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `b78de5712df6d3976e24cdebb2c2cedc9d780378` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-uWSGI-2.0.0.20240311/setup.py` & `types-uWSGI-2.0.0.20240414/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,34 +19,34 @@
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/uWSGI. All fixes for
 types and metadata should be contributed there.
 
 Type hints for uWSGI's [Python API](https://uwsgi-docs.readthedocs.io/en/latest/PythonModule.html). Note that this API is available only when running Python code inside a uWSGI process and some parts of the API are only present when corresponding configuration options have been enabled.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `b78de5712df6d3976e24cdebb2c2cedc9d780378` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="2.0.0.20240311",
+      version="2.0.0.20240414",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/uWSGI.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
-      packages=['uwsgi-stubs', 'uwsgidecorators-stubs'],
-      package_data={'uwsgi-stubs': ['__init__.pyi', 'METADATA.toml'], 'uwsgidecorators-stubs': ['__init__.pyi', 'METADATA.toml']},
+      packages=['uwsgidecorators-stubs', 'uwsgi-stubs'],
+      package_data={'uwsgidecorators-stubs': ['__init__.pyi', 'METADATA.toml', 'py.typed'], 'uwsgi-stubs': ['__init__.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
```

### Comparing `types-uWSGI-2.0.0.20240311/types_uWSGI.egg-info/PKG-INFO` & `types-uWSGI-2.0.0.20240414/types_uWSGI.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-uWSGI
-Version: 2.0.0.20240311
+Version: 2.0.0.20240414
 Summary: Typing stubs for uWSGI
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/uWSGI.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -30,10 +30,10 @@
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/uWSGI. All fixes for
 types and metadata should be contributed there.
 
 Type hints for uWSGI's [Python API](https://uwsgi-docs.readthedocs.io/en/latest/PythonModule.html). Note that this API is available only when running Python code inside a uWSGI process and some parts of the API are only present when corresponding configuration options have been enabled.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `3802899a01269df575ea32a21534c5400fb9218a` and was tested
-with mypy 1.9.0, pyright 1.1.350, and
-pytype 2024.2.27.
+This package was generated from typeshed commit `b78de5712df6d3976e24cdebb2c2cedc9d780378` and was tested
+with mypy 1.9.0, pyright 1.1.358, and
+pytype 2024.4.11.
```

### Comparing `types-uWSGI-2.0.0.20240311/uwsgi-stubs/METADATA.toml` & `types-uWSGI-2.0.0.20240414/uwsgi-stubs/METADATA.toml`

 * *Files identical despite different names*

### Comparing `types-uWSGI-2.0.0.20240311/uwsgi-stubs/__init__.pyi` & `types-uWSGI-2.0.0.20240414/uwsgi-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-uWSGI-2.0.0.20240311/uwsgidecorators-stubs/METADATA.toml` & `types-uWSGI-2.0.0.20240414/uwsgidecorators-stubs/METADATA.toml`

 * *Files identical despite different names*

### Comparing `types-uWSGI-2.0.0.20240311/uwsgidecorators-stubs/__init__.pyi` & `types-uWSGI-2.0.0.20240414/uwsgidecorators-stubs/__init__.pyi`

 * *Files identical despite different names*

