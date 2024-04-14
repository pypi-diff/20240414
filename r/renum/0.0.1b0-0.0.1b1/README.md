# Comparing `tmp/renum-0.0.1b0.tar.gz` & `tmp/renum-0.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renum-0.0.1b0.tar", last modified: Fri Apr 12 06:01:39 2024, max compression
+gzip compressed data, was "renum-0.0.1b1.tar", last modified: Sun Apr 14 20:46:26 2024, max compression
```

## Comparing `renum-0.0.1b0.tar` & `renum-0.0.1b1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:01:39.394846 renum-0.0.1b0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:01:39.390846 renum-0.0.1b0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:01:39.394846 renum-0.0.1b0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-12 06:01:33.000000 renum-0.0.1b0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-12 06:01:33.000000 renum-0.0.1b0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-12 06:01:33.000000 renum-0.0.1b0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-12 06:01:33.000000 renum-0.0.1b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-12 06:01:39.394846 renum-0.0.1b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-12 06:01:33.000000 renum-0.0.1b0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-12 06:01:33.000000 renum-0.0.1b0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:01:39.394846 renum-0.0.1b0/renum/
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-12 06:01:33.000000 renum-0.0.1b0/renum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-12 06:01:33.000000 renum-0.0.1b0/renum/renum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-12 06:01:33.000000 renum-0.0.1b0/renum/renum.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 06:01:39.394846 renum-0.0.1b0/renum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5205 2024-04-12 06:01:39.000000 renum-0.0.1b0/renum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-12 06:01:39.000000 renum-0.0.1b0/renum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 06:01:39.000000 renum-0.0.1b0/renum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-12 06:01:39.000000 renum-0.0.1b0/renum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-12 06:01:39.000000 renum-0.0.1b0/renum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 06:01:39.394846 renum-0.0.1b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-12 06:01:33.000000 renum-0.0.1b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:46:26.014703 renum-0.0.1b1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:46:26.010703 renum-0.0.1b1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:46:26.014703 renum-0.0.1b1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-14 20:46:21.000000 renum-0.0.1b1/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-14 20:46:21.000000 renum-0.0.1b1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-14 20:46:21.000000 renum-0.0.1b1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-14 20:46:21.000000 renum-0.0.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-14 20:46:21.000000 renum-0.0.1b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-14 20:46:26.014703 renum-0.0.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-04-14 20:46:21.000000 renum-0.0.1b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-14 20:46:21.000000 renum-0.0.1b1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:46:26.014703 renum-0.0.1b1/renum/
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-14 20:46:21.000000 renum-0.0.1b1/renum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:46:21.000000 renum-0.0.1b1/renum/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6657 2024-04-14 20:46:21.000000 renum-0.0.1b1/renum/renum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-14 20:46:21.000000 renum-0.0.1b1/renum/renum.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:46:26.014703 renum-0.0.1b1/renum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4853 2024-04-14 20:46:25.000000 renum-0.0.1b1/renum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-14 20:46:26.000000 renum-0.0.1b1/renum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 20:46:25.000000 renum-0.0.1b1/renum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-14 20:46:25.000000 renum-0.0.1b1/renum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 20:46:25.000000 renum-0.0.1b1/renum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 20:46:26.014703 renum-0.0.1b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-14 20:46:21.000000 renum-0.0.1b1/setup.py
```

### Comparing `renum-0.0.1b0/.github/workflows/pythonpublish.yml` & `renum-0.0.1b1/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `renum-0.0.1b0/.gitignore` & `renum-0.0.1b1/.gitignore`

 * *Files identical despite different names*

### Comparing `renum-0.0.1b0/.pre-commit-config.yaml` & `renum-0.0.1b1/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     -   id: ruff-format
 -   repo: https://github.com/RobertCraigie/pyright-python
     rev: v1.1.358
     hooks:
     -   id: pyright
         additional_dependencies:
             # required dependencies
-        -   importlib_metadata >= 1.4.0
+        -   regex
 
             # typing
         -   typing_extensions
 ci:
     autoupdate_schedule: quarterly
     skip:
     # CI doesn't like pip scripts calling their own node, so skip this for now
