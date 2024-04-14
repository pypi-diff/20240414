# Comparing `tmp/EdgeGPT-fork-0.14.1.tar.gz` & `tmp/edgegpt_fork-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EdgeGPT-fork-0.14.1.tar", last modified: Thu Dec 21 08:58:59 2023, max compression
+gzip compressed data, was "edgegpt_fork-1.0.0.tar", last modified: Sun Apr 14 13:51:53 2024, max compression
```

## Comparing `EdgeGPT-fork-0.14.1.tar` & `edgegpt_fork-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 08:58:59.630556 EdgeGPT-fork-0.14.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-12-21 08:58:36.000000 EdgeGPT-fork-0.14.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12539 2023-12-21 08:58:59.630556 EdgeGPT-fork-0.14.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11545 2023-12-21 08:58:36.000000 EdgeGPT-fork-0.14.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-21 08:58:59.630556 EdgeGPT-fork-0.14.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2023-12-21 08:58:36.000000 EdgeGPT-fork-0.14.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 08:58:59.626556 EdgeGPT-fork-0.14.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 08:58:59.630556 EdgeGPT-fork-0.14.1/src/EdgeGPT/
--rw-r--r--   0 runner    (1001) docker     (127)     7976 2023-12-21 08:58:36.000000 EdgeGPT-fork-0.14.1/src/EdgeGPT/EdgeGPT.py
--rw-r--r--   0 runner    (1001) docker     (127)    14262 2023-12-21 08:58:36.000000 EdgeGPT-fork-0.14.1/src/EdgeGPT/EdgeUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2023-12-21 08:58:36.000000 EdgeGPT-fork-0.14.1/src/EdgeGPT/ImageGen.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-21 08:58:36.000000 EdgeGPT-fork-0.14.1/src/EdgeGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11006 2023-12-21 08:58:36.000000 EdgeGPT-fork-0.14.1/src/EdgeGPT/chathub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2023-12-21 08:58:36.000000 EdgeGPT-fork-0.14.1/src/EdgeGPT/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4644 2023-12-21 08:58:36.000000 EdgeGPT-fork-0.14.1/src/EdgeGPT/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2023-12-21 08:58:36.000000 EdgeGPT-fork-0.14.1/src/EdgeGPT/conversation_style.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-21 08:58:36.000000 EdgeGPT-fork-0.14.1/src/EdgeGPT/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2023-12-21 08:58:36.000000 EdgeGPT-fork-0.14.1/src/EdgeGPT/locale.py
--rw-r--r--   0 runner    (1001) docker     (127)     7500 2023-12-21 08:58:36.000000 EdgeGPT-fork-0.14.1/src/EdgeGPT/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6068 2023-12-21 08:58:36.000000 EdgeGPT-fork-0.14.1/src/EdgeGPT/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2023-12-21 08:58:36.000000 EdgeGPT-fork-0.14.1/src/EdgeGPT/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-21 08:58:59.630556 EdgeGPT-fork-0.14.1/src/EdgeGPT_fork.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12539 2023-12-21 08:58:59.000000 EdgeGPT-fork-0.14.1/src/EdgeGPT_fork.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      600 2023-12-21 08:58:59.000000 EdgeGPT-fork-0.14.1/src/EdgeGPT_fork.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-21 08:58:59.000000 EdgeGPT-fork-0.14.1/src/EdgeGPT_fork.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-12-21 08:58:59.000000 EdgeGPT-fork-0.14.1/src/EdgeGPT_fork.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-12-21 08:58:59.000000 EdgeGPT-fork-0.14.1/src/EdgeGPT_fork.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-21 08:58:59.000000 EdgeGPT-fork-0.14.1/src/EdgeGPT_fork.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:51:53.310997 edgegpt_fork-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12568 2024-04-14 13:51:53.310997 edgegpt_fork-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11545 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-14 13:51:53.310997 edgegpt_fork-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:51:53.306996 edgegpt_fork-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:51:53.310997 edgegpt_fork-1.0.0/src/EdgeGPT/
+-rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/EdgeGPT.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/EdgeUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/ImageGen.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11415 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/chathub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/conversation_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4407 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7500 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7047 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-04-14 13:51:32.000000 edgegpt_fork-1.0.0/src/EdgeGPT/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 13:51:53.310997 edgegpt_fork-1.0.0/src/EdgeGPT_fork.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12568 2024-04-14 13:51:53.000000 edgegpt_fork-1.0.0/src/EdgeGPT_fork.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-14 13:51:53.000000 edgegpt_fork-1.0.0/src/EdgeGPT_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 13:51:53.000000 edgegpt_fork-1.0.0/src/EdgeGPT_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-14 13:51:53.000000 edgegpt_fork-1.0.0/src/EdgeGPT_fork.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-14 13:51:53.000000 edgegpt_fork-1.0.0/src/EdgeGPT_fork.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-14 13:51:53.000000 edgegpt_fork-1.0.0/src/EdgeGPT_fork.egg-info/top_level.txt
```

### Comparing `EdgeGPT-fork-0.14.1/LICENSE` & `edgegpt_fork-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `EdgeGPT-fork-0.14.1/PKG-INFO` & `edgegpt_fork-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT-fork
-Version: 0.14.1
+Version: 1.0.0
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/xingty/EdgeGPT
 Author: Antonio Cheong,Bigbyto
 Author-email: acheong@student.dalat.org,bigbyto@gmail.com
 License: The Unlicense
 Project-URL: Bug Report, https://github.com/xingty/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -19,15 +19,16 @@
 Requires-Dist: httpx[socks]>=0.24.0
 Requires-Dist: aiohttp
 Requires-Dist: websockets
 Requires-Dist: rich
 Requires-Dist: certifi
 Requires-Dist: prompt_toolkit
 Requires-Dist: requests
-Requires-Dist: BingImageCreator>=0.4.4
+Requires-Dist: BingImageCreator-fork>=0.7.6
+Requires-Dist: curl_cffi
 
 <div align="center">
   <img src="https://socialify.git.ci/acheong08/EdgeGPT/image?font=Inter&language=1&logo=https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2F9%2F9c%2FBing_Fluent_Logo.svg&owner=1&pattern=Floating%20Cogs&theme=Auto" alt="EdgeGPT" width="640" height="320" />
 
 # Edge GPT
 
 _The reverse engineering the chat feature of the new version of Bing_
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: EdgeGPT-fork Version: 0.14.1 Summary: Reverse
+Metadata-Version: 2.1 Name: EdgeGPT-fork Version: 1.0.0 Summary: Reverse
 engineered Edge Chat API Home-page: https://github.com/xingty/EdgeGPT Author:
 Antonio Cheong,Bigbyto Author-email:
 acheong@student.dalat.org,bigbyto@gmail.com License: The Unlicense Project-URL:
 Bug Report, https://github.com/xingty/EdgeGPT/issues/new Classifier: License ::
 OSI Approved :: The Unlicense (Unlicense) Classifier: Intended Audience ::
 Developers Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: httpx
 [socks]>=0.24.0 Requires-Dist: aiohttp Requires-Dist: websockets Requires-Dist:
 rich Requires-Dist: certifi Requires-Dist: prompt_toolkit Requires-Dist:
-requests Requires-Dist: BingImageCreator>=0.4.4
+requests Requires-Dist: BingImageCreator-fork>=0.7.6 Requires-Dist: curl_cffi
    [EdgeGPT]# Edge GPT _The reverse engineering the chat feature of the new
  version of Bing_ English - _ç_®__ä_½__ä_¸_­_æ__ - _ç_¹__é_«__ä_¸_­_æ__ - _E_s_p_a_Ã_±_o_l - _æ__¥_æ__¬_è_ª_
                 _[_P_y_P_I_ _v_e_r_s_i_o_n_][Python version][Total downloads]
 # Setup ## Install package ```bash python3 -m pip install EdgeGPT-fork --
 upgrade ``` ## Requirements - python 3.8+ - A Microsoft Account with access to
 bing.com/chat> (Optional, depending on your region) - Required in a supported
 country or region with New Bing (Chinese mainland VPN required) - [Selenium]
```

