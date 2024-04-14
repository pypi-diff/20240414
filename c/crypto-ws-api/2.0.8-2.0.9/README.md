# Comparing `tmp/crypto-ws-api-2.0.8.tar.gz` & `tmp/crypto-ws-api-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-ws-api-2.0.8.tar", last modified: Sun Mar 31 09:19:04 2024, max compression
+gzip compressed data, was "crypto-ws-api-2.0.9.tar", last modified: Sun Apr 14 16:40:53 2024, max compression
```

## Comparing `crypto-ws-api-2.0.8.tar` & `crypto-ws-api-2.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      165 2022-06-06 16:51:29.613842 crypto-ws-api-2.0.8/.deepsource.toml
--rwxr-xr-x   0        0        0     2296 2024-03-31 09:15:49.328772 crypto-ws-api-2.0.8/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-06-30 17:01:10.037954 crypto-ws-api-2.0.8/LICENSE.md
--rw-r--r--   0        0        0     7137 2024-02-07 12:20:32.603137 crypto-ws-api-2.0.8/README.md
--rw-r--r--   0        0        0     1476 2024-03-31 09:15:49.336778 crypto-ws-api-2.0.8/crypto_ws_api/__init__.py
--rw-r--r--   0        0        0     4366 2023-11-02 13:31:35.402520 crypto-ws-api-2.0.8/crypto_ws_api/demo.py
--rw-r--r--   0        0        0      551 2023-07-01 18:52:39.110102 crypto-ws-api-2.0.8/crypto_ws_api/ws_api.toml.template
--rw-r--r--   0        0        0    17321 2024-03-26 18:39:58.170665 crypto-ws-api-2.0.8/crypto_ws_api/ws_session.py
--rw-r--r--   0        0        0      990 2024-01-05 14:15:28.636599 crypto-ws-api-2.0.8/pyproject.toml
--rw-r--r--   0        0        0       81 2024-01-05 14:15:28.636599 crypto-ws-api-2.0.8/requirements.txt
--rw-r--r--   0        0        0     7878 1970-01-01 00:00:00.000000 crypto-ws-api-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0      165 2022-06-06 16:51:29.613842 crypto-ws-api-2.0.9/.deepsource.toml
+-rwxr-xr-x   0        0        0     2368 2024-04-14 16:37:22.263406 crypto-ws-api-2.0.9/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-06-30 17:01:10.037954 crypto-ws-api-2.0.9/LICENSE.md
+-rw-r--r--   0        0        0     7137 2024-02-07 12:20:32.603137 crypto-ws-api-2.0.9/README.md
+-rw-r--r--   0        0        0     1476 2024-04-12 09:38:43.464068 crypto-ws-api-2.0.9/crypto_ws_api/__init__.py
+-rw-r--r--   0        0        0     4366 2023-11-02 13:31:35.402520 crypto-ws-api-2.0.9/crypto_ws_api/demo.py
+-rw-r--r--   0        0        0      551 2023-07-01 18:52:39.110102 crypto-ws-api-2.0.9/crypto_ws_api/ws_api.toml.template
+-rw-r--r--   0        0        0    17596 2024-04-13 14:52:17.107187 crypto-ws-api-2.0.9/crypto_ws_api/ws_session.py
+-rw-r--r--   0        0        0      990 2024-01-05 14:15:28.636599 crypto-ws-api-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0       81 2024-01-05 14:15:28.636599 crypto-ws-api-2.0.9/requirements.txt
+-rw-r--r--   0        0        0     7878 1970-01-01 00:00:00.000000 crypto-ws-api-2.0.9/PKG-INFO
```

### Comparing `crypto-ws-api-2.0.8/CHANGELOG.md` & `crypto-ws-api-2.0.9/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 2.0.9 - 2024-04-14
+### Fix
+* Creating asynchronous tasks done right
+
 ## 2.0.8 - 2024-03-31
 ### Fix
 * tons log records: `websockets socket.send() raised exception.`
 
 ## 2.0.7 - 2024-03-25
 ### Update
 * Refactoring and some minor fixes
```

### Comparing `crypto-ws-api-2.0.8/LICENSE.md` & `crypto-ws-api-2.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `crypto-ws-api-2.0.8/README.md` & `crypto-ws-api-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `crypto-ws-api-2.0.8/crypto_ws_api/__init__.py` & `crypto-ws-api-2.0.9/crypto_ws_api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 __authors__ = ["Jerry Fedorenko"]
 __license__ = "MIT"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 __email__ = "jerry.fedorenko@yahoo.com"
 __credits__ = ["https://github.com/DanyaSWorlD"]
