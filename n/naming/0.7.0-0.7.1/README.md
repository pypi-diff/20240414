# Comparing `tmp/naming-0.7.0.tar.gz` & `tmp/naming-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "B:\write\code\git\naming\dist\tmpqvl_cul_\naming-0.7.0.tar", last modified: Fri Sep 23 22:46:04 2022, max compression
+gzip compressed data, was "naming-0.7.1.tar", last modified: Sun Apr 14 01:59:03 2024, max compression
```

## Comparing `naming-0.7.0.tar` & `naming-0.7.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-09-23 22:46:04.635950 naming-0.7.0/
--rw-rw-rw-   0        0        0     1102 2022-09-23 22:35:45.000000 naming-0.7.0/LICENSE
--rw-rw-rw-   0        0        0     2234 2022-09-23 22:46:04.635950 naming-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     1699 2020-12-29 07:08:29.000000 naming-0.7.0/README.md
-drwxrwxrwx   0        0        0        0 2022-09-23 22:46:04.577954 naming-0.7.0/naming/
--rw-rw-rw-   0        0        0    12423 2021-02-27 02:00:09.000000 naming-0.7.0/naming/__init__.py
--rw-rw-rw-   0        0        0    10503 2022-09-13 11:43:08.000000 naming-0.7.0/naming/base.py
-drwxrwxrwx   0        0        0        0 2022-09-23 22:46:04.633950 naming-0.7.0/naming/tests/
--rw-rw-rw-   0        0        0    25781 2022-09-13 11:43:08.000000 naming-0.7.0/naming/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2022-09-23 22:46:04.618951 naming-0.7.0/naming.egg-info/
--rw-rw-rw-   0        0        0     2234 2022-09-23 22:46:04.000000 naming-0.7.0/naming.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2022-09-23 22:46:04.000000 naming-0.7.0/naming.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-23 22:46:04.000000 naming-0.7.0/naming.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2022-09-23 22:46:04.000000 naming-0.7.0/naming.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-09-23 22:46:04.000000 naming-0.7.0/naming.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      702 2022-09-23 22:46:04.644950 naming-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2020-12-29 06:56:05.000000 naming-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 01:59:03.271319 naming-0.7.1/
+-rw-rw-rw-   0        0        0     1102 2024-04-14 00:35:42.000000 naming-0.7.1/LICENSE
+-rw-rw-rw-   0        0        0     2746 2024-04-14 01:59:03.271319 naming-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1706 2024-04-14 01:52:12.000000 naming-0.7.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 01:59:03.261032 naming-0.7.1/naming/
+-rw-rw-rw-   0        0        0    12432 2024-04-14 01:52:12.000000 naming-0.7.1/naming/__init__.py
+-rw-rw-rw-   0        0        0    10502 2024-04-14 01:52:12.000000 naming-0.7.1/naming/base.py
+drwxrwxrwx   0        0        0        0 2024-04-14 01:59:03.271319 naming-0.7.1/naming.egg-info/
+-rw-rw-rw-   0        0        0     2746 2024-04-14 01:59:03.000000 naming-0.7.1/naming.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-04-14 01:59:03.000000 naming-0.7.1/naming.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 01:59:03.000000 naming-0.7.1/naming.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-04-14 01:59:03.000000 naming-0.7.1/naming.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-14 01:59:03.000000 naming-0.7.1/naming.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2023-10-27 08:19:00.000000 naming-0.7.1/pyproject.toml
+-rw-rw-rw-   0        0        0      844 2024-04-14 01:59:03.271319 naming-0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-14 00:35:42.000000 naming-0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 01:59:03.271319 naming-0.7.1/tests/
+-rw-rw-rw-   0        0        0    25781 2024-04-14 01:52:12.000000 naming-0.7.1/tests/test_naming.py
```

### Comparing `naming-0.7.0/LICENSE` & `naming-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `naming-0.7.0/PKG-INFO` & `naming-0.7.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,30 @@
-Metadata-Version: 2.1
-Name: naming
-Version: 0.7.0
-Summary: Object-oriented names for the digital era.
-Home-page: https://github.com/chrizzFTD/naming
-Author: Christian López Barrón
-Author-email: chris.gfz@gmail.com
-Keywords: name names naming convention configuration config cfg regex
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-License-File: LICENSE
-
 # naming
 [![Build Status](https://travis-ci.org/chrizzFTD/naming.svg?branch=master)](https://travis-ci.org/chrizzFTD/naming)
 [![Coverage Status](https://coveralls.io/repos/github/chrizzFTD/naming/badge.svg?branch=master)](https://coveralls.io/github/chrizzFTD/naming?branch=master)
 [![Documentation Status](https://readthedocs.org/projects/naming/badge/?version=latest)](https://naming.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/naming.svg)](https://badge.fury.io/py/naming)
 [![PyPI](https://img.shields.io/pypi/pyversions/naming.svg)](https://pypi.python.org/pypi/naming)
 
-Object-oriented names for the digital era.
+> Object-oriented names for the digital era.
 
 `naming` provides an interface for dealing with naming conventions; from
 defining them, to identifying names and creating new ones.
     
-### Installation
+## Installation
 
-`naming` is available for Python 3.7 onwards via PyPI.
+`naming` is available for Python 3.8+ via PyPI.
 
 ```bash
 $ pip install naming
 ```
 
-### Usage
+## Example
 
-Please refer to the [documentation](http://naming.readthedocs.io/en/latest/) for details on contents and usage.
+Please refer to the [documentation walkthrough](http://naming.readthedocs.io/en/latest/) for details on contents and usage.
 
 ```python
 >>> import naming
 >>> class NameFileConvention(naming.Name, naming.File):
 ...     config = dict(first=r'\w+', last=r'\w+', number=r'\d+')
 ...
 >>> name = NameFileConvention('john doe 07.jpg')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `naming-0.7.0/naming/__init__.py` & `naming-0.7.1/naming/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     and a `join` dictionary attribute for nesting existing fields into new ones (or to override other fields).
 
     All field names should be unique. No duplicates are allowed.
 
     Example:
         >>> from naming import Name
         >>> class MyName(Name):
-        ...     config = dict(base=r'\w+')
+        ...     config = dict(base=r'\\w+')
         ...
         >>> n = MyName()
         >>> n.get()  # no name has been set on the object, convention is solved with {missing} fields
         '{base}'
         >>> n.values
         {}
         >>> n.name = 'hello_world'
@@ -60,15 +60,15 @@
     ---------  --------------
     *suffix*   Any amount of word characters
     =========  ==============
 
     Example:
         >>> from naming import File
         >>> class MyFile(File):
-        ...     config = dict(base=r'\w+')
+        ...     config = dict(base=r'\\w+')
         ...
         >>> f = MyFile()
         >>> f.get()
         '{basse}.{suffix}'
         >>> f.get(suffix='png')
         '{base}.png'
         >>> f = MyFile('hello.world')
@@ -78,15 +78,15 @@
         'world'
         >>> f.suffix = 'abc'
         >>> f.name
         'hello.abc'
         >>> f.path
         WindowsPath('hello.abc')
     """
-    file_config = NameConfig(dict(suffix='\w+'))
+    file_config = NameConfig(dict(suffix=r'\w+'))
 
     @property
     def _pattern(self) -> str:
         sep = re.escape('.')
         casted = self.cast_config(self.file_config)
         pat = r'({sep}{suffix})'.format(sep=sep, **casted)
         return rf'{super()._pattern}{pat}'
@@ -135,22 +135,22 @@
     |           |                             |                                                                                                   |
     |           |                             |If used, the *output* field must also exist. This is to prevent ambiguity when solving the fields. |
     +-----------+-----------------------------+---------------------------------------------------------------------------------------------------+
 
     ======  ============
     **Composed Fields**
     --------------------
-    *pipe*  Combination of unique fields in the form of: (.{output})\*.{version}.{index}**
-    \* optional field. ** exists only when *output* is there as well.
+    *pipe*  Combination of unique fields in the form of: (.{output})*.{version}.{index}**
+    \\* optional field. ** exists only when *output* is there as well.
     ====================
 
     Example:
         >>> from naming import Pipe
         >>> class MyPipe(Pipe):
-        ...     config = dict(base=r'\w+')
+        ...     config = dict(base=r'\\w+')
         ...
         >>> p = MyPipe()
         >>> p.get()
         '{base}.{pipe}'
         >>> p.get(version=10)
         '{base}.10'
         >>> p.get(output='data')
@@ -172,15 +172,15 @@
         >>> p.index = 101
         >>> p.version = 7
         >>> p.name
         'my_wip_data.exchange.7.101'
         >>> p.values
         {'base': 'my_wip_data', 'pipe': '.exchange.7.101', 'output': 'exchange', 'version': '7', 'index': '101'}
     """
-    pipe_config = NameConfig(dict(pipe='\w+', output='\w+', version='\d+', index='\d+'))
+    pipe_config = NameConfig(dict(pipe=r'\w+', output=r'\w+', version=r'\d+', index=r'\d+'))
 
     @property
     def _pattern(self):
         sep = re.escape(self.pipe_sep)
         casted = self.cast_config(self.pipe_config)
         pat = r'(?P<pipe>({sep}{output})?{sep}{version}({sep}{index})?)'.format(sep=sep, **casted)
         return rf'{super()._pattern}{pat}'
@@ -230,15 +230,15 @@
 class PipeFile(File, Pipe):
     """
     A convenience mixin for pipeline files in a project.
 
     Example:
         >>> from naming import PipeFile
         >>> class MyPipeFile(PipeFile):
-        ...     config = dict(base=r'\w+')
+        ...     config = dict(base=r'\\w+')
         ...
         >>> p = MyPipeFile('wipfile.7.ext')
         >>> p.values
         {'base': 'wipfile', 'pipe': '.7', 'version': '7', 'suffix': 'ext'}
         >>> [p.get(index=x, output='render') for x in range(10)]
         ['wipfile.render.7.0.ext',
         'wipfile.render.7.1.ext',
```

