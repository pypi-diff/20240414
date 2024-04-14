# Comparing `tmp/goodwe-0.3.2.tar.gz` & `tmp/goodwe-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodwe-0.3.2.tar", last modified: Tue Apr  9 19:09:32 2024, max compression
+gzip compressed data, was "goodwe-0.3.3.tar", last modified: Sun Apr 14 20:20:43 2024, max compression
```

## Comparing `goodwe-0.3.2.tar` & `goodwe-0.3.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:09:32.031517 goodwe-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-09 19:09:19.000000 goodwe-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-09 19:09:32.031517 goodwe-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-09 19:09:19.000000 goodwe-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-09 19:09:27.000000 goodwe-0.3.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:09:32.031517 goodwe-0.3.2/goodwe/
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-09 19:09:19.000000 goodwe-0.3.2/goodwe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-04-09 19:09:19.000000 goodwe-0.3.2/goodwe/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-04-09 19:09:19.000000 goodwe-0.3.2/goodwe/dt.py
--rw-r--r--   0 runner    (1001) docker     (127)    22417 2024-04-09 19:09:19.000000 goodwe-0.3.2/goodwe/es.py
--rw-r--r--   0 runner    (1001) docker     (127)    38443 2024-04-09 19:09:19.000000 goodwe-0.3.2/goodwe/et.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-09 19:09:19.000000 goodwe-0.3.2/goodwe/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-04-09 19:09:19.000000 goodwe-0.3.2/goodwe/inverter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-09 19:09:19.000000 goodwe-0.3.2/goodwe/modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-09 19:09:19.000000 goodwe-0.3.2/goodwe/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    13162 2024-04-09 19:09:19.000000 goodwe-0.3.2/goodwe/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    34696 2024-04-09 19:09:19.000000 goodwe-0.3.2/goodwe/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:09:32.031517 goodwe-0.3.2/goodwe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-09 19:09:32.000000 goodwe-0.3.2/goodwe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-09 19:09:32.000000 goodwe-0.3.2/goodwe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 19:09:32.000000 goodwe-0.3.2/goodwe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-09 19:09:32.000000 goodwe-0.3.2/goodwe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-09 19:09:19.000000 goodwe-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-09 19:09:32.035517 goodwe-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 19:09:32.031517 goodwe-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    20438 2024-04-09 19:09:19.000000 goodwe-0.3.2/tests/test_dt.py
--rw-r--r--   0 runner    (1001) docker     (127)    29085 2024-04-09 19:09:19.000000 goodwe-0.3.2/tests/test_es.py
--rw-r--r--   0 runner    (1001) docker     (127)    66859 2024-04-09 19:09:19.000000 goodwe-0.3.2/tests/test_et.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-09 19:09:19.000000 goodwe-0.3.2/tests/test_modbus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-04-09 19:09:19.000000 goodwe-0.3.2/tests/test_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-04-09 19:09:19.000000 goodwe-0.3.2/tests/test_sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:20:43.465417 goodwe-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-14 20:20:36.000000 goodwe-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-14 20:20:43.465417 goodwe-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-14 20:20:36.000000 goodwe-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 20:20:40.000000 goodwe-0.3.3/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:20:43.461417 goodwe-0.3.3/goodwe/
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-04-14 20:20:36.000000 goodwe-0.3.3/goodwe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-04-14 20:20:36.000000 goodwe-0.3.3/goodwe/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10581 2024-04-14 20:20:36.000000 goodwe-0.3.3/goodwe/dt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22434 2024-04-14 20:20:36.000000 goodwe-0.3.3/goodwe/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39228 2024-04-14 20:20:36.000000 goodwe-0.3.3/goodwe/et.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-14 20:20:36.000000 goodwe-0.3.3/goodwe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10325 2024-04-14 20:20:36.000000 goodwe-0.3.3/goodwe/inverter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-04-14 20:20:36.000000 goodwe-0.3.3/goodwe/modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-14 20:20:36.000000 goodwe-0.3.3/goodwe/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13162 2024-04-14 20:20:36.000000 goodwe-0.3.3/goodwe/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36845 2024-04-14 20:20:36.000000 goodwe-0.3.3/goodwe/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:20:43.465417 goodwe-0.3.3/goodwe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-14 20:20:43.000000 goodwe-0.3.3/goodwe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-14 20:20:43.000000 goodwe-0.3.3/goodwe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 20:20:43.000000 goodwe-0.3.3/goodwe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 20:20:43.000000 goodwe-0.3.3/goodwe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-14 20:20:36.000000 goodwe-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-14 20:20:43.465417 goodwe-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:20:43.465417 goodwe-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    20434 2024-04-14 20:20:36.000000 goodwe-0.3.3/tests/test_dt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29085 2024-04-14 20:20:36.000000 goodwe-0.3.3/tests/test_es.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66856 2024-04-14 20:20:36.000000 goodwe-0.3.3/tests/test_et.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-14 20:20:36.000000 goodwe-0.3.3/tests/test_modbus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5233 2024-04-14 20:20:36.000000 goodwe-0.3.3/tests/test_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13867 2024-04-14 20:20:36.000000 goodwe-0.3.3/tests/test_sensor.py
```

### Comparing `goodwe-0.3.2/LICENSE` & `goodwe-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.2/PKG-INFO` & `goodwe-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodwe
-Version: 0.3.2
+Version: 0.3.3
 Summary: Read data from GoodWe inverter via local network
 Home-page: https://github.com/marcelblijleven/goodwe
 Author: Martin Letenay, Marcel Blijleven
 Author-email: 'marcelblijleven@gmail.com
 License: MIT
 Keywords: GoodWe,Solar Panel,Inverter,Photovoltaics,PV
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `goodwe-0.3.2/README.md` & `goodwe-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.2/goodwe/__init__.py` & `goodwe-0.3.3/goodwe/__init__.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.2/goodwe/const.py` & `goodwe-0.3.3/goodwe/const.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.2/goodwe/dt.py` & `goodwe-0.3.3/goodwe/dt.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.2/goodwe/es.py` & `goodwe-0.3.3/goodwe/es.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     ModbusReadCommand, ModbusWriteCommand, ModbusWriteMultiCommand
 from .sensor import *
 
 logger = logging.getLogger(__name__)
 
 
 class ES(Inverter):
-    """Class representing inverter of ES/EM/BP family"""
+    """Class representing inverter of ES/EM/BP family AKA platform 105"""
 
     _READ_DEVICE_VERSION_INFO: ProtocolCommand = Aa55ProtocolCommand("010200", "0182")
     _READ_DEVICE_RUNNING_DATA: ProtocolCommand = Aa55ProtocolCommand("010600", "0186")
     _READ_DEVICE_SETTINGS_DATA: ProtocolCommand = Aa55ProtocolCommand("010900", "0189")
 
     __sensors: Tuple[Sensor, ...] = (
         Voltage("vpv1", 0, "PV1 Voltage", Kind.PV),  # modbus 0x500
```