-__version__ = "2.0.8"
+__version__ = "2.0.9"
 
 from pathlib import Path
 import shutil
 from platformdirs import user_config_path
 
 
 TIMEOUT = 5  # sec timeout for WSS initialization and get response
```

### Comparing `crypto-ws-api-2.0.8/crypto_ws_api/demo.py` & `crypto-ws-api-2.0.9/crypto_ws_api/demo.py`

 * *Files identical despite different names*

### Comparing `crypto-ws-api-2.0.8/crypto_ws_api/ws_api.toml.template` & `crypto-ws-api-2.0.9/crypto_ws_api/ws_api.toml.template`

 * *Files identical despite different names*

### Comparing `crypto-ws-api-2.0.8/crypto_ws_api/ws_session.py` & `crypto-ws-api-2.0.9/crypto_ws_api/ws_session.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         "_retry_after",
         "ws_id",
         "operational_status",
         "order_handling",
         "request_limit_reached",
         "in_event",
         "_response_pool",
-        "tasks_list",
+        "tasks",
     )
 
     def __init__(self, method, ws_id, exchange, endpoint, api_key, api_secret, passphrase=None):
         self.init = True
         self.method = method
         self.exchange = exchange
         self.endpoint = endpoint
@@ -83,18 +83,25 @@
         self._response_pool = {}
         self._retry_after = int(time.time() * 1000) - 1
         self.ws_id = ws_id
         self.operational_status = None
         self.order_handling = False
         self.request_limit_reached = False
         self.in_event = asyncio.Event()
-        self.tasks_list = []
+        self.tasks = set()
+
+    def tasks_manage(self, coro, name=None):
+        _t = asyncio.create_task(coro)
+        if name:
+            _t.set_name(name)
+        self.tasks.add(_t)
+        _t.add_done_callback(self.tasks.discard)
 
     async def _ws_listener(self):
-        asyncio.ensure_future(self.ws_login())
+        self.tasks_manage(self.ws_login())
         async for msg in self._ws:
             # logger.info(f"_ws_listener: msg: {self.ws_id}: {msg}")
             if isinstance(msg, str):
                 res = await self._handle_msg(json.loads(msg))
                 # logger.info(f"_ws_listener: res: {self.ws_id}: {res}")
                 if res != 'pass':
                     if res is None:
@@ -115,39 +122,35 @@
                 await self._ws_listener()
             except ConnectionClosed as ex:
                 if ex.code == 4000:
                     logger.info(f"WSS closed for {self.ws_id}")
                     break
                 else:
                     self.operational_status = False
-                    [task.cancel() for task in self.tasks_list if not task.done()]
-                    self.tasks_list.clear()
+                    [task.cancel() for task in self.tasks if not task.done()]
+                    self.tasks.clear()
                     logger.warning(f"Restart WSS for {self.ws_id}")
                     continue
             except Exception as ex:
                 logger.error(f"WSS start_wss() other exception: {ex}")
 
     async def ws_login(self):
         res = await self.request('userDataStream.start', _api_key=True)
         if res is None:
             logger.warning(f"UserWSS: Not 'logged in' for {self.ws_id}")
             raise ConnectionClosed(None, None)
         else:
             if self.exchange == 'binance':
                 self._listen_key = res.get('listenKey')
-                _t = asyncio.ensure_future(self.heartbeat())
-                _t.set_name(f"heartbeat-{self.ws_id}")
-                self.tasks_list.append(_t)
+                self.tasks_manage(self.heartbeat(), f"heartbeat-{self.ws_id}")
             else:
                 self._listen_key = f"{int(time.time() * 1000)}{self.ws_id}"
             self.operational_status = True
             self.order_handling = True
