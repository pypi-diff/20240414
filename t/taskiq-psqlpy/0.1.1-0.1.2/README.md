# Comparing `tmp/taskiq_psqlpy-0.1.1.tar.gz` & `tmp/taskiq_psqlpy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_psqlpy-0.1.1.tar", max compression
+gzip compressed data, was "taskiq_psqlpy-0.1.2.tar", max compression
```

## Comparing `taskiq_psqlpy-0.1.1.tar` & `taskiq_psqlpy-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1765 2024-03-26 17:43:08.637277 taskiq_psqlpy-0.1.1/README.md
--rw-r--r--   0        0        0     3698 2024-03-26 17:43:08.637277 taskiq_psqlpy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      103 2024-03-26 17:43:08.637277 taskiq_psqlpy-0.1.1/taskiq_psqlpy/__init__.py
--rw-r--r--   0        0        0      212 2024-03-26 17:43:08.637277 taskiq_psqlpy-0.1.1/taskiq_psqlpy/exceptions.py
--rw-r--r--   0        0        0      492 2024-03-26 17:43:08.637277 taskiq_psqlpy-0.1.1/taskiq_psqlpy/queries.py
--rw-r--r--   0        0        0     4746 2024-03-26 17:43:08.637277 taskiq_psqlpy-0.1.1/taskiq_psqlpy/result_backend.py
--rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 taskiq_psqlpy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1765 2024-04-13 23:21:56.605410 taskiq_psqlpy-0.1.2/README.md
+-rw-r--r--   0        0        0     3698 2024-04-13 23:21:56.605410 taskiq_psqlpy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      103 2024-04-13 23:21:56.605410 taskiq_psqlpy-0.1.2/taskiq_psqlpy/__init__.py
+-rw-r--r--   0        0        0      212 2024-04-13 23:21:56.605410 taskiq_psqlpy-0.1.2/taskiq_psqlpy/exceptions.py
+-rw-r--r--   0        0        0      492 2024-04-13 23:21:56.605410 taskiq_psqlpy-0.1.2/taskiq_psqlpy/queries.py
+-rw-r--r--   0        0        0     4764 2024-04-13 23:21:56.605410 taskiq_psqlpy-0.1.2/taskiq_psqlpy/result_backend.py
+-rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 taskiq_psqlpy-0.1.2/PKG-INFO
```

### Comparing `taskiq_psqlpy-0.1.1/README.md` & `taskiq_psqlpy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `taskiq_psqlpy-0.1.1/pyproject.toml` & `taskiq_psqlpy-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq-psqlpy"
-version = "0.1.1"
+version = "0.1.2"
 description = "PSQLPy and PostgreSQL integration for taskiq"
 authors = ["taskiq-team <taskiq@norely.com>"]
 readme = "README.md"
 packages = [{ include = "taskiq_psqlpy" }]
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -25,15 +25,15 @@
     "postgresql",
     "result_backend",
     "psqlpy",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-psqlpy = "^0.3.3"
+psqlpy = "^0.5.1"
 taskiq = "^0.11.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 pre-commit = "^2.20.0"
 mypy = "^1.1.1"
 flake8 = "^6"
```

### Comparing `taskiq_psqlpy-0.1.1/taskiq_psqlpy/result_backend.py` & `taskiq_psqlpy-0.1.2/taskiq_psqlpy/result_backend.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pickle
 from typing import Any, Final, Literal, Optional, TypeVar, cast
 
-from psqlpy import PSQLPool
+from psqlpy import ConnectionPool
 from psqlpy.exceptions import RustPSQLDriverPyBaseError
 from taskiq import AsyncResultBackend, TaskiqResult
 
 from taskiq_psqlpy.exceptions import ResultIsMissingError
 from taskiq_psqlpy.queries import (
     CREATE_INDEX_QUERY,
     CREATE_TABLE_QUERY,
@@ -29,31 +29,31 @@
         field_for_task_id: Literal["VarChar", "Text"] = "VarChar",
         **connect_kwargs: Any,
     ) -> None:
         """Construct new result backend.
 
         :param dsn: connection string to PostgreSQL.
         :param keep_results: flag to not remove results from Redis after reading.
-        :param connect_kwargs: additional arguments for nats `PSQLPool` class.
+        :param connect_kwargs: additional arguments for nats `ConnectionPool` class.
         """
         self.dsn: Final = dsn
         self.keep_results: Final = keep_results
         self.table_name: Final = table_name
         self.field_for_task_id: Final = field_for_task_id
         self.connect_kwargs: Final = connect_kwargs
 
-        self._database_pool: PSQLPool
+        self._database_pool: ConnectionPool
 
     async def startup(self) -> None:
         """Initialize the result backend.
 
         Construct new connection pool
         and create new table for results if not exists.
         """
-        self._database_pool = PSQLPool(
+        self._database_pool = ConnectionPool(
             dsn=self.dsn,
             **self.connect_kwargs,
         )
         await self._database_pool.execute(
             querystring=CREATE_TABLE_QUERY.format(
                 self.table_name,
                 self.field_for_task_id,
@@ -64,15 +64,15 @@
                 self.table_name,
                 self.table_name,
             ),
         )
 
     async def shutdown(self) -> None:
         """Close the connection pool."""
-        await self._database_pool.close()
+        self._database_pool.close()
 
     async def set_result(
         self,
         task_id: str,
         result: TaskiqResult[_ReturnType],
     ) -> None:
         """Set result to the PostgreSQL table.
```

### Comparing `taskiq_psqlpy-0.1.1/PKG-INFO` & `taskiq_psqlpy-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: taskiq-psqlpy
-Version: 0.1.1
+Version: 0.1.2
 Summary: PSQLPy and PostgreSQL integration for taskiq
 Home-page: https://github.com/taskiq-python/taskiq-psqlpy
 Keywords: taskiq,tasks,distributed,async,postgresql,result_backend,psqlpy
 Author: taskiq-team
 Author-email: taskiq@norely.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: psqlpy (>=0.3.3,<0.4.0)
+Requires-Dist: psqlpy (>=0.5.1,<0.6.0)
 Requires-Dist: taskiq (>=0.11.0,<0.12.0)
 Project-URL: Repository, https://github.com/taskiq-python/taskiq-psqlpy
 Description-Content-Type: text/markdown
 
 # TaskIQ - PSQLPy
 
 TaskIQ-PSQLPy is a plugin for taskiq that adds a new result backend based on PostgreSQL and [PSQLPy](https://github.com/qaspen-python/psqlpy).
```

