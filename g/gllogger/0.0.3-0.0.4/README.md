# Comparing `tmp/gllogger-0.0.3.tar.gz` & `tmp/gllogger-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gllogger-0.0.3.tar", last modified: Sat Apr 13 04:00:09 2024, max compression
+gzip compressed data, was "gllogger-0.0.4.tar", last modified: Sun Apr 14 12:00:33 2024, max compression
```

## Comparing `gllogger-0.0.3.tar` & `gllogger-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-13 04:00:09.598448 gllogger-0.0.3/
--rw-rw-rw-   0        0        0      923 2024-04-13 04:00:09.596368 gllogger-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      536 2024-04-13 03:55:39.000000 gllogger-0.0.3/README.md
--rw-rw-rw-   0        0        0      384 2024-04-13 03:55:39.000000 gllogger-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-13 04:00:09.598448 gllogger-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-13 04:00:09.576500 gllogger-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-04-13 04:00:09.595138 gllogger-0.0.3/src/gllogger.egg-info/
--rw-rw-rw-   0        0        0      923 2024-04-13 04:00:09.000000 gllogger-0.0.3/src/gllogger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-13 04:00:09.000000 gllogger-0.0.3/src/gllogger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-13 04:00:09.000000 gllogger-0.0.3/src/gllogger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-13 04:00:09.000000 gllogger-0.0.3/src/gllogger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    17706 2024-04-13 03:55:39.000000 gllogger-0.0.3/src/gllogger.py
-drwxrwxrwx   0        0        0        0 2024-04-13 04:00:09.593593 gllogger-0.0.3/test/
--rw-rw-rw-   0        0        0     5005 2024-04-13 03:55:39.000000 gllogger-0.0.3/test/test.py
+drwxrwxrwx   0        0        0        0 2024-04-14 12:00:33.847736 gllogger-0.0.4/
+-rw-rw-rw-   0        0        0     1674 2024-04-14 12:00:33.846428 gllogger-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1253 2024-04-14 11:55:13.000000 gllogger-0.0.4/README.md
+-rw-rw-rw-   0        0        0      384 2024-04-14 11:55:13.000000 gllogger-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-14 12:00:33.848447 gllogger-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-14 12:00:33.821378 gllogger-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-04-14 12:00:33.844382 gllogger-0.0.4/src/gllogger.egg-info/
+-rw-rw-rw-   0        0        0     1674 2024-04-14 12:00:33.000000 gllogger-0.0.4/src/gllogger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-14 12:00:33.000000 gllogger-0.0.4/src/gllogger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 12:00:33.000000 gllogger-0.0.4/src/gllogger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-14 12:00:33.000000 gllogger-0.0.4/src/gllogger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    19750 2024-04-14 11:55:13.000000 gllogger-0.0.4/src/gllogger.py
+drwxrwxrwx   0        0        0        0 2024-04-14 12:00:33.842351 gllogger-0.0.4/test/
+-rw-rw-rw-   0        0        0     5005 2024-04-14 11:55:13.000000 gllogger-0.0.4/test/test.py
```

### Comparing `gllogger-0.0.3/src/gllogger.py` & `gllogger-0.0.4/src/gllogger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,64 @@
 """
 from gllogger import gL
 
 gL.getLogger(__name__)
 gL.setGlobalLevel(logging.DEBUG)
 
-gL.init("console")
+gL.init(gL.OT_console)
 
 def gL_function(text):
     print(text)
 gL.setFunction(gL_function)
-gL.init("function")
+gL.init(gL.OT_function)
 
 gL.setLogDir(os.path.join(os.getcwd(), "log", ))
-gL.init("logging")
+gL.init(gL.OT_logging)
 
 gL.debugs("a", 1, True, )
 gL.infos()
 gL.warns()
 gL.errors()
 
+# pip install better_exceptions==0.3.3
+gL.warns(gL(Exception))
+
 """
 
 __all__ = ["gL", ]
 
 import logging
 
 
 class GlobalLogger(logging.Logger):
+    OT_console = 0
+    OT_function = 1
+    OT_logging = 2
+
+    level_map = {
+        # 'WARNING': 'WARN',
+        # 'WARNING': 'W',
+        # 'ERROR': 'E',
+        # 'INFO': 'I',
+        # 'DEBUG': 'D',
+    }
+
     class FunctionHandler(logging.Handler):
         function = None
 
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
 
         def emit(self, record):  # logging.LogRecord
+            if not hasattr(record, "threadNameMe"):
+                return GlobalLogger._instance.warns(
+                    "NOTE: You should import gllogger before executing any other code.")
             if GlobalLogger.FunctionHandler.function is not None:
+                if record.levelname in GlobalLogger.level_map:
+                    record.levelname = GlobalLogger.level_map[record.levelname]
                 record.asyncTaskName = GlobalLogger.get_asyncio_current_task_name()
                 GlobalLogger.FunctionHandler.function(self.format(record))
 
     @classmethod
     def setFunction(cls, func, ):
         GlobalLogger.FunctionHandler.function = func
 
