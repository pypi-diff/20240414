# Comparing `tmp/prep-flow-0.1.0.tar.gz` & `tmp/prep_flow-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prep-flow-0.1.0.tar", last modified: Sat Apr 13 06:31:01 2024, max compression
+gzip compressed data, was "prep_flow-0.1.1.tar", last modified: Sun Apr 14 08:17:27 2024, max compression
```

## Comparing `prep-flow-0.1.0.tar` & `prep_flow-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,32 @@
-drwxr-xr-x   0 katoutomohiko   (501) staff       (20)        0 2024-04-13 06:31:01.994441 prep-flow-0.1.0/
--rw-r--r--   0 katoutomohiko   (501) staff       (20)     3116 2024-04-13 06:29:13.000000 prep-flow-0.1.0/.gitignore
--rw-r--r--   0 katoutomohiko   (501) staff       (20)      294 2024-04-13 02:04:39.000000 prep-flow-0.1.0/Dockerfile
--rw-r--r--   0 katoutomohiko   (501) staff       (20)     1070 2024-04-13 04:27:13.000000 prep-flow-0.1.0/LICENSE
--rw-r--r--   0 katoutomohiko   (501) staff       (20)     1949 2024-04-13 06:31:01.994387 prep-flow-0.1.0/PKG-INFO
--rw-r--r--   0 katoutomohiko   (501) staff       (20)       83 2024-04-13 04:28:24.000000 prep-flow-0.1.0/README.md
--rw-r--r--   0 katoutomohiko   (501) staff       (20)      216 2024-04-13 01:32:03.000000 prep-flow-0.1.0/docker-compose.yml
-drwxr-xr-x   0 katoutomohiko   (501) staff       (20)        0 2024-04-13 06:31:01.992344 prep-flow-0.1.0/prep_flow/
--rw-r--r--   0 katoutomohiko   (501) staff       (20)      672 2024-04-13 05:59:09.000000 prep-flow-0.1.0/prep_flow/__init__.py
--rw-r--r--   0 katoutomohiko   (501) staff       (20)    16240 2024-04-13 05:02:01.000000 prep-flow-0.1.0/prep_flow/base_loader.py
--rw-r--r--   0 katoutomohiko   (501) staff       (20)     1139 2024-03-20 01:51:52.000000 prep-flow-0.1.0/prep_flow/decorators.py
--rw-r--r--   0 katoutomohiko   (501) staff       (20)     2660 2024-04-13 04:35:44.000000 prep-flow-0.1.0/prep_flow/errors.py
--rw-r--r--   0 katoutomohiko   (501) staff       (20)     6274 2024-04-13 05:02:01.000000 prep-flow-0.1.0/prep_flow/expressions.py
--rw-r--r--   0 katoutomohiko   (501) staff       (20)     6633 2024-04-13 04:35:44.000000 prep-flow-0.1.0/prep_flow/validator.py
-drwxr-xr-x   0 katoutomohiko   (501) staff       (20)        0 2024-04-13 06:31:01.993817 prep-flow-0.1.0/prep_flow.egg-info/
--rw-r--r--   0 katoutomohiko   (501) staff       (20)     1949 2024-04-13 06:31:01.000000 prep-flow-0.1.0/prep_flow.egg-info/PKG-INFO
--rw-r--r--   0 katoutomohiko   (501) staff       (20)      453 2024-04-13 06:31:01.000000 prep-flow-0.1.0/prep_flow.egg-info/SOURCES.txt
--rw-r--r--   0 katoutomohiko   (501) staff       (20)        1 2024-04-13 06:31:01.000000 prep-flow-0.1.0/prep_flow.egg-info/dependency_links.txt
--rw-r--r--   0 katoutomohiko   (501) staff       (20)       93 2024-04-13 06:31:01.000000 prep-flow-0.1.0/prep_flow.egg-info/requires.txt
--rw-r--r--   0 katoutomohiko   (501) staff       (20)       21 2024-04-13 06:31:01.000000 prep-flow-0.1.0/prep_flow.egg-info/top_level.txt
--rw-r--r--   0 katoutomohiko   (501) staff       (20)      753 2024-04-13 06:30:42.000000 prep-flow-0.1.0/pyproject.toml
--rw-r--r--   0 katoutomohiko   (501) staff       (20)      479 2024-04-13 02:12:53.000000 prep-flow-0.1.0/requirements.txt
--rw-r--r--   0 katoutomohiko   (501) staff       (20)      321 2024-04-13 06:31:01.994673 prep-flow-0.1.0/setup.cfg
-drwxr-xr-x   0 katoutomohiko   (501) staff       (20)        0 2024-04-13 06:31:01.993559 prep-flow-0.1.0/tests/
--rw-r--r--   0 katoutomohiko   (501) staff       (20)    16811 2024-04-13 05:02:01.000000 prep-flow-0.1.0/tests/test_base_loader.py
--rw-r--r--   0 katoutomohiko   (501) staff       (20)     6423 2024-04-13 04:35:45.000000 prep-flow-0.1.0/tests/test_validator.py
+drwxr-xr-x   0 katoutomohiko   (501) staff       (20)        0 2024-04-14 08:17:27.726793 prep_flow-0.1.1/
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)     3127 2024-04-13 06:45:50.000000 prep_flow-0.1.1/.gitignore
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)      294 2024-04-13 02:04:39.000000 prep_flow-0.1.1/Dockerfile
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)     1070 2024-04-13 04:27:13.000000 prep_flow-0.1.1/LICENSE
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)     3774 2024-04-14 08:17:27.726717 prep_flow-0.1.1/PKG-INFO
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)     1870 2024-04-14 08:10:11.000000 prep_flow-0.1.1/README.md
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)      247 2024-04-13 07:57:42.000000 prep_flow-0.1.1/docker-compose.yml
+drwxr-xr-x   0 katoutomohiko   (501) staff       (20)        0 2024-04-14 08:17:27.723160 prep_flow-0.1.1/prep_flow/
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)      713 2024-04-14 05:23:56.000000 prep_flow-0.1.1/prep_flow/__init__.py
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)    19561 2024-04-14 05:24:01.000000 prep_flow-0.1.1/prep_flow/base.py
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)     1219 2024-04-14 05:24:01.000000 prep_flow-0.1.1/prep_flow/decorators.py
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)     4198 2024-04-14 05:24:01.000000 prep_flow-0.1.1/prep_flow/errors.py
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)     7196 2024-04-14 05:24:01.000000 prep_flow-0.1.1/prep_flow/expressions.py
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)     6538 2024-04-14 07:21:20.000000 prep_flow-0.1.1/prep_flow/validator.py
+drwxr-xr-x   0 katoutomohiko   (501) staff       (20)        0 2024-04-14 08:17:27.726180 prep_flow-0.1.1/prep_flow.egg-info/
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)     3774 2024-04-14 08:17:27.000000 prep_flow-0.1.1/prep_flow.egg-info/PKG-INFO
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)      560 2024-04-14 08:17:27.000000 prep_flow-0.1.1/prep_flow.egg-info/SOURCES.txt
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)        1 2024-04-14 08:17:27.000000 prep_flow-0.1.1/prep_flow.egg-info/dependency_links.txt
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)      101 2024-04-14 08:17:27.000000 prep_flow-0.1.1/prep_flow.egg-info/requires.txt
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)       29 2024-04-14 08:17:27.000000 prep_flow-0.1.1/prep_flow.egg-info/top_level.txt
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)      768 2024-04-14 08:17:03.000000 prep_flow-0.1.1/pyproject.toml
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)     2212 2024-04-13 07:13:25.000000 prep_flow-0.1.1/requirements.txt
+drwxr-xr-x   0 katoutomohiko   (501) staff       (20)        0 2024-04-14 08:17:27.724253 prep_flow-0.1.1/samples/
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)    19363 2024-04-14 08:16:13.000000 prep_flow-0.1.1/samples/01_simple_usage.ipynb
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)      321 2024-04-14 08:17:27.727025 prep_flow-0.1.1/setup.cfg
+drwxr-xr-x   0 katoutomohiko   (501) staff       (20)        0 2024-04-14 08:17:27.724962 prep_flow-0.1.1/tests/
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)        0 2024-04-13 06:49:37.000000 prep_flow-0.1.1/tests/__init__.py
+drwxr-xr-x   0 katoutomohiko   (501) staff       (20)        0 2024-04-14 08:17:27.725629 prep_flow-0.1.1/tests/data/
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)     9016 2024-03-17 02:23:28.000000 prep_flow-0.1.1/tests/data/test_parse_data.xlsx
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)     9025 2024-03-17 02:55:07.000000 prep_flow-0.1.1/tests/data/test_validate_sheet_name.xlsx
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)    24527 2024-04-14 05:24:15.000000 prep_flow-0.1.1/tests/test_base.py
+-rw-r--r--   0 katoutomohiko   (501) staff       (20)     6687 2024-04-14 07:18:59.000000 prep_flow-0.1.1/tests/test_validator.py
```

### Comparing `prep-flow-0.1.0/.gitignore` & `prep_flow-0.1.1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -156,8 +156,10 @@
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 .idea/
 
 # upload shell to pypi
