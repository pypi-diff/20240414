# Comparing `tmp/vallox_websocket_api-5.1.1.tar.gz` & `tmp/vallox_websocket_api-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vallox_websocket_api-5.1.1.tar", last modified: Mon Mar 11 19:35:37 2024, max compression
+gzip compressed data, was "vallox_websocket_api-5.2.0.tar", last modified: Sun Apr 14 18:29:40 2024, max compression
```

## Comparing `vallox_websocket_api-5.1.1.tar` & `vallox_websocket_api-5.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:35:37.971010 vallox_websocket_api-5.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    33888 2024-03-11 19:35:37.971010 vallox_websocket_api-5.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    32827 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-03-11 19:35:37.971010 vallox_websocket_api-5.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:35:37.967010 vallox_websocket_api-5.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/tests/test_fetch_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/tests/test_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/tests/test_set_temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/tests/test_vallox_alarm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/tests/test_vallox_fan_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/tests/test_vallox_filter_change.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/tests/test_vallox_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/tests/test_vallox_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/tests/test_vallox_temperatures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:35:37.967010 vallox_websocket_api-5.1.1/vallox_websocket_api/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/vallox_websocket_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/vallox_websocket_api/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:35:37.971010 vallox_websocket_api-5.1.1/vallox_websocket_api/data/
--rw-r--r--   0 runner    (1001) docker     (127)    54871 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/vallox_websocket_api/data/2.0.16.json
--rw-r--r--   0 runner    (1001) docker     (127)    56287 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/vallox_websocket_api/data/2.0.22.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/vallox_websocket_api/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/vallox_websocket_api/data/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8493 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/vallox_websocket_api/data/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/vallox_websocket_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/vallox_websocket_api/messages.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/vallox_websocket_api/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12566 2024-03-11 19:35:31.000000 vallox_websocket_api-5.1.1/vallox_websocket_api/vallox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 19:35:37.971010 vallox_websocket_api-5.1.1/vallox_websocket_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    33888 2024-03-11 19:35:37.000000 vallox_websocket_api-5.1.1/vallox_websocket_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-11 19:35:37.000000 vallox_websocket_api-5.1.1/vallox_websocket_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 19:35:37.000000 vallox_websocket_api-5.1.1/vallox_websocket_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-11 19:35:37.000000 vallox_websocket_api-5.1.1/vallox_websocket_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-11 19:35:37.000000 vallox_websocket_api-5.1.1/vallox_websocket_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 19:35:37.000000 vallox_websocket_api-5.1.1/vallox_websocket_api.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:29:40.588709 vallox_websocket_api-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    33888 2024-04-14 18:29:40.588709 vallox_websocket_api-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    32827 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-14 18:29:40.588709 vallox_websocket_api-5.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:29:40.584709 vallox_websocket_api-5.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/tests/test_fetch_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5288 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/tests/test_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/tests/test_set_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/tests/test_vallox_alarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/tests/test_vallox_fan_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/tests/test_vallox_filter_change.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/tests/test_vallox_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5361 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/tests/test_vallox_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/tests/test_vallox_temperatures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:29:40.584709 vallox_websocket_api-5.2.0/vallox_websocket_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/vallox_websocket_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11073 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/vallox_websocket_api/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:29:40.588709 vallox_websocket_api-5.2.0/vallox_websocket_api/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    54871 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/vallox_websocket_api/data/2.0.16.json
+-rw-r--r--   0 runner    (1001) docker     (127)    56287 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/vallox_websocket_api/data/2.0.22.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/vallox_websocket_api/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/vallox_websocket_api/data/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8493 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/vallox_websocket_api/data/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/vallox_websocket_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/vallox_websocket_api/messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/vallox_websocket_api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12566 2024-04-14 18:29:36.000000 vallox_websocket_api-5.2.0/vallox_websocket_api/vallox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 18:29:40.588709 vallox_websocket_api-5.2.0/vallox_websocket_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    33888 2024-04-14 18:29:40.000000 vallox_websocket_api-5.2.0/vallox_websocket_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-14 18:29:40.000000 vallox_websocket_api-5.2.0/vallox_websocket_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 18:29:40.000000 vallox_websocket_api-5.2.0/vallox_websocket_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-14 18:29:40.000000 vallox_websocket_api-5.2.0/vallox_websocket_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-14 18:29:40.000000 vallox_websocket_api-5.2.0/vallox_websocket_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 18:29:40.000000 vallox_websocket_api-5.2.0/vallox_websocket_api.egg-info/zip-safe
```

### Comparing `vallox_websocket_api-5.1.1/LICENSE.txt` & `vallox_websocket_api-5.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-5.1.1/PKG-INFO` & `vallox_websocket_api-5.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vallox_websocket_api
-Version: 5.1.1
+Version: 5.2.0
 Summary: Vallox WebSocket API
 Home-page: https://github.com/yozik04/vallox_websocket_api
 Author: Jevgeni Kiski
 Author-email: yozik04@gmail.com
 License: LGPL 3
 Project-URL: Bug Tracker, https://github.com/yozik04/vallox_websocket_api/issues
 Keywords: vallox api
