# Comparing `tmp/configparser-6.0.1.tar.gz` & `tmp/configparser-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configparser-6.0.1.tar", last modified: Sat Feb 24 16:33:15 2024, max compression
+gzip compressed data, was "configparser-7.0.0.tar", last modified: Sun Apr 14 15:59:00 2024, max compression
```

## Comparing `configparser-6.0.1.tar` & `configparser-7.0.0.tar`

### file list

```diff
@@ -1,48 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:33:15.682887 configparser-6.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-24 16:32:50.000000 configparser-6.0.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-24 16:32:50.000000 configparser-6.0.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:33:15.678887 configparser-6.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-24 16:32:50.000000 configparser-6.0.1/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-24 16:32:50.000000 configparser-6.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:33:15.678887 configparser-6.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-02-24 16:32:50.000000 configparser-6.0.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-24 16:32:50.000000 configparser-6.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-24 16:32:50.000000 configparser-6.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-02-24 16:32:50.000000 configparser-6.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-02-24 16:32:50.000000 configparser-6.0.1/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10791 2024-02-24 16:33:15.682887 configparser-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9357 2024-02-24 16:32:50.000000 configparser-6.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-24 16:32:50.000000 configparser-6.0.1/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:33:15.674887 configparser-6.0.1/backports/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:33:15.678887 configparser-6.0.1/backports/configparser/
--rw-r--r--   0 runner    (1001) docker     (127)    53363 2024-02-24 16:32:50.000000 configparser-6.0.1/backports/configparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-02-24 16:32:50.000000 configparser-6.0.1/backports/configparser/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:33:15.678887 configparser-6.0.1/configparser/
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-02-24 16:32:50.000000 configparser-6.0.1/configparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:33:15.678887 configparser-6.0.1/configparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10791 2024-02-24 16:33:15.000000 configparser-6.0.1/configparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-02-24 16:33:15.000000 configparser-6.0.1/configparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-24 16:33:15.000000 configparser-6.0.1/configparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-02-24 16:33:15.000000 configparser-6.0.1/configparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-24 16:33:15.000000 configparser-6.0.1/configparser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    50659 2024-02-24 16:32:50.000000 configparser-6.0.1/configparser.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-24 16:32:50.000000 configparser-6.0.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:33:15.678887 configparser-6.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-02-24 16:32:50.000000 configparser-6.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-24 16:32:50.000000 configparser-6.0.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-02-24 16:32:50.000000 configparser-6.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-24 16:32:50.000000 configparser-6.0.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-24 16:32:50.000000 configparser-6.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-02-24 16:32:50.000000 configparser-6.0.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-02-24 16:32:50.000000 configparser-6.0.1/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-02-24 16:33:15.682887 configparser-6.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-24 16:32:50.000000 configparser-6.0.1/tea.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 16:33:15.678887 configparser-6.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-24 16:32:50.000000 configparser-6.0.1/tests/cfgparser.1
--rw-r--r--   0 runner    (1001) docker     (127)    19472 2024-02-24 16:32:50.000000 configparser-6.0.1/tests/cfgparser.2
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-02-24 16:32:50.000000 configparser-6.0.1/tests/cfgparser.3
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-02-24 16:32:50.000000 configparser-6.0.1/tests/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-02-24 16:32:50.000000 configparser-6.0.1/tests/test_backport.py
--rw-r--r--   0 runner    (1001) docker     (127)    87725 2024-02-24 16:32:50.000000 configparser-6.0.1/tests/test_configparser.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-24 16:32:50.000000 configparser-6.0.1/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-02-24 16:32:50.000000 configparser-6.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:59:00.475168 configparser-7.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-14 15:58:44.000000 configparser-7.0.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-14 15:58:44.000000 configparser-7.0.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:59:00.471168 configparser-7.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-14 15:58:44.000000 configparser-7.0.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-14 15:58:44.000000 configparser-7.0.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:59:00.471168 configparser-7.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-14 15:58:44.000000 configparser-7.0.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-14 15:58:44.000000 configparser-7.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-14 15:58:44.000000 configparser-7.0.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-14 15:58:44.000000 configparser-7.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5745 2024-04-14 15:58:44.000000 configparser-7.0.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-14 15:59:00.475168 configparser-7.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-14 15:58:44.000000 configparser-7.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-14 15:58:44.000000 configparser-7.0.0/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:59:00.467168 configparser-7.0.0/backports/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:59:00.471168 configparser-7.0.0/backports/configparser/
+-rw-r--r--   0 runner    (1001) docker     (127)    54208 2024-04-14 15:58:44.000000 configparser-7.0.0/backports/configparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-14 15:58:44.000000 configparser-7.0.0/backports/configparser/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:59:00.475168 configparser-7.0.0/configparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-04-14 15:59:00.000000 configparser-7.0.0/configparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-14 15:59:00.000000 configparser-7.0.0/configparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 15:59:00.000000 configparser-7.0.0/configparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-14 15:59:00.000000 configparser-7.0.0/configparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 15:59:00.000000 configparser-7.0.0/configparser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:59:00.475168 configparser-7.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-14 15:58:44.000000 configparser-7.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-14 15:58:44.000000 configparser-7.0.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-14 15:58:44.000000 configparser-7.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-14 15:58:44.000000 configparser-7.0.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-14 15:58:44.000000 configparser-7.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-14 15:58:44.000000 configparser-7.0.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-14 15:58:44.000000 configparser-7.0.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-14 15:59:00.475168 configparser-7.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-14 15:58:44.000000 configparser-7.0.0/tea.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:59:00.475168 configparser-7.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-14 15:58:44.000000 configparser-7.0.0/tests/cfgparser.1
+-rw-r--r--   0 runner    (1001) docker     (127)    19472 2024-04-14 15:58:44.000000 configparser-7.0.0/tests/cfgparser.2
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-14 15:58:44.000000 configparser-7.0.0/tests/cfgparser.3
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-14 15:58:44.000000 configparser-7.0.0/tests/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-14 15:58:44.000000 configparser-7.0.0/tests/test_backport.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88793 2024-04-14 15:58:44.000000 configparser-7.0.0/tests/test_configparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-14 15:58:44.000000 configparser-7.0.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-14 15:58:44.000000 configparser-7.0.0/tox.ini
```

### Comparing `configparser-6.0.1/.github/workflows/main.yml` & `configparser-7.0.0/.github/workflows/main.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 name: tests
 
 on:
   merge_group:
   push:
     branches-ignore:
