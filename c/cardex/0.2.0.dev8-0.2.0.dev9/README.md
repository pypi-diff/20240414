# Comparing `tmp/cardex-0.2.0.dev8.tar.gz` & `tmp/cardex-0.2.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardex-0.2.0.dev8.tar", max compression
+gzip compressed data, was "cardex-0.2.0.dev9.tar", max compression
```

## Comparing `cardex-0.2.0.dev8.tar` & `cardex-0.2.0.dev9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35115 2023-11-25 19:28:16.618733 cardex-0.2.0.dev8/LICENSE
--rw-r--r--   0        0        0        0 2023-11-25 00:47:56.601477 cardex-0.2.0.dev8/README.md
--rw-r--r--   0        0        0      855 2023-12-29 18:35:31.566844 cardex-0.2.0.dev8/pyproject.toml
--rw-r--r--   0        0        0      439 2023-12-17 00:14:15.994916 cardex-0.2.0.dev8/src/cardex/__init__.py
--rw-r--r--   0        0        0        0 2023-11-25 19:37:10.561449 cardex-0.2.0.dev8/src/cardex/backend/__init__.py
--rw-r--r--   0        0        0        0 2023-12-20 00:40:05.071771 cardex-0.2.0.dev8/src/cardex/backend/blockfrost.py
--rw-r--r--   0        0        0     6606 2023-12-28 22:25:53.312378 cardex-0.2.0.dev8/src/cardex/backend/dbsync.py
--rw-r--r--   0        0        0        7 2023-12-15 21:46:07.338340 cardex-0.2.0.dev8/src/cardex/dataclasses/__init__.py
--rw-r--r--   0        0        0     2460 2023-12-28 21:29:45.268356 cardex-0.2.0.dev8/src/cardex/dataclasses/datums.py
--rw-r--r--   0        0        0     3620 2023-12-29 16:27:33.577720 cardex-0.2.0.dev8/src/cardex/dataclasses/models.py
--rw-r--r--   0        0        0        0 2023-12-15 21:07:11.663822 cardex-0.2.0.dev8/src/cardex/dexs/__init__.py
--rw-r--r--   0        0        0    16299 2023-12-29 18:25:19.681936 cardex-0.2.0.dev8/src/cardex/dexs/amm_base.py
--rw-r--r--   0        0        0     6785 2023-12-29 16:27:46.809898 cardex-0.2.0.dev8/src/cardex/dexs/amm_types.py
--rw-r--r--   0        0        0      507 2023-12-28 16:46:32.412198 cardex-0.2.0.dev8/src/cardex/dexs/errors.py
--rw-r--r--   0        0        0     5070 2023-12-29 03:02:11.760668 cardex-0.2.0.dev8/src/cardex/dexs/minswap.py
--rw-r--r--   0        0        0     7032 2023-12-29 16:27:33.577720 cardex-0.2.0.dev8/src/cardex/dexs/muesli.py
--rw-r--r--   0        0        0     8080 2023-12-29 16:27:33.577720 cardex-0.2.0.dev8/src/cardex/dexs/spectrum.py
--rw-r--r--   0        0        0     6331 2023-12-29 03:03:12.669431 cardex-0.2.0.dev8/src/cardex/dexs/sundae.py
--rw-r--r--   0        0        0     5967 2023-12-29 03:03:21.401540 cardex-0.2.0.dev8/src/cardex/dexs/vyfi.py
--rw-r--r--   0        0        0     6819 2023-12-29 03:03:31.701670 cardex-0.2.0.dev8/src/cardex/dexs/wingriders.py
--rw-r--r--   0        0        0     4526 2023-12-28 16:45:45.031601 cardex-0.2.0.dev8/src/cardex/utility.py
--rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 cardex-0.2.0.dev8/PKG-INFO
+-rw-r--r--   0        0        0    35115 2023-11-25 19:28:16.618733 cardex-0.2.0.dev9/LICENSE
+-rw-r--r--   0        0        0        0 2023-11-25 00:47:56.601477 cardex-0.2.0.dev9/README.md
+-rw-r--r--   0        0        0      855 2023-12-30 03:53:05.864880 cardex-0.2.0.dev9/pyproject.toml
+-rw-r--r--   0        0        0      439 2023-12-17 00:14:15.994916 cardex-0.2.0.dev9/src/cardex/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-25 19:37:10.561449 cardex-0.2.0.dev9/src/cardex/backend/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-20 00:40:05.071771 cardex-0.2.0.dev9/src/cardex/backend/blockfrost.py
+-rw-r--r--   0        0        0     6606 2023-12-28 22:25:53.312378 cardex-0.2.0.dev9/src/cardex/backend/dbsync.py
+-rw-r--r--   0        0        0        7 2023-12-15 21:46:07.338340 cardex-0.2.0.dev9/src/cardex/dataclasses/__init__.py
+-rw-r--r--   0        0        0     2460 2023-12-28 21:29:45.268356 cardex-0.2.0.dev9/src/cardex/dataclasses/datums.py
+-rw-r--r--   0        0        0     3620 2023-12-29 16:27:33.577720 cardex-0.2.0.dev9/src/cardex/dataclasses/models.py
+-rw-r--r--   0        0        0        0 2023-12-15 21:07:11.663822 cardex-0.2.0.dev9/src/cardex/dexs/__init__.py
+-rw-r--r--   0        0        0    16538 2023-12-30 02:36:16.805252 cardex-0.2.0.dev9/src/cardex/dexs/amm_base.py
+-rw-r--r--   0        0        0     6785 2023-12-30 02:34:01.987381 cardex-0.2.0.dev9/src/cardex/dexs/amm_types.py
+-rw-r--r--   0        0        0      507 2023-12-28 16:46:32.412198 cardex-0.2.0.dev9/src/cardex/dexs/errors.py
+-rw-r--r--   0        0        0     5070 2023-12-29 03:02:11.760668 cardex-0.2.0.dev9/src/cardex/dexs/minswap.py
+-rw-r--r--   0        0        0     7172 2023-12-30 03:52:33.944459 cardex-0.2.0.dev9/src/cardex/dexs/muesli.py
+-rw-r--r--   0        0        0     8080 2023-12-29 16:27:33.577720 cardex-0.2.0.dev9/src/cardex/dexs/spectrum.py
+-rw-r--r--   0        0        0     6331 2023-12-29 03:03:12.669431 cardex-0.2.0.dev9/src/cardex/dexs/sundae.py
+-rw-r--r--   0        0        0     5967 2023-12-29 03:03:21.401540 cardex-0.2.0.dev9/src/cardex/dexs/vyfi.py
+-rw-r--r--   0        0        0     6819 2023-12-29 03:03:31.701670 cardex-0.2.0.dev9/src/cardex/dexs/wingriders.py
+-rw-r--r--   0        0        0     4526 2023-12-28 16:45:45.031601 cardex-0.2.0.dev9/src/cardex/utility.py
+-rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 cardex-0.2.0.dev9/PKG-INFO
```

### Comparing `cardex-0.2.0.dev8/LICENSE` & `cardex-0.2.0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `cardex-0.2.0.dev8/pyproject.toml` & `cardex-0.2.0.dev9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cardex"
-version = "0.2.0-dev8"
+version = "0.2.0-dev9"
 description = ""
 authors = ["Elder Millenial <eldermillenial@protonmail.com>"]
 readme = "README.md"
 packages = [{include = "cardex", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `cardex-0.2.0.dev8/src/cardex/backend/dbsync.py` & `cardex-0.2.0.dev9/src/cardex/backend/dbsync.py`

 * *Files identical despite different names*

### Comparing `cardex-0.2.0.dev8/src/cardex/dataclasses/datums.py` & `cardex-0.2.0.dev9/src/cardex/dataclasses/datums.py`

 * *Files identical despite different names*

### Comparing `cardex-0.2.0.dev8/src/cardex/dataclasses/models.py` & `cardex-0.2.0.dev9/src/cardex/dataclasses/models.py`

 * *Files identical despite different names*

### Comparing `cardex-0.2.0.dev8/src/cardex/dexs/amm_base.py` & `cardex-0.2.0.dev9/src/cardex/dexs/amm_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,18 +307,19 @@
 
         # If no pool policy id defined, return nothing
         if cls.pool_policy is None:
             return None
 
         # If the pool nft is in the values, it's been parsed already
         elif "pool_nft" in values:
