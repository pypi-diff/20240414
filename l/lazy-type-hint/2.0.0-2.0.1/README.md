# Comparing `tmp/lazy_type_hint-2.0.0.tar.gz` & `tmp/lazy_type_hint-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_type_hint-2.0.0.tar", max compression
+gzip compressed data, was "lazy_type_hint-2.0.1.tar", max compression
```

## Comparing `lazy_type_hint-2.0.0.tar` & `lazy_type_hint-2.0.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-2.0.0/lazy_type_hint/__init__.py
--rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/__init__.py
--rw-r--r--   0        0        0     9883 2024-04-14 12:56:14.689752 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/data_type_tree.py
--rw-r--r--   0        0        0     5377 2024-04-14 12:56:14.695752 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/factory.py
--rw-r--r--   0        0        0      833 2024-04-14 12:56:14.700751 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/__init__.py
--rw-r--r--   0        0        0    16935 2024-04-03 15:48:14.628513 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
--rw-r--r--   0        0        0     4020 2024-04-03 08:50:18.649845 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
--rw-r--r--   0        0        0     1131 2024-04-03 08:50:18.650845 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
--rw-r--r--   0        0        0     4849 2024-04-14 10:52:55.353306 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
--rw-r--r--   0        0        0      225 2024-04-03 08:50:18.651845 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
--rw-r--r--   0        0        0     4822 2024-04-14 12:56:14.708824 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py
--rw-r--r--   0        0        0      767 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
--rw-r--r--   0        0        0     6051 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
--rw-r--r--   0        0        0     1562 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
--rw-r--r--   0        0        0     2138 2024-04-14 09:58:33.082160 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
--rw-r--r--   0        0        0      798 2024-04-14 12:56:14.714038 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
--rw-r--r--   0        0        0     2446 2024-04-03 08:50:18.654846 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
--rw-r--r--   0        0        0      993 2024-04-03 08:50:18.654846 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
--rw-r--r--   0        0        0      436 2024-04-14 12:56:14.719035 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/pandas_series_data_type_tree.py
--rw-r--r--   0        0        0     1003 2024-04-14 10:39:38.880313 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
--rw-r--r--   0        0        0      752 2024-04-03 08:50:18.655845 lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
--rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-2.0.0/lazy_type_hint/file_modifiers/__init__.py
--rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-2.0.0/lazy_type_hint/file_modifiers/py_file_modifier.py
--rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-2.0.0/lazy_type_hint/file_modifiers/yaml_file_modifier.py
--rw-r--r--   0        0        0     2368 2024-04-14 12:56:14.724035 lazy_type_hint-2.0.0/lazy_type_hint/generators/lazy_type_hint.py
--rw-r--r--   0        0        0     3149 2024-04-14 12:56:14.729212 lazy_type_hint-2.0.0/lazy_type_hint/generators/lazy_type_hint_abc.py
--rw-r--r--   0        0        0     9412 2024-04-03 15:48:14.649665 lazy_type_hint-2.0.0/lazy_type_hint/generators/lazy_type_hint_live.py
--rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-2.0.0/lazy_type_hint/py.typed
--rw-r--r--   0        0        0     1681 2024-04-14 12:56:14.734218 lazy_type_hint-2.0.0/lazy_type_hint/strategies.py
--rw-r--r--   0        0        0      706 2024-04-03 13:39:39.229769 lazy_type_hint-2.0.0/lazy_type_hint/utils/__init__.py
--rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-2.0.0/lazy_type_hint/utils/docstring_formatter.py
--rw-r--r--   0        0        0     5458 2024-04-14 12:56:14.735213 lazy_type_hint-2.0.0/lazy_type_hint/utils/import_manager.py
--rw-r--r--   0        0        0     5032 2024-04-14 12:56:14.741218 lazy_type_hint-2.0.0/lazy_type_hint/utils/mypy.py
--rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.0/lazy_type_hint/utils/ordered_set.py
--rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.0/lazy_type_hint/utils/test_ordered_set.py
--rw-r--r--   0        0        0     3770 2024-04-03 15:48:14.655819 lazy_type_hint-2.0.0/lazy_type_hint/utils/utils.py
--rw-r--r--   0        0        0     2397 2024-04-14 12:56:14.742212 lazy_type_hint-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     6573 2024-04-14 12:56:14.682746 lazy_type_hint-2.0.0/README.md
--rw-r--r--   0        0        0     6962 1970-01-01 00:00:00.000000 lazy_type_hint-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-2.0.1/lazy_type_hint/__init__.py
+-rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/__init__.py
+-rw-r--r--   0        0        0     9844 2024-04-14 13:10:15.517147 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/data_type_tree.py
+-rw-r--r--   0        0        0     5377 2024-04-14 12:56:14.695752 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/factory.py
+-rw-r--r--   0        0        0      833 2024-04-14 12:56:14.700751 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/__init__.py
+-rw-r--r--   0        0        0    16935 2024-04-03 15:48:14.628513 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
+-rw-r--r--   0        0        0     4020 2024-04-03 08:50:18.649845 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
+-rw-r--r--   0        0        0     1131 2024-04-03 08:50:18.650845 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
+-rw-r--r--   0        0        0     4849 2024-04-14 10:52:55.353306 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
+-rw-r--r--   0        0        0      225 2024-04-03 08:50:18.651845 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
+-rw-r--r--   0        0        0     4822 2024-04-14 12:56:14.708824 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py
+-rw-r--r--   0        0        0      767 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
+-rw-r--r--   0        0        0     6051 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
+-rw-r--r--   0        0        0     1562 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
+-rw-r--r--   0        0        0     2138 2024-04-14 09:58:33.082160 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
+-rw-r--r--   0        0        0      798 2024-04-14 12:56:14.714038 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
+-rw-r--r--   0        0        0     2446 2024-04-03 08:50:18.654846 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
+-rw-r--r--   0        0        0      993 2024-04-03 08:50:18.654846 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
+-rw-r--r--   0        0        0      436 2024-04-14 12:56:14.719035 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/pandas_series_data_type_tree.py
+-rw-r--r--   0        0        0     1003 2024-04-14 10:39:38.880313 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
+-rw-r--r--   0        0        0      752 2024-04-03 08:50:18.655845 lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
+-rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-2.0.1/lazy_type_hint/file_modifiers/__init__.py
+-rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-2.0.1/lazy_type_hint/file_modifiers/py_file_modifier.py
+-rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-2.0.1/lazy_type_hint/file_modifiers/yaml_file_modifier.py
+-rw-r--r--   0        0        0     2368 2024-04-14 12:56:14.724035 lazy_type_hint-2.0.1/lazy_type_hint/generators/lazy_type_hint.py
+-rw-r--r--   0        0        0     3149 2024-04-14 12:56:14.729212 lazy_type_hint-2.0.1/lazy_type_hint/generators/lazy_type_hint_abc.py
+-rw-r--r--   0        0        0     9412 2024-04-03 15:48:14.649665 lazy_type_hint-2.0.1/lazy_type_hint/generators/lazy_type_hint_live.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-2.0.1/lazy_type_hint/py.typed
+-rw-r--r--   0        0        0     1681 2024-04-14 12:56:14.734218 lazy_type_hint-2.0.1/lazy_type_hint/strategies.py
+-rw-r--r--   0        0        0      706 2024-04-03 13:39:39.229769 lazy_type_hint-2.0.1/lazy_type_hint/utils/__init__.py
+-rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-2.0.1/lazy_type_hint/utils/docstring_formatter.py
+-rw-r--r--   0        0        0     5458 2024-04-14 12:56:14.735213 lazy_type_hint-2.0.1/lazy_type_hint/utils/import_manager.py
+-rw-r--r--   0        0        0     5008 2024-04-14 13:10:20.018341 lazy_type_hint-2.0.1/lazy_type_hint/utils/mypy.py
+-rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.1/lazy_type_hint/utils/ordered_set.py
+-rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.1/lazy_type_hint/utils/test_ordered_set.py
+-rw-r--r--   0        0        0     3770 2024-04-03 15:48:14.655819 lazy_type_hint-2.0.1/lazy_type_hint/utils/utils.py
+-rw-r--r--   0        0        0     2397 2024-04-14 13:10:41.011512 lazy_type_hint-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6573 2024-04-14 12:56:14.682746 lazy_type_hint-2.0.1/README.md
+-rw-r--r--   0        0        0     6962 1970-01-01 00:00:00.000000 lazy_type_hint-2.0.1/PKG-INFO
```

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/data_type_tree.py` & `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/data_type_tree.py`

 * *Files 5% similar despite different names*

