# Comparing `tmp/relax_py-0.4.0.tar.gz` & `tmp/relax_py-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relax_py-0.4.0.tar", max compression
+gzip compressed data, was "relax_py-0.5.0.tar", max compression
```

## Comparing `relax_py-0.4.0.tar` & `relax_py-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       54 2023-11-05 14:43:09.827813 relax_py-0.4.0/README.md
--rw-r--r--   0        0        0     1508 2024-01-27 01:08:08.325065 relax_py-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-05 14:43:09.827813 relax_py-0.4.0/relax/__init__.py
--rw-r--r--   0        0        0     8065 2024-01-26 19:28:51.179076 relax_py-0.4.0/relax/app.py
--rw-r--r--   0        0        0    15512 2024-01-27 00:05:48.707480 relax_py-0.4.0/relax/html.py
--rw-r--r--   0        0        0     3899 2024-01-26 20:13:41.089047 relax_py-0.4.0/relax/injection.py
--rw-r--r--   0        0        0      414 2024-01-26 20:09:32.123920 relax_py-0.4.0/relax/injection.pyi
--rw-r--r--   0        0        0        0 2023-11-05 14:43:09.831147 relax_py-0.4.0/relax/py.typed
--rw-r--r--   0        0        0     1279 2023-12-19 21:31:47.401817 relax_py-0.4.0/relax/test.py
--rw-r--r--   0        0        0      240 2023-12-19 21:31:54.925092 relax_py-0.4.0/relax/test.pyi
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 relax_py-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       54 2023-11-05 14:43:09.827813 relax_py-0.5.0/README.md
+-rw-r--r--   0        0        0     1591 2024-02-17 09:10:44.732230 relax_py-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-05 14:43:09.827813 relax_py-0.5.0/relax/__init__.py
+-rw-r--r--   0        0        0    11671 2024-02-17 22:12:11.882405 relax_py-0.5.0/relax/app.py
+-rw-r--r--   0        0        0    16348 2024-02-17 09:22:01.240731 relax_py-0.5.0/relax/html.py
+-rw-r--r--   0        0        0     3899 2024-01-26 20:13:41.089047 relax_py-0.5.0/relax/injection.py
+-rw-r--r--   0        0        0      414 2024-01-26 20:09:32.123920 relax_py-0.5.0/relax/injection.pyi
+-rw-r--r--   0        0        0        0 2023-11-05 14:43:09.831147 relax_py-0.5.0/relax/py.typed
+-rw-r--r--   0        0        0     1279 2023-12-19 21:31:47.401817 relax_py-0.5.0/relax/test.py
+-rw-r--r--   0        0        0      240 2023-12-19 21:31:54.925092 relax_py-0.5.0/relax/test.pyi
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 relax_py-0.5.0/PKG-INFO
```

### Comparing `relax_py-0.4.0/pyproject.toml` & `relax_py-0.5.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "relax-py"
-version = "0.4.0"
+version = "0.5.0"
 description = ""
 authors = ["crpier <crpier42@gmail.com>"]
 readme = "README.md"
 packages = [
   {include = "relax"}
 ]
 
@@ -39,14 +39,16 @@
 "I001", # Let black/isort handle unsorted imports
 "ISC001",
 "N801", # allow classes to not have CamelCase name
 "PGH003", # let me use # type: ignore
 "PLR0913", # let me have lots of params in func signature
 # TODO: check if that can be ignored in file only
 "SLF001", # allow using private member
+"FBT001", # allow boolean args with default values
+"FBT002", # same thing I guess?
 ]
 
 [tool.isort]
 profile = "black"
 
 [[tool.mypy.overrides]]
 module = ["icecream", "sqlite_fts4"]
```

### Comparing `relax_py-0.4.0/relax/app.py` & `relax_py-0.5.0/relax/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import inspect
 from enum import StrEnum, auto
