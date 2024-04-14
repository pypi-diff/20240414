# Comparing `tmp/nonebot_plugin_nai3-0.0.6.tar.gz` & `tmp/nonebot_plugin_nai3-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nai3-0.0.6.tar", max compression
+gzip compressed data, was "nonebot_plugin_nai3-0.0.7.tar", max compression
```

## Comparing `nonebot_plugin_nai3-0.0.6.tar` & `nonebot_plugin_nai3-0.0.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.0.6/LICENSE
--rw-r--r--   0        0        0     5449 2024-04-14 04:35:27.021468 nonebot_plugin_nai3-0.0.6/nonebot_plugin_nai3/__init__.py
--rw-r--r--   0        0        0      527 2024-04-14 04:33:00.118668 nonebot_plugin_nai3-0.0.6/nonebot_plugin_nai3/config.py
--rw-r--r--   0        0        0     1551 2024-04-13 15:11:02.114168 nonebot_plugin_nai3-0.0.6/nonebot_plugin_nai3/utils.py
--rw-r--r--   0        0        0      846 2024-04-14 04:35:39.778372 nonebot_plugin_nai3-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3981 2024-04-14 04:03:10.205762 nonebot_plugin_nai3-0.0.6/README.md
--rw-r--r--   0        0        0     4485 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.0.7/LICENSE
+-rw-r--r--   0        0        0     8265 2024-04-14 10:15:04.711349 nonebot_plugin_nai3-0.0.7/nonebot_plugin_nai3/__init__.py
+-rw-r--r--   0        0        0      527 2024-04-14 10:08:34.777191 nonebot_plugin_nai3-0.0.7/nonebot_plugin_nai3/config.py
+-rw-r--r--   0        0        0     2242 2024-04-14 09:09:14.219821 nonebot_plugin_nai3-0.0.7/nonebot_plugin_nai3/utils.py
+-rw-r--r--   0        0        0      864 2024-04-14 10:14:54.594690 nonebot_plugin_nai3-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4271 2024-04-14 10:14:33.143274 nonebot_plugin_nai3-0.0.7/README.md
+-rw-r--r--   0        0        0     4799 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.0.7/PKG-INFO
```

### Comparing `nonebot_plugin_nai3-0.0.6/LICENSE` & `nonebot_plugin_nai3-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.0.6/nonebot_plugin_nai3/__init__.py` & `nonebot_plugin_nai3-0.0.7/nonebot_plugin_nai3/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,35 @@
+import asyncio
 import io
+import os
 import random
 import time
 import zipfile
 from argparse import Namespace
+from importlib.metadata import version
 
+import ujson as json
 from httpx import AsyncClient
-from nonebot.adapters.onebot.v11 import GroupMessageEvent, MessageEvent, MessageSegment, PrivateMessageEvent
+from nonebot.adapters.onebot.v11 import GROUP_ADMIN, GROUP_OWNER, Bot, GroupMessageEvent, Message, MessageEvent, MessageSegment, PrivateMessageEvent
 from nonebot.log import logger
-from nonebot.params import ShellCommandArgs
+from nonebot.params import CommandArg, ShellCommandArgs
+from nonebot.permission import SUPERUSER
 from nonebot.plugin import PluginMetadata
-from nonebot.plugin.on import on_shell_command
+from nonebot.plugin.on import on_command, on_shell_command
 from nonebot.rule import ArgumentParser
 
 from .config import Config, nai3_config
-from .utils import headers, json_for_t2i
+from .utils import format_str, get_at, headers, json_for_t2i, list_to_str
 
-__version__ = "0.0.4"
+ADMIN = SUPERUSER | GROUP_ADMIN | GROUP_OWNER
+
+try:
+    __version__ = version("nonebot_plugin_nai3")
+except Exception:
+    __version__ = "0.0.0"
 
 __plugin_meta__ = PluginMetadata(
     name="nonebot-plugin-nai3",
     description="通过 NovelAI 生成图片",
     usage="通过 NovelAI 生成图片",
     homepage="https://github.com/zhulinyv/nonebot_plugin_nai3",
     type="application",
@@ -32,39 +42,51 @@
         "author": "zhulinyv",
         "version": __version__,
     },
 )
 
 
 nai3_parser = ArgumentParser()
