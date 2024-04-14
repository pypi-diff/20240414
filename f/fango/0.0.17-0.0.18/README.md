# Comparing `tmp/fango-0.0.17.tar.gz` & `tmp/fango-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fango-0.0.17.tar", max compression
+gzip compressed data, was "fango-0.0.18.tar", max compression
```

## Comparing `fango-0.0.17.tar` & `fango-0.0.18.tar`

### file list

```diff
@@ -1,15 +1,19 @@
--rw-r--r--   0        0        0      620 2024-02-24 18:07:20.033525 fango-0.0.17/README.md
--rw-r--r--   0        0        0     2681 2024-02-24 18:05:05.402374 fango-0.0.17/fango/auth.py
--rw-r--r--   0        0        0      310 2024-02-24 18:05:05.402787 fango-0.0.17/fango/generics.py
--rw-r--r--   0        0        0     1116 2024-02-24 18:05:05.403166 fango-0.0.17/fango/logging.py
--rw-r--r--   0        0        0     5552 2024-02-24 18:05:05.403593 fango-0.0.17/fango/models.py
--rw-r--r--   0        0        0     6639 2024-02-24 18:05:05.404018 fango-0.0.17/fango/pagination.py
--rw-r--r--   0        0        0     2447 2024-02-24 18:05:05.404345 fango-0.0.17/fango/permissions.py
--rw-r--r--   0        0        0      438 2024-02-24 18:05:05.404694 fango-0.0.17/fango/routing.py
--rw-r--r--   0        0        0     1710 2024-02-24 18:05:05.405081 fango-0.0.17/fango/schemas.py
--rw-r--r--   0        0        0      284 2024-02-24 18:05:05.409504 fango-0.0.17/fango/tests/client.py
--rw-r--r--   0        0        0      723 2024-02-24 18:05:05.409821 fango-0.0.17/fango/tests/fixtures.py
--rw-r--r--   0        0        0     3116 2024-02-24 18:05:05.410143 fango-0.0.17/fango/utils.py
--rw-r--r--   0        0        0     6953 2024-02-24 18:05:05.410488 fango-0.0.17/fango/viewsets.py
--rw-r--r--   0        0        0      512 2024-02-24 18:07:56.479918 fango-0.0.17/pyproject.toml
--rw-r--r--   0        0        0     1422 1970-01-01 00:00:00.000000 fango-0.0.17/PKG-INFO
+-rw-r--r--   0        0        0      620 2024-02-24 18:07:20.033525 fango-0.0.18/README.md
+-rw-r--r--   0        0        0     7456 2024-04-14 16:48:43.151576 fango-0.0.18/fango/adapters/pydantic.py
+-rw-r--r--   0        0        0      848 2024-04-14 16:48:43.152107 fango-0.0.18/fango/adapters/types.py
+-rw-r--r--   0        0        0     2681 2024-04-14 16:48:43.152538 fango-0.0.18/fango/auth.py
+-rw-r--r--   0        0        0     4845 2024-04-14 16:48:43.152929 fango-0.0.18/fango/filters.py
+-rw-r--r--   0        0        0      310 2024-04-14 16:48:43.153250 fango-0.0.18/fango/generics.py
+-rw-r--r--   0        0        0     1907 2024-04-14 16:48:43.153595 fango-0.0.18/fango/log.py
+-rw-r--r--   0        0        0        0 2024-04-14 16:48:43.154606 fango-0.0.18/fango/middleware/__init__.py
+-rw-r--r--   0        0        0      997 2024-04-14 16:48:43.156087 fango-0.0.18/fango/middleware/common.py
+-rw-r--r--   0        0        0     6639 2024-04-14 16:48:43.156526 fango-0.0.18/fango/pagination.py
+-rw-r--r--   0        0        0     2447 2024-04-14 16:48:43.156924 fango-0.0.18/fango/permissions.py
+-rw-r--r--   0        0        0      440 2024-04-14 16:48:43.157427 fango-0.0.18/fango/routing.py
+-rw-r--r--   0        0        0     2123 2024-04-14 16:48:43.157748 fango-0.0.18/fango/schemas.py
+-rw-r--r--   0        0        0      284 2024-04-14 16:48:43.163550 fango-0.0.18/fango/tests/client.py
+-rw-r--r--   0        0        0      723 2024-04-14 16:48:43.163843 fango-0.0.18/fango/tests/fixtures.py
+-rw-r--r--   0        0        0     3518 2024-04-14 16:48:43.164120 fango-0.0.18/fango/utils.py
+-rw-r--r--   0        0        0     7253 2024-04-14 16:51:53.948819 fango-0.0.18/fango/viewsets.py
+-rw-r--r--   0        0        0      536 2024-04-14 16:53:16.859589 fango-0.0.18/pyproject.toml
+-rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 fango-0.0.18/PKG-INFO
```

### Comparing `fango-0.0.17/README.md` & `fango-0.0.18/README.md`

 * *Files identical despite different names*

### Comparing `fango-0.0.17/fango/auth.py` & `fango-0.0.18/fango/auth.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.17/fango/logging.py` & `fango-0.0.18/fango/log.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,18 @@
+import inspect
 import logging
