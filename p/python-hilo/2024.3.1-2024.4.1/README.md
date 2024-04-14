# Comparing `tmp/python_hilo-2024.3.1.tar.gz` & `tmp/python_hilo-2024.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_hilo-2024.3.1.tar", max compression
+gzip compressed data, was "python_hilo-2024.4.1.tar", max compression
```

## Comparing `python_hilo-2024.3.1.tar` & `python_hilo-2024.4.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1082 2024-03-02 01:22:10.748482 python_hilo-2024.3.1/LICENSE
--rw-r--r--   0        0        0      596 2024-03-02 01:22:10.748726 python_hilo-2024.3.1/README.md
--rw-r--r--   0        0        0      109 2024-03-02 01:22:10.749088 python_hilo-2024.3.1/pyhilo/__init__.py
--rw-r--r--   0        0        0    23690 2024-03-02 01:23:21.861292 python_hilo-2024.3.1/pyhilo/api.py
--rw-r--r--   0        0        0     7529 2024-03-02 01:23:21.861830 python_hilo-2024.3.1/pyhilo/const.py
--rw-r--r--   0        0        0     9762 2024-03-02 01:22:10.750426 python_hilo-2024.3.1/pyhilo/device/__init__.py
--rw-r--r--   0        0        0     1303 2024-03-02 01:22:10.750756 python_hilo-2024.3.1/pyhilo/device/climate.py
--rw-r--r--   0        0        0      946 2024-03-02 01:22:10.751032 python_hilo-2024.3.1/pyhilo/device/light.py
--rw-r--r--   0        0        0      462 2024-03-02 01:22:10.751282 python_hilo-2024.3.1/pyhilo/device/sensor.py
--rw-r--r--   0        0        0      454 2024-03-02 01:22:10.751538 python_hilo-2024.3.1/pyhilo/device/switch.py
--rw-r--r--   0        0        0     4070 2024-03-02 01:22:10.751809 python_hilo-2024.3.1/pyhilo/devices.py
--rw-r--r--   0        0        0     5599 2024-03-02 01:22:10.752100 python_hilo-2024.3.1/pyhilo/event.py
--rw-r--r--   0        0        0     1191 2024-03-02 01:22:10.752339 python_hilo-2024.3.1/pyhilo/exceptions.py
--rw-r--r--   0        0        0     2437 2024-03-02 01:23:21.862307 python_hilo-2024.3.1/pyhilo/oauth2.py
--rw-r--r--   0        0        0     1257 2024-03-02 01:22:10.752646 python_hilo-2024.3.1/pyhilo/util/__init__.py
--rw-r--r--   0        0        0     2988 2024-03-02 01:22:10.752818 python_hilo-2024.3.1/pyhilo/util/state.py
--rw-r--r--   0        0        0    13545 2024-03-02 01:22:10.753072 python_hilo-2024.3.1/pyhilo/websocket.py
--rw-r--r--   0        0        0     3195 2024-03-02 01:23:21.862865 python_hilo-2024.3.1/pyproject.toml
--rw-r--r--   0        0        0     1903 1970-01-01 00:00:00.000000 python_hilo-2024.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-04-06 01:10:40.539053 python_hilo-2024.4.1/LICENSE
+-rw-r--r--   0        0        0      596 2024-04-06 01:10:40.539134 python_hilo-2024.4.1/README.md
+-rw-r--r--   0        0        0      109 2024-04-06 01:10:40.539249 python_hilo-2024.4.1/pyhilo/__init__.py
+-rw-r--r--   0        0        0    24439 2024-04-07 23:54:14.080103 python_hilo-2024.4.1/pyhilo/api.py
+-rw-r--r--   0        0        0     7594 2024-04-14 11:24:13.274950 python_hilo-2024.4.1/pyhilo/const.py
+-rw-r--r--   0        0        0     9762 2024-04-06 01:10:40.539681 python_hilo-2024.4.1/pyhilo/device/__init__.py
+-rw-r--r--   0        0        0     1303 2024-04-06 01:10:40.539766 python_hilo-2024.4.1/pyhilo/device/climate.py
+-rw-r--r--   0        0        0      946 2024-04-06 01:10:40.539854 python_hilo-2024.4.1/pyhilo/device/light.py
+-rw-r--r--   0        0        0      462 2024-04-06 01:10:40.539935 python_hilo-2024.4.1/pyhilo/device/sensor.py
+-rw-r--r--   0        0        0      454 2024-04-06 01:10:40.540022 python_hilo-2024.4.1/pyhilo/device/switch.py
+-rw-r--r--   0        0        0     4070 2024-04-06 01:10:40.540120 python_hilo-2024.4.1/pyhilo/devices.py
+-rw-r--r--   0        0        0     5599 2024-04-06 01:10:40.540219 python_hilo-2024.4.1/pyhilo/event.py
+-rw-r--r--   0        0        0     1191 2024-04-06 01:10:40.540295 python_hilo-2024.4.1/pyhilo/exceptions.py
+-rw-r--r--   0        0        0     2437 2024-04-06 01:10:40.540384 python_hilo-2024.4.1/pyhilo/oauth2.py
+-rw-r--r--   0        0        0     1257 2024-04-06 01:10:40.540506 python_hilo-2024.4.1/pyhilo/util/__init__.py
+-rw-r--r--   0        0        0     2988 2024-04-06 01:10:40.540609 python_hilo-2024.4.1/pyhilo/util/state.py
+-rw-r--r--   0        0        0    13545 2024-04-06 01:10:40.540727 python_hilo-2024.4.1/pyhilo/websocket.py
+-rw-r--r--   0        0        0     3195 2024-04-08 01:03:46.002613 python_hilo-2024.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1903 1970-01-01 00:00:00.000000 python_hilo-2024.4.1/PKG-INFO
```

### Comparing `python_hilo-2024.3.1/LICENSE` & `python_hilo-2024.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_hilo-2024.3.1/README.md` & `python_hilo-2024.4.1/README.md`

 * *Files identical despite different names*

### Comparing `python_hilo-2024.3.1/pyhilo/api.py` & `python_hilo-2024.4.1/pyhilo/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -610,14 +610,15 @@
                 "status": "Success"
               },
             ]
           }
         ]
         """
         url = self._get_url("Seasons", location_id, challenge=True)
+        LOG.debug(f"Seasons URL is {url}")
         return cast(dict[str, Any], await self.async_request("get", url))
 
     async def get_gateway(self, location_id: int) -> dict[str, Any]:
         url = self._get_url("Gateways/Info", location_id)
         req = await self.async_request("get", url)
         saved_attrs = [
             "zigBeePairingActivated",
@@ -641,7 +642,26 @@
             "provider": 1,
             "model_number": "EQ000017",
             "sw_version": req[0].get("firmwareVersion"),
         }
         for attr in saved_attrs:
             gw[attr] = {"value": req[0].get(attr)}
         return gw
+
+    async def get_weather(self, location_id: int) -> dict[str, Any]:
+        """This will return the current weather like in the app
+        https://api.hiloenergie.com/Automation/v1/api/Locations/XXXX/Weather
+        [
+          {
+            "temperature": -9.0,
+            "time":"0001-01-01T00:00:00Z",
+            "condition":"Foggy",
+            "icon":0,
+            "humidity":92.0
+          }
+        ]
+        """
+        url = self._get_url("Weather", location_id)
+        LOG.debug(f"Weather URL is {url}")
+        response = await self.async_request("get", url)
+        LOG.debug(f"Weather API response: {response}")
+        return cast(dict[str, Any], await self.async_request("get", url))
```

### Comparing `python_hilo-2024.3.1/pyhilo/const.py` & `python_hilo-2024.4.1/pyhilo/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import aiohttp
 import homeassistant.core
 
 LOG: Final = logging.getLogger(__package__)
 DEFAULT_STATE_FILE: Final = "hilo_state.yaml"
 REQUEST_RETRY: Final = 9
-PYHILO_VERSION: Final = "2023.12.02"
+PYHILO_VERSION: Final = "2024.04.01"
 # TODO: Find a way to keep previous line in sync with pyproject.toml automatically
 
 CONTENT_TYPE_FORM: Final = "application/x-www-form-urlencoded"
 ANDROID_PKG_NAME: Final = "com.hiloenergie.hilo"
 DOMAIN: Final = "hilo"
 # Auth constants
 AUTH_HOSTNAME: Final = "connexion.hiloenergie.com"
@@ -235,30 +235,35 @@
     0: "Hass-Hilo",
     1: "Hilo",
     2: "Netatmo",
     3: "OneLink",
 }
 
 JASCO_MODELS: Final = [
+    "43080",
     "43082",
     "43076",
     "43078",
     "43100",
     "46199",
     "9063",
     "45678",
     "42405",
+    "43094",
     "43095",
     "45853",
 ]
 
 JASCO_OUTLETS: Final = [
     "42405",
+    "43094",
     "43095",
     "43100",
     "45853",
 ]
 
 UNMONITORED_DEVICES: Final = [
     "43076",
+    "43080",
+    "43094",
     "43100",
 ]
```

### Comparing `python_hilo-2024.3.1/pyhilo/device/__init__.py` & `python_hilo-2024.4.1/pyhilo/device/__init__.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2024.3.1/pyhilo/device/climate.py` & `python_hilo-2024.4.1/pyhilo/device/climate.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2024.3.1/pyhilo/device/light.py` & `python_hilo-2024.4.1/pyhilo/device/light.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2024.3.1/pyhilo/devices.py` & `python_hilo-2024.4.1/pyhilo/devices.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2024.3.1/pyhilo/event.py` & `python_hilo-2024.4.1/pyhilo/event.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2024.3.1/pyhilo/exceptions.py` & `python_hilo-2024.4.1/pyhilo/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2024.3.1/pyhilo/oauth2.py` & `python_hilo-2024.4.1/pyhilo/oauth2.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2024.3.1/pyhilo/util/__init__.py` & `python_hilo-2024.4.1/pyhilo/util/__init__.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2024.3.1/pyhilo/util/state.py` & `python_hilo-2024.4.1/pyhilo/util/state.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2024.3.1/pyhilo/websocket.py` & `python_hilo-2024.4.1/pyhilo/websocket.py`

 * *Files identical despite different names*

### Comparing `python_hilo-2024.3.1/pyproject.toml` & `python_hilo-2024.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 exclude = ".venv/.*"
 
 [tool.poetry]
 name = "python-hilo"
-version = "2024.3.1"
+version = "2024.4.1"
 description = "A Python3, async interface to the Hilo API"
 readme = "README.md"
 authors = ["David Vallee Delisle <me@dvd.dev>"]
 maintainers = ["David Vallee Delisle <me@dvd.dev>"]
 license = "MIT"
 repository = "https://github.com/dvd-dev/python-hilo"
 packages = [
@@ -78,15 +78,15 @@
 [tool.poetry.dev-dependencies]
 Sphinx = "^7.1.2"
 aresponses = "^3.0.0"
 asynctest = "^0.13.0"
 pre-commit = "^3.2.2"
 pytest = "^8.0.0"
 pytest-aiohttp = "^1.0.4"
-pytest-cov = "^4.0.0"
+pytest-cov = "^5.0.0"
 sphinx-rtd-theme = "^2.0.0"
 types-pytz = "^2024.1.0"
 
 [tool.pylint.BASIC]
 expected-line-ending-format = "LF"
 
 [tool.pylint."MESSAGES CONTROL"]
```

### Comparing `python_hilo-2024.3.1/PKG-INFO` & `python_hilo-2024.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-hilo
-Version: 2024.3.1
+Version: 2024.4.1
 Summary: A Python3, async interface to the Hilo API
 Home-page: https://github.com/dvd-dev/python-hilo
 License: MIT
 Author: David Vallee Delisle
 Author-email: me@dvd.dev
 Maintainer: David Vallee Delisle
 Maintainer-email: me@dvd.dev
```