```

### Comparing `renum-0.0.1b0/LICENSE` & `renum-0.0.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `renum-0.0.1b0/PKG-INFO` & `renum-0.0.1b1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renum
-Version: 0.0.1b0
+Version: 0.0.1b1
 Summary: Easily build Enum-like regular expression patterns
 Author: Zephyrkul
 License: MIT License
         
         Copyright (c) 2024 - 2024
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,37 +21,36 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: homepage, https://github.com/Zephyrkul/renum
-Project-URL: repository, https://github.com/Zephyrkul/renum.git
+Project-URL: Homepage, https://github.com/Zephyrkul/renum
+Project-URL: Repository, https://github.com/Zephyrkul/renum.git
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Python: <4.0,>=3.7.0
+Requires-Python: <4.0,>=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: regex
-Requires-Dist: importlib_metadata>=1.4.0; python_version < "3.8"
 Provides-Extra: docs
 Requires-Dist: Sphinx~=5.3; extra == "docs"
 
 # renum
 
 [![pypi](https://img.shields.io/pypi/v/renum.svg)](https://pypi.org/project/renum/)
 [![Licensed under the MIT License](https://img.shields.io/pypi/l/renum.svg)](https://choosealicense.com/licenses/mit/)
@@ -76,55 +75,55 @@
 
 ## Support
 
 If you need help with using renum, find a bug, or have a feature request, feel free to [file an issue](https://github.com/Zephyrkul/sans/issues/new/choose).
 
 ## Examples
 
-Scanning through happenings from an XML file:
+Parsing from standard input:
 
 ```py
-import xml.etree.ElementTree as ET
-
+import regex
 from renum import renum
 
 
-class HappeningsRenum(renum):
-    ADMITTED = r"@@(?P<nation>[^@]+)@@ was admitted to the World Assembly\."
-    MOVED = r"@@(?P<nation>[^@]+)@@ relocated from %%(?P<from>[^%]+)%% to %%(?P<to>[^%]+)%%\."
-    ENDORSED = r"@@(?P<endorser>[^@]+)@@ endorsed @@(?P<endorsee>[^@]+)@@\."
-    WITHDREW_ENDORSEMENT = r"@@(?P<endorser>[^@]+)@@ withdrew its endorsement from @@(?P<endorsee>[^@]+)@@\."
-
-
-def main():
-    root = ET.parse("happenings.xml")
-    for element in root.iterfind("HAPPENINGS/EVENT/TEXT"):
-        event = HappeningsRenum.fullmatch(element.text)
-        if event is HappeningsRenum.ADMITTED:
-            print("Welcome to the WA, %s!" % event.last_match.group("nation"))
-        elif (
-            event is HappeningsRenum.MOVED
-            and event.last_match.group("to") == "the_rejected_realms"
-        ):
-            print("Welcome to TRR, %s!" % event.last_match.group("nation"))
-        elif (
-            event is HappeningsRenum.ENDORSED
-            and event.last_match.group("endorsee") == "zephyrkul"
-        ):
-            print(
-                "Thanks for the endorsement, %s!" % event.last_match.group("endorser")
-            )
-        elif (
-            event is HappeningsRenum.WITHDREW_ENDORSEMENT
-            and event.last_match.group("endorsee") == "zephyrkul"
-        ):
-            print("But why, %s? \N{PENSIVE FACE}" % event.last_match.group("endorser"))
+class Actions(renum, flags=regex.IGNORECASE):
+    GO = r"go (?P<direction>north|south|east|west)"
+    EXAMINE = r"examine (?P<item>[\w\s]+)"
+    OPEN = r"open (?P<object>door|chest)"
 
 
 if __name__ == "__main__":
-    main()
+    while True:
+        line = input()
+        if not line:
+            break
+        action = Actions.match(line)  # The renum class acts like a Pattern...
+        if action is Actions.GO:
+            print("You went %s" % action.group("direction"))  # and each entry acts like a Match
+        elif action is Actions.EXAMINE:
+            print("You take a closer look at %s. Looks grungy." % action.group("item"))
+        elif action is Actions.OPEN:
+            print("You tried to open the %s, but it was locked." % action.group("object"))
+        else:
+            print("Unknown action: %s" % line)
+```
+
+Troubleshooting a misbehaving renum:
+
+```pycon
+>>> import regex
+>>> from renum import renum
+>>>
+>>> class Bad(renum, flags=regex.IGNORECASE | regex.DEBUG):
+...     GOOD = r"no (?:issues|problems) here"
+...     BAD = r"whoops,\s(?P<missed something)"
+...
+regex.error: bad character in group name at position 29 in BAD
+whoops,\s(?P<missed something)
+                             ^
 ```
 
 ## Requirements
 
-- [Python 3.7+](https://www.python.org/)
+- [Python 3.9+](https://www.python.org/)
 - [regex](https://pypi.org/project/regex/)
```

