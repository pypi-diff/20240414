# Comparing `tmp/exchanges_wrapper-2.1.8.tar.gz` & `tmp/exchanges_wrapper-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchanges_wrapper-2.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "exchanges_wrapper-2.1.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `exchanges_wrapper-2.1.8.tar` & `exchanges_wrapper-2.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1114 2024-04-08 17:59:39.823769 exchanges_wrapper-2.1.8/LICENSE.md
--rw-r--r--   0        0        0     7003 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/README.md
--rwxr-xr-x   0        0        0     1516 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/__init__.py
--rw-r--r--   0        0        0    78383 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/client.py
--rw-r--r--   0        0        0     2768 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/definitions.py
--rw-r--r--   0        0        0      796 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/errors.py
--rw-r--r--   0        0        0    12512 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/events.py
--rwxr-xr-x   0        0        0    36649 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/exch_srv.py
--rw-r--r--   0        0        0     5597 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/exch_srv_cfg.toml.template
--rw-r--r--   0        0        0    13216 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/http_client.py
--rwxr-xr-x   0        0        0     2500 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/lib.py
--rw-r--r--   0        0        0    53745 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/martin/__init__.py
--rw-r--r--   0        0        0    19230 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/parsers/bitfinex_parser.py
--rw-r--r--   0        0        0    16028 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/parsers/bybit_parser.py
--rw-r--r--   0        0        0    14390 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/parsers/huobi_parser.py
--rw-r--r--   0        0        0    16228 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/parsers/okx_parser.py
--rw-r--r--   0        0        0    10683 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/proto/martin.proto
--rw-r--r--   0        0        0    27755 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/exchanges_wrapper/web_sockets.py
--rw-r--r--   0        0        0     1227 2024-04-08 17:59:39.827769 exchanges_wrapper-2.1.8/pyproject.toml
--rw-r--r--   0        0        0     8020 1970-01-01 00:00:00.000000 exchanges_wrapper-2.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1114 2024-04-14 17:09:33.649731 exchanges_wrapper-2.1.9/LICENSE.md
+-rw-r--r--   0        0        0     7003 2024-04-14 17:09:33.649731 exchanges_wrapper-2.1.9/README.md
+-rwxr-xr-x   0        0        0     1516 2024-04-14 17:09:33.649731 exchanges_wrapper-2.1.9/exchanges_wrapper/__init__.py
+-rw-r--r--   0        0        0    78521 2024-04-14 17:09:33.649731 exchanges_wrapper-2.1.9/exchanges_wrapper/client.py
+-rw-r--r--   0        0        0     2768 2024-04-14 17:09:33.649731 exchanges_wrapper-2.1.9/exchanges_wrapper/definitions.py
+-rw-r--r--   0        0        0      796 2024-04-14 17:09:33.649731 exchanges_wrapper-2.1.9/exchanges_wrapper/errors.py
+-rw-r--r--   0        0        0    12208 2024-04-14 17:09:33.653731 exchanges_wrapper-2.1.9/exchanges_wrapper/events.py
+-rwxr-xr-x   0        0        0    36880 2024-04-14 17:09:33.653731 exchanges_wrapper-2.1.9/exchanges_wrapper/exch_srv.py
+-rw-r--r--   0        0        0     5597 2024-04-14 17:09:33.653731 exchanges_wrapper-2.1.9/exchanges_wrapper/exch_srv_cfg.toml.template
+-rw-r--r--   0        0        0    13216 2024-04-14 17:09:33.653731 exchanges_wrapper-2.1.9/exchanges_wrapper/http_client.py
+-rwxr-xr-x   0        0        0     2500 2024-04-14 17:09:33.653731 exchanges_wrapper-2.1.9/exchanges_wrapper/lib.py
+-rw-r--r--   0        0        0    53745 2024-04-14 17:09:33.653731 exchanges_wrapper-2.1.9/exchanges_wrapper/martin/__init__.py
+-rw-r--r--   0        0        0    19230 2024-04-14 17:09:33.653731 exchanges_wrapper-2.1.9/exchanges_wrapper/parsers/bitfinex_parser.py
+-rw-r--r--   0        0        0    16028 2024-04-14 17:09:33.653731 exchanges_wrapper-2.1.9/exchanges_wrapper/parsers/bybit_parser.py
+-rw-r--r--   0        0        0    14390 2024-04-14 17:09:33.653731 exchanges_wrapper-2.1.9/exchanges_wrapper/parsers/huobi_parser.py
+-rw-r--r--   0        0        0    16228 2024-04-14 17:09:33.653731 exchanges_wrapper-2.1.9/exchanges_wrapper/parsers/okx_parser.py
+-rw-r--r--   0        0        0    10683 2024-04-14 17:09:33.653731 exchanges_wrapper-2.1.9/exchanges_wrapper/proto/martin.proto
+-rw-r--r--   0        0        0    27785 2024-04-14 17:09:33.653731 exchanges_wrapper-2.1.9/exchanges_wrapper/web_sockets.py
+-rw-r--r--   0        0        0     1227 2024-04-14 17:09:33.653731 exchanges_wrapper-2.1.9/pyproject.toml
+-rw-r--r--   0        0        0     8020 1970-01-01 00:00:00.000000 exchanges_wrapper-2.1.9/PKG-INFO
```

### Comparing `exchanges_wrapper-2.1.8/LICENSE.md` & `exchanges_wrapper-2.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.8/README.md` & `exchanges_wrapper-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.8/exchanges_wrapper/__init__.py` & `exchanges_wrapper-2.1.9/exchanges_wrapper/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 __authors__ = ["Th0rgal", "Jerry Fedorenko"]
 __license__ = "MIT"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 __email__ = "jerry.fedorenko@yahoo.com"
 __credits__ = ["https://github.com/DanyaSWorlD"]
