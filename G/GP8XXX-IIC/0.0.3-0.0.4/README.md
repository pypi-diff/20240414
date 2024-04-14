# Comparing `tmp/GP8XXX_IIC-0.0.3.tar.gz` & `tmp/GP8XXX_IIC-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/GP8XXX_IIC-0.0.3.tar", last modified: Fri Apr  5 17:33:54 2024, max compression
+gzip compressed data, was "dist/GP8XXX_IIC-0.0.4.tar", last modified: Sun Apr 14 19:47:02 2024, max compression
```

## Comparing `GP8XXX_IIC-0.0.3.tar` & `GP8XXX_IIC-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:33:54.000000 GP8XXX_IIC-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:33:54.000000 GP8XXX_IIC-0.0.3/GP8XXX_IIC/
--rwxr-xr-x   0 runner    (1001) docker     (127)     8239 2024-04-05 17:33:41.000000 GP8XXX_IIC-0.0.3/GP8XXX_IIC/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 17:33:54.000000 GP8XXX_IIC-0.0.3/GP8XXX_IIC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-05 17:33:54.000000 GP8XXX_IIC-0.0.3/GP8XXX_IIC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-05 17:33:54.000000 GP8XXX_IIC-0.0.3/GP8XXX_IIC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 17:33:54.000000 GP8XXX_IIC-0.0.3/GP8XXX_IIC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-05 17:33:54.000000 GP8XXX_IIC-0.0.3/GP8XXX_IIC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 17:33:54.000000 GP8XXX_IIC-0.0.3/GP8XXX_IIC.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-05 17:33:54.000000 GP8XXX_IIC-0.0.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     1619 2024-04-05 17:33:41.000000 GP8XXX_IIC-0.0.3/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-04-05 17:33:41.000000 GP8XXX_IIC-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 17:33:54.000000 GP8XXX_IIC-0.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1085 2024-04-05 17:33:41.000000 GP8XXX_IIC-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:47:02.000000 GP8XXX_IIC-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:47:02.000000 GP8XXX_IIC-0.0.4/GP8XXX_IIC/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8953 2024-04-14 19:46:51.000000 GP8XXX_IIC-0.0.4/GP8XXX_IIC/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 19:47:02.000000 GP8XXX_IIC-0.0.4/GP8XXX_IIC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-14 19:47:02.000000 GP8XXX_IIC-0.0.4/GP8XXX_IIC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-14 19:47:02.000000 GP8XXX_IIC-0.0.4/GP8XXX_IIC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 19:47:02.000000 GP8XXX_IIC-0.0.4/GP8XXX_IIC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 19:47:02.000000 GP8XXX_IIC-0.0.4/GP8XXX_IIC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-14 19:47:02.000000 GP8XXX_IIC-0.0.4/GP8XXX_IIC.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-04-14 19:47:02.000000 GP8XXX_IIC-0.0.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1619 2024-04-14 19:46:51.000000 GP8XXX_IIC-0.0.4/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-04-14 19:46:51.000000 GP8XXX_IIC-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 19:47:02.000000 GP8XXX_IIC-0.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1085 2024-04-14 19:46:51.000000 GP8XXX_IIC-0.0.4/setup.py
```

### Comparing `GP8XXX_IIC-0.0.3/GP8XXX_IIC/__init__.py` & `GP8XXX_IIC-0.0.4/GP8XXX_IIC/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,16 +56,15 @@
         return not self._i2c.read_byte(self._device_addr) != 0
 
     def set_dac_outrange(self, output_range: int = GP8XXX.OUTPUT_RANGE_10V):
         """
         Set the DAC output range
         - param output_range [int]: DAC output range
         """
-        if isinstance(self, (GP8503, GP8512)) or \
-           isinstance(self, (GP8413)) and output_range == self.OUTPUT_RANGE_5V:
+        if isinstance(self, (GP8503, GP8512)):
             raise ValueError("DAC doesn't support another output range.")
 
         if output_range == self.OUTPUT_RANGE_5V:
             self._dac_voltage = 5000
             self._i2c.write_byte_data(
                 self._device_addr, self.GP8XXX_CONFIG_REG >> 1, 0x00)
         elif output_range == self.OUTPUT_RANGE_10V:
@@ -185,22 +184,22 @@
     def __init__(self, bus=1):
         super().__init__(bus=bus, resolution=self.RESOLUTION_15_BIT, auto_range=False)
         self._dac_voltage = 2500
 
 
 class GP8413(GP8XXX_IIC):
     """
-    15bit DAC Dual Channel I2C to 0-10V
+    15bit DAC Dual Channel I2C to 0-5V/0-10V
     - param bus: the i2c bus number
     - param i2c_addr: the I2C device address 
     """
 
