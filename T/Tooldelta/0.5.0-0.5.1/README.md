# Comparing `tmp/tooldelta-0.5.0.tar.gz` & `tmp/tooldelta-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tooldelta-0.5.0.tar", max compression
+gzip compressed data, was "tooldelta-0.5.1.tar", max compression
```

## Comparing `tooldelta-0.5.0.tar` & `tooldelta-0.5.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rwxr-xr-x   0        0        0     1497 2024-04-13 22:20:49.851509 tooldelta-0.5.0/LICENSE
--rwxr-xr-x   0        0        0     2504 2024-04-13 22:20:49.851509 tooldelta-0.5.0/README.md
--rwxr-xr-x   0        0        0      929 2024-04-13 22:20:57.339327 tooldelta-0.5.0/pyproject.toml
--rwxr-xr-x   0        0        0      330 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/__init__.py
--rw-r--r--   0        0        0     5906 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/auths.py
--rwxr-xr-x   0        0        0      599 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/basic_mods.py
--rwxr-xr-x   0        0        0    16782 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/builtins.py
--rwxr-xr-x   0        0        0    10594 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/cfg.py
--rwxr-xr-x   0        0        0     7848 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/color_print.py
--rw-r--r--   0        0        0     1960 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/constants.py
--rw-r--r--   0        0        0     5870 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/fb_conn/fbconn.py
--rwxr-xr-x   0        0        0    34048 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/frame.py
--rwxr-xr-x   0        0        0     3772 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/game_texts.py
--rwxr-xr-x   0        0        0      338 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/get_tool_delta_version.py
--rwxr-xr-x   0        0        0    32194 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/launch_cli.py
--rwxr-xr-x   0        0        0     1080 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/launch_options.py
--rwxr-xr-x   0        0        0     2138 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/logger.py
--rwxr-xr-x   0        0        0    29503 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/neo_libs/neo_conn.py
--rwxr-xr-x   0        0        0     1143 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/packets.py
--rwxr-xr-x   0        0        0    11373 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/plugin_load/PluginGroup.py
--rwxr-xr-x   0        0        0     2273 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/plugin_load/__init__.py
--rwxr-xr-x   0        0        0     6200 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/plugin_load/classic_plugin/__init__.py
--rwxr-xr-x   0        0        0      345 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/plugin_load/funcs.py
--rwxr-xr-x   0        0        0     6780 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/plugin_load/injected_plugin/__init__.py
--rwxr-xr-x   0        0        0     9235 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/plugin_load/injected_plugin/movent.py
--rwxr-xr-x   0        0        0    12447 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/plugin_manager.py
--rwxr-xr-x   0        0        0    13218 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/plugin_market.py
--rw-r--r--   0        0        0     1860 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/starter.py
--rwxr-xr-x   0        0        0      638 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/sys_args.py
--rwxr-xr-x   0        0        0     7057 2024-04-13 22:20:49.855509 tooldelta-0.5.0/tooldelta/urlmethod.py
--rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 tooldelta-0.5.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1497 2024-04-14 05:48:28.812056 tooldelta-0.5.1/LICENSE
+-rwxr-xr-x   0        0        0     2504 2024-04-14 05:48:28.812056 tooldelta-0.5.1/README.md
+-rwxr-xr-x   0        0        0      929 2024-04-14 05:48:40.952010 tooldelta-0.5.1/pyproject.toml
+-rwxr-xr-x   0        0        0      330 2024-04-14 05:48:28.812056 tooldelta-0.5.1/tooldelta/__init__.py
+-rw-r--r--   0        0        0     5906 2024-04-14 05:48:28.812056 tooldelta-0.5.1/tooldelta/auths.py
+-rwxr-xr-x   0        0        0      599 2024-04-14 05:48:28.812056 tooldelta-0.5.1/tooldelta/basic_mods.py
+-rwxr-xr-x   0        0        0    16782 2024-04-14 05:48:28.812056 tooldelta-0.5.1/tooldelta/builtins.py
+-rwxr-xr-x   0        0        0    10594 2024-04-14 05:48:28.812056 tooldelta-0.5.1/tooldelta/cfg.py
+-rwxr-xr-x   0        0        0     7848 2024-04-14 05:48:28.812056 tooldelta-0.5.1/tooldelta/color_print.py
+-rw-r--r--   0        0        0     2036 2024-04-14 05:48:28.812056 tooldelta-0.5.1/tooldelta/constants.py
+-rw-r--r--   0        0        0     5870 2024-04-14 05:48:28.812056 tooldelta-0.5.1/tooldelta/fb_conn/fbconn.py
+-rwxr-xr-x   0        0        0    34100 2024-04-14 05:48:28.812056 tooldelta-0.5.1/tooldelta/frame.py
+-rwxr-xr-x   0        0        0     3772 2024-04-14 05:48:28.812056 tooldelta-0.5.1/tooldelta/game_texts.py
+-rwxr-xr-x   0        0        0      338 2024-04-14 05:48:28.812056 tooldelta-0.5.1/tooldelta/get_tool_delta_version.py
+-rwxr-xr-x   0        0        0    30687 2024-04-14 05:48:28.812056 tooldelta-0.5.1/tooldelta/launch_cli.py
+-rwxr-xr-x   0        0        0     1080 2024-04-14 05:48:28.812056 tooldelta-0.5.1/tooldelta/launch_options.py
+-rwxr-xr-x   0        0        0     2138 2024-04-14 05:48:28.812056 tooldelta-0.5.1/tooldelta/logger.py
+-rwxr-xr-x   0        0        0    29503 2024-04-14 05:48:28.812056 tooldelta-0.5.1/tooldelta/neo_libs/neo_conn.py
+-rwxr-xr-x   0        0        0     1143 2024-04-14 05:48:28.812056 tooldelta-0.5.1/tooldelta/packets.py
+-rwxr-xr-x   0        0        0    11379 2024-04-14 05:48:28.812056 tooldelta-0.5.1/tooldelta/plugin_load/PluginGroup.py
+-rwxr-xr-x   0        0        0     2273 2024-04-14 05:48:28.816056 tooldelta-0.5.1/tooldelta/plugin_load/__init__.py
+-rwxr-xr-x   0        0        0     6200 2024-04-14 05:48:28.816056 tooldelta-0.5.1/tooldelta/plugin_load/classic_plugin/__init__.py
+-rwxr-xr-x   0        0        0      345 2024-04-14 05:48:28.816056 tooldelta-0.5.1/tooldelta/plugin_load/funcs.py
+-rwxr-xr-x   0        0        0     6780 2024-04-14 05:48:28.816056 tooldelta-0.5.1/tooldelta/plugin_load/injected_plugin/__init__.py
+-rwxr-xr-x   0        0        0     9235 2024-04-14 05:48:28.816056 tooldelta-0.5.1/tooldelta/plugin_load/injected_plugin/movent.py
+-rwxr-xr-x   0        0        0    13738 2024-04-14 05:48:28.816056 tooldelta-0.5.1/tooldelta/plugin_manager.py
+-rwxr-xr-x   0        0        0    13194 2024-04-14 05:48:28.816056 tooldelta-0.5.1/tooldelta/plugin_market.py
+-rw-r--r--   0        0        0     1864 2024-04-14 05:48:28.816056 tooldelta-0.5.1/tooldelta/starter.py
+-rwxr-xr-x   0        0        0      638 2024-04-14 05:48:28.816056 tooldelta-0.5.1/tooldelta/sys_args.py
+-rwxr-xr-x   0        0        0     7057 2024-04-14 05:48:28.816056 tooldelta-0.5.1/tooldelta/urlmethod.py
+-rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 tooldelta-0.5.1/PKG-INFO
```

### Comparing `tooldelta-0.5.0/LICENSE` & `tooldelta-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.0/README.md` & `tooldelta-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.0/pyproject.toml` & `tooldelta-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Tooldelta"
-version = "0.5.0" # This field is automatically set to the value in the version file
+version = "0.5.1" # This field is automatically set to the value in the version file
 description = "Plugin Loader for NeteaseRentalServer on Panel"
 authors = ["SuperScript-PRC"]
 license = ""
 
 readme = "README.md"
 homepage = "https://github.com/SuperScript-PRC/ToolDelta"
 repository = "https://github.com/SuperScript-PRC/ToolDelta"