-upload.prod.sh
+upload.prod.sh
+
+.DS_Store
```

### Comparing `prep-flow-0.1.0/LICENSE` & `prep_flow-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prep-flow-0.1.0/prep_flow/__init__.py` & `prep_flow-0.1.1/prep_flow/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from prep_flow.base_loader import BaseLoader
+from prep_flow.base import BaseFlow
 from prep_flow.decorators import creator, data_filter, modifier
 from prep_flow.errors import (
     ColumnCastError,
+    DecoratorError,
+    DecoratorReturnTypeError,
     InvalidCategoryFoundError,
     InvalidDateFoundError,
     InvalidDateLiteralFoundError,
     InvalidRegexpFoundError,
     NecessaryColumnsNotFoundError,
     NullValueFoundError,
     ReferenceDataNotFoundError,
```

### Comparing `prep-flow-0.1.0/prep_flow/base_loader.py` & `prep_flow-0.1.1/prep_flow/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 from __future__ import annotations
 
 import abc
-from typing import Optional, Union
+from typing import Callable, Optional, Union
 
 import numpy as np
 import pandas as pd
 
 from prep_flow.decorators import CREATOR_KEY, DECORATOR_KEY, FILTER_KEY, MODIFIER_KEY
 from prep_flow.errors import (
     ColumnCastError,
+    DecoratorError,
+    DecoratorReturnTypeError,
     ReferenceDataNotFoundError,
     ReferenceDataNotInitializationError,
     SheetNotFoundError,
     ValueCastError,
 )
 from prep_flow.expressions import Column, DateTime, Dtype, ReferenceColumn
 from prep_flow.validator import CategoryCondition, RegexpCondition, Validator
 
 DEFAULT_SHEET_NAME = "Sheet1"
 PYPREP_PARENT_CLASS_NAME = "__pyprep_parent_class_name__"
 
 
-class BaseLoader(abc.ABC):
+class BaseFlow(abc.ABC):
     __sheetname__ = DEFAULT_SHEET_NAME
     __replace_none_to_nan__ = True
 
     def __init__(
         self,
         data: Union[pd.DataFrame, pd.ExcelFile],
-        reference_data: Optional[list[BaseLoader]] = None,
+        reference: Optional[list[BaseFlow]] = None,
     ) -> None:
         self.original = self.parse_data(data)
         self.pre_data = None
         self.data = self.original.copy()
-        self.reference_data = [] if reference_data is None else reference_data
+        self.reference = [] if reference is None else reference
         self.validator = Validator()
 
         self.execute()
 
     @classmethod
     def parse_data(cls, data: Union[pd.DataFrame, pd.ExcelFile]) -> pd.DataFrame:
         """
@@ -84,38 +86,47 @@
                 for key, val in vars(cls).items()
                 if isinstance(val, Column) or isinstance(val, ReferenceColumn)
             ]
         )
 
     def execute(self) -> None:
         # Argument Verification.
-        self.confirm_reference_data_exists()
+        self.confirm_reference_exists()
 
         # Add metadata.
         self.set_class_name_to_columns()
 
         # Convert raw data column names and verify that they are the expected type.
         self.rename()
         self.pre_validate()
         self.pre_cast()
         self.pre_data = self.data.copy()
 
         for order in self.orders():
-            # Modify original columns and validate modified columns.
-            self.apply_modifier(order=order)
+            # Modify values with Column.modifier.
+            self.apply_column_modifier(order=order)
 
-            # Create user defined columns.
-            self.apply_creator(order=order)
+            # Modify values with decorator referring to Column.
+            self.apply_column_modifier_with_decorator(order=order)
+
+            # Create user defined columns with decorator.
+            self.apply_creator_with_decorator(order=order)
 
             # Filter data.
-            self.apply_filter(order=order)
+            self.apply_filter_with_decorator(order=order)
 
             # Merge Reference columns.
             self.merge(order=order)
 
+            # Modify values with ReferenceColumn.modifier.
+            self.apply_reference_column_modifier(order=order)
+
+            # Modify values with decorator referring to ReferenceColumn.
+            self.apply_reference_column_modifier_with_decorator(order=order)
+
         # Validate all columns.
         self.post_validate(only_base=False)
         self.post_cast(only_base=False)
 
         if self.__replace_none_to_nan__:
             self.replace_none_to_nan()
 
@@ -242,14 +253,32 @@
                 for key, val in self.definitions().items()
                 if (isinstance(val, Column))
                 and (val.original_category is not None)
                 and (key not in self.additional_columns())
             ]
         )
 
+    def modifier_columns(self, order: int) -> dict[str, Callable]:
+        return dict(
+            [
+                (key, val.modifier)
+                for key, val in self.definitions().items()
+                if (not isinstance(val, ReferenceColumn)) and (val.order == order) and (val.modifier is not None)
+            ]
+        )
+
+    def modifier_reference_columns(self, order: int) -> dict[str, Callable]:
+        return dict(
+            [
+                (key, val.modifier)
+                for key, val in self.definitions().items()
+                if (isinstance(val, ReferenceColumn)) and (val.order == order) and (val.modifier is not None)
+            ]
+        )
+
     def rename_dict(self) -> dict:
         return dict(
             [
                 (val.name, key)
                 for key, val in self.definitions().items()
                 if (isinstance(val, Column)) and (val.name is not None)
             ]
@@ -324,15 +353,15 @@
         for column, dtype in self.dtype_dict().items():
             if only_base and (column in self.additional_columns()):
                 continue
             self.cast_series(column, dtype)
             self.cast_value(column, dtype)
 
     def replace_none_to_nan(self) -> None:
-        self.data = self.data.replace({None: np.nan})
+        self.data = self.data.infer_objects(copy=False).replace({None: np.nan})
 
     @classmethod
     def get_num_of_args(cls, func_name: str) -> int:
         return len(getattr(cls, func_name).__code__.co_varnames[: getattr(cls, func_name).__code__.co_argcount])
 
     @classmethod
     def get_decorators(cls, decorator_key: Optional[str] = None) -> dict:
@@ -345,40 +374,80 @@
                     if getattr(obj, DECORATOR_KEY)[0] == decorator_key:
                         decorators[attr] = getattr(obj, DECORATOR_KEY)
                 else:
                     decorators[attr] = getattr(obj, DECORATOR_KEY)
 
         return decorators
 
-    def apply_creator(self, order: int) -> None:
+    def apply_column_modifier(self, order: int) -> None:
+        modifier_columns = self.modifier_columns(order=order)
+        for column, modifier in modifier_columns.items():
+            self.data[column] = self.data[column].apply(modifier)
+
+    def apply_reference_column_modifier(self, order: int) -> None:
+        modifier_reference_columns = self.modifier_reference_columns(order=order)
+        for column, modifier in modifier_reference_columns.items():
+            self.data[column] = self.data[column].apply(modifier)
+
+    def apply_creator_with_decorator(self, order: int) -> None:
         decorators = self.get_decorators(CREATOR_KEY)
         for attr, (_, _column, _order) in decorators.items():
             if order != _order:
                 continue
+            if _column in self.reference_columns():
+                raise DecoratorError(
+                    column=_column,
+                    detail=f"Creator cannot specify reference-columns.(column: {_column})",
+                )
             if self.get_num_of_args(attr) == 1:
                 self.data[_column] = getattr(self, attr)()
             else:
-                self.data[_column] = getattr(self, attr)(self.data)
+                self.data[_column] = getattr(self, attr)(self.data.copy())
 
-    def apply_modifier(self, order: int) -> None:
+    def apply_column_modifier_with_decorator(self, order: int) -> None:
         decorators = self.get_decorators(MODIFIER_KEY)
         for attr, (_, _column, _order) in decorators.items():
+            if _column in self.reference_columns():
+                continue
             if order != _order:
                 continue
+            if _column not in self.columns(only_base=True):
+                raise DecoratorError(
+                    column=_column,
+                    detail=f"You have specified a column name that does not exist.(column: {_column})",
+                )
             if self.get_num_of_args(attr) == 1:
                 self.data[_column] = getattr(self, attr)()
             else:
-                self.data[_column] = getattr(self, attr)(self.data)
+                self.data[_column] = getattr(self, attr)(self.data.copy())
 
-    def apply_filter(self, order: int) -> None:
+    def apply_reference_column_modifier_with_decorator(self, order: int) -> None:
+        decorators = self.get_decorators(MODIFIER_KEY)
+        for attr, (_, _column, _order) in decorators.items():
+            if _column not in self.reference_columns():
+                continue
+            if order != _order:
+                continue
+            if self.get_num_of_args(attr) == 1:
+                self.data[_column] = getattr(self, attr)()
+            else:
+                self.data[_column] = getattr(self, attr)(self.data.copy())
+
+    def apply_filter_with_decorator(self, order: int) -> None:
         decorators = self.get_decorators(FILTER_KEY)
         for attr, (_, _, _order) in decorators.items():
             if order != _order:
                 continue
-            self.data = getattr(self, attr)(self.data)
+            result = getattr(self, attr)(self.data.copy())
+            if not isinstance(result, pd.DataFrame):
+                raise DecoratorReturnTypeError(
+                    dtype=type(result),
+                    detail=f"Expected return type is pd.DataFrame, But you return f{type(result)}",
+                )
+            self.data = result
 
     def sort_columns(self) -> None:
         self.data = self.data[self.columns()]
 
     @classmethod
     def set_class_name_to_columns(cls) -> None:
         for key, val in vars(cls).items():
@@ -410,33 +479,36 @@
                     tuple(sorted(val.on)) if isinstance(val.on, list) else (val.on,),
                     val.order,
                 )
             )
 
         return list(set(names))
 
-    def confirm_reference_data_exists(self) -> None:
+    def confirm_reference_exists(self) -> None:
         for _class_name, _, _, _, _ in self.get_reference_info():
-            if _class_name in [data.__class__.__name__ for data in self.reference_data]:
+            if _class_name in [data.__class__.__name__ for data in self.reference]:
                 continue
             raise ReferenceDataNotFoundError(name=_class_name)
 
     def merge(self, order: int) -> None:
         for _class_name, _columns, _how, _on, _order in self.get_reference_info():
             if order != _order:
                 continue
-            reference_data = [data for data in self.reference_data if data.__class__.__name__ == _class_name][0]
+            reference_data = [data for data in self.reference if data.__class__.__name__ == _class_name][0]
             self.data = pd.merge(
                 self.data,
                 reference_data.data[list(_columns) + list(_on)],
                 how=_how,
                 on=_on,
             )
 
     def decorator_orders(self) -> list[int]:
         return list(set([val[2] for key, val in self.get_decorators().items()]))
 
+    def column_orders(self) -> list[int]:
+        return list(set([self.column_info(column).order for column in self.columns(only_base=True)]))
+
     def reference_orders(self) -> list[int]:
         return list(set([self.column_info(column).order for column in self.reference_columns()]))
 
     def orders(self) -> list[int]:
-        return list(set(self.decorator_orders() + self.reference_orders()))
+        return list(set(self.decorator_orders() + self.column_orders() + self.reference_orders()))
```

### Comparing `prep-flow-0.1.0/prep_flow/decorators.py` & `prep_flow-0.1.1/prep_flow/decorators.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 
 DECORATOR_KEY = "__decorator__"
 CREATOR_KEY = "__creator__"
 MODIFIER_KEY = "__modifier__"
 FILTER_KEY = "__filter__"
 
 
-# TODO: ReferenceColumnに付与できないようにする
-def creator(column: str, order: int = 0) -> Callable:
+def creator(column: str, use_reference: bool = False, order: int = 0) -> Callable:
     if column is None:
         raise Exception("creator with no column specified.")
 
+    if use_reference:
+        order = 1
+
     def dec(f: Callable) -> classmethod:
         f_cls = classmethod(f)
         setattr(f_cls, DECORATOR_KEY, (CREATOR_KEY, column, order))
         return f_cls
 
     return dec
 
@@ -27,14 +29,17 @@
         f_cls = f if isinstance(f, classmethod) else classmethod(f)
         setattr(f_cls, DECORATOR_KEY, (MODIFIER_KEY, column, order))
         return f_cls
 
     return dec
 
 
-def data_filter(order: int = 0) -> Callable:
+def data_filter(use_reference: bool = False, order: int = 0) -> Callable:
+    if use_reference:
+        order = 1
+
     def dec(f: Callable) -> classmethod:
         f_cls = f if isinstance(f, classmethod) else classmethod(f)
         setattr(f_cls, DECORATOR_KEY, (FILTER_KEY, None, order))
         return f_cls
 
     return dec
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `prep-flow-0.1.0/prep_flow/expressions.py` & `prep_flow-0.1.1/prep_flow/expressions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Annotated, Any, Generic, Optional, Type, TypeVar, Union
+from typing import Annotated, Any, Callable, Generic, Optional, Type, TypeVar, Union
 
 import pandas as pd
 from pandas._libs.tslibs.timestamps import Timestamp  # noqa
 from pydantic import (
     BaseModel,
     ConfigDict,
     Field,
@@ -96,26 +96,32 @@
     nullable: bool = Field(default=True)
     regexp: Optional[str] = Field(default=None)
     category: Optional[list[Union[str, int]]] = Field(default=None)
     original_dtype: Optional[Annotated[Dtype, PlainValidator(validate_dtype)]] = Field(default=None)
     original_nullable: bool = Field(default=True)
     original_regexp: Optional[str] = Field(default=None)
     original_category: Optional[list[str]] = Field(default=None)
+    modifier: Optional[Callable] = Field(default=None)
+    order: int = Field(default=0)
+    description: Optional[str] = Field(default=None)
 
     def __init__(
         self,
         dtype: Type[Dtype],
         name: Optional[str] = None,
         nullable: Optional[bool] = True,
         regexp: Optional[str] = None,
         category: Optional[list[Union[str, int]]] = None,
         original_dtype: Optional[Type[Dtype]] = None,
         original_nullable: Optional[bool] = True,
         original_regexp: Optional[str] = None,
         original_category: Optional[list[str]] = None,
+        modifier: Optional[Callable] = None,
+        order: int = 0,
+        description: Optional[str] = None,
     ):
 
         super().__init__(
             **dict(
                 (key, val)
                 for key, val in {
                     "dtype": dtype,
@@ -123,14 +129,17 @@
                     "nullable": nullable,
                     "regexp": regexp,
                     "category": category,
                     "original_dtype": original_dtype,
                     "original_nullable": original_nullable,
                     "original_regexp": original_regexp,
                     "original_category": original_category,
+                    "modifier": modifier,
+                    "order": order,
+                    "description": description,
                 }.items()
                 if val is not None
             )
         )
 
     def __eq__(self, other) -> bool:
         if not isinstance(other, Column):
@@ -142,14 +151,17 @@
             and self.nullable == other.nullable
             and self.regexp == other.regexp
             and self.category == other.category
             and self.original_dtype == other.original_dtype
             and self.original_nullable == other.original_nullable
             and self.original_regexp == other.original_regexp
             and self.original_category == other.original_category
+            and self.modifier == other.modifier
+            and self.order == other.order
+            and self.description == other.description
         ):
             return False
 
         return True
 
 
 class ReferenceColumn(BaseModel):
@@ -159,39 +171,45 @@
     on: Union[str | list[str]]
     how: str
     order: int = Field(default=0)
     dtype: Annotated[Dtype, PlainValidator(validate_dtype)] = Field(default=None)
     nullable: bool = Field(default=True)
     regexp: Optional[str] = Field(default=None)
     category: Optional[list[str]] = Field(default=None)
+    modifier: Optional[Callable] = Field(default=None)
+    description: Optional[str] = Field(default=None)
 
     def __init__(
         self,
         column: Column,
         on: Union[str | list[str]],
         how: str,
         order: int = 0,
         dtype: Optional[Type[Dtype]] = None,
         nullable: Optional[bool] = True,
         regexp: Optional[str] = None,
         category: Optional[list[str]] = None,
+        modifier: Optional[Callable] = None,
+        description: Optional[str] = None,
     ):
 
         super().__init__(
             **dict(
                 (key, val)
                 for key, val in {
                     "column": column,
                     "on": on,
                     "how": how,
                     "order": order,
                     "dtype": dtype,
                     "nullable": nullable,
                     "regexp": regexp,
                     "category": category,
+                    "modifier": modifier,
+                    "description": description,
                 }.items()
                 if val is not None
             )
         )
 
     @field_validator("how")
     def validate_how(cls, v: Any) -> str:  # noqa
@@ -209,11 +227,13 @@
             and self.on == other.on
             and self.how == other.how
             and self.order == other.order
             and self.dtype == other.dtype
             and self.nullable == other.nullable
             and self.regexp == other.regexp
             and self.category == other.category
+            and self.modifier == other.modifier
+            and self.description == other.description
         ):
             return False
 
         return True
```

### Comparing `prep-flow-0.1.0/prep_flow/validator.py` & `prep_flow-0.1.1/prep_flow/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import re
-from typing import TypedDict
+from typing import TypedDict, Union
 
 import pandas as pd
 from pandas._libs.tslibs.parsing import DateParseError  # noqa
 
 from prep_flow.errors import (
     InvalidCategoryFoundError,
     InvalidDateFoundError,
@@ -19,15 +19,15 @@
 
 class RegexpCondition(TypedDict):
     regexp: str
     nullable: bool
 
 
 class CategoryCondition(TypedDict):
-    category: list[str]
+    category: list[Union[str, int]]
     nullable: bool
 
 
 class Validator:
     @staticmethod
     def validate_necessary_columns(data: pd.DataFrame, necessary_columns: list[str]) -> None:
         """
@@ -187,15 +187,14 @@
         InvalidCategoryFoundError
             If the specified category doesn't contain values.
         """
         for column, condition in conditions.items():
             for i, target in enumerate(data[column]):
                 if condition["nullable"] and pd.isna(target):
                     continue
-                casted_target = target if isinstance(target, str) or pd.isna(target) else str(int(target))
-                if casted_target not in condition["category"]:
+                if target not in condition["category"]:
                     raise InvalidCategoryFoundError(
                         column=column,
                         row_number=i + 1,
                         value=target,
                         category=condition["category"],
                     )
```

### Comparing `prep-flow-0.1.0/pyproject.toml` & `prep_flow-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -16,22 +16,23 @@
 ]
 dependencies = [
     "numpy>=1.20.3",
     "pandas>=1.2.4",
     "openpyxl>=3.0.0",
     "pydantic>=2.0.0",
 ]
-version = "0.1.0"
+version = "0.1.1"
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "flake8",
     "black",
     "isort",
+    "jupyter",
 ]
 
 [tool.setuptools.packages.find]
 exclude = ["build", "tests"]
 
 [tool.black]
 line-length = 119
```

### Comparing `prep-flow-0.1.0/tests/test_validator.py` & `prep_flow-0.1.1/tests/test_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,7 +185,17 @@
     assert e.value.row_number == 1
     assert pd.isna(e.value.value)
     assert e.value.category == ["man", "woman"]
 
     conditions_3_2 = {"gender": {"category": ["man", "woman"], "nullable": True}}
     Validator.validate_category(data_3, conditions_3_2)
     assert True
+
+    data_4 = pd.DataFrame(
+        {
+            "name": ["taro", "hanako"],
+            "gender": [0, 1],
+        }
+    )
+    conditions_4 = {"gender": {"category": [0, 1], "nullable": False}}
+    Validator.validate_category(data_4, conditions_4)
+    assert True
```

