# Comparing `tmp/python3-commons-0.3.8.tar.gz` & `tmp/python3-commons-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3-commons-0.3.8.tar", last modified: Mon Feb  5 16:28:24 2024, max compression
+gzip compressed data, was "python3-commons-0.3.9.tar", last modified: Wed Feb 14 13:33:21 2024, max compression
```

## Comparing `python3-commons-0.3.8.tar` & `python3-commons-0.3.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:28:24.343610 python3-commons-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-05 16:28:13.000000 python3-commons-0.3.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:28:24.335610 python3-commons-0.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:28:24.339610 python3-commons-0.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-02-05 16:28:13.000000 python3-commons-0.3.8/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-02-05 16:28:13.000000 python3-commons-0.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-05 16:28:13.000000 python3-commons-0.3.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-05 16:28:13.000000 python3-commons-0.3.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34575 2024-02-05 16:28:13.000000 python3-commons-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-02-05 16:28:24.343610 python3-commons-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-05 16:28:13.000000 python3-commons-0.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-05 16:28:13.000000 python3-commons-0.3.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:28:24.339610 python3-commons-0.3.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-02-05 16:28:13.000000 python3-commons-0.3.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:28:24.339610 python3-commons-0.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-05 16:28:13.000000 python3-commons-0.3.8/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-05 16:28:13.000000 python3-commons-0.3.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-05 16:28:13.000000 python3-commons-0.3.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-02-05 16:28:13.000000 python3-commons-0.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-02-05 16:28:13.000000 python3-commons-0.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-05 16:28:13.000000 python3-commons-0.3.8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-05 16:28:13.000000 python3-commons-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-05 16:28:13.000000 python3-commons-0.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-05 16:28:13.000000 python3-commons-0.3.8/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-05 16:28:13.000000 python3-commons-0.3.8/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-02-05 16:28:24.343610 python3-commons-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-02-05 16:28:13.000000 python3-commons-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:28:24.335610 python3-commons-0.3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:28:24.339610 python3-commons-0.3.8/src/python3_commons/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-02-05 16:28:13.000000 python3-commons-0.3.8/src/python3_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-02-05 16:28:13.000000 python3-commons-0.3.8/src/python3_commons/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-02-05 16:28:13.000000 python3-commons-0.3.8/src/python3_commons/db.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-05 16:28:13.000000 python3-commons-0.3.8/src/python3_commons/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-02-05 16:28:13.000000 python3-commons-0.3.8/src/python3_commons/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:28:24.343610 python3-commons-0.3.8/src/python3_commons/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 16:28:13.000000 python3-commons-0.3.8/src/python3_commons/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-05 16:28:13.000000 python3-commons-0.3.8/src/python3_commons/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-02-05 16:28:13.000000 python3-commons-0.3.8/src/python3_commons/logging/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-02-05 16:28:13.000000 python3-commons-0.3.8/src/python3_commons/minio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-02-05 16:28:13.000000 python3-commons-0.3.8/src/python3_commons/object_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:28:24.343610 python3-commons-0.3.8/src/python3_commons/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-05 16:28:13.000000 python3-commons-0.3.8/src/python3_commons/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-02-05 16:28:13.000000 python3-commons-0.3.8/src/python3_commons/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-02-05 16:28:13.000000 python3-commons-0.3.8/src/python3_commons/serializers/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-02-05 16:28:13.000000 python3-commons-0.3.8/src/python3_commons/serializers/msgspec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:28:24.343610 python3-commons-0.3.8/src/python3_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-02-05 16:28:24.000000 python3-commons-0.3.8/src/python3_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-02-05 16:28:24.000000 python3-commons-0.3.8/src/python3_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 16:28:24.000000 python3-commons-0.3.8/src/python3_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 16:28:24.000000 python3-commons-0.3.8/src/python3_commons.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-05 16:28:24.000000 python3-commons-0.3.8/src/python3_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-05 16:28:24.000000 python3-commons-0.3.8/src/python3_commons.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 16:28:24.343610 python3-commons-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-02-05 16:28:13.000000 python3-commons-0.3.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-02-05 16:28:13.000000 python3-commons-0.3.8/tests/test_msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-02-05 16:28:13.000000 python3-commons-0.3.8/tests/test_msgspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:33:21.269012 python3-commons-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-14 13:33:08.000000 python3-commons-0.3.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:33:21.261012 python3-commons-0.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:33:21.261012 python3-commons-0.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-02-14 13:33:08.000000 python3-commons-0.3.9/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-02-14 13:33:08.000000 python3-commons-0.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-14 13:33:08.000000 python3-commons-0.3.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-14 13:33:08.000000 python3-commons-0.3.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34575 2024-02-14 13:33:08.000000 python3-commons-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-02-14 13:33:21.269012 python3-commons-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-14 13:33:08.000000 python3-commons-0.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-14 13:33:08.000000 python3-commons-0.3.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:33:21.265012 python3-commons-0.3.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-02-14 13:33:08.000000 python3-commons-0.3.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:33:21.265012 python3-commons-0.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-14 13:33:08.000000 python3-commons-0.3.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-14 13:33:08.000000 python3-commons-0.3.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-14 13:33:08.000000 python3-commons-0.3.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-02-14 13:33:08.000000 python3-commons-0.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-02-14 13:33:08.000000 python3-commons-0.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-14 13:33:08.000000 python3-commons-0.3.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-14 13:33:08.000000 python3-commons-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-14 13:33:08.000000 python3-commons-0.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-14 13:33:08.000000 python3-commons-0.3.9/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-14 13:33:08.000000 python3-commons-0.3.9/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-02-14 13:33:21.269012 python3-commons-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-02-14 13:33:08.000000 python3-commons-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:33:21.261012 python3-commons-0.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:33:21.265012 python3-commons-0.3.9/src/python3_commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-02-14 13:33:08.000000 python3-commons-0.3.9/src/python3_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-02-14 13:33:08.000000 python3-commons-0.3.9/src/python3_commons/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-02-14 13:33:08.000000 python3-commons-0.3.9/src/python3_commons/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-14 13:33:08.000000 python3-commons-0.3.9/src/python3_commons/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-02-14 13:33:08.000000 python3-commons-0.3.9/src/python3_commons/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:33:21.265012 python3-commons-0.3.9/src/python3_commons/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 13:33:08.000000 python3-commons-0.3.9/src/python3_commons/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-14 13:33:08.000000 python3-commons-0.3.9/src/python3_commons/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-02-14 13:33:08.000000 python3-commons-0.3.9/src/python3_commons/logging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-02-14 13:33:08.000000 python3-commons-0.3.9/src/python3_commons/minio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-02-14 13:33:08.000000 python3-commons-0.3.9/src/python3_commons/object_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:33:21.265012 python3-commons-0.3.9/src/python3_commons/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-14 13:33:08.000000 python3-commons-0.3.9/src/python3_commons/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-02-14 13:33:08.000000 python3-commons-0.3.9/src/python3_commons/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-02-14 13:33:08.000000 python3-commons-0.3.9/src/python3_commons/serializers/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-02-14 13:33:08.000000 python3-commons-0.3.9/src/python3_commons/serializers/msgspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:33:21.269012 python3-commons-0.3.9/src/python3_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-02-14 13:33:21.000000 python3-commons-0.3.9/src/python3_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-02-14 13:33:21.000000 python3-commons-0.3.9/src/python3_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 13:33:21.000000 python3-commons-0.3.9/src/python3_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 13:33:21.000000 python3-commons-0.3.9/src/python3_commons.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-14 13:33:21.000000 python3-commons-0.3.9/src/python3_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-14 13:33:21.000000 python3-commons-0.3.9/src/python3_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 13:33:21.265012 python3-commons-0.3.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-02-14 13:33:08.000000 python3-commons-0.3.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-02-14 13:33:08.000000 python3-commons-0.3.9/tests/test_msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-02-14 13:33:08.000000 python3-commons-0.3.9/tests/test_msgspec.py
```

### Comparing `python3-commons-0.3.8/.coveragerc` & `python3-commons-0.3.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `python3-commons-0.3.8/.github/workflows/python-publish.yaml` & `python3-commons-0.3.9/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `python3-commons-0.3.8/.gitignore` & `python3-commons-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `python3-commons-0.3.8/LICENSE` & `python3-commons-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python3-commons-0.3.8/PKG-INFO` & `python3-commons-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.3.8
+Version: 0.3.9
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.12
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: asyncpg==0.29.0
-Requires-Dist: minio==7.2.3
+Requires-Dist: minio==7.2.4
 Requires-Dist: msgpack==1.0.7
 Requires-Dist: msgspec==0.18.6
 Requires-Dist: pydantic[email]==2.6.1
 Requires-Dist: pydantic-settings==2.1.0
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
```