-            assert any(
+            if not any(
                 any(p.startswith(d) for d in cls.pool_policy)
                 for p in values["pool_nft"]
-            )
+            ):
+                raise InvalidPoolError(f"{cls.__name__}: Invalid pool NFT: {values}")
             pool_nft = Assets(
                 **{key: value for key, value in values["pool_nft"].items()},
             )
 
         # Check for the pool nft
         else:
             nfts = [
@@ -358,18 +359,21 @@
         # If no pool policy id defined, return nothing
         if cls.lp_policy is None:
             return None
 
         # If the pool nft is in the values, it's been parsed already
         elif "lp_tokens" in values:
             if values["lp_tokens"] is not None:
-                assert any(
+                if not any(
                     any(p.startswith(d) for d in cls.lp_policy)
                     for p in values["lp_tokens"]
-                )
+                ):
+                    raise InvalidPoolError(
+                        f"{cls.__name__}: Pool has invalid LP tokens.",
+                    )
             lp_tokens = values["lp_tokens"]
 
         # Check for the pool nft
         else:
             nfts = [
                 asset
                 for asset in assets
@@ -448,15 +452,15 @@
 
         if cls.skip_init(values):
             return values
 
         # Parse the pool datum
         try:
             datum = cls.pool_datum_class.from_cbor(values["datum_cbor"])
-        except DeserializeException:
+        except (DeserializeException, TypeError):
             raise NotAPoolError(
                 f"Pool datum could not be deserialized: {values['datum_cbor']}",
             )
 
         # To help prevent edge cases, remove pool tokens while running other checks
         pair = Assets({})
         if datum.pool_pair() is not None:
```

### Comparing `cardex-0.2.0.dev8/src/cardex/dexs/amm_types.py` & `cardex-0.2.0.dev9/src/cardex/dexs/amm_types.py`

 * *Files identical despite different names*

### Comparing `cardex-0.2.0.dev8/src/cardex/dexs/minswap.py` & `cardex-0.2.0.dev9/src/cardex/dexs/minswap.py`

 * *Files identical despite different names*

### Comparing `cardex-0.2.0.dev8/src/cardex/dexs/muesli.py` & `cardex-0.2.0.dev9/src/cardex/dexs/muesli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from dataclasses import dataclass
 from typing import Any
+from typing import ClassVar
 from typing import Optional
 
 from pycardano import Address
 from pycardano import PlutusData
 
 from cardex.dataclasses.datums import AssetClass
 from cardex.dataclasses.datums import PlutusFullAddress
 from cardex.dataclasses.datums import PlutusNone
 from cardex.dataclasses.models import PoolSelector
 from cardex.dexs.amm_types import AbstractConstantLiquidityPoolState
 from cardex.dexs.amm_types import AbstractConstantProductPoolState
 from cardex.dexs.errors import InvalidPoolError
-from cardex.dexs.errors import NotAPoolError
 from cardex.utility import Assets
 
 
 @dataclass
 class MuesliOrderConfig(PlutusData):
     CONSTR_ID = 0
 
@@ -105,15 +105,17 @@
     unknown: int
 
 
 class MuesliSwapCPPState(AbstractConstantProductPoolState):
     fee: int = 30
     _batcher = Assets(lovelace=950000)
     _deposit = Assets(lovelace=1700000)
-    _test_pool = "a8512101cb1163cc218e616bb4d4070349a1c9395313f1323cc583634d7565736c695377617054657374506f6f6c"
+    _test_pool: ClassVar[
+        str
+    ] = "a8512101cb1163cc218e616bb4d4070349a1c9395313f1323cc583634d7565736c695377617054657374506f6f6c"
     _stake_address = Address.from_primitive(
         "addr1zyq0kyrml023kwjk8zr86d5gaxrt5w8lxnah8r6m6s4jp4g3r6dxnzml343sx8jweqn4vn3fz2kj8kgu9czghx0jrsyqqktyhv",
     )
 
     @classmethod
     @property
     def dex(cls) -> str:
@@ -201,21 +203,24 @@
             values: The pool UTXO inputs.
 
         Returns:
             Assets: None or the dex nft.
         """
         assets = values["assets"]
 
-        nfts = [asset for asset, quantity in assets.items() if quantity == 1]
-        if len(nfts) != 1:
-            raise NotAPoolError(
-                f"MuesliSwap pools must have exactly one pool nft: assets={assets}",
-            )
-        pool_nft = Assets(**{nfts[0]: assets.root.pop(nfts[0])})
-        values["pool_nft"] = pool_nft
+        if "pool_nft" in values:
+            pool_nft = Assets(root=values["pool_nft"])
+        else:
+            nfts = [asset for asset, quantity in assets.items() if quantity == 1]
+            if len(nfts) != 1:
+                raise InvalidPool(
+                    f"MuesliSwap pools must have exactly one pool nft: assets={assets}",
+                )
+            pool_nft = Assets(**{nfts[0]: assets.root.pop(nfts[0])})
+            values["pool_nft"] = pool_nft
 
         return pool_nft
 
 
 class MuesliSwapCLPState(AbstractConstantLiquidityPoolState, MuesliSwapCPPState):
     inactive: bool = True
```

### Comparing `cardex-0.2.0.dev8/src/cardex/dexs/spectrum.py` & `cardex-0.2.0.dev9/src/cardex/dexs/spectrum.py`

 * *Files identical despite different names*

### Comparing `cardex-0.2.0.dev8/src/cardex/dexs/sundae.py` & `cardex-0.2.0.dev9/src/cardex/dexs/sundae.py`

 * *Files identical despite different names*

### Comparing `cardex-0.2.0.dev8/src/cardex/dexs/vyfi.py` & `cardex-0.2.0.dev9/src/cardex/dexs/vyfi.py`

 * *Files identical despite different names*

### Comparing `cardex-0.2.0.dev8/src/cardex/dexs/wingriders.py` & `cardex-0.2.0.dev9/src/cardex/dexs/wingriders.py`

 * *Files identical despite different names*

### Comparing `cardex-0.2.0.dev8/src/cardex/utility.py` & `cardex-0.2.0.dev9/src/cardex/utility.py`

 * *Files identical despite different names*

### Comparing `cardex-0.2.0.dev8/PKG-INFO` & `cardex-0.2.0.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardex
-Version: 0.2.0.dev8
+Version: 0.2.0.dev9
 Summary: 
 Author: Elder Millenial
 Author-email: eldermillenial@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

