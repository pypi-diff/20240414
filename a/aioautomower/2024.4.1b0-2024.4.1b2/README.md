# Comparing `tmp/aioautomower-2024.4.1b0.tar.gz` & `tmp/aioautomower-2024.4.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioautomower-2024.4.1b0.tar", last modified: Sat Apr 13 18:55:05 2024, max compression
+gzip compressed data, was "aioautomower-2024.4.1b2.tar", max compression
```

## Comparing `aioautomower-2024.4.1b0.tar` & `aioautomower-2024.4.1b2.tar`

### file list

```diff
@@ -1,27 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:55:05.643852 aioautomower-2024.4.1b0/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-13 18:55:05.643852 aioautomower-2024.4.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:55:05.639852 aioautomower-2024.4.1b0/aioautomower/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/aioautomower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7302 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/aioautomower/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/aioautomower/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/aioautomower/example.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/aioautomower/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/aioautomower/model.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/aioautomower/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/aioautomower/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/aioautomower/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:55:05.643852 aioautomower-2024.4.1b0/aioautomower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-13 18:55:05.000000 aioautomower-2024.4.1b0/aioautomower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-13 18:55:05.000000 aioautomower-2024.4.1b0/aioautomower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 18:55:05.000000 aioautomower-2024.4.1b0/aioautomower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 18:55:05.000000 aioautomower-2024.4.1b0/aioautomower.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 18:55:05.000000 aioautomower-2024.4.1b0/aioautomower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-13 18:55:05.000000 aioautomower-2024.4.1b0/aioautomower.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-13 18:55:03.000000 aioautomower-2024.4.1b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 18:55:05.643852 aioautomower-2024.4.1b0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 18:55:05.643852 aioautomower-2024.4.1b0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/tests/test_error_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/tests/test_high_feature_mower_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/tests/test_jwt_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-13 18:54:59.000000 aioautomower-2024.4.1b0/tests/test_low_feature_mower_model.py
+-rw-r--r--   0        0        0     1152 2024-04-14 18:10:24.543923 aioautomower-2024.4.1b2/README.md
+-rw-r--r--   0        0        0     2177 2024-04-14 18:10:36.255894 aioautomower-2024.4.1b2/pyproject.toml
+-rw-r--r--   0        0        0      138 2024-04-14 18:10:24.543923 aioautomower-2024.4.1b2/src/aioautomower/__init__.py
+-rw-r--r--   0        0        0     7302 2024-04-14 18:10:24.543923 aioautomower-2024.4.1b2/src/aioautomower/auth.py
+-rw-r--r--   0        0        0     5812 2024-04-14 18:10:24.543923 aioautomower-2024.4.1b2/src/aioautomower/const.py
+-rw-r--r--   0        0        0     4358 2024-04-14 18:10:24.543923 aioautomower-2024.4.1b2/src/aioautomower/example.py
+-rw-r--r--   0        0        0      969 2024-04-14 18:10:24.543923 aioautomower-2024.4.1b2/src/aioautomower/exceptions.py
+-rw-r--r--   0        0        0    10741 2024-04-14 18:10:24.547923 aioautomower-2024.4.1b2/src/aioautomower/model.py
+-rw-r--r--   0        0        0        0 2024-04-14 18:10:24.547923 aioautomower-2024.4.1b2/src/aioautomower/py.typed
+-rw-r--r--   0        0        0    12222 2024-04-14 18:10:24.547923 aioautomower-2024.4.1b2/src/aioautomower/session.py
+-rw-r--r--   0        0        0     4200 2024-04-14 18:10:24.547923 aioautomower-2024.4.1b2/src/aioautomower/utils.py
+-rw-r--r--   0        0        0     1964 1970-01-01 00:00:00.000000 aioautomower-2024.4.1b2/PKG-INFO
```

### Comparing `aioautomower-2024.4.1b0/PKG-INFO` & `aioautomower-2024.4.1b2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: aioautomower
-Version: 2024.4.1b0
+Version: 2024.4.1b2
 Summary: MPython module to talk to Husqvarna Automower.
