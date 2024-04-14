# Comparing `tmp/watson_poetry-0.1.3.tar.gz` & `tmp/watson_poetry-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watson_poetry-0.1.3.tar", max compression
+gzip compressed data, was "watson_poetry-0.1.4.tar", max compression
```

## Comparing `watson_poetry-0.1.3.tar` & `watson_poetry-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       18 2024-04-10 15:27:33.675428 watson_poetry-0.1.3/README.md
--rw-r--r--   0        0        0      623 2024-04-14 21:40:53.716697 watson_poetry-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2532 2024-04-14 21:37:52.857203 watson_poetry-0.1.3/src/watson_poetry/plugin.py
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 watson_poetry-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       15 2024-04-14 21:41:19.182560 watson_poetry-0.1.4/README.md
+-rw-r--r--   0        0        0      620 2024-04-14 21:42:29.429876 watson_poetry-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2512 2024-04-14 21:41:41.360899 watson_poetry-0.1.4/src/watson_poetry/plugin.py
+-rw-r--r--   0        0        0      492 1970-01-01 00:00:00.000000 watson_poetry-0.1.4/PKG-INFO
```

### Comparing `watson_poetry-0.1.3/src/watson_poetry/plugin.py` & `watson_poetry-0.1.4/src/watson_poetry/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,18 +41,18 @@
             self._rebuild_rust_code(io)
 
     def read_pyproject_toml(self) -> None:
         try:
             with open("pyproject.toml", "rb") as file:
                 config = toml.load(file)
 
-                self.is_needed =  config.get("tool", {}).get("rubber-duck", {}).get("always_compile_before_running", False)
-                self.compile_command = config.get("tool", {}).get("rubber-duckg", {}).get("command", self.command)
-                self.run_in_venv = config.get("tool", {}).get("rubber-duck", {}).get("run_in_venv", self.run_in_venv)
-                self.venv_path = config.get("tool", {}).get("rubber-duck", {}).get("venv_path", self.venv_path)
+                self.is_needed =  config.get("tool", {}).get("watson", {}).get("always_compile_before_running", False)
+                self.compile_command = config.get("tool", {}).get("watsong", {}).get("command", self.command)
+                self.run_in_venv = config.get("tool", {}).get("watson", {}).get("run_in_venv", self.run_in_venv)
+                self.venv_path = config.get("tool", {}).get("watson", {}).get("venv_path", self.venv_path)
 
         except FileNotFoundError:
             self.is_needed = False
 
     def _rebuild_rust_code(self, io: IO):
         """
         Rebuild Rust code using maturin.
```