+from functools import wraps
+
+from django.conf import settings
 
 logger = logging.Logger("uvicorn.access")
 handler = logging.StreamHandler()
 
+__all__ = ["logger", "log_params"]
+
 
 class ColoredFormatter(logging.Formatter):
     grey = "\x1b[38;21m"
     blue = "\x1b[38;5;39m"
     yellow = "\x1b[38;5;226m"
     red = "\x1b[38;5;196m"
     bold_red = "\x1b[31;1m"
@@ -30,10 +36,30 @@
         return formatter.format(record)
 
 
 handler.setFormatter(ColoredFormatter("%(levelname)s%(message)s"))
 logger.setLevel(logging.INFO)
 logger.addHandler(handler)
 
-__slots__ = [
-    "logger",
-]
+arg_prefix = "\t\t--> "
+
+
+def log_params(prefix):
+    """
+    Decorator for logging function call with args.
+
+    """
+
+    def log(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            if settings.ENABLE_CALL_LOG:
+                bound_arguments = inspect.signature(func).bind(*args, **kwargs)
+                bound_arguments.apply_defaults()
+                args_reprs = [arg_prefix + f"{name}={value!r}" for name, value in bound_arguments.arguments.items()]
+                signature = "\n".join(args_reprs)
+                logger.info(f"[{prefix}] call: {func.__name__} with params:\n{signature}\n")
+            return func(*args, **kwargs)
+
+        return wrapper
+
+    return log
```

### Comparing `fango-0.0.17/fango/pagination.py` & `fango-0.0.18/fango/pagination.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.17/fango/permissions.py` & `fango-0.0.18/fango/permissions.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.17/fango/schemas.py` & `fango-0.0.18/fango/schemas.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,28 @@
 from dataclasses import dataclass
 from typing import Generic, TypedDict, TypeVar, get_args
 
 from django.db.models import Manager
 from pydantic import BaseModel, ConfigDict, field_validator
 from typing_extensions import NotRequired
 
-__all__ = ["Cursor", "Page", "Entry", "ChoicesItem", "ReadOnlyModel"]
+from fango.adapters.types import PK
+
+__all__ = [
+    "Cursor",
+    "Page",
+    "Entry",
+    "ChoicesItem",
+    "FormModel",
+    "ActionClasses",
+    "Multiselect",
+    "CRUDAdapter",
+    "UnlinkAdapter",
+    "DBModel",
+]
 
 T = TypeVar("T")
 
 
 @dataclass
 class Cursor:
     offset: int
@@ -19,50 +32,63 @@
 
 class Page(BaseModel, Generic[T]):
     next: str | None
     previous: str | None
     results: list[T]
 
 
+class CRUDAdapter(BaseModel, Generic[T]):
+    create: list[T] = []
+    update: list[T] = []
+    delete: list[PK]
+
+
+class UnlinkAdapter(BaseModel, Generic[T]):
+    unlink: list[PK]
+
+
 class Entry(BaseModel, Generic[T]):
     title: str | None
     results: T
 
 
 class ChoicesItem(BaseModel, Generic[T]):
     id: T
     name: str | None
 
 
-class ReadOnlyModel(BaseModel):
-    model_config = ConfigDict(from_attributes=True, frozen=True)
-
-    id: int
+class FormModel(BaseModel):
+    model_config = ConfigDict(from_attributes=True)
 
     @field_validator("*", mode="before")
-    def render_complex_fields(cls, value, info):
+    def validate_complex_fields(cls, value, info):
         from fango.utils import get_choices_label
 
         for type_ in get_args(cls.model_fields[info.field_name].annotation):
             if metadata := getattr(type_, "__pydantic_generic_metadata__", None):
                 if value is not None and metadata["origin"] is ChoicesItem:
                     return {"id": value, "name": get_choices_label(metadata["args"][0], value)}
 
         if isinstance(value, Manager):
             return value.all()
+
         return value
 
 
-class Multiselect(ReadOnlyModel):
+class Multiselect(FormModel):
     id: int
-    name: str | None
+    name: str | None = None
+
+
+class DBModel(BaseModel):
+    model_config = ConfigDict(populate_by_name=True, from_attributes=True)
 
 
 class ActionClasses(TypedDict):
-    list: NotRequired[type[BaseModel]]
+    table: NotRequired[type[BaseModel]]
     retrieve: NotRequired[type[BaseModel]]
     update: NotRequired[type[BaseModel]]
     delete: NotRequired[type[BaseModel]]
 
 
 class Token(BaseModel):
     access: str
```

### Comparing `fango-0.0.17/fango/tests/fixtures.py` & `fango-0.0.18/fango/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `fango-0.0.17/fango/utils.py` & `fango-0.0.18/fango/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,27 +5,31 @@
 from typing import Any, Callable
 
 from django.conf import settings
 from django.core.cache import cache
 from django.db.models import Choices
 from django.db.models.enums import ChoicesMeta
 from fastapi.concurrency import run_in_threadpool
+from fastapi.routing import APIRoute
 
+from base.main import app
+from base.urls import router
 from fango.generics import MethodT
 from fango.schemas import ChoicesItem
 
 __all__ = [
     "ttl_cache",
     "reverse_ordering",
     "replace_proto",
     "run_async",
     "run_sync",
     "get_choices_as_data",
     "copy_instance_method",
     "get_choices_label",
+    "get_all_routes_basenames",
 ]
 
 
 def ttl_cache(ttl=None) -> Any:
     """
     Decorator for TTL caching.
 
@@ -117,7 +121,19 @@
 
 def get_choices_label(enum: type[Choices], value: int) -> str:
     """
     Function returns choices text.
 
     """
     return enum.choices[value][1]
+
+
+def get_all_routes_basenames() -> set:
+    """
+    Function returns set of all routes basenames
+
+    """
+
+    fastapi = {x.tags[0] for x in app.routes if isinstance(x, APIRoute) and x.tags}
+    django = {x.name.split("-")[0] for x in router.urls}
+
+    return fastapi | django
```

### Comparing `fango-0.0.17/fango/viewsets.py` & `fango-0.0.18/fango/viewsets.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from typing import Generic, TypeVar, cast
 
 from django.db.models import QuerySet
 from fastapi import Request
 from fastapi.routing import APIRoute
 from pydantic import BaseModel
 
+from fango.filters import generate_filterset_by_pydantic
 from fango.generics import BaseModelT, ModelT
 from fango.permissions import ALLOW_ANY
 from fango.routing import FangoRouter, action
 from fango.schemas import ActionClasses
 from fango.utils import copy_instance_method
 
 
@@ -28,28 +29,29 @@
     http_method_names: set[str]
     lookup_value_converter: str = "int"
     pydantic_model_action_classes: ActionClasses = {}
     dependencies = []
 
     def __init__(self, router: FangoRouter, basename: str) -> None:
         self.request: Request
+        self.filterset_class = generate_filterset_by_pydantic(self.pydantic_model)
         self._router = router
         self._basename = basename
         self.__initialize_http_methods()
         self.__initialize_pydantic_model_classes()
         self.__merge_routers()
 
     def __initialize_http_methods(self) -> None:
-        RO_METHODS = {"HEAD", "TRACE", "OPTIONS", "GET"}
-        RW_METHODS = {"PATCH", "POST", "PUT", "DELETE"}
+        ro_methods = {"HEAD", "TRACE", "OPTIONS", "GET"}
+        rw_methods = {"PATCH", "POST", "PUT", "DELETE"}
 
         if hasattr(self, "queryset") and self.queryset.model._meta.managed:
-            self.http_method_names = RO_METHODS | RW_METHODS
+            self.http_method_names = ro_methods | rw_methods
         else:
-            self.http_method_names = RO_METHODS
+            self.http_method_names = ro_methods
 
     def __initialize_pydantic_model_classes(self) -> None:
         """
         Method for init pydantic_model_action_classes for all viewset routes.
 
         """
         action_classes = ActionClasses({x.name: self.pydantic_model for x in self._internal.routes})  # type: ignore
@@ -101,15 +103,15 @@
             if route.name not in exclude  # type: ignore
             and route.methods & self.http_method_names  # type: ignore
         ]
         for route in router.routes:
             route = cast(APIRoute, route)
             route.dependencies = [*self._router.dependencies, *self.dependencies]
 
