# Comparing `tmp/py_research-4.8.0.tar.gz` & `tmp/py_research-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_research-4.8.0.tar", last modified: Fri Feb  2 15:13:30 2024, max compression
+gzip compressed data, was "py_research-5.0.0.tar", last modified: Sun Apr 14 08:56:25 2024, max compression
```

## Comparing `py_research-4.8.0.tar` & `py_research-5.0.0.tar`

### file list

```diff
@@ -1,42 +1,47 @@
--rw-r--r--   0        0        0     1070 2024-02-02 15:13:24.640784 py_research-4.8.0/LICENSE
--rw-r--r--   0        0        0     3079 2024-02-02 15:13:24.640784 py_research-4.8.0/README.md
--rw-r--r--   0        0        0     2211 2024-02-02 15:13:30.864763 py_research-4.8.0/pyproject.toml
--rw-r--r--   0        0        0       56 2024-02-02 15:13:24.644784 py_research-4.8.0/src/py_research/__init__.py
--rw-r--r--   0        0        0     9277 2024-02-02 15:13:24.644784 py_research-4.8.0/src/py_research/caching.py
--rw-r--r--   0        0        0     3805 2024-02-02 15:13:24.644784 py_research-4.8.0/src/py_research/colors.py
--rw-r--r--   0        0        0     4904 2024-02-02 15:13:24.644784 py_research-4.8.0/src/py_research/data.py
--rw-r--r--   0        0        0      249 2024-02-02 15:13:24.644784 py_research-4.8.0/src/py_research/db/__init__.py
--rw-r--r--   0        0        0    53189 2024-02-02 15:13:24.644784 py_research-4.8.0/src/py_research/db/base.py
--rw-r--r--   0        0        0      799 2024-02-02 15:13:24.644784 py_research-4.8.0/src/py_research/db/conflicts.py
--rw-r--r--   0        0        0    16309 2024-02-02 15:13:24.644784 py_research-4.8.0/src/py_research/db/importing.py
--rw-r--r--   0        0        0      432 2024-02-02 15:13:24.644784 py_research-4.8.0/src/py_research/enums.py
--rw-r--r--   0        0        0      613 2024-02-02 15:13:24.644784 py_research-4.8.0/src/py_research/files.py
--rw-r--r--   0        0        0    14046 2024-02-02 15:13:24.644784 py_research-4.8.0/src/py_research/geo.py
--rw-r--r--   0        0        0     2658 2024-02-02 15:13:24.644784 py_research-4.8.0/src/py_research/hashing.py
--rw-r--r--   0        0        0    28664 2024-02-02 15:13:24.644784 py_research-4.8.0/src/py_research/intl.py
--rw-r--r--   0        0        0    10319 2024-02-02 15:13:24.644784 py_research-4.8.0/src/py_research/plots/__init__.py
--rw-r--r--   0        0        0     1986 2024-02-02 15:13:24.644784 py_research-4.8.0/src/py_research/plots/responsive_plotly.js
--rw-r--r--   0        0        0     4778 2024-02-02 15:13:24.644784 py_research-4.8.0/src/py_research/ranking.py
--rw-r--r--   0        0        0    18055 2024-02-02 15:13:24.644784 py_research-4.8.0/src/py_research/reflect.py
--rw-r--r--   0        0        0    23613 2024-02-02 15:13:24.644784 py_research-4.8.0/src/py_research/sql.py
--rw-r--r--   0        0        0     2907 2024-02-02 15:13:24.644784 py_research-4.8.0/src/py_research/stats.py
--rw-r--r--   0        0        0    23075 2024-02-02 15:13:24.644784 py_research-4.8.0/src/py_research/tables.py
--rw-r--r--   0        0        0     7502 2024-02-02 15:13:24.644784 py_research-4.8.0/src/py_research/telemetry.py
--rw-r--r--   0        0        0     4955 2024-02-02 15:13:24.644784 py_research-4.8.0/src/py_research/time.py
--rw-r--r--   0        0        0     2421 2024-02-02 15:13:24.644784 py_research-4.8.0/tests/py_research/test_caching.py
--rw-r--r--   0        0        0      588 2024-02-02 15:13:24.644784 py_research-4.8.0/tests/py_research/test_colors.py
--rw-r--r--   0        0        0    18077 2024-02-02 15:13:24.644784 py_research-4.8.0/tests/py_research/test_db_base.py
--rw-r--r--   0        0        0     6692 2024-02-02 15:13:24.644784 py_research-4.8.0/tests/py_research/test_db_importing.py
--rw-r--r--   0        0        0      348 2024-02-02 15:13:24.644784 py_research-4.8.0/tests/py_research/test_enums.py
--rw-r--r--   0        0        0      950 2024-02-02 15:13:24.644784 py_research-4.8.0/tests/py_research/test_files.py
--rw-r--r--   0        0        0     6106 2024-02-02 15:13:24.644784 py_research-4.8.0/tests/py_research/test_geo.py
--rw-r--r--   0        0        0      717 2024-02-02 15:13:24.644784 py_research-4.8.0/tests/py_research/test_hashing.py
--rw-r--r--   0        0        0     3754 2024-02-02 15:13:24.644784 py_research-4.8.0/tests/py_research/test_intl.py
--rw-r--r--   0        0        0     1380 2024-02-02 15:13:24.644784 py_research-4.8.0/tests/py_research/test_plots.py
--rw-r--r--   0        0        0     3130 2024-02-02 15:13:24.644784 py_research-4.8.0/tests/py_research/test_ranking.py
--rw-r--r--   0        0        0      847 2024-02-02 15:13:24.644784 py_research-4.8.0/tests/py_research/test_reflect.py
--rw-r--r--   0        0        0     2374 2024-02-02 15:13:24.644784 py_research-4.8.0/tests/py_research/test_stats.py
--rw-r--r--   0        0        0     4444 2024-02-02 15:13:24.648784 py_research-4.8.0/tests/py_research/test_tables.py
--rw-r--r--   0        0        0      319 2024-02-02 15:13:24.648784 py_research-4.8.0/tests/py_research/test_telemetry.py
--rw-r--r--   0        0        0      625 2024-02-02 15:13:24.648784 py_research-4.8.0/tests/py_research/test_time.py
--rw-r--r--   0        0        0     4391 1970-01-01 00:00:00.000000 py_research-4.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-14 08:56:22.218037 py_research-5.0.0/LICENSE
+-rw-r--r--   0        0        0     3079 2024-04-14 08:56:22.218037 py_research-5.0.0/README.md
+-rw-r--r--   0        0        0     2290 2024-04-14 08:56:25.026020 py_research-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0       56 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/__init__.py
+-rw-r--r--   0        0        0     9849 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/caching.py
+-rw-r--r--   0        0        0     3805 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/colors.py
+-rw-r--r--   0        0        0     4904 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/data.py
+-rw-r--r--   0        0        0      249 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/db/__init__.py
+-rw-r--r--   0        0        0    53926 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/db/base.py
+-rw-r--r--   0        0        0      799 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/db/conflicts.py
+-rw-r--r--   0        0        0    16309 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/db/importing.py
+-rw-r--r--   0        0        0      432 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/enums.py
+-rw-r--r--   0        0        0      613 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/files.py
+-rw-r--r--   0        0        0    14046 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/geo.py
+-rw-r--r--   0        0        0     2658 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/hashing.py
+-rw-r--r--   0        0        0    28664 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/intl.py
+-rw-r--r--   0        0        0    10319 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/plots/__init__.py
+-rw-r--r--   0        0        0     1986 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/plots/responsive_plotly.js
+-rw-r--r--   0        0        0     4778 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/ranking.py
+-rw-r--r--   0        0        0       40 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/reflect/__init__.py
+-rw-r--r--   0        0        0     5689 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/reflect/deps.py
+-rw-r--r--   0        0        0     3720 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/reflect/dist.py
+-rw-r--r--   0        0        0     1852 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/reflect/env.py
+-rw-r--r--   0        0        0     8354 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/reflect/ref.py
+-rw-r--r--   0        0        0     1735 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/reflect/runtime.py
+-rw-r--r--   0        0        0    23621 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/sql.py
+-rw-r--r--   0        0        0     4539 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/stats.py
+-rw-r--r--   0        0        0    23444 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/tables.py
+-rw-r--r--   0        0        0     7541 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/telemetry.py
+-rw-r--r--   0        0        0     4955 2024-04-14 08:56:22.222037 py_research-5.0.0/src/py_research/time.py
+-rw-r--r--   0        0        0     2421 2024-04-14 08:56:22.222037 py_research-5.0.0/tests/py_research/test_caching.py
+-rw-r--r--   0        0        0      588 2024-04-14 08:56:22.222037 py_research-5.0.0/tests/py_research/test_colors.py
+-rw-r--r--   0        0        0    18077 2024-04-14 08:56:22.226037 py_research-5.0.0/tests/py_research/test_db_base.py
+-rw-r--r--   0        0        0     6692 2024-04-14 08:56:22.226037 py_research-5.0.0/tests/py_research/test_db_importing.py
+-rw-r--r--   0        0        0      348 2024-04-14 08:56:22.226037 py_research-5.0.0/tests/py_research/test_enums.py
+-rw-r--r--   0        0        0      950 2024-04-14 08:56:22.226037 py_research-5.0.0/tests/py_research/test_files.py
+-rw-r--r--   0        0        0     6106 2024-04-14 08:56:22.226037 py_research-5.0.0/tests/py_research/test_geo.py
+-rw-r--r--   0        0        0      717 2024-04-14 08:56:22.226037 py_research-5.0.0/tests/py_research/test_hashing.py
+-rw-r--r--   0        0        0     3754 2024-04-14 08:56:22.226037 py_research-5.0.0/tests/py_research/test_intl.py
+-rw-r--r--   0        0        0     1376 2024-04-14 08:56:22.226037 py_research-5.0.0/tests/py_research/test_plots.py
+-rw-r--r--   0        0        0     3130 2024-04-14 08:56:22.226037 py_research-5.0.0/tests/py_research/test_ranking.py
+-rw-r--r--   0        0        0     1250 2024-04-14 08:56:22.226037 py_research-5.0.0/tests/py_research/test_reflect.py
+-rw-r--r--   0        0        0     2374 2024-04-14 08:56:22.226037 py_research-5.0.0/tests/py_research/test_stats.py
+-rw-r--r--   0        0        0     4501 2024-04-14 08:56:22.226037 py_research-5.0.0/tests/py_research/test_tables.py
+-rw-r--r--   0        0        0      319 2024-04-14 08:56:22.226037 py_research-5.0.0/tests/py_research/test_telemetry.py
+-rw-r--r--   0        0        0      625 2024-04-14 08:56:22.226037 py_research-5.0.0/tests/py_research/test_time.py
+-rw-r--r--   0        0        0     4493 1970-01-01 00:00:00.000000 py_research-5.0.0/PKG-INFO
```

### Comparing `py_research-4.8.0/LICENSE` & `py_research-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/README.md` & `py_research-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/pyproject.toml` & `py_research-5.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -30,31 +30,34 @@
     "pandas-stubs>=2.1.4.231227",
     "packaging>=23.2",
     "requests>=2.31.0",
     "pydantic-core>=2.14.6",
     "notebook>=7.0.6",
     "ipywidgets>=8.1.1",
     "ipython>=8.21.0",