### Comparing `renum-0.0.1b0/pyproject.toml` & `renum-0.0.1b1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -7,62 +7,61 @@
     ]
     build-backend = 'setuptools.build_meta'
 
 [project]
     name = 'renum'
     description = 'Easily build Enum-like regular expression patterns'
     readme = 'README.md'
-    requires-python = '>=3.7.0,<4.0'
+    requires-python = '>=3.9.0,<4.0'
     classifiers = [
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: MIT License',
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3 :: Only',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
+        'Topic :: Text Processing',
+        'Topic :: Text Processing :: General',
         'Topic :: Utilities',
         'Typing :: Typed',
     ]
     dependencies = [
-        'regex',
-        'importlib_metadata >= 1.4.0; python_version < "3.8"'
+        'regex'
     ]
     dynamic = ['version']
 
 [project.license]
     file = 'LICENSE'
 
 [[project.authors]]
     name = 'Zephyrkul'
 
 [project.urls]
-    homepage = 'https://github.com/Zephyrkul/renum'
-    #   documentation = 'https://renum.readthedocs.io/en/stable/'
-    repository = 'https://github.com/Zephyrkul/renum.git'
+    Homepage = 'https://github.com/Zephyrkul/renum'
+    #   Documentation = 'https://renum.readthedocs.io/en/stable/'
+    Repository = 'https://github.com/Zephyrkul/renum.git'
 
 [project.optional-dependencies]
     docs = ['Sphinx ~= 5.3']
 
 [tool.setuptools_scm]
 
 [tool.pyright]
-    pythonVersion = '3.7'
+    pythonVersion = '3.9'
     reportUnnecessaryTypeIgnoreComment = 'warning'
     typeCheckingMode = 'strict'
 
 [tool.ruff]
-    target-version = 'py37'
+    target-version = 'py39'
 
 [tool.ruff.lint]
     select = ['E', 'F', 'B', 'Q', 'I', 'W']
     ignore = [
         # ignore rules incompatible with ruff-format: https://docs.astral.sh/ruff/formatter/#conflicting-lint-rules
         'E501', 'W191', 'E111', 'E114', 'E117', 'D206', 'D300', 'Q000', 'Q001', 'Q002', 'Q003', 'COM812', 'COM819', 'ISC001', 'ISC002'
     ]
```

### Comparing `renum-0.0.1b0/renum/__init__.py` & `renum-0.0.1b1/renum/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,24 +17,20 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import sys as _sys
+from importlib.metadata import metadata as _metadata
 
 from .renum import RenumType, renum
 
 __all__ = ("RenumType", "renum")
 
-if _sys.version_info < (3, 8):
-    from importlib_metadata import metadata as _metadata
-else:
-    from importlib.metadata import metadata as _metadata
-
 __copyright__ = "Copyright 2024-2024 Zephyrkul"
 
 _meta = _metadata(__name__)
 __title__ = _meta["Name"]
 __author__ = _meta["Author"]
 __license__ = _meta["License"]
 __version__ = _meta["Version"]
