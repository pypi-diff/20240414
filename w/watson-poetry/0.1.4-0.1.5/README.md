# Comparing `tmp/watson_poetry-0.1.4.tar.gz` & `tmp/watson_poetry-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watson_poetry-0.1.4.tar", max compression
+gzip compressed data, was "watson_poetry-0.1.5.tar", max compression
```

## Comparing `watson_poetry-0.1.4.tar` & `watson_poetry-0.1.5.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       15 2024-04-14 21:41:19.182560 watson_poetry-0.1.4/README.md
--rw-r--r--   0        0        0      620 2024-04-14 21:42:29.429876 watson_poetry-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2512 2024-04-14 21:41:41.360899 watson_poetry-0.1.4/src/watson_poetry/plugin.py
--rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 watson_poetry-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       15 2024-04-14 21:41:19.182560 watson_poetry-0.1.5/README.md
+-rw-r--r--   0        0        0      620 2024-04-14 21:46:58.728891 watson_poetry-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2534 2024-04-14 21:46:50.583088 watson_poetry-0.1.5/src/watson_poetry/plugin.py
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 watson_poetry-0.1.5/PKG-INFO
```

### Comparing `watson_poetry-0.1.4/pyproject.toml` & `watson_poetry-0.1.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "watson-poetry"
-version = "0.1.4"
+version = "0.1.5"
 description = "Build via maturin when changes are detected"
 authors = ["Jocelyn-Gas <jocelyn.gas@dillygence.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 poetry = "^1.8.2"
```

### Comparing `watson_poetry-0.1.4/src/watson_poetry/plugin.py` & `watson_poetry-0.1.5/src/watson_poetry/plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,20 +29,20 @@
     ) -> None:
         command = event.command
         if not isinstance(command, EnvCommand):
             return
         io = event.io
 
         verbose_level= io.is_verbose() + io.is_very_verbose() + io.is_debug()
-        
-        if verbose_level ==3:
-            io.write_line("Maturin Watchdog not set to run any command.")
+        print(verbose_level)
         
         if self.is_needed:
             self._rebuild_rust_code(io)
+        elif verbose_level ==3:
+            io.write_line("Maturin Watchdog not set to run any command.")
 
     def read_pyproject_toml(self) -> None:
         try:
             with open("pyproject.toml", "rb") as file:
                 config = toml.load(file)
 
                 self.is_needed =  config.get("tool", {}).get("watson", {}).get("always_compile_before_running", False)
```

