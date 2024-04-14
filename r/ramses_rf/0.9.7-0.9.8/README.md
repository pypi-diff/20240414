# Comparing `tmp/ramses-rf-0.9.7.tar.gz` & `tmp/ramses-rf-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramses-rf-0.9.7.tar", last modified: Thu May 20 20:47:16 2021, max compression
+gzip compressed data, was "ramses-rf-0.9.8.tar", last modified: Sat May 22 18:46:56 2021, max compression
```

## Comparing `ramses-rf-0.9.7.tar` & `ramses-rf-0.9.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-20 20:47:16.358146 ramses-rf-0.9.7/
--rw-r--r--   0 root         (0) root         (0)     1069 2021-05-20 20:47:11.000000 ramses-rf-0.9.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3127 2021-05-20 20:47:16.358146 ramses-rf-0.9.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2096 2021-05-20 20:47:11.000000 ramses-rf-0.9.7/README.md
--rw-r--r--   0 root         (0) root         (0)       57 2021-05-20 20:47:11.000000 ramses-rf-0.9.7/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-20 20:47:16.358146 ramses-rf-0.9.7/ramses_rf/
--rw-r--r--   0 root         (0) root         (0)    15006 2021-05-20 20:47:11.000000 ramses-rf-0.9.7/ramses_rf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3202 2021-05-20 20:47:11.000000 ramses-rf-0.9.7/ramses_rf/address.py
--rw-r--r--   0 root         (0) root         (0)    37324 2021-05-20 20:47:11.000000 ramses-rf-0.9.7/ramses_rf/command.py
--rw-r--r--   0 root         (0) root         (0)    16649 2021-05-20 20:47:11.000000 ramses-rf-0.9.7/ramses_rf/const.py
--rw-r--r--   0 root         (0) root         (0)    43908 2021-05-20 20:47:11.000000 ramses-rf-0.9.7/ramses_rf/devices.py
--rw-r--r--   0 root         (0) root         (0)    10777 2021-05-20 20:47:11.000000 ramses-rf-0.9.7/ramses_rf/discovery.py
--rw-r--r--   0 root         (0) root         (0)     3127 2021-05-20 20:47:11.000000 ramses-rf-0.9.7/ramses_rf/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     9112 2021-05-20 20:47:11.000000 ramses-rf-0.9.7/ramses_rf/helpers.py
--rw-r--r--   0 root         (0) root         (0)    26742 2021-05-20 20:47:11.000000 ramses-rf-0.9.7/ramses_rf/message.py
--rw-r--r--   0 root         (0) root         (0)    30183 2021-05-20 20:47:11.000000 ramses-rf-0.9.7/ramses_rf/opentherm.py
--rw-r--r--   0 root         (0) root         (0)     9356 2021-05-20 20:47:11.000000 ramses-rf-0.9.7/ramses_rf/packet.py
--rw-r--r--   0 root         (0) root         (0)    69217 2021-05-20 20:47:11.000000 ramses-rf-0.9.7/ramses_rf/parsers.py
--rw-r--r--   0 root         (0) root         (0)    17446 2021-05-20 20:47:11.000000 ramses-rf-0.9.7/ramses_rf/protocol.py
--rw-r--r--   0 root         (0) root         (0)    19784 2021-05-20 20:47:11.000000 ramses-rf-0.9.7/ramses_rf/ramses.py
--rw-r--r--   0 root         (0) root         (0)    13574 2021-05-20 20:47:11.000000 ramses-rf-0.9.7/ramses_rf/schema.py
--rw-r--r--   0 root         (0) root         (0)    36259 2021-05-20 20:47:11.000000 ramses-rf-0.9.7/ramses_rf/systems.py
--rw-r--r--   0 root         (0) root         (0)    29817 2021-05-20 20:47:11.000000 ramses-rf-0.9.7/ramses_rf/transport.py
--rw-r--r--   0 root         (0) root         (0)      131 2021-05-20 20:47:11.000000 ramses-rf-0.9.7/ramses_rf/version.py
--rw-r--r--   0 root         (0) root         (0)    33158 2021-05-20 20:47:11.000000 ramses-rf-0.9.7/ramses_rf/zones.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-20 20:47:16.358146 ramses-rf-0.9.7/ramses_rf.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3127 2021-05-20 20:47:16.000000 ramses-rf-0.9.7/ramses_rf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      608 2021-05-20 20:47:16.000000 ramses-rf-0.9.7/ramses_rf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-05-20 20:47:16.000000 ramses-rf-0.9.7/ramses_rf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2021-05-20 20:47:16.000000 ramses-rf-0.9.7/ramses_rf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2021-05-20 20:47:16.000000 ramses-rf-0.9.7/ramses_rf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-05-20 20:47:16.358146 ramses-rf-0.9.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1792 2021-05-20 20:47:11.000000 ramses-rf-0.9.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-22 18:46:56.073027 ramses-rf-0.9.8/
+-rw-r--r--   0 root         (0) root         (0)     1069 2021-05-22 18:46:51.000000 ramses-rf-0.9.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3127 2021-05-22 18:46:56.073027 ramses-rf-0.9.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2096 2021-05-22 18:46:51.000000 ramses-rf-0.9.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       57 2021-05-22 18:46:51.000000 ramses-rf-0.9.8/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-22 18:46:56.073027 ramses-rf-0.9.8/ramses_rf/
+-rw-r--r--   0 root         (0) root         (0)    14860 2021-05-22 18:46:51.000000 ramses-rf-0.9.8/ramses_rf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3202 2021-05-22 18:46:51.000000 ramses-rf-0.9.8/ramses_rf/address.py
+-rw-r--r--   0 root         (0) root         (0)    37324 2021-05-22 18:46:51.000000 ramses-rf-0.9.8/ramses_rf/command.py
+-rw-r--r--   0 root         (0) root         (0)    16649 2021-05-22 18:46:51.000000 ramses-rf-0.9.8/ramses_rf/const.py
+-rw-r--r--   0 root         (0) root         (0)    43908 2021-05-22 18:46:51.000000 ramses-rf-0.9.8/ramses_rf/devices.py
+-rw-r--r--   0 root         (0) root         (0)    10777 2021-05-22 18:46:51.000000 ramses-rf-0.9.8/ramses_rf/discovery.py
+-rw-r--r--   0 root         (0) root         (0)     3127 2021-05-22 18:46:51.000000 ramses-rf-0.9.8/ramses_rf/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     9112 2021-05-22 18:46:51.000000 ramses-rf-0.9.8/ramses_rf/helpers.py
+-rw-r--r--   0 root         (0) root         (0)    26742 2021-05-22 18:46:51.000000 ramses-rf-0.9.8/ramses_rf/message.py
+-rw-r--r--   0 root         (0) root         (0)    30183 2021-05-22 18:46:51.000000 ramses-rf-0.9.8/ramses_rf/opentherm.py
+-rw-r--r--   0 root         (0) root         (0)     9356 2021-05-22 18:46:51.000000 ramses-rf-0.9.8/ramses_rf/packet.py
+-rw-r--r--   0 root         (0) root         (0)    69217 2021-05-22 18:46:51.000000 ramses-rf-0.9.8/ramses_rf/parsers.py
+-rw-r--r--   0 root         (0) root         (0)    17654 2021-05-22 18:46:51.000000 ramses-rf-0.9.8/ramses_rf/protocol.py
+-rw-r--r--   0 root         (0) root         (0)    19784 2021-05-22 18:46:51.000000 ramses-rf-0.9.8/ramses_rf/ramses.py
+-rw-r--r--   0 root         (0) root         (0)    14607 2021-05-22 18:46:51.000000 ramses-rf-0.9.8/ramses_rf/schema.py
+-rw-r--r--   0 root         (0) root         (0)    36259 2021-05-22 18:46:51.000000 ramses-rf-0.9.8/ramses_rf/systems.py
+-rw-r--r--   0 root         (0) root         (0)    30325 2021-05-22 18:46:51.000000 ramses-rf-0.9.8/ramses_rf/transport.py
+-rw-r--r--   0 root         (0) root         (0)      131 2021-05-22 18:46:51.000000 ramses-rf-0.9.8/ramses_rf/version.py
+-rw-r--r--   0 root         (0) root         (0)    33158 2021-05-22 18:46:51.000000 ramses-rf-0.9.8/ramses_rf/zones.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-22 18:46:56.073027 ramses-rf-0.9.8/ramses_rf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3127 2021-05-22 18:46:55.000000 ramses-rf-0.9.8/ramses_rf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      608 2021-05-22 18:46:55.000000 ramses-rf-0.9.8/ramses_rf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2021-05-22 18:46:55.000000 ramses-rf-0.9.8/ramses_rf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2021-05-22 18:46:55.000000 ramses-rf-0.9.8/ramses_rf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2021-05-22 18:46:55.000000 ramses-rf-0.9.8/ramses_rf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2021-05-22 18:46:56.073027 ramses-rf-0.9.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1792 2021-05-22 18:46:51.000000 ramses-rf-0.9.8/setup.py
```

### Comparing `ramses-rf-0.9.7/LICENSE` & `ramses-rf-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ramses-rf-0.9.7/PKG-INFO` & `ramses-rf-0.9.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ramses-rf
-Version: 0.9.7
+Version: 0.9.8
 Summary: An interface for the RAMSES RF protocol,         as used by Honeywell-compatible HVAC & CH/DHW systems.     
 Home-page: https://github.com/zxdavb/ramses_rf
 Author: David Bonnes
 Author-email: zxdavb@gmail.com
 License: MIT
