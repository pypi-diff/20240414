# Comparing `tmp/runtime_generics-3.1.0.tar.gz` & `tmp/runtime_generics-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtime_generics-3.1.0.tar", max compression
+gzip compressed data, was "runtime_generics-3.2.0.tar", max compression
```

## Comparing `runtime_generics-3.1.0.tar` & `runtime_generics-3.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1092 2024-03-16 17:20:52.318019 runtime_generics-3.1.0/LICENSE
--rw-r--r--   0        0        0     8043 2024-03-16 17:20:52.318019 runtime_generics-3.1.0/README.md
--rw-r--r--   0        0        0     5367 2024-03-16 17:20:52.322019 runtime_generics-3.1.0/pyproject.toml
--rw-r--r--   0        0        0    22205 2024-03-16 17:20:52.322019 runtime_generics-3.1.0/runtime_generics/__init__.py
--rw-r--r--   0        0        0        0 2024-03-16 17:20:52.322019 runtime_generics-3.1.0/runtime_generics/py.typed
--rw-r--r--   0        0        0     9109 1970-01-01 00:00:00.000000 runtime_generics-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-04-14 00:43:43.672735 runtime_generics-3.2.0/LICENSE
+-rw-r--r--   0        0        0     8137 2024-04-14 00:43:43.672735 runtime_generics-3.2.0/README.md
+-rw-r--r--   0        0        0     5429 2024-04-14 00:43:43.676735 runtime_generics-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0    22205 2024-04-14 00:43:43.676735 runtime_generics-3.2.0/runtime_generics/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 00:43:43.676735 runtime_generics-3.2.0/runtime_generics/py.typed
+-rw-r--r--   0        0        0     9195 1970-01-01 00:00:00.000000 runtime_generics-3.2.0/PKG-INFO
```

### Comparing `runtime_generics-3.1.0/LICENSE` & `runtime_generics-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runtime_generics-3.1.0/README.md` & `runtime_generics-3.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# runtime_generics [![skeleton](https://img.shields.io/badge/0.0.2rc–180–g2a2d737-skeleton?label=%F0%9F%92%80%20bswck/skeleton&labelColor=black&color=grey&link=https%3A//github.com/bswck/skeleton)](https://github.com/bswck/skeleton/tree/0.0.2rc-180-g2a2d737) [![Supported Python versions](https://img.shields.io/pypi/pyversions/runtime-generics.svg?logo=python&label=Python)](https://pypi.org/project/runtime-generics/) [![Package version](https://img.shields.io/pypi/v/runtime-generics?label=PyPI)](https://pypi.org/project/runtime-generics/)
+# <div align="center">runtime_generics<br>[![skeleton](https://img.shields.io/badge/0.0.2rc–215–g792492f-skeleton?label=%F0%9F%92%80%20skeleton-ci/skeleton-python&labelColor=black&color=grey&link=https%3A//github.com/skeleton-ci/skeleton-python)](https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-215-g792492f) [![Supported Python versions](https://img.shields.io/pypi/pyversions/runtime-generics.svg?logo=python&label=Python)](https://pypi.org/project/runtime-generics/) [![Package version](https://img.shields.io/pypi/v/runtime-generics?label=PyPI)](https://pypi.org/project/runtime-generics/)</div>
 
 [![Tests](https://github.com/bswck/runtime_generics/actions/workflows/test.yml/badge.svg)](https://github.com/bswck/runtime_generics/actions/workflows/test.yml)
 [![Coverage](https://coverage-badge.samuelcolvin.workers.dev/bswck/runtime_generics.svg)](https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/runtime_generics)
 [![Documentation Status](https://readthedocs.org/projects/runtime-generics/badge/?version=latest)](https://runtime-generics.readthedocs.io/en/latest/?badge=latest)
 [![Lifted?](https://tidelift.com/badges/package/pypi/runtime-generics)](https://tidelift.com/subscription/pkg/pypi-runtime-generics?utm_source=pypi-runtime-generics&utm_medium=readme)
 
 Highly into type-safe Python code?
@@ -135,17 +135,17 @@
 ```
 
 ## For Contributors
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 <!--
-This section was generated from bswck/skeleton@0.0.2rc-180-g2a2d737.
+This section was generated from skeleton-ci/skeleton-python@0.0.2rc-215-g792492f.
 Instead of changing this particular file, you might want to alter the template:
-https://github.com/bswck/skeleton/tree/0.0.2rc-180-g2a2d737/project/README.md.jinja
+https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-215-g792492f/project/README.md.jinja
 -->
 > [!Note]
 > If you use Windows, it is highly recommended to complete the installation in the way presented below through [WSL2](https://learn.microsoft.com/en-us/windows/wsl/install).
 1.  Fork the [runtime_generics repository](https://github.com/bswck/runtime_generics) on GitHub.
 
 1.  [Install Poetry](https://python-poetry.org/docs/#installation).<br/>
     Poetry is an amazing tool for managing dependencies & virtual environments, building packages and publishing them.
```

### Comparing `runtime_generics-3.1.0/pyproject.toml` & `runtime_generics-3.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-# This file was generated from bswck/skeleton@0.0.2rc-180-g2a2d737.
+# This file was generated from skeleton-ci/skeleton-python@0.0.2rc-215-g792492f.
 # Instead of changing this particular file, you might want to alter the template:
-# https://github.com/bswck/skeleton/tree/0.0.2rc-180-g2a2d737/project/pyproject.toml.jinja
+# https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-215-g792492f/project/pyproject.toml.jinja
 
 [tool.poetry]
 name = "runtime_generics"
-version = "3.1.0"
+version = "3.2.0"
 description = "Reuse generic class type arguments at runtime."
-authors = ["bswck <bswck.dev@gmail.com>"]
+authors = ["bswck <bartoszpiotrslawecki@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "runtime_generics/" }]
 homepage = "https://github.com/bswck/runtime_generics"
 
 [tool.poetry.urls]
 Documentation = "https://runtime-generics.readthedocs.io/en/latest/"
 Issues = "https://github.com/bswck/runtime_generics/issues"
 Distribution = "https://pypi.org/project/runtime-generics/"
 Coverage = "https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/runtime_generics"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
-typing-extensions = "^4.9.0"
-backframe = "^0.1.1"
+python = ">=3.8"
+typing-extensions = ">=4.9.0"
+backframe = ">=0.1.2"
 
 [tool.poetry.group.dev.dependencies]
 
 [tool.poetry.group.dev-skeleton.dependencies]
-# This dependency group was generated from bswck/skeleton@0.0.2rc-180-g2a2d737.
+# This dependency group was generated from skeleton-ci/skeleton-python@0.0.2rc-215-g792492f.
 # Instead of changing this particular file, you might want to alter the template:
-# https://github.com/bswck/skeleton/tree/0.0.2rc-180-g2a2d737/project/pyproject.toml.jinja
-mypy = "^1.7.0"
-ruff = "^0.3.2"
-towncrier = "^23.11.0"
-coverage = "^7.4.2"
-pytest = "^8.0.1"
-pytest-doctestplus = "^1.1.0"
-covdefaults = "^2.3.0"
-poethepoet = "^0.24.3"
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
 pre-commit = "<3.6.0"
-smokeshow = "^0.4.0"
-keyring = "^24.3.0"
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
-skeleton = "scripts/skeleton.0.0.2rc-180-g2a2d737.bash"
+skeleton = "scripts/skeleton.0.0.2rc-215-g792492f.bash"
 check = [
     { ref="test" },
     { ref="lint" },
 ]
 release.script = "scripts.release:main"
 
 [tool.poe.tasks.added]
@@ -126,17 +126,14 @@
 
 [tool.ruff.lint.isort]
 required-imports = ["from __future__ import annotations"]
 
 [tool.mypy]
 strict = true
 
-[tool.isort]
-profile = "black"
-
 [tool.towncrier]
 directory = "news"
 package = "runtime_generics"
 filename = "CHANGELOG.md"
 start_string = "<!-- insertion marker -->\n"
 underlines = ["", "", ""]  # We use Markdown
 title_format = "## [{version}](https://github.com/bswck/runtime_generics/tree/{version}) ({project_date})"
```

### Comparing `runtime_generics-3.1.0/runtime_generics/__init__.py` & `runtime_generics-3.2.0/runtime_generics/__init__.py`

 * *Files identical despite different names*

### Comparing `runtime_generics-3.1.0/PKG-INFO` & `runtime_generics-3.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: runtime_generics
-Version: 3.1.0
+Version: 3.2.0
 Summary: Reuse generic class type arguments at runtime.
 Home-page: https://github.com/bswck/runtime_generics
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
-Requires-Dist: backframe (>=0.1.1,<0.2.0)
-Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
+Requires-Dist: backframe (>=0.1.2)
+Requires-Dist: typing-extensions (>=4.9.0)
 Project-URL: Coverage, https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/runtime_generics
 Project-URL: Documentation, https://runtime-generics.readthedocs.io/en/latest/
 Project-URL: Distribution, https://pypi.org/project/runtime-generics/
 Project-URL: Issues, https://github.com/bswck/runtime_generics/issues
 Description-Content-Type: text/markdown
 
-# runtime_generics [![skeleton](https://img.shields.io/badge/0.0.2rc–180–g2a2d737-skeleton?label=%F0%9F%92%80%20bswck/skeleton&labelColor=black&color=grey&link=https%3A//github.com/bswck/skeleton)](https://github.com/bswck/skeleton/tree/0.0.2rc-180-g2a2d737) [![Supported Python versions](https://img.shields.io/pypi/pyversions/runtime-generics.svg?logo=python&label=Python)](https://pypi.org/project/runtime-generics/) [![Package version](https://img.shields.io/pypi/v/runtime-generics?label=PyPI)](https://pypi.org/project/runtime-generics/)
+# <div align="center">runtime_generics<br>[![skeleton](https://img.shields.io/badge/0.0.2rc–215–g792492f-skeleton?label=%F0%9F%92%80%20skeleton-ci/skeleton-python&labelColor=black&color=grey&link=https%3A//github.com/skeleton-ci/skeleton-python)](https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-215-g792492f) [![Supported Python versions](https://img.shields.io/pypi/pyversions/runtime-generics.svg?logo=python&label=Python)](https://pypi.org/project/runtime-generics/) [![Package version](https://img.shields.io/pypi/v/runtime-generics?label=PyPI)](https://pypi.org/project/runtime-generics/)</div>
 
 [![Tests](https://github.com/bswck/runtime_generics/actions/workflows/test.yml/badge.svg)](https://github.com/bswck/runtime_generics/actions/workflows/test.yml)
 [![Coverage](https://coverage-badge.samuelcolvin.workers.dev/bswck/runtime_generics.svg)](https://coverage-badge.samuelcolvin.workers.dev/redirect/bswck/runtime_generics)
 [![Documentation Status](https://readthedocs.org/projects/runtime-generics/badge/?version=latest)](https://runtime-generics.readthedocs.io/en/latest/?badge=latest)
 [![Lifted?](https://tidelift.com/badges/package/pypi/runtime-generics)](https://tidelift.com/subscription/pkg/pypi-runtime-generics?utm_source=pypi-runtime-generics&utm_medium=readme)
 
 Highly into type-safe Python code?
@@ -159,17 +159,17 @@
 ```
 
 ## For Contributors
 [![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 <!--
-This section was generated from bswck/skeleton@0.0.2rc-180-g2a2d737.
+This section was generated from skeleton-ci/skeleton-python@0.0.2rc-215-g792492f.
 Instead of changing this particular file, you might want to alter the template:
-https://github.com/bswck/skeleton/tree/0.0.2rc-180-g2a2d737/project/README.md.jinja
+https://github.com/skeleton-ci/skeleton-python/tree/0.0.2rc-215-g792492f/project/README.md.jinja
 -->
 > [!Note]
 > If you use Windows, it is highly recommended to complete the installation in the way presented below through [WSL2](https://learn.microsoft.com/en-us/windows/wsl/install).
 1.  Fork the [runtime_generics repository](https://github.com/bswck/runtime_generics) on GitHub.
 
 1.  [Install Poetry](https://python-poetry.org/docs/#installation).<br/>
     Poetry is an amazing tool for managing dependencies & virtual environments, building packages and publishing them.
```