+    "sphinx>=7.2.6",
 ]
 name = "py-research"
 description = "Collection of utilities for R&D coding in Python 🐍"
 readme = "README.md"
-version = "4.8.0"
+version = "5.0.0"
+
+[project.urls]
+Documentation = "https://cloudlane-one.github.io/py-research/"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "black>=24",
     "pytest>=7.4.3",
-    "sphinx>=7.2.6",
     "pygments>=2.17.2",
     "nbsphinx>=0.9.3",
     "myst-parser>=2.0.0",
     "pydata-sphinx-theme>=0.14.4",
     "autodoc-pydantic>=1.9.0",
     "deptry>=0.12.0",
     "ruff>=0.1.7",
```

### Comparing `py_research-4.8.0/src/py_research/caching.py` & `py_research-5.0.0/src/py_research/caching.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,24 +3,28 @@
 import datetime
 import json
 import pickle
 from collections.abc import Callable
 from dataclasses import dataclass
 from functools import wraps
 from pathlib import Path
-from typing import Any, ParamSpec, TypeVar, cast
+from typing import Any, ParamSpec, TypeVar, cast, overload
 
 import numpy as np
 import pandas as pd
 import yaml
 from bs4 import BeautifulSoup, Tag
 
 from py_research.data import gen_id
 from py_research.files import ensure_dir_exists
