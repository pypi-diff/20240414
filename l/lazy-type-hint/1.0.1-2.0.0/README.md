# Comparing `tmp/lazy_type_hint-1.0.1.tar.gz` & `tmp/lazy_type_hint-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_type_hint-1.0.1.tar", max compression
+gzip compressed data, was "lazy_type_hint-2.0.0.tar", max compression
```

## Comparing `lazy_type_hint-1.0.1.tar` & `lazy_type_hint-2.0.0.tar`

### file list

```diff
@@ -1,37 +1,39 @@
--rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-1.0.1/lazy_type_hint/__init__.py
--rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/__init__.py
--rw-r--r--   0        0        0     9844 2024-04-03 08:50:18.647695 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/data_type_tree.py
--rw-r--r--   0        0        0     4239 2024-04-03 08:50:18.647695 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/factory.py
--rw-r--r--   0        0        0      596 2024-04-03 08:50:18.648845 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/__init__.py
--rw-r--r--   0        0        0    16935 2024-04-03 15:48:14.628513 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
--rw-r--r--   0        0        0     4020 2024-04-03 08:50:18.649845 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
--rw-r--r--   0        0        0     1131 2024-04-03 08:50:18.650845 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
--rw-r--r--   0        0        0     4849 2024-04-03 15:48:14.634513 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
--rw-r--r--   0        0        0      225 2024-04-03 08:50:18.651845 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
--rw-r--r--   0        0        0      767 2024-04-03 08:50:18.652845 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
--rw-r--r--   0        0        0     6051 2024-04-03 08:50:18.652845 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
--rw-r--r--   0        0        0     1562 2024-04-03 08:50:18.652845 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
--rw-r--r--   0        0        0     2138 2024-04-03 08:50:18.653845 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
--rw-r--r--   0        0        0      562 2024-04-03 08:50:18.653845 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
--rw-r--r--   0        0        0     2446 2024-04-03 08:50:18.654846 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
--rw-r--r--   0        0        0      993 2024-04-03 08:50:18.654846 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
--rw-r--r--   0        0        0     1003 2024-04-03 08:50:18.655845 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
--rw-r--r--   0        0        0      752 2024-04-03 08:50:18.655845 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
--rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-1.0.1/lazy_type_hint/file_modifiers/__init__.py
--rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-1.0.1/lazy_type_hint/file_modifiers/py_file_modifier.py
--rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-1.0.1/lazy_type_hint/file_modifiers/yaml_file_modifier.py
--rw-r--r--   0        0        0     2380 2024-04-13 18:49:52.549938 lazy_type_hint-1.0.1/lazy_type_hint/generators/lazy_type_hint.py
--rw-r--r--   0        0        0     3149 2024-04-03 13:39:39.224765 lazy_type_hint-1.0.1/lazy_type_hint/generators/lazy_type_hint_abc.py
--rw-r--r--   0        0        0     9412 2024-04-03 15:48:14.649665 lazy_type_hint-1.0.1/lazy_type_hint/generators/lazy_type_hint_live.py
--rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-1.0.1/lazy_type_hint/py.typed
--rw-r--r--   0        0        0     1638 2024-04-03 08:50:18.659845 lazy_type_hint-1.0.1/lazy_type_hint/strategies.py
--rw-r--r--   0        0        0      706 2024-04-03 13:39:39.229769 lazy_type_hint-1.0.1/lazy_type_hint/utils/__init__.py
--rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-1.0.1/lazy_type_hint/utils/docstring_formatter.py
--rw-r--r--   0        0        0     4681 2024-04-03 08:50:18.660845 lazy_type_hint-1.0.1/lazy_type_hint/utils/import_manager.py
--rw-r--r--   0        0        0     4952 2024-04-03 08:50:18.661845 lazy_type_hint-1.0.1/lazy_type_hint/utils/mypy.py
--rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-1.0.1/lazy_type_hint/utils/ordered_set.py
--rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-1.0.1/lazy_type_hint/utils/test_ordered_set.py
--rw-r--r--   0        0        0     3770 2024-04-03 15:48:14.655819 lazy_type_hint-1.0.1/lazy_type_hint/utils/utils.py
--rw-r--r--   0        0        0     2362 2024-04-13 19:30:35.977434 lazy_type_hint-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6440 2024-04-13 19:31:38.569848 lazy_type_hint-1.0.1/README.md
--rw-r--r--   0        0        0     6832 1970-01-01 00:00:00.000000 lazy_type_hint-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-2.0.0/lazy_type_hint/__init__.py
+-rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/__init__.py
+-rw-r--r--   0        0        0     9883 2024-04-14 12:56:14.689752 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/data_type_tree.py
+-rw-r--r--   0        0        0     5377 2024-04-14 12:56:14.695752 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/factory.py
+-rw-r--r--   0        0        0      833 2024-04-14 12:56:14.700751 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/__init__.py
+-rw-r--r--   0        0        0    16935 2024-04-03 15:48:14.628513 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
+-rw-r--r--   0        0        0     4020 2024-04-03 08:50:18.649845 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
+-rw-r--r--   0        0        0     1131 2024-04-03 08:50:18.650845 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
+-rw-r--r--   0        0        0     4849 2024-04-14 10:52:55.353306 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
+-rw-r--r--   0        0        0      225 2024-04-03 08:50:18.651845 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
+-rw-r--r--   0        0        0     4822 2024-04-14 12:56:14.708824 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py
+-rw-r--r--   0        0        0      767 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
+-rw-r--r--   0        0        0     6051 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
+-rw-r--r--   0        0        0     1562 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
+-rw-r--r--   0        0        0     2138 2024-04-14 09:58:33.082160 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
+-rw-r--r--   0        0        0      798 2024-04-14 12:56:14.714038 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
+-rw-r--r--   0        0        0     2446 2024-04-03 08:50:18.654846 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
+-rw-r--r--   0        0        0      993 2024-04-03 08:50:18.654846 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
+-rw-r--r--   0        0        0      436 2024-04-14 12:56:14.719035 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/pandas_series_data_type_tree.py
+-rw-r--r--   0        0        0     1003 2024-04-14 10:39:38.880313 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
+-rw-r--r--   0        0        0      752 2024-04-03 08:50:18.655845 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
+-rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-2.0.0/lazy_type_hint/file_modifiers/__init__.py
+-rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-2.0.0/lazy_type_hint/file_modifiers/py_file_modifier.py
+-rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-2.0.0/lazy_type_hint/file_modifiers/yaml_file_modifier.py
+-rw-r--r--   0        0        0     2368 2024-04-14 12:56:14.724035 lazy_type_hint-2.0.0/lazy_type_hint/generators/lazy_type_hint.py
+-rw-r--r--   0        0        0     3149 2024-04-14 12:56:14.729212 lazy_type_hint-2.0.0/lazy_type_hint/generators/lazy_type_hint_abc.py
+-rw-r--r--   0        0        0     9412 2024-04-03 15:48:14.649665 lazy_type_hint-2.0.0/lazy_type_hint/generators/lazy_type_hint_live.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-2.0.0/lazy_type_hint/py.typed
+-rw-r--r--   0        0        0     1681 2024-04-14 12:56:14.734218 lazy_type_hint-2.0.0/lazy_type_hint/strategies.py
+-rw-r--r--   0        0        0      706 2024-04-03 13:39:39.229769 lazy_type_hint-2.0.0/lazy_type_hint/utils/__init__.py
+-rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-2.0.0/lazy_type_hint/utils/docstring_formatter.py
+-rw-r--r--   0        0        0     5458 2024-04-14 12:56:14.735213 lazy_type_hint-2.0.0/lazy_type_hint/utils/import_manager.py
+-rw-r--r--   0        0        0     5032 2024-04-14 12:56:14.741218 lazy_type_hint-2.0.0/lazy_type_hint/utils/mypy.py
+-rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.0/lazy_type_hint/utils/ordered_set.py
+-rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.0/lazy_type_hint/utils/test_ordered_set.py
+-rw-r--r--   0        0        0     3770 2024-04-03 15:48:14.655819 lazy_type_hint-2.0.0/lazy_type_hint/utils/utils.py
+-rw-r--r--   0        0        0     2397 2024-04-14 12:56:14.742212 lazy_type_hint-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6573 2024-04-14 12:56:14.682746 lazy_type_hint-2.0.0/README.md
+-rw-r--r--   0        0        0     6962 1970-01-01 00:00:00.000000 lazy_type_hint-2.0.0/PKG-INFO
```

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/data_type_tree.py` & `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/data_type_tree.py`

 * *Files 5% similar despite different names*

