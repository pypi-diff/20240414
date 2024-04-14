# Comparing `tmp/aiooss2-0.2.8.tar.gz` & `tmp/aiooss2-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiooss2-0.2.8.tar", last modified: Tue Dec  5 16:30:41 2023, max compression
+gzip compressed data, was "aiooss2-0.2.9.tar", last modified: Fri Feb  2 20:15:50 2024, max compression
```

## Comparing `aiooss2-0.2.8.tar` & `aiooss2-0.2.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:30:41.267514 aiooss2-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)      766 2023-12-05 16:30:19.000000 aiooss2-0.2.8/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-12-05 16:30:19.000000 aiooss2-0.2.8/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:30:41.259514 aiooss2-0.2.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      737 2023-12-05 16:30:19.000000 aiooss2-0.2.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:30:41.259514 aiooss2-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      724 2023-12-05 16:30:19.000000 aiooss2-0.2.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-12-05 16:30:19.000000 aiooss2-0.2.8/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      298 2023-12-05 16:30:19.000000 aiooss2-0.2.8/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2023-12-05 16:30:19.000000 aiooss2-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2023-12-05 16:30:19.000000 aiooss2-0.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-12-05 16:30:19.000000 aiooss2-0.2.8/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2023-12-05 16:30:19.000000 aiooss2-0.2.8/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2023-12-05 16:30:19.000000 aiooss2-0.2.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2023-12-05 16:30:19.000000 aiooss2-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-12-05 16:30:19.000000 aiooss2-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2023-12-05 16:30:41.267514 aiooss2-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2023-12-05 16:30:19.000000 aiooss2-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2023-12-05 16:30:19.000000 aiooss2-0.2.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:30:41.259514 aiooss2-0.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:30:41.259514 aiooss2-0.2.8/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2023-12-05 16:30:19.000000 aiooss2-0.2.8/docs/assets/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      759 2023-12-05 16:30:19.000000 aiooss2-0.2.8/docs/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-05 16:30:19.000000 aiooss2-0.2.8/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:30:41.259514 aiooss2-0.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2023-12-05 16:30:19.000000 aiooss2-0.2.8/examples/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2023-12-05 16:30:19.000000 aiooss2-0.2.8/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2023-12-05 16:30:19.000000 aiooss2-0.2.8/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2023-12-05 16:30:19.000000 aiooss2-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2023-12-05 16:30:41.267514 aiooss2-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:30:41.255514 aiooss2-0.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:30:41.263514 aiooss2-0.2.8/src/aiooss2/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-05 16:30:19.000000 aiooss2-0.2.8/src/aiooss2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7187 2023-12-05 16:30:19.000000 aiooss2-0.2.8/src/aiooss2/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    29416 2023-12-05 16:30:19.000000 aiooss2-0.2.8/src/aiooss2/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2023-12-05 16:30:19.000000 aiooss2-0.2.8/src/aiooss2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2023-12-05 16:30:19.000000 aiooss2-0.2.8/src/aiooss2/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     6208 2023-12-05 16:30:19.000000 aiooss2-0.2.8/src/aiooss2/iterators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5673 2023-12-05 16:30:19.000000 aiooss2-0.2.8/src/aiooss2/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    10159 2023-12-05 16:30:19.000000 aiooss2-0.2.8/src/aiooss2/multipart.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 16:30:19.000000 aiooss2-0.2.8/src/aiooss2/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    19767 2023-12-05 16:30:19.000000 aiooss2-0.2.8/src/aiooss2/resumable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2938 2023-12-05 16:30:19.000000 aiooss2-0.2.8/src/aiooss2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:30:41.263514 aiooss2-0.2.8/src/aiooss2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2023-12-05 16:30:41.000000 aiooss2-0.2.8/src/aiooss2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-12-05 16:30:41.000000 aiooss2-0.2.8/src/aiooss2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 16:30:41.000000 aiooss2-0.2.8/src/aiooss2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-05 16:30:41.000000 aiooss2-0.2.8/src/aiooss2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      297 2023-12-05 16:30:41.000000 aiooss2-0.2.8/src/aiooss2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-05 16:30:41.000000 aiooss2-0.2.8/src/aiooss2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:30:41.263514 aiooss2-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-12-05 16:30:19.000000 aiooss2-0.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2023-12-05 16:30:19.000000 aiooss2-0.2.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:30:41.263514 aiooss2-0.2.8/tests/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 16:30:19.000000 aiooss2-0.2.8/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2023-12-05 16:30:19.000000 aiooss2-0.2.8/tests/func/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     9370 2023-12-05 16:30:19.000000 aiooss2-0.2.8/tests/func/test_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2023-12-05 16:30:19.000000 aiooss2-0.2.8/tests/func/test_resumable.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-12-05 16:30:19.000000 aiooss2-0.2.8/tests/test_aiooss2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-05 16:30:41.263514 aiooss2-0.2.8/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-05 16:30:19.000000 aiooss2-0.2.8/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2023-12-05 16:30:19.000000 aiooss2-0.2.8/tests/unit/test_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:15:50.755165 aiooss2-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-02-02 20:15:26.000000 aiooss2-0.2.9/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-02 20:15:26.000000 aiooss2-0.2.9/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:15:50.747165 aiooss2-0.2.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-02-02 20:15:26.000000 aiooss2-0.2.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:15:50.747165 aiooss2-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-02-02 20:15:26.000000 aiooss2-0.2.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-02-02 20:15:26.000000 aiooss2-0.2.9/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-02-02 20:15:26.000000 aiooss2-0.2.9/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-02-02 20:15:26.000000 aiooss2-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-02-02 20:15:26.000000 aiooss2-0.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-02 20:15:26.000000 aiooss2-0.2.9/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-02-02 20:15:26.000000 aiooss2-0.2.9/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-02-02 20:15:26.000000 aiooss2-0.2.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-02-02 20:15:26.000000 aiooss2-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-02 20:15:26.000000 aiooss2-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-02-02 20:15:50.755165 aiooss2-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-02-02 20:15:26.000000 aiooss2-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-02-02 20:15:26.000000 aiooss2-0.2.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:15:50.747165 aiooss2-0.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:15:50.747165 aiooss2-0.2.9/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-02-02 20:15:26.000000 aiooss2-0.2.9/docs/assets/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-02-02 20:15:26.000000 aiooss2-0.2.9/docs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-02 20:15:26.000000 aiooss2-0.2.9/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:15:50.747165 aiooss2-0.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-02-02 20:15:26.000000 aiooss2-0.2.9/examples/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-02-02 20:15:26.000000 aiooss2-0.2.9/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-02-02 20:15:26.000000 aiooss2-0.2.9/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-02-02 20:15:26.000000 aiooss2-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-02-02 20:15:50.755165 aiooss2-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:15:50.743165 aiooss2-0.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:15:50.751165 aiooss2-0.2.9/src/aiooss2/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-02-02 20:15:26.000000 aiooss2-0.2.9/src/aiooss2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-02-02 20:15:26.000000 aiooss2-0.2.9/src/aiooss2/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29416 2024-02-02 20:15:26.000000 aiooss2-0.2.9/src/aiooss2/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-02-02 20:15:26.000000 aiooss2-0.2.9/src/aiooss2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-02-02 20:15:26.000000 aiooss2-0.2.9/src/aiooss2/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6208 2024-02-02 20:15:26.000000 aiooss2-0.2.9/src/aiooss2/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5673 2024-02-02 20:15:26.000000 aiooss2-0.2.9/src/aiooss2/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10159 2024-02-02 20:15:26.000000 aiooss2-0.2.9/src/aiooss2/multipart.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 20:15:26.000000 aiooss2-0.2.9/src/aiooss2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19767 2024-02-02 20:15:26.000000 aiooss2-0.2.9/src/aiooss2/resumable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-02-02 20:15:26.000000 aiooss2-0.2.9/src/aiooss2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:15:50.755165 aiooss2-0.2.9/src/aiooss2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-02-02 20:15:50.000000 aiooss2-0.2.9/src/aiooss2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-02 20:15:50.000000 aiooss2-0.2.9/src/aiooss2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 20:15:50.000000 aiooss2-0.2.9/src/aiooss2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 20:15:50.000000 aiooss2-0.2.9/src/aiooss2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-02-02 20:15:50.000000 aiooss2-0.2.9/src/aiooss2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-02 20:15:50.000000 aiooss2-0.2.9/src/aiooss2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:15:50.751165 aiooss2-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-02 20:15:26.000000 aiooss2-0.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-02-02 20:15:26.000000 aiooss2-0.2.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:15:50.751165 aiooss2-0.2.9/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 20:15:26.000000 aiooss2-0.2.9/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-02 20:15:26.000000 aiooss2-0.2.9/tests/func/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9370 2024-02-02 20:15:26.000000 aiooss2-0.2.9/tests/func/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-02-02 20:15:26.000000 aiooss2-0.2.9/tests/func/test_resumable.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-02 20:15:26.000000 aiooss2-0.2.9/tests/test_aiooss2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 20:15:50.751165 aiooss2-0.2.9/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 20:15:26.000000 aiooss2-0.2.9/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2024-02-02 20:15:26.000000 aiooss2-0.2.9/tests/unit/test_adapter.py
```

### Comparing `aiooss2-0.2.8/.cruft.json` & `aiooss2-0.2.9/.cruft.json`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/.github/dependabot.yml` & `aiooss2-0.2.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/.github/workflows/release.yml` & `aiooss2-0.2.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/.github/workflows/tests.yml` & `aiooss2-0.2.9/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/.gitignore` & `aiooss2-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/.pre-commit-config.yaml` & `aiooss2-0.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/CODE_OF_CONDUCT.rst` & `aiooss2-0.2.9/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/CONTRIBUTING.rst` & `aiooss2-0.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/LICENSE` & `aiooss2-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/PKG-INFO` & `aiooss2-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiooss2
-Version: 0.2.8
+Version: 0.2.9
 Summary: Async client for aliyun OSS(Object Storage Service) using oss2 and aiohttp/asyncio
 Home-page: https://github.com/karajan1001/aiooss2
 Maintainer-email: mishanyo1001@gmail.com
 License: Apache-2.0
 Keywords: "oss,aio"
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: aiohttp==3.9.1
+Requires-Dist: aiohttp<4,>=3.9.1
 Requires-Dist: oss2==2.18.1
 Provides-Extra: tests
 Requires-Dist: pytest==7.2.0; extra == "tests"
 Requires-Dist: pytest-sugar==0.9.5; extra == "tests"
 Requires-Dist: pytest-cov==3.0.0; extra == "tests"
 Requires-Dist: pytest-mock==3.8.2; extra == "tests"
 Requires-Dist: pylint==2.15.0; extra == "tests"
```

