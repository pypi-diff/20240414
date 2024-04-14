# Comparing `tmp/pysma-plus-0.1.4.tar.gz` & `tmp/pysma_plus-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysma-plus-0.1.4.tar", last modified: Sat Apr  6 09:25:57 2024, max compression
+gzip compressed data, was "pysma_plus-0.1.5.tar", last modified: Sun Apr 14 07:30:36 2024, max compression
```

## Comparing `pysma-plus-0.1.4.tar` & `pysma_plus-0.1.5.tar`

### file list

```diff
@@ -1,32 +1,43 @@
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-06 09:25:57.315550 pysma-plus-0.1.4/
--rw-rw-r--   0 sven      (1001) sven      (1001)     1075 2024-03-27 10:30:58.000000 pysma-plus-0.1.4/LICENSE
--rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-03-30 19:14:11.000000 pysma-plus-0.1.4/MANIFEST.in
--rw-r--r--   0 sven      (1001) sven      (1001)     3112 2024-04-06 09:25:57.315550 pysma-plus-0.1.4/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)     1085 2024-04-04 19:52:13.000000 pysma-plus-0.1.4/README.md
--rw-rw-r--   0 sven      (1001) sven      (1001)      895 2024-04-06 09:25:53.000000 pysma-plus-0.1.4/pyproject.toml
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-06 09:25:57.315550 pysma-plus-0.1.4/pysma_plus.egg-info/
--rw-r--r--   0 sven      (1001) sven      (1001)     3112 2024-04-06 09:25:57.000000 pysma-plus-0.1.4/pysma_plus.egg-info/PKG-INFO
--rw-rw-r--   0 sven      (1001) sven      (1001)      597 2024-04-06 09:25:57.000000 pysma-plus-0.1.4/pysma_plus.egg-info/SOURCES.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-04-06 09:25:57.000000 pysma-plus-0.1.4/pysma_plus.egg-info/dependency_links.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)       35 2024-04-06 09:25:57.000000 pysma-plus-0.1.4/pysma_plus.egg-info/requires.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)       10 2024-04-06 09:25:57.000000 pysma-plus-0.1.4/pysma_plus.egg-info/top_level.txt
--rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-03-30 19:16:34.000000 pysma-plus-0.1.4/pysma_plus.egg-info/zip-safe
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-06 09:25:57.314550 pysma-plus-0.1.4/pysmaplus/
--rw-rw-r--   0 sven      (1001) sven      (1001)     1920 2024-03-29 07:19:41.000000 pysma-plus-0.1.4/pysmaplus/__init__.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     6668 2024-04-05 16:45:56.000000 pysma-plus-0.1.4/pysmaplus/const.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    21131 2024-03-28 08:57:32.000000 pysma-plus-0.1.4/pysmaplus/definitions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      603 2024-04-05 19:39:26.000000 pysma-plus-0.1.4/pysmaplus/device.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      426 2024-03-27 10:31:31.000000 pysma-plus-0.1.4/pysmaplus/exceptions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      695 2024-03-27 10:31:31.000000 pysma-plus-0.1.4/pysmaplus/helpers.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     6237 2024-04-05 16:46:03.000000 pysma-plus-0.1.4/pysmaplus/sensor.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    15781 2024-04-05 19:32:42.000000 pysma-plus-0.1.4/pysmaplus/smaennexos.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     9809 2024-04-05 19:23:38.000000 pysma-plus-0.1.4/pysmaplus/smaspeedwireem.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    16194 2024-04-05 16:40:53.000000 pysma-plus-0.1.4/pysmaplus/smawebconnect.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-04-06 09:25:57.316550 pysma-plus-0.1.4/setup.cfg
--rw-rw-r--   0 sven      (1001) sven      (1001)      758 2024-04-06 09:25:53.000000 pysma-plus-0.1.4/setup.py
-drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-06 09:25:57.315550 pysma-plus-0.1.4/tests/
--rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-03-27 10:30:58.000000 pysma-plus-0.1.4/tests/__init__.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      883 2024-03-27 10:30:58.000000 pysma-plus-0.1.4/tests/test_definitions.py
--rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-03-27 10:30:58.000000 pysma-plus-0.1.4/tests/test_helpers.py
--rw-rw-r--   0 sven      (1001) sven      (1001)    17280 2024-03-27 10:30:58.000000 pysma-plus-0.1.4/tests/test_init.py
--rw-rw-r--   0 sven      (1001) sven      (1001)     4785 2024-03-27 10:30:58.000000 pysma-plus-0.1.4/tests/test_sensor.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-14 07:30:36.476540 pysma_plus-0.1.5/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1075 2024-03-27 10:30:58.000000 pysma_plus-0.1.5/LICENSE
+-rw-rw-r--   0 sven      (1001) sven      (1001)       80 2024-03-30 19:14:11.000000 pysma_plus-0.1.5/MANIFEST.in
+-rw-r--r--   0 sven      (1001) sven      (1001)     3112 2024-04-14 07:30:36.476540 pysma_plus-0.1.5/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1085 2024-04-04 19:52:13.000000 pysma_plus-0.1.5/README.md
+-rw-rw-r--   0 sven      (1001) sven      (1001)      895 2024-04-14 07:30:28.000000 pysma_plus-0.1.5/pyproject.toml
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-14 07:30:36.475540 pysma_plus-0.1.5/pysma_plus.egg-info/
+-rw-r--r--   0 sven      (1001) sven      (1001)     3112 2024-04-14 07:30:36.000000 pysma_plus-0.1.5/pysma_plus.egg-info/PKG-INFO
+-rw-rw-r--   0 sven      (1001) sven      (1001)      981 2024-04-14 07:30:36.000000 pysma_plus-0.1.5/pysma_plus.egg-info/SOURCES.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-04-14 07:30:36.000000 pysma_plus-0.1.5/pysma_plus.egg-info/dependency_links.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)       35 2024-04-14 07:30:36.000000 pysma_plus-0.1.5/pysma_plus.egg-info/requires.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)       10 2024-04-14 07:30:36.000000 pysma_plus-0.1.5/pysma_plus.egg-info/top_level.txt
+-rw-rw-r--   0 sven      (1001) sven      (1001)        1 2024-03-30 19:16:34.000000 pysma_plus-0.1.5/pysma_plus.egg-info/zip-safe
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-14 07:30:36.471540 pysma_plus-0.1.5/pysmaplus/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1225 2024-04-10 13:24:27.000000 pysma_plus-0.1.5/pysmaplus/__init__.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6009 2024-04-10 16:37:53.000000 pysma_plus-0.1.5/pysmaplus/const.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1283 2024-04-08 19:36:48.000000 pysma_plus-0.1.5/pysmaplus/const_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    13616 2024-04-14 05:54:46.000000 pysma_plus-0.1.5/pysmaplus/definitions_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    21242 2024-04-11 08:50:06.000000 pysma_plus-0.1.5/pysmaplus/definitions_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      576 2024-04-10 13:24:57.000000 pysma_plus-0.1.5/pysmaplus/device.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     9602 2024-04-10 16:40:01.000000 pysma_plus-0.1.5/pysmaplus/device_em.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    11551 2024-04-14 07:26:35.000000 pysma_plus-0.1.5/pysmaplus/device_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    16414 2024-04-10 14:31:01.000000 pysma_plus-0.1.5/pysmaplus/device_webconnect.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      426 2024-03-27 10:31:31.000000 pysma_plus-0.1.5/pysmaplus/exceptions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      695 2024-03-27 10:31:31.000000 pysma_plus-0.1.5/pysmaplus/helpers.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6357 2024-04-10 19:19:27.000000 pysma_plus-0.1.5/pysmaplus/sensor.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      229 2024-04-14 07:30:36.476540 pysma_plus-0.1.5/setup.cfg
+-rw-rw-r--   0 sven      (1001) sven      (1001)      758 2024-04-14 07:30:28.000000 pysma_plus-0.1.5/setup.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-14 07:30:36.472540 pysma_plus-0.1.5/tests/
+-rw-rw-r--   0 sven      (1001) sven      (1001)   315314 2024-04-08 20:09:20.000000 pysma_plus-0.1.5/tests/__init__.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      916 2024-04-10 14:29:16.000000 pysma_plus-0.1.5/tests/test_definitions.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     1668 2024-04-09 20:11:50.000000 pysma_plus-0.1.5/tests/test_em.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     8246 2024-04-11 15:05:50.000000 pysma_plus-0.1.5/tests/test_ennexos.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)      433 2024-03-27 10:30:58.000000 pysma_plus-0.1.5/tests/test_helpers.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)     4807 2024-04-10 14:26:59.000000 pysma_plus-0.1.5/tests/test_sensor.py
+-rw-rw-r--   0 sven      (1001) sven      (1001)    17687 2024-04-10 19:09:44.000000 pysma_plus-0.1.5/tests/test_webconnect.py
+drwxrwxr-x   0 sven      (1001) sven      (1001)        0 2024-04-14 07:30:36.474540 pysma_plus-0.1.5/tests/testdata/
+-rw-rw-r--   0 sven      (1001) sven      (1001)     6266 2024-04-11 10:21:03.000000 pysma_plus-0.1.5/tests/testdata/EVCharger-measurements.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)      227 2024-04-11 10:20:59.000000 pysma_plus-0.1.5/tests/testdata/EVCharger-measurements.json.source
+-rw-rw-r--   0 sven      (1001) sven      (1001)      831 2024-04-09 19:24:27.000000 pysma_plus-0.1.5/tests/testdata/SunnyHomeManager2.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)      609 2024-04-09 13:01:16.000000 pysma_plus-0.1.5/tests/testdata/TripowerX15-deviceinfo.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)    23412 2024-04-03 12:07:59.000000 pysma_plus-0.1.5/tests/testdata/TripowerX15-measurements.json
+-rw-rw-r--   0 sven      (1001) sven      (1001)   140175 2024-04-09 13:09:32.000000 pysma_plus-0.1.5/tests/testdata/TripowerX15-parameters.json
```

### Comparing `pysma-plus-0.1.4/LICENSE` & `pysma_plus-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.4/PKG-INFO` & `pysma_plus-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.1.4
+Version: 0.1.5
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.1.4
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.1.5
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 kellerza
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pysma-plus-0.1.4/README.md` & `pysma_plus-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.4/pysma_plus.egg-info/PKG-INFO` & `pysma_plus-0.1.5/pysma_plus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pysma-plus
-Version: 0.1.4
+Version: 0.1.5
 Summary: Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices
 Home-page: https://github.com/littleyoda/pysma
