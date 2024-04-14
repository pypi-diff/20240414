# Comparing `tmp/netbound-0.1.8.tar.gz` & `tmp/netbound-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbound-0.1.8.tar", last modified: Fri Mar 22 03:32:31 2024, max compression
+gzip compressed data, was "netbound-0.1.9.tar", last modified: Fri Mar 22 05:38:23 2024, max compression
```

## Comparing `netbound-0.1.8.tar` & `netbound-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 03:32:31.685914 netbound-0.1.8/
--rw-rw-rw-   0        0        0     4439 2024-03-22 03:32:31.684910 netbound-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     4242 2024-03-22 01:51:55.000000 netbound-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-22 03:32:31.603197 netbound-0.1.8/netbound/
--rw-rw-rw-   0        0        0        0 2024-03-22 01:51:55.000000 netbound-0.1.8/netbound/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-22 03:32:31.666254 netbound-0.1.8/netbound/app/
--rw-rw-rw-   0        0        0       41 2024-03-22 01:51:55.000000 netbound-0.1.8/netbound/app/__init__.py
--rw-rw-rw-   0        0        0      598 2024-03-22 01:51:55.000000 netbound-0.1.8/netbound/app/logging_adapter.py
--rw-rw-rw-   0        0        0     3891 2024-03-22 01:51:55.000000 netbound-0.1.8/netbound/app/protocol.py
--rw-rw-rw-   0        0        0     7277 2024-03-22 01:51:55.000000 netbound-0.1.8/netbound/app/server.py
--rw-rw-rw-   0        0        0       41 2024-03-22 01:51:55.000000 netbound-0.1.8/netbound/constants.py
--rw-rw-rw-   0        0        0     3468 2024-03-22 01:51:55.000000 netbound-0.1.8/netbound/packet.py
-drwxrwxrwx   0        0        0        0 2024-03-22 03:32:31.682824 netbound-0.1.8/netbound/state/
--rw-rw-rw-   0        0        0       88 2024-03-22 01:51:55.000000 netbound-0.1.8/netbound/state/__init__.py
--rw-rw-rw-   0        0        0     2795 2024-03-22 01:51:55.000000 netbound-0.1.8/netbound/state/base.py
-drwxrwxrwx   0        0        0        0 2024-03-22 03:32:31.634226 netbound-0.1.8/netbound.egg-info/
--rw-rw-rw-   0        0        0     4439 2024-03-22 03:32:31.000000 netbound-0.1.8/netbound.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2024-03-22 03:32:31.000000 netbound-0.1.8/netbound.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 03:32:31.000000 netbound-0.1.8/netbound.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      338 2024-03-22 03:32:31.000000 netbound-0.1.8/netbound.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-22 03:32:31.000000 netbound-0.1.8/netbound.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-22 03:32:31.685914 netbound-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      578 2024-03-22 03:31:00.000000 netbound-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-22 05:38:23.658347 netbound-0.1.9/
+-rw-rw-rw-   0        0        0     4439 2024-03-22 05:38:23.658347 netbound-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4242 2024-03-22 01:51:55.000000 netbound-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-03-22 05:38:23.602296 netbound-0.1.9/netbound/
+-rw-rw-rw-   0        0        0        0 2024-03-22 01:51:55.000000 netbound-0.1.9/netbound/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-22 05:38:23.645335 netbound-0.1.9/netbound/app/
+-rw-rw-rw-   0        0        0       41 2024-03-22 01:51:55.000000 netbound-0.1.9/netbound/app/__init__.py
+-rw-rw-rw-   0        0        0      598 2024-03-22 01:51:55.000000 netbound-0.1.9/netbound/app/logging_adapter.py
+-rw-rw-rw-   0        0        0     3792 2024-03-22 05:20:35.000000 netbound-0.1.9/netbound/app/protocol.py
+-rw-rw-rw-   0        0        0     9919 2024-03-22 05:29:50.000000 netbound-0.1.9/netbound/app/server.py
+-rw-rw-rw-   0        0        0      139 2024-03-22 03:43:49.000000 netbound-0.1.9/netbound/constants.py
+-rw-rw-rw-   0        0        0     4702 2024-03-22 03:53:18.000000 netbound-0.1.9/netbound/packet.py
+drwxrwxrwx   0        0        0        0 2024-03-22 05:38:23.656345 netbound-0.1.9/netbound/state/
+-rw-rw-rw-   0        0        0       88 2024-03-22 01:51:55.000000 netbound-0.1.9/netbound/state/__init__.py
+-rw-rw-rw-   0        0        0     5395 2024-03-22 05:20:04.000000 netbound-0.1.9/netbound/state/base.py
+drwxrwxrwx   0        0        0        0 2024-03-22 05:38:23.623315 netbound-0.1.9/netbound.egg-info/
+-rw-rw-rw-   0        0        0     4439 2024-03-22 05:38:23.000000 netbound-0.1.9/netbound.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2024-03-22 05:38:23.000000 netbound-0.1.9/netbound.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-22 05:38:23.000000 netbound-0.1.9/netbound.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      338 2024-03-22 05:38:23.000000 netbound-0.1.9/netbound.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-03-22 05:38:23.000000 netbound-0.1.9/netbound.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-03-22 05:38:23.659347 netbound-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      578 2024-03-22 05:37:49.000000 netbound-0.1.9/setup.py
```

### Comparing `netbound-0.1.8/PKG-INFO` & `netbound-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbound
-Version: 0.1.8
+Version: 0.1.9
 Home-page: https://github.com/tristanbatchler/netbound
 Author: Tristan Batchler
 License: MIT
 Description-Content-Type: text/markdown
 
 # Netbound
 A safe and fair way to play games with friends over the internet
