# Comparing `tmp/etl_pipes-0.8.8.tar.gz` & `tmp/etl_pipes-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_pipes-0.8.8.tar", max compression
+gzip compressed data, was "etl_pipes-0.8.9.tar", max compression
```

## Comparing `etl_pipes-0.8.8.tar` & `etl_pipes-0.8.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     7429 2024-04-10 23:23:16.412874 etl_pipes-0.8.8/README.md
--rw-r--r--   0        0        0        0 2023-09-03 18:03:42.309231 etl_pipes-0.8.8/etl_pipes/__init__.py
--rw-r--r--   0        0        0        0 2024-03-31 18:15:41.760794 etl_pipes-0.8.8/etl_pipes/actors/__init__.py
--rw-r--r--   0        0        0     2217 2024-04-09 11:57:50.370449 etl_pipes-0.8.8/etl_pipes/actors/actor.py
--rw-r--r--   0        0        0     9002 2024-04-09 13:10:44.698790 etl_pipes-0.8.8/etl_pipes/actors/actor_system.py
--rw-r--r--   0        0        0        0 2024-03-31 18:15:41.762064 etl_pipes-0.8.8/etl_pipes/actors/common/__init__.py
--rw-r--r--   0        0        0      829 2024-03-31 18:15:41.762369 etl_pipes-0.8.8/etl_pipes/actors/common/logging.py
--rw-r--r--   0        0        0     1797 2024-04-09 12:27:49.338234 etl_pipes-0.8.8/etl_pipes/actors/common/types.py
--rw-r--r--   0        0        0        0 2023-09-03 21:40:10.190762 etl_pipes-0.8.8/etl_pipes/common/__init__.py
--rw-r--r--   0        0        0        0 2023-09-03 21:40:14.655898 etl_pipes-0.8.8/etl_pipes/common/utils/__init__.py
--rw-r--r--   0        0        0      108 2023-09-03 22:08:31.373727 etl_pipes-0.8.8/etl_pipes/common/utils/type_hints.py
--rw-r--r--   0        0        0      949 2024-04-08 19:20:17.455265 etl_pipes-0.8.8/etl_pipes/context.py
--rw-r--r--   0        0        0        0 2023-09-12 21:09:45.406624 etl_pipes-0.8.8/etl_pipes/domain/__init__.py
--rw-r--r--   0        0        0      126 2024-03-30 18:10:45.704746 etl_pipes-0.8.8/etl_pipes/domain/types.py
--rw-r--r--   0        0        0        0 2023-09-03 19:52:04.178084 etl_pipes-0.8.8/etl_pipes/pipes/__init__.py
--rw-r--r--   0        0        0     2958 2024-04-08 19:20:17.455523 etl_pipes-0.8.8/etl_pipes/pipes/base_pipe.py
--rw-r--r--   0        0        0      347 2024-03-30 18:10:45.705264 etl_pipes-0.8.8/etl_pipes/pipes/broadcast_parallel.py
--rw-r--r--   0        0        0      754 2024-03-30 18:10:45.705554 etl_pipes-0.8.8/etl_pipes/pipes/map_reduce.py
--rw-r--r--   0        0        0      966 2024-03-30 18:10:45.705891 etl_pipes-0.8.8/etl_pipes/pipes/maybe.py
--rw-r--r--   0        0        0      780 2024-03-30 18:10:45.706672 etl_pipes-0.8.8/etl_pipes/pipes/parallel.py
--rw-r--r--   0        0        0        0 2023-09-03 21:51:24.387827 etl_pipes-0.8.8/etl_pipes/pipes/pipeline/__init__.py
--rw-r--r--   0        0        0     1718 2023-09-12 21:22:40.624232 etl_pipes-0.8.8/etl_pipes/pipes/pipeline/exceptions.py
--rw-r--r--   0        0        0     4175 2024-04-01 15:12:43.908804 etl_pipes-0.8.8/etl_pipes/pipes/pipeline/pipe_welding_validator.py
--rw-r--r--   0        0        0     2042 2024-04-08 19:23:03.911275 etl_pipes-0.8.8/etl_pipes/pipes/pipeline/pipeline.py
--rw-r--r--   0        0        0     1133 2024-04-10 23:23:35.241616 etl_pipes-0.8.8/pyproject.toml
--rw-r--r--   0        0        0     7747 1970-01-01 00:00:00.000000 etl_pipes-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0     7429 2024-04-10 23:24:43.384306 etl_pipes-0.8.9/README.md
+-rw-r--r--   0        0        0        0 2023-09-03 18:03:42.309231 etl_pipes-0.8.9/etl_pipes/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-31 18:15:41.760794 etl_pipes-0.8.9/etl_pipes/actors/__init__.py
+-rw-r--r--   0        0        0     2217 2024-04-09 11:57:50.370449 etl_pipes-0.8.9/etl_pipes/actors/actor.py
+-rw-r--r--   0        0        0     9002 2024-04-09 13:10:44.698790 etl_pipes-0.8.9/etl_pipes/actors/actor_system.py
+-rw-r--r--   0        0        0        0 2024-03-31 18:15:41.762064 etl_pipes-0.8.9/etl_pipes/actors/common/__init__.py
+-rw-r--r--   0        0        0      829 2024-03-31 18:15:41.762369 etl_pipes-0.8.9/etl_pipes/actors/common/logging.py
+-rw-r--r--   0        0        0     1797 2024-04-09 12:27:49.338234 etl_pipes-0.8.9/etl_pipes/actors/common/types.py
+-rw-r--r--   0        0        0        0 2023-09-03 21:40:10.190762 etl_pipes-0.8.9/etl_pipes/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-03 21:40:14.655898 etl_pipes-0.8.9/etl_pipes/common/utils/__init__.py
+-rw-r--r--   0        0        0      108 2023-09-03 22:08:31.373727 etl_pipes-0.8.9/etl_pipes/common/utils/type_hints.py
+-rw-r--r--   0        0        0      949 2024-04-08 19:20:17.455265 etl_pipes-0.8.9/etl_pipes/context.py
+-rw-r--r--   0        0        0        0 2023-09-12 21:09:45.406624 etl_pipes-0.8.9/etl_pipes/domain/__init__.py
+-rw-r--r--   0        0        0      126 2024-03-30 18:10:45.704746 etl_pipes-0.8.9/etl_pipes/domain/types.py
+-rw-r--r--   0        0        0        0 2023-09-03 19:52:04.178084 etl_pipes-0.8.9/etl_pipes/pipes/__init__.py
+-rw-r--r--   0        0        0     2958 2024-04-08 19:20:17.455523 etl_pipes-0.8.9/etl_pipes/pipes/base_pipe.py
+-rw-r--r--   0        0        0      347 2024-03-30 18:10:45.705264 etl_pipes-0.8.9/etl_pipes/pipes/broadcast_parallel.py
+-rw-r--r--   0        0        0      754 2024-03-30 18:10:45.705554 etl_pipes-0.8.9/etl_pipes/pipes/map_reduce.py
+-rw-r--r--   0        0        0      966 2024-03-30 18:10:45.705891 etl_pipes-0.8.9/etl_pipes/pipes/maybe.py
+-rw-r--r--   0        0        0      780 2024-03-30 18:10:45.706672 etl_pipes-0.8.9/etl_pipes/pipes/parallel.py
+-rw-r--r--   0        0        0        0 2023-09-03 21:51:24.387827 etl_pipes-0.8.9/etl_pipes/pipes/pipeline/__init__.py
+-rw-r--r--   0        0        0     1718 2023-09-12 21:22:40.624232 etl_pipes-0.8.9/etl_pipes/pipes/pipeline/exceptions.py
+-rw-r--r--   0        0        0     4175 2024-04-01 15:12:43.908804 etl_pipes-0.8.9/etl_pipes/pipes/pipeline/pipe_welding_validator.py
+-rw-r--r--   0        0        0     2042 2024-04-08 19:23:03.911275 etl_pipes-0.8.9/etl_pipes/pipes/pipeline/pipeline.py
+-rw-r--r--   0        0        0     1133 2024-04-10 23:24:45.983942 etl_pipes-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0     7747 1970-01-01 00:00:00.000000 etl_pipes-0.8.9/PKG-INFO
```

### Comparing `etl_pipes-0.8.8/README.md` & `etl_pipes-0.8.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Etl-Pipes
 
 ## Description
 