-nai3_parser.add_argument("prompt", help="提示词(支持你喜欢的画风串)", type=str)
-nai3_parser.add_argument("-n", "--negative", help="负面提示词", type=str, dest="negative")
+nai3_parser.add_argument("prompt", nargs="*", help="提示词(支持你喜欢的画风串)", type=str)
+nai3_parser.add_argument("-n", "--negative", nargs="*", help="负面提示词", type=str, dest="negative")
 nai3_parser.add_argument("-r", "--resolution", help="画布形状/分辨率", type=str, dest="resolution")
 nai3_parser.add_argument("-s", "--scale", help="提示词相关性", type=float, dest="scale")
 nai3_parser.add_argument("-sm", help="sm", type=bool, dest="sm")
 nai3_parser.add_argument("-smdyn", help="smdyn", type=bool, dest="smdyn")
 nai3_parser.add_argument("--sampler", help="采样器", type=str, dest="sampler")
 nai3_parser.add_argument("--schedule", help="噪声计划表", type=str, dest="schedule")
 
-nai3 = on_shell_command("nai3", aliases={"nai"}, parser=nai3_parser, priority=30, block=True)
 
+nai3 = on_shell_command("nai3", aliases={"nai"}, parser=nai3_parser, priority=30, block=True)
+nai3_black = on_command("nai3黑名单", aliases={"nai3 黑名单", "nai黑名单", "nai 黑名单"}, priority=20, permission=ADMIN, block=True)
 
 cd = {}
 
 
 @nai3.handle()
-async def _(event: MessageEvent, args: Namespace = ShellCommandArgs()):
+async def _(bot: Bot, event: MessageEvent, args: Namespace = ShellCommandArgs()):
     if isinstance(event, PrivateMessageEvent):
         gid = uid = str(event.user_id)
     elif isinstance(event, GroupMessageEvent):
         gid = str(event.group_id)
         uid = str(event.user_id)
     else:
         await nai3.send("不支持该聊天捏~请切换至群聊或私聊重试!", at_sender=True)
 
+    try:
+        with open("./data/nai3/black_data.json", "r") as f:
+            black_data = json.load(f)
+        if event.get_user_id() not in bot.config.superusers:
+            if gid in black_data["group"]:
+                await nai3.finish("当前群聊在画图黑名单中!", at_sender=True)
+            if uid in black_data["user"]:
+                await nai3.finish("你在画图黑名单中!", at_sender=True)
+    except FileNotFoundError:
+        pass
+
     now_time = time.time()
     try:
         cd[gid]["user"][uid]["limit"]
     except KeyError:
         cd[gid] = {"cool_time": now_time - nai3_config.nai3_cooltime_group, "user": {uid: {"limit": nai3_config.nai3_limit, "cool_time": now_time - nai3_config.nai3_cooltime_user}}}
 
     if now_time - cd[gid]["cool_time"] < nai3_config.nai3_cooltime_group:
@@ -72,15 +94,15 @@
     if now_time - cd[gid]["user"][uid]["cool_time"] < nai3_config.nai3_cooltime_user:
         await nai3.finish("个人绘画冷却中, 剩余时间: {}...".format(round(nai3_config.nai3_cooltime_user - now_time + cd[gid]["cool_time"], 3)), at_sender=True)
     if cd[gid]["user"][uid]["limit"] <= 0:
         await nai3.finish("今天已经没次数了哦~", at_send=True)
 
     await nai3.send("脑积水已收到绘画指令, 正在生成图片(剩余次数: {})...".format(cd[gid]["user"][uid]["limit"]), at_sender=True)
 