```

### Comparing `netbound-0.1.8/README.md` & `netbound-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `netbound-0.1.8/netbound/app/logging_adapter.py` & `netbound-0.1.9/netbound/app/logging_adapter.py`

 * *Files identical despite different names*

### Comparing `netbound-0.1.8/netbound/app/protocol.py` & `netbound-0.1.9/netbound/app/protocol.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,29 +6,28 @@
 from netbound.state import BaseState
 from sqlalchemy.ext.asyncio import async_sessionmaker
 from typing import Callable, Coroutine, Any, Optional
 from netbound.constants import EVERYONE
 from base64 import b64encode
 from netbound.app.logging_adapter import ProtocolLoggingAdapter
 
-class GameProtocol:
+class _GameProtocol:
     def __init__(
             self, 
             websocket: ws.WebSocketServerProtocol, 
             pid: bytes, 
-            disconnect_callback: Callable[[GameProtocol, str], Coroutine[Any, Any, None]], 
+            disconnect_callback: Callable[[_GameProtocol, str], Coroutine[Any, Any, None]], 
             db_session_callback: async_sessionmaker
         ) -> None:
-        """WARNING: This class must only be instantiated from within the server.app.ServerApp class"""
         self._websocket: ws.WebSocketServerProtocol = websocket
         self._pid: bytes = pid
         self._local_receive_packet_queue: asyncio.Queue[BasePacket] = asyncio.Queue()
         self._local_protos_send_packet_queue: asyncio.Queue[BasePacket] = asyncio.Queue()
         self._local_client_send_packet_queue: asyncio.Queue[BasePacket] = asyncio.Queue()
-        self._disconnect: Callable[[GameProtocol, str], Coroutine[Any, Any, None]] = disconnect_callback
+        self._disconnect: Callable[[_GameProtocol, str], Coroutine[Any, Any, None]] = disconnect_callback
         self._get_db_session: async_sessionmaker = db_session_callback
         self._state: Optional[BaseState] = None
         self._logger: ProtocolLoggingAdapter = ProtocolLoggingAdapter(logging.getLogger(__name__), {
             'pid': pid
         })
 
     def __repr__(self) -> str:
@@ -71,15 +70,15 @@
             await self._local_receive_packet_queue.put(p)
 
         self._logger.debug(f"{self} stopped")
         await self._disconnect(self, "Client disconnected")
 
     async def _change_state(self, new_state: BaseState, previous_state_view: Optional[BaseState.View]=None) -> None:
         self._state = new_state