-from functools import wraps
+from functools import partial, wraps
 from inspect import Parameter, signature
 from typing import (
     Annotated,
     Any,
     Awaitable,
     Callable,
     Concatenate,
     Generic,
     Literal,
     Mapping,
     Protocol,
+    Type,
     TypedDict,
     TypeVar,
     get_args,
     get_origin,
 )
 from starlette.datastructures import URL
 
@@ -47,25 +48,64 @@
         content: relax.html.Element,
         status_code: int = 200,
         headers: Mapping[str, str] | None = None,
     ) -> None:
         super().__init__(content.render(), status_code, headers)
 
 
+def new_decorator(func, auth_scopes: list | None):
+    @wraps(func)
+    @requires(auth_scopes or [])
+    async def inner(request: starlette.requests.Request):
+        request = Request(request)
+        params: dict[str, Any] = {}
+        request.scope["from_htmx"] = request.headers.get("HX-Request", False) == "true"
+        for param_name, param in signature(func).parameters.items():
+            if (args := get_annotated(param)) and args[1] == "query_param":
+                if (param_value := request.query_params.get(param_name)) is None:
+                    if param.default is inspect._empty:
+                        msg = (
+                            f"parameter {param_name} from function "
+                            f"{func.__name__} has no default value "
+                            "and was not provided in the request"
+                        )
+                        raise TypeError(msg)
+                    params[param_name] = param.default
+                else:
+                    # TODO: also allow something like
+                    # \ Annotated[Path | None, "query_param"] = Path("/")
+                    params[param_name] = args[0](param_value)
+            elif (args := get_annotated(param)) and args[1] == "path_param":
+                if (param_value := request.path_params.get(param_name)) is None:
+                    if param.default is inspect._empty:
+                        msg = (
+                            f"parameter {param_name} from function "
+                            f"{func.__name__} has no default value "
+                            "and was not provided in the request"
+                        )
+                        raise TypeError(msg)
+                    params[param_name] = param.default
+                else:
+                    params[param_name] = args[0](param_value)
+        return await func(request, **params)
+
+    return inner
+
+
 class AuthScope(StrEnum):
     Authenticated = auto()
 
 
 class Scope(TypedDict):
     from_htmx: bool
 
 
 class Request(starlette.requests.Request, Generic[T]):
     user: T
-    scope: Scope
+    scope: Scope  # type: ignore
 
     def __init__(self, base_request: starlette.requests.Request):
         super().__init__(base_request.scope, base_request._receive, base_request._send)
 
     def url_of(
         self,
         func: Callable[Concatenate["Request", P], Awaitable[Any]],
@@ -99,15 +139,63 @@
             return get_args(get_args(param.annotation)[0])
     except IndexError:
         return None
 
     return None
 
 
+class RelaxRoute:
+    def __init__(
+        self,
+        path: str,
+        method: Method,
+        endpoint: Callable[Concatenate[Request, P], Awaitable[Any]],
+        # TODO: runtime validation of the signature
+        sig: Type[Callable[P, Any]] | None = None,
+        auth_scopes: list[AuthScope] | None = None,
+    ) -> None:
+        self.path = path
+        self.endpoint = endpoint
+        self.method = method
+        self.auth_scopes = auth_scopes
+        self.sig = sig
+
+
+class ViewContext:
+    def __init__(self) -> None:
+        self.endpoints: dict[Callable, Any] = {}
+
+    def add_endpoint(self, sig: Any, endpoint: Callable) -> None:
+        self.endpoints[sig] = endpoint
+
+    def endpoint(self, sig: Type[T]) -> T:
+        return self.endpoints[sig]
+
+
 class App(Starlette):
+    def __init__(self, *args, **kwargs) -> None:
+        super().__init__(*args, **kwargs)
+        self.view_context = ViewContext()
+
+    def add_routes(self, routes: list[RelaxRoute]) -> None:
+        for route in routes:
+            # TODO: maybe make the name file + fn_name?
+            # TODO: also, error out when finding a duplicate name
+            route_name = route.endpoint.__name__
+            new_route = Route(
+                path=route.path,
+                endpoint=new_decorator(route.endpoint, route.auth_scopes),
+                methods=[route.method],
+                name=route_name,
+            )
+            self.routes.append(new_route)
+            if route.sig:
+                lol = partial(self.url_path_for, route_name)
+                self.view_context.add_endpoint(sig=route.sig, endpoint=lol)
+
     # TODO: method should be enum maybe?
     def path_function(
         self,
         method: Method,
         endpoint: str,
         auth_scopes: list[AuthScope] | None = None,
     ):
@@ -161,23 +249,28 @@
             )
 
             return inner
 
         return decorator
 
 
