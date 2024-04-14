# Comparing `tmp/anycorn-0.16.0.tar.gz` & `tmp/anycorn-0.17.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycorn-0.16.0.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `anycorn-0.16.0.tar` & `anycorn-0.17.0.tar`

### file list

```diff
@@ -1,33 +1,69 @@
--rw-r--r--   0        0        0     1050 2024-04-03 20:43:26.606098 anycorn-0.16.0/LICENSE
--rw-r--r--   0        0        0     3526 2024-04-03 20:43:26.606098 anycorn-0.16.0/README.rst
--rw-r--r--   0        0        0     3033 2024-04-03 20:43:26.610098 anycorn-0.16.0/pyproject.toml
--rw-r--r--   0        0        0     1589 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/__init__.py
--rw-r--r--   0        0        0    10586 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/__main__.py
--rw-r--r--   0        0        0     5504 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/app_wrappers.py
--rw-r--r--   0        0        0    13376 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/config.py
--rw-r--r--   0        0        0      383 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/events.py
--rw-r--r--   0        0        0     3543 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/lifespan.py
--rw-r--r--   0        0        0     7381 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/logging.py
--rw-r--r--   0        0        0      341 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/middleware/__init__.py
--rw-r--r--   0        0        0     2630 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/middleware/dispatcher.py
--rw-r--r--   0        0        0     2619 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/middleware/http_to_https.py
--rw-r--r--   0        0        0     2693 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/middleware/proxy_fix.py
--rw-r--r--   0        0        0      997 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/middleware/wsgi.py
--rwxr-xr-x   0        0        0     2808 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/protocol/__init__.py
--rw-r--r--   0        0        0     1013 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/protocol/events.py
--rwxr-xr-x   0        0        0    11657 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/protocol/h11.py
--rwxr-xr-x   0        0        0    15015 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/protocol/h2.py
--rw-r--r--   0        0        0     5358 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/protocol/h3.py
--rw-r--r--   0        0        0     7946 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/protocol/http_stream.py
--rw-r--r--   0        0        0     5097 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/protocol/quic.py
--rw-r--r--   0        0        0    14943 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/protocol/ws_stream.py
--rw-r--r--   0        0        0        7 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/py.typed
--rw-r--r--   0        0        0     9085 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/run.py
--rw-r--r--   0        0        0     4246 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/statsd.py
--rw-r--r--   0        0        0     2502 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/task_group.py
--rw-r--r--   0        0        0     5458 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/tcp_server.py
--rw-r--r--   0        0        0     7210 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/typing.py
--rw-r--r--   0        0        0     1481 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/udp_server.py
--rw-r--r--   0        0        0     6506 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/utils.py
--rw-r--r--   0        0        0     1165 2024-04-03 20:43:26.610098 anycorn-0.16.0/src/anycorn/worker_context.py
--rw-r--r--   0        0        0     5298 1970-01-01 00:00:00.000000 anycorn-0.16.0/PKG-INFO
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 anycorn-0.17.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 anycorn-0.17.0/.readthedocs.yaml
+-rw-r--r--   0        0        0    20871 2020-02-02 00:00:00.000000 anycorn-0.17.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     3096 2020-02-02 00:00:00.000000 anycorn-0.17.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 anycorn-0.17.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 anycorn-0.17.0/compliance/autobahn/fuzzingclient.json
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 anycorn-0.17.0/compliance/autobahn/summarise.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 anycorn-0.17.0/compliance/autobahn/ws_server.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 anycorn-0.17.0/compliance/h2spec/cert.pem
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 anycorn-0.17.0/compliance/h2spec/http_server.py
+-rw-r--r--   0        0        0     3272 2020-02-02 00:00:00.000000 anycorn-0.17.0/compliance/h2spec/key.pem
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/__init__.py
+-rw-r--r--   0        0        0    10592 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/__main__.py
+-rw-r--r--   0        0        0     5520 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/app_wrappers.py
+-rw-r--r--   0        0        0    13238 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/config.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/events.py
+-rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/lifespan.py
+-rw-r--r--   0        0        0     7344 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/logging.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/py.typed
+-rw-r--r--   0        0        0     9348 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/run.py
+-rw-r--r--   0        0        0     4408 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/statsd.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/task_group.py
+-rw-r--r--   0        0        0     5747 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/tcp_server.py
+-rw-r--r--   0        0        0     7128 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/typing.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/udp_server.py
+-rw-r--r--   0        0        0     6469 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/utils.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/worker_context.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/middleware/__init__.py
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/middleware/dispatcher.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/middleware/http_to_https.py
+-rw-r--r--   0        0        0     2664 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/middleware/proxy_fix.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/middleware/wsgi.py
+-rwxr-xr-x   0        0        0     2769 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/protocol/__init__.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/protocol/events.py
+-rwxr-xr-x   0        0        0    11624 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/protocol/h11.py
+-rwxr-xr-x   0        0        0    14996 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/protocol/h2.py
+-rw-r--r--   0        0        0     5334 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/protocol/h3.py
+-rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/protocol/http_stream.py
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/protocol/quic.py
+-rw-r--r--   0        0        0    14902 2020-02-02 00:00:00.000000 anycorn-0.17.0/src/anycorn/protocol/ws_stream.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/__init__.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/conftest.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/helpers.py
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/test___main__.py
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/test_app_wrappers.py
+-rw-r--r--   0        0        0     5800 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/test_config.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/test_keep_alive.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/test_lifespan.py
+-rw-r--r--   0        0        0     4030 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/test_logging.py
+-rw-r--r--   0        0        0     8390 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/test_sanity.py
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/test_utils.py
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/assets/cert.pem
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/assets/config.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/assets/config.toml
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/assets/config_ssl.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/assets/key.pem
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/middleware/__init__.py
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/middleware/test_dispatcher.py
+-rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/middleware/test_http_to_https.py
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/middleware/test_proxy_fix.py
+-rwxr-xr-x   0        0        0    15366 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/protocol/test_h11.py
+-rw-r--r--   0        0        0     3542 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/protocol/test_h2.py
+-rw-r--r--   0        0        0     9873 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/protocol/test_http_stream.py
+-rw-r--r--   0        0        0    17121 2020-02-02 00:00:00.000000 anycorn-0.17.0/tests/protocol/test_ws_stream.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 anycorn-0.17.0/.gitignore
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 anycorn-0.17.0/LICENSE
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 anycorn-0.17.0/README.md
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 anycorn-0.17.0/pyproject.toml
+-rw-r--r--   0        0        0     2449 2020-02-02 00:00:00.000000 anycorn-0.17.0/PKG-INFO
```

### Comparing `anycorn-0.16.0/LICENSE` & `anycorn-0.17.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anycorn-0.16.0/pyproject.toml` & `anycorn-0.17.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,20 @@
-[tool.poetry]
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
 name = "anycorn"
-version = "0.16.0"
-description = "A ASGI Server based on Hyper libraries and inspired by Gunicorn"
-authors = ["pgjones <philip.graham.jones@googlemail.com>", "David Brochart <david.brochart@gmail.com>"]
+dynamic = ["version"]
+requires-python = ">=3.8"
+description = "A fork of Hypercorn that uses AnyIO"
+authors = [
+    { name = "Philip Graham Jones", email = "philip.graham.jones@googlemail.com" },
+    { name = "David Brochart", email = "david.brochart@gmail.com" },
+]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
@@ -17,64 +25,41 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = ["src/anycorn/py.typed"]
 license = "MIT"
-readme = "README.rst"
+readme = "README.md"
 repository = "https://github.com/davidbrochart/anycorn/"
-documentation = "https://hypercorn.readthedocs.io"
-
-[tool.poetry.dependencies]
-python = ">=3.8"
-aioquic = { version = ">= 0.9.0, < 1.0", optional = true }
-exceptiongroup = ">= 1.1.0"
-h11 = "*"
-h2 = ">=3.1.0"
-anyio = ">=4.0, <5.0"
-priority = "*"
-pydata_sphinx_theme = { version = "*", optional = true }
-sphinxcontrib_mermaid = { version = "*", optional = true }
-taskgroup = { version = "*", python = "<3.11", allow-prereleases = true }
-tomli = { version = "*", python = "<3.11" }
-uvloop = { version = "*", markers = "platform_system != 'Windows'", optional = true }
-wsproto = ">=0.14.0"
-
-[tool.poetry.dev-dependencies]
-hypothesis = "*"
-mock = "*"
-pytest = "*"
-pytest-asyncio = "*"
-pytest-trio = "*"
-trio = "*"
 
-[tool.poetry.scripts]
-anycorn = "anycorn.__main__:main"
-
-[tool.poetry.extras]
-docs = ["pydata_sphinx_theme", "sphinxcontrib_mermaid"]
-h3 = ["aioquic"]
-trio = ["exceptiongroup", "trio"]
-uvloop = ["uvloop"]
+dependencies = [
+    "exceptiongroup >= 1.2.0, <2.0; python_version<'3.11'",
+    "h11",
+    "h2 >=3.1.0",
+    "anyio >=4.0, <5.0",
+    "priority",
+    "taskgroup >=0.0.0a4; python_version<'3.11'",
+    "tomli; python_version<'3.11'",
+    "wsproto >=0.14.0",
+]
 
-[tool.black]
-line-length = 100
-target-version = ["py38"]
+[project.optional-dependencies]
+h3 = [
+    "aioquic >= 0.9.0, < 1.0",
+]
+test = [
+    "pytest",
+    "mock",
+    "trio",
+    "mypy",
+]
 
-[tool.isort]
-combine_as_imports = true
-force_grid_wrap = 0
-include_trailing_comma = true
-known_first_party = "anycorn, tests"
-line_length = 100
-multi_line_output = 3
-no_lines_before = "LOCALFOLDER"
-order_by_type = false
-reverse_relative = true
+[project.scripts]
+anycorn = "anycorn.__main__:main"
 
 [tool.mypy]
 allow_redefinition = true
 disallow_any_generics = false
 disallow_subclassing_any = true
 disallow_untyped_calls = false
 disallow_untyped_defs = true
@@ -86,18 +71,29 @@
 strict_optional = false
 warn_redundant_casts = true
 warn_return_any = false
 warn_unused_configs = true
 warn_unused_ignores = true
 
 [[tool.mypy.overrides]]
-module =["aioquic.*", "cryptography.*", "h11.*", "h2.*", "priority.*", "pytest_asyncio.*", "trio.*", "uvloop.*"]
+module =["aioquic.*", "cryptography.*", "h11.*", "h2.*", "priority.*", "trio.*"]
 ignore_missing_imports = true
 
 [tool.pytest.ini_options]
-addopts = "--no-cov-on-fail --showlocals --strict-markers"
-asyncio_mode = "strict"
+addopts = "--showlocals --strict-markers --color=yes -v"
 testpaths = ["tests"]
 
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+[tool.ruff]
+line-length = 100
+lint.select = [
+    "ASYNC",        # flake8-async
+    "E", "F", "W",  # default Flake8
+    "G",            # flake8-logging-format
+    "I",            # isort
+    "ISC",          # flake8-implicit-str-concat
+    "PGH",          # pygrep-hooks
+    "RUF100",       # unused noqa (yesqa)
+    "UP",           # pyupgrade
+]
+
+[tool.hatch.version]
+path = "src/anycorn/__init__.py"
```

### Comparing `anycorn-0.16.0/src/anycorn/__init__.py` & `anycorn-0.17.0/src/anycorn/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from __future__ import annotations
 
 import warnings
-from typing import Awaitable, Callable, Literal, Optional
+from typing import Awaitable, Callable, Literal
 
 import anyio
 
 from .config import Config
 from .run import worker_serve
 from .typing import Framework
 from .utils import wrap_app
 
 __all__ = ("Config", "serve")
