# Comparing `tmp/teelebot-2.5.0-py3-none-any.whl.zip` & `tmp/teelebot-2.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 43082 bytes, number of entries: 20
+Zip file size: 43078 bytes, number of entries: 20
 -rw-rw-rw-  2.0 fat     4279 b- defN 23-Dec-26 02:00 teelebot/__init__.py
 -rw-rw-rw-  2.0 fat      165 b- defN 23-May-08 17:02 teelebot/__main__.py
 -rw-rw-rw-  2.0 fat    39084 b- defN 24-Feb-29 03:17 teelebot/bot.py
--rw-rw-rw-  2.0 fat    20701 b- defN 24-Mar-04 05:23 teelebot/buffer.py
+-rw-rw-rw-  2.0 fat    20714 b- defN 24-Apr-14 01:23 teelebot/buffer.py
 -rw-rw-rw-  2.0 fat     1771 b- defN 24-Feb-29 02:04 teelebot/common.py
 -rw-rw-rw-  2.0 fat    25637 b- defN 24-Feb-28 03:52 teelebot/handler.py
 -rw-rw-rw-  2.0 fat     1869 b- defN 23-Dec-25 01:59 teelebot/logger.py
 -rw-rw-rw-  2.0 fat     7236 b- defN 24-Feb-29 01:47 teelebot/metadata.py
 -rw-rw-rw-  2.0 fat      898 b- defN 23-Dec-26 02:32 teelebot/polling.py
 -rw-rw-rw-  2.0 fat     3997 b- defN 24-Feb-28 01:38 teelebot/request.py
 -rw-rw-rw-  2.0 fat     4308 b- defN 24-Feb-28 03:22 teelebot/schedule.py
--rw-rw-rw-  2.0 fat      483 b- defN 24-Mar-04 05:05 teelebot/version.py
+-rw-rw-rw-  2.0 fat      483 b- defN 24-Apr-14 01:33 teelebot/version.py
 -rw-rw-rw-  2.0 fat     2796 b- defN 23-Dec-11 02:32 teelebot/webhook.py
--rw-rw-rw-  2.0 fat    35823 b- defN 24-Mar-04 06:06 teelebot-2.5.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     9964 b- defN 24-Mar-04 06:06 teelebot-2.5.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-04 06:06 teelebot-2.5.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       43 b- defN 24-Mar-04 06:06 teelebot-2.5.0.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 24-Mar-04 06:06 teelebot-2.5.0.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat        2 b- defN 24-Mar-04 06:06 teelebot-2.5.0.dist-info/zip-safe
--rw-rw-r--  2.0 fat     1559 b- defN 24-Mar-04 06:06 teelebot-2.5.0.dist-info/RECORD
-20 files, 160716 bytes uncompressed, 40576 bytes compressed:  74.8%
+-rw-rw-rw-  2.0 fat    35823 b- defN 24-Apr-14 01:49 teelebot-2.5.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     9964 b- defN 24-Apr-14 01:49 teelebot-2.5.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-14 01:49 teelebot-2.5.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       43 b- defN 24-Apr-14 01:49 teelebot-2.5.1.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-14 01:49 teelebot-2.5.1.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 24-Apr-14 01:49 teelebot-2.5.1.dist-info/zip-safe
+-rw-rw-r--  2.0 fat     1559 b- defN 24-Apr-14 01:49 teelebot-2.5.1.dist-info/RECORD
+20 files, 160729 bytes uncompressed, 40572 bytes compressed:  74.8%
```

## zipnote {}

```diff
@@ -33,29 +33,29 @@
 
 Filename: teelebot/version.py
 Comment: 
 
 Filename: teelebot/webhook.py
 Comment: 
 
-Filename: teelebot-2.5.0.dist-info/LICENSE
+Filename: teelebot-2.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: teelebot-2.5.0.dist-info/METADATA
+Filename: teelebot-2.5.1.dist-info/METADATA
 Comment: 
 
-Filename: teelebot-2.5.0.dist-info/WHEEL
+Filename: teelebot-2.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: teelebot-2.5.0.dist-info/entry_points.txt
+Filename: teelebot-2.5.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: teelebot-2.5.0.dist-info/top_level.txt
+Filename: teelebot-2.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: teelebot-2.5.0.dist-info/zip-safe
+Filename: teelebot-2.5.1.dist-info/zip-safe
 Comment: 
 
-Filename: teelebot-2.5.0.dist-info/RECORD
+Filename: teelebot-2.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## teelebot/buffer.py

```diff
@@ -1,10 +1,10 @@
 '''
 @creation date: 2021-04-25
-@last modification: 2024-03-04
+@last modification: 2024-04-14
 '''
 from __future__ import print_function
 from sys import getsizeof, stderr
 from itertools import chain
 from collections import deque
 from pathlib import Path
 from typing import Tuple, Union
@@ -263,15 +263,15 @@
                                 if key in list(log.keys()) and log[key] == value:
                                     conditions_ok_count += 1
                             if conditions_ok_count == len(conditions):
                                     selected_logs_idx.append(id_x)
 
                     for id_x in selected_logs_idx:
                         changed_size += self.__total_size(self.__buffer[plugin_name][buffer_name][id_x])
-                        self.__buffer[plugin_name].pop(id_x)
+                        self.__buffer[plugin_name][buffer_name].pop(id_x)
                     
                 return True, str(changed_size)
             except Exception as e:
                 _logger.error(e)
                 traceback.print_exc()
                 return False, str(e)
         else:
```

## teelebot/version.py

