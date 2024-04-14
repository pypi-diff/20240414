# Comparing `tmp/backframe-0.1.1.tar.gz` & `tmp/backframe-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backframe-0.1.1.tar", max compression
+gzip compressed data, was "backframe-0.1.2.tar", max compression
```

## Comparing `backframe-0.1.1.tar` & `backframe-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1092 2024-02-20 06:58:16.597633 backframe-0.1.1/LICENSE
--rw-r--r--   0        0        0     3605 2024-02-20 06:58:16.597633 backframe-0.1.1/README.md
--rw-r--r--   0        0        0     4722 2024-02-20 06:58:16.597633 backframe-0.1.1/backframe/__init__.py
--rw-r--r--   0        0        0        0 2024-02-20 06:58:16.597633 backframe-0.1.1/backframe/py.typed
--rw-r--r--   0        0        0     5213 2024-02-20 06:58:16.601633 backframe-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4510 1970-01-01 00:00:00.000000 backframe-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-04-14 00:34:06.541772 backframe-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3697 2024-04-14 00:34:06.541772 backframe-0.1.2/README.md
+-rw-r--r--   0        0        0     4722 2024-04-14 00:34:06.541772 backframe-0.1.2/backframe/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 00:34:06.541772 backframe-0.1.2/backframe/py.typed
+-rw-r--r--   0        0        0     5273 2024-04-14 00:34:06.545771 backframe-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4608 1970-01-01 00:00:00.000000 backframe-0.1.2/PKG-INFO
```

### Comparing `backframe-0.1.1/LICENSE` & `backframe-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `backframe-0.1.1/README.md` & `backframe-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-# backframe [![skeleton](https://img.shields.io/badge/0.0.2rc–149–gaad3c42-skeleton?label=%F0%9F%92%80%20bswck/skeleton&labelColor=black&color=grey&link=https%3A//github.com/bswck/skeleton)](https://github.com/bswck/skeleton/tree/0.0.2rc-149-gaad3c42) [![Supported Python versions](https://img.shields.io/pypi/pyversions/backframe.svg?logo=python&label=Python)](https://pypi.org/project/backframe/) [![Package version](https://img.shields.io/pypi/v/backframe?label=PyPI)](https://pypi.org/project/backframe/)
+# <div align="center">backframe<br>[![skeleton](https://img.shields.io/badge/0.0.2rc–215–g792492f-skeleton?label=%F0%9F%92%80%20skeleton-ci/skeleton-python&labelColor=black&color=grey&link=https%3A//github.com/skeleton-ci/skeleton-python)](https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-215-g792492f) [![Supported Python versions](https://img.shields.io/pypi/pyversions/backframe.svg?logo=python&label=Python)](https://pypi.org/project/backframe/) [![Package version](https://img.shields.io/pypi/v/backframe?label=PyPI)](https://pypi.org/project/backframe/)</div>
 
 [![Tests](https://github.com/bswck/backframe/actions/workflows/test.yml/badge.svg)](https://github.com/bswck/backframe/actions/workflows/test.yml)
 [![Coverage](https://coverage-badge.samuelcolvin.workers.dev/bswck/backframe.svg)](https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/backframe)
 [![Documentation Status](https://readthedocs.org/projects/backframe/badge/?version=latest)](https://backframe.readthedocs.io/en/latest/?badge=latest)
 
-
-
 Inspect the caller.
 
 # Installation
 You might simply install it with pip:
 
 ```shell
 pip install backframe