+__version__ = "0.17.0"
 
 
 async def serve(
     app: Framework,
     config: Config,
     *,
-    shutdown_trigger: Optional[Callable[..., Awaitable[None]]] = None,
-    task_status: anyio.abc.TaskStatus[None] = anyio.TASK_STATUS_IGNORED,
-    mode: Optional[Literal["asgi", "wsgi"]] = None,
+    shutdown_trigger: Callable[..., Awaitable[None]] | None = None,
+    task_status: anyio.abc.TaskStatus[list[str]] = anyio.TASK_STATUS_IGNORED,
+    mode: Literal["asgi", "wsgi"] | None = None,
 ) -> None:
     """Serve an ASGI framework app given the config.
 
     This allows for a programmatic way to serve an ASGI framework, it
     can be used via,
 
     .. code-block:: python
```

### Comparing `anycorn-0.16.0/src/anycorn/__main__.py` & `anycorn-0.17.0/src/anycorn/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 from __future__ import annotations
 
 import argparse
 import ssl
 import sys
 import warnings
-from typing import List, Optional
 
 from .config import Config
 from .run import run
 
 sentinel = object()
 
 
-def _load_config(config_path: Optional[str]) -> Config:
+def _load_config(config_path: str | None) -> Config:
     if config_path is None:
         return Config()
     elif config_path.startswith("python:"):
         return Config.from_object(config_path[len("python:") :])
     elif config_path.startswith("file:"):
         return Config.from_pyfile(config_path[len("file:") :])
     else:
         return Config.from_toml(config_path)
 
 
-def main(sys_args: Optional[List[str]] = None) -> int:
+def main(sys_args: list[str] | None = None) -> int:
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "application", help="The application to dispatch to as path.to.module:instance.path"
     )
     parser.add_argument("--access-log", help="Deprecated, see access-logfile", default=sentinel)
     parser.add_argument(
         "--access-logfile",
@@ -133,23 +132,24 @@
     )
     parser.add_argument(
         "--log-level", help="The (error) log level, defaults to info", default=sentinel
     )
     parser.add_argument(
         "-p", "--pid", help="Location to write the PID (Program ID) to.", default=sentinel
     )
-    parser.add_argument(
-        "--quic-bind",
-        dest="quic_binds",
-        help="""The UDP/QUIC host/address to bind to. See *bind* for formatting
-        options.
-        """,
-        default=[],
-        action="append",
-    )
+    # FIXME
+    # parser.add_argument(
+    #     "--quic-bind",
+    #     dest="quic_binds",
+    #     help="""The UDP/QUIC host/address to bind to. See *bind* for formatting
+    #     options.
+    #     """,
+    #     default=[],
+    #     action="append",
+    # )
     parser.add_argument(
         "--reload",
         help="Enable automatic reloads on code changes",
         action="store_true",
         default=sentinel,
     )
     parser.add_argument(
@@ -281,16 +281,17 @@
     if args.workers is not sentinel:
         config.workers = args.workers
 
     if len(args.binds) > 0:
         config.bind = args.binds
     if len(args.insecure_binds) > 0:
         config.insecure_bind = args.insecure_binds
-    if len(args.quic_binds) > 0:
-        config.quic_bind = args.quic_binds
+    # FIXME
+    # if len(args.quic_binds) > 0:
+    #     config.quic_bind = args.quic_binds
     if len(args.server_names) > 0:
         config.server_names = args.server_names
 
     return run(config)
 
 
 if __name__ == "__main__":
```

### Comparing `anycorn-0.16.0/src/anycorn/app_wrappers.py` & `anycorn-0.17.0/src/anycorn/app_wrappers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import sys
 from functools import partial
 from io import BytesIO
-from typing import Callable, List, Optional, Tuple
+from typing import Callable
 
 from .typing import (
     ASGIFramework,
     ASGIReceiveCallable,
     ASGISendCallable,
     HTTPScope,
     Scope,
@@ -46,15 +46,15 @@
         send: ASGISendCallable,
         sync_spawn: Callable,
         call_soon: Callable,
     ) -> None:
         if scope["type"] == "http":
             await self.handle_http(scope, receive, send, sync_spawn, call_soon)
         elif scope["type"] == "websocket":
-            await send({"type": "websocket.close"})  # type: ignore
+            await send({"type": "websocket.close"})  # type: ignore[arg-type, misc]
         elif scope["type"] == "lifespan":
             return
         else:
             raise Exception(f"Unknown scope type, {scope['type']}")
 
     async def handle_http(
         self,
@@ -63,15 +63,15 @@
         send: ASGISendCallable,
         sync_spawn: Callable,
         call_soon: Callable,
     ) -> None:
         body = bytearray()
         while True:
             message = await receive()
-            body.extend(message.get("body", b""))  # type: ignore
+            body.extend(message.get("body", b""))  # type: ignore[arg-type]
             if len(body) > self.max_body_size:
                 await send({"type": "http.response.start", "status": 400, "headers": []})
                 await send({"type": "http.response.body", "body": b"", "more_body": False})
                 return
             if not message.get("more_body"):
                 break
 
@@ -80,30 +80,30 @@
         except InvalidPathError:
             await send({"type": "http.response.start", "status": 404, "headers": []})
         else:
             await sync_spawn(self.run_app, environ, partial(call_soon, send))
         await send({"type": "http.response.body", "body": b"", "more_body": False})
 
     def run_app(self, environ: dict, send: Callable) -> None:
-        headers: List[Tuple[bytes, bytes]]
+        headers: list[tuple[bytes, bytes]] = []
         headers_sent = False
         response_started = False
-        status_code: Optional[int] = None
+        status_code: int | None = None
 
         def start_response(
             status: str,
-            response_headers: List[Tuple[str, str]],
-            exc_info: Optional[Exception] = None,
+            response_headers: list[tuple[str, str]],
+            exc_info: Exception | None = None,
         ) -> None:
             nonlocal headers, response_started, status_code
 
             raw, _ = status.split(" ", 1)
             status_code = int(raw)
             headers = [
-                (name.lower().encode("ascii"), value.encode("ascii"))
+                (name.lower().encode("latin-1"), value.encode("latin-1"))
                 for name, value in response_headers
             ]
             response_started = True
 
         response_body = self.app(environ, start_response)
 
         if not response_started:
@@ -158,10 +158,10 @@
         elif name == "content-type":
             corrected_name = "CONTENT_TYPE"
         else:
             corrected_name = "HTTP_%s" % name.upper().replace("-", "_")
         # HTTPbis say only ASCII chars are allowed in headers, but we latin1 just in case
         value = raw_value.decode("latin1")
         if corrected_name in environ:
-            value = environ[corrected_name] + "," + value  # type: ignore
+            value = environ[corrected_name] + "," + value  # type: ignore[operator]
         environ[corrected_name] = value
     return environ
```

### Comparing `anycorn-0.16.0/src/anycorn/config.py` & `anycorn-0.17.0/src/anycorn/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 import socket
 import stat
 import sys
 import types
 import warnings
 from dataclasses import dataclass
 from ssl import (
-    create_default_context,
     OP_NO_COMPRESSION,
     Purpose,
     SSLContext,
     TLSVersion,
     VerifyFlags,
     VerifyMode,
+    create_default_context,
 )
 from time import time
-from typing import Any, AnyStr, Dict, List, Mapping, Optional, Tuple, Type, Union
+from typing import Any, AnyStr, Mapping, Union
 from wsgiref.handlers import format_date_time
 
 if sys.version_info >= (3, 11):
     import tomllib
 else:
     import tomli as tomllib
 
@@ -36,82 +36,82 @@
 
 FilePath = Union[AnyStr, os.PathLike]
 SocketKind = Union[int, socket.SocketKind]
 
 
 @dataclass
 class Sockets:
-    secure_sockets: List[socket.socket]
-    insecure_sockets: List[socket.socket]
-    quic_sockets: List[socket.socket]
+    secure_sockets: list[socket.socket]
+    insecure_sockets: list[socket.socket]
+    quic_sockets: list[socket.socket]
 
 
 class SocketTypeError(Exception):
     def __init__(self, expected: SocketKind, actual: SocketKind) -> None:
         super().__init__(
             f'Unexpected socket type, wanted "{socket.SocketKind(expected)}" got '
             f'"{socket.SocketKind(actual)}"'
         )
 
 
 class Config:
     _bind = ["127.0.0.1:8000"]
-    _insecure_bind: List[str] = []
-    _quic_bind: List[str] = []
-    _quic_addresses: List[Tuple] = []
-    _log: Optional[Logger] = None
+    _insecure_bind: list[str] = []
+    _quic_bind: list[str] = []
+    _quic_addresses: list[tuple] = []
+    _log: Logger | None = None
     _root_path: str = ""
 
     access_log_format = '%(h)s %(l)s %(l)s %(t)s "%(r)s" %(s)s %(b)s "%(f)s" "%(a)s"'
-    accesslog: Union[logging.Logger, str, None] = None
+    accesslog: logging.Logger | str | None = None
     alpn_protocols = ["h2", "http/1.1"]
-    alt_svc_headers: List[str] = []
+    alt_svc_headers: list[str] = []
     application_path: str
     backlog = 100
-    ca_certs: Optional[str] = None
-    certfile: Optional[str] = None
+    ca_certs: str | None = None
+    certfile: str | None = None
     ciphers: str = "ECDHE+AESGCM"
     debug = False
     dogstatsd_tags = ""
-    errorlog: Union[logging.Logger, str, None] = "-"
+    errorlog: logging.Logger | str | None = "-"
     graceful_timeout: float = 3 * SECONDS
-    read_timeout: Optional[int] = None
-    group: Optional[int] = None
+    read_timeout: int | None = None
+    group: int | None = None
     h11_max_incomplete_size = 16 * 1024 * BYTES
     h11_pass_raw_headers = False
     h2_max_concurrent_streams = 100
     h2_max_header_list_size = 2**16
     h2_max_inbound_frame_size = 2**14 * OCTETS
     include_date_header = True
     include_server_header = True
     keep_alive_timeout = 5 * SECONDS
     keep_alive_max_requests = 1000
-    keyfile: Optional[str] = None
-    keyfile_password: Optional[str] = None
-    logconfig: Optional[str] = None
-    logconfig_dict: Optional[dict] = None
+    keyfile: str | None = None
+    keyfile_password: str | None = None
+    logconfig: str | None = None
+    logconfig_dict: dict | None = None
     logger_class = Logger
     loglevel: str = "INFO"
     max_app_queue_size: int = 10
-    max_requests: Optional[int] = None
+    max_requests: int | None = None
     max_requests_jitter: int = 0
-    pid_path: Optional[str] = None
-    server_names: List[str] = []
+    pid_path: str | None = None
+    server_names: list[str] = []
     shutdown_timeout = 60 * SECONDS
     ssl_handshake_timeout = 60 * SECONDS
     startup_timeout = 60 * SECONDS
-    statsd_host: Optional[str] = None
+    statsd_host: str | None = None
     statsd_prefix = ""
-    umask: Optional[int] = None
+    umask: int | None = None
     use_reloader = False
-    user: Optional[int] = None
-    verify_flags: Optional[VerifyFlags] = None
-    verify_mode: Optional[VerifyMode] = None
+    user: int | None = None
+    verify_flags: VerifyFlags | None = None
+    verify_mode: VerifyMode | None = None
     websocket_max_message_size = 16 * 1024 * 1024 * BYTES
-    websocket_ping_interval: Optional[float] = None
+    websocket_ping_interval: float | None = None
     workers = 1
     wsgi_max_body_size = 16 * 1024 * 1024 * BYTES
 
     def set_cert_reqs(self, value: int) -> None:
         warnings.warn("Please use verify_mode instead", Warning)
         self.verify_mode = VerifyMode(value)
 
@@ -120,55 +120,55 @@
     @property
     def log(self) -> Logger:
         if self._log is None:
             self._log = self.logger_class(self)
         return self._log
 
     @property
-    def bind(self) -> List[str]:
+    def bind(self) -> list[str]:
         return self._bind
 
     @bind.setter
-    def bind(self, value: Union[List[str], str]) -> None:
+    def bind(self, value: list[str] | str) -> None:
         if isinstance(value, str):
             self._bind = [value]
         else:
             self._bind = value
 
     @property
-    def insecure_bind(self) -> List[str]:
+    def insecure_bind(self) -> list[str]:
         return self._insecure_bind
 
     @insecure_bind.setter
-    def insecure_bind(self, value: Union[List[str], str]) -> None:
+    def insecure_bind(self, value: list[str] | str) -> None:
         if isinstance(value, str):
             self._insecure_bind = [value]
         else:
             self._insecure_bind = value
 
     @property
-    def quic_bind(self) -> List[str]:
+    def quic_bind(self) -> list[str]:
         return self._quic_bind
 
     @quic_bind.setter
-    def quic_bind(self, value: Union[List[str], str]) -> None:
+    def quic_bind(self, value: list[str] | str) -> None:
         if isinstance(value, str):
             self._quic_bind = [value]
         else:
             self._quic_bind = value
 
     @property
     def root_path(self) -> str:
         return self._root_path
 
     @root_path.setter
     def root_path(self, value: str) -> None:
         self._root_path = value.rstrip("/")
 
-    def create_ssl_context(self) -> Optional[SSLContext]:
+    def create_ssl_context(self) -> SSLContext | None:
         if not self.ssl_enabled:
             return None
 
         context = create_default_context(Purpose.CLIENT_AUTH)
         context.set_ciphers(self.ciphers)
         context.minimum_version = TLSVersion.TLSv1_2  # RFC 7540 Section 9.2: MUST be TLS >=1.2
         context.options = OP_NO_COMPRESSION  # RFC 7540 Section 9.2.1: MUST disable compression
@@ -202,30 +202,30 @@
             self._set_quic_addresses(quic_sockets)
         else:
             secure_sockets = []
             insecure_sockets = self._create_sockets(self.bind)
             quic_sockets = []
         return Sockets(secure_sockets, insecure_sockets, quic_sockets)
 
-    def _set_quic_addresses(self, sockets: List[socket.socket]) -> None:
+    def _set_quic_addresses(self, sockets: list[socket.socket]) -> None:
         self._quic_addresses = []
         for sock in sockets:
             name = sock.getsockname()
-            if type(name) is not str and len(name) >= 2:
+            if not isinstance(name, str) and len(name) >= 2:
                 self._quic_addresses.append(name)
             else:
                 warnings.warn(
                     f'Cannot create a alt-svc header for the QUIC socket with address "{name}"',
                     Warning,
                 )
 
     def _create_sockets(
-        self, binds: List[str], type_: int = socket.SOCK_STREAM
-    ) -> List[socket.socket]:
-        sockets: List[socket.socket] = []
+        self, binds: list[str], type_: int = socket.SOCK_STREAM
+    ) -> list[socket.socket]:
+        sockets: list[socket.socket] = []
         for bind in binds:
             binding: Any = None
             if bind.startswith("unix:"):
                 sock = socket.socket(socket.AF_UNIX, type_)
                 binding = bind[5:]
                 try:
                     if stat.S_ISSOCK(os.stat(binding).st_mode):