### Comparing `aiooss2-0.2.8/README.md` & `aiooss2-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/README.rst` & `aiooss2-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/docs/assets/logo.svg` & `aiooss2-0.2.9/docs/assets/logo.svg`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/docs/gen_ref_pages.py` & `aiooss2-0.2.9/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/examples/simple.py` & `aiooss2-0.2.9/examples/simple.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/mkdocs.yml` & `aiooss2-0.2.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/noxfile.py` & `aiooss2-0.2.9/noxfile.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/pyproject.toml` & `aiooss2-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/setup.cfg` & `aiooss2-0.2.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 python_requires = >=3.8
 zip_safe = False
 packages = find:
 package_dir = 
 	=src
 include_package_data = True
 install_requires = 
-	aiohttp==3.9.1
+	aiohttp>=3.9.1,<4
 	oss2==2.18.1
 
 [options.extras_require]
 tests = 
 	pytest==7.2.0
 	pytest-sugar==0.9.5
 	pytest-cov==3.0.0
```

### Comparing `aiooss2-0.2.8/src/aiooss2/adapter.py` & `aiooss2-0.2.9/src/aiooss2/adapter.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/src/aiooss2/api.py` & `aiooss2-0.2.9/src/aiooss2/api.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/src/aiooss2/exceptions.py` & `aiooss2-0.2.9/src/aiooss2/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/src/aiooss2/http.py` & `aiooss2-0.2.9/src/aiooss2/http.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/src/aiooss2/iterators.py` & `aiooss2-0.2.9/src/aiooss2/iterators.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/src/aiooss2/models.py` & `aiooss2-0.2.9/src/aiooss2/models.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/src/aiooss2/multipart.py` & `aiooss2-0.2.9/src/aiooss2/multipart.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/src/aiooss2/resumable.py` & `aiooss2-0.2.9/src/aiooss2/resumable.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/src/aiooss2/utils.py` & `aiooss2-0.2.9/src/aiooss2/utils.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/src/aiooss2.egg-info/PKG-INFO` & `aiooss2-0.2.9/src/aiooss2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiooss2
-Version: 0.2.8
+Version: 0.2.9
 Summary: Async client for aliyun OSS(Object Storage Service) using oss2 and aiohttp/asyncio
 Home-page: https://github.com/karajan1001/aiooss2
 Maintainer-email: mishanyo1001@gmail.com
 License: Apache-2.0
 Keywords: "oss,aio"
 Platform: any
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: aiohttp==3.9.1
+Requires-Dist: aiohttp<4,>=3.9.1
 Requires-Dist: oss2==2.18.1
 Provides-Extra: tests
 Requires-Dist: pytest==7.2.0; extra == "tests"
 Requires-Dist: pytest-sugar==0.9.5; extra == "tests"
 Requires-Dist: pytest-cov==3.0.0; extra == "tests"
 Requires-Dist: pytest-mock==3.8.2; extra == "tests"
 Requires-Dist: pylint==2.15.0; extra == "tests"
```

### Comparing `aiooss2-0.2.8/src/aiooss2.egg-info/SOURCES.txt` & `aiooss2-0.2.9/src/aiooss2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/tests/conftest.py` & `aiooss2-0.2.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/tests/func/test_bucket.py` & `aiooss2-0.2.9/tests/func/test_bucket.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/tests/func/test_object.py` & `aiooss2-0.2.9/tests/func/test_object.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/tests/func/test_resumable.py` & `aiooss2-0.2.9/tests/func/test_resumable.py`

 * *Files identical despite different names*

### Comparing `aiooss2-0.2.8/tests/unit/test_adapter.py` & `aiooss2-0.2.9/tests/unit/test_adapter.py`

 * *Files identical despite different names*

