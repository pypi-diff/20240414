# Comparing `tmp/python_dev_utils-0.2.0.tar.gz` & `tmp/python_dev_utils-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_dev_utils-0.2.0.tar", last modified: Tue Apr  9 13:32:55 2024, max compression
+gzip compressed data, was "python_dev_utils-1.0.6.tar", last modified: Sun Apr 14 10:12:32 2024, max compression
```

## Comparing `python_dev_utils-0.2.0.tar` & `python_dev_utils-1.0.6.tar`

### file list

```diff
@@ -1,41 +1,68 @@
--rw-r--r--   0        0        0     1063 2024-03-20 07:39:19.724729 python_dev_utils-0.2.0/LICENCE
--rw-r--r--   0        0        0     1962 2024-04-05 12:10:37.518458 python_dev_utils-0.2.0/README.md
--rw-r--r--   0        0        0        0 2024-03-19 07:18:12.341673 python_dev_utils-0.2.0/dev_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 06:33:01.146013 python_dev_utils-0.2.0/dev_utils/core/__init__.py
--rw-r--r--   0        0        0     4806 2024-04-04 10:15:44.718260 python_dev_utils-0.2.0/dev_utils/core/abstract.py
--rw-r--r--   0        0        0     1165 2024-03-26 12:21:23.530800 python_dev_utils-0.2.0/dev_utils/core/exc.py
--rw-r--r--   0        0        0      229 2024-03-26 14:07:13.958342 python_dev_utils-0.2.0/dev_utils/core/guards.py
--rw-r--r--   0        0        0      823 2024-04-01 13:22:15.897317 python_dev_utils-0.2.0/dev_utils/core/logging.py
--rw-r--r--   0        0        0     1687 2024-04-09 13:20:36.940262 python_dev_utils-0.2.0/dev_utils/core/results.py
--rw-r--r--   0        0        0      776 2024-03-28 08:22:11.212881 python_dev_utils-0.2.0/dev_utils/core/utils.py
--rw-r--r--   0        0        0      210 2024-03-28 10:44:02.392930 python_dev_utils-0.2.0/dev_utils/profiling/__init__.py
--rw-r--r--   0        0        0     1737 2024-03-29 13:52:13.342131 python_dev_utils-0.2.0/dev_utils/profiling/containers.py
--rw-r--r--   0        0        0     2850 2024-04-04 09:56:53.374155 python_dev_utils-0.2.0/dev_utils/profiling/middlewares.py
--rw-r--r--   0        0        0     9754 2024-04-04 10:02:43.937276 python_dev_utils-0.2.0/dev_utils/profiling/profilers.py
--rw-r--r--   0        0        0      940 2024-04-05 07:27:22.705464 python_dev_utils-0.2.0/dev_utils/profiling/utils.py
--rw-r--r--   0        0        0      340 2024-03-25 06:40:13.495555 python_dev_utils-0.2.0/dev_utils/sqlalchemy/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 06:19:39.723653 python_dev_utils-0.2.0/dev_utils/sqlalchemy/filters/__init__.py
--rw-r--r--   0        0        0    16331 2024-04-04 08:59:51.727121 python_dev_utils-0.2.0/dev_utils/sqlalchemy/filters/converters.py
--rw-r--r--   0        0        0     1562 2024-03-26 14:07:50.698059 python_dev_utils-0.2.0/dev_utils/sqlalchemy/filters/guards.py
--rw-r--r--   0        0        0     9556 2024-03-29 14:18:20.445990 python_dev_utils-0.2.0/dev_utils/sqlalchemy/filters/operators.py
--rw-r--r--   0        0        0     1283 2024-03-25 07:02:41.449042 python_dev_utils-0.2.0/dev_utils/sqlalchemy/filters/types.py
--rw-r--r--   0        0        0    12623 2024-03-26 08:35:25.401470 python_dev_utils-0.2.0/dev_utils/sqlalchemy/utils.py
--rw-r--r--   0        0        0     2962 2024-04-09 13:32:55.342253 python_dev_utils-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-20 07:06:32.612246 python_dev_utils-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     9104 2024-04-01 13:25:07.596658 python_dev_utils-0.2.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-03-26 14:08:14.537876 python_dev_utils-0.2.0/tests/core/__init__.py
--rw-r--r--   0        0        0     1589 2024-04-04 10:35:52.893988 python_dev_utils-0.2.0/tests/core/test_abstract.py
--rw-r--r--   0        0        0      508 2024-03-26 14:08:33.510730 python_dev_utils-0.2.0/tests/core/test_guards.py
--rw-r--r--   0        0        0     1040 2024-04-09 13:22:59.336479 python_dev_utils-0.2.0/tests/core/test_results.py
--rw-r--r--   0        0        0      933 2024-03-29 06:21:02.987051 python_dev_utils-0.2.0/tests/core/test_utils.py
--rw-r--r--   0        0        0        0 2024-03-28 08:10:36.944938 python_dev_utils-0.2.0/tests/profiling/__init__.py
--rw-r--r--   0        0        0      349 2024-03-29 13:58:08.366680 python_dev_utils-0.2.0/tests/profiling/test_middlewares.py
--rw-r--r--   0        0        0     3027 2024-04-04 10:01:48.346733 python_dev_utils-0.2.0/tests/profiling/test_profilers.py
--rw-r--r--   0        0        0        0 2024-03-25 06:27:13.006325 python_dev_utils-0.2.0/tests/sqlalchemy/__init__.py
--rw-r--r--   0        0        0    17186 2024-03-29 13:24:07.386873 python_dev_utils-0.2.0/tests/sqlalchemy/filters/test_converters.py
--rw-r--r--   0        0        0     1210 2024-03-26 14:08:03.098964 python_dev_utils-0.2.0/tests/sqlalchemy/filters/test_guards.py
--rw-r--r--   0        0        0     7428 2024-03-25 06:40:32.137462 python_dev_utils-0.2.0/tests/sqlalchemy/filters/test_operators.py
--rw-r--r--   0        0        0     7366 2024-03-25 06:19:19.846082 python_dev_utils-0.2.0/tests/sqlalchemy/test_utils.py
--rw-r--r--   0        0        0      820 2024-03-29 06:17:35.440257 python_dev_utils-0.2.0/tests/types.py
--rw-r--r--   0        0        0     7174 2024-03-29 06:15:40.110095 python_dev_utils-0.2.0/tests/utils.py
--rw-r--r--   0        0        0     2451 1970-01-01 00:00:00.000000 python_dev_utils-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-03-20 07:39:19.724729 python_dev_utils-1.0.6/LICENCE
+-rw-r--r--   0        0        0     1992 2024-04-12 13:50:09.038622 python_dev_utils-1.0.6/README.md
+-rw-r--r--   0        0        0        0 2024-03-19 07:18:12.341673 python_dev_utils-1.0.6/dev_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 06:33:01.146013 python_dev_utils-1.0.6/dev_utils/core/__init__.py
+-rw-r--r--   0        0        0     5015 2024-04-12 09:11:29.068964 python_dev_utils-1.0.6/dev_utils/core/abstract.py
+-rw-r--r--   0        0        0     1165 2024-03-26 12:21:23.530800 python_dev_utils-1.0.6/dev_utils/core/exc.py
+-rw-r--r--   0        0        0      571 2024-04-12 12:22:55.526998 python_dev_utils-1.0.6/dev_utils/core/guards.py
+-rw-r--r--   0        0        0      823 2024-04-12 09:11:29.068964 python_dev_utils-1.0.6/dev_utils/core/logging.py
+-rw-r--r--   0        0        0     1687 2024-04-09 13:20:36.940262 python_dev_utils-1.0.6/dev_utils/core/results.py
+-rw-r--r--   0        0        0      776 2024-04-12 09:11:29.068964 python_dev_utils-1.0.6/dev_utils/core/utils.py
+-rw-r--r--   0        0        0     1618 2024-04-12 10:34:31.616028 python_dev_utils-1.0.6/dev_utils/fastapi/__init__.py
+-rw-r--r--   0        0        0      315 2024-04-12 10:32:28.920904 python_dev_utils-1.0.6/dev_utils/fastapi/middlewares/__init__.py
+-rw-r--r--   0        0        0     2889 2024-04-12 09:11:29.068964 python_dev_utils-1.0.6/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py
+-rw-r--r--   0        0        0     1564 2024-04-12 10:31:39.700255 python_dev_utils-1.0.6/dev_utils/fastapi/verbose_http_exceptions/__init__.py
+-rw-r--r--   0        0        0    12481 2024-04-12 12:10:40.465060 python_dev_utils-1.0.6/dev_utils/fastapi/verbose_http_exceptions/exc.py
+-rw-r--r--   0        0        0     4341 2024-04-12 12:19:20.576031 python_dev_utils-1.0.6/dev_utils/fastapi/verbose_http_exceptions/handlers.py
+-rw-r--r--   0        0        0      691 2024-04-12 09:58:17.224272 python_dev_utils-1.0.6/dev_utils/fastapi/verbose_http_exceptions/utils.py
+-rw-r--r--   0        0        0      340 2024-03-25 06:40:13.495555 python_dev_utils-1.0.6/dev_utils/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:19:39.723653 python_dev_utils-1.0.6/dev_utils/sqlalchemy/filters/__init__.py
+-rw-r--r--   0        0        0    16331 2024-04-12 09:11:29.070964 python_dev_utils-1.0.6/dev_utils/sqlalchemy/filters/converters.py
+-rw-r--r--   0        0        0     1538 2024-04-12 09:11:29.068964 python_dev_utils-1.0.6/dev_utils/sqlalchemy/filters/guards.py
+-rw-r--r--   0        0        0     9556 2024-04-12 09:11:29.069965 python_dev_utils-1.0.6/dev_utils/sqlalchemy/filters/operators.py
+-rw-r--r--   0        0        0     1283 2024-04-12 09:11:29.068964 python_dev_utils-1.0.6/dev_utils/sqlalchemy/filters/types.py
+-rw-r--r--   0        0        0        0 2024-04-09 13:34:17.832279 python_dev_utils-1.0.6/dev_utils/sqlalchemy/mixins/__init__.py
+-rw-r--r--   0        0        0     3050 2024-04-10 14:09:42.769706 python_dev_utils-1.0.6/dev_utils/sqlalchemy/mixins/audit.py
+-rw-r--r--   0        0        0     1141 2024-04-10 08:55:37.140201 python_dev_utils-1.0.6/dev_utils/sqlalchemy/mixins/base.py
+-rw-r--r--   0        0        0     1302 2024-04-10 10:08:21.445027 python_dev_utils-1.0.6/dev_utils/sqlalchemy/mixins/general.py
+-rw-r--r--   0        0        0      888 2024-04-12 09:11:29.068964 python_dev_utils-1.0.6/dev_utils/sqlalchemy/mixins/ids.py
+-rw-r--r--   0        0        0        0 2024-04-11 07:41:17.195661 python_dev_utils-1.0.6/dev_utils/sqlalchemy/profiling/__init__.py
+-rw-r--r--   0        0        0     1737 2024-04-12 09:11:29.068964 python_dev_utils-1.0.6/dev_utils/sqlalchemy/profiling/containers.py
+-rw-r--r--   0        0        0     9776 2024-04-12 09:11:29.069965 python_dev_utils-1.0.6/dev_utils/sqlalchemy/profiling/profilers.py
+-rw-r--r--   0        0        0      951 2024-04-12 09:11:29.068964 python_dev_utils-1.0.6/dev_utils/sqlalchemy/profiling/utils.py
+-rw-r--r--   0        0        0        0 2024-04-10 14:06:40.669620 python_dev_utils-1.0.6/dev_utils/sqlalchemy/types/__init__.py
+-rw-r--r--   0        0        0     2241 2024-04-12 13:02:27.561733 python_dev_utils-1.0.6/dev_utils/sqlalchemy/types/datetime.py
+-rw-r--r--   0        0        0      652 2024-04-11 07:40:31.379144 python_dev_utils-1.0.6/dev_utils/sqlalchemy/types/encryption.py
+-rw-r--r--   0        0        0     1955 2024-04-12 09:11:29.068964 python_dev_utils-1.0.6/dev_utils/sqlalchemy/types/pydantic.py
+-rw-r--r--   0        0        0    12623 2024-04-12 09:11:29.069965 python_dev_utils-1.0.6/dev_utils/sqlalchemy/utils.py
+-rw-r--r--   0        0        0     3005 2024-04-14 10:12:32.389819 python_dev_utils-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-20 07:06:32.612246 python_dev_utils-1.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     9123 2024-04-12 09:01:52.921056 python_dev_utils-1.0.6/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-26 14:08:14.537876 python_dev_utils-1.0.6/tests/core/__init__.py
+-rw-r--r--   0        0        0     2110 2024-04-12 09:01:52.921056 python_dev_utils-1.0.6/tests/core/test_abstract.py
+-rw-r--r--   0        0        0      508 2024-04-12 09:01:52.921056 python_dev_utils-1.0.6/tests/core/test_guards.py
+-rw-r--r--   0        0        0     1040 2024-04-12 09:01:52.921056 python_dev_utils-1.0.6/tests/core/test_results.py
+-rw-r--r--   0        0        0      933 2024-04-12 09:01:52.920056 python_dev_utils-1.0.6/tests/core/test_utils.py
+-rw-r--r--   0        0        0        0 2024-04-11 07:48:56.872907 python_dev_utils-1.0.6/tests/fastapi/__init__.py
+-rw-r--r--   0        0        0     1407 2024-04-12 12:14:52.442153 python_dev_utils-1.0.6/tests/fastapi/conftest.py
+-rw-r--r--   0        0        0      342 2024-04-12 09:01:52.921056 python_dev_utils-1.0.6/tests/fastapi/test_middlewares.py
+-rw-r--r--   0        0        0     6068 2024-04-12 12:24:15.157626 python_dev_utils-1.0.6/tests/fastapi/test_verbose_http_exceptions.py
+-rw-r--r--   0        0        0     2072 2024-04-12 12:18:33.383580 python_dev_utils-1.0.6/tests/fastapi/test_verbose_http_exceptions_handlers.py
+-rw-r--r--   0        0        0      803 2024-04-12 12:23:22.923870 python_dev_utils-1.0.6/tests/fastapi/test_verbose_http_exceptions_utils.py
+-rw-r--r--   0        0        0        0 2024-03-25 06:27:13.006325 python_dev_utils-1.0.6/tests/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:04:52.305307 python_dev_utils-1.0.6/tests/sqlalchemy/filters/__init__.py
+-rw-r--r--   0        0        0    17186 2024-04-12 09:01:52.922056 python_dev_utils-1.0.6/tests/sqlalchemy/filters/test_converters.py
+-rw-r--r--   0        0        0     1210 2024-04-12 09:01:52.921056 python_dev_utils-1.0.6/tests/sqlalchemy/filters/test_guards.py
+-rw-r--r--   0        0        0     7428 2024-04-12 09:01:52.929056 python_dev_utils-1.0.6/tests/sqlalchemy/filters/test_operators.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:04:47.480359 python_dev_utils-1.0.6/tests/sqlalchemy/mixins/__init__.py
+-rw-r--r--   0        0        0     1263 2024-04-10 09:43:27.113285 python_dev_utils-1.0.6/tests/sqlalchemy/mixins/test_audit.py
+-rw-r--r--   0        0        0     1241 2024-04-12 09:01:52.921056 python_dev_utils-1.0.6/tests/sqlalchemy/mixins/test_base.py
+-rw-r--r--   0        0        0     1122 2024-04-12 09:01:52.921056 python_dev_utils-1.0.6/tests/sqlalchemy/mixins/test_general.py
+-rw-r--r--   0        0        0      452 2024-04-12 09:01:52.920056 python_dev_utils-1.0.6/tests/sqlalchemy/mixins/test_ids.py
+-rw-r--r--   0        0        0        0 2024-03-28 08:10:36.944938 python_dev_utils-1.0.6/tests/sqlalchemy/profiling/__init__.py
+-rw-r--r--   0        0        0     3038 2024-04-12 09:01:52.921056 python_dev_utils-1.0.6/tests/sqlalchemy/profiling/test_profilers.py
+-rw-r--r--   0        0        0     1423 2024-04-12 13:01:52.229885 python_dev_utils-1.0.6/tests/sqlalchemy/test_types.py
+-rw-r--r--   0        0        0     7407 2024-04-12 12:47:25.071609 python_dev_utils-1.0.6/tests/sqlalchemy/test_utils.py
+-rw-r--r--   0        0        0      804 2024-04-12 09:01:52.920056 python_dev_utils-1.0.6/tests/types.py
+-rw-r--r--   0        0        0     7467 2024-04-12 13:03:36.658336 python_dev_utils-1.0.6/tests/utils.py
+-rw-r--r--   0        0        0     2481 1970-01-01 00:00:00.000000 python_dev_utils-1.0.6/PKG-INFO
```

### Comparing `python_dev_utils-0.2.0/LICENCE` & `python_dev_utils-1.0.6/LICENCE`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.2.0/README.md` & `python_dev_utils-1.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+
 # Dev utils
 
+![coverage](./coverage.svg)
+
 ## For what?
 
 I made this project to avoid copy-pasting with utils in my projects. I was aiming to simplify
 working with sqlalchemy, FastAPI and other libs.
 
 ## Profiling
```

### Comparing `python_dev_utils-0.2.0/dev_utils/core/abstract.py` & `python_dev_utils-1.0.6/dev_utils/core/abstract.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import Any, Generic, Never, TypeVar, cast
 from warnings import warn
 
 from dev_utils.core.utils import get_object_class_absolute_name
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 class AbstractClassWithoutAbstractPropertiesWarning(Warning):
     """Warning about situation, when class inherited by Abstract, but has no abstract props."""
 
 
 class _AbstractClassProperty(Generic[T]):
     __repr_template: str = (
-        '{cls_path}({property_type_name}) on {containing_klass_name}.{property_name}'
+        "{cls_path}({property_type_name}) on {containing_klass_name}.{property_name}"
     )
     __name__: str
     __containing_klass_name__: str
     __propertytype_name__: str
 
     def __init__(self, propertytype: type[T]) -> None:
         object.__setattr__(self, "__propertytype_name__", str(propertytype))
@@ -112,16 +112,22 @@
     """
     return cast(T, _AbstractClassProperty(propertytype))
 
 
 class Abstract:
     """Abstract class for to use with abstract_class_property."""
 
+    __skip_abstract_raise_error__: bool = False
+
     def __init_subclass__(cls, **kwargs: Any) -> None:  # noqa: ANN401, D105
         super().__init_subclass__(**kwargs)
+        if cls.__skip_abstract_raise_error__:
+            # NOTE: for further inherit.
+            cls.__skip_abstract_raise_error__ = False
+            return
         if Abstract in cls.__bases__:
             for name in dir(cls):
                 if name.startswith("__") and name.endswith("__"):
                     continue
                 if isinstance(getattr(cls, name), _AbstractClassProperty):
                     break
             else:
```

### Comparing `python_dev_utils-0.2.0/dev_utils/core/exc.py` & `python_dev_utils-1.0.6/dev_utils/core/exc.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.2.0/dev_utils/core/logging.py` & `python_dev_utils-1.0.6/dev_utils/core/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,8 +28,8 @@
     "loggers": {
         "dev_utils": {"handlers": ["console"], "level": "INFO"},
     },
 }
 
 
 logging.config.dictConfig(LOGGER_CONFIG)
-logger = logging.getLogger('dev_utils')
+logger = logging.getLogger("dev_utils")
```

### Comparing `python_dev_utils-0.2.0/dev_utils/core/results.py` & `python_dev_utils-1.0.6/dev_utils/core/results.py`

 * *Files identical despite different names*

### Comparing `python_dev_utils-0.2.0/dev_utils/core/utils.py` & `python_dev_utils-1.0.6/dev_utils/core/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
     Absolute name is name with all modules, which this object is contains in. For example,
     we have package ``my_package`` with module ``my_module`` with class ``MyClass``. This Function
     will return ``my_package.my_module.MyClass``
     """
     class_ = obj if inspect.isclass(obj) else obj.__class__
     module = class_.__module__
