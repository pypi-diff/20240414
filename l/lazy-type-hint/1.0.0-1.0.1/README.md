# Comparing `tmp/lazy_type_hint-1.0.0.tar.gz` & `tmp/lazy_type_hint-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_type_hint-1.0.0.tar", max compression
+gzip compressed data, was "lazy_type_hint-1.0.1.tar", max compression
```

## Comparing `lazy_type_hint-1.0.0.tar` & `lazy_type_hint-1.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-1.0.0/lazy_type_hint/__init__.py
--rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/__init__.py
--rw-r--r--   0        0        0     9844 2024-04-03 08:50:18.647695 lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/data_type_tree.py
--rw-r--r--   0        0        0     4239 2024-04-03 08:50:18.647695 lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/factory.py
--rw-r--r--   0        0        0      596 2024-04-03 08:50:18.648845 lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/generic_type/__init__.py
--rw-r--r--   0        0        0    16935 2024-04-03 15:48:14.628513 lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
--rw-r--r--   0        0        0     4020 2024-04-03 08:50:18.649845 lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
--rw-r--r--   0        0        0     1131 2024-04-03 08:50:18.650845 lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
--rw-r--r--   0        0        0     4849 2024-04-03 15:48:14.634513 lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
--rw-r--r--   0        0        0      225 2024-04-03 08:50:18.651845 lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
--rw-r--r--   0        0        0      767 2024-04-03 08:50:18.652845 lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
--rw-r--r--   0        0        0     6051 2024-04-03 08:50:18.652845 lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
--rw-r--r--   0        0        0     1562 2024-04-03 08:50:18.652845 lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
--rw-r--r--   0        0        0     2138 2024-04-03 08:50:18.653845 lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
--rw-r--r--   0        0        0      562 2024-04-03 08:50:18.653845 lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
--rw-r--r--   0        0        0     2446 2024-04-03 08:50:18.654846 lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
--rw-r--r--   0        0        0      993 2024-04-03 08:50:18.654846 lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
--rw-r--r--   0        0        0     1003 2024-04-03 08:50:18.655845 lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
--rw-r--r--   0        0        0      752 2024-04-03 08:50:18.655845 lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
--rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-1.0.0/lazy_type_hint/file_modifiers/__init__.py
--rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-1.0.0/lazy_type_hint/file_modifiers/py_file_modifier.py
--rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-1.0.0/lazy_type_hint/file_modifiers/yaml_file_modifier.py
--rw-r--r--   0        0        0     2380 2024-04-13 18:49:52.549938 lazy_type_hint-1.0.0/lazy_type_hint/generators/lazy_type_hint.py
--rw-r--r--   0        0        0     3149 2024-04-03 13:39:39.224765 lazy_type_hint-1.0.0/lazy_type_hint/generators/lazy_type_hint_abc.py
--rw-r--r--   0        0        0     9412 2024-04-03 15:48:14.649665 lazy_type_hint-1.0.0/lazy_type_hint/generators/lazy_type_hint_live.py
--rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-1.0.0/lazy_type_hint/py.typed
--rw-r--r--   0        0        0     1638 2024-04-03 08:50:18.659845 lazy_type_hint-1.0.0/lazy_type_hint/strategies.py
--rw-r--r--   0        0        0      706 2024-04-03 13:39:39.229769 lazy_type_hint-1.0.0/lazy_type_hint/utils/__init__.py
--rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-1.0.0/lazy_type_hint/utils/docstring_formatter.py
--rw-r--r--   0        0        0     4681 2024-04-03 08:50:18.660845 lazy_type_hint-1.0.0/lazy_type_hint/utils/import_manager.py
--rw-r--r--   0        0        0     4952 2024-04-03 08:50:18.661845 lazy_type_hint-1.0.0/lazy_type_hint/utils/mypy.py
--rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-1.0.0/lazy_type_hint/utils/ordered_set.py
--rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-1.0.0/lazy_type_hint/utils/test_ordered_set.py
--rw-r--r--   0        0        0     3770 2024-04-03 15:48:14.655819 lazy_type_hint-1.0.0/lazy_type_hint/utils/utils.py
--rw-r--r--   0        0        0     2317 2024-04-13 19:21:57.993559 lazy_type_hint-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6431 2024-04-13 19:19:02.648766 lazy_type_hint-1.0.0/README.md
--rw-r--r--   0        0        0     6778 1970-01-01 00:00:00.000000 lazy_type_hint-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-1.0.1/lazy_type_hint/__init__.py
+-rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/__init__.py
+-rw-r--r--   0        0        0     9844 2024-04-03 08:50:18.647695 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/data_type_tree.py
+-rw-r--r--   0        0        0     4239 2024-04-03 08:50:18.647695 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/factory.py
+-rw-r--r--   0        0        0      596 2024-04-03 08:50:18.648845 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/__init__.py
+-rw-r--r--   0        0        0    16935 2024-04-03 15:48:14.628513 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
+-rw-r--r--   0        0        0     4020 2024-04-03 08:50:18.649845 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
+-rw-r--r--   0        0        0     1131 2024-04-03 08:50:18.650845 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
+-rw-r--r--   0        0        0     4849 2024-04-03 15:48:14.634513 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
+-rw-r--r--   0        0        0      225 2024-04-03 08:50:18.651845 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
+-rw-r--r--   0        0        0      767 2024-04-03 08:50:18.652845 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
+-rw-r--r--   0        0        0     6051 2024-04-03 08:50:18.652845 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
+-rw-r--r--   0        0        0     1562 2024-04-03 08:50:18.652845 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
+-rw-r--r--   0        0        0     2138 2024-04-03 08:50:18.653845 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
+-rw-r--r--   0        0        0      562 2024-04-03 08:50:18.653845 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
+-rw-r--r--   0        0        0     2446 2024-04-03 08:50:18.654846 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
+-rw-r--r--   0        0        0      993 2024-04-03 08:50:18.654846 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
+-rw-r--r--   0        0        0     1003 2024-04-03 08:50:18.655845 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
+-rw-r--r--   0        0        0      752 2024-04-03 08:50:18.655845 lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
+-rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-1.0.1/lazy_type_hint/file_modifiers/__init__.py
+-rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-1.0.1/lazy_type_hint/file_modifiers/py_file_modifier.py
+-rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-1.0.1/lazy_type_hint/file_modifiers/yaml_file_modifier.py
+-rw-r--r--   0        0        0     2380 2024-04-13 18:49:52.549938 lazy_type_hint-1.0.1/lazy_type_hint/generators/lazy_type_hint.py
+-rw-r--r--   0        0        0     3149 2024-04-03 13:39:39.224765 lazy_type_hint-1.0.1/lazy_type_hint/generators/lazy_type_hint_abc.py
+-rw-r--r--   0        0        0     9412 2024-04-03 15:48:14.649665 lazy_type_hint-1.0.1/lazy_type_hint/generators/lazy_type_hint_live.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-1.0.1/lazy_type_hint/py.typed
+-rw-r--r--   0        0        0     1638 2024-04-03 08:50:18.659845 lazy_type_hint-1.0.1/lazy_type_hint/strategies.py
+-rw-r--r--   0        0        0      706 2024-04-03 13:39:39.229769 lazy_type_hint-1.0.1/lazy_type_hint/utils/__init__.py
+-rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-1.0.1/lazy_type_hint/utils/docstring_formatter.py
+-rw-r--r--   0        0        0     4681 2024-04-03 08:50:18.660845 lazy_type_hint-1.0.1/lazy_type_hint/utils/import_manager.py
+-rw-r--r--   0        0        0     4952 2024-04-03 08:50:18.661845 lazy_type_hint-1.0.1/lazy_type_hint/utils/mypy.py
+-rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-1.0.1/lazy_type_hint/utils/ordered_set.py
+-rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-1.0.1/lazy_type_hint/utils/test_ordered_set.py
+-rw-r--r--   0        0        0     3770 2024-04-03 15:48:14.655819 lazy_type_hint-1.0.1/lazy_type_hint/utils/utils.py
+-rw-r--r--   0        0        0     2362 2024-04-13 19:30:35.977434 lazy_type_hint-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6440 2024-04-13 19:31:38.569848 lazy_type_hint-1.0.1/README.md
+-rw-r--r--   0        0        0     6832 1970-01-01 00:00:00.000000 lazy_type_hint-1.0.1/PKG-INFO
```

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/data_type_tree.py` & `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/factory.py` & `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/factory.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/generic_type/__init__.py` & `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py` & `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py` & `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py` & `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py` & `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py` & `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py` & `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py` & `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py` & `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py` & `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py` & `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py` & `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py` & `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py` & `lazy_type_hint-1.0.1/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/file_modifiers/py_file_modifier.py` & `lazy_type_hint-1.0.1/lazy_type_hint/file_modifiers/py_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/file_modifiers/yaml_file_modifier.py` & `lazy_type_hint-1.0.1/lazy_type_hint/file_modifiers/yaml_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/generators/lazy_type_hint.py` & `lazy_type_hint-1.0.1/lazy_type_hint/generators/lazy_type_hint.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/generators/lazy_type_hint_abc.py` & `lazy_type_hint-1.0.1/lazy_type_hint/generators/lazy_type_hint_abc.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/generators/lazy_type_hint_live.py` & `lazy_type_hint-1.0.1/lazy_type_hint/generators/lazy_type_hint_live.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/strategies.py` & `lazy_type_hint-1.0.1/lazy_type_hint/strategies.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/utils/__init__.py` & `lazy_type_hint-1.0.1/lazy_type_hint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/utils/docstring_formatter.py` & `lazy_type_hint-1.0.1/lazy_type_hint/utils/docstring_formatter.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/utils/import_manager.py` & `lazy_type_hint-1.0.1/lazy_type_hint/utils/import_manager.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/utils/mypy.py` & `lazy_type_hint-1.0.1/lazy_type_hint/utils/mypy.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/utils/ordered_set.py` & `lazy_type_hint-1.0.1/lazy_type_hint/utils/ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/utils/test_ordered_set.py` & `lazy_type_hint-1.0.1/lazy_type_hint/utils/test_ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/lazy_type_hint/utils/utils.py` & `lazy_type_hint-1.0.1/lazy_type_hint/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-1.0.0/pyproject.toml` & `lazy_type_hint-1.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "lazy-type-hint"
-version = "1.0.0"
-description = ""
+version = "1.0.1"
+description = "Automate type hint generation in an easy way."
 authors = ["Manuel Floriano Vázquez <mflovaa@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.urls]
 Source = "https://github.com/mflova/lazy-type-hint"
 
 [tool.poetry.dependencies]
```

