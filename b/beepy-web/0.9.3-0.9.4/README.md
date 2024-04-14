# Comparing `tmp/beepy_web-0.9.3.tar.gz` & `tmp/beepy_web-0.9.4.tar.gz`

## Comparing `beepy_web-0.9.3.tar` & `beepy_web-0.9.4.tar`

### file list

```diff
@@ -1,53 +1,54 @@
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 beepy_web-0.9.3/.env.template
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 beepy_web-0.9.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 beepy_web-0.9.3/.python-version
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 beepy_web-0.9.3/requirements.txt
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/__init__.py
--rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/attrs.py
--rw-r--r--   0        0        0     7314 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/children.py
--rw-r--r--   0        0        0    12926 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/components.py
--rw-r--r--   0        0        0     8964 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/context.py
--rw-r--r--   0        0        0    20944 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/framework.py
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/listeners.py
--rw-r--r--   0        0        0     4705 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/router.py
--rw-r--r--   0        0        0     7926 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/style.py
--rw-r--r--   0        0        0     5294 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/tags.py
--rw-r--r--   0        0        0     6701 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/trackable.py
--rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/types.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/dev/__init__.py
--rwxr-xr-x   0        0        0     5051 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/dev/__main__.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/dev/example.html
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/dev/example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/modules/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/modules/actions.py
--rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/modules/context_menu.py
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/modules/local_storage.py
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/modules/modal.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/modules/plot.py
--rw-r--r--   0        0        0     5151 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/modules/table.py
--rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/modules/tabs.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/utils/__init__.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/utils/api.py
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/utils/asyncio.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/utils/common.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/utils/dev.py
--rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/utils/import_hooks.py
--rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/utils/internal.py
--rw-r--r--   0        0        0     8363 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/utils/js.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 beepy_web-0.9.3/beepy/utils/js_py.py
--rw-r--r--   0        0        0   179387 2020-02-02 00:00:00.000000 beepy_web-0.9.3/web/package-lock.json
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 beepy_web-0.9.3/web/package.json
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 beepy_web-0.9.3/web/webpack.dev.js
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 beepy_web-0.9.3/web/webpack.prod.js
--rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 beepy_web-0.9.3/web/src/beepy.js
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 beepy_web-0.9.3/web/src/dev-server.js
--rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 beepy_web-0.9.3/web/src/files.js
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 beepy_web-0.9.3/web/src/index.js
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 beepy_web-0.9.3/web/src/main.css
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 beepy_web-0.9.3/web/src/python.js
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 beepy_web-0.9.3/web/src/utils.js
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 beepy_web-0.9.3/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 beepy_web-0.9.3/LICENSE
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 beepy_web-0.9.3/README.md
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 beepy_web-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 beepy_web-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 beepy_web-0.9.4/.env.template
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 beepy_web-0.9.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 beepy_web-0.9.4/.python-version
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 beepy_web-0.9.4/requirements.txt
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/__init__.py
+-rw-r--r--   0        0        0    14690 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/attrs.py
+-rw-r--r--   0        0        0     7310 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/children.py
+-rw-r--r--   0        0        0    12781 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/components.py
+-rw-r--r--   0        0        0     8585 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/context.py
+-rw-r--r--   0        0        0    21111 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/framework.py
+-rw-r--r--   0        0        0     5423 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/listeners.py
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/router.py
+-rw-r--r--   0        0        0     8097 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/style.py
+-rw-r--r--   0        0        0     5285 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/tags.py
+-rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/trackable.py
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/types.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/dev/__init__.py
+-rwxr-xr-x   0        0        0     5055 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/dev/__main__.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/dev/example.html
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/dev/example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/modules/__init__.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/modules/actions.py
+-rw-r--r--   0        0        0     2730 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/modules/context_menu.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/modules/local_storage.py
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/modules/modal.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/modules/plot.py
+-rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/modules/table.py
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/modules/tabs.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/utils/__init__.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/utils/api.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/utils/asyncio.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/utils/common.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/utils/dev.py
+-rw-r--r--   0        0        0     1904 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/utils/import_hooks.py
+-rw-r--r--   0        0        0     2540 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/utils/internal.py
+-rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/utils/js.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 beepy_web-0.9.4/beepy/utils/js_py.py
+-rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 beepy_web-0.9.4/scripts/publish.sh
+-rw-r--r--   0        0        0   179387 2020-02-02 00:00:00.000000 beepy_web-0.9.4/web/package-lock.json
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 beepy_web-0.9.4/web/package.json
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 beepy_web-0.9.4/web/webpack.dev.js
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 beepy_web-0.9.4/web/webpack.prod.js
+-rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 beepy_web-0.9.4/web/src/beepy.js
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 beepy_web-0.9.4/web/src/dev-server.js
+-rw-r--r--   0        0        0     3027 2020-02-02 00:00:00.000000 beepy_web-0.9.4/web/src/files.js
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 beepy_web-0.9.4/web/src/index.js
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 beepy_web-0.9.4/web/src/main.css
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 beepy_web-0.9.4/web/src/python.js
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 beepy_web-0.9.4/web/src/utils.js
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 beepy_web-0.9.4/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 beepy_web-0.9.4/LICENSE
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 beepy_web-0.9.4/README.md
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 beepy_web-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 beepy_web-0.9.4/PKG-INFO
```

### Comparing `beepy_web-0.9.3/.pre-commit-config.yaml` & `beepy_web-0.9.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.3/beepy/__init__.py` & `beepy_web-0.9.4/beepy/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,35 +8,34 @@
     sys.modules['js'] = js
     del sys, js
 
 import beepy.children  # must be loaded before .framework due to circular import
 import beepy.utils.import_hooks  # allows to use `import` for local files  # noqa: F401
 from beepy.attrs import attr, html_attr, state
 from beepy.components import Directive
-from beepy.context import CONTENT, OVERWRITE, SUPER
+from beepy.context import SpecialChild
 from beepy.framework import Tag, __version__, empty_tag, mount
 from beepy.listeners import on
-from beepy.style import Style
+from beepy.style import Style, import_css
 from beepy.tags import Body, Head
 from beepy.types import safe_html, safe_html_content
 from beepy.utils import __CONFIG__
 
 __all__ = [
     'Head',
     'Body',
     'Style',
+    'import_css',
     '__CONFIG__',
     'attr',
     'state',
     'html_attr',
     'on',
     'safe_html',
     'safe_html_content',
     'Directive',
-    'OVERWRITE',
-    'SUPER',
-    'CONTENT',
+    'SpecialChild',
     'Tag',
     'empty_tag',
     'mount',
     '__version__',
 ]
```

### Comparing `beepy_web-0.9.3/beepy/attrs.py` & `beepy_web-0.9.4/beepy/attrs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import keyword
 from collections import defaultdict
 from typing import TYPE_CHECKING, Any, get_type_hints
 
 from boltons.iterutils import first
-from boltons.typeutils import issubclass, make_sentinel
+from boltons.typeutils import issubclass
 
 from beepy.types import AttrType, AttrValue
 from beepy.utils import log
 from beepy.utils.common import NONE_TYPE, call_handler_with_optional_arguments, to_kebab_case, wraps_with_name
 
 if TYPE_CHECKING:
     import builtins
@@ -28,32 +28,29 @@
 }
 
 
 def convert_boolean_attribute_value(value):
     return '' if value else None
 
 
-_MISSING = make_sentinel(var_name='_MISSING')
-
-
 def set_html_attribute(el, name: str, value, *, type: builtins.type = NONE_TYPE):
     if value is None:
         el.removeAttribute(name)
     elif name.endswith('_'):
         el.setAttribute(name[:-1], value)
     elif not hasattr(el, name) or issubclass(type, bool):
         el.setAttribute(name, value)
     else:
         setattr(el, name, value)
 
 
 class attr:
     __slots__ = (
         'name',
-        'initial_value',
+        '_initial_value',
         'type',
         'const',
         'required',
         'notify',
         'static',
         'move_on',
         'model',
@@ -67,15 +64,15 @@
         '_cache',
     )
 
     _view = True
     _set_on_render = False
 
     name: str | None
-    initial_value: T
+    _initial_value: T
     type: builtins.type | None
     const: bool
     required: bool
     notify: bool
     static: bool
     move_on: bool
     model: str | None
@@ -107,15 +104,15 @@
         **kwargs,
     ):
         _type = kwargs.get('type')
 
         self.name = None
         self.const = const
         assert not const or default is None, f'Const {type(self).__name__} cannot have initial value'
-        self.initial_value = default
+        self._initial_value = default
         self.required = required or const  # const attr must be also required
         self.notify = notify
         self.static = static
         self.move_on = move_on
         self.model = 'change' if model is True else model
         self.model_options = {'attribute': None} | (model_options or {})
         self._from_model_cache = []
@@ -137,33 +134,33 @@
 
         self.handlers = defaultdict(list)
         self.enum = enum
 
         self._cache = {}
 
     @property
-    def priority(self):
+    def _priority(self):
         if self.move_on:
             return 0
         elif self.model:
             return 2
         else:
             return 1
 
     @classmethod
