# Comparing `tmp/dropbase-0.3.2.tar.gz` & `tmp/dropbase-0.3.3.tar.gz`

## Comparing `dropbase-0.3.2.tar` & `dropbase-0.3.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/__init__.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/constants.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/database/__init__.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/database/connect.py
--rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/database/database.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/database/sources.py
--rw-r--r--   0        0        0    14338 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/database/databases/mysql.py
--rw-r--r--   0        0        0    14547 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/database/databases/postgres.py
--rw-r--r--   0        0        0    15098 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/database/databases/snowflake.py
--rw-r--r--   0        0        0    14519 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/database/databases/sqlite.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/helpers/__init__.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/helpers/dataframe.py
--rw-r--r--   0        0        0     7354 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/helpers/display_rules.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/helpers/utils.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/models/__init__.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/models/category.py
--rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/models/common.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/models/table/__init__.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/models/table/button_column.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/models/table/mysql_column.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/models/table/pg_column.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/models/table/py_column.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/models/table/snowflake_column.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/models/table/sqlite_column.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/models/table/tables.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/models/widget/__init__.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/models/widget/boolean.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/models/widget/button.py
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/models/widget/input.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/models/widget/select.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/models/widget/text.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/models/widget/widgets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/schemas/__init__.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/schemas/columns.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/schemas/database.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/schemas/display_rules.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/schemas/edit_cell.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/schemas/files.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/schemas/function.py
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/schemas/page.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/schemas/query.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/schemas/run_python.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/schemas/table.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/schemas/workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/worker/__init__.py
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/worker/run_python_file.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 dropbase-0.3.2/src/dropbase/worker/run_python_string.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dropbase-0.3.2/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 dropbase-0.3.2/LICENSE
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 dropbase-0.3.2/README.md
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 dropbase-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 dropbase-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/__init__.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/constants.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/database/__init__.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/database/connect.py
+-rw-r--r--   0        0        0     4011 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/database/database.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/database/sources.py
+-rw-r--r--   0        0        0    14338 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/database/databases/mysql.py
+-rw-r--r--   0        0        0    14547 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/database/databases/postgres.py
+-rw-r--r--   0        0        0    15098 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/database/databases/snowflake.py
+-rw-r--r--   0        0        0    14519 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/database/databases/sqlite.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/helpers/__init__.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/helpers/dataframe.py
+-rw-r--r--   0        0        0     7354 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/helpers/display_rules.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/helpers/utils.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/models/__init__.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/models/category.py
+-rw-r--r--   0        0        0     2611 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/models/common.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/models/table/__init__.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/models/table/button_column.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/models/table/mysql_column.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/models/table/pg_column.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/models/table/py_column.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/models/table/snowflake_column.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/models/table/sqlite_column.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/models/table/tables.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/models/widget/__init__.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/models/widget/boolean.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/models/widget/button.py
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/models/widget/input.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/models/widget/select.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/models/widget/text.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/models/widget/widgets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/schemas/__init__.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/schemas/columns.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/schemas/database.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/schemas/display_rules.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/schemas/edit_cell.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/schemas/files.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/schemas/function.py
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/schemas/page.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/schemas/query.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/schemas/run_python.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/schemas/table.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/schemas/workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/worker/__init__.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/worker/run_python_file.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 dropbase-0.3.3/src/dropbase/worker/run_python_string.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dropbase-0.3.3/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 dropbase-0.3.3/LICENSE
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 dropbase-0.3.3/README.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 dropbase-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 dropbase-0.3.3/PKG-INFO
```

### Comparing `dropbase-0.3.2/src/dropbase/database/connect.py` & `dropbase-0.3.3/src/dropbase/database/connect.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/database/database.py` & `dropbase-0.3.3/src/dropbase/database/database.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/database/sources.py` & `dropbase-0.3.3/src/dropbase/database/sources.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/database/databases/mysql.py` & `dropbase-0.3.3/src/dropbase/database/databases/mysql.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/database/databases/postgres.py` & `dropbase-0.3.3/src/dropbase/database/databases/postgres.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/database/databases/snowflake.py` & `dropbase-0.3.3/src/dropbase/database/databases/snowflake.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/database/databases/sqlite.py` & `dropbase-0.3.3/src/dropbase/database/databases/sqlite.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/helpers/dataframe.py` & `dropbase-0.3.3/src/dropbase/helpers/dataframe.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/helpers/display_rules.py` & `dropbase-0.3.3/src/dropbase/helpers/display_rules.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/helpers/utils.py` & `dropbase-0.3.3/src/dropbase/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/models/common.py` & `dropbase-0.3.3/src/dropbase/models/common.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/models/table/button_column.py` & `dropbase-0.3.3/src/dropbase/models/table/button_column.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/models/table/mysql_column.py` & `dropbase-0.3.3/src/dropbase/models/table/mysql_column.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/models/table/pg_column.py` & `dropbase-0.3.3/src/dropbase/models/table/pg_column.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/models/table/snowflake_column.py` & `dropbase-0.3.3/src/dropbase/models/table/snowflake_column.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/models/table/sqlite_column.py` & `dropbase-0.3.3/src/dropbase/models/table/sqlite_column.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/models/table/tables.py` & `dropbase-0.3.3/src/dropbase/models/table/tables.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/models/widget/boolean.py` & `dropbase-0.3.3/src/dropbase/models/widget/boolean.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/models/widget/button.py` & `dropbase-0.3.3/src/dropbase/models/widget/button.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/models/widget/input.py` & `dropbase-0.3.3/src/dropbase/models/widget/input.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/models/widget/select.py` & `dropbase-0.3.3/src/dropbase/models/widget/select.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     data_type: Annotated[
         Literal["string", "integer", "float", "boolean", "string_array"],
         PropertyCategory.default,
     ]
 
     use_fetcher: Annotated[bool, PropertyCategory.default] = False
     options: Annotated[Optional[List[Dict]], PropertyCategory.default]