-    if module == 'builtins':
+    if module == "builtins":
         return class_.__qualname__
-    return module + '.' + class_.__qualname__
+    return module + "." + class_.__qualname__
 
 
 def trim_and_plain_text(text: str) -> str:
     """Make text plain and trim."""
     text = text.strip()
-    while '  ' in text:
-        text = text.replace('  ', ' ')
-    return text.replace('\n', ' ').strip()
+    while "  " in text:
+        text = text.replace("  ", " ")
+    return text.replace("\n", " ").strip()
```

### Comparing `python_dev_utils-0.2.0/dev_utils/profiling/containers.py` & `python_dev_utils-1.0.6/dev_utils/sqlalchemy/profiling/containers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dev_utils.core.utils import get_object_class_absolute_name, trim_and_plain_text
 
 if TYPE_CHECKING:
     from sqlalchemy.engine.cursor import CursorResult
     from sqlalchemy.sql import ClauseElement
     from sqlalchemy.sql.compiler import Compiled
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 class QueryInfo:
     """Data class (not actually has @dataclass decorator) for profiling results.
 
     Contains full info about query itself, but not any additional context.
     """
@@ -22,20 +22,20 @@
         "<class {cls_path} text='{text}' params={params} duration={duration:3f} "
         "rowcount={rowcount}>"
     )
 
     def __init__(
         self,
         *,
-        text: 'ClauseElement | Compiled',
+        text: "ClauseElement | Compiled",
         stack: list[traceback.FrameSummary],
         start_time: float,
         end_time: float,
         params_dict: dict[Any, Any],
-        results: 'CursorResult[Any]',
+        results: "CursorResult[Any]",
     ) -> None:
         self.text = trim_and_plain_text(str(text))
         self.params = params_dict
         self.stack = self.stack_text = stack
         self.start_time = start_time
         self.end_time = end_time
         self.duration = end_time - start_time
```

### Comparing `python_dev_utils-0.2.0/dev_utils/profiling/middlewares.py` & `python_dev_utils-1.0.6/dev_utils/fastapi/middlewares/sqlalchemy_profiling.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from fastapi import FastAPI, Request
 from sqlalchemy import Engine
 from starlette.middleware.base import RequestResponseEndpoint
 from starlette.responses import Response
 
 from dev_utils.core.logging import logger as default_logger
-from dev_utils.profiling import profilers
+from dev_utils.sqlalchemy.profiling.profilers import SQLAlchemyQueryCounter, SQLAlchemyQueryProfiler
 
 
 def add_query_profiling_middleware(
     app: FastAPI,
     engine: Engine | type[Engine] = Engine,
     *,
     profiler_id: str | None = None,
@@ -26,24 +26,24 @@
     version.
     """
 
     async def _profiling_middleware(
         request: Request,
         call_next: RequestResponseEndpoint,
     ) -> Response:
-        with profilers.SQLAlchemyQueryProfiler(
+        with SQLAlchemyQueryProfiler(
             engine=engine,
             profiler_id=profiler_id,
             logger=logger,
             log_query_states=log_query_stats,
         ) as profiler:
-            logger.info('Profiler %s: start profiling %s', profiler.profiler_id, request.url)
+            logger.info("Profiler %s: start profiling %s", profiler.profiler_id, request.url)
             response = await call_next(request)
         profiler.report(report_to)
-        logger.info('Profiler %s finished.', profiler.profiler_id)
+        logger.info("Profiler %s finished.", profiler.profiler_id)
         return response
 
     app.middleware("http")(_profiling_middleware)
     return app
 
 
 def add_query_counter_middleware(
@@ -61,28 +61,28 @@
     version.
     """
 
     async def _counter_middleware(
         request: Request,
         call_next: RequestResponseEndpoint,
     ) -> Response:
-        with profilers.SQLAlchemyQueryCounter(
+        with SQLAlchemyQueryCounter(
             engine=engine,
             profiler_id=profiler_id,
             logger=logger,
             log_query_states=log_query_stats,
         ) as profiler:
             logger.info(
-                'Counter %s: start counting queries for %s',
+                "Counter %s: start counting queries for %s",
                 profiler.profiler_id,
                 request.url,
             )
             response = await call_next(request)
         logger.info(
-            'Counter: %s. Count of queries for %s: %s',
+            "Counter: %s. Count of queries for %s: %s",
             profiler.profiler_id,
             request.url,
             profiler.collect(),
         )
         return response
 
     app.middleware("http")(_counter_middleware)
```

### Comparing `python_dev_utils-0.2.0/dev_utils/profiling/profilers.py` & `python_dev_utils-1.0.6/dev_utils/sqlalchemy/profiling/profilers.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,40 +13,40 @@
 from sqlalchemy import event
 from sqlalchemy.engine import Engine
 from sqlalchemy.ext.asyncio import AsyncEngine
 
 from dev_utils.core.guards import all_dict_keys_are_str
 from dev_utils.core.logging import logger as default_logger
 from dev_utils.core.utils import trim_and_plain_text
-from dev_utils.profiling.containers import QueryInfo
-from dev_utils.profiling.utils import pretty_query_info
+from dev_utils.sqlalchemy.profiling.containers import QueryInfo
+from dev_utils.sqlalchemy.profiling.utils import pretty_query_info
 
 if TYPE_CHECKING:
     from sqlalchemy.engine import Connection
     from sqlalchemy.engine.cursor import CursorResult
     from sqlalchemy.sql import ClauseElement
     from sqlalchemy.sql.compiler import SQLCompiler
     from sqlalchemy.util import immutabledict
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 class BaseSQLAlchemyProfiler(ABC, Generic[T]):
     """Abstract base sqlalchemy profiling class.
 
     It is a generic class, so use it with typing. Generic uses in:
 
     * ``__init__``: self.collector - queue of ``<Generic>`` objects. For example, it could be
         queue of QueryInfo objects.
     * ``collect``: return value - Sequence of ``<Generic>``.
     """
 
     def __init__(
         self,
-        engine: 'type[Engine] | Engine | AsyncEngine' = Engine,
+        engine: "type[Engine] | Engine | AsyncEngine" = Engine,
         *,
         profiler_id: str | None = None,
         logger: Logger = default_logger,
         log_query_states: bool = False,
     ) -> None:
         self.started = False
         if isinstance(engine, AsyncEngine):
@@ -60,44 +60,44 @@
 
         self._result: T | None = None
         self.collector: queue.Queue[T] = queue.Queue()
 
     @abstractmethod
     def _before_exec(
         self,
-        conn: 'Connection',
-        clause: 'SQLCompiler',
-        multiparams: 'Sequence[Mapping[str, Any]]',  # noqa: F841
-        params: 'Mapping[str, Any]',
-        execution_options: 'immutabledict[str, Any]',  # noqa: F841
+        conn: "Connection",
+        clause: "SQLCompiler",
+        multiparams: "Sequence[Mapping[str, Any]]",  # noqa: F841
+        params: "Mapping[str, Any]",
+        execution_options: "immutabledict[str, Any]",  # noqa: F841
     ) -> None:
         """Method, which will be bounded to `before_execute` handler in SQLAlchemy."""  # noqa: D401
         raise NotImplementedError()
 
     @abstractmethod
     def _after_exec(
         self,
-        conn: 'Connection',
-        clause: 'ClauseElement',
-        multiparams: 'Sequence[Mapping[str, Any]]',  # noqa: F841
-        params: 'Mapping[str, Any]',
-        execution_options: 'immutabledict[str, Any]',  # noqa: F841
-        results: 'CursorResult[Any]',
+        conn: "Connection",
+        clause: "ClauseElement",
+        multiparams: "Sequence[Mapping[str, Any]]",  # noqa: F841
+        params: "Mapping[str, Any]",
+        execution_options: "immutabledict[str, Any]",  # noqa: F841
+        results: "CursorResult[Any]",
     ) -> None:
         """Method, which will be bounded to `after_execute` handler in SQLAlchemy."""  # noqa: D401
         raise NotImplementedError()
 
     @final
     def _extract_parameters_from_results(
         self,
-        query_results: 'CursorResult[Any]',
+        query_results: "CursorResult[Any]",
     ) -> dict[str, Any]:
         """Get parameters from query results object."""
         params_dict: dict[str, Any] = {}
-        compiled_parameters = getattr(query_results.context, 'compiled_parameters', [])
+        compiled_parameters = getattr(query_results.context, "compiled_parameters", [])
         if not compiled_parameters or not isinstance(  # pragma: no cover
             compiled_parameters,
             Sequence,
         ):
             return {}
         for compiled_param_dict in compiled_parameters:
             if not isinstance(compiled_param_dict, dict):  # pragma: no cover
@@ -166,54 +166,54 @@
         queries: list[T] = []
         with suppress(queue.Empty):
             while True:
                 queries.append(self.collector.get(block=False))
 
         return queries
 
-    def report(self, stdout: 'str | Path | Logger | None' = None) -> None:  # noqa: F841
+    def report(self, stdout: "str | Path | Logger | None" = None) -> None:  # noqa: F841
         """Make report about profiling."""
         return  # pragma: no coverage
 
 
 class SQLAlchemyQueryProfiler(BaseSQLAlchemyProfiler[QueryInfo]):
     """SQLAlchemy query profiler."""
 
     def _before_exec(
         self,
-        conn: 'Connection',
-        clause: 'SQLCompiler',
-        multiparams: 'Sequence[Mapping[str, Any]]',  # noqa: F841
-        params: 'Mapping[str, Any]',
-        execution_options: 'immutabledict[str, Any]',  # noqa: F841
+        conn: "Connection",
+        clause: "SQLCompiler",
+        multiparams: "Sequence[Mapping[str, Any]]",  # noqa: F841
+        params: "Mapping[str, Any]",
+        execution_options: "immutabledict[str, Any]",  # noqa: F841
     ) -> None:
         conn.info.setdefault("query_start_time", []).append(time.time())
         if self.log_query_states:  # pragma: no cover
             msg = (
-                f'Profiler {self.profiler_id}. '
-                f'Query started: {trim_and_plain_text(str(clause))}. Params: {params}'
+                f"Profiler {self.profiler_id}. "
+                f"Query started: {trim_and_plain_text(str(clause))}. Params: {params}"
             )
             self.logger.info(msg)
 
     def _after_exec(
         self,
-        conn: 'Connection',
-        clause: 'ClauseElement',
-        multiparams: 'Sequence[Mapping[str, Any]]',  # noqa: F841
-        params: 'Mapping[str, Any]',
-        execution_options: 'immutabledict[str, Any]',  # noqa: F841
-        results: 'CursorResult[Any]',
+        conn: "Connection",
+        clause: "ClauseElement",
+        multiparams: "Sequence[Mapping[str, Any]]",  # noqa: F841
+        params: "Mapping[str, Any]",
+        execution_options: "immutabledict[str, Any]",  # noqa: F841
+        results: "CursorResult[Any]",
     ) -> None:
         end_time = time.time()
         start_time = conn.info["query_start_time"].pop(-1)
         if self.log_query_states:  # pragma: no cover
             msg = (
-                f'Profiler {self.profiler_id}. '
+                f"Profiler {self.profiler_id}. "
                 f'Query "{trim_and_plain_text(str(clause))}" (params: {params}) '
-                f'finished in {(end_time - start_time) * 1000} milliseconds.'
+                f"finished in {(end_time - start_time) * 1000} milliseconds."
             )
             self.logger.info(msg)
 
         text = clause
         with suppress(AttributeError):
             text = clause.compile(dialect=conn.engine.dialect)
 
@@ -234,46 +234,46 @@
     def report(self, stdout: str | Path | Logger | None = None) -> None:  # noqa: D102
         if not stdout:  # pragma: no coverage
             stdout = self.logger
         data = pretty_query_info(self.collect())
         if isinstance(stdout, Logger):
             stdout.info(data)
             return
-        with Path(stdout).open('a') as writer:
+        with Path(stdout).open("a") as writer:
             writer.write(data)
 
 
 class SQLAlchemyQueryCounter(BaseSQLAlchemyProfiler[int]):
     """SQLAlchemy query counter."""
 
     def collect(self) -> int:  # type: ignore  # noqa: D102
         if self._result is None:  # pragma: no cover
             return 0
         return self._result
 
     def _before_exec(
         self,
-        conn: 'Connection',
-        clause: 'SQLCompiler',
-        multiparams: 'Sequence[Mapping[str, Any]]',  # noqa: F841
-        params: 'Mapping[str, Any]',
-        execution_options: 'immutabledict[str, Any]',  # noqa: F841
+        conn: "Connection",
+        clause: "SQLCompiler",
+        multiparams: "Sequence[Mapping[str, Any]]",  # noqa: F841
+        params: "Mapping[str, Any]",
+        execution_options: "immutabledict[str, Any]",  # noqa: F841
     ) -> None:
         if self._result is None:  # pragma: no cover
             self._result = 0
         self._result += 1
 
     def _after_exec(
         self,
-        conn: 'Connection',
-        clause: 'ClauseElement',
-        multiparams: 'Sequence[Mapping[str, Any]]',  # noqa: F841
-        params: 'Mapping[str, Any]',
-        execution_options: 'immutabledict[str, Any]',  # noqa: F841
-        results: 'CursorResult[Any]',
+        conn: "Connection",
+        clause: "ClauseElement",
+        multiparams: "Sequence[Mapping[str, Any]]",  # noqa: F841
+        params: "Mapping[str, Any]",
+        execution_options: "immutabledict[str, Any]",  # noqa: F841
+        results: "CursorResult[Any]",
     ) -> None:
         pass
 
     def start(self) -> None:  # noqa: D102
         if not self.started:  # pragma: no cover
             self._result = 0
         return super().start()
```

### Comparing `python_dev_utils-0.2.0/dev_utils/profiling/utils.py` & `python_dev_utils-1.0.6/dev_utils/sqlalchemy/profiling/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from collections.abc import Sequence
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from dev_utils.profiling.containers import QueryInfo
+    from dev_utils.sqlalchemy.profiling.containers import QueryInfo
 
 
-def pretty_query_info(info: 'QueryInfo | Sequence[QueryInfo]') -> str:  # pragma: no coverage
+def pretty_query_info(info: "QueryInfo | Sequence[QueryInfo]") -> str:  # pragma: no coverage
     """Pretty text from QueryInfo.
 
     Make string from information to log it.
     """
     query_template = (
-        'index: {query_index}\n'
-        'query text: {query_text}\n'
-        'query params: {query_params}\n'
-        'query duration: {query_duration}\n'
-        'query rowcount (may be incorrect): {query_rowcount}\n'
+        "index: {query_index}\n"
+        "query text: {query_text}\n"
+        "query params: {query_params}\n"
+        "query duration: {query_duration}\n"
+        "query rowcount (may be incorrect): {query_rowcount}\n"
     )
     if not isinstance(info, Sequence):
         info = [info]
-    return '\n'.join(
+    return "\n".join(
         query_template.format(
             query_index=idx,
             query_text=query.text,
             query_params=query.params,
             query_duration=query.duration,
             query_rowcount=query.rowcount,
         )
```

### Comparing `python_dev_utils-0.2.0/dev_utils/sqlalchemy/filters/converters.py` & `python_dev_utils-1.0.6/dev_utils/sqlalchemy/filters/converters.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,22 +35,22 @@
 NestedFilterNames = set[str]
 LookupMapping = dict[enum.Enum | str, OperatorFunction]
 LookupMappingWithNested = dict[enum.Enum | str, tuple[OperatorFunction, NestedFilterNames]]
 AnyLookupMapping = LookupMapping | LookupMappingWithNested
 
 empty_nested_filter_names: NestedFilterNames = set()
 django_nested_filter_names: NestedFilterNames = {
-    'exact',
-    'iexact',
-    'in',
-    'gt',
-    'gte',
-    'lt',
-    'lte',
-    'range',
+    "exact",
+    "iexact",
+    "in",
+    "gt",
+    "gte",
+    "lt",
+    "lte",
+    "range",
 }
 
 
 def execute_operator_function(  # noqa: ANN201
     func: OperatorFunction,
     a: Any,  # noqa: ANN401
     b: Any,  # noqa: ANN401
@@ -58,15 +58,15 @@
 ):
     """Call given operator function with checking for ``subproduct_use`` signature.
 
     Simple wrapper to not execute function every time with checking, that operator has
     subproduct_use.
     """
     function_signature = signature(func)
-    if function_signature.parameters.get('subproduct_use'):
+    if function_signature.parameters.get("subproduct_use"):
         return func(a, b, subproduct_use=subproduct_use)
     # function has no subproduct_use param.
     return func(a, b)
 
 
 class BaseFilterConverter(ABC, Abstract):
     """Base class for filter converters."""
@@ -162,24 +162,24 @@
             filters = [filters]
         for filter_ in filters:
             if isinstance(filter_, ColumnElement):
                 result.append(filter_)
                 continue
             is_valid, message = cls._is_filter_valid(model, filter_)
             if not is_valid:
-                msg = f'Filter with data {filter_} is not valid: {message}'
+                msg = f"Filter with data {filter_} is not valid: {message}"
                 raise FilterError(msg)
             result.extend(cls._convert_filter(model, filter_))
         return result
 
     @classmethod
     @final
     def _recursive_apply_operator(
         cls,
-        model: 'type[DeclarativeBase]',
+        model: "type[DeclarativeBase]",
         field_name: str,
         parent_lookup: str,
         value: Any,  # noqa: ANN401
         rest_lookups: list[str] | None = None,
     ) -> SQLAlchemyFilter:
         """Apply operator to SQLAlchemy field and value.
 
@@ -239,15 +239,15 @@
         cls,
         model: type["DeclarativeBase"],
         filter_: FilterDict,
     ) -> tuple[IsValid, Message]:
         for field_name in filter_:
             if field_name not in get_valid_field_names(model):
                 return False, f'Model or select statement {model} has no field "{field_name}".'
-        return True, ''
+        return True, ""
 
     @classmethod
     def _convert_filter(
         cls,
         model: type["DeclarativeBase"],
         filter_: FilterDict,
     ) -> Sequence[SQLAlchemyFilter]:
@@ -270,53 +270,53 @@
             "value": "Any value of any type.",
             "operator": "== (Can one of the available (see schemas of lookup_mapping)).",
         }
     ```
     """
 
     lookup_mapping: LookupMapping = {  # type: ignore
-        '=': builtin_operator.eq,
-        '>': builtin_operator.gt,
-        '<': builtin_operator.lt,
-        '>=': builtin_operator.ge,
-        '<=': builtin_operator.le,
-        'is': custom_operator.is_,
-        'is_not': custom_operator.is_not,
-        'between': custom_operator.between,
-        'contains': custom_operator.contains,
+        "=": builtin_operator.eq,
+        ">": builtin_operator.gt,
+        "<": builtin_operator.lt,
+        ">=": builtin_operator.ge,
+        "<=": builtin_operator.le,
+        "is": custom_operator.is_,
+        "is_not": custom_operator.is_not,
+        "between": custom_operator.between,
+        "contains": custom_operator.contains,
         # TODO: add values validation for operators.
         # For example, for between - only two values in Sequence, otherwise FilterError.
     }
 
     @classmethod
     def _is_filter_valid(
         cls,
         model: type["DeclarativeBase"],
         filter_: FilterDict,
     ) -> tuple[IsValid, Message]:
         if not is_dict_simple_filter_dict(filter_):
-            return False, 'filter dict is not subtype of OperatorFilterDict.'
-        field = filter_['field']
+            return False, "filter dict is not subtype of OperatorFilterDict."
+        field = filter_["field"]
         if field not in get_valid_field_names(model):
             return False, f'Model or select statement {model} has no field "{field}".'
-        return True, ''
+        return True, ""
 
     @classmethod
     def _convert_filter(
         cls,
         model: type["DeclarativeBase"],
         filter_: FilterDict,
-    ) -> 'Sequence[SQLAlchemyFilter]':
+    ) -> "Sequence[SQLAlchemyFilter]":
         if not is_dict_simple_filter_dict(filter_):
             msg = "Never situation. Don't use _convert_filter method directly!"
             raise FilterError(msg)
-        operator_str = filter_.get('operator', '=')
+        operator_str = filter_.get("operator", "=")
         operator_func = cls.lookup_mapping[operator_str]
-        sqlalchemy_field = get_sqlalchemy_attribute(model, filter_['field'])
-        return [operator_func(sqlalchemy_field, filter_['value'])]
+        sqlalchemy_field = get_sqlalchemy_attribute(model, filter_["field"])
+        return [operator_func(sqlalchemy_field, filter_["value"])]
 
 
 class DjangoLikeFilterConverter(BaseFilterConverter):
     """Django filters adapter for SQLAlchemy.
 
     Attention (1)!
     --------------
@@ -327,91 +327,91 @@
     Attention (2)!
     --------------
     Not production ready. Tested only by pytest (no manual tests in other
     projects).
     """
 
     lookup_mapping: LookupMappingWithNested = {  # type: ignore
-        'exact': (custom_operator.django_exact, empty_nested_filter_names),
-        'iexact': (custom_operator.django_iexact, empty_nested_filter_names),
-        'contains': (custom_operator.django_contains, empty_nested_filter_names),
-        'icontains': (custom_operator.django_icontains, empty_nested_filter_names),
-        'in': (custom_operator.django_in, empty_nested_filter_names),
-        'gt': (builtin_operator.gt, empty_nested_filter_names),
-        'gte': (builtin_operator.ge, empty_nested_filter_names),
-        'lt': (builtin_operator.lt, empty_nested_filter_names),
-        'lte': (builtin_operator.le, empty_nested_filter_names),
-        'startswith': (custom_operator.django_startswith, empty_nested_filter_names),
-        'istartswith': (custom_operator.django_istartswith, empty_nested_filter_names),
-        'endswith': (custom_operator.django_endswith, empty_nested_filter_names),
-        'iendswith': (custom_operator.django_iendswith, empty_nested_filter_names),
-        'range': (custom_operator.django_range, empty_nested_filter_names),
-        'date': (custom_operator.django_date, django_nested_filter_names),
-        'year': (custom_operator.django_year, django_nested_filter_names),
-        'iso_year': (custom_operator.django_iso_year, django_nested_filter_names),
-        'month': (custom_operator.django_month, django_nested_filter_names),
-        'day': (custom_operator.django_day, django_nested_filter_names),
-        'week': (custom_operator.django_week, django_nested_filter_names),
-        'week_day': (custom_operator.django_week_day, django_nested_filter_names),
-        'iso_week_day': (custom_operator.django_iso_week_day, django_nested_filter_names),
-        'quarter': (custom_operator.django_quarter, django_nested_filter_names),
-        'time': (custom_operator.django_time, django_nested_filter_names),
-        'hour': (custom_operator.django_hour, django_nested_filter_names),
-        'minute': (custom_operator.django_minute, django_nested_filter_names),
-        'second': (custom_operator.django_second, django_nested_filter_names),
-        'isnull': (custom_operator.django_isnull, empty_nested_filter_names),
-        'regex': (custom_operator.django_regex, empty_nested_filter_names),
-        'iregex': (custom_operator.django_iregex, empty_nested_filter_names),
+        "exact": (custom_operator.django_exact, empty_nested_filter_names),
+        "iexact": (custom_operator.django_iexact, empty_nested_filter_names),
+        "contains": (custom_operator.django_contains, empty_nested_filter_names),
+        "icontains": (custom_operator.django_icontains, empty_nested_filter_names),
+        "in": (custom_operator.django_in, empty_nested_filter_names),
+        "gt": (builtin_operator.gt, empty_nested_filter_names),
+        "gte": (builtin_operator.ge, empty_nested_filter_names),
+        "lt": (builtin_operator.lt, empty_nested_filter_names),
+        "lte": (builtin_operator.le, empty_nested_filter_names),
+        "startswith": (custom_operator.django_startswith, empty_nested_filter_names),
+        "istartswith": (custom_operator.django_istartswith, empty_nested_filter_names),
+        "endswith": (custom_operator.django_endswith, empty_nested_filter_names),
+        "iendswith": (custom_operator.django_iendswith, empty_nested_filter_names),
+        "range": (custom_operator.django_range, empty_nested_filter_names),
+        "date": (custom_operator.django_date, django_nested_filter_names),
+        "year": (custom_operator.django_year, django_nested_filter_names),
+        "iso_year": (custom_operator.django_iso_year, django_nested_filter_names),
+        "month": (custom_operator.django_month, django_nested_filter_names),
+        "day": (custom_operator.django_day, django_nested_filter_names),
+        "week": (custom_operator.django_week, django_nested_filter_names),
+        "week_day": (custom_operator.django_week_day, django_nested_filter_names),
+        "iso_week_day": (custom_operator.django_iso_week_day, django_nested_filter_names),
+        "quarter": (custom_operator.django_quarter, django_nested_filter_names),
+        "time": (custom_operator.django_time, django_nested_filter_names),
+        "hour": (custom_operator.django_hour, django_nested_filter_names),
+        "minute": (custom_operator.django_minute, django_nested_filter_names),
+        "second": (custom_operator.django_second, django_nested_filter_names),
+        "isnull": (custom_operator.django_isnull, empty_nested_filter_names),
+        "regex": (custom_operator.django_regex, empty_nested_filter_names),
+        "iregex": (custom_operator.django_iregex, empty_nested_filter_names),
     }
 
     @classmethod
     def _is_filter_valid(
         cls,
         model: type["DeclarativeBase"],
         filter_: FilterDict,
     ) -> tuple[IsValid, Message]:
         for field in filter_:
-            field_parts = field.split('__')
+            field_parts = field.split("__")
             if len(field_parts) == 1:
                 field_name = field_parts[0]
-                lookup = 'exact'
+                lookup = "exact"
                 rest_lookups: list[str] = []
             else:
                 field_name, lookup, *rest_lookups = field_parts
             if not all(rest_lookup in cls.lookup_mapping for rest_lookup in rest_lookups):
-                rest_lookups_str = ', '.join(rest_lookups)
+                rest_lookups_str = ", ".join(rest_lookups)
                 msg = (
-                    f'Not all sub-lookups ({rest_lookups_str}) are in cls.lookup_mapping keys. '
-                    'Perhaps, you tried to pass related model name to filter by it. Not it is not '
-                    'possible. Use sub-lookups only for filtering inside main model (like '
-                    'field__hour__gt=12 or something like this)'
+                    f"Not all sub-lookups ({rest_lookups_str}) are in cls.lookup_mapping keys. "
+                    "Perhaps, you tried to pass related model name to filter by it. Not it is not "
+                    "possible. Use sub-lookups only for filtering inside main model (like "
+                    "field__hour__gt=12 or something like this)"
                 )
                 raise FilterError(msg)
             # FIXME: add validation for value for lookup (like, no integer for field__date filter)
             if field_name not in get_valid_field_names(model):
                 return False, f'Model or select statement {model} has no field "{field_name}".'
             if lookup not in cls.lookup_mapping:
                 all_lookup_mapping = list(cls.lookup_mapping.keys())
-                message = f'Unexpected lookup "{lookup}".' f'Valid lookups: {all_lookup_mapping}.'
+                message = f'Unexpected lookup "{lookup}".' f"Valid lookups: {all_lookup_mapping}."
                 return False, message
-        return True, ''
+        return True, ""
 
     @classmethod
     def _convert_filter(
         cls,
         model: type["DeclarativeBase"],
         filter_: FilterDict,
     ) -> Sequence[SQLAlchemyFilter]:
         sqlalchemy_filters: Sequence[SQLAlchemyFilter] = []
         for field, value in filter_.items():
-            field_parts = field.split('__')
+            field_parts = field.split("__")
             # TODO: add filtering by relationships.
             if len(field_parts) == 1:
                 field_name = field_parts[0]
-                lookup = 'exact'
+                lookup = "exact"
                 rest_lookups: list[str] = []
             else:
                 field_name, lookup, *rest_lookups = field_parts
             sqlalchemy_filters.append(
                 cls._recursive_apply_operator(
                     model=model,
                     field_name=field_name,
```

### Comparing `python_dev_utils-0.2.0/dev_utils/sqlalchemy/filters/guards.py` & `python_dev_utils-1.0.6/dev_utils/sqlalchemy/filters/guards.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,41 +7,39 @@
 
 from dev_utils.sqlalchemy.filters.types import AdvancedOperatorsSet, OperatorFilterDict
 
 if TYPE_CHECKING:
     from dev_utils.sqlalchemy.filters.converters import AnyLookupMapping, LookupMappingWithNested
 
 
-def is_dict_simple_filter_dict(value: dict[Any, Any]) -> TypeGuard['OperatorFilterDict']:
+def is_dict_simple_filter_dict(value: dict[Any, Any]) -> TypeGuard["OperatorFilterDict"]:
     """TypeGuard for checking dict is ``OperatorFilterDict`` (typed dict) instance.
 
     OperatorFilterDict should has ``field``, ``value``, and ``operator`` keys with validated values:
 
     ``field``: any string.
     ``value``: any value.
     ``operator``: any string of ``AdvancedOperatorsLiteral``.
     """
-    if 'field' not in value or not isinstance(value['field'], str):
+    if "field" not in value or not isinstance(value["field"], str):
         return False
-    if 'value' not in value:
+    if "value" not in value:
         return False
-    if 'operator' in value and value['operator'] not in AdvancedOperatorsSet:
+    if "operator" in value and value["operator"] not in AdvancedOperatorsSet:
         return False
     return True
 
 
-def has_nested_lookups(mapping: 'AnyLookupMapping') -> TypeGuard['LookupMappingWithNested']:
+def has_nested_lookups(mapping: "AnyLookupMapping") -> TypeGuard["LookupMappingWithNested"]:
     """TypeGuard for specify converter mapping type with nested lookups.
 
     By default, all mappings can has either operator function or tuple of operator function and
     available sub-lookups set.
     """
     if not mapping:
         return False
     for value in mapping.values():
         if (
-            not isinstance(value, tuple)
-            or len(value) != 2
-            or not isinstance(value[1], set)  # type: ignore
+            not isinstance(value, tuple) or len(value) != 2 or not isinstance(value[1], set)  # type: ignore
         ):
             return False
     return True
```

### Comparing `python_dev_utils-0.2.0/dev_utils/sqlalchemy/filters/operators.py` & `python_dev_utils-1.0.6/dev_utils/sqlalchemy/filters/operators.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from sqlalchemy.orm import QueryableAttribute
 
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     from sqlalchemy.sql.elements import ColumnElement
 
-    T = TypeVar('T')
+    T = TypeVar("T")
 
 
 class OperatorFunctionProtocol(Protocol):  # noqa: D101
     def __call__(  # noqa: D102
         self,
         a: Any,  # noqa: ANN401
         b: Any,  # noqa: ANN401
@@ -45,330 +45,330 @@
     """Real do nothing function.
 
     Return None, receive any parameters.
     """
     return None
 
 
-def return_value(value: 'T') -> 'T':
+def return_value(value: "T") -> "T":
     """Return value, passed into it."""
     return value
 
 
 def is_(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: Any,  # noqa
-) -> 'ColumnElement[bool]':
+) -> "ColumnElement[bool]":
     """SQLAlchemy ``a.is_(b)`` alias."""
     return a.is_(b)
 
 
 def is_not(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: Any,  # noqa
-) -> 'ColumnElement[bool]':
+) -> "ColumnElement[bool]":
     """SQLAlchemy ``a.is_not(b)`` alias."""
     return a.is_not(b)
 
 
 def between(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: tuple[Any, Any],
-) -> 'ColumnElement[bool]':
+) -> "ColumnElement[bool]":
     """SQLAlchemy ``a.between(b_1, b_2)`` alias.
 
     Also check [] b length (if not equals 2, then force return false statement).
     """
     if len(b) != 2:
         return false()
     return a.between(*b)
 
 
 def contains(
     a: QueryableAttribute[Any],  # noqa: ANN401
-    b: 'Sequence[Any]',
-) -> 'ColumnElement[bool]':
+    b: "Sequence[Any]",
+) -> "ColumnElement[bool]":
     """SQLALchemy ``a.in_(b)`` alias."""
     return a.in_(b)
 
 
 # =================================================================
 # |                       DJANGO OPERATORS                        |
 # =================================================================
 
 
 def django_exact(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: Any,  # noqa: ANN401
-) -> 'ColumnElement[bool]':
+) -> "ColumnElement[bool]":
     """Django to SQLAlchemy adapter of ``exact`` lookup."""
     if b is None or isinstance(b, bool):
         return a.is_(None)
     return a == b
 
 
 def django_iexact(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: Any,  # noqa
-) -> 'ColumnElement[bool]':
+) -> "ColumnElement[bool]":
     """Django to SQLAlchemy adapter of ``iexact`` lookup."""
     if b is None or isinstance(b, bool):
         return a.is_(None)
     if isinstance(b, str):
         return a.ilike(b)
     return a == b
 
 
 def django_contains(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: Any,  # noqa: ANN401
-) -> 'ColumnElement[bool]':
+) -> "ColumnElement[bool]":
     """Django to SQLAlchemy adapter of ``contains`` lookup."""
     if isinstance(b, str):
