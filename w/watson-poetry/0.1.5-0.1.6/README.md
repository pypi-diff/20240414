# Comparing `tmp/watson_poetry-0.1.5.tar.gz` & `tmp/watson_poetry-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watson_poetry-0.1.5.tar", max compression
+gzip compressed data, was "watson_poetry-0.1.6.tar", max compression
```

## Comparing `watson_poetry-0.1.5.tar` & `watson_poetry-0.1.6.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       15 2024-04-14 21:41:19.182560 watson_poetry-0.1.5/README.md
--rw-r--r--   0        0        0      620 2024-04-14 21:46:58.728891 watson_poetry-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2534 2024-04-14 21:46:50.583088 watson_poetry-0.1.5/src/watson_poetry/plugin.py
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 watson_poetry-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       15 2024-04-14 21:41:19.182560 watson_poetry-0.1.6/README.md
+-rw-r--r--   0        0        0      620 2024-04-14 21:56:13.250323 watson_poetry-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3042 2024-04-14 21:55:59.415691 watson_poetry-0.1.6/src/watson_poetry/plugin.py
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 watson_poetry-0.1.6/PKG-INFO
```

### Comparing `watson_poetry-0.1.5/src/watson_poetry/plugin.py` & `watson_poetry-0.1.6/src/watson_poetry/plugin.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,23 @@
+from enum import IntEnum
 import subprocess
 import tomllib as toml
 from cleo.io.io import IO
 from cleo.events.console_events import COMMAND
 from cleo.events.console_command_event import ConsoleCommandEvent
 from cleo.events.event_dispatcher import EventDispatcher
 from poetry.console.application import Application
 from poetry.console.commands.env_command import EnvCommand
 from poetry.plugins.application_plugin import ApplicationPlugin
 
+class Verbosity(IntEnum):
+    QUIET = 0
+    VERBOSE = 1
+    VERY_VERBOSE = 2
+    DEBUG = 3
 
 class PoetryPlugin(ApplicationPlugin):
     is_needed: bool = False
     command: str | None = None
     run_in_venv: bool = False
     venv_path = ".venv"
 
@@ -28,41 +34,44 @@
         dispatcher: EventDispatcher
     ) -> None:
         command = event.command
         if not isinstance(command, EnvCommand):
             return
         io = event.io
 
-        verbose_level= io.is_verbose() + io.is_very_verbose() + io.is_debug()
+        verbose_level= Verbosity(io.is_verbose() + io.is_very_verbose() + io.is_debug())
         print(verbose_level)
         
         if self.is_needed:
-            self._rebuild_rust_code(io)
-        elif verbose_level ==3:
-            io.write_line("Maturin Watchdog not set to run any command.")
+            self._run_command(io, verbose_level)
+        elif verbose_level >= Verbosity.VERBOSE:
+            io.write_line("Watson not set to run any command.")
 
     def read_pyproject_toml(self) -> None:
         try:
             with open("pyproject.toml", "rb") as file:
                 config = toml.load(file)
 
                 self.is_needed =  config.get("tool", {}).get("watson", {}).get("always_compile_before_running", False)
                 self.compile_command = config.get("tool", {}).get("watsong", {}).get("command", self.command)
                 self.run_in_venv = config.get("tool", {}).get("watson", {}).get("run_in_venv", self.run_in_venv)
                 self.venv_path = config.get("tool", {}).get("watson", {}).get("venv_path", self.venv_path)
 
         except FileNotFoundError:
             self.is_needed = False
 
-    def _rebuild_rust_code(self, io: IO):
-        """
-        Rebuild Rust code using maturin.
-        """
+    def _run_command(self, io: IO, verbosity: Verbosity):
         if self.run_in_venv:
+            if verbosity is Verbosity.DEBUG:
+                io.write_line(f"Adding prefix to activate venv: source {self.venv_path}/bin/activate &&")
             prefix = f"source {self.venv_path}/bin/activate && "
         else: 
+            if verbosity is Verbosity.DEBUG:
+                io.write_line("No prefix to activate venv.")
             prefix = ""
-
+        if verbosity is Verbosity.DEBUG:
+            io.write_line(f"Running command: {prefix}{self.compile_command}")
         process = subprocess.run(f"{prefix}{self.compile_command}", capture_output=True, shell=True, text=True)
         if process.returncode != 0:
-            io.write_error("Failed to rebuild Rust code. Are you sure maturin is installed?")
+            if verbosity is Verbosity.DEBUG:
+                io.write_line(f"Command failed with return code {process.returncode}.")
             raise subprocess.CalledProcessError(process.returncode, process.args)
```