-            _t = asyncio.ensure_future(self._keepalive())
-            _t.set_name(f"keepalive-{self.ws_id}")
-            self.tasks_list.append(_t)
+            self.tasks_manage(self._keepalive(), f"keepalive-{self.ws_id}")
             logger.info(f"UserWSS: 'logged in' for {self.ws_id}")
 
     async def request(self, _method=None, _params=None, _api_key=False, _signed=False):
         """
         Construct and handling request/response to WS API endpoint, use a description of the methods on
         https://developers.binance.com/docs/binance-trading-api/websocket_api#request-format
         :return: result: {} or None if temporary Out-of-Service state
@@ -271,16 +274,16 @@
     async def stop(self):
         """
         Stop data stream
         """
         self.operational_status = None  # Not restart and break all loops
         self.order_handling = False
         self.init = True
-        [task.cancel() for task in self.tasks_list if not task.done()]
-        self.tasks_list.clear()
+        [task.cancel() for task in self.tasks if not task.done()]
+        self.tasks.clear()
         if self._ws and not self._ws.closed:
             await self._ws.close(code=4000)
         gc.collect()
         logger.info(f"User WSS for {self.ws_id} stopped")
 
     async def _handle_msg(self, msg):
         if self.exchange == 'binance':
@@ -293,15 +296,15 @@
             if msg.get('code') != '0':
                 await self.okx_error_handle(msg)
                 msg = None
             return msg
         elif self.exchange == 'bitfinex':
             return await self.bitfinex_error_handle(msg)
 
-    #region BitfinexErrorHandle
+    # region BitfinexErrorHandle
     async def bitfinex_error_handle(self, msg):
         if isinstance(msg, dict):
             return await self._handle_dict_message(msg)
         elif isinstance(msg, list) and msg[1] == 'n' and msg[2][1] in ('on-req', 'oc-req', 'oc_multi-req'):
             return self._transform_list_message(msg)
         else:
             return 'pass'
@@ -345,15 +348,15 @@
                 None,
                 [msg[2][4]] if msg[2][1] == 'on-req' else msg[2][4],
                 None,
                 msg[2][6],
                 msg[2][7]
             ]
         }
-    #endregion
+    # endregion
 
     async def okx_error_handle(self, msg):
         if msg.get('code') == '1':
             logger.warning(f"Operation failed: {msg}")
         elif msg.get('code') == '63999':
             logger.warning(f"An issue occurred on exchange's side: {msg}")
         elif msg.get('code') == '60014':
@@ -387,26 +390,28 @@
     __slots__ = (
         "exchange",
         "endpoint",
         "_api_key",
         "_api_secret",
         "_passphrase",
         "user_wss",
+        "tasks_wss",
     )
 
     def __init__(self, exchange, endpoint, api_key, api_secret, passphrase=None):
         if exchange not in ('binance', 'okx', 'bitfinex'):
             raise UserWarning(f"UserWSSession: exchange {exchange} not serviced")
         self.exchange = exchange
         self.endpoint = endpoint
         #
         self._api_key = api_key
         self._api_secret = api_secret
         self._passphrase = passphrase
         self.user_wss = {}
+        self.tasks_wss = set()
 
     async def handle_request(
         self,
         trade_id: str,
         method: str,
         _params=None,
         _api_key=False,
@@ -425,15 +430,17 @@
                 self._passphrase
             )
         )
 
         if user_wss.init:
             user_wss.init = False
             user_wss.operational_status = False
-            asyncio.ensure_future(user_wss.start_wss())
+            _t = asyncio.create_task(user_wss.start_wss())
+            self.tasks_wss.add(_t)
+            _t.add_done_callback(self.tasks_wss.discard)
 
         duration = 0
         while not (user_wss.operational_status and user_wss.order_handling):
             await asyncio.sleep(DELAY)
             if duration > TIMEOUT:
                 return None
             duration += DELAY
@@ -447,7 +454,9 @@
         return None
 
     async def stop(self):
         user_wss_copy = dict(self.user_wss)
         for ws in user_wss_copy.values():
             await ws.stop()
         self.user_wss.clear()
+        [task.cancel() for task in self.tasks_wss if not task.done()]
+        self.tasks_wss.clear()
```

### Comparing `crypto-ws-api-2.0.8/pyproject.toml` & `crypto-ws-api-2.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `crypto-ws-api-2.0.8/PKG-INFO` & `crypto-ws-api-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-ws-api
-Version: 2.0.8
+Version: 2.0.9
 Summary: Crypto WS API connector for ASYNC requests
 Author-email: Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: crypto-ws-api Version: 2.0.8 Summary: Crypto WS API
+Metadata-Version: 2.1 Name: crypto-ws-api Version: 2.0.9 Summary: Crypto WS API
 connector for ASYNC requests Author-email: Jerry Fedorenko
 yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3 Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix Classifier: Operating System :: Microsoft
 :: Windows Classifier: Operating System :: MacOS Requires-Dist:
 shortuuid~=1.0.11 Requires-Dist: platformdirs~=3.10.0 Requires-Dist:
```