-        b = f'%{b}%'
+        b = f"%{b}%"
     return a.like(b)
 
 
 def django_icontains(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: Any,  # noqa: ANN401
-) -> 'ColumnElement[bool]':
+) -> "ColumnElement[bool]":
     """Django to SQLAlchemy adapter of ``icontains`` lookup."""
     if isinstance(b, str):
-        b = f'%{b}%'
+        b = f"%{b}%"
     return a.ilike(b)
 
 
 def django_in(
     a: QueryableAttribute[Any],  # noqa: ANN401
-    b: 'Sequence[Any]',
-) -> 'ColumnElement[bool]':
+    b: "Sequence[Any]",
+) -> "ColumnElement[bool]":
     """Django to SQLAlchemy adapter of ``in`` lookup."""
     return a.in_(b)
 
 
 def django_startswith(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: Any,  # noqa: ANN401
-) -> 'ColumnElement[bool]':
+) -> "ColumnElement[bool]":
     """Django to SQLAlchemy adapter of ``startswith`` lookup."""
     if isinstance(b, str):
-        b = f'{b}%'
+        b = f"{b}%"
     return a.like(b)
 
 
 def django_istartswith(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: Any,  # noqa: ANN401
-) -> 'ColumnElement[bool]':
+) -> "ColumnElement[bool]":
     """Django to SQLAlchemy adapter of ``istartswith`` lookup."""
     if isinstance(b, str):
-        b = f'{b}%'
+        b = f"{b}%"
     return a.ilike(b)
 
 
 def django_endswith(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: Any,  # noqa: ANN401
-) -> 'ColumnElement[bool]':
+) -> "ColumnElement[bool]":
     """Django to SQLAlchemy adapter of ``endswith`` lookup."""
     if isinstance(b, str):
-        b = f'%{b}'
+        b = f"%{b}"
     return a.like(b)
 
 
 def django_iendswith(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: Any,  # noqa: ANN401
-) -> 'ColumnElement[bool]':
+) -> "ColumnElement[bool]":
     """Django to SQLAlchemy adapter of ``iendswith`` lookup."""
     if isinstance(b, str):
-        b = f'%{b}'
+        b = f"%{b}"
     return a.ilike(b)
 
 
 def django_range(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: tuple[Any, Any],
-) -> 'ColumnElement[bool]':
+) -> "ColumnElement[bool]":
     """Django to SQLAlchemy adapter of ``range`` lookup."""
     return between(a, b)
 
 
 def django_date(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: datetime.date,
     *,
     subproduct_use: bool = False,
-) -> 'ColumnElement[Any]':
+) -> "ColumnElement[Any]":
     """Django to SQLAlchemy adapter of ``date`` lookup."""
     if subproduct_use:
         return cast(a, Date)
     return cast(a, Date) == b
 
 
 def django_year(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: int | str,
     *,
     subproduct_use: bool = False,
-) -> 'ColumnElement[Any]':
+) -> "ColumnElement[Any]":
     """Django to SQLAlchemy adapter of ``year`` lookup."""
     if subproduct_use:
-        return extract('year', a)
-    return extract('year', a) == b
+        return extract("year", a)
+    return extract("year", a) == b
 
 
 def django_iso_year(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: int | str,
     *,
     subproduct_use: bool = False,
-) -> 'ColumnElement[Any]':
+) -> "ColumnElement[Any]":
     """Django to SQLAlchemy adapter of ``iso_year`` lookup."""
     if subproduct_use:
-        return extract('isoyear', a)
-    return extract('isoyear', a) == b
+        return extract("isoyear", a)
+    return extract("isoyear", a) == b
 
 
 def django_month(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: int | str,
     *,
     subproduct_use: bool = False,
-) -> 'ColumnElement[Any]':
+) -> "ColumnElement[Any]":
     """Django to SQLAlchemy adapter of ``month`` lookup."""
     if subproduct_use:
-        return extract('month', a)
-    return extract('month', a) == b
+        return extract("month", a)
+    return extract("month", a) == b
 
 
 def django_day(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: int | str,
     *,
     subproduct_use: bool = False,
-) -> 'ColumnElement[Any]':
+) -> "ColumnElement[Any]":
     """Django to SQLAlchemy adapter of ``day`` lookup."""
     if subproduct_use:
-        return extract('day', a)
-    return extract('day', a) == b
+        return extract("day", a)
+    return extract("day", a) == b
 
 
 def django_week(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: int | str,
     *,
     subproduct_use: bool = False,
-) -> 'ColumnElement[Any]':
+) -> "ColumnElement[Any]":
     """Django to SQLAlchemy adapter of ``week`` lookup."""
     if subproduct_use:
-        return extract('week', a)
-    return extract('week', a) == b
+        return extract("week", a)
+    return extract("week", a) == b
 
 
 def django_week_day(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: int | str,
     *,
     subproduct_use: bool = False,
-) -> 'ColumnElement[Any]':
+) -> "ColumnElement[Any]":
     """Django to SQLAlchemy adapter of ``week_day`` lookup."""
     if subproduct_use:
-        return extract('dow', a)
-    return extract('dow', a) == b
+        return extract("dow", a)
+    return extract("dow", a) == b
 
 
 def django_iso_week_day(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: int | str,
     *,
     subproduct_use: bool = False,
-) -> 'ColumnElement[Any]':
+) -> "ColumnElement[Any]":
     """Django to SQLAlchemy adapter of ``iso_week_day`` lookup."""
     if subproduct_use:
-        return extract('isodow', a)
-    return extract('isodow', a) == b
+        return extract("isodow", a)
+    return extract("isodow", a) == b
 
 
 def django_quarter(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: int | str,
     *,
     subproduct_use: bool = False,
-) -> 'ColumnElement[Any]':
+) -> "ColumnElement[Any]":
     """Django to SQLAlchemy adapter of ``quarter`` lookup."""
     if subproduct_use:
-        return extract('quarter', a)
-    return extract('quarter', a) == b
+        return extract("quarter", a)
+    return extract("quarter", a) == b
 
 
 def django_time(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: datetime.time,
     *,
     subproduct_use: bool = False,
-) -> 'ColumnElement[Any]':
+) -> "ColumnElement[Any]":
     """Django to SQLAlchemy adapter of ``time`` lookup."""
     if subproduct_use:
         return cast(a, Time)
     return cast(a, Time) == b
 
 
 def django_hour(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: int,
     *,
     subproduct_use: bool = False,
-) -> 'ColumnElement[Any]':
+) -> "ColumnElement[Any]":
     """Django to SQLAlchemy adapter of ``hour`` lookup."""
     if subproduct_use:
-        return extract('hour', a)
-    return extract('hour', a) == b
+        return extract("hour", a)
+    return extract("hour", a) == b
 
 
 def django_minute(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: int,
     *,
     subproduct_use: bool = False,
-) -> 'ColumnElement[Any]':
+) -> "ColumnElement[Any]":
     """Django to SQLAlchemy adapter of ``minute`` lookup."""
     if subproduct_use:
-        return extract('minute', a)
-    return extract('minute', a) == b
+        return extract("minute", a)
+    return extract("minute", a) == b
 
 
 def django_second(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: int,
     *,
     subproduct_use: bool = False,
-) -> 'ColumnElement[Any]':
+) -> "ColumnElement[Any]":
     """Django to SQLAlchemy adapter of ``second`` lookup."""
     if subproduct_use:
-        return extract('second', a)
-    return extract('second', a) == b
+        return extract("second", a)
+    return extract("second", a) == b
 
 
 def django_isnull(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: bool,  # noqa: FBT001
-) -> 'ColumnElement[bool]':
+) -> "ColumnElement[bool]":
     """Django to SQLAlchemy adapter of ``isnull`` lookup."""
     return a.is_(None) if b else a.is_not(None)
 
 
 def django_regex(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: str,
-) -> 'ColumnElement[bool]':
+) -> "ColumnElement[bool]":
     """Django to SQLAlchemy adapter of ``regex`` lookup."""
     return a.regexp_match(b)
 
 
 def django_iregex(
     a: QueryableAttribute[Any],  # noqa: ANN401
     b: str,
-) -> 'ColumnElement[bool]':
+) -> "ColumnElement[bool]":
     """Django to SQLAlchemy adapter of ``iregex`` lookup."""
     return func.lower(a).regexp_match(b.lower())
```

### Comparing `python_dev_utils-0.2.0/dev_utils/sqlalchemy/utils.py` & `python_dev_utils-1.0.6/dev_utils/sqlalchemy/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,35 +24,35 @@
     from collections.abc import Callable, Sequence
 
     from sqlalchemy.orm import Mapper, QueryableAttribute
     from sqlalchemy.orm.base import InspectionAttr
     from sqlalchemy.orm.clsregistry import _ClsRegistryType  # type: ignore
     from sqlalchemy.orm.strategy_options import _AbstractLoad  # type: ignore
 
-    T = TypeVar('T', bound=Select[Any])
+    T = TypeVar("T", bound=Select[Any])
 
 Statement = (
-    Select[tuple['DeclarativeBase']]
-    | Update['DeclarativeBase']
-    | Delete['DeclarativeBase']
-    | Insert['DeclarativeBase']
+    Select[tuple["DeclarativeBase"]]
+    | Update["DeclarativeBase"]
+    | Delete["DeclarativeBase"]
+    | Insert["DeclarativeBase"]
 )
 
 
 def get_utc_now() -> datetime.datetime:
     """Get current UTC datetime.
 
     Returns
     -------
         datetime: current datetime with UTC timezone.
     """
-    return datetime.datetime.now(zoneinfo.ZoneInfo('UTC'))
+    return datetime.datetime.now(zoneinfo.ZoneInfo("UTC"))
 
 
-def is_declarative(model: Any) -> TypeGuard['Mapper[Any]']:  # noqa: ANN401
+def is_declarative(model: Any) -> TypeGuard["Mapper[Any]"]:  # noqa: ANN401
     """Get sqlalchemy field (column) or relationship object from given model.
 
     Args
     ----
     model : Any
         Any object.
     field_name : str
@@ -60,19 +60,19 @@
 
     Returns
     -------
     QueryableAttribute[Any]
         any attribute from model, that can be used in queries.
     """
     try:
-        mapper: 'Mapper[Any]' = inspect(model)
+        mapper: "Mapper[Any]" = inspect(model)
     except Exception:
         return False
     else:
-        if not hasattr(mapper, 'is_mapper'):
+        if not hasattr(mapper, "is_mapper"):
             return False
         return mapper.is_mapper
 
 
 def get_sqlalchemy_attribute(
     model: type["DeclarativeBase"],
     field_name: str,
@@ -89,61 +89,61 @@
     Returns
     -------
     QueryableAttribute[Any]
         any attribute from model, that can be used in queries.
     """
     valid_attributes = get_all_valid_queryable_attributes(model)
     if field_name not in valid_attributes:
-        valid_field = ', '.join(valid_attributes)
+        valid_field = ", ".join(valid_attributes)
         msg = (
             f'No sqlalchemy attribute "{field_name}" was found in model "{model}". '
-            f'Valid attributes for {model}: {valid_field}'
+            f"Valid attributes for {model}: {valid_field}"
         )
         raise NoModelAttributeError(msg)
     sqlalchemy_field = getattr(model, field_name)
     if isinstance(sqlalchemy_field, types.MethodType):
         sqlalchemy_field = sqlalchemy_field()
     return sqlalchemy_field
 
 
-def get_model_classes_from_statement(stmt: Statement) -> 'Sequence[type[DeclarativeBase]]':
+def get_model_classes_from_statement(stmt: Statement) -> "Sequence[type[DeclarativeBase]]":
     """Get sqlalchemy model classes from given statement.
 
     Args
     ----
     stmt : Statement
         SQLAlchemy statement (select, update, delete, insert).
 
     Returns
     -------
     Sequence['DeclarativeBase']
         sequence of model classes.
     """
     if isinstance(stmt, Select):
         model_classes = [
-            col_desc['entity'] for col_desc in stmt.column_descriptions if col_desc['entity']
+            col_desc["entity"] for col_desc in stmt.column_descriptions if col_desc["entity"]
         ]
         for _from_clause in stmt._from_obj:  # type: ignore
             if not isinstance(_from_clause, Table):
-                msg = 'From clause without table binding was found and skipped for statement.'
+                msg = "From clause without table binding was found and skipped for statement."
                 logger.warning(msg)
                 continue
             if not is_declarative(_from_clause.entity_namespace):  # pragma: no cover
                 msg = (
                     f'Table with name "{_from_clause.name}" without Declarative model mapped '
-                    'class was found and skipped. Use declarative models.'
+                    "class was found and skipped. Use declarative models."
                 )
                 logger.error(msg)
                 raise NoDeclarativeModelError(msg)
             model_classes.append(_from_clause.entity_namespace)
         return list(set(model_classes))
-    return [stmt.entity_description['entity']]
+    return [stmt.entity_description["entity"]]
 
 
-def get_registry_class(model: type['DeclarativeBase']) -> '_ClsRegistryType':
+def get_registry_class(model: type["DeclarativeBase"]) -> "_ClsRegistryType":
     """Get sqlalchemy registry class from any model.
 
     Args
     ----
     model : type[DeclarativeBase]
         SQLAlchemy declarative model.
 
@@ -152,39 +152,39 @@
     _ClsRegistryType
         SQLAlchemy registry of all models and other specific objects.
     """
     return model.registry._class_registry  # type: ignore
 
 
 def get_model_class_by_tablename(
-    registry: '_ClsRegistryType',
+    registry: "_ClsRegistryType",
     tablename: str,
-) -> type['DeclarativeBase'] | None:
+) -> type["DeclarativeBase"] | None:
     """Return class reference mapped to table.
 
     Args
     ----
     registry : _ClsRegistryType
         SQLAlchemy registry of all models and other specific objects.
     name : str
         name of model to find in registry.
 
     Returns
     -------
     Class reference or None.
     """
     for c in registry.values():
-        if getattr(c, '__tablename__', None) == tablename:
+        if getattr(c, "__tablename__", None) == tablename:
             return c  # type: ignore
 
 
 def get_model_class_by_name(
-    registry: '_ClsRegistryType',
+    registry: "_ClsRegistryType",
     name: str,
-) -> type['DeclarativeBase'] | None:
+) -> type["DeclarativeBase"] | None:
     """Return the model class matching `name` in the given `registry`.
 
     Args
     ----
     registry : _ClsRegistryType
         SQLAlchemy registry of all models and other specific objects.
     name : str
@@ -192,19 +192,19 @@
 
     Returns
     -------
     type['DeclarativeBase'] | None
         Optional model class.
     """
     for cls in registry.values():
-        if getattr(cls, '__name__', None) == name:
+        if getattr(cls, "__name__", None) == name:
             return cls  # type: ignore
 
 
-def get_valid_model_class_names(registry: '_ClsRegistryType') -> set[str]:
+def get_valid_model_class_names(registry: "_ClsRegistryType") -> set[str]:
     """Get sqlalchemy model names as strings from given registry.
 
     Args
     ----
     registry : _ClsRegistryType
         SQLAlchemy registry of all models and other specific objects.
 
@@ -212,20 +212,20 @@
     -------
     set[str]
         set of model names as strings.
     """
     return set(
         filter(
             None,
-            (getattr(ele, '__name__', None) for ele in registry.values()),
+            (getattr(ele, "__name__", None) for ele in registry.values()),
         ),
     )
 
 
-def get_valid_relationships_names(model: type['DeclarativeBase']) -> set[str]:
+def get_valid_relationships_names(model: type["DeclarativeBase"]) -> set[str]:
     """Get sqlalchemy relationship names as strings from given model.
 
     Args
     ----
     model : type[DeclarativeBase]
         SQLAlchemy declarative model.
 
@@ -248,15 +248,15 @@
         SQLAlchemy declarative model.
 
     Returns
     -------
     set[str]
         set of model fields as strings.
     """
-    inspect_mapper: 'Mapper[Any]' = inspect(model)  # type: ignore
+    inspect_mapper: "Mapper[Any]" = inspect(model)  # type: ignore
     columns = inspect_mapper.columns
     orm_descriptors = inspect_mapper.all_orm_descriptors
 
     column_names = columns.keys()
     hybrid_names = [
         key
         for key, item in orm_descriptors.items()
@@ -293,15 +293,15 @@
         SQLAlchemy declarative model.
 
     Returns
     -------
     list[DeclarativeBase]
         list of related models.
     """
-    inspect_mapper: 'Mapper[Any]' = inspect(model)  # type: ignore
+    inspect_mapper: "Mapper[Any]" = inspect(model)  # type: ignore
     return [_relationship.mapper.class_ for _relationship in inspect_mapper.relationships]
 
 
 def is_hybrid_property(orm_descriptor: "InspectionAttr") -> bool:
     """Check, if given field inspected object is hybrid property or not.
 
     Args
@@ -332,15 +332,15 @@
     """
     return orm_descriptor.extension_type == HybridExtensionType.HYBRID_METHOD
 
 
 def apply_loads(
     stmt: "T",
     *relationship_names: str,
-    load_strategy: 'Callable[[Any], _AbstractLoad]' = joinedload,
+    load_strategy: "Callable[[Any], _AbstractLoad]" = joinedload,
 ) -> "T":
     """Apply loads from string.
 
     String joins should represent relations, not model classes.
 
     Args
     ----
@@ -353,24 +353,24 @@
 
     Returns
     -------
     stmt : TypeVar (Statement)
         select statement instance with applied joins.
     """
     model_classes = get_model_classes_from_statement(stmt)
-    loaders: list['_AbstractLoad'] = []
+    loaders: list["_AbstractLoad"] = []
     for relationship_ in relationship_names:
         sqlalchemy_relationship = None
         for model_ in model_classes:
             if relationship_ in get_valid_relationships_names(model_):
                 sqlalchemy_relationship = get_sqlalchemy_attribute(model_, relationship_)
         if not sqlalchemy_relationship:
             msg = (
                 f'SQLAlchemy relationship "{relationship_}" was not found in {model_classes}. '
-                'Maybe you passed incorrect relationship name or passed model name.'
+                "Maybe you passed incorrect relationship name or passed model name."
             )
             logger.error(msg)
             # TODO: add all available relationships or nearest (fuzzy search) in message.
             raise NoModelRelationshipError(msg)
         load = load_strategy(sqlalchemy_relationship)
         loaders.append(load)
     stmt = stmt.options(*loaders)
@@ -412,15 +412,15 @@
         for model_ in model_classes:
             valid_relationships_names = model_to_valid_relationship_names[model_]
             if relationship_ in valid_relationships_names:
                 sqlalchemy_relationship = get_sqlalchemy_attribute(model_, relationship_)
         if not sqlalchemy_relationship:
             msg = (
                 f'SQLAlchemy relationship "{relationship_}" was not found in {model_classes}. '
-                'Maybe you passed incorrect relationship name or passed model name.'
+                "Maybe you passed incorrect relationship name or passed model name."
             )
             logger.error(msg)
             # TODO: add all available relationships or nearest (fuzzy search) in message.
             raise NoModelRelationshipError(msg)
         stmt = stmt.join(  # type: ignore
             sqlalchemy_relationship,
             isouter=left_outer_join,
```

### Comparing `python_dev_utils-0.2.0/pyproject.toml` & `python_dev_utils-1.0.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,24 @@
 [tool.ruff]
+output-format = "full"
+line-length = 100
+exclude = [
+    ".git",
+    "__pycache__",
+    ".venv",
+    ".eggs",
+    "*.egg",
+    "dist",
+    "tests/fixtures/**",
+    "tests/**/snapshots/**",
+    "alembic",
+    "airich",
+]
+
+[tool.ruff.lint]
 select = [
     "A",
     "B",
     "D",
     "E",
     "F",
     "G",
@@ -11,15 +27,14 @@
     "S",
     "C90",
     "UP",
     "ANN",
     "ASYNC",
     "FBT",
     "COM",
-    "COM",
     "DTZ",
     "DJ",
     "EM",
     "ICN",
     "PIE",
     "T20",
     "PYI",
@@ -27,55 +42,42 @@
     "SIM",
     "TCH",
     "INT",
     "PTH",
     "ERA",
     "TRY",
 ]
-line-length = 100
-show-source = true
-exclude = [
-    ".git",
-    "__pycache__",
-    ".venv",
-    ".eggs",
-    "*.egg",
-    "dist",
-    "tests/fixtures/**",
-    "tests/**/snapshots/**",
-    "alembic",
-    "airich",
-]
 ignore = [
     "D100",
     "B008",
     "D104",
     "Q000",
     "S101",
     "PT016",
     "ANN101",
     "ANN102",
+    "N805",
 ]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "numpy"
 ignore-decorators = [
     "typing.overload",
 ]
 
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 11
 
-[tool.ruff.flake8-bugbear]
+[tool.ruff.lint.flake8-bugbear]
 extend-immutable-calls = [
     "fastapi.Depends",
     "fastapi.Query",
 ]
 
-[tool.ruff.extend-per-file-ignores]
+[tool.ruff.lint.extend-per-file-ignores]
 "__init__.py" = [
     "F401",
 ]
 "*/migrations/versions/*" = [
     "D103",
 ]
 "src/app/main.py" = [
@@ -163,15 +165,15 @@
     "asyncpg>=0.29.0",
     "pytest-asyncio>=0.23.6",
     "httpx>=0.27.0",
 ]
 
 [project]
 name = "python_dev_utils"
-version = "0.2.0"
+version = "1.0.6"
 description = "My project utils package, that I use in my projects."
 authors = [
     { name = "Dmitriy Lunev", email = "dima.lunev14@gmail.com" },
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 dependencies = []
```

### Comparing `python_dev_utils-0.2.0/tests/conftest.py` & `python_dev_utils-1.0.6/tests/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from fastapi.testclient import TestClient
 from mimesis import Datetime, Locale, Text
 from sqlalchemy import create_engine, select
 from sqlalchemy.exc import SQLAlchemyError
 from sqlalchemy.ext.asyncio import async_scoped_session, async_sessionmaker, create_async_engine
 from sqlalchemy.orm import scoped_session, sessionmaker
 
-from dev_utils.profiling.middlewares import (
+from dev_utils.fastapi.middlewares.sqlalchemy_profiling import (
     add_query_counter_middleware,
     add_query_profiling_middleware,
 )
 from tests.utils import (
     Base,
     MyModel,
     OtherModel,
@@ -34,159 +34,159 @@
     from sqlalchemy import Engine
     from sqlalchemy.ext.asyncio import AsyncEngine, AsyncSession
     from sqlalchemy.orm import Session
 
     from tests.types import AsyncFactoryFunctionProtocol, SyncFactoryFunctionProtocol
 
 
-true_stmt = {'y', 'Y', 'yes', 'Yes', 't', 'true', 'True', '1'}
-IS_DOCKER_TEST = os.environ.get('IS_DOCKER_TEST', 'false') in true_stmt
+true_stmt = {"y", "Y", "yes", "Yes", "t", "true", "True", "1"}
+IS_DOCKER_TEST = os.environ.get("IS_DOCKER_TEST", "false") in true_stmt
 
 
 @pytest.fixture(scope="session")
-def event_loop() -> 'Generator[asyncio.AbstractEventLoop, None, None]':
+def event_loop() -> "Generator[asyncio.AbstractEventLoop, None, None]":
     """Event loop fixture."""
     loop = asyncio.get_event_loop_policy().new_event_loop()
     yield loop
     loop.close()
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def db_name() -> str:
     """Db name as fixture."""
-    return 'test_db'
+    return "test_db"
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def db_user() -> str:
     """DB user as fixture."""
-    return 'postgres'
+    return "postgres"
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def db_password() -> str:
     """DB password as fixture."""
-    return 'postgres'
+    return "postgres"
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def db_host() -> str:
     """DB host as fixture."""
-    return 'db' if IS_DOCKER_TEST else 'localhost'
+    return "db" if IS_DOCKER_TEST else "localhost"
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def db_port() -> int:
     """DB port as fixture."""
     return 5432
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def db_domain(db_name: str, db_user: str, db_password: str, db_host: str, db_port: int) -> str:
     """Domain for test db without specified driver."""
-    return f'{db_user}:{db_password}@{db_host}:{db_port}/{db_name}'
+    return f"{db_user}:{db_password}@{db_host}:{db_port}/{db_name}"
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def db_sync_url(db_domain: str) -> str:
     """URL for test db (will be created in db_engine): sync driver."""
-    return f'postgresql://{db_domain}'
+    return f"postgresql://{db_domain}"
 
 
-@pytest.fixture(scope='session')
+@pytest.fixture(scope="session")
 def db_async_url(db_domain: str) -> str:
     """URL for test db (will be created in db_engine): async driver."""
-    return f'postgresql+asyncpg://{db_domain}'
+    return f"postgresql+asyncpg://{db_domain}"
 
 
-@pytest.fixture(scope='session')
-def db_sync_engine(db_sync_url: str) -> 'Generator[Engine, None, None]':
+@pytest.fixture(scope="session")
+def db_sync_engine(db_sync_url: str) -> "Generator[Engine, None, None]":
     """SQLAlchemy engine session-based fixture."""
     with suppress(SQLAlchemyError):
         create_db(db_sync_url)
     engine = create_engine(db_sync_url, echo=False, pool_pre_ping=True)
     try:
         yield engine
     finally:
         engine.dispose()
     with suppress(SQLAlchemyError):
         destroy_db(db_sync_url)
 
 
-@pytest_asyncio.fixture(scope='session')  # type: ignore
-async def db_async_engine(db_async_url: str) -> 'AsyncGenerator[AsyncEngine, None]':  # type: ignore
+@pytest_asyncio.fixture(scope="session")  # type: ignore
+async def db_async_engine(db_async_url: str) -> "AsyncGenerator[AsyncEngine, None]":  # type: ignore
     """SQLAlchemy engine session-based fixture."""
     engine = create_async_engine(db_async_url, echo=True, pool_pre_ping=True)
     try:
         yield engine
     finally:
         await engine.dispose()
 
 
-@pytest.fixture(scope='session')
-def db_sync_session_factory(db_sync_engine: 'Engine') -> 'scoped_session[Session]':
+@pytest.fixture(scope="session")
+def db_sync_session_factory(db_sync_engine: "Engine") -> "scoped_session[Session]":
     """SQLAlchemy session factory session-based fixture."""
     return scoped_session(
         sessionmaker(
             bind=db_sync_engine,
             autoflush=False,
             expire_on_commit=False,
         ),
     )
 
 
-@pytest.fixture(scope='session')  # type: ignore
+@pytest.fixture(scope="session")  # type: ignore
 def db_async_session_factory(
-    db_async_engine: 'AsyncEngine',
-) -> 'async_scoped_session[AsyncSession]':
+    db_async_engine: "AsyncEngine",
+) -> "async_scoped_session[AsyncSession]":
     """SQLAlchemy session factory session-based fixture."""
     return async_scoped_session(
         async_sessionmaker(
             bind=db_async_engine,
             autoflush=False,
             expire_on_commit=False,
         ),
         asyncio.current_task,
     )
 
 
 @pytest.fixture()
 def db_sync_session(
-    db_sync_engine: 'Engine',
-    db_sync_session_factory: 'scoped_session[Session]',
-) -> 'Generator[Session, None, None]':
+    db_sync_engine: "Engine",
+    db_sync_session_factory: "scoped_session[Session]",
+) -> "Generator[Session, None, None]":
     """SQLAlchemy session fixture."""
     Base.metadata.drop_all(db_sync_engine)
     Base.metadata.create_all(db_sync_engine)
     with db_sync_session_factory() as session:
         yield session
 
 
 @pytest_asyncio.fixture()  # type: ignore
 async def db_async_session(
-    db_async_engine: 'AsyncEngine',
-    db_async_session_factory: 'async_scoped_session[AsyncSession]',
-) -> 'AsyncGenerator[AsyncSession, None]':
+    db_async_engine: "AsyncEngine",
+    db_async_session_factory: "async_scoped_session[AsyncSession]",
+) -> "AsyncGenerator[AsyncSession, None]":
     """SQLAlchemy session fixture."""
     async with db_async_engine.begin() as conn:
         await conn.run_sync(Base.metadata.drop_all)
         await conn.run_sync(Base.metadata.create_all)
     async with db_async_session_factory() as session:
         yield session
 
 
 @pytest.fixture()
 def mymodel_sync_factory(
     dt_faker: Datetime,
     text_faker: Text,
-) -> 'SyncFactoryFunctionProtocol[MyModel]':
+) -> "SyncFactoryFunctionProtocol[MyModel]":
     """Function-factory, that create MyModel instances."""
 
     def _create(
-        session: 'Session',
+        session: "Session",
         *,
         commit: bool = False,
         **kwargs: Any,  # noqa: ANN401
     ) -> MyModel:
         params: dict[str, Any] = dict(
             name=text_faker.sentence(),
             other_name=text_faker.sentence(),
@@ -198,28 +198,28 @@
 
     return _create
 
 
 @pytest.fixture()
 def othermodel_sync_factory(
     text_faker: Text,
-    mymodel_sync_factory: 'SyncFactoryFunctionProtocol[MyModel]',
-) -> 'SyncFactoryFunctionProtocol[OtherModel]':
+    mymodel_sync_factory: "SyncFactoryFunctionProtocol[MyModel]",
+) -> "SyncFactoryFunctionProtocol[OtherModel]":
     """Function-factory, that create OtherModel instances."""
 
     def _create(
-        session: 'Session',
+        session: "Session",
         *,
         commit: bool = False,
         **kwargs: Any,  # noqa: ANN401
     ) -> OtherModel:
-        if 'model_id' not in kwargs:
+        if "model_id" not in kwargs:
             model_id = mymodel_sync_factory(session, commit=commit).id
         else:
-            model_id = kwargs.pop('model_id')
+            model_id = kwargs.pop("model_id")
         params: dict[str, Any] = dict(
             name=text_faker.sentence(),
             other_name=text_faker.sentence(),
             model_id=model_id,
         )
         params.update(kwargs)
         return create_db_item_sync(session, OtherModel, params, commit=commit)
@@ -227,19 +227,19 @@
     return _create
 
 
 @pytest.fixture()
 def mymodel_async_factory(
     text_faker: Text,
     dt_faker: Datetime,
-) -> 'AsyncFactoryFunctionProtocol[MyModel]':
+) -> "AsyncFactoryFunctionProtocol[MyModel]":
     """Function-factory, that create MyModel instances."""
 
     async def _create(
-        session: 'AsyncSession',
+        session: "AsyncSession",
         *,
         commit: bool = False,
         **kwargs: Any,  # noqa: ANN401
     ) -> MyModel:
         params: dict[str, Any] = dict(
             name=text_faker.sentence(),
             other_name=text_faker.sentence(),
@@ -251,29 +251,29 @@
 
     return _create
 
 
 @pytest.fixture()
 def othermodel_async_factory(
     text_faker: Text,
-    mymodel_async_factory: 'AsyncFactoryFunctionProtocol[MyModel]',
-) -> 'AsyncFactoryFunctionProtocol[OtherModel]':
+    mymodel_async_factory: "AsyncFactoryFunctionProtocol[MyModel]",
+) -> "AsyncFactoryFunctionProtocol[OtherModel]":
     """Function-factory, that create OtherModel instances."""
 
     async def _create(
-        session: 'AsyncSession',
+        session: "AsyncSession",
         *,
         commit: bool = False,
         **kwargs: Any,  # noqa: ANN401
     ) -> OtherModel:
-        if 'model_id' not in kwargs:
+        if "model_id" not in kwargs:
             model = await mymodel_async_factory(session, commit=commit)
             model_id = model.id
         else:
-            model_id = kwargs.pop('model_id')
+            model_id = kwargs.pop("model_id")
         params: dict[str, Any] = dict(
             name=text_faker.sentence(),
             other_name=text_faker.sentence(),
             model_id=model_id,
         )
         params.update(kwargs)
         return await create_db_item_async(session, OtherModel, params, commit=commit)
@@ -289,29 +289,29 @@
 @pytest.fixture()
 def dt_faker() -> Datetime:
     return Datetime(locale=Locale.EN)
 
 
 @pytest.fixture()
 def test_sync_app(
-    db_sync_session: 'Session',
-    db_sync_engine: 'Engine',
-    mymodel_sync_factory: 'SyncFactoryFunctionProtocol[MyModel]',
-) -> 'Generator[TestClient, None, None]':
+    db_sync_session: "Session",
+    db_sync_engine: "Engine",
+    mymodel_sync_factory: "SyncFactoryFunctionProtocol[MyModel]",
+) -> "Generator[TestClient, None, None]":
     app = FastAPI()
     add_query_profiling_middleware(app, engine=db_sync_engine)
     add_query_counter_middleware(app, engine=db_sync_engine)
     for _ in range(10):
         mymodel_sync_factory(db_sync_session)
 
-    @app.get('/')
+    @app.get("/")
     def index():  # type: ignore  # noqa: ANN202
         stmt = select(MyModel)
         items = db_sync_session.execute(stmt).scalars().all()
-        items = [{'id': item.id} for item in items]
+        items = [{"id": item.id} for item in items]
         return items
 
     with TestClient(
         app=app,
         base_url="http://test/",
     ) as c:
         yield c
```

### Comparing `python_dev_utils-0.2.0/tests/core/test_abstract.py` & `python_dev_utils-1.0.6/tests/core/test_abstract.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,20 +29,37 @@
 
 def test_attr_raises() -> None:
     with pytest.raises(TypeError):
         str(CorrectClass.a)
     with pytest.raises(TypeError):
         bool(CorrectClass.a)
     with pytest.raises(TypeError):
-        CorrectClass.a == '2'  # type: ignore  # noqa: B015
+        CorrectClass.a == "2"  # type: ignore  # noqa: B015
     with pytest.raises(TypeError):
-        CorrectClass.a > '2'  # type: ignore  # noqa: B015
+        CorrectClass.a > "2"  # type: ignore  # noqa: B015
     with pytest.raises(TypeError):
-        CorrectClass.a < '2'  # type: ignore  # noqa: B015
+        CorrectClass.a < "2"  # type: ignore  # noqa: B015
     with pytest.raises(TypeError):
-        CorrectClass.a >= '2'  # type: ignore  # noqa: B015
+        CorrectClass.a >= "2"  # type: ignore  # noqa: B015
     with pytest.raises(TypeError):
-        CorrectClass.a <= '2'  # type: ignore  # noqa: B015
+        CorrectClass.a <= "2"  # type: ignore  # noqa: B015
     with pytest.raises(TypeError):
         CorrectClass.a.some_attr  # type: ignore  # noqa: B015, B018
     with pytest.raises(TypeError):
-        CorrectClass.a.some_attr = ''  # type: ignore  # noqa: B015, B018
+        CorrectClass.a.some_attr = ""  # type: ignore  # noqa: B015, B018
+
+
+def test_inherit_abstract_type_error() -> None:
+    class CorrectClass(abstract.Abstract):  # type: ignore
+        a: str = abstract.abstract_class_property(str)
+
+    with pytest.raises(TypeError):
+
+        class InheritClass(CorrectClass): ...  # type: ignore
+
+
+def test_inherit_abstract_skip() -> None:
+    class CorrectClass(abstract.Abstract):  # type: ignore
+        a: str = abstract.abstract_class_property(str)
+
+    class InheritClass(CorrectClass):  # type: ignore
+        __skip_abstract_raise_error__ = True
```

### Comparing `python_dev_utils-0.2.0/tests/core/test_results.py` & `python_dev_utils-1.0.6/tests/core/test_results.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,21 +15,21 @@
     other_ne_result = some_func(-100)
     assert isinstance(result, results.Ok)
     assert result.err() is None
     assert isinstance(result.unwrap(), int)
     assert result == other_result
     assert result != other_ne_result
     assert result != 25
-    assert repr(result) == 'Ok(25)'
+    assert repr(result) == "Ok(25)"
 
 
 def test_error() -> None:
-    result = some_func('string')
-    other_result = some_func('string')
-    other_ne_result = some_func('not string')
+    result = some_func("string")
+    other_result = some_func("string")
+    other_ne_result = some_func("not string")
     assert isinstance(result, results.Err)
     assert isinstance(result.err(), TypeError)
     with pytest.raises(TypeError):
         result.unwrap()
     assert result == other_result
     assert result != other_ne_result
     assert result != 25
```

### Comparing `python_dev_utils-0.2.0/tests/core/test_utils.py` & `python_dev_utils-1.0.6/tests/core/test_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 class MyObject:  # noqa: D101
     pass
 
 
 @pytest.mark.parametrize(
-    ('obj', 'expected_result'),
+    ("obj", "expected_result"),
     [
-        (obj, 'object'),
-        (MyObject, 'tests.core.test_utils.MyObject'),
-        (MyObject(), 'tests.core.test_utils.MyObject'),
+        (obj, "object"),
+        (MyObject, "tests.core.test_utils.MyObject"),
+        (MyObject(), "tests.core.test_utils.MyObject"),
     ],
 )
 def test_get_object_class_absolute_name(obj: object, expected_result: str) -> None:
     assert utils.get_object_class_absolute_name(obj) == expected_result
 
 
 @pytest.mark.parametrize(
-    ('obj', 'expected_result'),
+    ("obj", "expected_result"),
     [
-        ('                 abc                ', 'abc'),
-        ('                 abc\nabc                ', 'abc abc'),
-        ('                 abc  abc                ', 'abc abc'),
-        ('                 abc   abc                ', 'abc abc'),
+        ("                 abc                ", "abc"),
+        ("                 abc\nabc                ", "abc abc"),
+        ("                 abc  abc                ", "abc abc"),
+        ("                 abc   abc                ", "abc abc"),
     ],
 )
 def test_trim_and_plain_text(obj: str, expected_result: str) -> None:
     assert utils.trim_and_plain_text(obj) == expected_result
```

### Comparing `python_dev_utils-0.2.0/tests/profiling/test_profilers.py` & `python_dev_utils-1.0.6/tests/sqlalchemy/profiling/test_profilers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,100 +1,100 @@
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import pytest
 from sqlalchemy import select
 
 from dev_utils.core.utils import trim_and_plain_text
-from dev_utils.profiling import profilers
+from dev_utils.sqlalchemy.profiling import profilers
 from tests.utils import MyModel
 
 if TYPE_CHECKING:
     from sqlalchemy import Engine
     from sqlalchemy.ext.asyncio import AsyncEngine, AsyncSession
     from sqlalchemy.orm import Session
 
 
 def test_sync_sql_alchemy_query_profiler(
-    db_sync_engine: 'Engine',
-    db_sync_session: 'Session',
+    db_sync_engine: "Engine",
+    db_sync_session: "Session",
 ) -> None:
     profiler = profilers.SQLAlchemyQueryProfiler(db_sync_engine)
     profiler.start()
     stmt = select(MyModel)
     db_sync_session.execute(stmt)
     profiler.stop()
     report = profiler.collect()
     assert len(report) == 1
     assert isinstance(report[0], profilers.QueryInfo)
     assert report[0].text == trim_and_plain_text(str(stmt))
 
 
 def test_sync_sql_alchemy_query_profiler_double_start(
-    db_sync_engine: 'Engine',
+    db_sync_engine: "Engine",
 ) -> None:
     profiler = profilers.SQLAlchemyQueryProfiler(db_sync_engine)
     profiler.start()
     profiler.start()
     profiler.stop()
 
 
 def test_sync_sql_alchemy_query_profiler_report(
-    db_sync_engine: 'Engine',
+    db_sync_engine: "Engine",
 ) -> None:
     profiler = profilers.SQLAlchemyQueryProfiler(db_sync_engine)
     profiler.start()
     profiler.stop()
-    file = Path('report.txt')
+    file = Path("report.txt")
     profiler.report(file)
     assert file.exists()
 
 
 def test_sync_sql_alchemy_query_profiler_double_stop(
-    db_sync_engine: 'Engine',
+    db_sync_engine: "Engine",
 ) -> None:
     profiler = profilers.SQLAlchemyQueryProfiler(db_sync_engine)
     profiler.start()
     profiler.stop()
     profiler.stop()
 
 
 def test_sync_sql_alchemy_query_profiler_context_manager(
-    db_sync_engine: 'Engine',
-    db_sync_session: 'Session',
+    db_sync_engine: "Engine",
+    db_sync_session: "Session",
 ) -> None:
     with profilers.SQLAlchemyQueryProfiler(db_sync_engine) as profiler:
         stmt = select(MyModel)
         db_sync_session.execute(stmt)
     report = profiler.collect()
     assert len(report) == 1
     assert isinstance(report[0], profilers.QueryInfo)
     assert report[0].text == trim_and_plain_text(str(stmt))
 
 
 @pytest.mark.asyncio()
 async def test_async_sql_alchemy_query_profiler(
-    db_async_engine: 'AsyncEngine',
-    db_async_session: 'AsyncSession',
+    db_async_engine: "AsyncEngine",
+    db_async_session: "AsyncSession",
 ) -> None:
     profiler = profilers.SQLAlchemyQueryProfiler(db_async_engine)
     profiler.start()
     stmt = select(MyModel)
     await db_async_session.execute(stmt)
     profiler.stop()
     report = profiler.collect()
     assert len(report) == 1
     assert isinstance(report[0], profilers.QueryInfo)
     assert report[0].text == trim_and_plain_text(str(stmt))
 
 
 @pytest.mark.asyncio()
 async def test_async_sql_alchemy_query_profiler_context_manager(
-    db_async_engine: 'AsyncEngine',
-    db_async_session: 'AsyncSession',
+    db_async_engine: "AsyncEngine",
+    db_async_session: "AsyncSession",
 ) -> None:
     with profilers.SQLAlchemyQueryProfiler(db_async_engine) as profiler:
         stmt = select(MyModel)
         await db_async_session.execute(stmt)
     report = profiler.collect()
     assert len(report) == 1
     assert isinstance(report[0], profilers.QueryInfo)
```

### Comparing `python_dev_utils-0.2.0/tests/sqlalchemy/filters/test_converters.py` & `python_dev_utils-1.0.6/tests/sqlalchemy/filters/test_converters.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,346 +10,346 @@
     AdvancedOperatorFilterConverter,
     BaseFilterConverter,
     DjangoLikeFilterConverter,
     SimpleFilterConverter,
 )
 from tests.utils import MyModel
 
