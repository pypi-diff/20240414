# Comparing `tmp/maturin_watchdog-0.1.9.tar.gz` & `tmp/maturin_watchdog-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maturin_watchdog-0.1.9.tar", max compression
+gzip compressed data, was "maturin_watchdog-0.2.0.tar", max compression
```

## Comparing `maturin_watchdog-0.1.9.tar` & `maturin_watchdog-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       18 2024-04-10 15:27:33.675428 maturin_watchdog-0.1.9/README.md
--rw-r--r--   0        0        0      529 2024-04-10 16:59:59.293063 maturin_watchdog-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     2858 2024-04-10 16:59:52.222914 maturin_watchdog-0.1.9/src/maturin_watchdog/plugin.py
--rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 maturin_watchdog-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0       18 2024-04-10 15:27:33.675428 maturin_watchdog-0.2.0/README.md
+-rw-r--r--   0        0        0      657 2024-04-14 21:05:51.211594 maturin_watchdog-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1948 2024-04-14 21:04:40.043429 maturin_watchdog-0.2.0/src/maturin_watchdog/plugin.py
+-rw-r--r--   0        0        0      498 1970-01-01 00:00:00.000000 maturin_watchdog-0.2.0/PKG-INFO
```

### Comparing `maturin_watchdog-0.1.9/pyproject.toml` & `maturin_watchdog-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maturin-watchdog"
-version = "0.1.9"
+version = "0.2.0"
 description = "Build via maturin when changes are detected"
 authors = ["Jocelyn-Gas <jocelyn.gas@dillygence.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 poetry = "^1.8.2"
@@ -14,8 +14,12 @@
 ruff = "^0.3.5"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."poetry.application.plugin"]
-maturin-watchdog = "maturin_watchdog.plugin:PoetryPlugin"
+maturin-watchdog = "maturin_watchdog.plugin:PoetryPlugin"
+
+[tool.maturin-watchdog]
+always_compile_before_running = false
+compile_command = "source .venv/bin/activate && maturin develop"
```