### Comparing `goodwe-0.3.2/goodwe/et.py` & `goodwe-0.3.3/goodwe/et.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 import logging
 from typing import Tuple
 
 from .exceptions import RequestRejectedException
 from .inverter import Inverter
 from .inverter import OperationMode
 from .inverter import SensorKind as Kind
-from .model import is_2_battery, is_4_mppt, is_single_phase
+from .model import is_2_battery, is_4_mppt, is_745_platform, is_single_phase
 from .protocol import ProtocolCommand, ModbusReadCommand, ModbusWriteCommand, ModbusWriteMultiCommand
 from .sensor import *
 
 logger = logging.getLogger(__name__)
 
 
 class ET(Inverter):
-    """Class representing inverter of ET/EH/BT/BH or GE's GEH families"""
+    """Class representing inverter of ET/EH/BT/BH or GE's GEH families AKA platform 205 or 745"""
 
     # Modbus registers from offset 0x891c (35100), count 0x7d (125)
     __all_sensors: Tuple[Sensor, ...] = (
         Timestamp("timestamp", 35100, "Timestamp"),
         Voltage("vpv1", 35103, "PV1 Voltage", Kind.PV),
         Current("ipv1", 35104, "PV1 Current", Kind.PV),
         Power4("ppv1", 35105, "PV1 Power", Kind.PV),
@@ -380,27 +380,33 @@
         EcoModeV2("eco_mode_3", 47559, "Eco Mode Group 3"),
         ByteH("eco_mode_3_switch", 47561, "Eco Mode Group 3 Switch"),
         EcoModeV2("eco_mode_4", 47565, "Eco Mode Group 4"),
         ByteH("eco_mode_4_switch", 47567, "Eco Mode Group 4 Switch"),
 
         Integer("load_control_mode", 47595, "Load Control Mode", "", Kind.AC),
         Integer("load_control_switch", 47596, "Load Control Switch", "", Kind.AC),
-        Integer("load_control_soc", 47596, "Load Control SoC", "", Kind.AC),
+        Integer("load_control_soc", 47597, "Load Control SoC", "", Kind.AC),
 
         Integer("fast_charging_power", 47603, "Fast Charging Power", "%", Kind.BAT),
     )
 
     # Settings added in ARM firmware 22
     __settings_arm_fw_22: Tuple[Sensor, ...] = (
+        Long("peak_shaving_power_limit", 47542, "Peak Shaving Power Limit"),
+        Integer("peak_shaving_soc", 47544, "Peak Shaving SoC"),
         # EcoModeV2("eco_modeV2_5", 47571, "Eco Mode Version 2 Power Group 5"),
         # EcoModeV2("eco_modeV2_6", 47577, "Eco Mode Version 2 Power Group 6"),
         # EcoModeV2("eco_modeV2_7", 47583, "Eco Mode Version 2 Power Group 7"),
         PeakShavingMode("peak_shaving_mode", 47589, "Peak Shaving Mode"),
 
         Integer("dod_holding", 47602, "DoD Holding", "", Kind.BAT),
+        Integer("backup_mode_enable", 47605, "Backup Mode Switch"),
+        Integer("max_charge_power", 47606, "Max Charge Power"),
+        Integer("smart_charging_enable", 47609, "Smart Charging Mode Switch"),
+        Integer("eco_mode_enable", 47612, "Eco Mode Switch"),
     )
 
     def __init__(self, host: str, comm_addr: int = 0, timeout: int = 1, retries: int = 3):
         super().__init__(host, comm_addr, timeout, retries)
         if not self.comm_addr:
             # Set the default inverter address
             self.comm_addr = 0xf7