-    fetcher: Annotated[str, PropertyCategory.default]
-    name_column: Annotated[str, PropertyCategory.default]
-    value_column: Annotated[str, PropertyCategory.default]
+    fetcher: Annotated[Optional[str], PropertyCategory.default]
+    name_column: Annotated[Optional[str], PropertyCategory.default]
+    value_column: Annotated[Optional[str], PropertyCategory.default]
 
     default: Annotated[Optional[Any], PropertyCategory.other]
     multiple: Annotated[Optional[bool], PropertyCategory.other] = False
 
     # events
     on_change: Annotated[Optional[OnEvent], PropertyCategory.events]
```

### Comparing `dropbase-0.3.2/src/dropbase/models/widget/text.py` & `dropbase-0.3.3/src/dropbase/models/widget/text.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/models/widget/widgets.py` & `dropbase-0.3.3/src/dropbase/models/widget/widgets.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/schemas/database.py` & `dropbase-0.3.3/src/dropbase/schemas/database.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/schemas/files.py` & `dropbase-0.3.3/src/dropbase/schemas/files.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/schemas/page.py` & `dropbase-0.3.3/src/dropbase/schemas/page.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/schemas/run_python.py` & `dropbase-0.3.3/src/dropbase/schemas/run_python.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/schemas/table.py` & `dropbase-0.3.3/src/dropbase/schemas/table.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/worker/run_python_file.py` & `dropbase-0.3.3/src/dropbase/worker/run_python_file.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/src/dropbase/worker/run_python_string.py` & `dropbase-0.3.3/src/dropbase/worker/run_python_string.py`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/LICENSE` & `dropbase-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dropbase-0.3.2/pyproject.toml` & `dropbase-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dropbase"
-version = "0.3.2"
+version = "0.3.3"
 authors = [{ name = "Dropbase", email = "support@dropbase.io" }]
 description = "Dropbase"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [
   "sqlalchemy==1.4.46",
   "pymysql==1.1.0",
```

### Comparing `dropbase-0.3.2/PKG-INFO` & `dropbase-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: dropbase
-Version: 0.3.2
+Version: 0.3.3
 Summary: Dropbase
 Project-URL: Homepage, https://github.com/dropbase/dropbase_package
 Project-URL: Bug Tracker, https://github.com/dropbase/dropbase_package/issues
 Author-email: Dropbase <support@dropbase.io>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