-__version__ = "2.1.8"
+__version__ = "2.1.9"
 
 from pathlib import Path
 import shutil
 
 from grpclib.server import Server, GRPCError, Status
 from grpclib.client import Channel
 from grpclib.utils import graceful_exit
```

### Comparing `exchanges_wrapper-2.1.8/exchanges_wrapper/client.py` & `exchanges_wrapper-2.1.9/exchanges_wrapper/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,14 +104,20 @@
         self.on_order_update_queues = {}
         self.account_id = None
         self.account_uid = None
         self.main_account_id = None
         self.main_account_uid = None
         self.ledgers_id = []
         self.ts_start = {}
+        self.tasks = set()
+
+    def tasks_manage(self, coro):
+        _t = asyncio.create_task(coro)
+        self.tasks.add(_t)
+        _t.add_done_callback(self.tasks.discard)
 
     async def fetch_object(self, key):
         res = None
         while res is None:
             await asyncio.sleep(0.05)
             res = self.wss_buffer.pop(key, None)
         return res
@@ -141,15 +147,15 @@
             if self.main_account_uid == '0':
                 logger.info(f"It is main ByBit account, UID: {self.account_uid}")
             else:
                 logger.info(f"Main ByBit account UID: {self.main_account_uid}, sub-UID: {self.account_uid}")
         # load rate limits
         self.rate_limits = infos["rateLimits"]
         self.loaded = True
-        logger.info(f"Info for {self.exchange}:{symbol} loaded success")
+        logger.info(f"Info for {self.exchange}:{symbol} loaded successfully")
 
     async def close(self):
         await self.session.close()
 
     @property
     def events(self):
         if not hasattr(self, "_events"):
@@ -172,41 +178,40 @@
                                                           self.exchange,
                                                           _trade_id,
                                                           self.symbol_to_okx(symbol))
         elif self.exchange == 'bybit':
             user_data_stream = BBTPrivateEventsDataStream(self, self.endpoint_ws_auth, self.exchange, _trade_id)
         if user_data_stream:
             self.data_streams[_trade_id] |= {user_data_stream}
