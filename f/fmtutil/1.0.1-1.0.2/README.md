# Comparing `tmp/fmtutil-1.0.1.tar.gz` & `tmp/fmtutil-1.0.2.tar.gz`

## Comparing `fmtutil-1.0.1.tar` & `fmtutil-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 fmtutil-1.0.1/fmtutil/__about__.py
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 fmtutil-1.0.1/fmtutil/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fmtutil-1.0.1/fmtutil/__main__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 fmtutil-1.0.1/fmtutil/__type.py
--rw-r--r--   0        0        0    36676 2020-02-02 00:00:00.000000 fmtutil-1.0.1/fmtutil/__version.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 fmtutil-1.0.1/fmtutil/cli.py
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 fmtutil-1.0.1/fmtutil/exceptions.py
--rw-r--r--   0        0        0   133174 2020-02-02 00:00:00.000000 fmtutil-1.0.1/fmtutil/formatter.py
--rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 fmtutil-1.0.1/fmtutil/utils.py
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 fmtutil-1.0.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fmtutil-1.0.1/LICENSE
--rw-r--r--   0        0        0     7726 2020-02-02 00:00:00.000000 fmtutil-1.0.1/README.md
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 fmtutil-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     8836 2020-02-02 00:00:00.000000 fmtutil-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 fmtutil-1.0.2/fmtutil/__about__.py
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 fmtutil-1.0.2/fmtutil/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 fmtutil-1.0.2/fmtutil/__main__.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 fmtutil-1.0.2/fmtutil/__type.py
+-rw-r--r--   0        0        0    36758 2020-02-02 00:00:00.000000 fmtutil-1.0.2/fmtutil/__version.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 fmtutil-1.0.2/fmtutil/cli.py
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 fmtutil-1.0.2/fmtutil/exceptions.py
+-rw-r--r--   0        0        0   133452 2020-02-02 00:00:00.000000 fmtutil-1.0.2/fmtutil/formatter.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 fmtutil-1.0.2/fmtutil/utils.py
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 fmtutil-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fmtutil-1.0.2/LICENSE
+-rw-r--r--   0        0        0     7978 2020-02-02 00:00:00.000000 fmtutil-1.0.2/README.md
+-rw-r--r--   0        0        0     3334 2020-02-02 00:00:00.000000 fmtutil-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     9126 2020-02-02 00:00:00.000000 fmtutil-1.0.2/PKG-INFO
```

### Comparing `fmtutil-1.0.1/fmtutil/__init__.py` & `fmtutil-1.0.2/fmtutil/__init__.py`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.1/fmtutil/__type.py` & `fmtutil-1.0.2/fmtutil/__type.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 # * https://github.com/python-semver/python-semver
 # * https://github.com/pypa/packaging
 # ------------------------------------------------------------------------------
 from __future__ import annotations
 
 from typing import Union
 
-String = Union[str, bytes]
-DictStr = dict[str, str]
-TupleInt = tuple[int, ...]
+from typing_extensions import TypeAlias
+
+String: TypeAlias = Union[str, bytes]
+DictStr: TypeAlias = dict[str, str]
+TupleInt: TypeAlias = tuple[int, ...]
 
 
 class InfObject:
     def __repr__(self) -> str:
         return "Infinity"
 
     def __hash__(self) -> int:
```

### Comparing `fmtutil-1.0.1/fmtutil/__version.py` & `fmtutil-1.0.2/fmtutil/__version.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,22 +21,29 @@
     Optional,
     SupportsInt,
     Union,
     cast,
     get_args,
 )
 
+from typing_extensions import TypeAlias
+
 from .__type import (
     Inf,
     NegInf,
     String,
 )
 