-    def order_dict_by_priority(cls, dict_attrs):
-        return dict(sorted(dict_attrs.items(), key=lambda item: item[1].priority))
+    def _order_dict_by_priority(cls, dict_attrs):
+        return dict(sorted(dict_attrs.items(), key=lambda item: item[1]._priority))
 
     def __get__(self, instance, owner=None):
         if instance is None:
             return self
         return (self.fget or self._fget)(instance)
 
     def _fget(self, instance):
-        return self._cache.get(None if self.static else instance, self.initial_value)
+        return self._cache.get(None if self.static else instance, self._initial_value)
 
     def __call__(self, fget):
         self.fget = fget
         self.name = to_kebab_case(fget.__name__)
         if self.type is NONE_TYPE:
             type_hints = get_type_hints(fget)
             if 'return' in type_hints:
@@ -176,24 +173,24 @@
             raise AttributeError
 
         if current_value == value:
             return
 
         (self.fset or self._fset)(instance, value)
 
-        if instance.parent_defined:
+        if instance._parent_ is not None:
             for handler in self.handlers['change']:
                 if _prevent_model and _prevent_model in (True, self) and handler.__name__.startswith('@attr'):
                     continue
                 call_handler_with_optional_arguments(handler, instance, {'value': value})
 
         if self.notify:
             instance.__notify__(self.name, self, value)
 
-    def __set_first__(self, instance, value, parent):
+    def _set_first_value(self, instance, value, parent):
         if self.model and (
             isinstance(value, attr) and value.name is not None and (instance, self, None) not in value._from_model_cache
         ):
             value._from_model_cache.append((instance, self, value.name))
             instance._kwargs.pop(self.name)
 
     def _fset(self, instance, value):
@@ -253,19 +250,19 @@
     def _prepare_attribute_for_model(self, instance):
         if attribute := self.model_options['attribute']:
             if callable(attribute):
                 return attribute(instance)
             return attribute
 
     def _set_model_value(self, instance, attr_, component: Component):
-        initial_value = self.__get__(instance.parent if instance.parent_defined else component)
+        initial_value = self.__get__(instance.parent if instance._parent_ is not None else component)
 
         if initial_value is None:
-            if self.initial_value is not None:
-                initial_value = self.initial_value
+            if self._initial_value is not None:
+                initial_value = self._initial_value
             elif self.type and (value_from_type := self._get_type_instance()) is not None:
                 initial_value = value_from_type
         if attribute_ := self._prepare_attribute_for_model(instance):
             initial_value = getattr(initial_value, attribute_)
         if initial_value is None:
             initial_value = ''
 
@@ -277,15 +274,15 @@
         to_remove_indexes = []
 
         for index, (instance, attr_, name) in enumerate(self._from_model_cache):
             if name is None:
                 to_remove_indexes.append(index)
                 continue
 
-            if instance.parent_defined and instance.parent != component:
+            if instance._parent_ is not None and instance.parent != component:
                 continue
 
             attribute_ = self._set_model_value(instance, attr_, component)
 
             _attribute_str = f'({attribute_})' if attribute_ else ''
 
             @instance.on(attr_.model)
@@ -308,22 +305,22 @@
                     value = getattr(value, current_attribute)
 
                 _attr_.__set__(instance_, value, _prevent_model=current_attribute)
 
         for index in reversed(to_remove_indexes):
             self._from_model_cache.pop(index)
 
-    def __init_ctx__(self, ctx: Context, value):
+    def _init_ctx(self, ctx: Context, value):
         for handler in self.handlers['init']:
             call_handler_with_optional_arguments(handler, ctx, {'value': value})
 
-    def __mount_cmpt__(self, component: Component):
+    def _mount_cmpt(self, component: Component):
         self._handle_model_listeners(component)
 
-    def __post_mount_cmpt__(self, component: Component):
+    def _post_mount_cmpt(self, component: Component):
         for instance, attr_, _ in self._from_model_cache:
             self._set_model_value(instance, attr_, component)
 
         if self.handlers['mount']:
             value = self.__get__(component)
             for handler in self.handlers['mount']:
                 call_handler_with_optional_arguments(handler, component, {'value': value})
@@ -342,19 +339,19 @@
     def deleter(self, fdel):
         self.fdel = fdel
         return self
 
     def __repr__(self):
         return (
             f'{self.name} = {type(self).__name__}'
-            f'(default={self.initial_value!r}, type={self.type}, static={self.static})'
+            f'(default={self._initial_value!r}, type={self.type}, static={self.static})'
         )
 
     def __str__(self):
-        return f'{self.name}({self.initial_value!r})'
+        return f'{self.name}({self._initial_value!r})'
 
     def on(self, *triggers):
         def wrapper(handler):
             if self.static or self._from_model_cache:  # check if _from_model_cache is required
                 if not hasattr(handler, '_attrs_static_'):
                     handler._attrs_static_ = defaultdict(list)
                 for trigger in triggers:
@@ -434,15 +431,15 @@
     __slots__ = ('provider', 'subscribers')
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.provider = None
         self.subscribers = []
 
-    def __mount_cmpt__(self, component: Component):
+    def _mount_cmpt(self, component: Component):
         if self.provider is None:
             self.provider = component
         else:
             self.subscribers.append(component)
 
     def __set__(self, instance, value, *, _prevent_model=False):
         super().__set__(instance, value, _prevent_model=_prevent_model)
```

### Comparing `beepy_web-0.9.3/beepy/children.py` & `beepy_web-0.9.4/beepy/children.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         self.mount_parent = None
         self.children = None
 
     def __mount__(self, element, parent: Tag, index=None):
         self.parent = parent
         self.mount_parent = element
         if self.tag:
-            self.mount_element = self.tag.clone(parent).mount_element
+            self.mount_element = self.tag._clone(parent).mount_element
             self.mount_parent.insertChild(self.mount_element, index)
         else:
             self.mount_element = js.document.createDocumentFragment()
             self.mount_parent.insertChild(self.mount_element, index)
         setattr(self.mount_element, _PY_TAG_ATTRIBUTE, self)
 
     def _mount_children(self):
@@ -194,16 +194,16 @@
 
 class ComponentRef(ChildRef[Component]):
     __slots__ = ()
 
     child: Component
 
     def _update_child(self, parent: Tag, index):  # noqa: ARG002 - arguments for overriding
-        clone = self.__get__(parent).clone(parent)
-        clone.__set_ref__(parent, self)
+        clone = self.__get__(parent)._clone(parent)
+        clone._set_ref(parent, self)
         self.__set__(parent, clone)
         return clone
 
 
 class TagRef(ComponentRef, ChildRef[Tag]):
     __slots__ = ()
 
@@ -213,15 +213,15 @@
 class ChildrenRef(ChildRef):
     __slots__ = ()
 
     child: Children
 
     def _update_child(self, parent, index):
         copy = self.__get__(parent).copy()
-        copy.__set_parent__(parent, index, self)
+        copy._set_parent(parent, index, self)
         self.__set__(parent, copy)
         return copy
 
     def __set__(self, instance, value):
         if isinstance(value, Children):
             super().__set__(instance, value)
         else:
```

### Comparing `beepy_web-0.9.3/beepy/components.py` & `beepy_web-0.9.4/beepy/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         else:
             cls._static_listeners = defaultdict(list)
             cls._static_onchange_handlers = []
             cls._lifecycle_methods = _lifecycle_methods
 
         if hasattr(cls, '__extra_attributes__'):
             cls.__extra_attributes__ = {
-                key: value.as_child(None) if isinstance(value, Component) else value
+                key: value._as_child(None) if isinstance(value, Component) else value
                 for key, value in cls.__extra_attributes__.items()
             }
 
         return cls
 
 
 class Component(WebBase, Context, metaclass=_MetaComponent, _root=True):
@@ -157,15 +157,15 @@
     _lifecycle_methods: list[str]
 
     @LifecycleMethod
     def __mount__(self, *args, **kwargs):
         result = yield 'call'
         yield 'attrs'
 
-        for name, attribute in self.__states__.items():
+        for name, attribute in self._states.items():
             if callable(attribute) and not isinstance(attribute, MethodType):
                 setattr(self, name, MethodType(attribute, self.parent))
 
         self._post_mount_attrs()
 
         for event, listeners in self._listeners.items():
             for listener in listeners:
@@ -218,15 +218,15 @@
     def __render__(self, attrs: dict[str, AttrType] | None = None, *args, **kwargs):
         # TODO: maybe function 'render' could return some content, appended to args?
         yield 'pre_call'
 
         if attrs is None:
             attrs = {}
 
-        for name, value in {**self.__attrs__, **attrs}.items():
+        for name, value in {**self._attrs_values, **attrs}.items():
             # TODO: optimize this - set only changed attributes
 
             type = _attr.type if (_attr := self.attrs.get(name)) else NONE_TYPE
             set_html_attribute(self.mount_element, name, value, type=type)
 
         yield 'post_call'
         yield 'call'
@@ -238,43 +238,39 @@
                 self.render()
             case 'post_call':
                 self.post_render()
             case 'call':
                 return self._render_(*args, **kwargs)
 
     @property
-    def parent_defined(self):
-        return self._parent_ is not None
-
-    @property
     def parent(self):
         if self._parent_ is None:
             _debugger("ValueError: Trying to get .parent, but it's undefined")
         return self._parent_
 
     @parent.setter
     def parent(self, v):
         self._parent_ = v
 
