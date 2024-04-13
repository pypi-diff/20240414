# Comparing `tmp/alamos-0.3.4.tar.gz` & `tmp/alamos-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alamos-0.3.4.tar", max compression
+gzip compressed data, was "alamos-0.3.5.tar", max compression
```

## Comparing `alamos-0.3.4.tar` & `alamos-0.3.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2024-04-09 16:43:52.810296 alamos-0.3.4/README.md
--rw-r--r--   0        0        0      493 2024-04-09 16:43:52.810296 alamos-0.3.4/alamos/__init__.py
--rw-r--r--   0        0        0     1240 2024-04-09 16:43:52.810296 alamos-0.3.4/alamos/dev/__init__.py
--rw-r--r--   0        0        0     1221 2024-04-09 16:43:52.810296 alamos-0.3.4/alamos/environment.py
--rw-r--r--   0        0        0     4455 2024-04-09 16:43:52.810296 alamos-0.3.4/alamos/instrumentation.py
--rw-r--r--   0        0        0     1708 2024-04-09 16:43:52.810296 alamos-0.3.4/alamos/log.py
--rw-r--r--   0        0        0     1001 2024-04-09 16:43:52.810296 alamos-0.3.4/alamos/meta.py
--rw-r--r--   0        0        0      988 2024-04-09 16:43:52.810296 alamos-0.3.4/alamos/noop.py
--rw-r--r--   0        0        0     6530 2024-04-09 16:43:52.810296 alamos-0.3.4/alamos/trace.py
--rw-r--r--   0        0        0      613 2024-04-09 16:44:02.938255 alamos-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 alamos-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-13 22:43:59.052286 alamos-0.3.5/README.md
+-rw-r--r--   0        0        0      493 2024-04-13 22:43:59.052286 alamos-0.3.5/alamos/__init__.py
+-rw-r--r--   0        0        0     1240 2024-04-13 22:43:59.052286 alamos-0.3.5/alamos/dev/__init__.py
+-rw-r--r--   0        0        0     1221 2024-04-13 22:43:59.052286 alamos-0.3.5/alamos/environment.py
+-rw-r--r--   0        0        0     4455 2024-04-13 22:43:59.052286 alamos-0.3.5/alamos/instrumentation.py
+-rw-r--r--   0        0        0     1708 2024-04-13 22:43:59.052286 alamos-0.3.5/alamos/log.py
+-rw-r--r--   0        0        0     1001 2024-04-13 22:43:59.052286 alamos-0.3.5/alamos/meta.py
+-rw-r--r--   0        0        0      988 2024-04-13 22:43:59.052286 alamos-0.3.5/alamos/noop.py
+-rw-r--r--   0        0        0     6530 2024-04-13 22:43:59.052286 alamos-0.3.5/alamos/trace.py
+-rw-r--r--   0        0        0      613 2024-04-13 22:44:09.308363 alamos-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 alamos-0.3.5/PKG-INFO
```

### Comparing `alamos-0.3.4/alamos/dev/__init__.py` & `alamos-0.3.5/alamos/dev/__init__.py`

 * *Files identical despite different names*

### Comparing `alamos-0.3.4/alamos/environment.py` & `alamos-0.3.5/alamos/environment.py`

 * *Files identical despite different names*

### Comparing `alamos-0.3.4/alamos/instrumentation.py` & `alamos-0.3.5/alamos/instrumentation.py`

 * *Files identical despite different names*

### Comparing `alamos-0.3.4/alamos/log.py` & `alamos-0.3.5/alamos/log.py`

 * *Files identical despite different names*

### Comparing `alamos-0.3.4/alamos/meta.py` & `alamos-0.3.5/alamos/meta.py`

 * *Files identical despite different names*

### Comparing `alamos-0.3.4/alamos/noop.py` & `alamos-0.3.5/alamos/noop.py`

 * *Files identical despite different names*

### Comparing `alamos-0.3.4/alamos/trace.py` & `alamos-0.3.5/alamos/trace.py`

 * *Files identical despite different names*

### Comparing `alamos-0.3.4/pyproject.toml` & `alamos-0.3.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alamos"
-version = "0.3.4"
+version = "0.3.5"
 description = ""
 authors = ["Emiliano Bonilla <ebonilla@synnaxlabs.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "^1.10.0"
```

### Comparing `alamos-0.3.4/PKG-INFO` & `alamos-0.3.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alamos
-Version: 0.3.4
+Version: 0.3.5
 Summary: 
 Author: Emiliano Bonilla
 Author-email: ebonilla@synnaxlabs.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

