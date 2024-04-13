# Comparing `tmp/gena-1.6.6.tar.gz` & `tmp/gena-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gena-1.6.6.tar", max compression
+gzip compressed data, was "gena-1.6.7.tar", max compression
```

## Comparing `gena-1.6.6.tar` & `gena-1.6.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1064 2023-12-22 08:00:10.634678 gena-1.6.6/LICENSE
--rw-r--r--   0        0        0    11698 2023-12-22 08:00:10.634678 gena-1.6.6/README.md
--rw-r--r--   0        0        0      109 2023-12-22 08:00:10.662679 gena-1.6.6/gena/__init__.py
--rw-r--r--   0        0        0    19938 2023-12-22 08:00:10.662679 gena-1.6.6/gena/api_generator.py
--rw-r--r--   0        0        0     2122 2023-12-22 08:00:10.662679 gena-1.6.6/gena/api_testsuite.py
--rw-r--r--   0        0        0     1868 2023-12-22 08:00:10.662679 gena-1.6.6/gena/app_generator.py
--rw-r--r--   0        0        0     3314 2023-12-22 08:00:10.662679 gena-1.6.6/gena/client.py
--rw-r--r--   0        0        0     1391 2023-12-22 08:00:10.662679 gena-1.6.6/gena/config.py
--rw-r--r--   0        0        0     2329 2023-12-22 08:00:10.662679 gena-1.6.6/gena/custom_fields.py
--rw-r--r--   0        0        0    16115 2023-12-22 08:00:10.662679 gena-1.6.6/gena/deserializer.py
--rw-r--r--   0        0        0    10294 2023-12-22 08:00:10.662679 gena-1.6.6/gena/serializer.py
--rw-r--r--   0        0        0      576 2023-12-22 08:00:10.662679 gena-1.6.6/pyproject.toml
--rw-r--r--   0        0        0    12566 1970-01-01 00:00:00.000000 gena-1.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-13 23:35:28.564433 gena-1.6.7/LICENSE
+-rw-r--r--   0        0        0    11698 2024-04-13 23:35:28.564433 gena-1.6.7/README.md
+-rw-r--r--   0        0        0      109 2024-04-13 23:35:28.592433 gena-1.6.7/gena/__init__.py
+-rw-r--r--   0        0        0    20027 2024-04-13 23:35:28.592433 gena-1.6.7/gena/api_generator.py
+-rw-r--r--   0        0        0     2122 2024-04-13 23:35:28.592433 gena-1.6.7/gena/api_testsuite.py
+-rw-r--r--   0        0        0     1868 2024-04-13 23:35:28.592433 gena-1.6.7/gena/app_generator.py
+-rw-r--r--   0        0        0     3314 2024-04-13 23:35:28.592433 gena-1.6.7/gena/client.py
+-rw-r--r--   0        0        0     1391 2024-04-13 23:35:28.592433 gena-1.6.7/gena/config.py
+-rw-r--r--   0        0        0     2329 2024-04-13 23:35:28.592433 gena-1.6.7/gena/custom_fields.py
+-rw-r--r--   0        0        0    16115 2024-04-13 23:35:28.592433 gena-1.6.7/gena/deserializer.py
+-rw-r--r--   0        0        0    10294 2024-04-13 23:35:28.592433 gena-1.6.7/gena/serializer.py
+-rw-r--r--   0        0        0      576 2024-04-13 23:35:28.592433 gena-1.6.7/pyproject.toml
+-rw-r--r--   0        0        0    12566 1970-01-01 00:00:00.000000 gena-1.6.7/PKG-INFO
```

### Comparing `gena-1.6.6/LICENSE` & `gena-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `gena-1.6.6/README.md` & `gena-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `gena-1.6.6/gena/api_generator.py` & `gena-1.6.7/gena/api_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 
 import re
 from collections import defaultdict
 from enum import Enum
 from typing import Any, Callable, Mapping, Optional, Type, TypeVar
 
 from flask import Blueprint, jsonify, request
-from gena.deserializer import generate_deserializer
-from gena.serializer import Serializer, get_peewee_serializer
 from peewee import DoesNotExist, ForeignKeyField
 from peewee import Model as PeeweeModel
 from peewee import fn
 from werkzeug.exceptions import BadRequest, NotFound
 
+from gena.deserializer import generate_deserializer
+from gena.serializer import Serializer, get_peewee_serializer
+
 T = TypeVar("T")
 
 
 class APIFuncs(str, Enum):
     get = "get"
     get_by_ids = "get_by_ids"
     get_one = "get_one"
@@ -455,14 +456,17 @@
         if len(lst) > 1:
             raise BadRequest(f"Invalid query. Only one field is allowed but get: {lst}")
 
         if len(lst) == 0:
             raise BadRequest(f"Invalid query. Must provide at least one field")
 
         id = unique_field_funcs[lst[0]](request.args[lst[0]])
+        if id not in id2ent:
+            raise NotFound(f"Record {id} does not exist")
+
         record = serialize(id2ent[id])
         if len(field_names) > 0:
             record = {k: record[k] for k in field_names if k in record}
 
         return jsonify({"items": [record], "total": 1})
 
     @bp.route(f"/{name}/find_by_ids", methods=["POST"])
```

### Comparing `gena-1.6.6/gena/api_testsuite.py` & `gena-1.6.7/gena/api_testsuite.py`

 * *Files identical despite different names*

### Comparing `gena-1.6.6/gena/app_generator.py` & `gena-1.6.7/gena/app_generator.py`

 * *Files identical despite different names*

### Comparing `gena-1.6.6/gena/client.py` & `gena-1.6.7/gena/client.py`

 * *Files identical despite different names*

### Comparing `gena-1.6.6/gena/config.py` & `gena-1.6.7/gena/config.py`

 * *Files identical despite different names*

### Comparing `gena-1.6.6/gena/custom_fields.py` & `gena-1.6.7/gena/custom_fields.py`

 * *Files identical despite different names*

### Comparing `gena-1.6.6/gena/deserializer.py` & `gena-1.6.7/gena/deserializer.py`

 * *Files identical despite different names*

### Comparing `gena-1.6.6/gena/serializer.py` & `gena-1.6.7/gena/serializer.py`

 * *Files identical despite different names*

### Comparing `gena-1.6.6/pyproject.toml` & `gena-1.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gena"
-version = "1.6.6"
+version = "1.6.7"
 description = "Generate APIs from Database Models"
 authors = ["Binh Vu <binh@toan2.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `gena-1.6.6/PKG-INFO` & `gena-1.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gena
-Version: 1.6.6
+Version: 1.6.7
 Summary: Generate APIs from Database Models
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