-    def as_child(self, parent: Tag | None, *, exists_ok=False):
+    def _as_child(self, parent: Tag | None, *, exists_ok=False):
         if self._ref:
             if exists_ok:
-                self.__set_ref__(parent, self._ref)
+                self._set_ref(parent, self._ref)
                 return self._ref
             else:
                 raise TypeError(f'Component {self._context_name_} already is child')
         ref = beepy.children.ComponentRef(self)
-        self.__set_ref__(parent, ref)
+        self._set_ref(parent, ref)
         return ref
 
-    def __set_ref__(self, parent: Tag | None, ref: ComponentRef):
+    def _set_ref(self, parent: Tag | None, ref: ComponentRef):
         self._ref = ref
 
-    def clone(self, parent=None) -> Self:
-        clone = super().clone(parent=parent)
+    def _clone(self, parent=None) -> Self:
+        clone = super()._clone(parent=parent)
         clone._listeners = defaultdict(list, **nested_copy(self._listeners))
         clone._handlers = defaultdict(list, **nested_copy(self._handlers))
         return clone
 
     def __new__(cls, *args, **kwargs: AttrType):
         self: Component = super().__new__(cls, *args, **kwargs)
         self._parent_ = None
@@ -288,25 +284,23 @@
 
         return self
 
     def _mount_(self, element, parent: Tag, index=None):  # noqa: ARG002 - unused `element`, `index`
         self.parent = parent
         self.pre_mount()
 
-        args, kwargs = self.args_kwargs
-        kwargs = self._attrs_defaults | kwargs
-        self.init(*args, **kwargs)
+        self.init(*self._args, **(self._attrs_defaults | self._kwargs))
 
     def _mount_attrs(self):
         for attribute in self.attrs.values():
-            attribute.__mount_cmpt__(self)
+            attribute._mount_cmpt(self)
 
     def _post_mount_attrs(self):
         for attribute in self.attrs.values():
-            attribute.__post_mount_cmpt__(self)
+            attribute._post_mount_cmpt(self)
 
     def pre_mount(self):
         """empty method for easy override with code for run before mount"""
 
     def mount(self):
         """empty method for easy override with code for run after mount"""
 
@@ -342,15 +336,15 @@
             if action:
                 return partial(wrapper, action_name=action)
 
             return wrapper
 
         def wrapper(callback: Callable):
             event_listener = on(method)(callback, child=self)
-            event_name = event_listener.name or callback.__name__
+            event_name = event_listener._name or callback.__name__
             event_listener.__set_name__(self, event_name)
             self._listeners[event_name] = [*self._listeners[event_name].copy(), event_listener]
             return callback
 
         if not isinstance(method, str):
             return wrapper(method)
```

### Comparing `beepy_web-0.9.3/beepy/context.py` & `beepy_web-0.9.4/beepy/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import enum
 from abc import ABCMeta
 from typing import TYPE_CHECKING, TypeVar
 
 from boltons.typeutils import make_sentinel
 
 import beepy
 from beepy.attrs import attr
@@ -11,24 +12,22 @@
 from beepy.utils.common import get_random_name, log10_ceil, to_kebab_case
 from beepy.utils.js_py import Interval, create_once_callable
 
 if TYPE_CHECKING:
     from beepy.types import AttrType
 
 _base_obj_dir = (*dir(object()), '__abstractmethods__')
-
-
 Self = TypeVar('Self', bound='Context')
-
 _CONTEXT_INITIALIZED = False
 
-OVERWRITE = make_sentinel('_OVERWRITE', var_name='OVERWRITE')
-SUPER = make_sentinel('_SUPER', var_name='SUPER')
-CONTENT = make_sentinel('_CONTENT', var_name='CONTENT')
-_SPECIAL_CHILD_STRINGS = (OVERWRITE, SUPER, CONTENT)
+
+class SpecialChild(enum.StrEnum):
+    OVERWRITE = 'OVERWRITE'
+    SUPER = 'SUPER'
+    CONTENT = 'CONTENT'
 
 
 class _MetaContext(ABCMeta):
     _to_load_before_top_render: list = []
     _wait_onload_interval: dict[Context, Interval] = {}
     _context_classes = []
     __clean_class_attribute_names = ()
@@ -66,23 +65,23 @@
                     (isinstance(child, attr) and not isinstance(new_attr, attr))
                     or (isinstance(child, _children.ChildrenRef) and not isinstance(new_attr, _children.ChildrenRef))
                 ):
                     attrs_defaults[attribute_name] = namespace.pop(attribute_name)
 
         is_root = kwargs.get('_root')
         ctx_name = '' if is_root else kwargs.get('name')
-        namespace['__ROOT__'] = is_root
+        namespace['_meta_root'] = is_root
 
         if ctx_name or (initialized and not hasattr(base_cls, '_context_name_')):
             namespace['_context_name_'] = ctx_name or to_kebab_case(_name)
 
         cls: type[Context] | type = super().__new__(mcs, _name, bases, namespace)
 
         if initialized:
-            cls._static_attrs = attr.order_dict_by_priority(cls._static_attrs.copy() | static_attrs)
+            cls._static_attrs = attr._order_dict_by_priority(cls._static_attrs.copy() | static_attrs)
             cls._attrs_defaults = cls._attrs_defaults.copy() | attrs_defaults
         else:
             cls._static_attrs = {}
             cls._attrs_defaults = {}
 
         cls._contexts = []
 
@@ -150,15 +149,15 @@
                 mcs._wait_onload_interval.pop(element._root_parent)
             mcs._top_render(element)
 
 
 class Context(metaclass=_MetaContext, _root=True):
     __slots__ = ('_id_', '_args', '_kwargs', 'attrs')
 
-    __ROOT__ = False
+    _meta_root = False
 
     _id_: str
     _args: tuple[AttrType, ...]
     _kwargs: dict[str, AttrType]
 
     _static_attrs: dict[str, attr]
     _attrs_defaults: dict[str, AttrType]
@@ -181,20 +180,19 @@
             attribute._link_cmpt(name, self, force=False)
 
         return self
 
     def _clone_link_parent(self, parent):
         for name, attribute in self.attrs.items():
             if name in self._kwargs:
-                attribute.__set_first__(self, self._kwargs[name], parent)
-        self.link_parent_attrs(parent)
+                attribute._set_first_value(self, self._kwargs[name], parent)
+        self._link_parent_attrs(parent)
 
-    def link_parent_attrs(self, parent):
-        p_args, p_kwargs = parent.args_kwargs
-        p_data = parent._attrs_defaults | p_kwargs
+    def _link_parent_attrs(self, parent):
+        p_data = parent._attrs_defaults | parent._kwargs
 
         for name, attr_to_move_on in parent.attrs.items():
             if attr_to_move_on.move_on:
                 attr_to_move_on._link_cmpt(name, self, force_cls_set=True)
                 if name in p_data:
                     self._attrs_defaults[name] = p_data[name]
 
@@ -208,55 +206,50 @@
             if key not in kwargs:
                 if attr_.required:
                     raise TypeError(f'Attribute {attr_.name!r} is required')
                 continue
 
             value = kwargs[key]
             setattr(self, key, value)
-            attr_.__init_ctx__(self, value)
+            attr_._init_ctx(self, value)
 
         self.post_init()
 
     def post_init(self):
         pass
 
     @property
-    def __view_attrs__(self) -> dict[str, AttrType]:
-        return {_attr.name: _attr._get_view_value(self) for _attr in self.attrs.values() if _attr._view}
-
-    @property
-    def __attrs__(self) -> dict[str, AttrType]:
+    def _attrs_values(self) -> dict[str, AttrType]:
         return {
             _attr.name: _attr._get_view_value(self)
             for _attr in self.attrs.values()
             if _attr._view and not _attr._set_on_render
         }
 
     @property
-    def __states__(self) -> dict[str, AttrType]:
+    def _states(self) -> dict[str, AttrType]:
         return {_attr.name: _attr.__get__(self) for _attr in self.attrs.values()}
 
     @property
-    def args_kwargs(self):
+    def _args_kwargs(self):
         if not hasattr(self, '_args'):
             return None
         # TODO: make self._kwargs as frozendict
         return self._args, self._kwargs
 
     def __hash__(self):
         # TODO: make force immutable this attributes
         return hash((self._context_name_, self._id_))
 
     def __notify__(self, attr_name: str, attribute: attr, value: AttrType):
         pass
 
-    def clone(self, parent=None) -> Self:
-        args, kwargs = self.args_kwargs
-        clone = type(self)(*args, **kwargs)
+    def _clone(self, parent=None) -> Self:
+        clone = type(self)(*self._args, **self._kwargs)
         clone._clone_link_parent(parent)
         return clone
 
 
 _CONTEXT_INITIALIZED = True
 
 
-__all__ = ['OVERWRITE', 'SUPER', 'CONTENT', '_SPECIAL_CHILD_STRINGS', '_MetaContext', 'Context']
+__all__ = ['SpecialChild', '_MetaContext', 'Context']
```

### Comparing `beepy_web-0.9.3/beepy/framework.py` & `beepy_web-0.9.4/beepy/framework.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from __future__ import annotations
 
 import traceback
 from collections.abc import Callable, Iterable
 from functools import cache
 from types import MethodType
