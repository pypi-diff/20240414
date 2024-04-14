# Comparing `tmp/kucoin_futures_lib-0.8.0.tar.gz` & `tmp/kucoin_futures_lib-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kucoin_futures_lib-0.8.0.tar", max compression
+gzip compressed data, was "kucoin_futures_lib-0.9.0.tar", max compression
```

## Comparing `kucoin_futures_lib-0.8.0.tar` & `kucoin_futures_lib-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    11357 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/LICENSE
--rw-r--r--   0        0        0     1760 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/README.md
--rw-r--r--   0        0        0      719 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/__init__.py
--rw-r--r--   0        0        0     2329 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/factory.py
--rw-r--r--   0        0        0      424 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/handlers/__init__.py
--rw-r--r--   0        0        0      961 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/handlers/base.py
--rw-r--r--   0        0        0     2695 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/handlers/entry.py
--rw-r--r--   0        0        0     2044 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/handlers/message.py
--rw-r--r--   0        0        0     2769 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/handlers/oco.py
--rw-r--r--   0        0        0     3611 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/handlers/trailing.py
--rw-r--r--   0        0        0     1813 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/helper.py
--rw-r--r--   0        0        0     2464 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/kucoinf.py
--rw-r--r--   0        0        0     3117 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/market.py
--rw-r--r--   0        0        0    17231 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/trade.py
--rw-r--r--   0        0        0     1068 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/user.py
--rw-r--r--   0        0        0     3879 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/kucoin_futures_lib/websocket.py
--rw-r--r--   0        0        0      598 2024-04-12 03:12:40.884737 kucoin_futures_lib-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2389 1970-01-01 00:00:00.000000 kucoin_futures_lib-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-13 01:10:39.315499 kucoin_futures_lib-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1760 2024-04-13 01:10:39.315499 kucoin_futures_lib-0.9.0/README.md
+-rw-r--r--   0        0        0      719 2024-04-13 01:10:39.315499 kucoin_futures_lib-0.9.0/kucoin_futures_lib/__init__.py
+-rw-r--r--   0        0        0     2329 2024-04-13 01:10:39.315499 kucoin_futures_lib-0.9.0/kucoin_futures_lib/factory.py
+-rw-r--r--   0        0        0      424 2024-04-13 01:10:39.315499 kucoin_futures_lib-0.9.0/kucoin_futures_lib/handlers/__init__.py
+-rw-r--r--   0        0        0      961 2024-04-13 01:10:39.315499 kucoin_futures_lib-0.9.0/kucoin_futures_lib/handlers/base.py
+-rw-r--r--   0        0        0     2695 2024-04-13 01:10:39.315499 kucoin_futures_lib-0.9.0/kucoin_futures_lib/handlers/entry.py
+-rw-r--r--   0        0        0     2519 2024-04-13 01:10:39.315499 kucoin_futures_lib-0.9.0/kucoin_futures_lib/handlers/message.py
+-rw-r--r--   0        0        0     2769 2024-04-13 01:10:39.315499 kucoin_futures_lib-0.9.0/kucoin_futures_lib/handlers/oco.py
+-rw-r--r--   0        0        0     3611 2024-04-13 01:10:39.315499 kucoin_futures_lib-0.9.0/kucoin_futures_lib/handlers/trailing.py
+-rw-r--r--   0        0        0     1813 2024-04-13 01:10:39.315499 kucoin_futures_lib-0.9.0/kucoin_futures_lib/helper.py
+-rw-r--r--   0        0        0     2464 2024-04-13 01:10:39.315499 kucoin_futures_lib-0.9.0/kucoin_futures_lib/kucoinf.py
+-rw-r--r--   0        0        0     3117 2024-04-13 01:10:39.315499 kucoin_futures_lib-0.9.0/kucoin_futures_lib/market.py
+-rw-r--r--   0        0        0    17231 2024-04-13 01:10:39.315499 kucoin_futures_lib-0.9.0/kucoin_futures_lib/trade.py
+-rw-r--r--   0        0        0     1068 2024-04-13 01:10:39.315499 kucoin_futures_lib-0.9.0/kucoin_futures_lib/user.py
+-rw-r--r--   0        0        0     3879 2024-04-13 01:10:39.315499 kucoin_futures_lib-0.9.0/kucoin_futures_lib/websocket.py
+-rw-r--r--   0        0        0      598 2024-04-13 01:10:39.315499 kucoin_futures_lib-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2389 1970-01-01 00:00:00.000000 kucoin_futures_lib-0.9.0/PKG-INFO
```

### Comparing `kucoin_futures_lib-0.8.0/LICENSE` & `kucoin_futures_lib-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.8.0/README.md` & `kucoin_futures_lib-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.8.0/kucoin_futures_lib/__init__.py` & `kucoin_futures_lib-0.9.0/kucoin_futures_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.8.0/kucoin_futures_lib/factory.py` & `kucoin_futures_lib-0.9.0/kucoin_futures_lib/factory.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.8.0/kucoin_futures_lib/handlers/base.py` & `kucoin_futures_lib-0.9.0/kucoin_futures_lib/handlers/base.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.8.0/kucoin_futures_lib/handlers/entry.py` & `kucoin_futures_lib-0.9.0/kucoin_futures_lib/handlers/entry.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.8.0/kucoin_futures_lib/handlers/message.py` & `kucoin_futures_lib-0.9.0/kucoin_futures_lib/handlers/message.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,22 +9,25 @@
 
 
 class MessageHandler(HandlerABC):
 
     def __init__(
         self,
         order_id: str,
+        order_status: Optional[Literal["match", "open", "done"]] = None,
         message_type: Optional[List[Literal["open", "match", "filled", "canceled", "update"]]] = None,
     ):
         """The handler will stop listening when any of the message_type is received.
+        If both order_status and message_type are None, the handler will react to the first message received for the order.
         :param order_id: The order ID to listen for.
         :param message_type: The message type to listen for. Default is None."""
 
         self.order_id = order_id
         self.message_type = message_type