-    json_for_t2i["input"] = args.prompt
+    json_for_t2i["input"] = format_str(list_to_str(args.prompt))
     resolution = args.resolution if args.resolution else "mb"
     if resolution == "mb":
         width = 832
         height = 1216
     elif resolution == "pc":
         width = 1216
         height = 832
@@ -94,27 +116,66 @@
     json_for_t2i["parameters"]["sampler"] = args.sampler if args.sampler else "k_euler"
     json_for_t2i["parameters"]["steps"] = 28
     json_for_t2i["parameters"]["sm"] = args.sm if args.sm else False
     json_for_t2i["parameters"]["sm_dyn"] = args.smdyn if args.smdyn else False
     json_for_t2i["parameters"]["noise_schedule"] = args.schedule if args.schedule else "native"
     seed = random.randint(1000000000, 9999999999)
     json_for_t2i["parameters"]["seed"] = seed
-    json_for_t2i["parameters"]["negative_prompt"] = args.negative if args.negative else nai3_config.nai3_negative
+    json_for_t2i["parameters"]["negative_prompt"] = format_str(list_to_str(args.negative)) if args.negative else nai3_config.nai3_negative
 
     logger.debug(">>>>>")
     logger.debug(json_for_t2i)
 
     try:
         async with AsyncClient() as client:
             response = await client.post("https://image.novelai.net/ai/generate-image", json=json_for_t2i, headers=headers, timeout=300)
-            logger.debug(response.status_code)
+            while response.status_code == 429:
+                await asyncio.sleep(random.randint(4, 8))
+                response = await client.post("https://image.novelai.net/ai/generate-image", json=json_for_t2i, headers=headers, timeout=300)
+                logger.debug(response.status_code)
             logger.debug("<<<<<")
             with zipfile.ZipFile(io.BytesIO(response.content), mode="r") as zip:
                 with zip.open("image_0.png") as image:
                     now_time = time.time()
                     cd[gid]["cool_time"] = now_time
                     cd[gid]["user"][uid]["limit"] = cd[gid]["user"][uid]["limit"] - 1
                     cd[gid]["user"][uid]["cool_time"] = now_time
                     await nai3.send(f"种子: {seed}\n" + MessageSegment.image(image.read()), at_sender=True)
                     return
     except Exception as e:
         await nai3.finish(f"出现错误: {e}", at_sender=True)
+
+
+@nai3_black.handle()
+async def _(event: MessageEvent, msg: Message = CommandArg()):
+    text_msg = msg.extract_plain_text().strip()
+    id = await get_at(event)
+    if id == -1:
+        id = text_msg.replace("添加", "").replace("删除", "").replace("群聊", "").replace("用户", "")
+
+    if not os.path.exists("./data/nai3"):
+        os.makedirs("./data/nai3")
+        black_data = {"user": [], "group": []}
+        with open("./data/nai3/black_data.json", "w", encoding="utf-8") as f:
+            json.dump(black_data, f, indent=4, ensure_ascii=False)
+
+    with open("./data/nai3/black_data.json", "r") as f:
+        black_data = json.load(f)
+    if "添加" in text_msg:
+        if "群聊" in text_msg:
+            black_data["group"].append(str(id))
+        elif "用户" in text_msg:
+            black_data["user"].append(str(id))
+        else:
+            await nai3_black.finish("输入有误!", at_sender=True)
+        action_msg = "添加成功!"
+    if "删除" in text_msg:
+        if "群聊" in text_msg:
+            black_data["group"].remove(str(id))
+        elif "用户" in text_msg:
+            black_data["user"].remove(str(id))
+        else:
+            await nai3_black.finish("输入有误!", at_sender=True)
+        action_msg = "删除成功!"
+    with open("./data/nai3/black_data.json", "w", encoding="utf-8") as f:
+        json.dump(black_data, f, indent=4, ensure_ascii=False)
+    await nai3_black.finish(action_msg, at_sender=True)
```

### Comparing `nonebot_plugin_nai3-0.0.6/nonebot_plugin_nai3/config.py` & `nonebot_plugin_nai3-0.0.7/nonebot_plugin_nai3/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.0.6/nonebot_plugin_nai3/utils.py` & `nonebot_plugin_nai3-0.0.7/nonebot_plugin_nai3/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from nonebot.adapters.onebot.v11 import GroupMessageEvent
+
 from .config import nai3_config
 
 headers = {
     "Accept": "*/*",
     "Accept-Encoding": "gzip, deflate, br",
     "Accept-Language": "en-GB,en;q=0.9,zh-CN;q=0.8,zh;q=0.7,en-US;q=0.6",
     "Authorization": f"Bearer {nai3_config.nai3_token}",
@@ -43,7 +45,32 @@
         "seed": int,
         "negative_prompt": str,
         "reference_image_multiple": [],
         "reference_information_extracted_multiple": [],
         "reference_strength_multiple": [],
     },
 }
