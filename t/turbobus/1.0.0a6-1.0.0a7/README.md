# Comparing `tmp/turbobus-1.0.0a6.tar.gz` & `tmp/turbobus-1.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbobus-1.0.0a6.tar", last modified: Sun Apr 14 15:01:19 2024, max compression
+gzip compressed data, was "turbobus-1.0.0a7.tar", last modified: Sun Apr 14 15:02:40 2024, max compression
```

## Comparing `turbobus-1.0.0a6.tar` & `turbobus-1.0.0a7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:01:19.663352 turbobus-1.0.0a6/
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-14 15:01:19.663352 turbobus-1.0.0a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-14 15:01:05.000000 turbobus-1.0.0a6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-14 15:01:05.000000 turbobus-1.0.0a6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 15:01:19.663352 turbobus-1.0.0a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-14 15:01:05.000000 turbobus-1.0.0a6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:01:19.659352 turbobus-1.0.0a6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-14 15:01:05.000000 turbobus-1.0.0a6/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-14 15:01:05.000000 turbobus-1.0.0a6/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-14 15:01:05.000000 turbobus-1.0.0a6/tests/test_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:01:19.659352 turbobus-1.0.0a6/turbobus/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-14 15:01:05.000000 turbobus-1.0.0a6/turbobus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-14 15:01:05.000000 turbobus-1.0.0a6/turbobus/command.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-14 15:01:05.000000 turbobus-1.0.0a6/turbobus/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-14 15:01:05.000000 turbobus-1.0.0a6/turbobus/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-14 15:01:05.000000 turbobus-1.0.0a6/turbobus/injection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:01:19.663352 turbobus-1.0.0a6/turbobus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-14 15:01:19.000000 turbobus-1.0.0a6/turbobus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-14 15:01:19.000000 turbobus-1.0.0a6/turbobus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 15:01:19.000000 turbobus-1.0.0a6/turbobus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 15:01:19.000000 turbobus-1.0.0a6/turbobus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:02:40.553468 turbobus-1.0.0a7/
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-14 15:02:40.553468 turbobus-1.0.0a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-14 15:02:25.000000 turbobus-1.0.0a7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-14 15:02:25.000000 turbobus-1.0.0a7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 15:02:40.553468 turbobus-1.0.0a7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-14 15:02:25.000000 turbobus-1.0.0a7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:02:40.549468 turbobus-1.0.0a7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-14 15:02:25.000000 turbobus-1.0.0a7/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-14 15:02:25.000000 turbobus-1.0.0a7/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-14 15:02:25.000000 turbobus-1.0.0a7/tests/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:02:40.549468 turbobus-1.0.0a7/turbobus/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-14 15:02:25.000000 turbobus-1.0.0a7/turbobus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-04-14 15:02:25.000000 turbobus-1.0.0a7/turbobus/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-14 15:02:25.000000 turbobus-1.0.0a7/turbobus/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-14 15:02:25.000000 turbobus-1.0.0a7/turbobus/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-14 15:02:25.000000 turbobus-1.0.0a7/turbobus/injection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:02:40.553468 turbobus-1.0.0a7/turbobus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-14 15:02:40.000000 turbobus-1.0.0a7/turbobus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-14 15:02:40.000000 turbobus-1.0.0a7/turbobus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 15:02:40.000000 turbobus-1.0.0a7/turbobus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 15:02:40.000000 turbobus-1.0.0a7/turbobus.egg-info/top_level.txt
```

### Comparing `turbobus-1.0.0a6/PKG-INFO` & `turbobus-1.0.0a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: turbobus
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: TurboBus is an opinionated implementation of Command Responsibility Segregation pattern in python.
 Home-page: https://github.com/cafadev/turbobus
-Download-URL: https://github.com/cafadev/turbobus/releases/tag/v1.0.0-alpha.6
+Download-URL: https://github.com/cafadev/turbobus/releases/tag/v1.0.0-alpha.7
 Author: Christopher A. Flores
 Author-email: cafadev@outlook.com
 License: MIT
 Keywords: command,bus,cqrs,commandbus,ddd
 Description-Content-Type: text/markdown
 
 # TurboBus