+from typing import ClassVar
 
 from beepy.attrs import attr, state
 from beepy.children import ChildRef, Children, ContentWrapper, CustomWrapper, StringWrapper, TagRef
 from beepy.components import Component, _MetaComponent
-from beepy.context import _SPECIAL_CHILD_STRINGS, CONTENT, OVERWRITE, SUPER
+from beepy.context import SpecialChild
 from beepy.types import AttrType, ContentType, Mounter, Renderer
 from beepy.utils import __CONFIG__, js, log
 from beepy.utils.common import NONE_TYPE, get_random_name, to_kebab_case
 from beepy.utils.dev import _debugger
 from beepy.utils.internal import _PY_TAG_ATTRIBUTE
 
-__version__ = '0.9.3'  # For internal development set to 0.0a0
+__version__ = '0.9.4'  # For internal development set to 0.0a0
 __CONFIG__['version'] = __version__
 
 
 _TAG_INITIALIZED = False
 
 
 class _MetaTag(_MetaComponent):
@@ -36,15 +37,15 @@
         # for example: extending classes Tag and WithRouter must produce correct state 'router'
         mock_cls: type[Tag] | type = type.__new__(mcs, _name, bases, {})
 
         initialized = _TAG_INITIALIZED  # As base classes is also declared here, we must be sure base class exists
 
         is_root = kwargs.get('_root')
         tag_name = '' if is_root else kwargs.get('name')
-        namespace['__ROOT__'] = is_root
+        namespace['_meta_root'] = is_root
 
         if tag_name or (initialized and not hasattr(mock_cls, '_tag_name_')):
             namespace['_tag_name_'] = to_kebab_case(tag_name or _name)
 
         if 'raw_html' in kwargs:
             namespace['_raw_html'] = kwargs['raw_html']
 
@@ -76,16 +77,16 @@
         children_arg = namespace.get('children', [])
         if isinstance(children_arg, property):
             children_arg = []
 
         if children_arg:
             namespace.pop('children')
             children_arg = list(children_arg)
-            if OVERWRITE not in children_arg and SUPER not in children_arg:
-                children_arg.insert(0, SUPER)
+            if SpecialChild.OVERWRITE not in children_arg and SpecialChild.SUPER not in children_arg:
+                children_arg.insert(0, SpecialChild.SUPER)
         elif children_arg not in (None, False, []):
             namespace['_static_children'] = namespace.pop('children')
             children_arg = []
 
         if initialized:
             mcs._update_namespace_with_extra_attributes(namespace)
 
@@ -96,34 +97,34 @@
                 if isinstance(child, Component | Children | ChildRef):
                     if child in children_arg:
                         ref_children.append(child)
                         # TODO: make possible inherit without replacement?
                         if (old_child := getattr(mock_cls, attribute_name, None)) and isinstance(old_child, ChildRef):
                             to_remove_children.append(old_child)
                         if isinstance(child, Component | Children):
-                            children_arg[children_arg.index(child)] = namespace[attribute_name] = child.as_child(None)
+                            children_arg[children_arg.index(child)] = namespace[attribute_name] = child._as_child(None)
 
                     if isinstance(child, Component) and child._force_ref:
                         # TODO: add support '_force_ref' for Children too
-                        namespace[attribute_name] = _ref = child.as_child(None)
+                        namespace[attribute_name] = _ref = child._as_child(None)
                         _ref.__set_name__(None, attribute_name)
                         children_arg.insert(0, _ref)
                         ref_children.append(_ref)
 
                     if isinstance(child, ChildRef) and child.child._force_ref:
                         children_arg.insert(0, child)
                         ref_children.append(child)
 
             for _index, child in enumerate(children_arg):
-                if isinstance(child, str) and child not in _SPECIAL_CHILD_STRINGS:
+                if isinstance(child, str):
                     children_arg[_index] = StringWrapper(child)
 
                 if isinstance(child, Component) and child not in ref_children:
                     # TODO: replace 5 in get_random_name(5) with some log
-                    children_arg[_index] = namespace[f'_{get_random_name(5)}_'] = child.as_child(None)
+                    children_arg[_index] = namespace[f'_{get_random_name(5)}_'] = child._as_child(None)
 
         cls: type[Tag] | type = super().__new__(mcs, _name, bases, namespace, **kwargs)
 
         if not hasattr(cls, '_raw_html'):
             cls._raw_html = False
 
         if initialized:
@@ -137,34 +138,34 @@
             cls._static_children_tag = None
 
         for child in to_remove_children:
             cls._static_children.remove(child)
 
         if getattr(cls, '_tag_name_', None) or not isinstance(getattr(cls, 'children', None), property):
             if children_arg:
-                if CONTENT in children_arg and CONTENT in cls._static_children:
-                    cls._static_children.remove(CONTENT)
-                if SUPER in children_arg:
-                    super_children_index = children_arg.index(SUPER)
+                if SpecialChild.CONTENT in children_arg and SpecialChild.CONTENT in cls._static_children:
+                    cls._static_children.remove(SpecialChild.CONTENT)
+                if SpecialChild.SUPER in children_arg:
+                    super_children_index = children_arg.index(SpecialChild.SUPER)
                     children_arg[super_children_index : super_children_index + 1] = cls._static_children
                 else:
                     children_arg.extend(cls._static_children)
                 cls._static_children = children_arg
         else:
-            cls._static_children = [CONTENT]
+            cls._static_children = [SpecialChild.CONTENT]
 
         cls._tags = []
 
         mcs._tag_classes.append(cls)
 
         if initialized and 'mount' in kwargs:
             cls._root_parent = None
             setattr(cls.mount_element, _PY_TAG_ATTRIBUTE, cls())
 
-        if cls.__ROOT__:
+        if cls._meta_root:
             cls.__root_declared__()
         else:
             cls.__class_declared__()
 
         return cls
 
 
@@ -198,14 +199,16 @@
     _static_children: list[ContentType]
     _children: list[Mounter]
     _children_element: js.HTMLElement
     _static_children_tag: Tag
     _children_tag: Tag
     _mount_finished_: bool
 
+    children: ClassVar[Component | state | SpecialChild | str]
+
     @classmethod
     def __root_declared__(cls):
         """This method is called, when root Tag is defined"""
 
     @classmethod
     def __class_declared__(cls):
         """This method is called, when common Tag is defined"""
@@ -225,15 +228,15 @@
                 child.__mount__(self._children_element, self)
             else:
                 log.warn(f'Cannot mount: {child}')
 
         if self._children_tag:
             self.mount_element.insertChild(self._children_element)
 
-        if (content_child := self.get_content_child()) is None:
+        if (content_child := self._get_content_child()) is None:
             _debugger(self)  # wtf?
         else:
             content_child._mount_children()
 
         super().__mount__.call_as_super(self, args, kwargs)
 
         self._mount_finished_ = True
@@ -313,24 +316,24 @@
 
             if is_child_arg_string and children_argument:
                 self._content = children_argument
             elif is_child_arg_function and children_argument and len(children_argument) == 1:
                 self._content = MethodType(children_argument[0], self)
             elif is_child_arg_tag:
                 self._children = self._children.copy() + [
-                    child.clone(self).as_child(self) for child in children_argument
+                    child._clone(self)._as_child(self) for child in children_argument
                 ]
             else:
                 self._children = [*self._children.copy(), *children_argument]
 
         for key, value in kwargs.items():
             if not isinstance(value, Component | Children) or key in self.attrs:
                 continue
             value: Component | Children
-            child = value.as_child(self, exists_ok=True)
+            child = value._as_child(self, exists_ok=True)
             child.__set_name__(self, key)
             setattr(type(self), key, child)
             self._children.append(child)
 
         self._shadow_root = None
         self.mount_parent = None
         self._mount_finished_ = False
@@ -338,15 +341,15 @@
         if not hasattr(self, 'mount_element'):
             self.mount_element = js.document.createElement(self._tag_name_)
         if getattr(self.mount_element, _PY_TAG_ATTRIBUTE, None):
             raise ValueError(f'Coping or using as child is not allowed for "{self._tag_name_}"')
         else:
             setattr(self.mount_element, _PY_TAG_ATTRIBUTE, self)
         if self._static_children_tag:
-            self._children_tag = self._static_children_tag.clone(self)
+            self._children_tag = self._static_children_tag._clone(self)
             self._children_element = self._children_tag.mount_element
             setattr(self._children_element, _PY_TAG_ATTRIBUTE, self)
         else:
             self._children_tag = None
             self._children_element = self.mount_element
 
         return self
@@ -357,38 +360,38 @@
     def __hash__(self):
         # TODO: make force immutable this attributes
         return hash((self._tag_name_, self._id_))
 
     def __getitem__(self, key):
         return getattr(self, key)
 
-    def as_child(self, parent: Tag | None, *, exists_ok=False, inline_def=False):
+    def _as_child(self, parent: Tag | None, *, exists_ok=False, inline_def=False):
         if self._ref:
             if exists_ok:
-                self.__set_ref__(parent, self._ref)
+                self._set_ref(parent, self._ref)
                 return self._ref
             else:
                 raise TypeError(f'Tag {self._tag_name_} already is child')
         ref = TagRef(self, inline_def=inline_def)