### Comparing `naming-0.7.0/naming/base.py` & `naming-0.7.1/naming/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import typing
 from itertools import chain
 from collections import ChainMap
 from types import MappingProxyType
 
 
 def _dct_from_mro(cls: type, attr_name: str) -> dict:
-    """"Get a merged dictionary from `cls` bases attribute `attr_name`. MRO defines importance (closest = strongest)."""
+    """Get a merged dictionary from `cls` bases attribute `attr_name`. MRO defines importance (closest = strongest)."""
     d = {}
     for c in reversed(cls.mro()):
         d.update(getattr(c, attr_name, {}))
     return d
 
 
 def _sorted_items(mapping: typing.Mapping) -> typing.Generator:
```

### Comparing `naming-0.7.0/naming/tests/__init__.py` & `naming-0.7.1/tests/test_naming.py`

 * *Files identical despite different names*

### Comparing `naming-0.7.0/naming.egg-info/PKG-INFO` & `naming-0.7.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 Metadata-Version: 2.1
 Name: naming
-Version: 0.7.0
+Version: 0.7.1
 Summary: Object-oriented names for the digital era.
 Home-page: https://github.com/chrizzFTD/naming
 Author: Christian López Barrón
 Author-email: chris.gfz@gmail.com
 Keywords: name names naming convention configuration config cfg regex
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
-Provides-Extra: docs
 License-File: LICENSE
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: myst-parser; extra == "docs"
+Requires-Dist: sphinx-toggleprompt; extra == "docs"
+Requires-Dist: sphinx-copybutton; extra == "docs"
+Requires-Dist: sphinx-togglebutton; extra == "docs"
+Requires-Dist: sphinx-hoverxref; extra == "docs"
+Requires-Dist: sphinx_autodoc_typehints; extra == "docs"
+Requires-Dist: sphinx_rtd_theme; extra == "docs"
 
 # naming
 [![Build Status](https://travis-ci.org/chrizzFTD/naming.svg?branch=master)](https://travis-ci.org/chrizzFTD/naming)
 [![Coverage Status](https://coveralls.io/repos/github/chrizzFTD/naming/badge.svg?branch=master)](https://coveralls.io/github/chrizzFTD/naming?branch=master)
 [![Documentation Status](https://readthedocs.org/projects/naming/badge/?version=latest)](https://naming.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/naming.svg)](https://badge.fury.io/py/naming)
 [![PyPI](https://img.shields.io/pypi/pyversions/naming.svg)](https://pypi.python.org/pypi/naming)
 
-Object-oriented names for the digital era.
+> Object-oriented names for the digital era.
 
 `naming` provides an interface for dealing with naming conventions; from
 defining them, to identifying names and creating new ones.
     
-### Installation
+## Installation
 
-`naming` is available for Python 3.7 onwards via PyPI.
+`naming` is available for Python 3.8+ via PyPI.
 
 ```bash
 $ pip install naming
 ```
 
-### Usage
+## Example
 
-Please refer to the [documentation](http://naming.readthedocs.io/en/latest/) for details on contents and usage.
+Please refer to the [documentation walkthrough](http://naming.readthedocs.io/en/latest/) for details on contents and usage.
 
 ```python
 >>> import naming
 >>> class NameFileConvention(naming.Name, naming.File):
 ...     config = dict(first=r'\w+', last=r'\w+', number=r'\d+')
 ...
 >>> name = NameFileConvention('john doe 07.jpg')
```

### Comparing `naming-0.7.0/setup.cfg` & `naming-0.7.1/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206e 616d 696e 670d 0a76 6572 7369   = naming..versi
-00000020: 6f6e 203d 2030 2e37 2e30 0d0a 6465 7363  on = 0.7.0..desc
+00000020: 6f6e 203d 2030 2e37 2e31 0d0a 6465 7363  on = 0.7.1..desc
 00000030: 7269 7074 696f 6e20 3d20 4f62 6a65 6374  ription = Object
 00000040: 2d6f 7269 656e 7465 6420 6e61 6d65 7320  -oriented names 
 00000050: 666f 7220 7468 6520 6469 6769 7461 6c20  for the digital 
 00000060: 6572 612e 0d0a 6c6f 6e67 5f64 6573 6372  era...long_descr
 00000070: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
 00000080: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
 00000090: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
@@ -20,25 +20,34 @@
 00000130: 7269 7374 6961 6e20 4cc3 b370 657a 2042  ristian L..pez B
 00000140: 6172 72c3 b36e 0d0a 7572 6c20 3d20 6874  arr..n..url = ht
 00000150: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00000160: 2f63 6872 697a 7a46 5444 2f6e 616d 696e  /chrizzFTD/namin
 00000170: 670d 0a63 6c61 7373 6966 6965 7273 203d  g..classifiers =
 00000180: 200d 0a09 5072 6f67 7261 6d6d 696e 6720   ...Programming 
 00000190: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000001a0: 6f6e 203a 3a20 332e 370d 0a09 5072 6f67  on :: 3.7...Prog
+000001a0: 6f6e 203a 3a20 332e 380d 0a09 5072 6f67  on :: 3.8...Prog
 000001b0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
 000001c0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-000001d0: 380d 0a09 5072 6f67 7261 6d6d 696e 6720  8...Programming 
+000001d0: 390d 0a09 5072 6f67 7261 6d6d 696e 6720  9...Programming 
 000001e0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-000001f0: 6f6e 203a 3a20 332e 390d 0a0d 0a5b 6f70  on :: 3.9....[op
-00000200: 7469 6f6e 735d 0d0a 7061 636b 6167 6573  tions]..packages
-00000210: 203d 2066 696e 643a 0d0a 0d0a 5b6f 7074   = find:....[opt
-00000220: 696f 6e73 2e65 7874 7261 735f 7265 7175  ions.extras_requ
-00000230: 6972 655d 0d0a 646f 6373 203d 2073 7068  ire]..docs = sph
-00000240: 696e 785f 6175 746f 646f 635f 7479 7065  inx_autodoc_type
-00000250: 6869 6e74 733b 2073 7068 696e 785f 7274  hints; sphinx_rt
-00000260: 645f 7468 656d 653b 2073 7068 696e 782d  d_theme; sphinx-
-00000270: 746f 6767 6c65 7072 6f6d 7074 3b20 7370  toggleprompt; sp
-00000280: 6869 6e78 2d63 6f70 7962 7574 746f 6e3b  hinx-copybutton;
-00000290: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
-000002a0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
-000002b0: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
+000001f0: 6f6e 203a 3a20 332e 3130 0d0a 0950 726f  on :: 3.10...Pro
+00000200: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+00000210: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+00000220: 2e31 310d 0a09 5072 6f67 7261 6d6d 696e  .11...Programmin
+00000230: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000240: 7468 6f6e 203a 3a20 332e 3132 0d0a 0d0a  thon :: 3.12....
+00000250: 5b6f 7074 696f 6e73 5d0d 0a70 6163 6b61  [options]..packa
+00000260: 6765 7320 3d20 6669 6e64 3a0d 0a0d 0a5b  ges = find:....[
+00000270: 6f70 7469 6f6e 732e 6578 7472 6173 5f72  options.extras_r
+00000280: 6571 7569 7265 5d0d 0a64 6f63 7320 3d20  equire]..docs = 
+00000290: 7370 6869 6e78 3b20 6d79 7374 2d70 6172  sphinx; myst-par
+000002a0: 7365 723b 2073 7068 696e 782d 746f 6767  ser; sphinx-togg
+000002b0: 6c65 7072 6f6d 7074 3b20 7370 6869 6e78  leprompt; sphinx
+000002c0: 2d63 6f70 7962 7574 746f 6e3b 2073 7068  -copybutton; sph
+000002d0: 696e 782d 746f 6767 6c65 6275 7474 6f6e  inx-togglebutton
+000002e0: 3b20 7370 6869 6e78 2d68 6f76 6572 7872  ; sphinx-hoverxr
+000002f0: 6566 3b20 7370 6869 6e78 5f61 7574 6f64  ef; sphinx_autod
+00000300: 6f63 5f74 7970 6568 696e 7473 3b20 7370  oc_typehints; sp
+00000310: 6869 6e78 5f72 7464 5f74 6865 6d65 0d0a  hinx_rtd_theme..
+00000320: 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a 7461  ..[egg_info]..ta
+00000330: 675f 6275 696c 6420 3d20 0d0a 7461 675f  g_build = ..tag_
+00000340: 6461 7465 203d 2030 0d0a 0d0a            date = 0....
```