```diff
@@ -1,16 +1,16 @@
 # -*- coding:utf-8 -*-
 """
 @description: A Python-based Telegram Bot framework
 @creation date: 2019-11-15
-@last modification: 2024-03-04
+@last modification: 2024-04-14
 @author: Pluto (github:plutobell)
 """
 
-__version__ = "2.5.0"
+__version__ = "2.5.1"
 
 __author__ = "Pluto"
 __email__ = "hi@ojoll.com"
 __blog__ = "https://ojoll.com"
 __github__ = "https://github.com/plutobell/teelebot"
 __description__ = "teelebot is a Python-based Telegram Bot framework with a plugin system that supports hot reload and hot loading."
```

## Comparing `teelebot-2.5.0.dist-info/LICENSE` & `teelebot-2.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `teelebot-2.5.0.dist-info/METADATA` & `teelebot-2.5.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teelebot
-Version: 2.5.0
+Version: 2.5.1
 Summary: teelebot is a Python-based Telegram Bot framework with a plugin system that supports hot reload and hot loading.
 Home-page: https://ojoll.com
 Author: Pluto
 Author-email: hi@ojoll.com
 License: GPLv3
 Keywords: teelebot telegram bot telegram bot api telegram
 Classifier: Programming Language :: Python :: 3
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: teelebot Version: 2.5.0 Summary: teelebot is a
+Metadata-Version: 2.1 Name: teelebot Version: 2.5.1 Summary: teelebot is a
 Python-based Telegram Bot framework with a plugin system that supports hot
 reload and hot loading. Home-page: https://ojoll.com Author: Pluto Author-
 email: hi@ojoll.com License: GPLv3 Keywords: teelebot telegram bot telegram bot
 api telegram Classifier: Programming Language :: Python :: 3 Classifier:
 Operating System :: OS Independent Classifier: License :: OSI Approved :: GNU
 General Public License v3 (GPLv3) Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: requests
```

## Comparing `teelebot-2.5.0.dist-info/RECORD` & `teelebot-2.5.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 teelebot/__init__.py,sha256=kAq6jlmvcxByifHdMlapLN-el_IL9h6pIkggxzvnn8c,4279
 teelebot/__main__.py,sha256=_j6f3hj0VtlcCsabcIvuS0uBI0NVbCVwmH138tqYGFo,165
 teelebot/bot.py,sha256=ZNFL1aGwRVz2PVtQXJ0EjIJP6h5nucvR4si2e3sr49U,39084
-teelebot/buffer.py,sha256=YOfZ3ukM0iLjHi2uggZnJLjMu39icdOmWnrj11c22L8,20701
+teelebot/buffer.py,sha256=payjL7pxJRn1rszs5IFq7DHEpB261dny0fO16Ko86pE,20714
 teelebot/common.py,sha256=ltYHihcrxrYVtjvBLQ8rXjEpO-4pfqJ6w_oqrTXK1ys,1771
 teelebot/handler.py,sha256=jxrMraJz5lh5bZJ5jKZsBjMgSMfeEfV8Krc5quYdghQ,25637
 teelebot/logger.py,sha256=I7UJxLdxRz5HxzwEgBPf_gILZuDlPCLwZPxioIahS2A,1869
 teelebot/metadata.py,sha256=e1UR2Nz2eP9hoLByb_j-4byPd6vpNk1SIN52o04PmYM,7236
 teelebot/polling.py,sha256=p_JO9TOgyTifTbZEcGpPRYAHp4MyoFkJ3wY0-D7yC4Q,898
 teelebot/request.py,sha256=HenftV-3frTxNks1HjMVQCCYo8SeDA2Jhhe8T1xpjD4,3997
 teelebot/schedule.py,sha256=0jwTwu2iewO0y9nWW86uxKTGeP42FfSFyKIxjW25Znc,4308
-teelebot/version.py,sha256=3TzS6HOmXFiukMrL4BSkWXhkf9oEMhOMdUIyZ2fb1Bs,483
+teelebot/version.py,sha256=hCsg57E8rdw2vAgHxV7TgsBa13HkGKhrw8Y160y9SLo,483
 teelebot/webhook.py,sha256=5cd9GPAv4_LHTxDZC9s0NsKKq5eZGx_3L1i6Bl4lbig,2796
-teelebot-2.5.0.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
-teelebot-2.5.0.dist-info/METADATA,sha256=-K6X-OZCLi1Pb85Bdzbqiwdc7A7X4EPXIanms-5kpAU,9964
-teelebot-2.5.0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-teelebot-2.5.0.dist-info/entry_points.txt,sha256=IZHSiwFVJ6BPPTW3j7I1i34AESCOPaTYiC1qoWfpj6k,43
-teelebot-2.5.0.dist-info/top_level.txt,sha256=vMgTMVZJd4P3KjMwVpgWfIUvNLYKqfyHO4Cul-YwuyQ,9
-teelebot-2.5.0.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-teelebot-2.5.0.dist-info/RECORD,,
+teelebot-2.5.1.dist-info/LICENSE,sha256=IwGE9guuL-ryRPEKi6wFPI_zOhg7zDZbTYuHbSt_SAk,35823
+teelebot-2.5.1.dist-info/METADATA,sha256=ilgfCjAdaMdmoJ-JaN9SrUH2K3DK4MtCfKURfQ6exXY,9964
+teelebot-2.5.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+teelebot-2.5.1.dist-info/entry_points.txt,sha256=IZHSiwFVJ6BPPTW3j7I1i34AESCOPaTYiC1qoWfpj6k,43
+teelebot-2.5.1.dist-info/top_level.txt,sha256=vMgTMVZJd4P3KjMwVpgWfIUvNLYKqfyHO4Cul-YwuyQ,9
+teelebot-2.5.1.dist-info/zip-safe,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+teelebot-2.5.1.dist-info/RECORD,,
```

