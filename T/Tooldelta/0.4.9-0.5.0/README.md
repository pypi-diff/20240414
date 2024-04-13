# Comparing `tmp/tooldelta-0.4.9.tar.gz` & `tmp/tooldelta-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooldelta-0.4.9.tar", max compression
+gzip compressed data, was "tooldelta-0.5.0.tar", max compression
```

## Comparing `tooldelta-0.4.9.tar` & `tooldelta-0.5.0.tar`

### file list

```diff
@@ -1,33 +1,31 @@
--rwxr-xr-x   0        0        0     1497 2024-03-20 04:18:37.807537 tooldelta-0.4.9/LICENSE
--rwxr-xr-x   0        0        0     4376 2024-03-20 04:18:37.807537 tooldelta-0.4.9/README.md
--rwxr-xr-x   0        0        0      885 2024-03-20 04:18:46.263443 tooldelta-0.4.9/pyproject.toml
--rwxr-xr-x   0        0        0      290 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/__init__.py
--rwxr-xr-x   0        0        0     1591 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/basic_mods.py
--rwxr-xr-x   0        0        0    13640 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/builtins.py
--rwxr-xr-x   0        0        0     9338 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/cfg.py
--rwxr-xr-x   0        0        0     7848 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/color_print.py
--rw-r--r--   0        0        0     1945 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/constants.py
--rw-r--r--   0        0        0     5870 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/fb_conn/fbconn.py
--rwxr-xr-x   0        0        0    38486 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/frame.py
--rwxr-xr-x   0        0        0     3367 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/game_texts.py
--rwxr-xr-x   0        0        0     1663 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/get_python_libs.py
--rwxr-xr-x   0        0        0      338 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/get_tool_delta_version.py
--rwxr-xr-x   0        0        0    25909 2024-03-20 04:18:37.807537 tooldelta-0.4.9/tooldelta/launch_cli.py
--rwxr-xr-x   0        0        0     1054 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/launch_options.py
--rwxr-xr-x   0        0        0     2138 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/logger.py
--rwxr-xr-x   0        0        0    33949 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/neo_libs/neo_conn.py
--rwxr-xr-x   0        0        0     9089 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/old_dotcs_env.py
--rwxr-xr-x   0        0        0     1143 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/packets.py
--rwxr-xr-x   0        0        0    11936 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/plugin_load/PluginGroup.py
--rwxr-xr-x   0        0        0     2177 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/plugin_load/__init__.py
--rwxr-xr-x   0        0        0     6359 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/plugin_load/classic_plugin/__init__.py
--rwxr-xr-x   0        0        0     7579 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/plugin_load/dotcs_plugin/__init__.py
--rwxr-xr-x   0        0        0      345 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/plugin_load/funcs.py
--rwxr-xr-x   0        0        0     6914 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/plugin_load/injected_plugin/__init__.py
--rwxr-xr-x   0        0        0     9235 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/plugin_load/injected_plugin/movent.py
--rwxr-xr-x   0        0        0    14849 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/plugin_manager.py
--rwxr-xr-x   0        0        0    12409 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/plugin_market.py
--rw-r--r--   0        0        0     1822 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/starter.py
--rwxr-xr-x   0        0        0      639 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/sys_args.py
--rwxr-xr-x   0        0        0     6602 2024-03-20 04:18:37.811537 tooldelta-0.4.9/tooldelta/urlmethod.py
--rw-r--r--   0        0        0     5449 1970-01-01 00:00:00.000000 tooldelta-0.4.9/PKG-INFO
+-rwxr-xr-x   0        0        0     1497 2024-04-13 22:20:49.851509 tooldelta-0.5.0/LICENSE
+-rwxr-xr-x   0        0        0     2504 2024-04-13 22:20:49.851509 tooldelta-0.5.0/README.md
+-rwxr-xr-x   0        0        0      929 2024-04-13 22:20:57.339327 tooldelta-0.5.0/pyproject.toml
+-rwxr-xr-x   0        0        0      330 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/__init__.py
+-rw-r--r--   0        0        0     5906 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/auths.py
+-rwxr-xr-x   0        0        0      599 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/basic_mods.py
+-rwxr-xr-x   0        0        0    16782 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/builtins.py
+-rwxr-xr-x   0        0        0    10594 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/cfg.py
+-rwxr-xr-x   0        0        0     7848 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/color_print.py
+-rw-r--r--   0        0        0     1960 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/constants.py
+-rw-r--r--   0        0        0     5870 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/fb_conn/fbconn.py
+-rwxr-xr-x   0        0        0    34048 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/frame.py
+-rwxr-xr-x   0        0        0     3772 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/game_texts.py
+-rwxr-xr-x   0        0        0      338 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/get_tool_delta_version.py
+-rwxr-xr-x   0        0        0    32194 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/launch_cli.py
+-rwxr-xr-x   0        0        0     1080 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/launch_options.py
+-rwxr-xr-x   0        0        0     2138 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/logger.py
+-rwxr-xr-x   0        0        0    29503 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/neo_libs/neo_conn.py
+-rwxr-xr-x   0        0        0     1143 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/packets.py
+-rwxr-xr-x   0        0        0    11373 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/plugin_load/PluginGroup.py
+-rwxr-xr-x   0        0        0     2273 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/plugin_load/__init__.py
+-rwxr-xr-x   0        0        0     6200 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/plugin_load/classic_plugin/__init__.py
+-rwxr-xr-x   0        0        0      345 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/plugin_load/funcs.py
+-rwxr-xr-x   0        0        0     6780 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/plugin_load/injected_plugin/__init__.py
+-rwxr-xr-x   0        0        0     9235 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/plugin_load/injected_plugin/movent.py
+-rwxr-xr-x   0        0        0    12447 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/plugin_manager.py
+-rwxr-xr-x   0        0        0    13218 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/plugin_market.py
+-rw-r--r--   0        0        0     1860 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/starter.py
+-rwxr-xr-x   0        0        0      638 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/sys_args.py
+-rwxr-xr-x   0        0        0     7057 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/urlmethod.py
+-rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 tooldelta-0.5.0/PKG-INFO
```

### Comparing `tooldelta-0.4.9/LICENSE` & `tooldelta-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.9/pyproject.toml` & `tooldelta-0.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Tooldelta"
-version = "0.4.9" # This field is automatically set to the value in the version file
+version = "0.5.0" # This field is automatically set to the value in the version file
 description = "Plugin Loader for NeteaseRentalServer on Panel"
 authors = ["SuperScript-PRC"]
 license = ""
 
 readme = "README.md"
 homepage = "https://github.com/SuperScript-PRC/ToolDelta"
 repository = "https://github.com/SuperScript-PRC/ToolDelta"
@@ -22,11 +22,13 @@
 rich = "13.7.0"
 colorama = "^0.4.6"
 pillow = "^10.2.0"
 shellescape = "^3.8.1"
 pyspeedtest = "1.2.7"
 tqdm = "4.66.2"
 aiohttp = "^3.9.3"
+python-socketio = "5.11.1"
+flask = "^3.0.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tooldelta-0.4.9/tooldelta/builtins.py` & `tooldelta-0.5.0/tooldelta/builtins.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from .color_print import Print
 import ujson
 import os
 import threading
 import traceback
 import copy
 import ctypes
+import time
 from typing import Any, Dict, List, Tuple, Optional
 
 event_pool = {"tmpjson_save": threading.Event()}
 event_flags_pool = {"tmpjson_save": True}
-
+threads_list: list["Builtins.createThread"] = []
 
 class Builtins:
     class ThreadExit(SystemExit):
         "线程退出."
 
     class ClassicThread(threading.Thread):
         def __init__(self, func, args: tuple = (), usage="", **kwargs):
@@ -30,20 +31,23 @@
             self.func = func
             self.daemon = True
             self.all_args = [args, kwargs]
             self.usage = usage
             self.start()
 
         def run(self):
+            threads_list.append(self)
             try:
                 self.func(*self.all_args[0], **self.all_args[1])
-            except Builtins.ThreadExit:
+            except (Builtins.ThreadExit, SystemExit):
                 pass
             except:
-                Print.print_err(f"线程 {self.usage} 出错:\n" + traceback.format_exc())
+                Print.print_err(f"线程 {self.usage or self.func.__name__} 出错:\n" + traceback.format_exc())
+            finally:
+                threads_list.remove(self)
 
         def get_id(self):
             if hasattr(self, '_thread_id'):
                 return self._thread_id
             for id, thread in threading._active.items():
                 if thread is self:
                     return id
@@ -63,15 +67,15 @@
         def loadPathJson(path: str, needFileExists: bool = True):
             """
             将json文件从磁盘加载到缓存区, 以便快速读写.
             在缓存文件已加载的情况下, 再使用一次该方法不会有任何作用.
 
             参数:
                 path: 作为文件的磁盘内路径的同时也会作为在缓存区的虚拟路径
-                needFileExists: 默认为 True, 为 False 时, 若文件路径不存在, 就会自动创建一个文件.
+                needFileExists: 默认为 True, 为 False 时, 若文件路径不存在, 就会自动创建一个文件, 且默认值为null
             """
             if path in jsonPathTmp:
                 return
             try:
                 js = Builtins.SimpleJsonDataReader.SafeJsonLoad(path)
             except FileNotFoundError as err:
                 if not needFileExists:
@@ -109,28 +113,76 @@
                 val = jsonPathTmp.get(path)[1]
                 if isinstance(val, (list, dict)):
                     val = copy.deepcopy(val)
                 return val
             raise Exception("json路径未初始化, 不能进行读取和写入操作: " + path)
 
         @staticmethod
+        def get(path: str):
+            """
+            直接获取缓存区的该虚拟路径的JSON, 不使用copy
+            WARNING: 如果你不知道有什么后果, 请老老实实使用`read(...)`而不是`get(...)`!
+
+            参数:
+                path: 文件的虚拟路径
+            """
+            if path in jsonPathTmp:
+                val = jsonPathTmp.get(path)[1]
+                return val
+            raise Exception("json路径未初始化, 不能进行读取和写入操作: " + path)
+
+
+        @staticmethod
         def write(path: str, obj: Any):
             """
             对缓存区的该虚拟路径的文件进行写操作, 这将会覆盖之前的内容
 
             参数:
                 path: 文件的虚拟路径
                 obj: 任何合法的JSON类型 例如 dict/list/str/bool/int/float
             """
             if path in jsonPathTmp:
                 jsonPathTmp[path] = [True, obj]
             else:
                 raise Exception("json路径未初始化, 不能进行读取和写入操作: " + path)
 
         @staticmethod
+        def read_as_tmp(path: str, needFileExists: bool = True, timeout: int = 60):
+            """
+            读取json文件并将其从磁盘加载到缓存区, 以便一段时间内能快速读写.
+            推荐使用.
+
+            参数:
+                path: 作为文件的磁盘内路径的同时也会作为在缓存区的虚拟路径
+                needFileExists: 默认为 True, 为 False 时, 若文件路径不存在, 就会自动创建一个文件, 且写入默认值null
+                timeout: 多久没有再进行读取操作时卸载缓存
+            """
+            if path not in jsonUnloadPathTmp and not path in jsonPathTmp:
+                jsonUnloadPathTmp[path] = timeout + int(time.time())
+                Builtins.TMPJson.loadPathJson(path, needFileExists)
+            return Builtins.TMPJson.read(path)
+
+        @staticmethod
+        def write_as_tmp(path: str, obj: Any, needFileExists: bool = True, timeout: int = 60):
+            """
+            写入json文件并将其从磁盘加载到缓存区, 以便一段时间内能快速读写.
+            推荐使用.
+
+            参数:
+                path: 作为文件的磁盘内路径的同时也会作为在缓存区的虚拟路径
+                obj: 任何合法的JSON类型 例如 dict/list/str/bool/int/float
+                needFileExists: 默认为 True, 为 False 时, 若文件路径不存在, 就会自动创建一个文件, 且写入默认值null
+                timeout: 多久没有再进行读取操作时卸载缓存
+            """
+            if path not in jsonUnloadPathTmp and not path in jsonPathTmp:
+                jsonUnloadPathTmp[path] = timeout + int(time.time())
+                Builtins.TMPJson.loadPathJson(path, needFileExists)
+            Builtins.TMPJson.write(obj)
+
+        @staticmethod
         def cancel_change(path):
             "取消缓存json所做的更改, 非必要情况请勿调用, 你不知道什么时候会自动保存所做更改"
             jsonPathTmp[path][0] = False
 
         @staticmethod
         def get_tmps():
             "不要调用!"
@@ -140,15 +192,15 @@
         @staticmethod
         def SafeJsonDump(obj: str | dict | list, fp):
             """
             导出一个json文件, 会自动关闭文件读写接口.
 
             参数:
                 obj: json对象.
-                fp: 由open(...)打开的文件读写口 或 文件路径.
+                fp: 由 `open(...)` 打开的文件读写口 或 文件路径.
             """
             if isinstance(fp, str):
                 with open(fp, "w", encoding="utf-8") as file:
                     file.write(ujson.dumps(obj, indent=4, ensure_ascii=False))
             else:
                 with fp:
                     fp.write(ujson.dumps(obj, indent=4, ensure_ascii=False))
@@ -213,14 +265,19 @@
                 obj: 任何合法的JSON类型 例如 dict/list/str/bool/int/float
             """
             os.makedirs(f"插件数据文件/{plugin_name}", exist_ok=True)
             with open(f"插件数据文件/{plugin_name}/{file}.json", "w", encoding="utf-8") as f:
                 Builtins.SimpleJsonDataReader.SafeJsonDump(obj, f)
 
     @staticmethod
+    def get_threads_list():
+        "返回使用 createThread 创建的全线程列表."
+        return threads_list
+
+    @staticmethod
     def SimpleFmt(kw: Dict[str, Any], __sub: str) -> str:
         """
         快速将字符串内按照给出的dict的键值对替换掉内容.
 
         参数:
             kw: Dict[str, Any], 键值对应替换的内容
             __sub: str, 需要被替换的字符串
@@ -234,34 +291,37 @@
         for k, v in kw.items():
             if k in __sub:
                 __sub = __sub.replace(k, str(v))
         return __sub
 
     @staticmethod
     def simpleAssert(cond: Any, exc: Any) -> None:
-        """相当于 assert cond, 但是可以自定义引发的异常的类型"""
+        """
+        相当于 assert cond, 但是可以自定义引发的异常的类型
+        """
         if not cond:
             raise exc
 
     @staticmethod
-    def new_thread(func: Any) -> Any:
+    def thread_func(func: Any) -> Any:
         """
         在事件方法可能执行较久会造成堵塞时使用, 方便快捷地创建一个新线程, 例如:
 
         @Builtins.run_as_new_thread
         def on_inject(self):
             ...
         """
 
         def thread_fun(*args: Tuple, **kwargs: Any) -> None:
-            Builtins.createThread(func, args=args, **kwargs)
+            Builtins.createThread(func, usage="简易线程方法:"+func.__name__, args=args, **kwargs)
 
         return thread_fun
 
-    run_as_new_thread = new_thread
+    run_as_new_thread = thread_func
+    new_thread = thread_func
 
     @staticmethod
     def try_int(arg: Any) -> Optional[int]:
         """尝试将提供的参数化为int类型并返回, 否则返回None"""
         try:
             return int(arg)
         except:
@@ -359,30 +419,36 @@
             return __sub
 
 
 def safe_close():
     event_pool["tmpjson_save"].set()
     event_flags_pool["tmpjson_save"] = False
 
-
 def _tmpjson_save_thread():
     evt = event_pool["tmpjson_save"]
+    secs = 0
     while 1:
-        evt.wait(60)
-        for k, (isChanged, dat) in jsonPathTmp.copy().items():
-            if isChanged:
-                Builtins.SimpleJsonDataReader.SafeJsonDump(dat, k)
-                jsonPathTmp[k][0] = False
+        evt.wait(2)
+        secs += 2
+        if secs >= 60:
+            secs = 0
+            for k, (isChanged, dat) in jsonPathTmp.copy().items():
+                if isChanged:
+                    Builtins.SimpleJsonDataReader.SafeJsonDump(dat, k)
+                    jsonPathTmp[k][0] = False
+        for k, v in jsonUnloadPathTmp.copy().items():
+            if time.time() - v > 0:
+                Builtins.TMPJson.unloadPathJson(k)
+                del jsonUnloadPathTmp[k]
         if not event_flags_pool["tmpjson_save"]:
             return
 
 
 def tmpjson_save_thread():
-    Builtins.createThread(_tmpjson_save_thread)
-
+    Builtins.createThread(_tmpjson_save_thread, usage="JSON缓存文件定时保存")
 
 def _dialogue_thread_run(player, func, exc_cb, args, kwargs):
     if not Builtins.player_in_dialogue(player):
         Builtins.add_in_dialogue_player(player)
     else:
         if exc_cb is not None:
             exc_cb(player)
@@ -393,7 +459,8 @@
         Print.print_err(f"玩家{player}的会话线程 出现问题:")
         Print.print_err(traceback.format_exc())
     Builtins.remove_in_dialogue_player(player)
 
 
 jsonPathTmp = {}
 in_dialogue_list = []
