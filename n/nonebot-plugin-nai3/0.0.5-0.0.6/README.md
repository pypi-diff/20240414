# Comparing `tmp/nonebot_plugin_nai3-0.0.5.tar.gz` & `tmp/nonebot_plugin_nai3-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_nai3-0.0.5.tar", max compression
+gzip compressed data, was "nonebot_plugin_nai3-0.0.6.tar", max compression
```

## Comparing `nonebot_plugin_nai3-0.0.5.tar` & `nonebot_plugin_nai3-0.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.0.5/LICENSE
--rw-r--r--   0        0        0     5445 2024-04-14 04:33:27.624889 nonebot_plugin_nai3-0.0.5/nonebot_plugin_nai3/__init__.py
--rw-r--r--   0        0        0      527 2024-04-14 04:33:00.118668 nonebot_plugin_nai3-0.0.5/nonebot_plugin_nai3/config.py
--rw-r--r--   0        0        0     1551 2024-04-13 15:11:02.114168 nonebot_plugin_nai3-0.0.5/nonebot_plugin_nai3/utils.py
--rw-r--r--   0        0        0      846 2024-04-14 04:33:40.173182 nonebot_plugin_nai3-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3981 2024-04-14 04:03:10.205762 nonebot_plugin_nai3-0.0.5/README.md
--rw-r--r--   0        0        0     4485 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-04-13 00:11:40.913503 nonebot_plugin_nai3-0.0.6/LICENSE
+-rw-r--r--   0        0        0     5449 2024-04-14 04:35:27.021468 nonebot_plugin_nai3-0.0.6/nonebot_plugin_nai3/__init__.py
+-rw-r--r--   0        0        0      527 2024-04-14 04:33:00.118668 nonebot_plugin_nai3-0.0.6/nonebot_plugin_nai3/config.py
+-rw-r--r--   0        0        0     1551 2024-04-13 15:11:02.114168 nonebot_plugin_nai3-0.0.6/nonebot_plugin_nai3/utils.py
+-rw-r--r--   0        0        0      846 2024-04-14 04:35:39.778372 nonebot_plugin_nai3-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3981 2024-04-14 04:03:10.205762 nonebot_plugin_nai3-0.0.6/README.md
+-rw-r--r--   0        0        0     4485 1970-01-01 00:00:00.000000 nonebot_plugin_nai3-0.0.6/PKG-INFO
```

### Comparing `nonebot_plugin_nai3-0.0.5/LICENSE` & `nonebot_plugin_nai3-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.0.5/nonebot_plugin_nai3/__init__.py` & `nonebot_plugin_nai3-0.0.6/nonebot_plugin_nai3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 __version__ = "0.0.4"
 
 __plugin_meta__ = PluginMetadata(
     name="nonebot-plugin-nai3",
     description="通过 NovelAI 生成图片",
     usage="通过 NovelAI 生成图片",
     homepage="https://github.com/zhulinyv/nonebot_plugin_nai3",
-    type="library",
+    type="application",
     supported_adapters={
         "~onebot.v11",
         "~onebot.v12",
     },
     config=Config,
     extra={
         "author": "zhulinyv",
```

### Comparing `nonebot_plugin_nai3-0.0.5/nonebot_plugin_nai3/config.py` & `nonebot_plugin_nai3-0.0.6/nonebot_plugin_nai3/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.0.5/nonebot_plugin_nai3/utils.py` & `nonebot_plugin_nai3-0.0.6/nonebot_plugin_nai3/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.0.5/pyproject.toml` & `nonebot_plugin_nai3-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-nai3"
-version = "0.0.5"
+version = "0.0.6"
 description = "通过 NovelAI 生成图片"
 authors = ["zhulinyv <zhulinyv2005@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_nai3"}]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_plugin_nai3-0.0.5/README.md` & `nonebot_plugin_nai3-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_nai3-0.0.5/PKG-INFO` & `nonebot_plugin_nai3-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-nai3
-Version: 0.0.5
+Version: 0.0.6
 Summary: 通过 NovelAI 生成图片
 License: MIT
 Author: zhulinyv
 Author-email: zhulinyv2005@outlook.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.0.5 Summary: éè¿
+Metadata-Version: 2.1 Name: nonebot-plugin-nai3 Version: 0.0.6 Summary: éè¿
 NovelAI çæå¾ç License: MIT Author: zhulinyv Author-email:
 zhulinyv2005@outlook.com Requires-Python: >=3.9,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.1,<0.25.0) Requires-Dist: nonebot-adapter-onebot
 (>=2.2.3,<3.0.0) Requires-Dist: nonebot2 (>=2.2.1,<3.0.0) Description-Content-
```

