# Comparing `tmp/audiconnectpy-1.5.4.tar.gz` & `tmp/audiconnectpy-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiconnectpy-1.5.4.tar", last modified: Sat Apr 13 17:47:15 2024, max compression
+gzip compressed data, was "audiconnectpy-1.5.5.tar", last modified: Sun Apr 14 15:45:15 2024, max compression
```

## Comparing `audiconnectpy-1.5.4.tar` & `audiconnectpy-1.5.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:47:15.431876 audiconnectpy-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-13 17:47:15.431876 audiconnectpy-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:47:15.431876 audiconnectpy-1.5.4/audiconnectpy/
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/audiconnectpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19481 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/audiconnectpy/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/audiconnectpy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    22828 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/audiconnectpy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/audiconnectpy/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/audiconnectpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/audiconnectpy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    20137 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/audiconnectpy/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    10618 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/audiconnectpy/services.py
--rw-r--r--   0 runner    (1001) docker     (127)    12474 2024-04-13 17:47:00.000000 audiconnectpy-1.5.4/audiconnectpy/vehicle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 17:47:15.431876 audiconnectpy-1.5.4/audiconnectpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-13 17:47:15.000000 audiconnectpy-1.5.4/audiconnectpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-13 17:47:15.000000 audiconnectpy-1.5.4/audiconnectpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 17:47:15.000000 audiconnectpy-1.5.4/audiconnectpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 17:47:15.000000 audiconnectpy-1.5.4/audiconnectpy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-13 17:47:15.000000 audiconnectpy-1.5.4/audiconnectpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-13 17:47:15.000000 audiconnectpy-1.5.4/audiconnectpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-13 17:47:12.000000 audiconnectpy-1.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 17:47:15.431876 audiconnectpy-1.5.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:45:15.834628 audiconnectpy-1.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-14 15:45:15.834628 audiconnectpy-1.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2809 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:45:15.834628 audiconnectpy-1.5.5/audiconnectpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/audiconnectpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19481 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/audiconnectpy/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/audiconnectpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22856 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/audiconnectpy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/audiconnectpy/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/audiconnectpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/audiconnectpy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24025 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/audiconnectpy/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11650 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/audiconnectpy/services.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12482 2024-04-14 15:45:04.000000 audiconnectpy-1.5.5/audiconnectpy/vehicle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:45:15.834628 audiconnectpy-1.5.5/audiconnectpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-14 15:45:15.000000 audiconnectpy-1.5.5/audiconnectpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-14 15:45:15.000000 audiconnectpy-1.5.5/audiconnectpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 15:45:15.000000 audiconnectpy-1.5.5/audiconnectpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 15:45:15.000000 audiconnectpy-1.5.5/audiconnectpy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-14 15:45:15.000000 audiconnectpy-1.5.5/audiconnectpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-14 15:45:15.000000 audiconnectpy-1.5.5/audiconnectpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-14 15:45:13.000000 audiconnectpy-1.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 15:45:15.834628 audiconnectpy-1.5.5/setup.cfg
```

### Comparing `audiconnectpy-1.5.4/LICENSE` & `audiconnectpy-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.4/PKG-INFO` & `audiconnectpy-1.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.5.4
+Version: 1.5.5
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-1.5.4/README.md` & `audiconnectpy-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.4/audiconnectpy/actions.py` & `audiconnectpy-1.5.5/audiconnectpy/actions.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.4/audiconnectpy/api.py` & `audiconnectpy-1.5.5/audiconnectpy/api.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.4/audiconnectpy/auth.py` & `audiconnectpy-1.5.5/audiconnectpy/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     ServiceNotFoundError,
     TimeoutExceededError,
 )
 from .helpers import ExtendedDict, json_loads
 
 TIMEOUT = 120
 DELAY = 10
-HDR_XAPP_VERSION = "4.13.0"
-HDR_USER_AGENT = "myAudi-Android/4.13.0 (Build 800238275.2210271555) Android/11"
+HDR_XAPP_VERSION = "4.23.1"
+HDR_USER_AGENT = "Android/4.23.1 (Build 800240120.root project 'onetouch-android'.ext.buildTime) Android/11"
 MARKET_URL = "https://content.app.my.audi.com/service/mobileapp/configurations"
 CLIENT_ID = "09b6cbec-cd19-4589-82fd-363dfa8c24da@apps_vw-dilab_com"
 MBB_URL = "https://mbboauth-1d.prd.ece.vwg-connect.com/mbbcoauth"
 
 _LOGGER = logging.getLogger(__name__)