+jsonUnloadPathTmp = {}
```

### Comparing `tooldelta-0.4.9/tooldelta/cfg.py` & `tooldelta-0.5.0/tooldelta/cfg.py`

 * *Files 8% similar despite different names*

```diff
@@ -221,26 +221,60 @@
             for val in value:
                 self.check_auto(pattern[1], val, fromkey)
         else:
             for single_type in pattern:
                 try:
                     self.check_auto(single_type, value, fromkey)
                     return
-                except:
+                except Exception as err:
                     pass
             raise self.ConfigValueError(
                 f"JSON列表的值 \"{fromkey}\" 类型不正确: 需要 {' 或 '.join(_CfgShowType(i) for i in pattern)}, 实际上为 {_CfgShowType(value)}"
             )
 
+    def auto_to_std(self, cfg):
+        """
+        自动以默认配置文件生成标准配置文件格式.
+        注意: 不支持固定长度列表以及Cfg.NeccessaryKey与Cfg.Group的自动转换
+
+        参数:
+            cfg: 默认的CFG配置文件
+        返回:
+            标准cfg样式, 用于 checkDict
+        """
+        if isinstance(cfg, dict):
+            res = {}
+            for k, v in cfg.items():
+                if isinstance(v, (dict, list)):
+                    res[k] = self.auto_to_std(v)
+                elif isinstance(v, (str, int, float, bool)):
+                    res[k] = type(v)
+            return res
+        if isinstance(cfg, list):
+            setting_types = []
+            for v in cfg:
+                if isinstance(v, (dict, list)):
+                    t = self.auto_to_std(v)
+                else:
+                    t = type(v)
+                if t not in setting_types:
+                    setting_types.append(t)
+            if len(setting_types) == 1:
+                return [r"%list", setting_types[0]]
+            return [r"%list", setting_types]
+        raise ValueError("auto_to_std() 仅接受 dict 与 list 参数")
+
     checkDict = check_dict_2
 
 
 if __name__ == "__main__":
     # Test Part
     try:
-        test_cfg = 12
-        a_std = [int, [r"%list", str]]
-        Cfg().check_auto(a_std, test_cfg)
+        test_cfg = [{"b": 1}]
+        a = [1, 2, 3, {"b": True}]
+        std = Cfg().auto_to_std(a)
+        print(std)
+        Cfg().check_auto(std, test_cfg)
     except Cfg.ConfigError:
         import traceback
 
         print(traceback.format_exc())
```

### Comparing `tooldelta-0.4.9/tooldelta/color_print.py` & `tooldelta-0.5.0/tooldelta/color_print.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.9/tooldelta/constants.py` & `tooldelta-0.5.0/tooldelta/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from typing import List
 from tooldelta.launch_cli import FrameFBConn, FrameNeOmg, FrameNeOmgRemote
 from tooldelta.cfg import Cfg
 
+PRG_NAME = "ToolDelta"
+
 PLUGIN_MARKET_SOURCE_OFFICIAL = "https://mirror.ghproxy.com/raw.githubusercontent.com/ToolDelta/ToolDelta-PluginMarket/main"
 
 LAUNCHERS: List[
     tuple[str, type[FrameFBConn | FrameNeOmg | FrameNeOmgRemote]]
 ] = [
     (
         "FastBuilder External 模式 (经典模式) §c(已停止维护, 无法适应新版本租赁服!)",
@@ -20,24 +22,24 @@
 
 LAUNCH_CFG: dict = {
     "服务器号": 0,
     "密码": 0,
     "启动器启动模式(请不要手动更改此项, 改为0可重置)": 0,
     "验证服务器地址(更换时记得更改fbtoken)": "",
     "是否记录日志": True,
-    "插件市场源": PLUGIN_MARKET_SOURCE_OFFICIAL,
+    "插件市场源": PLUGIN_MARKET_SOURCE_OFFICIAL
 }
 
 LAUNCH_CFG_STD: dict = {
     "服务器号": int,
     "密码": int,
     "启动器启动模式(请不要手动更改此项, 改为0可重置)": Cfg.NNInt,
     "验证服务器地址(更换时记得更改fbtoken)": str,
     "是否记录日志": bool,
-    "插件市场源": str,
+    "插件市场源": str
 }
 
 FB_APIS = [
     "https://api.fastbuilder.pro/api/phoenix/login",
     "https://api.fastbuilder.pro/api/new",
     "https://api.fastbuilder.pro/api/api",
     "https://api.fastbuilder.pro/api/login",
@@ -52,10 +54,10 @@
 ]
 
 AUTH_SERVERS = [
     ("FastBuilder 官方验证服务器", "https://api.fastbuilder.pro"),
     ("咕咕酱 FB验证服务器", "https://liliya233.uk"),
 ]
 
-TOOLDELTA_DOTCSEMU_PLUGIN = "原DotCS插件"
+TOOLDELTA_PLUGIN_DIR = "插件文件"
 TOOLDELTA_CLASSIC_PLUGIN = "ToolDelta类式插件"
 TOOLDELTA_INJECTED_PLUGIN = "ToolDelta注入式插件"
```

### Comparing `tooldelta-0.4.9/tooldelta/fb_conn/fbconn.py` & `tooldelta-0.5.0/tooldelta/fb_conn/fbconn.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.9/tooldelta/frame.py` & `tooldelta-0.5.0/tooldelta/frame.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import List, Union
 
 import tooldelta
 from tooldelta import (
+    auths,
     constants,
     builtins,
-    old_dotcs_env,
     plugin_market,
     sys_args,
 )
 
 from tooldelta.get_tool_delta_version import get_tool_delta_version
 from tooldelta.color_print import Print
 from tooldelta.basic_mods import (
@@ -17,16 +17,15 @@
     sys,
     time,
     traceback,
     requests,
     platform,
     subprocess,
     threading,
-    getpass,
-    hashlib,
+    getpass
 )
 
 from tooldelta.cfg import Cfg as _Cfg
 from tooldelta.logger import publicLogger
 from tooldelta.plugin_load.PluginGroup import PluginGroup
 from tooldelta.game_texts import GameTextsLoader
 from tooldelta.urlmethod import download_file_multithreading, test_site_latency
@@ -49,15 +48,14 @@
     execute_player_message,
     execute_repeat,
     safe_jump,
 )
 
 sys_args_dict = sys_args_to_dict(sys.argv)
 createThread = builtins.Builtins.createThread
-PRG_NAME = "ToolDelta"
 VERSION = get_tool_delta_version()
 Builtins = builtins.Builtins
 Config = _Cfg()
 
 # 整个系统由三个部分组成
 #  Frame: 负责整个 ToolDelta 的基本框架运行
 #  GameCtrl: 负责对接游戏
@@ -72,30 +70,29 @@
     class FrameBasic:
         system_version = VERSION
         max_connect_fb_time = 60
         connect_fb_start_time = time.time()
         data_path = "插件数据文件/"
 
     createThread = ClassicThread = Builtins.createThread
-    PRG_NAME = PRG_NAME
+    PRG_NAME = constants.PRG_NAME
     sys_data = FrameBasic()
     serverNumber: str = ""
     serverPasswd: str
     launchMode: int = 0
     consoleMenu = []
     link_game_ctrl = None
     link_plugin_group = None
-    old_dotcs_threadinglist = []
     on_plugin_err = staticmethod(
         lambda name, _, err: Print.print_err(f"插件 <{name}> 出现问题: \n{err}")
     )
 
     @staticmethod
     def check_use_token(tok_name="", check_md=""):
-        res = sys_args.sys_args_to_dict(sys.argv)
+        res = sys_args.sys_args_to_dict()
         res = res.get(tok_name, 1)
         if (res == 1 and check_md) or res != check_md:
             Print.print_err("启动参数错误")
             raise SystemExit
 
     @staticmethod
     def if_token():
@@ -107,169 +104,35 @@
             if fbtoken:
                 with open("fbtoken", "w", encoding="utf-8") as f:
                     f.write(fbtoken)
             else:
                 Print.print_err("未输入fbtoken, 无法继续")
                 raise SystemExit
 
-    def login_gugu(self) -> requests.Response:
-        hash_obj: hashlib._Hash = hashlib.sha256()
-        username: str = input(Print.fmt_info("请输入账号:", "§6 账号 "))
-        hash_obj.update(
-            getpass.getpass(Print.fmt_info("请输入密码(已隐藏):", "§6 密码 ")).encode()
-        )
-        __password: str = hash_obj.hexdigest()
-        Authorization: str = requests.get(url=constants.GUGU_APIS[1], timeout=5).text
-        repo: requests.Response = requests.post(
-            url=constants.GUGU_APIS[0],
-            data=json.dumps(
-                {
-                    "client_public_key": "",
-                    "server_code": "::DRY::",
-                    "server_passcode": "::DRY::",
-                    "username": username,
-                    "password": __password,
-                },
-                ensure_ascii=False,
-            ),
-            headers={
-                "Content-Type": "application/json",
-                "Authorization": f"Bearer {Authorization}",
-            },timeout=5
-        )
-        repo_text: dict = json.loads(repo.text)
-        if repo.status_code != 200:
-            Print.print_war(
-                f"请求Api接口失败，将自动使用Token登陆!状态码:{repo.status_code}，返回值:{repo.text}"
-            )
-            self.if_token()
-        self.token = repo_text["token"]
-        with open("fbtoken", "w", encoding="utf-8") as f:
-            f.write(self.token)
-
-    def login_fbuc(self) -> requests.Response:
-        hash_obj: hashlib._Hash = hashlib.sha256()
-        username: str = input(Print.fmt_info("请输入账号:", "§6 账号 "))
-        hash_obj.update(
-            getpass.getpass(
-                Print.fmt_info("请输入密码(已隐藏):", "§6 密码 ")
-            ).encode()
-        )
-        __password: str = hash_obj.hexdigest()
-        __mfa_code: str = getpass.getpass(
-            Print.fmt_info(
-                "请输入双重验证码(已隐藏)(如未设置请直接回车):", "§6 MFA  "
-            )
-        )
-        Authorization: str = requests.get(url=constants.FB_APIS[1], timeout=5).text
-        repo: requests.Response = requests.post(
-            url=constants.FB_APIS[3],
-            data=json.dumps(
-                {
-                    "username": username,
-                    "password": __password,
-                    "mfa_code": __mfa_code,
-                },
-                ensure_ascii=False,
-            ),
-            headers={
-                "Content-Type": "application/json",
-                "authorization": f"Bearer {Authorization}",
-            },
-        )
-        repo_text: dict = json.loads(repo.text)
-        repo_message: str = repo_text["message"]
-        repo_success: bool = repo_text["success"]
-        if repo.status_code != 200:
-            Print.print_war(
-                f"请求Api接口失败，将自动使用Token登陆!状态码:{repo.status_code}，返回值:{repo.text}"
-            )
-            self.if_token()
-        if not repo_success:
-            if "Invalid username, password, or MFA code." in repo_message:
-                Print.print_war("登陆失败，无效的用户名、密码或MFA代码!")
-                self.login_fbuc()
-        else:
-            with_perfix: dict = json.loads(
-                requests.get(
-                    url=constants.FB_APIS[2],
-                    data=json.dumps({"with_prefix": constants.FB_APIS[4]}),
-                    timeout=5,
-                    headers={
-                        "Content-Type": "application/json",
-                        "authorization": f"Bearer {Authorization}",
-                    },
-                ).text
-            )
-            fetch_announcements: dict = json.loads(
-                requests.get(
-                    url=constants.FB_APIS[4] + with_perfix["fetch_announcements"],
-                    timeout=5,
-                    headers={
-                        "Content-Type": "application/json",
-                        "authorization": f"Bearer {Authorization}",
-                    },
-                ).text
-            )
-            fetch_profile: dict = json.loads(
-                requests.get(
-                    url=constants.FB_APIS[4] + with_perfix["fetch_profile"],
-                    timeout=5,
-                    headers={
-                        "Content-Type": "application/json",
-                        "authorization": f"Bearer {Authorization}",
-                    },
-                ).text
-            )
-            get_helper_status: dict = json.loads(
-                requests.get(
-                    url=constants.FB_APIS[4] + with_perfix["get_helper_status"],
-                    timeout=5,
-                    headers={
-                        "Content-Type": "application/json",
-                        "authorization": f"Bearer {Authorization}",
-                    },
-                ).text
-            )
-            self.UserInfo: dict = {
-                "isadmin": repo_text["isadmin"],
-                "blc": fetch_profile["blc"],
-                "cn_username": fetch_profile["cn_username"],
-                "phoenix_otp": fetch_profile["phoenix_otp"],
-                "points": fetch_profile["points"],
-                "slots": fetch_profile["slots"],
-                "get_helper_status": get_helper_status,
-            }
-            self.token = requests.get(
-                url=constants.FB_APIS[4] + with_perfix["get_phoenix_token"],
-                data=json.dumps({"secret": f"{Authorization}"}),
-                timeout=5,
-                headers={
-                    "Content-Type": "application/json",
-                    "authorization": f"Bearer {Authorization}",
-                },
-            ).text
-            with open("fbtoken", "w", encoding="utf-8") as f:
-                f.write(self.token)
-
     class ToolDeltaUpdater:
-        def __init__(self):
-            self.auto_update()
+        def __init__(self, launcher):
+            self.launcher = launcher
+            self.auto_update(self.launcher)
             self.start_auto_update_thread()
 
         def start_auto_update_thread(self):
-            # 每6小时检查一次更新
-            threading.Timer(6 * 60 * 60, self.auto_update).start()
+            # 每24小时检查一次更新
+            threading.Timer(24 * 60 * 60, self.auto_update, args=(self.launcher)).start()
 
         @staticmethod
-        def auto_update():
+        def auto_update(launcher):
             try:
-                latest_version = requests.get(
-                    "https://api.github.com/repos/ToolDelta/ToolDelta/releases/latest"
-                ).json()["tag_name"]
+                try:
+                    num:int = 0 # 初始化计次器数据
+                    while True:
+                        if launcher.TDC.SocketIO.connected:latest_version = launcher.TDC.get_version_updates();break
+                        else:time.sleep(0.1);num = num + 1
+                        if num >=50:latest_version = requests.get("https://api.github.com/repos/ToolDelta/ToolDelta/releases/latest").json()["tag_name"];break
+                except:
+                    latest_version = requests.get("https://api.github.com/repos/ToolDelta/ToolDelta/releases/latest").json()["tag_name"]
                 current_version = ".".join(map(str, get_tool_delta_version()[:3]))
 
                 if latest_version == current_version:
                     # Print.print_suc(f"检测成功,当前为最新版本 -> {current_version}，无需更新")
                     return
                 if ".py" in os.path.basename(
                     __file__
@@ -334,40 +197,38 @@
                             if platform.system() == "Linux"
                             else "upgrade.bat"
                         )
                         with open(
                             upgrade_script_path, "w", encoding="utf-8"
                         ) as upgrade_script:
                             temp_shell = (
-                                f'#!/bin/bash\nif [ -f "{file_path}" ];then\n  sleep 3\n  rm -f {os.getcwd()}/{os.path.basename(__file__)}\n  mv {os.getcwd()}/ToolDelta-linux_new {os.getcwd()}/{os.path.basename(__file__)}\n  chmod 777 {os.path.basename(__file__)}\n  ./{os.path.basename(__file__)} -l 1\nelse\n  exit\nfi'
+                                f'#!/bin/bash\nif [ -f "{file_path}" ];then\n  sleep 3\n  rm -f {os.getcwd()}/{os.path.basename(__file__)}\n  mv {os.getcwd()}/ToolDelta-linux_new {os.getcwd()}/{os.path.basename(__file__)}\n  /usr/bin/chmod 777 {os.path.basename(__file__)}\n  ./{os.path.basename(__file__)} -l 1\nelse\n  exit\nfi'
                                 if platform.system() == "Linux"
                                 else f"@echo off\ncd {os.getcwd()}\nif not exist {win_old_tool_delta_path} exit\ntimeout /T 3 /NOBREAK\ndel {win_old_tool_delta_path}\nren ToolDelta-windows_new.exe {os.path.basename(win_old_tool_delta_path)}\nstart {os.path.basename(win_old_tool_delta_path)}"
                             )
                             upgrade_script.write(temp_shell)
                         threading.Thread(
                             target=tooldelta.safe_jump, kwargs={"exit_directly": True}
                         ).start()
                         upgrade_process = subprocess.Popen(
                             (
                                 f"sh {upgrade_script_path}"
                                 if platform.system() == "Linux"
                                 else f"{upgrade_script_path}"
                             ),
                             cwd=os.getcwd(),
-                            shell=True,
                         )
                         upgrade_process.communicate()
 
             except Exception as err:
                 Print.print_war(
                     f"在检测最新版本或更新ToolDelta至最新版本时出现异常，ToolDelta将会在下次启动时重新更新: {err}"
                 )
 
     def read_cfg(self):
-
         Config.default_cfg("ToolDelta基本配置.json", constants.LAUNCH_CFG)
         try:
             cfgs = Config.get_cfg("ToolDelta基本配置.json", constants.LAUNCH_CFG_STD)
             self.serverNumber = str(cfgs["服务器号"])
             self.serverPasswd = cfgs["密码"]
             self.launchMode = cfgs["启动器启动模式(请不要手动更改此项, 改为0可重置)"]
             self.plugin_market_url = cfgs["插件市场源"]
@@ -376,62 +237,62 @@
             if self.launchMode != 0 and self.launchMode not in range(
                 1, len(constants.LAUNCHERS) + 1
             ):
                 raise Config.ConfigError(
                     "你不该随意修改启动器模式, 现在赶紧把它改回0吧"
                 )
         except Config.ConfigError as err:
-            r = self.upgrade_cfg(constants.LAUNCH_CFG)
+            r = self.upgrade_cfg()
             if r:
                 Print.print_war("配置文件未升级, 已自动升级, 请重启 ToolDelta")
             else:
                 Print.print_err(f"ToolDelta基本配置有误, 需要更正: {err}")
             raise SystemExit
         if self.serverNumber == "0":
             while 1:
                 try:
                     self.serverNumber = input(
                         Print.fmt_info("请输入租赁服号: ", "§b 输入 ")
                     )
                     self.serverPasswd = (
-                        input(
+                        getpass.getpass(
                             Print.fmt_info(
-                                "请输入租赁服密码(没有请直接回车): ", "§b 输入 "
+                                "请输入租赁服密码(不会回显, 没有请直接回车): ", "§b 输入 "
                             )
                         )
                         or "0"
                     )
                     std = constants.LAUNCH_CFG.copy()
                     std["服务器号"] = int(self.serverNumber)
                     std["密码"] = int(self.serverPasswd)
                     Config.default_cfg("ToolDelta基本配置.json", std, True)
-                    Print.print_suc("登陆配置设置成功")
+                    Print.print_suc("登录配置设置成功")
                     cfgs = std
                     break
                 except:
                     Print.print_err("输入有误， 租赁服号和密码应当是纯数字")
 
         auth_servers = constants.AUTH_SERVERS
         if auth_server == "":
             Print.print_inf("选择 ToolDelta机器人账号 使用的验证服务器:")
             for i, (auth_server_name, _) in enumerate(auth_servers):
                 Print.print_inf(f" {i + 1} - {auth_server_name}")
             Print.print_inf(
-                "NOTE: 使用的机器人账号是在哪里获取的就选择哪一个验证服务器, 不能混用"
+                "§cNOTE: 使用的机器人账号是在哪里获取的就选择哪一个验证服务器, 不能混用"
             )
             while 1:
                 try:
                     ch = int(input(Print.fmt_info("请选择: ", "§f 输入 ")))
                     if ch not in range(1, len(auth_servers) + 1):
-                        raise AssertionError
+                        raise ValueError
                     cfgs["验证服务器地址(更换时记得更改fbtoken)"] = auth_servers[
                         ch - 1
                     ][1]
                     break
-                except (ValueError, AssertionError):
+                except ValueError:
                     Print.print_err("输入不合法, 或者是不在范围内, 请重新输入")
             Config.default_cfg("ToolDelta基本配置.json", cfgs, True)
             # 读取启动配置等
         if not os.path.isfile("fbtoken"):
             Print.print_inf(
                 "请选择登录方法:\n 1 - 使用账号密码(登录成功后将自动获取Token到工作目录)\n 2 - 使用Token(如果Token文件不存在则需要输入或将文件放入工作目录)\r"
             )
@@ -446,34 +307,37 @@
                         Print.fmt_info("输入有误, 请输入正确的序号: ", "§6 警告 ")
                     )
                 else:
                     break
             if Login_method == "1":
                 match cfgs["验证服务器地址(更换时记得更改fbtoken)"]:
                     case "https://liliya233.uk":
-                        self.login_gugu()
+                        auths.login_liliya()
                     case "https://api.fastbuilder.pro":
-                        self.login_fbuc()
+                        auths.login_fbuc()
+                    case _:
+                        Print.print_err("暂无法登录该验证服务器")
+                        raise SystemExit
             elif Login_method == "2":
                 self.if_token()
             else:
                 self.if_token()
         launchers = constants.LAUNCHERS
         if self.launchMode == 0:
             Print.print_inf("请选择启动器启动模式(之后可在ToolDelta启动配置更改):")
             for i, (launcher_name, _) in enumerate(launchers):
                 Print.print_inf(f" {i + 1} - {launcher_name}")
             while 1:
                 try:
                     ch = int(input(Print.fmt_info("请选择: ", "§f 输入 ")))
                     if ch not in range(1, len(launchers) + 1):
-                        raise AssertionError
+                        raise ValueError
                     cfgs["启动器启动模式(请不要手动更改此项, 改为0可重置)"] = ch
                     break
-                except (ValueError, AssertionError):
+                except ValueError:
                     Print.print_err("输入不合法, 或者是不在范围内, 请重新输入")
             Config.default_cfg("ToolDelta基本配置.json", cfgs, True)
         launcher: Callable = launchers[
             cfgs["启动器启动模式(请不要手动更改此项, 改为0可重置)"] - 1
         ][1]
         self.fbtokenFix()
         with open("fbtoken", "r", encoding="utf-8") as f:
@@ -482,71 +346,63 @@
             self.serverNumber,
             self.serverPasswd,
             fbtoken,
             auth_server,
         )
 
     @staticmethod