```

### Comparing `vallox_websocket_api-5.1.1/README.md` & `vallox_websocket_api-5.2.0/README.md`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-5.1.1/pyproject.toml` & `vallox_websocket_api-5.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-5.1.1/setup.cfg` & `vallox_websocket_api-5.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-5.1.1/tests/test_client.py` & `vallox_websocket_api-5.2.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-5.1.1/tests/test_fetch_logs.py` & `vallox_websocket_api-5.2.0/tests/test_fetch_logs.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-5.1.1/tests/test_messages.py` & `vallox_websocket_api-5.2.0/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-5.1.1/tests/test_set_temperature.py` & `vallox_websocket_api-5.2.0/tests/test_set_temperature.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-5.1.1/tests/test_vallox_alarm.py` & `vallox_websocket_api-5.2.0/tests/test_vallox_alarm.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-5.1.1/tests/test_vallox_fan_speed.py` & `vallox_websocket_api-5.2.0/tests/test_vallox_fan_speed.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-5.1.1/tests/test_vallox_filter_change.py` & `vallox_websocket_api-5.2.0/tests/test_vallox_filter_change.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-5.1.1/tests/test_vallox_info.py` & `vallox_websocket_api-5.2.0/tests/test_vallox_info.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-5.1.1/tests/test_vallox_profile.py` & `vallox_websocket_api-5.2.0/tests/test_vallox_profile.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-5.1.1/vallox_websocket_api/client.py` & `vallox_websocket_api-5.2.0/vallox_websocket_api/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,14 +101,15 @@
         re.compile(r"^A_CYC_(?:FIREPLACE|EXTRA)_(?:EXTR|SUPP)_FAN$"),
         re.compile(r"^A_CYC_(?:EXTR|SUPP)_FAN_BALANCE_BASE$"),
         re.compile(
             r"^A_CYC_FILTER_CHANGED_(?:DAY|MONTH|YEAR)|A_CYC_FILTER_CHANGE_INTERVAL$"
         ),
         re.compile(r"^A_CYC_FAULT_ACTIVITY(?:_\d{1,2})?$"),
         re.compile(r"^A_CYC_BYPASS_LOCKED$"),
+        re.compile(r"^A_CYC_.*_SETPOINT$"),
     }
 
     _settable_addresses: Dict[int, type]
 
     def __init__(self, ip_address: str):
         self.ip_address = ip_address
         self.data_model = DataModel()
@@ -176,25 +177,38 @@
             self._settable_addresses[key] = var_type
             return
 
         raise ValloxInvalidInputException(
             f"Unable to add address '{address}' to settable list"
         )
 
+    def is_temperature(self, key: str) -> bool:
+        if key.startswith("A_CYC_TEMP_"):
+            return True
+        if key.endswith("TEMP_TARGET"):
+            return True
+        if key.endswith("DEFROST_TEMP"):
+            return True
+        if key.endswith("SETPOINT"):
+            return True
+        if key.endswith("SUPPLY_LOWER_LIMIT"):
+            return True
+        return False
+
     def _encode_pair(
         self, key: str, value: Union[int, float, str]
     ) -> Tuple[int, Union[int, float]]:
         if key not in self.data_model.addresses:
             raise ValloxInvalidInputException(f"Unknown address {key}")
 
         address = int(self.data_model.addresses[key])
         addresses = self.get_settable_addresses()
         assert address in addresses, f"{key} setting is not settable"
 
-        if "_TEMP_" in key:
+        if self.is_temperature(key):
             value = to_kelvin(float(value))
         raw_value: Union[int, float]
         try:
             raw_value = int(value)
         except ValueError:
             raw_value = float(value)
 
@@ -242,15 +256,15 @@
             metric_keys = list(self.data_model.addresses.keys())
 
         for key in metric_keys:
             value = data[
                 self.data_model.calculate_offset(self.data_model.addresses[key])
             ]
 
-            if "_TEMP_" in key:
+            if self.is_temperature(key):
                 value = to_celsius(value)
             elif value == 0xFFFF:
                 value = None
 
             metrics[key] = value
 
         return metrics
```

### Comparing `vallox_websocket_api-5.1.1/vallox_websocket_api/data/2.0.16.json` & `vallox_websocket_api-5.2.0/vallox_websocket_api/data/2.0.16.json`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-5.1.1/vallox_websocket_api/data/2.0.22.json` & `vallox_websocket_api-5.2.0/vallox_websocket_api/data/2.0.22.json`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-5.1.1/vallox_websocket_api/data/constants.py` & `vallox_websocket_api-5.2.0/vallox_websocket_api/data/constants.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-5.1.1/vallox_websocket_api/data/model.py` & `vallox_websocket_api-5.2.0/vallox_websocket_api/data/model.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-5.1.1/vallox_websocket_api/messages.py` & `vallox_websocket_api-5.2.0/vallox_websocket_api/messages.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-5.1.1/vallox_websocket_api/vallox.py` & `vallox_websocket_api-5.2.0/vallox_websocket_api/vallox.py`

 * *Files identical despite different names*

### Comparing `vallox_websocket_api-5.1.1/vallox_websocket_api.egg-info/PKG-INFO` & `vallox_websocket_api-5.2.0/vallox_websocket_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vallox_websocket_api
-Version: 5.1.1
+Version: 5.2.0
 Summary: Vallox WebSocket API
 Home-page: https://github.com/yozik04/vallox_websocket_api
 Author: Jevgeni Kiski
 Author-email: yozik04@gmail.com
 License: LGPL 3
 Project-URL: Bug Tracker, https://github.com/yozik04/vallox_websocket_api/issues
 Keywords: vallox api
```

### Comparing `vallox_websocket_api-5.1.1/vallox_websocket_api.egg-info/SOURCES.txt` & `vallox_websocket_api-5.2.0/vallox_websocket_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

