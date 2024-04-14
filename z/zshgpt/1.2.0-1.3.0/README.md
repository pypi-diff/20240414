# Comparing `tmp/zshgpt-1.2.0.tar.gz` & `tmp/zshgpt-1.3.0.tar.gz`

## Comparing `zshgpt-1.2.0.tar` & `zshgpt-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,30 @@
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 zshgpt-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    70626 2020-02-02 00:00:00.000000 zshgpt-1.2.0/Peek 2023-07-17 17-27.gif
--rw-r--r--   0        0        0    99423 2020-02-02 00:00:00.000000 zshgpt-1.2.0/Screenshot_1_0_1.png
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 zshgpt-1.2.0/cicd_plan.md
--rw-r--r--   0        0        0    75940 2020-02-02 00:00:00.000000 zshgpt-1.2.0/icon.png
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 zshgpt-1.2.0/zshgpt.plugin.zsh
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 zshgpt-1.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 zshgpt-1.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 zshgpt-1.2.0/snap/snapcraft.yaml
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 zshgpt-1.2.0/src/zshgpt/__about__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-1.2.0/src/zshgpt/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 zshgpt-1.2.0/src/zshgpt/__main__.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 zshgpt-1.2.0/src/zshgpt/cli/__init__.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 zshgpt-1.2.0/src/zshgpt/util/chat_util.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 zshgpt-1.2.0/src/zshgpt/util/messages.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-1.2.0/tests/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 zshgpt-1.2.0/tests/test_chat_util.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 zshgpt-1.2.0/tests/test_invalid_key.py
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 zshgpt-1.2.0/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 zshgpt-1.2.0/LICENSE
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 zshgpt-1.2.0/LICENSE.txt
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 zshgpt-1.2.0/README.md
--rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 zshgpt-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     4181 2020-02-02 00:00:00.000000 zshgpt-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 zshgpt-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    70626 2020-02-02 00:00:00.000000 zshgpt-1.3.0/Peek 2023-07-17 17-27.gif
+-rw-r--r--   0        0        0    99423 2020-02-02 00:00:00.000000 zshgpt-1.3.0/Screenshot_1_0_1.png
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 zshgpt-1.3.0/cicd_plan.md
+-rw-r--r--   0        0        0    75940 2020-02-02 00:00:00.000000 zshgpt-1.3.0/icon.png
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 zshgpt-1.3.0/zshgpt.plugin.zsh
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 zshgpt-1.3.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 zshgpt-1.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 zshgpt-1.3.0/snap/snapcraft.yaml
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 zshgpt-1.3.0/src/zshgpt/__about__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-1.3.0/src/zshgpt/__init__.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 zshgpt-1.3.0/src/zshgpt/__main__.py
+-rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 zshgpt-1.3.0/src/zshgpt/settings.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 zshgpt-1.3.0/src/zshgpt/cli/__init__.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 zshgpt-1.3.0/src/zshgpt/util/assistant.py
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 zshgpt-1.3.0/src/zshgpt/util/chat_util.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 zshgpt-1.3.0/src/zshgpt/util/client.py
+-rw-r--r--   0        0        0     2171 2020-02-02 00:00:00.000000 zshgpt-1.3.0/src/zshgpt/util/messages.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 zshgpt-1.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 zshgpt-1.3.0/tests/test_chat_util.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 zshgpt-1.3.0/tests/test_create_assistant.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 zshgpt-1.3.0/tests/test_invalid_key.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 zshgpt-1.3.0/tests/test_send_message.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 zshgpt-1.3.0/~/.zshgpt/config.json
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 zshgpt-1.3.0/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 zshgpt-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 zshgpt-1.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 zshgpt-1.3.0/README.md
+-rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 zshgpt-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 zshgpt-1.3.0/PKG-INFO
```

### Comparing `zshgpt-1.2.0/Peek 2023-07-17 17-27.gif` & `zshgpt-1.3.0/Peek 2023-07-17 17-27.gif`

 * *Files identical despite different names*

### Comparing `zshgpt-1.2.0/Screenshot_1_0_1.png` & `zshgpt-1.3.0/Screenshot_1_0_1.png`

 * *Files identical despite different names*

### Comparing `zshgpt-1.2.0/icon.png` & `zshgpt-1.3.0/icon.png`

 * *Files identical despite different names*

### Comparing `zshgpt-1.2.0/zshgpt.plugin.zsh` & `zshgpt-1.3.0/zshgpt.plugin.zsh`

 * *Files identical despite different names*

### Comparing `zshgpt-1.2.0/.github/workflows/release.yml` & `zshgpt-1.3.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `zshgpt-1.2.0/.github/workflows/test.yml` & `zshgpt-1.3.0/.github/workflows/test.yml`

 * *Files 1% similar despite different names*