-now = datetime.datetime.now(tz=zoneinfo.ZoneInfo('UTC'))
+now = datetime.datetime.now(tz=zoneinfo.ZoneInfo("UTC"))
 _date = now.date()
 _date_future = now.date() + datetime.timedelta(days=1)
 _time = now.time()
 _time_future = (now + datetime.timedelta(hours=1)).time()
 
 
 @pytest.mark.parametrize(
-    ('converter_class', 'filters', 'expected_result'),
+    ("converter_class", "filters", "expected_result"),
     [
         (
             SimpleFilterConverter,
             None,
             [],
         ),
         (
             SimpleFilterConverter,
             [MyModel.id == 25],
             [str(MyModel.id == 25)],
         ),
         (
             SimpleFilterConverter,
-            {'id': 25, 'name': 'name'},
-            [str(MyModel.id == 25), str(MyModel.name == 'name')],
+            {"id": 25, "name": "name"},
+            [str(MyModel.id == 25), str(MyModel.name == "name")],
         ),
         (
             SimpleFilterConverter,
-            [{'id': 25}, {'name': 'name'}],
-            [str(MyModel.id == 25), str(MyModel.name == 'name')],
+            [{"id": 25}, {"name": "name"}],
+            [str(MyModel.id == 25), str(MyModel.name == "name")],
         ),
         (
             SimpleFilterConverter,
-            {'full_name': 'abc'},
-            [str(MyModel.full_name == 'abc')],
+            {"full_name": "abc"},
+            [str(MyModel.full_name == "abc")],
         ),
         (
             AdvancedOperatorFilterConverter,
-            [{'field': 'id', 'value': 25}, {'field': 'name', 'value': 'abc'}],
-            [str(MyModel.id == 25), str(MyModel.name == 'abc')],
+            [{"field": "id", "value": 25}, {"field": "name", "value": "abc"}],
+            [str(MyModel.id == 25), str(MyModel.name == "abc")],
         ),
         (
             AdvancedOperatorFilterConverter,
             [
-                {'field': 'id', 'value': 25, 'operator': '='},
-                {'field': 'id', 'value': 25, 'operator': '>'},
-                {'field': 'id', 'value': 25, 'operator': '>='},
-                {'field': 'id', 'value': 25, 'operator': '<'},
-                {'field': 'id', 'value': 25, 'operator': '<='},
-                {'field': 'id', 'value': (25, 28), 'operator': 'between'},
-                {'field': 'id', 'value': [1, 2, 3], 'operator': 'contains'},
+                {"field": "id", "value": 25, "operator": "="},
+                {"field": "id", "value": 25, "operator": ">"},
+                {"field": "id", "value": 25, "operator": ">="},
+                {"field": "id", "value": 25, "operator": "<"},
+                {"field": "id", "value": 25, "operator": "<="},
+                {"field": "id", "value": (25, 28), "operator": "between"},
+                {"field": "id", "value": [1, 2, 3], "operator": "contains"},
             ],
             [
                 str(MyModel.id == 25),
                 str(MyModel.id > 25),
                 str(MyModel.id >= 25),
                 str(MyModel.id < 25),
                 str(MyModel.id <= 25),
                 str(MyModel.id.between(25, 28)),
                 str(MyModel.id.in_([1, 2, 3])),
             ],
         ),
         (
             DjangoLikeFilterConverter,
             {
-                'id': 25,
-                'id__exact': 25,
-                'name__exact': None,
-                'name__iexact': 'abc',
-                'name__contains': 'abc',
-                'name__icontains': 'abc',
-                'name__in': ['abc', 'bca', 'dce'],
-                'name__startswith': 'abc',
-                'name__istartswith': 'abc',
-                'name__endswith': 'abc',
-                'name__iendswith': 'abc',
-                'id__range': [1, 2],
-                'dt__date': _date,
-                'dt__date__exact': _date,
-                'dt__date__iexact': _date,
-                'dt__date__in': [_date, _date_future],
-                'dt__date__gt': _date,
-                'dt__date__lt': _date,
-                'dt__date__gte': _date,
-                'dt__date__lte': _date,
-                'dt__date__range': (_date, _date_future),
-                'dt__year': 2024,
-                'dt__year__exact': 2024,
-                'dt__year__iexact': 2024,
-                'dt__year__in': [2024, 2025],
-                'dt__year__gt': 2024,
-                'dt__year__lt': 2024,
-                'dt__year__gte': 2024,
-                'dt__year__lte': 2024,
-                'dt__year__range': (2024, 2025),
-                'dt__iso_year': 2025,
-                'dt__iso_year__exact': 2024,
-                'dt__iso_year__iexact': 2024,
-                'dt__iso_year__in': [2024, 2025],
-                'dt__iso_year__gt': 2024,
-                'dt__iso_year__lt': 2024,
-                'dt__iso_year__gte': 2024,
-                'dt__iso_year__lte': 2024,
-                'dt__iso_year__range': (2024, 2025),
-                'dt__month': 1,
-                'dt__month__exact': 1,
-                'dt__month__iexact': 1,
-                'dt__month__in': [1, 2],
-                'dt__month__gt': 1,
-                'dt__month__lt': 1,
-                'dt__month__gte': 1,
-                'dt__month__lte': 1,
-                'dt__month__range': (1, 2),
-                'dt__day': 2,
-                'dt__day__exact': 2,
-                'dt__day__iexact': 2,
-                'dt__day__in': [2, 3],
-                'dt__day__gt': 2,
-                'dt__day__lt': 2,
-                'dt__day__gte': 2,
-                'dt__day__lte': 2,
-                'dt__day__range': (2, 3),
-                'dt__week': 3,
-                'dt__week__exact': 3,
-                'dt__week__iexact': 3,
-                'dt__week__in': [3, 4],
-                'dt__week__gt': 3,
-                'dt__week__lt': 3,
-                'dt__week__gte': 3,
-                'dt__week__lte': 3,
-                'dt__week__range': (3, 4),
-                'dt__week_day': 4,
-                'dt__week_day__exact': 4,
-                'dt__week_day__iexact': 4,
-                'dt__week_day__in': [4, 5],
-                'dt__week_day__gt': 4,
-                'dt__week_day__lt': 4,
-                'dt__week_day__gte': 4,
-                'dt__week_day__lte': 4,
-                'dt__week_day__range': (4, 5),
-                'dt__iso_week_day': 5,
-                'dt__iso_week_day__exact': 5,
-                'dt__iso_week_day__iexact': 5,
-                'dt__iso_week_day__in': [5, 6],
-                'dt__iso_week_day__gt': 5,
-                'dt__iso_week_day__lt': 5,
-                'dt__iso_week_day__gte': 5,
-                'dt__iso_week_day__lte': 5,
-                'dt__iso_week_day__range': (5, 6),
-                'dt__quarter': 1,
-                'dt__quarter__exact': 1,
-                'dt__quarter__iexact': 1,
-                'dt__quarter__in': [1, 2],
-                'dt__quarter__gt': 1,
-                'dt__quarter__lt': 1,
-                'dt__quarter__gte': 1,
-                'dt__quarter__lte': 1,
-                'dt__quarter__range': (1, 2),
-                'dt__time': _time,
-                'dt__time__exact': _time,
-                'dt__time__iexact': _time,
-                'dt__time__in': [_time, _time_future],
-                'dt__time__gt': _time,
-                'dt__time__lt': _time,
-                'dt__time__gte': _time,
-                'dt__time__lte': _time,
-                'dt__time__range': (_time, _time_future),
-                'dt__hour': 1,
-                'dt__hour__exact': 1,
-                'dt__hour__iexact': 1,
-                'dt__hour__in': [1, 2],
-                'dt__hour__gt': 1,
-                'dt__hour__lt': 1,
-                'dt__hour__gte': 1,
-                'dt__hour__lte': 1,
-                'dt__hour__range': (1, 2),
-                'dt__minute': 1,
-                'dt__minute__exact': 1,
-                'dt__minute__iexact': 1,
-                'dt__minute__in': [1, 2],
-                'dt__minute__gt': 1,
-                'dt__minute__lt': 1,
-                'dt__minute__gte': 1,
-                'dt__minute__lte': 1,
-                'dt__minute__range': (1, 2),
-                'dt__second': 1,
-                'dt__second__exact': 1,
-                'dt__second__iexact': 1,
-                'dt__second__in': [1, 2],
-                'dt__second__gt': 1,
-                'dt__second__lt': 1,
-                'dt__second__gte': 1,
-                'dt__second__lte': 1,
-                'dt__second__range': (1, 2),
-                'id__isnull': True,
-                'name__isnull': False,
-                'name__regex': '^(b|c)',
-                'other_name__iregex': '^(b|c)',
+                "id": 25,
+                "id__exact": 25,
+                "name__exact": None,
+                "name__iexact": "abc",
+                "name__contains": "abc",
+                "name__icontains": "abc",
+                "name__in": ["abc", "bca", "dce"],
+                "name__startswith": "abc",
+                "name__istartswith": "abc",
+                "name__endswith": "abc",
+                "name__iendswith": "abc",
+                "id__range": [1, 2],
+                "dt__date": _date,
+                "dt__date__exact": _date,
+                "dt__date__iexact": _date,
+                "dt__date__in": [_date, _date_future],
+                "dt__date__gt": _date,
+                "dt__date__lt": _date,
+                "dt__date__gte": _date,
+                "dt__date__lte": _date,
+                "dt__date__range": (_date, _date_future),
+                "dt__year": 2024,
+                "dt__year__exact": 2024,
+                "dt__year__iexact": 2024,
+                "dt__year__in": [2024, 2025],
+                "dt__year__gt": 2024,
+                "dt__year__lt": 2024,
+                "dt__year__gte": 2024,
+                "dt__year__lte": 2024,
+                "dt__year__range": (2024, 2025),
+                "dt__iso_year": 2025,
+                "dt__iso_year__exact": 2024,
+                "dt__iso_year__iexact": 2024,
+                "dt__iso_year__in": [2024, 2025],
+                "dt__iso_year__gt": 2024,
+                "dt__iso_year__lt": 2024,
+                "dt__iso_year__gte": 2024,
+                "dt__iso_year__lte": 2024,
+                "dt__iso_year__range": (2024, 2025),
+                "dt__month": 1,
+                "dt__month__exact": 1,
+                "dt__month__iexact": 1,
+                "dt__month__in": [1, 2],
+                "dt__month__gt": 1,
+                "dt__month__lt": 1,
+                "dt__month__gte": 1,
+                "dt__month__lte": 1,
+                "dt__month__range": (1, 2),
+                "dt__day": 2,
+                "dt__day__exact": 2,
+                "dt__day__iexact": 2,
+                "dt__day__in": [2, 3],
+                "dt__day__gt": 2,
+                "dt__day__lt": 2,
+                "dt__day__gte": 2,
+                "dt__day__lte": 2,
+                "dt__day__range": (2, 3),
+                "dt__week": 3,
+                "dt__week__exact": 3,
+                "dt__week__iexact": 3,
+                "dt__week__in": [3, 4],
+                "dt__week__gt": 3,
+                "dt__week__lt": 3,
+                "dt__week__gte": 3,
+                "dt__week__lte": 3,
+                "dt__week__range": (3, 4),
+                "dt__week_day": 4,
+                "dt__week_day__exact": 4,
+                "dt__week_day__iexact": 4,
+                "dt__week_day__in": [4, 5],
+                "dt__week_day__gt": 4,
+                "dt__week_day__lt": 4,
+                "dt__week_day__gte": 4,
+                "dt__week_day__lte": 4,
+                "dt__week_day__range": (4, 5),
+                "dt__iso_week_day": 5,
+                "dt__iso_week_day__exact": 5,
+                "dt__iso_week_day__iexact": 5,
+                "dt__iso_week_day__in": [5, 6],
+                "dt__iso_week_day__gt": 5,
+                "dt__iso_week_day__lt": 5,
+                "dt__iso_week_day__gte": 5,
+                "dt__iso_week_day__lte": 5,
+                "dt__iso_week_day__range": (5, 6),
+                "dt__quarter": 1,
+                "dt__quarter__exact": 1,
+                "dt__quarter__iexact": 1,
+                "dt__quarter__in": [1, 2],
+                "dt__quarter__gt": 1,
+                "dt__quarter__lt": 1,
+                "dt__quarter__gte": 1,
+                "dt__quarter__lte": 1,
+                "dt__quarter__range": (1, 2),
+                "dt__time": _time,
+                "dt__time__exact": _time,
+                "dt__time__iexact": _time,
+                "dt__time__in": [_time, _time_future],
+                "dt__time__gt": _time,
+                "dt__time__lt": _time,
+                "dt__time__gte": _time,
+                "dt__time__lte": _time,
+                "dt__time__range": (_time, _time_future),
+                "dt__hour": 1,
+                "dt__hour__exact": 1,
+                "dt__hour__iexact": 1,
+                "dt__hour__in": [1, 2],
+                "dt__hour__gt": 1,
+                "dt__hour__lt": 1,
+                "dt__hour__gte": 1,
+                "dt__hour__lte": 1,
+                "dt__hour__range": (1, 2),
+                "dt__minute": 1,
+                "dt__minute__exact": 1,
+                "dt__minute__iexact": 1,
+                "dt__minute__in": [1, 2],
+                "dt__minute__gt": 1,
+                "dt__minute__lt": 1,
+                "dt__minute__gte": 1,
+                "dt__minute__lte": 1,
+                "dt__minute__range": (1, 2),
+                "dt__second": 1,
+                "dt__second__exact": 1,
+                "dt__second__iexact": 1,
+                "dt__second__in": [1, 2],
+                "dt__second__gt": 1,
+                "dt__second__lt": 1,
+                "dt__second__gte": 1,
+                "dt__second__lte": 1,
+                "dt__second__range": (1, 2),
+                "id__isnull": True,
+                "name__isnull": False,
+                "name__regex": "^(b|c)",
+                "other_name__iregex": "^(b|c)",
             },
             [
                 str(MyModel.id == 25),
                 str(MyModel.id == 25),
                 str(MyModel.name.is_(None)),
-                str(MyModel.name.ilike('abc')),
-                str(MyModel.name.like(r'%abc%')),
-                str(MyModel.name.ilike(r'%abc%')),
-                str(MyModel.name.in_(['abc', 'bca', 'dce'])),
-                str(MyModel.name.like(r'abc%')),
-                str(MyModel.name.ilike(r'abc%')),
-                str(MyModel.name.like(r'%abc')),
-                str(MyModel.name.ilike(r'%abc')),
+                str(MyModel.name.ilike("abc")),
+                str(MyModel.name.like(r"%abc%")),
+                str(MyModel.name.ilike(r"%abc%")),
+                str(MyModel.name.in_(["abc", "bca", "dce"])),
+                str(MyModel.name.like(r"abc%")),
+                str(MyModel.name.ilike(r"abc%")),
+                str(MyModel.name.like(r"%abc")),
+                str(MyModel.name.ilike(r"%abc")),
                 str(MyModel.id.between(1, 2)),
                 str(cast(MyModel.dt, Date) == _date),
                 str(cast(MyModel.dt, Date) == _date),
                 str(cast(MyModel.dt, Date) == _date),
                 str(cast(MyModel.dt, Date).in_([_date, _date_future])),
                 str(cast(MyModel.dt, Date) > _date),
                 str(cast(MyModel.dt, Date) < _date),
                 str(cast(MyModel.dt, Date) >= _date),
                 str(cast(MyModel.dt, Date) <= _date),
                 str(cast(MyModel.dt, Date).between(_date, _date_future)),
-                str(extract('year', MyModel.dt) == 2024),
-                str(extract('year', MyModel.dt) == 2024),
-                str(extract('year', MyModel.dt) == 2024),
-                str(extract('year', MyModel.dt).in_([2024, 2025])),
-                str(extract('year', MyModel.dt) > 2024),
-                str(extract('year', MyModel.dt) < 2024),
-                str(extract('year', MyModel.dt) >= 2024),
-                str(extract('year', MyModel.dt) <= 2024),
-                str(extract('year', MyModel.dt).between(2024, 2025)),
-                str(extract('isoyear', MyModel.dt) == 2025),
-                str(extract('isoyear', MyModel.dt) == 2025),
-                str(extract('isoyear', MyModel.dt) == 2025),
-                str(extract('isoyear', MyModel.dt).in_([2025, 2026])),
-                str(extract('isoyear', MyModel.dt) > 2025),
-                str(extract('isoyear', MyModel.dt) < 2025),
-                str(extract('isoyear', MyModel.dt) >= 2025),
-                str(extract('isoyear', MyModel.dt) <= 2025),
-                str(extract('isoyear', MyModel.dt).between(2024, 2025)),
-                str(extract('month', MyModel.dt) == 1),
-                str(extract('month', MyModel.dt) == 1),
-                str(extract('month', MyModel.dt) == 1),
-                str(extract('month', MyModel.dt).in_([1, 2])),
-                str(extract('month', MyModel.dt) > 1),
-                str(extract('month', MyModel.dt) < 1),
-                str(extract('month', MyModel.dt) >= 1),
-                str(extract('month', MyModel.dt) <= 1),
-                str(extract('month', MyModel.dt).between(1, 2)),
-                str(extract('day', MyModel.dt) == 2),
-                str(extract('day', MyModel.dt) == 2),
-                str(extract('day', MyModel.dt) == 2),
-                str(extract('day', MyModel.dt).in_([2, 3])),
-                str(extract('day', MyModel.dt) > 2),
-                str(extract('day', MyModel.dt) < 2),
-                str(extract('day', MyModel.dt) >= 2),
-                str(extract('day', MyModel.dt) <= 2),
-                str(extract('day', MyModel.dt).between(2, 3)),
-                str(extract('week', MyModel.dt) == 3),
-                str(extract('week', MyModel.dt) == 3),
-                str(extract('week', MyModel.dt) == 3),
-                str(extract('week', MyModel.dt).in_([3, 4])),
-                str(extract('week', MyModel.dt) > 3),
-                str(extract('week', MyModel.dt) < 3),
-                str(extract('week', MyModel.dt) >= 3),
-                str(extract('week', MyModel.dt) <= 3),
-                str(extract('week', MyModel.dt).between(3, 4)),
-                str(extract('dow', MyModel.dt) == 4),
-                str(extract('dow', MyModel.dt) == 4),
-                str(extract('dow', MyModel.dt) == 4),
-                str(extract('dow', MyModel.dt).in_([4, 5])),
-                str(extract('dow', MyModel.dt) > 4),
-                str(extract('dow', MyModel.dt) < 4),
-                str(extract('dow', MyModel.dt) >= 4),
-                str(extract('dow', MyModel.dt) <= 4),
-                str(extract('dow', MyModel.dt).between(4, 5)),
-                str(extract('isodow', MyModel.dt) == 5),
-                str(extract('isodow', MyModel.dt) == 5),
-                str(extract('isodow', MyModel.dt) == 5),
-                str(extract('isodow', MyModel.dt).in_([5, 6])),
-                str(extract('isodow', MyModel.dt) > 5),
-                str(extract('isodow', MyModel.dt) < 5),
-                str(extract('isodow', MyModel.dt) >= 5),
-                str(extract('isodow', MyModel.dt) <= 5),
-                str(extract('isodow', MyModel.dt).between(5, 6)),
-                str(extract('quarter', MyModel.dt) == 1),
-                str(extract('quarter', MyModel.dt) == 1),
-                str(extract('quarter', MyModel.dt) == 1),
-                str(extract('quarter', MyModel.dt).in_([1, 2])),
-                str(extract('quarter', MyModel.dt) > 1),
-                str(extract('quarter', MyModel.dt) < 1),
-                str(extract('quarter', MyModel.dt) >= 1),
-                str(extract('quarter', MyModel.dt) <= 1),
-                str(extract('quarter', MyModel.dt).between(1, 2)),
+                str(extract("year", MyModel.dt) == 2024),
+                str(extract("year", MyModel.dt) == 2024),
+                str(extract("year", MyModel.dt) == 2024),
+                str(extract("year", MyModel.dt).in_([2024, 2025])),
+                str(extract("year", MyModel.dt) > 2024),
+                str(extract("year", MyModel.dt) < 2024),
+                str(extract("year", MyModel.dt) >= 2024),
+                str(extract("year", MyModel.dt) <= 2024),
+                str(extract("year", MyModel.dt).between(2024, 2025)),
+                str(extract("isoyear", MyModel.dt) == 2025),
+                str(extract("isoyear", MyModel.dt) == 2025),
+                str(extract("isoyear", MyModel.dt) == 2025),
+                str(extract("isoyear", MyModel.dt).in_([2025, 2026])),
+                str(extract("isoyear", MyModel.dt) > 2025),
+                str(extract("isoyear", MyModel.dt) < 2025),
+                str(extract("isoyear", MyModel.dt) >= 2025),
+                str(extract("isoyear", MyModel.dt) <= 2025),
+                str(extract("isoyear", MyModel.dt).between(2024, 2025)),
+                str(extract("month", MyModel.dt) == 1),
+                str(extract("month", MyModel.dt) == 1),
+                str(extract("month", MyModel.dt) == 1),
+                str(extract("month", MyModel.dt).in_([1, 2])),
+                str(extract("month", MyModel.dt) > 1),
+                str(extract("month", MyModel.dt) < 1),
+                str(extract("month", MyModel.dt) >= 1),
+                str(extract("month", MyModel.dt) <= 1),
+                str(extract("month", MyModel.dt).between(1, 2)),
+                str(extract("day", MyModel.dt) == 2),
+                str(extract("day", MyModel.dt) == 2),
+                str(extract("day", MyModel.dt) == 2),
+                str(extract("day", MyModel.dt).in_([2, 3])),
+                str(extract("day", MyModel.dt) > 2),
+                str(extract("day", MyModel.dt) < 2),
+                str(extract("day", MyModel.dt) >= 2),
+                str(extract("day", MyModel.dt) <= 2),
+                str(extract("day", MyModel.dt).between(2, 3)),
+                str(extract("week", MyModel.dt) == 3),
+                str(extract("week", MyModel.dt) == 3),
+                str(extract("week", MyModel.dt) == 3),
+                str(extract("week", MyModel.dt).in_([3, 4])),
+                str(extract("week", MyModel.dt) > 3),
+                str(extract("week", MyModel.dt) < 3),
+                str(extract("week", MyModel.dt) >= 3),
+                str(extract("week", MyModel.dt) <= 3),
+                str(extract("week", MyModel.dt).between(3, 4)),
+                str(extract("dow", MyModel.dt) == 4),
+                str(extract("dow", MyModel.dt) == 4),
+                str(extract("dow", MyModel.dt) == 4),
+                str(extract("dow", MyModel.dt).in_([4, 5])),
+                str(extract("dow", MyModel.dt) > 4),
+                str(extract("dow", MyModel.dt) < 4),
+                str(extract("dow", MyModel.dt) >= 4),
+                str(extract("dow", MyModel.dt) <= 4),
+                str(extract("dow", MyModel.dt).between(4, 5)),
+                str(extract("isodow", MyModel.dt) == 5),
+                str(extract("isodow", MyModel.dt) == 5),
+                str(extract("isodow", MyModel.dt) == 5),
+                str(extract("isodow", MyModel.dt).in_([5, 6])),
+                str(extract("isodow", MyModel.dt) > 5),
+                str(extract("isodow", MyModel.dt) < 5),
+                str(extract("isodow", MyModel.dt) >= 5),
+                str(extract("isodow", MyModel.dt) <= 5),
+                str(extract("isodow", MyModel.dt).between(5, 6)),
+                str(extract("quarter", MyModel.dt) == 1),
+                str(extract("quarter", MyModel.dt) == 1),
+                str(extract("quarter", MyModel.dt) == 1),
+                str(extract("quarter", MyModel.dt).in_([1, 2])),
+                str(extract("quarter", MyModel.dt) > 1),
+                str(extract("quarter", MyModel.dt) < 1),
+                str(extract("quarter", MyModel.dt) >= 1),
+                str(extract("quarter", MyModel.dt) <= 1),
+                str(extract("quarter", MyModel.dt).between(1, 2)),
                 str(cast(MyModel.dt, Time) == _time),
                 str(cast(MyModel.dt, Time) == _time),
                 str(cast(MyModel.dt, Time) == _time),
                 str(cast(MyModel.dt, Time).in_([_time, _time_future])),
                 str(cast(MyModel.dt, Time) > _time),
                 str(cast(MyModel.dt, Time) < _time),
                 str(cast(MyModel.dt, Time) >= _time),
                 str(cast(MyModel.dt, Time) <= _time),
                 str(cast(MyModel.dt, Time).between(_time, _time_future)),
-                str(extract('hour', MyModel.dt) == 1),
-                str(extract('hour', MyModel.dt) == 1),
-                str(extract('hour', MyModel.dt) == 1),
-                str(extract('hour', MyModel.dt).in_([1, 2])),
-                str(extract('hour', MyModel.dt) > 1),
-                str(extract('hour', MyModel.dt) < 1),
-                str(extract('hour', MyModel.dt) >= 1),
-                str(extract('hour', MyModel.dt) <= 1),
-                str(extract('hour', MyModel.dt).between(1, 2)),
-                str(extract('minute', MyModel.dt) == 1),
-                str(extract('minute', MyModel.dt) == 1),
-                str(extract('minute', MyModel.dt) == 1),
-                str(extract('minute', MyModel.dt).in_([1, 2])),
-                str(extract('minute', MyModel.dt) > 1),
-                str(extract('minute', MyModel.dt) < 1),
-                str(extract('minute', MyModel.dt) >= 1),
-                str(extract('minute', MyModel.dt) <= 1),
-                str(extract('minute', MyModel.dt).between(1, 2)),
-                str(extract('second', MyModel.dt) == 1),
-                str(extract('second', MyModel.dt) == 1),
-                str(extract('second', MyModel.dt) == 1),
-                str(extract('second', MyModel.dt).in_([1, 2])),
-                str(extract('second', MyModel.dt) > 1),
-                str(extract('second', MyModel.dt) < 1),
-                str(extract('second', MyModel.dt) >= 1),
-                str(extract('second', MyModel.dt) <= 1),
-                str(extract('second', MyModel.dt).between(1, 2)),
+                str(extract("hour", MyModel.dt) == 1),
+                str(extract("hour", MyModel.dt) == 1),
+                str(extract("hour", MyModel.dt) == 1),
+                str(extract("hour", MyModel.dt).in_([1, 2])),
+                str(extract("hour", MyModel.dt) > 1),
+                str(extract("hour", MyModel.dt) < 1),
+                str(extract("hour", MyModel.dt) >= 1),
+                str(extract("hour", MyModel.dt) <= 1),
+                str(extract("hour", MyModel.dt).between(1, 2)),
+                str(extract("minute", MyModel.dt) == 1),
+                str(extract("minute", MyModel.dt) == 1),
+                str(extract("minute", MyModel.dt) == 1),
+                str(extract("minute", MyModel.dt).in_([1, 2])),
+                str(extract("minute", MyModel.dt) > 1),
+                str(extract("minute", MyModel.dt) < 1),
+                str(extract("minute", MyModel.dt) >= 1),
+                str(extract("minute", MyModel.dt) <= 1),
+                str(extract("minute", MyModel.dt).between(1, 2)),
+                str(extract("second", MyModel.dt) == 1),
+                str(extract("second", MyModel.dt) == 1),
+                str(extract("second", MyModel.dt) == 1),
+                str(extract("second", MyModel.dt).in_([1, 2])),
+                str(extract("second", MyModel.dt) > 1),
+                str(extract("second", MyModel.dt) < 1),
+                str(extract("second", MyModel.dt) >= 1),
+                str(extract("second", MyModel.dt) <= 1),
+                str(extract("second", MyModel.dt).between(1, 2)),
                 str(MyModel.id.is_(None)),
                 str(MyModel.name.is_not(None)),
-                str(MyModel.name.regexp_match('^(b|c)')),
-                str(func.lower(MyModel.other_name).regexp_match('^(b|c)')),
+                str(MyModel.name.regexp_match("^(b|c)")),
+                str(func.lower(MyModel.other_name).regexp_match("^(b|c)")),
             ],
         ),
     ],
 )
 def test_converter(  # noqa
     converter_class: type[BaseFilterConverter],
     filters: Any,  # noqa
@@ -361,50 +361,50 @@
     else:
         assert len(converted_filters) == 0
     for index, _filter in enumerate(converted_filters):
         assert str(_filter) == str(expected_result[index])
 
 
 @pytest.mark.parametrize(
-    ('converter_class', 'filters'),
+    ("converter_class", "filters"),
     [
         (
             SimpleFilterConverter,
-            {'wrong_field_name': 25},
+            {"wrong_field_name": 25},
         ),
         (
             AdvancedOperatorFilterConverter,
-            {'field': 'wrong_field_name', 'value': 'abc'},
+            {"field": "wrong_field_name", "value": "abc"},
         ),
         (
             AdvancedOperatorFilterConverter,
-            {'no_field_key': 'wrong_field_name'},
+            {"no_field_key": "wrong_field_name"},
         ),
         (
             DjangoLikeFilterConverter,
-            {'id__wrong_lookup': 25},
+            {"id__wrong_lookup": 25},
         ),
         (
             DjangoLikeFilterConverter,
-            {'dt__hour__gt__abc': 2},
+            {"dt__hour__gt__abc": 2},
         ),
         (
             DjangoLikeFilterConverter,
-            {'dt_hour__wrong__gt': 2},
+            {"dt_hour__wrong__gt": 2},
         ),
         (
             DjangoLikeFilterConverter,
-            {'wrong_field_name__gt': 2},
+            {"wrong_field_name__gt": 2},
         ),
     ],
 )
 def test_filter_not_valid(
     converter_class: type[BaseFilterConverter],
     filters: Any,  # noqa
 ) -> None:
     with pytest.raises(FilterError):
         converter_class.convert(MyModel, filters)
 
 
 def test_advanced_filter_never_situation() -> None:
-    with pytest.raises(FilterError, match=''):
-        AdvancedOperatorFilterConverter._convert_filter(MyModel, {'abc': 'abc'})  # type: ignore
+    with pytest.raises(FilterError, match=""):
+        AdvancedOperatorFilterConverter._convert_filter(MyModel, {"abc": "abc"})  # type: ignore
```

### Comparing `python_dev_utils-0.2.0/tests/sqlalchemy/filters/test_operators.py` & `python_dev_utils-1.0.6/tests/sqlalchemy/filters/test_operators.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,117 +17,117 @@
     func,
 )
 
 from dev_utils.sqlalchemy.filters import operators
 
 metadata = MetaData()
 table = Table(
-    'table',
+    "table",
     metadata,
-    Column('id', Integer, primary_key=True),
-    Column('name', String),
-    Column('dt', DateTime),
+    Column("id", Integer, primary_key=True),
+    Column("name", String),
+    Column("dt", DateTime),
 )
 now = datetime.datetime.now(tz=datetime.timezone.utc)
 _date = now.date()
 _time = now.time()
 
 
 def test_do_nothing() -> None:  # noqa
     assert operators.do_nothing() is None
 
 
 @pytest.mark.parametrize(
-    'value',
-    ['abc', 125, None, 215.125],
+    "value",
+    ["abc", 125, None, 215.125],
 )
 def test_return_value(value: Any) -> None:  # noqa
     assert operators.return_value(value) == value
 
 
 @pytest.mark.parametrize(
-    ('operator', 'a', 'b', 'result'),
+    ("operator", "a", "b", "result"),
     [
         (operators.is_, table.c.id, 1, table.c.id.is_(1)),
         (operators.is_not, table.c.id, 1, table.c.id.is_not(1)),
         (operators.between, table.c.id, (1, 2), table.c.id.between(*(1, 2))),
         (operators.between, table.c.id, (1, 2, 3), false()),
         (operators.contains, table.c.id, (1, 2, 3), table.c.id.in_((1, 2, 3))),
         (operators.django_exact, table.c.id, 1, table.c.id == 1),
         (operators.django_exact, table.c.id, None, table.c.id.is_(None)),
-        (operators.django_iexact, table.c.name, 'abc', table.c.name.ilike('abc')),
+        (operators.django_iexact, table.c.name, "abc", table.c.name.ilike("abc")),
         (operators.django_iexact, table.c.name, 123, table.c.name == 123),
         (operators.django_iexact, table.c.name, None, table.c.name.is_(None)),
-        (operators.django_contains, table.c.name, 'abc', table.c.name.like(r'%abc%')),
+        (operators.django_contains, table.c.name, "abc", table.c.name.like(r"%abc%")),
         (operators.django_contains, table.c.id, 25, table.c.id.like(25)),
-        (operators.django_icontains, table.c.name, 'abc', table.c.name.ilike(r'%abc%')),
+        (operators.django_icontains, table.c.name, "abc", table.c.name.ilike(r"%abc%")),
         (operators.django_icontains, table.c.id, 25, table.c.id.ilike(25)),
         (operators.django_in, table.c.id, (1, 2, 3), table.c.id.in_((1, 2, 3))),
-        (operators.django_startswith, table.c.name, 'abc', table.c.name.like(r'abc%')),
+        (operators.django_startswith, table.c.name, "abc", table.c.name.like(r"abc%")),
         (operators.django_startswith, table.c.id, 25, table.c.id.like(25)),
-        (operators.django_istartswith, table.c.name, 'abc', table.c.name.ilike(r'abc%')),
+        (operators.django_istartswith, table.c.name, "abc", table.c.name.ilike(r"abc%")),
         (operators.django_istartswith, table.c.id, 25, table.c.id.ilike(25)),
-        (operators.django_endswith, table.c.name, 'abc', table.c.name.like(r'%abc')),
+        (operators.django_endswith, table.c.name, "abc", table.c.name.like(r"%abc")),
         (operators.django_endswith, table.c.id, 25, table.c.id.like(25)),
-        (operators.django_iendswith, table.c.name, 'abc', table.c.name.ilike(r'%abc')),
+        (operators.django_iendswith, table.c.name, "abc", table.c.name.ilike(r"%abc")),
         (operators.django_iendswith, table.c.id, 25, table.c.id.ilike(25)),
         (operators.django_range, table.c.id, (1, 2), table.c.id.between(*(1, 2))),
         (operators.django_range, table.c.id, (1, 2, 3), false()),
         (operators.django_date, table.c.dt, now, cast(table.c.dt, Date) == _date),
-        (operators.django_year, table.c.dt, '2024', extract('year', table.c.dt) == 2024),
-        (operators.django_year, table.c.dt, 2024, extract('year', table.c.dt) == 2024),
-        (operators.django_year, table.c.dt, '2024', extract('year', table.c.dt) == '2024'),
-        (operators.django_year, table.c.dt, 2024, extract('year', table.c.dt) == '2024'),
-        (operators.django_iso_year, table.c.dt, '2024', extract('isoyear', table.c.dt) == 2024),
-        (operators.django_iso_year, table.c.dt, 2024, extract('isoyear', table.c.dt) == 2024),
-        (operators.django_iso_year, table.c.dt, '2024', extract('isoyear', table.c.dt) == '2024'),
-        (operators.django_iso_year, table.c.dt, 2024, extract('isoyear', table.c.dt) == '2024'),
-        (operators.django_month, table.c.dt, '3', extract('month', table.c.dt) == 3),
-        (operators.django_month, table.c.dt, 3, extract('month', table.c.dt) == 3),
-        (operators.django_month, table.c.dt, '3', extract('month', table.c.dt) == '3'),
-        (operators.django_month, table.c.dt, 3, extract('month', table.c.dt) == '3'),
-        (operators.django_day, table.c.dt, '3', extract('day', table.c.dt) == 3),
-        (operators.django_day, table.c.dt, 3, extract('day', table.c.dt) == 3),
-        (operators.django_day, table.c.dt, '3', extract('day', table.c.dt) == '3'),
-        (operators.django_day, table.c.dt, 3, extract('day', table.c.dt) == '3'),
-        (operators.django_week, table.c.dt, '3', extract('week', table.c.dt) == 3),
-        (operators.django_week, table.c.dt, 3, extract('week', table.c.dt) == 3),
-        (operators.django_week, table.c.dt, '3', extract('week', table.c.dt) == '3'),
-        (operators.django_week, table.c.dt, 3, extract('week', table.c.dt) == '3'),
-        (operators.django_week_day, table.c.dt, '3', extract('dow', table.c.dt) == 3),
-        (operators.django_week_day, table.c.dt, 3, extract('dow', table.c.dt) == 3),
-        (operators.django_week_day, table.c.dt, '3', extract('dow', table.c.dt) == '3'),
-        (operators.django_week_day, table.c.dt, 3, extract('dow', table.c.dt) == '3'),
-        (operators.django_iso_week_day, table.c.dt, '3', extract('isodow', table.c.dt) == 3),
-        (operators.django_iso_week_day, table.c.dt, 3, extract('isodow', table.c.dt) == 3),
-        (operators.django_iso_week_day, table.c.dt, '3', extract('isodow', table.c.dt) == '3'),
-        (operators.django_iso_week_day, table.c.dt, 3, extract('isodow', table.c.dt) == '3'),
-        (operators.django_quarter, table.c.dt, '3', extract('quarter', table.c.dt) == 3),
-        (operators.django_quarter, table.c.dt, 3, extract('quarter', table.c.dt) == 3),
-        (operators.django_quarter, table.c.dt, '3', extract('quarter', table.c.dt) == '3'),
-        (operators.django_quarter, table.c.dt, 3, extract('quarter', table.c.dt) == '3'),
+        (operators.django_year, table.c.dt, "2024", extract("year", table.c.dt) == 2024),
+        (operators.django_year, table.c.dt, 2024, extract("year", table.c.dt) == 2024),
+        (operators.django_year, table.c.dt, "2024", extract("year", table.c.dt) == "2024"),
+        (operators.django_year, table.c.dt, 2024, extract("year", table.c.dt) == "2024"),
+        (operators.django_iso_year, table.c.dt, "2024", extract("isoyear", table.c.dt) == 2024),
+        (operators.django_iso_year, table.c.dt, 2024, extract("isoyear", table.c.dt) == 2024),
+        (operators.django_iso_year, table.c.dt, "2024", extract("isoyear", table.c.dt) == "2024"),
+        (operators.django_iso_year, table.c.dt, 2024, extract("isoyear", table.c.dt) == "2024"),
+        (operators.django_month, table.c.dt, "3", extract("month", table.c.dt) == 3),
+        (operators.django_month, table.c.dt, 3, extract("month", table.c.dt) == 3),
+        (operators.django_month, table.c.dt, "3", extract("month", table.c.dt) == "3"),
+        (operators.django_month, table.c.dt, 3, extract("month", table.c.dt) == "3"),
+        (operators.django_day, table.c.dt, "3", extract("day", table.c.dt) == 3),
+        (operators.django_day, table.c.dt, 3, extract("day", table.c.dt) == 3),
+        (operators.django_day, table.c.dt, "3", extract("day", table.c.dt) == "3"),
+        (operators.django_day, table.c.dt, 3, extract("day", table.c.dt) == "3"),
+        (operators.django_week, table.c.dt, "3", extract("week", table.c.dt) == 3),
+        (operators.django_week, table.c.dt, 3, extract("week", table.c.dt) == 3),
+        (operators.django_week, table.c.dt, "3", extract("week", table.c.dt) == "3"),
+        (operators.django_week, table.c.dt, 3, extract("week", table.c.dt) == "3"),
+        (operators.django_week_day, table.c.dt, "3", extract("dow", table.c.dt) == 3),
+        (operators.django_week_day, table.c.dt, 3, extract("dow", table.c.dt) == 3),
+        (operators.django_week_day, table.c.dt, "3", extract("dow", table.c.dt) == "3"),
+        (operators.django_week_day, table.c.dt, 3, extract("dow", table.c.dt) == "3"),
+        (operators.django_iso_week_day, table.c.dt, "3", extract("isodow", table.c.dt) == 3),
+        (operators.django_iso_week_day, table.c.dt, 3, extract("isodow", table.c.dt) == 3),
+        (operators.django_iso_week_day, table.c.dt, "3", extract("isodow", table.c.dt) == "3"),
+        (operators.django_iso_week_day, table.c.dt, 3, extract("isodow", table.c.dt) == "3"),
+        (operators.django_quarter, table.c.dt, "3", extract("quarter", table.c.dt) == 3),
+        (operators.django_quarter, table.c.dt, 3, extract("quarter", table.c.dt) == 3),
+        (operators.django_quarter, table.c.dt, "3", extract("quarter", table.c.dt) == "3"),
+        (operators.django_quarter, table.c.dt, 3, extract("quarter", table.c.dt) == "3"),
         (operators.django_time, table.c.dt, _time, cast(table.c.dt, Time) == _time),
-        (operators.django_hour, table.c.dt, '3', extract('hour', table.c.dt) == 3),
-        (operators.django_hour, table.c.dt, 3, extract('hour', table.c.dt) == 3),
-        (operators.django_hour, table.c.dt, '3', extract('hour', table.c.dt) == '3'),
-        (operators.django_hour, table.c.dt, 3, extract('hour', table.c.dt) == '3'),
-        (operators.django_minute, table.c.dt, '3', extract('minute', table.c.dt) == 3),
-        (operators.django_minute, table.c.dt, 3, extract('minute', table.c.dt) == 3),
-        (operators.django_minute, table.c.dt, '3', extract('minute', table.c.dt) == '3'),
-        (operators.django_minute, table.c.dt, 3, extract('minute', table.c.dt) == '3'),
-        (operators.django_second, table.c.dt, '3', extract('second', table.c.dt) == 3),
-        (operators.django_second, table.c.dt, 3, extract('second', table.c.dt) == 3),
-        (operators.django_second, table.c.dt, '3', extract('second', table.c.dt) == '3'),
-        (operators.django_second, table.c.dt, 3, extract('second', table.c.dt) == '3'),
+        (operators.django_hour, table.c.dt, "3", extract("hour", table.c.dt) == 3),
+        (operators.django_hour, table.c.dt, 3, extract("hour", table.c.dt) == 3),
+        (operators.django_hour, table.c.dt, "3", extract("hour", table.c.dt) == "3"),
+        (operators.django_hour, table.c.dt, 3, extract("hour", table.c.dt) == "3"),
+        (operators.django_minute, table.c.dt, "3", extract("minute", table.c.dt) == 3),
+        (operators.django_minute, table.c.dt, 3, extract("minute", table.c.dt) == 3),
+        (operators.django_minute, table.c.dt, "3", extract("minute", table.c.dt) == "3"),
+        (operators.django_minute, table.c.dt, 3, extract("minute", table.c.dt) == "3"),
+        (operators.django_second, table.c.dt, "3", extract("second", table.c.dt) == 3),
+        (operators.django_second, table.c.dt, 3, extract("second", table.c.dt) == 3),
+        (operators.django_second, table.c.dt, "3", extract("second", table.c.dt) == "3"),
+        (operators.django_second, table.c.dt, 3, extract("second", table.c.dt) == "3"),
         (operators.django_isnull, table.c.name, True, table.c.name.is_(None)),
         (operators.django_isnull, table.c.name, False, table.c.name.is_not(None)),
-        (operators.django_regex, table.c.name, '^(b|c)', table.c.name.regexp_match('^(b|c)')),
+        (operators.django_regex, table.c.name, "^(b|c)", table.c.name.regexp_match("^(b|c)")),
         (
             operators.django_iregex,
             table.c.name,
-            '^(b|c)',
-            func.lower(table.c.name).regexp_match('^(b|c)'),
+            "^(b|c)",
+            func.lower(table.c.name).regexp_match("^(b|c)"),
         ),
     ],
 )
 def test_operator(operator: Callable[..., Any], a: Any, b: Any, result: Any) -> None:  # noqa
     assert str(operator(a, b)) == str(result)