+        self.order_status = order_status
         self.received_message = None
         self._reached = asyncio.Event()
         self._topic = "/contractMarket/tradeOrders"
 
     def __repr__(self):
         return f"MessageHandler(order_id='{self.order_id}', message_type={self.message_type})"
 
@@ -51,12 +54,16 @@
         """
         if self._reached.is_set():
             return
 
         trade_order = msg.get("data", {})
         trade_order_id = trade_order.get("orderId", "")
         message_type = trade_order.get("type", "")
+        status = trade_order.get("status", "")
 
-        if trade_order_id == self.order_id and message_type in self.message_type:
-            logger.info("Order %s received %s", self.order_id, message_type)
-            self.received_message = message_type
-            self._reached.set()
+        if trade_order_id == self.order_id:
+            status_match = self.order_status is None or status in self.order_status
+            message_match = self.message_type is None or message_type in self.message_type
+            if status_match and message_match:
+                logger.info("Order %s is %s", self.order_id, message_type)
+                self.received_message = message_type
+                self._reached.set()
```

### Comparing `kucoin_futures_lib-0.8.0/kucoin_futures_lib/handlers/oco.py` & `kucoin_futures_lib-0.9.0/kucoin_futures_lib/handlers/oco.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.8.0/kucoin_futures_lib/handlers/trailing.py` & `kucoin_futures_lib-0.9.0/kucoin_futures_lib/handlers/trailing.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.8.0/kucoin_futures_lib/helper.py` & `kucoin_futures_lib-0.9.0/kucoin_futures_lib/helper.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.8.0/kucoin_futures_lib/kucoinf.py` & `kucoin_futures_lib-0.9.0/kucoin_futures_lib/kucoinf.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.8.0/kucoin_futures_lib/market.py` & `kucoin_futures_lib-0.9.0/kucoin_futures_lib/market.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.8.0/kucoin_futures_lib/trade.py` & `kucoin_futures_lib-0.9.0/kucoin_futures_lib/trade.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.8.0/kucoin_futures_lib/user.py` & `kucoin_futures_lib-0.9.0/kucoin_futures_lib/user.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.8.0/kucoin_futures_lib/websocket.py` & `kucoin_futures_lib-0.9.0/kucoin_futures_lib/websocket.py`

 * *Files identical despite different names*

### Comparing `kucoin_futures_lib-0.8.0/pyproject.toml` & `kucoin_futures_lib-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kucoin-futures-lib"
-version = "0.8.0"
+version = "0.9.0"
 description = "Kucoin Futures wrapper library"
 authors = ["Evgeny Aleshin"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `kucoin_futures_lib-0.8.0/PKG-INFO` & `kucoin_futures_lib-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kucoin-futures-lib
-Version: 0.8.0
+Version: 0.9.0
 Summary: Kucoin Futures wrapper library
 License: Apache-2.0
 Author: Evgeny Aleshin
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

