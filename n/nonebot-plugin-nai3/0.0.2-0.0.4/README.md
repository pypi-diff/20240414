# Comparing `tmp/nonebot_plugin_nai3-0.0.2.tar.gz` & `tmp/nonebot_plugin_nai3-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nai3-0.0.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_nai3-0.0.4.tar", max compression
```

## Comparing `nonebot_plugin_nai3-0.0.2.tar` & `nonebot_plugin_nai3-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.0.2/LICENSE
--rw-r--r--   0        0        0     2210 2024-04-13 15:42:40.029877 nonebot_plugin_nai3-0.0.2/nonebot_plugin_nai3/__init__.py
--rw-r--r--   0        0        0      214 2024-04-13 15:11:01.050188 nonebot_plugin_nai3-0.0.2/nonebot_plugin_nai3/config.py
--rw-r--r--   0        0        0     1551 2024-04-13 15:11:02.114168 nonebot_plugin_nai3-0.0.2/nonebot_plugin_nai3/utils.py
--rw-r--r--   0        0        0      846 2024-04-13 15:44:22.140763 nonebot_plugin_nai3-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3217 2024-04-13 15:06:54.185038 nonebot_plugin_nai3-0.0.2/README.md
--rw-r--r--   0        0        0     3742 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.0.4/LICENSE
+-rw-r--r--   0        0        0     5383 2024-04-14 03:48:35.298066 nonebot_plugin_nai3-0.0.4/nonebot_plugin_nai3/__init__.py
+-rw-r--r--   0        0        0      559 2024-04-14 03:32:45.975587 nonebot_plugin_nai3-0.0.4/nonebot_plugin_nai3/config.py
+-rw-r--r--   0        0        0     1551 2024-04-13 15:11:02.114168 nonebot_plugin_nai3-0.0.4/nonebot_plugin_nai3/utils.py
+-rw-r--r--   0        0        0      846 2024-04-14 04:03:46.477744 nonebot_plugin_nai3-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3981 2024-04-14 04:03:10.205762 nonebot_plugin_nai3-0.0.4/README.md
+-rw-r--r--   0        0        0     4485 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.0.4/PKG-INFO
```

### Comparing `nonebot_plugin_nai3-0.0.2/LICENSE` & `nonebot_plugin_nai3-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.0.2/nonebot_plugin_nai3/utils.py` & `nonebot_plugin_nai3-0.0.4/nonebot_plugin_nai3/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.0.2/pyproject.toml` & `nonebot_plugin_nai3-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nai3"
-version = "0.0.2"
+version = "0.0.4"
 description = "通过 NovelAI 生成图片"
 authors = ["zhulinyv <zhulinyv2005@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_nai3"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_nai3-0.0.2/PKG-INFO` & `nonebot_plugin_nai3-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nai3
-Version: 0.0.2
+Version: 0.0.4
 Summary: 通过 NovelAI 生成图片
 License: MIT
 Author: zhulinyv
 Author-email: zhulinyv2005@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -81,37 +81,58 @@
 ## ⚙️ 配置
 
 在 nonebot2 项目的`.env`文件中添加下表中的必填配置
 
 | 配置项 | 必填 | 类型 | 默认值 | 说明 |
 |:-----:|:----:|:----:|:----:|:----:|
 | nai3_token | 是 | str | xxx | 请求头中必需的 token |
+| nai3_negative | 否 | str | nsfw,... | 负面提示词 |
+| nai3_limit | 否 | int | 10 | 每人最多生成次数 |
+| nai3_cooltime_group | 否 | int | 30 | 群聊画图冷却时间(单位: 秒) |
+| nai3_cooltime_user | 否 | int | 300 | 个人画图冷却时间(单位: 秒) |
 
 ⚠️ token 的获取:
 
 - 1.登录 https://novelai.net/login
 - 2.F12 打开控制台并切换到控制台
 - 3.输入 `console.log(JSON.parse(localStorage.session).auth_token)` 回车, 返回的字符串即为 token
 - ![e3756ce75c6f6850efa633dbaa3a5ae6](https://github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-446d-9401-e559628ad079)
 
 ## 🎉 使用
 
-| 指令 | 参数 | 示例 | 结果 |
-|:---:|:---:|:---:|:---:|
-| nai3 | prompt | nai3 1girl, loli, cute | ![img](./img/8356736520_None_None.png) |
+```
+指令: nai3/nai
+参数:
+    prompt          提示词(支持你喜欢的画风串), 默认: None
+    -n/--negative   负面提示词, 默认: nsfw,...
+    -r/--resolution 画布形状/分辨率, ["mb", "pc", "sq"] 三选一, 默认: mb
+    -s/--scale      提示词相关性, 默认: 5.0
+    -sm             sm, 默认: False
+    -smdyn          smdyn, 默认: False
+    --sampler       采样器, 默认: k_euler
+    --schedule      噪声计划表, 默认: native
+示例: nai3 1girl, loli, cute -r mb -s 5.0
+返回: 
+```
+
+![img](./img/1.png)
 
 ## 📖 待办
 
 + [x] 文生图
 + [ ] 图生图
-+ [ ] 自定义参数
++ [x] 自定义参数
 + [ ] 队列功能
-+ [ ] 冷却功能
-+ [ ] 上限功能
++ [x] 冷却功能
++ [x] 上限功能
 + [ ] 黑名单功能
++ [ ] 代理
++ [ ] R18 检测
++ [ ] 翻译
++ [ ] 帮助指令
 + [ ] ...
 
 ## 🤝 鸣谢
 
 本项目逐步迁移自 [Semi-Auto-NovelAI-to-Pixiv](https://github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.0.2 Summary: éè¿
+Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.0.4 Summary: éè¿
 NovelAI çæå¾ç License: MIT Author: zhulinyv Author-email:
 zhulinyv2005@outlook.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.2.3,<3.0.0) Requires-Dist: nonebot2 (>=2.2.1,<3.0.0) Description-Content-
@@ -23,21 +23,30 @@
 æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
 pip pip install nonebot-plugin-nai3 pdm pdm add nonebot-plugin-nai3 poetry
 poetry add nonebot-plugin-nai3 conda conda install nonebot-plugin-nai3 æå¼
 nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç `pyproject.toml` æä»¶, å¨ `[tool.nonebot]`
 é¨åè¿½å åå¥ plugins = ["nonebot_plugin_hoshino_sign"] ## âï¸ éç½®
 å¨ nonebot2 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹
 | å¿å¡« | ç±»å | é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:|:----:
-| | nai3_token | æ¯ | str | xxx | è¯·æ±å¤´ä¸­å¿éç token | â ï¸ token
-çè·å: - 1.ç»å½ https://novelai.net/login - 2.F12
-æå¼æ§å¶å°å¹¶åæ¢å°æ§å¶å° - 3.è¾å¥ `console.log(JSON.parse
-(localStorage.session).auth_token)` åè½¦, è¿åçå­ç¬¦ä¸²å³ä¸º token - !
-[e3756ce75c6f6850efa633dbaa3a5ae6](https://github.com/zhulinyv/Semi-Auto-
-NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-446d-9401-e559628ad079) ## ð
-ä½¿ç¨ | æä»¤ | åæ° | ç¤ºä¾ | ç»æ | |:---:|:---:|:---:|:---:| | nai3 |
-prompt | nai3 1girl, loli, cute | ![img](./img/8356736520_None_None.png) | ##
-ð å¾å + [x] æçå¾ + [ ] å¾çå¾ + [ ] èªå®ä¹åæ° + [ ]
-éååè½ + [ ] å·å´åè½ + [ ] ä¸éåè½ + [ ] é»åååè½ + [ ]
-... ## ð¤ é¸£è°¢ æ¬é¡¹ç®éæ­¥è¿ç§»èª [Semi-Auto-NovelAI-to-Pixiv](https:
-//github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv)
+| | nai3_token | æ¯ | str | xxx | è¯·æ±å¤´ä¸­å¿éç token | |
+nai3_negative | å¦ | str | nsfw,... | è´é¢æç¤ºè¯ | | nai3_limit | å¦ |
+int | 10 | æ¯äººæå¤çææ¬¡æ° | | nai3_cooltime_group | å¦ | int | 30 |
+ç¾¤èç»å¾å·å´æ¶é´(åä½: ç§) | | nai3_cooltime_user | å¦ | int | 300
+| ä¸ªäººç»å¾å·å´æ¶é´(åä½: ç§) | â ï¸ token çè·å: - 1.ç»å½
+https://novelai.net/login - 2.F12 æå¼æ§å¶å°å¹¶åæ¢å°æ§å¶å° -
+3.è¾å¥ `console.log(JSON.parse(localStorage.session).auth_token)` åè½¦,
+è¿åçå­ç¬¦ä¸²å³ä¸º token - ![e3756ce75c6f6850efa633dbaa3a5ae6](https://
+github.com/zhulinyv/Semi-Auto-NovelAI-to-Pixiv/assets/66541860/502c9a49-6a73-
+446d-9401-e559628ad079) ## ð ä½¿ç¨ ``` æä»¤: nai3/nai åæ°: prompt
+æç¤ºè¯(æ¯æä½ åæ¬¢çç»é£ä¸²), é»è®¤: None -n/--negative
+è´é¢æç¤ºè¯, é»è®¤: nsfw,... -r/--resolution ç»å¸å½¢ç¶/åè¾¨ç,
+["mb", "pc", "sq"] ä¸éä¸, é»è®¤: mb -s/--scale æç¤ºè¯ç¸å³æ§, é»è®¤:
+5.0 -sm sm, é»è®¤: False -smdyn smdyn, é»è®¤: False --sampler éæ ·å¨,
+é»è®¤: k_euler --schedule åªå£°è®¡åè¡¨, é»è®¤: native ç¤ºä¾: nai3 1girl,
+loli, cute -r mb -s 5.0 è¿å: ``` ![img](./img/1.png) ## ð å¾å + [x]
+æçå¾ + [ ] å¾çå¾ + [x] èªå®ä¹åæ° + [ ] éååè½ + [x]
+å·å´åè½ + [x] ä¸éåè½ + [ ] é»åååè½ + [ ] ä»£ç + [ ] R18
+æ£æµ + [ ] ç¿»è¯ + [ ] å¸®å©æä»¤ + [ ] ... ## ð¤ é¸£è°¢
+æ¬é¡¹ç®éæ­¥è¿ç§»èª [Semi-Auto-NovelAI-to-Pixiv](https://github.com/
+zhulinyv/Semi-Auto-NovelAI-to-Pixiv)
 ===============================================================================
 [https://count.getloli.com/get/@zhulinyv?theme=rule34]
```