### Comparing `python3-commons-0.3.8/docs/Makefile` & `python3-commons-0.3.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python3-commons-0.3.8/docs/conf.py` & `python3-commons-0.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.3.8/docs/index.rst` & `python3-commons-0.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python3-commons-0.3.8/setup.cfg` & `python3-commons-0.3.9/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python3-commons
-version = 0.3.8
+version = 0.3.9
 description = Re-usable Python3 code
 author = Oleg Korsak
 author_email = kamikaze.is.waiting.you@gmail.com
 license = gpl-3
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/kamikaze/python3-commons
@@ -20,15 +20,15 @@
 packages = find:
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = pyscaffold>=3.2a0,<3.3a0
 install_requires = 
 	asyncpg==0.29.0
-	minio==7.2.3
+	minio==7.2.4
 	msgpack==1.0.7
 	msgspec==0.18.6
 	pydantic[email]==2.6.1
 	pydantic-settings==2.1.0
 python_requires = >=3.12
 
 [options.packages.find]
```

### Comparing `python3-commons-0.3.8/src/python3_commons/conf.py` & `python3-commons-0.3.9/src/python3_commons/conf.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.3.8/src/python3_commons/db.py` & `python3-commons-0.3.9/src/python3_commons/db.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.3.8/src/python3_commons/helpers.py` & `python3-commons-0.3.9/src/python3_commons/helpers.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.3.8/src/python3_commons/minio.py` & `python3-commons-0.3.9/src/python3_commons/minio.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.3.8/src/python3_commons/object_storage.py` & `python3-commons-0.3.9/src/python3_commons/object_storage.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.3.8/src/python3_commons/serializers/json.py` & `python3-commons-0.3.9/src/python3_commons/serializers/json.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.3.8/src/python3_commons/serializers/msgpack.py` & `python3-commons-0.3.9/src/python3_commons/serializers/msgpack.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.3.8/src/python3_commons/serializers/msgspec.py` & `python3-commons-0.3.9/src/python3_commons/serializers/msgspec.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.3.8/src/python3_commons.egg-info/PKG-INFO` & `python3-commons-0.3.9/src/python3_commons.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.3.8
+Version: 0.3.9
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.12
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE
 License-File: AUTHORS.rst
 Requires-Dist: asyncpg==0.29.0
-Requires-Dist: minio==7.2.3
+Requires-Dist: minio==7.2.4
 Requires-Dist: msgpack==1.0.7
 Requires-Dist: msgspec==0.18.6
 Requires-Dist: pydantic[email]==2.6.1
 Requires-Dist: pydantic-settings==2.1.0
 Provides-Extra: testing
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
```

### Comparing `python3-commons-0.3.8/src/python3_commons.egg-info/SOURCES.txt` & `python3-commons-0.3.9/src/python3_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python3-commons-0.3.8/tests/conftest.py` & `python3-commons-0.3.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.3.8/tests/test_msgpack.py` & `python3-commons-0.3.9/tests/test_msgpack.py`

 * *Files identical despite different names*

### Comparing `python3-commons-0.3.8/tests/test_msgspec.py` & `python3-commons-0.3.9/tests/test_msgspec.py`

 * *Files identical despite different names*