-Comparable = Union["BaseVersion", dict[str, int], Collection[int], str]
-Comparator = Callable[["BaseVersion", Comparable], bool]
+Comparable: TypeAlias = Union[
+    "BaseVersion",
+    dict[str, int],
+    Collection[int],
+    str,
+]
+Comparator: TypeAlias = Callable[["BaseVersion", Comparable], bool]
 
 
 class RegVersion:
     """Regular Expression for Any Version object.
 
     .. class-attributes::
         * version:
```

### Comparing `fmtutil-1.0.1/fmtutil/cli.py` & `fmtutil-1.0.2/fmtutil/cli.py`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.1/fmtutil/exceptions.py` & `fmtutil-1.0.2/fmtutil/exceptions.py`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.1/fmtutil/formatter.py` & `fmtutil-1.0.2/fmtutil/formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     Optional,
     TypedDict,
     Union,
     final,  # docs: https://github.com/python/mypy/issues/9953
 )
 
 from dateutil.relativedelta import relativedelta
+from typing_extensions import TypeAlias
 
 from .__type import (
     DictStr,
     String,
     TupleInt,
 )
 from .__version import (
@@ -59,16 +60,20 @@
     remove_pad,
 )
 
 FormatterType = type["Formatter"]
 FormatterGroupType = type["FormatterGroup"]
 ConstantType = type["Constant"]
 
-PriorityCallable = Union[Callable[[Any], Any], Callable[[], Any], partial[Any]]
-FormatterCallable = Union[Callable[[], Any], partial[Any]]
+PriorityCallable: TypeAlias = Union[
+    Callable[[Any], Any],
+    Callable[[], Any],
+    partial[Any],
+]
+FormatterCallable: TypeAlias = Union[Callable[[], Any], partial[Any]]
 
 
 class PriorityValue(TypedDict):
     """Type Dictionary for value of mapping of ``cls.priorities``"""
 
     value: PriorityCallable
     level: Optional[Union[int, TupleInt]]
@@ -86,16 +91,16 @@
 class RegexValue(TypedDict):
     """Type Dictionary for value of mapping of ``cls.formatter``"""
 
     value: Union[FormatterCallable, str]
     regex: str
 
 
-ReturnPrioritiesType = dict[str, PriorityValue]
-ReturnFormattersType = dict[str, Union[CRegexValue, RegexValue]]
+ReturnPrioritiesType: TypeAlias = dict[str, PriorityValue]
+ReturnFormattersType: TypeAlias = dict[str, Union[CRegexValue, RegexValue]]
 
 
 @total_ordering
 class SlotLevel:
     """Slot level object for order priority values. This was mean if
     you implement this slot level object to attribute on your class
     and update level to an instance when it has some action, it will
@@ -915,14 +920,17 @@
 
     def __rsub__(self, other: Union[Formatter, Any]) -> Any:
         try:
             return other - self.value
         except (TypeError, FormatterValueError):
             return NotImplemented
 
+    def __format__(self, format_spec) -> str:
+        return self.format(format_spec)
+
 
 class Serial(Formatter):
     """Serial formatter object that parse and format any serial (positive
     integer) value.
     """
 
     base_fmt: str = "%n"
