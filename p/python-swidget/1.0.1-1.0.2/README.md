# Comparing `tmp/python_swidget-1.0.1.tar.gz` & `tmp/python_swidget-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_swidget-1.0.1.tar", max compression
+gzip compressed data, was "python_swidget-1.0.2.tar", max compression
```

## Comparing `python_swidget-1.0.1.tar` & `python_swidget-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      539 2024-04-10 14:24:43.925014 python_swidget-1.0.1/README.md
--rw-r--r--   0        0        0     2112 2024-04-10 14:26:35.525013 python_swidget-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1330 2024-04-10 14:24:43.935014 python_swidget-1.0.1/swidget/__init__.py
--rw-r--r--   0        0        0     9046 2024-04-10 14:24:43.935014 python_swidget-1.0.1/swidget/cli.py
--rw-r--r--   0        0        0     3829 2024-04-10 14:24:49.375014 python_swidget-1.0.1/swidget/discovery.py
--rw-r--r--   0        0        0       79 2023-01-11 19:11:12.359430 python_swidget-1.0.1/swidget/exceptions.py
--rw-r--r--   0        0        0     4591 2024-04-10 14:24:43.935014 python_swidget-1.0.1/swidget/provision.py
--rw-r--r--   0        0        0        0 2023-01-11 19:11:12.359430 python_swidget-1.0.1/swidget/py.typed
--rw-r--r--   0        0        0    18701 2024-04-10 14:24:43.935014 python_swidget-1.0.1/swidget/swidgetdevice.py
--rw-r--r--   0        0        0     1680 2024-04-10 14:24:43.935014 python_swidget-1.0.1/swidget/swidgetdimmer.py
--rw-r--r--   0        0        0      402 2024-04-10 14:24:43.935014 python_swidget-1.0.1/swidget/swidgetoutlet.py
--rw-r--r--   0        0        0      592 2024-04-10 14:24:43.935014 python_swidget-1.0.1/swidget/swidgetswitch.py
--rw-r--r--   0        0        0      789 2024-04-10 14:24:43.935014 python_swidget-1.0.1/swidget/swidgettimerswitch.py
--rw-r--r--   0        0        0     3943 2024-04-10 14:24:43.935014 python_swidget-1.0.1/swidget/websocket.py
--rw-r--r--   0        0        0     1741 1970-01-01 00:00:00.000000 python_swidget-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      539 2024-04-10 14:24:43.925014 python_swidget-1.0.2/README.md
+-rw-r--r--   0        0        0     2167 2024-04-14 18:19:53.397240 python_swidget-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1330 2024-04-10 14:24:43.935014 python_swidget-1.0.2/swidget/__init__.py
+-rw-r--r--   0        0        0     8982 2024-04-14 18:19:53.397240 python_swidget-1.0.2/swidget/cli.py
+-rw-r--r--   0        0        0     3865 2024-04-14 18:19:53.397240 python_swidget-1.0.2/swidget/discovery.py
+-rw-r--r--   0        0        0       79 2023-01-11 19:11:12.359430 python_swidget-1.0.2/swidget/exceptions.py
+-rw-r--r--   0        0        0     4591 2024-04-10 14:24:43.935014 python_swidget-1.0.2/swidget/provision.py
+-rw-r--r--   0        0        0        0 2023-01-11 19:11:12.359430 python_swidget-1.0.2/swidget/py.typed
+-rw-r--r--   0        0        0    19107 2024-04-14 18:19:53.397240 python_swidget-1.0.2/swidget/swidgetdevice.py
+-rw-r--r--   0        0        0     1696 2024-04-14 18:19:53.397240 python_swidget-1.0.2/swidget/swidgetdimmer.py
+-rw-r--r--   0        0        0      402 2024-04-10 14:24:43.935014 python_swidget-1.0.2/swidget/swidgetoutlet.py
+-rw-r--r--   0        0        0      402 2024-04-14 18:19:53.397240 python_swidget-1.0.2/swidget/swidgetswitch.py
+-rw-r--r--   0        0        0      820 2024-04-14 18:19:53.397240 python_swidget-1.0.2/swidget/swidgettimerswitch.py
+-rw-r--r--   0        0        0     4229 2024-04-14 18:19:53.397240 python_swidget-1.0.2/swidget/websocket.py
+-rw-r--r--   0        0        0     1826 1970-01-01 00:00:00.000000 python_swidget-1.0.2/PKG-INFO
```

### Comparing `python_swidget-1.0.1/README.md` & `python_swidget-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `python_swidget-1.0.1/pyproject.toml` & `python_swidget-1.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-swidget"
-version = "1.0.1"
+version = "1.0.2"
 description = "Python API for Swidget smart devices"
 license = "GPL-3.0-or-later"
 authors = ["Swidget"]
 repository = "https://github.com/swidget/python-swidget"
 readme = "README.md"
 packages = [
   { include = "swidget" }
@@ -18,14 +18,16 @@
 python = "^3.8"
 aiohttp = ">=3.8.1"
 anyio = "*"  # see https://github.com/python-trio/asyncclick/issues/18
 importlib-metadata = "*"
 asyncclick = ">=8"
 pydantic = "^1"
 ssdp = "1.1.1"
+requests = "2.31.0"
+types-requests = "2.31.0.20240406"
 
 # required only for docs
 sphinx = { version = "^4", optional = true }
 m2r = { version = "^0", optional = true }
 mistune = { version = "<2.0.0", optional = true }
 sphinx_rtd_theme = { version = "^0", optional = true }
 sphinxcontrib-programoutput = { version = "^0", optional = true }
```