```diff
@@ -32,8 +32,8 @@
     - name: Install Hatch
       run: pip install --upgrade hatch
 
     - name: Lint test
       run: hatch run lint:style
 
     - name: Run tests
-      run: hatch run cov
+      run: hatch run cli_test
```

### Comparing `zshgpt-1.2.0/src/zshgpt/cli/__init__.py` & `zshgpt-1.3.0/src/zshgpt/cli/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 # SPDX-FileCopyrightText: 2023-present Anders Steen <asteennilsen@gmail.com
 #
 # SPDX-License-Identifier: MIT
 import click
 from openai import AuthenticationError
 
 from zshgpt.__about__ import __version__
+from zshgpt.util.assistant import send_message
 
 
 @click.group(context_settings={'help_option_names': ['-h', '--help']}, invoke_without_command=True)
 @click.version_option(version=__version__, prog_name='zshgpt')
 @click.argument('user_query')
 def zshgpt(user_query: str) -> str:
-    from zshgpt.util.chat_util import get_message
-
     try:
-        message = get_message(user_query)
+        response: str = send_message(user_query)
     except AuthenticationError as auth_error:
         raise click.ClickException(auth_error.message) from auth_error
-    click.echo(message.content, nl=False)
+    click.echo(response)
```

### Comparing `zshgpt-1.2.0/src/zshgpt/util/chat_util.py` & `zshgpt-1.3.0/src/zshgpt/util/chat_util.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def model_selection(user_query: str) -> str:
     match user_query.strip()[:2]:
         case '#':
             return 'gpt-3.5-turbo'
         case '##':
-            return 'gpt-4'
+            return 'gpt-4-turbo'
         case _:
             return 'gpt-3.5-turbo'
 
 
 def get_message(user_query: str) -> str:
     client = OpenAI()
     model = model_selection(user_query)
```

### Comparing `zshgpt-1.2.0/.gitignore` & `zshgpt-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `zshgpt-1.2.0/LICENSE` & `zshgpt-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zshgpt-1.2.0/LICENSE.txt` & `zshgpt-1.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zshgpt-1.2.0/README.md` & `zshgpt-1.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 
 [![PyPI - Version](https://img.shields.io/pypi/v/zshgpt.svg)](https://pypi.org/project/zshgpt)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/zshgpt.svg)](https://pypi.org/project/zshgpt)
 [![zshgpt](https://snapcraft.io/zshgpt/badge.svg)](https://snapcraft.io/zshgpt)
-
+[![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
+[![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 # zshgpt
 
 -----
 
 **Table of Contents**
 
 - [About](#about)
@@ -20,15 +21,15 @@
 
 Heavily inspired by the abandoned project [https://github.com/microsoft/Codex-CLI](https://github.com/microsoft/Codex-CLI)
 Made into a oh-my-zsh plugin.
 
 In your zsh console, type a question, starting with comment sign `#`, hit `ctrl+g` and get an answer.
 
 > [!TIP]
