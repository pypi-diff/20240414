# Comparing `tmp/airton_ac-2.2.0.tar.gz` & `tmp/airton_ac-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airton_ac-2.2.0.tar", max compression
+gzip compressed data, was "airton_ac-2.2.1.tar", max compression
```

## Comparing `airton_ac-2.2.0.tar` & `airton_ac-2.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2023-03-09 17:12:43.283299 airton_ac-2.2.0/LICENSE
--rw-r--r--   0        0        0     2606 2023-03-09 17:12:43.283299 airton_ac-2.2.0/README.md
--rw-r--r--   0        0        0       67 2023-03-09 17:12:43.283299 airton_ac-2.2.0/airton_ac/__init__.py
--rw-r--r--   0        0        0     4664 2023-03-09 17:12:43.283299 airton_ac-2.2.0/airton_ac/device.py
--rw-r--r--   0        0        0        0 2023-03-09 17:12:43.283299 airton_ac-2.2.0/airton_ac/domoticz/__init__.py
--rw-r--r--   0        0        0     5141 2023-03-09 17:12:43.283299 airton_ac-2.2.0/airton_ac/domoticz/install.py
--rw-r--r--   0        0        0        0 2023-03-09 17:12:43.283299 airton_ac-2.2.0/airton_ac/py.typed
--rw-r--r--   0        0        0     1081 2023-03-09 17:12:43.283299 airton_ac-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     3383 1970-01-01 00:00:00.000000 airton_ac-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-14 20:37:58.403951 airton_ac-2.2.1/LICENSE
+-rw-r--r--   0        0        0     2621 2024-04-14 20:37:58.403951 airton_ac-2.2.1/README.md
+-rw-r--r--   0        0        0       67 2024-04-14 20:37:58.403951 airton_ac-2.2.1/airton_ac/__init__.py
+-rw-r--r--   0        0        0     4684 2024-04-14 20:37:58.403951 airton_ac-2.2.1/airton_ac/device.py
+-rw-r--r--   0        0        0        0 2024-04-14 20:37:58.403951 airton_ac-2.2.1/airton_ac/domoticz/__init__.py
+-rw-r--r--   0        0        0     5141 2024-04-14 20:37:58.403951 airton_ac-2.2.1/airton_ac/domoticz/install.py
+-rw-r--r--   0        0        0        0 2024-04-14 20:37:58.403951 airton_ac-2.2.1/airton_ac/py.typed
+-rw-r--r--   0        0        0     1071 2024-04-14 20:37:58.403951 airton_ac-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3449 1970-01-01 00:00:00.000000 airton_ac-2.2.1/PKG-INFO
```

### Comparing `airton_ac-2.2.0/LICENSE` & `airton_ac-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `airton_ac-2.2.0/README.md` & `airton_ac-2.2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # airton-ac
 
-[![tests](https://github.com/gpajot/airton-ac/workflows/Test/badge.svg?branch=main&event=push)](https://github.com/gpajot/airton-ac/actions?query=workflow%3ATest+branch%3Amain+event%3Apush)
-[![version](https://img.shields.io/pypi/v/airton-ac?label=stable)](https://pypi.org/project/airton-ac/)
-[![python](https://img.shields.io/pypi/pyversions/airton-ac)](https://pypi.org/project/airton-ac/)
+[![tests](https://github.com/gpajot/airton-ac/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/gpajot/airton-ac/actions/workflows/test.yml?query=branch%3Amain+event%3Apush)
+[![version](https://img.shields.io/pypi/v/airton_ac?label=stable)](https://pypi.org/project/airton_ac/)
+[![python](https://img.shields.io/pypi/pyversions/airton_ac)](https://pypi.org/project/airton_ac/)
 
 Control an Airton AC device over LAN.
 This requires having the [wifi module](https://eu.airton.shop/en/products/kit-module-wifi-pour-climatiseurs-airton-en-wifi-ready).
 
 ## Features
 - asynchronous methods and transport
 - persistent communication to the device
```

### Comparing `airton_ac-2.2.0/airton_ac/device.py` & `airton_ac-2.2.1/airton_ac/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         config: DeviceConfig,
         state_updated_callback: Optional[Callable[[ACState], Any]] = None,
     ):
         super().__init__(
             config,
             ACState.load,
             state_updated_callback,
-            Constraints(
+            constraints=Constraints(
                 Constraint(
                     ACDataPoint.ECO,
                     True,
                     (ACDataPoint.SET_POINT, None),
                     (ACDataPoint.FAN, {ACFanSpeed.TURBO}),
                     (ACDataPoint.SLEEP, None),
                 ),
@@ -146,17 +146,17 @@
         await self._update({ACDataPoint.LIGHT: status})
 
     async def switch_swing(self, status: bool) -> None:
         """Toggle swing."""
         await self._update(
             {
                 ACDataPoint.SWING: "un_down" if status else "off",
-                ACDataPoint.SWING_DIRECTION: ACDataPoint.SWING.value
-                if status
-                else "off",
+                ACDataPoint.SWING_DIRECTION: (
+                    ACDataPoint.SWING.value if status else "off"
+                ),
             }
         )
 
     async def switch_sleep(self, status: bool) -> None:
         """Toggle sleep."""
         await self._update({ACDataPoint.SLEEP: status})
```

### Comparing `airton_ac-2.2.0/airton_ac/domoticz/install.py` & `airton_ac-2.2.1/airton_ac/domoticz/install.py`

 * *Files identical despite different names*

### Comparing `airton_ac-2.2.0/pyproject.toml` & `airton_ac-2.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "airton_ac"
-version = "2.2.0"
+version = "2.2.1"
 description = "Control an Airton AC device over LAN."
 authors = ["Gabriel Pajot <gab@les-cactus.co>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/gpajot/airton-ac"
 include = ["airton_ac/py.typed"]
 exclude = ["airton_ac/domoticz/types.py"]
@@ -15,33 +15,33 @@
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

### Comparing `airton_ac-2.2.0/PKG-INFO` & `airton_ac-2.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
-Name: airton-ac
-Version: 2.2.0
+Name: airton_ac
+Version: 2.2.1
 Summary: Control an Airton AC device over LAN.
 Home-page: https://github.com/gpajot/airton-ac
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
 Project-URL: Repository, https://github.com/gpajot/airton-ac
 Description-Content-Type: text/markdown
 
 # airton-ac
 
-[![tests](https://github.com/gpajot/airton-ac/workflows/Test/badge.svg?branch=main&event=push)](https://github.com/gpajot/airton-ac/actions?query=workflow%3ATest+branch%3Amain+event%3Apush)
-[![version](https://img.shields.io/pypi/v/airton-ac?label=stable)](https://pypi.org/project/airton-ac/)
-[![python](https://img.shields.io/pypi/pyversions/airton-ac)](https://pypi.org/project/airton-ac/)
+[![tests](https://github.com/gpajot/airton-ac/actions/workflows/test.yml/badge.svg?branch=main&event=push)](https://github.com/gpajot/airton-ac/actions/workflows/test.yml?query=branch%3Amain+event%3Apush)
+[![version](https://img.shields.io/pypi/v/airton_ac?label=stable)](https://pypi.org/project/airton_ac/)
+[![python](https://img.shields.io/pypi/pyversions/airton_ac)](https://pypi.org/project/airton_ac/)
 
 Control an Airton AC device over LAN.
 This requires having the [wifi module](https://eu.airton.shop/en/products/kit-module-wifi-pour-climatiseurs-airton-en-wifi-ready).
 
 ## Features
 - asynchronous methods and transport
 - persistent communication to the device
```

