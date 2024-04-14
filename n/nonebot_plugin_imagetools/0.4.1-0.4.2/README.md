# Comparing `tmp/nonebot_plugin_imagetools-0.4.1.tar.gz` & `tmp/nonebot_plugin_imagetools-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_imagetools-0.4.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_imagetools-0.4.2.tar", max compression
```

## Comparing `nonebot_plugin_imagetools-0.4.1.tar` & `nonebot_plugin_imagetools-0.4.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1063 2024-03-12 09:52:38.301013 nonebot_plugin_imagetools-0.4.1/LICENSE
--rw-r--r--   0        0        0     2223 2024-03-12 09:52:38.301013 nonebot_plugin_imagetools-0.4.1/README.md
--rw-r--r--   0        0        0     3938 2024-03-12 09:52:38.301013 nonebot_plugin_imagetools-0.4.1/nonebot_plugin_imagetools/__init__.py
--rw-r--r--   0        0        0     6839 2024-03-12 09:52:38.301013 nonebot_plugin_imagetools-0.4.1/nonebot_plugin_imagetools/color_table.py
--rw-r--r--   0        0        0      276 2024-03-12 09:52:38.301013 nonebot_plugin_imagetools-0.4.1/nonebot_plugin_imagetools/config.py
--rw-r--r--   0        0        0     1593 2024-03-12 09:52:38.301013 nonebot_plugin_imagetools-0.4.1/nonebot_plugin_imagetools/data_source.py
--rw-r--r--   0        0        0     2199 2024-03-12 09:52:38.301013 nonebot_plugin_imagetools-0.4.1/nonebot_plugin_imagetools/depends.py
--rw-r--r--   0        0        0    11131 2024-03-12 09:52:38.301013 nonebot_plugin_imagetools-0.4.1/nonebot_plugin_imagetools/functions.py
--rw-r--r--   0        0        0     3089 2024-03-12 09:52:38.301013 nonebot_plugin_imagetools-0.4.1/nonebot_plugin_imagetools/utils.py
--rw-r--r--   0        0        0      899 2024-03-12 09:52:38.301013 nonebot_plugin_imagetools-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3183 1970-01-01 00:00:00.000000 nonebot_plugin_imagetools-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-14 08:17:04.049036 nonebot_plugin_imagetools-0.4.2/LICENSE
+-rw-r--r--   0        0        0     3185 2024-04-14 08:17:04.049036 nonebot_plugin_imagetools-0.4.2/README.md
+-rw-r--r--   0        0        0     7858 2024-04-14 08:17:04.049036 nonebot_plugin_imagetools-0.4.2/nonebot_plugin_imagetools/__init__.py
+-rw-r--r--   0        0        0     6839 2024-04-14 08:17:04.049036 nonebot_plugin_imagetools-0.4.2/nonebot_plugin_imagetools/color_table.py
+-rw-r--r--   0        0        0      856 2024-04-14 08:17:04.049036 nonebot_plugin_imagetools-0.4.2/nonebot_plugin_imagetools/config.py
+-rw-r--r--   0        0        0     1593 2024-04-14 08:17:04.049036 nonebot_plugin_imagetools-0.4.2/nonebot_plugin_imagetools/data_source.py
+-rw-r--r--   0        0        0     2249 2024-04-14 08:17:04.049036 nonebot_plugin_imagetools-0.4.2/nonebot_plugin_imagetools/depends.py
+-rw-r--r--   0        0        0    11168 2024-04-14 08:17:04.049036 nonebot_plugin_imagetools-0.4.2/nonebot_plugin_imagetools/functions.py
+-rw-r--r--   0        0        0     3089 2024-04-14 08:17:04.049036 nonebot_plugin_imagetools-0.4.2/nonebot_plugin_imagetools/utils.py
+-rw-r--r--   0        0        0      933 2024-04-14 08:17:04.049036 nonebot_plugin_imagetools-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     4145 1970-01-01 00:00:00.000000 nonebot_plugin_imagetools-0.4.2/PKG-INFO
```

### Comparing `nonebot_plugin_imagetools-0.4.1/LICENSE` & `nonebot_plugin_imagetools-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_imagetools-0.4.1/README.md` & `nonebot_plugin_imagetools-0.4.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -26,18 +26,44 @@
 ```
 DRIVER=~fastapi+~httpx+~websockets
 ```
 
 
 ### 配置项
 