```

### Comparing `audiconnectpy-1.5.4/audiconnectpy/helpers.py` & `audiconnectpy-1.5.5/audiconnectpy/helpers.py`

 * *Files identical despite different names*

### Comparing `audiconnectpy-1.5.4/audiconnectpy/models.py` & `audiconnectpy-1.5.5/audiconnectpy/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Definition class."""
 
 from __future__ import annotations
 
-import logging
 from dataclasses import dataclass
 from datetime import datetime as dt
+import logging
+from typing import Any
 
 from .helpers import ExtendedDict
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class Globals:
@@ -127,115 +128,121 @@
     def attributes(self) -> ExtendedDict:
         """Attributes properties."""
         return self._vehicle_data
 
     def _get_attributes(self) -> ExtendedDict:
         attrs = ExtendedDict({"last_access": dt.now()})
 
-        default = self.data.getr("CurrentVehicleDataByRequestResponse.vehicleData.data")
-        vehicle_data = self.data.getr(
-            "StoredVehicleDataResponse.vehicleData.data", default
-        )
+        vehicle_data = self.data
         if vehicle_data is None:
             return ExtendedDict(attrs)
 
-        for raw_data in vehicle_data:
-            for raw_field in raw_data.get("field", {}):
-                ids = raw_field.get("id")
-                value = raw_field.get("value")
-                unit = raw_field.get("unit")
-                if ids == "0x0101010001":
-                    self.measure_time = raw_field.get("tsCarCaptured")
-                    self.send_time = raw_field.get("tsCarSent")
-                    self.send_time_utc = raw_field.get("tsCarSentUtc")
-                    self.measure_mileage = raw_field.get("milCarCaptured")
-                    self.send_mileage = raw_field.get("milCarSent")
-                    attrs.update({"last_update_time": self.send_time_utc})
-
-                if identity := self.IDS.get(ids):
-                    try:
-                        attrs.update({identity: int(value)})
-                    except Exception:  # pylint: disable=broad-except
-                        try:
-                            attrs.update({identity: float(value)})
-                        except Exception:  # pylint: disable=broad-except
-                            attrs.update({identity: value})
-
-                    if UNIT_SYSTEM == "imperial" and unit == "km":  # type: ignore
-                        attrs[identity] = round(attrs[identity] * 0.621371, 2)
-
-                else:
-                    _LOGGER.error("%s not found", ids)
-
-        # Append meta sensors
-        attrs.update(self._metadatas(attrs))
-
+        for key, raw_data in vehicle_data.items():
+            match key:
+                case "access":
+                    data = raw_data.get("accessStatus", {}).get("value", {})
+                    windows_status = self.windows_status(
+                        self.map_name_status(data.get("windows"))
+                    )
+                    doors_status = self.doors_status(
+                        self.map_name_status(data.get("doors"))
+                    )
+                    attrs.update(
+                        {
+                            "overall_status": data.get("overallStatus"),
+                            "doors_lock_status": data.get("doorLockStatus"),
+                            "last_update_time": data.get("carCapturedTimestamp"),
+                            **windows_status,
+                            **doors_status,
+                        }
+                    )
+                case "userCapabilities":
+                    capabilities = raw_data.get("capabilitiesStatus", {}).get(
+                        "value", {}
+                    )
+                    caps = [capability.get("id") for capability in capabilities]
+                    attrs.update({"capabilities": caps})
+                case "fuelStatus":
+                    data = raw_data.get("rangeStatus", {}).get("value", {})
+                    primary_engine = data.get("primaryEngine", {})
+                    secondary_engine = data.get("secondaryEngine", {})
+                    attrs.update(
+                        {
+                            "primary_engine_type": primary_engine.get("type"),
+                            "tank_level_in_percentage": primary_engine.get(
+                                "currentFuelLevel_pct"
+                            ),
+                            "primary_engine_range": primary_engine.get(
+                                "remainingRange_km"
+                            ),
+                        }
+                    )
+                    if secondary_engine:
+                        attrs.update(
+                            {
+                                "secondary_engine_type": secondary_engine.get("type"),
+                                "secondary_engine_range": secondary_engine.get(
+                                    "remainingRange_km"
+                                ),
+                            }
+                        )
+                case "measurements":
+                    range = raw_data.get("rangeStatus", {}).get("value", {})
+                    # fuel_level = raw_data.get("fuelLevelStatus", {}).get("value", {})
+                    odometer = raw_data.get("odometerStatus", {}).get("value", {})
+                    attrs.update(
+                        {
+                            "measure_mileage": odometer.get("odometer"),
+                            "gasoline_range": range.get("gasolineRange"),
+                        }
+                    )
+                case "oiLevel":
+                    data = raw_data.get("oilLevelStatus", {}).get("value", {})
+                    attrs.update({"oil_level_status": data.get("value")})
+                case "vehicleLights":
+                    data = (
+                        raw_data.get("lightsStatus", {})
+                        .get("value", {})
+                        .get("lights", [])
+                    )
+                    for light in data:
+                        attrs.update(
+                            {
+                                f"lights_{light.get('name')}_turn_off": light.get(
+                                    "status"
+                                )
+                                == "Off"
+                            }
+                        )
+                case "vehicleHealthInspection":
+                    data = raw_data.get("maintenanceStatus", {}).get("value", {})
+                    attrs.update(
+                        {
+                            "maintenance_interval_time_to_inspection": data.get(
+                                "inspectionDue_days"
+                            ),
+                            "maintenance_interval_distance_to_inspection": data.get(
+                                "inspectionDue_km"
+                            ),
+                            "total_range": data.get("mileage_km"),
+                            "maintenance_interval_distance_to_oil_change": data.get(
+                                "oilServiceDue_km"
+                            ),
+                            "maintenance_interval_time_to_oil_change": data.get(
+                                "oilServiceDue_days"
+                            ),
+                        }
+                    )
+                case "vehicleHealthWarnings":
+                    data = raw_data.get("warningLights", {}).get("value", {})
         return attrs
 
     @staticmethod
-    def _metadatas(attrs: ExtendedDict) -> ExtendedDict:
+    def tyres_status(attrs: ExtendedDict) -> ExtendedDict:
         metadatas = ExtendedDict({})
-
-        # Windows open status
-        left_check: int | None = attrs.get("state_left_front_window")
-        left_rear_check: int | None = attrs.get("state_left_rear_window")
-        right_check: int | None = attrs.get("state_right_front_window")
-        right_rear_check: int | None = attrs.get("state_right_rear_window")
-        if None not in [left_check, left_rear_check, right_check, right_rear_check]:
-            any_window_open = (
-                left_check != 3
-                and left_rear_check != 3
-                and right_check != 3
-                and right_rear_check != 3
-            )
-            metadatas.update({"any_window_open": any_window_open})
-
-        # Doors lock status
-        left_check = attrs.get("lock_state_left_front_door")
-        left_rear_check = attrs.get("lock_state_left_rear_door")
-        right_check = attrs.get("lock_state_right_front_door")
-        right_rear_check = attrs.get("lock_state_right_rear_door")
-        trunk_unlocked = attrs.get("lock_state_trunk_lid") != 2
-        if b_any_door_unlocked := (
-            None not in [left_check, left_rear_check, right_check, right_rear_check]
-        ):
-            any_door_unlocked = (
-                left_check != 2
-                and left_rear_check != 2
-                and right_check != 2
-                and right_rear_check != 2
-            )
-            metadatas.update({"any_door_unlocked": any_door_unlocked})
-
-        # Doors open status
-        left_check = attrs.get("open_state_left_front_door")
-        left_rear_check = attrs.get("open_state_left_rear_door")
-        right_check = attrs.get("open_state_right_front_door")
-        right_rear_check = attrs.get("open_state_right_rear_door")
-        trunk_open = attrs.get("open_state_trunk_lid") != 3
-        if b_any_door_open := (
-            None not in [left_check, left_rear_check, right_check, right_rear_check]
-        ):
-            any_door_open = (
-                left_check != 3
-                and left_rear_check != 3
-                and right_check != 3
-                and right_rear_check != 3
-            )
-            metadatas.update({"any_door_open": any_door_open})
-
-        # Door trunk status
-        if b_any_door_open and b_any_door_unlocked and trunk_open and trunk_unlocked:
-            if any_door_open and trunk_open:
-                metadatas.update({"doors_trunk_status": "Open"})
-            elif any_door_unlocked and trunk_unlocked:
-                metadatas.update({"doors_trunk_status": "Closed"})
-            else:
-                metadatas.update({"doors_trunk_status": "Locked"})
-
         # Tyre pressure status
         left_check = attrs.get("tyre_pressure_left_front_tyre_difference")
         left_rear_check = attrs.get("tyre_pressure_left_rear_tyre_difference")
         right_check = attrs.get("tyre_pressure_right_front_tyre_difference")
         right_rear_check = attrs.get("tyre_pressure_right_rear_tyre_difference")
         spare_check = attrs.get("tyre_pressure_spare_tyre_difference")
         if None not in [
@@ -252,14 +259,105 @@
                 and right_rear_check != 1
                 and spare_check != 1
             )
             metadatas.update({"any_tyre_problem": any_tyre_pressure})
 
         return metadatas
 
+    @staticmethod
+    def windows_status(attrs: ExtendedDict) -> ExtendedDict:
+        # Windows open status
+        metadatas = ExtendedDict({})
+        left_open = "closed" not in attrs.get("frontLeft", [])
+        left_rear_open = "closed" not in attrs.get("rearLeft", [])
+        right_open = "closed" not in attrs.get("frontRight", [])
+        right_rear_open = "closed" not in attrs.get("rearRight", [])
+        any_window_open = (
+            left_open and left_rear_open and right_open and right_rear_open
+        )
+        metadatas.update(
+            {
+                "open_left_front_window": left_open,
+                "open_left_rear_window": left_rear_open,
+                "open_right_front_window": right_open,
+                "open_right_rear_window": right_rear_open,
+                "open_any_window": any_window_open,
+            }
+        )
+
+        if "unsupported" not in attrs.get("roofCover"):
+            metadatas.update(
+                {"open_roof_cover": "closed" not in attrs.get("roofCover", [])}
+            )
+        if "unsupported" not in attrs.get("sunRoof"):
+            metadatas.update(
+                {"open_sun_roof": "closed" not in attrs.get("sunRoof", [])}
+            )
+
+        return metadatas
+
+    @staticmethod
+    def doors_status(attrs: ExtendedDict) -> ExtendedDict:
+        # Doors lock status
+        metadatas = ExtendedDict({})
+        left_unlock = "locked" not in attrs.get("frontLeft", [])
+        left_rear_unlock = "locked" not in attrs.get("rearLeft", [])
+        right_unlock = "locked" not in attrs.get("frontRight", [])
+        right_rear_unlock = "locked" not in attrs.get("rearRight", [])
+        trunk_unlock = "locked" not in attrs.get("trunk", [])
+        unlock_any_door = (
+            left_unlock and left_rear_unlock and right_unlock and right_rear_unlock
+        )
+        metadatas.update(
+            {
+                "lock_left_front_door": left_unlock,
+                "lock_left_rear_door": left_rear_unlock,
+                "lock_right_front_door": right_unlock,
+                "lock_right_rear_door": right_rear_unlock,
+                "lock_trunk": trunk_unlock,
+                "lock_any_door": unlock_any_door,
+                "lock_doors_trunk": True if unlock_any_door and trunk_unlock else False,
+            }
+        )
+
+        # Doors open status
+        left_open = "closed" not in attrs.get("frontLeft", [])
+        left_rear_open = "closed" not in attrs.get("rearLeft", [])
+        right_open = "closed" not in attrs.get("frontRight", [])
+        right_rear_open = "closed" not in attrs.get("rearRight", [])
+        trunk_open = "closed" not in attrs.get("trunk", [])
+        bonnet_open = "closed" not in attrs.get("bonnet", [])
+        open_any_door = (
+            left_open
+            and left_rear_open
+            and right_open
+            and right_rear_open
+            and trunk_open
+            and bonnet_open
+        )
+
+        metadatas.update(
+            {
+                "open_left_front_door": left_open,
+                "open_left_rear_door": left_rear_open,
+                "open_right_front_door": right_open,
+                "open_right_rear_door": right_rear_open,
+                "open_trunk": trunk_open,
+                "open_bonnet": bonnet_open,
+                "open_any_door": open_any_door,
+            }
+        )
+
+        return metadatas
+
+    @staticmethod
+    def map_name_status(array: dict[str, Any]) -> dict[str, Any]:
+        """Convert name/status to dictionary."""
+        return {item.get("name"): item.get("status") for item in array}
+
 
 @dataclass
 class PreheaterDataResponse:
     """Preheater class."""
 
     data: ExtendedDict
 
@@ -428,30 +526,25 @@
     """Position class."""
 
     data: ExtendedDict
 
     @property
     def is_supported(self) -> bool:
         """Supported status."""
-        return self.data.getr("findCarResponse.Position") is not None
+        return self.data.get("data") is not None
 
     @property
     def attributes(self) -> ExtendedDict:
         """Attributes properties."""
-        coordinate = self.data.getr("findCarResponse.Position.carCoordinate", {})
-        timestamp = self.data.getr("findCarResponse.Position.timestampCarSentUTC")
         attrs = {
             "position": ExtendedDict(
                 {
-                    "latitude": coordinate.get("latitude", 0) / 1000000,
-                    "longitude": coordinate.get("longitude", 0) / 1000000,
-                    "timestamp": timestamp,
-                    "parktime": self.data.getr(
-                        "findCarResponse.parkingTimeUTC", timestamp
-                    ),
+                    "latitude": self.data.getr("data.lat", 0),
+                    "longitude": self.data.getr("data.lon", 0),
+                    "parktime": self.data.getr("data.carCapturedTimestamp"),
                 }
             )
         }
         return ExtendedDict(attrs)
 
 
 @dataclass
```

### Comparing `audiconnectpy-1.5.4/audiconnectpy/services.py` & `audiconnectpy-1.5.5/audiconnectpy/services.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 """Call url service."""
 
 from __future__ import annotations
 
-import logging
 from dataclasses import dataclass
 from datetime import datetime, timedelta
+import logging
 from typing import Any, Literal
 
 from .auth import Auth
-from .const import (
-    BRAND,
-)
+from .const import BRAND
 from .exceptions import AudiException
 from .helpers import ExtendedDict
 from .models import (
     ChargerDataResponse,
     ClimaterDataResponse,
     ClimaterTimerDataResponse,
     DestinationDataResponse,
@@ -61,17 +59,21 @@
             f"{self.url}/bs/vsr/v1/{BRAND}/{self.country}/vehicles/{self.vin}/status"
         )
         data = data if data else ExtendedDict()
         return VehicleDataResponse(data, self.spin is not None)
 
     async def async_get_stored_position(self) -> PositionDataResponse:
         """Get position data."""
+        headers = await self.auth.async_get_headers(token_type="idk")
+        region = "emea" if self.country.upper() != "US" else "na"
         data = await self.auth.get(
-            f"{self.url}/bs/cf/v1/{BRAND}/{self.country}/vehicles/{self.vin}/position"
+            f"https://{region}.bff.cariad.digital/vehicle/v1/vehicles/{self.vin}/parkingposition",
+            headers=headers,
         )
+
         data = data if data else ExtendedDict()
         return PositionDataResponse(data)
 
     async def async_get_destinations(self) -> DestinationDataResponse:
         """Get destination data."""
         data = await self.auth.get(
             f"{self.url}/destinationfeedservice/mydestinations/v1/{BRAND}/{self.country}/vehicles/{self.vin}/destinations"
@@ -170,18 +172,19 @@
             f"{self.url}/bs/departuretimer/v1/{BRAND}/{self.country}/vehicles/{self.vin}/timer"
         )
         data = data if data else ExtendedDict()
         return ClimaterTimerDataResponse(data)
 
     async def async_get_capabilities(self) -> VehicleDataResponse:
         """Get capabilities."""
-        url = "https://emea.bff.cariad.digital"
         headers = await self.auth.async_get_headers(token_type="idk")
+        region = "emea" if self.country.upper() != "US" else "na"
         data = await self.auth.get(
-            f"{url}/vehicle/v1/vehicles/{self.vin}/capabilities", headers=headers
+            f"https://{region}.bff.cariad.digital/vehicle/v1/vehicles/{self.vin}/capabilities",
+            headers=headers,
         )
         data = data if data else ExtendedDict()
         return VehicleDataResponse(data, self.spin is not None)
 
     async def async_get_honkflash(self) -> Any:
         """Get Honk & Flash status."""
         data = await self.auth.get(
@@ -262,15 +265,42 @@
             f"{self.url}/bs/speedalert/v1/{BRAND}/{self.country}/vehicles/{self.vin}/speedAlertConfiguration"
         )
         data = data if data else ExtendedDict()
         return data
 
     async def async_get_selectivestatus(self) -> VehicleDataResponse:
         """Get capabilities."""
-        url = "https://emea.bff.cariad.digital"
+        JOBS2QUERY = {
+            "access",
+            "activeVentilation",
+            "auxiliaryHeating",
+            "batteryChargingCare",
+            "batterySupport",
+            "charging",
+            "chargingProfiles",
+            "chargingTimers",
+            "climatisation",
+            "climatisationTimers",
+            "departureProfiles",
+            "departureTimers",
+            "emergencyCalling",
+            "fuelStatus",
+            "honkAndFlash",
+            "hybridCarAuxiliaryHeating",
+            "lvBattery",
+            "measurements",
+            "oilLevel",
+            "readiness",
+            "userCapabilities",
+            "vehicleHealthInspection",
+            "vehicleHealthWarnings",
+            "vehicleLights",
+        }
+        jobs = ",".join(JOBS2QUERY)
         headers = await self.auth.async_get_headers(token_type="idk")
+        region = "emea" if self.country.upper() != "US" else "na"
         data = await self.auth.get(
-            f"{url}/vehicle/v1/vehicles/{self.vin}/selectivestatus?jobs=access,charging,fuelStatus,climatisation,measurements",
+            f"https://{region}.bff.cariad.digital/vehicle/v1/vehicles/{self.vin}/selectivestatus?jobs={jobs}",
             headers=headers,
         )
         data = data if data else ExtendedDict()
         return VehicleDataResponse(data, self.spin is not None)
```

### Comparing `audiconnectpy-1.5.4/audiconnectpy/vehicle.py` & `audiconnectpy-1.5.5/audiconnectpy/vehicle.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         return True
 
     @retry(exceptions=TimeoutExceededError, tries=3, delay=2)
     async def async_update_vehicle(self) -> None:
         """Update vehicle status."""
         if self.support_vehicle is not False:
             try:
-                result = await self.async_get_vehicle()
+                result = await self.async_get_selectivestatus()
                 if result.is_supported:
                     self.support_vehicle = result.is_supported
                     self.states.update(result.attributes)
             except ServiceNotFoundError as error:
                 if error.args[0] in (401, 403, 502):
                     self.support_vehicle = False
                 else:
```

### Comparing `audiconnectpy-1.5.4/audiconnectpy.egg-info/PKG-INFO` & `audiconnectpy-1.5.5/audiconnectpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiconnectpy
-Version: 1.5.4
+Version: 1.5.5
 Summary: Provides asynchronous authentication and access to Audi Connect
 Author-email: Cyr-ius <cyr-ius@ipocus.net>
 License: GPL-3
 Keywords: connect,async,audi
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `audiconnectpy-1.5.4/pyproject.toml` & `audiconnectpy-1.5.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name        = "audiconnectpy"
-version     = "1.5.4"
+version     = "1.5.5"
 license     = {text = "GPL-3"}
 description = "Provides asynchronous authentication and access to Audi Connect"
 readme      = "README.md"
 authors     = [
     {name = "Cyr-ius", email = "cyr-ius@ipocus.net"}
 ]
 keywords    = ["connect", "async", "audi"]
```

