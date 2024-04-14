# Comparing `tmp/solaxx3-0.1.3.tar.gz` & `tmp/solaxx3-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solaxx3-0.1.3.tar", last modified: Sun Mar  5 06:29:41 2023, max compression
+gzip compressed data, was "solaxx3-1.0.0.tar", last modified: Sun Apr 14 06:31:52 2024, max compression
```

## Comparing `solaxx3-0.1.3.tar` & `solaxx3-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-03-05 06:29:41.280268 solaxx3-0.1.3/
--rw-r--r--   0 pi        (1000) pi        (1000)     1100 2022-10-18 05:31:28.000000 solaxx3-0.1.3/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     2674 2023-03-05 06:29:41.280268 solaxx3-0.1.3/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      987 2022-10-18 05:31:28.000000 solaxx3-0.1.3/README.md
--rw-r--r--   0 pi        (1000) pi        (1000)      737 2023-03-05 06:06:56.000000 solaxx3-0.1.3/pyproject.toml
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-03-05 06:29:41.280268 solaxx3-0.1.3/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2022-10-18 05:31:28.000000 solaxx3-0.1.3/setup.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-03-05 06:29:41.270268 solaxx3-0.1.3/src/
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-03-05 06:29:41.270268 solaxx3-0.1.3/src/solaxx3/
--rw-r--r--   0 pi        (1000) pi        (1000)       57 2023-03-05 06:25:40.000000 solaxx3-0.1.3/src/solaxx3/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)    51871 2023-03-05 06:05:10.000000 solaxx3-0.1.3/src/solaxx3/registers.py
--rw-r--r--   0 pi        (1000) pi        (1000)     5521 2022-11-24 05:58:22.000000 solaxx3-0.1.3/src/solaxx3/rs485.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-03-05 06:29:41.280268 solaxx3-0.1.3/src/solaxx3.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     2674 2023-03-05 06:29:41.000000 solaxx3-0.1.3/src/solaxx3.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      285 2023-03-05 06:29:41.000000 solaxx3-0.1.3/src/solaxx3.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-03-05 06:29:41.000000 solaxx3-0.1.3/src/solaxx3.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       24 2023-03-05 06:29:41.000000 solaxx3-0.1.3/src/solaxx3.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        8 2023-03-05 06:29:41.000000 solaxx3-0.1.3/src/solaxx3.egg-info/top_level.txt
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-14 06:31:52.736317 solaxx3-1.0.0/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1100 2024-04-14 06:29:27.000000 solaxx3-1.0.0/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     2715 2024-04-14 06:31:52.736317 solaxx3-1.0.0/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      989 2024-04-14 06:29:27.000000 solaxx3-1.0.0/README.md
+-rw-r--r--   0 pi        (1000) pi        (1000)      737 2024-04-14 06:29:27.000000 solaxx3-1.0.0/pyproject.toml
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2024-04-14 06:31:52.736317 solaxx3-1.0.0/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2024-04-14 06:29:27.000000 solaxx3-1.0.0/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-14 06:31:52.728317 solaxx3-1.0.0/src/
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-14 06:31:52.732317 solaxx3-1.0.0/src/solaxx3/
+-rw-r--r--   0 pi        (1000) pi        (1000)       57 2024-04-14 06:29:27.000000 solaxx3-1.0.0/src/solaxx3/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)   115419 2024-04-14 06:29:27.000000 solaxx3-1.0.0/src/solaxx3/solax_registers_info.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6591 2024-04-14 06:29:27.000000 solaxx3-1.0.0/src/solaxx3/solaxx3.py
+-rw-r--r--   0 pi        (1000) pi        (1000)      374 2024-04-14 06:29:27.000000 solaxx3-1.0.0/src/solaxx3/utils.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2024-04-14 06:31:52.736317 solaxx3-1.0.0/src/solaxx3.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     2715 2024-04-14 06:31:52.000000 solaxx3-1.0.0/src/solaxx3.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      319 2024-04-14 06:31:52.000000 solaxx3-1.0.0/src/solaxx3.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2024-04-14 06:31:52.000000 solaxx3-1.0.0/src/solaxx3.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       24 2024-04-14 06:31:52.000000 solaxx3-1.0.0/src/solaxx3.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        8 2024-04-14 06:31:52.000000 solaxx3-1.0.0/src/solaxx3.egg-info/top_level.txt
```

### Comparing `solaxx3-0.1.3/LICENSE` & `solaxx3-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `solaxx3-0.1.3/PKG-INFO` & `solaxx3-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solaxx3
-Version: 0.1.3
+Version: 1.0.0
 Summary: Read Solax X3 inverter registers via modbus interface (RS-485)
 Author-email: Flavius Moldovan <mkfam@protonmail.com>
 License: The MIT License (MIT)
         Copyright © 2022 <copyright Flavius Moldovan>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -15,14 +15,15 @@
 Keywords: Solax,solax-x3,solaxx3,solar inverter,RTU,MODBUS
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pymodbus[serial]>=3.0.0
 
 # solax-x3
 ####  Read in real-time all parameters provided by Solax X3 solar inverter via its Modbus S-485 serial interface.
 
 <br />
 
 ## Prerequisites
@@ -39,15 +40,15 @@
 pip install solaxx3
 ```  
 
 ## Usage
 
 
 ```
-from solaxx3.rs485 import SolaxX3
+from solaxx3.solaxx3 import SolaxX3
 
 # adjust the serial port and baud rate as necessary
 s = SolaxX3(port="/dev/ttyUSB0", baudrate=115200)
 
 if s.connect():
     s.read_all_registers()
```