### Comparing `python_swidget-1.0.1/swidget/__init__.py` & `python_swidget-1.0.2/swidget/__init__.py`

 * *Files identical despite different names*

### Comparing `python_swidget-1.0.1/swidget/cli.py` & `python_swidget-1.0.2/swidget/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """python-swidget cli tool."""
 import logging
 import sys
+from typing import Any, cast
 from pprint import pformat as pf
-from typing import cast
 
 import asyncclick as click
 from contextlib import asynccontextmanager
 
 from swidget import (
     discover_devices,
     discover_single,
@@ -21,16 +21,14 @@
 TYPE_TO_CLASS = {
     "dimmer": SwidgetDimmer,
     "switch": SwidgetSwitch,
     "outlet": SwidgetOutlet,
     "pana_switch": SwidgetTimerSwitch
 }
 
-click.anyio_backend = "asyncio"
-
 
 pass_dev = click.make_pass_decorator(SwidgetDevice)
 
 
 @click.group(invoke_without_command=True)
 @click.option("--host",
     envvar="SWIDGET_HOST",
@@ -68,15 +66,15 @@
         logging.basicConfig(level=logging.DEBUG)
     else:
         logging.basicConfig(level=logging.INFO)
 
     if ctx.invoked_subcommand == "discover" or ctx.invoked_subcommand == "wifi":
         return
     if host is None:
-        click.echo("No host name given, trying discovery..")
+        click.echo("No hostname or IP given, trying discovery..")
         await ctx.invoke(discover)
         return
     if type is not None:
         dev = TYPE_TO_CLASS[type](host=host,
                                   token_name='x-secret-key',
                                   secret_key=password,
                                   use_https=http_only,
@@ -189,39 +187,33 @@
 @pass_dev
 @click.argument("assembly")
 @click.argument("component")
 @click.argument("function")
 @click.argument("command")
 async def raw_command(dev: SwidgetDevice, assembly, component, function, command):
     """Run a raw command on the device."""
-    import ast
-
-    if parameters is not None:
-        parameters = ast.literal_eval(parameters)
-
-    res = await dev.send_command(assembly, component, function, command)
-
-    click.echo(res)
-    return res
+    await dev.send_command(assembly, component, function, command)
+    click.echo("Command sent")
 
 
 @cli.command()
 @click.argument("brightness", type=click.IntRange(0, 100), default=None, required=False)
 @pass_dev
-async def brightness(dev: SwidgetDimmer, brightness: int):
+async def brightness(dev: SwidgetDevice, brightness: Any=None):
+    dimmer_dev = cast(SwidgetDimmer, dev)
     """Get or set brightness."""
-    if not dev.is_dimmer:
+    if not dimmer_dev.is_dimmer:
         click.echo("This device does not support brightness.")
         return
 
     if brightness is None:
-        click.echo(f"Brightness: {dev.brightness}")
+        click.echo(f"Brightness: {dimmer_dev.brightness}")
     else:
         click.echo(f"Setting brightness to {brightness}")
-        return await dev.set_brightness(brightness)
+        return await dimmer_dev.set_brightness(brightness)
 
 
 @cli.command()
 @pass_dev
 async def blink(dev):
     """Set the device insert to blink"""
     click.echo(f"Requesting the device to blink")
```

### Comparing `python_swidget-1.0.1/swidget/discovery.py` & `python_swidget-1.0.2/swidget/discovery.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import asyncio
-import json
 import logging
 import socket
-from typing import Awaitable, Callable, Dict, Optional, Type, cast
+from typing import Any, Type
 from urllib.parse import urlparse
 
-import ssdp
+import ssdp  # type: ignore
 
 from swidget.swidgetdevice import DeviceType, SwidgetDevice
 from .swidgetdimmer import SwidgetDimmer
 from .swidgetoutlet import SwidgetOutlet
 from .swidgetswitch import SwidgetSwitch
 from .swidgettimerswitch import SwidgetTimerSwitch
 from .exceptions import SwidgetException
@@ -35,15 +34,15 @@
         mac_address = headers["USN"].split("-")[-1]
         ip_address = urlparse(headers["LOCATION"]).hostname
         if headers["ST"] == SWIDGET_ST:
             device_type = headers["SERVER"].split(" ")[1].split("+")[0]
             insert_type = headers["SERVER"].split(" ")[1].split("+")[1].split("/")[0]
             friendly_name = headers["SERVER"].split("/")[2].strip('"')
             devices[mac_address] = SwidgetDiscoveredDevice(mac_address, ip_address, friendly_name)
-            _LOGGER.debug(f"Swidget device '{friendly_name}' at {ip_address}")
+            _LOGGER.debug(f"Swidget device '{friendly_name}' at {ip_address}. {device_type}/{insert_type}")
 
 
 async def discover_devices(timeout=RESPONSE_SEC):
     global devices
     loop = asyncio.get_event_loop()
     devices = dict()
     transport, protocol = await loop.create_datagram_endpoint(
@@ -61,15 +60,15 @@
         },
     )
     search_request.sendto(transport, (SwidgetProtocol.MULTICAST_ADDRESS, 1900))
     await asyncio.sleep(timeout)
     return devices
 
 
-async def discover_single(host: str, token_name: str, password: str, use_https: bool, use_websockets: bool) -> SwidgetDevice:
+async def discover_single(host: str, token_name: str, password: str, use_https: bool, use_websockets: bool) -> Any:
     """Discover a single device by the given IP address.
 
     :param host: Hostname of device to query
     :rtype: SwidgetDevice
     :return: Object for querying/controlling found device.
     """
     _LOGGER.debug(f"Checking for device at {host}")
@@ -84,20 +83,20 @@
     device_class = _get_device_class(device_type)
     _LOGGER.debug(f"{device_class}")
     dev = device_class(host, token_name, password, use_https, use_websockets)
     await dev.start()
     return dev
 
 
-def _get_device_class(device_type: str) -> Type[SwidgetDevice]:
+def _get_device_class(device_type: DeviceType) -> Type[SwidgetDevice]:
     """Find SmartDevice subclass for device described by passed data."""
-    if device_type == "outlet":
+    if device_type == DeviceType.Outlet:
         return SwidgetOutlet
-    elif device_type == "switch":
+    elif device_type == DeviceType.Switch:
         return SwidgetSwitch
-    elif device_type == "dimmer":
+    elif device_type == DeviceType.Dimmer:
         return SwidgetDimmer
-    elif device_type == "pana_switch": # This is the timer switch
+    elif device_type == DeviceType.TimerSwitch: # This is the timer switch
         return SwidgetTimerSwitch
-    elif device_type == "relay_switch":
+    elif device_type == DeviceType.RelaySwitch:
         return SwidgetSwitch
     raise SwidgetException("Unknown device type: %s" % device_type)
```

### Comparing `python_swidget-1.0.1/swidget/provision.py` & `python_swidget-1.0.2/swidget/provision.py`

 * *Files identical despite different names*

### Comparing `python_swidget-1.0.1/swidget/swidgetdevice.py` & `python_swidget-1.0.2/swidget/swidgetdevice.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import logging
 import time
 
 from aiohttp import ClientSession, TCPConnector
 import asyncio
 from enum import Enum
-from typing import Dict, List, Set
+from typing import Any, Dict, List
 
 from .exceptions import SwidgetException
 from .websocket import SwidgetWebsocket
 
 _LOGGER = logging.getLogger(__name__)
 
 class DeviceType(Enum):
@@ -20,141 +20,140 @@
     Switch = "switch"
     TimerSwitch = "pana_switch"
     RelaySwitch = "relay_switch"
     Unknown = -1
 
 
 class SwidgetDevice:
-    def __init__(self, host, token_name, secret_key, use_https=True, use_websockets=True):
+    def __init__(self, host, token_name, secret_key, use_https=True, use_websockets=True) -> None:
         self.token_name = token_name
         self.ip_address = host
-
         self.use_https = use_https
         self.uri_scheme = 'https' if self.use_https is True else 'http'
         self.secret_key = secret_key
         self.use_websockets = use_websockets
         self.device_type = DeviceType.Unknown
         self._friendly_name = "Unknown Swidget Device"
-        self.assemblies = {}
+        self.assemblies: Dict[Any, Any] = dict()
         headers = {self.token_name: self.secret_key,
                    'Connection': 'keep-alive'}
         connector = TCPConnector(verify_ssl=False, force_close=True)
         self._session = ClientSession(headers=headers, connector=connector)
-        self._last_update = None
+        self._last_update: int = 0
         if self.use_websockets:
             self._websocket = SwidgetWebsocket(
                 host=self.ip_address,
                 token_name=self.token_name,
                 secret_key=self.secret_key,
                 callback=self.message_callback,
                 session=self._session)
 
-    def get_websocket(self):
+    def get_websocket(self) -> SwidgetWebsocket | None:
         if self.use_websockets:
             return self._websocket
         return None
 
-    def set_countdown_timer(self, minutes):
+    def set_countdown_timer(self, minutes) -> Any:
         raise NotImplementedError()
 
-    async def connect(self):
+    async def connect(self) -> None:
         await self._websocket.connect()
 
-    async def start(self):
+    async def start(self) -> None:
         """Start the websocket."""
         _LOGGER.debug("SwidgetDevice.start()")
         if self.use_websockets:
             _LOGGER.debug("Calling self._websocket.connect()")
             await self._websocket.connect()
         _LOGGER.debug("Calling self.update() ")
         await self.update()
 
-    async def stop(self):
+    async def stop(self) -> None:
         """Stop the websocket."""
         _LOGGER.debug("SwidgetDevice.stop()")
         if hasattr(self, '_websocket'):
             await self._websocket.close()
         await self._session.close()
 
-    async def close(self):
+    async def close(self) -> None:
         await self.stop()
 
-    async def message_callback(self, message):
+    async def message_callback(self, message) -> None:
         """Entrypoint for a websocket callback"""
         _LOGGER.debug("SwidgetDevice.message_callback() called")
         if message["request_id"] == "summary":
             _LOGGER.debug("Calling SwidgetDevice.process_summary()")
             await self.process_summary(message)
         elif message["request_id"] == "state" or message["request_id"] == "DYNAMIC_UPDATE" or message["request_id"] == "command":
             _LOGGER.debug("Calling SwidgetDevice.process_state()")
             await self.process_state(message)
         else:
             _LOGGER.error(f"Unknown message type from websocket. Type given was: {message["request_id"]}")
 
-    async def get_summary(self):
+    async def get_summary(self) -> None:
         """Get a summary of the device over HTTP"""
         _LOGGER.debug("SwidgetDevice.get_summary() called")
         if self.use_websockets:
             _LOGGER.debug("In websocket mode. Sending get_summary() command over websocket")
             await self._websocket.send_str(json.dumps({"type": "summary", "request_id": "summary"}))
         else:
             _LOGGER.debug("In http mode. Sending get_summary() command over http")
             async with self._session.get(
                 url=f"{self.uri_scheme}://{self.ip_address}/api/v1/summary", ssl=False
             ) as response:
                 summary = await response.json()
             await self.process_summary(summary)
 
-    async def process_summary(self, summary):
+    async def process_summary(self, summary) -> None:
         """ Process the data around the summary of the device"""
         _LOGGER.debug("SwidgetDevice.process_summary() called")
         _LOGGER.debug(f"Summary to process: {summary}")
         self.model = summary["model"]
         self.mac_address = summary["mac"]
         self.version = summary["version"]
         self.assemblies = {
             "host": SwidgetAssembly(summary["host"]),
             "insert": SwidgetAssembly(summary["insert"]),
         }
-        self.device_type = self.assemblies['host'].type
+        self.device_type = DeviceType(self.assemblies['host'].type)
         self.insert_type = self.assemblies['insert'].type
         self.id = self.assemblies['host'].id
         self._last_update = int(time.time())
 
-    async def get_friendly_name(self):
+    async def get_friendly_name(self) -> None:
         _LOGGER.debug("SwidgetDevice.get_friendly_name() called")
         try:
             async with self._session.get(
                 url=f"{self.uri_scheme}://{self.ip_address}/api/v1/name", ssl=False
             ) as response:
                 name = await response.json()
         except Exception:
             name = {"name": f"Swidget {self.device_type} w/{self.insert_type} insert"}
         await self.process_friendly_name(name['name'])
 
-    async def process_friendly_name(self, name):
+    async def process_friendly_name(self, name) -> None:
         _LOGGER.debug("SwidgetDevice.process_friendly_name() called")
         self._friendly_name = name
         self._last_update = int(time.time())
 
-    async def get_state(self):
+    async def get_state(self) -> None:
         """ Get the state of the device over HTTP"""
         _LOGGER.debug("SwidgetDevice.get_state() called")
         if self.use_websockets:
             _LOGGER.debug("In websocket mode. Sending get_summary() command over websocket")
             await self._websocket.send_str(json.dumps({"type": "state", "request_id": "state"}))
         else:
             _LOGGER.debug("In http mode. Sending get_summary() command over http")
             async with self._session.get(
                 url=f"{self.uri_scheme}://{self.ip_address}/api/v1/state", ssl=False
             ) as response:
                 state = await response.json()
             await self.process_state(state)
 
-    async def process_state(self, state):
+    async def process_state(self, state) -> None:
         """ Process any information about the state of the device or insert"""
         # State is not always in the state (during callback)
         _LOGGER.debug("SwidgetDevice.process_state() called")
         _LOGGER.debug(f"State to process: {state}")
         try:
             self.rssi = state["connection"]["rssi"]
         except:
@@ -163,151 +162,151 @@
             for id, component in self.assemblies[assembly].components.items():
                 try:
                     component.functions.update(state[assembly]["components"][id])
                 except:
                     pass
         self._last_update = int(time.time())
 
-    async def update(self):
+    async def update(self) -> None:
         _LOGGER.debug("SwidgetDevice.update() called")
-        if self._last_update is None:
+        if self._last_update == 0:
             _LOGGER.debug("Performing the initial update to obtain sysinfo")
             await self.get_summary()
             await self.get_state()
             if self._friendly_name == "Unknown Swidget Device":
                 await self.get_friendly_name()
         elif (int(time.time()) - self._last_update) < 5:
             _LOGGER.debug("update() recently called, not executing")
         else:
             _LOGGER.debug("Requesting an update of the device")
             await self.get_summary()
             await self.get_state()
 
-    async def send_config(self, payload: dict):
+    async def send_config(self, payload: dict) -> None:
         _LOGGER.debug("SwidgetDevice.send_config() called")
         data = json.dumps({"type":"config","request_id":"send_config", "payload": payload})
         await self._websocket.send_str(data)
 
     async def send_command(
         self, assembly: str, component: str, function: str, command: dict
-    ):
+    ) -> None:
         _LOGGER.debug("SwidgetDevice.send_command() called")
         """Send a command to the Swidget device either using a HTTP call or the existing websocket"""
         data = {assembly: {"components": {component: {function: command}}}}
         _LOGGER.debug(f"Command to send: {data}")
         if self.use_websockets:
             _LOGGER.debug("In websocket mode. Sending command over websocket")
-            data = json.dumps({"type": "command",
+            command_data = json.dumps({"type": "command",
                                "request_id": "command",
                                "payload": data
                                })
-            await self._websocket.send_str(data)
+            await self._websocket.send_str(command_data)
         else:
             _LOGGER.debug("NOT in websocket mode, sending command over HTTP")
             async with self._session.post(
                 url=f"{self.uri_scheme}://{self.ip_address}/api/v1/command",
                 ssl=False,
                 data=json.dumps(data),
             ) as response:
                 state = await response.json()
 
             # Do a hard set of the new state of the device. May change this in the future
             function_value = state[assembly]["components"][component][function]
             self.assemblies[assembly].components[component].functions[function] = function_value  # fmt: skip
 
-    async def ping(self):
+    async def ping(self) -> int | SwidgetException:
         """Ping the device to ensure it's devices
 
         :raises SwidgetException: Raise the exception if there we are unable to connect to the Swidget device
         """
         _LOGGER.debug("SwidgetDevice.ping() called")
         try:
             async with self._session.get(
                 url=f"{self.uri_scheme}://{self.ip_address}/ping",
                 ssl=False
             ) as response:
                 return response.status
         except:
             raise SwidgetException
 
-    async def blink(self):
+    async def blink(self) -> Any:
         """Make the device LED blink
 
         :raises SwidgetException: Raise the exception if there we are unable to connect to the Swidget device
         """
         _LOGGER.debug("SwidgetDevice.blink() called")
         try:
             async with self._session.get(
                 url=f"{self.uri_scheme}://{self.ip_address}/blink",
                 ssl=False
             ) as response:
                 return await response.json()
         except:
             raise SwidgetException
 
-    async def enable_debug_server(self):
+    async def enable_debug_server(self) -> Any:
         """Enable the Swidget local debug server
 
         :raises SwidgetException: Raise the exception if there we are unable to connect to the Swidget device
         """
         _LOGGER.debug("SwidgetDevice.enable_debug_server() called")
         try:
             async with self._session.get(
                 url=f"{self.uri_scheme}://{self.ip_address}/debug?x-secret-key={self.secret_key}",
                 ssl=False
             ) as response:
                 return await response.json()
         except:
             raise SwidgetException
 
-    async def factory_reset(self):
+    async def factory_reset(self) -> Any:
         """Factory reset the Swidget device
 
         :raises SwidgetException: Raise the exception if there we are unable to connect to the Swidget device
         """
         try:
 
             async with self._session.delete(
                 url=f"{self.uri_scheme}://{self.ip_address}/api/v1/reset",
                 ssl=False
             ) as response:
                 return await response.json()
         except:
             raise SwidgetException
 
-    async def check_for_updates(self):
+    async def check_for_updates(self) -> Any:
         """Tell the device to contact the Swidget servers to see if there is an available update
 
         :raises SwidgetException: Raise the exception if there we are unable to connect to the Swidget device
         """
         try:
 
             async with self._session.get(
                 url=f"{self.uri_scheme}://{self.ip_address}/api/v1/update",
                 ssl=False
             ) as response:
                 return await response.json()
         except:
             raise SwidgetException
 
-    async def update_version(self, version):
+    async def update_version(self, version) -> Any:
         """Tell the device to download and apply an update
 
         :raises SwidgetException: Raise the exception if there we are unable to connect to the Swidget device
         """
         try:
             data = {
                 "version": version
             }
             async with self._session.post(
                 url=f"{self.uri_scheme}://{self.ip_address}/api/v1/update",
                 ssl=False,
                 data=json.dumps(data)
             ) as response:
-                return await response
+                return await response.json()
         except:
             raise SwidgetException
 
     @property
     def hw_info(self) -> Dict:
         """
         Return hardware information.
@@ -322,35 +321,35 @@
             "model": self.model,
             "insert_type": self.insert_type,
             "insert_features": self.insert_features,
             "host_features": self.host_features,
             "rssi": self.rssi
         }
 
-    async def get_child_consumption(self, plug_id=0):
+    async def get_child_consumption(self, plug_id=0) -> Any:
         """Get the power consumption of a plug in watts."""
         if plug_id == "all":
             return_dict = {}
             for id, properties in self.assemblies['host'].components.items():
                 try:
                     return_dict[f"power_{id}"] = properties.functions['power']['current']
                 except KeyError: # Hits this when there is no power metering
                     return None
             return return_dict
         return self.assemblies['host'].components[str(plug_id)].functions['power']['current']
 
-    async def total_consumption(self):
+    async def total_consumption(self) -> float:
         """Get the total power consumption in watts."""
         total_consumption = 0
         for id, properties in self.assemblies['host'].components.items():
             total_consumption += properties.functions['power']['current']
         return total_consumption
 
     @property
-    async def realtime_values(self):
+    async def realtime_values(self) -> Dict:
         """Get a dict of realtime value attributes from the insert and host
 
         :return: A dictionary of insert sensor values and power consumption values
         :rtype: dict
         """
         return_dict = {}
         for feature in self.insert_features:
@@ -363,62 +362,62 @@
 
     @property
     def host_features(self) -> List[str]:
         """Return a set of features that the host supports."""
         try:
             return list(self.assemblies['host'].components['0'].functions.keys())
         except KeyError:
-            return set()
+            return list()
 
     @property
     def insert_features(self) -> List[str]:
         """Return a set of features that the insert supports."""
         try:
             return list(self.assemblies['insert'].components.keys())
         except KeyError:
-            return set()
+            return list()
 
-    def get_function_values(self, function: str):
+    def get_function_values(self, function: str) -> Dict:
         """Return the values of an insert function."""
         return_values = dict()
         for function, data in self.assemblies['insert'].components[function].functions.items():
             if function == "occupied":
                 return_values[function] = data['state']
             elif function == "toggle":
                 pass
             else:
                 return_values[function] = data['now']
         return return_values
 
-    def get_sensor_value(self, function, sensor):
+    def get_sensor_value(self, function, sensor) -> float | str:
         """Return the value of a sensor given a function and sensor"""
         if sensor == "occupied":
             return self.assemblies['insert'].components[function].functions['occupied']['state']
         else:
             return self.assemblies['insert'].components[function].functions[sensor]['now']
 
     @property
     def is_outlet(self) -> bool:
         """Return True if the device is an outlet."""
-        return self.device_type == "outlet"
+        return self.device_type == DeviceType.Outlet
 
     @property
     def is_switch(self) -> bool:
         """Return True if the device is a switch"""
-        return self.device_type == "switch" or self.device_type == "pana_switch" or self.device_type == "relay_switch"
+        return self.device_type == DeviceType.Switch or self.device_type == DeviceType.TimerSwitch or self.device_type == DeviceType.RelaySwitch
 
     @property
     def is_pana_switch(self) -> bool:
         """Return True if the device is a pana_switch"""
-        return self.device_type == "pana_switch"
+        return self.device_type == DeviceType.TimerSwitch
 
     @property
     def is_dimmer(self) -> bool:
         """Return True if the device is a dimmer"""
-        return self.device_type == "dimmer"
+        return self.device_type == DeviceType.Dimmer
 
     @property
     def is_dimmable(self) -> bool:
         """Return  True if the device is dimmable."""
         return self.is_dimmer
 
     @property  # type: ignore
@@ -430,50 +429,50 @@
     def is_on(self) -> bool:
         """Return whether device is on."""
         dimmer_state = self.assemblies['host'].components["0"].functions['toggle']["state"]
         if dimmer_state == "on":
             return True
         return False
 
-    async def turn_on(self):
+    async def turn_on(self) -> None:
         """Turn the device on."""
         _LOGGER.debug("SwidgetDevice.turn_on() called")
         await self.send_command(
             assembly="host", component="0", function="toggle", command={"state": "on"}
         )
 
-    async def turn_off(self):
+    async def turn_off(self) -> None:
         """Turn the device off."""
         _LOGGER.debug("SwidgetDevice.turn_off() called")
         await self.send_command(
             assembly="host", component="0", function="toggle", command={"state": "off"}
         )
 
-    async def turn_on_usb_insert(self):
+    async def turn_on_usb_insert(self) -> None:
         """Turn the USB insert on."""
         await self.send_command(
             assembly="insert", component="usb", function="toggle", command={"state": "on"}
         )
 
-    async def turn_off_usb_insert(self):
+    async def turn_off_usb_insert(self) -> None:
         """Turn the USB insert off."""
         await self.send_command(
             assembly="insert", component="usb", function="toggle", command={"state": "off"}
         )
 
     @property  # type: ignore
     def usb_is_on(self) -> bool:
         """Return whether USB is on."""
         usb_state = self.assemblies['insert'].components["usb"].functions['toggle']["state"]
         if usb_state == "on":
             return True
         return False
 
-    def __repr__(self):
-        if self._last_update is None:
+    def __repr__(self) -> str:
+        if self._last_update == 0:
             return f"<{self.device_type} at {self.ip_address} - update() needed>"
         return f"<{self.device_type} model {self.model} at {self.ip_address}>"
 
 
 class SwidgetAssembly:
     def __init__(self, summary: dict):
         self.type = summary["type"]
```

### Comparing `python_swidget-1.0.1/swidget/swidgetdimmer.py` & `python_swidget-1.0.2/swidget/swidgetdimmer.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,22 +24,22 @@
         if not self.is_dimmable:
             raise SwidgetException("Device is not dimmable.")
         try:
             return self.assemblies['host'].components["0"].functions["level"]["now"]
         except KeyError:
             return self.assemblies['host'].components["0"].functions["level"]["default"]
 
-    async def set_brightness(self, brightness):
+    async def set_brightness(self, brightness) -> None:
         """Set the brightness of the device."""
         _LOGGER.debug("SwidgetDimmer.set_brightness() called")
         await self.send_command(
             assembly="host", component="0", function="level", command={"now": brightness}
         )
 
-    async def set_default_brightness(self, brightness):
+    async def set_default_brightness(self, brightness) -> None:
         _LOGGER.debug("SwidgetDimmer.set_default_brightness() called")
         await self.send_command(
             assembly="host", component="0", function="level", command={"default": brightness}
         )
 
     @property  # type: ignore
     def is_dimmable(self) -> bool:
```

### Comparing `python_swidget-1.0.1/swidget/swidgettimerswitch.py` & `python_swidget-1.0.2/swidget/swidgettimerswitch.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import logging
+from typing import Any
+
 from swidget.swidgetdevice import (
     DeviceType,
 )
 from swidget.swidgetswitch import SwidgetSwitch
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class SwidgetTimerSwitch(SwidgetSwitch):
 
     def __init__(self, host,  token_name: str, secret_key: str, use_https: bool, use_websockets: bool) -> None:
         super().__init__(host=host, token_name=token_name, secret_key=secret_key, use_https=use_https, use_websockets=use_websockets)
         self._device_type = DeviceType.TimerSwitch
 
-    async def set_countdown_timer(self, minutes):
+    async def set_countdown_timer(self, minutes) -> Any:
         """Set the countdown timer."""
         _LOGGER.debug("SwidgetTimerSwitch.set_brightness() called")
         await self.send_command(
             assembly="host", component="0", function="timer", command={"duration": minutes}
         )
```

### Comparing `python_swidget-1.0.1/swidget/websocket.py` & `python_swidget-1.0.2/swidget/websocket.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         host,
         token_name,
         secret_key,
         callback,
         session=None,
         use_security=True,
     ):
-
+        self.host = host
         self.session = session or aiohttp.ClientSession()
         self.use_security = use_security
         self.uri = self.get_uri(host, token_name, secret_key)
         self.callback = callback
         self._verify_ssl = False
         self._state = None
         self.failed_attempts = 0
@@ -48,15 +48,15 @@
     @property
     def connected(self) -> bool:
         return self._client is not None and not self._client.closed
 
     @property
     def websocket(self) -> ClientWebSocketResponse | None:
         """Return the web socket."""
-        return self._ws
+        return self._client
 
     def get_uri(self, host, token_name, secret_key):
         """Generate the websocket URI"""
         if self.use_security:
             return f"wss://{host}/api/v1/sock?{token_name}={secret_key}"
         else:
             return f"ws://{host}/api/v1/sock?{token_name}={secret_key}"
@@ -71,24 +71,26 @@
 
         if not self.session:
             raise
 
         try:
             self._client = await self.session.ws_connect(url=self.uri, headers=self.headers, verify_ssl=self._verify_ssl, heartbeat=30)
             _LOGGER.debug("Websocket now connected")
-        except (
-            aiohttp.WSServerHandshakeError,
-            aiohttp.ClientConnectionError,
-            socket.gaierror,
-        ) as exception:
-            msg = (
-                "Error occurred while communicating with WLED device"
-                f" on WebSocket at {self.host}"
-            )
-            raise(msg)
+        except aiohttp.WSServerHandshakeError as handshake_error:
+            _LOGGER.error(f"Error occurred during websocket handshake: {handshake_error}")
+            raise
+        except aiohttp.ClientConnectionError as connection_error:
+            _LOGGER.error(f"Error connecting to the websocket server: {connection_error}")
+            raise
+        except socket.gaierror as gai_error:
+            _LOGGER.error(f"Error resolving host: {gai_error}")
+            raise
+        except Exception as e:
+            _LOGGER.error(f"An unexpected error occurred: {e}")
+            raise
         self._receiver_task = asyncio.ensure_future(self.listen())
 
     async def close(self) -> None:
         _LOGGER.debug("websocket.close() called")
         if not self._client or not self.connected:
             return
         await self._client.close()
```

### Comparing `python_swidget-1.0.1/PKG-INFO` & `python_swidget-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-swidget
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python API for Swidget smart devices
 Home-page: https://github.com/swidget/python-swidget
 License: GPL-3.0-or-later
 Author: Swidget
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -17,18 +17,20 @@
 Requires-Dist: aiohttp (>=3.8.1)
 Requires-Dist: anyio
 Requires-Dist: asyncclick (>=8)
 Requires-Dist: importlib-metadata
 Requires-Dist: m2r (>=0,<1) ; extra == "docs"
 Requires-Dist: mistune (<2.0.0) ; extra == "docs"
 Requires-Dist: pydantic (>=1,<2)
+Requires-Dist: requests (==2.31.0)
 Requires-Dist: sphinx (>=4,<5) ; extra == "docs"
 Requires-Dist: sphinx_rtd_theme (>=0,<1) ; extra == "docs"
 Requires-Dist: sphinxcontrib-programoutput (>=0,<1) ; extra == "docs"
 Requires-Dist: ssdp (==1.1.1)
+Requires-Dist: types-requests (==2.31.0.20240406)
 Project-URL: Repository, https://github.com/swidget/python-swidget
 Description-Content-Type: text/markdown
 
 # python-swidget
 A library to manage Swidget smart devices
 
 # Basic Usage
```