@@ -622,31 +628,39 @@
             await self._set_offline(False)
             await self._clear_battery_mode_param()
         elif operation_mode == OperationMode.OFF_GRID:
             await self.write_setting('work_mode', 1)
             await self._set_offline(True)
             await self.write_setting('backup_supply', 1)
             await self.write_setting('cold_start', 4)
+            await self._clear_battery_mode_param()
         elif operation_mode == OperationMode.BACKUP:
             await self.write_setting('work_mode', 2)
             await self._set_offline(False)
             await self._clear_battery_mode_param()
         elif operation_mode == OperationMode.ECO:
             await self.write_setting('work_mode', 3)
             await self._set_offline(False)
         elif operation_mode == OperationMode.PEAK_SHAVING:
             await self.write_setting('work_mode', 4)
             await self._set_offline(False)
+            await self._clear_battery_mode_param()
         elif operation_mode in (OperationMode.ECO_CHARGE, OperationMode.ECO_DISCHARGE):
             if eco_mode_power < 0 or eco_mode_power > 100:
                 raise ValueError()
             if eco_mode_soc < 0 or eco_mode_soc > 100:
                 raise ValueError()
+
             eco_mode: EcoMode | Sensor = self._settings.get('eco_mode_1')
-            await self._read_setting(eco_mode)
+            # Load the current values to try to detect schedule type
+            try:
+                await self._read_setting(eco_mode)
+            except ValueError:
+                pass
+            eco_mode.set_schedule_type(ScheduleType.ECO_MODE, is_745_platform(self))
             if operation_mode == OperationMode.ECO_CHARGE:
                 await self.write_setting('eco_mode_1', eco_mode.encode_charge(eco_mode_power, eco_mode_soc))
             else:
                 await self.write_setting('eco_mode_1', eco_mode.encode_discharge(eco_mode_power))
             await self.write_setting('eco_mode_2_switch', 0)
             await self.write_setting('eco_mode_3_switch', 0)
             await self.write_setting('eco_mode_4_switch', 0)
