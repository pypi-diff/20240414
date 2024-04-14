# Comparing `tmp/nonebot_plugin_ghtiles-0.1.3.tar.gz` & `tmp/nonebot_plugin_ghtiles-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ghtiles-0.1.3.tar", last modified: Sun Apr  7 09:32:20 2024, max compression
+gzip compressed data, was "nonebot_plugin_ghtiles-0.1.4.tar", last modified: Sun Apr 14 14:27:40 2024, max compression
```

## Comparing `nonebot_plugin_ghtiles-0.1.3.tar` & `nonebot_plugin_ghtiles-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2024-04-07 09:32:07.684982 nonebot_plugin_ghtiles-0.1.3/LICENSE
--rw-r--r--   0        0        0     3002 2024-04-07 09:32:07.684982 nonebot_plugin_ghtiles-0.1.3/README.md
--rw-r--r--   0        0        0     7248 2024-04-07 09:32:07.684982 nonebot_plugin_ghtiles-0.1.3/nonebot_plugin_ghtiles/__init__.py
--rw-r--r--   0        0        0      241 2024-04-07 09:32:07.684982 nonebot_plugin_ghtiles-0.1.3/nonebot_plugin_ghtiles/config.py
--rw-r--r--   0        0        0     2303 2024-04-07 09:32:07.684982 nonebot_plugin_ghtiles-0.1.3/nonebot_plugin_ghtiles/utils.py
--rw-r--r--   0        0        0     1172 2024-04-07 09:32:20.524912 nonebot_plugin_ghtiles-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 nonebot_plugin_ghtiles-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-14 14:27:21.998700 nonebot_plugin_ghtiles-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3000 2024-04-14 14:27:21.998700 nonebot_plugin_ghtiles-0.1.4/README.md
+-rw-r--r--   0        0        0     8578 2024-04-14 14:27:21.998700 nonebot_plugin_ghtiles-0.1.4/nonebot_plugin_ghtiles/__init__.py
+-rw-r--r--   0        0        0      241 2024-04-14 14:27:21.998700 nonebot_plugin_ghtiles-0.1.4/nonebot_plugin_ghtiles/config.py
+-rw-r--r--   0        0        0     2298 2024-04-14 14:27:21.998700 nonebot_plugin_ghtiles-0.1.4/nonebot_plugin_ghtiles/utils.py
+-rw-r--r--   0        0        0     1172 2024-04-14 14:27:40.250859 nonebot_plugin_ghtiles-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3750 1970-01-01 00:00:00.000000 nonebot_plugin_ghtiles-0.1.4/PKG-INFO
```

### Comparing `nonebot_plugin_ghtiles-0.1.3/LICENSE` & `nonebot_plugin_ghtiles-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ghtiles-0.1.3/README.md` & `nonebot_plugin_ghtiles-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分的 `plugins` 项里追加写入
 
 ```toml
 [tool.nonebot]
 plugins = [
     # ...
-    "nonebot_plugin_picstatus"
+    "nonebot_plugin_ghtiles"
 ]
 ```
 
 </details>
 
 ## ⚙️ 配置
 
@@ -120,15 +120,15 @@
 
 查看你的 GitHub 瓷砖
 
 #### `tile.bind <username>`
 
 绑定你的 GitHub 用户名
 
-#### `tile.remine`
+#### `tile.remind`
 
 创建一个提醒，当这一天即将过去而你还没有提交时，会提醒你
 
 ## 💡 鸣谢
 
 ### [nonebot/plugin-alconna](https://github.com/nonebot/plugin-alconna)
