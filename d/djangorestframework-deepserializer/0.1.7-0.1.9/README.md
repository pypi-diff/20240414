# Comparing `tmp/djangorestframework-deepserializer-0.1.7.tar.gz` & `tmp/djangorestframework-deepserializer-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangorestframework-deepserializer-0.1.7.tar", last modified: Thu Dec 21 17:45:20 2023, max compression
+gzip compressed data, was "djangorestframework-deepserializer-0.1.9.tar", last modified: Fri Jan  5 09:43:48 2024, max compression
```

## Comparing `djangorestframework-deepserializer-0.1.7.tar` & `djangorestframework-deepserializer-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 17:45:20.741750 djangorestframework-deepserializer-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-12-21 17:45:12.000000 djangorestframework-deepserializer-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      762 2023-12-21 17:45:20.741750 djangorestframework-deepserializer-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-12-21 17:45:12.000000 djangorestframework-deepserializer-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 17:45:20.741750 djangorestframework-deepserializer-0.1.7/deepserializer/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-21 17:45:12.000000 djangorestframework-deepserializer-0.1.7/deepserializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16904 2023-12-21 17:45:12.000000 djangorestframework-deepserializer-0.1.7/deepserializer/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6910 2023-12-21 17:45:12.000000 djangorestframework-deepserializer-0.1.7/deepserializer/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 17:45:20.741750 djangorestframework-deepserializer-0.1.7/djangorestframework_deepserializer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      762 2023-12-21 17:45:20.000000 djangorestframework-deepserializer-0.1.7/djangorestframework_deepserializer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-12-21 17:45:20.000000 djangorestframework-deepserializer-0.1.7/djangorestframework_deepserializer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 17:45:20.000000 djangorestframework-deepserializer-0.1.7/djangorestframework_deepserializer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-21 17:45:20.000000 djangorestframework-deepserializer-0.1.7/djangorestframework_deepserializer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-12-21 17:45:20.000000 djangorestframework-deepserializer-0.1.7/djangorestframework_deepserializer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-12-21 17:45:20.741750 djangorestframework-deepserializer-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      782 2023-12-21 17:45:12.000000 djangorestframework-deepserializer-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 09:43:48.896285 djangorestframework-deepserializer-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-01-05 09:43:40.000000 djangorestframework-deepserializer-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-01-05 09:43:48.896285 djangorestframework-deepserializer-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-01-05 09:43:40.000000 djangorestframework-deepserializer-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 09:43:48.896285 djangorestframework-deepserializer-0.1.9/deepserializer/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-01-05 09:43:40.000000 djangorestframework-deepserializer-0.1.9/deepserializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20974 2024-01-05 09:43:40.000000 djangorestframework-deepserializer-0.1.9/deepserializer/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-01-05 09:43:40.000000 djangorestframework-deepserializer-0.1.9/deepserializer/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-05 09:43:48.896285 djangorestframework-deepserializer-0.1.9/djangorestframework_deepserializer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-01-05 09:43:48.000000 djangorestframework-deepserializer-0.1.9/djangorestframework_deepserializer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-01-05 09:43:48.000000 djangorestframework-deepserializer-0.1.9/djangorestframework_deepserializer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-05 09:43:48.000000 djangorestframework-deepserializer-0.1.9/djangorestframework_deepserializer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-05 09:43:48.000000 djangorestframework-deepserializer-0.1.9/djangorestframework_deepserializer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-05 09:43:48.000000 djangorestframework-deepserializer-0.1.9/djangorestframework_deepserializer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-05 09:43:48.896285 djangorestframework-deepserializer-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-01-05 09:43:40.000000 djangorestframework-deepserializer-0.1.9/setup.py
```

### Comparing `djangorestframework-deepserializer-0.1.7/LICENSE` & `djangorestframework-deepserializer-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `djangorestframework-deepserializer-0.1.7/PKG-INFO` & `djangorestframework-deepserializer-0.1.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestframework-deepserializer
-Version: 0.1.7
+Version: 0.1.9
 Summary: A package to create deep serializer for django rest framework
 Home-page: https://github.com/Horou/djangorestframework-deepserializer
 Author: Horou and Enzo_frnt
 Keywords: Django,Django REST Framework,Deep,Depth,serializer,viewset,nested,nested serializer
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django
```