@@ -3024,15 +3032,15 @@
         :rtype: decimal.Decimal
         :return: A converted byte value that depend on an input order value.
         """
         p: Decimal = Decimal(math.pow(1024, SIZE.index(order)))
         return Storage.round_up(Decimal(value.replace(order, "")) * p)
 
 
-ConstantComparator = Callable[["Constant", "Constant"], bool]
+ConstantComparator: TypeAlias = Callable[["Constant", "Constant"], bool]
 
 
 def const_comparison(operator: ConstantComparator) -> ConstantComparator:
     @wraps(operator)
     def wrapper(self: Constant, other) -> bool:
         if not issubclass(other.__class__, Constant):
             return NotImplemented
@@ -3426,23 +3434,27 @@
     """Type Dictionary for value of mapping of ``ReturnParseType``."""
 
     fmt: str
     value: str
     props: DictStr
 
 
-ReturnGroupGenFormatType = dict[str, GenFormatValue]
-ReturnParseType = dict[str, ParseValue]
+ReturnGroupGenFormatType: TypeAlias = dict[str, GenFormatValue]
+ReturnParseType: TypeAlias = dict[str, ParseValue]
 
 
-BaseGroupsType = dict[str, FormatterType]
-GroupsType = dict[str, Formatter]
-FormatsGroupType = Union[dict[str, DictStr], GroupsType, dict[str, Any]]
+BaseGroupsType: TypeAlias = dict[str, FormatterType]
+GroupsType: TypeAlias = dict[str, Formatter]
+FormatsGroupType: TypeAlias = Union[
+    dict[str, DictStr],
+    GroupsType,
+    dict[str, Any],
+]
 
-Comparator = Callable[["FormatterGroup", "FormatterGroup"], bool]
+Comparator: TypeAlias = Callable[["FormatterGroup", "FormatterGroup"], bool]
 
 
 def comparison(operator: Comparator) -> Comparator:
     @wraps(operator)
     def wrapper(self: FormatterGroup, other) -> bool:
         if not (
             issubclass(other.__class__, FormatterGroup)
```

### Comparing `fmtutil-1.0.1/fmtutil/utils.py` & `fmtutil-1.0.2/fmtutil/utils.py`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.1/.gitignore` & `fmtutil-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.1/LICENSE` & `fmtutil-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fmtutil-1.0.1/README.md` & `fmtutil-1.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,40 @@
-# Utility Package: *Formatter*
+# _Formatter Utility_
 
 [![test](https://github.com/korawica/fmtutil/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/korawica/fmtutil/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/korawica/fmtutil/branch/main/graph/badge.svg?token=J2MN63IFT0)](https://codecov.io/gh/korawica/fmtutil)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fmtutil?logo=pypi)](https://pypi.org/project/fmtutil/)
 [![size](https://img.shields.io/github/languages/code-size/korawica/fmtutil)](https://github.com/korawica/fmtutil)
 
 **Table of Contents**:
 
-- [Installation](#installation)
-- [Formatter Objects](#formatter-objects)
-  - [Datetime](#datetime)
-  - [Version](#version)
-  - [Serial](#serial)
-  - [Naming](#naming)
-  - [Storage](#storage)
-  - [Constant](#constant)
-- [FormatterGroup Object](#formattergroup-object)
-- [Usecase](#usecase)
+* [Installation](#installation)
+* [Formatter Objects](#formatter-objects)
+  * [Datetime](#datetime)
+  * [Version](#version)
+  * [Serial](#serial)
+  * [Naming](#naming)
+  * [Storage](#storage)
+  * [Constant](#constant)
+* [FormatterGroup Object](#formattergroup-object)
+* [Usecase](#usecase)
 
 This **Formatter Utility Objects** package was created for `parse` and `format`
 any string values that match a format pattern string with Python regular
 expression. This package be the co-pylot project for stating to my
 **Python Software Developer** role.
 
 :dart: First objective of this project is include necessary formatter objects for
 any data components package which mean we can `parse` any complicate names on
 data source and ingest the right names to in-house or data target.
 
 ## Installation
 
 ```shell
-pip install fmtutil
+pip install -U fmtutil
 ```
 
 For example, we want to get filename with the format like, `filename_20220101.csv`,
 on the file system storage, and we want to incremental ingest the latest file with
 date **2022-03-25** date. So we will implement `Datetime` object and parse
 that filename to it,
 
@@ -54,40 +54,47 @@
 {filename:%s}_{datetime:%Y_%m_%d}.{version:%m.%n.%c}.csv
 ```
 
 From above filename format string, the `datetime` package does not enough for
 this scenario right? but you can handle by your hard-code object or create the
 better package than this project.
 
-> **Note**: \
+> [!NOTE]
 > Any formatter object was implemented the `self.valid` method for help us validate
 > format string value like the above the example scenario,
 > ```python
 > this_date = Datetime.parse('20220101', '%Y%m%d')
-> this_date.valid('any_files_20220101.csv', 'any_files_%Y%m%d.csv')  # True
+> assert this_date.valid('any_files_20220101.csv', 'any_files_%Y%m%d.csv')
 > ```
 
+**Dependency supported**:
+
+| Python Version  | Installation                        |
+|-----------------|-------------------------------------|
+| `== 3.8`        | `pip install "fmtutil>=0.4,<0.5.0"` |
+| `>=3.9,<3.13`   | `pip install -U fmtutil`            |
+
 ## Formatter Objects
 
-- [Datetime](#datetime)
-- [Version](#version)
-- [Serial](#serial)
-- [Naming](#naming)
-- [Storage](#storage)
-- [Constant](#constant)
+* [Datetime](#datetime)
+* [Version](#version)
+* [Serial](#serial)
+* [Naming](#naming)
+* [Storage](#storage)
+* [Constant](#constant)
 
 The main purpose is **Formatter Objects** for `parse` and `format` with string
 value, such as `Datetime`, `Version`, and `Serial` formatter objects. These objects
 were used for parse any filename with put the format string value.
 
 The formatter able to enhancement any format value from sting value, like in
 `Datetime`, for `%B` value that was designed for month shortname (`Jan`,
 `Feb`, etc.) that does not support in build-in `datetime` package.
 
-> **Note**: \
+> [!IMPORTANT]
 > The main usage of this formatter object is `parse` and `format` method.
 
 ### Datetime
 
 ```python
 from fmtutil import Datetime
 
@@ -175,15 +182,15 @@
     pass
 ```
 
 ```text
 >>> 'The value of %s is special'
 ```
 
-> **Note**: \
+> [!NOTE]
 > This package already implement the environment constant object,
 > `fmtutil.EnvConst`. \
 > [Read more about this formats](/docs/en/docs/API.md#environment-constant)
 
 ## FormatterGroup Object
 
 The **FormatterGroup** object, `FormatterGroup`, which is the grouping of needed
@@ -232,15 +239,18 @@
 
 from fmtutil import (
   make_group, Naming, Datetime, FormatterGroup, FormatterGroupType, FormatterArgumentError,
 )
 
 name: Naming = Naming.parse('Google Map', fmt='%t')
 
-fmt_group: FormatterGroupType = make_group({"naming": name.to_const(), "timestamp": Datetime})
+fmt_group: FormatterGroupType = make_group({
+    "naming": name.to_const(),
+    "timestamp": Datetime,
+})
 
 rs: List[FormatterGroup] = []
 for file in (
     'googleMap_20230101.json',
     'googleMap_20230103.json',
     'googleMap_20230103_bk.json',
     'googleMap_with_usage_20230105.json',
@@ -256,15 +266,15 @@
 repr(max(rs).groups['timestamp'])
 ```
 
 ```text
 >>> <Datetime.parse('2023-01-03 00:00:00.000000', '%Y-%m-%d %H:%M:%S.%f')>
 ```
 
-> **Note**: \
+> [!TIP]
 > The above example will convert the `name`, Naming instance, to Constant
 > instance before passing to the formatter group because it does not want
 > to dynamic this naming format when find any filenames in target path.
 
 ## License
 
 This project was licensed under the terms of the [MIT license](LICENSE).
```

### Comparing `fmtutil-1.0.1/pyproject.toml` & `fmtutil-1.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -27,25 +27,28 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
-dependencies = ["python-dateutil>=2.8.2,<3.0.0"]
+dependencies = [
+    "python-dateutil>=2.8.2,<3.0.0",
+    "typing-extensions",
+]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/korawica/fmtutil/"
 "Source Code" = "https://github.com/korawica/fmtutil/"
 
 [project.optional-dependencies]
 dev = [
     "clishelf",
-    "types-python-dateutil==2.8.19.14",
+    "types-python-dateutil==2.9.0.20240316",
 ]
 perf = [
     "memory-profiler==0.61.0",
 ]
 
 [project.scripts]
 fmtutil = "fmtutil.__main__:main"
@@ -136,30 +139,30 @@
         | venv
     )/
 )
 """
 
 [tool.ruff]
 line-length = 80