-class Router:
+class BaseRouter(Protocol):
+    ...
+
+
+class Router(BaseRouter):
     def __init__(self) -> None:
         self.routes: list[Route] = []
 
     def path_function(
         self,
         method: Method,
         endpoint: str,
         auth_scopes: list[AuthScope] | None = None,
+        sig: Any = None,
     ):
         if auth_scopes is None:
             auth_scopes = []
 
         def decorator(func):
             @wraps(func)
             @requires(auth_scopes)
```

### Comparing `relax_py-0.4.0/relax/html.py` & `relax_py-0.5.0/relax/html.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,17 +218,20 @@
     def __init__(
         self,
         *,
         classes: list[str] | None = None,
         attrs: dict | None = None,
         id: str | None = None,
         hyperscript: str | None = None,
+        text: str | None = None,
     ) -> None:
         super().__init__(classes=classes, attrs=attrs, id=id, hyperscript=hyperscript)
         self._children: list[Element] = []
+        if text is not None:
+            self.text(text)
 
     def render(self) -> str:
         return (
             f"<{self.name}{self._render_attributes()}>"
             f"{self._render_children()}"
             f"</{self.name}>"
         )
@@ -472,22 +475,25 @@
         type: InputType,
         value: str | None = None,
         placeholder: str | None = None,
         classes: list[str] | None = None,
         attrs: dict | None = None,
         id: str | None = None,
         hyperscript: str | None = None,
+        disabled: bool = False,
     ) -> None:
         super().__init__(classes=classes, attrs=attrs, id=id, hyperscript=hyperscript)
         self._attributes["name"] = name
         self._attributes["type"] = type
         if value:
             self._attributes["value"] = value
         if placeholder:
             self._attributes["placeholder"] = placeholder
+        if disabled is True:
+            self._attributes["disabled"] = True
 
 
 class img(SelfClosingTag):
     name = "img"
 
     def __init__(
         self,
@@ -521,14 +527,32 @@
         if controls:
             self._attributes["controls"] = "true"
 
 
 class textarea(Tag):
     name = "textarea"
 
+    def __init__(
+        self,
+        name: str,
+        type: InputType,
+        placeholder: str | None = None,
+        classes: list[str] | None = None,
+        attrs: dict | None = None,
+        id: str | None = None,
+        hyperscript: str | None = None,
+        disabled: bool = False,
+    ) -> None:
+        super().__init__(classes=classes, attrs=attrs, id=id, hyperscript=hyperscript)
+        self._attributes["name"] = name
+        self._attributes["type"] = type
+        if placeholder:
+            self._attributes["placeholder"] = placeholder
+        if disabled is True:
+            self._attributes["disabled"] = True
 
 class meta(SelfClosingTag):
     name = "meta"
 
     def __init__(
         self,
         *,
```

### Comparing `relax_py-0.4.0/relax/injection.py` & `relax_py-0.5.0/relax/injection.py`

 * *Files identical despite different names*

### Comparing `relax_py-0.4.0/relax/test.py` & `relax_py-0.5.0/relax/test.py`

 * *Files identical despite different names*