-    def __init__(self, bus=1, i2c_addr=0x58):
+    def __init__(self, bus=1, i2c_addr=0x58, auto_range=True):
         super().__init__(bus=bus, resolution=self.RESOLUTION_15_BIT,
-                         device_addr=i2c_addr, auto_range=False)
+                         device_addr=i2c_addr, auto_range=auto_range)
         self.set_dac_outrange(self.OUTPUT_RANGE_10V)
 
 
 class GP8403(GP8XXX_IIC):
     """
     12bit DAC Dual Channel I2C to 0-5V/0-10V
     - param bus: the i2c bus number
@@ -211,23 +210,40 @@
     def __init__(self, bus=1, i2c_addr=0x58, auto_range=True):
         super().__init__(bus=bus, resolution=self.RESOLUTION_12_BIT,
                          device_addr=i2c_addr, auto_range=auto_range)
 
 
 class GP8302(GP8XXX_IIC):
     """
-    12bit DAC Dual Channel I2C to 0-5V/0-10V
+    12bit DAC I2C to 0-25mA
     - param bus: the i2c bus number
-    - param i2c_addr: the I2C device address 
-    - param auto_range: automatically selects the correct output range 
     """
 
-    def __init__(self, bus=1, i2c_addr=0x58, auto_range=True):
+    def __init__(self, bus=1, i2c_addr=0x58):
         super().__init__(bus=bus, resolution=self.RESOLUTION_12_BIT,
-                         device_addr=i2c_addr, auto_range=auto_range)
+                         device_addr=i2c_addr, auto_range=False)
+        self._dac_4 = 0
+        self._dac_20 = 0
+        self._calibration = False
+        self._dac_voltage = 2500
+
+
+    def calibration4_20ma(self, dac_4 = 655, dac_20 = 3277):
+        """
+        Calibrate the current within 4-20mA
+        - param dac_4: Range 0-0xFFF, the calibration is invalid if the value is out of range, the DAC value corresponding to current of 4mA generally fluctuates at about 655, the actual value needs to be tested by the user in actual applications
+        - param dac_20: Range 0-0xFFF, the calibration is invalid if the value is out of range, the DAC value corresponding to current of 20mA generally fluctuates at about 3277, the actual value needs to be tested by the user in actual applications
+        """
+        
+        if dac_4 >= dac_20 or dac_20 > self._resolution:
+            return None
+        self._dac_4       = dac_4
+        self._dac_20      = dac_20
+        self._calibration = True
+
 
     def set_dac_out_electric_current(self, current: int):
         """
         Set different channel output DAC values
-        - param current [int]: value corresponding to the output current value (e.g. 1.321A is 1321)
+        - param current [int]: value corresponding to the output current value (e.g. 0.03A)
         """
         return self.set_dac_out_voltage(current)
```

### Comparing `GP8XXX_IIC-0.0.3/GP8XXX_IIC.egg-info/PKG-INFO` & `GP8XXX_IIC-0.0.4/GP8XXX_IIC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GP8XXX-IIC
-Version: 0.0.3
+Version: 0.0.4
 Summary: The GP8XXX Python module offers an intuitive interface for controlling DAC (Digital to Analog Converter) devices via the I2C protocol. With support for various DAC models.
 Home-page: https://github.com/joe2824/GP8XXX_IIC/
 Author: Joel Klein
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/joe2824/GP8XXX_IIC/issues
 Project-URL: Github, https://github.com/joe2824/GP8XXX_IIC/
 Description: # GP8XXX-IIC
```

### Comparing `GP8XXX_IIC-0.0.3/PKG-INFO` & `GP8XXX_IIC-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GP8XXX_IIC
-Version: 0.0.3
+Version: 0.0.4
 Summary: The GP8XXX Python module offers an intuitive interface for controlling DAC (Digital to Analog Converter) devices via the I2C protocol. With support for various DAC models.
 Home-page: https://github.com/joe2824/GP8XXX_IIC/
 Author: Joel Klein
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/joe2824/GP8XXX_IIC/issues
 Project-URL: Github, https://github.com/joe2824/GP8XXX_IIC/
 Description: # GP8XXX-IIC
```

### Comparing `GP8XXX_IIC-0.0.3/README.md` & `GP8XXX_IIC-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `GP8XXX_IIC-0.0.3/setup.py` & `GP8XXX_IIC-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="GP8XXX_IIC",
     keywords='Raspberry Pi, Raspi, GP8403, GP8503, GP8211S, GP8512, GP8413, GP8302, DAC',
-    version="0.0.3",
+    version="0.0.4",
     author="Joel Klein",
     description="The GP8XXX Python module offers an intuitive interface for controlling DAC (Digital to Analog Converter) devices via the I2C protocol. With support for various DAC models.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/joe2824/GP8XXX_IIC/",
     project_urls={
         "Bug Tracker": "https://github.com/joe2824/GP8XXX_IIC/issues",
```