-            asyncio.ensure_future(user_data_stream.start())
+            self.tasks_manage(user_data_stream.start())
             timeout = STATUS_TIMEOUT / 0.1
             while not user_data_stream.wss_started:
                 timeout -= 1
                 if not timeout:
                     logger.warning(f"{self.exchange} user WSS start timeout reached for {_trade_id}")
                     break
                 await asyncio.sleep(0.05)
 
     async def start_market_events_listener(self, _trade_id):
         _events = self.events.registered_streams.get(self.exchange, {}).get(_trade_id, set())
         if self.exchange == 'binance':
             market_data_stream = MarketEventsDataStream(self, self.endpoint_ws_public, self.exchange, _trade_id)
             self.data_streams[_trade_id] |= {market_data_stream}
-            asyncio.ensure_future(market_data_stream.start())
-            # start_list.append(market_data_stream.start())
+            self.tasks_manage(market_data_stream.start())
         else:
             for channel in _events:
                 # https://www.okx.com/help-center/changes-to-v5-api-websocket-subscription-parameter-and-url
                 if self.exchange == 'okx' and 'kline' in channel:
                     _endpoint = self.ws_add_on
                 else:
                     _endpoint = self.endpoint_ws_public
                 #
                 market_data_stream = MarketEventsDataStream(self, _endpoint, self.exchange, _trade_id, channel)
                 self.data_streams[_trade_id] |= {market_data_stream}
-                asyncio.ensure_future(market_data_stream.start())
+                self.tasks_manage(market_data_stream.start())
 
     async def stop_events_listener(self, _trade_id):
         logger.info(f"Stop events listener data streams for {_trade_id}")
         stopped_data_stream = self.data_streams.pop(_trade_id, set())
         for data_stream in stopped_data_stream:
             await data_stream.stop()
         if self.user_wss_session:
@@ -1245,32 +1250,33 @@
                 ids_canceled = [int(ordr['ordId']) for ordr in res if ordr['sCode'] == '0']
                 orders_canceled[:] = [i for i in orders_canceled if i['orderId'] in ids_canceled]
                 binance_res.extend(orders_canceled)
         elif self.exchange == 'bybit':
             params = {'category': 'spot', 'symbol': symbol}
             res, _ = await self.http.send_api_call("/v5/order/cancel-all", method="POST", signed=True, **params)
 
-            tasks = []
+            tasks = set()
             for order in res.get('list', []):
                 _id = order.get('orderId')
-                task = asyncio.ensure_future(self.fetch_object(f"oc-{_id}"))
+                task = asyncio.create_task(self.fetch_object(f"oc-{_id}"))
                 task.set_name(f"{_id}")
-                tasks.append(task)
+                tasks.add(task)
 
             if tasks:
                 done, pending = await asyncio.wait(tasks, timeout=STATUS_TIMEOUT)
                 binance_res = [task.result() for task in done]
                 if pending:
                     [task.cancel() for task in pending]
                     if res.get("success"):
                         for task in pending:
                             _id = task.get_name()
                             _res = await self.fetch_order(trade_id, symbol, order_id=_id, response_type=True)
                             binance_res.append(_res)
                     pending.clear()
+                tasks.clear()
 
         return binance_res
 
     # https://github.com/binance/binance-spot-api-docs/blob/master/rest-api.md#current-open-orders-user_data
     async def fetch_open_orders(self, trade_id, symbol, receive_window=None, response_type=None):
         self.assert_symbol(symbol)
         binance_res = []