-        self.__set_ref__(parent, ref)
+        self._set_ref(parent, ref)
         return ref
 
     def __notify__(self, attr_name: str, attribute: attr, value: AttrType):
         super().__notify__(attr_name, attribute, value)
         self.__render__()
 
-    def __set_ref__(self, parent: Tag | None, ref: TagRef):
-        super().__set_ref__(parent, ref)
+    def _set_ref(self, parent: Tag | None, ref: TagRef):
+        super()._set_ref(parent, ref)
         if ref.inline_def:
             setattr(type(parent), ref.name, self)
 
     def _render_(self, attrs: dict[str, AttrType] | None = None):  # noqa: ARG002 - unused `attrs`
         self._current_render.append(self)
 
-        content_index = self.get_content_index()
+        content_index = self._get_content_index()
         if content_index is not None:
             self.children[content_index].__render__()
 
         for index, child in enumerate(self.children):
             # TODO: optimize this - re-render the only children, that need this
             if isinstance(child, ChildRef):
                 child.__render__(self)
@@ -441,20 +444,20 @@
     def own_children(self) -> list[Mounter]:
         return [child for child in self.children if not isinstance(child, ChildRef | CustomWrapper)]
 
     @property
     def ref_children(self) -> dict[str, Mounter]:
         return {child.name: child.__get__(self) for child in self.children if isinstance(child, ChildRef)}
 
-    def get_content_child(self) -> ContentWrapper:
+    def _get_content_child(self) -> ContentWrapper:
         for child in self.children:
             if isinstance(child, ContentWrapper) and child.content.__func__.__name__ == 'content':
                 return child
 
-    def get_content_index(self):
+    def _get_content_index(self):
         for index, child in enumerate(self.children):
             if isinstance(child, ContentWrapper) and child.content.__func__.__name__ == 'content':
                 return index
 
     @property
     def children(self) -> list[Mounter | Renderer | ChildRef | ContentWrapper]:
         return self._children
@@ -465,42 +468,42 @@
 
         for new_child in children:
             child = new_child
 
             if isinstance(child, ContentWrapper):
                 child = child.content.__func__
                 if child.__name__ == 'content':
-                    child = CONTENT
+                    child = SpecialChild.CONTENT
 
-            if child == CONTENT:
+            if child == SpecialChild.CONTENT:
                 child = self.content
 
             if isinstance(child, attr):
 
                 def child(s, _n=child.name):
                     return getattr(s, _n)
 
             if isinstance(child, Component) and child in self._children and child._ref is not None:
                 # using Component as descriptor/just child; this allows save reference from parent to new copy of child
                 child = child._ref._update_child(self, self._children.index(child))
             elif isinstance(child, ChildRef) and child in self._children:
                 child._update_child(self, self._children.index(child))
-            # TODO: make ContentWrapper descriptor, here call .clone()
+            # TODO: make ContentWrapper descriptor, here call ._clone()
             #  make possible to use ContentWrapper separately from function 'content'
             elif callable(child):
                 if not isinstance(child, MethodType):
                     child = MethodType(child, self)
                 child = ContentWrapper(child, self._content_tag, self._current_render)
 
             result.append(child)
 
         self._children = result
 
-    def clone(self, parent=None):
-        clone = super().clone(parent=parent)
+    def _clone(self, parent=None):
+        clone = super()._clone(parent=parent)
         clone._children = self.children
         return clone
 
     @property
     def _current_render(self):
         try:
             return _MetaTag._current_render[self._root_parent]
@@ -529,17 +532,17 @@
     js.beepy.stopLoading()
     if clear or js.beepy.dev_server.started:
         root.innerHTML = ''
     js.beepy.startLoading(mountPoint=root)
 
     name = root.tagName.lower()
     parent = _MetaTag(name, (Tag,), {'_root_parent': state(type=Tag, move_on=True)}, name=name, content_tag=None)()
-    parent._attrs_defaults['_root_parent'] = parent.__class__._root_parent.initial_value = parent
+    parent._attrs_defaults['_root_parent'] = parent.__class__._root_parent._initial_value = parent
     parent.mount_element = root
-    element.link_parent_attrs(parent)
+    element._link_parent_attrs(parent)
 
     _MetaTag._top_mount(element)
 
     if not js.document.title:
         js.document.title = 'BeePy'
         log.warn(f'Document title is not set, use default title: {js.document.title}')