```diff
@@ -157,14 +157,15 @@
     @abstractmethod
     def _get_hash(self) -> Hashable:
         """Get a unique hash that identifies the current data type."""
 
     @final
     def __hash__(self) -> int:
         """Unique hash that identifies whether the current tree is considered to be unique."""
+        print(hash(self._get_hash()))
         return hash(self._get_hash())
 
     @abstractmethod
     def _get_str_top_node(self) -> str:
         """Get the type alias or the representation only for the current self.
 
         It does not include children.
```

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/factory.py` & `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/factory.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,117 +14,149 @@
         Optional,
         Sequence,
         Set,
         Tuple,
         Union,
     )
 
+    import pandas as pd
+
     from lazy_type_hint.data_type_tree.generic_type.dict_data_type_tree import DictDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.list_data_type_tree import ListDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.mapping_data_type_tree import MappingDataTypeTree
+    from lazy_type_hint.data_type_tree.generic_type.pandas_data_frame_data_type_tree import PandasDataFrameDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.sequence_data_type_tree import SequenceDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.set_data_type_tree import SetDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.tuple_data_type_tree import TupleDataTypeTree
     from lazy_type_hint.data_type_tree.simple_data_type_tree.simple_data_type_tree import SimpleDataTypeTree
+    from lazy_type_hint.data_type_tree.simple_data_type_tree.pandas_series_data_type_tree import (
+        PandasSeriesDataTypeTree,
+    )
     from lazy_type_hint.utils import ImportManager
 
 
 @overload
 def data_type_tree_factory(
+    data: "pd.Series",
+    name: str,
+    *,
+    imports: "Optional[ImportManager]" = None,
+    depth: int = 0,
+    strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
+    parent: "Optional[DataTypeTree]" = None,
+) -> "PandasSeriesDataTypeTree":
+    ...
+
+
+@overload
+def data_type_tree_factory(  # type: ignore[misc]
+    data: "pd.DataFrame",
+    name: str,
+    *,
+    imports: "Optional[ImportManager]" = None,
+    depth: int = 0,
+    strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
+    parent: "Optional[DataTypeTree]" = None,
+) -> "PandasDataFrameDataTypeTree":
+    ...
+
+
+@overload
+def data_type_tree_factory(  # type: ignore[misc]
     data: "List[Any]",
     name: str,
     *,
     imports: "Optional[ImportManager]" = None,
     depth: int = 0,
     strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
     parent: "Optional[DataTypeTree]" = None,
 ) -> "ListDataTypeTree":
     ...
 
 
 @overload
