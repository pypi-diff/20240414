# Comparing `tmp/oxtapus-0.3.0-py3-none-any.whl.zip` & `tmp/oxtapus-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,27 @@
-Zip file size: 37587 bytes, number of entries: 25
+Zip file size: 37774 bytes, number of entries: 25
 -rw-r--r--  2.0 unx     6148 b- defN 80-Jan-01 00:00 oxtapus/.DS_Store
 -rw-r--r--  2.0 unx      102 b- defN 80-Jan-01 00:00 oxtapus/__init__.py
 -rw-r--r--  2.0 unx     2746 b- defN 80-Jan-01 00:00 oxtapus/codal.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 oxtapus/models/__init__.py
 -rw-r--r--  2.0 unx     2122 b- defN 80-Jan-01 00:00 oxtapus/models/rahavard.py
--rw-r--r--  2.0 unx     2230 b- defN 80-Jan-01 00:00 oxtapus/models/tsetmc.py
+-rw-r--r--  2.0 unx     2731 b- defN 80-Jan-01 00:00 oxtapus/models/tsetmc.py
 -rw-r--r--  2.0 unx    25365 b- defN 80-Jan-01 00:00 oxtapus/rahavard.py
 -rw-r--r--  2.0 unx     6082 b- defN 80-Jan-01 00:00 oxtapus/tgju.py
--rw-r--r--  2.0 unx    83546 b- defN 80-Jan-01 00:00 oxtapus/tsetmc.py
+-rw-r--r--  2.0 unx    83931 b- defN 80-Jan-01 00:00 oxtapus/tsetmc.py
 -rw-r--r--  2.0 unx      165 b- defN 80-Jan-01 00:00 oxtapus/utils/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 oxtapus/utils/codal/__init__.py
 -rw-r--r--  2.0 unx    10916 b- defN 80-Jan-01 00:00 oxtapus/utils/codal/clean_data.py
 -rw-r--r--  2.0 unx     6854 b- defN 80-Jan-01 00:00 oxtapus/utils/codal/items.py
 -rw-r--r--  2.0 unx     4882 b- defN 80-Jan-01 00:00 oxtapus/utils/codal/models.py
 -rw-r--r--  2.0 unx     1036 b- defN 80-Jan-01 00:00 oxtapus/utils/codal/request.py
 -rw-r--r--  2.0 unx     1042 b- defN 80-Jan-01 00:00 oxtapus/utils/codal/utils.py
 -rw-r--r--  2.0 unx     5767 b- defN 80-Jan-01 00:00 oxtapus/utils/columns.py
 -rw-r--r--  2.0 unx       47 b- defN 80-Jan-01 00:00 oxtapus/utils/http/__init__.py
 -rw-r--r--  2.0 unx     2156 b- defN 80-Jan-01 00:00 oxtapus/utils/http/requests.py
 -rw-r--r--  2.0 unx     2926 b- defN 80-Jan-01 00:00 oxtapus/utils/models.py
 -rw-r--r--  2.0 unx      825 b- defN 80-Jan-01 00:00 oxtapus/utils/normalize.py
--rw-r--r--  2.0 unx     1071 b- defN 80-Jan-01 00:00 oxtapus-0.3.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    19557 b- defN 80-Jan-01 00:00 oxtapus-0.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 oxtapus-0.3.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2004 b- defN 16-Jan-01 00:00 oxtapus-0.3.0.dist-info/RECORD
-25 files, 187677 bytes uncompressed, 34381 bytes compressed:  81.7%
+-rw-r--r--  2.0 unx     1071 b- defN 80-Jan-01 00:00 oxtapus-0.3.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    19557 b- defN 80-Jan-01 00:00 oxtapus-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 oxtapus-0.3.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2004 b- defN 16-Jan-01 00:00 oxtapus-0.3.1.dist-info/RECORD
+25 files, 188563 bytes uncompressed, 34568 bytes compressed:  81.7%
```

## zipnote {}

```diff
@@ -57,20 +57,20 @@
 
 Filename: oxtapus/utils/models.py
 Comment: 
 
 Filename: oxtapus/utils/normalize.py
 Comment: 
 
-Filename: oxtapus-0.3.0.dist-info/LICENSE.txt
+Filename: oxtapus-0.3.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: oxtapus-0.3.0.dist-info/METADATA
+Filename: oxtapus-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: oxtapus-0.3.0.dist-info/WHEEL
+Filename: oxtapus-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: oxtapus-0.3.0.dist-info/RECORD
+Filename: oxtapus-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## oxtapus/models/tsetmc.py

