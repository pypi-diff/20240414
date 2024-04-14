# Comparing `tmp/nonebot_plugin_nai3-0.0.1.tar.gz` & `tmp/nonebot_plugin_nai3-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nai3-0.0.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_nai3-0.0.2.tar", max compression
```

## Comparing `nonebot_plugin_nai3-0.0.1.tar` & `nonebot_plugin_nai3-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.0.1/LICENSE
--rw-r--r--   0        0        0     1724 2024-04-13 15:10:59.474261 nonebot_plugin_nai3-0.0.1/nonebot_plugin_nai3/__init__.py
--rw-r--r--   0        0        0      214 2024-04-13 15:11:01.050188 nonebot_plugin_nai3-0.0.1/nonebot_plugin_nai3/config.py
--rw-r--r--   0        0        0     1551 2024-04-13 15:11:02.114168 nonebot_plugin_nai3-0.0.1/nonebot_plugin_nai3/utils.py
--rw-r--r--   0        0        0      811 2024-04-13 15:10:56.870184 nonebot_plugin_nai3-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     3217 2024-04-13 15:06:54.185038 nonebot_plugin_nai3-0.0.1/README.md
--rw-r--r--   0        0        0     3687 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2210 2024-04-13 15:42:40.029877 nonebot_plugin_nai3-0.0.2/nonebot_plugin_nai3/__init__.py
+-rw-r--r--   0        0        0      214 2024-04-13 15:11:01.050188 nonebot_plugin_nai3-0.0.2/nonebot_plugin_nai3/config.py
+-rw-r--r--   0        0        0     1551 2024-04-13 15:11:02.114168 nonebot_plugin_nai3-0.0.2/nonebot_plugin_nai3/utils.py
+-rw-r--r--   0        0        0      846 2024-04-13 15:44:22.140763 nonebot_plugin_nai3-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3217 2024-04-13 15:06:54.185038 nonebot_plugin_nai3-0.0.2/README.md
+-rw-r--r--   0        0        0     3742 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.0.2/PKG-INFO
```

### Comparing `nonebot_plugin_nai3-0.0.1/LICENSE` & `nonebot_plugin_nai3-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.0.1/nonebot_plugin_nai3/__init__.py` & `nonebot_plugin_nai3-0.0.2/nonebot_plugin_nai3/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,17 +2,37 @@
 import random
 import zipfile
 
 from httpx import AsyncClient
 from nonebot import logger, on_command
 from nonebot.adapters.onebot.v11 import Message, MessageSegment
 from nonebot.params import CommandArg
+from nonebot.plugin import PluginMetadata
 
 from .utils import headers, json_for_t2i
 
+__version__ = "0.0.2"
+
+__plugin_meta__ = PluginMetadata(
+    name="nonebot-plugin-nai3",
+    description="通过 NovelAI 生成图片",
+    usage="通过 NovelAI 生成图片",
+    homepage="https://github.com/zhulinyv/nonebot_plugin_nai3",
+    type="library",
+    supported_adapters={
+        "~onebot.v11",
+        "~onebot.v12",
+    },
+    extra={
+        "author": "zhulinyv",
+        "version": __version__,
+    },
+)
+
+
 nai3 = on_command("nai3", aliases={"nai"}, priority=30, block=True)
 
 
 @nai3.handle()
 async def _(msg: Message = CommandArg()):
     prompt = msg.extract_plain_text().strip()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_plugin_nai3-0.0.1/nonebot_plugin_nai3/utils.py` & `nonebot_plugin_nai3-0.0.2/nonebot_plugin_nai3/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.0.1/pyproject.toml` & `nonebot_plugin_nai3-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "nonebot-plugin-nai3"
-version = "0.0.1"
+version = "0.0.2"
 description = "通过 NovelAI 生成图片"
 authors = ["zhulinyv <zhulinyv2005@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_nai3"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 nonebot2 = "^2.2.1"
 httpx = "^0.24.1"
+nonebot-adapter-onebot = "^2.2.3"
 
 # https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html
 [tool.black]
 line-length = 500
 
 # https://beta.ruff.rs/docs/settings/
 [tool.ruff]
```

### Comparing `nonebot_plugin_nai3-0.0.1/README.md` & `nonebot_plugin_nai3-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.0.1/PKG-INFO` & `nonebot_plugin_nai3-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nai3
-Version: 0.0.1
+Version: 0.0.2
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
+Requires-Dist: nonebot-adapter-onebot (>=2.2.3,<3.0.0)
 Requires-Dist: nonebot2 (>=2.2.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/A-kirami/nonebot-plugin-template/raw/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/A-kirami/nonebot-plugin-template/raw/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.0.1 Summary: éè¿
+Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.0.2 Summary: éè¿
 NovelAI çæå¾ç License: MIT Author: zhulinyv Author-email:
 zhulinyv2005@outlook.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist: nonebot2
-(>=2.2.1,<3.0.0) Description-Content-Type: text/markdown
+Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist: nonebot-adapter-onebot
+(>=2.2.3,<3.0.0) Requires-Dist: nonebot2 (>=2.2.1,<3.0.0) Description-Content-
+Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
                        ************ nnoonneebboott__pplluuggiinn__nnaaii33 ************
                    ****** ?â??¨?é???è?¿? NNoovveellAAII ?ç???æ???å??¾?ç???â??¨ ******
        [https://img.shields.io/badge/Python-3.9+-blue]_[_l_i_c_e_n_s_e_][https://
       img.shields.io/github/issues/zhulinyv/nonebot_plugin_nai3][https://
       img.shields.io/github/stars/zhulinyv/nonebot_plugin_nai3][https://
```