-            if "%s" in route.path:
+            if "%" in route.path:
                 route.path = route.path % self.lookup_value_converter
                 route.path_format = route.path_format % self.lookup_value_converter
 
             route.endpoint = self.__get_route_endpoint(route)
             if route.response_model:
                 self.__fix_generic_response_annotations(route)
 
@@ -155,20 +157,25 @@
                 if issubclass(klass, Generic) and issubclass(klass, BaseModel):
                     if route.response_model.__pydantic_generic_metadata__.get("args"):
                         route.response_model = klass[pydantic_model]  # type: ignore
                     else:
                         route.response_model = klass
                     break
 
-    def get_pydantic_model_class(self, request: Request) -> BaseModelT:
+    def get_pydantic_model_class(self, request: Request) -> type[BaseModelT]:
         """
         Method for get concrete pydantic_model for route.
 
         """
-        return self.pydantic_model_action_classes[request.scope["route"].name]
+        route_name = request.scope["route"].name
+
+        if model := self.pydantic_model_action_classes.get(route_name):
+            return model
+        else:
+            return self.pydantic_model_action_classes["table"]
 
     def get_queryset(self, request: Request) -> QuerySet:
         """
         Method for get queryset defined in ViewSet.
 
         """
         return self.queryset
@@ -178,15 +185,15 @@
     queryset: QuerySet
 
     async def create_entry(self, payload: BaseModelT) -> ModelT:
         """
         Method for create new entry.
 
         """