-def data_type_tree_factory(
+def data_type_tree_factory(  # type: ignore[misc]
     data: "Union[Set[Any], FrozenSet[Any]]",
     name: str,
     *,
     imports: "Optional[ImportManager]" = None,
     depth: int = 0,
     strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
     parent: "Optional[DataTypeTree]" = None,
 ) -> "SetDataTypeTree":
     ...
 
 
 @overload
-def data_type_tree_factory(
+def data_type_tree_factory(  # type: ignore[misc]
     data: "Union[bool, float, slice, None]",
     name: str,
     *,
     imports: "Optional[ImportManager]" = None,
     depth: int = 0,
     strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
     parent: "Optional[DataTypeTree]" = None,
 ) -> "SimpleDataTypeTree":
     ...
 
 
 @overload
-def data_type_tree_factory(
+def data_type_tree_factory(  # type: ignore[misc]
     data: "Tuple[Any, ...]",
     name: str,
     *,
     imports: "Optional[ImportManager]" = None,
     depth: int = 0,
     strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
     parent: "Optional[DataTypeTree]" = None,
 ) -> "TupleDataTypeTree":
     ...
 
 
 @overload
-def data_type_tree_factory(
+def data_type_tree_factory(  # type: ignore[misc]
     data: "Dict[Any, Any]",
     name: str,
     *,
     imports: "Optional[ImportManager]" = None,
     depth: int = 0,
     strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
     parent: "Optional[DataTypeTree]" = None,
 ) -> "DictDataTypeTree":
     ...
 
 
 @overload
-def data_type_tree_factory(
+def data_type_tree_factory(  # type: ignore[misc]
     data: "Sequence[Any]",
     name: str,
     *,
     imports: "Optional[ImportManager]" = None,
     depth: int = 0,
     strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
     parent: "Optional[DataTypeTree]" = None,
 ) -> "SequenceDataTypeTree":
     ...
 
 
 @overload
-def data_type_tree_factory(
+def data_type_tree_factory(  # type: ignore[misc]
     data: "Union[Mapping[Any, Any], MappingProxyType[Any, Any]]",
     name: str,
     *,
     imports: "Optional[ImportManager]" = None,
     depth: int = 0,
     strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
     parent: "Optional[DataTypeTree]" = None,
 ) -> "MappingDataTypeTree":
     ...
 
 
 @overload
-def data_type_tree_factory(
+def data_type_tree_factory(  # type: ignore[misc]
     data: object,
     name: str,
     *,
     imports: "Optional[ImportManager]" = None,
     depth: int = 0,
     strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
     parent: "Optional[DataTypeTree]" = None,
```

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py` & `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py` & `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py` & `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py` & `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py` & `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py` & `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py` & `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py` & `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py` & `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-from lazy_type_hint.data_type_tree.simple_data_type_tree.function_data_type_tree import (
-    FunctionDataTypeTree as FunctionDataTypeTree,
+from contextlib import suppress
+
+from lazy_type_hint.data_type_tree.generic_type.dict_data_type_tree import DictDataTypeTree as DictDataTypeTree
+from lazy_type_hint.data_type_tree.generic_type.list_data_type_tree import ListDataTypeTree as ListDataTypeTree
+from lazy_type_hint.data_type_tree.generic_type.mapping_data_type_tree import (
+    MappingDataTypeTree as MappingDataTypeTree,
 )
-from lazy_type_hint.data_type_tree.simple_data_type_tree.instance_data_type_tree import (
-    InstanceDataTypeTree as InstanceDataTypeTree,
-)
-from lazy_type_hint.data_type_tree.simple_data_type_tree.simple_data_type_tree import (
-    SimpleDataTypeTree as SimpleDataTypeTree,
-)
-from lazy_type_hint.data_type_tree.simple_data_type_tree.type_data_type_tree import (
-    TypeDataTypeTree as TypeDataTypeTree,
+
+with suppress(ImportError):
+    from lazy_type_hint.data_type_tree.generic_type.pandas_data_frame_data_type_tree import (
+        PandasDataFrameDataTypeTree as PandasDataFrameDataTypeTree,
+    )
+from lazy_type_hint.data_type_tree.generic_type.set_data_type_tree import SetDataTypeTree as SetDataTypeTree
+from lazy_type_hint.data_type_tree.generic_type.tuple_data_type_tree import (
+    TupleDataTypeTree as TupleDataTypeTree,
 )
```

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py` & `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py` & `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py` & `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py` & `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/file_modifiers/py_file_modifier.py` & `lazy_type_hint-2.0.0/lazy_type_hint/file_modifiers/py_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/file_modifiers/yaml_file_modifier.py` & `lazy_type_hint-2.0.0/lazy_type_hint/file_modifiers/yaml_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/generators/lazy_type_hint.py` & `lazy_type_hint-2.0.0/lazy_type_hint/generators/lazy_type_hint.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,36 +24,35 @@
 PathT = TypeVar("PathT", str, Path)
 
 
 @dataclass(frozen=True)
 class Tree:
     _tree: DataTypeTree
 
-    def as_string(self, *, include_imports: bool = True) -> str:
+    def to_string(self, *, include_imports: bool = True) -> str:
         return self._tree.get_str_all_nodes(include_imports=include_imports)
 
     def to_file(self, path_to_py: Union[Path, str], *, create_non_existing_dir: bool = False) -> None:
         path_to_py = Path(path_to_py)
         if not path_to_py.parent.exists():
             if not create_non_existing_dir:
                 raise ValueError(
                     "The given directory does not exist and permissions to create the folder "
                     "(create_non_existing_dir input argument) were not set"
                 )
             os.makedirs(path_to_py.parent)
-        path_to_py.write_text(self.as_string(include_imports=True))
+        path_to_py.write_text(self.to_string(include_imports=True))
 
 
 class LazyTypeHint(LazyTypeHintABC):
     strategies: ParsingStrategies
     """Strategies to follow when parsing the objects."""
 
     def __init__(
         self,
-        *,
         strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
         **kwargs: Any,
     ) -> None:
         self.strategies = strategies
 
     def from_yaml_file(
         self,
```

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/generators/lazy_type_hint_abc.py` & `lazy_type_hint-2.0.0/lazy_type_hint/generators/lazy_type_hint_abc.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,27 +25,27 @@
 PathT = TypeVar("PathT", str, Path)
 
 
 @dataclass(frozen=True)
 class Tree:
     _tree: DataTypeTree
 
-    def as_string(self, *, include_imports: bool = True) -> str:
+    def to_string(self, *, include_imports: bool = True) -> str:
         return self._tree.get_str_all_nodes(include_imports=include_imports)
 
     def to_file(self, path_to_py: Union[Path, str], *, create_non_existing_dir: bool = False) -> None:
         path_to_py = Path(path_to_py)
         if not path_to_py.exists():
             if not create_non_existing_dir:
                 raise ValueError(
                     "The given directory does not exist and permissions to create the folder "
                     "(create_non_existing_dir input argument) were not set"
                 )
             os.makedirs(path_to_py.parent)
-        path_to_py.write_text(self.as_string(include_imports=True))
+        path_to_py.write_text(self.to_string(include_imports=True))
 
 
 class LazyTypeHintABC(ABC):
     strategies: ParsingStrategies
     """Strategies to follow when parsing the objects."""
 
     def __init__(
```

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/generators/lazy_type_hint_live.py` & `lazy_type_hint-2.0.0/lazy_type_hint/generators/lazy_type_hint_live.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/strategies.py` & `lazy_type_hint-2.0.0/lazy_type_hint/strategies.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 
 @dataclass(frozen=True)
 class ParsingStrategies:
     list_strategy: LIST_STRATEGIES = "list"
     tuple_size_strategy: TUPLE_SIZE_STRATEGIES = "fixed"
     dict_strategy: MAPPING_STRATEGIES = "TypedDict"
+    pandas_type_hint_columns: bool = True
     min_height_to_define_type_alias: int = 1
     key_used_as_doc: str = ""
     merge_different_typed_dicts_if_similarity_above: int = 50
     typed_dict_read_only_values: bool = False
 
     def __post_init__(self) -> None:
         type_hints = get_type_hints(self)
```

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/utils/__init__.py` & `lazy_type_hint-2.0.0/lazy_type_hint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/utils/docstring_formatter.py` & `lazy_type_hint-2.0.0/lazy_type_hint/utils/docstring_formatter.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/utils/mypy.py` & `lazy_type_hint-2.0.0/lazy_type_hint/utils/mypy.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     Attributes:
         Result: A named tuple representing the result of running Mypy.
     """
 
     @staticmethod
     def is_available() -> bool:
-        return check_if_command_available("mypy")
+        return check_if_command_available("python3 -m poetry run mypy")
 
     class Result(NamedTuple):
         """Results returned by Mypy."""
 
         success: bool
         errors: List[str]
         scanned: Union[Path, str]
@@ -59,21 +59,22 @@
             python_version (str, optional): The Python version to use for type checking. Defaults to "3.8".
             ignore_errors (Iterable[str], optional): A collection of error keywords to ignore during type checking.
                 Defaults to ().
 
         Returns:
             Result: The result of the type checking, including success status, errors, and the scanned string.
         """
-        command = ["mypy"]
+        command = ["python3", "-m", "poetry", "run", "mypy"]
         if strict:
             command.append("--strict")
         command.append("--python-version")
         command.append(python_version)
         command.append("-c")
         command.append(string)
+        print(command)
         result = subprocess.run(command, capture_output=True)
         if result.stderr:
             return self.Result(success=False, errors=[str(result.stderr)], scanned=string)
         stdout = str(result.stdout)
         errors: List[str] = []
         lines = stdout.split("error: ")
         for error in lines:
```

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/utils/ordered_set.py` & `lazy_type_hint-2.0.0/lazy_type_hint/utils/ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/utils/test_ordered_set.py` & `lazy_type_hint-2.0.0/lazy_type_hint/utils/test_ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.1/lazy_type_hint/utils/utils.py` & `lazy_type_hint-2.0.0/lazy_type_hint/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.1/pyproject.toml` & `lazy_type_hint-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazy-type-hint"
-version = "1.0.1"
+version = "2.0.0"
 description = "Automate type hint generation in an easy way."
 authors = ["Manuel Floriano Vázquez <mflovaa@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.urls]
 Source = "https://github.com/mflova/lazy-type-hint"
 
@@ -19,14 +19,16 @@
 codespell = "2.2.6"  # Spell checker
 black = "23.12.1"  # Autoformatter
 pytest-clarity = "^1.0.1"
 pyyaml = "*"  # Used by the `check_code.py` script
 types-pyyaml = "*"
 filelock = "*"
 pytest_xdist = "*"  # Parallel execution tests
+pandas = "*"
+
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 # Config for developer tools
 [tool.black]
@@ -62,9 +64,10 @@
 "tests/**/test_func_data_type_tree.py" = ["ARG005", "ARG001"]
 "lazy_type_hint/**/lazy_type_hint*.py" = ["ARG002"]
 
 [tool.codespell]
 ignore-words-list = "bu"  # Comma separated
 
 [tool.pytest.ini_options]
+# addopts = "-vv"
 addopts = "-n auto"
 testpaths = ["tests"]
```

### Comparing `lazy_type_hint-1.0.1/README.md` & `lazy_type_hint-2.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # LazyTypeHint
 
-Type hint any built-in Python data structure!
+Type hint any Python (nested) data structure! Dictionaries, callables, Pandas DataFrames...
 
 ```
 pip install lazy-type-hint
 ```
 
 ## Main features
 
@@ -47,15 +47,15 @@
           LazyTypeHint(
               strategies=ParsingStrategies(
                   min_height_to_define_type_alias=2,
                   tuple_size_strategy="any size",
               )
           )
           .from_data(people, class_name="People")
-          .as_string()
+          .to_string()
       )
       print(people_type_hint)
    ```
 
    ```py
     # OUTPUT
     from typing import List, Tuple, TypedDict
@@ -131,15 +131,15 @@
 
 
     print(LazyTypeHint().from_yaml_file(
         loader=load_yaml_file,
         path="example.yaml",
         class_name="Sensors",
         comments_are=("above", "side"),
-    ).as_string())
+    ).to_string())
    ```
 
    Generate type hints like:
 
    ```py
    from typing import List, TypedDict
 
@@ -162,18 +162,20 @@
    class Sensors(TypedDict):
        sensors: SensorsSensors
        """Collection of sensors."""
    ```
 
 ## What makes it a different tool?
 
-There are some tools that aim to perform something similar.
-`Cattrs` or `pydantic` require knowing the structure beforehand. Then, the developer is responsible for writing it. They are
-validation-oriented. This tool is more geared towards providing better type hints in an automated way and
-ensuring that the structure is accessed correctly. Although other tools such as `Stubgen` are able to generate `.pyi` files in an automated way, it might be required to edit the environment to indicate where these stub-based files are located.
+There are some tools that aim to perform something similar. `Cattrs` or `pydantic` require
+knowing the structure beforehand. Then, the developer is responsible for writing it. They
+are validation-oriented. This tool is more geared towards providing better type hints in
+an automated way and ensuring that the structure is accessed correctly. Although other
+tools such as `Stubgen` are able to generate `.pyi` files in an automated way, it might be
+required to edit the environment to indicate where these stub-based files are located.
 
 ## All features
 
 Main features:
  - Type hint any (nested) structure.
  - Dictionaries can be type hinted as `TypedDict`, meaning that the IDE will have extra
    information about its underlying structures. Developer can therefore benefit from extra
@@ -195,10 +197,11 @@
    - Minimum percentage of similarity between dicts to be merged.
    - Mutable or read-only based `TypedDict`.
  
 Structures that can be type hinted:
  - Sequences: list, tuples
  - Sets: sets, frozensets
  - Dictionaries: dict, MappingProxyType
+ - Pandas DataFrame: Full support for string-based columns and `MultiIndex` columns
  - Simple built-in types: bool, int, float, range, slice, None, str
  - Callables: lambdas, functions, staticmethods, classmethods
  - Custom objects: instances and classes
```

### Comparing `lazy_type_hint-1.0.1/PKG-INFO` & `lazy_type_hint-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-type-hint
-Version: 1.0.1
+Version: 2.0.0
 Summary: Automate type hint generation in an easy way.
 Author: Manuel Floriano Vázquez
 Author-email: mflovaa@gmail.com
 Requires-Python: >=3.8,<=3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: typing_extensions
 Project-URL: Source, https://github.com/mflova/lazy-type-hint
 Description-Content-Type: text/markdown
 
 # LazyTypeHint
 
-Type hint any built-in Python data structure!
+Type hint any Python (nested) data structure! Dictionaries, callables, Pandas DataFrames...
 
 ```
 pip install lazy-type-hint
 ```
 
 ## Main features
 
@@ -63,15 +63,15 @@
           LazyTypeHint(
               strategies=ParsingStrategies(
                   min_height_to_define_type_alias=2,
                   tuple_size_strategy="any size",
               )
           )
           .from_data(people, class_name="People")
-          .as_string()
+          .to_string()
       )
       print(people_type_hint)
    ```
 
    ```py
     # OUTPUT
     from typing import List, Tuple, TypedDict
@@ -147,15 +147,15 @@
 
 
     print(LazyTypeHint().from_yaml_file(
         loader=load_yaml_file,
         path="example.yaml",
         class_name="Sensors",
         comments_are=("above", "side"),
-    ).as_string())
+    ).to_string())
    ```
 
    Generate type hints like:
 
    ```py
    from typing import List, TypedDict
 
@@ -178,18 +178,20 @@
    class Sensors(TypedDict):
        sensors: SensorsSensors
        """Collection of sensors."""
    ```
 
 ## What makes it a different tool?
 
-There are some tools that aim to perform something similar.
-`Cattrs` or `pydantic` require knowing the structure beforehand. Then, the developer is responsible for writing it. They are
-validation-oriented. This tool is more geared towards providing better type hints in an automated way and
-ensuring that the structure is accessed correctly. Although other tools such as `Stubgen` are able to generate `.pyi` files in an automated way, it might be required to edit the environment to indicate where these stub-based files are located.
+There are some tools that aim to perform something similar. `Cattrs` or `pydantic` require
+knowing the structure beforehand. Then, the developer is responsible for writing it. They
+are validation-oriented. This tool is more geared towards providing better type hints in
+an automated way and ensuring that the structure is accessed correctly. Although other
+tools such as `Stubgen` are able to generate `.pyi` files in an automated way, it might be
+required to edit the environment to indicate where these stub-based files are located.
 
 ## All features
 
 Main features:
  - Type hint any (nested) structure.
  - Dictionaries can be type hinted as `TypedDict`, meaning that the IDE will have extra
    information about its underlying structures. Developer can therefore benefit from extra
@@ -211,10 +213,11 @@
    - Minimum percentage of similarity between dicts to be merged.
    - Mutable or read-only based `TypedDict`.
  
 Structures that can be type hinted:
  - Sequences: list, tuples
  - Sets: sets, frozensets
  - Dictionaries: dict, MappingProxyType
+ - Pandas DataFrame: Full support for string-based columns and `MultiIndex` columns
  - Simple built-in types: bool, int, float, range, slice, None, str
  - Callables: lambdas, functions, staticmethods, classmethods
  - Custom objects: instances and classes
```