```

### Comparing `goodwe-0.3.2/goodwe/exceptions.py` & `goodwe-0.3.3/goodwe/exceptions.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.2/goodwe/inverter.py` & `goodwe-0.3.3/goodwe/inverter.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,16 +72,16 @@
     """
 
     GENERAL = 0
     OFF_GRID = 1
     BACKUP = 2
     ECO = 3
     PEAK_SHAVING = 4
-    ECO_CHARGE = 5
-    ECO_DISCHARGE = 6
+    ECO_CHARGE = 10
+    ECO_DISCHARGE = 11
 
 
 class Inverter(ABC):
     """
     Common superclass for various inverter models implementations.
     Represents the inverter state and its basic behavior
     """
```

### Comparing `goodwe-0.3.2/goodwe/modbus.py` & `goodwe-0.3.3/goodwe/modbus.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.2/goodwe/protocol.py` & `goodwe-0.3.3/goodwe/protocol.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.2/goodwe/sensor.py` & `goodwe-0.3.3/goodwe/sensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,70 +17,74 @@
 class ScheduleType(IntEnum):
     ECO_MODE = 0,
     DRY_CONTACT_LOAD = 1,
     DRY_CONTACT_SMART_LOAD = 2,
     PEAK_SHAVING = 3,
     BACKUP_MODE = 4,
     SMART_CHARGE_MODE = 5,
-    ECO_MODE_745 = 6
+    ECO_MODE_745 = 6,
+    NOT_SET = 85
 
     @classmethod
     def detect_schedule_type(cls, value: int) -> ScheduleType:
         """Detect schedule type from its on/off value"""
-        if value in (0, -1, 85):
+        if value in (0, -1):
             return ScheduleType.ECO_MODE
         elif value in (1, -2):
             return ScheduleType.DRY_CONTACT_LOAD
         elif value in (2, -3):
             return ScheduleType.DRY_CONTACT_SMART_LOAD
         elif value in (3, -4):
             return ScheduleType.PEAK_SHAVING
         elif value in (4, -5):
             return ScheduleType.BACKUP_MODE
         elif value in (5, -6):
             return ScheduleType.SMART_CHARGE_MODE
         elif value in (6, -7):
             return ScheduleType.ECO_MODE_745
+        elif value == 85:
+            return ScheduleType.NOT_SET
         else:
             raise ValueError(f"{value}: on_off value {value} out of range.")
 
     def power_unit(self):
         """Return unit of power parameter"""
         if self == ScheduleType.PEAK_SHAVING:
             return "W"
         else:
             return "%"
 
     def decode_power(self, value: int) -> int:
         """Decode human readable value of power parameter"""
-        if self == ScheduleType.ECO_MODE:
-            return value
-        elif self == ScheduleType.PEAK_SHAVING:
+        if self == ScheduleType.PEAK_SHAVING:
             return value * 10
-        if self == ScheduleType.ECO_MODE_745:
+        elif self == ScheduleType.ECO_MODE_745:
             return int(value / 10)
+        elif self == ScheduleType.NOT_SET:
+            # Prevent out of range values when changing mode
+            return value if -100 <= value <= 100 else int(value / 10)
         else:
             return value
 
     def encode_power(self, value: int) -> int:
         """Encode human readable value of power parameter"""
         if self == ScheduleType.ECO_MODE:
             return value
         elif self == ScheduleType.PEAK_SHAVING:
             return int(value / 10)
-        if self == ScheduleType.ECO_MODE_745:
+        elif self == ScheduleType.ECO_MODE_745:
             return value * 10
         else:
             return value
 
     def is_in_range(self, value: int) -> bool:
         """Check if the value fits in allowed values range"""
         if self == ScheduleType.ECO_MODE:
             return -100 <= value <= 100
-        if self == ScheduleType.ECO_MODE_745:
+        elif self == ScheduleType.ECO_MODE_745:
             return -1000 <= value <= 1000
         else:
             return True
 
 
 class Voltage(Sensor):
     """Sensor representing voltage [V] value encoded in 2 (unsigned) bytes"""
@@ -294,27 +298,53 @@
     def encode_value(self, value: Any, register_value: bytes = None) -> bytes:
         word = bytearray(register_value)
         word[1] = int.to_bytes(int(value), length=1, byteorder="big", signed=True)[0]
         return bytes(word)
 
 
 class Integer(Sensor):
+    """Sensor representing unsigned int value encoded in 2 bytes"""
+
+    def __init__(self, id_: str, offset: int, name: str, unit: str = "", kind: Optional[SensorKind] = None):
+        super().__init__(id_, offset, name, 2, unit, kind)
+
+    def read_value(self, data: ProtocolResponse):
+        return read_bytes2(data)
+
+    def encode_value(self, value: Any, register_value: bytes = None) -> bytes:
+        return int.to_bytes(int(value), length=2, byteorder="big", signed=False)
+
+
+class IntegerS(Sensor):
     """Sensor representing signed int value encoded in 2 bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, unit: str = "", kind: Optional[SensorKind] = None):
         super().__init__(id_, offset, name, 2, unit, kind)
 
     def read_value(self, data: ProtocolResponse):
         return read_bytes2_signed(data)
 
     def encode_value(self, value: Any, register_value: bytes = None) -> bytes:
         return int.to_bytes(int(value), length=2, byteorder="big", signed=True)
 
 
 class Long(Sensor):
+    """Sensor representing unsigned int value encoded in 4 bytes"""
+
+    def __init__(self, id_: str, offset: int, name: str, unit: str = "", kind: Optional[SensorKind] = None):
+        super().__init__(id_, offset, name, 4, unit, kind)
+
+    def read_value(self, data: ProtocolResponse):
+        return read_bytes4(data)
+
+    def encode_value(self, value: Any, register_value: bytes = None) -> bytes:
+        return int.to_bytes(int(value), length=4, byteorder="big", signed=False)
+
+
+class LongS(Sensor):
     """Sensor representing signed int value encoded in 4 bytes"""
 
     def __init__(self, id_: str, offset: int, name: str, unit: str = "", kind: Optional[SensorKind] = None):
         super().__init__(id_, offset, name, 4, unit, kind)
 
     def read_value(self, data: ProtocolResponse):
         return read_bytes4_signed(data)
@@ -472,14 +502,22 @@
     def is_eco_charge_mode(self) -> bool:
         """Answer if it represents the emulated 24/7 fulltime discharge mode"""
 
     @abstractmethod
     def is_eco_discharge_mode(self) -> bool:
         """Answer if it represents the emulated 24/7 fulltime discharge mode"""
 