-        return await self.queryset.model.from_schema(payload)
+        return await self.queryset.model.save_from_schema(payload)
 
     async def update_entry(self, payload: BaseModelT, pk: int) -> ModelT:
         """
         Method for update existance entry.
 
         """
-        return await self.queryset.model.from_schema(payload, pk)
+        return await self.queryset.model.save_from_schema(payload, pk)
```

### Comparing `fango-0.0.17/pyproject.toml` & `fango-0.0.18/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "fango"
-version = "0.0.17"
+version = "0.0.18"
 description = "Metaframework for web with combined FastAPI and Django"
 repository = "https://github.com/egorgam/fango"
 keywords = ["fastapi", "django", "fango"]
 authors = ["Egor Gamazin <egorgamazin@yandex.ru>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 django = ">=4.2,<6.0"
 fastapi = "^0.108.0"
 python-jose = "^3.3.0"
 pytest = "^8.0.1"
+django-filter = "^24.2"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fango-0.0.17/PKG-INFO` & `fango-0.0.18/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: fango
-Version: 0.0.17
+Version: 0.0.18
 Summary: Metaframework for web with combined FastAPI and Django
 Home-page: https://github.com/egorgam/fango
 License: MIT
 Keywords: fastapi,django,fango
 Author: Egor Gamazin
 Author-email: egorgamazin@yandex.ru
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: django (>=4.2,<6.0)
+Requires-Dist: django-filter (>=24.2,<25.0)
 Requires-Dist: fastapi (>=0.108.0,<0.109.0)
 Requires-Dist: pytest (>=8.0.1,<9.0.0)
 Requires-Dist: python-jose (>=3.3.0,<4.0.0)
 Project-URL: Repository, https://github.com/egorgam/fango
 Description-Content-Type: text/markdown
 
 # <img src='https://github.com/egorgam/fango/assets/13712792/e541fff2-3833-4f30-ba9b-09ea5c375077' width='30'> FANGO
```