-> New in v. 1.1.1 Use doble `##` to use gpt-4 model.
+> New in v. 1.2.0 Use doble `##` to use gpt-4 model.
 
 ```bash
 # Who edited README.MD last according to git history?
 ```
 ChatGPT will then answer with e.g.:
 ```bash
 git log -1 --format="%an" README.md
@@ -123,14 +124,21 @@
 `~/.zshrc`
 ```
 ...
 zplug "AndersSteenNilsen/zshgpt"
 zplug load
 ```
 
+## Dev setup
+
+* `pipx install hatch` More information: [https://hatch.pypa.io/dev/install/](https://hatch.pypa.io/dev/install/)
+* `hatch shell`
+    * You now should have everything installed.
+
+
 ## LOGO
 *Made with DALL-E*
 
 ![Icon](icon.png)
 ## License
 
 `zshgpt` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

### Comparing `zshgpt-1.2.0/pyproject.toml` & `zshgpt-1.3.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -6,75 +6,62 @@
 name = "zshgpt"
 dynamic = ["version"]
 description = 'Level up z shell with GPT'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = []
-authors = [
-  { name = "Anders Steen", email = "asteennilsen@gmail.com" },
-]
+authors = [{ name = "Anders Steen", email = "asteennilsen@gmail.com" }]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "License :: OSI Approved :: MIT License",
   "Framework :: Hatch",
-  "Topic :: Utilities"
-]
-dependencies = [
-  "click", "openai"
+  "Topic :: Utilities",
 ]
+dependencies = ["click", "openai~=1.2.4", "pydantic-settings"]
 
 [project.urls]
 Documentation = "https://github.com/AndersSteenNilsen/zshgpt#readme"
 Issues = "https://github.com/AndersSteenNilsen/zshgpt/issues"
 Source = "https://github.com/AndersSteenNilsen/zshgpt"
 
 [project.scripts]
 zshgpt = "zshgpt.cli:zshgpt"
 
 [tool.hatch.envs.default]
-dependencies = [
-  "coverage[toml]>=6.5",
-  "pytest",
-  "pre-commit"
-]
+dependencies = ["coverage[toml]>=6.5", "pytest", "pre-commit", "pytest-env"]
+
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
-cov-report = [
-  "- coverage combine",
-  "coverage report",
-]
-cov = [
-  "test-cov",
-  "cov-report",
-]
+cov-report = ["- coverage combine", "coverage report"]
+cov = ["test-cov", "cov-report"]
+cli_test = "pytest {args:tests} -m \"not need_OPENAI_API_KEY\""
 
 [[tool.hatch.envs.all.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
 
 [tool.hatch.version]
 # path = "src/zshgpt/__about__.py"
 source = "vcs"
 
 [tool.hatch.build.hooks.vcs]
 version-file = "src/zshgpt/__about__.py"
 
 [tool.hatch.build.targets.app]
 
-
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
   "mypy>=1.0.0",
   "ruff>=0.2.2",
 ]
 [tool.hatch.envs.lint.scripts]
@@ -88,18 +75,31 @@
   "style",
 ]
 all = [
   "style",
   "typing",
 ]
 
+[tool.pytest.ini_options]
+markers = [
+  "need_OPENAI_API_KEY: Test needs an OPENAI_API_KEY to work, do not run in CI/CD."
+]
+env = [
+  "OPENAI_API_KEY=WrongKey",
+]
+
 [tool.ruff]
 target-version = "py38"
 line-length = 120