-Download-URL: https://github.com/littleyoda/pysma/tarball/0.1.4
+Download-URL: https://github.com/littleyoda/pysma/tarball/0.1.5
 Author: Sven Bursch-Osewold, Johann Kellerman and other
 Author-email: Sven Bursch-Osewold <sb_pysma@bursch.com>, Johann Kellerman <kellerza@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 kellerza
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pysma-plus-0.1.4/pysmaplus/definitions.py` & `pysma_plus-0.1.5/pysmaplus/definitions_webconnect.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 """Sensor definitions for SMA WebConnect library for Python."""
-from .const import (
+from .const_webconnect import (
     DEVICE_INFO,
     ENERGY_METER_VIA_INVERTER,
     GENERIC_SENSORS,
     JMESPATHS_TAG,
     OPTIMIZERS_VIA_INVERTER,
 )
 from .sensor import Sensor
 from .const import Identifier
 
 # Status - Operation
 #: Status of the device
-status = Sensor("6180_08214800", "status", path=JMESPATHS_TAG, l10n_translate=True)
+status = Sensor("6180_08214800", Identifier.status, path=JMESPATHS_TAG, l10n_translate=True)
 #: General operating status
 operating_status_general = Sensor(
     "6180_08412800",
-    "operating_status_general",
+    Identifier.operating_status_genereal,
     path=JMESPATHS_TAG,
     l10n_translate=True,
     enabled=False,
 )
 #: Operating status
 operating_status = Sensor(
     "6180_08412B00",
-    "operating_status",
+    Identifier.operating_status,
     path=JMESPATHS_TAG,
     l10n_translate=True,
     enabled=False,
 )
 # Status - Operation - Inverter
 #: General operating status
 inverter_condition = Sensor(
     "6180_08414C00",
-    "inverter_condition",
+    Identifier.inverter_condition,
     path=JMESPATHS_TAG,
     l10n_translate=True,
     enabled=False,
 )
 #: Inverter Condition
 inverter_system_init = Sensor(
     "6800_08811F00",
-    "inverter_system_init",
+    Identifier.inverter_system_init,
     path=JMESPATHS_TAG,
     l10n_translate=True,
     enabled=False,
 )
 #: Grid connection status
 grid_connection_status = Sensor(
     "6180_0846A700",
-    "grid_connection_status",
+    Identifier.grid_connection_status,
     path=JMESPATHS_TAG,
     l10n_translate=True,
     enabled=False,
 )
 #: Grid relay status
 grid_relay_status = Sensor(
     "6180_08416400",
-    "grid_relay_status",
+    Identifier.grid_relay_status,
     path=JMESPATHS_TAG,
     l10n_translate=True,
     enabled=False,
 )
 
 # DC side - DC measurements PV
 #: Current power generated by the solar panels (A side)
@@ -88,15 +88,15 @@
 #: Current amperage generated by the solar panels (C side)
 pv_current_c = Sensor(
     "6380_40452100_2", Identifier.pv_current_c, unit="A", factor=1000, enabled=False
 )
 #: Isolation Resistance
 pv_isolation_resistance = Sensor(
     "6102_00254F00_0",
-    "pv_isolation_resistance",
+    Identifier.pv_isolation_resistance,
     unit="kOhm",
     factor=1000,
     enabled=False,
 )
 
 # DC Side - Insulation monitoring
 #: Insulation residual current
@@ -163,15 +163,15 @@
 #: Grid Power factor
 grid_power_factor = Sensor(
     "6100_00665900", Identifier.grid_power_factor, unit="", factor=1000, enabled=False
 )
 #: Grid Power factor excitation
 grid_power_factor_excitation = Sensor(
     "6180_08465A00",
-    "grid_power_factor_excitation",
+    Identifier.grid_power_factor_excitation,
     path=JMESPATHS_TAG,
     l10n_translate=True,
     enabled=False,
 )
 
 # AC Side - Grid measurements - Phase Current
 #: Current for phase 1
@@ -273,15 +273,15 @@
 #: Current power consumption measured by energy meter
 metering_current_consumption = Sensor(
     "6100_00543100", Identifier.metering_current_consumption, unit="W", enabled=False
 )
 #: Total power consumption measured by energy meter
 metering_total_consumption = Sensor(
     "6400_00543A00",
-    "metering_total_consumption",
+    Identifier.metering_total_consumption,
     unit="kWh",
     factor=1000,
     enabled=False,
 )
 
 # AC Side - PV generation
 #: Total kWh generated to date
@@ -356,15 +356,15 @@
 #: Temperature battery B
 battery_temp_b = Sensor("6100_40495B00_1", Identifier.battery_temp_b, unit="°C", factor=10)
 #: Temperature battery C
 battery_temp_c = Sensor("6100_40495B00_2", Identifier.battery_temp_c, unit="°C", factor=10)
 #: Battery status operating mode
 battery_status_operating_mode = Sensor(
     "6180_08495E00",
-    "battery_status_operating_mode",
+    Identifier.battery_status_operating_mode,
     path=JMESPATHS_TAG,
     l10n_translate=True,
 )
 
 # Battery (inverter) - Diagnosis
 #: Total battery capacity
 battery_capacity_total = Sensor("6100_00696E00", Identifier.battery_capacity_total, unit="%")
```

### Comparing `pysma-plus-0.1.4/pysmaplus/device.py` & `pysma_plus-0.1.5/pysmaplus/device.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from abc import ABC, abstractmethod
 from typing import Dict
-from .sensor import Sensor
 from .sensor import Sensors
 
 class Device(ABC):
 
     @abstractmethod
     async def get_sensors(self) -> Sensors:
         pass
```

### Comparing `pysma-plus-0.1.4/pysmaplus/helpers.py` & `pysma_plus-0.1.5/pysmaplus/helpers.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.4/pysmaplus/sensor.py` & `pysma_plus-0.1.5/pysmaplus/sensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import copy
 import logging
 from typing import Any, Iterator, List, Optional, Union
 
 import attr
 import jmespath  # type: ignore
 
-from .const import JMESPATH_VAL, JMESPATH_VAL_IDX, JMESPATH_VAL_STR
+from .const_webconnect import JMESPATH_VAL, JMESPATH_VAL_IDX, JMESPATH_VAL_STR
 
 _LOGGER = logging.getLogger(__name__)
 
 
 @attr.s(slots=True)
 class Sensor:
     """pysma sensor."""
@@ -22,14 +22,16 @@
     unit: str = attr.ib(default=None)
     factor: int = attr.ib(default=None)
     path: Union[list, tuple] = attr.ib(default=None)
     enabled: bool = attr.ib(default=True)
     l10n_translate: bool = attr.ib(default=False)
     value: Any = attr.ib(default=None, init=False)
     key_idx: int = attr.ib(default=0, repr=False, init=False)
+    mapper: dict[int, str] = attr.ib(default=None)
+    mapped_value: Any = attr.ib(default=None, init=False)
 
     def __attrs_post_init__(self) -> None:
         """Post init Sensor."""
         key = str(self.key)
         skey = key.split("_")
         if len(skey) > 2 and skey[2].isdigit():
             self.key = f"{skey[0]}_{skey[1]}"
```

### Comparing `pysma-plus-0.1.4/pysmaplus/smaennexos.py` & `pysma_plus-0.1.5/pysmaplus/definitions_ennexos.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,396 +1,255 @@
-import asyncio
-import copy
-import json
-import logging
-from typing import Any, Dict, Optional
-
-
-from aiohttp import ClientSession, ClientTimeout, client_exceptions, hdrs
+from typing import Any, Dict
 from .sensor import Sensor
-from . import definitions
-from .const import (
-    DEFAULT_TIMEOUT,
-)
-from .exceptions import (
-    SmaAuthenticationException,
-    SmaConnectionException,
-    SmaReadException,
-)
-from .sensor import Sensors
-from .device import Device
 from .const import Identifier
 
 
-ennexosSensors = [
-
-    Sensor("Coolsys.Inverter.TmpVal.1", Identifier.temp_a, factor=1, unit="°C"),
-    Sensor("Coolsys.Inverter.TmpVal.2", Identifier.temp_b, factor=1, unit="°C"),
-    Sensor("Coolsys.Inverter.TmpVal.3", Identifier.temp_c, factor=1, unit="°C"),
-    Sensor("DcMs.Amp.1", Identifier.pv_current_a, factor=1, unit="A"),
-    Sensor("DcMs.Amp.2", Identifier.pv_current_b, factor=1, unit="A"),
-    Sensor("DcMs.Amp.3", Identifier.pv_current_c, factor=1, unit="A"),
-    Sensor("DcMs.TotDcEnCntWh.1", None, factor=1, unit=None),
-    Sensor("DcMs.TotDcEnCntWh.2", None, factor=1, unit=None),
-    Sensor("DcMs.TotDcEnCntWh.3", None, factor=1, unit=None),
-    Sensor("DcMs.Vol.1", Identifier.pv_voltage_a, factor=1, unit="V"),
-    Sensor("DcMs.Vol.2", Identifier.pv_voltage_b, factor=1, unit="V"),
-    Sensor("DcMs.Vol.3", Identifier.pv_voltage_c, factor=1, unit="V"),
-    Sensor("DcMs.Watt.1", Identifier.pv_power_a, factor=1, unit="W"),
-    Sensor("DcMs.Watt.2", Identifier.pv_power_b, factor=1, unit="W"),
-    Sensor("DcMs.Watt.3", Identifier.pv_power_c, factor=1, unit="W"),
-    Sensor("GridGuard.Cntry", None, factor=1, unit=None),
-    Sensor("GridMs.A.phsA", Identifier.current_l1, factor=1, unit="A"),
-    Sensor("GridMs.A.phsB", Identifier.current_l2, factor=1, unit="A"),
-    Sensor("GridMs.A.phsC", Identifier.current_l3, factor=1, unit="A"),
-    Sensor("GridMs.GriTyp", None, factor=1, unit=None),
-    Sensor("GridMs.Hz", Identifier.frequency, factor=1, unit="Hz"),
-    Sensor("GridMs.PhV.phsA", Identifier.voltage_l1, factor=1, unit="V"), 
-    Sensor("GridMs.PhV.phsA2B", None, factor=1, unit=None),
-    Sensor("GridMs.PhV.phsB", Identifier.voltage_l2, factor=1, unit="V"),
-    Sensor("GridMs.PhV.phsB2C", None, factor=1, unit=None),
-    Sensor("GridMs.PhV.phsC", Identifier.voltage_l3, factor=1, unit="V"),
-    Sensor("GridMs.PhV.phsC2A", None, factor=1, unit=None),
-    Sensor("GridMs.TotA", Identifier.current_total, factor=1, unit="A"),
-    Sensor("GridMs.TotPFEEI", None, factor=1, unit=None),
-    Sensor("GridMs.TotPFExt", None, factor=1, unit=None),
-    Sensor("GridMs.TotPFPrc", None, factor=1, unit=None),
-    Sensor("GridMs.TotVA", Identifier.grid_apparent_power, factor=1, unit="VA"),
-    Sensor("GridMs.TotVAr", Identifier.grid_reactive_power, factor=1, unit="var"),
-    Sensor("GridMs.TotW", Identifier.grid_power, factor=1, unit="W"),
-    Sensor("GridMs.TotW.Pv", Identifier.pv_power, factor=1, unit="W"),
-    Sensor("GridMs.VA.phsA", Identifier.grid_apparent_power_l1, factor=1, unit="VA"),
-    Sensor("GridMs.VA.phsB", Identifier.grid_apparent_power_l2, factor=1, unit="VA"),
-    Sensor("GridMs.VA.phsC", Identifier.grid_apparent_power_l3, factor=1, unit="VA"),
-    Sensor("GridMs.VAr.phsA", Identifier.grid_reactive_power_l1, factor=1, unit="var"),
-    Sensor("GridMs.VAr.phsB", Identifier.grid_reactive_power_l2, factor=1, unit="var"),
-    Sensor("GridMs.VAr.phsC", Identifier.grid_reactive_power_l3, factor=1, unit="var"),
-    Sensor("GridMs.W.phsA", Identifier.power_l1, factor=1, unit="W"),
-    Sensor("GridMs.W.phsB", Identifier.power_l2, factor=1, unit="W"),
-    Sensor("GridMs.W.phsC", Identifier.power_l3, factor=1, unit="W"),
-    Sensor("InOut.GI1", None, factor=1, unit=None),
-    Sensor("Inverter.VArModCfg.PFCtlVolCfg.Stt", None, factor=1, unit=None),
-    Sensor("Isolation.FltA", Identifier.insulation_residual_current, factor=1000, unit="mA"),
-    Sensor("Isolation.LeakRis", None, factor=1, unit="kOhm"), # TODO "pv_isolation_resistance"
-    Sensor("Metering.TotFeedTms", None, factor=1, unit=None),
-    Sensor("Metering.TotOpTms", None, factor=1, unit=None),
-    Sensor("Metering.TotWhOut", Identifier.total_yield, factor=1000, unit="kWh"),
-    Sensor("Metering.TotWhOut.Pv", Identifier.pv_gen_meter, factor=1000, unit="kWh"),
-    Sensor("Operation.BckStt", None, factor=1, unit=None),
-    Sensor("Operation.DrtStt", None, factor=1, unit=None),
-    Sensor("Operation.Evt.Dsc", None, factor=1, unit=None),
-    Sensor("Operation.Evt.EvtNo", None, factor=1, unit=None),
-    Sensor("Operation.Evt.Msg", None, factor=1, unit=None),
-    Sensor("Operation.EvtCntIstl", None, factor=1, unit=None),
-    Sensor("Operation.EvtCntUsr", None, factor=1, unit=None),
-    Sensor("Operation.GriSwCnt", None, factor=1, unit=None),
-    Sensor("Operation.GriSwStt", None, factor=1, unit=None),
-    Sensor("Operation.Health", None, factor=1, unit=None),
-    Sensor("Operation.HealthStt.Alm", None, factor=1, unit=None),
-    Sensor("Operation.HealthStt.Ok", None, factor=1, unit=None),
-    Sensor("Operation.HealthStt.Wrn", None, factor=1, unit=None),
-    Sensor("Operation.OpStt", None, factor=1, unit=None),
-    Sensor("Operation.PvGriConn", None, factor=1, unit=None),
-    Sensor("Operation.RstrLokStt", None, factor=1, unit=None),
-    Sensor("Operation.RunStt", None, factor=1, unit=None),
-    Sensor("Operation.StandbyStt", None, factor=1, unit=None),
-    Sensor("Operation.VArCtl.VArModAct", None, factor=1, unit=None),
-    Sensor("Operation.VArCtl.VArModStt", None, factor=1, unit=None),
-    Sensor("Operation.WMaxLimSrc", None, factor=1, unit=None),
-    Sensor("Operation.WMinLimSrc", None, factor=1, unit=None),
-    Sensor("PvGen.PvW", None, factor=1, unit=None),
-    Sensor("PvGen.PvWh", None, factor=1, unit=None),
-    Sensor("Spdwr.ComSocA.Stt", None, factor=1, unit=None),
-    Sensor("SunSpecSig.SunSpecTx.1", None, factor=1, unit=None),
-    Sensor("Upd.Stt", None, factor=1, unit=None),
-    Sensor("WebConn.Stt", None, factor=1, unit=None),
-    Sensor("Wl.AcqStt", None, factor=1, unit=None),
-    Sensor("Wl.AntMod", None, factor=1, unit=None),
-    Sensor("Wl.ConnStt", None, factor=1, unit=None),
-    Sensor("Wl.SigPwr", None, factor=1, unit=None),
-    Sensor("Wl.SoftAcsConnStt", None, factor=1, unit=None),
-    Sensor("Setpoint.PlantControl.InOut.GO1", None, factor=1, unit=None)
-]
-_LOGGER = logging.getLogger(__name__)
-class SMAennexos(Device):
-    """Class to connect to the ennexos based SMA inverters. (e.g. Tripower X Devices)"""
-
-    # pylint: disable=too-many-instance-attributes
-    _aio_session: ClientSession
-    _new_session_data: Optional[dict]
-    _url: str
-    _token: str
-    _authorization_header: str
-    _last_parameters: Any
-    _last_measurements: Any
-    _last_device: Any
-
-    def __init__(
-        self,
-        session: ClientSession,
-        url: str,
-        password: Optional[str],
-        group: str,
-    ):
-        """Init SMA connection.
-
-        Args:
-            session (ClientSession): aiohttp client session
-            url (str): Url or IP address of device
-            password (str, optional): Password to use during login.
-            group (str, optional): Username to use during login. 
-
-        """
-        self._url = url.rstrip("/")
-        if not url.startswith("http"):
-            self._url = "http://" + self._url
-        self._new_session_data = {"user": group, "pass": password}
-        self._aio_session = session
-
-
-
-    async def _jsonrequest(
-        self, url: str, parameters: Dict[str, Any], method: str = hdrs.METH_POST
-    ) -> dict:
-        """Request json data for requests.
-
-        Args:
-            url (str): URL to do request to
-            parameters (Dict[str, Any]): parameters
-            method (str): Post or Get-Request
-
-        Raises:
-            SmaConnectionException: Connection to device failed
-            SmaAuthenticationException: Authentication failed
-
-        Returns:
-            dict: json returned by device
-        """
-
-        #_LOGGER.debug("Sending Request to %s: %s", url, parameters)
-
-        try:
-                async with self._aio_session.request(
-                    method,
-                    url,
-                    timeout=ClientTimeout(total=DEFAULT_TIMEOUT),
-                    **parameters
-                ) as res:
-                    if (res.status == 401):
-                        raise SmaAuthenticationException(
-                            f"Token failed!"
-                        )
-                    res = await res.json()
-                   # _LOGGER.debug("Received reply %s", res)
-                    return res
-        except SmaAuthenticationException as e:
-                raise e
-        except (client_exceptions.ContentTypeError, json.decoder.JSONDecodeError):
-            _LOGGER.warning("Request to %s did not return a valid json.", url)
-        except client_exceptions.ServerDisconnectedError as exc:
-            raise SmaConnectionException(
-                f"Server at {self._url} disconnected."
-            ) from exc
-        except (
-            client_exceptions.ClientError,
-            asyncio.exceptions.TimeoutError,
-        ) as exc:
-            raise SmaConnectionException(
-                f"Could not connect to SMA at {self._url}: {exc}"
-            ) from exc
-        return {}
-
-
-    async def new_session(self) -> bool:
-        """Establish a new session.
-
-        Returns:
-            bool: authentication successful
-        """
-        loginurl = self._url + '/api/v1/token'
-        postdata = {'data':{'grant_type': 'password',
-                'username': self._new_session_data["user"],
-                'password': self._new_session_data["pass"],
-                }}
-        ret = await self._jsonrequest(loginurl,postdata)
-        if "access_token" not in ret:
-            raise SmaAuthenticationException(f"Login failed!")
-        self._token = ret["access_token"]
-        self._authorization_header = { "Authorization" : "Bearer " + self._token,
-                                       "Content-Type": "application/json"
-                                       }
-        _LOGGER.debug("Login successfull")
-        return True
-
-    async def _get_parameter(self : str) -> Dict:
-        url = self._url + '/api/v1/parameters/search'
-        postdata = {
-             'data': '{"queryItems":[{"componentId":"IGULD:SELF"}]}',
-             'headers': self._authorization_header
-        }
-        ret = await self._jsonrequest(url, postdata)
-        data = {}
-        if (len(ret) != 1):
-            _LOGGER.warning("Uncommon length of array in parameters request: %d", len(ret))
-
-        for d in ret[0]["values"]:
-            dname = d["channelId"].replace("Parameter.","").replace("[]", "")
-            if "value" in d:
-                v = d["value"]
-                data[dname] = {
-                        "name": dname,
-                        "value": v,
-                        "origname": d["channelId"]
-                    }
-            elif "values" in d:
-                # Split Value-Arrays
-                for idx in range(0, len(d["values"])):
-                    v = d["values"][idx]
-                    idxname = dname + "." + str(idx + 1)
-                    data[idxname] = {
-                            "name": idxname,
-                            "value": v,
-                            "origname": d["channelId"]
-                    }
-            else:
-                # Value current not available // night?
-                # TODO
-                pass
-        return data
-
-    async def _get_livedata(self : str) -> Dict:
-        liveurl = self._url + '/api/v1/measurements/live'
-        postdata = { 
-             'data': '[{"componentId":"IGULD:SELF"}]',
-             'headers': self._authorization_header
-        }
-        ret = await self._jsonrequest(liveurl,postdata)
-        self._last_measurements = ret
-        data = {}
-        for d in ret:
-            dname = d["channelId"].replace("Measurement.","").replace("[]", "")
-            if "value" in d["values"][0]:
-                v = d["values"][0]["value"]
-                if self._isfloat(v):
-                     v = round(v,2)
-                data[dname] = {
-                        "name": dname,
-                        "value": v,
-                        "origname": d["channelId"]
-                    }
-            elif "values" in d["values"][0]:
-                # Split Value-Arrays
-                for idx in range(0, len(d["values"][0]["values"])):
-                    v = d["values"][0]["values"][idx]
-                    if self._isfloat(v):
-                        v = round(v,2)
-                    idxname = dname + "." + str(idx + 1)
-                    data[idxname] = {
-                            "name": idxname,
-                            "value": v,
-                            "origname": d["channelId"]
-                    }
-            else:
-                # Value current not available // night?
-                # TODO
-                pass
-        return data
-    
-
-
-    async def get_sensors(self) -> Sensors:
-        """Get the sensors that are present on the device.
-
-        Returns:
-            Sensors: Sensors object containing Sensor objects
-        """
-        device_sensors = Sensors()
-        ret = await self._get_livedata()
-        _LOGGER.debug("Found Sensors: %s", ret)
-
-        for s in ennexosSensors:
-            if s.name:
-                device_sensors.add(copy.copy(s))
-        return device_sensors
-
-
-    async def close_session(self) -> None:
-        """Close the session login."""
-        # TODO
-        pass
-
-    def _isfloat(self,num):
-        try:
-            float(num)
-            return True
-        except ValueError:
-            return False
-
-
-    async def read(self, sensors: Sensors) -> bool:
-        """Read a set of keys.
-
-        Args:
-            sensors (Sensors): Sensors object containing Sensor objects to read
-
-        Returns:
-            bool: reading was successful
-        """
-        notfound = []
-        data = None
-        try:
-            data = await self._get_livedata()
-        except SmaAuthenticationException as e:
-            # Relogin
-            _LOGGER.debug("Re-login .. Starting new Session")
-            await self.new_session()
-            data = await self._get_livedata()
-
-        for sen in sensors:
-            if sen.enabled:
-                if sen.key in data:
-                    value = data[sen.key]["value"]
-                    if (sen.factor):
-                        value = round(value/sen.factor,4)
-                    sen.value = value
-                    continue
-                notfound.append(f"{sen.name} [{sen.key}]")
-
-        if notfound:
-            _LOGGER.info(
-                "No values for sensors: %s",
-                ",".join(notfound),
-            )
-
-        return True
-
-
-
-    async def device_info(self) -> dict:
-        """Read device info and return the results.
-
-        Returns:
-            dict: dict containing serial, name, type, manufacturer and sw_version
-        """
-        url = self._url + '/api/v1/plants/Plant:1/devices/IGULD:SELF'
-        requestdata = { 
-             'headers': self._authorization_header
-        }
-        dev = await self._jsonrequest(url,requestdata, hdrs.METH_GET)
-        self._last_device = dev
-        self._last_parameters = await self._get_parameter()
-        _LOGGER.debug("Found Device: %s", dev)
-        device_info = {
-            "serial": dev["serial"],
-            "name": dev["product"],
-            "type": dev["name"],
-            "manufacturer": dev["vendor"],
-            "sw_version": dev["firmwareVersion"],
-        }
-        return device_info
-
-    async def get_debug(self) -> Dict:
-        return {
-            "device": self._last_device,
-            "measurements": self._last_measurements,
-            "parameters": self._last_parameters
-        }
+'''
+Data-Source:
+https://www.sma.de/produkte/solar-wechselrichter/sunny-tripower-x
+Technical Information - Parameters and Measured Values STP 12-50 / STP 15-50 / STP 20-50 / STP 25-50 (Sunny Tripower X) with firmware package 03.02.07.R 
+
+
+
+'''
+ennexMapper: Dict[int, str] = {
+    35: "Error",
+    51: "Closed",
+    276: "Instantaneous value",
+    295: "MPP",
+    303: "Off",
+    307: "OK",
+    308: "On",
+    309: "Operation",
+    311: "Open",
+    325: "Phase L1 (phsA)",
+    326: "Phases L1, L2 and L3 (phsABC)",
+    327: "Phase L2 (phsB)",
+    329: "Phase L3 (phsC)",
+    336: "Contact the manufacturer",
+    337: "Contact the installer",
+    338: "Invalid",
+    381: "Stop",
+    402: "Phases L1 and L2 (phsAB)",
+    403: "Phases L1 and L3 (phsAC)",
+    404: "Phases L2 and L3 (phsBC)",
+    433: "Contant voltage",
+    455: "Warning",
+    461: "SMA",
+    887: "No recommended action",
+    1041: "leading / overexcited",
+    1042: "lagging / underexcited",
+    1069: "Reactive power / voltage characteristic curve Q(V)",
+    1070: "Reactive power Q, direct setpoint",
+    1071: "Reactive power const. Q (kVAr)",
+    1072: "Q specified by PV system control",
+    1073: "Reactive power Q(P)",
+    1074: "cos φ, direct setpoint",
+    1075: "cos φ, setpoint via system control",
+    1076: "cos φ(P) characteristic curve",
+    1077: "Active power limitation P (W)",
+    1078: "Active power limitation P (%) of PMAX",
+    1079: "Active power limitation P via system control",
+    1129: "Yes",
+    1130: "No",
+    1264: "Full dynamic grid support",
+    1265: "Limited dynamic grid support",
+    1387: "Reactive power Q, setpoint via analog input",
+    1388: "cos φ, setpoint via analog input",
+    1389: "Reactive power / voltage characteristic curve Q(U) with hysteresis and deadband",
+    1390: "Active power limitation P via analog input",
+    1391: "Active power limitation P via digital inputs",
+    1392: "Errors",
+    1393: "Wait for PV voltage",
+    1394: "Wait for valid AC grid",
+    1395: "DC area",
+    1396: "AC grid",
+    1438: "Automatic",
+    1455: "Emergency stop",
+    1466: "Waiting",
+    1467: "Starting",
+    1468: "MPP search",
+    1469: "Shutdown",
+    1470: "Event message",
+    1471: "Warning/error e-mail OK",
+    1472: "Warning/error e-mail not OK",
+    1473: "System info Parameter.Nameplate.Modele-mail OK",
+    1474: "System info e-mail not OK",
+    1475: "Error e-mail OK",
+    1476: "Error e-mail not OK",
+    1477: "Warning e-mail OK",
+    1478: "Warning e-mail not OK",
+    1479: "Wait after grid interruption",
+    1480: "Wait for electric utility company",
+    1749: "Full Stop",
+    # 2055: "Status digital inlet: DI1",
+    # 2056: "Status digital inlet: DI1, DI2",
+    # 2057: "Status digital inlet: DI1, DI2, DI3",
+    # 2058: "Status digital inlet: DI1, DI2, DI3, DI4",
+    # 2059: "Status digital inlet: DI1, DI2, DI4",
+    # 2060: "Status digital inlet: DI1, DI3",
+    # 2061: "Status digital inlet: DI1, DI3, DI4",
+    # 2062: "Status digital inlet: DI1, DI4",
+    # 2063: "Status digital inlet: DI2",
+    # 2064: "Status digital inlet: DI2, DI3",
+    # 2065: "Status digital inlet: DI2, DI3, DI4",
+    # 2066: "Status digital inlet: DI2, DI4",
+    # 2067: "Status digital inlet: DI3",
+    # 2068: "Status digital inlet: DI3, DI4",
+    # 2069: "Status digital inlet: DI4",
+    2270: "cos φ or Q specification through optimum PV system control",
+    2506: "Values maintained",
+    2507: "Apply fallback values",
+    4354: "Maximum active power export",
+    4405: "Maximum active power WMax",
+    4406: "Maximum reactive power VArMax",
+    4433: "Zero at dead band boundary",
+    4434: "Zero at origin (ZerAtZer)",
+    4443: "Current power",
+    4444: "Potential power",
+    4450: "Q limitation",
+    4562: "cos φ(V) charac. curve",
+    4520: "Mean value of the phase voltages",
+    4521: "Maximum phase voltage",
+    4718: "Boost Charging", # EV-Charger
+    4950: "Smart Chargig", # EV-Charger
+    5169: "Station locked", # EV-Charger
+    5249: "Potential power with characteristic curve break",
+
+
+
+    # DevClass
+    8001: "Solar Inveters",
+    8008: "SMAEVCharger",
+
+    9489: "STP-20-50",
+    9491: "STP-15-50",
+    9492: "STP-12-50",
+    9484: "EVC22-3AC-10",
+
+
+    200111: "Not connected", # EV-Charger
+    200112: "Sleep Mode", # EV-Charger
+    200113: "Active Mode", # EV-Charger
+
+    16777213: "Information not available",
+}
+
+ennexosSensorProfiles = {
+    "Sunny Tripower X ": [
+        Sensor("Coolsys.Inverter.TmpVal.1", Identifier.temp_a, factor=1, unit="°C"),
+        Sensor("Coolsys.Inverter.TmpVal.2", Identifier.temp_b, factor=1, unit="°C"),
+        Sensor("Coolsys.Inverter.TmpVal.3", Identifier.temp_c, factor=1, unit="°C"),
+        Sensor("DcMs.Amp.1", Identifier.pv_current_a, factor=1, unit="A"),
+        Sensor("DcMs.Amp.2", Identifier.pv_current_b, factor=1, unit="A"),
+        Sensor("DcMs.Amp.3", Identifier.pv_current_c, factor=1, unit="A"),
+        Sensor("DcMs.TotDcEnCntWh.1", None, factor=1, unit=None), # Energy released by string [A]
+        Sensor("DcMs.TotDcEnCntWh.2", None, factor=1, unit=None),
+        Sensor("DcMs.TotDcEnCntWh.3", None, factor=1, unit=None),
+        Sensor("DcMs.Vol.1", Identifier.pv_voltage_a, factor=1, unit="V"),
+        Sensor("DcMs.Vol.2", Identifier.pv_voltage_b, factor=1, unit="V"),
+        Sensor("DcMs.Vol.3", Identifier.pv_voltage_c, factor=1, unit="V"),
+        Sensor("DcMs.Watt.1", Identifier.pv_power_a, factor=1, unit="W"),
+        Sensor("DcMs.Watt.2", Identifier.pv_power_b, factor=1, unit="W"),
+        Sensor("DcMs.Watt.3", Identifier.pv_power_c, factor=1, unit="W"),
+        Sensor("GridGuard.Cntry", None, factor=1, unit=None), # Country standard set
+        Sensor("GridMs.A.phsA", Identifier.current_l1, factor=1, unit="A"),
+        Sensor("GridMs.A.phsB", Identifier.current_l2, factor=1, unit="A"),
+        Sensor("GridMs.A.phsC", Identifier.current_l3, factor=1, unit="A"),
+        Sensor("GridMs.GriTyp", None, factor=1, unit=None), # Measurement.GridMs.GriTyp
+        Sensor("GridMs.Hz", Identifier.frequency, factor=1, unit="Hz"),
+        Sensor("GridMs.PhV.phsA", Identifier.voltage_l1, factor=1, unit="V"),
+        Sensor("GridMs.PhV.phsA2B", None, factor=1, unit=None), # Grid voltage phase L1 against L2
+        Sensor("GridMs.PhV.phsB", Identifier.voltage_l2, factor=1, unit="V"),
+        Sensor("GridMs.PhV.phsB2C", None, factor=1, unit=None), # Grid voltage phase L2 against L3
+        Sensor("GridMs.PhV.phsC", Identifier.voltage_l3, factor=1, unit="V"),
+        Sensor("GridMs.PhV.phsC2A", None, factor=1, unit=None), # Grid voltage phase L3 against L1
+        Sensor("GridMs.TotA", Identifier.current_total, factor=1, unit="A"),
+        Sensor("GridMs.TotPFEEI", None, factor=1, unit=None),  # EEI displacement power factor
+        Sensor("GridMs.TotPFExt", None, factor=1, unit=None), # Excitation type of cos φ
+        Sensor("GridMs.TotPFPrc", None, factor=1, unit=None), # Displacement power factor
+        Sensor("GridMs.TotVA", Identifier.grid_apparent_power, factor=1, unit="VA"),
+        Sensor("GridMs.TotVAr", Identifier.grid_reactive_power, factor=1, unit="var"),
+        Sensor("GridMs.TotW", Identifier.grid_power, factor=1, unit="W"),
+        Sensor("GridMs.TotW.Pv", Identifier.pv_power, factor=1, unit="W"),
+        Sensor("GridMs.VA.phsA", Identifier.grid_apparent_power_l1, factor=1, unit="VA"),
+        Sensor("GridMs.VA.phsB", Identifier.grid_apparent_power_l2, factor=1, unit="VA"),
+        Sensor("GridMs.VA.phsC", Identifier.grid_apparent_power_l3, factor=1, unit="VA"),
+        Sensor("GridMs.VAr.phsA", Identifier.grid_reactive_power_l1, factor=1, unit="var"),
+        Sensor("GridMs.VAr.phsB", Identifier.grid_reactive_power_l2, factor=1, unit="var"),
+        Sensor("GridMs.VAr.phsC", Identifier.grid_reactive_power_l3, factor=1, unit="var"),
+        Sensor("GridMs.W.phsA", Identifier.power_l1, factor=1, unit="W"),
+        Sensor("GridMs.W.phsB", Identifier.power_l2, factor=1, unit="W"),
+        Sensor("GridMs.W.phsC", Identifier.power_l3, factor=1, unit="W"),
+        Sensor("InOut.GI1", None, factor=1, unit=None), # Digital group input
+        Sensor("Inverter.VArModCfg.PFCtlVolCfg.Stt", None, factor=1, unit=None),
+        Sensor("Isolation.FltA", Identifier.insulation_residual_current, factor=1000, unit="mA"),
+        Sensor("Isolation.LeakRis", None, factor=1, unit="kOhm"), # TODO "pv_isolation_resistance"
+        Sensor("Metering.TotFeedTms", None, factor=1, unit=None), 
+        Sensor("Metering.TotOpTms", None, factor=1, unit=None),
+        Sensor("Metering.TotWhOut", Identifier.total_yield, factor=1000, unit="kWh"),
+        Sensor("Metering.TotWhOut.Pv", Identifier.pv_gen_meter, factor=1000, unit="kWh"),
+        Sensor("Operation.BckStt", None, factor=1, unit=None),
+        Sensor("Operation.DrtStt", None, factor=1, unit=None),
+        Sensor("Operation.Evt.Dsc", None, factor=1, unit=None),
+        Sensor("Operation.Evt.EvtNo", None, factor=1, unit=None),
+        Sensor("Operation.Evt.Msg", None, factor=1, unit=None),
+        Sensor("Operation.EvtCntIstl", None, factor=1, unit=None),
+        Sensor("Operation.EvtCntUsr", None, factor=1, unit=None),
+        Sensor("Operation.GriSwCnt", None, factor=1, unit=None),
+        Sensor("Operation.GriSwStt", None, factor=1, unit=None),
+        Sensor("Operation.Health", Identifier.status, factor=1, unit=None, mapper=ennexMapper),
+        Sensor("Operation.HealthStt.Alm", None, factor=1, unit=None),
+        Sensor("Operation.HealthStt.Ok", None, factor=1, unit=None),
+        Sensor("Operation.HealthStt.Wrn", None, factor=1, unit=None),
+        Sensor("Operation.OpStt", None, factor=1, unit=None),
+        Sensor("Operation.PvGriConn", None, factor=1, unit=None),
+        Sensor("Operation.RstrLokStt", None, factor=1, unit=None),
+        Sensor("Operation.RunStt", None, factor=1, unit=None),
+        Sensor("Operation.StandbyStt", None, factor=1, unit=None),
+        Sensor("Operation.VArCtl.VArModAct", None, factor=1, unit=None),
+        Sensor("Operation.VArCtl.VArModStt", None, factor=1, unit=None),
+        Sensor("Operation.WMaxLimSrc", None, factor=1, unit=None),
+        Sensor("Operation.WMinLimSrc", None, factor=1, unit=None),
+        Sensor("PvGen.PvW", None, factor=1, unit=None), #  PV generation power
+        Sensor("PvGen.PvWh", None, factor=1, unit=None), # Meter count and PV gen. meter
+        Sensor("Spdwr.ComSocA.Stt", None, factor=1, unit=None), # Speedwire connection status of SMACOM A
+        Sensor("SunSpecSig.SunSpecTx.1", None, factor=1, unit=None), #SunSpec life sign [1]
+        Sensor("Upd.Stt", None, factor=1, unit=None),
+        Sensor("WebConn.Stt", None, factor=1, unit=None), #  Status of the Webconnect functionality
+        Sensor("Wl.AcqStt", None, factor=1, unit=None), # Status of WiFi scan
+        Sensor("Wl.AntMod", None, factor=1, unit=None), #  WiFi antenna type
+        Sensor("Wl.ConnStt", None, factor=1, unit=None), # WiFi connection status
+        Sensor("Wl.SigPwr", None, factor=1, unit=None), # Signal strength of the selected network
+        Sensor("Wl.SoftAcsConnStt", None, factor=1, unit=None), #Soft Access Point status
+        Sensor("Setpoint.PlantControl.InOut.GO1", None, factor=1, unit=None)
+    ],
+    "SMA EV Charger ": [
+        Sensor("ChaSess.WhIn", None, factor=1, unit=None), # charging_session_energy
+        Sensor("Chrg.ModSw", None, factor=1, unit=None, mapper=ennexMapper), # position_of_rotary_switch 4950 or 4718
+        Sensor("GridMs.A.phsA", Identifier.current_l1, factor=1, unit="A"), #Netzstrom Phase L1
+        Sensor("GridMs.A.phsB", Identifier.current_l2, factor=1, unit="A"),
+        Sensor("GridMs.A.phsC", Identifier.current_l3, factor=1, unit="A"),
+        Sensor("GridMs.Hz", Identifier.frequency, factor=1, unit="Hz"),
+        Sensor("GridMs.PhV.phsA", Identifier.voltage_l1, factor=1, unit="V"),#Netzspannung Phase L1
+        Sensor("GridMs.PhV.phsB", Identifier.voltage_l2, factor=1, unit="V"),
+        Sensor("GridMs.PhV.phsC", Identifier.voltage_l3, factor=1, unit="V"),
+        Sensor("GridMs.TotPF", None, factor=1, unit=None),
+        Sensor("GridMs.TotVA", Identifier.grid_apparent_power, factor=1, unit="VA"),
+        Sensor("GridMs.TotVAr", Identifier.grid_reactive_power, factor=1, unit="var"),
+        Sensor("InOut.GI1", None, factor=1, unit=None),
+        Sensor("Metering.GridMs.TotWIn", Identifier.metering_power_absorbed, factor=1, unit="W"), #
+        Sensor("Metering.GridMs.TotWIn.ChaSta", None, factor=1, unit=None), # same as Metering.GridMs.TotWIn
+        Sensor("Metering.GridMs.TotWhIn", Identifier.metering_total_absorbed, factor=1, unit="Wh"), # charging_station_meter_reading
+        Sensor("Metering.GridMs.TotWhIn.ChaSta", None, factor=1, unit=None), # same as Metering.GridMs.TotWhIn 
+        Sensor("Operation.EVeh.ChaStt", Identifier.operating_status, factor=1, unit=None, mapper=ennexMapper), # charging_session_status
+        Sensor("Operation.EVeh.Health", Identifier.status, factor=1, unit=None, mapper=ennexMapper), 
+        Sensor("Operation.Evt.Msg", None, factor=1, unit=None),
+        Sensor("Operation.Health", None, factor=1, unit=None), # same as EVeh.Health?
+        Sensor("Operation.WMaxLimNom", None, factor=1, unit=None),
+        Sensor("Operation.WMaxLimSrc", None, factor=1, unit=None),
+        Sensor("Wl.AcqStt", None, factor=1, unit=None),
+        Sensor("Wl.ConnStt", None, factor=1, unit=None),
+        Sensor("Wl.SigPwr", None, factor=1, unit=None),
+        Sensor("Wl.SoftAcsConnStt", None, factor=1, unit=None),
+    ]
+}
```

### Comparing `pysma-plus-0.1.4/pysmaplus/smaspeedwireem.py` & `pysma_plus-0.1.5/pysmaplus/device_em.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 import base64
 import socket
 import struct
-import asyncio
 import copy
 import logging
-import binascii
-from typing import Any, Dict, Optional
+from typing import Any, Dict
 import datetime
 
 # https://www.unifox.at/software/sma-em-daemon/
 # https://cdn.sma.de/fileadmin/content/www.developer.sma.de/docs/EMETER-Protokoll-TI-en-10.pdf?v=1699276024
 
 
 from .sensor import Sensor
 from .const import Identifier
 
 from .exceptions import (
     SmaConnectionException,
     SmaReadException,
 )
-from .helpers import version_int_to_string
 from .sensor import Sensors
 from .device import Device
 
 obis2sensor= [
     Sensor("1:4:0", Identifier.metering_power_absorbed, factor=10, unit="W"), # p consume
     Sensor("1:8:0", Identifier.metering_total_absorbed, factor=3600000, unit="kWh"),
     Sensor("2:4:0", Identifier.metering_power_supplied, factor=10, unit="W"), # p supply
@@ -109,22 +106,14 @@
             url (str): Url or IP address of device
             password (str, optional): Password to use during login.
             group (str, optional): Username to use during login. 
 
         """
         pass
 
-
-
-    async def run(self):
-        while True:
-            await watch(self._q._connection)
-            msg = self._q.receive()
-            print(msg)
-
     async def new_session(self) -> bool:
         """Establish a new session.
 
         Returns:
             bool: authentication successful
         """
         MCAST_GRP = '239.12.255.254'
@@ -136,15 +125,15 @@
         self._sock.settimeout(5)
         self._sock.bind(("", MCAST_PORT))
         try:
             mreq = struct.pack("4s4s", socket.inet_aton(MCAST_GRP), socket.inet_aton(IPBIND))
             self._sock.setsockopt(socket.IPPROTO_IP, socket.IP_ADD_MEMBERSHIP, mreq)
         except BaseException as exc:
             raise SmaConnectionException(
-                f"Could not start multicast"
+                "Could not start multicast"
             ) from exc
 
 
         return True
 
 
     async def get_sensors(self) -> Sensors:
@@ -160,43 +149,44 @@
                 device_sensors.add(copy.copy(s)) 
 
         return device_sensors
 
 
     async def close_session(self) -> None:
         """Close the session login."""
-        # TODO
-        pass
+        self._sock.close()
 
+    def _recv(self):
+        return self._sock.recv(608)
 
-    def getData(self):
+    def _getData(self):
         """
 
         Hack:
             If the function is called less frequently than the device supplies data,
             the UDP packets will be stored in the buffer.
             If the read instruction (sock.recv) takes only milliseconds, I assume that
             the data came from the buffer and discard it. Otherwise outdated values would
             be used.
             One of my most ugly hacks.
 
         """
         data = None
-        tries = 4
+        tries = 50
         try:
             while tries > 0:
+                tries -= 1
                 a = datetime.datetime.now()
-                self._last_packet = self._sock.recv(608)
+                self._last_packet = self._recv()
                 data=self._decode(self._last_packet)
                 b = datetime.datetime.now()
                 if data and (b-a).total_seconds() < 0.1:
                     continue
                 if data:
                     break
-                tries -= 1
         except TimeoutError as e:
             raise SmaConnectionException("No speedwire packet received!") from e
         if not data:
             raise SmaReadException("No usable data received!")
         return data
 
     async def read(self, sensors: Sensors) -> bool:
@@ -205,15 +195,15 @@
         Args:
             sensors (Sensors): Sensors object containing Sensor objects to read
 
         Returns:
             bool: reading was successful
         """
         notfound = []
-        data = self.getData()
+        data = self._getData()
             
         for sensor in sensors:
           if (sensor.key in data):
               value = data[sensor.key]
               if (sensor.factor):
                   value /= sensor.factor
               sensor.value = value
@@ -231,16 +221,15 @@
 
     async def device_info(self) -> dict:
         """Read device info and return the results.
 
         Returns:
             dict: dict containing serial, name, type, manufacturer and sw_version
         """
-        notfound = []
-        data = self.getData()
+        data = self._getData()
 
         device_info = {
             "serial": data["serial"],
             "name": data["device"],
             "type": data["susyid"],
             "manufacturer": "SMA",
             "sw_version": data["sw_version"],
```

### Comparing `pysma-plus-0.1.4/pysmaplus/smawebconnect.py` & `pysma_plus-0.1.5/pysmaplus/device_webconnect.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,23 @@
+"""SMA WebConnect library for Python.
+
+See: http://www.sma.de/en/products/monitoring-control/webconnect.html
+
+Source: http://www.github.com/kellerza/pysma
+"""
 import asyncio
 import copy
 import json
 import logging
 from typing import Any, Dict, Optional
 
 import jmespath  # type: ignore
 from aiohttp import ClientSession, ClientTimeout, client_exceptions, hdrs
-from .sensor import Sensor
-from . import definitions
-from .const import (
+from . import definitions_webconnect
+from .const_webconnect import (
     DEFAULT_LANG,
     DEFAULT_TIMEOUT,
     DEVICE_INFO,
     ENERGY_METER_VIA_INVERTER,
     FALLBACK_DEVICE_INFO,
     GENERIC_SENSORS,
     OPTIMIZERS_VIA_INVERTER,
@@ -87,15 +92,15 @@
             self._url = "http://" + self._url
         self._aio_session = session
         self._sid = None
         self._uid = uid
         self._lang = lang
         self._l10n = None
         self._devclass = None
-        self._device_info_sensors = Sensors(definitions.sensor_map[DEVICE_INFO])
+        self._device_info_sensors = Sensors(definitions_webconnect.sensor_map[DEVICE_INFO])
 
     async def _request_json(
         self, method: str, url: str, **kwargs: Dict[str, Any]
     ) -> dict:
         """Request json data for requests.
 
         Args:
@@ -401,15 +406,15 @@
         """
         all_sensors = await self._read_all_sensors()
         sensor_keys = all_sensors.keys()
         device_sensors = Sensors()
 
         _LOGGER.debug("Matching generic sensors")
 
-        for sensor in definitions.sensor_map[GENERIC_SENSORS]:
+        for sensor in definitions_webconnect.sensor_map[GENERIC_SENSORS]:
             if sensor.key in sensor_keys:
                 if isinstance(all_sensors[sensor.key], list):
                     # SB1.5 multi value
                     val_len = len(all_sensors[sensor.key])
                 elif "val" in all_sensors[sensor.key]:
                     # SB1.5 single value
                     val_len = 1
@@ -426,44 +431,44 @@
                         sensor.key,
                         sensor.key_idx,
                     )
                     device_sensors.add(sensor)
 
         _LOGGER.debug("Checking if Energy Meter is present...")
         # Detect and add Energy Meter sensors
-        em_sensor = copy.copy(definitions.energy_meter)
+        em_sensor = copy.copy(definitions_webconnect.energy_meter)
         em_sensor.extract_value(all_sensors)
 
         if em_sensor.value:
             _LOGGER.debug(
                 "Energy Meter with serial %s detected. Adding extra sensors.",
                 em_sensor.value,
             )
             device_sensors.add(
                 [
                     sensor
-                    for sensor in definitions.sensor_map[ENERGY_METER_VIA_INVERTER]
+                    for sensor in definitions_webconnect.sensor_map[ENERGY_METER_VIA_INVERTER]
                     if sensor not in device_sensors
                 ]
             )
 
         _LOGGER.debug("Finding connected optimizers...")
         # Detect and add Optimizer Sensors
-        optimizers = all_sensors.get(definitions.optimizer_serial.key)
+        optimizers = all_sensors.get(definitions_webconnect.optimizer_serial.key)
         if optimizers:
             serials = optimizers.popitem()[1]
 
             for idx, serial in enumerate(serials or []):
                 if serial["val"]:
                     _LOGGER.debug(
                         "Optimizer %s with serial %s detected. Adding extra sensors.",
                         idx,
                         serial,
                     )
-                    for sensor_definition in definitions.sensor_map[
+                    for sensor_definition in definitions_webconnect.sensor_map[
                         OPTIMIZERS_VIA_INVERTER
                     ]:
                         new_sensor = copy.copy(sensor_definition)
                         new_sensor.key_idx = idx
                         new_sensor.name = f"{sensor_definition.name}_{idx}"
                         device_sensors.add(new_sensor)
```

### Comparing `pysma-plus-0.1.4/setup.py` & `pysma_plus-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 """pysma library setup."""
 from pathlib import Path
 
 from setuptools import setup
 
-VERSION = "0.1.4"
+VERSION = "0.1.5"
 URL = "https://github.com/littleyoda/pysma"
 
 setup(
     name="pysma-plus",
     version=VERSION,
     description="Library to interface SMA Devices via WebConnect, EnnexOS and Energy Meter Devices",
     long_description=Path("README.md").read_text(),
```

### Comparing `pysma-plus-0.1.4/tests/__init__.py` & `pysma_plus-0.1.5/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pysma-plus-0.1.4/tests/test_definitions.py` & `pysma_plus-0.1.5/tests/test_definitions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Test pysma const file."""
 
-import pysma.definitions
+import pysma.definitions_webconnect
 from pysma.sensor import Sensor
 
 
 def test_duplicate_sensors():
     """Test if defined sensors have unique key and name."""
-    variables = vars(pysma.definitions)
+    variables = vars(pysma.definitions_webconnect)
     found_keys = []
     found_names = []
     for value in variables.values():
         if isinstance(value, Sensor):
             found_key = f"{value.key}_{value.key_idx}"
             found_name = value.name
 
@@ -19,10 +19,10 @@
 
             assert found_name not in found_names
             found_names.append(found_name)
 
 
 def test_sensor_map():
     """Test if all map entries only contain unique items."""
-    for sensor_map in pysma.definitions.sensor_map.values():
+    for sensor_map in pysma.definitions_webconnect.sensor_map.values():
         unique_items = list({f"{s.key}_{s.key_idx}": s for s in sensor_map}.values())
         assert unique_items == sensor_map
```

### Comparing `pysma-plus-0.1.4/tests/test_init.py` & `pysma_plus-0.1.5/tests/test_webconnect.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 import re
 from unittest.mock import patch
 
 import aiohttp
 import pytest
 
 from pysma import SMA
-from pysma.definitions import device_type as device_type_sensor
+from pysma.definitions_webconnect import device_type as device_type_sensor
 from pysma.exceptions import (
     SmaAuthenticationException,
     SmaConnectionException,
     SmaReadException,
 )
 from pysma.sensor import Sensors
+from pysma.device_webconnect import SMAwebconnect
 
 from . import MOCK_DEVICE, MOCK_L10N, SMA_TESTDATA, mock_aioresponse  # noqa: F401
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class Test_SMA_class:
@@ -40,61 +41,61 @@
     async def test_request_json_connect_error(self, mock_aioresponse):  # noqa: F811
         """Test request_json with a SmaConnectionException."""
         mock_aioresponse.get(
             f"{self.base_url}/dummy-url",
             exception=aiohttp.client_exceptions.ClientConnectionError("mocked error"),
         )
         session = aiohttp.ClientSession()
-        sma = SMA(session, self.host, "pass")
+        sma = SMAwebconnect(session, self.host, "pass")
         with pytest.raises(SmaConnectionException):
             await sma._get_json("/dummy-url")
 
     async def test_request_json_server_disconnect_error(
         self, mock_aioresponse  # noqa: F811
     ):
         """Test request_json with a SmaConnectionException from ServerDisconnectedError."""
         mock_aioresponse.get(
             f"{self.base_url}/dummy-url",
             exception=aiohttp.client_exceptions.ServerDisconnectedError("mocked error"),
             repeat=True,
         )
         session = aiohttp.ClientSession()
-        sma = SMA(session, self.host, "pass")
+        sma = SMAwebconnect(session, self.host, "pass")
         with pytest.raises(SmaConnectionException):
             await sma._get_json("/dummy-url")
 
     async def test_timeout_error(self, mock_aioresponse):  # noqa: F811
         """Test request_json with a SmaConnectionException from TimeoutError."""
         mock_aioresponse.get(
             f"{self.base_url}/dummy-url",
             exception=asyncio.TimeoutError("mocked error"),
             repeat=True,
         )
         session = aiohttp.ClientSession()
-        sma = SMA(session, self.host, "pass")
+        sma = SMAwebconnect(session, self.host, "pass")
         with pytest.raises(SmaConnectionException):
             await sma._get_json("/dummy-url")
 
-    @patch("pysma._LOGGER.warning")
+    @patch("pysma.device_webconnect._LOGGER.warning")
     async def test_request_json_invalid_json(
         self, mock_warn, mock_aioresponse  # noqa: F811
     ):
         """Test request_json with invalid json."""
         mock_aioresponse.get(
             f"{self.base_url}/dummy-url",
             body="THIS IS NOT A VALID JSON",
         )
         session = aiohttp.ClientSession()
-        sma = SMA(session, self.host, "pass")
+        sma = SMAwebconnect(session, self.host, "pass")
         json = await sma._get_json("/dummy-url")
         assert isinstance(json, dict)
         assert json == {}
         assert mock_warn.call_count == 1
 
-    @patch("pysma._LOGGER.warning")
+    @patch("pysma.device_webconnect._LOGGER.warning")
     async def test_read_no_password(self, mock_warn, mock_aioresponse):  # noqa: F811
         """Test read_body without password."""
         mock_aioresponse.post(
             f"{self.base_url}/dyn/getDashValues.json",
             payload={
                 "result": {
                     "0199-xxxxx385": {
@@ -107,49 +108,49 @@
                             ]
                         },
                     }
                 }
             },
         )
         session = aiohttp.ClientSession()
-        sma = SMA(session, self.host)
+        sma = SMAwebconnect(session, self.host)
         sensors = Sensors(device_type_sensor)
         assert await sma.read(sensors)
         assert sensors["6800_08822000"].value == "Sunny Boy 3.6"
         assert mock_warn.call_count == 0
 
-    @patch("pysma._LOGGER.warning")
+    @patch("pysma.device_webconnect._LOGGER.warning")
     async def test_read_body_error(self, mock_warn, mock_aioresponse):  # noqa: F811
         """Test read_body with SmaReadException."""
         mock_aioresponse.post(
             f"{self.base_url}/dyn/getValues.json?sid=ABCD", payload={"err": 401}
         )
         session = aiohttp.ClientSession()
-        sma = SMA(session, self.host, "pass")
+        sma = SMAwebconnect(session, self.host, "pass")
         sma._sid = "ABCD"
         with pytest.raises(SmaReadException):
             await sma._read_body("/dyn/getValues.json", payload={"dummy": "payload"})
         assert mock_warn.call_count == 1
 
-    @patch("pysma._LOGGER.warning")
+    @patch("pysma.device_webconnect._LOGGER.warning")
     async def test_read_body_unexpected(
         self, mock_warn, mock_aioresponse  # noqa: F811
     ):
         """Test read_body with unexpected body."""
         mock_aioresponse.post(
             f"{self.base_url}/dyn/getValues.json?sid=ABCD",
             payload={
                 "result": {
                     "0199-xxxxx385": {},
                     "0199-yyyyy385": {},
                 }
             },
         )
         session = aiohttp.ClientSession()
-        sma = SMA(session, self.host, "pass")
+        sma = SMAwebconnect(session, self.host, "pass")
         sma._sid = "ABCD"
         result_body = await sma._read_body(
             "/dyn/getValues.json", payload={"dummy": "payload"}
         )
         assert result_body == {}
         assert mock_warn.call_count == 1
 
@@ -174,15 +175,15 @@
                         },
                     }
                 }
             },
         )
 
         session = aiohttp.ClientSession()
-        sma = SMA(session, self.host)
+        sma = SMAwebconnect(session, self.host)
         read_dash_logger = await sma.read_dash_logger()
         assert read_dash_logger == {
             "7000": {
                 "1": [
                     {"t": 1622569500, "v": 4565239},
                     {"t": 1622569800, "v": 4565249},
                 ]
@@ -209,15 +210,15 @@
                         {"t": 1622584800, "v": 4565355},
                     ]
                 }
             },
         )
 
         session = aiohttp.ClientSession()
-        sma = SMA(session, self.host, "pass")
+        sma = SMAwebconnect(session, self.host, "pass")
         read_logger = await sma.read_logger(28704, 1622592000, 1622491200)
         assert read_logger == [
             {"t": 1622498400, "v": 4542749},
             {"t": 1622584800, "v": 4565355},
         ]
 
     async def test_read_logger_error(self, mock_aioresponse):  # noqa: F811
@@ -227,55 +228,55 @@
         )
         mock_aioresponse.post(
             f"{self.base_url}/dyn/getLogger.json?sid=ABCD",
             payload={"result": {"0199-xxxxx385": "NOT A LIST"}},
         )
 
         session = aiohttp.ClientSession()
-        sma = SMA(session, self.host, "pass")
+        sma = SMAwebconnect(session, self.host, "pass")
 
         with pytest.raises(SmaReadException):
             await sma.read_logger(28704, 1622592000, 1622491200)
 
-    @patch("pysma._LOGGER.warning")
+    @patch("pysma.device_webconnect._LOGGER.warning")
     async def test_new_session(self, mock_warn, mock_aioresponse):  # noqa: F811
         """Test new_session."""
         mock_aioresponse.post(
             f"{self.base_url}/dyn/login.json", payload={"result": {"sid": "ABCD"}}
         )
         session = aiohttp.ClientSession()
-        sma = SMA(session, self.host, "extralongpassword")
+        sma = SMAwebconnect(session, self.host, "extralongpassword")
         assert await sma.new_session()
 
         assert mock_warn.call_count == 1
         await sma.close_session()
         await sma.close_session()
 
         assert mock_warn.call_count == 1
 
     async def test_new_session_invalid_group(self, mock_aioresponse):  # noqa: F811
         """Test new_session with invalid group."""
         session = aiohttp.ClientSession()
         with pytest.raises(KeyError):
-            SMA(session, self.host, "pass", "invalid-group")
+            SMAwebconnect(session, self.host, "pass", "invalid-group")
 
     async def test_new_session_fail(self, mock_aioresponse):  # noqa: F811
         """Test new_session with empty result."""
         mock_aioresponse.post(f"{self.base_url}/dyn/login.json", payload={"result": {}})
 
         session = aiohttp.ClientSession()
-        sma = SMA(session, self.host, "pass")
+        sma = SMAwebconnect(session, self.host, "pass")
         with pytest.raises(SmaAuthenticationException):
             await sma.new_session()
 
-    @patch("pysma._LOGGER.error")
+    @patch("pysma.device_webconnect._LOGGER.error")
     async def test_new_session_error(self, mock_error, mock_aioresponse):  # noqa: F811
         """Test new_session with error."""
         session = aiohttp.ClientSession()
-        sma = SMA(session, self.host, "pass")
+        sma = SMAwebconnect(session, self.host, "pass")
 
         mock_aioresponse.post(
             f"{self.base_url}/dyn/login.json", payload={"err": "dummy-error"}
         )
         with pytest.raises(SmaAuthenticationException):
             await sma.new_session()
         assert mock_error.call_count == 1
@@ -328,15 +329,15 @@
                         },
                         "6800_10821E00": {"1": [{"val": MOCK_DEVICE["name"]}]},
                     }
                 }
             },
         )
         session = aiohttp.ClientSession()
-        sma = SMA(session, self.host, "pass")
+        sma = SMAwebconnect(session, self.host, "pass")
         result = await sma.device_info()
         assert result
         assert result == MOCK_DEVICE
 
     async def test_device_info_fallback(self, mock_aioresponse):  # noqa: F811
         """Test device_info fallback."""
         mock_aioresponse.post(
@@ -352,15 +353,15 @@
                         },
                         "6800_10821E00": {"1": [{"val": MOCK_DEVICE["name"]}]},
                     }
                 }
             },
         )
         session = aiohttp.ClientSession()
-        sma = SMA(session, self.host, "pass")
+        sma = SMAwebconnect(session, self.host, "pass")
         assert await sma.new_session()
         result = await sma.device_info()
         assert result
         assert result["manufacturer"] == "SMA"
         assert result["name"] == MOCK_DEVICE["name"]
         assert result["type"] == ""
         assert result["serial"] == "9999999999"
@@ -372,15 +373,15 @@
             f"{self.base_url}/dyn/login.json", payload={"result": {"sid": "ABCD"}}
         )
         mock_aioresponse.post(
             f"{self.base_url}/dyn/getValues.json?sid=ABCD",
             payload={},
         )
         session = aiohttp.ClientSession()
-        sma = SMA(session, self.host, "pass")
+        sma = SMAwebconnect(session, self.host, "pass")
         assert await sma.new_session()
         with pytest.raises(SmaReadException):
             await sma.device_info()
 
     @pytest.mark.parametrize(
         "get_all_onl_values,get_all_param_values,number_of_sensors", SMA_TESTDATA
     )
@@ -427,44 +428,44 @@
                     }
                 }
             },
             repeat=True,
         )
 
         session = aiohttp.ClientSession()
-        sma = SMA(session, self.host, "pass")
+        sma = SMAwebconnect(session, self.host, "pass")
         assert len(await sma.get_sensors()) == number_of_sensors
 
     async def test_post_json(self):
         session = aiohttp.ClientSession()
-        sma = SMA(session, self.host, "pass")
+        sma = SMAwebconnect(session, self.host, "pass")
 
-        with patch("pysma.SMA._request_json") as mock_request_json:
+        with patch("pysma.SMAwebconnect._request_json") as mock_request_json:
             await sma._post_json("dummy_url")
             mock_request_json.assert_called_once_with(
                 "POST",
                 "dummy_url",
                 data="{}",
                 headers={"content-type": "application/json"},
             )
 
-        with patch("pysma.SMA._request_json") as mock_request_json:
+        with patch("pysma.SMAwebconnect._request_json") as mock_request_json:
             await sma._post_json("dummy_url", {"data": "dummy"})
             mock_request_json.assert_called_once_with(
                 "POST",
                 "dummy_url",
                 data='{"data": "dummy"}',
                 headers={"content-type": "application/json"},
             )
 
-    @patch("pysma._LOGGER.warning")
+    @patch("pysma.device_webconnect._LOGGER.warning")
     async def test_unsupported_lang(self, mock_warn, mock_aioresponse):  # noqa: F811
         """Test fallback lang in case requested lang is not available."""
         mock_aioresponse.get(
             f"{self.base_url}/data/l10n/de-CH.json",
             status=400,
         )
         session = aiohttp.ClientSession()
-        sma = SMA(session, self.host, "pass", lang="de-CH")
+        sma = SMAwebconnect(session, self.host, "pass", lang="de-CH")
         await sma._read_l10n()
         assert mock_warn.call_count == 1
         assert len(sma._l10n) > 0
```

### Comparing `pysma-plus-0.1.4/tests/test_sensor.py` & `pysma_plus-0.1.5/tests/test_sensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Test pysma sensors."""
 import logging
 from json import loads
 from unittest.mock import patch
 
 import pytest
 
-from pysma.const import (
+from pysma.const_webconnect import (
     GENERIC_SENSORS,
     JMESPATH_VAL,
     JMESPATH_VAL_IDX,
     JMESPATH_VAL_STR,
 )
-from pysma.definitions import sensor_map
+from pysma.definitions_webconnect import sensor_map
 from pysma.sensor import Sensor, Sensors
 
 _LOGGER = logging.getLogger(__name__)
 
 
 SB_1_5 = loads(
     # {"result": {"012F-7309879F":
```