-from py_research.reflect import get_calling_module, get_full_args_dict, get_return_type
+from py_research.reflect.runtime import (
+    get_calling_module,
+    get_full_args_dict,
+    get_return_type,
+)
 from py_research.telemetry import get_logger
 
 log = get_logger()
 
 default_root_path = Path.cwd() / ".cache"
 
 
@@ -50,24 +54,40 @@
     def __filter_outdated(self, f: Path):
         if self.__get_date_from_filename(f) > self.__earliest_date:
             return True
         else:
             f.unlink()
             return False
 
+    @overload
+    def function(self, func: Callable[P, R]) -> Callable[P, R]: ...
+
+    @overload
+    def function(
+        self,
+        *,
+        id_arg_subset: list[int] | list[str] | None = None,
+        use_raw_arg: bool = False,
+        id_callback: Callable[P, dict[str, Any] | None] | None = None,
+        use_json: bool = True,
+    ) -> Callable[[Callable[P, R]], Callable[P, R]]: ...
+
     def function(  # noqa: C901
         self,
+        func: Callable[P, R] | None = None,
+        *,
         id_arg_subset: list[int] | list[str] | None = None,
         use_raw_arg: bool = False,
         id_callback: Callable[P, dict[str, Any] | None] | None = None,
         use_json: bool = True,
-    ) -> Callable[[Callable[P, R]], Callable[P, R]]:
+    ) -> Callable[P, R] | Callable[[Callable[P, R]], Callable[P, R]]:
         """Decorator to cache wrapped function.
 
         Args:
+            func: Function to cache.
             id_arg_subset:
                 Number or name of the arguments to base hash id of result on.
             use_raw_arg:
                 If ``True``, use the unhashed, string-formatted value of the id arg
                 as filename. Only works for single id arg.
             id_callback:
                 Callback function to use for retrieving a unique id from the arguments.
@@ -211,15 +231,15 @@
                                 ),
                             )
 
                 return result
 
             return inner_inner
 
-        return inner
+        return inner if func is None else inner(func)
 
 
 def get_cache(
     name: str | None = None,
     root_path: Path | None = None,
     max_cache_time: datetime.timedelta = datetime.timedelta(days=7),
 ):
```

### Comparing `py_research-4.8.0/src/py_research/colors.py` & `py_research-5.0.0/src/py_research/colors.py`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/src/py_research/data.py` & `py_research-5.0.0/src/py_research/data.py`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/src/py_research/db/base.py` & `py_research-5.0.0/src/py_research/db/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from functools import reduce
 from pathlib import Path
 from typing import Any, Literal, cast, overload
 
 import pandas as pd
 
 from py_research.data import parse_dtype
-from py_research.reflect import PyObjectRef
+from py_research.reflect.ref import PyObjectRef
 
 from .conflicts import DataConflictError, DataConflictPolicy
 
 
 def _unmerge(df: pd.DataFrame) -> dict[str, pd.DataFrame]:
     """Extract this table into its own database.
 
@@ -890,19 +890,36 @@
                 f" x {n_attrs} attributes"
                 if (n_attrs := len(self[name].columns) - 2) > 0
                 else ""
             )
             for name in self.join_tables
         }
 
