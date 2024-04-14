# Comparing `tmp/turbobus-1.0.0a5.tar.gz` & `tmp/turbobus-1.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbobus-1.0.0a5.tar", last modified: Thu Oct 12 02:53:41 2023, max compression
+gzip compressed data, was "turbobus-1.0.0a6.tar", last modified: Sun Apr 14 15:01:19 2024, max compression
```

## Comparing `turbobus-1.0.0a5.tar` & `turbobus-1.0.0a6.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 02:53:41.982897 turbobus-1.0.0a5/
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2023-10-12 02:53:41.978896 turbobus-1.0.0a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2616 2023-10-12 02:53:21.000000 turbobus-1.0.0a5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      574 2023-10-12 02:53:21.000000 turbobus-1.0.0a5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-12 02:53:41.982897 turbobus-1.0.0a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-10-12 02:53:21.000000 turbobus-1.0.0a5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 02:53:41.978896 turbobus-1.0.0a5/turbobus/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-10-12 02:53:21.000000 turbobus-1.0.0a5/turbobus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2023-10-12 02:53:21.000000 turbobus-1.0.0a5/turbobus/bus.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2023-10-12 02:53:21.000000 turbobus-1.0.0a5/turbobus/command.py
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-12 02:53:21.000000 turbobus-1.0.0a5/turbobus/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2023-10-12 02:53:21.000000 turbobus-1.0.0a5/turbobus/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2023-10-12 02:53:21.000000 turbobus-1.0.0a5/turbobus/injection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 02:53:41.978896 turbobus-1.0.0a5/turbobus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2023-10-12 02:53:41.000000 turbobus-1.0.0a5/turbobus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      284 2023-10-12 02:53:41.000000 turbobus-1.0.0a5/turbobus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-12 02:53:41.000000 turbobus-1.0.0a5/turbobus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-12 02:53:41.000000 turbobus-1.0.0a5/turbobus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:01:19.663352 turbobus-1.0.0a6/
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-14 15:01:19.663352 turbobus-1.0.0a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-04-14 15:01:05.000000 turbobus-1.0.0a6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-14 15:01:05.000000 turbobus-1.0.0a6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 15:01:19.663352 turbobus-1.0.0a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-14 15:01:05.000000 turbobus-1.0.0a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:01:19.659352 turbobus-1.0.0a6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-14 15:01:05.000000 turbobus-1.0.0a6/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-14 15:01:05.000000 turbobus-1.0.0a6/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-14 15:01:05.000000 turbobus-1.0.0a6/tests/test_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:01:19.659352 turbobus-1.0.0a6/turbobus/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-14 15:01:05.000000 turbobus-1.0.0a6/turbobus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-14 15:01:05.000000 turbobus-1.0.0a6/turbobus/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-14 15:01:05.000000 turbobus-1.0.0a6/turbobus/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-14 15:01:05.000000 turbobus-1.0.0a6/turbobus/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-14 15:01:05.000000 turbobus-1.0.0a6/turbobus/injection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:01:19.663352 turbobus-1.0.0a6/turbobus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-14 15:01:19.000000 turbobus-1.0.0a6/turbobus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-14 15:01:19.000000 turbobus-1.0.0a6/turbobus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 15:01:19.000000 turbobus-1.0.0a6/turbobus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 15:01:19.000000 turbobus-1.0.0a6/turbobus.egg-info/top_level.txt
```

### Comparing `turbobus-1.0.0a5/PKG-INFO` & `turbobus-1.0.0a6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,88 +1,85 @@
-Metadata-Version: 2.1
-Name: turbobus
-Version: 1.0.0a5
-Summary: TurboBus is an opinionated implementation of Command Responsibility Segregation pattern in python.
-Home-page: https://github.com/cafadev/turbobus
-Download-URL: https://github.com/cafadev/turbobus/releases/tag/v1.0.0-alpha.5
-Author: Christopher A. Flores
-Author-email: cafadev@outlook.com
-License: MIT
-Keywords: command,bus,cqrs,commandbus,ddd
-Description-Content-Type: text/markdown
-
 # TurboBus
 
 TurboBus is an opinionated implementation of Command Responsibility Segregation pattern in python.
 
