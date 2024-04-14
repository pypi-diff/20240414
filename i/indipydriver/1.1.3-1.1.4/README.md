# Comparing `tmp/indipydriver-1.1.3.tar.gz` & `tmp/indipydriver-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipydriver-1.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "indipydriver-1.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `indipydriver-1.1.3.tar` & `indipydriver-1.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-07-31 15:52:08.000000 indipydriver-1.1.3/LICENSE
--rw-r--r--   0        0        0     2411 2023-07-11 05:27:01.000000 indipydriver-1.1.3/README.md
--rw-r--r--   0        0        0      573 2024-04-05 12:16:24.000000 indipydriver-1.1.3/indipydriver/__init__.py
--rw-r--r--   0        0        0    19033 2024-03-21 12:23:56.000000 indipydriver-1.1.3/indipydriver/comms.py
--rw-r--r--   0        0        0    21399 2024-01-06 13:04:44.000000 indipydriver-1.1.3/indipydriver/events.py
--rw-r--r--   0        0        0    21349 2024-04-05 12:04:08.000000 indipydriver-1.1.3/indipydriver/ipydriver.py
--rw-r--r--   0        0        0    12064 2024-02-07 20:19:44.000000 indipydriver-1.1.3/indipydriver/ipyserver.py
--rw-r--r--   0        0        0    12236 2024-02-23 14:46:47.000000 indipydriver-1.1.3/indipydriver/propertymembers.py
--rw-r--r--   0        0        0    43405 2024-02-23 14:49:50.000000 indipydriver-1.1.3/indipydriver/propertyvectors.py
--rw-r--r--   0        0        0      814 2024-04-05 12:16:14.000000 indipydriver-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     3124 1970-01-01 00:00:00.000000 indipydriver-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-31 15:52:08.000000 indipydriver-1.1.4/LICENSE
+-rw-r--r--   0        0        0     2470 2024-04-14 12:44:57.000000 indipydriver-1.1.4/README.md
+-rw-r--r--   0        0        0      573 2024-04-14 13:06:50.000000 indipydriver-1.1.4/indipydriver/__init__.py
+-rw-r--r--   0        0        0    19033 2024-03-21 12:23:56.000000 indipydriver-1.1.4/indipydriver/comms.py
+-rw-r--r--   0        0        0    21399 2024-01-06 13:04:44.000000 indipydriver-1.1.4/indipydriver/events.py
+-rw-r--r--   0        0        0    21349 2024-04-05 12:04:08.000000 indipydriver-1.1.4/indipydriver/ipydriver.py
+-rw-r--r--   0        0        0    12064 2024-02-07 20:19:44.000000 indipydriver-1.1.4/indipydriver/ipyserver.py
+-rw-r--r--   0        0        0    12236 2024-02-23 14:46:47.000000 indipydriver-1.1.4/indipydriver/propertymembers.py
+-rw-r--r--   0        0        0    43405 2024-02-23 14:49:50.000000 indipydriver-1.1.4/indipydriver/propertyvectors.py
+-rw-r--r--   0        0        0      814 2024-04-14 13:06:41.000000 indipydriver-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3183 1970-01-01 00:00:00.000000 indipydriver-1.1.4/PKG-INFO
```

### Comparing `indipydriver-1.1.3/LICENSE` & `indipydriver-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `indipydriver-1.1.3/README.md` & `indipydriver-1.1.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # indipydriver
 
-This is a pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver.
+This is a pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver and serve the INDI communications protocol on a port.
 
 INDI - Instrument Neutral Distributed Interface.
 
 See https://en.wikipedia.org/wiki/Instrument_Neutral_Distributed_Interface
 
 Typically the driver created with this package interfaces between your code which controls an instrument, or GPIO pins on the computer itself, and the INDI protocol which communicates to an INDI client.
 
 This package can be used to create the drivers, it does not include client functions. The INDI protocol is defined so that drivers should operate with any INDI client.
 
+This is a companion package to 'indipyclient' which provides a terminal client.
+
 The protocol defines the format of the data sent, such as light, number, text or switch, and the client can send commands to control the instrument.  The client can be general purpose, taking the format of switches, numbers etc., from the protocol.
 
 INDI is often used with astronomical instruments, but is a general purpose protocol which can be used for any instrument control providing drivers are available.
 
 The driver object created contains 'device' objects, each of which can contain 'vector' objects, such as a SwitchVector or LightVector. These Vector objects can contain one or more 'members', such as a number of 'switches', or a number of 'lights'.
 
 Typically you would create a subclass of IPyDriver.
@@ -26,20 +28,19 @@
 
 async def hardware(self)
 
 This should be a contuously running coroutine which you can use to operate your instruments, and if required send updates to the client.
 
 async def snoopevent(self, event)
 
-This is only used if one device is monitoring (snooping) on other devices.
-
-Having created an instance of your IPyDriver subclass, you would run the driver using:
+This is only used if the device is monitoring (snooping) on other devices.
 
-asyncio.run(driver.asyncrun())
+Having created an instance of your IPyDriver subclass, you would serve this, and any other drivers with an IPyServer object::
 
-The driver can transmit/receive either by stdin/stdout, or by a port.
+    server = IPyServer([driver], host="localhost", port=7624, maxconnections=5)
+    asyncio.run(server.asyncrun())
 
-A further class provided in the package, IPyServer can operate with multiple driver instances, and serves them all via a port, a connected client can then control all the drivers.
+A connected client can then control all the drivers.
 
 Documentation at https://indipydriver.readthedocs.io
 
 Installation from https://pypi.org/project/indipydriver
```