```

### Comparing `python_dev_utils-0.2.0/tests/sqlalchemy/test_utils.py` & `python_dev_utils-1.0.6/tests/sqlalchemy/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,58 +10,58 @@
 
 from dev_utils.core.exc import NoModelAttributeError, NoModelRelationshipError
 from dev_utils.sqlalchemy import utils
 from tests.utils import Base, MyModel, OtherModel, generate_datetime_list
 
 
 @pytest.mark.parametrize(
-    'dt',
-    generate_datetime_list(n=10, tz=zoneinfo.ZoneInfo('UTC')),
+    "dt",
+    generate_datetime_list(n=10, tz=zoneinfo.ZoneInfo("UTC")),
 )
 def test_get_utc_now(dt: datetime.datetime) -> None:  # noqa
     with freeze_time(dt):
         assert utils.get_utc_now() == dt
 
 
 @pytest.mark.parametrize(
-    ('obj', 'expected_result'),
+    ("obj", "expected_result"),
     [
         (MyModel, True),
         (254, False),
         (MyModel.__table__, False),
     ],
 )
 def test_is_declarative(obj: Any, expected_result: bool) -> None:  # noqa: D103, ANN401, FBT001
     assert utils.is_declarative(obj) == expected_result
 
 
 @pytest.mark.parametrize(
-    ('field', 'expected_result'),
+    ("field", "expected_result"),
     [
-        ('id', MyModel.id),
-        ('name', MyModel.name),
-        ('full_name', MyModel.full_name),
-        ('get_full_name', MyModel.get_full_name()),
+        ("id", MyModel.id),
+        ("name", MyModel.name),
+        ("full_name", MyModel.full_name),
+        ("get_full_name", MyModel.get_full_name()),
     ],
 )
 def test_get_sqlalchemy_attribute(field: str, expected_result: Any) -> None:  # noqa
     assert str(utils.get_sqlalchemy_attribute(MyModel, field)) == str(expected_result)
 
 
 def test_get_sqlalchemy_attribute_incorrect() -> None:  # noqa
     with pytest.raises(NoModelAttributeError):