### Comparing `solaxx3-0.1.3/README.md` & `solaxx3-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 pip install solaxx3
 ```  
 
 ## Usage
 
 
 ```
-from solaxx3.rs485 import SolaxX3
+from solaxx3.solaxx3 import SolaxX3
 
 # adjust the serial port and baud rate as necessary
 s = SolaxX3(port="/dev/ttyUSB0", baudrate=115200)
 
 if s.connect():
     s.read_all_registers()
```

### Comparing `solaxx3-0.1.3/pyproject.toml` & `solaxx3-1.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "solaxx3"
-version = "0.1.3"
+version = "1.0.0"
 description = "Read Solax X3 inverter registers via modbus interface (RS-485)"
 readme = "README.md"
 authors = [{ name = "Flavius Moldovan", email = "mkfam@protonmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `solaxx3-0.1.3/src/solaxx3/rs485.py` & `solaxx3-1.0.0/src/solaxx3/solaxx3.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,44 @@
-from typing import Any
+from datetime import datetime
+from struct import unpack
+from typing import Any, Literal
 
 from pymodbus.client import ModbusSerialClient
-from datetime import date, datetime, timedelta
-from struct import *
-from solaxx3.registers import SolaxRegistersInfo
-from time import sleep, perf_counter
+
+from .solax_registers_info import SolaxRegistersInfo
+from .utils import join_msb_lsb, twos_complement
 
 
 class SolaxX3:
+    """
+    Class interacting with values from the inverter.
+    Initialization parameters:
+        - method (default: rtu)
+        - port (default: /dev/ttyUSB0 )
+        - baudrate: Bits per second (default: 115,200 )
+        - timeout: Timeout for a request, in seconds. (default: 3)
+        - parity: 'E'ven, 'O'dd, 'N'one (default: N)
+        - stopbits: Number of stop bits 0-2 (default: 1)
+        - bytesize: Number of bits per byte (7 or 8) (default: 8)
+    """
+
     connected: bool = False
 
     def __init__(
         self,
-        method="rtu",
-        port="/dev/ttyUSB0",
-        baudrate=115200,
-        timeout=3,
-        parity="N",
-        stopbits=1,
-        bytesize=8,
+        method: str = "rtu",
+        port: str = "/dev/ttyUSB0",
+        baudrate: int = 115200,
+        timeout: int = 3,
+        parity: Literal["E", "O", "N"] = "N",
+        stopbits: Literal[0, 1, 2] = 1,
+        bytesize: Literal[7, 8] = 8,
     ) -> None:
-        self._input_registers_values_list = []
-        self._holding_registers_values_list = []
+        self._input_registers_values = []
+        self._holding_registers_values = []
 
         self.client = ModbusSerialClient(
             method=method,
             port=port,
             baudrate=baudrate,
             timeout=timeout,
             parity=parity,
@@ -33,136 +46,141 @@
             bytesize=bytesize,
         )
 
     def connect(self) -> bool:
         self.connected = self.client.connect()
         return self.connected
 
-    def _join_msb_lsb(self, msb: int, lsb: int) -> int:
-        return (msb << 16) | lsb
-
-    def _unsigned16(self, type: str, addr: int, count: int = 1, unit: int = 1) -> int:
-
-        self._input_registers_values_list
-        if type == "input":
-            return self._input_registers_values_list[addr]
-        elif type == "holding":
-            return self._holding_registers_values_list[addr]
+    def _get_unsigned_16(self, value_type: str, address: int) -> int:
+        if value_type == "input":
+            return self._input_registers_values[address]
+        elif value_type == "holding":
+            return self._holding_registers_values[address]
 
-    def _readRegisterRange(
-        self, type: str, addr: int, count: int = 1, unit: int = 1
+    def _read_register_range(
+        self, value_type: str, address: int, count: int = 1
     ) -> list:
-        if type == "input":
-            return self._input_registers_values_list[addr : addr + count]
-        elif type == "holding":
-            return self._holding_registers_values_list[addr : addr + count]
+        if value_type == "input":
+            return self._input_registers_values[address : address + count]
+        elif value_type == "holding":
+            return self._holding_registers_values[address : address + count]
 
-    def _twos_complement(self, number: int, bits: int) -> int:
-        """
-        Compute the 2's complement of the int value val
+    def _read_format_register_value(self, register_info: dict) -> Any:
+        """Read the values from a register based on length and sign
+
+        Parameters:
+            register_info:dict  - dictionary with register definition fields
         """
 
-        # if sign bit is set e.g., 8bit: 128-255
-        if (number & (1 << (bits - 1))) != 0:
+        if self.is_register_type_integer(register_info):
+            value = self._get_integer_value(register_info)
+            value = value / register_info["si_adj"]
 
-            # compute negative value
-            number = number - (1 << bits)
+        elif self._is_register_type_string(register_info):
+            value = self._get_string_value(register_info)
 
-        return number
+        elif self._is_register_type_datetime(register_info):
+            value = self._get_datetime_value(register_info)
 
-    def _read_register(self, register_type: str, register_info: dict) -> Any:
-        """Read the values from a register based on length and sign
+        return value
 
-        Parameters:
+    def _get_datetime_value(self, register_info):
+        register_type = register_info["register_type"]
 
-            register_info:dict  - dictionary with register definition fields
-        """
+        sec, min, hr, day, mon, year = self._read_register_range(
+            register_type, register_info["address"], register_info["data_length"]
+        )
+        # modified !!!
+        inverter_datetime = f"{year:02}-{mon:02}-{day:02} {hr:02}:{min:02}:{sec:02}"
+        value = datetime.strptime(inverter_datetime, "%y-%m-%d %H:%M:%S")
+        return value
 
-        if "int" in register_info["data_format"]:
-            if register_info["data_length"] == 1:
-                val = self._unsigned16(register_type, register_info["address"])
-
-            if register_info["data_length"] == 2:
-                val = self._join_msb_lsb(
-                    self._unsigned16(register_type, register_info["address"] + 1),
-                    self._unsigned16(register_type, register_info["address"]),
-                )
-
-            if register_info["signed"]:
-                val = self._twos_complement(val, register_info["data_length"] * 16)
-
-            val = val / register_info["si_adj"]
-
-        elif "varchar" in register_info["data_format"]:
-            block = self._readRegisterRange(
-                register_type, register_info["address"], register_info["data_length"]
-            )
-            sn = []
-            for i in range(register_info["data_length"]):
-                first_byte, second_byte = unpack(
-                    "BB", int.to_bytes(block[i], 2, "little")
-                )
-                if not second_byte == 0x0:
-                    sn.append(chr(second_byte))
-                if not first_byte == 0x0:
-                    sn.append(chr(first_byte))
-            val = "".join(sn)
-
-        elif "datetime" in register_info["data_format"]:
-            sec, min, hr, day, mon, year = self._readRegisterRange(
-                register_type, register_info["address"], register_info["data_length"]
-            )
+    def _is_register_type_datetime(self, register_info):
+        return "datetime" in register_info["data_format"]
+
+    def _get_string_value(self, register_info):
+        register_type = register_info["register_type"]
 
-            inverter_datetime = (
-                f"{(year+2000):02}-{mon:02}-{day:02} {hr:02}:{min:02}:{sec:02}"
+        block = self._read_register_range(
+            register_type, register_info["address"], register_info["data_length"]
+        )
+        sn = []
+        for i in range(register_info["data_length"]):
+            first_byte, second_byte = unpack("BB", int.to_bytes(block[i], 2, "little"))
+            if not second_byte == 0x0:
+                sn.append(chr(second_byte))
+            if not first_byte == 0x0:
+                sn.append(chr(first_byte))
+
+        return "".join(sn)
+
+    def _is_register_type_string(self, register_info):
+        return "varchar" in register_info["data_format"]
+
+    def _get_integer_value(self, register_info):
+        register_type = register_info["register_type"]
+
+        if register_info["data_length"] == 1:
+            val = self._get_unsigned_16(register_type, register_info["address"])
+
+        if register_info["data_length"] == 2:
+            val = join_msb_lsb(
+                self._get_unsigned_16(register_type, register_info["address"] + 1),
+                self._get_unsigned_16(register_type, register_info["address"]),
             )
-            val = datetime.strptime(inverter_datetime, "%Y-%m-%d %H:%M:%S")
 
+        if register_info["signed"]:
+            val = twos_complement(val, register_info["data_length"] * 16)
         return val
 
-    def read_register(self, register_info: dict) -> tuple:
-        """Read the values from a register based on length and sign
+    def is_register_type_integer(self, register_info: dict[str, Any]) -> bool:
+        return "int" in register_info["data_format"]
 
-        Parameters:
+    def read_register_value(self, register_info: dict) -> tuple:
+        """Read the values from a register based on length and sign.
 
-            register_info:dict  - dictionary with register definition fields
+        Parameters:
+            :param register_info: dictionary with register definition fields
+            :return: Tuple containing the value and data unit
         """
 
-        val = self._read_register(register_info["register_type"], register_info)
-
-        if not "data_unit" in register_info:
-            return (val, "N/A")
-
+        val = self._read_format_register_value(register_info)
         return (val, register_info["data_unit"])
 
     def read(self, name: str):
         """Retrieve the value for the register with the provided name"""
 
-        r = SolaxRegistersInfo()
+        registers = SolaxRegistersInfo()
 
-        register_info = r.get_register_info(name)
-        value = self.read_register(register_info)
+        register_info = registers.get_register_info(name)
+        value_data_unit = self.read_register_value(register_info)
 
-        return value
+        return value_data_unit
 
     def list_register_names(self):
         r = SolaxRegistersInfo()
         return r.list_register_names()
 
     def read_all_registers(self) -> None:
-        self._input_registers_values_list = []
-        self._holding_registers_values_list = []
+        self._input_registers_values = []
+        self._holding_registers_values = []
 
-        read_block_length = 100
-        for i in range(3):
-            address = i * read_block_length
-            values_list = self.client.read_input_registers(
-                address=address, count=read_block_length, slave=1
+        READ_BLOCK_LENGTH = 100
+        self._read_input_registers(READ_BLOCK_LENGTH)
+        self._read_holding_registers(READ_BLOCK_LENGTH)
+
+    def _read_holding_registers(self, READ_BLOCK_LENGTH):
+        for count in range(4):
+            address = count * READ_BLOCK_LENGTH
+            values = self.client.read_holding_registers(
+                address=address, count=READ_BLOCK_LENGTH, slave=1
             ).registers
-            self._input_registers_values_list.extend(values_list)
+            self._holding_registers_values.extend(values)
+
+    def _read_input_registers(self, READ_BLOCK_LENGTH):
+        for count in range(4):
+            address = count * READ_BLOCK_LENGTH
 
-        for i in range(3):
-            address = i * read_block_length
-            values_list = self.client.read_holding_registers(
-                address=address, count=read_block_length, slave=1
+            values = self.client.read_input_registers(
+                address=address, count=READ_BLOCK_LENGTH, slave=1
             ).registers
-            self._holding_registers_values_list.extend(values_list)
+            self._input_registers_values.extend(values)
```

### Comparing `solaxx3-0.1.3/src/solaxx3.egg-info/PKG-INFO` & `solaxx3-1.0.0/src/solaxx3.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solaxx3
-Version: 0.1.3
+Version: 1.0.0
 Summary: Read Solax X3 inverter registers via modbus interface (RS-485)
 Author-email: Flavius Moldovan <mkfam@protonmail.com>
 License: The MIT License (MIT)
         Copyright © 2022 <copyright Flavius Moldovan>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -15,14 +15,15 @@
 Keywords: Solax,solax-x3,solaxx3,solar inverter,RTU,MODBUS
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pymodbus[serial]>=3.0.0
 
 # solax-x3
 ####  Read in real-time all parameters provided by Solax X3 solar inverter via its Modbus S-485 serial interface.
 
 <br />
 
 ## Prerequisites
@@ -39,15 +40,15 @@
 pip install solaxx3
 ```  
 
 ## Usage
 
 
 ```
-from solaxx3.rs485 import SolaxX3
+from solaxx3.solaxx3 import SolaxX3
 
 # adjust the serial port and baud rate as necessary
 s = SolaxX3(port="/dev/ttyUSB0", baudrate=115200)
 
 if s.connect():
     s.read_all_registers()
```

