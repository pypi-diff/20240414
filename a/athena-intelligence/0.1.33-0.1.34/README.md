# Comparing `tmp/athena_intelligence-0.1.33.tar.gz` & `tmp/athena_intelligence-0.1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athena_intelligence-0.1.33.tar", max compression
+gzip compressed data, was "athena_intelligence-0.1.34.tar", max compression
```

## Comparing `athena_intelligence-0.1.33.tar` & `athena_intelligence-0.1.34.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     4235 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/README.md
--rw-r--r--   0        0        0      435 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/pyproject.toml
--rw-r--r--   0        0        0      905 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/__init__.py
--rw-r--r--   0        0        0     4806 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/base_client.py
--rw-r--r--   0        0        0     3576 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/client.py
--rw-r--r--   0        0        0      790 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/core/api_error.py
--rw-r--r--   0        0        0     1198 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/core/file.py
--rw-r--r--   0        0        0     4882 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/core/request_options.py
--rw-r--r--   0        0        0       65 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/dataset/__init__.py
--rw-r--r--   0        0        0     6087 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/dataset/client.py
--rw-r--r--   0        0        0      165 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/environment.py
--rw-r--r--   0        0        0      170 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0       65 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/message/__init__.py
--rw-r--r--   0        0        0    12185 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/message/client.py
--rw-r--r--   0        0        0     3998 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/polling_message_client.py
--rw-r--r--   0        0        0        0 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/py.typed
--rw-r--r--   0        0        0       65 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/query/__init__.py
--rw-r--r--   0        0        0     6243 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/query/client.py
--rw-r--r--   0        0        0       65 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/report/__init__.py
--rw-r--r--   0        0        0     6528 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/report/client.py
--rw-r--r--   0        0        0       65 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/snippet/__init__.py
--rw-r--r--   0        0        0     6087 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/snippet/client.py
--rw-r--r--   0        0        0      918 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/__init__.py
--rw-r--r--   0        0        0     1014 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/dataset.py
--rw-r--r--   0        0        0      989 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/get_datasets_response.py
--rw-r--r--   0        0        0      989 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/get_snippets_response.py
--rw-r--r--   0        0        0      973 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/http_validation_error.py
--rw-r--r--   0        0        0      865 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/message_out.py
--rw-r--r--   0        0        0     1051 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/message_out_dto.py
--rw-r--r--   0        0        0     2390 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/model.py
--rw-r--r--   0        0        0      946 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/report.py
--rw-r--r--   0        0        0     1126 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/snippet.py
--rw-r--r--   0        0        0      900 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/sql_results.py
--rw-r--r--   0        0        0      672 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/status_enum.py
--rw-r--r--   0        0        0     1277 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/tools.py
--rw-r--r--   0        0        0      992 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-01 14:56:46.668142 athena_intelligence-0.1.33/src/athena/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.33/PKG-INFO
+-rw-r--r--   0        0        0     4235 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/README.md
+-rw-r--r--   0        0        0      435 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/pyproject.toml
+-rw-r--r--   0        0        0      905 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/__init__.py
+-rw-r--r--   0        0        0     4806 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/base_client.py
+-rw-r--r--   0        0        0     3576 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/client.py
+-rw-r--r--   0        0        0      790 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/core/api_error.py
+-rw-r--r--   0        0        0     1198 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/core/file.py
+-rw-r--r--   0        0        0     4882 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/core/http_client.py
+-rw-r--r--   0        0        0     3799 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/core/request_options.py
+-rw-r--r--   0        0        0       65 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/dataset/__init__.py
+-rw-r--r--   0        0        0     6087 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/dataset/client.py
+-rw-r--r--   0        0        0      165 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/environment.py
+-rw-r--r--   0        0        0      170 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0       65 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/message/__init__.py
+-rw-r--r--   0        0        0    12185 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/message/client.py
+-rw-r--r--   0        0        0     3998 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/polling_message_client.py
+-rw-r--r--   0        0        0        0 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/py.typed
+-rw-r--r--   0        0        0       65 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/query/__init__.py
+-rw-r--r--   0        0        0     6243 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/query/client.py
+-rw-r--r--   0        0        0       65 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/report/__init__.py
+-rw-r--r--   0        0        0     6528 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/report/client.py
+-rw-r--r--   0        0        0       65 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/snippet/__init__.py
+-rw-r--r--   0        0        0     6087 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/snippet/client.py
+-rw-r--r--   0        0        0      918 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/types/__init__.py
+-rw-r--r--   0        0        0     1014 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/types/dataset.py
+-rw-r--r--   0        0        0      989 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/types/get_datasets_response.py
+-rw-r--r--   0        0        0      989 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/types/get_snippets_response.py
+-rw-r--r--   0        0        0      973 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/types/http_validation_error.py
+-rw-r--r--   0        0        0      865 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/types/message_out.py
+-rw-r--r--   0        0        0     1051 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/types/message_out_dto.py
+-rw-r--r--   0        0        0     2390 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/types/model.py
+-rw-r--r--   0        0        0      946 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/types/report.py
+-rw-r--r--   0        0        0     1126 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/types/snippet.py
+-rw-r--r--   0        0        0      900 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/types/sql_results.py
+-rw-r--r--   0        0        0      672 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/types/status_enum.py
+-rw-r--r--   0        0        0     1422 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/types/tools.py
+-rw-r--r--   0        0        0      992 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-04-12 21:59:18.626396 athena_intelligence-0.1.34/src/athena/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 athena_intelligence-0.1.34/PKG-INFO
```

### Comparing `athena_intelligence-0.1.33/README.md` & `athena_intelligence-0.1.34/README.md`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/__init__.py` & `athena_intelligence-0.1.34/src/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/base_client.py` & `athena_intelligence-0.1.34/src/athena/base_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/client.py` & `athena_intelligence-0.1.34/src/athena/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/core/__init__.py` & `athena_intelligence-0.1.34/src/athena/core/__init__.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/core/client_wrapper.py` & `athena_intelligence-0.1.34/src/athena/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self.api_key = api_key
         self._base_url = base_url
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "athena-intelligence",
-            "X-Fern-SDK-Version": "0.1.33",
+            "X-Fern-SDK-Version": "0.1.34",
         }
         headers["X-API-KEY"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `athena_intelligence-0.1.33/src/athena/core/datetime_utils.py` & `athena_intelligence-0.1.34/src/athena/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/core/file.py` & `athena_intelligence-0.1.34/src/athena/core/file.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/core/http_client.py` & `athena_intelligence-0.1.34/src/athena/core/http_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/core/jsonable_encoder.py` & `athena_intelligence-0.1.34/src/athena/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/core/request_options.py` & `athena_intelligence-0.1.34/src/athena/core/request_options.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/dataset/client.py` & `athena_intelligence-0.1.34/src/athena/dataset/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/message/client.py` & `athena_intelligence-0.1.34/src/athena/message/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/polling_message_client.py` & `athena_intelligence-0.1.34/src/athena/polling_message_client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/query/client.py` & `athena_intelligence-0.1.34/src/athena/query/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/report/client.py` & `athena_intelligence-0.1.34/src/athena/report/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/snippet/client.py` & `athena_intelligence-0.1.34/src/athena/snippet/client.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/types/__init__.py` & `athena_intelligence-0.1.34/src/athena/types/__init__.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/types/dataset.py` & `athena_intelligence-0.1.34/src/athena/types/dataset.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/types/get_datasets_response.py` & `athena_intelligence-0.1.34/src/athena/types/get_datasets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/types/get_snippets_response.py` & `athena_intelligence-0.1.34/src/athena/types/get_snippets_response.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/types/http_validation_error.py` & `athena_intelligence-0.1.34/src/athena/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/types/message_out.py` & `athena_intelligence-0.1.34/src/athena/types/message_out.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/types/message_out_dto.py` & `athena_intelligence-0.1.34/src/athena/types/message_out_dto.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/types/model.py` & `athena_intelligence-0.1.34/src/athena/types/model.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/types/report.py` & `athena_intelligence-0.1.34/src/athena/types/report.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/types/snippet.py` & `athena_intelligence-0.1.34/src/athena/types/snippet.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/types/sql_results.py` & `athena_intelligence-0.1.34/src/athena/types/sql_results.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/types/status_enum.py` & `athena_intelligence-0.1.34/src/athena/types/status_enum.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/src/athena/types/tools.py` & `athena_intelligence-0.1.34/src/athena/types/tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,34 +9,38 @@
 class Tools(str, enum.Enum):
     """
     An enumeration.
     """
 
     SEARCH = "search"
     BROWSE = "browse"