-        utils.get_sqlalchemy_attribute(MyModel, 'incorrect_field')
+        utils.get_sqlalchemy_attribute(MyModel, "incorrect_field")
 
 
 def test_get_registry_class() -> None:  # noqa
     assert utils.get_registry_class(MyModel) == MyModel.registry._class_registry  # type: ignore
 
 
 @pytest.mark.parametrize(
-    ('stmt', 'expected_result'),
+    ("stmt", "expected_result"),
     [
         (select(MyModel), [MyModel]),
         (select(MyModel, OtherModel), [MyModel, OtherModel]),
         (select(), []),
         (insert(MyModel), [MyModel]),
         (update(MyModel), [MyModel]),
         (delete(MyModel), [MyModel]),
@@ -74,121 +74,123 @@
     stmt: utils.Statement,
     expected_result: Sequence[type[Base]],
 ) -> None:
     assert set(utils.get_model_classes_from_statement(stmt)) == set(expected_result)
 
 
 @pytest.mark.parametrize(
-    ('name', 'expected_result'),
+    ("name", "expected_result"),
     [
-        ('MyModel', MyModel),
-        ('OtherModel', OtherModel),
-        ('NoModel', None),
+        ("MyModel", MyModel),
+        ("OtherModel", OtherModel),
+        ("NoModel", None),
     ],
 )
 def test_get_model_class_by_name(name: str, expected_result: type[Base] | None) -> None:  # noqa
     register = utils.get_registry_class(MyModel)
     assert utils.get_model_class_by_name(register, name) == expected_result
 
 
 @pytest.mark.parametrize(
-    ('name', 'expected_result'),
+    ("name", "expected_result"),
     [
-        ('my_model', MyModel),
-        ('other_model', OtherModel),
-        ('no_model', None),
+        ("my_model", MyModel),
+        ("other_model", OtherModel),
+        ("no_model", None),
     ],
 )
 def test_get_model_class_by_tablename(  # noqa
     name: str,
     expected_result: type[Base] | None,
 ) -> None:
     register = utils.get_registry_class(MyModel)
     assert utils.get_model_class_by_tablename(register, name) == expected_result
 
 
 def test_get_valid_model_class_names() -> None:  # noqa
     register = utils.get_registry_class(MyModel)
-    assert utils.get_valid_model_class_names(register) == set(['MyModel', 'OtherModel'])
+    assert utils.get_valid_model_class_names(register) == set(
+        ["MyModel", "OtherModel", "TableWithUTCDT"],
+    )
 
 
 @pytest.mark.parametrize(
-    ('model', 'expected_result'),
+    ("model", "expected_result"),
     [
         (MyModel, [OtherModel]),
         (OtherModel, [MyModel]),
     ],
 )
 def test_get_related_models(  # noqa
     model: type[DeclarativeBase],
     expected_result: list[type[DeclarativeBase]],
 ):
     assert utils.get_related_models(model) == expected_result
 
 
 def test_get_valid_field_names() -> None:  # noqa
     assert utils.get_valid_field_names(MyModel) == {
-        'id',
-        'name',
-        'other_name',
-        'dt',
-        'bl',
-        'full_name',
-        'get_full_name',
+        "id",
+        "name",
+        "other_name",
+        "dt",
+        "bl",
+        "full_name",
+        "get_full_name",
     }
 
 
 @pytest.mark.parametrize(
-    ('field', 'expected_result'),
+    ("field", "expected_result"),
     [
-        ('id', False),
-        ('name', False),
-        ('other_name', False),
-        ('full_name', True),
-        ('get_full_name', False),
+        ("id", False),
+        ("name", False),
+        ("other_name", False),
+        ("full_name", True),
+        ("get_full_name", False),
     ],
 )
 def test_is_hybrid_property(field: str, expected_result: bool) -> None:  # noqa
     insp = inspect(MyModel).all_orm_descriptors
     assert utils.is_hybrid_property(insp[field]) == expected_result
 
 
 @pytest.mark.parametrize(
-    ('field', 'expected_result'),
+    ("field", "expected_result"),
     [
-        ('id', False),
-        ('name', False),
-        ('other_name', False),
-        ('full_name', False),
-        ('get_full_name', True),
+        ("id", False),
+        ("name", False),
+        ("other_name", False),
+        ("full_name", False),
+        ("get_full_name", True),
     ],
 )
 def test_is_hybrid_method(field: str, expected_result: bool) -> None:  # noqa
     insp = inspect(MyModel).all_orm_descriptors
     assert utils.is_hybrid_method(insp[field]) == expected_result
 
 
 @pytest.mark.parametrize(
-    ('stmt', 'relationship_names', 'load_strategy', 'expected_result'),
+    ("stmt", "relationship_names", "load_strategy", "expected_result"),
     [
         (
             select(MyModel),
-            ('other_models',),
+            ("other_models",),
             joinedload,
             select(MyModel).options(joinedload(MyModel.other_models)),
         ),
         (
             select(MyModel),
-            ('other_models',),
+            ("other_models",),
             selectinload,
             select(MyModel).options(selectinload(MyModel.other_models)),
         ),
         (
             select(MyModel),
-            ('other_models',),
+            ("other_models",),
             subqueryload,
             select(MyModel).options(subqueryload(MyModel.other_models)),
         ),
     ],
 )
 def test_apply_loads(  # noqa
     stmt: Any,  # noqa
@@ -203,39 +205,39 @@
             load_strategy=load_strategy,
         ),
     ) == str(  # type: ignore
         expected_result,
     )
 
 
-def test_apply_incorrect_loads():
+def test_apply_incorrect_loads() -> None:
     with pytest.raises(NoModelRelationshipError):
-        utils.apply_loads(select(MyModel), 'no_model_rel')
+        utils.apply_loads(select(MyModel), "no_model_rel")
 
 
 @pytest.mark.parametrize(
-    ('stmt', 'relationship_names', 'left_outer_join', 'full_join', 'expected_result'),
+    ("stmt", "relationship_names", "left_outer_join", "full_join", "expected_result"),
     [
         (
             select(MyModel),
-            ('other_models',),
+            ("other_models",),
             False,
             False,
             select(MyModel).join(MyModel.other_models),
         ),
         (
             select(MyModel),
-            ('other_models',),
+            ("other_models",),
             True,
             False,
             select(MyModel).join(MyModel.other_models, isouter=True),
         ),
         (
             select(MyModel),
-            ('other_models',),
+            ("other_models",),
             False,
             True,
             select(MyModel).join(MyModel.other_models, full=True),
         ),
     ],
 )
 def test_apply_joins(  # noqa
@@ -255,8 +257,8 @@
     ) == str(  # type: ignore
         expected_result,
     )
 
 
 def test_apply_incorrect_joins() -> None:
     with pytest.raises(NoModelRelationshipError):
-        utils.apply_joins(select(MyModel), 'no_model_rel')
+        utils.apply_joins(select(MyModel), "no_model_rel")
```

### Comparing `python_dev_utils-0.2.0/tests/types.py` & `python_dev_utils-1.0.6/tests/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from typing import TYPE_CHECKING, Any, Protocol, TypeVar
 
 if TYPE_CHECKING:
     from sqlalchemy.ext.asyncio import AsyncSession
     from sqlalchemy.orm import Session
 
 
-T = TypeVar('T', covariant=True)
+T = TypeVar("T", covariant=True)
 
 
 class SyncFactoryFunctionProtocol(Protocol[T]):
     """Protocol for Sync functions-factories that create db items."""
 
     @staticmethod
     def __call__(  # noqa: D102
-        session: 'Session',
+        session: "Session",
         *,
         commit: bool = False,
         **kwargs: Any,  # noqa: ANN401
-    ) -> T:
-        ...
+    ) -> T: ...
 
 
 class AsyncFactoryFunctionProtocol(Protocol[T]):
     """Protocol for Sync functions-factories that create db items."""
 
     @staticmethod
     async def __call__(  # noqa: D102
-        session: 'AsyncSession',
+        session: "AsyncSession",
         *,
         commit: bool = False,
         **kwargs: Any,  # noqa: ANN401
-    ) -> T:
-        ...
+    ) -> T: ...
```

### Comparing `python_dev_utils-0.2.0/tests/utils.py` & `python_dev_utils-1.0.6/tests/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 
 from sqlalchemy import ForeignKey, inspect
 from sqlalchemy.exc import SQLAlchemyError
 from sqlalchemy.ext.hybrid import hybrid_method, hybrid_property
 from sqlalchemy.orm import DeclarativeBase, Mapped, mapped_column, relationship
 from sqlalchemy_utils import create_database, database_exists, drop_database  # type: ignore
 
+from dev_utils.sqlalchemy.types.datetime import UTCDateTime  # type: ignore
+
 if TYPE_CHECKING:
     from collections.abc import Sequence
 
     from sqlalchemy.ext.asyncio import AsyncSession
     from sqlalchemy.orm import Session
 
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 def coin_flip() -> bool:
     """Coin flip: True or False."""
     return bool(random.getrandbits(1))
 
 
@@ -41,119 +43,119 @@
     res = [now]
     for i in range(1, n):
         delta = datetime.timedelta(days=i)
         res.append(now + delta)
     return res
 
 
-def assert_compare_db_items(item1: 'DeclarativeBase', item2: 'DeclarativeBase') -> None:
+def assert_compare_db_items(item1: "DeclarativeBase", item2: "DeclarativeBase") -> None:
     """Assert if 2 models not compare to each other."""
     if item1 is item2:
         return
     assert (
         item1.__class__ == item2.__class__
-    ), 'item1 and item2 has different classes. Cant compare.'
+    ), "item1 and item2 has different classes. Cant compare."
     item1_fields = set(inspect(item1.__class__).columns.keys())
     item2_fields = set(inspect(item2.__class__).columns.keys())
-    assert item1_fields == item2_fields, ''
+    assert item1_fields == item2_fields, ""
     for field in item1_fields:
         assert getattr(
             item1,
             field,
-            float('nan'),
+            float("nan"),
         ) == getattr(
             item2,
             field,
-            float('nan'),
-        ), f'field {field} is not compared. Different values.'
+            float("nan"),
+        ), f"field {field} is not compared. Different values."
 
 
 def assert_compare_db_item_list(
-    items1: 'Sequence[DeclarativeBase]',
-    items2: 'Sequence[DeclarativeBase]',
+    items1: "Sequence[DeclarativeBase]",
+    items2: "Sequence[DeclarativeBase]",
 ) -> None:
     """Assert if 2 model lists not compare to each other."""
-    assert len(items1) == len(items2), f'Different lists count: {len(items1)} != {len(items2)}'
+    assert len(items1) == len(items2), f"Different lists count: {len(items1)} != {len(items2)}"
     for item1, item2 in zip(
         sorted(items1, key=lambda x: x.id),  # type: ignore
         sorted(items2, key=lambda x: x.id),  # type: ignore
         strict=True,
     ):
         assert_compare_db_items(item1, item2)
 
 
 def assert_compare_db_item_with_dict(
-    item: 'DeclarativeBase',
+    item: "DeclarativeBase",
     data: dict[str, Any],
     *,
     skip_keys_check: bool = False,
 ) -> None:
     """Assert if model not compare to dict."""
     data_fields = set(data.keys())
     item_fields = set(inspect(item.__class__).columns.keys())
-    msg = f'data fields ({data_fields}) are not compare to item fields ({item_fields}).'
+    msg = f"data fields ({data_fields}) are not compare to item fields ({item_fields})."
     if not skip_keys_check:
         assert set(data_fields).issubset(item_fields), msg
     for field, value in data.items():
-        item_field_value = getattr(item, field, float('nan'))
+        item_field_value = getattr(item, field, float("nan"))
         msg = (
             f'data ({field=} {value=}) not compare '
             f'to item ({field=} value={getattr(item, field, "<not present in item>")})'
         )
         assert item_field_value == value, msg
 
 
 def assert_compare_db_item_list_with_dict(
-    items: 'Sequence[DeclarativeBase]',
+    items: "Sequence[DeclarativeBase]",
     data: dict[str, Any],
     *,
     skip_keys_check: bool = False,
 ) -> None:
     """Assert if list of models not compare to dict."""
     data_fields = set(data.keys())
     for item in items:
         item_class = item.__class__
         item_fields = set(inspect(item_class).columns.keys())
         msg = (
-            f'data fields ({data_fields}) are not compare to item '
-            f'({item_class}) fields ({item_fields}).'
+            f"data fields ({data_fields}) are not compare to item "
+            f"({item_class}) fields ({item_fields})."
         )
         if not skip_keys_check:
             assert set(data_fields).issubset(item_fields), msg
         for field, value in data.items():
-            item_field_value = getattr(item, field, float('nan'))
+            item_field_value = getattr(item, field, float("nan"))
             msg = (
                 f'data ({field=} {value=}) not compare '
                 f'to item ({field=} value={getattr(item, field, "<not present in item>")})'
             )
             assert item_field_value == value, msg
 
 
-def assert_compare_db_item_none_fields(item: 'DeclarativeBase', none_fields: set[str]) -> None:
+def assert_compare_db_item_none_fields(item: "DeclarativeBase", none_fields: set[str]) -> None:
     """Assert compare model instance fields for none value."""
     for field in none_fields:
-        item_value = getattr(item, field, float('nan'))
+        item_value = getattr(item, field, float("nan"))
         msg = f'Field "{field}" is not None.'
         assert item_value is None, msg
 
 
 def assert_compare_db_item_list_none_fields(
-    items: 'Sequence[DeclarativeBase]',
+    items: "Sequence[DeclarativeBase]",
     none_fields: set[str],
 ) -> None:
     """Assert compare list of model instances fields for none value."""
     for item in items:
         for field in none_fields:
-            item_value = getattr(item, field, float('nan'))
+            item_value = getattr(item, field, float("nan"))
             msg = f'Field "{field}" of item {item} is not None.'
             assert item_value is None, msg
 
 
 def create_db_item_sync(
-    session: 'Session',
+    session: "Session",
     model: type[T],
     params: dict[str, Any],
     *,
     commit: bool = False,
 ) -> T:
     """Create SQLAlchemy model item and add it to DB."""
     item = model(**params)
@@ -163,15 +165,15 @@
     except SQLAlchemyError:
         session.rollback()
         raise
     return item
 
 
 async def create_db_item_async(
-    session: 'AsyncSession',
+    session: "AsyncSession",
     model: type[T],
     params: dict[str, Any],
     *,
     commit: bool = False,
 ) -> T:
     """Create SQLAlchemy model item and add it to DB."""
     item = model(**params)
@@ -185,41 +187,48 @@
 
 
 class Base(DeclarativeBase):  # noqa
     pass
 
 
 class MyModel(Base):  # noqa
-    __tablename__ = 'my_model'
+    __tablename__ = "my_model"
 
     id: Mapped[int] = mapped_column(primary_key=True)  # noqa
     name: Mapped[str | None]
     other_name: Mapped[str | None]
     dt: Mapped[datetime.datetime | None]
     bl: Mapped[bool | None]
-    other_models: Mapped[list['OtherModel']] = relationship(back_populates='my_model', uselist=True)
+    other_models: Mapped[list["OtherModel"]] = relationship(back_populates="my_model", uselist=True)
 
     @hybrid_property
     def full_name(self) -> str:  # noqa # type: ignore
-        return self.name + '' + self.other_name  # type: ignore
+        return self.name + "" + self.other_name  # type: ignore
 
     @hybrid_method
     def get_full_name(self) -> str:  # noqa # type: ignore
-        return self.name + '' + self.other_name  # type: ignore
+        return self.name + "" + self.other_name  # type: ignore
 
 
 class OtherModel(Base):  # noqa
-    __tablename__ = 'other_model'
+    __tablename__ = "other_model"
 
     id: Mapped[int] = mapped_column(primary_key=True)  # noqa
     name: Mapped[str]
     other_name: Mapped[str]
-    my_model_id: Mapped[int | None] = mapped_column(ForeignKey('my_model.id', ondelete='CASCADE'))
-    my_model: Mapped['MyModel'] = relationship(back_populates='other_models', uselist=False)
+    my_model_id: Mapped[int | None] = mapped_column(ForeignKey("my_model.id", ondelete="CASCADE"))
+    my_model: Mapped["MyModel"] = relationship(back_populates="other_models", uselist=False)
 
     @hybrid_property
     def full_name(self):  # noqa
-        return self.name + '' + self.other_name
+        return self.name + "" + self.other_name
 
     @hybrid_method
     def get_full_name(self):  # noqa
-        return self.name + '' + self.other_name
+        return self.name + "" + self.other_name
+
+
+class TableWithUTCDT(Base):  # noqa: D101
+    __tablename__ = "table_with_UTC_dt"
+
+    id: Mapped[int] = mapped_column(primary_key=True)  # noqa
+    dt_field: Mapped[datetime.datetime] = mapped_column(UTCDateTime)
```

### Comparing `python_dev_utils-0.2.0/PKG-INFO` & `python_dev_utils-1.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: python_dev_utils
-Version: 0.2.0
+Version: 1.0.6
 Summary: My project utils package, that I use in my projects.
 Author-Email: Dmitriy Lunev <dima.lunev14@gmail.com>
 License: MIT
 Requires-Python: >=3.11
 Provides-Extra: profiling
-Provides-Extra: sqlalchemy_filters
+Provides-Extra: sqlalchemy-filters
 Requires-Dist: fastapi>=0.110.0; extra == "profiling"
 Requires-Dist: sqlalchemy>=2.0.28; extra == "profiling"
 Requires-Dist: sqlalchemy>=2.0.28; extra == "sqlalchemy-filters"
 Description-Content-Type: text/markdown
 
+
 # Dev utils
 
+![coverage](./coverage.svg)
+
 ## For what?
 
 I made this project to avoid copy-pasting with utils in my projects. I was aiming to simplify
 working with sqlalchemy, FastAPI and other libs.
 
 ## Profiling
```

