# Comparing `tmp/local_tuya_ceiling_fan-1.5.0.tar.gz` & `tmp/local_tuya_ceiling_fan-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local_tuya_ceiling_fan-1.5.0.tar", max compression
+gzip compressed data, was "local_tuya_ceiling_fan-1.5.1.tar", max compression
```

## Comparing `local_tuya_ceiling_fan-1.5.0.tar` & `local_tuya_ceiling_fan-1.5.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-03-10 20:53:18.870644 local_tuya_ceiling_fan-1.5.0/LICENSE
--rw-r--r--   0        0        0     2476 2023-03-10 20:53:18.870644 local_tuya_ceiling_fan-1.5.0/README.md
--rw-r--r--   0        0        0      199 2023-03-10 20:53:18.870644 local_tuya_ceiling_fan-1.5.0/local_tuya_ceiling_fan/__init__.py
--rw-r--r--   0        0        0     3404 2023-03-10 20:53:18.870644 local_tuya_ceiling_fan-1.5.0/local_tuya_ceiling_fan/device.py
--rw-r--r--   0        0        0        0 2023-03-10 20:53:18.870644 local_tuya_ceiling_fan-1.5.0/local_tuya_ceiling_fan/domoticz/__init__.py
--rw-r--r--   0        0        0     3172 2023-03-10 20:53:18.870644 local_tuya_ceiling_fan-1.5.0/local_tuya_ceiling_fan/domoticz/install.py
--rw-r--r--   0        0        0     1077 2023-03-10 20:53:18.870644 local_tuya_ceiling_fan-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     3291 1970-01-01 00:00:00.000000 local_tuya_ceiling_fan-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-14 20:38:42.959087 local_tuya_ceiling_fan-1.5.1/LICENSE
+-rw-r--r--   0        0        0     2491 2024-04-14 20:38:42.959087 local_tuya_ceiling_fan-1.5.1/README.md
+-rw-r--r--   0        0        0      199 2024-04-14 20:38:42.959087 local_tuya_ceiling_fan-1.5.1/local_tuya_ceiling_fan/__init__.py
+-rw-r--r--   0        0        0     3416 2024-04-14 20:38:42.959087 local_tuya_ceiling_fan-1.5.1/local_tuya_ceiling_fan/device.py
+-rw-r--r--   0        0        0        0 2024-04-14 20:38:42.959087 local_tuya_ceiling_fan-1.5.1/local_tuya_ceiling_fan/domoticz/__init__.py
+-rw-r--r--   0        0        0     3172 2024-04-14 20:38:42.959087 local_tuya_ceiling_fan-1.5.1/local_tuya_ceiling_fan/domoticz/install.py
+-rw-r--r--   0        0        0     1067 2024-04-14 20:38:42.963088 local_tuya_ceiling_fan-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 local_tuya_ceiling_fan-1.5.1/PKG-INFO
```

### Comparing `local_tuya_ceiling_fan-1.5.0/LICENSE` & `local_tuya_ceiling_fan-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `local_tuya_ceiling_fan-1.5.0/README.md` & `local_tuya_ceiling_fan-1.5.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # local-tuya-ceiling-fan
 
-[![tests](https://github.com/gpajot/local-tuya-ceiling-fan/workflows/Test/badge.svg?branch=main&event=push)](https://github.com/gpajot/local-tuya-ceiling-fan/actions?query=workflow%3ATest+branch%3Amain+event%3Apush)
-[![version](https://img.shields.io/pypi/v/local-tuya-ceiling-fan?label=stable)](https://pypi.org/project/local-tuya-ceiling-fan/)
-[![python](https://img.shields.io/pypi/pyversions/local-tuya-ceiling-fan)](https://pypi.org/project/local-tuya-ceiling-fan/)
+[![tests](https://github.com/gpajot/local-tuya-ceiling-fan/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/gpajot/local-tuya-ceiling-fan/actions/workflows/test.yml?query=branch%3Amain+event%3Apush)
+[![version](https://img.shields.io/pypi/v/local_tuya_ceiling_fan?label=stable)](https://pypi.org/project/local_tuya_ceiling_fan/)
+[![python](https://img.shields.io/pypi/pyversions/local_tuya_ceiling_fan)](https://pypi.org/project/local_tuya_ceiling_fan/)
 
 Control a Tuya Ceiling fan over LAN.
 
 ## Features
 - asynchronous methods and transport
 - persistent communication to the device
 - automatic remote device state updates (remotes can still be used)
```