### Comparing `djangorestframework-deepserializer-0.1.7/deepserializer/serializers.py` & `djangorestframework-deepserializer-0.1.9/deepserializer/serializers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 A unique serializer for all your need of deep read and deep write, made easy
 """
-
 from collections import OrderedDict
 
+from django.db.models import Model
 from django.db.transaction import atomic
 from rest_framework import serializers
 from rest_framework.exceptions import ValidationError
 from rest_framework.utils import model_meta
 from rest_framework.utils.field_mapping import (get_nested_relation_kwargs, )
 
 
@@ -17,94 +17,151 @@
 
 
 class DeepSerializer(serializers.ModelSerializer):
     """
     A unique serializer for all your need of deep read and deep write, made easy
     """
     _serializers = {}
-    _mode = ""
+    _pk_error = "Failed to Serialize"
 
     def __init_subclass__(cls, **kwargs):
         """
         Used to save the important information like:
-        -> all the serializer inheriting this class
-        -> all the nested models for this serializer
+        -> all the serializer inheriting DeepSerializer
+        -> all the types of relationships for this serializer
         -> all the prefetch_related for this serializer
 
         You can modify the cls.prefetch_related so that it only have certain fields
         the read_only_fields will be modified latter, but for the moment it works
         """
         super().__init_subclass__(**kwargs)
         if hasattr(cls, "Meta"):
             model = cls.Meta.model
-            cls._serializers[cls._mode + model.__name__] = cls
-            cls._nested_models = cls.build_nested_models(model)
-            cls._prefetch_related = [
-                prefetch[2:]
-                for prefetch in cls.build_prefetch_related(model, [model])
-            ]
-            cls.prefetch_related = cls.to_prefetch_related()
-            cls.Meta.read_only_fields = tuple(
+            if not hasattr(cls.Meta, "use_case"):
+                cls.Meta.use_case = ""
+            if not hasattr(cls.Meta, "read_only_fields"):
+                cls.Meta.read_only_fields = tuple()
+            cls._serializers[cls.Meta.use_case + model.__name__] = cls
+            cls._many_to_many = cls.build_many_to_many_models(model)
+            cls._one_to_many = cls.build_one_to_many_models(model)
+            cls._any_to_one = dict(cls.build_one_to_one_models(model),
+                                   **cls.build_many_to_one_models(model))
+            cls._relationships = cls.build_relationship_models(model)
+            cls._prefetch_related = cls.build_prefetch_related(model, [model])
+            cls.prefetch_related = cls.get_prefetch_related()
+            cls.Meta.read_only_fields += tuple(
                 model_meta.get_field_info(model).reverse_relations)
 
     @classmethod
-    def build_nested_models(cls, model) -> dict:
+    def build_one_to_one_models(cls, model: Model) -> dict[str, Model]:
+        """
+        Get all the one_to_one relationships models for a given model.
+        With the field name in key and the Model in Value
+        """
+        return {
+            field_relation.name: field_relation.related_model
+            for field_relation in model._meta.get_fields()
+            if field_relation.one_to_one
+        }
+
+    @classmethod
+    def build_one_to_many_models(cls, model: Model) -> dict[str, tuple[Model, str]]:
+        """
+        Get tuple of all the one_to_many relationships.
+        Get all the one_to_many relationships models for a given model.
+        With the field name in key and a tuple in Value with:
+        -> models
+        -> field name of the related_model for a given model
+        (the reverse of related_name)
+        """
+        return {
+            field_relation.name: (
+                field_relation.related_model,
+                field_relation.field.name
+            )
+            for field_relation in model._meta.get_fields()
+            if field_relation.one_to_many
+            and field_relation.related_name
+        }
+
+    @classmethod
+    def build_many_to_one_models(cls, model: Model) -> dict[str, Model]:
+        """
+        Get all the many_to_one relationships models for a given model.
+        With the field name in key and the Model in Value
         """
-        Create a dict with the field name in key and the associated model in value.
+        return {
+            field_relation.name: field_relation.related_model
+            for field_relation in model._meta.get_fields()
+            if field_relation.many_to_one
+        }
 
-        model: contain the model to get the nested model from
+    @classmethod
+    def build_many_to_many_models(cls, model: Model) -> dict[str, Model]:
         """