-    # disabled for jaraco/skeleton#103
-    # - gh-readonly-queue/**  # Temporary merge queue-related GH-made branches
+    # temporary GH branches relating to merge queues (jaraco/skeleton#93)
+    - gh-readonly-queue/**
+    tags:
+    # required if branches-ignore is supplied (jaraco/skeleton#103)
+    - '**'
   pull_request:
 
 permissions:
   contents: read
 
 env:
   # Environment variable to support color support (jaraco/skeleton#66)
@@ -24,28 +27,30 @@
   TOX_OVERRIDE: >-
     testenv.pass_env+=GITHUB_*,FORCE_COLOR
 
 
 jobs:
   test:
     strategy:
+      # https://blog.jaraco.com/efficient-use-of-ci-resources/
       matrix:
         python:
         - "3.8"
-        - "3.11"
         - "3.12"
         platform:
         - ubuntu-latest
         - macos-latest
         - windows-latest
         include:
         - python: "3.9"
           platform: ubuntu-latest
         - python: "3.10"
           platform: ubuntu-latest
+        - python: "3.11"
+          platform: ubuntu-latest
         - python: pypy3.10
           platform: ubuntu-latest
     runs-on: ${{ matrix.platform }}
     continue-on-error: ${{ matrix.python == '3.13' }}
     steps:
       - uses: actions/checkout@v4
       - name: Setup Python
```

### Comparing `configparser-6.0.1/LICENSE` & `configparser-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `configparser-6.0.1/NEWS.rst` & `configparser-7.0.0/NEWS.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+v7.0.0
+======
+
+Deprecations and Removals
+-------------------------
+
+- Refreshed with implementation from CPython 3.13.0a6.
+- Remove 'configparser' as a top-level name, as it's already masked by the stdlib on all supported Pythons.
+
+
 v6.0.1
 ======
 
 Bugfixes
 --------
 
 - Fixed failing tests introduced by upstream test suite changes. (#70)
```

### Comparing `configparser-6.0.1/backports/configparser/__init__.py` & `configparser-7.0.0/backports/configparser/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
     methods:
 
     __init__(defaults=None, dict_type=_default_dict, allow_no_value=False,
              delimiters=('=', ':'), comment_prefixes=('#', ';'),
              inline_comment_prefixes=None, strict=True,
              empty_lines_in_values=True, default_section='DEFAULT',
-             interpolation=<unset>, converters=<unset>):
-
+             interpolation=<unset>, converters=<unset>,
+             allow_unnamed_section=False):
         Create the parser. When `defaults` is given, it is initialized into the
         dictionary or intrinsic defaults. The keys must be strings, the values
         must be appropriate for %()s string interpolation.
 
         When `dict_type` is given, it will be used to create the dictionary
         objects for the list of sections, for the options within a section, and
         for the default values.
@@ -64,14 +64,18 @@
 
         When `converters` is given, it should be a dictionary where each key
         represents the name of a type converter and each value is a callable
         implementing the conversion from string to the desired datatype. Every
         converter gets its corresponding get*() method on the parser object and
         section proxies.
 
+        When `allow_unnamed_section` is True (default: False), options
+        without section are accepted: the section for these is
+        ``configparser.UNNAMED_SECTION``.
+
     sections()
         Return all the configuration section names, sans DEFAULT.
 
     has_section(section)
         Return whether the given section exists.
 
     has_option(section, option)
@@ -135,46 +139,50 @@
 
     write(fp, space_around_delimiters=True)
         Write the configuration state in .ini format. If
         `space_around_delimiters` is True (the default), delimiters
         between keys and values are surrounded by spaces.
 """
 
+from __future__ import annotations
+
 from collections.abc import MutableMapping
 from collections import ChainMap as _ChainMap
+import contextlib
+from dataclasses import dataclass, field
 import functools
 from .compat import io
 import itertools
 import os
 import re
 import sys
-import warnings
-
+from typing import Iterable
 
 __all__ = (
     "NoSectionError",
     "DuplicateOptionError",
     "DuplicateSectionError",
     "NoOptionError",
     "InterpolationError",
     "InterpolationDepthError",
     "InterpolationMissingOptionError",
     "InterpolationSyntaxError",
     "ParsingError",
     "MissingSectionHeaderError",
+    "MultilineContinuationError",
     "ConfigParser",
     "RawConfigParser",
     "Interpolation",
     "BasicInterpolation",
     "ExtendedInterpolation",
-    "LegacyInterpolation",
     "SectionProxy",
     "ConverterMapping",
     "DEFAULTSECT",
     "MAX_INTERPOLATION_DEPTH",
+    "UNNAMED_SECTION",
 )
 
 _default_dict = dict
 DEFAULTSECT = "DEFAULT"
 
 MAX_INTERPOLATION_DEPTH = 10
 
@@ -309,23 +317,40 @@
         InterpolationError.__init__(self, option, section, msg)
         self.args = (option, section, rawval)
 
 
 class ParsingError(Error):
     """Raised when a configuration file does not follow legal syntax."""
 
-    def __init__(self, source):
+    def __init__(self, source, *args):
         super().__init__(f'Source contains parsing errors: {source!r}')
         self.source = source
         self.errors = []
         self.args = (source,)
+        if args:
+            self.append(*args)
 
     def append(self, lineno, line):
         self.errors.append((lineno, line))
-        self.message += '\n\t[line %2d]: %s' % (lineno, line)
+        self.message += '\n\t[line %2d]: %s' % (lineno, repr(line))
+
+    def combine(self, others):
+        for other in others:
+            for error in other.errors:
+                self.append(*error)
+        return self
+
+    @staticmethod
+    def _raise_all(exceptions: Iterable['ParsingError']):
+        """
+        Combine any number of ParsingErrors into one and raise it.
+        """
+        exceptions = iter(exceptions)
+        with contextlib.suppress(StopIteration):
+            raise next(exceptions).combine(exceptions)
 
 
 class MissingSectionHeaderError(ParsingError):
     """Raised when a key-value pair is found before any section header."""
 
     def __init__(self, filename, lineno, line):
         Error.__init__(
@@ -335,14 +360,37 @@
         )
         self.source = filename
         self.lineno = lineno
         self.line = line
         self.args = (filename, lineno, line)
 
 
+class MultilineContinuationError(ParsingError):
+    """Raised when a key without value is followed by continuation line"""
+
+    def __init__(self, filename, lineno, line):
+        Error.__init__(
+            self,
+            "Key without value continued with an indented line.\n"
+            "file: %r, line: %d\n%r" % (filename, lineno, line),
+        )
+        self.source = filename
+        self.lineno = lineno
+        self.line = line
+        self.args = (filename, lineno, line)
+
+
+class _UnnamedSection:
+    def __repr__(self):
+        return "<UNNAMED_SECTION>"
+
+
+UNNAMED_SECTION = _UnnamedSection()
+
+
 # Used in parser getters to indicate the default behaviour when a specific
 # option is not found it to raise an exception. Created to enable `None` as
 # a valid fallback value.
 _UNSET = object()
 
 
 class Interpolation:
@@ -526,60 +574,60 @@
                 raise InterpolationSyntaxError(
                     option,
                     section,
                     "'$' must be followed by '$' or '{', " "found: %r" % (rest,),
                 )
 
 
-class LegacyInterpolation(Interpolation):
-    """Deprecated interpolation used in old versions of ConfigParser.
-    Use BasicInterpolation or ExtendedInterpolation instead."""
-
-    _KEYCRE = re.compile(r"%\(([^)]*)\)s|.")
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        warnings.warn(
-            "LegacyInterpolation has been deprecated since Python 3.2 "
-            "and will be removed from the configparser module in Python 3.13. "
-            "Use BasicInterpolation or ExtendedInterpolation instead.",
-            DeprecationWarning,
-            stacklevel=2,
-        )
+@dataclass
+class _ReadState:
+    elements_added: set[str] = field(default_factory=set)
+    cursect: dict[str, str] | None = None
+    sectname: str | None = None
+    optname: str | None = None
+    lineno: int = 0
+    indent_level: int = 0
+    errors: list[ParsingError] = field(default_factory=list)
+
+
+@dataclass
+class _Prefixes:
+    full: Iterable[str]
+    inline: Iterable[str]
+
+
+class _Line(str):
+    def __new__(cls, val, *args, **kwargs):
+        return super().__new__(cls, val)
+
+    def __init__(self, val, prefixes: _Prefixes):
+        self.prefixes = prefixes
+
+    @functools.cached_property
+    def clean(self):
+        return self._strip_full() and self._strip_inline()
+
+    @property
+    def has_comments(self):
+        return self.strip() != self.clean
 
-    def before_get(self, parser, section, option, value, vars):
-        rawval = value
-        depth = MAX_INTERPOLATION_DEPTH
-        while depth:  # Loop through this until it's done
-            depth -= 1
-            if value and "%(" in value:
-                replace = functools.partial(self._interpolation_replace, parser=parser)
-                value = self._KEYCRE.sub(replace, value)
-                try:
-                    value = value % vars
-                except KeyError as e:
-                    raise InterpolationMissingOptionError(
-                        option, section, rawval, e.args[0]
-                    ) from None
-            else:
-                break
-        if value and "%(" in value:
-            raise InterpolationDepthError(option, section, rawval)
-        return value
-
-    def before_set(self, parser, section, option, value):
-        return value
+    def _strip_inline(self):
+        """
+        Search for the earliest prefix at the beginning of the line or following a space.
+        """
+        matcher = re.compile(
+            '|'.join(rf'(^|\s)({re.escape(prefix)})' for prefix in self.prefixes.inline)
+            # match nothing if no prefixes
+            or '(?!)'
+        )
+        match = matcher.search(self)
+        return self[: match.start() if match else None].strip()
 
-    @staticmethod
-    def _interpolation_replace(match, parser):
-        s = match.group(1)
-        if s is None:
-            return match.group()
-        else:
-            return "%%(%s)s" % parser.optionxform(s)
+    def _strip_full(self):
+        return '' if any(map(self.strip().startswith, self.prefixes.full)) else True
 
 
 class RawConfigParser(MutableMapping):
     """ConfigParser that does not do interpolation."""
 
     # Regular expressions for parsing section headers and options
     _SECT_TMPL = r"""
@@ -637,14 +685,15 @@
         comment_prefixes=('#', ';'),
         inline_comment_prefixes=None,
         strict=True,
         empty_lines_in_values=True,
         default_section=DEFAULTSECT,
         interpolation=_UNSET,
         converters=_UNSET,
+        allow_unnamed_section=False,
     ):
         self._dict = dict_type
         self._sections = self._dict()
         self._defaults = self._dict()
         self._converters = ConverterMapping(self)
         self._proxies = self._dict()
         self._proxies[default_section] = SectionProxy(self, default_section)
@@ -653,16 +702,18 @@
             self._optcre = self.OPTCRE_NV if allow_no_value else self.OPTCRE
         else:
             d = "|".join(re.escape(d) for d in delimiters)
             if allow_no_value:
                 self._optcre = re.compile(self._OPT_NV_TMPL.format(delim=d), re.VERBOSE)
             else:
                 self._optcre = re.compile(self._OPT_TMPL.format(delim=d), re.VERBOSE)
-        self._comment_prefixes = tuple(comment_prefixes or ())
-        self._inline_comment_prefixes = tuple(inline_comment_prefixes or ())
+        self._prefixes = _Prefixes(
+            full=tuple(comment_prefixes or ()),
+            inline=tuple(inline_comment_prefixes or ()),
+        )
         self._strict = strict
         self._allow_no_value = allow_no_value
         self._empty_lines_in_values = empty_lines_in_values
         self.default_section = default_section
         self._interpolation = interpolation
         if self._interpolation is _UNSET:
             self._interpolation = self._DEFAULT_INTERPOLATION
@@ -673,14 +724,15 @@
                 f"interpolation= must be None or an instance of Interpolation;"
                 f" got an object of type {type(self._interpolation)}"
             )
         if converters is not _UNSET:
             self._converters.update(converters)
         if defaults:
             self._read_defaults(defaults)
+        self._allow_unnamed_section = allow_unnamed_section
 
     def defaults(self):
         return self._defaults
 
     def sections(self):
         """Return a list of section names, excluding [DEFAULT]"""
         # self._sections will never have [DEFAULT] in it
@@ -959,20 +1011,32 @@
         """
         if space_around_delimiters:
             d = " {} ".format(self._delimiters[0])
         else:
             d = self._delimiters[0]
         if self._defaults:
             self._write_section(fp, self.default_section, self._defaults.items(), d)
+        if UNNAMED_SECTION in self._sections:
+            self._write_section(
+                fp,
+                UNNAMED_SECTION,
+                self._sections[UNNAMED_SECTION].items(),
+                d,
+                unnamed=True,
+            )
+
         for section in self._sections:
+            if section is UNNAMED_SECTION:
+                continue
             self._write_section(fp, section, self._sections[section].items(), d)
 
-    def _write_section(self, fp, section_name, section_items, delimiter):
-        """Write a single section to the specified `fp`."""
-        fp.write("[{}]\n".format(section_name))
+    def _write_section(self, fp, section_name, section_items, delimiter, unnamed=False):
+        """Write a single section to the specified `fp'."""
+        if not unnamed:
+            fp.write("[{}]\n".format(section_name))
         for key, value in section_items:
             value = self._interpolation.before_write(self, section_name, key, value)
             if value is not None or not self._allow_no_value:
                 value = delimiter + str(value).replace('\n', '\n\t')
             else:
                 value = ""
             fp.write("{}{}\n".format(key, value))
@@ -1050,118 +1114,129 @@
 
         Configuration files may include comments, prefixed by specific
         characters (`#` and `;` by default). Comments may appear on their own
         in an otherwise empty line or may be entered in lines holding values or
         section names. Please note that comments get stripped off when reading
         configuration files.
         """
-        elements_added = set()
-        cursect = None  # None, or a dictionary
-        sectname = None
-        optname = None
-        lineno = 0
-        indent_level = 0
-        e = None  # None, or an exception
-        for lineno, line in enumerate(fp, start=1):
-            comment_start = sys.maxsize
-            # strip inline comments
-            inline_prefixes = {p: -1 for p in self._inline_comment_prefixes}
-            while comment_start == sys.maxsize and inline_prefixes:
-                next_prefixes = {}
-                for prefix, index in inline_prefixes.items():
-                    index = line.find(prefix, index + 1)
-                    if index == -1:
-                        continue
-                    next_prefixes[prefix] = index
-                    if index == 0 or (index > 0 and line[index - 1].isspace()):
-                        comment_start = min(comment_start, index)
-                inline_prefixes = next_prefixes
-            # strip full line comments
-            for prefix in self._comment_prefixes:
-                if line.strip().startswith(prefix):
-                    comment_start = 0
-                    break
-            if comment_start == sys.maxsize:
-                comment_start = None
-            value = line[:comment_start].strip()
-            if not value:
+
+        try:
+            ParsingError._raise_all(self._read_inner(fp, fpname))
+        finally:
+            self._join_multiline_values()
+
+    def _read_inner(self, fp, fpname):
+        st = _ReadState()
+
+        Line = functools.partial(_Line, prefixes=self._prefixes)
+        for st.lineno, line in enumerate(map(Line, fp), start=1):
+            if not line.clean:
                 if self._empty_lines_in_values:
                     # add empty line to the value, but only if there was no
                     # comment on the line
                     if (
-                        comment_start is None
-                        and cursect is not None
-                        and optname
-                        and cursect[optname] is not None
+                        not line.has_comments
+                        and st.cursect is not None
+                        and st.optname
+                        and st.cursect[st.optname] is not None
                     ):
-                        cursect[optname].append('')  # newlines added at join
+                        st.cursect[st.optname].append('')  # newlines added at join
                 else:
                     # empty line marks end of value
-                    indent_level = sys.maxsize
+                    st.indent_level = sys.maxsize
                 continue
-            # continuation line?
+
             first_nonspace = self.NONSPACECRE.search(line)
-            cur_indent_level = first_nonspace.start() if first_nonspace else 0
-            if cursect is not None and optname and cur_indent_level > indent_level:
-                cursect[optname].append(value)
-            # a section header or option header?
-            else:
-                indent_level = cur_indent_level
-                # is it a section header?
-                mo = self.SECTCRE.match(value)
-                if mo:
-                    sectname = mo.group('header')
-                    if sectname in self._sections:
-                        if self._strict and sectname in elements_added:
-                            raise DuplicateSectionError(sectname, fpname, lineno)
-                        cursect = self._sections[sectname]
-                        elements_added.add(sectname)
-                    elif sectname == self.default_section:
-                        cursect = self._defaults
-                    else:
-                        cursect = self._dict()
-                        self._sections[sectname] = cursect
-                        self._proxies[sectname] = SectionProxy(self, sectname)
-                        elements_added.add(sectname)
-                    # So sections can't start with a continuation line
-                    optname = None
-                # no section header in the file?
-                elif cursect is None:
-                    raise MissingSectionHeaderError(fpname, lineno, line)
-                # an option line?
-                else:
-                    mo = self._optcre.match(value)
-                    if mo:
-                        optname, vi, optval = mo.group('option', 'vi', 'value')
-                        if not optname:
-                            e = self._handle_error(e, fpname, lineno, line)
-                        optname = self.optionxform(optname.rstrip())
-                        if self._strict and (sectname, optname) in elements_added:
-                            raise DuplicateOptionError(
-                                sectname, optname, fpname, lineno
-                            )
-                        elements_added.add((sectname, optname))
-                        # This check is fine because the OPTCRE cannot
-                        # match if it would set optval to None
-                        if optval is not None:
-                            optval = optval.strip()
-                            cursect[optname] = [optval]
-                        else:
-                            # valueless option handling
-                            cursect[optname] = None
-                    else:
-                        # a non-fatal parsing error occurred. set up the
-                        # exception but keep going. the exception will be
-                        # raised at the end of the file and will contain a
-                        # list of all bogus lines
-                        e = self._handle_error(e, fpname, lineno, line)
-        self._join_multiline_values()
-        # if any parsing errors occurred, raise an exception
-        if e:
-            raise e
+            st.cur_indent_level = first_nonspace.start() if first_nonspace else 0
+
+            if self._handle_continuation_line(st, line, fpname):
+                continue
+
+            self._handle_rest(st, line, fpname)
+
+        return st.errors
+
+    def _handle_continuation_line(self, st, line, fpname):
+        # continuation line?
+        is_continue = (
+            st.cursect is not None
+            and st.optname
+            and st.cur_indent_level > st.indent_level
+        )
+        if is_continue:
+            if st.cursect[st.optname] is None:
+                raise MultilineContinuationError(fpname, st.lineno, line)
+            st.cursect[st.optname].append(line.clean)
+        return is_continue
+
+    def _handle_rest(self, st, line, fpname):
+        # a section header or option header?
+        if self._allow_unnamed_section and st.cursect is None:
+            st.sectname = UNNAMED_SECTION
+            st.cursect = self._dict()
+            self._sections[st.sectname] = st.cursect
+            self._proxies[st.sectname] = SectionProxy(self, st.sectname)
+            st.elements_added.add(st.sectname)
+
+        st.indent_level = st.cur_indent_level
+        # is it a section header?
+        mo = self.SECTCRE.match(line.clean)
+
+        if not mo and st.cursect is None:
+            raise MissingSectionHeaderError(fpname, st.lineno, line)
+
+        self._handle_header(st, mo, fpname) if mo else self._handle_option(
+            st, line, fpname
+        )
+
+    def _handle_header(self, st, mo, fpname):
+        st.sectname = mo.group('header')
+        if st.sectname in self._sections:
+            if self._strict and st.sectname in st.elements_added:
+                raise DuplicateSectionError(st.sectname, fpname, st.lineno)
+            st.cursect = self._sections[st.sectname]
+            st.elements_added.add(st.sectname)
+        elif st.sectname == self.default_section:
+            st.cursect = self._defaults
+        else:
+            st.cursect = self._dict()
+            self._sections[st.sectname] = st.cursect
+            self._proxies[st.sectname] = SectionProxy(self, st.sectname)
+            st.elements_added.add(st.sectname)
+        # So sections can't start with a continuation line
+        st.optname = None
+
+    def _handle_option(self, st, line, fpname):
+        # an option line?
+        st.indent_level = st.cur_indent_level
+
+        mo = self._optcre.match(line.clean)
+        if not mo:
+            # a non-fatal parsing error occurred. set up the
+            # exception but keep going. the exception will be
+            # raised at the end of the file and will contain a
+            # list of all bogus lines
+            st.errors.append(ParsingError(fpname, st.lineno, line))
+            return
+
+        st.optname, vi, optval = mo.group('option', 'vi', 'value')
+        if not st.optname:
+            st.errors.append(ParsingError(fpname, st.lineno, line))
+        st.optname = self.optionxform(st.optname.rstrip())
+        if self._strict and (st.sectname, st.optname) in st.elements_added:
+            raise DuplicateOptionError(st.sectname, st.optname, fpname, st.lineno)
+        st.elements_added.add((st.sectname, st.optname))
+        # This check is fine because the OPTCRE cannot
+        # match if it would set optval to None
+        if optval is not None:
+            optval = optval.strip()
+            st.cursect[st.optname] = [optval]
+        else:
+            # valueless option handling
+            st.cursect[st.optname] = None
 
     def _join_multiline_values(self):
         defaults = self.default_section, self._defaults
         all_sections = itertools.chain((defaults,), self._sections.items())
         for section, options in all_sections:
             for name, val in options.items():
                 if isinstance(val, list):
@@ -1172,20 +1247,14 @@
 
     def _read_defaults(self, defaults):
         """Read the defaults passed in the initializer.
         Note: values can be non-string."""
         for key, value in defaults.items():
             self._defaults[self.optionxform(key)] = value
 
-    def _handle_error(self, exc, fpname, lineno, line):
-        if not exc:
-            exc = ParsingError(fpname)
-        exc.append(lineno, repr(line))
-        return exc
-
     def _unify_values(self, section, vars):
         """Create a sequence of lookups with 'vars' taking priority over
         the 'section' which takes priority over the DEFAULTSECT.
 
         """
         sectiondict = {}
         try:
```

### Comparing `configparser-6.0.1/configparser.egg-info/SOURCES.txt` & `configparser-7.0.0/configparser.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,30 +2,27 @@
 .editorconfig
 .pre-commit-config.yaml
 .readthedocs.yaml
 LICENSE
 NEWS.rst
 README.rst
 SECURITY.md
-configparser.rst
-conftest.py
 mypy.ini
 pyproject.toml
 pytest.ini
 ruff.toml
 setup.cfg
 tea.yaml
 towncrier.toml
 tox.ini
 .github/FUNDING.yml
 .github/dependabot.yml
 .github/workflows/main.yml
 backports/configparser/__init__.py
 backports/configparser/compat.py
-configparser/__init__.py
 configparser.egg-info/PKG-INFO
 configparser.egg-info/SOURCES.txt
 configparser.egg-info/dependency_links.txt
 configparser.egg-info/requires.txt
 configparser.egg-info/top_level.txt
 docs/conf.py
 docs/history.rst
```

### Comparing `configparser-6.0.1/docs/conf.py` & `configparser-7.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `configparser-6.0.1/pytest.ini` & `configparser-7.0.0/pytest.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [pytest]
 norecursedirs=dist build .tox .eggs
 addopts=
 	--doctest-modules
 	--import-mode importlib
+consider_namespace_packages=true
 filterwarnings=
 	## upstream
 
 	# Ensure ResourceWarnings are emitted
 	default::ResourceWarning
 
 	# realpython/pytest-mypy#152
```

### Comparing `configparser-6.0.1/setup.cfg` & `configparser-7.0.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -13,38 +13,30 @@
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
-packages = find_namespace:
 include_package_data = true
 python_requires = >=3.8
 install_requires = 
 
-[options.packages.find]
-exclude = 
-	tests
-	docs
-
 [options.extras_require]
 testing = 
-	pytest >= 6
+	pytest >= 6, != 8.1.1
 	pytest-checkdocs >= 2.4
 	pytest-cov
-	pytest-mypy; \
-	python_implementation != "PyPy"
+	pytest-mypy
 	pytest-enabler >= 2.2
 	pytest-ruff >= 0.2.1
 	
 	types-backports
 docs = 
 	sphinx >= 3.5
-	sphinx < 7.2.5
 	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
 	furo
 	sphinx-lint
 	
 	jaraco.tidelift >= 1.4
```

### Comparing `configparser-6.0.1/tests/cfgparser.2` & `configparser-7.0.0/tests/cfgparser.2`

 * *Files identical despite different names*

### Comparing `configparser-6.0.1/tests/cfgparser.3` & `configparser-7.0.0/tests/cfgparser.3`

 * *Files identical despite different names*

### Comparing `configparser-6.0.1/tests/compat.py` & `configparser-7.0.0/tests/compat.py`

 * *Files identical despite different names*

### Comparing `configparser-6.0.1/tests/test_backport.py` & `configparser-7.0.0/tests/test_backport.py`

 * *Files identical despite different names*

### Comparing `configparser-6.0.1/tests/test_configparser.py` & `configparser-7.0.0/tests/test_configparser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import collections
 import io
 import os
 import pathlib
 import textwrap
 import unittest
-import warnings
 
 from typing import Type, Iterable
 
 from .compat import support, os_helper
 
 from backports import configparser
 
@@ -555,15 +554,15 @@
         self.assertEqual(e.args, ('<???>', 1, "No Section!\n"))
         if not self.allow_no_value:
             e = self.parse_error(
                 cf, configparser.ParsingError, "[Foo]\n  wrong-indent\n"
             )
             self.assertEqual(e.args, ('<???>',))
             # read_file on a real file
-            tricky = support.findfile("cfgparser.3")
+            tricky = support.findfile("cfgparser.3", subdir="configdata")
             if self.delimiters[0] == '=':
                 error = configparser.ParsingError
                 expected = (tricky,)
             else:
                 error = configparser.MissingSectionHeaderError
                 expected = (
                     tricky,
@@ -675,14 +674,31 @@
             self.assertEqual(
                 str(e),
                 "While reading from {0!r}: option {1!r} "
                 "in section {2!r} already exists".format('<dict>', 'opt', 'Bar'),
             )
             self.assertEqual(e.args, ("Bar", "opt", "<dict>", None))
 
+    def test_get_after_duplicate_option_error(self):
+        cf = self.newconfig()
+        ini = textwrap.dedent(
+            """\
+            [Foo]
+            x{equals}1
+            y{equals}2
+            y{equals}3
+        """.format(equals=self.delimiters[0])
+        )
+        if self.strict:
+            with self.assertRaises(configparser.DuplicateOptionError):
+                cf.read_string(ini)
+        else:
+            cf.read_string(ini)
+        self.assertEqual(cf.get('Foo', 'x'), '1')
+
     def test_write(self):
         config_string = (
             "[Long Line]\n"
             "foo{0[0]} this line is much, much longer than my editor\n"
             "   likes it.\n"
             "[{default_section}]\n"
             "foo{0[1]} another very\n"
@@ -744,15 +760,15 @@
         cf.set("sect", "option2", mystr("splat"))
         cf.set("sect", "option1", "splat")
         cf.set("sect", "option2", "splat")
 
     def test_read_returns_file_list(self):
         if self.delimiters[0] != '=':
             self.skipTest('incompatible format')
-        file1 = support.findfile("cfgparser.1")
+        file1 = support.findfile("cfgparser.1", subdir="configdata")
         # check when we pass a mix of readable and non-readable files:
         cf = self.newconfig()
         parsed_files = cf.read([file1, "nonexistent-file"], encoding="utf-8")
         self.assertEqual(parsed_files, [file1])
         self.assertEqual(cf.get("Foo Bar", "foo"), "newbar")
         # check when we pass only a filename:
         cf = self.newconfig()
@@ -777,15 +793,15 @@
         cf = self.newconfig()
         parsed_files = cf.read([], encoding="utf-8")
         self.assertEqual(parsed_files, [])
 
     def test_read_returns_file_list_with_bytestring_path(self):
         if self.delimiters[0] != '=':
             self.skipTest('incompatible format')
-        file1_bytestring = support.findfile("cfgparser.1").encode()
+        file1_bytestring = support.findfile("cfgparser.1", subdir="configdata").encode()
         # check when passing an existing bytestring path
         cf = self.newconfig()
         parsed_files = cf.read(file1_bytestring, encoding="utf-8")
         self.assertEqual(parsed_files, [file1_bytestring])
         # check when passing an non-existing bytestring path
         cf = self.newconfig()
         parsed_files = cf.read(b'nonexistent-file', encoding="utf-8")
@@ -952,23 +968,14 @@
                 e.args,
                 (
                     "bar11",
                     "Foo",
                     "something %(with11)s lots of interpolation (11 steps)",
                 ),
             )
-        elif isinstance(self.interpolation, configparser.LegacyInterpolation):
-            self.assertEqual(
-                e.args,
-                (
-                    "bar11",
-                    "Foo",
-                    "something %(with11)s lots of interpolation (11 steps)",
-                ),
-            )
 
     def test_interpolation_missing_value(self):
         cf = self.get_interpolation_config()
         e = self.get_error(
             cf,
             configparser.InterpolationMissingOptionError,
             "Interpolation Error",
@@ -977,18 +984,14 @@
         self.assertEqual(e.reference, "reference")
         self.assertEqual(e.section, "Interpolation Error")
         self.assertEqual(e.option, "name")
         if self.interpolation == configparser._UNSET:
             self.assertEqual(
                 e.args, ('name', 'Interpolation Error', '%(reference)s', 'reference')
             )
-        elif isinstance(self.interpolation, configparser.LegacyInterpolation):
-            self.assertEqual(
-                e.args, ('name', 'Interpolation Error', '%(reference)s', 'reference')
-            )
 
     def test_items(self):
         self.check_items_config([
             ('default', '<default>'),
             ('getdefault', '|<default>|'),
             ('key', '|value|'),
             ('name', 'value'),
@@ -1002,17 +1005,14 @@
             "option2{eq}%(option1)s/xxx\n"
             "ok{eq}%(option1)s/%%s\n"
             "not_ok{eq}%(option2)s/%%s".format(eq=self.delimiters[0])
         )
         self.assertEqual(cf.get("section", "ok"), "xxx/%s")
         if self.interpolation == configparser._UNSET:
             self.assertEqual(cf.get("section", "not_ok"), "xxx/xxx/%s")
-        elif isinstance(self.interpolation, configparser.LegacyInterpolation):
-            with self.assertRaises(TypeError):
-                cf.get("section", "not_ok")
 
     def test_set_malformatted_interpolation(self):
         cf = self.fromstring(
             "[sect]\n" "option1{eq}foo\n".format(eq=self.delimiters[0])
         )
 
         self.assertEqual(cf.get('sect', "option1"), "foo")
@@ -1090,39 +1090,14 @@
             _DEFAULT_INTERPOLATION = None
 
         cf = CustomConfigParser()
         cf.read_string(self.ini)
         self.assertMatchesIni(cf)
 
 
-class ConfigParserTestCaseLegacyInterpolation(ConfigParserTestCase):
-    config_class = configparser.ConfigParser
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore", DeprecationWarning)
-        interpolation = configparser.LegacyInterpolation()
-
-    def test_set_malformatted_interpolation(self):
-        cf = self.fromstring(
-            "[sect]\n" "option1{eq}foo\n".format(eq=self.delimiters[0])
-        )
-
-        self.assertEqual(cf.get('sect', "option1"), "foo")
-
-        cf.set("sect", "option1", "%foo")
-        self.assertEqual(cf.get('sect', "option1"), "%foo")
-        cf.set("sect", "option1", "foo%")
-        self.assertEqual(cf.get('sect', "option1"), "foo%")
-        cf.set("sect", "option1", "f%oo")
-        self.assertEqual(cf.get('sect', "option1"), "f%oo")
-
-        # bug #5741: double percents are *not* malformed
-        cf.set("sect", "option2", "foo%%bar")
-        self.assertEqual(cf.get("sect", "option2"), "foo%%bar")
-
-
 class ConfigParserTestCaseInvalidInterpolationType(unittest.TestCase):
     def test_error_on_wrong_type_for_interpolation(self):
         for value in [configparser.ExtendedInterpolation, 42, "a string"]:
             with self.subTest(value=value):
                 with self.assertRaises(TypeError):
                     configparser.ConfigParser(interpolation=value)
 
@@ -1233,15 +1208,15 @@
 class RawConfigParserTestSambaConf(CfgParserTestCaseClass, unittest.TestCase):
     config_class = configparser.RawConfigParser
     comment_prefixes = ('#', ';', '----')
     inline_comment_prefixes = ('//',)
     empty_lines_in_values = False
 
     def test_reading(self):
-        smbconf = support.findfile("cfgparser.2")
+        smbconf = support.findfile("cfgparser.2", subdir="configdata")
         # check when we pass a mix of readable and non-readable files:
         cf = self.newconfig()
         parsed_files = cf.read([smbconf, "nonexistent-file"], encoding='utf-8')
         self.assertEqual(parsed_files, [smbconf])
         sections = [
             'global',
             'homes',
@@ -1451,15 +1426,15 @@
 class ConfigParserTestCaseTrickyFile(CfgParserTestCaseClass, unittest.TestCase):
     config_class = configparser.ConfigParser
     delimiters = ['=']
     comment_prefixes = ['#']
     allow_no_value = True
 
     def test_cfgparser_dot_3(self):
-        tricky = support.findfile("cfgparser.3")
+        tricky = support.findfile("cfgparser.3", subdir="configdata")
         cf = self.newconfig()
         self.assertEqual(len(cf.read(tricky, encoding='utf-8')), 1)
         self.assertEqual(
             cf.sections(),
             [
                 'strange',
                 'corruption',
@@ -1488,15 +1463,15 @@
         self.assertEqual(cf.get('tricky interpolation', 'lets'), 'do this')
         self.assertEqual(
             cf.get('tricky interpolation', 'lets'), cf.get('tricky interpolation', 'go')
         )
         self.assertEqual(cf.get('more interpolation', 'lets'), 'go shopping')
 
     def test_unicode_failure(self):
-        tricky = support.findfile("cfgparser.3")
+        tricky = support.findfile("cfgparser.3", subdir="configdata")
         cf = self.newconfig()
         with self.assertRaises(UnicodeDecodeError):
             cf.read(tricky, encoding='ascii')
 
 
 class Issue7005TestCase(unittest.TestCase):
     """Test output when None is set() as a value and allow_no_value == False.
@@ -1582,15 +1557,15 @@
                 if section[default] == value:
                     del section[default]
         return cf_copy
 
 
 class FakeFile:
     def __init__(self):
-        file_path = support.findfile("cfgparser.1")
+        file_path = support.findfile("cfgparser.1", subdir="configdata")
         with open(file_path, encoding="utf-8") as f:
             self.lines = f.readlines()
             self.lines.reverse()
 
     def readline(self):
         if len(self.lines):
             return self.lines.pop()
@@ -1603,15 +1578,15 @@
     while line:
         yield line
         line = f.readline()
 
 
 class ReadFileTestCase(unittest.TestCase):
     def test_file(self):
-        file_paths = [support.findfile("cfgparser.1")]
+        file_paths = [support.findfile("cfgparser.1", subdir="configdata")]
         try:
             file_paths.append(file_paths[0].encode('utf8'))
         except UnicodeEncodeError:
             pass  # unfortunately we can't test bytes on this path
         for file_path in file_paths:
             parser = configparser.ConfigParser()
             with open(file_path, encoding="utf-8") as f:
@@ -1715,14 +1690,36 @@
         with self.assertRaises(configparser.MissingSectionHeaderError) as dse:
             parser.read_file(lines, source=b"badbad")
         self.assertEqual(
             nice_literals(str(dse.exception)),
             "File contains no section headers.\nfile: 'badbad', line: 1\n" "'[badbad'",
         )
 
+    def test_keys_without_value_with_extra_whitespace(self):
+        lines = [
+            '[SECT]\n',
+            'KEY1\n',
+            ' KEY2 = VAL2\n',  # note the Space before the key!
+        ]
+        parser = configparser.ConfigParser(
+            comment_prefixes="",
+            allow_no_value=True,
+            strict=False,
+            delimiters=('=',),
+            interpolation=None,
+        )
+        with self.assertRaises(configparser.MultilineContinuationError) as dse:
+            parser.read_file(lines)
+        self.assertEqual(
+            str(dse.exception),
+            "Key without value continued with an indented line.\n"
+            "file: '<???>', line: 3\n"
+            "' KEY2 = VAL2\\n'",
+        )
+
 
 class CoverageOneHundredTestCase(unittest.TestCase):
     """Covers edge cases in the codebase."""
 
     def test_duplicate_option_error(self):
         error = configparser.DuplicateOptionError('section', 'option')
         self.assertEqual(error.section, 'section')
@@ -1770,22 +1767,14 @@
         with self.assertRaises(configparser.InterpolationSyntaxError) as cm:
             parser['section']['invalid_reference']
         self.assertEqual(
             str(cm.exception),
             "bad interpolation variable " "reference {0!r}".format('%(()'),
         )
 
-    def test_legacyinterpolation_deprecation(self):
-        with warnings.catch_warnings(record=True) as w:
-            warnings.simplefilter("always", DeprecationWarning)
-            configparser.LegacyInterpolation()
-        self.assertGreaterEqual(len(w), 1)
-        for warning in w:
-            self.assertIs(warning.category, DeprecationWarning)
-
     def test_sectionproxy_repr(self):
         parser = configparser.ConfigParser()
         parser.read_string(
             """
             [section]
             key = value
         """
@@ -2293,14 +2282,63 @@
         # be available on the section proxies.
         with self.assertRaises(AttributeError):
             self.assertEqual(cfg['one'].getlen('one'), 5)
         with self.assertRaises(AttributeError):
             self.assertEqual(cfg['two'].getlen('one'), 5)
 
 
+class SectionlessTestCase(unittest.TestCase):
+    def fromstring(self, string):
+        cfg = configparser.ConfigParser(allow_unnamed_section=True)
+        cfg.read_string(string)
+        return cfg
+
+    def test_no_first_section(self):
+        cfg1 = self.fromstring("""
+        a = 1
+        b = 2
+        [sect1]
+        c = 3
+        """)
+
+        self.assertEqual(
+            set([configparser.UNNAMED_SECTION, 'sect1']), set(cfg1.sections())
+        )
+        self.assertEqual('1', cfg1[configparser.UNNAMED_SECTION]['a'])
+        self.assertEqual('2', cfg1[configparser.UNNAMED_SECTION]['b'])
+        self.assertEqual('3', cfg1['sect1']['c'])
+
+        output = io.StringIO()
+        cfg1.write(output)
+        cfg2 = self.fromstring(output.getvalue())
+
+        # self.assertEqual(set([configparser.UNNAMED_SECTION, 'sect1']), set(cfg2.sections()))
+        self.assertEqual('1', cfg2[configparser.UNNAMED_SECTION]['a'])
+        self.assertEqual('2', cfg2[configparser.UNNAMED_SECTION]['b'])
+        self.assertEqual('3', cfg2['sect1']['c'])
+
+    def test_no_section(self):
+        cfg1 = self.fromstring("""
+        a = 1
+        b = 2
+        """)
+
+        self.assertEqual([configparser.UNNAMED_SECTION], cfg1.sections())
+        self.assertEqual('1', cfg1[configparser.UNNAMED_SECTION]['a'])
+        self.assertEqual('2', cfg1[configparser.UNNAMED_SECTION]['b'])
+
+        output = io.StringIO()
+        cfg1.write(output)
+        cfg2 = self.fromstring(output.getvalue())
+
+        self.assertEqual([configparser.UNNAMED_SECTION], cfg2.sections())
+        self.assertEqual('1', cfg2[configparser.UNNAMED_SECTION]['a'])
+        self.assertEqual('2', cfg2[configparser.UNNAMED_SECTION]['b'])
+
+
 class MiscTestCase(unittest.TestCase):
     def test__all__(self):
         support.check__all__(self, configparser, not_exported={"Error"})
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `configparser-6.0.1/tox.ini` & `configparser-7.0.0/tox.ini`

 * *Files 18% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 usedevelop = True
 extras =
 	testing
 
 [testenv:diffcov]
 description = run tests and check that diff from main is covered
 deps =
+	{[testenv]deps}
 	diff-cover
 commands =
 	pytest {posargs} --cov-report xml
 	diff-cover coverage.xml --compare-branch=origin/main --html-report diffcov.html
 	diff-cover coverage.xml --compare-branch=origin/main --fail-under=100
 
 [testenv:docs]
```