-select = [
+lint.select = [
     "E",  # pycodestyle errors
     "W",  # pycodestyle warnings
     "F",  # pyflakes
     "I",  # isort
     "C",  # flake8-comprehensions
     "B",  # flake8-bugbear
 ]
-ignore = [
+lint.ignore = [
     "E501",  # line too long, handled by black
     "B008",  # do not perform function calls in argument defaults
     "C901",  # too complex
 ]
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".git",
     ".mypy_cache",
     ".ruff_cache",
     "venv",
 ]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
```

### Comparing `fmtutil-1.0.1/PKG-INFO` & `fmtutil-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: fmtutil
-Version: 1.0.1
+Version: 1.0.2
 Summary: The Utility Formatter Objects
 Project-URL: Homepage, https://github.com/korawica/fmtutil/
 Project-URL: Source Code, https://github.com/korawica/fmtutil/
 Author-email: korawica <korawich.anu@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: formatter,utility
@@ -16,54 +16,55 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Requires-Python: >=3.9.0
 Requires-Dist: python-dateutil<3.0.0,>=2.8.2
+Requires-Dist: typing-extensions
 Provides-Extra: dev
 Requires-Dist: clishelf; extra == 'dev'
-Requires-Dist: types-python-dateutil==2.8.19.14; extra == 'dev'
+Requires-Dist: types-python-dateutil==2.9.0.20240316; extra == 'dev'
 Provides-Extra: perf
 Requires-Dist: memory-profiler==0.61.0; extra == 'perf'
 Description-Content-Type: text/markdown
 
-# Utility Package: *Formatter*
+# _Formatter Utility_
 
 [![test](https://github.com/korawica/fmtutil/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/korawica/fmtutil/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/korawica/fmtutil/branch/main/graph/badge.svg?token=J2MN63IFT0)](https://codecov.io/gh/korawica/fmtutil)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fmtutil?logo=pypi)](https://pypi.org/project/fmtutil/)
 [![size](https://img.shields.io/github/languages/code-size/korawica/fmtutil)](https://github.com/korawica/fmtutil)
 
 **Table of Contents**:
 
-- [Installation](#installation)
-- [Formatter Objects](#formatter-objects)
-  - [Datetime](#datetime)
-  - [Version](#version)
-  - [Serial](#serial)
-  - [Naming](#naming)
-  - [Storage](#storage)
-  - [Constant](#constant)
-- [FormatterGroup Object](#formattergroup-object)
-- [Usecase](#usecase)
+* [Installation](#installation)
+* [Formatter Objects](#formatter-objects)
+  * [Datetime](#datetime)
+  * [Version](#version)
+  * [Serial](#serial)
+  * [Naming](#naming)
+  * [Storage](#storage)
+  * [Constant](#constant)
+* [FormatterGroup Object](#formattergroup-object)
+* [Usecase](#usecase)
 
 This **Formatter Utility Objects** package was created for `parse` and `format`
 any string values that match a format pattern string with Python regular
 expression. This package be the co-pylot project for stating to my
 **Python Software Developer** role.
 
 :dart: First objective of this project is include necessary formatter objects for
 any data components package which mean we can `parse` any complicate names on
 data source and ingest the right names to in-house or data target.
 
 ## Installation
 
 ```shell
-pip install fmtutil
+pip install -U fmtutil
 ```
 
 For example, we want to get filename with the format like, `filename_20220101.csv`,
 on the file system storage, and we want to incremental ingest the latest file with
 date **2022-03-25** date. So we will implement `Datetime` object and parse
 that filename to it,
 
@@ -83,40 +84,47 @@
 {filename:%s}_{datetime:%Y_%m_%d}.{version:%m.%n.%c}.csv
 ```
 
 From above filename format string, the `datetime` package does not enough for
 this scenario right? but you can handle by your hard-code object or create the
 better package than this project.
 
-> **Note**: \
+> [!NOTE]
 > Any formatter object was implemented the `self.valid` method for help us validate
 > format string value like the above the example scenario,
 > ```python
 > this_date = Datetime.parse('20220101', '%Y%m%d')
-> this_date.valid('any_files_20220101.csv', 'any_files_%Y%m%d.csv')  # True
+> assert this_date.valid('any_files_20220101.csv', 'any_files_%Y%m%d.csv')
 > ```
 
+**Dependency supported**:
+
+| Python Version  | Installation                        |
+|-----------------|-------------------------------------|
+| `== 3.8`        | `pip install "fmtutil>=0.4,<0.5.0"` |
+| `>=3.9,<3.13`   | `pip install -U fmtutil`            |
+
 ## Formatter Objects
 
-- [Datetime](#datetime)
-- [Version](#version)
-- [Serial](#serial)
-- [Naming](#naming)
-- [Storage](#storage)
-- [Constant](#constant)
+* [Datetime](#datetime)
+* [Version](#version)
+* [Serial](#serial)
+* [Naming](#naming)
+* [Storage](#storage)
+* [Constant](#constant)
 
 The main purpose is **Formatter Objects** for `parse` and `format` with string
 value, such as `Datetime`, `Version`, and `Serial` formatter objects. These objects
 were used for parse any filename with put the format string value.
 
 The formatter able to enhancement any format value from sting value, like in
 `Datetime`, for `%B` value that was designed for month shortname (`Jan`,
 `Feb`, etc.) that does not support in build-in `datetime` package.
 
-> **Note**: \
+> [!IMPORTANT]
 > The main usage of this formatter object is `parse` and `format` method.
 
 ### Datetime
 
 ```python
 from fmtutil import Datetime
 
@@ -204,15 +212,15 @@
     pass
 ```
 
 ```text
 >>> 'The value of %s is special'
 ```
 
-> **Note**: \
+> [!NOTE]
 > This package already implement the environment constant object,
 > `fmtutil.EnvConst`. \
 > [Read more about this formats](/docs/en/docs/API.md#environment-constant)
 
 ## FormatterGroup Object
 
 The **FormatterGroup** object, `FormatterGroup`, which is the grouping of needed
@@ -261,15 +269,18 @@
 
 from fmtutil import (
   make_group, Naming, Datetime, FormatterGroup, FormatterGroupType, FormatterArgumentError,
 )
 
 name: Naming = Naming.parse('Google Map', fmt='%t')
 
-fmt_group: FormatterGroupType = make_group({"naming": name.to_const(), "timestamp": Datetime})
+fmt_group: FormatterGroupType = make_group({
+    "naming": name.to_const(),
+    "timestamp": Datetime,
+})
 
 rs: List[FormatterGroup] = []
 for file in (
     'googleMap_20230101.json',
     'googleMap_20230103.json',
     'googleMap_20230103_bk.json',
     'googleMap_with_usage_20230105.json',
@@ -285,15 +296,15 @@
 repr(max(rs).groups['timestamp'])
 ```
 
 ```text
 >>> <Datetime.parse('2023-01-03 00:00:00.000000', '%Y-%m-%d %H:%M:%S.%f')>
 ```
 
-> **Note**: \
+> [!TIP]
 > The above example will convert the `name`, Naming instance, to Constant
 > instance before passing to the formatter group because it does not want
 > to dynamic this naming format when find any filenames in target path.
 
 ## License
 
 This project was licensed under the terms of the [MIT license](LICENSE).
```