```

### Comparing `beepy_web-0.9.3/beepy/listeners.py` & `beepy_web-0.9.4/beepy/listeners.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     'keyup': js.document,
     'keypress': js.document,
     'keydown': js.document,
     'popstate': js.window,
     'hashchange': js.window,
 }
 _key_codes = {
+    # TODO: add all symbols and support raw keyCodes
     'esc': (27,),
     'tab': (9,),
     'enter': (13,),
     'space': (32,),
     'up': (38,),
     'left': (37,),
     'right': (39,),
@@ -39,147 +40,148 @@
 # TODO: click.(right|middle) ; click.left ; etc.
 
 
 def key_code_check(key_name, event):
     return event.keyCode in _key_codes[key_name]
 
 
-RAW_JS_CHECKS = ('prevent', 'stop', 'stop_all')
+_raw_js_checks = ('prevent', 'stop', 'stop_all')
 
 
 class on:
-    __slots__ = ('name', 'callback', 'pass_event', 'child_restrict', 'modifiers', 'checks', 'js_checks')
+    __slots__ = ('_name', '_callback', '_pass_event', '_child_restrict', '_modifiers', '_checks', '_js_checks')
 
-    name: str | None
-    callback: Callable[[Component, ...], Any]
-    pass_event: bool
-    child_restrict: type[Component] | None
-    modifiers: list[str]
-    checks: list[Callable[[js.Event], bool]]
-    js_checks: list[str]
+    _name: str | None
+    _callback: Callable[[Component, ...], Any]
+    _pass_event: bool
+    _child_restrict: type[Component] | None
+    _modifiers: list[str]
+    _checks: list[Callable[[js.Event], bool]]
+    _js_checks: list[str]
 
     def __init__(self, method):  # TODO: add 'mount' callbacks?
-        self.child_restrict = None
-        self.pass_event = True
-        self.modifiers = []
-        self.checks = []
-        self.js_checks = []
-
-        if isinstance(method, str):
-            if '.' in method:
-                method, *self.modifiers = method.split('.')
-                for modifier in self.modifiers:
-                    if modifier in _key_codes:
-                        # TODO: check for visibility?
-                        self.checks.append(partial(key_code_check, modifier))
-                    elif modifier in RAW_JS_CHECKS:
-                        self.js_checks.append(modifier)
-                    else:
-                        raise ValueError(f'Unknown event modifier ".{modifier}"!')
+        self._child_restrict = None
+        self._pass_event = True
+        self._modifiers = []
+        self._checks = []
+        self._js_checks = []
+
+        if not isinstance(method, str):
+            self._name = None
+            self(method)
+            return
 
-            self.name = method
+        if '.' not in method:
+            self._name = method
             return
 
-        self.name = None
-        self(method)
+        self._name, *self._modifiers = method.split('.')
+        for modifier in self._modifiers:
+            if modifier in _key_codes:
+                # TODO: check for visibility?
+                self._checks.append(partial(key_code_check, modifier))
+            elif modifier in _raw_js_checks:
+                self._js_checks.append(modifier)
+            else:
+                raise ValueError(f'Unknown event modifier ".{modifier}"!')
 
     def __call__(self, method, child=None):
-        self.callback = method
-        self.child_restrict = child
+        self._callback = method
+        self._child_restrict = child
 
         sig = inspect.signature(method)
-        self.pass_event = 'event' in sig.parameters
+        self._pass_event = 'event' in sig.parameters
         return self
 
     def _get_cb_and_instance(self, cmpt):
         if (
-            self.child_restrict
-            and cmpt.parent_defined
-            and (self.child_restrict == cmpt or (cmpt._ref and self.child_restrict == cmpt._ref.child))
+            self._child_restrict
+            and cmpt._parent_ is not None
+            and (self._child_restrict == cmpt or (cmpt._ref and self._child_restrict == cmpt._ref.child))
         ):
             cmpt = cmpt.parent
 
-        if isinstance(self.callback, MethodType):
-            return self.callback, cmpt
+        if isinstance(self._callback, MethodType):
+            return self._callback, cmpt
         else:
-            return MethodType(self.callback, cmpt), cmpt
+            return MethodType(self._callback, cmpt), cmpt
 
     def __get__(self, instance, owner=None):
         if instance is None:
             return self
         return self._get_cb_and_instance(instance)[0]
 
     def _prepare_call(self, cmpt, event):
-        for check in self.checks:
+        for check in self._checks:
             if not check(event):
                 return
 
         return self._get_cb_and_instance(cmpt)
 
     async def _a_call(self, cmpt, event):
         if (prepare := self._prepare_call(cmpt, event)) is None:
             return
 
         fn, cmpt = prepare
 
-        args = (event,) if self.pass_event else ()
+        args = (event,) if self._pass_event else ()
         data = await fn(*args)
         self._after_call(cmpt, event)
         return data
 
     def _call(self, cmpt, event):
         if (prepare := self._prepare_call(cmpt, event)) is None:
             return
 
         fn, cmpt = prepare
-        args = (event,) if self.pass_event else ()
+        args = (event,) if self._pass_event else ()
         data = fn(*args)
         self._after_call(cmpt, event)
         return data
 
     def _after_call(self, cmpt, event):
         for dependent in cmpt._dependents:
             # TODO: move to other place
             dependent.__render__()
 
         getattr(event.currentTarget, _PY_TAG_ATTRIBUTE, cmpt).__render__()
 
     def _make_listener(self, event_name: str, cmpt: Component):
-        if inspect.iscoroutinefunction(self.callback):
+        if inspect.iscoroutinefunction(self._callback):
 
-            @wraps(self.callback)
+            @wraps(self._callback)
             async def method(event):
                 return await self._a_call(cmpt, event)
 
         else:
 
-            @wraps(self.callback)
+            @wraps(self._callback)
             def method(event):
                 return self._call(cmpt, event)
 
         return js.beepy.addAsyncListener(
-            global_events.get(event_name, cmpt.mount_element), event_name, create_proxy(method), to_js(self.js_checks)
+            global_events.get(event_name, cmpt.mount_element), event_name, create_proxy(method), to_js(self._js_checks)
         )
 
     @classmethod
     def _remove_listener(cls, event_name: str, cmpt: Component, event_listener: Callable):
         global_events.get(event_name, cmpt.mount_element).removeEventListener(event_name, event_listener)
 
     def __set__(self, instance, value):
-        raise AttributeError(f'Cannot set on_{self.name} event handler')
+        raise AttributeError(f'Cannot set on_{self._name} event handler')
 
     def __delete__(self, instance):
         pass
 
     def __set_name__(self, owner, name):
-        if self.name is None:
-            self.name = name
+        if self._name is None:
+            self._name = name
 
-        if self.child_restrict is None:
+        if self._child_restrict is None:
             owner._static_listeners = defaultdict(list, **nested_copy(owner._static_listeners))
-            owner._static_listeners[self.name].append(self)
+            owner._static_listeners[self._name].append(self)
 
     def __repr__(self):
-        return f'on_{self.name}({self.callback})'
+        return f'on_{self._name}({self._callback})'
 
 
-__all__ = ['on', '_key_codes', 'RAW_JS_CHECKS']
+__all__ = ['on']
```

### Comparing `beepy_web-0.9.3/beepy/router.py` & `beepy_web-0.9.4/beepy/router.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         self.components.append(self.import_tag_component(tag_cls, match=match))
 
     def _load_children(self):
         self._current_render.clear()
 
         old_components = list(self.components)
 
-        with self.components._disable_onchange:  # can Locker also be descriptor with auto-replace as in last two lines?
+        with self.components.onchange_locker:  # can Locker also be descriptor with auto-replace as in last two lines?
             self.components.clear()
 
             for path, tag_cls in self.routes.items():
                 if match := re.search(self.basename + path, js.location.pathname):
                     self.add_tag_component(tag_cls, match=match, path=path)
                     if self.single_tag:
                         break
@@ -145,14 +145,12 @@
                 if fallback := self.fallback_tag_cls:
                     self.add_tag_component(fallback, match=None, path=None)
                 else:
                     # TODO: maybe create BeePyError?
                     raise ValueError('No route to use!')
 
             for child in self.components:
-                child.link_parent_attrs(self)
-                args, kwargs = child.args_kwargs
-                kwargs = child._attrs_defaults | kwargs
-                child.init(*args, _load_children=False, **kwargs)
+                child._link_parent_attrs(self)
+                child.init(*child._args, _load_children=False, **(child._attrs_defaults | child._kwargs))
 
             new_components, self.components = list(self.components), old_components
         self.components[:] = new_components  # triggers correct onchange handlers
```

### Comparing `beepy_web-0.9.3/beepy/style.py` & `beepy_web-0.9.4/beepy/style.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import re
 from collections.abc import Iterable
-from typing import Any
+from typing import Any, Protocol
 
+from beepy.context import Context
 from beepy.framework import __CONFIG__, Tag, attr, state
 from beepy.tags import Head
 from beepy.types import AttrValue, safe_html, safe_html_content
 from beepy.utils import js
 from beepy.utils.common import MISSING, get_random_name, log10_ceil, safe_issubclass, to_kebab_case
 
 
@@ -132,32 +133,36 @@
 
 
 class Raw:
     def __bool__(self):
         return False
 
 
+class TagWithStyle(Protocol):
+    style_id: StyleRef
+
+
 class Style(Tag, name='style', content_tag=None, raw_html=True, force_ref=True):
     __slots__ = ('styles', '_main_style', 'real_parent')
 
     __extra_attributes__ = {
         'style_id': attr(type=StyleRef),
     }
 
     _global = {
         'styles_count': 1,
     }
 
     options = state(type=dict)
-    real_parent: Tag | None
+    real_parent: Tag | TagWithStyle | None  # Actually it's only `Tag`;   `TagWithStyle` is used only for type checking
 
     @classmethod
     def from_css(cls, _file):
-        # TODO: implement import from css/scss/pycss
-        raise NotImplementedError
+        # TODO: implement converting from css/scss/pycss to Style
+        raise NotImplementedError('TBD...')
 
     def __init__(self, styles=None, options=None, get_vars=None, **styles_dict):
         super().__init__()
         if styles and not styles_dict:
             styles_dict = styles
         if options is None:
             options = {}
@@ -206,15 +211,15 @@
         if self.options['global'] or not self._content:
             return self._content
 
         parent = self.real_parent
         params: dict[str, Any] = {'__VARS__': ''}
 
         if self.options['render_states']:
-            params.update(parent.__states__)
+            params.update(parent._states)
 
         if self.options['render_children']:
             params.update(parent.ref_children)
 
         if get_vars := self.options['get_vars_callback']:
             params.update(get_vars(self=parent, ref=get_reference, **params))
 
@@ -236,24 +241,24 @@
             if new_value is None:
                 del parent.style_id.vars[name]
             else:
                 parent.style_id.vars[name] = new_value
             if parent._mount_finished_:
                 parent.__render__()
 
-    @classmethod
-    def import_file(cls, file_path):
-        return js.beepy.addElement(
-            js.document.head,
-            'link',
-            href=js.beepy.files.getPathWithCurrentPathAndOrigin(file_path),
-            onload=cls.create_onload(),
-            type='text/css',
-            rel='stylesheet',
-        )
+
+def import_css(file_path):
+    return js.beepy.addElement(
+        js.document.head,
+        'link',
+        href=js.beepy.files.getPathWithCurrentPathAndOrigin(file_path),
+        onload=Context.create_onload(),
+        type='text/css',
+        rel='stylesheet',
+    )
 
 
 def with_style(style_or_tag_cls: Style | type[Tag] | None = None):
     """
     @with_style
     class Button(Tag, name='button'):
         ...
@@ -267,8 +272,8 @@
     if safe_issubclass(style_or_tag_cls, Tag):
         _tag_cls, style_or_tag_cls = style_or_tag_cls, None
         return wrapper(_tag_cls)
 
     return wrapper
 
 
-__all__ = ['dict_to_css_iter', 'dict_to_css', 'Style', 'with_style']
+__all__ = ['Style', 'import_css', 'with_style', 'dict_to_css_iter', 'dict_to_css']
```

### Comparing `beepy_web-0.9.3/beepy/tags.py` & `beepy_web-0.9.4/beepy/tags.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 
 class html_tag(Tag, _root=True, content_tag=None):
     contenteditable = html_attr(type=bool)
     id = html_attr(type=str)
     class_ = html_attr(type=str)
 
-    def __set_ref__(self, parent, ref):
-        super().__set_ref__(parent, ref)
+    def _set_ref(self, parent, ref):
+        super()._set_ref(parent, ref)
         if type(self).id is html_tag.id and (self.id is AUTO_ID or (__CONFIG__['inputs_auto_id'] and self.id is None)):
             # TODO: replace 5 and 2 with some log value
             self.id = f'{ref.name or get_random_name(5)}-{get_random_name(2)}'
 
 
 def by__input_id(input_tag):
     return input_tag.id.rsplit('-', 1)[0]
@@ -96,16 +96,16 @@
 class td(html_tag, name='td'):
     pass
 
 
 class label(html_tag, name='label'):
     for_ = attr(type=str)
 
-    def __set_ref__(self, parent, ref):
-        super().__set_ref__(parent, ref)
+    def _set_ref(self, parent, ref):
+        super()._set_ref(parent, ref)
         if parent and isinstance(self.for_, Tag):
             self.for_ = self.for_._ref.__get__(parent).id
 
 
 class form(html_tag, name='form'):
     pass
 
@@ -212,19 +212,19 @@
 
     def _mount_(self, element, parent: Tag, index=None):  # noqa: ARG002 - unused `index`
         # too many copy-paste?
         self.parent = parent
         self.mount_parent = element
         self.pre_mount()
 
-    def clone(self, parent=None):  # noqa: ARG002 - arguments for overriding
+    def _clone(self, parent=None):  # noqa: ARG002 - arguments for overriding
         return self
 
-    def as_child(self, parent: Tag | None, *, exists_ok=False, inline_def=False):  # noqa: ARG002 - args for overriding
-        return super().as_child(parent, exists_ok=True, inline_def=inline_def)
+    def _as_child(self, parent: Tag | None, *, exists_ok=False, inline_def=False):  # noqa: ARG002 - args for overriding
+        return super()._as_child(parent, exists_ok=True, inline_def=inline_def)
 
 
 class Head(StandaloneTag, name='head', mount=js.document.head):
     title = state()
 
     def render(self):
         if self.title:
```

### Comparing `beepy_web-0.9.3/beepy/trackable.py` & `beepy_web-0.9.4/beepy/trackable.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,23 +9,23 @@
     __slots__ = ()
 
     onchange_triggers: list[Callable]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.onchange_triggers = []
-        self._disable_onchange = Locker('Disable onchange()')
+        self.onchange_locker = Locker('Disable onchange()')
 
     @abstractmethod
     def onchange_notify(self):
         pass
 
     def onchange(self, handler=None):
         if handler is None:
-            if not self._disable_onchange:
+            if not self.onchange_locker:
                 self.onchange_notify()
         else:
             if handler in self.onchange_triggers:
                 raise AttributeError('This @onchange trigger is already set')
             self.onchange_triggers.append(handler)
             return handler
 
@@ -47,15 +47,15 @@
 
     @abstractmethod
     def _notify_post_remove(self):
         pass
 
 
 class TrackableList(Trackable, list):
-    __slots__ = ('onchange_triggers', '_disable_onchange')
+    __slots__ = ('onchange_triggers', 'onchange_locker')
 
     def _notify_add(self, key: SupportsIndex | slice, added: Iterable):
         length = len(self)
         if isinstance(key, slice):
             for index, value in zip(range(key.start or 0, key.stop or length, key.step or 1), added, strict=True):
                 if index < 0:
                     index += length  # noqa: PLW2901
@@ -81,88 +81,88 @@
             if index < 0:
                 index += len(self)
             self._notify_remove_one(index, to_remove[0])
 
     def append(self, __object):
         super().append(__object)
 
-        if not self._disable_onchange:
+        if not self.onchange_locker:
             self._notify_add(-1, (self[-1],))
 
     def clear(self):
         length = len(self)
-        if not self._disable_onchange:
+        if not self.onchange_locker:
             self._notify_remove(slice(0, length), self)
         super().clear()
-        if not self._disable_onchange and length:
+        if not self.onchange_locker and length:
             self._notify_post_remove()
             self.onchange()
 
     def extend(self, __iterable):
-        if self._disable_onchange:
+        if self.onchange_locker:
             super().extend(__iterable)
             return
 
         length = len(self)
         super().extend(__iterable)
         self._notify_add(slice(length, len(self)), self[length : len(self)])
 
     def insert(self, __index, __object):
-        if self._disable_onchange:
+        if self.onchange_locker:
             super().insert(__index, __object)
             return
 
         index = __index.__index__()
         super().insert(index, __object)
         self._notify_add(index, (self[index],))
 
     def pop(self, __index=None):
-        if self._disable_onchange:
+        if self.onchange_locker:
             return super().pop(__index)
 
         index = len(self) - 1 if __index is None else __index.__index__()
 
         self._notify_remove(index, (self[index],))
         result = super().pop(__index)
         self._notify_post_remove()
         self.onchange()
         return result
 
     def remove(self, __value):
-        if self._disable_onchange:
+        if self.onchange_locker:
             super().remove(__value)
             return
 
         self._notify_remove(self.index(__value), (__value,))
         super().remove(__value)
         self._notify_post_remove()
         self.onchange()
 
     def copy(self):
         result = type(self)(super().copy())
         result.onchange_triggers = self.onchange_triggers.copy()
         return result
 
     def reverse(self):
-        if self._disable_onchange:
+        if self.onchange_locker:
             super().reverse()
             return
 
         length = len(self)
         self._notify_remove(slice(0, length), self)
 
         super().reverse()
 
         if length:
             self._notify_post_remove()
 
         self._notify_add(slice(0, len(self)), self)
 
     def sort(self, *, key=..., reverse=...):
-        if self._disable_onchange:
+        if self.onchange_locker:
             super().sort(key=key, reverse=reverse)
             return
 
         # TODO: rewrite this after `key=` implemented
         length = len(self)
         self._notify_remove(slice(0, length), self)
 
@@ -170,15 +170,15 @@
 
         if length:
             self._notify_post_remove()
 
         self._notify_add(slice(0, len(self)), self)
 
     def __delitem__(self, key):
-        if self._disable_onchange:
+        if self.onchange_locker:
             super().__delitem__(key)
             return
 
         to_remove = self[key]
         if not isinstance(to_remove, list):
             to_remove = (to_remove,)
 
@@ -189,15 +189,15 @@
             self.onchange()
 
     def __iadd__(self, other):
         self.extend(other)
         return self
 
     def __imul__(self, n):
-        if self._disable_onchange:
+        if self.onchange_locker:
             return super().__imul__(n)
 
         length = len(self)
         n = n.__index__()
         if n <= 0:
             self._notify_remove(slice(0, length), self)
         super().__imul__(n)
@@ -205,15 +205,15 @@
             if length:
                 self._notify_post_remove()
         else:
             self._notify_add(slice(length, len(self)), self[length : len(self)])
         return self
 
     def __setitem__(self, key, value):
-        if self._disable_onchange:
+        if self.onchange_locker:
             super().__setitem__(key, value)
             return
 
         to_remove = self[key]
         if not isinstance(to_remove, list):
             to_remove = (to_remove,)
```

### Comparing `beepy_web-0.9.3/beepy/types.py` & `beepy_web-0.9.4/beepy/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,27 +98,27 @@
     def __init__(self, iterable=()):
         super().__init__(iterable)
         self.parent = None
         self.parent_index = 0
         self.ref = None
         self.mounted = False
 
-    def as_child(self, parent: Tag | None, *, exists_ok=False):
+    def _as_child(self, parent: Tag | None, *, exists_ok=False):
         from beepy.children import ChildrenRef
 
         if self.ref:
             if exists_ok:
                 return self.ref
             else:
                 raise TypeError(f'{self} already is child')
         ref = ChildrenRef(self)
-        self.__set_parent__(parent, 0, ref)
+        self._set_parent(parent, 0, ref)
         return ref
 
-    def __set_parent__(self, parent: Tag | None, index: int, ref: ChildrenRef):
+    def _set_parent(self, parent: Tag | None, index: int, ref: ChildrenRef):
         self.parent = parent
         self.parent_index = index
         self.ref = ref
         if ref.inline_def:
             setattr(type(parent), ref.name, self)
 
     def onchange_notify(self):
@@ -128,15 +128,15 @@
         for trigger in self.onchange_triggers:
             trigger(self.parent)
 
     def _notify_add_one(self, key: int, child: Tag):
         if not self.mounted and not self.parent:
             return
 
-        child.link_parent_attrs(self.parent)
+        child._link_parent_attrs(self.parent)
         child.__mount__(self.parent._children_element, self.parent, key + self.parent_index)
         if self.parent._mount_finished_:
             child.__render__()
 
     def _notify_remove_one(self, _key: int, child: Tag):
         if not self.mounted and not self.parent:
             return
@@ -149,15 +149,15 @@
 
     def __mount__(self, element, parent: Tag, index=None):
         self.mounted = True
 
         if index is not None:
             index += self.parent_index
         for child in self:
-            child.link_parent_attrs(parent)
+            child._link_parent_attrs(parent)
             child.__mount__(element, parent, index)
 
     def __unmount__(self, element, parent):
         self.mounted = False
 
         for child in self:
             child.__unmount__(element, parent)
```

### Comparing `beepy_web-0.9.3/beepy/dev/__main__.py` & `beepy_web-0.9.4/beepy/dev/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,27 +28,27 @@
     def on_any_event(self, event):
         if not (
             event.event_type in ('opened', 'closed')
             or event.is_directory
             or event.src_path.endswith(('~', '.tmp'))
             or re.search(r'/(__pycache__|.git|.idea|dist|build)/', event.src_path)
         ):
-            self.server.handle_file_event(event)
+            self.server._handle_file_event(event)
 
 
 class DevServer:
     def __init__(self, *, root_path=None, parse_cmd=True):
         self.websockets = []
         self.root_path = root_path
         self.observer = None
         self.developer_mode = 'DEVELOPMENT' in os.environ
         if parse_cmd:
-            self.handle_cmd_args()
+            self._handle_cmd_args()
 
-    def handle_cmd_args(self):
+    def _handle_cmd_args(self):
         parser = argparse.ArgumentParser(prog='beepy.dev', description='Simple dev server for BeePy')
         parser.add_argument(
             '-d', '--root-dir', default=Path.cwd(), help='Root directory to start server and watch file changes'
         )
         parser.add_argument('--create', action='store_true', help='Create a default .html and .py files before start')
         args = parser.parse_args()
 
@@ -76,15 +76,15 @@
                 await ws.send(message)
             except ConnectionClosedOK:
                 self.websockets.remove(ws)
 
         if not self.websockets:
             print('[BeePy] No clients connected! Please, restart your page to connect to the dev server')
 
-    def handle_file_event(self, event):
+    def _handle_file_event(self, event):
         path: str = event.src_path.removeprefix(str(self.root_path)).removeprefix('/')
 
         print(f'[BeePy] Found file change: {path}')
         if self.developer_mode:
             if path.endswith('.py'):
                 os.system('hatch build')
             elif path.endswith('.js'):
```

### Comparing `beepy_web-0.9.3/beepy/modules/context_menu.py` & `beepy_web-0.9.4/beepy/modules/context_menu.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.3/beepy/modules/local_storage.py` & `beepy_web-0.9.4/beepy/modules/local_storage.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import json
-from collections.abc import Mapping
+from collections.abc import MutableMapping
 
 from beepy.utils import js
 
 
-class LocalStorage(Mapping):
+class LocalStorage(MutableMapping):
     __slots__ = ('prefix',)
 
     def __init__(self, key: str):
         if not key.strip():
             raise TypeError('Local Storage key cannot be empty')
 
         self.prefix = key
@@ -20,16 +20,19 @@
 
     def __getitem__(self, key):
         return json.loads(js.localStorage.getItem(self.prefix + key) or 'null')
 
     def __setitem__(self, key, value):
         js.localStorage.setItem(self.prefix + key, json.dumps(value))
 
+    def __delitem__(self, key):
+        js.localStorage.removeItem(self.prefix + key)
+
     def __iter__(self):
-        return (key[len(self.prefix) :] for key in js.Object.keys(js.localStorage) if key.startswith(self.prefix))
+        return (key.removeprefix(self.prefix) for key in js.Object.keys(js.localStorage) if key.startswith(self.prefix))
 
     def __len__(self):
         return len(tuple(iter(self)))
 
 
 class _GlobalLocalStorage(LocalStorage):
     def __init__(self):
```

### Comparing `beepy_web-0.9.3/beepy/modules/modal.py` & `beepy_web-0.9.4/beepy/modules/modal.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.3/beepy/modules/table.py` & `beepy_web-0.9.4/beepy/modules/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
     children = [
         _columns := Children(),
     ]
 
     @columns.on('mount', 'change')
     def sync(self):
-        if not self.parent_defined:
+        if self._parent_ is None:
             return
 
         self._columns[:] = [TH(column['label']) for column in self.columns]
         if self.parent.actions:
             self._columns.append(TH('Actions'))
 
 
@@ -105,15 +105,15 @@
 
     children = [
         _rows := Children(),
     ]
 
     @rows.on('mount', 'change')
     def sync(self):
-        if not self.parent_defined:
+        if self._parent_ is None:
             return
 
         self._rows[:] = [
             TR(
                 data=[
                     *(
                         {'value': cell, 'view': col['view'](cell).__view_value__() if 'view' in col else cell}
```

### Comparing `beepy_web-0.9.3/beepy/modules/tabs.py` & `beepy_web-0.9.4/beepy/modules/tabs.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 
     @attr()
     def id(self) -> str:
         return f'tab-{self.parent.name}/{self.tab_id}'
 
     parent: tabs
 
-    def __set_ref__(self, parent, ref):
-        super().__set_ref__(parent, ref)
+    def _set_ref(self, parent, ref):
+        super()._set_ref(parent, ref)
         self.tab_id = ref.name
 
 
 class tab_title(Tag, name='li', content_tag=None):
     _tab: tab = state(type=tab)
     selected = attr(default=False)
 
@@ -108,15 +108,15 @@
     @classmethod
     def __class_declared__(cls):
         for tab_id, _tab_title in cls.tabs_titles.child.ref_children.items():
             _tab_title.on('click')(lambda _ul, _tab_id=tab_id: _ul.parent.select_tab(_tab_id))
 
     def mount(self):
         for tab_id, _tab in self.tabs_list.items():
-            getattr(self.tabs_titles, tab_id).link_parent_attrs(self)
+            getattr(self.tabs_titles, tab_id)._link_parent_attrs(self)
 
         url = js.URL.new(js.location.href)
 
         selected = None
         if url.hash and url.hash.startswith(f'#tab-{self.name}/'):
             selected = self.select_tab(url.hash[len(f'#tab-{self.name}/') :])
             if selected:
```

### Comparing `beepy_web-0.9.3/beepy/utils/api.py` & `beepy_web-0.9.4/beepy/utils/api.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.3/beepy/utils/asyncio.py` & `beepy_web-0.9.4/beepy/utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.3/beepy/utils/common.py` & `beepy_web-0.9.4/beepy/utils/common.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.3/beepy/utils/dev.py` & `beepy_web-0.9.4/beepy/utils/dev.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.3/beepy/utils/import_hooks.py` & `beepy_web-0.9.4/beepy/utils/import_hooks.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.3/beepy/utils/internal.py` & `beepy_web-0.9.4/beepy/utils/internal.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.3/beepy/utils/js.py` & `beepy_web-0.9.4/beepy/utils/js.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,14 +188,17 @@
 class LocalStorage(dict):
     def getItem(self, key):
         return self[key]
 
     def setItem(self, key, value):
         self[key] = value
 
+    def removeItem(self, key):
+        del self[key]
+
 
 localStorage = LocalStorage()
 
 
 def decodeURI(text):
     return text
```

### Comparing `beepy_web-0.9.3/beepy/utils/js_py.py` & `beepy_web-0.9.4/beepy/utils/js_py.py`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.3/web/package-lock.json` & `beepy_web-0.9.4/web/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.899982970027248%*

 * *Differences: {"'packages'": "{'': {'version': '0.9.4'}}", "'version'": "'0.9.4'"}*

```diff
@@ -12,15 +12,15 @@
                 "webpack": "^5.89.0",
                 "webpack-cli": "^5.1.4",
                 "webpack-dev-server": "^4.15.1",
                 "webpack-merge": "^5.10.0"
             },
             "license": "MIT",
             "name": "@kor0p/beepy",
-            "version": "0.9.3"
+            "version": "0.9.4"
         },
         "node_modules/@discoveryjs/json-ext": {
             "dev": true,
             "engines": {
                 "node": ">=10.0.0"
             },
             "integrity": "sha512-dBVuXR082gk3jsFp7Rd/JI4kytwGHecnCoTtXFb7DB6CNHp4rg5k1bhg0nWdLGLnOV71lmDzGQaLMy8iPLY0pw==",
@@ -4174,9 +4174,9 @@
             "dev": true,
             "integrity": "sha512-3wdGidZyq5PB084XLES5TpOSRA3wjXAlIWMhum2kRcv/41Sn2emQ0dycQW4uZXLejwKvg6EsvbdlVL+FYEct7A==",
             "resolved": "https://registry.npmjs.org/yallist/-/yallist-4.0.0.tgz",
             "version": "4.0.0"
         }
     },
     "requires": true,
-    "version": "0.9.3"
+    "version": "0.9.4"
 }
```

### Comparing `beepy_web-0.9.3/web/package.json` & `beepy_web-0.9.4/web/package.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9400000000000001%*

 * *Differences: {"'scripts'": "{delete: ['publish-2']}", "'version'": "'0.9.4'"}*

```diff
@@ -27,14 +27,13 @@
         "webassembly"
     ],
     "license": "MIT",
     "main": "",
     "name": "@kor0p/beepy",
     "scripts": {
         "build": "webpack --config webpack.prod.js",
-        "publish-2": "cp ../README.md . && npm publish --access=public && rm README.md",
         "start": "webpack serve --config webpack.dev.js",
         "test": "echo \"Error: no test specified\" && exit 1",
         "watch": "webpack --watch"
     },
-    "version": "0.9.3"
+    "version": "0.9.4"
 }
```

### Comparing `beepy_web-0.9.3/web/webpack.prod.js` & `beepy_web-0.9.4/web/webpack.prod.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.3/web/src/beepy.js` & `beepy_web-0.9.4/web/src/beepy.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -21,15 +21,15 @@
 const _script = document.currentScript
 let localConfig = {}
 if (!!window.beepy) {
     localConfig = window.beepy
 }
 
 class BeePy {
-    __version__ = '0.9.3'
+    __version__ = '0.9.4'
 
     pyodideIndexURL = null
     globals = null
     dev_server = dev_server
     dev_path = ''
     python_api = python
```

### Comparing `beepy_web-0.9.3/web/src/dev-server.js` & `beepy_web-0.9.4/web/src/dev-server.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.3/web/src/files.js` & `beepy_web-0.9.4/web/src/files.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.3/web/src/main.css` & `beepy_web-0.9.4/web/src/main.css`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.3/web/src/python.js` & `beepy_web-0.9.4/web/src/python.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.3/web/src/utils.js` & `beepy_web-0.9.4/web/src/utils.js`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.3/.gitignore` & `beepy_web-0.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.3/LICENSE` & `beepy_web-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.3/README.md` & `beepy_web-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.3/pyproject.toml` & `beepy_web-0.9.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `beepy_web-0.9.3/PKG-INFO` & `beepy_web-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beepy-web
-Version: 0.9.3
+Version: 0.9.4
 Summary: The modern frontend web framework for Python
 Project-URL: Homepage, https://bit.ly/beepy
 Project-URL: Repository, https://github.com/kor0p/BeePy
 Project-URL: Docs, https://kor0p.github.io/BeePy/
 Author-email: kor0p <3.kor0p@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
```