```

### Comparing `exchanges_wrapper-2.1.8/exchanges_wrapper/definitions.py` & `exchanges_wrapper-2.1.9/exchanges_wrapper/definitions.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.8/exchanges_wrapper/errors.py` & `exchanges_wrapper-2.1.9/exchanges_wrapper/errors.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.8/exchanges_wrapper/events.py` & `exchanges_wrapper-2.1.9/exchanges_wrapper/events.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,28 @@
-import asyncio
-import functools
+
 from collections import defaultdict
 import logging
 
 from exchanges_wrapper.errors import UnknownEventType
 
 logger = logging.getLogger(__name__)
 
 
 # based on: https://stackoverflow.com/a/2022629/10144963
 class Handlers(list):
     async def __call__(self, *args, **kwargs):
-        loop = asyncio.get_running_loop()
         trade_id = kwargs.pop('trade_id', None)
         _trade_id = None
         for func in self:
             try:
                 _trade_id = func.args[2]
             except Exception as ex:  # skipcq: PYL-W0703
                 logger.warning(f"Handlers error when try get trade_id: {ex}")
             if trade_id is None or trade_id == _trade_id:
-                if asyncio.iscoroutinefunction(func):
-                    await func(*args, **kwargs)
-                    continue
-                if kwargs:
-                    func = functools.partial(func, **kwargs)
-                loop.run_in_executor(None, func, *args)
+                await func(*args, **kwargs)
 
     def __repr__(self):
         return f"Handlers({list.__repr__(self)})"
 
 
 class Events:
     def __init__(self):
```

### Comparing `exchanges_wrapper-2.1.8/exchanges_wrapper/exch_srv.py` & `exchanges_wrapper-2.1.9/exchanges_wrapper/exch_srv.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,22 +181,24 @@
                         logger.warning("No account IDs were received for the Huobi master account")
                     await main_client.close()
             except UserWarning as ex:
                 print(f"OpenClientConnection: {ex}")
                 raise GRPCError(status=Status.FAILED_PRECONDITION, message=str(ex))
 
         try:
-            await open_client.client.load(request.symbol)
+            await asyncio.wait_for(open_client.client.load(request.symbol), timeout=HEARTBEAT * 60)
         except asyncio.CancelledError:
             pass  # Task cancellation should not be logged as an error
+        except asyncio.exceptions.TimeoutError:
+            await OpenClient.get_client(client_id).client.session.close()
+            OpenClient.remove_client(request.account_name)
+            raise GRPCError(status=Status.UNAVAILABLE, message=f"'{open_client.name}' timeout error")
         except Exception as ex:
             logger.warning(f"OpenClientConnection for '{open_client.name}' exception: {ex}")
             logger.debug(f"Exception traceback: {traceback.format_exc()}")