+    @abstractmethod
+    def get_schedule_type(self) -> ScheduleType:
+        """Answer the schedule type"""
+
+    @abstractmethod
+    def set_schedule_type(self, schedule_type: ScheduleType, is745: bool):
+        """Set the schedule type"""
+
 
 class EcoModeV1(Sensor, EcoMode):
     """Sensor representing Eco Mode Battery Power Group encoded in 8 bytes"""
 
     def __init__(self, id_: str, offset: int, name: str):
         super().__init__(id_, offset, name, 8, "", SensorKind.BAT)
         self.start_h: int | None = None
@@ -514,16 +552,14 @@
         if self.power < -100 or self.power > 100:
             raise ValueError(f"{self.id_}: power value {self.power} out of range.")
         self.on_off = read_byte(data)
         if self.on_off not in (0, -1):
             raise ValueError(f"{self.id_}: on_off value {self.on_off} out of range.")
         self.day_bits = read_byte(data)
         self.days = decode_day_of_week(self.day_bits)
-        if self.day_bits < 0:
-            raise ValueError(f"{self.id_}: day_bits value {self.day_bits} out of range.")
         return self
 
     def encode_value(self, value: Any, register_value: bytes = None) -> bytes:
         if isinstance(value, bytes) and len(value) == 8:
             # try to read_value to check if values are valid
             if self.read_value(ProtocolResponse(value, None)):
                 return value
@@ -557,14 +593,22 @@
             and self.start_m == 0 \
             and self.end_h == 23 \
             and self.end_m == 59 \
             and self.on_off != 0 \
             and self.day_bits == 127 \
             and self.power > 0
 
+    def get_schedule_type(self) -> ScheduleType:
+        """Answer the schedule type"""
+        return ScheduleType.ECO_MODE
+
+    def set_schedule_type(self, schedule_type: ScheduleType, is745: bool):
+        """Set the schedule type"""
+        pass
+
     def as_eco_mode_v2(self) -> EcoModeV2:
         """Convert V1 to V2 EcoMode"""
         result = EcoModeV2(self.id_, self.offset, self.name)
         result.start_h = self.start_h
         result.start_m = self.start_m
         result.end_h = self.end_h
         result.end_m = self.end_m
@@ -613,16 +657,14 @@
         self.end_m = read_byte(data)
         if (self.end_m < 0 or self.end_m > 59) and self.end_m != -1:
             raise ValueError(f"{self.id_}: end_m value {self.end_m} out of range.")
         self.on_off = read_byte(data)
         self.schedule_type = ScheduleType.detect_schedule_type(self.on_off)
         self.day_bits = read_byte(data)
         self.days = decode_day_of_week(self.day_bits)
-        if self.day_bits < 0:
-            raise ValueError(f"{self.id_}: day_bits value {self.day_bits} out of range.")
         self.power = read_bytes2_signed(data)  # negative=charge, positive=discharge
         if not self.schedule_type.is_in_range(self.power):
             raise ValueError(f"{self.id_}: power value {self.power} out of range.")
         self.soc = read_bytes2_signed(data)
         if self.soc < 0 or self.soc > 100:
             raise ValueError(f"{self.id_}: SoC value {self.soc} out of range.")
         self.month_bits = read_bytes2_signed(data)
@@ -676,14 +718,27 @@
             and self.end_h == 23 \
             and self.end_m == 59 \
             and self.on_off == (-1 - self.schedule_type) \
             and self.day_bits == 127 \
             and self.power > 0 \
             and (self.month_bits == 0 or self.month_bits == 0x0fff)
 
+    def get_schedule_type(self) -> ScheduleType:
+        """Answer the schedule type"""
+        return self.schedule_type
+
+    def set_schedule_type(self, schedule_type: ScheduleType, is745: bool):
+        """Set the schedule type"""
+        if schedule_type == ScheduleType.ECO_MODE:
+            # try to keep-reuse the type, use is745 only when necessary
+            if self.schedule_type not in (ScheduleType.ECO_MODE, ScheduleType.ECO_MODE_745):
+                self.schedule_type = ScheduleType.ECO_MODE_745 if is745 else ScheduleType.ECO_MODE
+        else:
+            self.schedule_type = schedule_type
+
     def as_eco_mode_v1(self) -> EcoModeV1:
         """Convert V2 to V1 EcoMode"""
         result = EcoModeV1(self.id_, self.offset, self.name)
         result.start_h = self.start_h
         result.start_m = self.start_m
         result.end_h = self.end_h
         result.end_m = self.end_m
@@ -887,28 +942,32 @@
             if bitmap.get(i, f'err{i}'):
                 result.append(bitmap.get(i, f'err{i}'))
         bits = bits >> 1
     return ", ".join(result)
 
 
 def decode_day_of_week(data: int) -> str:
+    if data == -1:
+        return "Mon-Sun"
+    elif data == 0:
+        return ""
     bits = bin(data)[2:]
     daynames = list(DAY_NAMES)
     days = ""
     for each in bits[::-1]:
         if each == '1':
             if len(days) > 0:
                 days += ","
             days += daynames[0]
         daynames.pop(0)
     return days
 
 
 def decode_months(data: int) -> str | None:
-    if data == 0 or data == 0x0fff:
+    if data <= 0 or data == 0x0fff:
         return None
     bits = bin(data)[2:]
     monthnames = list(MONTH_NAMES)
     months = ""
     for each in bits[::-1]:
         if each == '1':
             if len(months) > 0:
```

### Comparing `goodwe-0.3.2/goodwe.egg-info/PKG-INFO` & `goodwe-0.3.3/goodwe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodwe
-Version: 0.3.2
+Version: 0.3.3
 Summary: Read data from GoodWe inverter via local network
 Home-page: https://github.com/marcelblijleven/goodwe
 Author: Martin Letenay, Marcel Blijleven
 Author-email: 'marcelblijleven@gmail.com
 License: MIT
 Keywords: GoodWe,Solar Panel,Inverter,Photovoltaics,PV
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `goodwe-0.3.2/setup.cfg` & `goodwe-0.3.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.2/tests/test_dt.py` & `goodwe-0.3.3/tests/test_dt.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         self.assertSensor('e_total', 13350.2, 'kWh', data)
         self.assertSensor('h_total', 8451, 'h', data)
         self.assertSensor('safety_country', 20, '', data)
         self.assertSensor('safety_country_label', 'NL-A', '', data)
         self.assertSensor('funbit', 0, '', data)
         self.assertSensor('vbus', 601.2, 'V', data)
         self.assertSensor('vnbus', 305.4, 'V', data)
-        self.assertSensor('derating_mode', -1, '', data)
+        self.assertSensor('derating_mode', 0, '', data)
         self.assertSensor('derating_mode_label', '', '', data)
 
         self.assertFalse(self.sensor_map, f"Some sensors were not tested {self.sensor_map}")
 
     def test_GW6000_DT_setting(self):
         self.assertEqual(4, len(self.settings()))
         settings = {s.id_: s for s in self.settings()}
@@ -165,15 +165,15 @@
         self.assertSensor('error_codes', 0, '', data)
         self.assertSensor('warning_code', 0, '', data)
         self.assertSensor("apparent_power", 0, "VA", data),
         self.assertSensor("reactive_power", 0, "var", data),
         self.assertSensor('temperature', 45.3, 'C', data)
         self.assertSensor('e_day', 0.0, 'kWh', data)
         self.assertSensor('e_total', 0.0, 'kWh', data)
-        self.assertSensor('h_total', -1, 'h', data)
+        self.assertSensor('h_total', 0, 'h', data)
         self.assertSensor('safety_country', 32, '', data)
         self.assertSensor('safety_country_label', '50Hz 230Vac Default', '', data)
         self.assertSensor('funbit', 512, '', data)
         self.assertSensor('vbus', 624.2, 'V', data)
         self.assertSensor('vnbus', 316.8, 'V', data)
         self.assertSensor('derating_mode', 0, '', data)
         self.assertSensor('derating_mode_label', '', '', data)
@@ -225,15 +225,15 @@
         self.assertSensor('e_total', 881.7, 'kWh', data)
         self.assertSensor('h_total', 955, 'h', data)
         self.assertSensor('safety_country', 73, '', data)
         self.assertSensor('safety_country_label', 'Australia Victoria', '', data)
         self.assertSensor('funbit', 2400, '', data)
         self.assertSensor('vbus', 291.7, 'V', data)
         self.assertSensor('vnbus', 0, 'V', data)
-        self.assertSensor('derating_mode', -1, '', data)
+        self.assertSensor('derating_mode', 0, '', data)
         self.assertSensor('derating_mode_label', '', '', data)
 
     def test_get_grid_export_limit(self):
         self.loop.run_until_complete(self.read_device_info())
         self.loop.run_until_complete(self.get_grid_export_limit())
         self.assertEqual('7f039d8800026193', self.request.hex())
 
@@ -291,15 +291,15 @@
         self.assertSensor('e_total', 6.8, 'kWh', data)
         self.assertSensor('h_total', 7, 'h', data)
         self.assertSensor('safety_country', 73, '', data)
         self.assertSensor('safety_country_label', 'Australia Victoria', '', data)
         self.assertSensor('funbit', 2384, '', data)
         self.assertSensor('vbus', 393.9, 'V', data)
         self.assertSensor('vnbus', 0, 'V', data)
-        self.assertSensor('derating_mode', -1, '', data)
+        self.assertSensor('derating_mode', 0, '', data)
         self.assertSensor('derating_mode_label', '', '', data)
 
 
 class GW10K_MS_30_Test(DtMock):
 
     def __init__(self, methodName='runTest'):
         DtMock.__init__(self, methodName)
```