@@ -17,22 +15,22 @@
 
 If you use [Poetry](https://python-poetry.org/), then you might want to run:
 
 ```shell
 poetry add backframe
 ```
 
-## For contributors
+## For Contributors
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 <!--
-This section was generated from bswck/skeleton@0.0.2rc-149-gaad3c42.
+This section was generated from skeleton-ci/skeleton-python@0.0.2rc-215-g792492f.
 Instead of changing this particular file, you might want to alter the template:
-https://github.com/bswck/skeleton/tree/0.0.2rc-149-gaad3c42/project/README.md.jinja
+https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-215-g792492f/project/README.md.jinja
 -->
 > [!Note]
 > If you use Windows, it is highly recommended to complete the installation in the way presented below through [WSL2](https://learn.microsoft.com/en-us/windows/wsl/install).
 1.  Fork the [backframe repository](https://github.com/bswck/backframe) on GitHub.
 
 1.  [Install Poetry](https://python-poetry.org/docs/#installation).<br/>
     Poetry is an amazing tool for managing dependencies & virtual environments, building packages and publishing them.
@@ -65,10 +63,10 @@
     poetry shell
     pre-commit install
     ```
 
 For more information on how to contribute, check out [CONTRIBUTING.md](https://github.com/bswck/backframe/blob/HEAD/CONTRIBUTING.md).<br/>
 Always happy to accept contributions! ❤️
 
-# Legal info
+# Legal Info
 © Copyright by Bartosz Sławecki ([@bswck](https://github.com/bswck)).
 <br />This software is licensed under the terms of [MIT License](https://github.com/bswck/backframe/blob/HEAD/LICENSE).
```

### Comparing `backframe-0.1.1/backframe/__init__.py` & `backframe-0.1.2/backframe/__init__.py`

 * *Files identical despite different names*

### Comparing `backframe-0.1.1/pyproject.toml` & `backframe-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-# This file was generated from bswck/skeleton@0.0.2rc-149-gaad3c42.
+# This file was generated from skeleton-ci/skeleton-python@0.0.2rc-215-g792492f.
 # Instead of changing this particular file, you might want to alter the template:
-# https://github.com/bswck/skeleton/tree/0.0.2rc-149-gaad3c42/project/pyproject.toml.jinja
+# https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-215-g792492f/project/pyproject.toml.jinja
 
 [tool.poetry]
 name = "backframe"
-version = "0.1.1"
+version = "0.1.2"
 description = "Inspect the caller."
-authors = ["bswck <bswck.dev@gmail.com>"]
+authors = ["bswck <bartoszpiotrslawecki@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "backframe/" }]
 homepage = "https://github.com/bswck/backframe"
 
 [tool.poetry.urls]
 Documentation = "https://backframe.readthedocs.io/en/latest/"
 Issues = "https://github.com/bswck/backframe/issues"
 Distribution = "https://pypi.org/project/backframe/"
 Coverage = "https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/backframe"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.8"
 
 [tool.poetry.group.dev.dependencies]
 
 [tool.poetry.group.dev-skeleton.dependencies]
-# This dependency group was generated from bswck/skeleton@0.0.2rc-149-gaad3c42.
+# This dependency group was generated from skeleton-ci/skeleton-python@0.0.2rc-215-g792492f.
 # Instead of changing this particular file, you might want to alter the template:
-# https://github.com/bswck/skeleton/tree/0.0.2rc-149-gaad3c42/project/pyproject.toml.jinja
-mypy = "^1.7.0"
-ruff = "^0.2.1"
-towncrier = "^23.11.0"
-coverage = "^7.4.0"
-pytest = "^8.0.0"
-pytest-doctestplus = "^1.1.0"
-covdefaults = "^2.3.0"
-poethepoet = "^0.24.3"
-pre-commit = "^3.5.0"
-smokeshow = "^0.4.0"
-keyring = "^24.3.0"
+# https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-215-g792492f/project/pyproject.toml.jinja
+mypy = ">=1.9.0"
+ruff = ">=0.3.4"
+towncrier = ">=23.11.0"
+coverage = ">=7.4.4"
+pytest = ">=8.1.1"
+pytest-doctestplus = ">=1.2.1"
+pytest-sugar = ">=1.0.0"
+covdefaults = ">=2.3.0"
+poethepoet = ">=0.25.0"
+pre-commit = "<3.6.0"
+smokeshow = ">=0.4.0"
+keyring = ">=25.0.0"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules"
 
 
-
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 markdown-exec = ">=1.3.0"
 mkdocs-material = ">=8.2,<10.0.0"
 mkdocstrings = { version = ">=0.19.0", extras = ["python"] }
 
 [tool.poe.tasks]
 test = "pytest -v"
 lint = "ruff check ."
-skeleton = "scripts/skeleton.0.0.2rc-149-gaad3c42.bash"
+skeleton = "scripts/skeleton.0.0.2rc-215-g792492f.bash"
 check = [
     { ref="test" },
     { ref="lint" },
 ]
 release.script = "scripts.release:main"
 
 [tool.poe.tasks.added]
@@ -124,17 +124,14 @@
 
 [tool.ruff.lint.isort]
 required-imports = ["from __future__ import annotations"]
 
 [tool.mypy]
 strict = true
 
-[tool.isort]
-profile = "black"
-
 [tool.towncrier]
 directory = "news"
 package = "backframe"
 filename = "CHANGELOG.md"
 start_string = "<!-- insertion marker -->\n"
 underlines = ["", "", ""]  # We use Markdown
 title_format = "## [{version}](https://github.com/bswck/backframe/tree/{version}) ({project_date})"
```

### Comparing `backframe-0.1.1/PKG-INFO` & `backframe-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 Metadata-Version: 2.1
 Name: backframe
-Version: 0.1.1
+Version: 0.1.2
 Summary: Inspect the caller.
 Home-page: https://github.com/bswck/backframe
 License: MIT
 Author: bswck
-Author-email: bswck.dev@gmail.com
-Requires-Python: >=3.8,<4.0
+Author-email: bartoszpiotrslawecki@gmail.com
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Coverage, https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/backframe
 Project-URL: Documentation, https://backframe.readthedocs.io/en/latest/
 Project-URL: Distribution, https://pypi.org/project/backframe/
 Project-URL: Issues, https://github.com/bswck/backframe/issues
 Description-Content-Type: text/markdown
 
-# backframe [![skeleton](https://img.shields.io/badge/0.0.2rc–149–gaad3c42-skeleton?label=%F0%9F%92%80%20bswck/skeleton&labelColor=black&color=grey&link=https%3A//github.com/bswck/skeleton)](https://github.com/bswck/skeleton/tree/0.0.2rc-149-gaad3c42) [![Supported Python versions](https://img.shields.io/pypi/pyversions/backframe.svg?logo=python&label=Python)](https://pypi.org/project/backframe/) [![Package version](https://img.shields.io/pypi/v/backframe?label=PyPI)](https://pypi.org/project/backframe/)
+# <div align="center">backframe<br>[![skeleton](https://img.shields.io/badge/0.0.2rc–215–g792492f-skeleton?label=%F0%9F%92%80%20skeleton-ci/skeleton-python&labelColor=black&color=grey&link=https%3A//github.com/skeleton-ci/skeleton-python)](https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-215-g792492f) [![Supported Python versions](https://img.shields.io/pypi/pyversions/backframe.svg?logo=python&label=Python)](https://pypi.org/project/backframe/) [![Package version](https://img.shields.io/pypi/v/backframe?label=PyPI)](https://pypi.org/project/backframe/)</div>
 
 [![Tests](https://github.com/bswck/backframe/actions/workflows/test.yml/badge.svg)](https://github.com/bswck/backframe/actions/workflows/test.yml)
 [![Coverage](https://coverage-badge.samuelcolvin.workers.dev/bswck/backframe.svg)](https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/backframe)
 [![Documentation Status](https://readthedocs.org/projects/backframe/badge/?version=latest)](https://backframe.readthedocs.io/en/latest/?badge=latest)
 
-
-
 Inspect the caller.
 
 # Installation
 You might simply install it with pip:
 
 ```shell
 pip install backframe
@@ -39,22 +37,22 @@
 
 If you use [Poetry](https://python-poetry.org/), then you might want to run:
 
 ```shell
 poetry add backframe
 ```
 
-## For contributors
+## For Contributors
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 <!--
-This section was generated from bswck/skeleton@0.0.2rc-149-gaad3c42.
+This section was generated from skeleton-ci/skeleton-python@0.0.2rc-215-g792492f.
 Instead of changing this particular file, you might want to alter the template:
-https://github.com/bswck/skeleton/tree/0.0.2rc-149-gaad3c42/project/README.md.jinja
+https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-215-g792492f/project/README.md.jinja
 -->
 > [!Note]
 > If you use Windows, it is highly recommended to complete the installation in the way presented below through [WSL2](https://learn.microsoft.com/en-us/windows/wsl/install).
 1.  Fork the [backframe repository](https://github.com/bswck/backframe) on GitHub.
 
 1.  [Install Poetry](https://python-poetry.org/docs/#installation).<br/>
     Poetry is an amazing tool for managing dependencies & virtual environments, building packages and publishing them.
@@ -87,11 +85,11 @@
     poetry shell
     pre-commit install
     ```
 
 For more information on how to contribute, check out [CONTRIBUTING.md](https://github.com/bswck/backframe/blob/HEAD/CONTRIBUTING.md).<br/>
 Always happy to accept contributions! ❤️
 
-# Legal info
+# Legal Info
 © Copyright by Bartosz Sławecki ([@bswck](https://github.com/bswck)).
 <br />This software is licensed under the terms of [MIT License](https://github.com/bswck/backframe/blob/HEAD/LICENSE).
```