-Author-email: Thomas Protzner <thomas.protzner@gmail.com>
-License: Apache-2.0
+Home-page: https://github.com/Thomas55555/aioautomower
+License: Apache 2.0
+Author: Thomas55555
+Requires-Python: >=3.11,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: PyJWT (>=2.8.0,<3.0.0)
+Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
+Requires-Dist: mashumaro (>=3.12,<4.0)
 Project-URL: Documentation, https://github.com/Thomas55555/aioautomower
-Project-URL: Repository, https://github.com/Thomas55555/aioautomower
 Project-URL: Issues, https://github.com/Thomas55555/aioautomower/issues
-Platform: any
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
+Project-URL: Repository, https://github.com/Thomas55555/aioautomower
 Description-Content-Type: text/markdown
-Requires-Dist: aiohttp
-Requires-Dist: mashumaro
-Requires-Dist: PyJWT
 
 # Aioautomower
 
 Asynchronous library to communicate with the Automower Connect API
 To use this library, you need to register on the [Husqvarna Developers Portal](https://developer.husqvarnagroup.cloud/).
 And connect your account to the `Authentication API` and the `Automower Connect API`.
 
@@ -36,12 +38,7 @@
 For a first start you can run the `example.py`, by doing the following steps
 
 - `git clone https://github.com/Thomas55555/aioautomower.git`
 - `pip install -e ./`
 - Enter your personal `client_id` and `client_secret` in the `example.py`
 - Run with `python3 ./aioautomower/example.py`
 
-## AutomowerCLI example
-
-An AutomowerSession that provides you with the data in a CLI
-
-`automower --client_secret 12312312-12ec-486b-a7a7-9d9b06644a14  --api-key 12312312-0126-6222-2662-3e6c49f0012c`
```

### Comparing `aioautomower-2024.4.1b0/README.md` & `aioautomower-2024.4.1b2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -17,13 +17,7 @@
 
 For a first start you can run the `example.py`, by doing the following steps
 
 - `git clone https://github.com/Thomas55555/aioautomower.git`
 - `pip install -e ./`
 - Enter your personal `client_id` and `client_secret` in the `example.py`
 - Run with `python3 ./aioautomower/example.py`
-
-## AutomowerCLI example
-
-An AutomowerSession that provides you with the data in a CLI
-
-`automower --client_secret 12312312-12ec-486b-a7a7-9d9b06644a14  --api-key 12312312-0126-6222-2662-3e6c49f0012c`
```

### Comparing `aioautomower-2024.4.1b0/aioautomower/auth.py` & `aioautomower-2024.4.1b2/src/aioautomower/auth.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.4.1b0/aioautomower/const.py` & `aioautomower-2024.4.1b2/src/aioautomower/const.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.4.1b0/aioautomower/example.py` & `aioautomower-2024.4.1b2/src/aioautomower/example.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.4.1b0/aioautomower/exceptions.py` & `aioautomower-2024.4.1b2/src/aioautomower/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.4.1b0/aioautomower/model.py` & `aioautomower-2024.4.1b2/src/aioautomower/model.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.4.1b0/aioautomower/session.py` & `aioautomower-2024.4.1b2/src/aioautomower/session.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.4.1b0/aioautomower/utils.py` & `aioautomower-2024.4.1b2/src/aioautomower/utils.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2024.4.1b0/pyproject.toml` & `aioautomower-2024.4.1b2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,141 +1,102 @@
 [build-system]
-requires = [
-    "setuptools>=62.3",
-]
-build-backend = "setuptools.build_meta"
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
 
-[project]
+[tool.poetry]
 name = "aioautomower"
-version = "2024.4.1b"
+# The version is set by GH action on release
+version = "2024.4.1b2"
 description = "MPython module to talk to Husqvarna Automower."
+authors = ["Thomas55555"]
+license = "Apache 2.0"
 readme = "README.md"
-requires-python = ">=3.10"
-authors = [
-    { name = "Thomas Protzner", email = "thomas.protzner@gmail.com" },
-]
-classifiers = [
-    "Environment :: Console",
-    "Programming Language :: Python :: 3",
-]
-dependencies = [
-    "aiohttp",
-    "mashumaro",
-    "PyJWT",
+packages = [
+    { include = "aioautomower", from = "src" },
 ]
+homepage = "https://github.com/Thomas55555/aioautomower"
+repository = "https://github.com/Thomas55555/aioautomower"
+documentation = "https://github.com/Thomas55555/aioautomower"
 
-[project.license]
-text = "Apache-2.0"
-
-[project.urls]
-Documentation = "https://github.com/Thomas55555/aioautomower"
-Repository = "https://github.com/Thomas55555/aioautomower"
+[tool.poetry.urls]
 Issues = "https://github.com/Thomas55555/aioautomower/issues"
 
-[tool.poetry]
-name = "aioautomower"
-version = "0.0.0"
-description = "MPython module to talk to Husqvarna Automower."
-authors = [
-    "Thomas55555",
-]
-license = "Apache 2.0"
-
 [tool.poetry.dependencies]
 python = "^3.11"
 aiohttp = "^3.9.3"
 mashumaro = "^3.12"
 PyJWT = "^2.8.0"
 
 [tool.poetry.group.dev.dependencies]
 codespell = "2.2.6"
 covdefaults = "2.3.0"
+coverage = {version = "7.4.4", extras = ["toml"]}
 mypy = "1.9.0"
 pre-commit = "3.7.0"
 pre-commit-hooks = "4.6.0"
 pylint = "3.1.0"
 pytest = "8.1.1"
 pytest-asyncio = "0.23.6"
 pytest-cov = "5.0.0"
-ruff = "0.3.6"
+ruff = "0.3.7"
 safety = "3.1.0"
 yamllint = "1.35.1"
 syrupy = "4.6.1"
 aioresponses = "0.7.6"
 freezegun = "^1.4.0"
 
-[tool.poetry.group.dev.dependencies.coverage]
-version = "7.4.4"
-extras = [
-    "toml",
-]
-
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
-
-[tool.setuptools]
-platforms = [
-    "any",
-]
-zip-safe = false
-packages = [
-    "aioautomower",
-]
-include-package-data = true
-
-[tool.setuptools.package-data]
-aioautomower = [
-    "py.typed",
-]
+pythonpath = ["src"]
 
 [tool.ruff]
 fix = true
 show-fixes = true
 
+[tool.pylint.FORMAT]
+max-line-length = 88
+
 [tool.ruff.lint.flake8-annotations]
 allow-star-arg-any = true
 suppress-dummy-args = true
 
 [tool.ruff.lint.flake8-builtins]
-builtins-ignorelist = [
-    "id",
-]
+builtins-ignorelist = ["id"]
 
 [tool.ruff.lint.pydocstyle]
+# Use Google-style docstrings.
 convention = "pep257"
 
 [tool.ruff.lint.pylint]
-max-branches = 25
-max-returns = 15
-max-args = 10
-max-statements = 50
+max-branches=25
+max-returns=15
+max-args=10
+max-statements=50
 
 [tool.pylint]
-ignore = [
-    "R0902",
-]
-
-[tool.pylint.FORMAT]
-max-line-length = 88
+ignore = ["R0902"]
 
 [tool.pylint.MASTER]
 ignore = [
-    "tests",
+  "tests",
 ]
 
 [tool.mypy]
+# Specify the target platform details in config, so your developers are
+# free to run mypy on Windows, Linux, or macOS and get consistent
+# results.
 platform = "linux"
 python_version = "3.11"
+
+# show error messages from unrelated files
 follow_imports = "normal"
+
+# suppress errors about unsatisfied imports
 ignore_missing_imports = true
 
 [tool.coverage.report]
 show_missing = true
 fail_under = 30
 
 [tool.coverage.run]
-plugins = [
-    "covdefaults",
-]
-source = [
-    "aioautomower/*.py",
-]
+plugins = ["covdefaults"]
+source = ["aioautomower/*.py"]
```