### Comparing `goodwe-0.3.2/tests/test_es.py` & `goodwe-0.3.3/tests/test_es.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.2/tests/test_et.py` & `goodwe-0.3.3/tests/test_et.py`

 * *Files 0% similar despite different names*

```diff
@@ -365,15 +365,15 @@
         self.assertEqual(167, self.dsp_svn_version)
         self.assertEqual(23, self.arm_version)
         self.assertEqual(237, self.arm_svn_version)
         self.assertEqual('04029-10-S11', self.firmware)
         self.assertEqual('02041-23-S00', self.arm_firmware)
 
     def test_GW10K_ET_setting_fw1023(self):
-        self.assertEqual(40, len(self.settings()))
+        self.assertEqual(46, len(self.settings()))
         settings = {s.id_: s for s in self.settings()}
         self.assertEqual('PeakShavingMode', type(settings.get("peak_shaving_mode")).__name__)
 
 
 class GW6000_EH_Test(EtMock):
 
     def __init__(self, methodName='runTest'):
@@ -445,15 +445,15 @@
         self.assertSensor('battery_mode', 0, '', data)
         self.assertSensor('battery_mode_label', 'No battery', '', data)
         self.assertSensor('warning_code', 0, '', data)
         self.assertSensor('safety_country', 3, '', data)
         self.assertSensor('safety_country_label', 'ES-A', '', data)
         self.assertSensor('work_mode', 1, '', data)
         self.assertSensor('work_mode_label', 'Normal (On-Grid)', '', data)
-        self.assertSensor('operation_mode', -1, '', data)
+        self.assertSensor('operation_mode', 0, '', data)
         self.assertSensor('error_codes', 0, '', data)
         self.assertSensor('errors', '', '', data)
         self.assertSensor("e_total", 59.4, 'kWh', data)
         self.assertSensor("e_day", 22.0, 'kWh', data)
         self.assertSensor("e_total_exp", 58.6, 'kWh', data)
         self.assertSensor('h_total', 33, 'h', data)
         self.assertSensor("e_day_exp", 21.6, 'kWh', data)
@@ -546,15 +546,15 @@
         self.assertSensor('battery_mode', 3, '', data)
         self.assertSensor('battery_mode_label', 'Charge', '', data)
         self.assertSensor('warning_code', 0, '', data)
         self.assertSensor('safety_country', 9, '', data)
         self.assertSensor('safety_country_label', 'Australia A', '', data)
         self.assertSensor('work_mode', 1, '', data)
         self.assertSensor('work_mode_label', 'Normal (On-Grid)', '', data)
-        self.assertSensor('operation_mode', -1, '', data)
+        self.assertSensor('operation_mode', 0, '', data)
         self.assertSensor('error_codes', 0, '', data)
         self.assertSensor('errors', '', '', data)
         self.assertSensor('e_total', 10225.8, 'kWh', data)
         self.assertSensor('e_day', 23.1, 'kWh', data)
         self.assertSensor('e_total_exp', 10273.3, 'kWh', data)
         self.assertSensor('h_total', 3256, 'h', data)
         self.assertSensor('e_day_exp', 16.6, 'kWh', data)
@@ -1081,15 +1081,15 @@
         self.assertSensor('meter_reactive_power3', 1077, 'var', data)
         self.assertSensor('meter_reactive_power_total', 2831, 'var', data)
         self.assertSensor('meter_apparent_power1', -1076, 'VA', data)
         self.assertSensor('meter_apparent_power2', -1414, 'VA', data)
         self.assertSensor('meter_apparent_power3', -3175, 'VA', data)
         self.assertSensor('meter_apparent_power_total', -5667, 'VA', data)
         self.assertSensor('meter_type', 2, '', data)
-        self.assertSensor('meter_sw_version', -1, '', data)
+        self.assertSensor('meter_sw_version', 0, '', data)
         self.assertSensor('meter2_active_power', 0, 'W', data)
         self.assertSensor('meter2_e_total_exp', 0.0, 'kWh', data)
         self.assertSensor('meter2_e_total_imp', 0.0, 'kWh', data)
         self.assertSensor('meter2_comm_status', 0, '', data)
         self.assertSensor('meter_voltage1', 231.1, 'V', data)
         self.assertSensor('meter_voltage2', 233.2, 'V', data)
         self.assertSensor('meter_voltage3', 232.6, 'V', data)
```