-        schema_desc = (
-            {"schema": PyObjectRef.reference(self.schema).to_url()}
-            if self.schema is not None
-            else {}
-        )
+        schema_desc = {}
+        if self.schema is not None:
+            schema_ref = PyObjectRef.reference(self.schema)
+
+            schema_desc = {
+                "schema": {
+                    "repo": schema_ref.repo,
+                    "package": schema_ref.package,
+                    "class": f"{schema_ref.module}.{schema_ref.object}",
+                }
+            }
+
+            if schema_ref.object_version is not None:
+                schema_desc["schema"]["version"] = schema_ref.object_version
+            elif schema_ref.package_version is not None:
+                schema_desc["schema"]["version"] = schema_ref.package_version
+
+            if schema_ref.repo_revision is not None:
+                schema_desc["schema"]["revision"] = schema_ref.repo_revision
+
+            if schema_ref.docs_url is not None:
+                schema_desc["schema"]["docs"] = schema_ref.docs_url
 
         return {
             **schema_desc,
             "tables": {
                 name: f"{len(df)} objects x {len(df.columns)} attributes"
                 for name, df in self.items()
                 if name not in join_tables
```

### Comparing `py_research-4.8.0/src/py_research/db/conflicts.py` & `py_research-5.0.0/src/py_research/db/conflicts.py`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/src/py_research/db/importing.py` & `py_research-5.0.0/src/py_research/db/importing.py`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/src/py_research/files.py` & `py_research-5.0.0/src/py_research/files.py`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/src/py_research/geo.py` & `py_research-5.0.0/src/py_research/geo.py`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/src/py_research/hashing.py` & `py_research-5.0.0/src/py_research/hashing.py`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/src/py_research/intl.py` & `py_research-5.0.0/src/py_research/intl.py`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/src/py_research/plots/__init__.py` & `py_research-5.0.0/src/py_research/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/src/py_research/plots/responsive_plotly.js` & `py_research-5.0.0/src/py_research/plots/responsive_plotly.js`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/src/py_research/ranking.py` & `py_research-5.0.0/src/py_research/ranking.py`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/src/py_research/sql.py` & `py_research-5.0.0/src/py_research/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     is_integer_dtype,
     is_numeric_dtype,
     is_string_dtype,
 )
 from pandas.util import hash_pandas_object
 from typing_extensions import Self
 
-from py_research.reflect import get_all_subclasses
+from py_research.reflect.runtime import get_all_subclasses
 
 
 def _hash_df(df: pd.DataFrame | pd.Series) -> str:
     return hex(abs(sum(hash_pandas_object(df))))[2:12]
 
 
 Params = ParamSpec("Params")
```

### Comparing `py_research-4.8.0/src/py_research/stats.py` & `py_research-5.0.0/src/py_research/stats.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,48 +2,96 @@
 
 from collections.abc import Hashable
 
 import numpy as np
 import pandas as pd
 
 
+def _union_children_on_parents(
+    df: pd.DataFrame, name_col: str, parent_col: str
+) -> pd.DataFrame:
+    """Add union of all their children's ids to each parent node, recursively."""
+    tree = df[[name_col, parent_col]].drop_duplicates()
+
+    child_ids = df
+    for _ in range(20):
+        df = (
+            pd.concat(
+                [
+                    df,
+                    (
+                        child_ids.drop(columns=[name_col])
+                        .rename(columns={parent_col: name_col})
+                        .merge(tree, on=name_col, how="left")
+                    ),
+                ]
+            )
+            .drop_duplicates()
+            .dropna(subset=[name_col])
+        )
+
+        child_ids = df.loc[df[name_col].isin(child_ids[parent_col].dropna().unique())]
+        if child_ids.empty:
+            break
+
+    return df
+
+
 def dist_table(
     df: pd.DataFrame,
     category_cols: str | list[str],
     id_cols: str | list[str] | None = None,
     value_col: str | None = None,
     domains: dict[str, list[Hashable] | np.ndarray | pd.Index] = {},
+    category_parent_cols: str | dict[str, str] | None = None,
 ) -> pd.Series:
     """Return a frequency table of the distribution of unique entities.
 
     Entities are identified by ``id_cols``. Distribution is presented over
     unique categories in ``category_cols``.
 
     Args:
         df: Dataframe to evaluate.
         category_cols: Columns to evaluate distribution over.
         id_cols: Columns to identify entities by.
         value_col: Unique values per entity to sum up.
         domains:
             Force the distribution to be evaluated over these domains,
             filling missing values with 0.
+        category_parent_cols:
+            If category values are discrete and hierarchical, you may supply
+            a parent column for each category column. This will be used to
+            aggregate the distribution over the parent categories.
 
     Returns:
         Series of the distribution's values (count or sum) given the categories
         in the index.
     """
     id_cols = (
         [id_cols]
         if isinstance(id_cols, str)
         else id_cols if id_cols is not None else [n or "index" for n in df.index.names]
     )
     category_cols = [
         *([category_cols] if isinstance(category_cols, str) else category_cols)
     ]
 
+    if category_parent_cols is not None:
+        category_parent_cols = (
+            category_parent_cols
+            if isinstance(category_parent_cols, dict)
+            else {category_cols[0]: category_parent_cols}
+        )
+        df = pd.concat(
+            [
+                _union_children_on_parents(df, name_col=col, parent_col=parent_col)
+                for col, parent_col in category_parent_cols.items()
+            ]
+        ).drop_duplicates()
+
     counts = (
         df.reset_index()[
             [*category_cols, *id_cols, *([value_col] if value_col else [])]
         ]
         .groupby(by=category_cols, group_keys=True)
         .apply(
             lambda df: (
```

### Comparing `py_research-4.8.0/src/py_research/tables.py` & `py_research-5.0.0/src/py_research/tables.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Utilities for creating pretty result tables."""
 
 from collections.abc import Callable
 from dataclasses import InitVar, dataclass, field
 from functools import reduce
+from itertools import product
 from pathlib import Path
 from typing import Any, Literal, TextIO, cast
 
 import imgkit
 import pandas as pd
 import pdfkit
 from pandas.api.types import is_float_dtype, is_integer_dtype, is_numeric_dtype
@@ -14,45 +15,49 @@
 from typing_extensions import deprecated
 
 
 @dataclass
 class TableStyle:
     """Define a pretty table column format."""
 
-    cols: str | tuple[str, str] | list[str | tuple[str, str]] | None = None
-    """Column(s) to apply this style to. If None, apply to all columns.
+    dfs: str | list[str] | None = None
+    """Dataframe names to apply this style to. If None, apply to all dataframes."""
+
+    cols: str | list[str] | None = None
+    """Column name(s) to apply this style to. If None, apply to all columns.
     Index levels can be styled via their names as if they were columns.
     """
 
     rows: pd.Series | None = None
     """Rows to apply this style to. If None, apply to all rows."""
 
     name: str | None = None
     """Name of this style"""
 
-    str_format: str | Callable[[Any], str] | None = None
-    """Format string or callback function to use for formatting numerical values"""
-
-    alignment: Literal["left", "center", "right"] | None = None
-    """How to align the columns' text"""
+    format: str | Callable[[Any], str] | None = None
+    """Format string or callback function to use for formatting data values"""
 
     css: dict[str, str] | Callable[[Any], str] | None = None
-    """Custom CSS styles to apply to matched cells"""
+    """Custom CSS styles to apply to matched cells.
+    Supplied as a mapping from CSS property to value.
+    """
 
-    hide_headers: bool | None = None
-    """Whether to hide headers of given ``cols``."""
+    header_css: dict[str, str] | None = None
+    """Custom CSS styles applied to the headers of matched cells.
+    Supplied as a mapping from CSS property to value.
+    """
 
-    hide_rows: bool | None = None
-    """Whether to hide cols/rows if matched by this selection."""
+    hide: Literal["headers", "rows", "cols", "cells"] | None = None
+    """Whether to hide headers, rows, columns or cells matched by this style"""
 
-    filter_inclusive: bool | None = None
-    """Whether to show cols/rows if matched by this selection."""
+    include: bool | None = None
+    """Whether to show rows if matched by this selection."""
 
-    filter_exclusive: bool | None = None
-    """Whether to only show cols/rows if matched by this selection."""
+    require: bool | None = None
+    """Whether to only show rows if matched by this selection."""
 
 
 @dataclass
 class TableColors:
     """Define colors for a pretty table."""
 
     row_even: str = "#f2f2f2"
@@ -91,78 +96,80 @@
     If a float, the width is relative to the sum of all widths.
     If a string, the width is set to the CSS string value.
     """
 
     title: str | None = None
     """Title of the table."""
 
-    hide_index: bool | list[str] = True
-    """Whether to hide the index columns."""
-
     max_row_cutoff: int = 100
     """Maximum number of rows to render."""
 
     font_size: float = 1.0
     """Default font size to use for the table."""
 
     default_style: TableStyle = field(default_factory=TableStyle)
     """Default style to apply to the table."""
 
     column_flatten_format: str | None = None
     """Format string to use for flatteting multi-index column labels.
-    Leave as None to keep multi-index column labels as tuples.
+    Leave as None to keep a multi-level column header.
     Format string must take two positional arguments, e.g. "{0}_{1}".
     """
 
+    show_index: bool = False
+    """Whether to show the index as the first columns of the styled table."""
+
     table_colors: TableColors = field(default_factory=TableColors)
     """Colors to use for this table."""
 
-    table_styles: dict[str, dict[str, str]] = field(default_factory=dict)
+    table_css: dict[str, dict[str, str]] = field(default_factory=dict)
     """Additional styles to apply to the table.
     Dictionary keys must be CSS selectors and
     values must be dictionaries of CSS properties.
     """
 
     def __post_init__(self, df: pd.DataFrame):  # noqa: D105
-        if self.hide_index is not True:
-            hidden_indexes = (
-                self.hide_index if isinstance(self.hide_index, list) else []
-            )
-            index_names = (
-                df.index.names
-                if all(df.index.names)
-                else [f"index_{i}" for i in range(df.index.nlevels)]
-            )
+        if not self.show_index:
+            self.data = df
+            return
 
-            df = df.rename_axis(index=index_names)
+        index_names = (
+            df.index.names
+            if all(df.index.names)
+            else [f"index_{i}" for i in range(df.index.nlevels)]
+        )
 
-            index_col_names = [
-                name for name in index_names if name not in hidden_indexes
-            ]
-            if df.columns.nlevels > 1:
-                index_col_names = [("", name) for name in index_col_names]
+        df = df.rename_axis(index=index_names)
 
-            df = df.copy()
-            for col_name in index_col_names:
-                index_name = col_name if isinstance(col_name, str) else col_name[1]
-                df[col_name] = df.index.get_level_values(index_name)
+        index_col_names = [name for name in index_names]
+        if df.columns.nlevels > 1:
+            index_col_names = [("", name) for name in index_col_names]
+
+        df = df.copy()
+        for col_name in index_col_names:
+            index_name = col_name if isinstance(col_name, str) else col_name[1]
+            df[col_name] = df.index.get_level_values(index_name)
 
-            self.data = df[
-                [*index_col_names, *[c for c in df.columns if c not in index_col_names]]
-            ]
-        else:
-            self.data = df
+        self.data = df[
+            [*index_col_names, *[c for c in df.columns if c not in index_col_names]]
+        ]
 
     @property
-    def __hidden_headers(self) -> set[str | tuple[str, str]]:
+    def _hidden_headers(self) -> set[tuple[str | None, str]]:
         hide_styles = [
-            set([style.cols] if isinstance(style.cols, str) else style.cols)
+            set(
+                product(
+                    style.dfs if isinstance(style.dfs, list) else [style.dfs],
+                    style.cols if isinstance(style.cols, list) else [style.cols],
+                )
+            )
             for style in self.styles
-            if style.cols is not None and style.hide_headers is True
+            if style.cols is not None and style.hide == "headers"
         ]
+
         return (
             reduce(
                 lambda x, y: x | y,
                 hide_styles,
             )
             if len(hide_styles) > 0
             else set()
@@ -192,29 +199,29 @@
             )
             for h in self.styles
         ]
 
         exclusive_h = [
             (h, css)
             for h, css in highlights
-            if h.name is not None and css is not None and h.filter_exclusive
+            if h.name is not None and css is not None and h.require
         ]
         inclusive_h = [
             (h, css)
             for h, css in highlights
-            if h.name is not None and css is not None and h.filter_inclusive
+            if h.name is not None and css is not None and h.include
         ]
         highlight_h = [
             (h, css)
             for h, css in highlights
             if h.name is not None
             and css is not None
-            and not any([h.filter_exclusive, h.filter_inclusive, h.hide_rows])
+            and not any([h.require, h.include, h.hide in ["rows", "cells"]])
         ]
-        hide_h = [h for h, _ in highlights if h.name is not None and h.hide_rows]
+        hide_h = [h for h, _ in highlights if h.name is not None and h.hide is not None]
 
         desc = "\n".join(
             [
                 (
                     f"""<h2>Show rows where all of:</h2>
             <ul>
                 {
@@ -274,21 +281,21 @@
                 }
             </ul>
             """
                     if len(highlight_h) > 0
                     else ""
                 ),
                 (
-                    f"""<h2>Hide rows where any of:</h2>
+                    f"""<h2>Hide:</h2>
             <ul>
                 {
                     ''.join(
                         [
                             '<li style="margin-bottom: 0.5rem;">'
-                            + f'{h.name}'
+                            + f'{h.hide} where {h.name}'
                             + '</li>'
                             for h in hide_h
                         ]
                     )
                 }
             </ul>
             """
@@ -311,17 +318,15 @@
             </body>
         </html>
         """
             if full_doc
             else desc
         )
 
-    def _get_cols_by_second_level(
-        self, cols: list[str | tuple[str, str]]
-    ) -> list[tuple[str, str]]:
+    def _get_cols_by_second_level(self, cols: list[str]) -> list[tuple[str, str]]:
         return [
             cast(tuple[str, str], cc)
             for c in cols
             for cc in self.data.columns
             if (isinstance(c, str) and cc[1] == c) or cc == c
         ]
 
@@ -428,15 +433,15 @@
                                 + ": "
                                 + prop_value.rstrip(" ").rstrip(";")
                                 + " !important;"
                                 for prop_name, prop_value in props.items()
                             ]
                         ),
                     }
-                    for selector, props in self.table_styles.items()
+                    for selector, props in self.table_css.items()
                 ),
             ]
         ).format(na_rep="")
 
     def _apply_default_style(self, styled: Styler) -> Styler:
         if isinstance(self.default_style.css, dict):
             styled = styled.set_properties(
@@ -451,25 +456,31 @@
         return styled
 
     def _apply_col_defaults(self, styled: Styler) -> Styler:
         res = styled
         for col in self.data.columns:
             res = res.set_properties(
                 subset=[self._to_styler_col(col)],
-                **{
-                    "text-align": self.default_style.alignment
-                    or self._default_alignment(col)
-                },
+                **{"text-align": self._default_alignment(col)},
             )
+
             res = res.format(
                 subset=[self._to_styler_col(col)],
-                formatter=self.default_style.str_format
-                or self._default_str_format(col),
+                formatter=self.default_style.format or self._default_str_format(col),
             )
 
+            if isinstance(self.default_style.css, dict):
+                res = res.set_properties(
+                    subset=[self._to_styler_col(col)], **self.default_style.css
+                )
+            elif isinstance(self.default_style.css, Callable):
+                res = res.applymap(
+                    self.default_style.css, subset=[self._to_styler_col(col)]
+                )
+
         return res
 
     def _apply_styles(self, styled: Styler) -> Styler:
         for style in self.styles:
             rows, cols = (
                 style.rows if style.rows is not None else slice(None),
                 (
@@ -482,53 +493,53 @@
             if isinstance(cols, list) and self.data.columns.nlevels > 1:
                 cols = [
                     self._to_styler_col(c) for c in self._get_cols_by_second_level(cols)
                 ]
 
             subset = (rows, cols)
 
-            if style.hide_rows is not None:
-                styled = styled.hide(
-                    subset[0],  # type: ignore
-                    axis="index",
-                )
+            if style.hide is not None:
+                if style.hide in ["rows", "cells"]:
+                    styled = styled.hide(
+                        subset[0],  # type: ignore
+                        axis="index",
+                    )
+                if style.hide in ["cols", "cells"]:
+                    styled = styled.hide(
+                        subset[1],  # type: ignore
+                        axis="columns",
+                    )
                 continue
 
-            if style.alignment is not None:
-                styled = styled.set_properties(
-                    subset=subset,  # type: ignore
-                    **{"text-align": style.alignment},
-                )
-
             if isinstance(style.css, dict):
                 styled = styled.set_properties(
                     subset=subset,  # type: ignore
                     **style.css,
                 )
             elif isinstance(style.css, Callable):
                 styled = styled.applymap(
                     subset=subset,  # type: ignore
                     func=style.css,
                 )
 
-            if style.str_format is not None:
+            if style.format is not None:
                 styled = styled.format(
                     subset=subset,  # type: ignore
                     formatter=(
-                        f"{{:{style.str_format}}}"
-                        if isinstance(style.str_format, str)
-                        else style.str_format
+                        f"{{:{style.format}}}"
+                        if isinstance(style.format, str)
+                        else style.format
                     ),
                 )
 
         return styled
 
-    def __apply_widths(self, styled: Styler) -> Styler:
+    def _apply_widths(self, styled: Styler) -> Styler:
         widths = {
-            c: (self.widths.get(c if self.data.columns.nlevels == 1 else c[1]) or 1)
+            c: (self.widths.get(c if isinstance(c, str) else c[1]) or 1)
             for c in self.data.columns
         }
         width_sum = sum(w for w in widths.values() if isinstance(w, int | float))
         for col, width in widths.items():
             styled = styled.set_properties(
                 subset=(slice(None), [self._to_styler_col(col)]),  # type: ignore
                 width=(
@@ -536,26 +547,26 @@
                     if isinstance(width, int | float)
                     else width
                 ),
             )
 
         return styled
 
-    def __apply_labels(self, styled: Styler) -> Styler:
+    def _apply_labels(self, styled: Styler) -> Styler:
         label_func = self.labels.get if isinstance(self.labels, dict) else self.labels
         labels = (
             {
-                c: "" if c in self.__hidden_headers else label_func(c) or c
+                c: "" if (None, c) in self._hidden_headers else label_func(c) or c
                 for c in self.data.columns
             }
             if self.data.columns.nlevels == 1
             else {
                 c: (
                     ("", "")
-                    if c[1] in self.__hidden_headers
+                    if c in self._hidden_headers or (None, c[1]) in self._hidden_headers
                     else (
                         (c[0], label_func(c[1]) or c[1])
                         if c[1]
                         else ("", label_func(c[0]) or c[0])
                     )
                 )
                 for c in self.data.columns
@@ -583,32 +594,32 @@
 
         if self.column_flatten_format is not None and self.data.columns.nlevels > 1:
             data.columns = [self.column_flatten_format.format(*c) for c in data.columns]
 
         incl_filters = [
             style.rows
             for style in self.styles
-            if style.filter_inclusive is True and style.rows is not None
+            if style.include is True and style.rows is not None
         ]
         if len(incl_filters) > 0:
             data = data.loc[reduce(lambda x, y: x | y, incl_filters)]
 
         excl_filters = [
             style.rows
             for style in self.styles
-            if style.filter_exclusive is True and style.rows is not None
+            if style.require is True and style.rows is not None
         ]
         if len(excl_filters) > 0:
             data = data.loc[reduce(lambda x, y: x & y, excl_filters)]
 
         styled = self._prettify_df(data.iloc[: self.max_row_cutoff], self.font_size)
         styled = self._apply_default_style(styled)
         styled = self._apply_col_defaults(styled)
-        styled = self.__apply_widths(styled)
-        styled = self.__apply_labels(styled)
+        styled = self._apply_widths(styled)
+        styled = self._apply_labels(styled)
         styled = self._apply_styles(styled)
 
         if self.title is not None:
             styled = styled.set_caption(self.title)
 
         styled = styled.hide(axis="index")
```

### Comparing `py_research-4.8.0/src/py_research/telemetry.py` & `py_research-5.0.0/src/py_research/telemetry.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         super().__init__(*args, **kwargs)
 
     def emit(self, record):  # noqa: D102
         try:
             msg = self.format(record)
 
             if self.tqdm is not None:
-                self.tqdm.set_postfix_str(msg)
+                self.tqdm.set_postfix_str(f"{msg[:50]}..." if len(msg) > 50 else msg)
         except Exception:  # pylint: disable=broad-except
             self.handleError(record)
 
 
 def _check_streamlit():
     """Check whether python code is run within streamlit."""
     try:
```

### Comparing `py_research-4.8.0/src/py_research/time.py` & `py_research-5.0.0/src/py_research/time.py`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/tests/py_research/test_caching.py` & `py_research-5.0.0/tests/py_research/test_caching.py`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/tests/py_research/test_colors.py` & `py_research-5.0.0/tests/py_research/test_colors.py`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/tests/py_research/test_db_base.py` & `py_research-5.0.0/tests/py_research/test_db_base.py`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/tests/py_research/test_db_importing.py` & `py_research-5.0.0/tests/py_research/test_db_importing.py`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/tests/py_research/test_files.py` & `py_research-5.0.0/tests/py_research/test_files.py`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/tests/py_research/test_geo.py` & `py_research-5.0.0/tests/py_research/test_geo.py`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/tests/py_research/test_hashing.py` & `py_research-5.0.0/tests/py_research/test_hashing.py`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/tests/py_research/test_intl.py` & `py_research-5.0.0/tests/py_research/test_intl.py`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/tests/py_research/test_plots.py` & `py_research-5.0.0/tests/py_research/test_plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from pathlib import Path
 from tempfile import gettempdir
 
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
-
 from py_research.plots import export_html, plotly_to_html, with_dropdown
 
 
 def plot_func(df: pd.DataFrame) -> go.Figure:
     """Plot a scatter plot of GDP per capita vs population with a slider for year."""
     return px.scatter(
         df,
@@ -45,13 +44,13 @@
     html = plotly_to_html(fig, write_to=path)
 
     assert isinstance(html, str)
     assert path.is_file()
 
 
 def test_with_dropdown():
-    """Test ``with_dropdown`` decorator.""" ""
+    """Test ``with_dropdown`` decorator."""
     df = px.data.gapminder()
     plot_func_wd = with_dropdown("continent")(plot_func)
 
     fig = plot_func_wd(df)
     assert isinstance(fig, go.Figure)
```

### Comparing `py_research-4.8.0/tests/py_research/test_ranking.py` & `py_research-5.0.0/tests/py_research/test_ranking.py`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/tests/py_research/test_stats.py` & `py_research-5.0.0/tests/py_research/test_stats.py`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/tests/py_research/test_tables.py` & `py_research-5.0.0/tests/py_research/test_tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
     # Test the table_colors attribute
     table.table_colors = TableColors(header_even="#123456")
     rendered = table.to_html()
     assert "background-color: #123456;" in rendered
 
     # Test the table_styles attribute
-    table.table_styles = {"th": {"color": "#654321"}}
+    table.table_css = {"th": {"color": "#654321"}}
     rendered = table.to_html()
     assert "color: #654321 !important;" in rendered
 
 
 def test_result_table_multi_df():
     """Test ResultTable."""
     # Create a DataFrame
@@ -87,15 +87,16 @@
         }
     ).set_index(["D", "E"])
 
     # Merge the two DataFrames
     merge_df = pd.concat({"df1": df, "df2": df2}, axis="columns")
 
     # Create a ResultTable
-    table = ResultTable(merge_df, hide_index=["E"])
+    table = ResultTable(merge_df, show_index=True)
+    table.styles.append(TableStyle(cols=["E"], hide="cols"))
 
     # Test the render method
     rendered = table.to_html()
     assert isinstance(rendered, str)
     assert "df1" in rendered
     assert "df2" in rendered
     assert "A" in rendered
@@ -113,15 +114,15 @@
     # Test the styles attribute with a row filter
     style = TableStyle(rows=(merge_df[("df1", "A")] < 3), css={"color": "blue"})
     table.styles.append(style)
     rendered = table.to_html()
     assert "color: blue;" in rendered
 
     # Test the styles attribute with an exact col
-    style = TableStyle(cols=[("df1", "A")], css={"color": "red"})
+    style = TableStyle(dfs="df1", cols="A", css={"color": "red"})
     table.styles.append(style)
     rendered = table.to_html()
     assert "color: red;" in rendered
 
     # Test the labels attribute
     table.labels = {"A": "Alpha", "B": "Beta", "C": "Gamma"}
     rendered = table.to_html()
```

### Comparing `py_research-4.8.0/tests/py_research/test_time.py` & `py_research-5.0.0/tests/py_research/test_time.py`

 * *Files identical despite different names*

### Comparing `py_research-4.8.0/PKG-INFO` & `py_research-5.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: py-research
-Version: 4.8.0
+Version: 5.0.0
 Summary: Collection of utilities for R&D coding in Python 🐍
 Author-Email: Lorenzo Wormer <l.wormer@mailbox.org>
+Project-URL: Documentation, https://cloudlane-one.github.io/py-research/
 Requires-Python: <3.12,>=3.10
 Requires-Dist: pandas<3.0,>=2.2.0
 Requires-Dist: PyYAML<7.0,>=6.0
 Requires-Dist: openpyxl<4.0.0,>=3.0.9
 Requires-Dist: country-converter<2.0,>=1.2
 Requires-Dist: pydantic<3.0,>=2.5.3
 Requires-Dist: streamlit<2.0.0,>=1.7.0
@@ -29,14 +30,15 @@
 Requires-Dist: pandas-stubs>=2.1.4.231227
 Requires-Dist: packaging>=23.2
 Requires-Dist: requests>=2.31.0
 Requires-Dist: pydantic-core>=2.14.6
 Requires-Dist: notebook>=7.0.6
 Requires-Dist: ipywidgets>=8.1.1
 Requires-Dist: ipython>=8.21.0
+Requires-Dist: sphinx>=7.2.6
 Description-Content-Type: text/markdown
 
 # py-research
 
 [![PyPI - Version](https://img.shields.io/pypi/v/py-research)](https://pypi.org/project/py-research)
 [![Docs](https://github.com/cloudlane-one/py-research/actions/workflows/docs.yml/badge.svg)](https://cloudlane-one.github.io/py-research)
 [![Tests](https://github.com/cloudlane-one/py-research/actions/workflows/lint-and-test.yml/badge.svg)](https://github.com/cloudlane-one/py-research/actions/workflows/lint-and-test.yml)
```