-    def upgrade_cfg(cfg_std):
+    def upgrade_cfg():
         # 升级本地的配置文件
         old_cfg = Config.get_cfg("ToolDelta基本配置.json", {})
         old_cfg_keys = old_cfg.keys()
         need_upgrade_cfg = False
-        if "验证服务器地址(更换时记得更改fbtoken)" not in old_cfg_keys:
-            old_cfg["验证服务器地址(更换时记得更改fbtoken)"] = ""
-            need_upgrade_cfg = True
-        if "是否记录日志" not in old_cfg_keys:
-            old_cfg["是否记录日志"] = False
-            need_upgrade_cfg = True
-        if "插件市场源" not in old_cfg_keys:
-            old_cfg["插件市场源"] = cfg_std["插件市场源"]
-            need_upgrade_cfg = True
+        for k, v in constants.LAUNCH_CFG.items():
+            if k not in old_cfg_keys:
+                old_cfg[k] = v
+                need_upgrade_cfg = True
         if need_upgrade_cfg:
             Config.default_cfg("ToolDelta基本配置.json", old_cfg, True)
         return need_upgrade_cfg
 
-    @staticmethod
-    def welcome():
+    def welcome(self):
         # 欢迎提示
         Print.print_with_info(
-            f"§d{PRG_NAME} Panel Embed By SuperScript", Print.INFO_LOAD
+            f"§d{self.PRG_NAME} Panel Embed By SuperScript", Print.INFO_LOAD
         )
         Print.print_with_info(
-            f"§d{PRG_NAME} Wiki: https://tooldelta-wiki.tblstudio.cn/", Print.INFO_LOAD
+            f"§d{self.PRG_NAME} Wiki: https://tooldelta-wiki.tblstudio.cn/", Print.INFO_LOAD
         )
         Print.print_with_info(
-            f"§d{PRG_NAME} 项目地址: https://github.com/ToolDelta", Print.INFO_LOAD
+            f"§d{self.PRG_NAME} 项目地址: https://github.com/ToolDelta", Print.INFO_LOAD
         )
         Print.print_with_info(
-            f"§d{PRG_NAME} v {'.'.join([str(i) for i in VERSION])}", Print.INFO_LOAD
+            f"§d{self.PRG_NAME} v {'.'.join([str(i) for i in VERSION])}", Print.INFO_LOAD
         )
-        Print.print_with_info(f"§d{PRG_NAME} Panel 已启动", Print.INFO_LOAD)
+        Print.print_with_info(f"§d{self.PRG_NAME} Panel 已启动", Print.INFO_LOAD)
 
     @staticmethod
     def plugin_load_finished(plugins: PluginGroup):
         # 插件成功载入提示
         Print.print_suc(
-            f"成功载入 §f{plugins.normal_plugin_loaded_num}§a 个组合式插件, §f{plugins.injected_plugin_loaded_num}§a 个注入式插件, §f{plugins.dotcs_plugin_loaded_num}§a 个DotCS插件"
+            f"成功载入 §f{plugins.normal_plugin_loaded_num}§a 个组合式插件, §f{plugins.injected_plugin_loaded_num}§a 个注入式插件"
         )
 
     @staticmethod
     def basic_operation():
         # 初始化文件夹
         if os.path.isdir("插件文件/ToolDelta组合式插件"):
             os.rename(
                 "插件文件/ToolDelta组合式插件",
                 f"插件文件/{constants.TOOLDELTA_CLASSIC_PLUGIN}",
             )
-        os.makedirs("插件文件/原DotCS插件", exist_ok=True)
         os.makedirs(f"插件文件/{constants.TOOLDELTA_CLASSIC_PLUGIN}", exist_ok=True)
         os.makedirs(f"插件文件/{constants.TOOLDELTA_INJECTED_PLUGIN}", exist_ok=True)
         os.makedirs("插件配置文件", exist_ok=True)
         os.makedirs("tooldelta/fb_conn", exist_ok=True)
         os.makedirs("tooldelta/neo_libs", exist_ok=True)
-        os.makedirs("status", exist_ok=True)
         os.makedirs("插件数据文件/status", exist_ok=True)
         os.makedirs("插件数据文件/players", exist_ok=True)
         os.makedirs("插件数据文件/game_texts", exist_ok=True)
 
     @staticmethod
     def fbtokenFix():
         # 对异常FbToken的自动修复
@@ -580,15 +436,15 @@
             self.consoleMenu.append([usage, arg_hint, func, triggers])
 
     def init_basic_help_menu(self, _):
         menu = self.get_console_menus()
         Print.print_inf("§a以下是可选的菜单指令项: ")
         for usage, arg_hint, _, triggers in menu:
             if arg_hint:
-                Print.print_inf(f" §e{' 或 '.join(triggers)} {arg_hint}  §f->  {usage}")
+                Print.print_inf(f" §e{' 或 '.join(triggers)} §b{arg_hint} §f->  {usage}")
             else:
                 Print.print_inf(f" §e{' 或 '.join(triggers)}  §f->  {usage}")
 
     def comsole_cmd_start(self):
         def _try_execute_console_cmd(func, rsp, mode, arg1):
             try:
                 if mode == 0:
@@ -600,43 +456,82 @@
                 return
             try:
                 return func(rsp_arg) or 0
             except:
                 Print.print_err(f"控制台指令出错： {traceback.format_exc()}")
                 return 0
 
+        @Builtins.thread_func
+        def _execute_mc_command_and_get_callback(cmd: str):
+            cmd = " ".join(cmd)
+            try:
+                result = self.link_game_ctrl.sendcmd(cmd, True, 10)
+                if (result.OutputMessages[0].Message == "commands.generic.syntax") | (
+                    result.OutputMessages[0].Message == "commands.generic.unknown"
+                ):
+                    Print.print_err(f'未知的MC指令， 可能是指令格式有误： "{cmd}"')
+                else:
+                    jso = json.dumps(
+                        result.as_dict["OutputMessages"], indent=2, ensure_ascii=False
+                    )
+                    if not result.SuccessCount:
+                        Print.print_war(f"指令执行失败: \n{jso}")
+                    else:
+                        Print.print_suc(f"指令执行成功: \n{jso}")
+            except IndexError:
+                if result.SuccessCount:
+                    Print.print_suc(
+                        f"指令执行成功: \n{json.dumps(result.as_dict['OutputMessages'], indent=2, ensure_ascii=False)}"
+                    )
+            except TimeoutError:
+                Print.print_err("[超时] 指令获取结果返回超时")
+
         def _console_cmd_thread():
             self.add_console_cmd_trigger(
                 ["?", "help", "帮助"],
                 None,
                 "查询可用菜单指令",
                 self.init_basic_help_menu,
             )
             self.add_console_cmd_trigger(
                 ["exit"],
                 None,
-                f"退出并关闭{PRG_NAME}",
+                f"退出并关闭{self.PRG_NAME}",
                 lambda _: tooldelta.safe_jump(out_task=True),
             )
             self.add_console_cmd_trigger(
                 ["插件市场"],
                 None,
                 "进入插件市场",
                 lambda _: plugin_market.market.enter_plugin_market(
                     self.plugin_market_url, in_game=True
                 ),
             )
+            self.add_console_cmd_trigger(
+                ["/"],
+                "[指令]",
+                "执行MC指令",
+                _execute_mc_command_and_get_callback
+            )
+            self.add_console_cmd_trigger(
+                ["list"],
+                None,
+                "查询在线玩家",
+                lambda _: Print.print_inf(
+                    "在线玩家: " + ", ".join(self.link_game_ctrl.allplayers)
+                ),
+            )
             while 1:
                 rsp = ""
                 while True:
                     res = sys.stdin.read(1)
                     if res == "\n":  # 如果是换行符，则输出当前输入并清空输入
                         break
-                    if res in ("", "^C"):
-                        Print.print_inf("使用 Ctrl+C 退出中...")
+                    if res in ("", "^C", "^D"):
+                        Print.print_inf("按退出键退出中...")
                         self.launcher.status = SysStatus.NORMAL_EXIT
                         self.system_exit()
                         return
                     rsp += res
                 for _, _, func, triggers in self.consoleMenu:
                     if not rsp:
                         continue
@@ -664,18 +559,14 @@
                     f"/kick {self.link_game_ctrl.bot_name} ToolDelta 退出中(看到这条消息请重新加入游戏)\nSTATUS CODE: {exit_status_code}"
                 )
             except:
                 pass
         time.sleep(0.5)
         self.launcher.exit_event.set()
 
-    def _get_old_dotcs_env(self):
-        # 获取 dotcs 的插件环境
-        return old_dotcs_env.get_dotcs_env(self, Print)
-
     def get_console_menus(self):
         # 获取所有控制台命令菜单
         return self.consoleMenu
 
     def set_game_control(self, game_ctrl):
         "使用外源GameControl..."
         self.link_game_ctrl: GameCtrl = game_ctrl
@@ -834,15 +725,15 @@
                     msg_text = json.loads(msg)["rawtext"]
                     msg_text = "".join([i["text"] for i in msg_text])
                     Print.print_inf(msg_text)
                 except:
                     pass
 
     def Inject(self):
-        # 载入游戏时的初始化）
+        # 载入游戏时的初始化
         res = self.launcher.get_players_and_uuids()
         if res:
             self.allplayers = list(res.keys())
             self.players_uuid.update(res)
         else:
             while 1:
                 try:
@@ -872,17 +763,14 @@
         # 载入游戏后的欢迎提示语
         Print.print_suc(
             "初始化完成, 在线玩家: "
             + ", ".join(self.allplayers)
             + ", 机器人ID: "
             + self.bot_name
         )