-        await self._state.on_transition(previous_state_view)
+        await self._state._on_transition(previous_state_view)
 
     async def _process_packets(self) -> None:
         while not self._local_receive_packet_queue.empty():
             p: BasePacket = await self._local_receive_packet_queue.get()
             if self._state:
-                await self._state.handle_packet(p)
+                await self._state._handle_packet(p)
             self._logger.debug(f"Processed packet: {p}")
```

### Comparing `netbound-0.1.8/netbound/packet.py` & `netbound-0.1.9/netbound/packet.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,43 @@
 import msgpack
 from netbound.constants import EVERYONE
 from pydantic import BaseModel, ValidationError
 from typing import Any, Type, Optional
 import base64
+from abc import ABC
+
+class BasePacket(BaseModel, ABC):
+    """
+    The base packet class. All user-defined packets must inherit from this class.
+    """
 
-class BasePacket(BaseModel):
     from_pid: bytes
-    # If to_pid is None, it is either from the client to its protocol or vice-versa
+    """
+    The PID of the protocol that sent this packet.
+    """
+
     to_pid: Optional[bytes | list[Optional[bytes]]] = None
+    """
+    The PID, or PIDs, of the protocol(s) that this packet is intended for. If left as `None`, it 
+    the packet will be sent to the sender's own client (if the sender is a protocol) or to the 
+    sender's own protocol (if the sender is a client).
+    """
+
     exclude_sender: Optional[bool] = False
+    """
+    If `to_pid` is the special PID `EVERYONE`, this flag can be set to `True` to exclude the sender 
+    from the list of recipients. This can be useful to avoid infinite loops when broadcasting 
+    packets.
+    """
 
     def serialize(self) -> bytes:
+        """
+        Converts the packet to a MessagePack-encoded byte string to be sent over the network. The 
+        PID values are sent as base64-encoded strings.
+        """
         data = {}
         packet_name = self.__class__.__name__.removesuffix("Packet").title()
         m_dump = self.model_dump()
 
         data[packet_name] = m_dump
         return msgpack.packb(data, use_bin_type=True)
     
@@ -39,26 +62,36 @@
             d[TO_PID] = base64.b64encode(self.to_pid).decode()
         return f"{self.__class__.__name__}{d}"
     
     def __str__(self) -> str:
         return self.__repr__()
     
 class DisconnectPacket(BasePacket):
+    """
+    A packet that is broadcasted to all protocols when one protocol disconnects from the server.
+    """
     reason: str
 
 class MalformedPacketError(ValueError):
     pass
 
 class UnknownPacketError(ValueError):
     pass
 
 def register_packet(packet: Type[BasePacket]) -> None:
+    """
+    Injects a user-defined packet into the engine's global namespace so that it can be deserialized.
+    """
     globals()[packet.__name__] = packet
 
 def deserialize(packet_: bytes) -> BasePacket:
+    """
+    Converts a MessagePack-encoded byte string to a packet object. The returned object will be an 
+    instance of the specific packet class that the packet data corresponds to.
+    """
     try:
         packet_dict: dict[str, Any] = msgpack.unpackb(packet_, raw=False)
     except msgpack.StackError:
         raise MalformedPacketError("Packet too nested to unpack")
     except msgpack.ExtraData:
         raise MalformedPacketError("Extra data was sent with the packet")
     except msgpack.FormatError:
```

### Comparing `netbound-0.1.8/netbound.egg-info/PKG-INFO` & `netbound-0.1.9/netbound.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbound
-Version: 0.1.8
+Version: 0.1.9
 Home-page: https://github.com/tristanbatchler/netbound
 Author: Tristan Batchler
 License: MIT
 Description-Content-Type: text/markdown
 
 # Netbound
 A safe and fair way to play games with friends over the internet
```

### Comparing `netbound-0.1.8/setup.py` & `netbound-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 dependencies = (this_directory / "requirements.txt").read_text().splitlines()
 
 setup(
     name='netbound',
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(),
     url='https://github.com/tristanbatchler/netbound',
     install_requires=dependencies,
     license='MIT',
     author='Tristan Batchler',
     long_description=long_description,
     long_description_content_type='text/markdown'
```