### Comparing `indipydriver-1.1.3/indipydriver/__init__.py` & `indipydriver-1.1.4/indipydriver/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 
 from .ipydriver import IPyDriver, Device
 from .propertyvectors import SwitchVector, LightVector, TextVector, BLOBVector, NumberVector
 from .propertymembers import SwitchMember, LightMember, TextMember, BLOBMember, NumberMember
 from .events import getProperties, enableBLOB, newSwitchVector, newTextVector, newNumberVector, newBLOBVector, Message, delProperty, defSwitchVector, defTextVector, defNumberVector, defLightVector, defBLOBVector, setSwitchVector, setTextVector, setNumberVector, setLightVector, setBLOBVector
 from .ipyserver import IPyServer
 
-version = "1.1.3"
+version = "1.1.4"
```

### Comparing `indipydriver-1.1.3/indipydriver/comms.py` & `indipydriver-1.1.4/indipydriver/comms.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.1.3/indipydriver/events.py` & `indipydriver-1.1.4/indipydriver/events.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.1.3/indipydriver/ipydriver.py` & `indipydriver-1.1.4/indipydriver/ipydriver.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.1.3/indipydriver/ipyserver.py` & `indipydriver-1.1.4/indipydriver/ipyserver.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.1.3/indipydriver/propertymembers.py` & `indipydriver-1.1.4/indipydriver/propertymembers.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.1.3/indipydriver/propertyvectors.py` & `indipydriver-1.1.4/indipydriver/propertyvectors.py`

 * *Files identical despite different names*

### Comparing `indipydriver-1.1.3/pyproject.toml` & `indipydriver-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipydriver"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "1.1.3"
+version = "1.1.4"
 description="Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'driver', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipydriver.readthedocs.io"
```

### Comparing `indipydriver-1.1.3/PKG-INFO` & `indipydriver-1.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 Metadata-Version: 2.1
 Name: indipydriver
-Version: 1.1.3
+Version: 1.1.4
 Summary: Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver.
 Keywords: indi,driver,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator
 Project-URL: Documentation, https://indipydriver.readthedocs.io
 Project-URL: Source, https://github.com/bernie-skipole/indipydriver
 
 # indipydriver
 
-This is a pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver.
+This is a pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver and serve the INDI communications protocol on a port.
 
 INDI - Instrument Neutral Distributed Interface.
 
 See https://en.wikipedia.org/wiki/Instrument_Neutral_Distributed_Interface
 
 Typically the driver created with this package interfaces between your code which controls an instrument, or GPIO pins on the computer itself, and the INDI protocol which communicates to an INDI client.
 
 This package can be used to create the drivers, it does not include client functions. The INDI protocol is defined so that drivers should operate with any INDI client.
 
+This is a companion package to 'indipyclient' which provides a terminal client.
+
 The protocol defines the format of the data sent, such as light, number, text or switch, and the client can send commands to control the instrument.  The client can be general purpose, taking the format of switches, numbers etc., from the protocol.
 
 INDI is often used with astronomical instruments, but is a general purpose protocol which can be used for any instrument control providing drivers are available.
 
 The driver object created contains 'device' objects, each of which can contain 'vector' objects, such as a SwitchVector or LightVector. These Vector objects can contain one or more 'members', such as a number of 'switches', or a number of 'lights'.
 
 Typically you would create a subclass of IPyDriver.
@@ -41,21 +43,20 @@
 
 async def hardware(self)
 
 This should be a contuously running coroutine which you can use to operate your instruments, and if required send updates to the client.
 
 async def snoopevent(self, event)
 
-This is only used if one device is monitoring (snooping) on other devices.
-
-Having created an instance of your IPyDriver subclass, you would run the driver using:
+This is only used if the device is monitoring (snooping) on other devices.
 
-asyncio.run(driver.asyncrun())
+Having created an instance of your IPyDriver subclass, you would serve this, and any other drivers with an IPyServer object::
 
-The driver can transmit/receive either by stdin/stdout, or by a port.
+    server = IPyServer([driver], host="localhost", port=7624, maxconnections=5)
+    asyncio.run(server.asyncrun())
 
-A further class provided in the package, IPyServer can operate with multiple driver instances, and serves them all via a port, a connected client can then control all the drivers.
+A connected client can then control all the drivers.
 
 Documentation at https://indipydriver.readthedocs.io
 
 Installation from https://pypi.org/project/indipydriver
```