-            await OpenClient.get_client(client_id).client.session.close()
-            OpenClient.remove_client(request.account_name)
             raise GRPCError(status=Status.RESOURCE_EXHAUSTED, message=str(ex))
 
         # Set rate_limiter
         Martin.rate_limiter = max(Martin.rate_limiter or 0, request.rate_limiter)
         return mr.OpenClientConnectionId(
             client_id=client_id,
             srv_version=f"{ver_cw}:{ver_ew}",
@@ -847,15 +849,15 @@
         await server.start(host, port)
         logger.info(f"Starting server v:{ver_cw}:{ver_ew} on {host}:{port}")
         await server.wait_closed()
 
         for oc in OpenClient.open_clients:
             await oc.client.session.close()
 
-        [task.cancel() for task in asyncio.all_tasks() if not task.done()]
+        [task.cancel() for task in asyncio.all_tasks() if not task.done() and task is not asyncio.current_task()]
 
 
 def main():
     try:
         asyncio.run(amain())
     except (asyncio.exceptions.CancelledError, grpclib.exceptions.StreamTerminatedError):
         pass  # # Task cancellation should not be logged as an error
```

### Comparing `exchanges_wrapper-2.1.8/exchanges_wrapper/exch_srv_cfg.toml.template` & `exchanges_wrapper-2.1.9/exchanges_wrapper/exch_srv_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.8/exchanges_wrapper/http_client.py` & `exchanges_wrapper-2.1.9/exchanges_wrapper/http_client.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.8/exchanges_wrapper/lib.py` & `exchanges_wrapper-2.1.9/exchanges_wrapper/lib.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.8/exchanges_wrapper/martin/__init__.py` & `exchanges_wrapper-2.1.9/exchanges_wrapper/martin/__init__.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.8/exchanges_wrapper/parsers/bitfinex_parser.py` & `exchanges_wrapper-2.1.9/exchanges_wrapper/parsers/bitfinex_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.8/exchanges_wrapper/parsers/bybit_parser.py` & `exchanges_wrapper-2.1.9/exchanges_wrapper/parsers/bybit_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.8/exchanges_wrapper/parsers/huobi_parser.py` & `exchanges_wrapper-2.1.9/exchanges_wrapper/parsers/huobi_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.8/exchanges_wrapper/parsers/okx_parser.py` & `exchanges_wrapper-2.1.9/exchanges_wrapper/parsers/okx_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.8/exchanges_wrapper/proto/martin.proto` & `exchanges_wrapper-2.1.9/exchanges_wrapper/proto/martin.proto`

 * *Files identical despite different names*

### Comparing `exchanges_wrapper-2.1.8/exchanges_wrapper/web_sockets.py` & `exchanges_wrapper-2.1.9/exchanges_wrapper/web_sockets.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         self.exchange = exchange
         self.trade_id = trade_id
         self.websocket = None
         self.try_count = 0
         self.wss_event_buffer = {}
         self._order_book = None
         self._price = None
-        self.tasks_list = []
+        self.tasks = set()
         self.wss_started = False
 
     async def start(self):
         ping_interval = None if self.exchange == 'huobi' else 20
         async for self.websocket in websockets.connect(
                 self.endpoint,
                 logger=logger_ws,
@@ -80,16 +80,21 @@
         Stop data stream
         """
         self.tasks_cancel()
         if self.websocket:
             await self.websocket.close(code=4000)
 
     def tasks_cancel(self):
-        [task.cancel() for task in self.tasks_list if not task.done()]
-        self.tasks_list.clear()
+        [task.cancel() for task in self.tasks if not task.done()]
+        self.tasks.clear()
+
+    def tasks_manage(self, coro):
+        _t = asyncio.create_task(coro)
+        self.tasks.add(_t)
+        _t.add_done_callback(self.tasks.discard)
 
     async def _handle_event(self, *args):
         pass  # meant to be overridden in a subclass
 
     async def _handle_messages(self, msg, symbol=None, ch_type=str()):
         msg_data = json.loads(msg if isinstance(msg, str) else gzip.decompress(msg))
         if self.exchange == 'binance':
@@ -106,16 +111,15 @@
                     if msg_data["topic"] == "wallet":
                         _data[0]["creationTime"] = msg_data["creationTime"]
                 await self._handle_event(_data, symbol, ch_type)
             elif msg_data.get("ret_msg") == "pong" or msg_data.get("op") == "pong":
                 return
             elif ((msg_data.get("ret_msg") == "subscribe" or msg_data.get("op") in ("auth", "subscribe"))
                   and msg_data.get("success")):
-                _task = asyncio.ensure_future(self.bybit_heartbeat(ch_type or "private"))
-                self.tasks_list.append(_task)
+                self.tasks_manage(self.bybit_heartbeat(ch_type or "private"))
                 if msg_data["op"] == "subscribe" and msg_data["success"] and not msg_data["ret_msg"]:
                     self.wss_started = True
             elif ((msg_data.get("ret_msg") == "subscribe" or msg_data.get("op") in ("auth", "subscribe"))
                   and not msg_data.get("success")):
                 logger.warning(f"Reconnecting ByBit WSS: {symbol}: {ch_type}, msg_data: {msg_data}")
                 raise websockets.ConnectionClosed(None, None)
             else:
@@ -598,16 +602,15 @@
         # https://github.com/binance-exchange/binance-official-api-docs/blob/master/user-data-stream.md#pingkeep-alive-a-listenkey
         while True:
             await asyncio.sleep(interval)
             await self.client.keep_alive_listen_key(listen_key)
 
     async def start_wss(self):
         logger.info(f"Start User WSS for {self.exchange}")
-        _task = asyncio.ensure_future(self._heartbeat(self.listen_key))
-        self.tasks_list.append(_task)
+        self.tasks_manage(self._heartbeat(self.listen_key))
         try:
             await self.ws_listener()
         finally:
             self.tasks_cancel()
 
     async def _handle_event(self, content):
         # logger.debug(f"UserEventsDataStream._handle_event.content: {content}")
```

### Comparing `exchanges_wrapper-2.1.8/pyproject.toml` & `exchanges_wrapper-2.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
              "Operating System :: Unix",
              "Operating System :: Microsoft :: Windows",
              "Operating System :: MacOS"]
 dynamic = ["version", "description"]
 requires-python = ">=3.9"
 
 dependencies = [
-    "crypto-ws-api==2.0.8",
+    "crypto-ws-api==2.0.9",
     "grpcio==1.62.0",
     "pyotp~=2.9.0",
     "simplejson==3.19.2",
     "aiohttp==3.9.3",
     "Pympler~=1.0.1",
     "websockets~=12.0",
     "expiringdict~=1.2.2",
```

### Comparing `exchanges_wrapper-2.1.8/PKG-INFO` & `exchanges_wrapper-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: exchanges-wrapper
-Version: 2.1.8
+Version: 2.1.9
 Summary: REST API and WebSocket asyncio wrapper with grpc powered multiplexer server
 Author-email: Thomas Marchand <thomas.marchand@tuta.io>, Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Dist: crypto-ws-api==2.0.8
+Requires-Dist: crypto-ws-api==2.0.9
 Requires-Dist: grpcio==1.62.0
 Requires-Dist: pyotp~=2.9.0
 Requires-Dist: simplejson==3.19.2
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: Pympler~=1.0.1
 Requires-Dist: websockets~=12.0
 Requires-Dist: expiringdict~=1.2.2
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: exchanges-wrapper Version: 2.1.8 Summary: REST API
+Metadata-Version: 2.1 Name: exchanges-wrapper Version: 2.1.9 Summary: REST API
 and WebSocket asyncio wrapper with grpc powered multiplexer server Author-
 email: Thomas Marchand
 tuta.io>, Jerry Fedorenko
 yahoo.com> Requires-Python: >=3.9 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix Classifier: Operating System :: Microsoft
 :: Windows Classifier: Operating System :: MacOS Requires-Dist: crypto-ws-
-api==2.0.8 Requires-Dist: grpcio==1.62.0 Requires-Dist: pyotp~=2.9.0 Requires-
+api==2.0.9 Requires-Dist: grpcio==1.62.0 Requires-Dist: pyotp~=2.9.0 Requires-
 Dist: simplejson==3.19.2 Requires-Dist: aiohttp==3.9.3 Requires-Dist:
 Pympler~=1.0.1 Requires-Dist: websockets~=12.0 Requires-Dist:
 expiringdict~=1.2.2 Requires-Dist: ujson~=5.9.0 Requires-Dist:
 betterproto==2.0.0b6 Requires-Dist: grpclib~=0.4.7 Project-URL: Source, https:/
 /github.com/DogsTailFarmer/exchanges-wrapper
         ************ [[hhttttppss::////rraaww..ggiitthhuubbuusseerrccoonntteenntt..ccoomm//ggiisstt//DDooggssTTaaiillFFaarrmmeerr//
 116677eeaaff6655cceebbffee9955dd995544008822cc77ff118811aa22cccc//rraaww//aa6677227700ddee88666633aadd33ddee44773333333300ffff6644cc99bbaa33115533ff8877dd//
```