```

### Comparing `turbobus-1.0.0a6/README.md` & `turbobus-1.0.0a7/README.md`

 * *Files identical despite different names*

### Comparing `turbobus-1.0.0a6/pyproject.toml` & `turbobus-1.0.0a7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `turbobus-1.0.0a6/setup.py` & `turbobus-1.0.0a7/setup.py`

 * *Files identical despite different names*

### Comparing `turbobus-1.0.0a6/tests/test.py` & `turbobus-1.0.0a7/tests/test.py`

 * *Files identical despite different names*

### Comparing `turbobus-1.0.0a6/tests/test_command.py` & `turbobus-1.0.0a7/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `turbobus-1.0.0a6/tests/test_constants.py` & `turbobus-1.0.0a7/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `turbobus-1.0.0a6/turbobus/command.py` & `turbobus-1.0.0a7/turbobus/command.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from abc import abstractmethod, ABC
 from dataclasses import dataclass
 from typing import Any, Generic, TypeVar, cast, dataclass_transform
 
-from .exception import CommandHandlerDoesNotExistException
+from .exception import CommandHandlerDoesNotExist, IncompatibleCommandType, IncompatibleHandlerReturnType
 from .constants import Provider
 
 
 ReturnType = TypeVar('ReturnType')
 
 
 @dataclass_transform(kw_only_default=True, frozen_default=True)
-def command(cls):
+def kw_only_frozen(cls):
     C = dataclass(kw_only=True, frozen=True)(cls)
     return C
 
 
 class Command(Generic[ReturnType]):
     
     __return_type__: type[ReturnType]
 
-    def __class_getitem__(cls, item):
+    def __class_getitem__(cls, returnType):
+        
+
         C = type(cls.__name__, (), {
-            '__return_type__': item,
+            '__return_type__': returnType,
         })
 
         return C
 
 
 class CommandHandler(ABC, Generic[ReturnType]):
 
@@ -43,37 +45,37 @@
         function = cls.execute
 
         function_typing = list(function.__annotations__.values())
 
         if len(function_typing) < 2:
             return
         
-        cmd, returnType = function_typing
+        cmd, return_type = function_typing
 
         try:
             __return_type__ = cmd.__origin__.__return_type__
         except AttributeError:
             __return_type__ = cmd.__return_type__
 
         if cmd is not cls.__command__:
-            raise TypeError(f"Incompatible command type - expected {cls.__command__} but got {cmd} in {cls.__name__}")
+            raise IncompatibleCommandType(cls.__name__, cls.__command__, cmd)
 
-        if __return_type__ != returnType:
-            raise TypeError(f"Incompatible return type - expected {cmd.__return_type__} but got {returnType} in {cls.__name__}")
+        if __return_type__ != return_type:
+            raise IncompatibleHandlerReturnType(cls.__name__, __return_type__, return_type)
 
     @abstractmethod
     def execute(self, cmd: Command[ReturnType]) -> ReturnType:
         """Execute method to implement the command logic"""
 
 
 class CommandBus:
 
     def execute(self, cmd: Command[ReturnType], providers: dict[Any, Any] = {}) -> ReturnType:
         Handler = Provider.get(cmd.__class__.__name__)
 
         if Handler is None:
-            raise CommandHandlerDoesNotExistException()
+            raise CommandHandlerDoesNotExist()
 
         handler = Handler(**providers)
 
         result = handler.execute(cmd)
         return cast(ReturnType, result)
```

### Comparing `turbobus-1.0.0a6/turbobus/injection.py` & `turbobus-1.0.0a7/turbobus/injection.py`

 * *Files identical despite different names*

### Comparing `turbobus-1.0.0a6/turbobus.egg-info/PKG-INFO` & `turbobus-1.0.0a7/turbobus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: turbobus
-Version: 1.0.0a6
+Version: 1.0.0a7
 Summary: TurboBus is an opinionated implementation of Command Responsibility Segregation pattern in python.
 Home-page: https://github.com/cafadev/turbobus
-Download-URL: https://github.com/cafadev/turbobus/releases/tag/v1.0.0-alpha.6
+Download-URL: https://github.com/cafadev/turbobus/releases/tag/v1.0.0-alpha.7
 Author: Christopher A. Flores
 Author-email: cafadev@outlook.com
 License: MIT
 Keywords: command,bus,cqrs,commandbus,ddd
 Description-Content-Type: text/markdown
 
 # TurboBus
```