### Comparing `EdgeGPT-fork-0.14.1/README.md` & `edgegpt_fork-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `EdgeGPT-fork-0.14.1/setup.py` & `edgegpt_fork-1.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with Path.open(DOCS_PATH, encoding="utf-8") as f1:
         with Path.open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="EdgeGPT-fork",
-    version="0.14.1",
+    version="1.0.0",
     license="The Unlicense",
     author="Antonio Cheong,Bigbyto",
     author_email="acheong@student.dalat.org,bigbyto@gmail.com",
     description="Reverse engineered Edge Chat API",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://github.com/xingty/EdgeGPT",
@@ -31,15 +31,16 @@
         "httpx[socks]>=0.24.0",
         "aiohttp",
         "websockets",
         "rich",
         "certifi",
         "prompt_toolkit",
         "requests",
-        "BingImageCreator>=0.4.4",
+        "BingImageCreator-fork>=0.7.6",
+        "curl_cffi"
     ],
     long_description=Path.open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     py_modules=["EdgeGPT", "EdgeUtils", "ImageGen"],
     classifiers=[
         "License :: OSI Approved :: The Unlicense (Unlicense)",
         "Intended Audience :: Developers",
```

### Comparing `EdgeGPT-fork-0.14.1/src/EdgeGPT/EdgeGPT.py` & `edgegpt_fork-1.0.0/src/EdgeGPT/EdgeGPT.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 """
 Main.py
 """
 from __future__ import annotations
 
-import json
-from typing import Generator
-
 from .chathub import *
 from .conversation import *
-from .conversation_style import *
 from .request import *
 from .utilities import *
 
 
 class Chatbot:
     """
     Combines everything to make it seamless
@@ -96,14 +92,16 @@
         conversation_style: CONVERSATION_STYLE_TYPE = None,
         webpage_context: str | None = None,
         search_result: bool = False,
         locale: str = guess_locale(),
         simplify_response: bool = False,
         mode: str = None,
         no_search: bool = True,
+        persona: Persona = Persona.copilot,
+        plugins: set[Plugin] = {}
     ) -> dict:
         """
         Ask a question to the bot
         Response:
             {
                 item (dict):
                     messages (list[dict]):
@@ -115,18 +113,18 @@
             response["item"]["messages"][1]["adaptiveCards"][0]["body"][0]["text"]
         """
         async for final, response in self.chat_hub.ask_stream(
             prompt=prompt,
             conversation_style=conversation_style,
             wss_link=wss_link,
             webpage_context=webpage_context,
-            search_result=search_result,
             locale=locale,
-            mode=mode,
             no_search=no_search,
+            persona=persona,
+            plugins=plugins
         ):
             if final:
                 if not simplify_response:
                     return response
                 messages_left = response["item"]["throttling"][
                     "maxNumUserMessagesInConversation"
                 ] - response["item"]["throttling"].get(
@@ -156,53 +154,58 @@
                     adaptive_cards[0]["body"][0].get("text") if adaptive_cards else None
                 )
                 sources_text = (
                     adaptive_cards[0]["body"][-1].get("text")
                     if adaptive_cards
                     else None
                 )
+                media = response.get("media") or {}
+
                 return {
                     "text": message["text"],
                     "author": message["author"],
                     "sources": sources,
                     "sources_text": sources_text,
                     "suggestions": suggestions,
                     "messages_left": messages_left,
                     "max_messages": response["item"]["throttling"][
                         "maxNumUserMessagesInConversation"
                     ],
                     "adaptive_text": adaptive_text,
+                    "media": media
                 }
         return {}
 
     async def ask_stream(
         self,
         prompt: str,
         wss_link: str = "wss://sydney.bing.com/sydney/ChatHub",
         conversation_style: CONVERSATION_STYLE_TYPE = None,
         raw: bool = False,
         webpage_context: str | None = None,
         search_result: bool = False,
         locale: str = guess_locale(),
         mode: str = None,
         no_search: bool = True,
+        persona: Persona = Persona.copilot,
+        plugins: set[Plugin] = {}
     ) -> Generator[bool, dict | str, None]:
         """
         Ask a question to the bot
         """
         async for response in self.chat_hub.ask_stream(
             prompt=prompt,
             conversation_style=conversation_style,
             wss_link=wss_link,
             raw=raw,
             webpage_context=webpage_context,
-            search_result=search_result,
             locale=locale,
-            mode=mode,
             no_search=no_search,
+            persona=persona,
+            plugins=plugins
         ):
             yield response
 
     async def close(self) -> None:
         """
         Close the connection
         """
@@ -223,18 +226,19 @@
             client_id=client_id,
         )
 
     async def reset(self, delete=False) -> None:
         """
         Reset the conversation
         """
-        if delete:
-            await self.remove_and_close()
-        else:
-            await self.close()
+        # if delete:
+        #     await self.remove_and_close()
+        # else:
+        #     await self.close()
+        await self.close()
         self.chat_hub = ChatHub(
             await Conversation.create(self.proxy, cookies=self.chat_hub.cookies),
             proxy=self.proxy,
             cookies=self.chat_hub.cookies,
         )
```

### Comparing `EdgeGPT-fork-0.14.1/src/EdgeGPT/EdgeUtils.py` & `edgegpt_fork-1.0.0/src/EdgeGPT/EdgeUtils.py`

 * *Files identical despite different names*

### Comparing `EdgeGPT-fork-0.14.1/src/EdgeGPT/chathub.py` & `edgegpt_fork-1.0.0/src/EdgeGPT/chathub.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,39 @@
 import asyncio
 import json
 import os
-import ssl
-import sys
 from time import time
-from tkinter import NO
-from typing import Generator
-from typing import List
-from typing import Union
-
-import aiohttp
-import certifi
-import httpx
+from typing import Generator, List, Union, Optional, Tuple
+
+from curl_cffi import requests
+from curl_cffi.requests.websockets import WebSocket
+from curl_cffi.const import CurlWsFlag
+from curl_cffi import AsyncCurl
 import urllib
 from BingImageCreator import ImageGenAsync
 
-from .constants import DELIMITER
+from .constants import DELIMITER, PERSONATE
 from .constants import HEADERS
 from .constants import HEADERS_INIT_CONVER
 from .conversation import Conversation
-from .conversation_style import CONVERSATION_STYLE_TYPE
+from .conversation_style import CONVERSATION_STYLE_TYPE, Persona
+from .plugin import Plugin
 from .request import ChatHubRequest
 from .utilities import append_identifier
 from .utilities import get_ran_hex
 from .utilities import guess_locale
-
-ssl_context = ssl.create_default_context()
-ssl_context.load_verify_locations(certifi.where())
+from .utilities import parse_search_result
 
 
 class ChatHub:
     def __init__(
-        self,
-        conversation: Conversation,
-        proxy: str = None,
-        cookies: Union[List[dict], None] = None,
+            self,
+            conversation: Conversation,
+            proxy: str = None,
+            cookies: Union[List[dict], None] = None,
     ) -> None:
         conversationSignature = conversation.struct.get("conversationSignature") or None
         self.aio_session = None
         self.request: ChatHubRequest
         self.loop: bool
         self.task: asyncio.Task
         self.request = ChatHubRequest(
@@ -46,38 +41,39 @@
             client_id=conversation.struct["clientId"],
             conversation_id=conversation.struct["conversationId"],
         )
         self.sec_access_token = conversation.struct["secAccessToken"] or None
         self.cookies = cookies
         self.proxy: str = proxy
         proxy = (
-            proxy
-            or os.environ.get("all_proxy")
-            or os.environ.get("ALL_PROXY")
-            or os.environ.get("https_proxy")
-            or os.environ.get("HTTPS_PROXY")
-            or None
+                proxy
+                or os.environ.get("all_proxy")
+                or os.environ.get("ALL_PROXY")
+                or os.environ.get("https_proxy")
+                or os.environ.get("HTTPS_PROXY")
+                or None
         )
         if proxy is not None and proxy.startswith("socks5h://"):
-            proxy = "socks5://" + proxy[len("socks5h://") :]
-        self.session = httpx.AsyncClient(
-            proxies=proxy,
+            proxy = "socks5://" + proxy[len("socks5h://"):]
+        self.session = AsyncSession(
+            proxy=proxy,
             timeout=900,
             headers=HEADERS_INIT_CONVER,
+            impersonate=PERSONATE
         )
 
     async def get_conversation(
-        self,
-        conversation_id: str = None,
-        conversation_signature: str = None,
-        client_id: str = None,
+            self,
+            conversation_id: str = None,
+            conversation_signature: str = None,
+            client_id: str = None,
     ) -> dict:
         conversation_id = conversation_id or self.request.conversation_id
         conversation_signature = (
-            conversation_signature or self.request.conversation_signature
+                conversation_signature or self.request.conversation_signature
         )
         client_id = client_id or self.request.client_id
         url = f"https://sydney.bing.com/sydney/GetConversation?conversationId={conversation_id}&source=cib&participantId={client_id}&conversationSignature={conversation_signature}&traceId={get_ran_hex()}"
         response = await self.session.get(url)
         return response.json()
 
     async def get_activity(self) -> dict:
@@ -88,177 +84,191 @@
                 if cookie["name"] == "_U":
                     headers["Cookie"] = f"SUID=A; _U={cookie['value']};"
                     break
         response = await self.session.get(url, headers=headers)
         return response.json()
 
     async def ask_stream(
-        self,
-        prompt: str,
-        wss_link: str = None,
-        conversation_style: CONVERSATION_STYLE_TYPE = None,
-        raw: bool = False,
-        webpage_context: Union[str, None] = None,
-        search_result: bool = False,
-        locale: str = guess_locale(),
-        mode: str = None,
-        no_search: bool = True,
+            self,
+            prompt: str,
+            wss_link: str = None,
+            conversation_style: CONVERSATION_STYLE_TYPE = None,
+            raw: bool = False,
+            webpage_context: Union[str, None] = None,
+            locale: str = guess_locale(),
+            no_search: bool = True,
+            persona: Persona = Persona.copilot,
+            plugins: set[Plugin] = {}
     ) -> Generator[bool, Union[dict, str], None]:
         """ """
         cookies = {}
         if self.cookies is not None:
             for cookie in self.cookies:
                 cookies[cookie["name"]] = cookie["value"]
-        self.aio_session = aiohttp.ClientSession(cookies=cookies)
-        token = urllib.parse.quote_plus(self.sec_access_token) if self.sec_access_token else ''
-        wss_link = f'{wss_link}?sec_access_token={token}'
-        # Check if websocket is closed
-        wss = await self.aio_session.ws_connect(
-            wss_link or "wss://sydney.bing.com/sydney/ChatHub",
-            ssl=ssl_context,
+        # self.aio_session = aiohttp.ClientSession(cookies=cookies)
+        self.aio_session = AsyncSession(
+            cookies=cookies,
             headers=HEADERS,
             proxy=self.proxy,
+            impersonate=PERSONATE
         )
+        token = urllib.parse.quote_plus(self.sec_access_token) if self.sec_access_token else ''
+        wss_link = f'{wss_link}?sec_access_token={token}'
+        # Check if websocket is closed
+        wss = await self.aio_session.ws_connect(wss_link or "wss://sydney.bing.com/sydney/ChatHub")
         await self._initial_handshake(wss)
         # Construct a ChatHub request
         self.request.update(
             prompt=prompt,
             conversation_style=conversation_style,
             webpage_context=webpage_context,
-            search_result=search_result,
             locale=locale,
-            mode=mode,
-            no_search=no_search
+            no_search=no_search,
+            persona=persona,
+            plugins=plugins
         )
         # Send request
-        await wss.send_str(append_identifier(self.request.struct))
-        draw = False
+        await wss.asend(append_identifier(self.request.struct).encode("utf-8"))
         resp_txt = ""
-        result_text = ""
-        resp_txt_no_link = ""
-        retry_count = 5
-        while not wss.closed:
-            msg = await wss.receive_str()
-            if not msg:
-                retry_count -= 1
-                if retry_count == 0:
-                    raise Exception("No response from server")
-                continue
-            if isinstance(msg, str):
-                objects = msg.split(DELIMITER)
-            else:
+        generate = None
+        new_line = "\n"
+        search_hint = "Searching the web for:\n"
+        search_refs = []
+        images = []
+        search_keywords = ""
+        offset = 0
+        async for obj in self._receive_messages(wss):
+            if int(time()) % 6 == 0:
+                await wss.asend(append_identifier({"type": 6}).encode("utf-8"))
+
+            if obj is None or not obj:
                 continue
-            for obj in objects:
-                if int(time()) % 6 == 0:
-                    await wss.send_str(append_identifier({"type": 6}))
-                if obj is None or not obj:
+
+            response = json.loads(obj)
+            r_type = response.get("type")
+            if r_type in [6, 7]:
+                await wss.asend(append_identifier({"type": r_type}).encode("utf-8"))
+
+            if raw:
+                done = r_type == 2
+                yield done, response
+                if not done:
                     continue
-                response = json.loads(obj)
-                # print(response)
-                if response.get("type") == 1 and response["arguments"][0].get(
+                else:
+                    return
+
+            if r_type == 1 and response["arguments"][0].get(
                     "messages",
-                ):
-                    if not draw:
-                        msg_type = response["arguments"][0]["messages"][0].get("messageType")
-                        if (msg_type == "GenerateContentQuery"
-):
+            ):
+                message = response["arguments"][0]["messages"][0]
+                msg_type = message.get("messageType")
+                hidden_text = message.get("hiddenText")
+                text = message.get("text")
+                if msg_type == "InternalSearchQuery":
+                    search_keywords = f"{search_keywords}\n{search_hint}{hidden_text}\n"
+                    resp_txt = search_keywords
+                elif msg_type == "InternalSearchResult":
+                    search_refs += parse_search_result(message)
+                elif msg_type == "GenerateContentQuery":
+                    generate = {
+                        "content_type": message.get("contentType"),
+                        "prompt": text
+                    }
+                elif msg_type is None:
+                    if message.get("contentOrigin") == "Apology":
+                        print('message has been revoked')
+                        print(message)
+                        result = f"{message.get('text')} -end- (message has been revoked)"
+                        resp_txt = f"{resp_txt}\n{result}"
+
+                    text = new_line + text
+                    resp_txt = f"{resp_txt}{text[offset:]}"
+                    offset = len(text)
+                    new_line = ""
+
+                yield False, resp_txt
+            elif response.get("type") == 2:
+                if response["item"]["result"].get("error"):
+                    raise Exception(
+                        f"{response['item']['result']['value']}: {response['item']['result']['message']}",
+                    )
+
+                message = response["item"]["messages"][-1]
+                if generate:
+                    if generate["content_type"] == "IMAGE":
+                        async with ImageGenAsync(
+                                all_cookies=self.cookies,
+                                proxy=self.proxy
+                        ) as image_obj:
                             try:
-                                async with ImageGenAsync(
-                                    all_cookies=self.cookies,
-                                ) as image_generator:
-                                    images = await image_generator.get_images(
-                                        response["arguments"][0]["messages"][0]["text"],
-                                    )
-                                for i, image in enumerate(images):
-                                    resp_txt = f"{resp_txt}\n![image{i}]({image})"
-                                draw = True
+                                images = await image_obj.get_images(generate["prompt"])
                             except Exception as e:
-                                print(e)
-                                continue
-                        if (
-                            (
-                                response["arguments"][0]["messages"][0]["contentOrigin"]
-                                != "Apology"
-                            )
-                            and not draw
-                            and not raw
-                        ):
-                            body = response["arguments"][0]["messages"][0]["adaptiveCards"][0]["body"][0]
-                            resp_txt = result_text + body.get("text", "")
-                            resp_txt_no_link = result_text + response["arguments"][0][
-                                "messages"
-                            ][0].get("text", "")
-                            if msg_type and "inlines" in body:
-                                resp_txt = (
-                                    resp_txt
-                                    + body["inlines"][0].get("text")
-                                    + "\n"
-                                )
-                                result_text = (
-                                    result_text
-                                    + response["arguments"][0]["messages"][0][
-                                        "adaptiveCards"
-                                    ][0]["body"][0]["inlines"][0].get("text")
-                                    + "\n"
-                                )
-                        if not raw:
-                            yield False, resp_txt
-
-                elif response.get("type") == 2:
-                    if response["item"]["result"].get("error"):
-                        await self.close()
-                        raise Exception(
-                            f"{response['item']['result']['value']}: {response['item']['result']['message']}",
-                        )
-                    if draw:
-                        cache = response["item"]["messages"][1]["adaptiveCards"][0][
-                            "body"
-                        ][0]["text"]
-                        response["item"]["messages"][1]["adaptiveCards"][0]["body"][0][
-                            "text"
-                        ] = (cache + resp_txt)
-                    if (
-                        response["item"]["messages"][-1]["contentOrigin"] == "Apology"
-                        and resp_txt
-                    ):
-                        response["item"]["messages"][-1]["text"] = resp_txt_no_link
-                        response["item"]["messages"][-1]["adaptiveCards"][0]["body"][0][
-                            "text"
-                        ] = resp_txt
-                        print(
-                            "Preserved the message from being deleted",
-                            file=sys.stderr,
-                        )
-                    await wss.close()
-                    if not self.aio_session.closed:
-                        await self.aio_session.close()
-                    yield True, response
-                    return
-                if response.get("type") != 2:
-                    if response.get("type") == 6:
-                        await wss.send_str(append_identifier({"type": 6}))
-                    elif response.get("type") == 7:
-                        await wss.send_str(append_identifier({"type": 7}))
-                    elif raw:
-                        yield False, response
+                                print(str(e))
+                                hint = "Your prompt has been prohibited by third-service. Please modify it."
+                                resp_txt = f"{resp_txt}\n{e}\n{hint}"
+
+                if len(search_refs) > 0:
+                    refs_str = ""
+                    for index, item in enumerate(search_refs):
+                        refs_str += f'- [^{index}^] [{item["title"]}]({item["url"]})\n'
+
+                    resp_txt = f"{resp_txt}\n{refs_str}"
+
+                message["text"] = resp_txt
+                response["media"] = {
+                    "images": images
+                }
+
+                yield True, response
+                return
 
     async def _initial_handshake(self, wss) -> None:
-        await wss.send_str(append_identifier({"protocol": "json", "version": 1}))
-        await wss.receive_str()
-        await wss.send_str(append_identifier({"type": 6}))
+        proto = append_identifier({"protocol": "json", "version": 1})
+        await wss.asend(proto.encode("utf-8"))
+        await wss.arecv()
+        await wss.asend(append_identifier({"type": 6}).encode("utf8"))
+
+    async def _receive_messages(self, wss: WebSocket) -> Generator[str, Tuple[bytes, int], None]:
+        buffer = b''
+        retry_count = 5
+        is_connected = True
+        while is_connected:
+            # Receive the next chunk of data
+            chunk, flags = await wss.arecv()
+
+            if flags & CurlWsFlag.CLOSE:
+                is_connected = False
+
+            if not chunk:
+                retry_count -= 1
+                if retry_count == 0:
+                    raise Exception("No response from server")
+                continue
+
+            buffer += chunk
+            # Split the buffer by the delimiter
+            while b'\x1e' in buffer:
+                delimiter_index = buffer.index(b'\x1e')
+                # Extract the complete message up to the delimiter
+                complete_message = buffer[:delimiter_index]
+                yield complete_message.decode('utf-8')
+                # Remove the processed message from the buffer
+                buffer = buffer[delimiter_index + 1:]
+
+        return
 
     async def delete_conversation(
-        self,
-        conversation_id: str = None,
-        conversation_signature: str = None,
-        client_id: str = None,
+            self,
+            conversation_id: str = None,
+            conversation_signature: str = None,
+            client_id: str = None,
     ) -> None:
-        conversation_id = conversation_id or self.request.conversation_id
+        conversation_id = conversation_id or self.conversation_id
         conversation_signature = (
-            conversation_signature or self.request.conversation_signature
+                conversation_signature or self.request.conversation_signature
         )
         client_id = client_id or self.request.client_id
         url = "https://sydney.bing.com/sydney/DeleteSingleConversation"
         await self.session.post(
             url,
             json={
                 "conversationId": conversation_id,
@@ -266,8 +276,27 @@
                 "participant": {"id": client_id},
                 "source": "cib",
                 "optionsSets": ["autosave"],
             },
         )
 
     async def close(self) -> None:
-        await self.session.aclose()
+        await self.session.close()
+
+
+class AsyncSession(requests.AsyncSession):
+    def __init__(
+            self,
+            *,
+            loop=None,
+            async_curl: Optional[AsyncCurl] = None,
+            max_clients: int = 10,
+            **kwargs,
+    ):
+        super().__init__(loop=loop, async_curl=async_curl, max_clients=max_clients, **kwargs)
+
+    def is_closed(self):
+        return self._closed
+
+    async def close(self) -> None:
+        if not self._closed:
+            await super().close()
```

### Comparing `EdgeGPT-fork-0.14.1/src/EdgeGPT/constants.py` & `edgegpt_fork-1.0.0/src/EdgeGPT/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
 take_ip_socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
 take_ip_socket.connect(("8.8.8.8", 80))
 FORWARDED_IP: str = take_ip_socket.getsockname()[0]
 take_ip_socket.close()
 
 DELIMITER = "\x1e"
+PERSONATE = "chrome116"
 
 HEADERS = {
     "accept": "application/json",
     "accept-language": "en-US;q=0.9",
     "accept-encoding": "gzip, deflate, br, zsdch",
     "content-type": "application/json",
-    "sec-ch-ua": '"Not/A)Brand";v="99", "Microsoft Edge";v="115", "Chromium";v="115"',
     "sec-ch-ua-arch": '"x86"',
     "sec-ch-ua-bitness": '"64"',
     "sec-ch-ua-full-version": '"115.0.1901.188"',
     "sec-ch-ua-full-version-list": '"Not/A)Brand";v="99.0.0.0", "Microsoft Edge";v="115.0.1901.188", "Chromium";v="115.0.5790.114"',
     "sec-ch-ua-mobile": "?0",
     "sec-ch-ua-model": "",
     "sec-ch-ua-platform": '"Windows"',
@@ -31,24 +31,21 @@
     "Referer": "https://www.bing.com/search?",
     "Referrer-Policy": "origin-when-cross-origin",
     "x-forwarded-for": FORWARDED_IP,
 }
 
 HEADERS_INIT_CONVER = {
     "authority": "www.bing.com",
-    "accept": "application/json",
     "accept-language": "en-US;q=0.9",
     "cache-control": "max-age=0",
-    "sec-ch-ua": '"Not/A)Brand";v="99", "Microsoft Edge";v="115", "Chromium";v="115"',
     "sec-ch-ua-arch": '"x86"',
     "sec-ch-ua-bitness": '"64"',
     "sec-ch-ua-full-version": '"115.0.1901.188"',
     "sec-ch-ua-full-version-list": '"Not/A)Brand";v="99.0.0.0", "Microsoft Edge";v="115.0.1901.188", "Chromium";v="115.0.5790.114"',
     "sec-ch-ua-mobile": "?0",
     "sec-ch-ua-model": '""',
     "sec-ch-ua-platform": '"Windows"',
     "sec-ch-ua-platform-version": '"15.0.0"',
     "upgrade-insecure-requests": "1",
-    "user-agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/115.0.0.0 Safari/537.36 Edg/115.0.1901.188",
     "x-edge-shopping-flag": "1",
     "x-forwarded-for": FORWARDED_IP,
 }
```

### Comparing `EdgeGPT-fork-0.14.1/src/EdgeGPT/conversation.py` & `edgegpt_fork-1.0.0/src/EdgeGPT/conversation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import json
 import os
 from tkinter import NO
 from typing import List
 from typing import Union
 
-import httpx
+# import httpx.AsyncClient/
+from httpx import AsyncClient
+from curl_cffi import requests
+from curl_cffi.requests import AsyncSession
 
 from .constants import HEADERS_INIT_CONVER
 from .exceptions import NotAllowedToAccess
 
 
 class Conversation:
     def __init__(
@@ -23,28 +26,19 @@
             "conversationId": None,
             "clientId": None,
             "conversationSignature": None,
             "secAccessToken": None,
             "result": {"value": "Success", "message": None},
         }
         self.proxy = proxy
-        proxy = (
-            proxy
-            or os.environ.get("all_proxy")
-            or os.environ.get("ALL_PROXY")
-            or os.environ.get("https_proxy")
-            or os.environ.get("HTTPS_PROXY")
-            or None
-        )
-        if proxy is not None and proxy.startswith("socks5h://"):
-            proxy = "socks5://" + proxy[len("socks5h://") :]
-        self.session = httpx.Client(
-            proxies=proxy,
+        self.session = requests.Session(
+            proxy=proxy,
             timeout=900,
             headers=HEADERS_INIT_CONVER,
+            impersonate="chrome116"
         )
         if cookies:
             for cookie in cookies:
                 self.session.cookies.set(cookie["name"], cookie["value"])
         # Send GET request
         response = self.session.get(
             url=os.environ.get("BING_PROXY_URL")
@@ -59,14 +53,16 @@
             self.struct = response.json()
         except (json.decoder.JSONDecodeError, NotAllowedToAccess) as exc:
             raise Exception(
                 "Authentication failed. You have not been accepted into the beta.",
             ) from exc
         if self.struct["result"]["value"] == "UnauthorizedRequest":
             raise NotAllowedToAccess(self.struct["result"]["message"])
+        if 'X-Sydney-Encryptedconversationsignature' in response.headers:
+            self.struct['secAccessToken'] = response.headers['X-Sydney-Encryptedconversationsignature']
 
     @staticmethod
     async def create(
         proxy: Union[str, None] = None,
         cookies: Union[List[dict], None] = None,
     ) -> "Conversation":
         self = Conversation(async_mode=True)
@@ -84,45 +80,36 @@
             or os.environ.get("ALL_PROXY")
             or os.environ.get("https_proxy")
             or os.environ.get("HTTPS_PROXY")
             or None
         )
         if proxy is not None and proxy.startswith("socks5h://"):
             proxy = "socks5://" + proxy[len("socks5h://") :]
-        transport = httpx.AsyncHTTPTransport(retries=900)
-        # Convert cookie format to httpx format
-        formatted_cookies = None
-        if cookies:
-            formatted_cookies = httpx.Cookies()
-            for cookie in cookies:
-                formatted_cookies.set(cookie["name"], cookie["value"])
-        async with httpx.AsyncClient(
-            proxies=proxy,
-            timeout=30,
+
+        async with AsyncSession(
             headers=HEADERS_INIT_CONVER,
-            transport=transport,
-            cookies=formatted_cookies,
-        ) as client:
-            # Send GET request
-            response = await client.get(
-                url=os.environ.get("BING_PROXY_URL")
-                or "https://www.bing.com/turing/conversation/create",
-                follow_redirects=True,
-            )
-        if response.status_code != 200:
-            print(f"Status code: {response.status_code}")
-            print(response.text)
-            print(response.url)
-            raise Exception("Authentication failed")
-        try:
-            self.struct = response.json()
-        except (json.decoder.JSONDecodeError, NotAllowedToAccess) as exc:
-            print(response.text)
-            raise Exception(
-                "Authentication failed. You have not been accepted into the beta.",
-            ) from exc
-        if self.struct["result"]["value"] == "UnauthorizedRequest":
-            raise NotAllowedToAccess(self.struct["result"]["message"])
-        if 'X-Sydney-Encryptedconversationsignature' in response.headers:
-            self.struct['secAccessToken'] = response.headers['X-Sydney-Encryptedconversationsignature']
-        
-        return self
+            proxy=proxy,
+            impersonate="chrome116",
+        ) as s:
+            for cookie in cookies:
+                s.cookies.set(cookie["name"], cookie["value"])
+            url = os.environ.get("BING_PROXY_URL") or "https://www.bing.com/turing/conversation/create"
+            response = await s.get(url=url)
+            if response.status_code != 200:
+                print(f"Status code: {response.status_code}")
+                print(response.text)
+                print(response.url)
+                raise Exception("Authentication failed")
+
+            try:
+                self.struct = response.json()
+            except (json.decoder.JSONDecodeError, NotAllowedToAccess) as exc:
+                print(response.text)
+                raise Exception(
+                    "Authentication failed. You have not been accepted into the beta.",
+                ) from exc
+            if self.struct["result"]["value"] == "UnauthorizedRequest":
+                raise NotAllowedToAccess(self.struct["result"]["message"])
+            if 'X-Sydney-Encryptedconversationsignature' in response.headers:
+                self.struct['secAccessToken'] = response.headers['X-Sydney-Encryptedconversationsignature']
+
+            return self
```

### Comparing `EdgeGPT-fork-0.14.1/src/EdgeGPT/main.py` & `edgegpt_fork-1.0.0/src/EdgeGPT/main.py`

 * *Files identical despite different names*

### Comparing `EdgeGPT-fork-0.14.1/src/EdgeGPT/request.py` & `edgegpt_fork-1.0.0/src/EdgeGPT/request.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,86 @@
 import uuid
 from datetime import datetime
 from typing import Union
 
 from .conversation_style import CONVERSATION_STYLE_TYPE
-from .conversation_style import ConversationStyle
+from .conversation_style import ConversationStyle, Persona
+from .plugin import Plugin
 from .utilities import get_location_hint_from_locale
 from .utilities import get_ran_hex
 from .utilities import guess_locale
 import json
 
+
 class ChatHubRequest:
     def __init__(
-        self,
-        conversation_signature: str,
-        client_id: str,
-        conversation_id: str,
-        invocation_id: int = 3,
+            self,
+            conversation_signature: str,
+            client_id: str,
+            conversation_id: str,
+            invocation_id: int = 3,
     ) -> None:
         self.struct: dict = {}
 
         self.client_id: str = client_id
         self.conversation_id: str = conversation_id
         self.conversation_signature: str = conversation_signature
         self.invocation_id: int = invocation_id
 
     def update(
-        self,
-        prompt: str,
-        conversation_style: CONVERSATION_STYLE_TYPE,
-        webpage_context: Union[str, None] = None,
-        search_result: bool = False,
-        locale: str = guess_locale(),
-        mode: str = None,
-        no_search: bool = True,
+            self,
+            prompt: str,
+            conversation_style: CONVERSATION_STYLE_TYPE,
+            webpage_context: Union[str, None] = None,
+            locale: str = guess_locale(),
+            no_search: bool = True,
+            persona: Persona = Persona.copilot,
+            plugins: set[Plugin] = {}
     ) -> None:
         options = [
             "deepleo",
             "enable_debug_commands",
             "disable_emoji_spoken_text",
             "enablemm",
         ]
         if conversation_style:
             if not isinstance(conversation_style, ConversationStyle):
                 conversation_style = getattr(ConversationStyle, conversation_style)
             options = conversation_style.value.copy()
-        #enable gpt4_turbo
-        if mode == 'gpt4-turbo':
-            options.append('dlgpt4t')
-        
-        if no_search:
+        #enable gpt4_turbo deprecated
+        # if mode == 'gpt4-turbo':
+        #     options.append('gpt4tmncnp')
+
+        plugin_params = []
+        isSearchNeededforPlugin = False
+        for plugin in plugins:
+            val = plugin.value
+            if (val.id is not None):
+                plugin_params.append({
+                    "id": val.id,
+                    "category": 1
+                })
+
+            if (val.option_set is not None):
+                options.append(val.option_set)
+
+            if (not isSearchNeededforPlugin) and plugin != Plugin.codeInterpreter:
+                isSearchNeededforPlugin = True
+
+        if isSearchNeededforPlugin and (Plugin.search not in plugins):
+            plugin_params.append({
+                "id": Plugin.search.value.id,
+                "category": 1
+            })
+
+        if (not isSearchNeededforPlugin) and no_search:
             options.append('nosearchall')
 
+        options.append(persona.value)
+
         message_id = str(uuid.uuid4())
         # Get the current local time
         now_local = datetime.now()
 
         # Get the current UTC time
         now_utc = datetime.utcnow()
 
@@ -87,38 +113,49 @@
                         "RenderCardRequest",
                         "AdsQuery",
                         "SemanticSerp",
                         "GenerateContentQuery",
                         "SearchQuery",
                     ],
                     "sliceIds": [
-                        "winmuid1tf",
-                        "newmma-prod",
-                        "imgchatgptv2",
-                        "tts2",
-                        "voicelang2",
-                        "anssupfotest",
-                        "emptyoson",
-                        "tempcacheread",
-                        "temptacache",
-                        "ctrlworkpay",
-                        "winlongmsg2tf",
-                        "628fabocs0",
-                        "531rai268s0",
-                        "602refusal",
-                        "621alllocs0",
-                        "621docxfmtho",
-                        "621preclsvn",
-                        "330uaug",
-                        "529rweas0",
-                        "0626snptrcs0",
-                        "619dagslnv1nr"
+                        "0311tccs0",
+                        "gldidentitycf",
+                        "qnav2table1",
+                        "fltlatest",
+                        "ntbkwco",
+                        "cntralign2",
+                        "cntralign",
+                        "bcece403t",
+                        "crtcachenock",
+                        "romiccf",
+                        "rwt2",
+                        "cleanjsonctrl",
+                        "advtoknmic",
+                        "cacblvsdscf",
+                        "408mems0",
+                        "shopgptctrl",
+                        "0329mupcsts0",
+                        "unionfdbk",
+                        "fpallsticy",
+                        "0404redhoo",
+                        "saisgrds0",
+                        "duptelfix",
+                        "fixertel",
+                        "ntbkgoldcf",
+                        "kcclickthrucf",
+                        "cacfrwebt2",
+                        "sswebtop1cf",
+                        "sswebtop2",
+                        "sstopcf"
                     ],
                     "verbosity": "verbose",
+                    "scenario": "SERP",
+                    "plugins": plugin_params,
                     "traceId": get_ran_hex(32),
+                    "gptId": persona.name,
                     "isStartOfSession": self.invocation_id == 3,
                     "message": {
                         "locale": locale,
                         "market": locale,
                         "region": locale[-2:],  # en-US -> US
                         "locationHints": get_location_hint_from_locale(locale),
                         "timestamp": timestamp,
@@ -138,29 +175,20 @@
                     "conversationId": self.conversation_id,
                 },
             ],
             "invocationId": str(self.invocation_id),
             "target": "chat",
             "type": 4,
         }
-        if (not no_search) and (search_result):
-            have_search_result = [
-                "InternalSearchQuery",
-                "InternalSearchResult",
-                "InternalLoaderMessage",
-                "RenderCardRequest",
-            ]
-            self.struct["arguments"][0]["allowedMessageTypes"] += have_search_result
+
         if webpage_context:
             self.struct["arguments"][0]["previousMessages"] = [
                 {
                     "author": "user",
                     "description": webpage_context,
                     "contextType": "WebPage",
                     "messageType": "Context",
                     "messageId": "discover-web--page-ping-mriduna-----",
                 },
             ]
         self.invocation_id += 1
-
-        print(json.dumps(self.struct))
-        # print(timestamp)
+        # print(json.dumps(self.struct, indent=2, ensure_ascii=False))
```

### Comparing `EdgeGPT-fork-0.14.1/src/EdgeGPT/utilities.py` & `edgegpt_fork-1.0.0/src/EdgeGPT/utilities.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,17 +21,40 @@
     locale = locale.lower()
     if locale == "en-gb":
         hint = LocationHint.UK.value
     elif locale == "en-ie":
         hint = LocationHint.EU.value
     elif locale == "zh-cn":
         hint = LocationHint.CHINA.value
+    elif locale == "zh-hk":
+        hint = LocationHint.HONGKONG.value
+    elif locale == "zh-tw":
+        hint = LocationHint.TW.value
     else:
         hint = LocationHint.USA.value
     return hint.get("LocationHint")
 
 
 def guess_locale() -> str:
     if sys.platform.startswith("win"):
         return "en-us"
     loc, _ = locale.getlocale()
     return loc.replace("_", "-") if loc else "en-us"
+
+
+def parse_search_result(message):
+    if 'Web search returned no relevant result' in message['hiddenText']:
+        return [{
+            'title': 'No relevant result',
+            'url': None,
+            'snippet': message['hiddenText']
+        }]
+
+    data = []
+    for group in json.loads(message['text']).values():
+        for item in group:
+            data.append({
+                'title': item['title'],
+                'url': item['url'],
+            })
+
+    return data
```

### Comparing `EdgeGPT-fork-0.14.1/src/EdgeGPT_fork.egg-info/PKG-INFO` & `edgegpt_fork-1.0.0/src/EdgeGPT_fork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EdgeGPT-fork
-Version: 0.14.1
+Version: 1.0.0
 Summary: Reverse engineered Edge Chat API
 Home-page: https://github.com/xingty/EdgeGPT
 Author: Antonio Cheong,Bigbyto
 Author-email: acheong@student.dalat.org,bigbyto@gmail.com
 License: The Unlicense
 Project-URL: Bug Report, https://github.com/xingty/EdgeGPT/issues/new
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
@@ -19,15 +19,16 @@
 Requires-Dist: httpx[socks]>=0.24.0
 Requires-Dist: aiohttp
 Requires-Dist: websockets
 Requires-Dist: rich
 Requires-Dist: certifi
 Requires-Dist: prompt_toolkit
 Requires-Dist: requests
-Requires-Dist: BingImageCreator>=0.4.4
+Requires-Dist: BingImageCreator-fork>=0.7.6
+Requires-Dist: curl_cffi
 
 <div align="center">
   <img src="https://socialify.git.ci/acheong08/EdgeGPT/image?font=Inter&language=1&logo=https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2F9%2F9c%2FBing_Fluent_Logo.svg&owner=1&pattern=Floating%20Cogs&theme=Auto" alt="EdgeGPT" width="640" height="320" />
 
 # Edge GPT
 
 _The reverse engineering the chat feature of the new version of Bing_
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: EdgeGPT-fork Version: 0.14.1 Summary: Reverse
+Metadata-Version: 2.1 Name: EdgeGPT-fork Version: 1.0.0 Summary: Reverse
 engineered Edge Chat API Home-page: https://github.com/xingty/EdgeGPT Author:
 Antonio Cheong,Bigbyto Author-email:
 acheong@student.dalat.org,bigbyto@gmail.com License: The Unlicense Project-URL:
 Bug Report, https://github.com/xingty/EdgeGPT/issues/new Classifier: License ::
 OSI Approved :: The Unlicense (Unlicense) Classifier: Intended Audience ::
 Developers Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Description-
 Content-Type: text/markdown License-File: LICENSE Requires-Dist: httpx
 [socks]>=0.24.0 Requires-Dist: aiohttp Requires-Dist: websockets Requires-Dist:
 rich Requires-Dist: certifi Requires-Dist: prompt_toolkit Requires-Dist:
-requests Requires-Dist: BingImageCreator>=0.4.4
+requests Requires-Dist: BingImageCreator-fork>=0.7.6 Requires-Dist: curl_cffi
    [EdgeGPT]# Edge GPT _The reverse engineering the chat feature of the new
  version of Bing_ English - _ç_®__ä_½__ä_¸_­_æ__ - _ç_¹__é_«__ä_¸_­_æ__ - _E_s_p_a_Ã_±_o_l - _æ__¥_æ__¬_è_ª_
                 _[_P_y_P_I_ _v_e_r_s_i_o_n_][Python version][Total downloads]
 # Setup ## Install package ```bash python3 -m pip install EdgeGPT-fork --
 upgrade ``` ## Requirements - python 3.8+ - A Microsoft Account with access to
 bing.com/chat> (Optional, depending on your region) - Required in a supported
 country or region with New Bing (Chinese mainland VPN required) - [Selenium]
```

### Comparing `EdgeGPT-fork-0.14.1/src/EdgeGPT_fork.egg-info/SOURCES.txt` & `edgegpt_fork-1.0.0/src/EdgeGPT_fork.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 src/EdgeGPT/chathub.py
 src/EdgeGPT/constants.py
 src/EdgeGPT/conversation.py
 src/EdgeGPT/conversation_style.py
 src/EdgeGPT/exceptions.py
 src/EdgeGPT/locale.py
 src/EdgeGPT/main.py
+src/EdgeGPT/plugin.py
 src/EdgeGPT/request.py
 src/EdgeGPT/utilities.py
 src/EdgeGPT_fork.egg-info/PKG-INFO
 src/EdgeGPT_fork.egg-info/SOURCES.txt
 src/EdgeGPT_fork.egg-info/dependency_links.txt
 src/EdgeGPT_fork.egg-info/entry_points.txt
 src/EdgeGPT_fork.egg-info/requires.txt
```