+## Installation
+```
+pip install turbobus
+```
+
 ## Simple usage
 Let's see an example using python typings. You can omit all the typing stuffs if you want to.
 
 **God Mode ⚡**
 ```python3
-from  dataclasses  import  dataclass
-from  typing  import  TypeAlias
+from dataclasses import dataclass
+from typing import TypeAlias
 
-from  turbobus.command  import  Command, CommandHandler, CommandBus, handler_of
-from  turbobus.injection  import  injectable
+from turbobus.command import Command, CommandHandler, handler_of
+from turbobus.bus import CommandBus
 
 LogHandlerType: TypeAlias  =  "ILogHandler"
 
 @dataclass
-class  LogCommand(Command[LogHandlerType]):
-	content: str  
+class LogCommand(Command[LogHandlerType]):
+    content: str
 
 
-class  ILogHandler(CommandHandler[LogCommand, str]):
-	...
+class ILogHandler(CommandHandler[LogCommand, str]):
+    ...
 
 
 @handler_of(LogCommand)
-class  LogHandler(ILogHandler):
-	def  execute(self, cmd: LogCommand) -> str:
-		return  cmd.content
+class LogHandler(ILogHandler):
+    def execute(self, cmd: LogCommand) -> str:
+        return cmd.content
 
 
 if __name__ == '__main__':
-	bus  =  CommandBus()
+    bus = CommandBus()
 
-	result  =  bus.execute(
-		LogCommand('Hello dude!')
-	)
-	print(result)  # Hello dude
+    result = bus.execute(
+        LogCommand('Hello dude!')
+    )
+    print(result) # Hello dude
 ```
 
 **Human Mode 🥱**
 ```python3
-from  dataclasses  import  dataclass
+from dataclasses import dataclass
+from typing import TypeAlias
 
-from  turbobus.command  import  Command, CommandHandler, handler_of
-from  turbobus.decorators  import injectable
+from turbobus.command import Command, CommandHandler, handler_of
+from turbobus.bus import CommandBus
+
+LogHandlerType: TypeAlias  =  "ILogHandler"
 
 @dataclass
-class  LogCommand(Command):
-	content
+class LogCommand(Command[LogHandlerType]):
+    content: str
+
 
+class ILogHandler(CommandHandler[LogCommand, str]):
+    ...
 
-class  ILogHandler(CommandHandler):
-	...
 
 @handler_of(LogCommand)
-class  LogHandler(ILogHandler):
-	def  execute(self, cmd: LogCommand) -> str:
-		return  cmd.content
+class LogHandler(ILogHandler):
+    def execute(self, cmd: LogCommand) -> str:
+        return cmd.content
 
 
 if __name__ == '__main__':
-	bus  =  CommandBus()
+    bus = CommandBus()
 
-	result  =  bus.execute(
-		LogCommand('Hello dude!')
-	)
-	print(result)  # Hello dude
+    result = bus.execute(
+        LogCommand('Hello dude!')
+    )
+    print(result) # Hello dude
 ```
 
 ## Dependency injection
 In many cases we're going to need to inject dependencies to our command handler. To accomplish that we have two important tools: `@injectable_of` decorator and `inject` function. 
 
 With the `@injectable_of` decorator we can specify a class that is implementing the functionalities of the dependency. For example:
 
@@ -116,7 +113,21 @@
         return cmd.content
 
 ```
 
 As you can see in the example above, we're defining an abstract class with the logger method. Then we're doing the implementation of the `ILogger` and we're indicating that in the `@injectable_of(ILogger)`. 
 
 Then, using the `inject` function, TurboBus is going to map that dependency and inject the instance in the attribute.
+
+
+
+```
+from turbobus.bus import CommandBus
+
+from log.axioma import LogCommand
+
+bus = CommandBus()
+
+result = bus.execute(
+    LogCommand('Hello world')
+)
+```
```

### Comparing `turbobus-1.0.0a5/pyproject.toml` & `turbobus-1.0.0a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `turbobus-1.0.0a5/setup.py` & `turbobus-1.0.0a6/setup.py`

 * *Files identical despite different names*

### Comparing `turbobus-1.0.0a5/turbobus.egg-info/PKG-INFO` & `turbobus-1.0.0a6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,88 +1,97 @@
 Metadata-Version: 2.1
 Name: turbobus
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: TurboBus is an opinionated implementation of Command Responsibility Segregation pattern in python.
 Home-page: https://github.com/cafadev/turbobus
