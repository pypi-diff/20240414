# Comparing `tmp/rich-click-1.8.0.dev4.tar.gz` & `tmp/rich_click-1.8.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rich-click-1.8.0.dev4.tar", last modified: Thu Apr 11 00:47:32 2024, max compression
+gzip compressed data, was "rich_click-1.8.0.dev5.tar", last modified: Sat Apr 13 22:29:55 2024, max compression
```

## Comparing `rich-click-1.8.0.dev4.tar` & `rich_click-1.8.0.dev5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:47:32.778461 rich-click-1.8.0.dev4/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-11 00:47:28.000000 rich-click-1.8.0.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-04-11 00:47:32.778461 rich-click-1.8.0.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4256 2024-04-11 00:47:28.000000 rich-click-1.8.0.dev4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-11 00:47:28.000000 rich-click-1.8.0.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 00:47:32.778461 rich-click-1.8.0.dev4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:47:32.770461 rich-click-1.8.0.dev4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:47:32.774461 rich-click-1.8.0.dev4/src/rich_click/
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-11 00:47:28.000000 rich-click-1.8.0.dev4/src/rich_click/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-11 00:47:28.000000 rich-click-1.8.0.dev4/src/rich_click/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-11 00:47:28.000000 rich-click-1.8.0.dev4/src/rich_click/_compat_click.py
--rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-04-11 00:47:28.000000 rich-click-1.8.0.dev4/src/rich_click/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-11 00:47:28.000000 rich-click-1.8.0.dev4/src/rich_click/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-11 00:47:28.000000 rich-click-1.8.0.dev4/src/rich_click/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-11 00:47:28.000000 rich-click-1.8.0.dev4/src/rich_click/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-04-11 00:47:28.000000 rich-click-1.8.0.dev4/src/rich_click/rich_click.py
--rw-r--r--   0 runner    (1001) docker     (127)    15889 2024-04-11 00:47:28.000000 rich-click-1.8.0.dev4/src/rich_click/rich_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-11 00:47:28.000000 rich-click-1.8.0.dev4/src/rich_click/rich_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-11 00:47:28.000000 rich-click-1.8.0.dev4/src/rich_click/rich_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11162 2024-04-11 00:47:28.000000 rich-click-1.8.0.dev4/src/rich_click/rich_help_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-11 00:47:28.000000 rich-click-1.8.0.dev4/src/rich_click/rich_help_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    27415 2024-04-11 00:47:28.000000 rich-click-1.8.0.dev4/src/rich_click/rich_help_rendering.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-11 00:47:28.000000 rich-click-1.8.0.dev4/src/rich_click/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:47:32.774461 rich-click-1.8.0.dev4/src/rich_click.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7428 2024-04-11 00:47:32.000000 rich-click-1.8.0.dev4/src/rich_click.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-11 00:47:32.000000 rich-click-1.8.0.dev4/src/rich_click.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 00:47:32.000000 rich-click-1.8.0.dev4/src/rich_click.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-11 00:47:32.000000 rich-click-1.8.0.dev4/src/rich_click.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-11 00:47:32.000000 rich-click-1.8.0.dev4/src/rich_click.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-11 00:47:32.000000 rich-click-1.8.0.dev4/src/rich_click.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 00:47:32.774461 rich-click-1.8.0.dev4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-11 00:47:28.000000 rich-click-1.8.0.dev4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-11 00:47:28.000000 rich-click-1.8.0.dev4/tests/test_exit_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-04-11 00:47:28.000000 rich-click-1.8.0.dev4/tests/test_help.py
--rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-04-11 00:47:28.000000 rich-click-1.8.0.dev4/tests/test_rich_click_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:29:55.418796 rich_click-1.8.0.dev5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-04-13 22:29:55.418796 rich_click-1.8.0.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 22:29:55.418796 rich_click-1.8.0.dev5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:29:55.410796 rich_click-1.8.0.dev5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:29:55.414796 rich_click-1.8.0.dev5/src/rich_click/
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/_compat_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8741 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/rich_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15889 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/rich_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/rich_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/rich_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11162 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/rich_help_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/rich_help_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29574 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/rich_help_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/src/rich_click/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:29:55.418796 rich_click-1.8.0.dev5/src/rich_click.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-04-13 22:29:55.000000 rich_click-1.8.0.dev5/src/rich_click.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-13 22:29:55.000000 rich_click-1.8.0.dev5/src/rich_click.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 22:29:55.000000 rich_click-1.8.0.dev5/src/rich_click.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-13 22:29:55.000000 rich_click-1.8.0.dev5/src/rich_click.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-13 22:29:55.000000 rich_click-1.8.0.dev5/src/rich_click.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-13 22:29:55.000000 rich_click-1.8.0.dev5/src/rich_click.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:29:55.418796 rich_click-1.8.0.dev5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/tests/test_exit_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18650 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/tests/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2024-04-13 22:29:50.000000 rich_click-1.8.0.dev5/tests/test_rich_click_cli.py
```

### Comparing `rich-click-1.8.0.dev4/LICENSE` & `rich_click-1.8.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev4/PKG-INFO` & `rich_click-1.8.0.dev5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rich-click
-Version: 1.8.0.dev4
+Version: 1.8.0.dev5
 Summary: Format click help output nicely with rich
 Author-email: Phil Ewels <phil@ewels.co.uk>
 Maintainer-email: Phil Ewels <phil@ewels.co.uk>, Daniel Reeves <xdanielreeves@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Phil Ewels
         