### Comparing `goodwe-0.3.2/tests/test_modbus.py` & `goodwe-0.3.3/tests/test_modbus.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.2/tests/test_protocol.py` & `goodwe-0.3.3/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `goodwe-0.3.2/tests/test_sensor.py` & `goodwe-0.3.3/tests/test_sensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,25 @@
         testee = Integer("", 0, "", "", None)
 
         data = MockResponse("0031")
         self.assertEqual(49, testee.read(data))
         self.assertEqual("0031", testee.encode_value(49).hex())
 
         data = MockResponse("ff9e")
+        self.assertEqual(65438, testee.read(data))
+        self.assertEqual("ff9e", testee.encode_value(65438).hex())
+
+    def test_integer_signed(self):
+        testee = IntegerS("", 0, "", "", None)
+
+        data = MockResponse("0031")
+        self.assertEqual(49, testee.read(data))
+        self.assertEqual("0031", testee.encode_value(49).hex())
+
+        data = MockResponse("ff9e")
         self.assertEqual(-98, testee.read(data))
         self.assertEqual("ff9e", testee.encode_value(-98).hex())
 
     def test_decimal(self):
         testee = Decimal("", 0, 10, "", "", None)
 
         data = MockResponse("0031")
@@ -154,15 +165,14 @@
 
     def test_eco_mode_v1(self):
         testee = EcoModeV1("", 0, "")
 
         data = MockResponse("0d1e0e28ffc4ff1a")
         self.assertEqual("13:30-14:40 Mon,Wed,Thu -60% On", testee.read(data).__str__())
         self.assertEqual(bytes.fromhex("0d1e0e28ffc4ff1a"), testee.encode_value(bytes.fromhex("0d1e0e28ffc4ff1a")))
-        self.assertRaises(ValueError, lambda: testee.encode_value(bytes.fromhex("0d1e0e28ffc4ffff")))
         self.assertRaises(ValueError, lambda: testee.encode_value("some string"))
         self.assertFalse(testee.read(data).is_eco_charge_mode())
         self.assertFalse(testee.read(data).is_eco_discharge_mode())
 
         data = MockResponse(testee.encode_charge(-40).hex())
         self.assertEqual("0:0-23:59 Sun,Mon,Tue,Wed,Thu,Fri,Sat -40% On", testee.read(data).__str__())
         self.assertTrue(testee.read(data).is_eco_charge_mode())
@@ -184,15 +194,14 @@
         testee = Schedule("", 0, "")
 
         data = MockResponse("0d1e0e28ff1affc4005a0000")
         self.assertEqual("13:30-14:40 Mon,Wed,Thu -60% (SoC 90%) On", testee.read(data).__str__())
         self.assertEqual(ScheduleType.ECO_MODE, testee.schedule_type)
         self.assertEqual(bytes.fromhex("0d1e0e28ff1affc4005a0000"),
                          testee.encode_value(bytes.fromhex("0d1e0e28ff1affc4005a0000")))
-        self.assertRaises(ValueError, lambda: testee.encode_value(bytes.fromhex("0d1e0e28ffffffc4005a0000")))
         self.assertRaises(ValueError, lambda: testee.encode_value("some string"))
         self.assertFalse(testee.read(data).is_eco_charge_mode())
         self.assertFalse(testee.read(data).is_eco_discharge_mode())
 
         data = MockResponse(testee.encode_charge(-40, 80).hex())
         self.assertEqual("0:0-23:59 Sun,Mon,Tue,Wed,Thu,Fri,Sat -40% (SoC 80%) On", testee.read(data).__str__())
         self.assertTrue(testee.read(data).is_eco_charge_mode())
@@ -204,14 +213,16 @@
         self.assertTrue(testee.read(data).is_eco_discharge_mode())
         self.assertEqual("0:0-23:59 Sun,Mon,Tue,Wed,Thu,Fri,Sat 60% On", testee.as_eco_mode_v1().__str__())
         data = MockResponse(testee.encode_off().hex())
         self.assertEqual("48:0-48:0  100% (SoC 100%) Off", testee.read(data).__str__())
         self.assertFalse(testee.read(data).is_eco_charge_mode())
         self.assertFalse(testee.read(data).is_eco_discharge_mode())
 
+        data = MockResponse("0300080006fefd12005fcfff")
+        self.assertEqual("3:0-8:0 Mon -75% (SoC 95%) Off", testee.read(data).__str__())
         data = MockResponse("0000173b5500001400640000")
         self.assertEqual("0:0-23:59  20% (SoC 100%) Unset", testee.read(data).__str__())
         data = MockResponse("ffffffff557f000000010001")
         self.assertEqual("-1:-1--1:-1 Sun,Mon,Tue,Wed,Thu,Fri,Sat Jan 0% (SoC 1%) Unset", testee.read(data).__str__())
         data = MockResponse("000000005500000000000000")
         self.assertEqual("0:0-0:0  0% (SoC 0%) Unset", testee.read(data).__str__())
```