-Download-URL: https://github.com/zxdavb/ramses_rf/archive/0.9.7.tar.gz
+Download-URL: https://github.com/zxdavb/ramses_rf/archive/0.9.8.tar.gz
 Description: [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![CircleCI](https://circleci.com/gh/zxdavb/ramses_rf.svg?style=svg)](https://circleci.com/gh/zxdavb/ramses_rf) [![Join the chat at https://gitter.im/evohome_rf/community](https://badges.gitter.im/evohome_rf/community.svg)](https://gitter.im/evohome_rf/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
         
         ## Overview
         **ramses_rf** is a client library/CLI utility used to interface with some Honeywell-compatible HVAC & CH/DHW systems that use 868MHz RF, such as **evohome**, **Sundial**, **Hometronic**, **Chronotherm** and many others.
         
         It requires a USB-to-RF device, either a Honeywell HGI80 (somewhat rare, expensive) or something running the [evofw3](https://github.com/ghoti57/evofw3) firmware, such as the one from [here](https://indalo-tech.onlineweb.shop/).
```

### Comparing `ramses-rf-0.9.7/README.md` & `ramses-rf-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `ramses-rf-0.9.7/ramses_rf/__init__.py` & `ramses-rf-0.9.8/ramses_rf/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 """
 
 import asyncio
 import json
 import logging
 import os
 import signal
-from collections import deque
-from threading import Lock
 from typing import Callable, Dict, List, Optional, Tuple
 
 from .command import Command
 from .const import ATTR_DEVICES, ATTR_ORPHANS, NUL_DEVICE_ID, __dev_mode__
 from .devices import DEVICE_CLASSES, Device
 from .message import Message, process_msg
 from .packet import set_pkt_logging
@@ -83,20 +81,17 @@
 
         # if self.config[REDUCE_PROCESSING] >= DONT_CREATE_MESSAGES:
         #     return
 
         if self.config[REDUCE_PROCESSING] < DONT_CREATE_MESSAGES:
             self.msg_protocol, self.msg_transport = self.create_client(process_msg)
 
-        self._buffer = deque()
-        self._sched_zone = None
-        self._sched_lock = Lock()
-
-        # if config.get("ser2net_server"):
-        self._relay = None  # ser2net_server relay
+        # self._buffer = deque()
+        # self._sched_zone = None
+        # self._sched_lock = Lock()
 
         # if self.config[REDUCE_PROCESSING] > 0:
         self.rfg = None
         self.evo = None
         self.systems: List[SystemBase] = []
         self.system_by_id: Dict = {}
         self.devices: List[Device] = []
```

### Comparing `ramses-rf-0.9.7/ramses_rf/address.py` & `ramses-rf-0.9.8/ramses_rf/address.py`

 * *Files identical despite different names*

### Comparing `ramses-rf-0.9.7/ramses_rf/command.py` & `ramses-rf-0.9.8/ramses_rf/command.py`

 * *Files identical despite different names*

### Comparing `ramses-rf-0.9.7/ramses_rf/const.py` & `ramses-rf-0.9.8/ramses_rf/const.py`

 * *Files identical despite different names*

### Comparing `ramses-rf-0.9.7/ramses_rf/devices.py` & `ramses-rf-0.9.8/ramses_rf/devices.py`

 * *Files identical despite different names*

### Comparing `ramses-rf-0.9.7/ramses_rf/discovery.py` & `ramses-rf-0.9.8/ramses_rf/discovery.py`

 * *Files identical despite different names*

### Comparing `ramses-rf-0.9.7/ramses_rf/exceptions.py` & `ramses-rf-0.9.8/ramses_rf/exceptions.py`

 * *Files identical despite different names*

### Comparing `ramses-rf-0.9.7/ramses_rf/helpers.py` & `ramses-rf-0.9.8/ramses_rf/helpers.py`

 * *Files identical despite different names*

### Comparing `ramses-rf-0.9.7/ramses_rf/message.py` & `ramses-rf-0.9.8/ramses_rf/message.py`

 * *Files identical despite different names*

### Comparing `ramses-rf-0.9.7/ramses_rf/opentherm.py` & `ramses-rf-0.9.8/ramses_rf/opentherm.py`

 * *Files identical despite different names*

### Comparing `ramses-rf-0.9.7/ramses_rf/packet.py` & `ramses-rf-0.9.8/ramses_rf/packet.py`

 * *Files identical despite different names*

### Comparing `ramses-rf-0.9.7/ramses_rf/parsers.py` & `ramses-rf-0.9.8/ramses_rf/parsers.py`

 * *Files identical despite different names*

### Comparing `ramses-rf-0.9.7/ramses_rf/protocol.py` & `ramses-rf-0.9.8/ramses_rf/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,22 +143,25 @@
         if _LOGGER.getEffectiveLevel() == logging.INFO:  # i.e. don't log for DEBUG
             _LOGGER.info("rcvd: %s", pkt)
 
         for (
             hdr,
             callback,
         ) in self._callbacks.items():  # 1st, notify all expired callbacks
-            if callback.get(EXPIRES, dt.max) < pkt._dtm:
+            if callback.get(EXPIRES, dt.max) < pkt._dtm and not callback.get("expired"):
+                # see  also: PktProtocolQos.send_data()
                 _LOGGER.error("MsgTransport._pkt_receiver(%s): Expired callback", hdr)
                 callback[FUNC](False, *callback.get(ARGS, tuple()))
+                callback["expired"] = not callback.get(DEAMON, False)
 
         self._callbacks = {  # 2nd, discard any expired callbacks
             hdr: callback
             for hdr, callback in self._callbacks.items()
-            if callback.get(DEAMON) or callback[EXPIRES] >= pkt._dtm
+            if callback.get(DEAMON)
+            or (callback[EXPIRES] >= pkt._dtm and not not callback.get("expired"))
         }
 
         if len(self._protocols) == 0:
             return
 
         if self._gwy.config[REDUCE_PROCESSING] >= DONT_CREATE_MESSAGES:
             return
```

### Comparing `ramses-rf-0.9.7/ramses_rf/ramses.py` & `ramses-rf-0.9.8/ramses_rf/ramses.py`

 * *Files identical despite different names*

### Comparing `ramses-rf-0.9.7/ramses_rf/schema.py` & `ramses-rf-0.9.8/ramses_rf/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 """RAMSES RF - Schema processor."""
 
 import logging
 import re
-from typing import Tuple
+from typing import Any, Optional, Tuple
 
 import voluptuous as vol
 
 from .const import ALL_DEVICE_ID as DEVICE_ID_REGEX
 from .const import (
     ATTR_CONTROLLER,
     ATTR_DEVICES,
@@ -245,15 +245,15 @@
 
 _LOGGER = logging.getLogger(__name__)
 if DEV_MODE:
     _LOGGER.setLevel(logging.DEBUG)
 
 
 def load_config_schema(serial_port, input_file, **kwargs) -> Tuple[dict, list, list]:
-    """Process the schema, and the configuration and return True if it is valid."""
+    """Process the configuration, including any filter lists."""
 
     kwargs = GLOBAL_CONFIG_SCHEMA(kwargs)
 
     allow_list = kwargs.pop(ALLOW_LIST)
     block_list = kwargs.pop(BLOCK_LIST)
 
     config = CONFIG_SCHEMA.extend(
@@ -323,98 +323,127 @@
     # block_list = (
     #     list(block_list.keys()) if config[ENFORCE_BLOCKLIST] else []
     # )
 
     return (config, allow_list, block_list)
 
 
+def _get_device(gwy, dev_addr, ctl_addr=None, **kwargs) -> Optional[Any]:
+    """A wrapper to enforce device filters."""
+    err_msg = None
+
+    if gwy.config[ENFORCE_ALLOWLIST]:
+        if ctl_addr and ctl_addr.id not in gwy._include:
+            err_msg = f"{ctl_addr.id} is in the schema, but is not in the allow list"
+        elif dev_addr.id not in gwy._include:
+            err_msg = f"{dev_addr.id} is in the schema, but is not in the allow list"
+
+    elif gwy.config[ENFORCE_BLOCKLIST]:
+        if ctl_addr and ctl_addr.id in gwy._exclude:
+            err_msg = f"{ctl_addr.id} is in the schema, but is also in the block list"
+        elif dev_addr.id not in gwy._include:
+            err_msg = f"{dev_addr.id} is in the schema, but is also in the block list"
+
+    if not err_msg:
+        return gwy._get_device(dev_addr, ctl_addr=None, **kwargs)
+
+    _LOGGER.warning("%s: check the lists and the (cached) schema", err_msg)
+
+
 def load_system_schema(gwy, **kwargs) -> dict:
     """Process the schema, and the configuration and return True if it is valid."""
     # TODO: check a sensor is not a device in another zone
 
     gwy._clear_state()  # TODO: consider need for this (here, or at all)
 
     known_devices = kwargs.pop(ALLOW_LIST, {})
     known_devices.update(kwargs.pop(BLOCK_LIST, {}))
 
-    [gwy._get_device(addr(device_id)) for device_id in kwargs.pop(ATTR_ORPHANS, [])]
+    [_get_device(gwy, addr(device_id)) for device_id in kwargs.pop(ATTR_ORPHANS, [])]
 
     if SCHEMA in kwargs:
         _load_system_schema(gwy, kwargs[SCHEMA])
-        gwy.evo = gwy.system_by_id[kwargs[SCHEMA][ATTR_CONTROLLER]]
+        gwy.evo = gwy.system_by_id.get(kwargs[SCHEMA][ATTR_CONTROLLER])
 
     elif kwargs.get(MAIN_CONTROLLER):
         [
             _load_system_schema(gwy, schema)
             for k, schema in kwargs.items()
             if re.match(DEVICE_ID_REGEX, k)
         ]
-        gwy.evo = gwy.system_by_id[kwargs[MAIN_CONTROLLER]]
+        gwy.evo = gwy.system_by_id.get(kwargs[MAIN_CONTROLLER])
 
     return {
         **known_devices,
         **{d: None for d in gwy.device_by_id if d not in known_devices},
     }
 
 
 def _load_system_schema(gwy, schema) -> Tuple[dict, dict]:
     schema = SYSTEM_SCHEMA(schema)
 
     ctl_id = schema[ATTR_CONTROLLER]
     profile = schema[ATTR_HTG_SYSTEM].get(ATTR_SYS_PROFILE)
-    ctl = gwy._get_device(addr(ctl_id), ctl_addr=addr(ctl_id), profile=profile)
+    ctl = _get_device(gwy, addr(ctl_id), ctl_addr=addr(ctl_id), profile=profile)
+
+    if not ctl:
+        return
 
     htg_ctl_id = schema[ATTR_HTG_SYSTEM].get(ATTR_HTG_CONTROL)
     if htg_ctl_id:
-        ctl._evo._set_htg_control(gwy._get_device(addr(htg_ctl_id), ctl_addr=ctl))
+        ctl._evo._set_htg_control(_get_device(gwy, addr(htg_ctl_id), ctl_addr=ctl))
 
     dhw = schema.get(ATTR_DHW_SYSTEM, {})
     if dhw:
         ctl._evo._set_dhw(ctl._evo._get_zone("HW"))
 
         dhw_sensor_id = dhw.get(ATTR_DHW_SENSOR)
         if dhw_sensor_id:
-            ctl._evo.dhw._set_sensor(gwy._get_device(addr(dhw_sensor_id), ctl_addr=ctl))
+            ctl._evo.dhw._set_sensor(
+                _get_device(gwy, addr(dhw_sensor_id), ctl_addr=ctl)
+            )
 
         dhw_valve_id = dhw.get(ATTR_DHW_VALVE)
         if dhw_valve_id:
             ctl._evo.dhw._set_dhw_valve(
-                gwy._get_device(addr(dhw_valve_id), ctl_addr=ctl)
+                _get_device(gwy, addr(dhw_valve_id), ctl_addr=ctl)
             )
 
         htg_valve_id = dhw.get(ATTR_DHW_VALVE_HTG)
         if htg_valve_id:
             ctl._evo.dhw._set_htg_valve(
-                gwy._get_device(addr(htg_valve_id), ctl_addr=ctl)
+                _get_device(gwy, addr(htg_valve_id), ctl_addr=ctl)
             )
 
     for zone_idx, attr in schema[ATTR_ZONES].items():
         zone = ctl._evo._get_zone(zone_idx, zone_type=attr.get(ATTR_ZONE_TYPE))
 
         sensor_id = attr.get(ATTR_ZONE_SENSOR)
         is_faked = None
         if isinstance(sensor_id, dict):
             is_faked = sensor_id.get("is_faked")
             sensor_id = sensor_id[ATTR_DEVICE_ID]
 
         if sensor_id:
             zone._set_sensor(
-                gwy._get_device(addr(sensor_id), ctl_addr=ctl, domain_id=zone_idx)
+                _get_device(gwy, addr(sensor_id), ctl_addr=ctl, domain_id=zone_idx)
             )  # TODO: use domain_id=zone_idx or not
 
         if is_faked:
             zone.sensor._make_fake()
 
         for device_id in attr.get(ATTR_DEVICES, []):
-            gwy._get_device(addr(device_id), ctl_addr=ctl, domain_id=zone_idx)
+            _get_device(gwy, addr(device_id), ctl_addr=ctl, domain_id=zone_idx)
 
     # TODO: not create orphans by default?
     orphan_ids = schema.get(ATTR_ORPHANS, [])
     if orphan_ids:
-        [gwy._get_device(addr(device_id), ctl_addr=ctl) for device_id in orphan_ids]
+        [_get_device(gwy, addr(device_id), ctl_addr=ctl) for device_id in orphan_ids]
 
     ufh_ctl_ids = schema.get(ATTR_UFH_SYSTEM, {})
     if ufh_ctl_ids:
         for ufc_id, _ in ufh_ctl_ids.items():
-            _ = gwy._get_device(addr(ufc_id), ctl_addr=ctl)
+            _ = _get_device(gwy, addr(ufc_id), ctl_addr=ctl)
 
     # assert schema == gwy.system_by_id[ctl_id].schema
+
+    # return ctl._evo
```

### Comparing `ramses-rf-0.9.7/ramses_rf/systems.py` & `ramses-rf-0.9.8/ramses_rf/systems.py`

 * *Files identical despite different names*

### Comparing `ramses-rf-0.9.7/ramses_rf/transport.py` & `ramses-rf-0.9.8/ramses_rf/transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 from types import SimpleNamespace
 from typing import ByteString, Callable, Optional, Tuple
 
 from serial import SerialException, serial_for_url
 from serial_asyncio import SerialTransport as SerialTransportAsync
 
 from .command import (
+    ARGS,
+    DEAMON,
+    FUNC,
     QOS_MAX_BACKOFF,
     QOS_RX_TIMEOUT,
     QOS_TX_RETRIES,
     QOS_TX_TIMEOUT,
     Command,
     Priority,
 )
@@ -695,14 +698,22 @@
                 cmd.tx_header,
                 self._backoff,
                 self._tx_hdr or self._rx_hdr,
                 self._timeout_full,
                 message,
             )
 
+        def _expired_cmd(cmd):
+            hdr, callback = cmd.tx_header, cmd.callback
+            if callback and not callback.get("expired"):
+                # see also: MsgTransport._pkt_receiver()
+                _LOGGER.error("PktProtocolQos.send_data(%s): Expired callback", hdr)
+                callback[FUNC](False, *callback.get(ARGS, tuple()))
+                callback["expired"] = not callback.get(DEAMON, False)
+
         if self._gwy.config[DISABLE_SENDING]:
             raise RuntimeError("Sending is disabled")
 
         if not cmd.is_valid:
             _LOGGER.warning(
                 "PktProtocolQos.send_data(%s): invalid command: %s", cmd.tx_header, cmd
             )
@@ -748,15 +759,17 @@
                 _logger_send(
                     _LOGGER.warning,
                     f"RE-SENT ({self._tx_retries}/{self._tx_retry_limit})",
                 )  # TODO: should be info/debug
 
             else:
                 if self._qos_cmd.code != "7FFF":  # HACK: why expired when shouldn't
-                    _logger_send(_LOGGER.error, "EXPIRED")
+                    _logger_send(_LOGGER.warning, "EXPIRED")
+                    _expired_cmd(self._qos_cmd)
+
                 self._qos_lock.acquire()
                 self._qos_cmd = None
                 self._qos_lock.release()
                 self._backoff = 0  # TODO: need a better system
                 break
 
         else:
```

### Comparing `ramses-rf-0.9.7/ramses_rf/zones.py` & `ramses-rf-0.9.8/ramses_rf/zones.py`

 * *Files identical despite different names*

### Comparing `ramses-rf-0.9.7/ramses_rf.egg-info/PKG-INFO` & `ramses-rf-0.9.8/ramses_rf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: ramses-rf
-Version: 0.9.7
+Version: 0.9.8
 Summary: An interface for the RAMSES RF protocol,         as used by Honeywell-compatible HVAC & CH/DHW systems.     
 Home-page: https://github.com/zxdavb/ramses_rf
 Author: David Bonnes
 Author-email: zxdavb@gmail.com
 License: MIT
-Download-URL: https://github.com/zxdavb/ramses_rf/archive/0.9.7.tar.gz
+Download-URL: https://github.com/zxdavb/ramses_rf/archive/0.9.8.tar.gz
 Description: [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![CircleCI](https://circleci.com/gh/zxdavb/ramses_rf.svg?style=svg)](https://circleci.com/gh/zxdavb/ramses_rf) [![Join the chat at https://gitter.im/evohome_rf/community](https://badges.gitter.im/evohome_rf/community.svg)](https://gitter.im/evohome_rf/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
         
         ## Overview
         **ramses_rf** is a client library/CLI utility used to interface with some Honeywell-compatible HVAC & CH/DHW systems that use 868MHz RF, such as **evohome**, **Sundial**, **Hometronic**, **Chronotherm** and many others.
         
         It requires a USB-to-RF device, either a Honeywell HGI80 (somewhat rare, expensive) or something running the [evofw3](https://github.com/ghoti57/evofw3) firmware, such as the one from [here](https://indalo-tech.onlineweb.shop/).
```

### Comparing `ramses-rf-0.9.7/ramses_rf.egg-info/SOURCES.txt` & `ramses-rf-0.9.8/ramses_rf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ramses-rf-0.9.7/setup.py` & `ramses-rf-0.9.8/setup.py`

 * *Files identical despite different names*