```

### Comparing `renum-0.0.1b0/renum.egg-info/PKG-INFO` & `renum-0.0.1b1/renum.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: renum
-Version: 0.0.1b0
+Version: 0.0.1b1
 Summary: Easily build Enum-like regular expression patterns
 Author: Zephyrkul
 License: MIT License
         
         Copyright (c) 2024 - 2024
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,37 +21,36 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: homepage, https://github.com/Zephyrkul/renum
-Project-URL: repository, https://github.com/Zephyrkul/renum.git
+Project-URL: Homepage, https://github.com/Zephyrkul/renum
+Project-URL: Repository, https://github.com/Zephyrkul/renum.git
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Text Processing
+Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Python: <4.0,>=3.7.0
+Requires-Python: <4.0,>=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: regex
-Requires-Dist: importlib_metadata>=1.4.0; python_version < "3.8"
 Provides-Extra: docs
 Requires-Dist: Sphinx~=5.3; extra == "docs"
 
 # renum
 
 [![pypi](https://img.shields.io/pypi/v/renum.svg)](https://pypi.org/project/renum/)
 [![Licensed under the MIT License](https://img.shields.io/pypi/l/renum.svg)](https://choosealicense.com/licenses/mit/)
@@ -76,55 +75,55 @@
 
 ## Support
 
 If you need help with using renum, find a bug, or have a feature request, feel free to [file an issue](https://github.com/Zephyrkul/sans/issues/new/choose).
 
 ## Examples
 
-Scanning through happenings from an XML file:
+Parsing from standard input:
 
 ```py
-import xml.etree.ElementTree as ET
-
+import regex
 from renum import renum
 
 
-class HappeningsRenum(renum):
-    ADMITTED = r"@@(?P<nation>[^@]+)@@ was admitted to the World Assembly\."
-    MOVED = r"@@(?P<nation>[^@]+)@@ relocated from %%(?P<from>[^%]+)%% to %%(?P<to>[^%]+)%%\."
-    ENDORSED = r"@@(?P<endorser>[^@]+)@@ endorsed @@(?P<endorsee>[^@]+)@@\."
-    WITHDREW_ENDORSEMENT = r"@@(?P<endorser>[^@]+)@@ withdrew its endorsement from @@(?P<endorsee>[^@]+)@@\."
-
-
-def main():
-    root = ET.parse("happenings.xml")
-    for element in root.iterfind("HAPPENINGS/EVENT/TEXT"):
-        event = HappeningsRenum.fullmatch(element.text)
-        if event is HappeningsRenum.ADMITTED:
-            print("Welcome to the WA, %s!" % event.last_match.group("nation"))
-        elif (
-            event is HappeningsRenum.MOVED
-            and event.last_match.group("to") == "the_rejected_realms"
-        ):
-            print("Welcome to TRR, %s!" % event.last_match.group("nation"))
-        elif (
-            event is HappeningsRenum.ENDORSED
-            and event.last_match.group("endorsee") == "zephyrkul"
-        ):
-            print(
-                "Thanks for the endorsement, %s!" % event.last_match.group("endorser")
-            )
-        elif (
-            event is HappeningsRenum.WITHDREW_ENDORSEMENT
-            and event.last_match.group("endorsee") == "zephyrkul"
-        ):
-            print("But why, %s? \N{PENSIVE FACE}" % event.last_match.group("endorser"))
+class Actions(renum, flags=regex.IGNORECASE):
+    GO = r"go (?P<direction>north|south|east|west)"
+    EXAMINE = r"examine (?P<item>[\w\s]+)"
+    OPEN = r"open (?P<object>door|chest)"
 
 
 if __name__ == "__main__":
-    main()
+    while True:
+        line = input()
+        if not line:
+            break
+        action = Actions.match(line)  # The renum class acts like a Pattern...
+        if action is Actions.GO:
+            print("You went %s" % action.group("direction"))  # and each entry acts like a Match
+        elif action is Actions.EXAMINE:
+            print("You take a closer look at %s. Looks grungy." % action.group("item"))
+        elif action is Actions.OPEN:
+            print("You tried to open the %s, but it was locked." % action.group("object"))
+        else:
+            print("Unknown action: %s" % line)
+```
+
+Troubleshooting a misbehaving renum:
+
+```pycon
+>>> import regex
+>>> from renum import renum
+>>>
+>>> class Bad(renum, flags=regex.IGNORECASE | regex.DEBUG):
+...     GOOD = r"no (?:issues|problems) here"
+...     BAD = r"whoops,\s(?P<missed something)"
+...
+regex.error: bad character in group name at position 29 in BAD
+whoops,\s(?P<missed something)
+                             ^
 ```
 
 ## Requirements
 
-- [Python 3.7+](https://www.python.org/)
+- [Python 3.9+](https://www.python.org/)
 - [regex](https://pypi.org/project/regex/)
```

