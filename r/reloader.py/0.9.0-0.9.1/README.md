# Comparing `tmp/reloader_py-0.9.0.tar.gz` & `tmp/reloader_py-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reloader_py-0.9.0.tar", max compression
+gzip compressed data, was "reloader_py-0.9.1.tar", max compression
```

## Comparing `reloader_py-0.9.0.tar` & `reloader_py-0.9.1.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0     1063 2024-02-26 16:10:06.542598 reloader_py-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    17859 2024-02-26 16:36:08.715946 reloader_py-0.9.0/reloader.py
--rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 reloader_py-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-02-28 13:21:03.342323 reloader_py-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    17684 2024-02-28 13:56:02.574985 reloader_py-0.9.1/reloader.py
+-rw-r--r--   0        0        0     1045 1970-01-01 00:00:00.000000 reloader_py-0.9.1/PKG-INFO
```

### Comparing `reloader_py-0.9.0/pyproject.toml` & `reloader_py-0.9.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reloader.py"
-version = "0.9.0"
+version = "0.9.1"
 description = "A simple script reloader"
 license = "MIT"
 authors = ["EcmaXp <ecmaxp@ecmaxp.kr>"]
 repository = "https://github.com/EcmaXp/reloader.py"
 packages = [{ include = "reloader.py" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `reloader_py-0.9.0/reloader.py` & `reloader_py-0.9.1/reloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,23 +27,21 @@
 from types import ModuleType, MemberDescriptorType
 from typing import Any, Callable, ClassVar, cast, Generic, TypeVar
 
 from watchdog.events import FileSystemEvent
 from watchdog.observers import Observer
 
 __author__ = "EcmaXp"
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 __license__ = "MIT"
 __url__ = "https://pypi.org/project/reloader.py/"
 __all__ = ["ScriptReloader", "DaemonReloader"]
 
 T = TypeVar("T")
 
-CLEAR_TERM = "\x1b[2J\x1b[H"
-
 
 DEFAULT_DEBOUNCE_INTERVAL = 0.1
 
 
 class ReloadUnsupportedWarning(UserWarning):
     pass
 
@@ -391,15 +389,15 @@
     def watch_module(self, module: ModuleType) -> CodeModule:
         code_module = CodeModule(module)
         code_reloader = partial(self._reload, code_module)
         self._watchdog_handler.add(module.__file__, code_reloader)
         return code_module
 
     def watch_resource(self, path: Path | PathLike | str) -> None:
-        self._watchdog_handler.add(path, partial(self._reload))
+        self._watchdog_handler.add(path, partial(self._reload, self._script_module))
 
     def _run(self):
         try:
             self._CURRENT_INSTANCE.get()
         except LookupError:
             pass
         else:
@@ -539,15 +537,14 @@
             self.stop()
             self.thread.join()
 
 
 parser = argparse.ArgumentParser(description=__doc__.strip())
 parser.add_argument("--loop", "-l", action="store_true")
 parser.add_argument("--clear", "-c", action="store_true")
-parser.add_argument("--system-clear", "-C", action="store_true")
 parser.add_argument(
     "--debounce-interval",
     type=float,
     default=DEFAULT_DEBOUNCE_INTERVAL,
 )
 parser.add_argument(
     "-f",
@@ -575,17 +572,15 @@
         script_path,
         debounce_interval=args.debounce_interval,
     )
 
     for path in args.resource_file:
         reloader.watch_resource(path)
 
-    if args.system_clear:
+    if args.clear:
         reloader.before_tick = lambda: os.system("clear")
-    elif args.clear:
-        reloader.before_tick = lambda: print(end=CLEAR_TERM, flush=True)
 
     reloader.run()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `reloader_py-0.9.0/PKG-INFO` & `reloader_py-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reloader.py
-Version: 0.9.0
+Version: 0.9.1
 Summary: A simple script reloader
 Home-page: https://github.com/EcmaXp/reloader.py
 License: MIT
 Author: EcmaXp
 Author-email: ecmaxp@ecmaxp.kr
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