```

#### html2text {}

```diff
@@ -10,16 +10,16 @@
 ``` ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip ```bash pip install nonebot-plugin-ghtiles ``` pdm ```bash pdm add nonebot-
 plugin-ghtiles ``` poetry ```bash poetry add nonebot-plugin-ghtiles ``` conda
 ```bash conda install nonebot-plugin-ghtiles ``` æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
-"nonebot_plugin_picstatus" ] ``` ## âï¸ éç½® #### `ght_proxy` -
-**ç±»å**: `str` - **é»è®¤å¼**: `"https://github.com"` GitHub
+"nonebot_plugin_ghtiles" ] ``` ## âï¸ éç½® #### `ght_proxy` - **ç±»å**:
+`str` - **é»è®¤å¼**: `"https://github.com"` GitHub
 å°åï¼å¦æéè¦è§£å³å½åè®¿é® GitHub
 çé®é¢ï¼å¯ä»¥æ¿æ¢ä¸ºéåç«ç¹ ## ð ä½¿ç¨ ### æä»¤ #### `tile`
 æ¥çä½ ç GitHub ç·ç  #### `tile.bind ` ç»å®ä½ ç GitHub ç¨æ·å ####
-`tile.remine`
+`tile.remind`
 åå»ºä¸ä¸ªæéï¼å½è¿ä¸å¤©å³å°è¿å»èä½ è¿æ²¡ææäº¤æ¶ï¼ä¼æéä½ 
 ## ð¡ é¸£è°¢ ### [nonebot/plugin-alconna](https://github.com/nonebot/plugin-
 alconna) - å¼ºå¤§çå½ä»¤è§£æåºï¼åå¤å¹³å°ééæ¹æ¡
```

### Comparing `nonebot_plugin_ghtiles-0.1.3/nonebot_plugin_ghtiles/__init__.py` & `nonebot_plugin_ghtiles-0.1.4/nonebot_plugin_ghtiles/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -197,14 +197,31 @@
     user_info["username"] = username
     users_copy[user_id] = user_info
 
     _data["users"] = users_copy
     logger.debug(f"binded username: {username} to user_id: {user_id}")
     return await UniMessage(f"绑定成功，你的 GitHub 用户名是 {username}").send(event)
 
+tile_unbind_cmd = (
+    Command("tile.unbind", "解绑 GitHub 用户名")
+    .alias("解绑")
+    .usage("tile.unbind, 解绑 GitHub 用户名")
+    .build()
+)
+
+@tile_unbind_cmd.handle()
+async def tile_unbind_cmd_handle(event: Event, session: EventSession):
+    user_id = session.id1
+    if user_id not in _data["users"]:
+        return await UniMessage("你还没有绑定过 GitHub 用户名").send(event)
+    users_copy = _data["users"].copy()
+    del users_copy[user_id]
+    logger.debug(f"unbinded user_id: {user_id}")
+    return await UniMessage("解绑成功").send(event)
+
 
 tile_remine_cmd = (
     Command("tile.remind")
     .alias("创建提醒")
     .usage("tile.remind, 创建提醒，每天 23:30 发送")
     .build()
 )
@@ -223,7 +240,30 @@
     if user_id in on_reminder_updated[group_id]:
         return await UniMessage("你已经创建过提醒了").send(event)
 
     on_reminder_updated[group_id].append(user_id)
     _data["on_reminder"] = on_reminder_updated
     logger.debug(f"create reminder for user_id: {user_id} in group_id: {group_id}")
     return await UniMessage("创建提醒成功").send(event)
+
+
+tile_unremind_cmd = (
+    Command("tile.unremind")
+    .alias("取消提醒")
+    .usage("tile.unremind, 取消提醒")
+    .build()
+)
+
+@tile_unremind_cmd.handle()
+async def tile_unremind_cmd_handle(event: Event, session: EventSession):
+    user_id = session.id1
+    group_id = session.id2
+
+    on_reminder_updated = _data["on_reminder"].copy()
+
+    if group_id not in on_reminder_updated or not on_reminder_updated[group_id]:
+        return await UniMessage("你还没有过创建提醒").send(event)
+
+    on_reminder_updated[group_id].remove(user_id)
+    _data["on_reminder"] = on_reminder_updated
+    logger.debug(f"cancel reminder for user_id: {user_id} in group_id: {group_id}")
+    return await UniMessage("取消提醒成功").send(event)
```

### Comparing `nonebot_plugin_ghtiles-0.1.3/nonebot_plugin_ghtiles/utils.py` & `nonebot_plugin_ghtiles-0.1.4/nonebot_plugin_ghtiles/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,16 @@
     async with httpx.AsyncClient() as client:
         response = await client.get(url, headers=headers)
         response.raise_for_status()
         return response.text
 
 
 async def check_contributions(gh_html: str) -> bool:
-    return re.compile(r"\'s activity is private\<\/h2\>").search(gh_html) is None
+    soup = BeautifulSoup(gh_html, "html.parser")
+    return bool(soup.tbody)
 
 
 async def get_today_contributions(gh_html: str) -> int:
     soup = BeautifulSoup(gh_html, "html.parser")
     contributions = 0
     if soup.tbody is None:
         return contributions