+    WIKIPEDIA = "wikipedia"
     DATABASE_METADATA = "database_metadata"
     QUERY = "query"
     CHART = "chart"
     ENRICH_PERSON = "enrich_person"
     ENRICH_COMPANY = "enrich_company"
 
     def visit(
         self,
         search: typing.Callable[[], T_Result],
         browse: typing.Callable[[], T_Result],
+        wikipedia: typing.Callable[[], T_Result],
         database_metadata: typing.Callable[[], T_Result],
         query: typing.Callable[[], T_Result],
         chart: typing.Callable[[], T_Result],
         enrich_person: typing.Callable[[], T_Result],
         enrich_company: typing.Callable[[], T_Result],
     ) -> T_Result:
         if self is Tools.SEARCH:
             return search()
         if self is Tools.BROWSE:
             return browse()
+        if self is Tools.WIKIPEDIA:
+            return wikipedia()
         if self is Tools.DATABASE_METADATA:
             return database_metadata()
         if self is Tools.QUERY:
             return query()
         if self is Tools.CHART:
             return chart()
         if self is Tools.ENRICH_PERSON:
```

### Comparing `athena_intelligence-0.1.33/src/athena/types/validation_error.py` & `athena_intelligence-0.1.34/src/athena/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `athena_intelligence-0.1.33/PKG-INFO` & `athena_intelligence-0.1.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athena-intelligence
-Version: 0.1.33
+Version: 0.1.34
 Summary: 
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