@@ -271,15 +271,15 @@
             try:
                 sock.set_inheritable(True)
             except AttributeError:
                 pass
             sockets.append(sock)
         return sockets
 
-    def response_headers(self, protocol: str) -> List[Tuple[bytes, bytes]]:
+    def response_headers(self, protocol: str) -> list[tuple[bytes, bytes]]:
         headers = []
         if self.include_date_header:
             headers.append((b"date", format_date_time(time()).encode("ascii")))
         if self.include_server_header:
             headers.append((b"server", f"anycorn-{protocol}".encode("ascii")))
 
         for alt_svc_header in self.alt_svc_headers:
@@ -290,22 +290,22 @@
             for version in H3_ALPN:
                 for addr in self._quic_addresses:
                     port = addr[1]
                     headers.append((b"alt-svc", b'%s=":%d"; ma=3600' % (version.encode(), port)))
 
         return headers
 
-    def set_statsd_logger_class(self, statsd_logger: Type[Logger]) -> None:
+    def set_statsd_logger_class(self, statsd_logger: type[Logger]) -> None:
         if self.logger_class == Logger and self.statsd_host is not None:
             self.logger_class = statsd_logger
 
     @classmethod
     def from_mapping(
-        cls: Type["Config"], mapping: Optional[Mapping[str, Any]] = None, **kwargs: Any
-    ) -> "Config":
+        cls: type[Config], mapping: Mapping[str, Any] | None = None, **kwargs: Any
+    ) -> Config:
         """Create a configuration from a mapping.
 
         This allows either a mapping to be directly passed or as
         keyword arguments, for example,
 
         .. code-block:: python
 
@@ -314,29 +314,29 @@
             Config.from_mapping(keep_alive_timeout=10)
 
         Arguments:
             mapping: Optionally a mapping object.
             kwargs: Optionally a collection of keyword arguments to
                 form a mapping.
         """
-        mappings: Dict[str, Any] = {}
+        mappings: dict[str, Any] = {}
         if mapping is not None:
             mappings.update(mapping)
         mappings.update(kwargs)
         config = cls()
         for key, value in mappings.items():
             try:
                 setattr(config, key, value)
             except AttributeError:
                 pass
 
         return config
 
     @classmethod
-    def from_pyfile(cls: Type["Config"], filename: FilePath) -> "Config":
+    def from_pyfile(cls: type[Config], filename: FilePath) -> Config:
         """Create a configuration from a Python file.
 
         .. code-block:: python
 
             Config.from_pyfile('anycorn_config.py')
 
         Arguments:
@@ -345,15 +345,15 @@
         file_path = os.fspath(filename)
         spec = importlib.util.spec_from_file_location("module.name", file_path)
         module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(module)
         return cls.from_object(module)
 
     @classmethod
-    def from_toml(cls: Type["Config"], filename: FilePath) -> "Config":
+    def from_toml(cls: type[Config], filename: FilePath) -> Config:
         """Load the configuration values from a TOML formatted file.
 
         This allows configuration to be loaded as so
 
         .. code-block:: python
 
             Config.from_toml('config.toml')
@@ -363,15 +363,15 @@
         """
         file_path = os.fspath(filename)
         with open(file_path, "rb") as file_:
             data = tomllib.load(file_)
         return cls.from_mapping(data)
 
     @classmethod
-    def from_object(cls: Type["Config"], instance: Union[object, str]) -> "Config":
+    def from_object(cls: type[Config], instance: object | str) -> Config:
         """Create a configuration from a Python object.
 
         This can be used to reference modules or objects within
         modules for example,
 
         .. code-block:: python
```

### Comparing `anycorn-0.16.0/src/anycorn/lifespan.py` & `anycorn-0.17.0/src/anycorn/lifespan.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 
 class Lifespan:
     def __init__(self, app: AppWrapper, config: Config) -> None:
         self.app = app
         self.config = config
         self.startup = anyio.Event()
         self.shutdown = anyio.Event()
-        self.app_send_channel, self.app_receive_channel = anyio.create_memory_object_stream[dict[str, str]](
-            config.max_app_queue_size
-        )
+        self.app_send_channel, self.app_receive_channel = anyio.create_memory_object_stream[
+            ASGIReceiveEvent
+        ](config.max_app_queue_size)
         self.supported = True
 
     async def handle_lifespan(
         self, *, task_status: anyio.abc.TaskStatus[None] = anyio.TASK_STATUS_IGNORED
     ) -> None:
         task_status.started()
         scope: LifespanScope = {
```

### Comparing `anycorn-0.16.0/src/anycorn/logging.py` & `anycorn-0.17.0/src/anycorn/logging.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,42 +3,42 @@
 import json
 import logging
 import os
 import sys
 import time
 from http import HTTPStatus
 from logging.config import dictConfig, fileConfig
-from typing import Any, IO, Mapping, Optional, TYPE_CHECKING, Union
+from typing import IO, TYPE_CHECKING, Any, Mapping
 
 if sys.version_info >= (3, 11):
     import tomllib
 else:
     import tomli as tomllib
 
 
 if TYPE_CHECKING:
     from .config import Config
     from .typing import ResponseSummary, WWWScope
 
 
 def _create_logger(
     name: str,
-    target: Union[logging.Logger, str, None],
-    level: Optional[str],
+    target: logging.Logger | str | None,
+    level: str | None,
     sys_default: IO,
     *,
     propagate: bool = True,
-) -> Optional[logging.Logger]:
+) -> logging.Logger | None:
     if isinstance(target, logging.Logger):
         return target
 
     if target:
         logger = logging.getLogger(name)
         logger.handlers = [
-            logging.StreamHandler(sys_default) if target == "-" else logging.FileHandler(target)  # type: ignore # noqa: E501
+            logging.StreamHandler(sys_default) if target == "-" else logging.FileHandler(target)  # type: ignore[list-item]
         ]
         logger.propagate = propagate
         formatter = logging.Formatter(
             "%(asctime)s [%(process)d] [%(levelname)s] %(message)s",
             "[%Y-%m-%d %H:%M:%S %z]",
         )
         logger.handlers[0].setFormatter(formatter)
@@ -46,15 +46,15 @@
             logger.setLevel(logging.getLevelName(level.upper()))
         return logger
     else:
         return None
 
 
 class Logger:
-    def __init__(self, config: "Config") -> None:
+    def __init__(self, config: Config) -> None:
         self.access_log_format = config.access_log_format
 
         self.access_logger = _create_logger(
             "anycorn.access",
             config.accesslog,
             config.loglevel,
             sys.stdout,
@@ -78,15 +78,15 @@
                 }
                 fileConfig(config.logconfig, defaults=log_config, disable_existing_loggers=False)
         else:
             if config.logconfig_dict is not None:
                 dictConfig(config.logconfig_dict)
 
     async def access(
-        self, request: "WWWScope", response: "ResponseSummary", request_time: float
+        self, request: WWWScope, response: ResponseSummary, request_time: float
     ) -> None:
         if self.access_logger is not None:
             self.access_logger.info(
                 self.access_log_format, self.atoms(request, response, request_time)
             )
 
     async def critical(self, message: str, *args: Any, **kwargs: Any) -> None:
@@ -114,30 +114,30 @@
             self.error_logger.exception(message, *args, **kwargs)
 
     async def log(self, level: int, message: str, *args: Any, **kwargs: Any) -> None:
         if self.error_logger is not None:
             self.error_logger.log(level, message, *args, **kwargs)
 
     def atoms(
-        self, request: "WWWScope", response: Optional["ResponseSummary"], request_time: float
+        self, request: WWWScope, response: ResponseSummary | None, request_time: float
     ) -> Mapping[str, str]:
         """Create and return an access log atoms dictionary.
 
         This can be overidden and customised if desired. It should
         return a mapping between an access log format key and a value.
         """
         return AccessLogAtoms(request, response, request_time)
 
     def __getattr__(self, name: str) -> Any:
         return getattr(self.error_logger, name)
 
 
 class AccessLogAtoms(dict):
     def __init__(
-        self, request: "WWWScope", response: Optional["ResponseSummary"], request_time: float
+        self, request: WWWScope, response: ResponseSummary | None, request_time: float
     ) -> None:
         for name, value in request["headers"]:
             self[f"{{{name.decode('latin1').lower()}}}i"] = value.decode("latin1")
         for name, value in os.environ.items():
             self[f"{{{name.lower()}}}e"] = value
         protocol = request.get("http_version", "ws")
         client = request.get("client")
@@ -155,16 +155,16 @@
             method = "GET"
         query_string = request["query_string"].decode()
         path_with_qs = request["path"] + ("?" + query_string if query_string else "")
 
         status_code = "-"
         status_phrase = "-"
         if response is not None:
-            for name, value in response.get("headers", []):  # type: ignore
-                self[f"{{{name.decode('latin1').lower()}}}o"] = value.decode("latin1")  # type: ignore # noqa: E501
+            for name, value in response.get("headers", []):  # type: ignore[assignment]
+                self[f"{{{name.decode('latin1').lower()}}}o"] = value.decode("latin1")  # type: ignore[attr-defined]
             status_code = str(response["status"])
             try:
                 status_phrase = HTTPStatus(response["status"]).phrase
             except ValueError:
                 status_phrase = f"<???{status_code}???>"
         self.update(
             {
```

### Comparing `anycorn-0.16.0/src/anycorn/middleware/dispatcher.py` & `anycorn-0.17.0/src/anycorn/middleware/dispatcher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from __future__ import annotations
 
 from functools import partial
-from typing import Callable, Dict
+from typing import Any, Callable, Dict
 
 from ..typing import ASGIFramework, Scope
 
 MAX_QUEUE_SIZE = 10
 
 
 class _DispatcherMiddleware:
-    def __init__(self, mounts: Dict[str, ASGIFramework]) -> None:
+    def __init__(self, mounts: dict[str, ASGIFramework]) -> None:
         self.mounts = mounts
 
     async def __call__(self, scope: Scope, receive: Callable, send: Callable) -> None:
         if scope["type"] == "lifespan":
             await self._handle_lifespan(scope, receive, send)
         else:
             for path, app in self.mounts.items():
@@ -33,15 +33,24 @@
         pass
 
 
 class DispatcherMiddleware(_DispatcherMiddleware):
     async def _handle_lifespan(self, scope: Scope, receive: Callable, send: Callable) -> None:
         import anyio
 
-        self.app_queues = {path: anyio.create_memory_object_stream(MAX_QUEUE_SIZE) for path in self.mounts}
+        self.app_queues: dict[
+            str,
+            tuple[
+                anyio.streams.memory.MemoryObjectSendStream,
+                anyio.streams.memory.MemoryObjectReceiveStream,
+            ],
+        ] = {
+            path: anyio.create_memory_object_stream[Dict[str, Any]](MAX_QUEUE_SIZE)
+            for path in self.mounts
+        }
         self.startup_complete = {path: False for path in self.mounts}
         self.shutdown_complete = {path: False for path in self.mounts}
 
         async with anyio.create_task_group() as tg:
             for path, app in self.mounts.items():
                 tg.start_soon(
                     app,
```

### Comparing `anycorn-0.16.0/src/anycorn/middleware/http_to_https.py` & `anycorn-0.17.0/src/anycorn/middleware/http_to_https.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
-from typing import Callable, Optional
+from typing import Callable
 from urllib.parse import urlunsplit
 
 from ..typing import ASGIFramework, HTTPScope, Scope, WebsocketScope, WWWScope
 
 
 class HTTPToHTTPSRedirectMiddleware:
-    def __init__(self, app: ASGIFramework, host: Optional[str]) -> None:
+    def __init__(self, app: ASGIFramework, host: str | None) -> None:
         self.app = app
         self.host = host
 
     async def __call__(self, scope: Scope, receive: Callable, send: Callable) -> None:
         if scope["type"] == "http" and scope["scheme"] == "http":
             await self._send_http_redirect(scope, send)
         elif scope["type"] == "websocket" and scope["scheme"] == "ws":
```

### Comparing `anycorn-0.16.0/src/anycorn/middleware/proxy_fix.py` & `anycorn-0.17.0/src/anycorn/middleware/proxy_fix.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from copy import deepcopy
-from typing import Callable, Iterable, Literal, Optional, Tuple
+from typing import Callable, Iterable, Literal
 
 from ..typing import ASGIFramework, Scope
 
 
 class ProxyFixMiddleware:
     def __init__(
         self,
@@ -18,17 +18,17 @@
         self.trusted_hops = trusted_hops
 
     async def __call__(self, scope: Scope, receive: Callable, send: Callable) -> None:
         # Keep the `or` instead of `in {'http' …}` to allow type narrowing
         if scope["type"] == "http" or scope["type"] == "websocket":
             scope = deepcopy(scope)
             headers = scope["headers"]
-            client: Optional[str] = None
-            scheme: Optional[str] = None
-            host: Optional[str] = None
+            client: str | None = None
+            scheme: str | None = None
+            host: str | None = None
 
             if (
                 self.mode == "modern"
                 and (value := _get_trusted_value(b"forwarded", headers, self.trusted_hops))
                 is not None
             ):
                 for part in value.split(";"):
@@ -59,16 +59,16 @@
                 headers.append((b"host", host.encode()))
                 scope["headers"] = headers
 
         await self.app(scope, receive, send)
 
 
 def _get_trusted_value(
-    name: bytes, headers: Iterable[Tuple[bytes, bytes]], trusted_hops: int
-) -> Optional[str]:
+    name: bytes, headers: Iterable[tuple[bytes, bytes]], trusted_hops: int
+) -> str | None:
     if trusted_hops == 0:
         return None
 
     values = []
     for header_name, header_value in headers:
         if header_name.lower() == name:
             values.extend([value.decode("latin1").strip() for value in header_value.split(b",")])
```

### Comparing `anycorn-0.16.0/src/anycorn/middleware/wsgi.py` & `anycorn-0.17.0/src/anycorn/middleware/wsgi.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
-from functools import partial
-from typing import Any, Callable, Iterable
+from typing import Callable, Iterable
 
 from ..app_wrappers import WSGIWrapper
 from ..typing import ASGIReceiveCallable, ASGISendCallable, Scope, WSGIFramework
 
 MAX_BODY_SIZE = 2**16
 
 WSGICallable = Callable[[dict, Callable], Iterable[bytes]]
```

### Comparing `anycorn-0.16.0/src/anycorn/protocol/__init__.py` & `anycorn-0.17.0/src/anycorn/protocol/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from __future__ import annotations
 
-from typing import Awaitable, Callable, Optional, Tuple, Union
+from typing import Awaitable, Callable
 
-from .h2 import H2Protocol
-from .h11 import H2CProtocolRequiredError, H2ProtocolAssumedError, H11Protocol
 from ..config import Config
 from ..events import Event, RawData
 from ..typing import AppWrapper, TaskGroup, WorkerContext
+from .h2 import H2Protocol
+from .h11 import H2CProtocolRequiredError, H2ProtocolAssumedError, H11Protocol
 
 
 class ProtocolWrapper:
     def __init__(
         self,
         app: AppWrapper,
         config: Config,
         context: WorkerContext,
         task_group: TaskGroup,
         ssl: bool,
-        client: Optional[Tuple[str, int]],
-        server: Optional[Tuple[str, int]],
+        client: tuple[str, int] | None,
+        server: tuple[str, int] | None,
         send: Callable[[Event], Awaitable[None]],
-        alpn_protocol: Optional[str] = None,
+        alpn_protocol: str | None = None,
     ) -> None:
         self.app = app
         self.config = config
         self.context = context
         self.task_group = task_group
         self.ssl = ssl
         self.client = client
         self.server = server
         self.send = send
-        self.protocol: Union[H11Protocol, H2Protocol]
+        self.protocol: H11Protocol | H2Protocol
         if alpn_protocol == "h2":
             self.protocol = H2Protocol(
                 self.app,
                 self.config,
                 self.context,
                 self.task_group,
                 self.ssl,
```

### Comparing `anycorn-0.16.0/src/anycorn/protocol/events.py` & `anycorn-0.17.0/src/anycorn/protocol/events.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
-from typing import List, Tuple
 
 
 @dataclass(frozen=True)
 class Event:
     stream_id: int
 
 
 @dataclass(frozen=True)
 class Request(Event):
-    headers: List[Tuple[bytes, bytes]]
+    headers: list[tuple[bytes, bytes]]
     http_version: str
     method: str
     raw_path: bytes
 
 
 @dataclass(frozen=True)
 class Body(Event):
@@ -35,21 +34,21 @@
 @dataclass(frozen=True)
 class EndData(Event):
     pass
 
 
 @dataclass(frozen=True)
 class Response(Event):
-    headers: List[Tuple[bytes, bytes]]
+    headers: list[tuple[bytes, bytes]]
     status_code: int
 
 
 @dataclass(frozen=True)
 class InformationalResponse(Event):
-    headers: List[Tuple[bytes, bytes]]
+    headers: list[tuple[bytes, bytes]]
     status_code: int
 
     def __post_init__(self) -> None:
         if self.status_code >= 200 or self.status_code < 100:
             raise ValueError(f"Status code must be 1XX not {self.status_code}")
```

### Comparing `anycorn-0.16.0/src/anycorn/protocol/h11.py` & `anycorn-0.17.0/src/anycorn/protocol/h11.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from __future__ import annotations
 
 from itertools import chain
-from typing import Awaitable, Callable, cast, Optional, Tuple, Type, Union
+from typing import Awaitable, Callable, cast
 
 import h11
 
+from ..config import Config
+from ..events import Closed, Event, RawData, Updated
+from ..typing import AppWrapper, H11SendableEvent, TaskGroup, WorkerContext
 from .events import (
     Body,
     Data,
     EndBody,
     EndData,
-    Event as StreamEvent,
     InformationalResponse,
     Request,
     Response,
     StreamClosed,
 )
+from .events import (
+    Event as StreamEvent,
+)
 from .http_stream import HTTPStream
 from .ws_stream import WSStream
-from ..config import Config
-from ..events import Closed, Event, RawData, Updated
-from ..typing import AppWrapper, H11SendableEvent, TaskGroup, WorkerContext
 
 STREAM_ID = 1
 
 
 class H2CProtocolRequiredError(Exception):
     def __init__(self, data: bytes, request: h11.Request) -> None:
         settings = ""
@@ -58,15 +60,15 @@
     def __init__(self, h11_connection: h11.Connection) -> None:
         self.buffer = bytearray(h11_connection.trailing_data[0])
         self.h11_connection = h11_connection
 
     def receive_data(self, data: bytes) -> None:
         self.buffer.extend(data)
 
-    def next_event(self) -> Union[Data, Type[h11.NEED_DATA]]:
+    def next_event(self) -> Data | type[h11.NEED_DATA]:
         if self.buffer:
             event = Data(stream_id=STREAM_ID, data=bytes(self.buffer))
             self.buffer = bytearray()
             return event
         else:
             return h11.NEED_DATA
 
@@ -81,31 +83,31 @@
     def __init__(
         self,
         app: AppWrapper,
         config: Config,
         context: WorkerContext,
         task_group: TaskGroup,
         ssl: bool,
-        client: Optional[Tuple[str, int]],
-        server: Optional[Tuple[str, int]],
+        client: tuple[str, int] | None,
+        server: tuple[str, int] | None,
         send: Callable[[Event], Awaitable[None]],
     ) -> None:
         self.app = app
         self.can_read = context.event_class()
         self.client = client
         self.config = config
-        self.connection: Union[h11.Connection, H11WSConnection] = h11.Connection(
+        self.connection: h11.Connection | H11WSConnection = h11.Connection(
             h11.SERVER, max_incomplete_event_size=self.config.h11_max_incomplete_size
         )
         self.context = context
         self.keep_alive_requests = 0
         self.send = send
         self.server = server
         self.ssl = ssl
-        self.stream: Optional[Union[HTTPStream, WSStream]] = None
+        self.stream: HTTPStream | WSStream | None = None
         self.task_group = task_group
 
     async def initiate(self) -> None:
         pass
 
     async def handle(self, event: Event) -> None:
         if isinstance(event, RawData):
```

### Comparing `anycorn-0.16.0/src/anycorn/protocol/h2.py` & `anycorn-0.17.0/src/anycorn/protocol/h2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 from __future__ import annotations
 
-from typing import Awaitable, Callable, Dict, List, Optional, Tuple, Type, Union
+from typing import Awaitable, Callable
 
 import h2
 import h2.connection
 import h2.events
 import h2.exceptions
 import priority
 
+from ..config import Config
+from ..events import Closed, Event, RawData, Updated
+from ..typing import AppWrapper, TaskGroup, WorkerContext
+from ..typing import Event as IOEvent
+from ..utils import filter_pseudo_headers
 from .events import (
     Body,
     Data,
     EndBody,
     EndData,
-    Event as StreamEvent,
     InformationalResponse,
     Request,
     Response,
     StreamClosed,
 )
+from .events import (
+    Event as StreamEvent,
+)
 from .http_stream import HTTPStream
 from .ws_stream import WSStream
-from ..config import Config
-from ..events import Closed, Event, RawData, Updated
-from ..typing import AppWrapper, Event as IOEvent, TaskGroup, WorkerContext
-from ..utils import filter_pseudo_headers
 
 BUFFER_HIGH_WATER = 2 * 2**14  # Twice the default max frame size (two frames worth)
 BUFFER_LOW_WATER = BUFFER_HIGH_WATER / 2
 
 
 class BufferCompleteError(Exception):
     pass
 
 
 class StreamBuffer:
-    def __init__(self, event_class: Type[IOEvent]) -> None:
+    def __init__(self, event_class: type[IOEvent]) -> None:
         self.buffer = bytearray()
         self._complete = False
         self._is_empty = event_class()
         self._paused = event_class()
 
     async def drain(self) -> None:
         await self._is_empty.wait()
@@ -81,16 +84,16 @@
     def __init__(
         self,
         app: AppWrapper,
         config: Config,
         context: WorkerContext,
         task_group: TaskGroup,
         ssl: bool,
-        client: Optional[Tuple[str, int]],
-        server: Optional[Tuple[str, int]],
+        client: tuple[str, int] | None,
+        server: tuple[str, int] | None,
         send: Callable[[Event], Awaitable[None]],
     ) -> None:
         self.app = app
         self.client = client
         self.closed = False
         self.config = config
         self.context = context
@@ -109,26 +112,26 @@
             },
         )
 
         self.keep_alive_requests = 0
         self.send = send
         self.server = server
         self.ssl = ssl
-        self.streams: Dict[int, Union[HTTPStream, WSStream]] = {}
+        self.streams: dict[int, HTTPStream | WSStream] = {}
         # The below are used by the sending task
         self.has_data = self.context.event_class()
         self.priority = priority.PriorityTree()
-        self.stream_buffers: Dict[int, StreamBuffer] = {}
+        self.stream_buffers: dict[int, StreamBuffer] = {}
 
     @property
     def idle(self) -> bool:
         return len(self.streams) == 0 or all(stream.idle for stream in self.streams.values())
 
     async def initiate(
-        self, headers: Optional[List[Tuple[bytes, bytes]]] = None, settings: Optional[str] = None
+        self, headers: list[tuple[bytes, bytes]] | None = None, settings: str | None = None
     ) -> None:
         if settings is not None:
             self.connection.initiate_upgrade_connection(settings)
         else:
             self.connection.initiate_connection()
         await self._flush()
         if headers is not None:
@@ -230,15 +233,15 @@
             priority.MissingStreamError,
             h2.exceptions.ProtocolError,
         ):
             # Connection has closed whilst blocked on flow control or
             # connection has advanced ahead of the last emitted event.
             return
 
-    async def _handle_events(self, events: List[h2.events.Event]) -> None:
+    async def _handle_events(self, events: list[h2.events.Event]) -> None:
         for event in events:
             if isinstance(event, h2.events.RequestReceived):
                 if self.context.terminated.is_set():
                     self.connection.reset_stream(event.stream_id)
                     self.connection.update_settings(
                         {h2.settings.SettingCodes.MAX_CONCURRENT_STREAMS: 0}
                     )
@@ -272,15 +275,15 @@
         await self._flush()
 
     async def _flush(self) -> None:
         data = self.connection.data_to_send()
         if data != b"":
             await self.send(RawData(data=data))
 
-    async def _window_updated(self, stream_id: Optional[int]) -> None:
+    async def _window_updated(self, stream_id: int | None) -> None:
         if stream_id is None or stream_id == 0:
             # Unblock all streams
             for stream_id in list(self.stream_buffers.keys()):
                 self.priority.unblock(stream_id)
         elif stream_id is not None and stream_id in self.stream_buffers:
             self.priority.unblock(stream_id)
         await self.has_data.set()
@@ -353,15 +356,15 @@
                 raw_path=raw_path,
             )
         )
         self.keep_alive_requests += 1
         await self.context.mark_request()
 
     async def _create_server_push(
-        self, stream_id: int, path: bytes, headers: List[Tuple[bytes, bytes]]
+        self, stream_id: int, path: bytes, headers: list[tuple[bytes, bytes]]
     ) -> None:
         push_stream_id = self.connection.get_next_available_stream_id()
         request_headers = [(b":method", b"GET"), (b":path", path)]
         request_headers.extend(headers)
         request_headers.extend(self.config.response_headers("h2"))
         try:
             self.connection.push_stream(
```

### Comparing `anycorn-0.16.0/src/anycorn/protocol/h3.py` & `anycorn-0.17.0/src/anycorn/protocol/h3.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,57 @@
 from __future__ import annotations
 
-from typing import Awaitable, Callable, Dict, List, Optional, Tuple, Union
+from typing import Awaitable, Callable
 
 from aioquic.h3.connection import H3Connection
 from aioquic.h3.events import DataReceived, HeadersReceived
 from aioquic.h3.exceptions import NoAvailablePushIDError
 from aioquic.quic.connection import QuicConnection
 from aioquic.quic.events import QuicEvent
 
+from ..config import Config
+from ..typing import AppWrapper, TaskGroup, WorkerContext
+from ..utils import filter_pseudo_headers
 from .events import (
     Body,
     Data,
     EndBody,
     EndData,
-    Event as StreamEvent,
     InformationalResponse,
     Request,
     Response,
     StreamClosed,
 )
+from .events import (
+    Event as StreamEvent,
+)
 from .http_stream import HTTPStream
 from .ws_stream import WSStream
-from ..config import Config
-from ..typing import AppWrapper, TaskGroup, WorkerContext
-from ..utils import filter_pseudo_headers
 
 
 class H3Protocol:
     def __init__(
         self,
         app: AppWrapper,
         config: Config,
         context: WorkerContext,
         task_group: TaskGroup,
-        client: Optional[Tuple[str, int]],
-        server: Optional[Tuple[str, int]],
+        client: tuple[str, int] | None,
+        server: tuple[str, int] | None,
         quic: QuicConnection,
         send: Callable[[], Awaitable[None]],
     ) -> None:
         self.app = app
         self.client = client
         self.config = config
         self.context = context
         self.connection = H3Connection(quic)
         self.send = send
         self.server = server
-        self.streams: Dict[int, Union[HTTPStream, WSStream]] = {}
+        self.streams: dict[int, HTTPStream | WSStream] = {}
         self.task_group = task_group
 
     async def handle(self, quic_event: QuicEvent) -> None:
         for event in self.connection.handle_event(quic_event):
             if isinstance(event, HeadersReceived):
                 if not self.context.terminated.is_set():
                     await self._create_stream(event)
@@ -124,15 +126,15 @@
                 method=method,
                 raw_path=raw_path,
             )
         )
         await self.context.mark_request()
 
     async def _create_server_push(
-        self, stream_id: int, path: bytes, headers: List[Tuple[bytes, bytes]]
+        self, stream_id: int, path: bytes, headers: list[tuple[bytes, bytes]]
     ) -> None:
         request_headers = [(b":method", b"GET"), (b":path", path)]
         request_headers.extend(headers)
         request_headers.extend(self.config.response_headers("h3"))
         try:
             push_stream_id = self.connection.send_push_promise(
                 stream_id=stream_id, headers=request_headers
```

### Comparing `anycorn-0.16.0/src/anycorn/protocol/http_stream.py` & `anycorn-0.17.0/src/anycorn/protocol/http_stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from __future__ import annotations
 
-from enum import auto, Enum
+from enum import Enum, auto
 from time import time
-from typing import Awaitable, Callable, Optional, Tuple
+from typing import Awaitable, Callable
 from urllib.parse import unquote
 
-from .events import Body, EndBody, Event, InformationalResponse, Request, Response, StreamClosed
 from ..config import Config
 from ..typing import (
     AppWrapper,
     ASGISendEvent,
     HTTPResponseStartEvent,
     HTTPScope,
     TaskGroup,
     WorkerContext,
 )
 from ..utils import (
+    UnexpectedMessageError,
     build_and_validate_headers,
     suppress_body,
-    UnexpectedMessageError,
     valid_server_name,
 )
+from .events import Body, EndBody, Event, InformationalResponse, Request, Response, StreamClosed
 
 PUSH_VERSIONS = {"2", "3"}
 EARLY_HINTS_VERSIONS = {"2", "3"}
 
 
 class ASGIHTTPState(Enum):
     # The ASGI Spec is clear that a response should not start till the
@@ -39,16 +39,16 @@
     def __init__(
         self,
         app: AppWrapper,
         config: Config,
         context: WorkerContext,
         task_group: TaskGroup,
         ssl: bool,
-        client: Optional[Tuple[str, int]],
-        server: Optional[Tuple[str, int]],
+        client: tuple[str, int] | None,
+        server: tuple[str, int] | None,
         send: Callable[[Event], Awaitable[None]],
         stream_id: int,
     ) -> None:
         self.app = app
         self.client = client
         self.closed = False
         self.config = config
@@ -106,19 +106,20 @@
             await self.app_put(
                 {"type": "http.request", "body": bytes(event.data), "more_body": True}
             )
         elif isinstance(event, EndBody):
             await self.app_put({"type": "http.request", "body": b"", "more_body": False})
         elif isinstance(event, StreamClosed):
             self.closed = True
-            await self.config.log.access(self.scope, None, time() - self.start_time)
+            if self.state != ASGIHTTPState.CLOSED:
+                await self.config.log.access(self.scope, None, time() - self.start_time)
             if self.app_put is not None:
                 await self.app_put({"type": "http.disconnect"})
 
-    async def app_send(self, message: Optional[ASGISendEvent]) -> None:
+    async def app_send(self, message: ASGISendEvent | None) -> None:
         if message is None:  # ASGI App has finished sending messages
             if not self.closed:
                 # Cleanup if required
                 if self.state == ASGIHTTPState.REQUEST:
                     await self._send_error_response(500)
                 await self.send(StreamClosed(stream_id=self.stream_id))
         else:
```

### Comparing `anycorn-0.16.0/src/anycorn/protocol/quic.py` & `anycorn-0.17.0/src/anycorn/protocol/quic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 from __future__ import annotations
 
 from functools import partial
-from typing import Awaitable, Callable, Dict, Optional, Tuple
+from typing import Awaitable, Callable
 
 from aioquic.buffer import Buffer
 from aioquic.h3.connection import H3_ALPN
 from aioquic.quic.configuration import QuicConfiguration
 from aioquic.quic.connection import QuicConnection
 from aioquic.quic.events import (
     ConnectionIdIssued,
     ConnectionIdRetired,
     ConnectionTerminated,
     ProtocolNegotiated,
 )
 from aioquic.quic.packet import (
-    encode_quic_version_negotiation,
     PACKET_TYPE_INITIAL,
+    encode_quic_version_negotiation,
     pull_quic_header,
 )
 
-from .h3 import H3Protocol
 from ..config import Config
 from ..events import Closed, Event, RawData
 from ..typing import AppWrapper, TaskGroup, WorkerContext
+from .h3 import H3Protocol
 
 
 class QuicProtocol:
     def __init__(
         self,
         app: AppWrapper,
         config: Config,
         context: WorkerContext,
         task_group: TaskGroup,
-        server: Optional[Tuple[str, int]],
+        server: tuple[str, int] | None,
         send: Callable[[Event], Awaitable[None]],
     ) -> None:
         self.app = app
         self.config = config
         self.context = context
-        self.connections: Dict[bytes, QuicConnection] = {}
-        self.http_connections: Dict[QuicConnection, H3Protocol] = {}
+        self.connections: dict[bytes, QuicConnection] = {}
+        self.http_connections: dict[QuicConnection, H3Protocol] = {}
         self.send = send
         self.server = server
         self.task_group = task_group
 
         self.quic_config = QuicConfiguration(alpn_protocols=H3_ALPN, is_client=False)
         self.quic_config.load_cert_chain(certfile=config.certfile, keyfile=config.keyfile)
 
@@ -90,15 +90,15 @@
             pass
 
     async def send_all(self, connection: QuicConnection) -> None:
         for data, address in connection.datagrams_to_send(now=self.context.time()):
             await self.send(RawData(data=data, address=address))
 
     async def _handle_events(
-        self, connection: QuicConnection, client: Optional[Tuple[str, int]] = None
+        self, connection: QuicConnection, client: tuple[str, int] | None = None
     ) -> None:
         event = connection.next_event()
         while event is not None:
             if isinstance(event, ConnectionTerminated):
                 pass
             elif isinstance(event, ProtocolNegotiated):
                 self.http_connections[connection] = H3Protocol(
```

### Comparing `anycorn-0.16.0/src/anycorn/protocol/ws_stream.py` & `anycorn-0.17.0/src/anycorn/protocol/ws_stream.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,49 @@
 from __future__ import annotations
 
-from enum import auto, Enum
+from enum import Enum, auto
 from io import BytesIO, StringIO
 from time import time
-from typing import Awaitable, Callable, Iterable, List, Optional, Tuple, Union
+from typing import Awaitable, Callable, Iterable
 from urllib.parse import unquote
 
 from wsproto.connection import Connection, ConnectionState, ConnectionType
 from wsproto.events import (
     BytesMessage,
     CloseConnection,
-    Event as WSProtoEvent,
     Message,
     Ping,
     TextMessage,
 )
+from wsproto.events import (
+    Event as WSProtoEvent,
+)
 from wsproto.extensions import Extension, PerMessageDeflate
 from wsproto.frame_protocol import CloseReason
-from wsproto.handshake import server_extensions_handshake, WEBSOCKET_VERSION
-from wsproto.utilities import generate_accept_token, LocalProtocolError, split_comma_header
+from wsproto.handshake import WEBSOCKET_VERSION, server_extensions_handshake
+from wsproto.utilities import LocalProtocolError, generate_accept_token, split_comma_header
 
-from .events import Body, Data, EndBody, EndData, Event, Request, Response, StreamClosed
 from ..config import Config
 from ..typing import (
     AppWrapper,
     ASGISendEvent,
     TaskGroup,
     WebsocketAcceptEvent,
     WebsocketResponseBodyEvent,
     WebsocketResponseStartEvent,
     WebsocketScope,
     WorkerContext,
 )
 from ..utils import (
+    UnexpectedMessageError,
     build_and_validate_headers,
     suppress_body,
-    UnexpectedMessageError,
     valid_server_name,
 )
+from .events import Body, Data, EndBody, EndData, Event, Request, Response, StreamClosed
 
 
 class ASGIWebsocketState(Enum):
     # Hypercorn supports the ASGI websocket HTTP response extension,
     # which allows HTTP responses rather than acceptance.
     HANDSHAKE = auto()
     CONNECTED = auto()
@@ -51,22 +53,22 @@
 
 
 class FrameTooLargeError(Exception):
     pass
 
 
 class Handshake:
-    def __init__(self, headers: List[Tuple[bytes, bytes]], http_version: str) -> None:
+    def __init__(self, headers: list[tuple[bytes, bytes]], http_version: str) -> None:
         self.http_version = http_version
-        self.connection_tokens: Optional[List[str]] = None
-        self.extensions: Optional[List[str]] = None
-        self.key: Optional[bytes] = None
-        self.subprotocols: Optional[List[str]] = None
-        self.upgrade: Optional[bytes] = None
-        self.version: Optional[bytes] = None
+        self.connection_tokens: list[str] | None = None
+        self.extensions: list[str] | None = None
+        self.key: bytes | None = None
+        self.subprotocols: list[str] | None = None
+        self.upgrade: bytes | None = None
+        self.version: bytes | None = None
         for name, value in headers:
             name = name.lower()
             if name == b"connection":
                 self.connection_tokens = split_comma_header(value)
             elif name == b"sec-websocket-extensions":
                 self.extensions = split_comma_header(value)
             elif name == b"sec-websocket-key":
@@ -93,25 +95,25 @@
 
         if self.version != WEBSOCKET_VERSION:
             return False
         return True
 
     def accept(
         self,
-        subprotocol: Optional[str],
-        additional_headers: Iterable[Tuple[bytes, bytes]],
-    ) -> Tuple[int, List[Tuple[bytes, bytes]], Connection]:
+        subprotocol: str | None,
+        additional_headers: Iterable[tuple[bytes, bytes]],
+    ) -> tuple[int, list[tuple[bytes, bytes]], Connection]:
         headers = []
         if subprotocol is not None:
             if self.subprotocols is None or subprotocol not in self.subprotocols:
                 raise Exception("Invalid Subprotocol")
             else:
                 headers.append((b"sec-websocket-protocol", subprotocol.encode()))
 
-        extensions: List[Extension] = [PerMessageDeflate()]
+        extensions: list[Extension] = [PerMessageDeflate()]
         accepts = None
         if self.extensions is not None:
             accepts = server_extensions_handshake(self.extensions, extensions)
 
         if accepts:
             headers.append((b"sec-websocket-extensions", accepts))
 
@@ -130,15 +132,15 @@
             headers.append((name, value))
 
         return status_code, headers, Connection(ConnectionType.SERVER, extensions)
 
 
 class WebsocketBuffer:
     def __init__(self, max_length: int) -> None:
-        self.value: Optional[Union[BytesIO, StringIO]] = None
+        self.value: BytesIO | StringIO | None = None
         self.length = 0
         self.max_length = max_length
 
     def extend(self, event: Message) -> None:
         if self.value is None:
             if isinstance(event, TextMessage):
                 self.value = StringIO()
@@ -164,21 +166,21 @@
     def __init__(
         self,
         app: AppWrapper,
         config: Config,
         context: WorkerContext,
         task_group: TaskGroup,
         ssl: bool,
-        client: Optional[Tuple[str, int]],
-        server: Optional[Tuple[str, int]],
+        client: tuple[str, int] | None,
+        server: tuple[str, int] | None,
         send: Callable[[Event], Awaitable[None]],
         stream_id: int,
     ) -> None:
         self.app = app
-        self.app_put: Optional[Callable] = None
+        self.app_put: Callable | None = None
         self.buffer = WebsocketBuffer(config.websocket_max_message_size)
         self.client = client
         self.closed = False
         self.config = config
         self.context = context
         self.task_group = task_group
         self.response: WebsocketResponseStartEvent
@@ -240,15 +242,15 @@
             if self.app_put is not None:
                 if self.state in {ASGIWebsocketState.HTTPCLOSED, ASGIWebsocketState.CLOSED}:
                     code = CloseReason.NORMAL_CLOSURE.value
                 else:
                     code = CloseReason.ABNORMAL_CLOSURE.value
                 await self.app_put({"type": "websocket.disconnect", "code": code})
 
-    async def app_send(self, message: Optional[ASGISendEvent]) -> None:
+    async def app_send(self, message: ASGISendEvent | None) -> None:
         if self.closed:
             # Allow app to finish after close
             return
 
         if message is None:  # ASGI App has finished sending messages
             # Cleanup if required
             if self.state == ASGIWebsocketState.HANDSHAKE:
```

### Comparing `anycorn-0.16.0/src/anycorn/run.py` & `anycorn-0.17.0/src/anycorn/run.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,37 +8,37 @@
 from multiprocessing import get_context
 from multiprocessing.connection import wait
 from multiprocessing.context import BaseContext
 from multiprocessing.process import BaseProcess
 from multiprocessing.synchronize import Event as EventType
 from pickle import PicklingError
 from random import randint
-from typing import Any, Awaitable, Callable, List, Optional
+from typing import Any, Awaitable, Callable
 
 import anyio
 
 from .config import Config, Sockets
 from .lifespan import Lifespan
 from .statsd import StatsdLogger
 from .tcp_server import tcp_server_handler
 from .typing import AppWrapper, WorkerFunc
-from .udp_server import UDPServer
+
+# from .udp_server import UDPServer
 from .utils import (
+    ShutdownError,
     check_for_updates,
     check_multiprocess_shutdown_event,
     files_to_watch,
     load_application,
     raise_shutdown,
     repr_socket_addr,
-    ShutdownError,
     write_pid_file,
 )
 from .worker_context import WorkerContext
 
-
 if sys.version_info < (3, 11):
     from exceptiongroup import BaseExceptionGroup
 
 
 def run(config: Config) -> int:
     if config.pid_path is not None:
         write_pid_file(config.pid_path)
@@ -66,15 +66,15 @@
         shutdown_event = ctx.Event()
 
         def shutdown(*args: Any) -> None:
             nonlocal active, shutdown_event
             shutdown_event.set()
             active = False
 
-        processes: List[BaseProcess] = []
+        processes: list[BaseProcess] = []
         while active:
             # Ignore SIGINT before creating the processes, so that they
             # inherit the signal handling. This means that the shutdown
             # function controls the shutdown.
             signal.signal(signal.SIGINT, signal.SIG_IGN)
 
             _populate(processes, config, worker_func, sockets, shutdown_event, ctx)
@@ -115,39 +115,39 @@
         for sock in sockets.insecure_sockets:
             sock.close()
 
     return exitcode
 
 
 def _populate(
-    processes: List[BaseProcess],
+    processes: list[BaseProcess],
     config: Config,
     worker_func: WorkerFunc,
     sockets: Sockets,
     shutdown_event: EventType,
     ctx: BaseContext,
 ) -> None:
     for _ in range(config.workers - len(processes)):
-        process = ctx.Process(  # type: ignore
+        process = ctx.Process(  # type: ignore[attr-defined]
             target=worker_func,
             kwargs={"config": config, "shutdown_event": shutdown_event, "sockets": sockets},
         )
         process.daemon = True
         try:
             process.start()
         except PicklingError as error:
             raise RuntimeError(
-                "Cannot pickle the config, see https://docs.python.org/3/library/pickle.html#pickle-picklable"  # noqa: E501
+                "Cannot pickle the config, see https://docs.python.org/3/library/pickle.html#pickle-picklable"
             ) from error
         processes.append(process)
         if platform.system() == "Windows":
             time.sleep(0.1)
 
 
-def _join_exited(processes: List[BaseProcess]) -> int:
+def _join_exited(processes: list[BaseProcess]) -> int:
     exitcode = 0
     for index in reversed(range(len(processes))):
         worker = processes[index]
         if worker.exitcode is not None:
             worker.join()
             exitcode = worker.exitcode if exitcode == 0 else exitcode
             del processes[index]
@@ -155,102 +155,108 @@
     return exitcode
 
 
 async def worker_serve(
     app: AppWrapper,
     config: Config,
     *,
-    sockets: Optional[Sockets] = None,
-    shutdown_trigger: Optional[Callable[..., Awaitable[None]]] = None,
-    task_status: anyio.abc.TaskStatus[None] = anyio.TASK_STATUS_IGNORED,
+    sockets: Sockets | None = None,
+    shutdown_trigger: Callable[..., Awaitable[None]] | None = None,
+    task_status: anyio.abc.TaskStatus[list[str]] = anyio.TASK_STATUS_IGNORED,
 ) -> None:
     config.set_statsd_logger_class(StatsdLogger)
 
     lifespan = Lifespan(app, config)
     max_requests = None
     if config.max_requests is not None:
         max_requests = config.max_requests + randint(0, config.max_requests_jitter)
     context = WorkerContext(max_requests)
 
-    async with anyio.create_task_group() as lifespan_nursery:
-        await lifespan_nursery.start(lifespan.handle_lifespan)
+    async with anyio.create_task_group() as lifespan_tg:
+        await lifespan_tg.start(lifespan.handle_lifespan)
         await lifespan.wait_for_startup()
 
-        async with anyio.create_task_group() as server_nursery:
+        async with anyio.create_task_group() as server_tg:
             if sockets is None:
                 sockets = config.create_sockets()
                 for sock in sockets.secure_sockets:
                     sock.listen(config.backlog)
                 for sock in sockets.insecure_sockets:
                     sock.listen(config.backlog)
 
             ssl_context = config.create_ssl_context()
-            listeners = []
+            listeners: list[anyio.abc.SocketListener | anyio.streams.tls.TLSListener] = []
             binds = []
-            for sock in sockets.secure_sockets:
-                listeners.append(
-                    trio.SSLListener(
-                        trio.SocketListener(trio.socket.from_stdlib_socket(sock)),
-                        ssl_context,
-                        https_compatible=True,
-                    )
+            for secure_sock in sockets.secure_sockets:
+                asynclib = anyio._core._eventloop.get_async_backend()
+                secure_listener = anyio.streams.tls.TLSListener(
+                    asynclib.create_tcp_listener(secure_sock),
+                    ssl_context,
+                    True,
+                    config.ssl_handshake_timeout,
                 )
-                bind = repr_socket_addr(sock.family, sock.getsockname())
-                binds.append(f"https://{bind}")
-                await config.log.info(f"Running on https://{bind} (CTRL + C to quit)")
+                listeners.append(secure_listener)
+                bind = repr_socket_addr(secure_sock.family, secure_sock.getsockname())
+                url = f"https://{bind}"
+                binds.append(url)
+                await config.log.info("Running on %s (CTRL + C to quit)", url)
 
-            for sock in sockets.insecure_sockets:
+            for insecure_sock in sockets.insecure_sockets:
                 asynclib = anyio._core._eventloop.get_async_backend()
-                listener = asynclib.create_tcp_listener(sock)
-                listeners.append(listener)
-                bind = repr_socket_addr(sock.family, sock.getsockname())
-                binds.append(f"http://{bind}")
-                await config.log.info(f"Running on http://{bind} (CTRL + C to quit)")
-
-            for sock in sockets.quic_sockets:
-                await server_nursery.start(UDPServer(app, config, context, sock).run)
-                bind = repr_socket_addr(sock.family, sock.getsockname())
-                await config.log.info(f"Running on https://{bind} (QUIC) (CTRL + C to quit)")
+                insecure_listener = asynclib.create_tcp_listener(insecure_sock)
+                listeners.append(insecure_listener)
+                bind = repr_socket_addr(insecure_sock.family, insecure_sock.getsockname())
+                url = f"http://{bind}"
+                binds.append(url)
+                await config.log.info("Running on %s (CTRL + C to quit)", url)
+
+            # FIXME
+            # for quic_sock in sockets.quic_sockets:
+            #     await server_tg.start(UDPServer(app, config, context, quic_sock).run)
+            #     bind = repr_socket_addr(quic_sock.family, quic_sock.getsockname())
+            #     await config.log.info(f"Running on https://{bind} (QUIC) (CTRL + C to quit)")
 
             task_status.started(binds)
             try:
-                async with anyio.create_task_group() as nursery:
+                async with anyio.create_task_group() as tg:
                     if shutdown_trigger is not None:
-                        nursery.start_soon(raise_shutdown, shutdown_trigger)
-                    nursery.start_soon(raise_shutdown, context.terminate.wait)
+                        tg.start_soon(raise_shutdown, shutdown_trigger)
+                    tg.start_soon(raise_shutdown, context.terminate.wait)
 
                     for listener in listeners:
-                        nursery.start_soon(
+                        tg.start_soon(
                             partial(
                                 listener.serve,
                                 tcp_server_handler(app, config, context),
                             ),
                         )
 
                     await anyio.Event().wait()
             except BaseExceptionGroup as error:
                 _, other_errors = error.split((ShutdownError, KeyboardInterrupt))
                 if other_errors is not None:
                     raise other_errors
             finally:
                 await context.terminated.set()
-                server_nursery.cancel_scope.deadline = anyio.current_time() + config.graceful_timeout
+                server_tg.cancel_scope.deadline = anyio.current_time() + config.graceful_timeout
 
         await lifespan.wait_for_shutdown()
-        lifespan_nursery.cancel_scope.cancel()
+        lifespan_tg.cancel_scope.cancel()
 
 
 def anyio_worker(
-    config: Config, sockets: Optional[Sockets] = None, shutdown_event: Optional[EventType] = None
+    config: Config, sockets: Sockets | None = None, shutdown_event: EventType | None = None
 ) -> None:
     if sockets is not None:
         for sock in sockets.secure_sockets:
             sock.listen(config.backlog)
         for sock in sockets.insecure_sockets:
             sock.listen(config.backlog)
     app = load_application(config.application_path, config.wsgi_max_body_size)
 
     shutdown_trigger = None
     if shutdown_event is not None:
         shutdown_trigger = partial(check_multiprocess_shutdown_event, shutdown_event, anyio.sleep)
 
-    anyio.run(partial(worker_serve, app, config, sockets=sockets, shutdown_trigger=shutdown_trigger))
+    anyio.run(
+        partial(worker_serve, app, config, sockets=sockets, shutdown_trigger=shutdown_trigger)
+    )
```

### Comparing `anycorn-0.16.0/src/anycorn/statsd.py` & `anycorn-0.17.0/src/anycorn/statsd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import socket
-from typing import Any, TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 import anyio
 
-from .config import Config
 from .logging import Logger
 
 if TYPE_CHECKING:
     from .config import Config
     from .typing import ResponseSummary, WWWScope
 
 METRIC_VAR = "metric"
@@ -17,15 +16,15 @@
 MTYPE_VAR = "mtype"
 GAUGE_TYPE = "gauge"
 COUNTER_TYPE = "counter"
 HISTOGRAM_TYPE = "histogram"
 
 
 class BaseStatsdLogger(Logger):
-    def __init__(self, config: "Config") -> None:
+    def __init__(self, config: Config) -> None:
         super().__init__(config)
         self.dogstatsd_tags = config.dogstatsd_tags
         self.prefix = config.statsd_prefix
         if len(self.prefix) and self.prefix[-1] != ".":
             self.prefix += "."
 
     async def critical(self, message: str, *args: Any, **kwargs: Any) -> None:
@@ -67,15 +66,15 @@
 
             if message:
                 await super().log(level, message, *args, **kwargs)
         except Exception:
             await super().warning("Failed to log to statsd", exc_info=True)
 
     async def access(
-        self, request: "WWWScope", response: "ResponseSummary", request_time: float
+        self, request: WWWScope, response: ResponseSummary, request_time: float
     ) -> None:
         await super().access(request, response, request_time)
         await self.histogram("anycorn.request.duration", request_time * 1_000)
         await self.increment("anycorn.requests", 1)
         await self.increment(f"anycorn.request.status.{response['status']}", 1)
 
     async def gauge(self, name: str, value: int) -> None:
@@ -96,14 +95,20 @@
         await self._socket_send(message.encode("ascii"))
 
     async def _socket_send(self, message: bytes) -> None:
         raise NotImplementedError()
 
 
 class StatsdLogger(BaseStatsdLogger):
+    socket: anyio.abc.ConnectedUDPSocket | None
+
     def __init__(self, config: Config) -> None:
         super().__init__(config)
         self.address = tuple(config.statsd_host.rsplit(":", 1))
-        self.socket = anyio.create_udp_socket(family=socket.AF_INET)
+        self.socket = None
 
     async def _socket_send(self, message: bytes) -> None:
-        await self.socket.sendto(message, self.address)
+        if self.socket is None:
+            self.socket = await anyio.create_connected_udp_socket(
+                self.address[0], int(self.address[1]), family=socket.AddressFamily.AF_INET
+            )
+        await self.socket.send(message)
```

### Comparing `anycorn-0.16.0/src/anycorn/task_group.py` & `anycorn-0.17.0/src/anycorn/task_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import sys
 from contextlib import AsyncExitStack
 from types import TracebackType
-from typing import Any, Awaitable, Callable, Optional
+from typing import Any, Awaitable, Callable
 
 import anyio
 
 from .config import Config
 from .typing import AppWrapper, ASGIReceiveCallable, ASGIReceiveEvent, ASGISendEvent, Scope
 
 if sys.version_info < (3, 11):
@@ -15,15 +15,15 @@
 
 
 async def _handle(
     app: AppWrapper,
     config: Config,
     scope: Scope,
     receive: ASGIReceiveCallable,
-    send: Callable[[Optional[ASGISendEvent]], Awaitable[None]],
+    send: Callable[[ASGISendEvent | None], Awaitable[None]],
     sync_spawn: Callable,
     call_soon: Callable,
 ) -> None:
     try:
         await app(scope, receive, send, sync_spawn, call_soon)
     except anyio.get_cancelled_exc_class():
         raise
@@ -38,24 +38,26 @@
         await config.log.exception("Error in ASGI Framework")
     finally:
         await send(None)
 
 
 class TaskGroup:
     def __init__(self) -> None:
-        self._task_group: Optional[anyio.abc.TaskGroup] = None
+        self._task_group: anyio.abc.TaskGroup | None = None
 
     async def spawn_app(
         self,
         app: AppWrapper,
         config: Config,
         scope: Scope,
-        send: Callable[[Optional[ASGISendEvent]], Awaitable[None]],
+        send: Callable[[ASGISendEvent | None], Awaitable[None]],
     ) -> Callable[[ASGIReceiveEvent], Awaitable[None]]:
-        app_send_channel, app_receive_channel = anyio.create_memory_object_stream(config.max_app_queue_size)
+        app_send_channel, app_receive_channel = anyio.create_memory_object_stream[Any](
+            config.max_app_queue_size
+        )
         self._task_group.start_soon(
             _handle,
             app,
             config,
             scope,
             app_receive_channel.receive,
             send,
@@ -70,10 +72,10 @@
     async def __aenter__(self) -> TaskGroup:
         async with AsyncExitStack() as exit_stack:
             tg = anyio.create_task_group()
             self._task_group = await exit_stack.enter_async_context(tg)
             self._exit_stack = exit_stack.pop_all()
         return self
 
-    async def __aexit__(self, exc_type: type, exc_value: BaseException, tb: TracebackType) -> None:
+    async def __aexit__(self, exc_type: type, exc_value: BaseException, tb: TracebackType) -> Any:
         self._task_group = None
         return await self._exit_stack.__aexit__(exc_type, exc_value, tb)
```

### Comparing `anycorn-0.16.0/src/anycorn/tcp_server.py` & `anycorn-0.17.0/src/anycorn/tcp_server.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,57 @@
 from __future__ import annotations
 
 from math import inf
-from typing import Any, Generator, Optional
+from ssl import SSLError, SSLZeroReturnError
+from typing import Any, Callable, Generator
 
 import anyio
 
-from .task_group import TaskGroup
-from .worker_context import WorkerContext
 from .config import Config
 from .events import Closed, Event, RawData, Updated
 from .protocol import ProtocolWrapper
+from .task_group import TaskGroup
 from .typing import AppWrapper
 from .utils import parse_socket_addr
+from .worker_context import WorkerContext
 
 MAX_RECV = 2**16
 
 
 class TCPServer:
     def __init__(
-        self, app: AppWrapper, config: Config, context: WorkerContext, stream: trio.abc.Stream
+        self,
+        app: AppWrapper,
+        config: Config,
+        context: WorkerContext,
+        stream: anyio.abc.SocketStream,
     ) -> None:
         self.app = app
         self.config = config
         self.context = context
         self.protocol: ProtocolWrapper
         self.send_lock = anyio.Lock()
         self.idle_lock = anyio.Lock()
         self.stream = stream
 
-        self._idle_handle: Optional[anyio.CancelScope] = None
+        self._idle_handle: anyio.CancelScope | None = None
 
     def __await__(self) -> Generator[Any, None, None]:
         return self.run().__await__()
 
     async def run(self) -> None:
         try:
-            try:
-                with anyio.fail_after(self.config.ssl_handshake_timeout):
-                    await self.stream.do_handshake()
-            except (anyio.BrokenResourceError, TimeoutError):
-                return  # Handshake failed
-            alpn_protocol = self.stream.selected_alpn_protocol()
-            socket = self.stream.transport_stream.socket
+            alpn_protocol = self.stream.extra(anyio.streams.tls.TLSAttribute.alpn_protocol)
             ssl = True
-        except AttributeError:  # Not SSL
+        except anyio.TypedAttributeLookupError:  # Not SSL
             alpn_protocol = "http/1.1"
-            socket = self.stream.extra(anyio.abc.SocketAttribute.raw_socket)
             ssl = False
 
         try:
+            socket = self.stream.extra(anyio.abc.SocketAttribute.raw_socket)
             client = parse_socket_addr(socket.family, socket.getpeername())
             server = parse_socket_addr(socket.family, socket.getsockname())
 
             async with TaskGroup() as task_group:
                 self._task_group = task_group
                 self.protocol = ProtocolWrapper(
                     self.app,
@@ -73,18 +72,18 @@
         finally:
             await self._close()
 
     async def protocol_send(self, event: Event) -> None:
         if isinstance(event, RawData):
             async with self.send_lock:
                 try:
-                    with anyio.CancelScope(shield=True) as cancel_scope:
-                        #cancel_scope.shield = True
+                    with anyio.CancelScope(shield=True):  # as cancel_scope:
+                        # cancel_scope.shield = True
                         await self.stream.send(event.data)
-                except (anyio.BrokenResourceError, TimeoutError):
+                except (anyio.ClosedResourceError, anyio.BrokenResourceError, TimeoutError):
                     await self.protocol.handle(Closed())
         elif isinstance(event, Closed):
             await self._close()
             await self.protocol.handle(Closed())
         elif isinstance(event, Updated):
             if event.idle:
                 await self._start_idle()
@@ -97,65 +96,76 @@
                 with anyio.fail_after(self.config.read_timeout or inf):
                     data = await self.stream.receive(MAX_RECV)
             except (
                 anyio.ClosedResourceError,
                 anyio.BrokenResourceError,
                 anyio.EndOfStream,
                 TimeoutError,
+                SSLZeroReturnError,
             ):
                 break
             else:
                 await self.protocol.handle(RawData(data))
                 if data == b"":
                     break
         await self.protocol.handle(Closed())
 
     async def _close(self) -> None:
         try:
             await self.stream.send_eof()
         except (
             anyio.BrokenResourceError,
             AttributeError,
+            NotImplementedError,
+            TypeError,
             anyio.BusyResourceError,
             anyio.ClosedResourceError,
         ):
             # They're already gone, nothing to do
             # Or it is a SSL stream
             pass
-        await self.stream.aclose()
+        try:
+            await self.stream.aclose()
+        except (SSLError, anyio.ClosedResourceError, anyio.BrokenResourceError):
+            pass
 
     async def _initiate_server_close(self) -> None:
         await self.protocol.handle(Closed())
-        await self.stream.aclose()
+        try:
+            await self.stream.aclose()
+        except (SSLError, anyio.BrokenResourceError, anyio.BusyResourceError):
+            pass
 
     async def _start_idle(self) -> None:
         async with self.idle_lock:
             if self._idle_handle is None:
-                self._idle_handle = await self._task_group._task_group.start(self._run_idle)
+                if self._task_group._task_group is not None:
+                    self._idle_handle = await self._task_group._task_group.start(self._run_idle)
 
     async def _stop_idle(self) -> None:
         async with self.idle_lock:
             if self._idle_handle is not None:
                 self._idle_handle.cancel()
             self._idle_handle = None
 
     async def _run_idle(
         self,
-        *, 
-        task_status: anyio.abc.TaskStatus[None] = anyio.TASK_STATUS_IGNORED,
+        *,
+        task_status: anyio.abc.TaskStatus[anyio.CancelScope] = anyio.TASK_STATUS_IGNORED,
     ) -> None:
         cancel_scope = anyio.CancelScope()
         task_status.started(cancel_scope)
         with cancel_scope:
             with anyio.move_on_after(self.config.keep_alive_timeout):
                 await self.context.terminated.wait()
 
-            with anyio.CancelScope(shield=True) as scope:
-                #cancel_scope.shield = True
+            with anyio.CancelScope(shield=True):  # as cancel_scope:
+                # cancel_scope.shield = True
                 await self._initiate_server_close()
 
 
-def tcp_server_handler(app: AppWrapper, config: Config, context: WorkerContext):
-    async def handler(stream: trio.abc.Stream):
+def tcp_server_handler(app: AppWrapper, config: Config, context: WorkerContext) -> Callable:
+    async def handler(stream: anyio.abc.SocketStream) -> None:
         tcp_server = TCPServer(app, config, context, stream)
         await tcp_server.run()
+
     return handler
```

### Comparing `anycorn-0.16.0/src/anycorn/typing.py` & `anycorn-0.17.0/src/anycorn/typing.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,18 @@
 
 from multiprocessing.synchronize import Event as EventType
 from types import TracebackType
 from typing import (
     Any,
     Awaitable,
     Callable,
-    Dict,
     Iterable,
     Literal,
     Optional,
     Protocol,
-    Tuple,
-    Type,
     TypedDict,
     Union,
 )
 
 import h2.events
 import h11
 
@@ -25,47 +22,47 @@
 H11SendableEvent = Union[h11.Data, h11.EndOfMessage, h11.InformationalResponse, h11.Response]
 
 WorkerFunc = Callable[[Config, Optional[Sockets], Optional[EventType]], None]
 
 
 class ASGIVersions(TypedDict, total=False):
     spec_version: str
-    version: Union[Literal["2.0"], Literal["3.0"]]
+    version: Literal["2.0"] | Literal["3.0"]
 
 
 class HTTPScope(TypedDict):
     type: Literal["http"]
     asgi: ASGIVersions
     http_version: str
     method: str
     scheme: str
     path: str
     raw_path: bytes
     query_string: bytes
     root_path: str
-    headers: Iterable[Tuple[bytes, bytes]]
-    client: Optional[Tuple[str, int]]
-    server: Optional[Tuple[str, Optional[int]]]
-    extensions: Dict[str, dict]
+    headers: Iterable[tuple[bytes, bytes]]
+    client: tuple[str, int] | None
+    server: tuple[str, int | None] | None
+    extensions: dict[str, dict]
 
 
 class WebsocketScope(TypedDict):
     type: Literal["websocket"]
     asgi: ASGIVersions
     http_version: str
     scheme: str
     path: str
     raw_path: bytes
     query_string: bytes
     root_path: str
-    headers: Iterable[Tuple[bytes, bytes]]
-    client: Optional[Tuple[str, int]]
-    server: Optional[Tuple[str, Optional[int]]]
+    headers: Iterable[tuple[bytes, bytes]]
+    client: tuple[str, int] | None
+    server: tuple[str, int | None] | None
     subprotocols: Iterable[str]
-    extensions: Dict[str, dict]
+    extensions: dict[str, dict]
 
 
 class LifespanScope(TypedDict):
     type: Literal["lifespan"]
     asgi: ASGIVersions
 
 
@@ -78,27 +75,27 @@
     body: bytes
     more_body: bool
 
 
 class HTTPResponseStartEvent(TypedDict):
     type: Literal["http.response.start"]
     status: int
-    headers: Iterable[Tuple[bytes, bytes]]
+    headers: Iterable[tuple[bytes, bytes]]
 
 
 class HTTPResponseBodyEvent(TypedDict):
     type: Literal["http.response.body"]
     body: bytes
     more_body: bool
 
 
 class HTTPServerPushEvent(TypedDict):
     type: Literal["http.response.push"]
     path: str
-    headers: Iterable[Tuple[bytes, bytes]]
+    headers: Iterable[tuple[bytes, bytes]]
 
 
 class HTTPEarlyHintEvent(TypedDict):
     type: Literal["http.response.early_hint"]
     links: Iterable[bytes]
 
 
@@ -108,34 +105,34 @@
 
 class WebsocketConnectEvent(TypedDict):
     type: Literal["websocket.connect"]
 
 
 class WebsocketAcceptEvent(TypedDict):
     type: Literal["websocket.accept"]
-    subprotocol: Optional[str]
-    headers: Iterable[Tuple[bytes, bytes]]
+    subprotocol: str | None
+    headers: Iterable[tuple[bytes, bytes]]
 
 
 class WebsocketReceiveEvent(TypedDict):
     type: Literal["websocket.receive"]
-    bytes: Optional[bytes]
-    text: Optional[str]
+    bytes: bytes | None
+    text: str | None
 
 
 class WebsocketSendEvent(TypedDict):
     type: Literal["websocket.send"]
-    bytes: Optional[bytes]
-    text: Optional[str]
+    bytes: bytes | None
+    text: str | None
 
 
 class WebsocketResponseStartEvent(TypedDict):
     type: Literal["websocket.http.response.start"]
     status: int
-    headers: Iterable[Tuple[bytes, bytes]]
+    headers: Iterable[tuple[bytes, bytes]]
 
 
 class WebsocketResponseBodyEvent(TypedDict):
     type: Literal["websocket.http.response.body"]
     body: bytes
     more_body: bool
 
@@ -144,15 +141,15 @@
     type: Literal["websocket.disconnect"]
     code: int
 
 
 class WebsocketCloseEvent(TypedDict):
     type: Literal["websocket.close"]
     code: int
-    reason: Optional[str]
+    reason: str | None
 
 
 class LifespanStartupEvent(TypedDict):
     type: Literal["lifespan.startup"]
 
 
 class LifespanShutdownEvent(TypedDict):
@@ -236,16 +233,16 @@
     def close(self) -> None:
         ...
 
     async def handle_request(
         self,
         event: h2.events.RequestReceived,
         scheme: str,
-        client: Tuple[str, int],
-        server: Tuple[str, int],
+        client: tuple[str, int],
+        server: tuple[str, int],
     ) -> None:
         ...
 
 
 class H2AsyncStream(Protocol):
     scope: dict
 
@@ -261,16 +258,16 @@
     async def close(self) -> None:
         ...
 
     async def handle_request(
         self,
         event: h2.events.RequestReceived,
         scheme: str,
-        client: Tuple[str, int],
-        server: Tuple[str, int],
+        client: tuple[str, int],
+        server: tuple[str, int],
     ) -> None:
         ...
 
 
 class Event(Protocol):
     def __init__(self) -> None:
         ...
@@ -285,37 +282,37 @@
         ...
 
     def is_set(self) -> bool:
         ...
 
 
 class WorkerContext(Protocol):
-    event_class: Type[Event]
+    event_class: type[Event]
     terminate: Event
     terminated: Event
 
     async def mark_request(self) -> None:
         ...
 
     @staticmethod
-    async def sleep(wait: Union[float, int]) -> None:
+    async def sleep(wait: float | int) -> None:
         ...
 
     @staticmethod
     def time() -> float:
         ...
 
 
 class TaskGroup(Protocol):
     async def spawn_app(
         self,
         app: AppWrapper,
         config: Config,
         scope: Scope,
-        send: Callable[[Optional[ASGISendEvent]], Awaitable[None]],
+        send: Callable[[ASGISendEvent | None], Awaitable[None]],
     ) -> Callable[[ASGIReceiveEvent], Awaitable[None]]:
         ...
 
     def spawn(self, func: Callable, *args: Any) -> None:
         ...
 
     async def __aenter__(self) -> TaskGroup:
@@ -323,15 +320,15 @@
 
     async def __aexit__(self, exc_type: type, exc_value: BaseException, tb: TracebackType) -> None:
         ...
 
 
 class ResponseSummary(TypedDict):
     status: int
-    headers: Iterable[Tuple[bytes, bytes]]
+    headers: Iterable[tuple[bytes, bytes]]
 
 
 class AppWrapper(Protocol):
     async def __call__(
         self,
         scope: Scope,
         receive: ASGIReceiveCallable,
```

### Comparing `anycorn-0.16.0/src/anycorn/udp_server.py` & `anycorn-0.17.0/src/anycorn/udp_server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from __future__ import annotations
 
 import anyio
 
-from .task_group import TaskGroup
-from .worker_context import WorkerContext
 from .config import Config
 from .events import Event, RawData
+from .task_group import TaskGroup
 from .typing import AppWrapper
 from .utils import parse_socket_addr
-
-MAX_RECV = 2**16
+from .worker_context import WorkerContext
 
 
 class UDPServer:
     def __init__(
         self,
         app: AppWrapper,
         config: Config,
@@ -24,23 +22,26 @@
         self.config = config
         self.context = context
         self.socket = socket
 
     async def run(
         self, *, task_status: anyio.abc.TaskStatus[None] = anyio.TASK_STATUS_IGNORED
     ) -> None:
-        from ..protocol.quic import QuicProtocol  # h3/Quic is an optional part of Anycorn
+        from .protocol.quic import QuicProtocol  # h3/Quic is an optional part of Anycorn
 
         task_status.started()
-        server = parse_socket_addr(self.socket.family, self.socket.getsockname())
+        server = parse_socket_addr(
+            self.socket.extra(anyio.abc.SocketAttribute.raw_socket).family,
+            self.socket.extra(anyio.abc.SocketAttribute.raw_socket).getsockname(),
+        )
         async with TaskGroup() as task_group:
             self.protocol = QuicProtocol(
                 self.app, self.config, self.context, task_group, server, self.protocol_send
             )
 
             while not self.context.terminated.is_set() or not self.protocol.idle:
-                data, address = await self.socket.recvfrom(MAX_RECV)
+                data, address = await self.socket.receive()
                 await self.protocol.handle(RawData(data=data, address=address))
 
     async def protocol_send(self, event: Event) -> None:
         if isinstance(event, RawData):
-            await self.socket.sendto(event.data, event.address)
+            await self.socket.sendto(event.data, event.address[0], event.address[1])
```

### Comparing `anycorn-0.16.0/src/anycorn/utils.py` & `anycorn-0.17.0/src/anycorn/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,25 +5,21 @@
 import socket
 import sys
 from enum import Enum
 from importlib import import_module
 from multiprocessing.synchronize import Event as EventType
 from pathlib import Path
 from typing import (
+    TYPE_CHECKING,
     Any,
     Awaitable,
     Callable,
-    cast,
-    Dict,
     Iterable,
-    List,
     Literal,
-    Optional,
-    Tuple,
-    TYPE_CHECKING,
+    cast,
 )
 
 from .app_wrappers import ASGIWrapper, WSGIWrapper
 from .config import Config
 from .typing import AppWrapper, ASGIFramework, Framework, WSGIFramework
 
 if TYPE_CHECKING:
@@ -60,45 +56,47 @@
     pass
 
 
 def suppress_body(method: str, status_code: int) -> bool:
     return method == "HEAD" or 100 <= status_code < 200 or status_code in {204, 304}
 
 
-def build_and_validate_headers(headers: Iterable[Tuple[bytes, bytes]]) -> List[Tuple[bytes, bytes]]:
+def build_and_validate_headers(
+    headers: Iterable[tuple[bytes, bytes]],
+) -> list[tuple[bytes, bytes]]:
     # Validates that the header name and value are bytes
-    validated_headers: List[Tuple[bytes, bytes]] = []
+    validated_headers: list[tuple[bytes, bytes]] = []
     for name, value in headers:
         if name[0] == b":"[0]:
             raise ValueError("Pseudo headers are not valid")
         validated_headers.append((bytes(name).strip(), bytes(value).strip()))
     return validated_headers
 
 
-def filter_pseudo_headers(headers: List[Tuple[bytes, bytes]]) -> List[Tuple[bytes, bytes]]:
-    filtered_headers: List[Tuple[bytes, bytes]] = [(b"host", b"")]  # Placeholder
+def filter_pseudo_headers(headers: list[tuple[bytes, bytes]]) -> list[tuple[bytes, bytes]]:
+    filtered_headers: list[tuple[bytes, bytes]] = [(b"host", b"")]  # Placeholder
     authority = None
     host = b""
     for name, value in headers:
         if name == b":authority":  # h2 & h3 libraries validate this is present
             authority = value
         elif name == b"host":
             host = value
         elif name[0] != b":"[0]:
             filtered_headers.append((name, value))
     filtered_headers[0] = (b"host", authority if authority is not None else host)
     return filtered_headers
 
 
 def load_application(path: str, wsgi_max_body_size: int) -> AppWrapper:
-    mode: Optional[Literal["asgi", "wsgi"]] = None
+    mode: Literal["asgi", "wsgi"] | None = None
     if ":" not in path:
         module_name, app_name = path, "app"
     elif path.count(":") == 2:
-        mode, module_name, app_name = path.split(":", 2)  # type: ignore
+        mode, module_name, app_name = path.split(":", 2)  # type: ignore[assignment]
         if mode not in {"asgi", "wsgi"}:
             raise ValueError("Invalid mode, must be 'asgi', or 'wsgi'")
     else:
         module_name, app_name = path.split(":", 1)
 
     module_path = Path(module_name).resolve()
     sys.path.insert(0, str(module_path.parent))
@@ -118,39 +116,39 @@
     except NameError:
         raise NoAppError(f"Cannot load application from '{path}', application not found.")
     else:
         return wrap_app(app, wsgi_max_body_size, mode)
 
 
 def wrap_app(
-    app: Framework, wsgi_max_body_size: int, mode: Optional[Literal["asgi", "wsgi"]]
+    app: Framework, wsgi_max_body_size: int, mode: Literal["asgi", "wsgi"] | None
 ) -> AppWrapper:
     if mode is None:
         mode = "asgi" if is_asgi(app) else "wsgi"
     if mode == "asgi":
         return ASGIWrapper(cast(ASGIFramework, app))
     else:
         return WSGIWrapper(cast(WSGIFramework, app), wsgi_max_body_size)
 
 
-def files_to_watch() -> Dict[Path, float]:
-    last_updates: Dict[Path, float] = {}
+def files_to_watch() -> dict[Path, float]:
+    last_updates: dict[Path, float] = {}
     for module in list(sys.modules.values()):
         filename = getattr(module, "__file__", None)
         if filename is None:
             continue
         path = Path(filename)
         try:
             last_updates[Path(filename)] = path.stat().st_mtime
         except (FileNotFoundError, NotADirectoryError):
             pass
     return last_updates
 
 
-def check_for_updates(files: Dict[Path, float]) -> bool:
+def check_for_updates(files: dict[Path, float]) -> bool:
     for path, last_mtime in files.items():
         try:
             mtime = path.stat().st_mtime
         except FileNotFoundError:
             return True
         else:
             if mtime > last_mtime:
@@ -175,15 +173,15 @@
 
 
 def write_pid_file(pid_path: str) -> None:
     with open(pid_path, "w") as file_:
         file_.write(f"{os.getpid()}")
 
 
-def parse_socket_addr(family: int, address: tuple) -> Optional[Tuple[str, int]]:
+def parse_socket_addr(family: int, address: tuple) -> tuple[str, int] | None:
     if family == socket.AF_INET:
         return address
     elif family == socket.AF_INET6:
         return (address[0], address[1])
     else:
         return None
 
@@ -195,15 +193,15 @@
         return f"[{address[0]}]:{address[1]}"
     elif family == socket.AF_UNIX:
         return f"unix:{address}"
     else:
         return f"{address}"
 
 
-def valid_server_name(config: Config, request: "Request") -> bool:
+def valid_server_name(config: Config, request: Request) -> bool:
     if len(config.server_names) == 0:
         return True
 
     host = ""
     for name, value in request.headers:
         if name.lower() == b"host":
             host = value.decode()
```

### Comparing `anycorn-0.16.0/src/anycorn/worker_context.py` & `anycorn-0.17.0/src/anycorn/worker_context.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from __future__ import annotations
 
-from typing import Optional, Type, Union
-
 import anyio
 
 from .typing import Event
 
 
 class EventWrapper:
     def __init__(self) -> None:
@@ -21,30 +19,30 @@
         self._event.set()
 
     def is_set(self) -> bool:
         return self._event.is_set()
 
 
 class WorkerContext:
-    event_class: Type[Event] = EventWrapper
+    event_class: type[Event] = EventWrapper
 
-    def __init__(self, max_requests: Optional[int]) -> None:
+    def __init__(self, max_requests: int | None) -> None:
         self.max_requests = max_requests
         self.requests = 0
         self.terminate = self.event_class()
         self.terminated = self.event_class()
 
     async def mark_request(self) -> None:
         if self.max_requests is None:
             return
 
         self.requests += 1
         if self.requests > self.max_requests:
             await self.terminate.set()
 
     @staticmethod
-    async def sleep(wait: Union[float, int]) -> None:
+    async def sleep(wait: float | int) -> None:
         return await anyio.sleep(wait)
 
     @staticmethod
     def time() -> float:
         return anyio.current_time()
```