@@ -48,14 +68,19 @@
         GlobalLogger._instance.log_dir_path = dir
 
     class StreamHandler(logging.StreamHandler):
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
 
         def emit(self, record):
+            if not hasattr(record, "threadNameMe"):
+                return GlobalLogger._instance.warns(
+                    "NOTE: You should import gllogger before executing any other code.")
+            if record.levelname in GlobalLogger.level_map:
+                record.levelname = GlobalLogger.level_map[record.levelname]
             record.asyncTaskName = GlobalLogger.get_asyncio_current_task_name()
             return super().emit(record)
 
     @staticmethod
     def get_asyncio_current_task():
         try:
             _asyncio_current_task = asyncio.current_task()
@@ -83,60 +108,59 @@
                         _class_name = type(_class).__name__ + "::"
         return _class_name
 
     _instance = None
     _instance_init = False
 
     def __new__(cls, *args, **kwargs):
-        if len(args) > 0 and args[0] != "__main__":
-            return super().__new__(cls, )
-        else:
-            if not cls._instance:
-                cls._instance = super().__new__(cls, )
-            return cls._instance
+        if len(args) > 0:
+            if isinstance(args[0], BaseException):
+                return cls._better_exceptions(args[0])
+            elif args[0] != "__main__":
+                return super().__new__(cls, )
+        if not cls._instance:
+            cls._instance = super().__new__(cls, )
+        return cls._instance
 
     def __init__(self, *args, **kwargs):
         # print("__init__", args, kwargs)
-        if len(args) > 0 and args[0] != "__main__":
-            super().__init__(*args, **kwargs)
-            # self.setLevel(logging.DEBUG)
-        else:
-            if GlobalLogger._instance_init: return
-            GlobalLogger._instance_init = True
-            super().__init__(*args, **kwargs)
-            # self.setLevel(logging.DEBUG)
-            self.log_dir_path = os.path.join(os.path.dirname(os.path.abspath(sys.argv[0])), "log", )
-            self.output = "console"
-            self.log_format = None
-            self.log_start_time = None
-            self.log_file_path = None
-            self.log_file_fp = None
-            self.log_handler = None
+        if len(args) > 0:
+            if isinstance(args[0], BaseException):
+                return
+            elif args[0] != "__main__":
+                super().__init__(*args, **kwargs)
+                # self.setLevel(logging.DEBUG)
+                return
+        if GlobalLogger._instance_init: return
+        GlobalLogger._instance_init = True
+        super().__init__(*args, **kwargs)
+        self.log_dir_path = os.path.join(os.path.dirname(os.path.abspath(sys.argv[0])), "log", )
+        self.output = self.OT_console
+        self.log_format = None
+        self.log_start_time = None
+        self.log_file_path = None
+        self.log_file_fp = None
+        self.log_handler = None
 
     def init(self, output):
-        """
-        :param output: ("console", "function", "logging",)
-        :return: self
-        """
-        if output in ("console", "function", "logging",):
-            self.output = output
-        else:
+        if output not in (self.OT_console, self.OT_function, self.OT_logging,):
             raise ValueError(f'parameter "output" cannot be {output}.')
+        self.output = output
         self.log_start_time = time.time()
         self.log_file_path = os.path.join(self.log_dir_path, time.strftime("%Y-%m-%d_%H-%M-%S.log", self.utc8()))
-        if self.output == "console":
+        if self.output == self.OT_console:
             self.log_handler = GlobalLogger.StreamHandler(None)
-        elif self.output == "function":
+        elif self.output == self.OT_function:
             self.log_handler = GlobalLogger.FunctionHandler()
-        elif self.output == "logging":
+        elif self.output == self.OT_logging:
             os.makedirs(self.log_dir_path, exist_ok=True)
             self.log_file_fp = open(self.log_file_path, "a", encoding="utf8", buffering=1)
             self.log_handler = GlobalLogger.StreamHandler(self.log_file_fp)
 
-        if self.output in ("console", "function",):
+        if self.output in (self.OT_console, self.OT_function,):
             _fmt = "[%(levelname)s %(asctime)s %(fullModule)s[%(lineno)d].%(className)s%(funcName)s%(threadNameMe)s%(asyncTaskName)s] %(message)s"
             _datefmt = "%H:%M:%S"
         else:
             # %(name)s pid:%(process)d %(filename)s %(module)s %(pathname)s %(thread)d %(threadName)s
             _fmt = "[%(levelname)s %(asctime)s %(fullModule)s[%(lineno)d].%(className)s%(funcName)s%(threadNameMe)s%(asyncTaskName)s] %(message)s"
             _datefmt = "%m-%d %H:%M:%S"  # %Y-
         self.log_format = logging.Formatter(_fmt, _datefmt)
