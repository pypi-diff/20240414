# Comparing `tmp/synnax-0.8.0.tar.gz` & `tmp/synnax-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synnax-0.8.0.tar", max compression
+gzip compressed data, was "synnax-0.9.0.tar", max compression
```

## Comparing `synnax-0.8.0.tar` & `synnax-0.9.0.tar`

### file list

```diff
@@ -1,61 +1,62 @@
--rw-r--r--   0        0        0     1547 2023-08-30 16:58:58.430409 synnax-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1086 2023-08-29 15:02:18.834258 synnax-0.8.0/synnax/__init__.py
--rw-r--r--   0        0        0     2828 2023-08-11 20:26:13.240700 synnax-0.8.0/synnax/auth.py
--rw-r--r--   0        0        0      661 2023-08-29 15:02:18.834557 synnax-0.8.0/synnax/channel/__init__.py
--rw-r--r--   0        0        0    10614 2023-08-29 15:02:18.834804 synnax-0.8.0/synnax/channel/client.py
--rw-r--r--   0        0        0     1222 2023-08-11 20:26:13.243526 synnax-0.8.0/synnax/channel/create.py
--rw-r--r--   0        0        0     2076 2023-08-29 15:02:18.835122 synnax-0.8.0/synnax/channel/payload.py
--rw-r--r--   0        0        0     3703 2023-08-29 15:02:18.835300 synnax-0.8.0/synnax/channel/retrieve.py
--rw-r--r--   0        0        0      365 2023-08-11 20:26:13.243753 synnax-0.8.0/synnax/cli/__init__.py
--rw-r--r--   0        0        0     4337 2023-08-11 20:26:13.243848 synnax-0.8.0/synnax/cli/channel.py
--rw-r--r--   0        0        0     2558 2023-08-11 20:26:13.243903 synnax-0.8.0/synnax/cli/connect.py
--rw-r--r--   0        0        0      564 2023-08-11 20:26:13.243987 synnax-0.8.0/synnax/cli/console/__init__.py
--rw-r--r--   0        0        0     4494 2023-08-29 15:54:44.825141 synnax-0.8.0/synnax/cli/console/mock.py
--rw-r--r--   0        0        0     3299 2023-08-11 20:26:13.244144 synnax-0.8.0/synnax/cli/console/protocol.py
--rw-r--r--   0        0        0     3283 2023-08-29 15:02:18.835494 synnax-0.8.0/synnax/cli/console/rich.py
--rw-r--r--   0        0        0     7060 2023-08-11 20:26:13.244294 synnax-0.8.0/synnax/cli/console/sugared.py
--rw-r--r--   0        0        0      606 2023-08-11 20:26:13.244350 synnax-0.8.0/synnax/cli/default.py
--rw-r--r--   0        0        0     1369 2023-08-11 20:26:13.244436 synnax-0.8.0/synnax/cli/flow/__init__.py
--rw-r--r--   0        0        0    14472 2023-08-11 20:26:13.244524 synnax-0.8.0/synnax/cli/ingest.py
--rw-r--r--   0        0        0     1287 2023-08-11 20:26:13.244574 synnax-0.8.0/synnax/cli/io.py
--rw-r--r--   0        0        0     1647 2023-08-11 20:26:13.244623 synnax-0.8.0/synnax/cli/login.py
--rw-r--r--   0        0        0      590 2023-08-11 20:26:13.244681 synnax-0.8.0/synnax/cli/synnax.py
--rw-r--r--   0        0        0     1613 2023-08-29 15:02:18.835684 synnax-0.8.0/synnax/cli/telem.py
--rw-r--r--   0        0        0     5163 2023-08-29 15:02:18.835864 synnax-0.8.0/synnax/cli/ts_convert.py
--rw-r--r--   0        0        0     1622 2023-08-11 20:26:13.244903 synnax-0.8.0/synnax/config/__init__.py
--rw-r--r--   0        0        0     1222 2023-08-29 15:02:18.836059 synnax-0.8.0/synnax/config/clusters.py
--rw-r--r--   0        0        0     1947 2023-08-11 20:26:13.245009 synnax-0.8.0/synnax/config/file.py
--rw-r--r--   0        0        0        0 2023-08-29 15:02:18.836137 synnax-0.8.0/synnax/control/__init__.py
--rw-r--r--   0        0        0     4024 2023-08-29 16:02:03.323993 synnax-0.8.0/synnax/exceptions.py
--rw-r--r--   0        0        0      593 2023-08-11 20:26:13.245158 synnax-0.8.0/synnax/framer/__init__.py
--rw-r--r--   0        0        0     3027 2023-08-29 15:02:18.836516 synnax-0.8.0/synnax/framer/adapter.py
--rw-r--r--   0        0        0     5814 2023-08-29 15:02:18.836678 synnax-0.8.0/synnax/framer/client.py
--rw-r--r--   0        0        0     5839 2023-08-29 15:02:18.836821 synnax-0.8.0/synnax/framer/frame.py
--rw-r--r--   0        0        0     8235 2023-08-29 15:02:18.837076 synnax-0.8.0/synnax/framer/iterator.py
--rw-r--r--   0        0        0     2426 2023-08-29 15:02:18.837332 synnax-0.8.0/synnax/framer/streamer.py
--rw-r--r--   0        0        0    11407 2023-08-29 15:02:18.837598 synnax-0.8.0/synnax/framer/writer.py
--rw-r--r--   0        0        0      694 2023-08-11 20:26:13.246074 synnax-0.8.0/synnax/ingest/__init__.py
--rw-r--r--   0        0        0     3231 2023-08-29 15:02:18.837744 synnax-0.8.0/synnax/ingest/row.py
--rw-r--r--   0        0        0      575 2023-08-11 20:26:13.246228 synnax-0.8.0/synnax/io/__init__.py
--rw-r--r--   0        0        0     4812 2023-08-29 15:02:18.837923 synnax-0.8.0/synnax/io/csv.py
--rw-r--r--   0        0        0     2060 2023-08-11 20:26:13.246378 synnax-0.8.0/synnax/io/factory.py
--rw-r--r--   0        0        0      931 2023-08-11 20:26:13.246436 synnax-0.8.0/synnax/io/matcher.py
--rw-r--r--   0        0        0      661 2023-08-11 20:26:13.246489 synnax-0.8.0/synnax/io/meta.py
--rw-r--r--   0        0        0     4723 2023-08-11 20:26:13.246585 synnax-0.8.0/synnax/io/protocol.py
--rw-r--r--   0        0        0      574 2023-08-11 20:26:13.246639 synnax-0.8.0/synnax/options.py
--rw-r--r--   0        0        0      500 2023-08-11 20:26:13.246717 synnax-0.8.0/synnax/ranger/__init__.py
--rw-r--r--   0        0        0     3492 2023-08-29 15:02:18.838090 synnax-0.8.0/synnax/ranger/client.py
--rw-r--r--   0        0        0     1201 2023-08-11 20:26:13.246822 synnax-0.8.0/synnax/ranger/create.py
--rw-r--r--   0        0        0     1756 2023-08-29 15:02:18.838241 synnax-0.8.0/synnax/ranger/payload.py
--rw-r--r--   0        0        0     5412 2023-08-29 16:00:15.144440 synnax-0.8.0/synnax/ranger/range.py
--rw-r--r--   0        0        0     1642 2023-08-11 20:26:13.246981 synnax-0.8.0/synnax/ranger/retrieve.py
--rw-r--r--   0        0        0     5297 2023-08-29 15:02:18.838563 synnax-0.8.0/synnax/synnax.py
--rw-r--r--   0        0        0      433 2023-08-29 15:02:18.838658 synnax-0.8.0/synnax/telem/__init__.py
--rw-r--r--   0        0        0     4593 2023-08-29 16:00:56.622306 synnax-0.8.0/synnax/telem/series.py
--rw-r--r--   0        0        0    34106 2023-08-29 15:02:18.839047 synnax-0.8.0/synnax/telem/telem.py
--rw-r--r--   0        0        0     2345 2023-08-29 15:02:18.839195 synnax-0.8.0/synnax/transport.py
--rw-r--r--   0        0        0      365 2023-08-11 20:26:13.247283 synnax-0.8.0/synnax/user/__init__.py
--rw-r--r--   0        0        0      457 2023-08-11 20:26:13.247346 synnax-0.8.0/synnax/user/payload.py
--rw-r--r--   0        0        0      365 2023-08-11 20:26:13.247416 synnax-0.8.0/synnax/util/__init__.py
--rw-r--r--   0        0        0      814 2023-08-29 15:02:18.839338 synnax-0.8.0/synnax/util/normalize.py
--rw-r--r--   0        0        0      969 1970-01-01 00:00:00.000000 synnax-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1547 2023-09-08 16:45:26.039121 synnax-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1086 2023-08-30 17:33:33.658911 synnax-0.9.0/synnax/__init__.py
+-rw-r--r--   0        0        0     2828 2023-08-11 20:26:13.240700 synnax-0.9.0/synnax/auth.py
+-rw-r--r--   0        0        0      661 2023-08-30 17:33:33.659061 synnax-0.9.0/synnax/channel/__init__.py
+-rw-r--r--   0        0        0    10614 2023-08-30 17:33:33.659244 synnax-0.9.0/synnax/channel/client.py
+-rw-r--r--   0        0        0     1222 2023-08-11 20:26:13.243526 synnax-0.9.0/synnax/channel/create.py
+-rw-r--r--   0        0        0     2076 2023-08-30 17:33:33.659391 synnax-0.9.0/synnax/channel/payload.py
+-rw-r--r--   0        0        0     3703 2023-08-30 17:33:33.659506 synnax-0.9.0/synnax/channel/retrieve.py
+-rw-r--r--   0        0        0      365 2023-08-11 20:26:13.243753 synnax-0.9.0/synnax/cli/__init__.py
+-rw-r--r--   0        0        0     4337 2023-08-11 20:26:13.243848 synnax-0.9.0/synnax/cli/channel.py
+-rw-r--r--   0        0        0     2558 2023-08-11 20:26:13.243903 synnax-0.9.0/synnax/cli/connect.py
+-rw-r--r--   0        0        0      564 2023-08-11 20:26:13.243987 synnax-0.9.0/synnax/cli/console/__init__.py
+-rw-r--r--   0        0        0     4494 2023-08-30 17:33:33.660157 synnax-0.9.0/synnax/cli/console/mock.py
+-rw-r--r--   0        0        0     3299 2023-08-11 20:26:13.244144 synnax-0.9.0/synnax/cli/console/protocol.py
+-rw-r--r--   0        0        0     3283 2023-08-30 17:33:33.660290 synnax-0.9.0/synnax/cli/console/rich.py
+-rw-r--r--   0        0        0     7060 2023-08-11 20:26:13.244294 synnax-0.9.0/synnax/cli/console/sugared.py
+-rw-r--r--   0        0        0      606 2023-08-11 20:26:13.244350 synnax-0.9.0/synnax/cli/default.py
+-rw-r--r--   0        0        0     1369 2023-08-11 20:26:13.244436 synnax-0.9.0/synnax/cli/flow/__init__.py
+-rw-r--r--   0        0        0    14472 2023-08-11 20:26:13.244524 synnax-0.9.0/synnax/cli/ingest.py
+-rw-r--r--   0        0        0     1287 2023-08-11 20:26:13.244574 synnax-0.9.0/synnax/cli/io.py
+-rw-r--r--   0        0        0     1647 2023-08-11 20:26:13.244623 synnax-0.9.0/synnax/cli/login.py
+-rw-r--r--   0        0        0      590 2023-08-11 20:26:13.244681 synnax-0.9.0/synnax/cli/synnax.py
+-rw-r--r--   0        0        0     1613 2023-08-30 17:33:33.660413 synnax-0.9.0/synnax/cli/telem.py
+-rw-r--r--   0        0        0     5163 2023-08-30 17:33:33.660609 synnax-0.9.0/synnax/cli/ts_convert.py
+-rw-r--r--   0        0        0     1622 2023-08-11 20:26:13.244903 synnax-0.9.0/synnax/config/__init__.py
+-rw-r--r--   0        0        0     1222 2023-08-30 17:33:33.660731 synnax-0.9.0/synnax/config/clusters.py
+-rw-r--r--   0        0        0     1947 2023-08-11 20:26:13.245009 synnax-0.9.0/synnax/config/file.py
+-rw-r--r--   0        0        0        0 2023-09-05 09:42:56.909303 synnax-0.9.0/synnax/control/__init__.py
+-rw-r--r--   0        0        0      552 2023-09-08 16:37:43.461528 synnax-0.9.0/synnax/control/a.py
+-rw-r--r--   0        0        0     4024 2023-08-30 17:33:33.661185 synnax-0.9.0/synnax/exceptions.py
+-rw-r--r--   0        0        0      593 2023-08-11 20:26:13.245158 synnax-0.9.0/synnax/framer/__init__.py
+-rw-r--r--   0        0        0     3027 2023-08-30 17:33:33.661337 synnax-0.9.0/synnax/framer/adapter.py
+-rw-r--r--   0        0        0     5814 2023-09-05 09:42:56.909860 synnax-0.9.0/synnax/framer/client.py
+-rw-r--r--   0        0        0     5839 2023-08-30 17:33:33.661765 synnax-0.9.0/synnax/framer/frame.py
+-rw-r--r--   0        0        0     8235 2023-08-30 17:33:33.661968 synnax-0.9.0/synnax/framer/iterator.py
+-rw-r--r--   0        0        0     2426 2023-08-30 17:33:33.662327 synnax-0.9.0/synnax/framer/streamer.py
+-rw-r--r--   0        0        0    11300 2023-09-08 16:37:43.461928 synnax-0.9.0/synnax/framer/writer.py
+-rw-r--r--   0        0        0      694 2023-08-11 20:26:13.246074 synnax-0.9.0/synnax/ingest/__init__.py
+-rw-r--r--   0        0        0     3231 2023-08-30 17:33:33.662685 synnax-0.9.0/synnax/ingest/row.py
+-rw-r--r--   0        0        0      575 2023-08-11 20:26:13.246228 synnax-0.9.0/synnax/io/__init__.py
+-rw-r--r--   0        0        0     4812 2023-08-30 17:33:33.662904 synnax-0.9.0/synnax/io/csv.py
+-rw-r--r--   0        0        0     2060 2023-08-11 20:26:13.246378 synnax-0.9.0/synnax/io/factory.py
+-rw-r--r--   0        0        0      931 2023-08-11 20:26:13.246436 synnax-0.9.0/synnax/io/matcher.py
+-rw-r--r--   0        0        0      661 2023-08-11 20:26:13.246489 synnax-0.9.0/synnax/io/meta.py
+-rw-r--r--   0        0        0     4723 2023-08-11 20:26:13.246585 synnax-0.9.0/synnax/io/protocol.py
+-rw-r--r--   0        0        0      574 2023-08-11 20:26:13.246639 synnax-0.9.0/synnax/options.py
+-rw-r--r--   0        0        0      500 2023-08-11 20:26:13.246717 synnax-0.9.0/synnax/ranger/__init__.py
+-rw-r--r--   0        0        0     3492 2023-08-30 17:33:33.663046 synnax-0.9.0/synnax/ranger/client.py
+-rw-r--r--   0        0        0     1201 2023-08-11 20:26:13.246822 synnax-0.9.0/synnax/ranger/create.py
+-rw-r--r--   0        0        0     1756 2023-08-30 17:33:33.663173 synnax-0.9.0/synnax/ranger/payload.py
+-rw-r--r--   0        0        0     5412 2023-08-30 17:33:33.663515 synnax-0.9.0/synnax/ranger/range.py
+-rw-r--r--   0        0        0     1642 2023-08-11 20:26:13.246981 synnax-0.9.0/synnax/ranger/retrieve.py
+-rw-r--r--   0        0        0     5297 2023-08-30 17:33:33.663721 synnax-0.9.0/synnax/synnax.py
+-rw-r--r--   0        0        0      433 2023-08-30 17:33:33.663807 synnax-0.9.0/synnax/telem/__init__.py
+-rw-r--r--   0        0        0     4665 2023-09-08 16:37:43.462274 synnax-0.9.0/synnax/telem/series.py
+-rw-r--r--   0        0        0    34106 2023-08-31 18:49:20.974900 synnax-0.9.0/synnax/telem/telem.py
+-rw-r--r--   0        0        0     2345 2023-08-30 17:33:33.664490 synnax-0.9.0/synnax/transport.py
+-rw-r--r--   0        0        0      365 2023-08-11 20:26:13.247283 synnax-0.9.0/synnax/user/__init__.py
+-rw-r--r--   0        0        0      457 2023-08-11 20:26:13.247346 synnax-0.9.0/synnax/user/payload.py
+-rw-r--r--   0        0        0      365 2023-08-11 20:26:13.247416 synnax-0.9.0/synnax/util/__init__.py
+-rw-r--r--   0        0        0      814 2023-08-30 17:33:33.664640 synnax-0.9.0/synnax/util/normalize.py
+-rw-r--r--   0        0        0      969 1970-01-01 00:00:00.000000 synnax-0.9.0/PKG-INFO
```

### Comparing `synnax-0.8.0/pyproject.toml` & `synnax-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "synnax"
-version = "0.8.0"
+version = "0.9.0"
 description = "Synnax Client Library"
 keywords = ["Synnax", "Synnax Python Client"]
 authors = ["emiliano bonilla <emilbon99@gmail.com>"]
 repository = "https://github.com/synnaxlabs/synnax"
 homepage = "https://synnaxlabs.com"
 packages = [
 	{ include = "synnax/**/*.py" }
@@ -18,15 +18,15 @@
 websockets = "^11.0.3"
 mypy = "^1.3.0"
 pandas = "^2.0.2"
 PyJWT = "^2.5.0"
 rich = "^13.4.1"
 pick = "^2.0.2"
 pydantic = "^1.10.9"
-synnax-freighter = "^0.3.0"
+synnax-freighter = "^0.4.0"
 #synnax-freighter = { path = "../../freighter/py", develop = true }
 alamos = "^0.2.0"
 #alamos = { path = "../../alamos/py", develop = true }
 keyring = "^23.9.3"
 click = "^8.1.3"
 urllib3 = "^2.0.3"
 numpy = "^1.24.3"
```

### Comparing `synnax-0.8.0/synnax/__init__.py` & `synnax-0.9.0/synnax/__init__.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/auth.py` & `synnax-0.9.0/synnax/auth.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/channel/__init__.py` & `synnax-0.9.0/synnax/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/channel/client.py` & `synnax-0.9.0/synnax/channel/client.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/channel/create.py` & `synnax-0.9.0/synnax/channel/create.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/channel/payload.py` & `synnax-0.9.0/synnax/channel/payload.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/channel/retrieve.py` & `synnax-0.9.0/synnax/channel/retrieve.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/cli/channel.py` & `synnax-0.9.0/synnax/cli/channel.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/cli/connect.py` & `synnax-0.9.0/synnax/cli/connect.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/cli/console/__init__.py` & `synnax-0.9.0/synnax/cli/console/__init__.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/cli/console/mock.py` & `synnax-0.9.0/synnax/cli/console/mock.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/cli/console/protocol.py` & `synnax-0.9.0/synnax/cli/console/protocol.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/cli/console/rich.py` & `synnax-0.9.0/synnax/cli/console/rich.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/cli/console/sugared.py` & `synnax-0.9.0/synnax/cli/console/sugared.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/cli/default.py` & `synnax-0.9.0/synnax/cli/default.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/cli/flow/__init__.py` & `synnax-0.9.0/synnax/cli/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/cli/ingest.py` & `synnax-0.9.0/synnax/cli/ingest.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/cli/io.py` & `synnax-0.9.0/synnax/cli/io.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/cli/login.py` & `synnax-0.9.0/synnax/cli/login.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/cli/synnax.py` & `synnax-0.9.0/synnax/cli/synnax.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/cli/telem.py` & `synnax-0.9.0/synnax/cli/telem.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/cli/ts_convert.py` & `synnax-0.9.0/synnax/cli/ts_convert.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/config/__init__.py` & `synnax-0.9.0/synnax/config/__init__.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/config/clusters.py` & `synnax-0.9.0/synnax/config/clusters.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/config/file.py` & `synnax-0.9.0/synnax/config/file.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/exceptions.py` & `synnax-0.9.0/synnax/exceptions.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/framer/__init__.py` & `synnax-0.9.0/synnax/framer/__init__.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/framer/adapter.py` & `synnax-0.9.0/synnax/framer/adapter.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/framer/client.py` & `synnax-0.9.0/synnax/framer/client.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/framer/frame.py` & `synnax-0.9.0/synnax/framer/frame.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/framer/iterator.py` & `synnax-0.9.0/synnax/framer/iterator.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/framer/streamer.py` & `synnax-0.9.0/synnax/framer/streamer.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/framer/writer.py` & `synnax-0.9.0/synnax/framer/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,16 +214,14 @@
         if missing and extra:
             raise ValidationError(
                 Field(
                     "keys",
                     f"frame is missing keys {missing} and has extra keys {extra}",
                 )
             )
-        elif missing:
-            raise ValidationError(Field("keys", f"frame is missing keys {missing}"))
         elif extra:
             raise ValidationError(Field("keys", f"frame has extra keys {extra}"))
 
     def __prep_data_types(self, frame: Frame):
         for i, (label, series) in enumerate(frame.items()):
             ch = self.__adapter.retriever.retrieve(label)[0]  # type: ignore
             if series.data_type != ch.data_type:
```

### Comparing `synnax-0.8.0/synnax/ingest/__init__.py` & `synnax-0.9.0/synnax/ingest/__init__.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/ingest/row.py` & `synnax-0.9.0/synnax/ingest/row.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/io/__init__.py` & `synnax-0.9.0/synnax/io/__init__.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/io/csv.py` & `synnax-0.9.0/synnax/io/csv.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/io/factory.py` & `synnax-0.9.0/synnax/io/factory.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/io/matcher.py` & `synnax-0.9.0/synnax/io/matcher.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/io/meta.py` & `synnax-0.9.0/synnax/io/meta.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/io/protocol.py` & `synnax-0.9.0/synnax/io/protocol.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/options.py` & `synnax-0.9.0/synnax/options.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/ranger/client.py` & `synnax-0.9.0/synnax/ranger/client.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/ranger/create.py` & `synnax-0.9.0/synnax/ranger/create.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/ranger/payload.py` & `synnax-0.9.0/synnax/ranger/payload.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/ranger/range.py` & `synnax-0.9.0/synnax/ranger/range.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/ranger/retrieve.py` & `synnax-0.9.0/synnax/ranger/retrieve.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/synnax.py` & `synnax-0.9.0/synnax/synnax.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/telem/series.py` & `synnax-0.9.0/synnax/telem/series.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,23 +38,25 @@
     the first sample in the array (inclusive), while the end of the time range is set
     to the nanosecond AFTER the last sample in the array (exclusive).
     """
     data_type: DataType
     """The data type of the Series"""
     data: bytes
     """The underlying buffer"""
+    alignment: int = 0
 
     def __len__(self) -> int:
         return self.data_type.density.sample_count(len(self.data))
 
     def __init__(
         self,
         data: CrudeSeries,
         data_type: CrudeDataType | None = None,
         time_range: TimeRange | None = None,
+        alignment: int = 0,
     ):
         if isinstance(data, Series):
             data_type = data_type or data.data_type
             data_ = data.data
             time_range = data.time_range if time_range is None else time_range
         elif isinstance(data, pd.Series):
             data_type = data_type or DataType(data.dtype)
@@ -68,15 +70,15 @@
         else:
             if data_type is None:
                 raise ValueError(
                     "[Series] - data_type must be specified if a buffer is given",
                 )
             data_type = DataType(data_type)
             data_ = data
-        super().__init__(data_type=data_type, data=data_, time_range=time_range)
+        super().__init__(data_type=data_type, data=data_, time_range=time_range, alignment=alignment)
 
     class Config:
         arbitrary_types_allowed = True
 
     def __array__(self) -> np.ndarray:
         """Implemented to that the Series can be passed around as a numpy array. See
         https://numpy.org/doc/stable/user/basics.interoperability.html#the-array-method.
```

### Comparing `synnax-0.8.0/synnax/telem/telem.py` & `synnax-0.9.0/synnax/telem/telem.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/transport.py` & `synnax-0.9.0/synnax/transport.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/synnax/util/normalize.py` & `synnax-0.9.0/synnax/util/normalize.py`

 * *Files identical despite different names*

### Comparing `synnax-0.8.0/PKG-INFO` & `synnax-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synnax
-Version: 0.8.0
+Version: 0.9.0
 Summary: Synnax Client Library
 Home-page: https://synnaxlabs.com
 Keywords: Synnax,Synnax Python Client
 Author: emiliano bonilla
 Author-email: emilbon99@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -16,11 +16,11 @@
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: mypy (>=1.3.0,<2.0.0)
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
 Requires-Dist: pick (>=2.0.2,<3.0.0)
 Requires-Dist: pydantic (>=1.10.9,<2.0.0)
 Requires-Dist: rich (>=13.4.1,<14.0.0)
-Requires-Dist: synnax-freighter (>=0.3.0,<0.4.0)
+Requires-Dist: synnax-freighter (>=0.4.0,<0.5.0)
 Requires-Dist: urllib3 (>=2.0.3,<3.0.0)
 Requires-Dist: websockets (>=11.0.3,<12.0.0)
 Project-URL: Repository, https://github.com/synnaxlabs/synnax
```