-        time.sleep(0.5)
-        self.say_to("@a", "§l§7[§f!§7] §r§fToolDelta Enabled!\n§l§7[§f!§7] §r§f北京时间 "
-            + datetime.datetime.now().strftime("§a%H§f : §a%M") + "\n§l§7[§f!§7] §r§f输入.help获取更多帮助哦")
         self.sendcmd("/tag @s add robot")
         Print.print_suc("§f在控制台输入 §ahelp / ?§f可查看控制台命令")
 
     def say_to(self, target: str, msg: str):
         """
         向玩家发送聊天栏信息
```

### Comparing `tooldelta-0.4.9/tooldelta/game_texts.py` & `tooldelta-0.5.0/tooldelta/game_texts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,98 @@
-from .basic_mods import os, requests, re, tarfile, gzip, json, importlib, threading, time
+from .basic_mods import (
+    os,
+    requests,
+    re,
+    tarfile,
+    gzip,
+    json,
+    importlib,
+    threading,
+    time,
+)
 from .urlmethod import download_file_singlethreaded
 from typing import Dict
 from .color_print import Print
 from glob import glob
 
+
 class GameTextsLoader:
     def __init__(self) -> None:
         self.base_path = os.path.join(os.getcwd(), "插件数据文件", "game_texts")
         self.check_initial_run()
         self.start_auto_update_thread()
         self.game_texts_data: Dict[str, str] = self.load_data()
 
     @staticmethod
     def get_latest_version() -> str:
-        return re.match(r"(\d+\.\d+\.\d+)", requests.get("https://api.github.com/repos/ToolDelta/ToolDelta-Game_Texts/releases/latest", verify=False).json()["tag_name"]).group()
+        return re.match(
+            r"(\d+\.\d+\.\d+)",
+            requests.get(
+                "https://api.github.com/repos/ToolDelta/GameText/releases/latest"
+            ).json()["tag_name"],
+        ).group()
 
     def check_initial_run(self) -> None:
         version_file_path: str = os.path.join(self.base_path, "version")
         if not os.path.exists(version_file_path):
             latest_version: str = self.get_latest_version()
-            open(version_file_path, "w").write(latest_version)
+            with open(version_file_path, "w", encoding="utf-8") as f:
+                f.write(latest_version)
             self.download_and_extract(latest_version)
 
     def start_auto_update_thread(self) -> None:
         threading.Timer(24 * 60 * 60, self.auto_update).start()
 
     def auto_update(self) -> None:
         version_file_path: str = os.path.join(self.base_path, "version")
-        version: str = open(version_file_path, "r").read()
+        with open(version_file_path, "r", encoding="utf-8") as f:
+            version: str = f.read()
         latest_version: str = self.get_latest_version()
         if version != latest_version:
             self.download_and_extract(latest_version)
         threading.Timer(24 * 60 * 60, self.auto_update).start()
 
     def download_and_extract(self, version):
-        packets_url: str = f"https://hub.gitmirror.com/?q=https://github.com/ToolDelta/ToolDelta-Game_Texts/releases/download/{version}/ToolDelta_Game_Texts.tar.gz"
+        packets_url: str = (
+            f"https://hub.gitmirror.com/?q=https://github.com/ToolDelta/GameText/releases/download/{version}/ToolDelta_Game_Texts.tar.gz"
+        )
         archive_path = os.path.join(self.base_path, "ToolDelta_Game_Texts.tar.gz")
         download_file_singlethreaded(packets_url, archive_path)
         self.extract_data_archive(archive_path)
 
     def load_data(self) -> Dict[str, str]:
         try:
             all_values: Dict[str, str] = {}
-            for file_path in glob(os.path.join(self.base_path, "src", "**", "*.py"), recursive=True):
+            for file_path in glob(
+                os.path.join(self.base_path, "src", "**", "*.py"), recursive=True
+            ):
                 module_name: str = os.path.basename(file_path).replace(".py", "")
-                spec: importlib.util.spec_from_file_location = importlib.util.spec_from_file_location(module_name, file_path)
-                module: importlib.util.module_from_spec = importlib.util.module_from_spec(spec)
+                spec: importlib.util.spec_from_file_location = (
+                    importlib.util.spec_from_file_location(module_name, file_path)
+                )
+                module: importlib.util.module_from_spec = (
+                    importlib.util.module_from_spec(spec)
+                )
                 spec.loader.exec_module(module)
                 for var_name in dir(module):
                     if not var_name.startswith("__"):
                         var_value = getattr(module, var_name)
                         if isinstance(var_value, dict):
                             all_values.update(var_value)
             return all_values
         except Exception as err:
             return {}
 
     def extract_data_archive(self, zip_path: str) -> bool:
         try:
-            with gzip.open(zip_path, 'rb') as f_in, tarfile.open(fileobj=f_in, mode='r') as tar:
+            with gzip.open(zip_path, "rb") as f_in, tarfile.open(
+                fileobj=f_in, mode="r"
+            ) as tar:
                 tar.extractall(self.base_path)
-                open(os.path.join(self.base_path, "src_tree.json"), 'w').write(json.dumps(tar.getnames()))
+                with open(
+                    os.path.join(self.base_path, "src_tree.json"), "w", encoding="utf-8"
+                ) as f:
+                    json.dump(tar.getnames(), f)
                 return True
         except Exception as err:
             Print.print_war(f"Error extracting data archive: {err}")
             return False
```

### Comparing `tooldelta-0.4.9/tooldelta/launch_cli.py` & `tooldelta-0.5.0/tooldelta/launch_cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,35 @@
+from hmac import new
 import platform
 import os
+from poplib import CR
 import shlex
 import subprocess
+import uuid
 import time
 import json
+import ssl
 import requests
 import ujson
 import random
-import asyncio
-import aiohttp
-from typing import Callable
+from typing import Callable, Optional
 
 from .color_print import Print
 from .urlmethod import download_file_singlethreaded, get_free_port
 from .builtins import Builtins
+from .basic_mods import socketio
 from .packets import Packet_CommandOutput, PacketIDS
 from .sys_args import sys_args_to_dict
 
 from .fb_conn import fbconn
 import threading
 
 import tooldelta
 
 
-async def fetch(session, url):
-    async with session.get(url) as response:
-        return await response.read()
-
-
 class SysStatus:
     LOADING = 100
     LAUNCHING = 101
     RUNNING = 102
     NORMAL_EXIT = 103
     FB_LAUNCH_EXC = 104
     CRASHED_EXIT = 105
@@ -47,15 +45,15 @@
         self.serverNumber = serverNumber
         self.serverPassword = password
         self.fbToken = fbToken
         self.auth_server = auth_server_url
         self.status = SysStatus.LOADING
         self.system_type = platform.uname().system
         self.inject_events = []
-        self.packet_handler: Callable | None = None
+        self.packet_handler: Callable | None = lambda pckType, pck: None
         self.need_listen_packets = {9, 63, 79}
         self._launcher_listener = None
         self.exit_event = threading.Event()
 
     def add_listen_packets(self, *pcks: int):
         for i in pcks:
             self.need_listen_packets.add(i)
@@ -116,15 +114,15 @@
             Builtins.createThread(self.output_fb_msgs_thread)
             self.process_game_packets()
         except Exception as err:
             return err
 
     def runFB(self, ip="127.0.0.1", port=8080):
         if self.system_type == "Linux":
-            os.system("chmod +x ./phoenixbuilder")
+            os.system("/usr/bin/chmod +x ./phoenixbuilder")
             con_cmd = rf"./phoenixbuilder -A {self.auth_server} -t fbtoken --no-readline --no-update-check --listen-external {ip}:{port} -c {self.serverNumber} {f'-p {self.serverPassword}' if self.serverPassword else ''}"
 
         # windows updated "./PRGM" command.
         if self.system_type == "Windows":
             con_cmd = rf".\phoenixbuilder.exe -A {self.auth_server} -t fbtoken --no-readline --no-update-check --listen-external {ip}:{port} -c {self.serverNumber} {f'-p {self.serverPassword}' if self.serverPassword else ''}"
         self.fb_pipe = subprocess.Popen(
             con_cmd,
@@ -349,20 +347,21 @@
 
 class FrameNeOmg(StandardFrame):
     # 使用 NeOmega 框架连接到游戏
     launch_type = "NeOmega"
 
     def __init__(self, serverNumber, password, fbToken, auth_server):
         super().__init__(serverNumber, password, fbToken, auth_server)
-
         self.status = None
         self.launch_event = threading.Event()
         self.injected = False
         self.omega = None
-        asyncio.run(self.download_libs())
+        self.TDC = None
+        self.set_tooldelta_cli()
+        self.download_libs()
         self.init_all_functions()
         self.status = SysStatus.LOADING
         self.secret_exit_key = ""
 
     def set_omega(self, openat_port):
         from .neo_libs import neo_conn
 
@@ -385,28 +384,32 @@
                 time.sleep(5)
                 retries += 1
                 Print.print_war(f"OMEGA 连接失败, 重连: 第 {retries} 次: {err}")
                 if retries > 5:
                     Print.print_err("最大重试次数已达到")
                     raise SystemExit
 
+    def set_tooldelta_cli(self):
+        if type(self) == FrameNeOmg:
+            self.TDC = ToolDeltaCli()
+
     def start_neomega_proc(self):
         free_port = get_free_port(24016)
         access_point_file = (
             f"neomega_{platform.uname().system.lower()}_access_point_{self.sys_machine}"
         )
         if "TERMUX_VERSION" in os.environ:
             access_point_file = f"neomega_android_access_point_{self.sys_machine}"
         if platform.system() == "Windows":
             access_point_file += ".exe"
         py_file_path = os.path.join(
             os.getcwd(), "tooldelta", "neo_libs", access_point_file
         )
         if platform.uname().system.lower() == "linux":
-            os.system(f"chmod +x {shlex.quote(py_file_path)}")
+            os.system("chmod +x " + shlex.quote(py_file_path))
         # 只需要+x即可
         Print.print_inf(f"DEBUG: 将使用端口 {free_port}")
         self.neomg_proc = subprocess.Popen(
             [
                 py_file_path,
                 "-server",
                 self.serverNumber,
@@ -452,104 +455,132 @@
         self.status = SysStatus.LAUNCHING
         openat_port = self.start_neomega_proc()
         self.msg_show()
         self.launch_event.wait()
         self.make_secret_key()
         self.set_omega(openat_port)
         self.update_status(SysStatus.RUNNING)
-        Print.print_suc("已开启 NEOMG 进程")
+        Print.print_suc("已开启接入点进程")
         pcks = [
             self.omega.get_packet_id_to_name_mapping(i)
             for i in self.need_listen_packets
         ]
         self.omega.listen_packets(pcks, self.packet_handler_parent)
         self._launcher_listener()
-        # bug expired
-        self.omega.listen_player_chat(lambda _, _2: None)
-        Print.print_suc("NEOMEGA 接入已就绪!")
+        Print.print_suc("接入点已就绪!")
         self.exit_event.wait()  # 等待事件的触发
         if self.status == SysStatus.NORMAL_EXIT:
             return SystemExit("正常退出.")
         if self.status == SysStatus.CRASHED_EXIT:
             return Exception("NeOmega 已崩溃")
         return SystemError("未知的退出状态")
 
-    async def download_libs(self):
-        try:
-            async with aiohttp.ClientSession() as session:
-                res_text = await fetch(
-                    session,
-                    "https://mirror.ghproxy.com/https://raw.githubusercontent.com/ToolDelta/ToolDelta/main/require_files.json",
-                )
-                res = json.loads(res_text.decode("utf-8"))
-                use_mirror = res.get("Mirror", [""])[0]
-        except Exception as err:
-            Print.print_err(f"获取依赖库表出现问题: {err}")
-            raise SystemExit
-
-        self.sys_machine = platform.machine().lower()
-        self.sys_machine = (
-            "amd64"
-            if self.sys_machine == "x86_64"
-            else "arm64" if self.sys_machine == "aarch64" else self.sys_machine
-        )
-        sys_info_fmt = (
-            f"Android:{self.sys_machine.lower()}"
-            if "TERMUX_VERSION" in os.environ
-            else f"{platform.uname().system}:{self.sys_machine.lower()}"
-        )
-        source_dict = res.get(sys_info_fmt, {})
-
-        commit_file_path, commit_url = next(
-            iter(res.get("Commit", {}).items()), (None, None)
-        )
-        if not commit_file_path or not commit_url:
-            Print.print_err("未找到提交文件路径或URL")
-            raise SystemExit
-
-        async with aiohttp.ClientSession() as session:
-            async with session.get(
-                use_mirror + "/raw.githubusercontent.com/" + commit_url
-            ) as response:
-                commit_remote = await response.text()
-
-        commit_local = ""
-        commit_file_path = os.path.join(os.getcwd(), commit_file_path)
-        replace_file = False
-        if os.path.isfile(commit_file_path):
-            with open(commit_file_path, "r", encoding="utf-8") as f:
-                commit_local = f.read()
-
-            replace_file = commit_local != commit_remote
-
-            if replace_file:
-                Print.print_war("依赖库版本过期, 将重新下载" + f"{commit_local}-> {commit_remote}")
-
-        tasks = []
-        async with aiohttp.ClientSession() as session:
+    def download_libs(self):
+        if self.TDC.SocketIO.connected:
+            try:
+                res = self.TDC.get_depends_table_data()
+                use_mirror = res["mirror_data"]["Mirror"][0]
+            except Exception as err:
+                Print.print_err(f"获取依赖库表出现问题: {err}")
+                self.update_status(SysStatus.CRASHED_EXIT)
+                return
+            self.sys_machine = platform.machine().lower()
+            if self.sys_machine == "x86_64":
+                self.sys_machine = "amd64"
+            elif self.sys_machine == "aarch64":
+                self.sys_machine = "arm64"
+            if "TERMUX_VERSION" in os.environ:
+                sys_info_fmt = f"Android:{self.sys_machine.lower()}"
+            else:
+                sys_info_fmt = f"{platform.uname().system}:{self.sys_machine.lower()}"
+            source_dict = res["mirror_data"][sys_info_fmt]
+            commit_file_path = res["commit_file_path"]
+            commit_url = res["commit"]
+            commit_remote = res["commit"]
+            commit_local = ""
+            commit_file_path = os.path.join(os.getcwd(), commit_file_path)
+            replace_file = False
+            if os.path.isfile(commit_file_path):
+                with open(commit_file_path, "r", encoding="utf-8") as f:
+                    commit_local = f.read()
+                if commit_local != commit_remote:
+                    Print.print_war("依赖库版本过期, 将重新下载")
+                    replace_file = True
+            else:
+                replace_file = True
             for k, v in source_dict.items():
                 pathdir = os.path.join(os.getcwd(), k)
                 url = use_mirror + "/https://raw.githubusercontent.com/" + v
                 if not os.path.isfile(pathdir) or replace_file:
-                    Print.print_inf(f"正在下载依赖库 {pathdir} ...")
-                    tasks.append(fetch(session, url))
-
-            results = await asyncio.gather(*tasks)
+                    Print.print_with_info(f"正在下载依赖库 {pathdir} ...", "§a 下载 §r")
+                    try:
+                        download_file_singlethreaded(url, pathdir)
+                    except Exception as err:
+                        Print.print_err(f"下载依赖库出现问题: {err}")
+                        self.update_status(SysStatus.CRASHED_EXIT)
+                        return
+            if replace_file:
+                # 写入commit_remote，文字写入
+                with open(commit_file_path, "w", encoding="utf-8") as f:
+                    f.write(commit_remote)
+                Print.print_suc("已完成依赖更新！")
 
-            for i, result in enumerate(results):
-                k = list(source_dict.keys())[i]
+        elif not self.TDC.SocketIO.connected:
+            try:
+                res = json.loads(
+                    requests.get(
+                        "https://mirror.ghproxy.com/https://raw.githubusercontent.com/ToolDelta/ToolDelta/main/require_files.json"
+                    ).text
+                )
+                use_mirror = res["Mirror"][0]
+            except Exception as err:
+                Print.print_err(f"获取依赖库表出现问题: {err}")
+                self.update_status(SysStatus.CRASHED_EXIT)
+                return
+            self.sys_machine = platform.machine().lower()
+            if self.sys_machine == "x86_64":
+                self.sys_machine = "amd64"
+            elif self.sys_machine == "aarch64":
+                self.sys_machine = "arm64"
+            if "TERMUX_VERSION" in os.environ:
+                sys_info_fmt = f"Android:{self.sys_machine.lower()}"
+            else:
+                sys_info_fmt = f"{platform.uname().system}:{self.sys_machine.lower()}"
+            source_dict = res[sys_info_fmt]
+            commit_file_path, commit_url = list(res["Commit"].items())[0]
+            commit_remote = requests.get(
+                use_mirror + "/raw.githubusercontent.com/" + commit_url
+            ).text
+            commit_local = ""
+            commit_file_path = os.path.join(os.getcwd(), commit_file_path)
+            replace_file = False
+            if os.path.isfile(commit_file_path):
+                with open(commit_file_path, "r", encoding="utf-8") as f:
+                    commit_local = f.read()
+                if commit_local != commit_remote:
+                    Print.print_war("依赖库版本过期, 将重新下载")
+                    replace_file = True
+            else:
+                replace_file = True
+            for k, v in source_dict.items():
                 pathdir = os.path.join(os.getcwd(), k)
-                if not os.path.exists(pathdir) or replace_file:
-                    with open(pathdir, "wb") as f:
-                        f.write(result)
-
-        if replace_file:
-            with open(commit_file_path, "wb") as f:
-                f.write(commit_remote)
-            Print.print_suc("已完成依赖更新！")
+                url = use_mirror + "/https://raw.githubusercontent.com/" + v
+                if not os.path.isfile(pathdir) or replace_file:
+                    Print.print_with_info(f"正在下载依赖库 {pathdir} ...", "§a 下载 §r")
+                    try:
+                        download_file_singlethreaded(url, pathdir)
+                    except Exception as err:
+                        Print.print_err(f"下载依赖库出现问题: {err}")
+                        self.update_status(SysStatus.CRASHED_EXIT)
+                        return
+            if replace_file:
+                # 写入commit_remote，文字写入
+                with open(commit_file_path, "w", encoding="utf-8") as f:
+                    f.write(commit_remote)
+                Print.print_suc("已完成依赖更新！")
 
     def get_players_and_uuids(self):
         players_uuid = {}
         for i in self.omega.get_all_online_players():
             players_uuid[i.name] = i.uuid
         return players_uuid
 
@@ -610,29 +641,106 @@
         if openat_port == 0:
             Print.print_war(
                 "未用启动参数指定链接neOmega接入点开放端口, 尝试使用默认端口 24015"
             )
             Print.print_inf("可使用启动参数 -access-point-port 端口 以指定接入点端口.")
             openat_port = 24015
             return SystemExit
-        Print.print_inf(f"将从端口 {openat_port} 连接至 neOmega 接入点.")
+        Print.print_inf(f"将从端口 {openat_port} 连接至接入点(等待接入中).")
         self.set_omega(openat_port)
-        Print.print_suc("已连接上 NEOMG 接入点进程.")
+        Print.print_suc("已连接上接入点进程.")
         pcks = [
             self.omega.get_packet_id_to_name_mapping(i)
             for i in self.need_listen_packets
         ]
         self.omega.listen_packets(pcks, self.packet_handler_parent)
         self._launcher_listener()
-        # bug expired
-        self.omega.listen_player_chat(lambda _, _2: None)
-        Print.print_suc("NEOMEGA 已就绪")
+        Print.print_suc("接入点已就绪")
         self.exit_event.wait()
         self.update_status(SysStatus.NORMAL_EXIT)
         if self.status == SysStatus.NORMAL_EXIT:
             return SystemExit("正常退出.")
         if self.status == SysStatus.CRASHED_EXIT:
-            return Exception("NeOmega 已崩溃")
+            return Exception("接入点已崩溃")
         return SystemError("未知的退出状态")
 
     def download_libs(self):
         Print.print_inf("以 Remote 启动, 将不会检查库完整性")
+
+class ToolDeltaCli(object):
+    def __init__(self, address: dict = {"host": "tdaus.tooldelta.fit", "port": 0}) -> None:
+    # def __init__(self, address: dict = {"host": "127.0.0.1", "port": 9002}) -> None:
+        self.NoPort:bool = address.get("port", 0) == 0
+        self.S_ADDRESSS:dict = address
+        self.protocol:str = "http"
+        self.url:str = f'{self.protocol}://{self.S_ADDRESSS["host"]}:{self.S_ADDRESSS["port"]}' if self.NoPort ==False else f'{self.protocol}://{self.S_ADDRESSS["host"]}'
+        self.SocketIO:socketio.Client = socketio.Client()
+        self.data_received_event:threading.Event = threading.Event()
+        self.connected_to_server:bool = True
+        threading.Thread(target=self.conn_aus, name="SocketIO_Conn").start()
+        while not self.SocketIO.connected and self.connected_to_server:time.sleep(0.1)
+
+    def init_auth_v(self) -> None:
+        self.feature_code:str = str(uuid.uuid5(uuid.NAMESPACE_DNS, str(time.perf_counter())))
+        self.token_ec:tuple= (self.feature_code, self.get_new_token())
+
+    def get_new_token(self) -> None:
+        try:
+            response = requests.post(url=f'{self.url}/api/signin', data=json.dumps({"feature_code": self.feature_code}), timeout= 5)
+            if response.status_code == 200:
+                return response.text
+        except requests.exceptions.ConnectionError as err:return "null"
+
+    def conn_aus(self) -> None:
+        try:
+            self.init_auth_v()
+            self.SocketIO.connect(self.url, namespaces='/api', headers={'Authorization': f'Bearer {self.token_ec[1]}'})
+            Print.print_suc("ToolDelta成功连接到至Api服务器[Socket-IO]!")
+            while True:
+                if not self.SocketIO.connected:
+                    try:
+                        self.init_auth_v()
+                        self.SocketIO.connect(self.url, namespaces='/api', headers={'Authorization': f'Bearer {self.token_ec[1]}'})
+                        Print.print_suc("ToolDelta与Api服务器断开连接,已重新连接成功!")
+                    except:
+                        Print.print_war("ToolDeltaApi服务器可能存在故障或当前网络环境异常，将停止使用ToolDeltaApi服务器!")
+                        break
+                time.sleep(10)
+        except Exception as err:
+            Print.print_war("ToolDelta无法连接至Api服务器,将停止使用其提供的功能!")
+            self.connected_to_server = False
+            threading.Thread(target=self.reconnect_to_server).start()
+
+    def reconnect_to_server(self, interval=20):
+        while not self.connected_to_server:
+            try:
+                self.init_auth_v()
+                self.SocketIO.connect(self.url, namespaces='/api', headers={'Authorization': f'Bearer {self.token_ec[1]}'})
+                Print.print_suc("ToolDelta成功重新连接至Api服务器!")
+                self.connected_to_server = True
+            except Exception as err:
+                time.sleep(interval)
+
+    def get_depends_table_data(self) -> dict:
+        if self.SocketIO.connected:
+            @self.SocketIO.on('depends_table_data', namespace='/api')
+            def handle_depends_table_data(data):
+                self.data_received_event.set()
+                self.depend_table_data = data
+            self.SocketIO.emit('get_depends_table', namespace='/api')
+            self.data_received_event.wait()  # 等待数据返回
+            self.data_received_event.clear()
+            return self.depend_table_data
+        else:
+            Print.print_war("Namespace /api is not connected yet. Please wait for connection.")
+
+    def get_version_updates(self) -> any:
+        if self.SocketIO.connected:
+            @self.SocketIO.on('version_updates', namespace='/api')
+            def handle_version_updates_data(data):
+                self.data_received_event.set()
+                self.latest_version_data = data
+
+            self.SocketIO.emit('get_version_update', namespace='/api')
+            self.data_received_event.wait()
+            self.data_received_event.clear()
+            return self.latest_version_data["latest_version_str"]
```

### Comparing `tooldelta-0.4.9/tooldelta/launch_options.py` & `tooldelta-0.5.0/tooldelta/launch_options.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from tooldelta.color_print import Print
 from tooldelta.starter import start_tool_delta
 from tooldelta.plugin_manager import plugin_manager
 from tooldelta.plugin_market import market
 from tooldelta.sys_args import sys_args_to_dict
 
 # TODO: 这是启动界面, 在此方法下写启动选项(启动ToolDelta, 插件管理, 插件市场)
@@ -20,7 +21,8 @@
             start_tool_delta()
         case "2":
             plugin_manager.manage_plugins()
         case "3":
             market.enter_plugin_market()
         case _:
             Print.clean_print("§c不合法的模式: " + r)
+    os._exit(0)
```

### Comparing `tooldelta-0.4.9/tooldelta/logger.py` & `tooldelta-0.5.0/tooldelta/logger.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.9/tooldelta/neo_libs/neo_conn.py` & `tooldelta-0.5.0/tooldelta/neo_libs/neo_conn.py`

 * *Files 5% similar despite different names*

```diff
@@ -555,54 +555,28 @@
         return int(LIB.PlayerEntityRuntimeID(self._c_uuid))
 
     @property
     def entity_metadata(self) -> any:
         OmegaAvailable()
         return json.loads(toPyString(LIB.PlayerEntityMetadata(self._c_uuid)))
 
-    def say(self, msg: str):
-        OmegaAvailable()
-        LIB.PlayerChat(self._c_uuid, toCString(msg))
-
-    def ask(self, hint: str) -> str:
-        OmegaAvailable()
-        self.say(hint)
-        return self.parent.intercept_player_just_next_input(self._c_uuid).RawMsg.strip()
-
-    def title(self, title: str = "", subtitle: str = ""):
-        # subtitle 只有在 title 给出时才能实际生效
-        LIB.PlayerTitle(self._c_uuid, toCString(title), toCString(subtitle))
-
-    def action_bar(self, msg: str):
-        LIB.PlayerActionBar(self._c_uuid, toCString(msg))
-
     def query(self, conditions: Union[None, str, List[str]] = None) -> CommandOutput:
         query_str = f'querytarget @a[name="{self.name}"'
         if conditions is None:
             query_str += "]"
         elif isinstance(conditions, str):
             query_str += "," + conditions + "]"
         else:
             query_str += "," + ",".join(conditions) + "]"
         ret = self.parent.send_websocket_command_need_response(query_str)
         return ret
 
     def check_conditions(self, conditions: Union[None, str, List[str]] = None) -> bool:
         return self.query(conditions).SuccessCount > 0
 
-    def get_pos(self) -> QueriedPlayerPos:
-        pos = self.query().OutputMessages[0].Parameters[0][0]
-        return QueriedPlayerPos(
-            dimension=pos["dimension"],
-            yRot=pos["yRot"],
-            x=pos["position"]["x"],
-            y=pos["position"]["y"],
-            z=pos["position"]["z"],
-        )
-
     def set_ability_map(
         self, action_permission: ActionPermissionMap, adventure_flag: AdventureFlagsMap
     ):
         jsonFlags = json.dumps(
             {
                 "AdventureFlagsMap": adventure_flag.__dict__,
                 "ActionPermissionMap": action_permission.__dict__,
@@ -665,37 +639,27 @@
         self._bot_basic_info = ClientMaintainedBotBasicInfo(
             **json.loads(toPyString(LIB.GetClientMaintainedBotBasicInfo()))
         )
 
         # player hooks
         self._bind_players: Dict[str, PlayerKit] = {}
 
-        # player chat intercept callbacks
-        self._player_chat_intercept_callback_retriever_counter = Counter(
-            "player_chat_intercept"
-        )
-        self._player_chat_intercept_callback_events: Dict[str, Callable] = {}
-
-        # chat
-        LIB.ListenChat()
-        self._player_chat_listeners: List[Callable[[Chat, PlayerKit], None]] = []
-        self._specific_chat_listeners: Dict[
-            str, List[Callable[[Chat, PlayerKit], None]]
-        ] = {}
-
         # named command block msg
         self._name_command_block_msg_listeners: Dict[
             str, List[Callable[[Chat], None]]
         ] = {}
 
         # start routine
         self.start_new(self._react)
 
     def start_new(self, func: Callable, args: Iterable[Any] = ()):
-        thread_i = next(self._thread_counter)
+        try:
+            thread_i = next(self._thread_counter)
+        except StopIteration:
+            raise ValueError("thread counter overflow")
 
         def clean_up(*args):
             try:
                 func(*args)
             except Exception:
                 print(traceback.print_exc(limit=None, file=None, chain=True))
             finally:
@@ -741,40 +705,18 @@
                     action = toPyString(LIB.ConsumePlayerChange())
                     for callback in self._player_change_listeners:
                         self.start_new(
                             callback, (self._get_bind_player(playerUUID), action)
                         )
 
             elif eventType == "PlayerInterceptInput":
-                chat = ConsumeChat()
-                self._player_chat_intercept_callback_events[retriever](chat)
+                OmitEvent()
 
             elif eventType == "Chat":
-                chat = ConsumeChat()
-                if (
-                    not self._player_chat_listeners
-                    and not self._specific_chat_listeners.get(chat.Name)
-                    and not self._specific_chat_listeners.get(chat.RawName)
-                ):
-                    LIB.OmitEvent()
-                else:
-                    player = self.get_player_by_name(chat.Name)
-                    if not player:
-                        name = chat.Name
-                        if name in self._specific_chat_listeners:
-                            for callback in self._specific_chat_listeners[name]:
-                                self.start_new(callback, (chat,))
-                        if chat.Name != chat.RawName:
-                            name = chat.RawName
-                            if name in self._specific_chat_listeners:
-                                for callback in self._specific_chat_listeners[name]:
-                                    self.start_new(callback, (chat,))
-                    else:
-                        for callback in self._player_chat_listeners:
-                            self.start_new(callback, (chat, player))
+                OmitEvent()
 
             elif eventType == "NamedCommandBlockMsg":
                 blockName = retriever
                 listeners = self._name_command_block_msg_listeners[blockName]
                 if len(listeners) == 0:
                     LIB.OmitEvent()
                 else:
@@ -803,26 +745,32 @@
 
         return result_setter, result_getter
 
     def send_websocket_command_need_response(
         self, cmd: str, timeout: int = -1
     ) -> Optional[CommandOutput]:
         setter, getter = self._create_lock_and_result_setter()
-        retriever_id = next(self._cmd_callback_retriever_counter)
+        try:
+            retriever_id = next(self._cmd_callback_retriever_counter)
+        except StopIteration:
+            raise ValueError("retriever counter overflow")
         self._omega_cmd_callback_events[retriever_id] = setter
         SendWebSocketCommandNeedResponse(cmd, retriever_id)
         res = getter(timeout=timeout)
         del self._omega_cmd_callback_events[retriever_id]
         return res
 
     def send_player_command_need_response(
         self, cmd: str, timeout: int = -1
     ) -> Optional[CommandOutput]:
         setter, getter = self._create_lock_and_result_setter()
-        retriever_id = next(self._cmd_callback_retriever_counter)
+        try:
+            retriever_id = next(self._cmd_callback_retriever_counter)
+        except StopIteration:
+            raise ValueError("retriever counter overflow")
         self._omega_cmd_callback_events[retriever_id] = setter
         SendPlayerCommandNeedResponse(cmd, retriever_id)
         res = getter(timeout=timeout)
         del self._omega_cmd_callback_events[retriever_id]
         return res
 
     @staticmethod
@@ -852,59 +800,31 @@
         if requires is None:
             return dict(self._packet_id_to_name_mapping.items())
         if isinstance(requires, list):
             return {k: self._packet_id_to_name_mapping[k] for k in requires}
         return self._packet_id_to_name_mapping[requires]
 
     def listen_packets(
-        self, targets: Union[str, List[str]], callback: Callable[[str, Any], None], clr_datas = False
+        self,
+        targets: Union[str | int, List[str]],
+        callback: Callable[[str, Any], None],
     ):
-        if clr_datas:
-            for k in self._packet_listeners.copy():
-                self._packet_listeners[k].clear()
+        for k in self._packet_listeners.copy():
+            self._packet_listeners[k].clear()
         if isinstance(targets, str):
             targets = [targets]
         if isinstance(targets, int):
             targets = [f"{targets}"]
-        translate_targets = {}
+        res = []
         for t in targets:
-            hit = False
-            if t == "all":
-                translate_targets = {
-                    k: True for k in self.get_packet_name_to_id_mapping().keys()
-                }
-                hit = True
-            elif t.startswith("!"):
-                rt = t[1:]
-                if rt in self._packet_name_to_id_mapping.keys():
-                    translate_targets[rt] = False
-                    hit = True
-                try:
-                    packetID = int(rt)
-                    packetType = self._packet_id_to_name_mapping(packetID)
-                    translate_targets[packetType] = False
-                    hit = True
-                except:
-                    pass
-            else:
-                if t in self._packet_name_to_id_mapping.keys():
-                    translate_targets[t] = True
-                    hit = True
-                try:
-                    packetID = int(t)
-                    packetType = self.get_packet_id_to_name_mapping(packetID)
-                    translate_targets[packetType] = True
-                    hit = True
-                except:
-                    pass
-            if not hit:
-                raise ValueError(f"{t}")
-        for k, v in translate_targets.items():
-            if v:
-                self._packet_listeners[k].append(callback)
+            if isinstance(t, int):
+                t = self.get_packet_id_to_name_mapping(t)
+            res.append(t)
+        for t in res:
+            self._packet_listeners[t].append(callback)
 
     def construct_game_packet_bytes_in_json_as_is(
         self, packet_type: Union[int, str], content: Any
     ) -> tuple[int, bytes]:
         if isinstance(packet_type, str):
             packet_type = self.get_packet_name_to_id_mapping(packet_type)
         return packet_type, JsonStrAsIsGamePacketBytes(packet_type, json.dumps(content))
@@ -967,35 +887,14 @@
         return self._get_bind_player(playerUUID)
 
     def listen_player_change(self, callback: Callable[[PlayerKit, str], None]):
         for player in self.get_all_online_players():
             callback(player, "exist")
         self._player_change_listeners.append(callback)
 
-    def intercept_player_just_next_input(
-        self, player_c_uuid: CString, timeout: int = -1
-    ) -> Chat:
-        setter, getter = self._create_lock_and_result_setter()
-        retrieverID = next(self._player_chat_intercept_callback_retriever_counter)
-        self._player_chat_intercept_callback_events[retrieverID] = setter
-        LIB.InterceptPlayerJustNextInput(player_c_uuid, toCString(retrieverID))
-        res = getter(timeout=timeout)
-        del self._player_chat_intercept_callback_events[retrieverID]
-        return res
-
-    def listen_player_chat(self, callback: Callable[[Chat, PlayerKit], None]):
-        self._player_chat_listeners.append(callback)
-
-    def listen_specific_chat(
-        self, specific_name: str, callback: Callable[[Chat], None]
-    ):
-        if specific_name not in self._specific_chat_listeners:
-            self._specific_chat_listeners[specific_name] = []
-        self._specific_chat_listeners[specific_name].append(callback)
-
     def listen_named_command_block(
         self, command_block_name: str, callback: Callable[[Chat], None]
     ):
         if command_block_name not in self._name_command_block_msg_listeners:
             self._name_command_block_msg_listeners[command_block_name] = []
         LIB.ListenCommandBlock(toCString(command_block_name))
         self._name_command_block_msg_listeners[command_block_name].append(callback)
```

### Comparing `tooldelta-0.4.9/tooldelta/packets.py` & `tooldelta-0.5.0/tooldelta/packets.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.9/tooldelta/plugin_load/PluginGroup.py` & `tooldelta-0.5.0/tooldelta/plugin_load/PluginGroup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,229 +1,220 @@
 import asyncio
 import importlib
 import threading
 import time
 import traceback
 from typing import Any, Callable, Type
 
-from tooldelta import constants
-from tooldelta.basic_mods import dotcs_module_env
 from tooldelta.color_print import Print
-from tooldelta.get_python_libs import get_single_lib
 from tooldelta.plugin_load.classic_plugin import Plugin
 from tooldelta.plugin_load import (
     classic_plugin,
-    dotcs_plugin,
     injected_plugin,
     NON_FUNC,
     NotValidPluginError,
     PluginAPINotFoundError,
-    PluginAPIVersionError
+    PluginAPIVersionError,
 )
 
+
 class PluginGroup:
     plugins: list[Plugin] = []
     plugins_funcs: dict[str, list] = {
         "on_def": [],
         "on_inject": [],
         "on_player_prejoin": [],
         "on_player_join": [],
         "on_player_message": [],
         "on_player_death": [],
         "on_player_leave": [],
     }
     plugin_added_cache = {"plugin": None, "packets": []}
     pluginAPI_added_cache = []
+    _broadcast_evts_cache = {}
 
     def __init__(self):
-        self.listen_packet_ids = set()
-        self.old_dotcs_env = {}
-        self.dotcs_global_vars = {}
-        self.packet_funcs: dict[str, list[Callable]] = {}
-        self.plugins_api: dict[str, Plugin] = {}
+        self._listen_packet_ids = set()
+        self._packet_funcs: dict[str, list[Callable]] = {}
+        self._plugins_api: dict[str, Plugin] = {}
+        self._broadcast_listeners: dict[str, list[Callable]] = {}
         self.excType = 0
-        self._broadcast_evts = {}
-        self.dotcs_plugin_loaded_num = 0
         self.normal_plugin_loaded_num = 0
         self.injected_plugin_loaded_num = 0
-        self.dotcs_repeat_threadings = {"1s": [], "10s": [], "30s": [], "1m": []}
         self.loaded_plugins_name = []
         self.linked_frame = None
 
-    def set_frame(self, frame):
-        self.linked_frame = frame
-
-    @staticmethod
-    def require(module_name: str, pip_name=""):
-        try:
-            importlib.import_module(module_name)
-        except (ModuleNotFoundError, ImportError):
-            get_single_lib(pip_name if pip_name else module_name)
-
-    def read_all_plugins(self):
-        try:
-            dotcs_plugin.read_plugins(self, dotcs_module_env)
-            classic_plugin.read_plugins(self)
-            self.execute_def(self.linked_frame.on_plugin_err)
-            asyncio.run(injected_plugin.load_plugin(self))
-        except Exception:
-            err_str = '\n'.join(traceback.format_exc().split('\n')[1:])
-            Print.print_err(f"加载插件出现问题: \n{err_str}")
-            raise SystemExit
-
-    @staticmethod
-    def load_plugin_hot(plugin_name: str, plugin_type: str):
-        plugin = None
-        if plugin_type == "dotcs":
-            Print.print_war("暂时无法热载入DotCS插件")
-        elif plugin_type == "classic":
-            plugin = classic_plugin.load_plugin(plugin_name, True)
-        elif plugin_type == "injected":
-            asyncio.run(injected_plugin.load_plugin_file(plugin_name))
-        if plugin is not None:
-            plugin.on_def()
-        Print.print_suc(f"成功热加载插件: {plugin_name}")
-
-    def add_broadcast_listener(self, evt_name: str):
-        "将下面的方法作为一个广播事件接收器"
-
-        def deco(func: Callable[[Any], bool]):
-            if self._broadcast_evts.get(evt_name):
-                self._broadcast_evts[evt_name].append(func)
-            else:
-                self._broadcast_evts[evt_name] = [func]
-        return deco
-
-    def broadcastEvt(self, evt_name: str, **kwargs) -> list[Any] | None:
-        "向全局广播一个特定事件, 可以传入附加信息参数"
-        callback_list = []
-        res = self._broadcast_evts.get(evt_name)
-        if res:
-            for f in res:
-                interrupt, *res2 = f(**kwargs)
-                if res2:
-                    callback_list.append(res2)
-                    if interrupt:
-                        break
-            return callback_list
-        return None
-
-    def test_plugin(self, plugin: Plugin):
-        if self.linked_frame is None:
-            # 很可能是直接单独运行此插件的代码.
-            Print.clean_print(f"插件主类信息({plugin.name}): ")
-            Print.clean_print(f" - 作者: {plugin.author}\n - 版本: {plugin.version}")
-            Print.clean_print(f" - 数据包监听: {', '.join(str(i) for i in self.listen_packet_ids)}")
-
     def add_plugin(self, plugin: Plugin):
         try:
             if not Plugin.__subclasscheck__(plugin):
                 raise NotValidPluginError(f"插件主类必须继承Plugin类 而不是 {plugin}")
         except TypeError:
             if not Plugin.__subclasscheck__(type(plugin)):
                 raise NotValidPluginError(
                     f"插件主类必须继承Plugin类 而不是 {plugin.__class__.__name__}"
                 )
         self.plugin_added_cache["plugin"] = plugin
         self.test_plugin(plugin)
         return plugin
 
-    def add_packet_listener(self, pktID):
+    def add_plugin_as_api(self, apiName: str):
+        def _add_plugin_2_api(api_plugin: Type[Plugin]):
+            if not Plugin.__subclasscheck__(api_plugin):
+                raise NotValidPluginError("API插件主类必须继承Plugin类")
+            self.plugin_added_cache["plugin"] = api_plugin
+            self.pluginAPI_added_cache.append(apiName)
+            self.test_plugin(api_plugin)
+            return api_plugin
+
+        return _add_plugin_2_api
+
+    def add_packet_listener(self, pktID: int | list[int]):
+        """
+        将下面的方法作为一个MC数据包接收器
+        装饰器参数:
+            pktID: int | list[int], 数据包ID或多个ID
+        接收器方法参数:
+            pkt: dict, 数据包包体
+        """
         def deco(func):
             if isinstance(pktID, int):
                 self.plugin_added_cache["packets"].append((pktID, func))
             else:
                 for i in pktID:
                     self.plugin_added_cache["packets"].append((i, func))
             return func
 
         return deco
 
-    def add_plugin_as_api(self, apiName: str):
-        def _add_plugin_2_api(api_plugin: Type[Plugin]):
-            if not Plugin.__subclasscheck__(api_plugin):
-                raise NotValidPluginError(
-                    "API插件主类必须继承Plugin类"
+    def add_broadcast_listener(self, evt_name: str):
+        """
+        将下面的方法作为一个广播事件接收器
+        装饰器参数:
+            evt_name: str, 事件类型
+        传入方法接受参数:
+            data: Any, 若事件带有附加参数, 则会传入附加参数, 否则传入None
+        返回参数: Any(返回的数据, 会被广播事件源收集, 默认None)
+        原理:
+        方法1 广播: hi, what's ur name? 附加参数=english_only
+            方法2 接收到广播并被执行: 方法2(english_only) -> my name is Super. -> 收集表
+        事件1 获取到 收集表 作为返回: ["my name is Super."]
+        """
+
+        def deco(func: Callable[[Any], bool]):
+            if self._broadcast_evts_cache.get(evt_name):
+                self._broadcast_evts_cache[evt_name].append(func)
+            else:
+                self._broadcast_evts_cache[evt_name] = [func]
+            return func
+
+        return deco
+
+    def broadcastEvt(self, evt_name: str, data: Any = None) -> list[Any] | None:
+        """
+        向全局广播一个特定事件, 可以传入附加信息参数
+        参数:
+            evt_name: str, 事件名
+            **kwargs: 附加信息参数
+        返回:
+            收集到的数据的列表(如果接收到广播的方法返回了数据的话)
+        """
+        callback_list = []
+        res = self._broadcast_listeners.get(evt_name)
+        if res:
+            for f in res:
+                res2 = f(data)
+                if res2:
+                    callback_list.append(res2)
+        return callback_list
+
+    def test_plugin(self, plugin: Plugin):
+        if self.linked_frame is None:
+            # 很可能是直接单独运行此插件的代码.
+            Print.clean_print(f"插件主类信息({plugin.name}): ")
+            Print.clean_print(f" - 作者: {plugin.author}\n - 版本: {plugin.version}")
+            Print.clean_print(
+                f" - 数据包监听: {', '.join(str(i) for i in self._listen_packet_ids)}"
+            )
+    @staticmethod
+    def help(plugin: Plugin):
+        """
+        查看插件帮助.
+        常用于查看 get_plugin_api() 方法获取到的插件实例的帮助.
+        """
+        plugin_docs = "<plugins.help>: " + plugin.name + "开放的API接口说明:\n"
+        for attr_name, attr in plugin.__dict__.items():
+            if not attr_name.startswith("__") and attr.__doc__ is not None:
+                plugin_docs += (
+                    "\n §a"
+                    + attr_name
+                    + ":§f\n    "
+                    + attr.__doc__.replace("\n", "\n    ")
                 )
-            self.plugin_added_cache["plugin"] = api_plugin
-            self.pluginAPI_added_cache.append(apiName)
-            self.test_plugin(api_plugin)
-            return api_plugin
+        Print.clean_print(plugin_docs)
 
-        return _add_plugin_2_api
+    def checkSystemVersion(self, need_vers: tuple[int, int, int]):
+        """检查ToolDelta系统的最低版本"""
+        if need_vers > self.linked_frame.sys_data.system_version:
+            raise self.linked_frame.SystemVersionException(
+                f"该组件需要{self.linked_frame.PRG_NAME}为{'.'.join([str(i) for i in self.linked_frame.sys_data.system_version])}版本"
+            )
 
-    def get_plugin_api(
-        self, apiName: str, min_version: tuple | None = None
-    ) -> Plugin:
-        api = self.plugins_api.get(apiName)
+    def get_plugin_api(self, apiName: str, min_version: tuple | None = None) -> Plugin:
+        """
+        通过插件API名获取插件实例
+        参数:
+            apiName: 插件API名
+            min_version: API最低版本(若不填则默认不检查最低版本)
+        """
+        api = self._plugins_api.get(apiName)
         if api:
             if min_version and api.version < min_version:
                 raise PluginAPIVersionError(apiName, min_version, api.version)
             return api
         raise PluginAPINotFoundError(f"无法找到API插件：{apiName}")
 
-    def checkSystemVersion(self, need_vers: tuple[int, int, int]):
-        if need_vers > self.linked_frame.sys_data.system_version:
-            raise self.linked_frame.SystemVersionException(
-                f"该组件需要{self.linked_frame.PRG_NAME}为{'.'.join([str(i) for i in self.linked_frame.sys_data.system_version])}版本"
-            )
+    def set_frame(self, frame):
+        self.linked_frame = frame
 
-    def add_listen_packet_id(self, packetType: int):
-        self.listen_packet_ids.add(packetType)
+    def read_all_plugins(self):
+        try:
+            classic_plugin.read_plugins(self)
+            self.execute_def(self.linked_frame.on_plugin_err)
+            asyncio.run(injected_plugin.load_plugin(self))
+        except Exception:
+            err_str = "\n".join(traceback.format_exc().split("\n")[1:])
+            Print.print_err(f"加载插件出现问题: \n{err_str}")
+            raise SystemExit
+
+    @staticmethod
+    def load_plugin_hot(plugin_name: str, plugin_type: str):
+        plugin = None
+        if plugin_type == "classic":
+            plugin = classic_plugin.load_plugin(plugin_name, True)
+        elif plugin_type == "injected":
+            asyncio.run(injected_plugin.load_plugin_file(plugin_name))
+        if plugin is not None:
+            plugin.on_def()
+        Print.print_suc(f"成功热加载插件: {plugin_name}")
+
+    def _add_listen_packet_id(self, packetType: int):
+        self._listen_packet_ids.add(packetType)
         self.linked_frame.link_game_ctrl.add_listen_pkt(packetType)
 
-    def add_listen_packet_func(self, packetType, func: Callable):
-        if self.packet_funcs.get(str(packetType)):
-            self.packet_funcs[str(packetType)].append(func)
+    def _add_listen_packet_func(self, packetType, func: Callable):
+        if self._packet_funcs.get(str(packetType)):
+            self._packet_funcs[str(packetType)].append(func)
         else:
-            self.packet_funcs[str(packetType)] = [func]
+            self._packet_funcs[str(packetType)] = [func]
 
-    def execute_dotcs_repeat(self):
-        "启动dotcs插件的循环执行模式插件事件"
-        threading.Thread(target=self.run_dotcs_repeat_funcs).start()
-
-    def run_dotcs_repeat_funcs(self):
-        lastTime10s = 0
-        lastTime30s = 0
-        lastTime1m = 0
-        if not any(self.dotcs_repeat_threadings.values()):
-            return
-        Print.print_inf(
-            f"开始运行 {sum(len(funcs) for funcs in self.dotcs_repeat_threadings.values())} 个原dotcs计划任务方法"
-        )
-        while 1:
-            time.sleep(1)
-            nowTime = time.time()
-            if nowTime - lastTime1m > 60:
-                for fname, func in self.dotcs_repeat_threadings["1m"]:
-                    try:
-                        # A strong desire to remove "try" block !!
-                        func()
-                    except Exception as err:
-                        Print.print_err(f"原dotcs插件 <{fname}> (计划任务1min)报错: {err}")
-                lastTime1m = nowTime
-            if nowTime - lastTime30s > 30:
-                for fname, func in self.dotcs_repeat_threadings["30s"]:
-                    try:
-                        func()
-                    except Exception as err:
-                        Print.print_err(f"原dotcs插件 <{fname}> (计划任务30s)报错: {err}")
-                lastTime30s = nowTime
-            if nowTime - lastTime10s > 10:
-                for fname, func in self.dotcs_repeat_threadings["10s"]:
-                    try:
-                        func()
-                    except Exception as err:
-                        Print.print_err(f"原dotcs插件 <{fname}> (计划任务10s)报错: {err}")
-                lastTime10s = nowTime
-            for fname, func in self.dotcs_repeat_threadings["1s"]:
-                try:
-                    func()
-                except Exception as err:
-                    Print.print_err(f"原dotcs插件 <{fname}> (计划任务1s) 报错: {err}")
+    def _add_broadcast_evt(self, evt, func):
+        if self._broadcast_listeners.get(evt):
+            self._broadcast_listeners[evt].append(func)
+        else:
+            self._broadcast_listeners[evt] = [func]
 
     def execute_def(self, onerr: Callable[[str, Exception, str], None] = NON_FUNC):
         for name, func in self.plugins_funcs["on_def"]:
             try:
                 func()
             except PluginAPINotFoundError as err:
                 Print.print_err(f"插件 {name} 需要包含该种接口的前置组件: {err.name}")
@@ -292,20 +283,21 @@
         for name, func in self.plugins_funcs["on_player_death"]:
             try:
                 func(player, killer, msg)
             except Exception as err:
                 onerr(name, err, traceback.format_exc())
 
     def processPacketFunc(self, pktID: int, pkt: dict):
-        d = self.packet_funcs.get(str(pktID))
+        d = self._packet_funcs.get(str(pktID))
         if d:
             for func in d:
                 try:
                     res = func(pkt)
                     if res:
                         return True
                 except:
                     Print.print_err(f"插件方法 {func.__name__} 出错：")
                     Print.print_err(traceback.format_exc())
         return False
 
+
 plugin_group = PluginGroup()
```

### Comparing `tooldelta-0.4.9/tooldelta/plugin_load/__init__.py` & `tooldelta-0.5.0/tooldelta/plugin_load/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,52 +15,54 @@
 class PluginAPIVersionError(ModuleNotFoundError):
     def __init__(self, name, m_ver, n_ver):
         self.name = name
         self.m_ver = m_ver
         self.n_ver = n_ver
 
 class PluginRegData:
+    # 插件注册信息类
     def __init__(self, name: str, plugin_data: dict = None, is_registered=True, is_enabled=True):
         if plugin_data is None:
             plugin_data = {}
         self.name: str = name
         if isinstance(plugin_data.get("version"), str):
             self.version: tuple = tuple(
                 int(i) for i in plugin_data.get("version", "0.0.0").split(".")
             )
         else:
             self.version = plugin_data.get("version", (0, 0, 0))
         self.author: str = plugin_data.get("author", "unknown")
         self.plugin_type: str = plugin_data.get("plugin-type", "unknown")
         self.description: str = plugin_data.get("description", "")
         self.pre_plugins: dict[str, str] = plugin_data.get("pre-plugins", [])
+        self.plugin_id = plugin_data.get("plugin-id", "???")
         self.is_registered = is_registered
         if plugin_data.get("enabled") is not None:
-            self.is_enabled = plugin_data.get("enabled")
+            self.is_enabled = plugin_data["enabled"]
         else:
             self.is_enabled = is_enabled
 
     def dump(self):
         return {
             "author": self.author,
             "version": ".".join([str(i) for i in self.version]),
             "plugin-type": self.plugin_type,
             "description": self.description,
             "pre-plugins": self.pre_plugins,
+            "plugin-id": self.plugin_id,
             "enabled": self.is_enabled
         }
 
     @property
     def version_str(self):
         return ".".join(str(i) for i in self.version)
 
     @property
     def plugin_type_str(self):
         return {
             "classic": "主类式",
             "injected": "注入式",
-            "dotcs": "DotCS",
             "unknown": "未知类型",
         }.get(self.plugin_type, "未知类型")
 
 def plugin_is_enabled(pname: str):
     return not pname.endswith("+disabled")
```

### Comparing `tooldelta-0.4.9/tooldelta/plugin_load/injected_plugin/__init__.py` & `tooldelta-0.5.0/tooldelta/plugin_load/injected_plugin/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 from dataclasses import dataclass
 import os
 import sys
 import importlib
 import threading
 
 from tooldelta.color_print import Print
-from tooldelta.plugin_manager import plugin_manager
 from tooldelta.plugin_load import (
-    plugin_is_enabled, 
-    PluginAPINotFoundError, 
+    plugin_is_enabled,
+    PluginAPINotFoundError,
     PluginAPIVersionError
 )
-
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from tooldelta.plugin_load.PluginGroup import PluginGroup
 
 # 定义插件处理函数列表
 player_message_funcs = {}
 player_prejoin_funcs = {}
 player_join_funcs = {}
 player_left_funcs = {}
 player_death_funcs = {}
@@ -181,17 +182,14 @@
         module_name = file
         sys.path.append(os.path.join("插件文件", "ToolDelta注入式插件"))
         plugin_module = importlib.import_module(module_name)
         meta_data = create_plugin_metadata(
             getattr(plugin_module, "__plugin_meta__", {"name": module_name})
         )
         # 获取插件元数据
-        plugin_manager.test_name_same(meta_data.name, file)
-        if not plugin_manager.plugin_is_registered("injected", meta_data.name):
-            plugin_manager.auto_register_plugin("injected", meta_data)
         return meta_data
     except PluginAPIVersionError as err:
         Print.print_err(f"插件 {file} 加载出现问题: 需要 {err.name} 的API最低版本为 {err.m_ver}, 实际上只有 {err.n_ver}")
         raise
     except PluginAPINotFoundError as err:
         Print.print_err(f"插件 {file} 加载出现问题: 需要前置插件API {err.name}")
         raise
@@ -221,32 +219,32 @@
     usage = metadata_dict.get("usage", "")
     author = metadata_dict.get("author", "未知")
     homepage = metadata_dict.get("homepage", "")
 
     return PluginMetadata(name, author, description, version, usage, homepage)
 
 
-async def load_plugin(plugin_grp):
+async def load_plugin(plugin_grp: "PluginGroup"):
     tasks = []
 
     # 读取本目录下的文件夹名字
     PLUGIN_PATH = os.path.join(os.getcwd(), "插件文件", "ToolDelta注入式插件")
     for file in os.listdir(PLUGIN_PATH):
         if not plugin_is_enabled(file):
             continue
         if os.path.isdir(os.path.join(PLUGIN_PATH, file)):
             plugin_grp.injected_plugin_loaded_num += 1
+            plugin_grp.loaded_plugins_name.append(file)
             task = asyncio.create_task(load_plugin_file(file))
             tasks.append(task)
 
     # 顺序加载插件并收集插件元数据
     all_plugin_metadata = []
     for task in tasks:
         plugin_metadata = await task
         all_plugin_metadata.append(plugin_metadata)
-        plugin_grp.loaded_plugins_name.append(file)
 
     # 打印所有插件的元数据
     for metadata in all_plugin_metadata:
         Print.print_suc(
             f"成功载入插件 {metadata.name} 版本: {metadata.version} 作者: {metadata.author}"
         )
```

### Comparing `tooldelta-0.4.9/tooldelta/plugin_load/injected_plugin/movent.py` & `tooldelta-0.5.0/tooldelta/plugin_load/injected_plugin/movent.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.4.9/tooldelta/plugin_manager.py` & `tooldelta-0.5.0/tooldelta/plugin_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,84 +1,43 @@
 import os
 import platform
 import shutil
-
+import shlex
+import json
 from tooldelta.builtins import Builtins
 from tooldelta.color_print import Print
 from tooldelta.plugin_market import market
+from tooldelta.plugin_load import PluginRegData
 from tooldelta.constants import (
-    TOOLDELTA_DOTCSEMU_PLUGIN,
+    TOOLDELTA_PLUGIN_DIR,
     TOOLDELTA_CLASSIC_PLUGIN,
     TOOLDELTA_INJECTED_PLUGIN
 )
 
 JsonIO = Builtins.SimpleJsonDataReader
 
 if platform.system().lower() == "windows":
     CLS_CMD = "cls"
 else:
     CLS_CMD = "clear"
 
-clear_screen = lambda: os.system(CLS_CMD)
-
-class PluginRegData:
-    # 插件注册信息类
-    def __init__(self, name: str, plugin_data: dict = None, is_registered=True, is_enabled=True):
-        if plugin_data is None:
-            plugin_data = {}
-        self.name: str = name
-        if isinstance(plugin_data.get("version"), str):
-            self.version: tuple = tuple(
-                int(i) for i in plugin_data.get("version", "0.0.0").split(".")
-            )
-        else:
-            self.version = plugin_data.get("version", (0, 0, 0))
-        self.author: str = plugin_data.get("author", "unknown")
-        self.plugin_type: str = plugin_data.get("plugin-type", "unknown")
-        self.description: str = plugin_data.get("description", "")
-        self.pre_plugins: dict[str, str] = plugin_data.get("pre-plugins", [])
-        self.is_registered = is_registered
-        if plugin_data.get("enabled") is not None:
-            self.is_enabled = plugin_data["enabled"]
-        else:
-            self.is_enabled = is_enabled
-
-    def dump(self):
-        return {
-            "author": self.author,
-            "version": ".".join([str(i) for i in self.version]),
-            "plugin-type": self.plugin_type,
-            "description": self.description,
-            "pre-plugins": self.pre_plugins,
-            "enabled": self.is_enabled
-        }
-
-    @property
-    def version_str(self):
-        return ".".join(str(i) for i in self.version)
-
-    @property
-    def plugin_type_str(self):
-        return {
-            "classic": "主类式",
-            "injected": "注入式",
-            "dotcs": "DotCS",
-            "unknown": "未知类型",
-        }.get(self.plugin_type, "未知类型")
-
+clear_screen = lambda: os.system(shlex.quote(CLS_CMD))
 
 class PluginManager:
     plugin_reg_data_path = "插件注册表"
-    default_reg_data = {"dotcs": {}, "classic": {}, "injected": {}, "unknown": {}}
+    default_reg_data = {"classic": {}, "injected": {}, "unknown": {}}
     _plugin_datas_cache = []
 
     def manage_plugins(self):
         # 进入插件管理界面
+        clear_screen()
+        np = self.register_plugins_auto()
+        if np > 0:
+            Print.clean_print(f"§a已自动注册{np}个未被注册的插件.")
         while 1:
-            clear_screen()
             plugins = self.list_plugins_list()
             Print.clean_print("§f输入§bu§f更新本地所有插件, §f输入§cq§f退出")
             r = input(Print.clean_fmt("§f输入插件关键词进行选择\n(空格可分隔关键词):"))
             if r.strip() == "":
                 continue
             if r.lower() == "q":
                 return
@@ -88,26 +47,26 @@
                 )
             else:
                 res = self.search_plugin(r, plugins)
                 if res is None:
                     input()
                 else:
                     self.plugin_operation(res)
+            clear_screen()
 
     def plugin_operation(self, plugin: PluginRegData):
         # 对插件进行操作
         description_fixed = plugin.description.replace('\n', '\n    ')
         clear_screen()
         Print.clean_print(f"§d插件名: §f{plugin.name}")
         Print.clean_print(f" - 版本: {plugin.version_str}")
         Print.clean_print(f" - 作者: {plugin.author}")
         Print.clean_print(f" 描述: {description_fixed}")
         Print.clean_print(f"§f1.删除插件  2.检查更新  3.{'禁用插件' if plugin.is_enabled else '启用插件'}")
         f_dirname = {
-            "dotcs": TOOLDELTA_DOTCSEMU_PLUGIN,
             "classic": TOOLDELTA_CLASSIC_PLUGIN,
             "injected": TOOLDELTA_INJECTED_PLUGIN
         }[plugin.plugin_type]
         match input(Print.clean_fmt("§f请选择选项: ")):
             case "1":
                 r = input(
                     Print.clean_fmt("§c删除插件操作不可逆, 请输入y, 其他取消: ")
@@ -119,15 +78,15 @@
                     plugin_dir + ("+disabled" if not plugin.is_enabled else "")
                 )
                 Print.clean_print(f"§a已成功删除插件 {plugin.name}, 回车键继续")
                 self.pop_plugin_reg_data(plugin)
                 input()
                 return
             case "2":
-                latest_version = market.get_latest_plugin_version(plugin.plugin_type, plugin.name)
+                latest_version = market.get_latest_plugin_version(plugin.plugin_id)
                 if latest_version is None:
                     Print.clean_print("§6无法获取其的最新版本, 回车键继续")
                 elif latest_version == plugin.version_str:
                     Print.clean_print("§a此插件已经为最新版本, 回车键继续")
                 else:
                     Print.clean_print(f"§a插件有新版本可用 ({plugin.version_str} => {latest_version})")
                     r = input(Print.clean_fmt("输入§a1§f=立刻更新, §62§f=取消更新: ")).strip()
@@ -154,24 +113,24 @@
         self.push_plugin_reg_data(plugin)
         input()
 
     def update_all_plugins(self, plugins: list[PluginRegData]):
         market_datas = self.latest_version = market.get_datas_from_market()["MarketPlugins"]
         need_updates: list[tuple[PluginRegData, str]] = []
         for i in plugins:
-            s_data = market_datas.get(i.name)
+            s_data = market_datas.get(i.plugin_id)
             if s_data is None:
                 continue
             if i.version_str != s_data["version"]:
                 need_updates.append((i, s_data["version"]))
         if need_updates:
             clear_screen()
             Print.clean_print("§f以下插件可进行更新:")
             for plugin, v in need_updates:
-                Print.clean_print(f" - {plugin.name} §6{i.version_str}§f -> §a{v}")
+                Print.clean_print(f" - {plugin.name} §6{plugin.version_str}§f -> §a{v}")
             r = input(Print.clean_fmt("§f输入§a y §f开始更新, §c n §f取消: ")).strip().lower()
             if r == "y":
                 for plugin, v in need_updates:
                     market.download_plugin(plugin, market_datas)
                 Print.clean_print("§a全部插件已更新完成")
             else:
                 Print.clean_print("§6已取消插件更新.")
@@ -199,64 +158,35 @@
     def search_plugin_by_kw(kws: list[str], plugins: list[PluginRegData]):
         res = []
         for plugin in plugins:
             if all(kw in plugin.name for kw in kws):
                 res.append(plugin)
         return res
 
-    def plugin_is_registered(self, plugin_type: str, plugin_name: str):
+    def plugin_is_registered(self, plugin_name: str):
         if not self._plugin_datas_cache:
             _, self._plugin_datas_cache = self.get_plugin_reg_name_dict_and_datas()
         for i in self._plugin_datas_cache:
-            if i.name == plugin_name and i.plugin_type == plugin_type:
+            if i.name == plugin_name:
                 return True
         return False
 
-    def auto_register_plugin(self, plugin_type, p_data):
-        # 自动注册插件信息, 不允许直接调用
-        match plugin_type:
-            case "classic":
-                self.push_plugin_reg_data(
-                    PluginRegData(
-                        p_data.name,
-                        {
-                            "name": p_data.name,
-                            "author": p_data.author,
-                            "version": p_data.version,
-                            "plugin-type": "classic",
-                        },
-                    )
-                )
-            case "injected":
-                self.push_plugin_reg_data(
-                    PluginRegData(
-                        p_data.name,
-                        {
-                            "name": p_data.name,
-                            "author": p_data.author,
-                            "version": p_data.version,
-                            "description": p_data.description,
-                            "plugin-type": "injected",
-                        },
-                    )
-                )
-            case "dotcs":
-                assert isinstance(p_data, dict), "Not a valid dotcs plugin"
-                self.push_plugin_reg_data(
-                    PluginRegData(
-                        p_data.get("name", "未命名插件"),
-                        {
-                            "name": p_data.get("name", "未命名插件"),
-                            "author": p_data.get("author", "unknown"),
-                            "plugin-type": "dotcs",
-                        },
-                    )
-                )
-            case _:
-                Print.print_err("不合法的注册插件: " + plugin_type)
+    def register_plugins_auto(self):
+        dirs = [TOOLDELTA_CLASSIC_PLUGIN, TOOLDELTA_INJECTED_PLUGIN]
+        any_plugin_registered = 0
+        for f_dir in dirs:
+            dirs_type = {TOOLDELTA_CLASSIC_PLUGIN: "classic", TOOLDELTA_INJECTED_PLUGIN: "injected"}[f_dir]
+            for plugin_path in os.listdir(os.path.join(TOOLDELTA_PLUGIN_DIR, f_dir)):
+                datpath = os.path.join(TOOLDELTA_PLUGIN_DIR, f_dir, plugin_path, "datas.json")
+                if not self.plugin_is_registered(dirs_type) and os.path.isfile(datpath):
+                    with open(datpath, "r", encoding="utf-8") as f:
+                        jsdata = json.load(f)
+                        self.push_plugin_reg_data(PluginRegData(plugin_path, jsdata))
+                        any_plugin_registered += 1
+        return any_plugin_registered
 
     def push_plugin_reg_data(self, plugin_data: PluginRegData):
         # 向插件注册表推送插件注册信息
         r = JsonIO.readFileFrom(
             "主系统核心数据", self.plugin_reg_data_path, self.default_reg_data
         )
         r[plugin_data.plugin_type][plugin_data.name] = plugin_data.dump()
@@ -266,53 +196,54 @@
         # 从插件注册表删除插件注册信息
         r = JsonIO.readFileFrom("主系统核心数据", self.plugin_reg_data_path)
         del r[plugin_data.plugin_type][plugin_data.name]
         JsonIO.writeFileTo("主系统核心数据", self.plugin_reg_data_path, r)
 
     def get_plugin_reg_name_dict_and_datas(self):
         # 返回一个表示插件所在类别下的全部已注册插件的列表, 和全部已注册插件的插件注册信息列表
-        r0: dict[str, list[str]] = {"dotcs": [], "classic": [], "injected": []}
+        r0: dict[str, list[str]] = {"classic": [], "injected": []}
         r = JsonIO.readFileFrom(
             "主系统核心数据", self.plugin_reg_data_path, self.default_reg_data
         )
         f_dirname = {
-            "dotcs": TOOLDELTA_DOTCSEMU_PLUGIN,
             "classic": TOOLDELTA_CLASSIC_PLUGIN,
             "injected": TOOLDELTA_INJECTED_PLUGIN
         }
         res: list[PluginRegData] = []
         for _, r1 in r.items():
             for k, v in r1.items():
                 if not isinstance(k, str) or not isinstance(v, dict):
                     raise ValueError(
                         f"获取插件注册表出现问题: 类型出错: {k.__class__.__name__}, {v.__class__.__name__}"
                     )
                 v.update({"name": k})
                 p = PluginRegData(k, v)
-                if os.path.exists(os.path.join("插件文件", f_dirname[p.plugin_type], p.name)):
+                if (
+                    os.path.exists(os.path.join("插件文件", f_dirname[p.plugin_type], p.name))
+                    or os.path.exists(os.path.join("插件文件", f_dirname[p.plugin_type], p.name + "+disabled"))
+                ):
                     res.append(p)
                     r0[p.plugin_type].append(p.name)
         return r0, res
 
     def get_2_compare_plugins_reg(self):
         # 返回一个全注册插件的列表
         f_plugins: list[PluginRegData] = []
         reg_dict, reg_list = self.get_plugin_reg_name_dict_and_datas()
         for p, k in {
-            TOOLDELTA_DOTCSEMU_PLUGIN: "dotcs",
             TOOLDELTA_CLASSIC_PLUGIN: "classic",
             TOOLDELTA_INJECTED_PLUGIN: "injected",
         }.items():
             for i in os.listdir(os.path.join("插件文件", p)):
                 if i.replace("+disabled", "") not in reg_dict[k]:
                     f_plugins.append(PluginRegData(i, {"plugin-type": k}, False))
         return f_plugins + reg_list
     @staticmethod
     def make_plugin_icon(plugin: PluginRegData):
-        ico_colors = {"dotcs": "§6", "classic": "§b", "injected": "§d"}
+        ico_colors = { "classic": "§b", "injected": "§d"}
         return (
             ico_colors.get(plugin.plugin_type, "§7")
             + "■ "
             + (("§a"if plugin.is_enabled else "§7") if plugin.is_registered else "§6")
             + plugin.name
         )
```

### Comparing `tooldelta-0.4.9/tooldelta/plugin_market.py` & `tooldelta-0.5.0/tooldelta/plugin_market.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 import json
 import os
 import platform
 import shutil
 import tempfile
 import traceback
 import time
+import shlex
 from tooldelta import urlmethod
 from tooldelta.builtins import Builtins
 from tooldelta.color_print import Print
 from tooldelta.plugin_load import PluginRegData
 from tooldelta.cfg import Cfg
 from tooldelta.constants import (
     PLUGIN_MARKET_SOURCE_OFFICIAL,
     TOOLDELTA_CLASSIC_PLUGIN,
-    TOOLDELTA_DOTCSEMU_PLUGIN,
     TOOLDELTA_INJECTED_PLUGIN
 )
 from typing import Dict
 
 if platform.system().lower() == "windows":
     CLS_CMD = "cls"
 else:
     CLS_CMD = "clear"
 
-clear_screen = lambda: os.system(CLS_CMD)
+clear_screen = lambda: os.system(shlex.quote(CLS_CMD))
 
 
 def _path_dir(path: str):
     if "/" not in path:
         return None
     return "/".join(path.split("/")[:-1])
 
@@ -45,38 +45,47 @@
     try:
         return json.loads(resp)
     except json.JSONDecodeError:
         raise Exception(f"服务器返回了不正确的答复: {resp}")
 
 
 class PluginMarket:
+    plugin_id_name_map = None
     def enter_plugin_market(self, source_url: str = None, in_game = False):
         Print.clean_print("§6正在连接到插件市场..")
+        CTXS = 12
         try:
             market_datas = self.get_datas_from_market(source_url)
+            plugin_ids_map = self.get_plugin_id_name_map()
             plugins_list = list(market_datas["MarketPlugins"].items())
             all_indexes = len(plugins_list)
             now_index = 0
-            sum_pages = int((all_indexes - 1) / 8) + 1
+            sum_pages = int((all_indexes - 1) / CTXS) + 1
             now_page = 0
             last_operation = ""
             while True:
                 clear_screen()
                 Print.print_inf(
                     market_datas["SourceName"] + ": " + market_datas["Greetings"],
                     need_log=False
                 )
-                now_page = int(now_index / 8) + 1
-                for i in range(now_index, now_index + 8):
+                now_page = int(now_index / CTXS) + 1
+                for i in range(now_index, now_index + CTXS):
                     if i in range(all_indexes):
-                        plugin_data = PluginRegData(
-                            plugins_list[i][0], plugins_list[i][1]
-                        )
+                        plugin_id = plugins_list[i][0]
+                        plugin_name = plugin_ids_map[plugin_id]
+                        plugin_basic_datas = plugins_list[i][1]
+                        if plugin_basic_datas['plugin-type'] == "classic":
+                            plugin_type = "类式"
+                        elif plugin_basic_datas['plugin-type'] == "injected":
+                            plugin_type = "注入式"
+                        else:
+                            plugin_type = plugin_basic_datas['plugin-type']
                         Print.print_inf(
-                            f" {i + 1}. §e{plugin_data.name} §av{plugin_data.version_str} §b@{plugin_data.author} §d{plugin_data.plugin_type_str}插件",
+                            f" {i + 1}. §e{plugin_name} §av{plugin_basic_datas['version']} §b@{plugin_basic_datas['author']} §d{plugin_type}插件",
                             need_log=False
                         )
                     else:
                         Print.print_inf("")
                 Print.print_inf(f"§f第 {now_page} / {sum_pages} 页, 输入 §b+§f/§b- §f翻页", need_log=False)
                 Print.print_inf("§f输入插件序号选中插件并查看其下载页", need_log=False)
                 last_operation = (
@@ -84,26 +93,24 @@
                         input(Print.fmt_info("§f回车键继续上次操作, §bq§f退出, 请输入:", "§f 输入 "))
                         or last_operation
                     )
                     .lower()
                     .strip()
                 )
                 if last_operation == "+":
-                    now_index += 8
+                    now_index += CTXS
                 elif last_operation == "-":
-                    now_index -= 8
+                    now_index -= CTXS
                 elif last_operation == "q":
                     break
                 else:
                     res = Builtins.try_int(last_operation)
                     if res:
                         if res in range(1, all_indexes + 1):
-                            plugin_data = PluginRegData(
-                                plugins_list[res - 1][0], plugins_list[res - 1][1]
-                            )
+                            plugin_data = self.get_plugin_data_from_market(plugins_list[res - 1][0])
                             ok, pres = self.choice_plugin(
                                 plugin_data,
                                 market_datas["MarketPlugins"],
                             )
                             if ok:
                                 if in_game:
                                     from tooldelta.plugin_load.PluginGroup import plugin_group
@@ -130,37 +137,45 @@
                                 Print.print_inf("已取消.", need_log=False)
                                 time.sleep(1)
                         else:
                             Print.print_err("超出序号范围")
                 if now_index >= all_indexes:
                     now_index = 0
                 elif now_index < 0:
-                    now_index = max(all_indexes - 8, 0)
+                    now_index = max(now_index - CTXS, 0)
         except KeyError as err:
             Print.print_err(f"获取插件市场插件出现问题: 键值对错误: {err}")
             return
         except requests.RequestException as err:
             Print.print_err(f"获取插件市场插件出现问题: {err}")
             return
         except Exception as err:
-            Print.print_err("获取插件市场插件出现问题")
+            Print.print_err("获取插件市场插件出现问题, 报错如下:")
             Print.print_err(traceback.format_exc())
             return
         clear_screen()
         Print.clean_print("§a已从插件市场返回 ToolDelta 控制台.")
 
     def get_datas_from_market(self, source_url: str = None):
         if source_url is None:
             source_url = Cfg().get_cfg("ToolDelta基本配置.json", {"插件市场源": str})["插件市场源"]
         market_datas = _get_json_from_url(
             _url_join(source_url, "market_tree.json")
         )
         self.plugins_download_url = market_datas["DownloadRefURL"]
         return market_datas
 
+    def get_plugin_data_from_market(self, plugin_id: str):
+        plugin_name = self.plugin_id_name_map[plugin_id]
+        data_url = self.plugins_download_url + "/" + plugin_name + "/datas.json"
+        res = requests.get(data_url)
+        res.raise_for_status()
+        datas = json.loads(res.text)
+        return PluginRegData(plugin_name, datas)
+
     def choice_plugin(self, plugin_data: PluginRegData, all_plugins_dict: dict):
         pre_plugins_str = (
             ", ".join([f"{k}§7v{v}" for k, v in plugin_data.pre_plugins.items()]) or "无"
         )
         clear_screen()
         Print.print_inf(
             f"{plugin_data.name} v{plugin_data.version_str}", need_log=False
@@ -175,45 +190,48 @@
         res = input(Print.fmt_info("§f下载 = §aY§f, 取消 = §cN§f, 请输入:")).lower().strip()
         if res == "y":
             pres = self.download_plugin(plugin_data, all_plugins_dict)
             pres.reverse()
             return True, pres
         return False, None
 
+    def get_plugin_id_name_map(self):
+        res = requests.get(PLUGIN_MARKET_SOURCE_OFFICIAL + "/plugin_ids_map.json")
+        res.raise_for_status()
+        res1 = json.loads(res.text)
+        self.plugin_id_name_map = res1
+        return res1
+
     def download_plugin(
         self,
         plugin_data: PluginRegData,
         all_plugins_dict: Dict[str, str],
     ):
         pres = [plugin_data]
         download_paths = self.find_dirs(plugin_data)
-        for plugin_name in plugin_data.pre_plugins:
-            Print.print_inf(f"正在下载 {plugin_data.name} 的前置插件 {plugin_name}")
+        for plugin_id in plugin_data.pre_plugins:
+            plugin_name = self.plugin_id_name_map[plugin_id]
+            Print.clean_print(f"正在下载 {plugin_data.name} 的前置插件 {plugin_name}")
             pres += self.download_plugin(
-                PluginRegData(plugin_name, all_plugins_dict[plugin_name]),
+                PluginRegData(plugin_name, all_plugins_dict[plugin_id]),
                 all_plugins_dict,
             )
         cache_dir = tempfile.mkdtemp()
         try:
             for paths in download_paths:
                 if not paths.strip():
-                    # 不可能出现的状况, 出现了证明是你的问题
                     Print.print_war("下载路径为空, 跳过")
                     continue
                 url = _url_join(self.plugins_download_url, paths)
                 # Determine download path based on plugin type
                 match plugin_data.plugin_type:
                     case "classic":
                         download_path = os.path.join(
                             "插件文件", TOOLDELTA_CLASSIC_PLUGIN
                         )
-                    case "dotcs":
-                        download_path = os.path.join(
-                            "插件文件", TOOLDELTA_DOTCSEMU_PLUGIN
-                        )
                     case "injected":
                         download_path = os.path.join(
                             "插件文件", TOOLDELTA_INJECTED_PLUGIN
                         )
                     case _:
                         raise Exception(
                             f"未知插件类型: {plugin_data.plugin_type}, 你可能需要通知ToolDelta项目开发组解决"
@@ -224,27 +242,26 @@
                     # 自动创建文件夹
                     folder_path = os.path.join(cache_dir, path_last)
                     os.makedirs(folder_path, exist_ok=True)
                 urlmethod.download_unknown_file(url, os.path.join(cache_dir, paths))
             # Move downloaded files to target download path
             target_path = download_path
             os.makedirs(target_path, exist_ok=True)
+            # 制作所需的目录结构
             for root, _, files in os.walk(cache_dir):
                 for filename in files:
                     source_file = os.path.join(root, filename)
                     target_file = os.path.join(
                         target_path, os.path.relpath(source_file, cache_dir)
                     )
                     os.makedirs(os.path.dirname(target_file), exist_ok=True)
                     shutil.move(source_file, target_file)
             from tooldelta.plugin_manager import plugin_manager
             # 注册插件
-            plugin_manager.push_plugin_reg_data(PluginRegData(
-                plugin_data.name, all_plugins_dict[plugin_data.name]
-            ))
+            plugin_manager.push_plugin_reg_data(self.get_plugin_data_from_market(plugin_data.plugin_id))
             Print.clean_print(f"§a成功下载插件 §f{plugin_data.name}§a 至插件文件夹")
         finally:
             shutil.rmtree(cache_dir)
         return pres
 
     def find_dirs(self, plugin_data: PluginRegData):
         try:
@@ -262,17 +279,17 @@
             Print.print_err(f"获取插件市场插件目录结构出现问题: 无法找到 {err}, 有可能是未来得及更新目录")
             return
         except Exception as err:
             Print.print_err(f"获取插件市场插件目录结构出现问题: {err}")
             return
 
     @staticmethod
-    def get_latest_plugin_version(plugin_type: str, plugin_name: str):
+    def get_latest_plugin_version(plugin_id: str):
         try:
             src_url = Cfg().get_cfg("ToolDelta基本配置.json", {"插件市场源": str})["插件市场源"]
         except:
             src_url = PLUGIN_MARKET_SOURCE_OFFICIAL
         return _get_json_from_url(
             _url_join(src_url, "latest_versions.json")
-        )[plugin_type + "_plugin"].get(plugin_name)
+        ).get(plugin_id)
 
 market = PluginMarket()
```

### Comparing `tooldelta-0.4.9/tooldelta/starter.py` & `tooldelta-0.5.0/tooldelta/starter.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,40 +15,40 @@
     # 排除信号中断
     pass
 signal.signal(signal.SIGINT, signal_handler)
 
 def start_tool_delta():
     # 初始化系统
     try:
-        # TODO: 自动更新需要时间间隔
-        builtins.Builtins.createThread(frame.ToolDeltaUpdater, usage="Auto_update")
         frame.welcome()
         frame.basic_operation()
         frame.set_game_control(game_control)
         frame.set_plugin_group(plugin_group)
         movent.set_frame(frame)
         frame.read_cfg()
         game_control.init_funcs()
         plugin_group.read_all_plugins()
         frame.plugin_load_finished(plugin_group)
         builtins.tmpjson_save_thread()
         frame.launcher.listen_launched(game_control.Inject)
         game_control.set_listen_packets()
+        # TODO: 自动更新需要时间间隔
+        builtins.Builtins.createThread(frame.ToolDeltaUpdater, usage="自动更新 ToolDelta", launcher = frame.launcher)
         raise frame.launcher.launch()
     except (KeyboardInterrupt, SystemExit):
         pass
     except:
         Print.print_err("ToolDelta 运行过程中出现问题: " + traceback.format_exc())
 
 
 def safe_jump(*, out_task=True, exit_directly=True):
     if out_task:
         frame.system_exit()
     frame.safe_close()
     if exit_directly:
-        for _ in range(3, 0, -1):
+        for _ in range(2, 0, -1):
             Print.print_war(f"{_}秒后强制退出...", end="\r")
             time.sleep(1)
         Print.print_war("0秒后强制退出...", end="\r")
         Print.print_suc("ToolDelta 已退出.")
         os._exit(0)
     Print.print_suc("ToolDelta 已退出.")
```

### Comparing `tooldelta-0.4.9/tooldelta/sys_args.py` & `tooldelta-0.5.0/tooldelta/sys_args.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,8 @@
                     val = None
                 else:
                     i += 1
             except IndexError:
                 val = None
             d[arg] = val
         i += 1
-    return d
+    return d
```

### Comparing `tooldelta-0.4.9/tooldelta/urlmethod.py` & `tooldelta-0.5.0/tooldelta/urlmethod.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,32 +6,50 @@
 import time
 from typing import Union
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from tqdm import tqdm
 import pyspeedtest
 import requests
 
-from .color_print import Print
+from tooldelta.color_print import Print
 
+def progress_bar(
+    current: float | int, total: float | int, length = 20, color1="§f", color2="§b"
+):
+    pc = round(current / total * length)
+    return Print.colormode_replace(
+        color1 + " " * pc + color2 + " " * (20 - pc) + "§r ", 7
+    )
+
+def download_progress_bar(
+    current_bytes: int, total_bytes: int, speed = 0
+):
+    bar = progress_bar(current_bytes, total_bytes)
+    b = f"{bar} {_pretty_kb(current_bytes)}B / {_pretty_kb(total_bytes)}B"
+    if speed != 0:
+        b += f"{_pretty_kb(speed)}B/s)    "
+    Print.print_with_info(b, "§a 下载 ", need_log=False, end = "\r")
 
 def _pretty_kb(n: int) -> str:
     if n >= 1048576:
         return f"{round(n / 1048576, 2)}M"
     if n >= 1024:
         return f"{round(n / 1024, 2)}K"
     return f"{round(n, 1)}"
 
 
 def _path_get_filename(path: str) -> Union[str, None]:
+    "从路径中获取最末尾的文件夹/文件名."
     if "/" not in path:
         return None
     return path.split("/")[-1]
 
 
 def _is_common_text_file(url_path: str) -> bool:
+    "是否为正常的文本文件(常见的)."
     return any(
         url_path.endswith(i)
         for i in [".txt", ".yml", ".md", ".xml", ".py", ".h", ".c", ".pyi", ".json"]
     )
 
 
 def get_file_size(url: str) -> Union[int, None]:
@@ -60,47 +78,37 @@
 ) -> None:
     with requests.get(url, stream=True, timeout=10) as res:
         res.raise_for_status()
         filesize = get_file_size(url)
         try:
             if filesize < 256 and not ignore_warnings:
                 Print.print_war(f"下载 {url} 的文件警告: 文件大小异常, 不到 0.25KB")
-        except TypeError:pass
+        except TypeError:
+            pass
         chunk_size = 8192
         nowsize = 0
         succ = False
         lastime = time.time()
         useSpeed = 0
         with open(save_dir + ".tmp", "wb") as dwnf:
-            for chk in res.iter_content(chunk_size=8192):
+            for chk in res.iter_content(chunk_size):
                 nowtime = time.time()
                 if nowtime != lastime:
                     useSpeed = chunk_size / (nowtime - lastime)
                     lastime = nowtime
                 nowsize += len(chk)
                 dwnf.write(chk)
                 if nowsize % 81920 == 0:  # 每下载 10 个数据块更新一次进度
-                    prgs = nowsize / filesize
-                    _tmp = int(prgs * 20)
-                    bar = Print.colormode_replace(
-                        "§f" + " " * _tmp + "§b" + " " * (20 - _tmp) + "§r ", 7
-                    )
-                    Print.print_with_info(
-                        f"{bar} {_pretty_kb(nowsize)}B / {_pretty_kb(filesize)}B ({_pretty_kb(useSpeed)}B/s)    ",
-                        "§a 下载 §r",
-                        end="\r",
-                        need_log=False,
-                    )
+                    download_progress_bar(nowsize, filesize, useSpeed)
         succ = True
         if succ:
             shutil.move(save_dir + ".tmp", save_dir)
         else:
             os.remove(save_dir + ".tmp")
 
-
 def download_file_multithreading(
     url: str, save_dir: str, num_threads: int = 8, ignore_warnings: bool = False
 ):
     filesize = get_file_size(url)
     if filesize is None:
         download_file_singlethreaded(url=url, save_dir=save_dir)
     if filesize < 256 and not ignore_warnings:
@@ -134,19 +142,24 @@
             for future in futures:
                 future.result()
     shutil.move(save_dir + ".tmp", save_dir)
 
 
 def download_unknown_file(url: str, save_dir: str) -> None:
     # 鉴于 Content-Length 不一定表示文件原始大小, 二进制文件与文本文件需要分开下载
+    # 否则显示的下载条会异常
     resp = requests.get(url, timeout=10)
     resp.raise_for_status()
-
-    with open(save_dir, "wb") as f:
-        f.write(resp.content)
+    # Bad..
+    if _is_common_text_file(save_dir):
+        # 文本文件, 体积可能不大
+        with open(save_dir, "wb") as f:
+            f.write(resp.content)
+    else:
+        download_file_singlethreaded(url, save_dir)
 
 def test_site_latency(Da: dict) -> list:
     tmp_speed = {}
     urls = [Da["url"]] + Da["mirror_url"]
 
     with ThreadPoolExecutor() as executor:
         futures = [executor.submit(measure_latencyt, url) for url in urls]
```