+
+
+def list_to_str(str_list: list):
+    empty_str = ""
+    for i in str_list:
+        if i[-1] == ",":
+            empty_str += f"{i}"
+        else:
+            empty_str += f"{i},"
+    return empty_str
+
+
+def format_str(str_: str):
+    str_ = str_.replace(", ", ",")
+    str_ = str_.replace(",", ", ")
+    str_ = str_[:-2] if str_[-2:] == ", " else str_
+    return str_
+
+
+async def get_at(event: GroupMessageEvent) -> int:
+    msg = event.get_message()
+    for msg_seg in msg:
+        if msg_seg.type == "at":
+            return -1 if msg_seg.data["qq"] == "all" else int(msg_seg.data["qq"])
+    return -1
```

### Comparing `nonebot_plugin_nai3-0.0.6/pyproject.toml` & `nonebot_plugin_nai3-0.0.7/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "nonebot-plugin-nai3"
-version = "0.0.6"
+version = "0.0.7"
 description = "通过 NovelAI 生成图片"
 authors = ["zhulinyv <zhulinyv2005@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_nai3"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 nonebot2 = "^2.2.1"
 httpx = "^0.24.1"
 nonebot-adapter-onebot = "^2.2.3"
+ujson = "^5.9.0"
 
 # https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html
 [tool.black]
 line-length = 500
 
 # https://beta.ruff.rs/docs/settings/
 [tool.ruff]
```

### Comparing `nonebot_plugin_nai3-0.0.6/README.md` & `nonebot_plugin_nai3-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -94,23 +94,37 @@
     --schedule      噪声计划表, 默认: native
 示例: nai3 1girl, loli, cute -r mb -s 5.0
 返回: 
 ```
 
 ![img](./img/1.png)
 
+```
+指令: nai3黑名单/黑名单
+参数:
+    添加    添加黑名单
+    删除    删除黑名单
+    用户    指定添加类型
+    群聊    指定添加类型
+    群号/QQ号/@sb.
+示例: nai3黑名单添加用户 @脑积水
+返回: 
+```
+
+![img](./img/2.png)
+
 ## 📖 待办
 
 + [x] 文生图
 + [ ] 图生图
 + [x] 自定义参数
-+ [ ] 队列功能
++ [ ] ~~队列功能~~
 + [x] 冷却功能
 + [x] 上限功能
-+ [ ] 黑名单功能
++ [x] 黑名单功能
 + [ ] 代理
 + [ ] R18 检测
 + [ ] 翻译
 + [ ] 帮助指令
 + [ ] ...
 
 ## 🤝 鸣谢
```

#### html2text {}

```diff
@@ -29,15 +29,18 @@
 github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-
 446d-9401-e559628ad079) ## ð ä½¿ç¨ ``` æä»¤: nai3/nai åæ°: prompt
 æç¤ºè¯(æ¯æä½ åæ¬¢çç»é£ä¸²), é»è®¤: None -n/--negative
 è´é¢æç¤ºè¯, é»è®¤: nsfw,... -r/--resolution ç»å¸å½¢ç¶/åè¾¨ç,
 ["mb", "pc", "sq"] ä¸éä¸, é»è®¤: mb -s/--scale æç¤ºè¯ç¸å³æ§, é»è®¤:
 5.0 -sm sm, é»è®¤: False -smdyn smdyn, é»è®¤: False --sampler éæ ·å¨,
 é»è®¤: k_euler --schedule åªå£°è®¡åè¡¨, é»è®¤: native ç¤ºä¾: nai3 1girl,
-loli, cute -r mb -s 5.0 è¿å: ``` ![img](./img/1.png) ## ð å¾å + [x]
-æçå¾ + [ ] å¾çå¾ + [x] èªå®ä¹åæ° + [ ] éååè½ + [x]
-å·å´åè½ + [x] ä¸éåè½ + [ ] é»åååè½ + [ ] ä»£ç + [ ] R18
-æ£æµ + [ ] ç¿»è¯ + [ ] å¸®å©æä»¤ + [ ] ... ## ð¤ é¸£è°¢
-æ¬é¡¹ç®éæ­¥è¿ç§»èª [Semi-Auto-NovelAI-to-Pixiv](https://github.com/
-zhulinyv/Semi-Auto-NovelAI-to-Pixiv)
+loli, cute -r mb -s 5.0 è¿å: ``` ![img](./img/1.png) ``` æä»¤:
+nai3é»åå/é»åå åæ°: æ·»å  æ·»å é»åå å é¤ å é¤é»åå
+ç¨æ· æå®æ·»å ç±»å ç¾¤è æå®æ·»å ç±»å ç¾¤å·/QQå·/@sb. ç¤ºä¾:
+nai3é»ååæ·»å ç¨æ· @èç§¯æ°´ è¿å: ``` ![img](./img/2.png) ## ð
+å¾å + [x] æçå¾ + [ ] å¾çå¾ + [x] èªå®ä¹åæ° + [ ]
+~~éååè½~~ + [x] å·å´åè½ + [x] ä¸éåè½ + [x] é»åååè½ +
+[ ] ä»£ç + [ ] R18 æ£æµ + [ ] ç¿»è¯ + [ ] å¸®å©æä»¤ + [ ] ... ## ð¤
+é¸£è°¢ æ¬é¡¹ç®éæ­¥è¿ç§»èª [Semi-Auto-NovelAI-to-Pixiv](https://
+github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv)
 ===============================================================================
 [https://count.getloli.com/get/@zhulinyv?theme=rule34]
```

### Comparing `nonebot_plugin_nai3-0.0.6/PKG-INFO` & `nonebot_plugin_nai3-0.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nai3
-Version: 0.0.6
+Version: 0.0.7
 Summary: 通过 NovelAI 生成图片
 License: MIT
 Author: zhulinyv
 Author-email: zhulinyv2005@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
 Requires-Dist: nonebot2 (>=2.2.1,<3.0.0)
+Requires-Dist: ujson (>=5.9.0,<6.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/raw/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/raw/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
@@ -112,23 +113,37 @@
     --schedule      噪声计划表, 默认: native
 示例: nai3 1girl, loli, cute -r mb -s 5.0
 返回: 
 ```
 
 ![img](./img/1.png)
 
+```
+指令: nai3黑名单/黑名单
+参数:
+    添加    添加黑名单
+    删除    删除黑名单
+    用户    指定添加类型
+    群聊    指定添加类型
+    群号/QQ号/@sb.
+示例: nai3黑名单添加用户 @脑积水
+返回: 
+```
+
+![img](./img/2.png)
+
 ## 📖 待办
 
 + [x] 文生图
 + [ ] 图生图
 + [x] 自定义参数
-+ [ ] 队列功能
++ [ ] ~~队列功能~~
 + [x] 冷却功能
 + [x] 上限功能
-+ [ ] 黑名单功能
++ [x] 黑名单功能
 + [ ] 代理
 + [ ] R18 检测
 + [ ] 翻译
 + [ ] 帮助指令
 + [ ] ...
 
 ## 🤝 鸣谢
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.0.6 Summary: éè¿
+Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.0.7 Summary: éè¿
 NovelAI çæå¾ç License: MIT Author: zhulinyv Author-email:
 zhulinyv2005@outlook.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist: nonebot-adapter-onebot
-(>=2.2.3,<3.0.0) Requires-Dist: nonebot2 (>=2.2.1,<3.0.0) Description-Content-
-Type: text/markdown
+(>=2.2.3,<3.0.0) Requires-Dist: nonebot2 (>=2.2.1,<3.0.0) Requires-Dist: ujson
+(>=5.9.0,<6.0.0) Description-Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
                        ************ nnoonneebboott__pplluuggiinn__nnaaii33 ************
                    ****** ?â??¨?é???è?¿? NNoovveellAAII ?ç???æ???å??¾?ç???â??¨ ******
        [https://img.shields.io/badge/Python-3.9+-blue]_[_l_i_c_e_n_s_e_][https://
       img.shields.io/github/issues/zhulinyv/nonebot_plugin_nai3][https://
       img.shields.io/github/stars/zhulinyv/nonebot_plugin_nai3][https://
@@ -38,15 +38,18 @@
 github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-
 446d-9401-e559628ad079) ## ð ä½¿ç¨ ``` æä»¤: nai3/nai åæ°: prompt
 æç¤ºè¯(æ¯æä½ åæ¬¢çç»é£ä¸²), é»è®¤: None -n/--negative
 è´é¢æç¤ºè¯, é»è®¤: nsfw,... -r/--resolution ç»å¸å½¢ç¶/åè¾¨ç,
 ["mb", "pc", "sq"] ä¸éä¸, é»è®¤: mb -s/--scale æç¤ºè¯ç¸å³æ§, é»è®¤:
 5.0 -sm sm, é»è®¤: False -smdyn smdyn, é»è®¤: False --sampler éæ ·å¨,
 é»è®¤: k_euler --schedule åªå£°è®¡åè¡¨, é»è®¤: native ç¤ºä¾: nai3 1girl,
-loli, cute -r mb -s 5.0 è¿å: ``` ![img](./img/1.png) ## ð å¾å + [x]
-æçå¾ + [ ] å¾çå¾ + [x] èªå®ä¹åæ° + [ ] éååè½ + [x]
-å·å´åè½ + [x] ä¸éåè½ + [ ] é»åååè½ + [ ] ä»£ç + [ ] R18
-æ£æµ + [ ] ç¿»è¯ + [ ] å¸®å©æä»¤ + [ ] ... ## ð¤ é¸£è°¢
-æ¬é¡¹ç®éæ­¥è¿ç§»èª [Semi-Auto-NovelAI-to-Pixiv](https://github.com/
-zhulinyv/Semi-Auto-NovelAI-to-Pixiv)
+loli, cute -r mb -s 5.0 è¿å: ``` ![img](./img/1.png) ``` æä»¤:
+nai3é»åå/é»åå åæ°: æ·»å  æ·»å é»åå å é¤ å é¤é»åå
+ç¨æ· æå®æ·»å ç±»å ç¾¤è æå®æ·»å ç±»å ç¾¤å·/QQå·/@sb. ç¤ºä¾:
+nai3é»ååæ·»å ç¨æ· @èç§¯æ°´ è¿å: ``` ![img](./img/2.png) ## ð
+å¾å + [x] æçå¾ + [ ] å¾çå¾ + [x] èªå®ä¹åæ° + [ ]
+~~éååè½~~ + [x] å·å´åè½ + [x] ä¸éåè½ + [x] é»åååè½ +
+[ ] ä»£ç + [ ] R18 æ£æµ + [ ] ç¿»è¯ + [ ] å¸®å©æä»¤ + [ ] ... ## ð¤
+é¸£è°¢ æ¬é¡¹ç®éæ­¥è¿ç§»èª [Semi-Auto-NovelAI-to-Pixiv](https://
+github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv)
 ===============================================================================
 [https://count.getloli.com/get/@zhulinyv?theme=rule34]
```

