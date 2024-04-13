# Comparing `tmp/harlequin_adbc-0.1.0.tar.gz` & `tmp/harlequin_adbc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harlequin_adbc-0.1.0.tar", max compression
+gzip compressed data, was "harlequin_adbc-0.1.1.tar", max compression
```

## Comparing `harlequin_adbc-0.1.0.tar` & `harlequin_adbc-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2024-02-24 05:06:46.026211 harlequin_adbc-0.1.0/LICENSE
--rw-r--r--   0        0        0     5436 2024-02-24 05:06:46.026211 harlequin_adbc-0.1.0/README.md
--rw-r--r--   0        0        0     1951 2024-02-24 05:06:46.026211 harlequin_adbc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       92 2024-02-24 05:06:46.026211 harlequin_adbc-0.1.0/src/harlequin_adbc/__init__.py
--rw-r--r--   0        0        0     8966 2024-02-24 05:06:46.026211 harlequin_adbc-0.1.0/src/harlequin_adbc/adapter.py
--rw-r--r--   0        0        0      924 2024-02-24 05:06:46.026211 harlequin_adbc-0.1.0/src/harlequin_adbc/cli_options.py
--rw-r--r--   0        0        0        0 2024-02-24 05:06:46.026211 harlequin_adbc-0.1.0/src/harlequin_adbc/py.typed
--rw-r--r--   0        0        0     6535 1970-01-01 00:00:00.000000 harlequin_adbc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-13 23:09:29.387088 harlequin_adbc-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5436 2024-04-13 23:09:29.387088 harlequin_adbc-0.1.1/README.md
+-rw-r--r--   0        0        0     1951 2024-04-13 23:09:29.391088 harlequin_adbc-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       92 2024-04-13 23:09:29.391088 harlequin_adbc-0.1.1/src/harlequin_adbc/__init__.py
+-rw-r--r--   0        0        0     8966 2024-04-13 23:09:29.391088 harlequin_adbc-0.1.1/src/harlequin_adbc/adapter.py
+-rw-r--r--   0        0        0      924 2024-04-13 23:09:29.391088 harlequin_adbc-0.1.1/src/harlequin_adbc/cli_options.py
+-rw-r--r--   0        0        0        0 2024-04-13 23:09:29.391088 harlequin_adbc-0.1.1/src/harlequin_adbc/py.typed
+-rw-r--r--   0        0        0     6535 1970-01-01 00:00:00.000000 harlequin_adbc-0.1.1/PKG-INFO
```

### Comparing `harlequin_adbc-0.1.0/LICENSE` & `harlequin_adbc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `harlequin_adbc-0.1.0/README.md` & `harlequin_adbc-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `harlequin_adbc-0.1.0/pyproject.toml` & `harlequin_adbc-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "harlequin-adbc"
-version = "0.1.0"
+version = "0.1.1"
 description = "A Harlequin adapter for ADBC drivers."
 authors = ["Tyler Hillery <tylerhillery@users.noreply.github.com>"]
 homepage = "https://harlequin.sh"
 repository = "https://github.com/TylerHillery/harlequin-adbc"
 license = "MIT"
 readme = "README.md"
 packages = [
@@ -14,15 +14,15 @@
 [tool.poetry.plugins."harlequin.adapter"]
 adbc = "harlequin_adbc:HarlequinAdbcAdapter"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <4.0"
 harlequin = ">=1.7"
 adbc-driver-manager = ">=0.9.0"
-pyarrow = ">=15.0.0"
+pyarrow = ">=14.0.0"
 
 # driver adapters (optional install for extras)
 adbc-driver-flightsql = { version = ">=0.9", optional = true }
 adbc-driver-postgresql = { version = ">=0.9", optional = true }
 adbc-driver-snowflake = { version = ">=0.9", optional = true }
 adbc-driver-sqlite = { version = ">=0.9", optional = true }
```

### Comparing `harlequin_adbc-0.1.0/src/harlequin_adbc/adapter.py` & `harlequin_adbc-0.1.1/src/harlequin_adbc/adapter.py`

 * *Files identical despite different names*

### Comparing `harlequin_adbc-0.1.0/src/harlequin_adbc/cli_options.py` & `harlequin_adbc-0.1.1/src/harlequin_adbc/cli_options.py`

 * *Files identical despite different names*

### Comparing `harlequin_adbc-0.1.0/PKG-INFO` & `harlequin_adbc-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harlequin-adbc
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Harlequin adapter for ADBC drivers.
 Home-page: https://harlequin.sh
 License: MIT
 Author: Tyler Hillery
 Author-email: tylerhillery@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -18,15 +18,15 @@
 Provides-Extra: sqlite
 Requires-Dist: adbc-driver-flightsql (>=0.9) ; extra == "flightsql"
 Requires-Dist: adbc-driver-manager (>=0.9.0)
 Requires-Dist: adbc-driver-postgresql (>=0.9) ; extra == "postgresql"
 Requires-Dist: adbc-driver-snowflake (>=0.9) ; extra == "snowflake"
 Requires-Dist: adbc-driver-sqlite (>=0.9) ; extra == "sqlite"
 Requires-Dist: harlequin (>=1.7)
-Requires-Dist: pyarrow (>=15.0.0)
+Requires-Dist: pyarrow (>=14.0.0)
 Project-URL: Repository, https://github.com/TylerHillery/harlequin-adbc
 Description-Content-Type: text/markdown
 
 # harlequin-adbc
 This repo provides the Harlequin adapter for [ADBC](https://arrow.apache.org/adbc/main/index.html) (arrow database connectivity).
 
 ## Warning
```