-lint.select = [
+
+[tool.ruff.format]
+quote-style = "single"
+
+[tool.ruff.lint]
+select = [
   "A",
   "ARG",
   "B",
   "C",
   "DTZ",
   "E",
   "EM",
@@ -118,56 +118,48 @@
   "S",
   "T",
   "TID",
   "UP",
   "W",
   "YTT",
 ]
-lint.ignore = [
+ignore = [
   # Allow non-abstract empty methods in abstract base classes
   "B027",
   # Allow boolean positional values in function calls, like `dict.get(... True)`
   "FBT003",
   # Ignore checks for possible passwords
-  "S105", "S106", "S107",
+  "S105",
+  "S106",
+  "S107",
   # Ignore complexity
-  "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
+  "C901",
+  "PLR0911",
+  "PLR0912",
+  "PLR0913",
+  "PLR0915",
 ]
-lint.unfixable = [
+unfixable = [
   # Don't touch unused imports
-  "F401",
+  # "F401",
 ]
-
-[tool.ruff.format]
-quote-style = "single"
-
-[tool.ruff.lint.isort]
-known-first-party = ["zshgpt"]
-
-[tool.ruff.lint.flake8-tidy-imports]
-ban-relative-imports = "all"
-
-[tool.ruff.lint.flake8-quotes]
-inline-quotes = "single"
+isort.known-first-party = ["zshgpt"]
+flake8-tidy-imports.ban-relative-imports = "all"
+flake8-quotes.inline-quotes = "single"
 
 [tool.ruff.lint.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
+"src/zshgpt/settings.py" = ["ARG", "FBT001"]
 
 [tool.coverage.run]
 source_pkgs = ["zshgpt", "tests"]
 branch = true
 parallel = true
-omit = [
-  "src/zshgpt/__about__.py",
-]
+omit = ["src/zshgpt/__about__.py"]
 
 [tool.coverage.paths]
 zshgpt = ["src/zshgpt", "*/zshgpt/src/zshgpt"]
 tests = ["tests", "*/zshgpt/tests"]
 
 [tool.coverage.report]
-exclude_lines = [
-  "no cov",
-  "if __name__ == .__main__.:",
-  "if TYPE_CHECKING:",
-]
+exclude_lines = ["no cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:"]
```

### Comparing `zshgpt-1.2.0/PKG-INFO` & `zshgpt-1.3.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: zshgpt
-Version: 1.2.0
+Version: 1.3.0
 Summary: Level up z shell with GPT
 Project-URL: Documentation, https://github.com/AndersSteenNilsen/zshgpt#readme
 Project-URL: Issues, https://github.com/AndersSteenNilsen/zshgpt/issues
 Project-URL: Source, https://github.com/AndersSteenNilsen/zshgpt
 Author-email: Anders Steen <asteennilsen@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -19,22 +19,24 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Requires-Dist: click
-Requires-Dist: openai
+Requires-Dist: openai~=1.2.4
+Requires-Dist: pydantic-settings
 Description-Content-Type: text/markdown
 
 
 [![PyPI - Version](https://img.shields.io/pypi/v/zshgpt.svg)](https://pypi.org/project/zshgpt)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/zshgpt.svg)](https://pypi.org/project/zshgpt)
 [![zshgpt](https://snapcraft.io/zshgpt/badge.svg)](https://snapcraft.io/zshgpt)
-
+[![Hatch project](https://img.shields.io/badge/%F0%9F%A5%9A-Hatch-4051b5.svg)](https://github.com/pypa/hatch)
+[![linting - Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 # zshgpt
 
 -----
 
 **Table of Contents**
 
 - [About](#about)
@@ -48,15 +50,15 @@
 
 Heavily inspired by the abandoned project [https://github.com/microsoft/Codex-CLI](https://github.com/microsoft/Codex-CLI)
 Made into a oh-my-zsh plugin.
 
 In your zsh console, type a question, starting with comment sign `#`, hit `ctrl+g` and get an answer.
 
 > [!TIP]
-> New in v. 1.1.1 Use doble `##` to use gpt-4 model.
+> New in v. 1.2.0 Use doble `##` to use gpt-4 model.
 
 ```bash
 # Who edited README.MD last according to git history?
 ```
 ChatGPT will then answer with e.g.:
 ```bash
 git log -1 --format="%an" README.md
@@ -151,14 +153,21 @@
 `~/.zshrc`
 ```
 ...
 zplug "AndersSteenNilsen/zshgpt"
 zplug load
 ```
 
+## Dev setup
+
+* `pipx install hatch` More information: [https://hatch.pypa.io/dev/install/](https://hatch.pypa.io/dev/install/)
+* `hatch shell`
+    * You now should have everything installed.
+
+
 ## LOGO
 *Made with DALL-E*
 
 ![Icon](icon.png)
 ## License
 
 `zshgpt` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
```