@@ -147,29 +171,29 @@
 
     @staticmethod
     def utc8(*args, **kwargs):
         # (datetime.datetime.utcnow() + datetime.timedelta(hours=8)).timetuple()
         return time.gmtime(time.time() + (8 * 3600))  # gmtime localtime
 
     def switch(self, ):
-        if self.output != "logging": return
+        if self.output != self.OT_logging: return
         self.infos(f"""switch log files.""")
         os.makedirs(self.log_dir_path, exist_ok=True)
         self.unset_handler()
         self.log_handler.stream.close()
         self.log_start_time = time.time()
         self.log_file_path = os.path.join(self.log_dir_path, time.strftime("%Y-%m-%d_%H-%M-%S.log", self.utc8()))
         self.log_file_fp = open(self.log_file_path, "a", encoding="utf8", buffering=1)
         self.log_handler = GlobalLogger.StreamHandler(self.log_file_fp)
         self.log_handler.setFormatter(self.log_format)
         self.set_handler()
 
     @staticmethod
     def check_switch():
-        if GlobalLogger._instance.output != "logging": return
+        if GlobalLogger._instance.output != GlobalLogger.OT_logging: return
         if time.time() - GlobalLogger._instance.log_start_time >= 60 * 60 * 12:
             GlobalLogger._instance.switch()
 
     @staticmethod
     def unset_handler():
         # GlobalLogger._instance.removeHandler(GlobalLogger._instance.log_handler)
         logging.getLogger().removeHandler(GlobalLogger._instance.log_handler)
@@ -338,43 +362,63 @@
 
     @staticmethod
     def setGlobalLevel(level):
         return logging.getLogger().setLevel(level)
 
     @staticmethod
     def setLoggerClass():
-        return logging.setLoggerClass(GlobalLogger)
+        logging.setLoggerClass(GlobalLogger)
+        logging.setLoggerClass = lambda *args, **kwargs: GlobalLogger._instance.warns(args, kwargs)
+        return
 
     @staticmethod
     def loggers():
         # [print(i) for i in gL.loggers()]
         for logger_name in logging.Logger.manager.loggerDict:
             yield logging.getLogger(logger_name)
 
     """====================================="""
 
     @staticmethod
+    def _better_exceptions(e):
+        try:
+            import better_exceptions
+        except ImportError:
+            import traceback
+            return "".join(traceback.TracebackException.from_exception(e).format())
+        else:
+            _name = "_gllogger_SUPPORTS_COLOR"
+            if not hasattr(better_exceptions, _name):
+                setattr(better_exceptions, _name, better_exceptions.SUPPORTS_COLOR)
+            if getattr(better_exceptions, _name):
+                better_exceptions.SUPPORTS_COLOR = GlobalLogger._instance.output == GlobalLogger.OT_console
+            # better_exceptions.MAX_LENGTH = None
+            better_exceptions.encoding.ENCODING = 'utf-8'
+            return "".join(better_exceptions.format_exception(type(e), e, e.__traceback__))
+
+    @staticmethod
     def color(text):
         _ = re.search(_re1__color, text)
         head, text = _.group(1), _.group(2)
         _gn, _br, _space = "\n", "<br />", "&nbsp;"
         level = re.search(_re2__color, head).group(1)
-        if level in ("WARNING", "ERROR",):
+        if level in ("WARNING", "ERROR",
+                     GlobalLogger.level_map.get("WARNING", "W"), GlobalLogger.level_map.get("ERROR", "E"),):
             c = "#FF0000"
             _text, _ts = [], text.split("\n")
             for _i, i in enumerate(_ts):
-                if _i == len(_ts) - 1 and len(i) == 0: continue
+                # if _i == len(_ts) - 1 and len(i) == 0: continue
                 _text.append(f"{html.escape(i)}" if len(_text) == 0 else
                              f'<p style="color:{c};margin: 0;padding: 0;">{html.escape(i).replace(" ", _space)}</p>')
             return f'<p style="color:{c};margin: 0;padding: 0;">{html.escape(head)}{_text[0]}</p>{"".join(_text[1:])}'
         else:
             c = "#0000FF"
             _text, _ts = [], text.split("\n")
             for _i, i in enumerate(_ts):
-                if _i == len(_ts) - 1 and len(i) == 0: continue
+                # if _i == len(_ts) - 1 and len(i) == 0: continue
                 _text.append(f"{html.escape(i)}" if len(_text) == 0 else
                              f'<p style="margin: 0;padding: 0;">{html.escape(i).replace(" ", _space)}</p>')
             return f'<p style="color:{c};margin: 0;padding: 0;">{html.escape(head)}<span style="color:inherit;">{_text[0]}</span></p>{"".join(_text[1:])}'
 
 
 gL = GlobalLogger
 gL.setLoggerClass()
```

### Comparing `gllogger-0.0.3/test/test.py` & `gllogger-0.0.4/test/test.py`

 * *Files identical despite different names*