-        exclude_set = {
-            field_name
-            for field_name in model_meta.get_field_info(model).reverse_relations
-            if field_name.endswith("_set")
+        Get all the many_to_many relationships models for a given model.
+        With the field name in key and the Model in Value
+        """
+        return {
+            field_relation.name: field_relation.related_model
+            for field_relation in model._meta.get_fields()
+            if field_relation.many_to_many
         }
+
+    @classmethod
+    def build_relationship_models(cls, model: Model) -> dict[str, Model]:
+        """
+        Get all the relationships models for a given model.
+        With the field name in key and the Model in Value
+        """
         return {
             field_relation.name: field_relation.related_model
             for field_relation in model._meta.get_fields()
-            if field_relation.related_model and f"{field_relation.name}_set" not in exclude_set
+            if field_relation.related_model
+            and (not field_relation.one_to_many
+                 or field_relation.related_name)
         }
 
     @classmethod
-    def build_prefetch_related(cls, parent_model, exclude_models: list) -> list[str]:
+    def build_prefetch_related(cls, parent_model: Model, excludes: list[Model]) -> list[str]:
         """
         Create the prefetch_related list,
         With all the prefetch from the nested model at maximum depth
         """
         prefetch_related = []
-        for field_name, model in cls.build_nested_models(parent_model).items():
-            if model not in exclude_models:
-                current_prefetch = f"__{field_name}"
-                prefetch_related.append(current_prefetch)
-                for prefetch in cls.build_prefetch_related(model, exclude_models + [model]):
-                    prefetch_related.append(current_prefetch + prefetch)
+        for field_name, model in cls.build_relationship_models(parent_model).items():
+            if model not in excludes:
+                prefetch_related.append(field_name)
+                for prefetch in cls.build_prefetch_related(model, excludes + [model]):
+                    prefetch_related.append(f"{field_name}__{prefetch}")
         return prefetch_related
 
     @classmethod
-    def to_prefetch_related(cls, excludes: list[str] = []) -> list[str]:
+    def get_prefetch_related(cls, excludes: list[str] = []) -> list[str]:
         """
         Get the prefetch_related list for this class, two use case:
         -> queryset.prefetch_related(*self.to_prefetch_related())
-        -> class.prefetch_related = class.to_prefetch_related(exclude=['model1', 'model2'])
+        -> class.prefetch_related = class.to_prefetch_related(exclude=['Model1', 'Model2'])
 
         excludes: Field name of the model who will be removed from this serializer
         return: list of prefetch related filtered with the correct depth and without the excluded
         """
         return [
             prefetch_related
             for prefetch_related in cls._prefetch_related
-            if len(prefetch_related.split('__')) < cls.Meta.depth + 2 and not any(
+            if len(prefetch_related.split('__')) < cls.Meta.depth + 2
+            and not any(
                 prefetch_related.startswith(exclude)
                 for exclude in excludes
                 if exclude
             )
         ]
 
     @classmethod
-    def get_nested_prefetch(cls, field_name: str) -> list[str]:
+    def get_nested_prefetch_related(cls, field_name: str) -> list[str]:
         """
         Used to get the prefetch_related of a nested serializer
 
         field_name: Field name of the model to get the prefetch from
         return: list of prefetch related starting with 'field_name'
         """
         nested_prefetch = []
@@ -121,24 +178,24 @@
         return (
                 [model_info.pk.name] +
                 list(declared_fields) +
                 list(model_info.fields) +
                 list(set(field.split('__')[0] for field in self.prefetch_related))
         )
 
-    def build_nested_field(self, field_name: str, relation_info, nested_depth: int):
+    def build_nested_field(self, field_name: str, relation_info, nested_depth: int) -> tuple:
         """
         Has been overriden to enable the safe visualisation of a deeply nested models
         Without circular depth problem
         """
         serializer = self.get_serializer(
             relation_info.related_model,
-            mode=f"Read{self.Meta.model.__name__}Nested"
+            use_case=f"Read{self.Meta.model.__name__}Nested"
         )
-        serializer.prefetch_related = self.get_nested_prefetch(field_name)
+        serializer.prefetch_related = self.get_nested_prefetch_related(field_name)
         serializer.Meta.depth = nested_depth - 1
         return serializer, get_nested_relation_kwargs(relation_info)
 
     def deep_dict_travel(self, data: dict) -> tuple[str, dict]:
         """
         Recursively travel through a model to create the nested models first.
         Override it to change update_or_create into something else like get_or_create
@@ -146,70 +203,106 @@
         This algo only work with one_to_one, one_to_many or many_to_many relationships.
         If you need to create through a many_to_one, juste reverse your data
 
         data: The dict to create or update
         return: The primary key of the created instance and its data representation
         """
         nested = {}
-        for field_name, model in self._nested_models.items():
-            field_data = data.get(field_name, None)
-            serializer = self.get_serializer(model, mode="Nested")(context=self.context)
-            if isinstance(field_data, dict):
+        for field_name, model in self._any_to_one.items():
+            if isinstance(field_data := data.get(field_name, None), dict):
+                serializer = self.get_serializer(model, use_case="Nested")(context=self.context)
                 data[field_name], nested[field_name] = serializer.deep_dict_travel(field_data)
-            elif isinstance(field_data, list):
+        for field_name, model in self._many_to_many.items():
+            if isinstance(field_data := data.get(field_name, None), list):
+                serializer = self.get_serializer(model, use_case="Nested")(context=self.context)
                 if result := serializer.deep_list_travel(field_data):
-                    data[field_name], nested[field_name] = map(list, result)
-        return self.update_or_create(data, nested)
+                    data[field_name], nested[field_name] = map(list, zip(*result))
+        create_later = {}
+        for field_name, (model, reverse_name) in self._one_to_many.items():
+            if isinstance(field_data := data.pop(field_name, None), list):
+                create_later[field_name] = (model, reverse_name, field_data)
+        pk, representation = self.update_or_create(data, nested=nested)
+        for field_name, (model, reverse_name, field_data) in create_later.items():
+            for dict_data in field_data:
+                if isinstance(dict_data, dict):
+                    dict_data[reverse_name] = pk
+            serializer = self.get_serializer(model, use_case="Nested")(context=self.context)
+            if result := serializer.deep_list_travel(field_data):
+                _, representation[field_name] = map(list, zip(*result))
+                if any(f"ERROR" in item for item in representation[field_name]):
+                    if "ERROR" not in representation:
+                        representation["ERROR"] = "Failed to Serialize nested objects"
+        return pk, representation
 
-    def deep_list_travel(self, data_list: list[str | dict]) -> list[tuple[str, dict]]:
+    def deep_list_travel(self, datas: list[any]) -> list[tuple[str, dict]]:
         """
         Recursively travel through a list of model to create the nested models first.
         Override it to change bulk_update_or_create into something else like bulk_get_or_create
 
-        This algo only work with one_to_one, one_to_many or many_to_many relationships.
-        If you need to create through a many_to_one, juste reverse your data
-
         data_list: A list of dict to create or update
         return: List of tuple of the created instance primary key and its data representation
         """
-        data_and_nested_list = [(data, {}) for data in data_list]
-        to_create = [
-            data_and_nested
-            for data_and_nested in data_and_nested_list
-            if isinstance(data_and_nested[0], dict)
-        ]
-        for field_name, model in self._nested_models.items():
-            serializer = self.get_serializer(model, mode="Nested")(context=self.context)
-            if one_to_datas := [
-                data_and_nested
-                for data_and_nested in to_create
-                if isinstance(data_and_nested[0].get(field_name, None), dict)
-            ]:
-                nested_results = serializer.deep_list_travel([
-                    data[field_name]
-                    for data, _ in one_to_datas
-                ])
-                for (data, nested), nested_result in zip(one_to_datas, nested_results):
-                    data[field_name], nested[field_name] = nested_result
-            elif many_to_datas := [
-                data_and_nested
-                for data_and_nested in to_create
-                if isinstance(data_and_nested[0].get(field_name, None), list)
-            ]:
-                flatten_nested_results = serializer.deep_list_travel([
-                    data
-                    for data_sublist, _ in many_to_datas
-                    for data in data_sublist[field_name]
-                ])
-                for data, nested in many_to_datas:
-                    length = len(data[field_name])
-                    if nested_result := flatten_nested_results[:length]:
-                        data[field_name], nested[field_name] = map(list, zip(*nested_result))
-                        flatten_nested_results = flatten_nested_results[length:]
-        return self.bulk_update_or_create(data_and_nested_list)
+        data_and_nested = [(data, {}) for data in datas]
+        datas_to_process = [data for data in data_and_nested if isinstance(data[0], dict)]
+
+        for field_name, model in self._any_to_one.items():
+            filtered_data_and_nested, field_datas = [], []
+            for data, nested in datas_to_process:
+                if isinstance(field_data := data.get(field_name, None), dict):
+                    filtered_data_and_nested.append((data, nested))
+                    field_datas.append(field_data)
+            if filtered_data_and_nested:
+                serializer = self.get_serializer(model, use_case="Nested")(context=self.context)
+                results = serializer.deep_list_travel(field_datas)
+                for (data, nested), result in zip(filtered_data_and_nested, results):
+                    data[field_name], nested[field_name] = result
+
+        for field_name, model in self._many_to_many.items():
+            filtered_data_and_nested, field_datas = [], []
+            for data, nested in datas_to_process:
+                if isinstance(field_data := data.get(field_name, None), list):
+                    if (length := len(field_data)) > 0:
+                        filtered_data_and_nested.append((data, nested, length))
+                        field_datas += field_data
+            if filtered_data_and_nested:
+                serializer = self.get_serializer(model, use_case="Nested")(context=self.context)
+                results = serializer.deep_list_travel(field_datas)
+                for data, nested, length in filtered_data_and_nested:
+                    data[field_name], nested[field_name] = map(list, zip(*results[:length]))
+                    results = results[length:]
+
+        process_later = {}
+        for field_name, (model, reverse_name) in self._one_to_many.items():
+            filtered_data_information = []
+            for index, (data, nested) in enumerate(data_and_nested):
+                if isinstance(data, dict) and isinstance(field := data.pop(field_name, 0), list):
+                    if (length := len(field)) > 0:
+                        filtered_data_information.append((index, length, field))
+            if filtered_data_information:
+                process_later[field_name] = (model, reverse_name, filtered_data_information)
+
+        pk_and_representation = self.bulk_update_or_create(data_and_nested)
+
+        for field_name, (model, reverse_name, filtered_data_information) in process_later.items():
+            field_datas = []
+            for index, length, field_data in filtered_data_information:
+                for data in field_data:
+                    data[reverse_name] = pk_and_representation[index][0]
+                    field_datas.append(data)
+            serializer = self.get_serializer(model, use_case="Nested")(context=self.context)
+            results = serializer.deep_list_travel(field_datas)
+            for index, length, field_data in filtered_data_information:
+                pk, representation = pk_and_representation[index]
+                _, representation[field_name] = map(list, zip(*results[:length]))
+                results = results[length:]
+                if any(f"ERROR" in item for item in representation[field_name]):
+                    if "ERROR" not in representation:
+                        representation["ERROR"] = "Failed to Serialize nested objects"
+
+        return pk_and_representation
 
     def update_or_create(self, data: dict, nested: dict, instances: dict = None
                          ) -> tuple[str, dict]:
         """
         Create or update one instance with data, base on the model primary key
 
         data: the dict that contain the data who will be created or updated
@@ -225,18 +318,18 @@
             if instances is not None:
                 self.instance = instances.get(pk, None)
             else:
                 self.instance = self.Meta.model.objects.filter(pk=pk).first()
         self.initial_data, self.partial = data, bool(self.instance)
         if self.is_valid():
             return self.save().pk, OrderedDict(self.data, **nested)
-        return (f"Failed to serialize {self.Meta.model.__name__}",
-                OrderedDict(nested, ERROR=self.errors))
+        return self._pk_error, OrderedDict(ERROR=self._pk_error, **self.errors, **nested)
 
-    def bulk_update_or_create(self, data_and_nested: list[tuple[any, dict]]) -> list[tuple]:
+    def bulk_update_or_create(self, data_and_nested: list[tuple[any, dict]]
+                              ) -> list[tuple[str, dict]]:
         """
         Create or update multiple instance with the data in data_and_nested.
         The instances are updated or created one time base on the model primary key.
         If the primary_key exist, it will update the instance one time and reuse
         this instance result when the primary key is found inside data_and_nested again
         If the primary_key does not exist, it will create a new instance and reuse
         this instance result when the primary key is found inside data_and_nested again
@@ -250,122 +343,93 @@
         -> primary_key or 'Failed to serialize' for the created or updated model
         -> representation or ERROR information for the created or updated model
         """
         pks_and_representations, created = [], {}
         model = self.Meta.model
         pk_name = model._meta.pk.name
         found_pks = set(data[pk_name] for data, _ in data_and_nested if pk_name in data)
-        instances = model.objects.prefetch_related(*self.to_prefetch_related()
+        instances = model.objects.prefetch_related(*self.get_prefetch_related()
                                                    ).in_bulk(found_pks)
         for data, nested in data_and_nested:
             if isinstance(data, dict):
                 found_pk = data.get(pk_name, None)
                 if found_pk not in created:
                     created_pk, representation = self.update_or_create(
                         data, nested, instances=instances)
                     found_pk = found_pk if found_pk is not None else created_pk
                     created[found_pk] = (created_pk, representation)
                     self.instance = None
                     if "ERROR" not in representation:
                         del self._data, self._validated_data
                 pks_and_representations.append(created[found_pk])
             else:
-                pks_and_representations.append((data, data))
+                pks_and_representations.append((data, nested))
         return pks_and_representations
 
-    def deep_create(self, data: dict | list, verbose: bool = True) -> list[str] | list[dict]:
+    def deep_create(self, data: dict | list, verbose: bool = True, model: any = None
+                    ) -> list[str] | list[dict]:
         """
         Create either a list of model or a unique model with their nested models at any depth.
 
         It is recommended to construct the json that will be created after receiving the data
         and not use the pure request data, but you do you ¯\\_(ツ)_//¯
 
         If the resulting data is too big to be sent back,
         'verbose'=False is used to only send the primary_key of the created model.
         If there has been errors it will send the dict with the errors regardless of verbose
 
-        The deep_create only work with one_to_one, one_to_many or many_to_many relationships,
-            If you need to create a model through a many_to_one juste reverse it like:
-            example of 'Admin' group: {
-                "id": "Admin",
-                "description": "Group of admin"
-                "users": [
-                    {
-                        "firstname": 'john',
-                        "lastname": 'Doe'
-                    },
-                    {
-                        "firstname": 'jane',
-                        "lastname": 'Doe'
-                    }
-                ]
-            }
-            changed into: [
-                {
-                    "firstname": 'john',
-                    "lastname": 'Doe'
-                    "group": {
-                        "id": "Admin"
-                        "description": "Group of admin"
-                    }
-                },
-                {
-                    "firstname": 'Jane',
-                    "lastname": 'Doe'
-                    "group": {
-                        "id": "Admin"
-                        "description": "Group of admin"
-                    }
-                }
-            ]
+        The deep_create work with:
+        one_to_one, one_to_many, many_to_one and many_to_many relationships.
         """
         try:
             with atomic():
-                serializer = self.get_serializer(self.Meta.model,
-                                                 mode="Nested")(context=self.context)
+                serializer = self.get_serializer(
+                    model if model else self.Meta.model,
+                    use_case="Nested"
+                )(context=self.context)
                 if data and isinstance(data, dict):
                     primary_key, representation = serializer.deep_dict_travel(data)
                     if "ERROR" in representation:
                         raise ValidationError(representation)
                     return representation if verbose else primary_key
                 elif data and isinstance(data, list):
-                    primary_key, representation = map(list,
-                                                      zip(*serializer.deep_list_travel(data)))
+                    primary_key, representation = map(list, zip(*serializer.deep_list_travel(data)))
                     if errors := [d for d in representation if "ERROR" in d]:
                         raise ValidationError(errors)
                     return representation if verbose else primary_key
         except ValidationError as e:
             return e.detail
 
     @classmethod
-    def get_serializer(cls, _model, mode: str = ""):
+    def get_serializer(cls, model: Model, use_case: str = ""):
         """
-        Get back or create a serializer for the _model and its mode.
-        Manually created serializer inheriting DeepViewSet will automatically be used for its mode
+        Get back or create a serializer for the _model and its use case.
+        Manually created serializer inheriting DeepViewSet will automatically be used
+        for its use case.
 
-        If your serializer is only used in a specific use-case, write it in the mode
+        If your serializer is only used in a specific use-case, write it in the use_case
 
-        _model: Contain the model related to the serializer wanted
-        mode: Contain the use that this serializer will be used for,
+        model: Contain the model related to the serializer wanted
+        use_case: Contain the use that this serializer will be used for,
         -> if empty, it will be the main serializer for this model
         """
-        if mode + _model.__name__ not in cls._serializers:
-            parent = cls.get_serializer(_model) if mode else DeepSerializer
+        if use_case + model.__name__ not in cls._serializers:
+            parent = cls.get_serializer(model) if use_case else DeepSerializer
+            _use_case, _model = use_case, model
 
             class CommonSerializer(parent):
                 """
                 Common serializer template.
                 Inherit either the DeepSerializer or the main model serializer.
                 """
-                _mode = mode
 
                 class Meta:
                     model = _model
                     depth = 0
-                    fields = parent.Meta.fields if mode else '__all__'
-
-        return cls._serializers[mode + _model.__name__]
+                    fields = parent.Meta.fields if _use_case else '__all__'
+                    use_case = _use_case
 
+        return cls._serializers[use_case + model.__name__]
 
 ###################################################################################################
 #
 ###################################################################################################
```

### Comparing `djangorestframework-deepserializer-0.1.7/deepserializer/views.py` & `djangorestframework-deepserializer-0.1.9/deepserializer/views.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,28 +16,28 @@
 class ReadOnlyDeepViewSet(ReadOnlyModelViewSet):
     """
     A unique viewset for all your need of deep read and deep write, made easy
 
     Read only version
     """
     _viewsets = {}
-    _mode = "Read"
+    use_case = "Read"
     depth = 0
     exclude_nesteds = []
 
     def __init_subclass__(cls, **kwargs):
         """
         Used to save the important information like:
         -> all the viewset inheriting this class
         -> all the possible fields to 'filter by' or 'order by' the queryset
         """
         super().__init_subclass__(**kwargs)
-        if cls.queryset:
+        if hasattr(cls, 'queryset') and cls.queryset is not None:
             model = cls.queryset.model
-            cls._viewsets[cls._mode + model.__name__] = cls
+            cls._viewsets[cls.use_case + model.__name__] = cls
             cls._possible_fields = [
                 field_name[2:]
                 for field_name in cls.build_filter_fields(model, [model])
             ]
 
     @classmethod
     def build_filter_fields(cls, parent_model, exclude_models: list) -> list[str]:
@@ -69,18 +69,18 @@
         models: list of model to register in the router
         """
         for model in models:
             router.register(model.__name__, cls.get_view(model), basename=model.__name__)
 
     def get_serializer_class(self):
         """
-        Get the seralizer class for this viewset and its mode,
-        No mode mean it will get the main serializer for the model
+        Get the seralizer class for this viewset and its use_case,
+        No use_case mean it will get the main serializer for the model
         """
-        return DeepSerializer.get_serializer(self.queryset.model, mode=self._mode)
+        return DeepSerializer.get_serializer(self.queryset.model, use_case=self.use_case)
 
     def get_queryset(self):
         """
         Is used to modify the queryset to get exactly what you want
 
         Filtering is made with 'field_name=value'.
         -> Example: /?lastname=Doe&age=30
@@ -94,15 +94,15 @@
         Remove deeper model with 'exclude' like 'exclude=foo,bar'.
         If the nested model to exclude is nested in a nested model, separate them with '__'
         -> Example: /?exclude=job,user__group,user__comments__status
         """
         params = self.request.query_params
         serializer = self.get_serializer_class()
         serializer.Meta.depth = int(params.get("depth", self.depth))
-        serializer.prefetch_related = serializer.to_prefetch_related(
+        serializer.prefetch_related = serializer.get_prefetch_related(
             excludes=params.get("exclude", ",".join(self.exclude_nesteds)).split(","))
         queryset = self.queryset.prefetch_related(*serializer.prefetch_related)
         if filter_by := {
             field: value
             for field, value in params.items()
             if field in self._possible_fields
         }:
@@ -112,26 +112,28 @@
             for field in params.get("order_by", "").split(",")
             if field in self._possible_fields
         ]:
             queryset = queryset.order_by(*order_by)
         return queryset
 
     @classmethod
-    def get_view(cls, _model, mode: str = ""):
+    def get_view(cls, _model, use_case: str = ""):
         """
-        Get back or create a viewset for the _model and its mode.
-        Manually created viewset inheriting DeepViewSet will automatically be used for its mode
+        Get back or create a viewset for the _model and its use_case.
+        Manually created viewset inheriting DeepViewSet will automatically be used for its use_case
 
-        If your viewset is only used in a specific use-case, write it in the mode
+        If your viewset is only used in a specific use-case, write it in the use_case
 
         _model: Contain the model related to the viewset wanted
-        mode: Contain the use that this viewset will be used for,
+        use_case: Contain the use that this viewset will be used for,
             if empty, it will be the main viewset for this model
         """
-        if mode + _model.__name__ not in cls._viewsets:
+        if use_case + _model.__name__ not in cls._viewsets:
+            _use_case = use_case
+
             class CommonViewSet(cls):
                 """
                 For GET request:
                 Filtering is made with 'field_name=value'.
                 -> Example: /?lastname=Doe&age=30
                 Filter by nested model field with 'field_name__field_name=value'.
                 -> Example: /?group__label=bar
@@ -140,31 +142,31 @@
                 -> Example: /?order_by=lastname,firstname
                 Display deeper model with 'depth' like 'depth=level'.
                 -> Example: /?depth=5)
                 Remove deeper model with 'exclude' like 'exclude=foo,bar'.
                 Separate them with '__' if the model to exclude is in a nested model
                 -> Example: /?exclude=job,user__group,user__comments__status
                 """
-                _mode = mode
+                use_case = _use_case
                 queryset = _model.objects
 
             CommonViewSet.__name__ = _model.__name__
             CommonViewSet.__doc__ = f"""
             View Set for the model: '{_model.__name__}'
-            Used for {mode if mode else 'Read and Write'}
+            Used for {use_case if use_case else 'Read and Write'}
             
             """ + CommonViewSet.__doc__
 
-        return cls._viewsets[mode + _model.__name__]
+        return cls._viewsets[use_case + _model.__name__]
 
 
 class DeepViewSet(ReadOnlyDeepViewSet, ModelViewSet):
     """
     A unique viewset for all your need of deep read and deep write, made easy
 
     Read and Write version
     """
-    _mode = ""
+    use_case = ""
 
 ###################################################################################################
 #
 ###################################################################################################
```

### Comparing `djangorestframework-deepserializer-0.1.7/djangorestframework_deepserializer.egg-info/PKG-INFO` & `djangorestframework-deepserializer-0.1.9/djangorestframework_deepserializer.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangorestframework-deepserializer
-Version: 0.1.7
+Version: 0.1.9
 Summary: A package to create deep serializer for django rest framework
 Home-page: https://github.com/Horou/djangorestframework-deepserializer
 Author: Horou and Enzo_frnt
 Keywords: Django,Django REST Framework,Deep,Depth,serializer,viewset,nested,nested serializer
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django
```

### Comparing `djangorestframework-deepserializer-0.1.7/setup.py` & `djangorestframework-deepserializer-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='djangorestframework-deepserializer',
-    version='0.1.7',
+    version='0.1.9',
     packages=['deepserializer'],
     install_requires=[
         'Django',
         'djangorestframework',
     ],
     description='A package to create deep serializer for django rest framework',
     long_description=long_description,
```