### Comparing `local_tuya_ceiling_fan-1.5.0/local_tuya_ceiling_fan/device.py` & `local_tuya_ceiling_fan-1.5.1/local_tuya_ceiling_fan/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         # Seconds to wait until the fan stops before changing direction.
         change_direction_wait_safety: float = 30,
     ):
         super().__init__(
             config,
             FanState.load,
             state_updated_callback,
-            Constraints(
+            constraints=Constraints(
                 Constraint(
                     FanDataPoint.MODE,
                     FanMode.TEMP,
                     (FanDataPoint.SPEED, None),
                 ),
             ),
         )
```

### Comparing `local_tuya_ceiling_fan-1.5.0/local_tuya_ceiling_fan/domoticz/install.py` & `local_tuya_ceiling_fan-1.5.1/local_tuya_ceiling_fan/domoticz/install.py`

 * *Files identical despite different names*

### Comparing `local_tuya_ceiling_fan-1.5.0/pyproject.toml` & `local_tuya_ceiling_fan-1.5.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "local_tuya_ceiling_fan"
-version = "1.5.0"
+version = "1.5.1"
 description = "Control a Tuya Ceiling fan over LAN."
 authors = ["Gabriel Pajot <gab@les-cactus.co>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gpajot/local-tuya-ceiling-fan"
 include = ["local_tuya_ceiling_fan/py.typed"]
 
@@ -14,33 +14,33 @@
 local-tuya = ">=2.1,<3"
 local-tuya-domoticz-tools = { version = ">=1.1,<2", optional = true }
 
 [tool.poetry.extras]
 domoticz = ["local-tuya-domoticz-tools"]
 
 [tool.poetry.group.test.dependencies]
-pytest = "==7.2.2"
-pytest-asyncio = "==0.20.3"
-pytest-mock = "==3.10.0"
-ruff = "==0.0.254"
-mypy = "==1.1.1"
-black = "==23.1.0"
-pre-commit = "==3.1.1"
+pytest = "==8.1.1"
+pytest-asyncio = "==0.23.6"
+pytest-mock = "==3.14.0"
+ruff = "==0.3.7"
+mypy = "==1.9.0"
+pre-commit = "==3.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 ignore_missing_imports = true
 install_types = true
 non_interactive = true
 check_untyped_defs = true
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
-[tool.ruff]
+[tool.ruff.lint]
 select = ["A", "B", "E", "F", "I", "PT"]
 ignore = ["E501"]
-[tool.ruff.per-file-ignores]
+
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
```

### Comparing `local_tuya_ceiling_fan-1.5.0/PKG-INFO` & `local_tuya_ceiling_fan-1.5.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
-Name: local-tuya-ceiling-fan
-Version: 1.5.0
+Name: local_tuya_ceiling_fan
+Version: 1.5.1
 Summary: Control a Tuya Ceiling fan over LAN.
 Home-page: https://github.com/gpajot/local-tuya-ceiling-fan
 License: MIT
 Author: Gabriel Pajot
 Author-email: gab@les-cactus.co
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: domoticz
 Requires-Dist: local-tuya (>=2.1,<3)
 Requires-Dist: local-tuya-domoticz-tools (>=1.1,<2) ; extra == "domoticz"
 Project-URL: Repository, https://github.com/gpajot/local-tuya-ceiling-fan
 Description-Content-Type: text/markdown
 
 # local-tuya-ceiling-fan
 
-[![tests](https://github.com/gpajot/local-tuya-ceiling-fan/workflows/Test/badge.svg?branch=main&event=push)](https://github.com/gpajot/local-tuya-ceiling-fan/actions?query=workflow%3ATest+branch%3Amain+event%3Apush)
-[![version](https://img.shields.io/pypi/v/local-tuya-ceiling-fan?label=stable)](https://pypi.org/project/local-tuya-ceiling-fan/)
-[![python](https://img.shields.io/pypi/pyversions/local-tuya-ceiling-fan)](https://pypi.org/project/local-tuya-ceiling-fan/)
+[![tests](https://github.com/gpajot/local-tuya-ceiling-fan/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/gpajot/local-tuya-ceiling-fan/actions/workflows/test.yml?query=branch%3Amain+event%3Apush)
+[![version](https://img.shields.io/pypi/v/local_tuya_ceiling_fan?label=stable)](https://pypi.org/project/local_tuya_ceiling_fan/)
+[![python](https://img.shields.io/pypi/pyversions/local_tuya_ceiling_fan)](https://pypi.org/project/local_tuya_ceiling_fan/)
 
 Control a Tuya Ceiling fan over LAN.
 
 ## Features
 - asynchronous methods and transport
 - persistent communication to the device
 - automatic remote device state updates (remotes can still be used)
```