### Comparing `lazy_type_hint-1.0.0/README.md` & `lazy_type_hint-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -83,16 +83,16 @@
     |:-------------:|:-------------:|
     | ![Before executing the code](img/before.PNG) | ![After executing the code](img/after.PNG) |
 
     This will allow you to:
 
    |   Imagen 1    |   Imagen 2    |
     |:-------------:|:-------------:|
-    | Perform static analysis to detect issues | ![After executing the code](img/error.PNG) |
-    | Reuse your available type hints | ![After executing the code](img/reuse.PNG) |
+    | Perform static analysis to detect issues | ![After executing the code](img/errors.PNG) |
+    | Reuse your available type hints | ![After executing the code](img/reuse_classes.PNG) |
     | Have full autocompletion support from your IDE | ![After executing the code](img/autocomplete.PNG) |
 
 
 
 
 3. Easily type hint your files (YAML, JSON) and parse extra comments found within this
    file as part of the type hint docstrings. Given a yaml file like:
```

### Comparing `lazy_type_hint-1.0.0/PKG-INFO` & `lazy_type_hint-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: lazy-type-hint
-Version: 1.0.0
-Summary: 
+Version: 1.0.1
+Summary: Automate type hint generation in an easy way.
 Author: Manuel Floriano Vázquez
 Author-email: mflovaa@gmail.com
 Requires-Python: >=3.8,<=3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -99,16 +99,16 @@
     |:-------------:|:-------------:|
     | ![Before executing the code](img/before.PNG) | ![After executing the code](img/after.PNG) |
 
     This will allow you to:
 
    |   Imagen 1    |   Imagen 2    |
     |:-------------:|:-------------:|
-    | Perform static analysis to detect issues | ![After executing the code](img/error.PNG) |
-    | Reuse your available type hints | ![After executing the code](img/reuse.PNG) |
+    | Perform static analysis to detect issues | ![After executing the code](img/errors.PNG) |
+    | Reuse your available type hints | ![After executing the code](img/reuse_classes.PNG) |
     | Have full autocompletion support from your IDE | ![After executing the code](img/autocomplete.PNG) |
 
 
 
 
 3. Easily type hint your files (YAML, JSON) and parse extra comments found within this
    file as part of the type hint docstrings. Given a yaml file like:
```