```diff
@@ -157,15 +157,14 @@
     @abstractmethod
     def _get_hash(self) -> Hashable:
         """Get a unique hash that identifies the current data type."""
 
     @final
     def __hash__(self) -> int:
         """Unique hash that identifies whether the current tree is considered to be unique."""
-        print(hash(self._get_hash()))
         return hash(self._get_hash())
 
     @abstractmethod
     def _get_str_top_node(self) -> str:
         """Get the type alias or the representation only for the current self.
 
         It does not include children.
```

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/factory.py` & `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/factory.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/__init__.py` & `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py` & `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py` & `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py` & `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py` & `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py` & `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py` & `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py` & `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py` & `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py` & `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py` & `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py` & `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py` & `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py` & `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py` & `lazy_type_hint-2.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/file_modifiers/py_file_modifier.py` & `lazy_type_hint-2.0.1/lazy_type_hint/file_modifiers/py_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/file_modifiers/yaml_file_modifier.py` & `lazy_type_hint-2.0.1/lazy_type_hint/file_modifiers/yaml_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/generators/lazy_type_hint.py` & `lazy_type_hint-2.0.1/lazy_type_hint/generators/lazy_type_hint.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/generators/lazy_type_hint_abc.py` & `lazy_type_hint-2.0.1/lazy_type_hint/generators/lazy_type_hint_abc.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/generators/lazy_type_hint_live.py` & `lazy_type_hint-2.0.1/lazy_type_hint/generators/lazy_type_hint_live.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/strategies.py` & `lazy_type_hint-2.0.1/lazy_type_hint/strategies.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/utils/__init__.py` & `lazy_type_hint-2.0.1/lazy_type_hint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/utils/docstring_formatter.py` & `lazy_type_hint-2.0.1/lazy_type_hint/utils/docstring_formatter.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/utils/import_manager.py` & `lazy_type_hint-2.0.1/lazy_type_hint/utils/import_manager.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/utils/mypy.py` & `lazy_type_hint-2.0.1/lazy_type_hint/utils/mypy.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,14 @@
         command = ["python3", "-m", "poetry", "run", "mypy"]
         if strict:
             command.append("--strict")
         command.append("--python-version")
         command.append(python_version)
         command.append("-c")
         command.append(string)