```

### Comparing `tooldelta-0.5.0/tooldelta/auths.py` & `tooldelta-0.5.1/tooldelta/auths.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.0/tooldelta/basic_mods.py` & `tooldelta-0.5.1/tooldelta/basic_mods.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.0/tooldelta/builtins.py` & `tooldelta-0.5.1/tooldelta/builtins.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.0/tooldelta/cfg.py` & `tooldelta-0.5.1/tooldelta/cfg.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.0/tooldelta/color_print.py` & `tooldelta-0.5.1/tooldelta/color_print.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.0/tooldelta/constants.py` & `tooldelta-0.5.1/tooldelta/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,23 +22,25 @@
 
 LAUNCH_CFG: dict = {
     "服务器号": 0,
     "密码": 0,
     "启动器启动模式(请不要手动更改此项, 改为0可重置)": 0,
     "验证服务器地址(更换时记得更改fbtoken)": "",
     "是否记录日志": True,
+    "是否使用github镜像": True,
     "插件市场源": PLUGIN_MARKET_SOURCE_OFFICIAL
 }
 
 LAUNCH_CFG_STD: dict = {
     "服务器号": int,
     "密码": int,
     "启动器启动模式(请不要手动更改此项, 改为0可重置)": Cfg.NNInt,
     "验证服务器地址(更换时记得更改fbtoken)": str,
     "是否记录日志": bool,
+    "是否使用github镜像": bool,
     "插件市场源": str
 }
 
 FB_APIS = [
     "https://api.fastbuilder.pro/api/phoenix/login",
     "https://api.fastbuilder.pro/api/new",
     "https://api.fastbuilder.pro/api/api",
```

### Comparing `tooldelta-0.5.0/tooldelta/fb_conn/fbconn.py` & `tooldelta-0.5.1/tooldelta/fb_conn/fbconn.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.0/tooldelta/frame.py` & `tooldelta-0.5.1/tooldelta/frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import List, Union
 
 import tooldelta
 from tooldelta import (
     auths,
     constants,
     builtins,
     plugin_market,
@@ -20,28 +19,28 @@
     requests,
     platform,
     subprocess,
     threading,
     getpass
 )
 
-from tooldelta.cfg import Cfg as _Cfg
+from tooldelta.cfg import Cfg
 from tooldelta.logger import publicLogger
 from tooldelta.plugin_load.PluginGroup import PluginGroup
 from tooldelta.game_texts import GameTextsLoader
 from tooldelta.urlmethod import download_file_multithreading, test_site_latency
 from tooldelta.sys_args import sys_args_to_dict
 from tooldelta.launch_cli import (
     FrameFBConn,
     FrameNeOmg,
     FrameNeOmgRemote,
     SysStatus,
 )
 
-from .basic_mods import asyncio, datetime, json
+from .basic_mods import asyncio, json
 from .packets import PacketIDS
 from .plugin_load.injected_plugin import (
     execute_death_message,
     execute_init,
     execute_player_join,
     execute_player_prejoin,
     execute_player_left,
@@ -50,15 +49,15 @@
     safe_jump,
 )
 
 sys_args_dict = sys_args_to_dict(sys.argv)
 createThread = builtins.Builtins.createThread
 VERSION = get_tool_delta_version()
 Builtins = builtins.Builtins
-Config = _Cfg()
+Config = Cfg()
 
 # 整个系统由三个部分组成
 #  Frame: 负责整个 ToolDelta 的基本框架运行
 #  GameCtrl: 负责对接游戏
 #    - Launchers: 负责将不同启动器的游戏接口统一成固定的接口, 供插件在多平台游戏接口运行(FastBuilder External, NeOmega, (TLSP, etc.))
 #  PluginGroup: 负责管理和运行插件
 
@@ -81,14 +80,16 @@
     launchMode: int = 0
     consoleMenu = []
     link_game_ctrl = None
     link_plugin_group = None
     on_plugin_err = staticmethod(
         lambda name, _, err: Print.print_err(f"插件 <{name}> 出现问题: \n{err}")
     )
+    is_mir:bool
+    plugin_market_url:str
 
     @staticmethod
     def check_use_token(tok_name="", check_md=""):
         res = sys_args.sys_args_to_dict()
         res = res.get(tok_name, 1)
         if (res == 1 and check_md) or res != check_md:
             Print.print_err("启动参数错误")
@@ -110,14 +111,15 @@
 
     class ToolDeltaUpdater:
         def __init__(self, launcher):
             self.launcher = launcher
             self.auto_update(self.launcher)
             self.start_auto_update_thread()
 
+
         def start_auto_update_thread(self):
             # 每24小时检查一次更新
             threading.Timer(24 * 60 * 60, self.auto_update, args=(self.launcher)).start()
 
         @staticmethod
         def auto_update(launcher):
             try:
@@ -227,14 +229,15 @@
     def read_cfg(self):
         Config.default_cfg("ToolDelta基本配置.json", constants.LAUNCH_CFG)
         try:
             cfgs = Config.get_cfg("ToolDelta基本配置.json", constants.LAUNCH_CFG_STD)
             self.serverNumber = str(cfgs["服务器号"])
             self.serverPasswd = cfgs["密码"]
             self.launchMode = cfgs["启动器启动模式(请不要手动更改此项, 改为0可重置)"]
+            self.is_mir = cfgs["是否使用github镜像"]
             self.plugin_market_url = cfgs["插件市场源"]
             auth_server = cfgs["验证服务器地址(更换时记得更改fbtoken)"]
             publicLogger.switch_logger(cfgs["是否记录日志"])
             if self.launchMode != 0 and self.launchMode not in range(
                 1, len(constants.LAUNCHERS) + 1
             ):
                 raise Config.ConfigError(
```

### Comparing `tooldelta-0.5.0/tooldelta/game_texts.py` & `tooldelta-0.5.1/tooldelta/game_texts.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.0/tooldelta/launch_cli.py` & `tooldelta-0.5.1/tooldelta/launch_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,27 +7,30 @@
 import uuid
 import time
 import json
 import ssl
 import requests
 import ujson
 import random
-from typing import Callable, Optional
 
+from tooldelta import (
+    constants,
+)
+from typing import Callable, Optional
 from .color_print import Print
 from .urlmethod import download_file_singlethreaded, get_free_port
 from .builtins import Builtins
 from .basic_mods import socketio
 from .packets import Packet_CommandOutput, PacketIDS
 from .sys_args import sys_args_to_dict
-
+from tooldelta.cfg import Cfg
 from .fb_conn import fbconn
 import threading
-
 import tooldelta
+Config = Cfg()
 
 
 class SysStatus:
     LOADING = 100
     LAUNCHING = 101
     RUNNING = 102
     NORMAL_EXIT = 103
@@ -234,15 +237,16 @@
                     continue
                 packet_mapping = ujson.loads(
                     fbconn.GamePacketBytesAsIsJsonStr(packet_bytes)
                 )
                 if packet_type == PacketIDS.CommandOutput:
                     cmd_uuid = packet_mapping["CommandOrigin"]["UUID"].encode()
                     if cmd_uuid in self.cmds_reqs:
-                        self.cmds_resp[cmd_uuid] = [time.time(), packet_mapping]
+                        self.cmds_resp[cmd_uuid] = [
+                            time.time(), packet_mapping]
                 self.packet_handler(packet_type, packet_mapping)
                 if not self.injected and packet_type == PacketIDS.PlayerList:
                     self.injected = True
                     Builtins.createThread(self._launcher_listener)
         except StopIteration:
             pass
         self.update_status(SysStatus.CRASHED_EXIT)
@@ -252,15 +256,16 @@
         Print.print_with_info("§d将自动检测缺失文件并补全", "§d 加载 ")
         mirror_src = "https://mirror.ghproxy.com/"
         file_get_src = (
             mirror_src
             + "https://raw.githubusercontent.com/ToolDelta/ToolDelta/main/require_files.json"
         )
         try:
-            files_to_get = json.loads(requests.get(file_get_src, timeout=30).text)
+            files_to_get = json.loads(
+                requests.get(file_get_src, timeout=30).text)
         except json.JSONDecodeError:
             Print.print_err("自动下载缺失文件失败: 文件源 JSON 不合法")
             return False
         except requests.Timeout:
             Print.print_err("自动下载缺失文件失败: URL 请求出现问题: 请求超时")
             return False
         except Exception as err:
@@ -337,15 +342,16 @@
             lambda pckID, pck: fbconn.SendGamePacketBytes(
                 self.con,
                 fbconn.JsonStrAsIsGamePacketBytes(
                     pckID, ujson.dumps(pck, ensure_ascii=False)
                 ),
             )
         )
-        self.sendfbcmd = staticmethod(lambda cmd: fbconn.SendFBCommand(self.con, cmd))
+        self.sendfbcmd = staticmethod(
+            lambda cmd: fbconn.SendFBCommand(self.con, cmd))
         self.is_op = None
 
 
 class FrameNeOmg(StandardFrame):
     # 使用 NeOmega 框架连接到游戏
     launch_type = "NeOmega"
 
@@ -430,15 +436,16 @@
 
     def msg_show(self):
         def _msg_show_thread():
             while True:
                 msg_orig = self.neomg_proc.stdout.readline().decode("utf-8").strip("\n")
                 if msg_orig in ("", "SIGNAL: exit"):
                     with Print.lock:
-                        Print.print_with_info("ToolDelta: NEOMG 进程已结束", "§b NOMG ")
+                        Print.print_with_info(
+                            "ToolDelta: NEOMG 进程已结束", "§b NOMG ")
                     self.update_status(SysStatus.NORMAL_EXIT)
                     return
                 if "[neOmega 接入点]: 就绪" in msg_orig:
                     self.launch_event.set()
                 elif f"STATUS CODE: {self.secret_exit_key}" in msg_orig:
                     with Print.lock:
                         Print.print_with_info("§a机器人已退出", "§b NOMG ")
@@ -471,116 +478,75 @@
         if self.status == SysStatus.NORMAL_EXIT:
             return SystemExit("正常退出.")
         if self.status == SysStatus.CRASHED_EXIT:
             return Exception("NeOmega 已崩溃")
         return SystemError("未知的退出状态")
 
     def download_libs(self):
-        if self.TDC.SocketIO.connected:
-            try:
-                res = self.TDC.get_depends_table_data()
-                use_mirror = res["mirror_data"]["Mirror"][0]
-            except Exception as err:
-                Print.print_err(f"获取依赖库表出现问题: {err}")
-                self.update_status(SysStatus.CRASHED_EXIT)
-                return
-            self.sys_machine = platform.machine().lower()
-            if self.sys_machine == "x86_64":
-                self.sys_machine = "amd64"
-            elif self.sys_machine == "aarch64":
-                self.sys_machine = "arm64"
-            if "TERMUX_VERSION" in os.environ:
-                sys_info_fmt = f"Android:{self.sys_machine.lower()}"
-            else:
-                sys_info_fmt = f"{platform.uname().system}:{self.sys_machine.lower()}"
-            source_dict = res["mirror_data"][sys_info_fmt]
-            commit_file_path = res["commit_file_path"]
-            commit_url = res["commit"]
-            commit_remote = res["commit"]
-            commit_local = ""
-            commit_file_path = os.path.join(os.getcwd(), commit_file_path)
-            replace_file = False
-            if os.path.isfile(commit_file_path):
-                with open(commit_file_path, "r", encoding="utf-8") as f:
-                    commit_local = f.read()
-                if commit_local != commit_remote:
-                    Print.print_war("依赖库版本过期, 将重新下载")
-                    replace_file = True
-            else:
-                replace_file = True
-            for k, v in source_dict.items():
-                pathdir = os.path.join(os.getcwd(), k)
-                url = use_mirror + "/https://raw.githubusercontent.com/" + v
-                if not os.path.isfile(pathdir) or replace_file:
-                    Print.print_with_info(f"正在下载依赖库 {pathdir} ...", "§a 下载 §r")
-                    try:
-                        download_file_singlethreaded(url, pathdir)
-                    except Exception as err:
-                        Print.print_err(f"下载依赖库出现问题: {err}")
-                        self.update_status(SysStatus.CRASHED_EXIT)
-                        return
-            if replace_file:
-                # 写入commit_remote，文字写入
-                with open(commit_file_path, "w", encoding="utf-8") as f:
-                    f.write(commit_remote)
-                Print.print_suc("已完成依赖更新！")
-
-        elif not self.TDC.SocketIO.connected:
-            try:
-                res = json.loads(
-                    requests.get(
-                        "https://mirror.ghproxy.com/https://raw.githubusercontent.com/ToolDelta/ToolDelta/main/require_files.json"
-                    ).text
-                )
-                use_mirror = res["Mirror"][0]
-            except Exception as err:
-                Print.print_err(f"获取依赖库表出现问题: {err}")
-                self.update_status(SysStatus.CRASHED_EXIT)
-                return
-            self.sys_machine = platform.machine().lower()
-            if self.sys_machine == "x86_64":
-                self.sys_machine = "amd64"
-            elif self.sys_machine == "aarch64":
-                self.sys_machine = "arm64"
-            if "TERMUX_VERSION" in os.environ:
-                sys_info_fmt = f"Android:{self.sys_machine.lower()}"
-            else:
-                sys_info_fmt = f"{platform.uname().system}:{self.sys_machine.lower()}"
-            source_dict = res[sys_info_fmt]
-            commit_file_path, commit_url = list(res["Commit"].items())[0]
-            commit_remote = requests.get(
-                use_mirror + "/raw.githubusercontent.com/" + commit_url
-            ).text
-            commit_local = ""
-            commit_file_path = os.path.join(os.getcwd(), commit_file_path)
-            replace_file = False
-            if os.path.isfile(commit_file_path):
-                with open(commit_file_path, "r", encoding="utf-8") as f:
-                    commit_local = f.read()
-                if commit_local != commit_remote:
-                    Print.print_war("依赖库版本过期, 将重新下载")
-                    replace_file = True
-            else:
+        """根据系统架构和平台下载所需的库。"""
+        cfgs = Config.get_cfg("ToolDelta基本配置.json", constants.LAUNCH_CFG_STD)
+        is_mir: bool = cfgs["是否使用github镜像"]
+        if is_mir:
+            mirror_src = "https://gh.api.99988866.xyz/" + \
+                "https://raw.githubusercontent.com/ToolDelta/ToolDelta/main/"
+            depen_url = "https://gh.api.99988866.xyz/" + \
+                "https://raw.githubusercontent.com/ToolDelta/DependencyLibrary/main/"
+        else:
+            mirror_src = "https://raw.githubusercontent.com/ToolDelta/ToolDelta/main/"
+            depen_url = "https://raw.githubusercontent.com/ToolDelta/DependencyLibrary/main/"
+        try:
+            require_depen = json.loads(
+                requests.get(
+                    f"{mirror_src}require_files.json", timeout=5
+                ).text
+            )
+        except Exception as err:
+            Print.print_err(f"获取依赖库表出现问题: {err}")
+            self.update_status(SysStatus.CRASHED_EXIT)
+            return
+        self.sys_machine = platform.machine().lower()
+        if self.sys_machine == "x86_64":
+            self.sys_machine = "amd64"
+        elif self.sys_machine == "aarch64":
+            self.sys_machine = "arm64"
+        if "TERMUX_VERSION" in os.environ:
+            sys_info_fmt: str = f"Android:{self.sys_machine.lower()}"
+        else:
+            sys_info_fmt: str = f"{platform.uname().system}:{self.sys_machine.lower()}"
+        source_dict: list[str] = require_depen[sys_info_fmt]
+        commit_remote = requests.get(
+            f"{depen_url}commit", timeout=5
+        ).text
+        commit_file_path = os.path.join(
+            os.getcwd(), r"tooldelta\neo_libs\commit")
+        replace_file = False
+        if os.path.isfile(commit_file_path):
+            with open(commit_file_path, "r", encoding="utf-8") as f:
+                commit_local = f.read()
+            if commit_local != commit_remote:
+                Print.print_war("依赖库版本过期, 将重新下载")
                 replace_file = True
-            for k, v in source_dict.items():
-                pathdir = os.path.join(os.getcwd(), k)
-                url = use_mirror + "/https://raw.githubusercontent.com/" + v
-                if not os.path.isfile(pathdir) or replace_file:
-                    Print.print_with_info(f"正在下载依赖库 {pathdir} ...", "§a 下载 §r")
-                    try:
-                        download_file_singlethreaded(url, pathdir)
-                    except Exception as err:
-                        Print.print_err(f"下载依赖库出现问题: {err}")
-                        self.update_status(SysStatus.CRASHED_EXIT)
-                        return
-            if replace_file:
-                # 写入commit_remote，文字写入
-                with open(commit_file_path, "w", encoding="utf-8") as f:
-                    f.write(commit_remote)
-                Print.print_suc("已完成依赖更新！")
+        else:
+            replace_file = True
+        for v in source_dict:
+            pathdir = os.path.join(os.getcwd(), r"tooldelta\neo_libs", v)
+            url = depen_url + v
+            if not os.path.isfile(pathdir) or replace_file:
+                Print.print_with_info(f"正在下载依赖库 {pathdir} ...", "§a 下载 §r")
+                try:
+                    download_file_singlethreaded(url, pathdir)
+                except Exception as err:
+                    Print.print_err(f"下载依赖库出现问题: {err}")
+                    self.update_status(SysStatus.CRASHED_EXIT)
+                    return
+        if replace_file:
+            # 写入commit_remote，文字写入
+            with open(commit_file_path, "w", encoding="utf-8") as f:
+                f.write(commit_remote)
+            Print.print_suc("已完成依赖更新！")
 
     def get_players_and_uuids(self):
         players_uuid = {}
         for i in self.omega.get_all_online_players():
             players_uuid[i.name] = i.uuid
         return players_uuid
 
@@ -590,24 +556,26 @@
     def packet_handler_parent(self, pkt_type, pkt):
         pkt_type = self.omega.get_packet_name_to_id_mapping(pkt_type)
         self.packet_handler(pkt_type, pkt)
 
     def init_all_functions(self):
         def sendcmd(cmd: str, waitForResp: bool = False, timeout: int | float = 30):
             if waitForResp:
-                res = self.omega.send_player_command_need_response(cmd, timeout)
+                res = self.omega.send_player_command_need_response(
+                    cmd, timeout)
                 if res is None:
                     raise TimeoutError("指令超时")
                 return res
             self.omega.send_player_command_omit_response(cmd)
             return
 
         def sendwscmd(cmd: str, waitForResp: bool = False, timeout: int = 30):
             if waitForResp:
-                res = self.omega.send_websocket_command_need_response(cmd, timeout)
+                res = self.omega.send_websocket_command_need_response(
+                    cmd, timeout)
                 if res is None:
                     raise TimeoutError("指令超时")
                 return res
             self.omega.send_websocket_command_omit_response(cmd)
             return
 
         def sendwocmd(cmd: str):
@@ -629,15 +597,16 @@
         self.sendfbcmd = sendfbcmd
         self.is_op = is_op
 
 
 class FrameNeOmgRemote(FrameNeOmg):
     def launch(self):
         try:
-            openat_port = int(sys_args_to_dict().get("access-point-port", "24020"))
+            openat_port = int(sys_args_to_dict().get(
+                "access-point-port", "24020"))
             if openat_port not in range(65536):
                 raise AssertionError
         except (ValueError, AssertionError):
             Print.print_err("启动参数 -access-point-port 错误: 不是1~65535的整数")
         if openat_port == 0:
             Print.print_war(
                 "未用启动参数指定链接neOmega接入点开放端口, 尝试使用默认端口 24015"
@@ -662,63 +631,81 @@
         if self.status == SysStatus.CRASHED_EXIT:
             return Exception("接入点已崩溃")
         return SystemError("未知的退出状态")
 
     def download_libs(self):
         Print.print_inf("以 Remote 启动, 将不会检查库完整性")
 
+
+class MCBEWebSocket(StandardFrame):
+    def __init__(self, serverNumber, password, fbToken, auth_server):
+        global fcwslib
+        import fcwslib
+        self.ws_lib = fcwslib.server.Server(serverNumber, password)
+        self.ws_lib
+        self.ws_lib.run_forever()
+
+
 class ToolDeltaCli(object):
     def __init__(self, address: dict = {"host": "tdaus.tooldelta.fit", "port": 0}) -> None:
-    # def __init__(self, address: dict = {"host": "127.0.0.1", "port": 9002}) -> None:
-        self.NoPort:bool = address.get("port", 0) == 0
-        self.S_ADDRESSS:dict = address
-        self.protocol:str = "http"
-        self.url:str = f'{self.protocol}://{self.S_ADDRESSS["host"]}:{self.S_ADDRESSS["port"]}' if self.NoPort ==False else f'{self.protocol}://{self.S_ADDRESSS["host"]}'
-        self.SocketIO:socketio.Client = socketio.Client()
-        self.data_received_event:threading.Event = threading.Event()
-        self.connected_to_server:bool = True
+        # def __init__(self, address: dict = {"host": "127.0.0.1", "port": 9002}) -> None:
+        self.NoPort: bool = address.get("port", 0) == 0
+        self.S_ADDRESSS: dict = address
+        self.protocol: str = "http"
+        self.url: str = f'{self.protocol}://{self.S_ADDRESSS["host"]}:{self.S_ADDRESSS["port"]}' if self.NoPort == False else f'{self.protocol}://{self.S_ADDRESSS["host"]}'
+        self.SocketIO: socketio.Client = socketio.Client()
+        self.data_received_event: threading.Event = threading.Event()
+        self.connected_to_server: bool = True
         threading.Thread(target=self.conn_aus, name="SocketIO_Conn").start()
-        while not self.SocketIO.connected and self.connected_to_server:time.sleep(0.1)
+        while not self.SocketIO.connected and self.connected_to_server:
+            time.sleep(0.1)
 
     def init_auth_v(self) -> None:
-        self.feature_code:str = str(uuid.uuid5(uuid.NAMESPACE_DNS, str(time.perf_counter())))
-        self.token_ec:tuple= (self.feature_code, self.get_new_token())
+        self.feature_code: str = str(uuid.uuid5(
+            uuid.NAMESPACE_DNS, str(time.perf_counter())))
+        self.token_ec: tuple = (self.feature_code, self.get_new_token())
 
     def get_new_token(self) -> None:
         try:
-            response = requests.post(url=f'{self.url}/api/signin', data=json.dumps({"feature_code": self.feature_code}), timeout= 5)
+            response = requests.post(
+                url=f'{self.url}/api/signin', data=json.dumps({"feature_code": self.feature_code}), timeout=5)
             if response.status_code == 200:
                 return response.text
-        except requests.exceptions.ConnectionError as err:return "null"
+        except requests.exceptions.ConnectionError as err:
+            return "null"
 
     def conn_aus(self) -> None:
         try:
             self.init_auth_v()
-            self.SocketIO.connect(self.url, namespaces='/api', headers={'Authorization': f'Bearer {self.token_ec[1]}'})
+            self.SocketIO.connect(
+                self.url, namespaces='/api', headers={'Authorization': f'Bearer {self.token_ec[1]}'})
             Print.print_suc("ToolDelta成功连接到至Api服务器[Socket-IO]!")
             while True:
                 if not self.SocketIO.connected:
                     try:
                         self.init_auth_v()
-                        self.SocketIO.connect(self.url, namespaces='/api', headers={'Authorization': f'Bearer {self.token_ec[1]}'})
+                        self.SocketIO.connect(
+                            self.url, namespaces='/api', headers={'Authorization': f'Bearer {self.token_ec[1]}'})
                         Print.print_suc("ToolDelta与Api服务器断开连接,已重新连接成功!")
                     except:
-                        Print.print_war("ToolDeltaApi服务器可能存在故障或当前网络环境异常，将停止使用ToolDeltaApi服务器!")
+                        Print.print_war(
+                            "ToolDeltaApi服务器可能存在故障或当前网络环境异常，将停止使用ToolDeltaApi服务器!")
                         break
                 time.sleep(10)
         except Exception as err:
             Print.print_war("ToolDelta无法连接至Api服务器,将停止使用其提供的功能!")
             self.connected_to_server = False
             threading.Thread(target=self.reconnect_to_server).start()
 
     def reconnect_to_server(self, interval=20):
         while not self.connected_to_server:
             try:
                 self.init_auth_v()
-                self.SocketIO.connect(self.url, namespaces='/api', headers={'Authorization': f'Bearer {self.token_ec[1]}'})
+                self.SocketIO.connect(
+                    self.url, namespaces='/api', headers={'Authorization': f'Bearer {self.token_ec[1]}'})
                 Print.print_suc("ToolDelta成功重新连接至Api服务器!")
                 self.connected_to_server = True
             except Exception as err:
                 time.sleep(interval)
 
     def get_depends_table_data(self) -> dict:
         if self.SocketIO.connected:
@@ -727,20 +714,21 @@
                 self.data_received_event.set()
                 self.depend_table_data = data
             self.SocketIO.emit('get_depends_table', namespace='/api')
             self.data_received_event.wait()  # 等待数据返回
             self.data_received_event.clear()
             return self.depend_table_data
         else:
-            Print.print_war("Namespace /api is not connected yet. Please wait for connection.")
+            Print.print_war(
+                "Namespace /api is not connected yet. Please wait for connection.")
 
     def get_version_updates(self) -> any:
         if self.SocketIO.connected:
             @self.SocketIO.on('version_updates', namespace='/api')
             def handle_version_updates_data(data):
                 self.data_received_event.set()
                 self.latest_version_data = data
 
             self.SocketIO.emit('get_version_update', namespace='/api')
             self.data_received_event.wait()
             self.data_received_event.clear()
-            return self.latest_version_data["latest_version_str"]
+            return self.latest_version_data["latest_version_str"]
```

### Comparing `tooldelta-0.5.0/tooldelta/launch_options.py` & `tooldelta-0.5.1/tooldelta/launch_options.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.0/tooldelta/logger.py` & `tooldelta-0.5.1/tooldelta/logger.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.0/tooldelta/neo_libs/neo_conn.py` & `tooldelta-0.5.1/tooldelta/neo_libs/neo_conn.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.0/tooldelta/packets.py` & `tooldelta-0.5.1/tooldelta/packets.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.0/tooldelta/plugin_load/PluginGroup.py` & `tooldelta-0.5.1/tooldelta/plugin_load/PluginGroup.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         if res:
             for f in res:
                 res2 = f(data)
                 if res2:
                     callback_list.append(res2)
         return callback_list
 
-    def test_plugin(self, plugin: Plugin):
+    def test_plugin(self, plugin: type[Plugin]):
         if self.linked_frame is None:
             # 很可能是直接单独运行此插件的代码.
             Print.clean_print(f"插件主类信息({plugin.name}): ")
             Print.clean_print(f" - 作者: {plugin.author}\n - 版本: {plugin.version}")
             Print.clean_print(
                 f" - 数据包监听: {', '.join(str(i) for i in self._listen_packet_ids)}"
             )
```

### Comparing `tooldelta-0.5.0/tooldelta/plugin_load/__init__.py` & `tooldelta-0.5.1/tooldelta/plugin_load/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.0/tooldelta/plugin_load/classic_plugin/__init__.py` & `tooldelta-0.5.1/tooldelta/plugin_load/classic_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.0/tooldelta/plugin_load/injected_plugin/__init__.py` & `tooldelta-0.5.1/tooldelta/plugin_load/injected_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.0/tooldelta/plugin_load/injected_plugin/movent.py` & `tooldelta-0.5.1/tooldelta/plugin_load/injected_plugin/movent.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.0/tooldelta/plugin_manager.py` & `tooldelta-0.5.1/tooldelta/plugin_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import platform
 import shutil
 import shlex
 import json
+import time
 from tooldelta.builtins import Builtins
 from tooldelta.color_print import Print
 from tooldelta.plugin_market import market
 from tooldelta.plugin_load import PluginRegData
 from tooldelta.constants import (
     TOOLDELTA_PLUGIN_DIR,
     TOOLDELTA_CLASSIC_PLUGIN,
@@ -32,20 +33,26 @@
         clear_screen()
         np = self.register_plugins_auto()
         if np > 0:
             Print.clean_print(f"§a已自动注册{np}个未被注册的插件.")
         while 1:
             plugins = self.list_plugins_list()
             Print.clean_print("§f输入§bu§f更新本地所有插件, §f输入§cq§f退出")
+            Print.clean_print("§f输入§ds§f同步插件注册表信息(在手动安装插件后使用)")
             r = input(Print.clean_fmt("§f输入插件关键词进行选择\n(空格可分隔关键词):"))
-            if r.strip() == "":
+            r1 = r.strip().lower()
+            if r1 == "":
                 continue
-            if r.lower() == "q":
+            elif r1 == "s":
+                self.sync_plugin_datas_to_register()
+                Print.clean_print("§a同步插件注册表数据成功.")
+                time.sleep(2)
+            elif r1 == "q":
                 return
-            if r.lower() == "u":
+            elif r1 == "u":
                 self.update_all_plugins(
                     self.get_plugin_reg_name_dict_and_datas()[1]
                 )
             else:
                 res = self.search_plugin(r, plugins)
                 if res is None:
                     input()
@@ -180,14 +187,31 @@
                 if not self.plugin_is_registered(dirs_type) and os.path.isfile(datpath):
                     with open(datpath, "r", encoding="utf-8") as f:
                         jsdata = json.load(f)
                         self.push_plugin_reg_data(PluginRegData(plugin_path, jsdata))
                         any_plugin_registered += 1
         return any_plugin_registered
 
+    def sync_plugin_datas_to_register(self):
+        "同步所有插件注册数据至注册表"
+        dirs = [TOOLDELTA_CLASSIC_PLUGIN, TOOLDELTA_INJECTED_PLUGIN]
+        all_regs = {"classic": {}, "injected": {}}
+        sync_num = 0
+        for f_dir in dirs:
+            dirs_type = {TOOLDELTA_CLASSIC_PLUGIN: "classic", TOOLDELTA_INJECTED_PLUGIN: "injected"}[f_dir]
+            for plugin_path in os.listdir(os.path.join(TOOLDELTA_PLUGIN_DIR, f_dir)):
+                datpath = os.path.join(TOOLDELTA_PLUGIN_DIR, f_dir, plugin_path, "datas.json")
+                if os.path.isfile(datpath):
+                    with open(datpath, "r", encoding="utf-8") as f:
+                        jsdata = json.load(f)
+                        all_regs[dirs_type][plugin_path] = PluginRegData(plugin_path, jsdata).dump()
+                        sync_num += 1
+        JsonIO.writeFileTo("主系统核心数据", self.plugin_reg_data_path, all_regs)
+        return sync_num
+
     def push_plugin_reg_data(self, plugin_data: PluginRegData):
         # 向插件注册表推送插件注册信息
         r = JsonIO.readFileFrom(
             "主系统核心数据", self.plugin_reg_data_path, self.default_reg_data
         )
         r[plugin_data.plugin_type][plugin_data.name] = plugin_data.dump()
         JsonIO.writeFileTo("主系统核心数据", self.plugin_reg_data_path, r)
```

### Comparing `tooldelta-0.5.0/tooldelta/plugin_market.py` & `tooldelta-0.5.1/tooldelta/plugin_market.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 from tooldelta.plugin_load import PluginRegData
 from tooldelta.cfg import Cfg
 from tooldelta.constants import (
     PLUGIN_MARKET_SOURCE_OFFICIAL,
     TOOLDELTA_CLASSIC_PLUGIN,
     TOOLDELTA_INJECTED_PLUGIN
 )
-from typing import Dict
 
 if platform.system().lower() == "windows":
     CLS_CMD = "cls"
 else:
     CLS_CMD = "clear"
 
 clear_screen = lambda: os.system(shlex.quote(CLS_CMD))
@@ -200,15 +199,15 @@
         res1 = json.loads(res.text)
         self.plugin_id_name_map = res1
         return res1
 
     def download_plugin(
         self,
         plugin_data: PluginRegData,
-        all_plugins_dict: Dict[str, str],
+        all_plugins_dict: dict[str, str],
     ):
         pres = [plugin_data]
         download_paths = self.find_dirs(plugin_data)
         for plugin_id in plugin_data.pre_plugins:
             plugin_name = self.plugin_id_name_map[plugin_id]
             Print.clean_print(f"正在下载 {plugin_data.name} 的前置插件 {plugin_name}")
             pres += self.download_plugin(
```

### Comparing `tooldelta-0.5.0/tooldelta/starter.py` & `tooldelta-0.5.1/tooldelta/starter.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from tooldelta.frame import GameCtrl
 from tooldelta.basic_mods import os, traceback, threading
 from tooldelta.color_print import Print
 from tooldelta.plugin_load.PluginGroup import plugin_group
 from tooldelta.plugin_load.injected_plugin import movent
 
 frame = Frame()
-plugin_group.set_frame(frame)
 game_control = GameCtrl(frame)
 def signal_handler(*arg):
     # 排除信号中断
     pass
 signal.signal(signal.SIGINT, signal_handler)
 
 def start_tool_delta():
     # 初始化系统
+    plugin_group.set_frame(frame)
     try:
         frame.welcome()
         frame.basic_operation()
         frame.set_game_control(game_control)
         frame.set_plugin_group(plugin_group)
         movent.set_frame(frame)
         frame.read_cfg()
```

### Comparing `tooldelta-0.5.0/tooldelta/sys_args.py` & `tooldelta-0.5.1/tooldelta/sys_args.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.0/tooldelta/urlmethod.py` & `tooldelta-0.5.1/tooldelta/urlmethod.py`

 * *Files identical despite different names*

### Comparing `tooldelta-0.5.0/PKG-INFO` & `tooldelta-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tooldelta
-Version: 0.5.0
+Version: 0.5.1
 Summary: Plugin Loader for NeteaseRentalServer on Panel
 Home-page: https://github.com/SuperScript-PRC/ToolDelta
 Author: SuperScript-PRC
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Tooldelta Version: 0.5.0 Summary: Plugin Loader for
+Metadata-Version: 2.1 Name: Tooldelta Version: 0.5.1 Summary: Plugin Loader for
 NeteaseRentalServer on Panel Home-page: https://github.com/SuperScript-PRC/
 ToolDelta Author: SuperScript-PRC Requires-Python: >=3.9,<3.13 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: aiohttp (>=3.9.3,<4.0.0) Requires-Dist: colorama
 (>=0.4.6,<0.5.0) Requires-Dist: flask (>=3.0.2,<4.0.0) Requires-Dist: nbt
```

