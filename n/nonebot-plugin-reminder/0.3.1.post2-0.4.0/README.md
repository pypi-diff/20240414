# Comparing `tmp/nonebot_plugin_reminder-0.3.1.post2.tar.gz` & `tmp/nonebot_plugin_reminder-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_reminder-0.3.1.post2.tar", max compression
+gzip compressed data, was "nonebot_plugin_reminder-0.4.0.tar", max compression
```

## Comparing `nonebot_plugin_reminder-0.3.1.post2.tar` & `nonebot_plugin_reminder-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1066 2024-04-06 15:24:21.657883 nonebot_plugin_reminder-0.3.1.post2/LICENSE
--rw-r--r--   0        0        0     5030 2024-04-06 15:24:21.657883 nonebot_plugin_reminder-0.3.1.post2/README.md
--rw-r--r--   0        0        0    23268 2024-04-06 15:24:21.657883 nonebot_plugin_reminder-0.3.1.post2/nonebot_plugin_reminder/__init__.py
--rw-r--r--   0        0        0      544 2024-04-06 15:24:21.657883 nonebot_plugin_reminder-0.3.1.post2/nonebot_plugin_reminder/config.py
--rw-r--r--   0        0        0     4491 2024-04-06 15:24:21.657883 nonebot_plugin_reminder-0.3.1.post2/nonebot_plugin_reminder/data_utils.py
--rw-r--r--   0        0        0      581 2024-04-06 15:24:21.657883 nonebot_plugin_reminder-0.3.1.post2/pyproject.toml
--rw-r--r--   0        0        0     6032 1970-01-01 00:00:00.000000 nonebot_plugin_reminder-0.3.1.post2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-14 03:03:32.345770 nonebot_plugin_reminder-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5030 2024-04-14 03:03:32.345770 nonebot_plugin_reminder-0.4.0/README.md
+-rw-r--r--   0        0        0    20702 2024-04-14 03:03:32.345770 nonebot_plugin_reminder-0.4.0/nonebot_plugin_reminder/__init__.py
+-rw-r--r--   0        0        0      544 2024-04-14 03:03:32.345770 nonebot_plugin_reminder-0.4.0/nonebot_plugin_reminder/config.py
+-rw-r--r--   0        0        0     4491 2024-04-14 03:03:32.345770 nonebot_plugin_reminder-0.4.0/nonebot_plugin_reminder/data_utils.py
+-rw-r--r--   0        0        0      564 2024-04-14 03:03:32.345770 nonebot_plugin_reminder-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6011 1970-01-01 00:00:00.000000 nonebot_plugin_reminder-0.4.0/PKG-INFO
```

### Comparing `nonebot_plugin_reminder-0.3.1.post2/LICENSE` & `nonebot_plugin_reminder-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_reminder-0.3.1.post2/README.md` & `nonebot_plugin_reminder-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_reminder-0.3.1.post2/nonebot_plugin_reminder/__init__.py` & `nonebot_plugin_reminder-0.4.0/nonebot_plugin_reminder/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,25 @@
+import datetime
 import random
 import string
 from nonebot.plugin import on_regex
 from nonebot.params import ArgPlainText
+from nonebot.adapters.onebot.v11 import (
+    Bot,
+    MessageEvent,
+    Message,
+    MessageSegment,
+    GroupMessageEvent
+)
+
 from nonebot.rule import to_me
 from nonebot.params import Matcher, RegexGroup
 from nonebot.log import logger
 from nonebot.permission import SUPERUSER
 from nonebot import require, get_driver, get_bot, get_bots
-from nonebot.adapters import Message, Event, Bot
 from typing import Any, Dict, List, Optional, Tuple
 from pathlib import Path
 from datetime import date, datetime, timedelta
 import asyncio
 import aiofiles
 from .config import Config
 from functools import partial
@@ -20,19 +28,15 @@
     import ujson as json
 except ImportError:
     import json
 from nonebot.plugin import PluginMetadata
 from io import StringIO
 from nonebot.typing import T_State
 from nonebot.adapters import MessageTemplate
