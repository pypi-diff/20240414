# Comparing `tmp/nonebot_adapter_minecraft-1.1.0.tar.gz` & `tmp/nonebot_adapter_minecraft-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_adapter_minecraft-1.1.0.tar", max compression
+gzip compressed data, was "nonebot_adapter_minecraft-1.1.1.tar", max compression
```

## Comparing `nonebot_adapter_minecraft-1.1.0.tar` & `nonebot_adapter_minecraft-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1065 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/LICENSE
--rw-r--r--   0        0        0     1693 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/README.md
--rw-r--r--   0        0        0      386 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/__init__.py
--rw-r--r--   0        0        0     8733 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/adapter.py
--rw-r--r--   0        0        0     2317 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/bot.py
--rw-r--r--   0        0        0     1165 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/bot.pyi
--rw-r--r--   0        0        0     3794 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/collator.py
--rw-r--r--   0        0        0      527 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/compat.py
--rw-r--r--   0        0        0      310 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/config.py
--rw-r--r--   0        0        0     1392 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/event/__init__.py
--rw-r--r--   0        0        0     3621 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/event/base.py
--rw-r--r--   0        0        0     1578 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/event/fabric.py
--rw-r--r--   0        0        0     1424 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/event/forge.py
--rw-r--r--   0        0        0      598 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/event/minecraft.py
--rw-r--r--   0        0        0     1818 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/event/spigot.py
--rw-r--r--   0        0        0     2138 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/exception.py
--rw-r--r--   0        0        0     4844 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/message.py
--rw-r--r--   0        0        0     5468 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/model.py
--rw-r--r--   0        0        0      366 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/permission.py
--rw-r--r--   0        0        0     1008 2024-04-10 14:17:18.945326 nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/utils.py
--rw-r--r--   0        0        0     1543 2024-04-10 14:17:18.949326 nonebot_adapter_minecraft-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2409 1970-01-01 00:00:00.000000 nonebot_adapter_minecraft-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-14 14:59:55.232429 nonebot_adapter_minecraft-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1693 2024-04-14 14:59:55.232429 nonebot_adapter_minecraft-1.1.1/README.md
+-rw-r--r--   0        0        0      386 2024-04-14 14:59:55.232429 nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/__init__.py
+-rw-r--r--   0        0        0     8733 2024-04-14 14:59:55.232429 nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/adapter.py
+-rw-r--r--   0        0        0     2317 2024-04-14 14:59:55.232429 nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/bot.py
+-rw-r--r--   0        0        0     1165 2024-04-14 14:59:55.232429 nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/bot.pyi
+-rw-r--r--   0        0        0     3794 2024-04-14 14:59:55.232429 nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/collator.py
+-rw-r--r--   0        0        0      527 2024-04-14 14:59:55.232429 nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/compat.py
+-rw-r--r--   0        0        0      310 2024-04-14 14:59:55.232429 nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/config.py
+-rw-r--r--   0        0        0     1392 2024-04-14 14:59:55.232429 nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/event/__init__.py
+-rw-r--r--   0        0        0     3621 2024-04-14 14:59:55.232429 nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/event/base.py
+-rw-r--r--   0        0        0     1578 2024-04-14 14:59:55.232429 nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/event/fabric.py
+-rw-r--r--   0        0        0     1424 2024-04-14 14:59:55.232429 nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/event/forge.py
+-rw-r--r--   0        0        0      598 2024-04-14 14:59:55.232429 nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/event/minecraft.py
+-rw-r--r--   0        0        0     1818 2024-04-14 14:59:55.232429 nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/event/spigot.py
+-rw-r--r--   0        0        0     2138 2024-04-14 14:59:55.232429 nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/exception.py
+-rw-r--r--   0        0        0     4844 2024-04-14 14:59:55.232429 nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/message.py
+-rw-r--r--   0        0        0     5468 2024-04-14 14:59:55.232429 nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/model.py
+-rw-r--r--   0        0        0      366 2024-04-14 14:59:55.232429 nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/permission.py
+-rw-r--r--   0        0        0     1008 2024-04-14 14:59:55.232429 nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/utils.py
+-rw-r--r--   0        0        0     1543 2024-04-14 14:59:55.236429 nonebot_adapter_minecraft-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2409 1970-01-01 00:00:00.000000 nonebot_adapter_minecraft-1.1.1/PKG-INFO
```

### Comparing `nonebot_adapter_minecraft-1.1.0/LICENSE` & `nonebot_adapter_minecraft-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.0/README.md` & `nonebot_adapter_minecraft-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/adapter.py` & `nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/adapter.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/bot.py` & `nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/bot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/bot.pyi` & `nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/bot.pyi`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/collator.py` & `nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/collator.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/compat.py` & `nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/compat.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/event/__init__.py` & `nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/event/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/event/base.py` & `nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/event/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/event/fabric.py` & `nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/event/fabric.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/event/forge.py` & `nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/event/forge.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/event/minecraft.py` & `nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/event/minecraft.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/event/spigot.py` & `nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/event/spigot.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/exception.py` & `nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/message.py` & `nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/message.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/model.py` & `nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/model.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.0/nonebot/adapters/minecraft/utils.py` & `nonebot_adapter_minecraft-1.1.1/nonebot/adapters/minecraft/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_adapter_minecraft-1.1.0/pyproject.toml` & `nonebot_adapter_minecraft-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-adapter-minecraft"
-version = "1.1.0"
+version = "1.1.1"
 description = "NoneBot2与MineCraft Server互通的适配器。"
 authors = ["17TheWord <17theword@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "nonebot" }]
 
 [tool.poetry.dependencies]
```

### Comparing `nonebot_adapter_minecraft-1.1.0/PKG-INFO` & `nonebot_adapter_minecraft-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-adapter-minecraft
-Version: 1.1.0
+Version: 1.1.1
 Summary: NoneBot2与MineCraft Server互通的适配器。
 License: MIT
 Author: 17TheWord
 Author-email: 17theword@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