-#### `imagetools_zip_threshold`
+#### `imagetools_multiple_image_config`
+ - 类型：[MultipleImageConfig](https://github.com/noneplugin/nonebot-plugin-imagetools/blob/main/nonebot_plugin_imagetools/config.py)
+ - 说明：输出多张图片时的发送方式
+
+`MultipleImageConfig` 中的具体配置项：
+
+##### `send_one_by_one`
+ - 类型：`bool`
+ - 默认：`False`
+ - 说明：是否逐个发送图片，默认为 `False`，即一次性发送所有图片
+
+##### `direct_send_threshold`
  - 类型：`int`
- - 默认：`20`
- - 说明：输出图片数量大于该数目时，打包为zip文件并上传
+ - 默认：`10`
+ - 说明：输出图片数量大于该数目时，不再直接发送，视配置以文件或合并转发消息的形式发送
+
+##### `send_zip_file`
+ - 类型：`bool`
+ - 默认：`True`
+ - 说明：输出图片数量大于 `direct_send_threshold` 时，是否打包为zip以文件形式发送
+
+##### `send_forward_msg`
+ - 类型：`bool`
+ - 默认：`False`
+ - 说明：输出图片数量大于 `direct_send_threshold` 时，是否发送合并转发消息
+
+配置示例：
+```
+imagetools_multiple_image_config={"send_one_by_one":false,"direct_send_threshold":10,"send_zip_file":true,"send_forward_msg":true}
+```
 
 
 > [!NOTE]
 >
 > 本插件使用 [nonebot-plugin-alconna](https://github.com/nonebot/plugin-alconna) 插件来发送图片和文件，具体支持的平台和行为请参考该插件的文档
```

### Comparing `nonebot_plugin_imagetools-0.4.1/nonebot_plugin_imagetools/color_table.py` & `nonebot_plugin_imagetools-0.4.2/nonebot_plugin_imagetools/color_table.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_imagetools-0.4.1/nonebot_plugin_imagetools/data_source.py` & `nonebot_plugin_imagetools-0.4.2/nonebot_plugin_imagetools/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_imagetools-0.4.1/nonebot_plugin_imagetools/depends.py` & `nonebot_plugin_imagetools-0.4.2/nonebot_plugin_imagetools/depends.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,19 +17,22 @@
     async def dependency(
         bot: Bot, event: Event, state: T_State, msg: Message = CommandArg()
     ):
         imgs: List[bytes] = []
 
         uni_msg = UniMessage()
         if msg:
-            uni_msg = await UniMessage.generate(message=msg)
+            uni_msg = UniMessage.generate_without_reply(message=msg)
         uni_msg_with_reply = UniMessage()
-        if reply := await reply_fetch(event, bot):
-            if reply.msg and isinstance(reply.msg, Message):
-                uni_msg_with_reply = await UniMessage.generate(message=reply.msg)
+        if (
+            (reply := await reply_fetch(event, bot))
+            and reply.msg
+            and isinstance(reply.msg, Message)
+        ):
+            uni_msg_with_reply = UniMessage.generate_without_reply(message=reply.msg)
         uni_msg_with_reply.extend(uni_msg)
 
         for seg in uni_msg_with_reply:
             if isinstance(seg, Image):
                 try:
                     result = await image_fetch(
                         bot=bot, event=event, state=state, img=seg
```

### Comparing `nonebot_plugin_imagetools-0.4.1/nonebot_plugin_imagetools/functions.py` & `nonebot_plugin_imagetools-0.4.2/nonebot_plugin_imagetools/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,21 +219,22 @@
 
 
 def gif_change_fps(img: BuildImage = Img(), arg: str = Arg()):
     image = img.image
     if not getattr(image, "is_animated", False):
         return
     duration = get_avg_duration(image) / 1000
-    if match := re.fullmatch(r"([\d\.]{1,4})(?:x|X|倍速?)", arg):
+    p_float = r"\d{0,3}\.?\d{1,3}"
+    if match := re.fullmatch(rf"({p_float})(?:x|X|倍速?)", arg):
         duration /= float(match.group(1))
-    elif match := re.fullmatch(r"(\d{1,3})%", arg):
-        duration /= int(match.group(1)) / 100
-    elif match := re.fullmatch(r"(\d+(\.\d+)?)fps", arg, re.I):
+    elif match := re.fullmatch(rf"({p_float})%", arg):
+        duration /= float(match.group(1)) / 100
+    elif match := re.fullmatch(rf"({p_float})fps", arg, re.I):
         duration = 1 / float(match.group(1))
-    elif match := re.fullmatch(r"(\d+(\.\d+)?)(m?)s", arg, re.I):
+    elif match := re.fullmatch(rf"({p_float})(m?)s", arg, re.I):
         duration = (
             float(match.group(1)) / 1000 if match.group(2) else float(match.group(1))
         )
     else:
         return "请使用正确的倍率格式，如：0.5x、50%、20FPS、0.05s"
     if duration < 0.02:
         return (
```

### Comparing `nonebot_plugin_imagetools-0.4.1/nonebot_plugin_imagetools/utils.py` & `nonebot_plugin_imagetools-0.4.2/nonebot_plugin_imagetools/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_imagetools-0.4.1/pyproject.toml` & `nonebot_plugin_imagetools-0.4.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_imagetools"
-version = "0.4.1"
+version = "0.4.2"
 description = "Nonebot2 简单图片操作插件"
 authors = ["meetwq <meetwq@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/noneplugin/nonebot-plugin-imagetools"
 repository = "https://github.com/noneplugin/nonebot-plugin-imagetools"
 
@@ -13,14 +13,15 @@
 nonebot2 = "^2.2.0"
 nonebot-plugin-alconna = ">=0.40.1,<1.0.0"
 httpx = ">=0.20.0,<1.0.0"
 Pillow = "^10.0.0"
 pil-utils = "^0.1.8"
 
 [tool.poetry.group.dev.dependencies]
+nonebot-adapter-onebot = "^2.2.0"
 
 [tool.pyright]
 pythonVersion = "3.8"
 pythonPlatform = "All"
 typeCheckingMode = "basic"
 
 [tool.ruff]
```

### Comparing `nonebot_plugin_imagetools-0.4.1/PKG-INFO` & `nonebot_plugin_imagetools-0.4.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_imagetools
-Version: 0.4.1
+Version: 0.4.2
 Summary: Nonebot2 简单图片操作插件
 Home-page: https://github.com/noneplugin/nonebot-plugin-imagetools
 License: MIT
 Author: meetwq
 Author-email: meetwq@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -50,18 +50,44 @@
 ```
 DRIVER=~fastapi+~httpx+~websockets
 ```
 
 
 ### 配置项
 
-#### `imagetools_zip_threshold`
+#### `imagetools_multiple_image_config`
+ - 类型：[MultipleImageConfig](https://github.com/noneplugin/nonebot-plugin-imagetools/blob/main/nonebot_plugin_imagetools/config.py)
+ - 说明：输出多张图片时的发送方式
+
+`MultipleImageConfig` 中的具体配置项：
+
+##### `send_one_by_one`
+ - 类型：`bool`
+ - 默认：`False`
+ - 说明：是否逐个发送图片，默认为 `False`，即一次性发送所有图片
+
+##### `direct_send_threshold`
  - 类型：`int`
- - 默认：`20`
- - 说明：输出图片数量大于该数目时，打包为zip文件并上传
+ - 默认：`10`
+ - 说明：输出图片数量大于该数目时，不再直接发送，视配置以文件或合并转发消息的形式发送
+
+##### `send_zip_file`
+ - 类型：`bool`
+ - 默认：`True`
+ - 说明：输出图片数量大于 `direct_send_threshold` 时，是否打包为zip以文件形式发送
+
+##### `send_forward_msg`
+ - 类型：`bool`
+ - 默认：`False`
+ - 说明：输出图片数量大于 `direct_send_threshold` 时，是否发送合并转发消息
+
+配置示例：
+```
+imagetools_multiple_image_config={"send_one_by_one":false,"direct_send_threshold":10,"send_zip_file":true,"send_forward_msg":true}
+```
 
 
 > [!NOTE]
 >
 > 本插件使用 [nonebot-plugin-alconna](https://github.com/nonebot/plugin-alconna) 插件来发送图片和文件，具体支持的平台和行为请参考该插件的文档
```

