# Comparing `tmp/decorator_utils-1.0.0.tar.gz` & `tmp/decorator_utils-1.1.0.tar.gz`

## Comparing `decorator_utils-1.0.0.tar` & `decorator_utils-1.1.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 decorator_utils-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 decorator_utils-1.0.0/.github/workflows/publish-pypi.yaml
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 decorator_utils-1.0.0/decorator_utils/__init__.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 decorator_utils-1.0.0/decorator_utils/metadata.py
--rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 decorator_utils-1.0.0/decorator_utils/wrapper.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 decorator_utils-1.0.0/LICENSE
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 decorator_utils-1.0.0/README.md
--rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 decorator_utils-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 decorator_utils-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 decorator_utils-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 decorator_utils-1.1.0/.github/workflows/publish-pypi.yaml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 decorator_utils-1.1.0/decorator_utils/__init__.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 decorator_utils-1.1.0/decorator_utils/context.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 decorator_utils-1.1.0/decorator_utils/metadata.py
+-rw-r--r--   0        0        0     3581 2020-02-02 00:00:00.000000 decorator_utils-1.1.0/decorator_utils/wrapper.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 decorator_utils-1.1.0/LICENSE
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 decorator_utils-1.1.0/README.md
+-rw-r--r--   0        0        0     1809 2020-02-02 00:00:00.000000 decorator_utils-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 decorator_utils-1.1.0/PKG-INFO
```

### Comparing `decorator_utils-1.0.0/.github/workflows/publish-pypi.yaml` & `decorator_utils-1.1.0/.github/workflows/publish-pypi.yaml`

 * *Files identical despite different names*

### Comparing `decorator_utils-1.0.0/decorator_utils/metadata.py` & `decorator_utils-1.1.0/decorator_utils/metadata.py`

 * *Files identical despite different names*

### Comparing `decorator_utils-1.0.0/decorator_utils/wrapper.py` & `decorator_utils-1.1.0/decorator_utils/wrapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 from __future__ import annotations
 
 from functools import wraps
-from typing import Any, Callable, Tuple
+from typing import Any, Callable, NoReturn, Tuple
 
 from decorator_utils.metadata import FunctionMetadata
 
 
 def function_wrapper(pre_cb: Callable = None, post_cb: Callable = None, *,
                      use_result: bool = True, force_args: bool = True, forward_metadata: bool = False,
-                     return_metadata: bool = False) -> Any | Tuple[Any, FunctionMetadata]:
+                     return_metadata: bool = False) -> Callable[[...], Any | Tuple[Any, FunctionMetadata]]:
     """
     Decorator to wrap a function and execute callbacks before and after its execution.
     Both callback functions take the wrapped function parameters plus a `FunctionMetadata` object instance as
     `_func_metadata` kwarg if the function accepts them.
     Callback function will not get `args` or `kwargs` if they are not accepted unless they are forced and will check if
     they are accepted using their names.
     :param Callable pre_cb: Callback to execute before the wrapped function.
     :param Callable post_cb: Callback to execute after the wrapped function.
     :param bool use_result: Whether to pass decorated function result to `post_func` as first arg.
     :param bool force_args: Whether to force `args` or `kwargs` to be passed tho callback functions.
     :param bool forward_metadata: Whether to add `_func_metadata` to `kwargs`.
     :param bool return_metadata: Whether to also return `_func_metadata` as result in a tuple (`result`, `metadata`).
-    :return Any | Tuple[Any, ...]: The wrapped function return value.
+    :return Callable[[...], Any | Tuple[Any, FunctionMetadata]]: The wrapped function return value.
     """
 
-    def __decorator(decorated_function):
-        def __exec_callback(function: Callable, *args, insert_result: Any = None, **kwargs, ) -> Any:
+    def __decorator(decorated_function) -> Callable[[...], Any | Tuple[Any, FunctionMetadata]]:
+        def __exec_callback(function: Callable, *args, insert_result: Any = NoReturn, **kwargs) -> Any:
             """
             Utility to call functions and handle their supported `args` and `kwargs`.
             :param Callable function: Callback function.
             :param Any insert_result: Pass this value as first arg to the function if provided.
             :return: Any | Tuple[Any, ...]: The wrapped function return value.
             """
 
@@ -39,36 +39,36 @@
                 if metadata.accepts_pos_params(['self'], explicit=True):  # Handle class method self instance
                     args = [args[0], *[a for a in args[1:] if metadata.accepts_pos_params([a])]]
                 else:
                     args = [a for a in args if metadata.accepts_pos_params([a])]
 
                 kwargs = {p: v for p, v in kwargs.items() if metadata.accepts_kw_params([p])}
 
-            if insert_result is not None:  # Pass result as first arg if provided
+            if insert_result is not NoReturn:  # Pass result as first arg if provided
                 if isinstance(args, tuple):
                     args = list(args)
                 args.insert(0, insert_result)
 
             return function(*args, **kwargs)
 
         @wraps(decorated_function)
-        def __wrapper(*args, **kwargs):
+        def __wrapper(*args, **kwargs) -> Any | Tuple[Any, FunctionMetadata]:
             metadata = FunctionMetadata(decorated_function)
 
             if forward_metadata:
                 kwargs['_func_metadata'] = metadata
 
             if pre_cb is not None:
                 __exec_callback(pre_cb, *args, **kwargs)
 
             result = __exec_callback(decorated_function, *args, **kwargs)
 
             metadata.returns = type(result)
 
             if post_cb is not None:
-                __exec_callback(post_cb, *args, insert_result=result if use_result else None, **kwargs)
+                __exec_callback(post_cb, *args, insert_result=result if use_result else NoReturn, **kwargs)
 
             return (result, metadata) if return_metadata else result
 
         return __wrapper
 
     return __decorator
```

### Comparing `decorator_utils-1.0.0/LICENSE` & `decorator_utils-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `decorator_utils-1.0.0/README.md` & `decorator_utils-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `decorator_utils-1.0.0/pyproject.toml` & `decorator_utils-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `decorator_utils-1.0.0/PKG-INFO` & `decorator_utils-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: decorator-utils
-Version: 1.0.0
+Version: 1.1.0
 Summary: Simple and useful decorator utilities.
 Project-URL: Repository, https://github.com/stickm4n/decorator-utils
 Project-URL: Documentation, https://github.com/stickm4n/decorator-utils/wiki
 Project-URL: Issues, https://github.com/stickm4n/decorator-utils/issues
 Author-email: "Julio C. Galindo" <jcgalindo.jcgh@gmail.com>
 License: MIT License
```

