# Comparing `tmp/rlogging-1.1.9.tar.gz` & `tmp/rlogging-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlogging-1.1.9.tar", max compression
+gzip compressed data, was "rlogging-1.2.0.tar", max compression
```

## Comparing `rlogging-1.1.9.tar` & `rlogging-1.2.0.tar`

### file list

```diff
@@ -1,21 +1,19 @@
--rw-r--r--   0        0        0     1853 2023-08-25 20:21:43.714798 rlogging-1.1.9/pyproject.toml
--rw-r--r--   0        0        0     1465 2023-08-25 20:21:43.714798 rlogging-1.1.9/readme.md
--rw-r--r--   0        0        0       78 2023-08-25 20:21:43.714798 rlogging-1.1.9/rlogging/__init__.py
--rw-r--r--   0        0        0     3199 2023-08-25 20:21:43.714798 rlogging-1.1.9/rlogging/adapters.py
--rw-r--r--   0        0        0      125 2023-08-25 20:21:43.714798 rlogging-1.1.9/rlogging/filters.py
--rw-r--r--   0        0        0     2682 2023-08-25 20:21:43.714798 rlogging-1.1.9/rlogging/formatters.py
--rw-r--r--   0        0        0      990 2023-08-25 20:21:43.714798 rlogging-1.1.9/rlogging/handlers.py
--rw-r--r--   0        0        0        0 2023-08-25 20:25:56.729678 rlogging-1.1.9/rlogging/integration/__init__.py
--rw-r--r--   0        0        0        0 2023-08-25 20:25:56.729678 rlogging-1.1.9/rlogging/integration/aiogram/__init__.py
--rw-r--r--   0        0        0        0 2023-08-25 20:25:56.729678 rlogging-1.1.9/rlogging/integration/django/__init__.py
--rw-r--r--   0        0        0      727 2023-08-25 20:21:43.714798 rlogging-1.1.9/rlogging/integration/django/adapters.py
--rw-r--r--   0        0        0      125 2023-08-25 20:21:43.714798 rlogging-1.1.9/rlogging/integration/django/admin.py
--rw-r--r--   0        0        0      215 2023-08-25 20:21:43.714798 rlogging-1.1.9/rlogging/integration/django/apps.py
--rw-r--r--   0        0        0        0 2023-08-25 20:25:56.729678 rlogging-1.1.9/rlogging/integration/django/handlers.py
--rw-r--r--   0        0        0     1483 2023-08-25 20:21:43.714798 rlogging-1.1.9/rlogging/integration/django/middleware.py
--rw-r--r--   0        0        0       72 2023-08-25 20:21:43.714798 rlogging-1.1.9/rlogging/integration/django/models.py
--rw-r--r--   0        0        0     2019 2023-08-25 20:21:43.714798 rlogging-1.1.9/rlogging/integration/django/signals.py
--rw-r--r--   0        0        0        0 2023-08-25 20:25:56.729678 rlogging-1.1.9/rlogging/integration/fastapi/__init__.py
--rw-r--r--   0        0        0       50 2023-08-25 20:21:43.714798 rlogging-1.1.9/rlogging/namespaces.py
--rw-r--r--   0        0        0     1542 2023-08-25 20:21:43.714798 rlogging-1.1.9/rlogging/utils.py
--rw-r--r--   0        0        0     2496 1970-01-01 00:00:00.000000 rlogging-1.1.9/PKG-INFO
+-rw-r--r--   0        0        0     2029 2024-04-14 00:35:06.288466 rlogging-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1540 2024-04-14 00:35:06.288466 rlogging-1.2.0/readme.md
+-rw-r--r--   0        0        0       78 2024-04-14 00:35:06.288466 rlogging-1.2.0/rlogging/__init__.py
+-rw-r--r--   0        0        0     1842 2024-04-14 00:35:06.288466 rlogging-1.2.0/rlogging/adapters.py
+-rw-r--r--   0        0        0      125 2024-04-14 00:35:06.288466 rlogging-1.2.0/rlogging/filters.py
+-rw-r--r--   0        0        0     2673 2024-04-14 00:35:06.288466 rlogging-1.2.0/rlogging/formatters.py
+-rw-r--r--   0        0        0      990 2024-04-14 00:35:06.288466 rlogging-1.2.0/rlogging/handlers.py
+-rw-r--r--   0        0        0        0 2024-04-14 00:35:06.344466 rlogging-1.2.0/rlogging/integration/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 00:35:06.348466 rlogging-1.2.0/rlogging/integration/aiogram/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-14 00:35:06.348466 rlogging-1.2.0/rlogging/integration/django/__init__.py
+-rw-r--r--   0        0        0      769 2024-04-14 00:35:06.288466 rlogging-1.2.0/rlogging/integration/django/adapters.py
+-rw-r--r--   0        0        0      215 2024-04-14 00:35:06.288466 rlogging-1.2.0/rlogging/integration/django/apps.py
+-rw-r--r--   0        0        0        0 2024-04-14 00:35:06.348466 rlogging-1.2.0/rlogging/integration/django/handlers.py
+-rw-r--r--   0        0        0     1795 2024-04-14 00:35:06.288466 rlogging-1.2.0/rlogging/integration/django/middleware.py
+-rw-r--r--   0        0        0     2079 2024-04-14 00:35:06.288466 rlogging-1.2.0/rlogging/integration/django/signals.py
+-rw-r--r--   0        0        0        0 2024-04-14 00:35:06.348466 rlogging-1.2.0/rlogging/integration/fastapi/__init__.py
+-rw-r--r--   0        0        0       65 2024-04-14 00:35:06.288466 rlogging-1.2.0/rlogging/namespaces.py
+-rw-r--r--   0        0        0     1553 2024-04-14 00:35:06.288466 rlogging-1.2.0/rlogging/utils.py
+-rw-r--r--   0        0        0     2477 1970-01-01 00:00:00.000000 rlogging-1.2.0/PKG-INFO
```

### Comparing `rlogging-1.1.9/pyproject.toml` & `rlogging-1.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -9,46 +9,55 @@
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 packages = [{include = "rlogging"}]
 
 [tool.poetry.urls]
 homepage = "https://gitlab.com/rocshers/python/rlogging"
 repository = "https://gitlab.com/rocshers/python/rlogging"