-Download-URL: https://github.com/cafadev/turbobus/releases/tag/v1.0.0-alpha.5
+Download-URL: https://github.com/cafadev/turbobus/releases/tag/v1.0.0-alpha.6
 Author: Christopher A. Flores
 Author-email: cafadev@outlook.com
 License: MIT
 Keywords: command,bus,cqrs,commandbus,ddd
 Description-Content-Type: text/markdown
 
 # TurboBus
 
 TurboBus is an opinionated implementation of Command Responsibility Segregation pattern in python.
 
+## Installation
+```
+pip install turbobus
+```
+
 ## Simple usage
 Let's see an example using python typings. You can omit all the typing stuffs if you want to.
 
 **God Mode ⚡**
 ```python3
-from  dataclasses  import  dataclass
-from  typing  import  TypeAlias
+from dataclasses import dataclass
+from typing import TypeAlias
 
-from  turbobus.command  import  Command, CommandHandler, CommandBus, handler_of
-from  turbobus.injection  import  injectable
+from turbobus.command import Command, CommandHandler, handler_of
+from turbobus.bus import CommandBus
 
 LogHandlerType: TypeAlias  =  "ILogHandler"
 
 @dataclass
-class  LogCommand(Command[LogHandlerType]):
-	content: str  
+class LogCommand(Command[LogHandlerType]):
+    content: str
 
 
-class  ILogHandler(CommandHandler[LogCommand, str]):
-	...
+class ILogHandler(CommandHandler[LogCommand, str]):
+    ...
 
 
 @handler_of(LogCommand)
-class  LogHandler(ILogHandler):
-	def  execute(self, cmd: LogCommand) -> str:
-		return  cmd.content
+class LogHandler(ILogHandler):
+    def execute(self, cmd: LogCommand) -> str:
+        return cmd.content
 
 
 if __name__ == '__main__':
-	bus  =  CommandBus()
+    bus = CommandBus()
 
-	result  =  bus.execute(
-		LogCommand('Hello dude!')
-	)
-	print(result)  # Hello dude
+    result = bus.execute(
+        LogCommand('Hello dude!')
+    )
+    print(result) # Hello dude
 ```
 
 **Human Mode 🥱**
 ```python3
-from  dataclasses  import  dataclass
+from dataclasses import dataclass
+from typing import TypeAlias
+
+from turbobus.command import Command, CommandHandler, handler_of
+from turbobus.bus import CommandBus
 
-from  turbobus.command  import  Command, CommandHandler, handler_of
-from  turbobus.decorators  import injectable
+LogHandlerType: TypeAlias  =  "ILogHandler"
 
 @dataclass
-class  LogCommand(Command):
-	content
+class LogCommand(Command[LogHandlerType]):
+    content: str
 
 
-class  ILogHandler(CommandHandler):
-	...
+class ILogHandler(CommandHandler[LogCommand, str]):
+    ...
+
 
 @handler_of(LogCommand)
-class  LogHandler(ILogHandler):
-	def  execute(self, cmd: LogCommand) -> str:
-		return  cmd.content
+class LogHandler(ILogHandler):
+    def execute(self, cmd: LogCommand) -> str:
+        return cmd.content
 
 
 if __name__ == '__main__':
-	bus  =  CommandBus()
+    bus = CommandBus()
 
-	result  =  bus.execute(
-		LogCommand('Hello dude!')
-	)
-	print(result)  # Hello dude
+    result = bus.execute(
+        LogCommand('Hello dude!')
+    )
+    print(result) # Hello dude
 ```
 
 ## Dependency injection
 In many cases we're going to need to inject dependencies to our command handler. To accomplish that we have two important tools: `@injectable_of` decorator and `inject` function. 
 
 With the `@injectable_of` decorator we can specify a class that is implementing the functionalities of the dependency. For example:
 
@@ -116,7 +125,21 @@
         return cmd.content
 
 ```
 
 As you can see in the example above, we're defining an abstract class with the logger method. Then we're doing the implementation of the `ILogger` and we're indicating that in the `@injectable_of(ILogger)`. 
 
 Then, using the `inject` function, TurboBus is going to map that dependency and inject the instance in the attribute.
+
+
+
+```
+from turbobus.bus import CommandBus
+
+from log.axioma import LogCommand
+
+bus = CommandBus()
+
+result = bus.execute(
+    LogCommand('Hello world')
+)
+```
```