@@ -95,15 +95,16 @@
 
 The intention of `rich-click` is to provide attractive help output from
 Click, formatted with Rich, with minimal customisation required.
 
 ## Features
 
 - 🌈 Rich command-line formatting of click help and error messages
-- 💫 Nice styles be default, usage is simply `import rich_click as click`
+- 😌 Same API as Click: usage is simply `import rich_click as click`
+- 💫 Nice styles by default
 - 💻 CLI tool to run on _other people's_ tools (prefix the command with `rich-click`)
 - 📦 Export help text as HTML or SVG
 - 🎁 Group commands and options into named panels
 - ❌ Well formatted error messages
 - 🔢 Easily give custom sort order for options and commands
 - 🎨 Extensive customisation of styling and behaviour possible
 
@@ -138,15 +139,15 @@
 
 ![`python examples/11_hello.py --help`](docs/images/hello.svg)
 
 _Screenshot from [`examples/11_hello.py`](examples/11_hello.py)_
 
 ### More complex example
 
-![examples/03_groups_sorting.py](docs/images/command_groups.svg)
+![`python examples/03_groups_sorting.py`](docs/images/command_groups.svg)
 
 _Screenshot from [`examples/03_groups_sorting.py`](examples/03_groups_sorting.py)_
 
 ## Usage
 
 This is a quick overview of how to use **rich-click**. [Read the docs](https://ewels.github.io/rich-click) for more information.
 
@@ -162,17 +163,26 @@
 
 That's it! ✨ Then continue to use Click as you would normally.
 
 > See [`examples/01_simple.py`](examples/01_simple.py) for an example.
 
 ### Declarative
 
-If you prefer, you can `RichGroup` or `RichCommand` with the `cls` argument in your click usage instead.
+If you prefer, you can use `RichGroup` or `RichCommand` with the `cls` argument in your click usage instead.
 This means that you can continue to use the unmodified `click` package in parallel.
 
+```python
+import click
+from rich_click import RichCommand
+
+@click.command(cls=RichCommand)
+def main():
+    """My amazing tool does all the things."""
+```
+
 > See [`examples/02_declarative.py`](examples/02_declarative.py) for an example.
 
 ### `rich-click` CLI tool
 
 **rich-click** comes with a CLI tool that allows you to format the Click help output from _any_ package that uses Click.
 
 To use, prefix `rich-click` to your normal command.
```

### Comparing `rich-click-1.8.0.dev4/README.md` & `rich_click-1.8.0.dev5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 
 The intention of `rich-click` is to provide attractive help output from
 Click, formatted with Rich, with minimal customisation required.
 
 ## Features
 
 - 🌈 Rich command-line formatting of click help and error messages
-- 💫 Nice styles be default, usage is simply `import rich_click as click`
+- 😌 Same API as Click: usage is simply `import rich_click as click`
+- 💫 Nice styles by default
 - 💻 CLI tool to run on _other people's_ tools (prefix the command with `rich-click`)
 - 📦 Export help text as HTML or SVG
 - 🎁 Group commands and options into named panels
 - ❌ Well formatted error messages
 - 🔢 Easily give custom sort order for options and commands
 - 🎨 Extensive customisation of styling and behaviour possible
 
@@ -71,15 +72,15 @@
 
 ![`python examples/11_hello.py --help`](docs/images/hello.svg)
 
 _Screenshot from [`examples/11_hello.py`](examples/11_hello.py)_
 
 ### More complex example
 
-![examples/03_groups_sorting.py](docs/images/command_groups.svg)
+![`python examples/03_groups_sorting.py`](docs/images/command_groups.svg)
 
 _Screenshot from [`examples/03_groups_sorting.py`](examples/03_groups_sorting.py)_
 
 ## Usage
 
 This is a quick overview of how to use **rich-click**. [Read the docs](https://ewels.github.io/rich-click) for more information.
 
@@ -95,17 +96,26 @@
 
 That's it! ✨ Then continue to use Click as you would normally.
 
 > See [`examples/01_simple.py`](examples/01_simple.py) for an example.
 
 ### Declarative
 
-If you prefer, you can `RichGroup` or `RichCommand` with the `cls` argument in your click usage instead.
+If you prefer, you can use `RichGroup` or `RichCommand` with the `cls` argument in your click usage instead.
 This means that you can continue to use the unmodified `click` package in parallel.
 
+```python
+import click
+from rich_click import RichCommand
+
+@click.command(cls=RichCommand)
+def main():
+    """My amazing tool does all the things."""
+```
+
 > See [`examples/02_declarative.py`](examples/02_declarative.py) for an example.
 
 ### `rich-click` CLI tool
 
 **rich-click** comes with a CLI tool that allows you to format the Click help output from _any_ package that uses Click.
 
 To use, prefix `rich-click` to your normal command.
```

### Comparing `rich-click-1.8.0.dev4/pyproject.toml` & `rich_click-1.8.0.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev4/src/rich_click/__init__.py` & `rich_click-1.8.0.dev5/src/rich_click/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
 rich-click is a minimal Python module to combine the efforts of the excellent packages 'rich' and 'click'.
 
 The intention is to provide attractive help output from Click, formatted with Rich, with minimal
 customisation required.
 """
 
-__version__ = "1.8.0dev4"
+__version__ = "1.8.0dev5"
 
 # Import the entire click API here.
 # We need to manually import these instead of `from click import *` to force
 # mypy to recognize a few type annotation overrides for the rich_click decorators.
 from click.core import Argument as Argument
 from click.core import Command as Command
 from click.core import CommandCollection as CommandCollection
```

### Comparing `rich-click-1.8.0.dev4/src/rich_click/_compat_click.py` & `rich_click-1.8.0.dev5/src/rich_click/_compat_click.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev4/src/rich_click/cli.py` & `rich_click-1.8.0.dev5/src/rich_click/cli.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev4/src/rich_click/decorators.py` & `rich_click-1.8.0.dev5/src/rich_click/decorators.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev4/src/rich_click/patch.py` & `rich_click-1.8.0.dev5/src/rich_click/patch.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev4/src/rich_click/rich_click.py` & `rich_click-1.8.0.dev5/src/rich_click/rich_click.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev4/src/rich_click/rich_command.py` & `rich_click-1.8.0.dev5/src/rich_click/rich_command.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev4/src/rich_click/rich_context.py` & `rich_click-1.8.0.dev5/src/rich_click/rich_context.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev4/src/rich_click/rich_help_configuration.py` & `rich_click-1.8.0.dev5/src/rich_click/rich_help_configuration.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev4/src/rich_click/rich_help_formatter.py` & `rich_click-1.8.0.dev5/src/rich_click/rich_help_formatter.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev4/src/rich_click/rich_help_rendering.py` & `rich_click-1.8.0.dev5/src/rich_click/rich_help_rendering.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import inspect
 import re
-from typing import TYPE_CHECKING, Iterable, List, Optional, Tuple, Union
+from fnmatch import fnmatch
+from typing import TYPE_CHECKING, Dict, Iterable, List, Optional, Tuple, TypeVar, Union, overload
 
 import click
 
 # Due to how rich_click.cli.patch() works, it is safer to import Command types directly
 # rather than use the click module e.g. click.Command
 from click import Command, Group
 from rich import box
@@ -15,18 +16,19 @@
 from rich.highlighter import RegexHighlighter
 from rich.markdown import Markdown
 from rich.padding import Padding
 from rich.panel import Panel
 from rich.style import StyleType
 from rich.table import Table
 from rich.text import Text
+from typing_extensions import Literal
 
 from rich_click._compat_click import CLICK_IS_BEFORE_VERSION_8X, CLICK_IS_BEFORE_VERSION_9X, CLICK_IS_VERSION_80
 from rich_click.rich_help_formatter import RichHelpFormatter
-from rich_click.utils import OptionGroupDict
+from rich_click.utils import CommandGroupDict, OptionGroupDict
 
 
 # Support rich <= 10.6.0
 try:
     from rich.console import group
 except ImportError:
     from rich.console import render_group as group  # type: ignore[attr-defined,no-redef]
@@ -344,24 +346,76 @@
             Padding(
                 Align(_get_help_text(self, formatter), pad=False),
                 (0, 1, 1, 1),
             )
         )
 
 
+GroupType = TypeVar("GroupType", OptionGroupDict, CommandGroupDict)
+
+
+@overload
+def _resolve_groups(
+    ctx: click.Context, groups: Dict[str, List[OptionGroupDict]], group_attribute: Literal["options"]
+) -> List[OptionGroupDict]: ...
+
+
+@overload
+def _resolve_groups(
+    ctx: click.Context, groups: Dict[str, List[CommandGroupDict]], group_attribute: Literal["commands"]
+) -> List[CommandGroupDict]: ...
+
+
+def _resolve_groups(
+    ctx: click.Context, groups: Dict[str, List[GroupType]], group_attribute: Literal["commands", "options"]
+) -> List[GroupType]:
+    """Logic for resolving the groups."""
+    cmd_name = ctx.command.name
+    _ctx = ctx
+    while _ctx.parent is not None:
+        _ctx = _ctx.parent
+        cmd_name = f"{_ctx.command.name} {cmd_name}"
+    # 'command_path' is sometimes the file name, e.g. hello.py.
+    # We also want to make sure that the actual command name is supported as well.
+    if cmd_name != ctx.command_path:
+        paths = [cmd_name, ctx.command_path]
+    else:
+        paths = [cmd_name]
+    final_groups_list: List[GroupType] = []
+
+    # Assign wildcards, but make sure we do not overwrite anything already defined.
+    for _path in paths:
+        for mtch in reversed(sorted([_ for _ in groups if fnmatch(_path, _)])):
+            wildcard_option_groups = groups[mtch]
+            for grp in wildcard_option_groups:
+                grp = grp.copy()
+                opts = grp.get(group_attribute, []).copy()  # type: ignore[attr-defined]
+                for opt in grp.get(group_attribute, []):  # type: ignore[attr-defined]
+                    if opt in [
+                        _opt
+                        for _grp in final_groups_list
+                        for _opt in _grp.get(group_attribute, [])  # type: ignore[attr-defined]
+                    ]:
+                        opts.remove(opt)
+                grp[group_attribute] = opts  # type: ignore[typeddict-unknown-key]
+                final_groups_list.append(grp)
+
+    final_groups_list.append({group_attribute: []})  # type: ignore[misc]
+    return final_groups_list
+
+
 def get_rich_options(
     obj: Command,
     ctx: click.Context,
     formatter: RichHelpFormatter,
 ) -> None:
     """Richly render a click Command's options."""
     # Look through config.option_groups for this command
     # stick anything unmatched into a default group at the end
-    option_groups = formatter.config.option_groups.get(ctx.command_path, []).copy()
-    option_groups.append({"options": []})
+    option_groups = _resolve_groups(ctx=ctx, groups=formatter.config.option_groups, group_attribute="options")
     argument_group_options = []
 
     for param in obj.get_params(ctx):
         # Skip positional arguments - they don't have opts or helptext and are covered in usage
         # See https://click.palletsprojects.com/en/8.0.x/documentation/#documenting-arguments
         if isinstance(param, click.core.Argument) and not formatter.config.show_arguments:
             continue
@@ -523,16 +577,15 @@
 ) -> None:
     """Richly render a click Command's options."""
     # Look through config.option_groups for this command
     # stick anything unmatched into a default group at the end
 
     # Look through COMMAND_GROUPS for this command
     # stick anything unmatched into a default group at the end
-    cmd_groups = formatter.config.command_groups.get(ctx.command_path, []).copy()
-    cmd_groups.append({"commands": []})
+    cmd_groups = _resolve_groups(ctx=ctx, groups=formatter.config.command_groups, group_attribute="commands")
     for command in obj.list_commands(ctx):
         for cmd_group in cmd_groups:
             if command in cmd_group.get("commands", []):
                 break
         else:
             commands = cmd_groups[-1]["commands"]
             commands.append(command)
```

### Comparing `rich-click-1.8.0.dev4/src/rich_click/utils.py` & `rich_click-1.8.0.dev5/src/rich_click/utils.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev4/src/rich_click.egg-info/PKG-INFO` & `rich_click-1.8.0.dev5/src/rich_click.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rich-click
-Version: 1.8.0.dev4
+Version: 1.8.0.dev5
 Summary: Format click help output nicely with rich
 Author-email: Phil Ewels <phil@ewels.co.uk>
 Maintainer-email: Phil Ewels <phil@ewels.co.uk>, Daniel Reeves <xdanielreeves@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Phil Ewels
         
@@ -95,15 +95,16 @@
 
 The intention of `rich-click` is to provide attractive help output from
 Click, formatted with Rich, with minimal customisation required.
 
 ## Features
 
 - 🌈 Rich command-line formatting of click help and error messages
-- 💫 Nice styles be default, usage is simply `import rich_click as click`
+- 😌 Same API as Click: usage is simply `import rich_click as click`
+- 💫 Nice styles by default
 - 💻 CLI tool to run on _other people's_ tools (prefix the command with `rich-click`)
 - 📦 Export help text as HTML or SVG
 - 🎁 Group commands and options into named panels
 - ❌ Well formatted error messages
 - 🔢 Easily give custom sort order for options and commands
 - 🎨 Extensive customisation of styling and behaviour possible
 
@@ -138,15 +139,15 @@
 
 ![`python examples/11_hello.py --help`](docs/images/hello.svg)
 
 _Screenshot from [`examples/11_hello.py`](examples/11_hello.py)_
 
 ### More complex example
 
-![examples/03_groups_sorting.py](docs/images/command_groups.svg)
+![`python examples/03_groups_sorting.py`](docs/images/command_groups.svg)
 
 _Screenshot from [`examples/03_groups_sorting.py`](examples/03_groups_sorting.py)_
 
 ## Usage
 
 This is a quick overview of how to use **rich-click**. [Read the docs](https://ewels.github.io/rich-click) for more information.
 
@@ -162,17 +163,26 @@
 
 That's it! ✨ Then continue to use Click as you would normally.
 
 > See [`examples/01_simple.py`](examples/01_simple.py) for an example.
 
 ### Declarative
 
-If you prefer, you can `RichGroup` or `RichCommand` with the `cls` argument in your click usage instead.
+If you prefer, you can use `RichGroup` or `RichCommand` with the `cls` argument in your click usage instead.
 This means that you can continue to use the unmodified `click` package in parallel.
 
+```python
+import click
+from rich_click import RichCommand
+
+@click.command(cls=RichCommand)
+def main():
+    """My amazing tool does all the things."""
+```
+
 > See [`examples/02_declarative.py`](examples/02_declarative.py) for an example.
 
 ### `rich-click` CLI tool
 
 **rich-click** comes with a CLI tool that allows you to format the Click help output from _any_ package that uses Click.
 
 To use, prefix `rich-click` to your normal command.
```

### Comparing `rich-click-1.8.0.dev4/src/rich_click.egg-info/SOURCES.txt` & `rich_click-1.8.0.dev5/src/rich_click.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev4/tests/test_config.py` & `rich_click-1.8.0.dev5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev4/tests/test_exit_code.py` & `rich_click-1.8.0.dev5/tests/test_exit_code.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev4/tests/test_help.py` & `rich_click-1.8.0.dev5/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `rich-click-1.8.0.dev4/tests/test_rich_click_cli.py` & `rich_click-1.8.0.dev5/tests/test_rich_click_cli.py`

 * *Files identical despite different names*