-from .data_utils import detail_backup, get_datas, save_datas, clear_datas, item2string, backup, recover, list_backup
-require("nonebot_plugin_saa")
-from nonebot_plugin_saa import Text, MessageFactory, Image, \
-SaaTarget, PlatformTarget, TargetQQGroup, TargetQQPrivate, MessageSegmentFactory, \
-Mention, Reply
+from .data_utils import get_datas, save_datas, clear_datas, item2string
 __version__ = "0.1.1"
 
 __plugin_meta__ = PluginMetadata(
     name="定时提醒",
     description="主要用来提醒大家别忘记什么事情，可以看成定时提醒插件",
     usage='''
     定时 [date]→ 设置定时提醒，date为时间，格式为HH:MM，如 23:59， 不设置默认为17点 \n
@@ -56,427 +60,321 @@
     # 支持的适配器集合，其中 `~` 在此处代表前缀 `nonebot.adapters.`，其余适配器亦按此格式填写。
     # 若插件可以保证兼容所有适配器（即仅使用基本适配器功能）可不填写，否则应该列出插件支持的适配器。
 )
 driver = get_driver()
 plugin_config = Config.parse_obj(driver.config)
 CONFIG = get_datas()
 
+
 try:
     scheduler = require("nonebot_plugin_apscheduler").scheduler
 except Exception:
     scheduler = None
 
 logger.opt(colors=True).info(
     "已检测到软依赖<y>nonebot_plugin_apscheduler</y>, <g>开启定时任务功能</g>"
     if scheduler
     else "未检测到软依赖<y>nonebot_plugin_apscheduler</y>，<r>禁用定时任务功能</r>"
 )
-# ^(?:(?:\@.*))* 用于兼容一些插件，群聊时被@,没有去掉@的那一部分
-remainer_matcher = on_regex(r"^(?:(?:\@.*))*定时[\s]*(\d{1,2}:\d{1,2})?$", priority=999, rule=to_me())
-fetch_matcher = on_regex(r"^(?:(?:\@.*))*定时请求[\s]*(\d{1,2}:\d{1,2})?$", priority=999,rule=to_me())
-list_matcher = on_regex(r"^(?:(?:\@.*))*定时列表[\s]*(\d+)?", priority=999, rule=to_me())
-list_apsjob_matcher = on_regex(r"^(?:(?:\@.*))*定时jobs[\s]*(\d+)?", priority=999,rule=to_me())
-clear_matcher = on_regex(r"^(?:(?:\@.*))*清(空|除)定时$", priority=999,rule=to_me())
-turn_matcher = on_regex(rf"^(?:(?:\@.*))*(查看|开启|关闭|删除|执行)定时[\s]*({plugin_config.reminder_id_prefix + '_'}[a-zA-Z0-9]+)$", priority=999, permission=SUPERUSER,rule=to_me())
-update_matcher = on_regex(rf"^(?:(?:\@.*))*(修改|更新)定时[\s]*({plugin_config.reminder_id_prefix + '_'}[a-zA-Z0-9]+)$", priority=999, permission=SUPERUSER,rule=to_me())
-backup_matcher = on_regex(rf"^(?:(?:\@.*))*(备份定时|定时备份)$", priority=999, permission=SUPERUSER,rule=to_me())
-backup_list_matcher = on_regex(rf"^(?:(?:\@.*))*备份列表[\s]*(\d+)?", priority=999, permission=SUPERUSER,rule=to_me())
-backup_recover_matcher = on_regex(rf"^(?:(?:\@.*))*(?:备份恢复|恢复备份|还原备份|备份还原|使用备份|备份使用)[\s]*([_a-zA-Z0-9]+)$", priority=999, permission=SUPERUSER,rule=to_me())
-backup_detail_mathcer = on_regex(rf"^(?:(?:\@.*))*查看备份[\s]*([_a-zA-Z0-9]+)$", priority=999, permission=SUPERUSER,rule=to_me())
 
-lock = asyncio.Lock()
+remainer_matcher = on_regex(r"^定时[\s]*(\d{1,2}:\d{1,2})?$", priority=999, rule=to_me())
+fetch_matcher = on_regex(r"^定时请求[\s]*(\d{1,2}:\d{1,2})?$", priority=999,rule=to_me())
+list_matcher = on_regex(r"^定时列表[\s]*(\d+)?", priority=999,rule=to_me())
+list_apsjob_matcher = on_regex(r"^定时jobs", priority=999,rule=to_me())
+clear_matcher = on_regex(r"^清(空|除)定时", priority=999,rule=to_me())
+turn_matcher = on_regex(rf"^(查看|开启|关闭|删除|执行)定时[\s]*({plugin_config.reminder_id_prefix + '_'}[a-zA-Z0-9]+)$", priority=999, permission=SUPERUSER,rule=to_me())
+update_matcher = on_regex(rf"^(修改|更新)定时[\s]*({plugin_config.reminder_id_prefix + '_'}[a-zA-Z0-9]+)$", priority=999, permission=SUPERUSER,rule=to_me())
 
-targetTypes: Dict[str, str] = {
-    "qqGroup": TargetQQGroup(group_id=123456789).platform_type,
-    "qqPrivate": TargetQQPrivate(user_id=100101).platform_type,
-}
+lock = asyncio.Lock()
 
 
 @remainer_matcher.got("repeat", prompt="选择执行间隔:\n1.每天 回复1 \n2.某天回复具体日期，格式为yyyy-mm-dd,如2023-01-03 \n3.工作日 回复3")
 @remainer_matcher.got("word", prompt="请输入提醒语句，默认为 打卡!!!， 回复0即可")
 async def remainer_handler(
-    matcher: Matcher,
-    event: Event,
-    target: SaaTarget,
     bot: Bot,
+    event: MessageEvent,
+    matcher: Matcher,
     args: Tuple[Optional[str]] = RegexGroup(),
-    word: str = ArgPlainText(),
-    repeat: str = ArgPlainText(),
+    word: Message = ArgPlainText(),
+    repeat: Message = ArgPlainText(),
     url: str = None
 ):
-    userId = event.get_user_id()
+    logger.opt(colors=True).debug(
+        f"scheduler.print_jobs(): {scheduler.print_jobs()}"
+    )
     arg1 = args[0] if args[0] else f'{plugin_config.reminder_default_hour:02d}:{plugin_config.reminder_default_minute:02d}'
     
     word = word if word != '0' else "打卡!!!"
-
-    if not bot:
-        sendReply(f"当前用户:{bot.self_id} 不是bot")
+    
+    msg = Message("")
+    groupId = -1
+    if isinstance(event, GroupMessageEvent):
+        groupId = event.group_id
     try:
-        res = await addScheduler(bot.self_id, target,  arg1, word, repeat=repeat, url=url)
+        res = await addScheduler(bot.self_id, arg1, word, event.user_id, groupId=groupId, repeat=repeat, url=url)
         logger.opt(colors=True).debug(
             f"addScheduler.res: {res}"
         )
         if res is not None and res != "" and res["code"] != 0:
-            msg = Text(res['msg'])
+            msg = Message(res['msg'])
         else:
-            msg = Text("设置成功")
+            msg = Message("设置成功")
     except Exception as e:
         logger.exception(e)
-        msg = Text("设置失败")
+        msg = Message("设置失败")
     
-    await sendReply(msg, target)
+    await sendReply(bot, matcher, event, msg)
 
 @fetch_matcher.got("repeat", prompt="选择执行间隔:\n1.每天 回复1 \n2.某天回复具体日期，格式为yyyy-mm-dd,如2023-01-03 \n3.工作日 回复3")
 @fetch_matcher.got("word", prompt="请输入提醒语句，默认为 打卡!!!， 回复0即可")
 @fetch_matcher.got("url", prompt="请输入需要请求的url，目前支持图片")
 async def fetch_handler(
     bot: Bot,
-    event: Event,
+    event: MessageEvent,
     matcher: Matcher,
-    target: SaaTarget,
     args: Tuple[Optional[str]] = RegexGroup(),
-    word: str = ArgPlainText(),
-    repeat: str = ArgPlainText(),
+    word: Message = ArgPlainText(),
+    repeat: Message = ArgPlainText(),
     url: str = ArgPlainText()
 ):
     if url is None or url == "" or not isUrlSupport(url):
-        await sendReply("暂不支持该类型的请求", target)
+        await sendReply(bot, matcher, event, "暂不支持该类型的请求")
     else:
-        await remainer_handler( matcher=matcher, bot=bot, event=event, target=target, args=args, word=word, repeat=repeat, url=url)
+        await remainer_handler(bot, event, matcher, args, word, repeat, url)
 
 
-@update_matcher.got("type", prompt="请输入需要修改的地方： 1. 时间 2.间隔 3.提醒语句 4.url 5.私聊对象 6.群组")
+@update_matcher.got("type", prompt="请输入需要修改的地方： 1. 时间 2.间隔 3.提醒语句 4.url 5.对象 6.群组")
 async def update_handler(
     bot: Bot,
-    event: Event,
-    target: SaaTarget,
+    event: MessageEvent,
     matcher: Matcher,
     state: T_State,
     args: Tuple[Optional[str], ...] = RegexGroup(),
-    type: str = ArgPlainText()
+    type: Message = ArgPlainText()
 ):
     typeMap = {"1": "time", "2": "repeat", "3": "data", "4": "url", "5": "userId", "6": "groupId"}
     if not scheduler:
-        await sendReply("未安装软依赖nonebot_plugin_apscheduler，不能使用定时发送功能", target)
+        await sendReply(bot, matcher, event, "未安装软依赖nonebot_plugin_apscheduler，不能使用定时发送功能")
     if args[1] is None:
-        await sendReply("请输入具体的id", target)
+        await sendReply(bot, matcher, event, "请输入具体的id")
     schId = args[1]
  
     jobItem = findJobFromJSONById(schId)
     if jobItem is None:
-        await sendReply("未找到该id的定时提醒", target)
-    
-    oldValue = ""
-    if type in ["5", "6"]:
-        toTarget = buildTarget(jobItem["target"])
-        logger.opt(colors=True).debug(
-            f"修改发送目标 toTarget: {toTarget}"
-        )
-        oldValue = jobItem["target"]
-    else:
-        oldValue = jobItem[typeMap[type]] if jobItem and typeMap[type] in jobItem else ""
+        await sendReply(bot, matcher, event, "未找到该id的定时提醒")
+            
+    oldValue = jobItem[typeMap[type]] if jobItem and typeMap[type] in jobItem else ""
     
     state["reminder_update_old_value"] = oldValue
     state["reminder_update_type"] = type
     state["reminder_update_jobItem"] = jobItem
 
 @update_matcher.got("newValue", prompt=MessageTemplate("请输入更新后的值，当前为: {reminder_update_old_value}"))
 async def update_handler2(
     bot: Bot,
-    event: Event,
-    target: SaaTarget,
+    event: MessageEvent,
     matcher: Matcher,
     state: T_State,
-    newValue: str = ArgPlainText(),
+    newValue: Message = ArgPlainText(),
 ):
     item = state["reminder_update_jobItem"]
     if item is None:
-        sendReply("未找到定时提醒", target)
+        sendReply(bot, matcher, event, "未找到定时提醒")
     typeMap = {"1": "time", "2": "repeat", "3": "data", "4": "url", "5": "userId", "6": "groupId"}
-    if state["reminder_update_type"] in ["5", "6"]:
-        if state["reminder_update_type"] == "5":
-            toTarget = TargetQQPrivate(user_id=int(newValue))
-        else:
-            toTarget = TargetQQGroup(group_id=int(newValue))
-        logger.opt(colors=True).debug(
-            f"修改发送目标 toTarget: {toTarget}"
-        )
-        item["target"] = toTarget.dict()
-    else:
-        item[typeMap[state["reminder_update_type"]]] = newValue
+    item[typeMap[state["reminder_update_type"]]] = newValue
     
-    msg = Text("")
+    msg = Message("")
     res = await updateScheduler(item)
     if res is not None and res != "":
         if res["code"] != 0:
-            msg += res
+            msg.append(res)
         else:
-            msg += f"设置成功, 最新信息如下\n {item2string(item)}"
+            msg.append(f"设置成功, id更改为: {res['msg']}")
     else:
-        msg += "设置成功"
-    await sendReply(msg, target)
+        msg.append("设置成功")
+    await sendReply(bot, matcher, event, msg)
 
 @list_matcher.handle()
 async def list_matcher_handle(
-    target: SaaTarget,
+    bot: Bot,
+    event: MessageEvent,
+    matcher: Matcher,
     args: Tuple[Optional[int], ...] = RegexGroup(),
 ):
     page = args[0] if len(args) > 0 and args[0] else 1
-    page = int(page)
     pageSize = plugin_config.reminder_page_size
     startIdx = (page - 1) * pageSize
-    msg = ""
-    # logger.opt(colors=True).info(
-    #     f"CONFIG: {CONFIG}"
-    # )
-    msg += f"共计{len(CONFIG)}个定时提醒 \n\
--------------------------\n"
+    msg = Message("")
+    logger.opt(colors=True).info(
+        f"CONFIG: {CONFIG}"
+    )
+    msg.append(f"共计{len(CONFIG)}个定时提醒 \n\
+-------------------------\n")
     
     # 分页返回
     items = list(CONFIG.values())
-    logger.opt(colors=True).info(
-        f"<y>args:{args} startIdx: {startIdx}, len(items):{len(items)}, pageSize:{pageSize}, page:{page}</y>"
-    )
     for idx in range(startIdx, len(items)):
         if idx < (page - 1) * pageSize or idx >= page * pageSize:
             break
         item = items[idx]
         
-        msg += item2string(item)
+        msg.append(item2string(item))
 
-    if(str(msg) == ""):
-        msg += "没有定时提醒"
+    if(msg.extract_plain_text() == ""):
+        msg.append("没有定时提醒")
     
-    await sendReply(msg, target)
+    await sendReply(bot, matcher, event, msg)
 
 @list_apsjob_matcher.handle()
 async def list_apsjob_matcher_handle(
-    target: SaaTarget,
-    args: Tuple[Optional[int], ...] = RegexGroup(),
-):
-    page = args[0] if len(args) > 0 and args[0] else 1
-    page = int(page)
-    msg = None
-    if not scheduler:
-        msg = Text("未安装软依赖nonebot_plugin_apscheduler，不能使用此功能")
-    else:
-        msg = Text(get_jobs_info(page))
-    
-    await sendReply(msg, target)
-    
-@backup_matcher.handle()
-async def backup_matcher_handle(
-    target: SaaTarget
-):
-    try:
-        res = await backup(CONFIG, plugin_config.reminder_bk_size)
-    except Exception as e:
-        res = f"备份失败: {e}"
-    msg = Text(res)
-    
-    await sendReply(msg, target)
-
-@backup_list_matcher.handle()
-async def backup_matcher_handle(
-    target: SaaTarget,
-    args: Tuple[Optional[int], ...] = RegexGroup()
-):
-    page = args[0] if len(args) > 0 and args[0] else 1
-    page = int(page)
-    pageSize = plugin_config.reminder_page_size
-    try:
-        res = await list_backup(page_size=pageSize, page=page)
-    except Exception as e:
-        res = f"获取备份列表失败: {e}"
-    if(res is None or res == ""):
-        res = "没有备份"
-        
-    msg = Text(res)
-    await sendReply(msg, target)
-
-@backup_detail_mathcer.handle()
-async def backup_detail_matcher_handle(
-    target: SaaTarget,
-    args: Tuple[Optional[str], ...] = RegexGroup(),
-):
-    bkId = args[0] if args[0] else None
-    page = args[1] if len(args) > 1 and args[1] else 1
-    pageSize = plugin_config.reminder_page_size
-    
-    global CONFIG
-    try:
-        res = await detail_backup(bkId, page_size=pageSize, page=page)
-    except Exception as e:
-        res = f"获取备份失败: {e}"
-    msg = Text(res)
-    await sendReply(msg, target)
-
-@backup_recover_matcher.got("confirm", prompt="确定恢复备份？(y|n)")
-async def backup_recover_handle(
     bot: Bot,
-    event: Event,
-    matcher: Matcher,
-    target: SaaTarget,
-    confirm = ArgPlainText(),
-    args: Tuple[Optional[str], ...] = RegexGroup(),
+    event: MessageEvent,
+    matcher: Matcher
 ):
-    bkId = args[0] if args[0] else None
-
-    # 去掉前后的空白字符
-    confirm = confirm.strip().lower()
-    if(confirm != "y"):
-        await sendReply("取消操作",target)
-        return
+    # 创建StringIO对象作为重定向的目标
+    output = StringIO()
+    if not scheduler:
+        await matcher.finish("未安装软依赖nonebot_plugin_apscheduler，不能使用此功能")
+    # scheduler.print_jobs(out=output)
+    # msg = Message(output.getvalue())
+    msg = Message(get_jobs_info())
     
-    global CONFIG
-    try:
-        res = await recover(bkId)
-        CONFIG = get_datas()
-        await clearScheduler()
-        await recoverFromJson()
-    except Exception as e:
-        res = f"恢复备份失败: {e}"
-    msg = Text(res)
-    await sendReply(msg, target)
-
+    await sendReply(bot, matcher, event, msg)
 
-@clear_matcher.got("confirm", prompt="确定清除定时(y|n)")
+@clear_matcher.handle()
 async def clear_matcher_handle(
     bot: Bot,
-    event: Event,
-    matcher: Matcher,
-    target: SaaTarget,
-    confirm: str = ArgPlainText(),
+    event: MessageEvent,
+    matcher: Matcher
 ):
-    # 去掉前后的空白字符
-    confirm = confirm.strip().lower()
-    if(confirm != "y"):
-        await sendReply("取消操作",target)
-        return
-    
-    global CONFIG
     await clearScheduler()
-    CONFIG = clear_datas(CONFIG=CONFIG)
+    clear_datas(CONFIG=CONFIG)
     await save_datas(CONFIG=CONFIG)
-    logger.opt(colors=True).info(
-        f"保存配置: {CONFIG}"
-    )
-    CONFIG = get_datas()
-    await sendReply("已清空所有定时提醒",target)
+
+    await sendReply(bot, matcher, event, "已清空所有定时提醒")
 
 @turn_matcher.handle()
 async def _(
     bot: Bot,
-    target: SaaTarget,
-    event: Event,
+    event: MessageEvent,
     matcher: Matcher,
     args: Tuple[Optional[str], ...] = RegexGroup(),
 ):
     if not scheduler:
-        await sendReply("未安装软依赖nonebot_plugin_apscheduler，不能使用定时发送功能", target)
+        await sendReply(bot, matcher, event, "未安装软依赖nonebot_plugin_apscheduler，不能使用定时发送功能")
     mode = args[0]
     schId = args[1] if args[1] else None
     if(not schId):
-        await sendReply("请输入具体的id", target)
+        await sendReply(bot, matcher, event, "请输入具体的id")
     
     item = findJobFromJSONById(schId)
     if item is None:
-        await sendReply("未找到该id的定时提醒",target)
+        await sendReply(bot, matcher, event, "未找到该id的定时提醒")
         
     if mode == "开启":
         if item["status"] == 1:
-            await sendReply("该定时提醒已开启，无需重复开启",target)
+            await sendReply(bot, matcher, event, "该定时提醒已开启，无需重复开启")
         else:
             item["status"] = 1
     elif mode == "关闭":
         item["status"] = 0
         setScheduler(schId, 0)
     elif mode == "删除":
         CONFIG.pop(schId, {})
         await removeScheduler(schId)
     elif mode == "查看":
-        await sendReply(item2string(item),target)
+        await sendReply(bot, matcher, event, item2string(item))
     elif mode == "执行":
         job = scheduler.get_job(schId)
         if job:
             # 添加一个job并立即执行
             current_time = datetime.now()
 
             # 加上 10 秒
             new_time = current_time + timedelta(seconds=10)
             job.modify(next_run_time=new_time)
-            await sendReply(f"正在执行{schId}的定时提醒",target)
+            await sendReply(bot, matcher, event, f"正在执行{schId}的定时提醒")
             # new_job = scheduler.run_job(job, 'date', next_run_time=datetime.now())
                    
     await save_datas(CONFIG=CONFIG)
 
-async def post_scheduler(botId: str, target_dict: Dict, msg: str, judgeWorkDay: bool = False, url: str = None, useId: str = None):
+    await sendReply(bot, matcher, event, f"已成功{mode}{schId}的定时提醒")
+
+async def post_scheduler(botId: str, userId: int, groupId: int, msg: str, judgeWorkDay: bool = False, url: str = None, useId: str = None):
     logger.opt(colors=True).debug(
         f"执行任务<g>url: {url} msg:{msg}</g>"
     )
     if judgeWorkDay:
         if not is_workday(date.today()):
             logger.opt(colors=True).info(
                 f"今天不是工作日，不发送提醒"
             )
             return
+
+    msg_img = None
     if url is not None and url != "" and isUrlSupport(url):
-        msg_img = Image(url)
+        msg_img = MessageSegment.image(url)
         logger.opt(colors=True).debug(
             f"获取图片成功"
         )
-        msg = MessageFactory([msg, msg_img])
-    bot = None
-    try:
-        bot = get_bot(self_id=botId)
-    except:
-        logger.opt(colors=True).error(
-            f"botId: {botId} 未找到bot"
-        )
+        Message(msg_img)
+    
+    bot = get_bot(self_id=botId)
+    if(groupId > 0):
+        msg = Message(msg)
+        if userId > 0:
+            msg.append(MessageSegment.at(userId))
+        await bot.send_group_msg(group_id=groupId, message=msg)
+        if msg_img is not None:
+            await bot.send_group_msg(user_id=userId, message=msg_img)
         return
-        
+    
     logger.opt(colors=True).debug(
-        f"执行完成任务，发送给<g>target:{target_dict}</g>"
+        f"执行完成任务，发送给<g>userId: {userId} msg:{msg}</g>"
     )
-    target = buildTarget(target_dict)
     # 非循环的任务，执行后删除
     if useId is not None and useId != "":
-        removeScheduler(id=useId)
+        removeScheduler(id=userId)
         logger.opt(colors=True).debug(
             f"<y>执行完成任务{useId}，清除记录</y>"
         )
         CONFIG.pop(useId, {})
         await save_datas(CONFIG=CONFIG)
         
-    await sendToReply(msg= msg, bot = bot, target=target)
+    await bot.send_private_msg(user_id=userId, message=msg)
+    if msg_img is not None:
+        await bot.send_private_msg(user_id=userId, message=msg_img)
 
 
-async def addScheduler(botId: str, target: SaaTarget, time: str, data: str, repeat: str = 1, url: str = None, id=None):
+async def addScheduler(botId: str, time: str, data: str, userId: int , repeat: str = 1, url: str = None, groupId:int = 0, id=None, fn=None, fnParamsArrs=None):
     if scheduler:
-        logger.opt(colors=True).debug(
-            f"<y>target: {target} time:{time}</y>"
-        )
         ## 小时-分钟格式的时间提取出来
         hour, minute = time.split(":")
         logger.opt(colors=True).info(
             f"已设定于 <y>{str(hour).rjust(2, '0')}:{str(minute).rjust(2, '0')}</y> 定时发送提醒"
         )
         job = None
         plans = CONFIG
 
         useId = id if id else generateRandomId()
-        target_dict = target.dict()
+
         # 每天或工作日
         judgeWorkDay = False
         if repeat == '1' or repeat == '3':
             if repeat == '3':
                 judgeWorkDay = True
-            job = scheduler.add_job(
-                post_scheduler, "cron", hour=hour, minute=minute, id=useId, replace_existing=True, args=[botId, target_dict, data, judgeWorkDay, url]
-            )
+            if fn is not None:
+                job = scheduler.add_job(
+                    fn, "cron", hour=hour, minute=minute, id=useId, replace_existing=True, args=fnParamsArrs
+                )
+                # 不能保存job信息，因为请求天气的函数中matcher不支持序列化
+            else:
+                job = scheduler.add_job(
+                    post_scheduler, "cron", hour=hour, minute=minute, id=useId, replace_existing=True, args=[botId, userId, groupId, data, judgeWorkDay, url]
+                )
         
         # 某天
         else:
             # 检查date 格式是否符合 yyyy-mm-dd
             year = 1
             month = 1
             day = 1
@@ -484,22 +382,28 @@
                 date_object = datetime.strptime(repeat, '%Y-%m-%d')
                 year = date_object.year
                 month = date_object.month
                 day = date_object.day
             except ValueError:
                 return {"code": -1, "msg": f"日期格式错误，应为 yyyy-mm-dd，如 2021-01-01"}
             
-            job = scheduler.add_job(
-                post_scheduler, "date", run_date=datetime(int(year), int(month), int(day), int(hour), int(minute), 0), id=useId, \
-                    replace_existing=True,  args=[botId, target_dict, data, judgeWorkDay, url, useId]
-            )
+            if fn is not None:
+                job = scheduler.add_job(
+                    fn, "date", run_date=datetime(int(year), int(month), int(day), int(hour), int(minute), 0), id=useId, replace_existing=True, args=fnParamsArrs
+                )
+            else:
+                # 非循环任务
+                job = scheduler.add_job(
+                    post_scheduler, "date", run_date=datetime(int(year), int(month), int(day), int(hour), int(minute), 0), id=useId, \
+                        replace_existing=True,  args=[botId, userId, groupId, data, judgeWorkDay, url, useId]
+                )
 
         if job is not None:
             plans[job.id] = {"id": job.id, "bot":botId, "time": time, "data": data, \
-                "repeat": repeat, "target":target_dict, "url": url, "status": 1}
+                "repeat": repeat, "userId": userId, "groupId": groupId, "url": url, "status": 1, "type": "normal"}
             await save_datas(CONFIG=CONFIG)
             return {"code": 0, "msg": job.id}
             
 async def setScheduler(id: str, status: int = 1):
     if scheduler and isVaildId(id):
         if(status == 0):
             scheduler.pause_job(id)
@@ -512,32 +416,31 @@
     )
     if scheduler and isVaildId(id):
         try:
             scheduler.remove_job(id)
         except Exception as e:
             logger.opt(colors=True).debug(
                 f"删除定时任务出错，error: {e}"
-            )
+            )        
 async def clearScheduler():
     if scheduler:
         jobs = scheduler.get_jobs()
         if not jobs or len(jobs) == 0:
             return False
         for job in jobs:
             if isVaildId(job.id):
                 scheduler.remove_job(job.id)
 
 async def updateScheduler(item: Any):
     id = item["id"]
     botId = item["bot"]
-    target = buildTarget(item["target"])
-    return await addScheduler(botId, target, item["time"], item["data"], item["repeat"], item["url"], id= id)
-    
-def buildTarget(target_dict: Dict):
-    return PlatformTarget.deserialize(target_dict);
+    if botId is None or botId == "":
+        return {"code": -1, "msg": f"找不到bot"}
+    return await addScheduler(botId, item["time"], item["data"], int(item["userId"]), item["repeat"], item["url"], int(item["groupId"]), id= id)
+        
 def generateRandomId():
     characters = string.ascii_lowercase + string.digits
     random_id = plugin_config.reminder_id_prefix + '_' + ''.join(random.choices(characters, k=plugin_config.reminder_id_len))
     while checkIdExit(random_id):
         random_id = plugin_config.reminder_id_prefix + '_' + ''.join(random.choices(characters, k=plugin_config.reminder_id_len))
     return random_id
 
@@ -554,14 +457,41 @@
     # 判断url是否是图片
     image_extensions = ['.jpg', '.jpeg', '.png', '.gif', '.bmp']
     if url.lower().startswith('http') and any(url.lower().endswith(ext) for ext in image_extensions):
         return True
     else:
         return False
     
+def processGroupEvent(event: GroupMessageEvent, msg: Message = None):
+    userId = event.user_id
+    groupId = -1
+    if isinstance(event, GroupMessageEvent):
+        groupId = event.group_id
+    messageId = event.message_id
+    if msg is None:
+        msg = Message("")
+    if not isinstance(msg, Message):
+        msg = Message(msg)
+    if isinstance(event, GroupMessageEvent):
+        msg.append(MessageSegment.reply(messageId))
+        msg.append(MessageSegment.at(userId))
+    return userId, groupId, messageId, msg
+
+async def sendReply(bot: Bot, matcher: Matcher, event: GroupMessageEvent, msg: Message = None, finish = True):
+    #  处理群组消息
+    userId, groupId, messageId, msg = processGroupEvent(event, msg)
+    
+    if isinstance(event, GroupMessageEvent):
+        await bot.send_group_msg(group_id=groupId, message=msg)
+        msg = None
+        logger.opt(colors=True).info(
+            "<g>群组消息</g>"
+        )
+    if finish:
+        await matcher.finish(msg) 
 
 def findJobFromJSONById(id: str):
     if id in CONFIG:
         return CONFIG[id]
     return None
 
 def isVaildId(id: str):
@@ -583,21 +513,31 @@
             )
             return
     
     logger.opt(colors=True).info(
         f"初始化定时任务，尝试从json中恢复定时任务"
     )
     try:
+        notNormalIds = []
         for key in CONFIG:    
             item = CONFIG[key]
+            if('type' in item):
+                if item['type'] != 'normal':
+                    notNormalIds.append(item["id"])
+                    continue
+                
             res = await updateScheduler(item)
             if res is not None and res != "":
                 continue
             else:
                 raise Exception("回复定时任务：设置失败")
+        for id in notNormalIds:
+            CONFIG.pop(id, {})
+            await save_datas(CONFIG=CONFIG)
+            
         logger.opt(colors=True).info(
             f"<y>初始化定时任务完成</y>"
         )
         scheduler.print_jobs()
     except Exception as e:
         logger.error(f"尝试从json中恢复定时任务失败，error: {e}")
         raise e
@@ -615,28 +555,8 @@
             if isVaildId(job.id):
                 msg += "(本插件任务)"
             else:
                 msg += "(非本插件任务)"
             msg += f"jobId: {job.id} \n\
 trigger:{job.trigger} \n\
 下次运行时间: {job.next_run_time}\n"
-        return msg
-
-async def sendReply(msg: MessageSegmentFactory, target: PlatformTarget):
-    if(isinstance(msg, str)):
-        msg = Text(msg) 
-    if target and target.platform_type == targetTypes.get("qqGroup"):
-        await msg.send(reply=True, at_sender=True)
-    else:
-        await msg.send()
-async def sendToReply(msg: MessageSegmentFactory, bot: Bot, target: PlatformTarget, useId: str = None, messageId: str = None):
-    if(isinstance(msg, str)):
-        msg = Text(msg)
-    if(useId is not None):
-        mention = Mention(user_id=useId)
-        msg = MessageFactory([msg, mention])
-    if messageId is not None:
-        msg = MessageFactory([msg, Reply(message_id=messageId)])
-    if bot is None:
-        await msg.send_to(bot=get_bot(), target=target)
-    else:
-        await msg.send_to(bot=bot, target=target)
+        return msg
```

### Comparing `nonebot_plugin_reminder-0.3.1.post2/nonebot_plugin_reminder/config.py` & `nonebot_plugin_reminder-0.4.0/nonebot_plugin_reminder/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_reminder-0.3.1.post2/nonebot_plugin_reminder/data_utils.py` & `nonebot_plugin_reminder-0.4.0/nonebot_plugin_reminder/data_utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_reminder-0.3.1.post2/pyproject.toml` & `nonebot_plugin_reminder-0.4.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "nonebot-plugin-reminder"
-version = "0.3.1-2"
+version = "0.4.0"
 description = "This plugin can remind you not to forget something"
 authors = ["velor2012 <38395332+velor2012@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
+nonebot-adapter-onebot = "^2.3.1"
 chinese-calendar = "^1.9.0"
 nonebot2 = "^2.1.3"
 nonebot-plugin-apscheduler = "^0.3.0"
 nonebot-plugin-localstore = "^0.5.1"
-nonebot-plugin-send-anything-anywhere = "^0.5.0"
 aiofiles = "^23.2.1"
 ujson = "^5.9.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nonebot_plugin_reminder-0.3.1.post2/PKG-INFO` & `nonebot_plugin_reminder-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-reminder
-Version: 0.3.1.post2
+Version: 0.4.0
 Summary: This plugin can remind you not to forget something
 License: MIT
 Author: velor2012
 Author-email: 38395332+velor2012@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
 Requires-Dist: chinese-calendar (>=1.9.0,<2.0.0)
+Requires-Dist: nonebot-adapter-onebot (>=2.3.1,<3.0.0)
 Requires-Dist: nonebot-plugin-apscheduler (>=0.3.0,<0.4.0)
 Requires-Dist: nonebot-plugin-localstore (>=0.5.1,<0.6.0)
-Requires-Dist: nonebot-plugin-send-anything-anywhere (>=0.5.0,<0.6.0)
 Requires-Dist: nonebot2 (>=2.1.3,<3.0.0)
 Requires-Dist: ujson (>=5.9.0,<6.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/blob/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-reminder Version: 0.3.1.post2
-Summary: This plugin can remind you not to forget something License: MIT
-Author: velor2012 Author-email: 38395332+velor2012@users.noreply.github.com
-Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
+Metadata-Version: 2.1 Name: nonebot-plugin-reminder Version: 0.4.0 Summary:
+This plugin can remind you not to forget something License: MIT Author:
+velor2012 Author-email: 38395332+velor2012@users.noreply.github.com Requires-
+Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0) Requires-Dist: chinese-calendar
-(>=1.9.0,<2.0.0) Requires-Dist: nonebot-plugin-apscheduler (>=0.3.0,<0.4.0)
-Requires-Dist: nonebot-plugin-localstore (>=0.5.1,<0.6.0) Requires-Dist:
-nonebot-plugin-send-anything-anywhere (>=0.5.0,<0.6.0) Requires-Dist: nonebot2
+(>=1.9.0,<2.0.0) Requires-Dist: nonebot-adapter-onebot (>=2.3.1,<3.0.0)
+Requires-Dist: nonebot-plugin-apscheduler (>=0.3.0,<0.4.0) Requires-Dist:
+nonebot-plugin-localstore (>=0.5.1,<0.6.0) Requires-Dist: nonebot2
 (>=2.1.3,<3.0.0) Requires-Dist: ujson (>=5.9.0,<6.0.0) Description-Content-
 Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
  # nonebot-plugin-reminder _â¨ NoneBot æä»¶ç®åæè¿° â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_]
                                    [python]
 è¿æ¯ä¸ä¸ª nonebot2 æä»¶åº,
```