-source = "https://gitlab.com/rocshers/python/rlogging.git"
-documentation = "https://gitlab.com/rocshers/python/rlogging/-/blob/release/readme.md"
+documentation = "https://rocshers.gitlab.io/python/rlogging/"
 changelog = "https://gitlab.com/rocshers/python/rlogging/-/releases"
 issues = "https://gitlab.com/rocshers/python/rlogging/-/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 ruff = "^0.0.260"
 black = "^23.3.0"
 isort = "^5.12.0"
 pre-commit = "^3.2.2"
 mypy = "^1.2.0"
-django = "^4.1.7"
+pre-commit-hooks = "^4.5.0"
+
+[tool.poetry.group.docs.dependencies]
+mkdocs = "^1.5.3"
+mkdocs-material = "^9.5.2"
+mkdocstrings = {extras = ["python"], version = "^0.24.0"}
+griffe-typingdoc = "^0.2.4"
+
+[tool.poetry.group.extra.dependencies]
+django = "^4"
 
 [tool.black]
 skip-string-normalization = true
 line-length = 120
+target-version = ["py37"]
 
 [tool.isort]
 profile = "black"
 line_length = 120
 
 [tool.ruff]
 select = ["A", "B", "C", "E", "F", "I", "UP"]
 fixable = ["A", "B", "C", "D", "E", "F", "I", "UP"]
 ignore = ["UP004", "D100", "D101", "D102", "D103", "D104", "D107", "D400", "D415"]
 line-length = 120
-target-version = "py38"
+target-version = "py37"
 
 [tool.coverage.run]
 omit = [
     "*/tests/*",
     "install-poetry.py"
 ]