```diff
@@ -8,14 +8,26 @@
     bid_size: float = Field(alias="qmd")
     bid_price: float = Field(alias="pmd")
     ask_price: float = Field(alias="pmo")
     ask_size: float = Field(alias="qmo")
     ask_count: int = Field(alias="zmo")
 
 
+class ClientTypeAll(BaseModel):
+    ins_code: str = Field(alias="insCode")
+    buy_vol_ind: float = Field(alias="buy_I_Volume")
+    buy_vol_ins: float = Field(alias="buy_N_Volume")
+    buy_count_ind: int = Field(alias="buy_CountI")
+    buy_count_ins: int = Field(alias="buy_CountN")
+    sell_vol_ind: float = Field(alias="sell_I_Volume")
+    sell_vol_ins: float = Field(alias="sell_N_Volume")
+    sell_count_ind: int = Field(alias="sell_CountI")
+    sell_count_ins: int = Field(alias="sell_CountN")
+
+
 class MarketWatch(BaseModel):
     ins_code: str = Field(alias="insCode")
     ins_id: str = Field(alias="insID")
     symbol: str = Field(alias="lva")
     name: str = Field(alias="lvc")
     eps: float = Field(alias="eps")
     pe: float = Field(alias="pe")
```

## oxtapus/tsetmc.py

```diff
@@ -2,15 +2,15 @@
 import datetime
 from enum import Enum
 import polars as pl
 from typing import List
 from pydantic import validate_call
 from urllib.parse import urlencode
 import itertools
-from oxtapus.models.tsetmc import HistPrice, MarketWatch
+from oxtapus.models.tsetmc import HistPrice, MarketWatch, ClientTypeAll
 
 from oxtapus.utils.http import requests, async_requests
 from oxtapus.utils import (
     json_normalize,
     word_normalize,
     manipulation_cols,
     cols,
@@ -92,14 +92,17 @@
             "industrialGroup": "",
             **papers,
             "showTraded": "false",
             "withBestLimits": "true",
         }
         return f"{self.base_url}/ClosingPrice/GetMarketWatch?{urlencode(param)}"
 
+    def client_type_all(self):
+        return f"{self.base_url}/ClientType/GetClientTypeAll"
+
     def search_ins_code(self, symbol_far) -> str:
         """
         .. raw:: html
 
             <div dir="rtl">
                 لینکِ جست-و-جوی نماد رو می‌سازه.
             </div>
@@ -312,19 +315,23 @@
         example
         -------
         >>> from oxtapus import TSETMC
         >>> tsetmc = TSETMC()
         >>> tsetmc.mw(["stock", "etf", "options"])
         """
         r = self.requests(self.url.mw(sections), response="json")[0].get("marketwatch")
+        r_client_type = self.requests(self.url.client_type_all())[0]["clientTypeAllDto"]
         records = json_normalize(
             data=[MarketWatch.model_validate(i).model_dump() for i in r],
             record_path="order_book",
         )
-        return pl.DataFrame(records)
+        df = pl.DataFrame(records)
+        df_ct = pl.from_dicts([ClientTypeAll(**i).model_dump() for i in r_client_type])
+        df = df.join(df_ct, on=["ins_code"], how="left")
+        return df
 
     def tse_options_mw(self):
         """
         .. raw:: html
 
             <div dir="rtl">
                 داده‌های نمایِ بازارِ اختیارِ-معامله‌یِ بورسِ تهران رو بهت می‌ده
@@ -827,15 +834,16 @@
         """
         ins_code = symbol if symbol else ins_code
         if isinstance(ins_code, str):
             ins_code = [ins_code]
 
         df = self.hist_price(ins_code=ins_code)
         df = (
-            df.with_columns(
+            df.sort("date")
+            .with_columns(
                 factor=(pl.col("y_final").shift(-1) / pl.col("final"))
                 .fill_null(1)
                 .reverse()
                 .cumprod()
                 .reverse()
                 .over("ins_code")
             )
```

## Comparing `oxtapus-0.3.0.dist-info/LICENSE.txt` & `oxtapus-0.3.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `oxtapus-0.3.0.dist-info/METADATA` & `oxtapus-0.3.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxtapus
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Home-page: https://github.com/yghaderi/oxtapus
 Author: Yaghoub Ghadri
 Author-email: y.ghaderi@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: oxtapus Version: 0.3.0 Summary: Home-page: https://
+Metadata-Version: 2.1 Name: oxtapus Version: 0.3.1 Summary: Home-page: https://
 github.com/yghaderi/oxtapus Author: Yaghoub Ghadri Author-email:
 y.ghaderi@outlook.com Requires-Python: >=3.10,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: httpx (>=0.25.0,<0.26.0) Requires-
 Dist: polars (>=0.20.3,<0.21.0) Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: tarix (>=0.1.1,<0.2.0) Requires-Dist: tenacity (>=8.2.3,<9.0.0)