```

### Comparing `nonebot_plugin_ghtiles-0.1.3/pyproject.toml` & `nonebot_plugin_ghtiles-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-ghtiles"
-version = "0.1.3"
+version = "0.1.4"
 description = "A nonebot2 plugin for show GitHub contributions"
 readme = "README.md"
 requires-python = ">=3.9, <4.0"
 dependencies = [
     "nonebot2>=2.2.0",
     "httpx~=0.27",
     "nonebot-plugin-alconna>=0.38.1",
```

### Comparing `nonebot_plugin_ghtiles-0.1.3/PKG-INFO` & `nonebot_plugin_ghtiles-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-ghtiles
-Version: 0.1.3
+Version: 0.1.4
 Summary: A nonebot2 plugin for show GitHub contributions
 Home-page: https://github.com/Lipraty/nonebot-plugin-ghtiles
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/Lipraty/nonebot-plugin-ghtiles
 Requires-Python: <4.0,>=3.9
@@ -112,15 +112,15 @@
 
 打开 nonebot2 项目根目录下的 `pyproject.toml` 文件, 在 `[tool.nonebot]` 部分的 `plugins` 项里追加写入
 
 ```toml
 [tool.nonebot]
 plugins = [
     # ...
-    "nonebot_plugin_picstatus"
+    "nonebot_plugin_ghtiles"
 ]
 ```
 
 </details>
 
 ## ⚙️ 配置
 
@@ -139,15 +139,15 @@
 
 查看你的 GitHub 瓷砖
 
 #### `tile.bind <username>`
 
 绑定你的 GitHub 用户名
 
-#### `tile.remine`
+#### `tile.remind`
 
 创建一个提醒，当这一天即将过去而你还没有提交时，会提醒你
 
 ## 💡 鸣谢
 
 ### [nonebot/plugin-alconna](https://github.com/nonebot/plugin-alconna)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-ghtiles Version: 0.1.3 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-ghtiles Version: 0.1.4 Summary: A
 nonebot2 plugin for show GitHub contributions Home-page: https://github.com/
 Lipraty/nonebot-plugin-ghtiles Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Project-URL: Homepage, https://github.com/Lipraty/nonebot-
 plugin-ghtiles Requires-Python: <4.0,>=3.9 Requires-Dist: nonebot2>=2.2.0
 Requires-Dist: httpx~=0.27 Requires-Dist: nonebot-plugin-alconna>=0.38.1
 Requires-Dist: nonebot-plugin-apscheduler~=0.4 Requires-Dist: nonebot-plugin-
@@ -20,16 +20,16 @@
 ``` ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip ```bash pip install nonebot-plugin-ghtiles ``` pdm ```bash pdm add nonebot-
 plugin-ghtiles ``` poetry ```bash poetry add nonebot-plugin-ghtiles ``` conda
 ```bash conda install nonebot-plugin-ghtiles ``` æå¼ nonebot2
 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç
 `plugins` é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
-"nonebot_plugin_picstatus" ] ``` ## âï¸ éç½® #### `ght_proxy` -
-**ç±»å**: `str` - **é»è®¤å¼**: `"https://github.com"` GitHub
+"nonebot_plugin_ghtiles" ] ``` ## âï¸ éç½® #### `ght_proxy` - **ç±»å**:
+`str` - **é»è®¤å¼**: `"https://github.com"` GitHub
 å°åï¼å¦æéè¦è§£å³å½åè®¿é® GitHub
 çé®é¢ï¼å¯ä»¥æ¿æ¢ä¸ºéåç«ç¹ ## ð ä½¿ç¨ ### æä»¤ #### `tile`
 æ¥çä½ ç GitHub ç·ç  #### `tile.bind ` ç»å®ä½ ç GitHub ç¨æ·å ####
-`tile.remine`
+`tile.remind`
 åå»ºä¸ä¸ªæéï¼å½è¿ä¸å¤©å³å°è¿å»èä½ è¿æ²¡ææäº¤æ¶ï¼ä¼æéä½ 
 ## ð¡ é¸£è°¢ ### [nonebot/plugin-alconna](https://github.com/nonebot/plugin-
 alconna) - å¼ºå¤§çå½ä»¤è§£æåºï¼åå¤å¹³å°ééæ¹æ¡
```