```

### Comparing `rlogging-1.1.9/readme.md` & `rlogging-1.2.0/readme.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # rLogging
 
 Module with frequently used functions for advanced logging
 
 [![PyPI](https://img.shields.io/pypi/v/rlogging)](https://pypi.org/project/rlogging/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rlogging)](https://pypi.org/project/rlogging/)
 [![GitLab last commit](https://img.shields.io/gitlab/last-commit/rocshers/python/rlogging)](https://gitlab.com/rocshers/python/rlogging)
+[![Docs](https://img.shields.io/badge/docs-exist-blue)](https://rocshers.gitlab.io/python/rlogging/)
 
-[![Test coverage](https://codecov.io/gitlab/rocshers:python/rlogging/branch/release/graph/badge.svg?token=RPFNZ8SBQ6)](https://codecov.io/gitlab/rocshers:python/rlogging)
+[![Test coverage](https://codecov.io/gitlab/rocshers:python/rlogging/graph/badge.svg)](https://codecov.io/gitlab/rocshers:python/rlogging)
 [![Downloads](https://static.pepy.tech/badge/rlogging)](https://pepy.tech/project/rlogging)
 [![GitLab stars](https://img.shields.io/gitlab/stars/rocshers/python/rlogging)](https://gitlab.com/rocshers/python/rlogging)
 
 ## Functionality
 
 - Formatters
   - **JsonFormatter** - Convert log to json
@@ -20,29 +21,29 @@
   - **HttpLoggerAdapter**
 - Django
   - **DjangoLoggerAdapter**
   - **LoggingMiddleware**
 
 ## Usage
 
-```
+```bash
 pip install rlogging
 ```
 
 ### Python
 
 Normal logging setup with new classes
 
 ```bash
 
 ```
 
 ### Django
 
-```bash
+```python
 # settings.py
 
 INSTALLED_APPS = [
     ...
     'rlogging.integration.django',
     ...
 ]
```

### Comparing `rlogging-1.1.9/rlogging/adapters.py` & `rlogging-1.2.0/rlogging/adapters.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,69 +1,50 @@
-import inspect
 import logging
-import sys
 import uuid
-from types import FrameType
-from typing import Any, Optional, Tuple
+from typing import Any, Dict, Optional, Tuple
 
 
 class RLoggerAdapter(logging.LoggerAdapter):
-    """Путь логирования
+    """Адаптер над логгером
 
-    Создание логов, через флоу позволяет обоготить их
+    Позволяет логировать с передачей котекста
 
     """
 
     flow_id: uuid.UUID
 
-    def __init__(self, logger: logging.Logger, extra: Optional[dict] = None) -> None:
+    def __init__(self, logger: logging.Logger, extra: Optional[Dict[str, Any]] = None) -> None:
         extra = extra if extra is not None else {}
 
         super().__init__(logger, extra)
 
         self.flow_id = uuid.uuid1()
 
-    def _extra_update(self, kwargs: dict, extra: dict):
-        kwargs['extra'] = extra | kwargs.get('extra', {})
+    def _extra_update(self, kwargs: Dict[str, Any], extra: Dict[str, Any]):
+        extra = extra.copy()
 
-    def get_frame(self, stacklevel: int = 41) -> FrameType:
-        return sys._getframe(5)
+        extra.update(kwargs.get('extra', {}))
 
-    def get_class_info(self) -> Optional[dict]:
-        frame = self.get_frame()
-        obj = frame.f_locals.get('self')
+        kwargs['extra'] = extra
 
-        if obj is None:
-            return None
-
-        module = inspect.getmodule(obj.__class__)
-        class_path = f'{module.__name__}.{obj.__class__.__name__}'
-
-        return {'class': class_path, 'object': obj, 'object_id': id(obj)}
-
-    def process(self, msg: Any, kwargs: dict) -> Tuple[Any, dict]:
+    def process(self, msg: Any, kwargs: Dict[str, Any]) -> Tuple[Any, Dict[str, Any]]:
         kwargs.setdefault('stacklevel', 2)
 
         extra = {
             'flow_id': self.flow_id,
         }
 
         self._extra_update(kwargs, extra)
         self._extra_update(kwargs, self.extra)
 
-        if extra := self.get_class_info():
-            self._extra_update(kwargs, extra)
-
         return msg, kwargs
 
 
 class AppLoggerAdapter(RLoggerAdapter):
-    def queries(self, queries: list, *args, **kwargs):
-        kwargs.setdefault('stacklevel', 4)
-        self.info(f'processing queries: {len(queries)}', **kwargs)
+    pass
 
 
 class HttpLoggerAdapter(AppLoggerAdapter):
     """Флоу для логирования веб запросов/ответов"""
 
     def request(
         self,
@@ -91,36 +72,7 @@
             'http': {
                 'code': code,
             },
         }
         self._extra_update(kwargs, extra)
 
         self.info('http response', **kwargs)
-
-    def processing(
-        self,
-        path: str,
-        route: str,
-        route_name: str,
-        view: str,
-        view_args: tuple,
-        view_kwargs: dict,
-        namespace: str,
-        *args,
-        **kwargs,
-    ):
-        kwargs.setdefault('stacklevel', 4)
-
-        extra = {
-            'processing': {
-                'path': path,
-                'route': route,
-                'route_name': route_name,
-                'view': view,
-                'view_args': view_args,
-                'view_kwargs': view_kwargs,
-                'namespace': namespace,
-            },
-        }
-        self._extra_update(kwargs, extra)
-
-        self.info('http process_view', **kwargs)
```

### Comparing `rlogging-1.1.9/rlogging/formatters.py` & `rlogging-1.2.0/rlogging/formatters.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 
     def get_data_from_record(self, record: logging.LogRecord) -> dict:
         try:
             record.message = record.msg % record.args
 
         except:
             record.message = record.msg
-        
 
         if isinstance(record.msg, BaseException):
             record.exception = record.msg
             record.message = str(record.msg)
 
         record_data = {}
         record_data.update(self.default_extra)
```

### Comparing `rlogging-1.1.9/rlogging/handlers.py` & `rlogging-1.2.0/rlogging/handlers.py`

 * *Files identical despite different names*

### Comparing `rlogging-1.1.9/rlogging/integration/django/adapters.py` & `rlogging-1.2.0/rlogging/integration/django/adapters.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,22 +4,20 @@
 from rlogging import HttpLoggerAdapter
 
 
 class DjangoLoggerAdapter(HttpLoggerAdapter):
     def request(self, request: WSGIRequest, *args, **kwargs):
         kwargs.setdefault('stacklevel', 5)
 
-        path = request.path
-        view_func = request.resolver_match
+        kwargs['extra'] = kwargs.get('extra', {})
+        kwargs['extra'].update({'django': {'path': request.path, 'view_func': request.resolver_match}})
 
         return super().request(
             request.build_absolute_uri(),
             request.method,
-            path,
-            view_func,
             *args,
             **kwargs,
         )
 
     def response(self, response: HttpResponse, *args, **kwargs):
         kwargs.setdefault('stacklevel', 5)
         return super().response(response.status_code, *args, **kwargs)
```

### Comparing `rlogging-1.1.9/rlogging/integration/django/middleware.py` & `rlogging-1.2.0/rlogging/integration/django/middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,35 +12,47 @@
 
 class LoggingMiddleware(object):
     def __init__(self, get_response):
         self.get_response = get_response
 
     def __call__(self, request: WSGIRequest):
         request.logger = DjangoLoggerAdapter(
-            logging.getLogger(namespaces.HTTP), {'queries': LazyStrCallable(len, connection.queries)}
+            logging.getLogger(namespaces.HTTP),
+            {
+                'queries': LazyStrCallable(len, connection.queries),
+            },
         )
         request.logger.request(request)
 
         response: HttpResponse = self.get_response(request)
 
-        request.logger.queries(connection.queries)
         request.logger.response(response)
 
         return response
 
     def process_view(self, request: WSGIRequest, view_func: Any, view_args: tuple, view_kwargs: dict):
         request.logger: DjangoLoggerAdapter = request.logger
-        request.logger.processing(
-            request.path,
-            request.resolver_match.route,
-            request.resolver_match.url_name,
-            view_func.__name__,
-            view_args,
-            view_kwargs,
-            request.resolver_match.namespace,
+
+        request.logger.info(
+            'http process_view',
+            extra={
+                'processing': {
+                    'path': request.path,
+                    'route': request.resolver_match.route,
+                    'route_name': request.resolver_match.url_name,
+                    'view': view_func.__name__,
+                    'view_args': view_args,
+                    'view_kwargs': view_kwargs,
+                    'namespace': request.resolver_match.namespace,
+                },
+            },
         )
 
     def process_exception(self, request, exception):
         request.logger.info(
             'http process_exception',
-            extra={'processing': {'exception': exception}},
+            extra={
+                'processing': {
+                    'exception': exception,
+                }
+            },
         )
```

### Comparing `rlogging-1.1.9/rlogging/integration/django/signals.py` & `rlogging-1.2.0/rlogging/integration/django/signals.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from typing import Any
 
 from django.core.signals import *
 from django.db.models.signals import *
 
 from rlogging import namespaces
 
 logger = logging.getLogger(namespaces.DB)
@@ -29,19 +30,19 @@
     # plan(migration plan), apps(from django.apps import apps : Apps)
     post_migrate,
     # sender(AppConfig), app_config(AppConfig), verbosity, interactive(Bool),stdout,using(Model verbose_name),
     # plan(migration plan), apps(from django.apps import apps : Apps)
 ]
 
 
-def signal_handler(sender, *args, **kwargs):
+def signal_handler(sender: Any, *args: Any, **kwargs: Any):
     logger.info(
-        'django signal',
+        f'received django signal: {sender}',
         extra={
-            'processing': {
+            'djang_signal': {
                 'sender': sender,
                 'args': args,
                 'kwargs': kwargs,
             }
         },
     )
```

### Comparing `rlogging-1.1.9/rlogging/utils.py` & `rlogging-1.2.0/rlogging/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import traceback
 import types
 import uuid
 from typing import Any, Callable
 
 
 class LazyStrCallable(object):
-    def __init__(self, target_func: Callable, *args, **kwargs) -> None:
+    def __init__(self, target_func: Callable[[Any], Any], *args: Any, **kwargs: Any) -> None:
         self.target = target_func
         self.args = args
         self.kwargs = kwargs
 
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         return self.target(*self.args, **self.kwargs)
 
@@ -34,20 +34,21 @@
     if isinstance(obj, types.TracebackType):
         return ''.join(traceback.format_tb(obj)).strip()
 
     return str(obj)
 
 
 def flatten_dict(dict_data: dict, parent_key: str = '', sep: str = '.'):
-    """
-    Рекурсивно преобразует вложенный словарь в одномерный словарь
-    с объединенными ключами разных уровней через точку.
-    """
+    """Рекурсивно преобразует вложенный словарь в одномерный словарь с объединенными ключами разных уровней через точку"""
 
     items = []
+
     for k, v in dict_data.items():
         new_key = f'{parent_key}{sep}{k}' if parent_key else k
+
         if isinstance(v, dict):
             items.extend(flatten_dict(v, new_key, sep=sep).items())
+
         else:
             items.append((new_key, v))
+
     return dict(items)
```

### Comparing `rlogging-1.1.9/PKG-INFO` & `rlogging-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: rlogging
-Version: 1.1.9
+Version: 1.2.0
 Summary: 
 License: MIT
 Author: irocshers
 Author-email: develop.iam@rocshers.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Project-URL: changelog, https://gitlab.com/rocshers/python/rlogging/-/releases
-Project-URL: documentation, https://gitlab.com/rocshers/python/rlogging/-/blob/release/readme.md
+Project-URL: documentation, https://rocshers.gitlab.io/python/rlogging/
 Project-URL: homepage, https://gitlab.com/rocshers/python/rlogging
 Project-URL: issues, https://gitlab.com/rocshers/python/rlogging/-/issues
 Project-URL: repository, https://gitlab.com/rocshers/python/rlogging
-Project-URL: source, https://gitlab.com/rocshers/python/rlogging.git
 Description-Content-Type: text/markdown
 
 # rLogging
 
 Module with frequently used functions for advanced logging
 
 [![PyPI](https://img.shields.io/pypi/v/rlogging)](https://pypi.org/project/rlogging/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rlogging)](https://pypi.org/project/rlogging/)
 [![GitLab last commit](https://img.shields.io/gitlab/last-commit/rocshers/python/rlogging)](https://gitlab.com/rocshers/python/rlogging)
+[![Docs](https://img.shields.io/badge/docs-exist-blue)](https://rocshers.gitlab.io/python/rlogging/)
 
-[![Test coverage](https://codecov.io/gitlab/rocshers:python/rlogging/branch/release/graph/badge.svg?token=RPFNZ8SBQ6)](https://codecov.io/gitlab/rocshers:python/rlogging)
+[![Test coverage](https://codecov.io/gitlab/rocshers:python/rlogging/graph/badge.svg)](https://codecov.io/gitlab/rocshers:python/rlogging)
 [![Downloads](https://static.pepy.tech/badge/rlogging)](https://pepy.tech/project/rlogging)
 [![GitLab stars](https://img.shields.io/gitlab/stars/rocshers/python/rlogging)](https://gitlab.com/rocshers/python/rlogging)
 
 ## Functionality
 
 - Formatters
   - **JsonFormatter** - Convert log to json
@@ -43,29 +43,29 @@
   - **HttpLoggerAdapter**
 - Django
   - **DjangoLoggerAdapter**
   - **LoggingMiddleware**
 
 ## Usage
 
-```
+```bash
 pip install rlogging
 ```
 
 ### Python
 
 Normal logging setup with new classes
 
 ```bash
 
 ```
 
 ### Django
 
-```bash
+```python
 # settings.py
 
 INSTALLED_APPS = [
     ...
     'rlogging.integration.django',
     ...
 ]
```