```

## Comparing `oxtapus-0.3.0.dist-info/RECORD` & `oxtapus-0.3.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 oxtapus/.DS_Store,sha256=0rDOK8ZfHcSrcVGAzbYz4wStqJsCIq6ategrLYGyzp0,6148
 oxtapus/__init__.py,sha256=savGpOWlYPsqBhLAEXxOPKd1_sepJIF71yGDQHthrrU,102
 oxtapus/codal.py,sha256=iWVcQxJVAabma40UWSJVp-lfONrGOARnzPzODbdW6Qo,2746
 oxtapus/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 oxtapus/models/rahavard.py,sha256=pqD5p5EKDboB022qFCh_MTSGRHV7mzuU_yowo-e5y2k,2122
-oxtapus/models/tsetmc.py,sha256=-VFM6MJSU-NdO7pD_0TA_lSkYRMCwovju-6_m7JkPKA,2230
+oxtapus/models/tsetmc.py,sha256=1YokgDyML5TZX5fVxdhNBDqHWj5Ib9zLfriETnjidb4,2731
 oxtapus/rahavard.py,sha256=C5ra8ZpVspqKkYLuO3zKq7827z6dSo9t_ayKrIESXAQ,25365
 oxtapus/tgju.py,sha256=jIseeQuldq1FdHp9BIlau0KQimVvu_oydLuOfO5wakU,6082
-oxtapus/tsetmc.py,sha256=iWHC4y-6dIa61RXu8x8M7KHim0eQRO_VFE6ONyFF1pM,83546
+oxtapus/tsetmc.py,sha256=L1Cse_AfZoD_jpx3wxwEIVemJH0qo0RUYl7rSs9-Z6w,83931
 oxtapus/utils/__init__.py,sha256=8R6IZMUVZHW9E-ka0u-nyVq6lQsHMk7kv6qjkloUZIo,165
 oxtapus/utils/codal/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 oxtapus/utils/codal/clean_data.py,sha256=UR7jX36zzbX0qgekHnnzQ9tcZJRbIlehm24NjAk1NzQ,10916
 oxtapus/utils/codal/items.py,sha256=71sV_8bkpp1CdiiXnzfK_R74vng7l_oQWpj_z6liy9s,6854
 oxtapus/utils/codal/models.py,sha256=uLm7nlhKIlrbs06_jFl0oyTtA-JUMBdYJm0ZkQPaOrs,4882
 oxtapus/utils/codal/request.py,sha256=i5P-0UEces2sy_VHypap8TqcNEgV9FXEOp4OIY1JwQs,1036
 oxtapus/utils/codal/utils.py,sha256=FLcEbzFBMybCK5Xmmb_HrNETDM2cH_bwC5zegx97oBY,1042
 oxtapus/utils/columns.py,sha256=ZZNfyzYMCGCHYk5hb5fPFLCLU_egpVgtZQBtA2_mMpg,5767
 oxtapus/utils/http/__init__.py,sha256=447GDWyNp9xpyt7tERfZfZtS-jH34wOdFJITVmwXVkE,47
 oxtapus/utils/http/requests.py,sha256=_foEzr-vqdlyng0FdiIJjMN4AjJGiz2kTYP0RFLjnyM,2156
 oxtapus/utils/models.py,sha256=Y8WOP--2d9dbtCOnL125zHVXSuki_F3QZ5e630Mtu6k,2926
 oxtapus/utils/normalize.py,sha256=aCTA3bGdxx4_8Lm_Qc7dpVaue-L8ANTzr_LL5xaCX_Y,825
-oxtapus-0.3.0.dist-info/LICENSE.txt,sha256=rk-2xVGc7h8PusLyqRcXBBh3TiYtJXA-EE_YXpDfyC0,1071
-oxtapus-0.3.0.dist-info/METADATA,sha256=TMS2R3tP5OYzPZzWfUnvibFkhZNp2n2dmyLbrQizRF4,19557
-oxtapus-0.3.0.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
-oxtapus-0.3.0.dist-info/RECORD,,
+oxtapus-0.3.1.dist-info/LICENSE.txt,sha256=rk-2xVGc7h8PusLyqRcXBBh3TiYtJXA-EE_YXpDfyC0,1071
+oxtapus-0.3.1.dist-info/METADATA,sha256=Uz80Sw_gY32QA4MrqV3k-KAZXGqcAioGP6_ugQGAi2Q,19557
+oxtapus-0.3.1.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
+oxtapus-0.3.1.dist-info/RECORD,,
```

