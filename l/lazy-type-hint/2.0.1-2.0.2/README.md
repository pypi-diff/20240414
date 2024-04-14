# Comparing `tmp/lazy_type_hint-2.0.1.tar.gz` & `tmp/lazy_type_hint-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_type_hint-2.0.1.tar", max compression
+gzip compressed data, was "lazy_type_hint-2.0.2.tar", max compression
```

## Comparing `lazy_type_hint-2.0.1.tar` & `lazy_type_hint-2.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-2.0.1/lazy_type_hint/__init__.py
--rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/__init__.py
--rw-r--r--   0        0        0     9844 2024-04-14 13:10:15.517147 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/data_type_tree.py
--rw-r--r--   0        0        0     5377 2024-04-14 12:56:14.695752 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/factory.py
--rw-r--r--   0        0        0      833 2024-04-14 12:56:14.700751 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/__init__.py
--rw-r--r--   0        0        0    16935 2024-04-03 15:48:14.628513 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
--rw-r--r--   0        0        0     4020 2024-04-03 08:50:18.649845 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
--rw-r--r--   0        0        0     1131 2024-04-03 08:50:18.650845 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
--rw-r--r--   0        0        0     4849 2024-04-14 10:52:55.353306 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
--rw-r--r--   0        0        0      225 2024-04-03 08:50:18.651845 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
--rw-r--r--   0        0        0     4822 2024-04-14 12:56:14.708824 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py
--rw-r--r--   0        0        0      767 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
--rw-r--r--   0        0        0     6051 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
--rw-r--r--   0        0        0     1562 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
--rw-r--r--   0        0        0     2138 2024-04-14 09:58:33.082160 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
--rw-r--r--   0        0        0      798 2024-04-14 12:56:14.714038 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
--rw-r--r--   0        0        0     2446 2024-04-03 08:50:18.654846 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
--rw-r--r--   0        0        0      993 2024-04-03 08:50:18.654846 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
--rw-r--r--   0        0        0      436 2024-04-14 12:56:14.719035 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/pandas_series_data_type_tree.py
--rw-r--r--   0        0        0     1003 2024-04-14 10:39:38.880313 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
--rw-r--r--   0        0        0      752 2024-04-03 08:50:18.655845 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
--rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-2.0.1/lazy_type_hint/file_modifiers/__init__.py
--rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-2.0.1/lazy_type_hint/file_modifiers/py_file_modifier.py
--rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-2.0.1/lazy_type_hint/file_modifiers/yaml_file_modifier.py
--rw-r--r--   0        0        0     2368 2024-04-14 12:56:14.724035 lazy_type_hint-2.0.1/lazy_type_hint/generators/lazy_type_hint.py
--rw-r--r--   0        0        0     3149 2024-04-14 12:56:14.729212 lazy_type_hint-2.0.1/lazy_type_hint/generators/lazy_type_hint_abc.py
--rw-r--r--   0        0        0     9412 2024-04-03 15:48:14.649665 lazy_type_hint-2.0.1/lazy_type_hint/generators/lazy_type_hint_live.py
--rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-2.0.1/lazy_type_hint/py.typed
--rw-r--r--   0        0        0     1681 2024-04-14 12:56:14.734218 lazy_type_hint-2.0.1/lazy_type_hint/strategies.py
--rw-r--r--   0        0        0      706 2024-04-03 13:39:39.229769 lazy_type_hint-2.0.1/lazy_type_hint/utils/__init__.py
--rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-2.0.1/lazy_type_hint/utils/docstring_formatter.py
--rw-r--r--   0        0        0     5458 2024-04-14 12:56:14.735213 lazy_type_hint-2.0.1/lazy_type_hint/utils/import_manager.py
--rw-r--r--   0        0        0     5008 2024-04-14 13:10:20.018341 lazy_type_hint-2.0.1/lazy_type_hint/utils/mypy.py
--rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.1/lazy_type_hint/utils/ordered_set.py
--rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.1/lazy_type_hint/utils/test_ordered_set.py
--rw-r--r--   0        0        0     3770 2024-04-03 15:48:14.655819 lazy_type_hint-2.0.1/lazy_type_hint/utils/utils.py
--rw-r--r--   0        0        0     2397 2024-04-14 13:10:41.011512 lazy_type_hint-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     6573 2024-04-14 12:56:14.682746 lazy_type_hint-2.0.1/README.md
--rw-r--r--   0        0        0     6962 1970-01-01 00:00:00.000000 lazy_type_hint-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-2.0.2/lazy_type_hint/__init__.py
+-rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/__init__.py
+-rw-r--r--   0        0        0     9844 2024-04-14 13:10:15.517147 lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/data_type_tree.py
+-rw-r--r--   0        0        0     5377 2024-04-14 12:56:14.695752 lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/factory.py
+-rw-r--r--   0        0        0      833 2024-04-14 12:56:14.700751 lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/generic_type/__init__.py
+-rw-r--r--   0        0        0    16935 2024-04-03 15:48:14.628513 lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
+-rw-r--r--   0        0        0     4020 2024-04-03 08:50:18.649845 lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
+-rw-r--r--   0        0        0     1131 2024-04-03 08:50:18.650845 lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
+-rw-r--r--   0        0        0     4849 2024-04-14 10:52:55.353306 lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
+-rw-r--r--   0        0        0      225 2024-04-03 08:50:18.651845 lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
+-rw-r--r--   0        0        0     4415 2024-04-14 14:12:29.200950 lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py
+-rw-r--r--   0        0        0      767 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
+-rw-r--r--   0        0        0     6051 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
+-rw-r--r--   0        0        0     1562 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
+-rw-r--r--   0        0        0     2138 2024-04-14 09:58:33.082160 lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
+-rw-r--r--   0        0        0      798 2024-04-14 12:56:14.714038 lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
+-rw-r--r--   0        0        0     2446 2024-04-03 08:50:18.654846 lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
+-rw-r--r--   0        0        0      993 2024-04-03 08:50:18.654846 lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
+-rw-r--r--   0        0        0      436 2024-04-14 12:56:14.719035 lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/simple_data_type_tree/pandas_series_data_type_tree.py
+-rw-r--r--   0        0        0     1003 2024-04-14 10:39:38.880313 lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
+-rw-r--r--   0        0        0      752 2024-04-03 08:50:18.655845 lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
+-rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-2.0.2/lazy_type_hint/file_modifiers/__init__.py
+-rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-2.0.2/lazy_type_hint/file_modifiers/py_file_modifier.py
+-rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-2.0.2/lazy_type_hint/file_modifiers/yaml_file_modifier.py
+-rw-r--r--   0        0        0     2368 2024-04-14 12:56:14.724035 lazy_type_hint-2.0.2/lazy_type_hint/generators/lazy_type_hint.py
+-rw-r--r--   0        0        0     3149 2024-04-14 12:56:14.729212 lazy_type_hint-2.0.2/lazy_type_hint/generators/lazy_type_hint_abc.py
+-rw-r--r--   0        0        0     9412 2024-04-03 15:48:14.649665 lazy_type_hint-2.0.2/lazy_type_hint/generators/lazy_type_hint_live.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-2.0.2/lazy_type_hint/py.typed
+-rw-r--r--   0        0        0     1681 2024-04-14 12:56:14.734218 lazy_type_hint-2.0.2/lazy_type_hint/strategies.py
+-rw-r--r--   0        0        0      706 2024-04-03 13:39:39.229769 lazy_type_hint-2.0.2/lazy_type_hint/utils/__init__.py
+-rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-2.0.2/lazy_type_hint/utils/docstring_formatter.py
+-rw-r--r--   0        0        0     5458 2024-04-14 12:56:14.735213 lazy_type_hint-2.0.2/lazy_type_hint/utils/import_manager.py
+-rw-r--r--   0        0        0     5008 2024-04-14 13:10:20.018341 lazy_type_hint-2.0.2/lazy_type_hint/utils/mypy.py
+-rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.2/lazy_type_hint/utils/ordered_set.py
+-rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.2/lazy_type_hint/utils/test_ordered_set.py
+-rw-r--r--   0        0        0     3770 2024-04-03 15:48:14.655819 lazy_type_hint-2.0.2/lazy_type_hint/utils/utils.py
+-rw-r--r--   0        0        0     2397 2024-04-14 14:12:37.040458 lazy_type_hint-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6573 2024-04-14 12:56:14.682746 lazy_type_hint-2.0.2/README.md
+-rw-r--r--   0        0        0     6962 1970-01-01 00:00:00.000000 lazy_type_hint-2.0.2/PKG-INFO
```

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/data_type_tree.py` & `lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/factory.py` & `lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/factory.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/__init__.py` & `lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/generic_type/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py` & `lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py` & `lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py` & `lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py` & `lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py` & `lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import (
     Dict,
     Final,
     List,
     Mapping,
+    Set,
     Type,
 )
 
 import pandas as pd
 from typing_extensions import override
 
 from lazy_type_hint.data_type_tree import data_type_tree_factory
@@ -77,27 +78,26 @@
         children: Dict[str, DataTypeTree] = {}
         if not self.are_columns_either_all_str_or_all_tuple:
             return children
         for column in self.data.columns:
             if not self.can_be_accessed_multilevel:  # Here all columns will  be str
                 children[column] = self._create_child(column)
             else:  # Here all columns will be tuple
+                columns_processed: Set[str] = set()
                 for column in self.data.columns:
-                    children[column[0]] = self._create_child(column[0])
+                    if column[0] not in columns_processed:
+                        columns_processed.add(column[0])
+                        children[column[0]] = self._create_child(column[0])
         return children
 
     @override
     def _get_hash(self) -> str:
         if not self.strategies.pandas_type_hint_columns:
             return "pd.DataFrame"
-        if self.all_columns_are(str):
-            return str(self.data.columns)
-        if self.all_columns_are(tuple):
-            return str(column[0] for column in self.data.columns)
-        return "pd.DataFrame"
+        return str(self.data.columns)
 
     @override
     def _get_str_top_node(self) -> str:
         self.imports.add("pandas")
         if len(self) == 0 or not self.strategies.pandas_type_hint_columns:
             self.imports.add("TypeAlias")
             return f"{self.name}: TypeAlias = pd.DataFrame"
@@ -108,20 +108,14 @@
         self.imports.add("tuple")
         self.imports.add("list")
         self.imports.add("Hashable")
         self.imports.add("numpy")
         self.imports.add("pd.Scalar")
 
         overloads: List[str] = []
-        for literal, child in zip(self.data.columns, self):
+        for literal, child in self.children.items():
             if child.permission_to_be_created_as_type_alias:
-                if self.all_columns_are(str):
-                    overloads.append(OVERLOAD_TEMPLATE.format(literal=literal, rtype=child.name))
-                elif self.all_columns_are(tuple):
-                    overloads.append(OVERLOAD_TEMPLATE.format(literal=literal[0], rtype=child.name))
+                overloads.append(OVERLOAD_TEMPLATE.format(literal=literal, rtype=child.name))
             else:
                 rtype = "Union[pd.DataFrame, pd.Series]"
-                if self.all_columns_are(str):
-                    overloads.append(OVERLOAD_TEMPLATE.format(literal=literal, rtype=rtype))
-                elif self.all_columns_are(tuple):
-                    overloads.append(OVERLOAD_TEMPLATE.format(literal=literal[0], rtype=rtype))
+                overloads.append(OVERLOAD_TEMPLATE.format(literal=literal, rtype=rtype))
         return TEMPLATE.format(class_name=self.name, overloads="\n".join(overloads))
```

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py` & `lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py` & `lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py` & `lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py` & `lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py` & `lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py` & `lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py` & `lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py` & `lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py` & `lazy_type_hint-2.0.2/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/file_modifiers/py_file_modifier.py` & `lazy_type_hint-2.0.2/lazy_type_hint/file_modifiers/py_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/file_modifiers/yaml_file_modifier.py` & `lazy_type_hint-2.0.2/lazy_type_hint/file_modifiers/yaml_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/generators/lazy_type_hint.py` & `lazy_type_hint-2.0.2/lazy_type_hint/generators/lazy_type_hint.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/generators/lazy_type_hint_abc.py` & `lazy_type_hint-2.0.2/lazy_type_hint/generators/lazy_type_hint_abc.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/generators/lazy_type_hint_live.py` & `lazy_type_hint-2.0.2/lazy_type_hint/generators/lazy_type_hint_live.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/strategies.py` & `lazy_type_hint-2.0.2/lazy_type_hint/strategies.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/utils/__init__.py` & `lazy_type_hint-2.0.2/lazy_type_hint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/utils/docstring_formatter.py` & `lazy_type_hint-2.0.2/lazy_type_hint/utils/docstring_formatter.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/utils/import_manager.py` & `lazy_type_hint-2.0.2/lazy_type_hint/utils/import_manager.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/utils/mypy.py` & `lazy_type_hint-2.0.2/lazy_type_hint/utils/mypy.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/utils/ordered_set.py` & `lazy_type_hint-2.0.2/lazy_type_hint/utils/ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/utils/test_ordered_set.py` & `lazy_type_hint-2.0.2/lazy_type_hint/utils/test_ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/lazy_type_hint/utils/utils.py` & `lazy_type_hint-2.0.2/lazy_type_hint/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/pyproject.toml` & `lazy_type_hint-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazy-type-hint"
-version = "2.0.1"
+version = "2.0.2"
 description = "Automate type hint generation in an easy way."
 authors = ["Manuel Floriano Vázquez <mflovaa@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.urls]
 Source = "https://github.com/mflova/lazy-type-hint"
```

### Comparing `lazy_type_hint-2.0.1/README.md` & `lazy_type_hint-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.1/PKG-INFO` & `lazy_type_hint-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-type-hint
-Version: 2.0.1
+Version: 2.0.2
 Summary: Automate type hint generation in an easy way.
 Author: Manuel Floriano Vázquez
 Author-email: mflovaa@gmail.com
 Requires-Python: >=3.8,<=3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

