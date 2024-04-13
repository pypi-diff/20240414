# Comparing `tmp/BoostCLI-0.5.3.tar.gz` & `tmp/BoostCLI-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BoostCLI-0.5.3.tar", last modified: Wed Sep 14 04:25:54 2022, max compression
+gzip compressed data, was "BoostCLI-0.6.0.tar", last modified: Sat Apr 13 07:33:30 2024, max compression
```

## Comparing `BoostCLI-0.5.3.tar` & `BoostCLI-0.6.0.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-14 04:25:54.234984 BoostCLI-0.5.3/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-14 04:25:54.230984 BoostCLI-0.5.3/BoostCLI.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     3501 2022-09-14 04:25:54.000000 BoostCLI-0.5.3/BoostCLI.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      749 2022-09-14 04:25:54.000000 BoostCLI-0.5.3/BoostCLI.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2022-09-14 04:25:54.000000 BoostCLI-0.5.3/BoostCLI.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       41 2022-09-14 04:25:54.000000 BoostCLI-0.5.3/BoostCLI.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)      263 2022-09-14 04:25:54.000000 BoostCLI-0.5.3/BoostCLI.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        4 2022-09-14 04:25:54.000000 BoostCLI-0.5.3/BoostCLI.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1529 2022-03-04 08:12:35.000000 BoostCLI-0.5.3/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)     3501 2022-09-14 04:25:54.234984 BoostCLI-0.5.3/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     3211 2022-09-03 18:34:56.000000 BoostCLI-0.5.3/README.md
--rw-rw-r--   0 user      (1000) user      (1000)       89 2022-01-05 09:34:52.000000 BoostCLI-0.5.3/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)       38 2022-09-14 04:25:54.234984 BoostCLI-0.5.3/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1225 2022-09-14 04:24:30.000000 BoostCLI-0.5.3/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-14 04:25:54.230984 BoostCLI-0.5.3/src/
--rw-r--r--   0 user      (1000) user      (1000)        0 2021-11-04 06:30:20.000000 BoostCLI-0.5.3/src/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-14 04:25:54.230984 BoostCLI-0.5.3/src/cli/
--rw-rw-r--   0 user      (1000) user      (1000)      351 2022-09-14 04:12:34.000000 BoostCLI-0.5.3/src/cli/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)       56 2022-07-28 07:02:57.000000 BoostCLI-0.5.3/src/cli/__main__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3053 2022-09-03 18:34:56.000000 BoostCLI-0.5.3/src/cli/cli.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-14 04:25:54.230984 BoostCLI-0.5.3/src/cli/commands/
--rw-r--r--   0 user      (1000) user      (1000)        0 2022-09-14 04:23:19.000000 BoostCLI-0.5.3/src/cli/commands/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     9763 2022-09-03 18:34:56.000000 BoostCLI-0.5.3/src/cli/commands/boost.py
--rw-rw-r--   0 user      (1000) user      (1000)      668 2022-09-03 18:34:56.000000 BoostCLI-0.5.3/src/cli/commands/incoming_boosts.py
--rw-rw-r--   0 user      (1000) user      (1000)     1015 2022-09-03 18:34:56.000000 BoostCLI-0.5.3/src/cli/commands/received_boosts.py
--rw-rw-r--   0 user      (1000) user      (1000)      997 2022-09-03 18:34:56.000000 BoostCLI-0.5.3/src/cli/commands/sent_boosts.py
--rw-r--r--   0 user      (1000) user      (1000)     1903 2022-09-07 06:10:31.000000 BoostCLI-0.5.3/src/cli/commands/wip.py
--rw-rw-r--   0 user      (1000) user      (1000)     1961 2022-09-03 18:34:56.000000 BoostCLI-0.5.3/src/cli/print_value.py
--rw-rw-r--   0 user      (1000) user      (1000)     5148 2022-07-29 05:53:18.000000 BoostCLI-0.5.3/src/models.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-14 04:25:54.230984 BoostCLI-0.5.3/src/providers/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2022-01-06 05:20:40.000000 BoostCLI-0.5.3/src/providers/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      711 2022-02-27 19:19:15.000000 BoostCLI-0.5.3/src/providers/feed_provider.py
--rw-rw-r--   0 user      (1000) user      (1000)     2241 2022-03-27 05:02:41.000000 BoostCLI-0.5.3/src/providers/podcast_index_provider.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-09-14 04:25:54.230984 BoostCLI-0.5.3/src/services/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2022-01-06 05:19:03.000000 BoostCLI-0.5.3/src/services/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     3864 2022-05-05 05:11:57.000000 BoostCLI-0.5.3/src/services/feed_service.py
--rw-rw-r--   0 user      (1000) user      (1000)     9793 2022-09-03 18:34:56.000000 BoostCLI-0.5.3/src/services/lightning_service.py
--rw-rw-r--   0 user      (1000) user      (1000)     3183 2022-07-24 05:21:56.000000 BoostCLI-0.5.3/src/services/podcast_index_service.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-13 07:33:30.129745 BoostCLI-0.6.0/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-13 07:33:30.125745 BoostCLI-0.6.0/BoostCLI.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      798 2024-04-13 07:33:30.000000 BoostCLI-0.6.0/BoostCLI.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      746 2024-04-13 07:33:30.000000 BoostCLI-0.6.0/BoostCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-04-13 07:33:30.000000 BoostCLI-0.6.0/BoostCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       41 2024-04-13 07:33:30.000000 BoostCLI-0.6.0/BoostCLI.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1000) user      (1000)      289 2024-04-13 07:33:30.000000 BoostCLI-0.6.0/BoostCLI.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        4 2024-04-13 07:33:30.000000 BoostCLI-0.6.0/BoostCLI.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)     1529 2024-04-06 06:57:00.000000 BoostCLI-0.6.0/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)      798 2024-04-13 07:33:30.129745 BoostCLI-0.6.0/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     3211 2024-04-06 06:57:00.000000 BoostCLI-0.6.0/README.md
+-rw-r--r--   0 user      (1000) user      (1000)      861 2024-04-13 07:32:51.000000 BoostCLI-0.6.0/pyproject.toml
+-rw-r--r--   0 user      (1000) user      (1000)       38 2024-04-13 07:33:30.130745 BoostCLI-0.6.0/setup.cfg
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-13 07:33:30.110745 BoostCLI-0.6.0/src/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2024-04-06 06:57:00.000000 BoostCLI-0.6.0/src/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-13 07:33:30.114745 BoostCLI-0.6.0/src/cli/
+-rw-r--r--   0 user      (1000) user      (1000)      351 2024-04-06 06:57:00.000000 BoostCLI-0.6.0/src/cli/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)       56 2024-04-06 06:57:00.000000 BoostCLI-0.6.0/src/cli/__main__.py
+-rw-r--r--   0 user      (1000) user      (1000)     2988 2024-04-13 07:15:39.000000 BoostCLI-0.6.0/src/cli/cli.py
+-rw-r--r--   0 user      (1000) user      (1000)     1961 2024-04-06 06:57:00.000000 BoostCLI-0.6.0/src/cli/print_value.py
+-rw-r--r--   0 user      (1000) user      (1000)     5148 2024-04-06 06:57:00.000000 BoostCLI-0.6.0/src/models.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-13 07:33:30.115745 BoostCLI-0.6.0/src/providers/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2024-04-06 06:57:00.000000 BoostCLI-0.6.0/src/providers/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      711 2024-04-06 06:57:00.000000 BoostCLI-0.6.0/src/providers/feed_provider.py
+-rw-r--r--   0 user      (1000) user      (1000)     2241 2024-04-06 06:57:00.000000 BoostCLI-0.6.0/src/providers/podcast_index_provider.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-13 07:33:30.119745 BoostCLI-0.6.0/src/services/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2024-04-06 06:57:00.000000 BoostCLI-0.6.0/src/services/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     3865 2024-04-13 07:15:39.000000 BoostCLI-0.6.0/src/services/feed_service.py
+-rw-r--r--   0 user      (1000) user      (1000)    11051 2024-04-13 07:15:39.000000 BoostCLI-0.6.0/src/services/lightning_service.py
+-rw-r--r--   0 user      (1000) user      (1000)     3183 2024-04-06 06:57:00.000000 BoostCLI-0.6.0/src/services/podcast_index_service.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-13 07:33:30.124745 BoostCLI-0.6.0/tests/
+-rw-r--r--   0 user      (1000) user      (1000)      313 2024-04-06 06:57:00.000000 BoostCLI-0.6.0/tests/test_commands_boost.py
+-rw-r--r--   0 user      (1000) user      (1000)     1857 2024-04-06 06:57:00.000000 BoostCLI-0.6.0/tests/test_feed_provider.py
+-rw-r--r--   0 user      (1000) user      (1000)     5361 2024-04-06 06:57:00.000000 BoostCLI-0.6.0/tests/test_feed_service.py
+-rw-r--r--   0 user      (1000) user      (1000)        0 2024-04-06 06:57:00.000000 BoostCLI-0.6.0/tests/test_lightning_service.py
+-rw-r--r--   0 user      (1000) user      (1000)     2405 2024-04-06 06:57:00.000000 BoostCLI-0.6.0/tests/test_podcast_index_provider.py
+-rw-r--r--   0 user      (1000) user      (1000)     3648 2024-04-06 06:57:00.000000 BoostCLI-0.6.0/tests/test_podcast_index_service.py
```

### Comparing `BoostCLI-0.5.3/BoostCLI.egg-info/PKG-INFO` & `BoostCLI-0.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: BoostCLI
-Version: 0.5.3
-Summary: Command line tool to send and receive Podcasting 2.0 Value
-Author-email: boostcli.v1pty@slmail.me
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: deploy
-License-File: LICENSE
-
 
 # BoostCLI
 
 <img width=100 height=100 src="boostcli.png" />
 
 [![Tests](https://github.com/valcanobacon/BoostCLI/actions/workflows/ci.yml/badge.svg)](https://github.com/valcanobacon/BoostCLI/actions/workflows/ci.yml)
```

### Comparing `BoostCLI-0.5.3/LICENSE` & `BoostCLI-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `BoostCLI-0.5.3/src/cli/cli.py` & `BoostCLI-0.6.0/src/cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import click
 from rich.console import Console
 
 from src.services.feed_service import FeedService
 
 from src.providers.podcast_index_provider import PodcastIndexProvider
-from src.services.lightning_service import LightningService
 from src.services.lightning_service import client_from as lightning_client_from
 from src.services.podcast_index_service import PodcastIndexService
 
 
 CONTEXT_SETTINGS = dict(
     show_default=True,
 )
@@ -30,19 +29,21 @@
     metavar="PORT",
     help="Port of the LND server",
 )
 @click.option(
     "--macaroon",
     type=click.Path(exists=True),
     help="Path to the Macaroon for LND for access to the LND server",
+    default="admin.macaroon",
 )
 @click.option(
     "--tlscert",
     type=click.Path(exists=True),
     help="Path of the TLS Certificate for connection to the LND server",
+    default="tls.cert",
 )
 @click.pass_context
 def cli(ctx, **kwargs):
     """
     BoostCLI works by establishing a connection to an LND Server then
     preforming a Command. BoostCLI's first options configure the connection:
     `address`, `port`, `macaroon` and `tlscert`. After the connection
@@ -63,21 +64,19 @@
     # we need to use that cipher suite otherwise there will be a handhsake
     # error when we communicate with the lnd rpc server.
     os.environ["GRPC_SSL_CIPHER_SUITES"] = "HIGH+ECDSA"
 
     console = ctx.obj["console"] = Console()
     console_error = ctx.obj["console_error"] = Console(stderr=True, style="bold red")
 
-    lightning_service = ctx.obj["lightning_service"] = LightningService(
-        client=lightning_client_from(
-            host=kwargs["address"],
-            port=kwargs["port"],
-            cert_filepath=kwargs["tlscert"],
-            macaroon_filepath=kwargs["macaroon"],
-        )
+    lightning_service = ctx.obj["lightning_service"] = lightning_client_from(
+        host=kwargs["address"],
+        port=kwargs["port"],
+        cert_filepath=kwargs["tlscert"],
+        macaroon_filepath=kwargs["macaroon"],
     )
 
     ctx.obj["podcast_index_service"] = PodcastIndexService(
         provider=PodcastIndexProvider(
             user_agent="Boost Account",
             api_key="5K3YPBAKHWAEBR6R9ZNY",
             api_secret="zrnd^d9HtMH4aH#vBQSPsSKES6$pVtv^ra2dkQFq",
```

### Comparing `BoostCLI-0.5.3/src/cli/print_value.py` & `BoostCLI-0.6.0/src/cli/print_value.py`

 * *Files identical despite different names*

### Comparing `BoostCLI-0.5.3/src/models.py` & `BoostCLI-0.6.0/src/models.py`

 * *Files identical despite different names*

### Comparing `BoostCLI-0.5.3/src/providers/feed_provider.py` & `BoostCLI-0.6.0/src/providers/feed_provider.py`

 * *Files identical despite different names*

### Comparing `BoostCLI-0.5.3/src/providers/podcast_index_provider.py` & `BoostCLI-0.6.0/src/providers/podcast_index_provider.py`

 * *Files identical despite different names*

### Comparing `BoostCLI-0.5.3/src/services/feed_service.py` & `BoostCLI-0.6.0/src/services/feed_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
         podcast_value_soup = None
         podcast_liveitem_soup = None
 
         podcast_liveitems = response.data.find_all(
             "podcast:liveitem",
             recursive=True,
-            attrs={"status": "live"}
+            attrs={"status": "live"},
             # "podcast:liveitem", recursive=True,
         )
         for soup in podcast_liveitems:
             podcast_liveitem_soup = soup
             podcast_value_soup = next(
                 iter(soup.find_all("podcast:value")),
                 None,
```

### Comparing `BoostCLI-0.5.3/src/services/lightning_service.py` & `BoostCLI-0.6.0/src/services/lightning_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,60 +3,84 @@
 import itertools
 import json
 import secrets
 import time
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Generator, Optional
+import os
 
-import grpc
 from google.protobuf.json_format import MessageToJson
-from lndgrpc import LNDClient
 
 from src.models import BoostInvoice, ValueForValue
+from src.providers.lightning_provider import LightningProvider, channel_from
+from src.lnd import lightning_pb2 as ln
+
+
+def read_macaroon(filename):
+    with open(filename, "rb") as file_:
+        return codecs.encode(file_.read(), "hex")
+
+
+def read_tlscert(filename):
+    with open(filename, "rb") as file_:
+        return file_.read()
 
 
 def client_from(
     host: str, port: str, cert_filepath: str, macaroon_filepath: str
-) -> grpc.Channel:
-    return LNDClient(
-        ip_address=f"{host}:{port}",
-        cert_filepath=cert_filepath,
-        macaroon_filepath=macaroon_filepath,
+) -> "LightningService":
+    # from: https://github.com/lightningnetwork/lnd/blob/master/docs/grpc/python.md
+    # Due to updated ECDSA generated tls.cert we need to let gprc know that
+    # we need to use that cipher suite otherwise there will be a handhsake
+    # error when we communicate with the lnd rpc server.
+    os.environ["GRPC_SSL_CIPHER_SUITES"] = "HIGH+ECDSA"
+
+    return LightningService(
+        provider=LightningProvider.from_channel(
+            channel_from(
+                host=host,
+                port=port,
+                cert=read_tlscert(filename=cert_filepath),
+                macaroon=read_macaroon(filename=macaroon_filepath),
+            )
+        )
     )
 
 
 @dataclass(frozen=True)
 class LightningService:
 
-    client: LNDClient
+    provider: LightningProvider
 
     @classmethod
-    def from_client(cls, client: LNDClient) -> "LightningService":
-        return LightningService(client=client)
+    def from_client(cls, provider: LightningProvider) -> "LightningService":
+        return LightningService(provider=provider)
 
     def parse_grpc_message(self, grpc_message) -> Any:
         return json.loads(MessageToJson(grpc_message))
 
     def get_info(self):
-        return self.client.get_info()
+        return self.provider.lightning_stub.GetInfo(ln.GetInfoRequest())
 
     def invoices(
         self,
         index_offset=0,
         max_number_of_invoices=None,
         accending=True,
         pending_only=False,
     ) -> Generator:
 
-        response = self.client.list_invoices(
-            index_offset=index_offset,
-            num_max_invoices=max_number_of_invoices,
-            reversed=accending,
-            pending_only=pending_only,
+        response = self.provider.lightning_stub.ListInvoices(
+            ln.ListInvoiceRequest(
+                index_offset=index_offset,
+                num_max_invoices=max_number_of_invoices,
+                reversed=accending,
+                pending_only=pending_only,
+            )
         )
 
         if not response:
             return
 
         invoices = response.invoices
 
@@ -68,32 +92,36 @@
     def payments(
         self,
         index_offset=0,
         max_payments=None,
         accending=True,
     ) -> Generator:
 
-        response = self.client.list_payments(
-            index_offset=index_offset,
-            max_payments=max_payments,
-            reversed=accending,
+        response = self.provider.lightning_stub.ListPayments(
+            ln.ListPaymentsRequest(
+                index_offset=index_offset,
+                max_payments=max_payments,
+                reversed=accending,
+            )
         )
 
         if not response:
             return
 
         payments = response.payments
 
         if accending:
             payments = reversed(payments)
 
         yield from payments
 
     def watch_value_received(self):
-        for invoice in self.client.subscribe_invoices():
+        for invoice in self.provider.lightning_stub.SubscribeInvoices(
+            ln.InvoiceSubscription()
+        ):
             try:
                 value = self.invoice_to_value(invoice)
             except:
                 continue
             if value is not None:
                 yield value
 
@@ -255,22 +283,25 @@
             if destination.custom_key and destination.custom_value:
                 custom_records.append(
                     (destination.custom_key, destination.custom_value)
                 )
 
             dest = codecs.decode(destination.receiver_address, "hex")
 
-            response = self.client.send_payment(
-                payment_request=None,
-                fee_limit_msat=int(destination.amount_msats * 0.10),
-                dest=dest,
-                amt_msat=destination.amount_msats,
-                dest_custom_records=custom_records,
-                payment_hash=bytes.fromhex(hashed_secret),
-                allow_self_payment=True,
+            fee_limit = ln.FeeLimit(fixed_msat=int(destination.amount_msats * 0.10))
+            response = self.provider.lightning_stub.SendPaymentSync(
+                ln.SendRequest(
+                    payment_request=None,
+                    fee_limit=fee_limit,
+                    dest=dest,
+                    amt_msat=destination.amount_msats,
+                    dest_custom_records=custom_records,
+                    payment_hash=bytes.fromhex(hashed_secret),
+                    allow_self_payment=True,
+                )
             )
             if not response:
                 continue
             yield response
 
 
 def try_to_json_decode(value: str) -> Any:
```

### Comparing `BoostCLI-0.5.3/src/services/podcast_index_service.py` & `BoostCLI-0.6.0/src/services/podcast_index_service.py`

 * *Files identical despite different names*