-        print(command)
         result = subprocess.run(command, capture_output=True)
         if result.stderr:
             return self.Result(success=False, errors=[str(result.stderr)], scanned=string)
         stdout = str(result.stdout)
         errors: List[str] = []
         lines = stdout.split("error: ")
         for error in lines:
```

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/utils/ordered_set.py` & `lazy_type_hint-2.0.1/lazy_type_hint/utils/ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/utils/test_ordered_set.py` & `lazy_type_hint-2.0.1/lazy_type_hint/utils/test_ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/lazy_type_hint/utils/utils.py` & `lazy_type_hint-2.0.1/lazy_type_hint/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/pyproject.toml` & `lazy_type_hint-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazy-type-hint"
-version = "2.0.0"
+version = "2.0.1"
 description = "Automate type hint generation in an easy way."
 authors = ["Manuel Floriano Vázquez <mflovaa@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.urls]
 Source = "https://github.com/mflova/lazy-type-hint"
```

### Comparing `lazy_type_hint-2.0.0/README.md` & `lazy_type_hint-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.0/PKG-INFO` & `lazy_type_hint-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-type-hint
-Version: 2.0.0
+Version: 2.0.1
 Summary: Automate type hint generation in an easy way.
 Author: Manuel Floriano Vázquez
 Author-email: mflovaa@gmail.com
 Requires-Python: >=3.8,<=3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