-Pypelines is a Python library for creating flow-based programming pipelines.
+etl-pipes is a Python library for creating flow-based programming pipelines.
 
 ## Primitives
 
 ### Implemented
 
 - Pipeline
   - used to combine pipes into a single sequential pipeline, used to implement "|" operator
```

### Comparing `etl_pipes-0.8.8/etl_pipes/actors/actor.py` & `etl_pipes-0.8.9/etl_pipes/actors/actor.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.8.8/etl_pipes/actors/actor_system.py` & `etl_pipes-0.8.9/etl_pipes/actors/actor_system.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.8.8/etl_pipes/actors/common/logging.py` & `etl_pipes-0.8.9/etl_pipes/actors/common/logging.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.8.8/etl_pipes/actors/common/types.py` & `etl_pipes-0.8.9/etl_pipes/actors/common/types.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.8.8/etl_pipes/context.py` & `etl_pipes-0.8.9/etl_pipes/context.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.8.8/etl_pipes/pipes/base_pipe.py` & `etl_pipes-0.8.9/etl_pipes/pipes/base_pipe.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.8.8/etl_pipes/pipes/map_reduce.py` & `etl_pipes-0.8.9/etl_pipes/pipes/map_reduce.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.8.8/etl_pipes/pipes/maybe.py` & `etl_pipes-0.8.9/etl_pipes/pipes/maybe.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.8.8/etl_pipes/pipes/parallel.py` & `etl_pipes-0.8.9/etl_pipes/pipes/parallel.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.8.8/etl_pipes/pipes/pipeline/exceptions.py` & `etl_pipes-0.8.9/etl_pipes/pipes/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.8.8/etl_pipes/pipes/pipeline/pipe_welding_validator.py` & `etl_pipes-0.8.9/etl_pipes/pipes/pipeline/pipe_welding_validator.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.8.8/etl_pipes/pipes/pipeline/pipeline.py` & `etl_pipes-0.8.9/etl_pipes/pipes/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `etl_pipes-0.8.8/pyproject.toml` & `etl_pipes-0.8.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "etl-pipes"
-version = "0.8.8"
+version = "0.8.9"
 description = ""
 authors = [ "Tikhon Zaikin <th@thevhs.club>",]
 readme = "README.md"
 
 [tool.ruff]
 select = [ "E", "F", "UP", "W", "I", "N", "PL", "RUF", "PTH",]
```

### Comparing `etl_pipes-0.8.8/PKG-INFO` & `etl_pipes-0.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: etl-pipes
-Version: 0.8.8
+Version: 0.8.9
 Summary: 
 Author: Tikhon Zaikin
 Author-email: th@thevhs.club
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pip (>=23.2,<24.0)
 Description-Content-Type: text/markdown
 
 # Etl-Pipes
 
 ## Description
 
-Pypelines is a Python library for creating flow-based programming pipelines.
+etl-pipes is a Python library for creating flow-based programming pipelines.
 
 ## Primitives
 
 ### Implemented
 
 - Pipeline
   - used to combine pipes into a single sequential pipeline, used to implement "|" operator
```

