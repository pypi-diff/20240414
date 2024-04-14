# Comparing `tmp/pyprland-2.2.5.tar.gz` & `tmp/pyprland-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprland-2.2.5.tar", max compression
+gzip compressed data, was "pyprland-2.2.6.tar", max compression
```

## Comparing `pyprland-2.2.5.tar` & `pyprland-2.2.6.tar`

### file list

```diff
@@ -1,38 +1,36 @@
--rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.2.5/LICENSE
--rw-r--r--   0        0        0     4380 2024-04-12 19:57:34.959057 pyprland-2.2.5/README.md
--rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.5/pyprland/__init__.py
--rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.5/pyprland/adapters/__init__.py
--rw-r--r--   0        0        0      400 2024-04-05 20:13:47.397221 pyprland-2.2.5/pyprland/adapters/colors.py
--rw-r--r--   0        0        0     4377 2024-03-03 01:47:24.894367 pyprland-2.2.5/pyprland/adapters/menus.py
--rw-r--r--   0        0        0     1395 2024-04-08 20:00:16.866561 pyprland-2.2.5/pyprland/adapters/units.py
--rwxr-xr-x   0        0        0    16372 2024-04-12 20:05:41.571463 pyprland-2.2.5/pyprland/command.py
--rwxr-xr-x   0        0        0    15808 2024-04-05 22:08:40.562254 pyprland-2.2.5/pyprland/command.py.orig
--rw-r--r--   0        0        0     7410 2024-04-09 21:29:20.927222 pyprland-2.2.5/pyprland/common.py
--rw-r--r--   0        0        0     7197 2024-04-12 17:07:08.504043 pyprland-2.2.5/pyprland/ipc.py
--rw-r--r--   0        0        0       45 2024-03-03 01:47:24.897701 pyprland-2.2.5/pyprland/plugins/__init__.py
--rw-r--r--   0        0        0      106 2024-03-03 01:47:24.897701 pyprland-2.2.5/pyprland/plugins/experimental.py
--rw-r--r--   0        0        0     1647 2024-03-03 01:47:24.914368 pyprland-2.2.5/pyprland/plugins/expose.py
--rw-r--r--   0        0        0     1386 2024-03-30 16:09:04.631012 pyprland-2.2.5/pyprland/plugins/fetch_client_menu.py
--rw-r--r--   0        0        0     2589 2024-04-09 20:50:41.034540 pyprland-2.2.5/pyprland/plugins/interface.py
--rw-r--r--   0        0        0     7972 2024-03-03 01:47:24.917701 pyprland-2.2.5/pyprland/plugins/layout_center.py
--rw-r--r--   0        0        0     1677 2024-03-03 01:47:24.901034 pyprland-2.2.5/pyprland/plugins/lost_windows.py
--rw-r--r--   0        0        0     1239 2024-04-03 21:48:38.877707 pyprland-2.2.5/pyprland/plugins/magnify.py
--rw-r--r--   0        0        0     8684 2024-03-31 17:52:13.879696 pyprland-2.2.5/pyprland/plugins/monitors.py
--rw-r--r--   0        0        0     8720 2024-03-30 19:02:09.575863 pyprland-2.2.5/pyprland/plugins/monitors.py.orig
--rw-r--r--   0        0        0     3922 2024-03-03 01:47:24.904368 pyprland-2.2.5/pyprland/plugins/monitors_v0.py
--rw-r--r--   0        0        0        0 2024-04-04 16:21:22.101700 pyprland-2.2.5/pyprland/plugins/nohup.out
--rw-r--r--   0        0        0     1515 2024-04-11 16:23:54.463967 pyprland-2.2.5/pyprland/plugins/pyprland.py
--rw-r--r--   0        0        0    26125 2024-04-12 17:49:11.523202 pyprland-2.2.5/pyprland/plugins/scratchpads/__init__.py
--rw-r--r--   0        0        0     2641 2024-04-12 17:24:50.007112 pyprland-2.2.5/pyprland/plugins/scratchpads/animations.py
--rw-r--r--   0        0        0     2106 2024-04-12 17:23:41.858277 pyprland-2.2.5/pyprland/plugins/scratchpads/helpers.py
--rw-r--r--   0        0        0     3436 2024-04-12 17:21:22.436949 pyprland-2.2.5/pyprland/plugins/scratchpads/lookup.py
--rw-r--r--   0        0        0     4136 2024-04-12 17:19:16.255742 pyprland-2.2.5/pyprland/plugins/scratchpads/objects.py
--rw-r--r--   0        0        0     1058 2024-03-03 01:47:24.907701 pyprland-2.2.5/pyprland/plugins/shift_monitors.py
--rw-r--r--   0        0        0     4161 2024-04-09 15:53:04.519223 pyprland-2.2.5/pyprland/plugins/shortcuts_menu.py
--rw-r--r--   0        0        0     3983 2024-04-09 21:03:19.309538 pyprland-2.2.5/pyprland/plugins/system_notifier.py
--rw-r--r--   0        0        0      519 2024-03-03 01:47:24.911034 pyprland-2.2.5/pyprland/plugins/toggle_dpms.py
--rw-r--r--   0        0        0     1063 2024-03-03 01:47:24.917701 pyprland-2.2.5/pyprland/plugins/toggle_special.py
--rw-r--r--   0        0        0     5071 2024-04-12 19:31:07.396989 pyprland-2.2.5/pyprland/plugins/wallpapers.py
--rw-r--r--   0        0        0     2589 2024-03-03 01:47:24.911034 pyprland-2.2.5/pyprland/plugins/workspaces_follow_focus.py
--rw-r--r--   0        0        0      725 2024-04-12 20:05:41.561462 pyprland-2.2.5/pyproject.toml
--rw-r--r--   0        0        0     4919 1970-01-01 00:00:00.000000 pyprland-2.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-02-16 16:53:56.731771 pyprland-2.2.6/LICENSE
+-rw-r--r--   0        0        0     4458 2024-04-14 21:04:51.031595 pyprland-2.2.6/README.md
+-rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.6/pyprland/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-03 01:47:24.891034 pyprland-2.2.6/pyprland/adapters/__init__.py
+-rw-r--r--   0        0        0      400 2024-04-05 20:13:47.397221 pyprland-2.2.6/pyprland/adapters/colors.py
+-rw-r--r--   0        0        0     4377 2024-03-03 01:47:24.894367 pyprland-2.2.6/pyprland/adapters/menus.py
+-rw-r--r--   0        0        0     1395 2024-04-08 20:00:16.866561 pyprland-2.2.6/pyprland/adapters/units.py
+-rwxr-xr-x   0        0        0    16724 2024-04-14 21:05:55.379089 pyprland-2.2.6/pyprland/command.py
+-rw-r--r--   0        0        0     7573 2024-04-13 21:52:18.927484 pyprland-2.2.6/pyprland/common.py
+-rw-r--r--   0        0        0     7197 2024-04-12 17:07:08.504043 pyprland-2.2.6/pyprland/ipc.py
+-rw-r--r--   0        0        0       45 2024-03-03 01:47:24.897701 pyprland-2.2.6/pyprland/plugins/__init__.py
+-rw-r--r--   0        0        0      106 2024-03-03 01:47:24.897701 pyprland-2.2.6/pyprland/plugins/experimental.py
+-rw-r--r--   0        0        0     1818 2024-04-13 18:30:41.827307 pyprland-2.2.6/pyprland/plugins/expose.py
+-rw-r--r--   0        0        0     1386 2024-03-30 16:09:04.631012 pyprland-2.2.6/pyprland/plugins/fetch_client_menu.py
+-rw-r--r--   0        0        0     2018 2024-04-14 20:56:27.261784 pyprland-2.2.6/pyprland/plugins/gbar.py
+-rw-r--r--   0        0        0     2589 2024-04-09 20:50:41.034540 pyprland-2.2.6/pyprland/plugins/interface.py
+-rw-r--r--   0        0        0     7972 2024-03-03 01:47:24.917701 pyprland-2.2.6/pyprland/plugins/layout_center.py
+-rw-r--r--   0        0        0     1677 2024-03-03 01:47:24.901034 pyprland-2.2.6/pyprland/plugins/lost_windows.py
+-rw-r--r--   0        0        0     1239 2024-04-03 21:48:38.877707 pyprland-2.2.6/pyprland/plugins/magnify.py
+-rw-r--r--   0        0        0     8680 2024-04-13 18:26:06.759226 pyprland-2.2.6/pyprland/plugins/monitors.py
+-rw-r--r--   0        0        0     3922 2024-03-03 01:47:24.904368 pyprland-2.2.6/pyprland/plugins/monitors_v0.py
+-rw-r--r--   0        0        0     1770 2024-04-13 21:52:18.890816 pyprland-2.2.6/pyprland/plugins/pyprland.py
+-rw-r--r--   0        0        0    26132 2024-04-14 20:57:42.622754 pyprland-2.2.6/pyprland/plugins/scratchpads/__init__.py
+-rw-r--r--   0        0        0     2641 2024-04-12 17:24:50.007112 pyprland-2.2.6/pyprland/plugins/scratchpads/animations.py
+-rw-r--r--   0        0        0     2106 2024-04-12 17:23:41.858277 pyprland-2.2.6/pyprland/plugins/scratchpads/helpers.py
+-rw-r--r--   0        0        0     3436 2024-04-12 17:21:22.436949 pyprland-2.2.6/pyprland/plugins/scratchpads/lookup.py
+-rw-r--r--   0        0        0     4136 2024-04-12 17:19:16.255742 pyprland-2.2.6/pyprland/plugins/scratchpads/objects.py
+-rw-r--r--   0        0        0     1058 2024-03-03 01:47:24.907701 pyprland-2.2.6/pyprland/plugins/shift_monitors.py
+-rw-r--r--   0        0        0     4161 2024-04-09 15:53:04.519223 pyprland-2.2.6/pyprland/plugins/shortcuts_menu.py
+-rw-r--r--   0        0        0     3983 2024-04-09 21:03:19.309538 pyprland-2.2.6/pyprland/plugins/system_notifier.py
+-rw-r--r--   0        0        0      519 2024-03-03 01:47:24.911034 pyprland-2.2.6/pyprland/plugins/toggle_dpms.py
+-rw-r--r--   0        0        0     1063 2024-03-03 01:47:24.917701 pyprland-2.2.6/pyprland/plugins/toggle_special.py
+-rw-r--r--   0        0        0     5335 2024-04-13 18:20:53.870052 pyprland-2.2.6/pyprland/plugins/wallpapers.py
+-rw-r--r--   0        0        0     2559 2024-04-14 20:57:42.622754 pyprland-2.2.6/pyprland/plugins/workspaces_follow_focus.py
+-rw-r--r--   0        0        0      725 2024-04-14 21:05:55.369089 pyprland-2.2.6/pyproject.toml
+-rw-r--r--   0        0        0     4997 1970-01-01 00:00:00.000000 pyprland-2.2.6/PKG-INFO
```

### Comparing `pyprland-2.2.5/LICENSE` & `pyprland-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.5/README.md` & `pyprland-2.2.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 - ["It just works very very well" - The Linux Cast (video)](https://youtu.be/Cjn0SFyyucY?si=hGb0TM9IDvlbcD6A&t=131) - February 2024
 - [You NEED This in your Hyprland Config - LibrePhoenix (video)](https://www.youtube.com/watch?v=CwGlm-rpok4) - October 2023 (*Now [TOML](https://toml.io/en/) format is preferred over [JSON](https://www.w3schools.com/js/js_json_intro.asp))
 
 ## Contributing
 
 Check out the [creating a pull request](https://docs.github.com/fr/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) document for guidance.
 
-- Report bugs or propose features [here](https://github.com/hyprland-community/pyprland/issues).
+- Report bugs or propose features [here](https://github.com/hyprland-community/pyprland/issues)
 - Improve our [wiki](https://github.com/hyprland-community/pyprland/wiki)
 
 and if you have coding skills you can also
 
-- Enhance test coverage in our [tests](https://github.com/hyprland-community/pyprland/tree/main/tests).
+- Enhance the coverage of our [tests](https://github.com/hyprland-community/pyprland/tree/main/tests)
 - Propose & write new plugins or enhancements
 
 ## Dependencies
 
 - **Hyprland** >= 0.37
 - **Python** >= 3.11
     - **aiofiles**
@@ -47,15 +47,15 @@
 
 ### 2.2
 
 - Added [wallpapers](https://github.com/hyprland-community/pyprland/wiki/wallpapers) and [system_notifier](https://github.com/hyprland-community/pyprland/wiki/system_notifier) plugins.
 - Refactor in 2.2.5
   - updated the syntax for [wallpapers](https://github.com/hyprland-community/pyprland/wiki/wallpapers)
   - deprecated `class_match` in [scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads)
-
+- Added [gbar](https://github.com/hyprland-community/pyprland/wiki/gbar) in 2.2.6
 ### 2.1
 
 - Requires Hyprland >= 0.37
 - [Monitors](https://github.com/hyprland-community/pyprland/wiki/monitors) plugin improvements.
 
 ### 2.0
```

#### html2text {}

```diff
@@ -21,27 +21,28 @@
 - February 2024 - [You NEED This in your Hyprland Config - LibrePhoenix
 (video)](https://www.youtube.com/watch?v=CwGlm-rpok4) - October 2023 (*Now
 [TOML](https://toml.io/en/) format is preferred over [JSON](https://
 www.w3schools.com/js/js_json_intro.asp)) ## Contributing Check out the
 [creating a pull request](https://docs.github.com/fr/pull-requests/
 collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-
 requests/creating-a-pull-request) document for guidance. - Report bugs or
-propose features [here](https://github.com/hyprland-community/pyprland/issues).
+propose features [here](https://github.com/hyprland-community/pyprland/issues)
 - Improve our [wiki](https://github.com/hyprland-community/pyprland/wiki) and
-if you have coding skills you can also - Enhance test coverage in our [tests]
-(https://github.com/hyprland-community/pyprland/tree/main/tests). - Propose &
+if you have coding skills you can also - Enhance the coverage of our [tests]
+(https://github.com/hyprland-community/pyprland/tree/main/tests) - Propose &
 write new plugins or enhancements ## Dependencies - **Hyprland** >= 0.37 -
 **Python** >= 3.11 - **aiofiles** ## Latest major changes > [!note] > Check the
 [Releases change log](https://github.com/hyprland-community/pyprland/releases)
 for more information ### 2.2 - Added [wallpapers](https://github.com/hyprland-
 community/pyprland/wiki/wallpapers) and [system_notifier](https://github.com/
 hyprland-community/pyprland/wiki/system_notifier) plugins. - Refactor in 2.2.5
 - updated the syntax for [wallpapers](https://github.com/hyprland-community/
 pyprland/wiki/wallpapers) - deprecated `class_match` in [scratchpads](https://
-github.com/hyprland-community/pyprland/wiki/scratchpads) ### 2.1 - Requires
+github.com/hyprland-community/pyprland/wiki/scratchpads) - Added [gbar](https:/
+/github.com/hyprland-community/pyprland/wiki/gbar) in 2.2.6 ### 2.1 - Requires
 Hyprland >= 0.37 - [Monitors](https://github.com/hyprland-community/pyprland/
 wiki/monitors) plugin improvements. ### 2.0 - New dependency: [aiofiles](https:
 //pypi.org/project/aiofiles/) - Added [hysteresis](https://github.com/hyprland-
 community/pyprland/wiki/scratchpads#hysteresis-optional) support for
 [scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads).
 ### 1.10 - New [fetch_client_menu](https://github.com/hyprland-community/
 pyprland/wiki/fetch_client_menu) and [shortcuts_menu](https://github.com/
```

### Comparing `pyprland-2.2.5/pyprland/adapters/menus.py` & `pyprland-2.2.6/pyprland/adapters/menus.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.5/pyprland/adapters/units.py` & `pyprland-2.2.6/pyprland/adapters/units.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.5/pyprland/command.py` & `pyprland-2.2.6/pyprland/command.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/bin/env python
 """ Pyprland - an Hyprland companion app (cli client & daemon) """
 import asyncio
 import importlib
 import itertools
 from functools import partial
-from typing import Self
+from typing import Self, Callable
 import tomllib
 import json
 import os
 import sys
 
 from pyprland.common import (
     PyprError,
@@ -40,21 +40,24 @@
     "Main app object"
     server: asyncio.Server
     event_reader: asyncio.StreamReader
     stopped = False
     config: dict[str, dict] = {}
     tasks: None | asyncio.TaskGroup = None
     instance: Self | None = None
+    log_handler: Callable[[Plugin, str, tuple], None]
 
     @classmethod
     def _set_instance(cls, instance):
         "Set instance reference into class (for testing/debugging only)"
         cls.instance = instance
 
     def __init__(self):
+        self.pyprland_mutex_event = asyncio.Event()
+        self.pyprland_mutex_event.set()
         self.config = {}
         self.plugins: dict[str, Plugin] = {}
         self.log = get_logger()
         self.queues = {}
         self._set_instance(self)
 
     async def initialize(self):
@@ -64,47 +67,47 @@
     async def __open_config(self, config_filename=""):
         """Loads config file as self.config"""
         if config_filename:
             fname = os.path.expandvars(os.path.expanduser(config_filename))
         else:
             if os.path.exists(OLD_CONFIG_FILE) and not os.path.exists(CONFIG_FILE):
                 self.log.warning("Consider changing your configuration to TOML format.")
-
             self.config.clear()
             fname = os.path.expanduser(CONFIG_FILE)
 
+        config = self.__load_config_file(fname)
+
+        if not config_filename:
+            for extra_config in list(config["pyprland"].get("include", [])):
+                merge(config, await self.__open_config(extra_config))
+            self.config.update(config)
+        return config
+
+    def __load_config_file(self, fname):
+        """Loads a configuration file and returns it as a dictionary"""
         config = {}
         if os.path.exists(fname):
             self.log.info("Loading %s", fname)
             try:
                 with open(fname, "rb") as f:
                     config = tomllib.load(f)
             except FileNotFoundError as e:
-                self.log.critical(
-                    "No config file found, create one at ~/.config/hypr/pyprland.json with a valid pyprland.plugins list"
-                )
+                self.log.critical("Problem reading %s: %s", fname, e)
                 raise PyprError() from e
         elif os.path.exists(os.path.expanduser(OLD_CONFIG_FILE)):
             self.log.info("Loading %s", OLD_CONFIG_FILE)
             try:
                 with open(os.path.expanduser(OLD_CONFIG_FILE), encoding="utf-8") as f:
                     config = json.loads(f.read())
             except FileNotFoundError as e:
-                self.log.critical(
-                    "No config file found, create one at ~/.config/hypr/pyprland.json with a valid pyprland.plugins list"
-                )
+                self.log.critical("Problem reading %s: %s", fname, e)
                 raise PyprError() from e
         else:
             self.log.critical("Config file not found! Please create %s", fname)
             raise PyprError()
-
-        if not config_filename:
-            for extra_config in list(config["pyprland"].get("include", [])):
-                merge(config, await self.__open_config(extra_config))
-            self.config.update(config)
         return config
 
     async def _load_single_plugin(self, name, init) -> bool:
         "Load a single plugin, optionally calling `init`"
         if "." in name:
             modname = name
         elif "external:" in name:
@@ -163,22 +166,18 @@
         """loads the configuration (new plugins will be added & config updated)
 
         if `init` is true, also initializes the plugins"""
 
         await self.__open_config()
         assert self.config
         await self.__load_plugins_config(init=init)
-        if self.config["pyprland"].get("colored_handlers_log", True):
-            self.log_handler = (  # pylint: disable=attribute-defined-outside-init
-                self.colored_log_handler
-            )
-        else:
-            self.log_handler = (  # pylint: disable=attribute-defined-outside-init
-                self.plain_log_handler
-            )
+        colored_logs = self.config["pyprland"].get("colored_handlers_log", True)
+        self.log_handler = (
+            self.colored_log_handler if colored_logs else self.plain_log_handler
+        )  # pylint: disable=attribute-defined-outside-init
 
     def plain_log_handler(self, plugin, name, params):
         "log a handler method without color"
         plugin.log.debug(f"{name}{params}")
 
     def colored_log_handler(self, plugin, name, params):
         "log a handler method with color"
@@ -274,27 +273,34 @@
                 await self.server.serve_forever()
         finally:
             await asyncio.gather(*(plugin.exit() for plugin in self.plugins.values()))
 
     async def _plugin_runner_loop(self, name):
         "Runs tasks for a given plugin indefinitely"
         q = self.queues[name]
+        is_pyprland = name == "pyprland"
 
         while not self.stopped:
+            if not is_pyprland:
+                await self.pyprland_mutex_event.wait()
             try:
                 task = await q.get()
+                if is_pyprland:
+                    self.pyprland_mutex_event.clear()
             except RuntimeError as e:
                 self.log.error("Aborting [%s] loop: %s", name, e)
                 return
             try:
                 await task()
             except Exception as e:  # pylint: disable=W0718
                 self.log.error(
                     "Unhandled error running plugin %s::%s: %s", name, task, e
                 )
+            if is_pyprland and q.empty():
+                self.pyprland_mutex_event.set()
 
     async def plugins_runner(self):
         "Runs plugins' task using the created `tasks` TaskGroup attribute"
         async with asyncio.TaskGroup() as group:
             self.tasks = group
             for name in self.plugins:
                 group.create_task(self._plugin_runner_loop(name))
@@ -356,52 +362,55 @@
     finally:
         events_writer.close()
         await events_writer.wait_closed()
         manager.server.close()
         await manager.server.wait_closed()
 
 
+def show_help(manager):
+    "show the documentation"
+
+    def format_doc(txt):
+        return txt.split("\n")[0]
+
+    print(
+        """Syntax: pypr [command]
+
+If the command is ommited, runs the daemon which will start every configured plugin.
+
+Available commands:
+"""
+    )
+    for plug in manager.plugins.values():
+        for name in dir(plug):
+            if not name.startswith("run_"):
+                continue
+            fn = getattr(plug, name)
+            if callable(fn):
+                doc_txt = format_doc(fn.__doc__) if fn.__doc__ else "N/A"
+                print(f" {name[4:]:20s} {doc_txt} [{plug.name}]")
+
+
 async def run_client():
     "Runs the client (CLI)"
     manager = Pyprland()
 
     if sys.argv[1] == "version":
-        print("2.2.5")  # Automatically updated version
+        print("2.2.6")  # Automatically updated version
         return
 
     if sys.argv[1] == "edit":
         editor = os.environ.get("EDITOR", os.environ.get("VISUAL", "vi"))
         filename = os.path.expanduser(CONFIG_FILE)
         run_interactive_program(f'{editor} "{filename}"')
         sys.argv[1] = "reload"
 
     if sys.argv[1] in ("--help", "-h", "help"):
         await manager.load_config(init=False)
-
-        def format_doc(txt):
-            return txt.split("\n")[0]
-
-        print(
-            """Syntax: pypr [command]
-
-If the command is ommited, runs the daemon which will start every configured plugin.
-
-Available commands:
-"""
-        )
-        for plug in manager.plugins.values():
-            for name in dir(plug):
-                if name.startswith("run_"):
-                    fn = getattr(plug, name)
-                    if callable(fn):
-                        print(
-                            f" {name[4:]:20s} {format_doc(fn.__doc__) if fn.__doc__ else 'N/A'} [{plug.name}]"
-                        )
-
-        return
+        return show_help(manager)
 
     try:
         _, writer = await asyncio.open_unix_connection(CONTROL)
     except (ConnectionRefusedError, FileNotFoundError) as e:
         manager.log.critical("Failed to open control socket, is pypr daemon running ?")
         await notify_error("Pypr can't connect, is daemon running ?")
         raise PyprError() from e
```

### Comparing `pyprland-2.2.5/pyprland/common.py` & `pyprland-2.2.6/pyprland/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,25 +184,31 @@
 @dataclass
 class SharedState:
     "Stores commonly requested properties"
     active_workspace: str = ""  # workspace name
     active_monitor: str = ""  # monitor name
     active_window: str = ""  # window address
     variables: dict = field(default_factory=dict)
+    monitors: list[str] = field(default_factory=list)
 
 
 state = SharedState()
 """
 Exposes most-commonly accessed attributes to avoid specific IPC requests
 - `active_monitor` monitor's name
 - `active_workspace` workspace's name
 - `active_window` window's address
 """
 
 
+def prepare_for_quotes(text: str):
+    "Escapes double quotes in text"
+    return text.replace('"', '\\"')
+
+
 def apply_variables(template: str, variables: dict[str, str]):
     """Replace [var_name] with content from supplied variables
     Args:
         template: the string template
         variables: a dict containing the variables to replace
     """
     pattern = r"\[([^\[\]]+)\]"
```

### Comparing `pyprland-2.2.5/pyprland/ipc.py` & `pyprland-2.2.6/pyprland/ipc.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.5/pyprland/plugins/fetch_client_menu.py` & `pyprland-2.2.6/pyprland/plugins/fetch_client_menu.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.5/pyprland/plugins/interface.py` & `pyprland-2.2.6/pyprland/plugins/interface.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.5/pyprland/plugins/layout_center.py` & `pyprland-2.2.6/pyprland/plugins/layout_center.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.5/pyprland/plugins/lost_windows.py` & `pyprland-2.2.6/pyprland/plugins/lost_windows.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.5/pyprland/plugins/magnify.py` & `pyprland-2.2.6/pyprland/plugins/magnify.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.5/pyprland/plugins/monitors.py` & `pyprland-2.2.6/pyprland/plugins/monitors.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,24 +219,24 @@
         monitors_by_descr = {m["description"]: m for m in monitors}
         cleaned_config: dict[str, dict[str, Any]] = {}
         plugged_monitors = {m["name"]: m for m in monitors}
         for descr1, placement in placement_rules.items():
             mon = self._get_mon_by_pat(descr1, monitors_by_descr, plugged_monitors)
             if not mon:
                 continue
-            name1 = mon["name"]
-            if name1 not in plugged_monitors:
+            name = mon["name"]
+            if name not in plugged_monitors:
                 continue
-            cleaned_config[name1] = {}
+            cleaned_config[name] = {}
             for position, descr_list in placement.items():
                 if isinstance(descr_list, str):
                     descr_list = [descr_list]
                 resolved = []
                 for p in descr_list:
                     r = self._get_mon_by_pat(p, monitors_by_descr, plugged_monitors)
                     if r:
                         resolved.append(r["name"])
                 if resolved:
-                    cleaned_config[name1][clean_pos(position)] = [
+                    cleaned_config[name][clean_pos(position)] = [
                         r for r in resolved if r in plugged_monitors
                     ]
         return cleaned_config
```

### Comparing `pyprland-2.2.5/pyprland/plugins/monitors_v0.py` & `pyprland-2.2.6/pyprland/plugins/monitors_v0.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.5/pyprland/plugins/pyprland.py` & `pyprland-2.2.6/pyprland/plugins/pyprland.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,19 +6,25 @@
 class Extension(Plugin):
     "Internal built-in plugin allowing caching states and implementing special commands"
 
     async def init(self):
         "initializes the plugin"
         state.active_window = ""
         state.active_workspace = (await self.hyprctlJSON("activeworkspace"))["name"]
-        state.active_monitor = next(
-            mon["name"]
-            for mon in (await self.hyprctlJSON("monitors"))
-            if mon["focused"]
-        )
+        monitors = await self.hyprctlJSON("monitors")
+        state.monitors = [mon["name"] for mon in monitors]
+        state.active_monitor = next(mon["name"] for mon in monitors if mon["focused"])
+
+    async def event_monitoradded(self, name):
+        "track monitor"
+        state.monitors.append(name)
+
+    async def event_monitorremoved(self, name):
+        "track monitor"
+        state.monitors.remove(name)
 
     async def on_reload(self):
         state.variables = self.config.get("variables", {})
 
     async def event_activewindowv2(self, addr):
         "keep track of focused client"
         state.active_window = "0x" + addr
```

### Comparing `pyprland-2.2.5/pyprland/plugins/scratchpads/__init__.py` & `pyprland-2.2.6/pyprland/plugins/scratchpads/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -527,21 +527,21 @@
 
         await self._show_transition(item, monitor, was_alive)
         item.monitor = monitor["name"]
 
     async def _show_transition(self, item, monitor, was_alive):
         "perfoms the transition to visible state"
         animation_type = item.conf.get("animation", "").lower()
-        wrkspc = monitor["activeWorkspace"]["id"]
+        wrkspc = monitor["activeWorkspace"]["name"]
         item.meta["last_shown"] = time.time()
         # Start the transition
         await self.hyprctl(
             [
                 f"moveworkspacetomonitor special:scratch_{item.uid} {monitor['name']}",
-                f"movetoworkspacesilent {wrkspc},address:{item.full_address}",
+                f"movetoworkspacesilent name:{wrkspc},address:{item.full_address}",
                 f"alterzorder top,address:{item.full_address}",
             ]
         )
         preserve_aspect = self.cast_bool(item.conf.get("preserve_aspect"))
         should_set_aspect = (
             not (preserve_aspect and was_alive) or item.monitor != state.active_monitor
         )  # not aspect preserving or it's newly spawned
```

### Comparing `pyprland-2.2.5/pyprland/plugins/scratchpads/animations.py` & `pyprland-2.2.6/pyprland/plugins/scratchpads/animations.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.5/pyprland/plugins/scratchpads/helpers.py` & `pyprland-2.2.6/pyprland/plugins/scratchpads/helpers.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.5/pyprland/plugins/scratchpads/lookup.py` & `pyprland-2.2.6/pyprland/plugins/scratchpads/lookup.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.5/pyprland/plugins/scratchpads/objects.py` & `pyprland-2.2.6/pyprland/plugins/scratchpads/objects.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.5/pyprland/plugins/shift_monitors.py` & `pyprland-2.2.6/pyprland/plugins/shift_monitors.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.5/pyprland/plugins/shortcuts_menu.py` & `pyprland-2.2.6/pyprland/plugins/shortcuts_menu.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.5/pyprland/plugins/system_notifier.py` & `pyprland-2.2.6/pyprland/plugins/system_notifier.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.5/pyprland/plugins/toggle_dpms.py` & `pyprland-2.2.6/pyprland/plugins/toggle_dpms.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.5/pyprland/plugins/toggle_special.py` & `pyprland-2.2.6/pyprland/plugins/toggle_special.py`

 * *Files identical despite different names*

### Comparing `pyprland-2.2.5/pyprland/plugins/wallpapers.py` & `pyprland-2.2.6/pyprland/plugins/wallpapers.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,64 +2,70 @@
 import random
 import asyncio
 import os.path
 
 from aiofiles.os import listdir
 
 from .interface import Plugin
-from ..common import CastBoolMixin, apply_variables, state
+from ..common import CastBoolMixin, apply_variables, state, prepare_for_quotes
 
 
-async def iter_dir(path, extensions, recurse=True):
+async def get_files_with_ext(path, extensions, recurse=True):
     "Returns files matching `extension` in given `path`. Can optionally `recurse` subfolders."
     for fname in await listdir(path):
         ext = fname.rsplit(".", 1)[-1]
         full_path = os.path.join(path, fname)
         if ext.lower() in extensions:
             yield full_path
         elif recurse and os.path.isdir(full_path):
-            async for v in iter_dir(full_path, extensions, True):
+            async for v in get_files_with_ext(full_path, extensions, True):
                 yield v
 
 
 class Extension(CastBoolMixin, Plugin):
     "Manages the background image"
 
-    default_extensions: set[str] | list[str] = set(("png", "jpg", "jpeg"))
+    default_image_ext: set[str] | list[str] = set(("png", "jpg", "jpeg"))
     image_list: list[str] = []
     running = True
     proc: list = []
     loop = None
 
     next_background_event = asyncio.Event()
     cur_image = ""
 
     async def on_reload(self):
         "Re-build the image list"
-        image_list = []
         cfg_path = self.config["path"]
         paths = [cfg_path] if isinstance(cfg_path, str) else list(cfg_path)
-        extensions = self.config.get("extensions", self.default_extensions)
-        for path in paths:
-            async for fname in iter_dir(
+        extensions = self.config.get("extensions", self.default_image_ext)
+
+        self.image_list = [
+            os.path.join(path, fname)
+            for path in paths
+            async for fname in get_files_with_ext(
                 path, extensions, recurse=self.cast_bool(self.config.get("recurse"))
-            ):
-                image_list.append(os.path.join(path, fname))
-        self.image_list = image_list
-        # start the main loop if it's the first load of the config
+            )
+        ]
+
+        # Start the main loop if it's the first load of the config
         if self.loop is None:
             self.loop = asyncio.create_task(self.main_loop())
 
     async def exit(self):
         "terminates gracefully"
         self.running = False
         if self.loop:
             self.loop.cancel()
         await self.terminate()
 
+    async def event_monitoradded(self, _):
+        "When a new monitor is added, set the background"
+        self.next_background_event.set()
+
     def select_next_image(self):
         "Returns the next image (random is supported for now)"
         choice = random.choice(self.image_list)
         if choice == self.cur_image:
             choice = random.choice(self.image_list)
         self.cur_image = choice
         return choice
@@ -71,34 +77,44 @@
         self.proc.append(await asyncio.create_subprocess_shell(cmd))
 
     async def main_loop(self):
         "Main plugin loop, runs in the 'background'"
         self.proc = []
         unique = self.config.get("unique", False)
         variables = state.variables.copy()
+
         while self.running:
             self.next_background_event.clear()
+
+            # Define the command template based on the 'unique' flag
+            cmd_template = self.config.get(
+                "command",
+                (
+                    'swaybg -o [output] -m fill -i "[file]"'
+                    if unique
+                    else 'swaybg -m fill -i "[file]"'
+                ),
+            )
+
             if unique:
-                cmd_template = self.config.get(
-                    "command", 'swaybg -o [output] -m fill -i "[file]"'
-                )
                 monitors = await self.hyprctlJSON("monitors")
                 old_filename = None
                 for monitor in monitors:
-                    filename = self.select_next_image().replace('"', '\\"')
+                    filename = prepare_for_quotes(self.select_next_image())
                     while filename == old_filename:
-                        filename = self.select_next_image().replace('"', '\\"')
+                        filename = prepare_for_quotes(self.select_next_image())
                     variables.update({"file": filename, "output": monitor["name"]})
                     await self._run_one(cmd_template, variables)
             else:
-                cmd_template = self.config.get("command", 'swaybg -m fill -i "[file]"')
                 filename = self.select_next_image().replace('"', '\\"')
                 variables.update({"file": filename})
                 await self._run_one(cmd_template, variables)
+
             await asyncio.sleep(1)  # wait for the command(s) to start
+
             # check if the command failed
             for proc in self.proc:
                 if proc.returncode:
                     await self.notify_error("wallpaper command failed")
 
             interval = asyncio.sleep(60 * self.config.get("interval", 10) - 1)
             await asyncio.wait(
```

### Comparing `pyprland-2.2.5/pyprland/plugins/workspaces_follow_focus.py` & `pyprland-2.2.6/pyprland/plugins/workspaces_follow_focus.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,35 +8,34 @@
 class Extension(Plugin):  # pylint: disable=missing-class-docstring
     workspace_list: list[int] = []
 
     async def on_reload(self):
         "rebuild workspaces list"
         self.workspace_list = list(range(1, self.config.get("max_workspaces", 10) + 1))
 
-    async def event_focusedmon(self, screenid_index):
+    async def event_focusedmon(self, screenid_name):
         "reacts to monitor changes"
-        monitor_id, workspace_id = screenid_index.split(",")
-        workspace_id = int(workspace_id)
+        monitor_id, workspace_name = screenid_name.split(",")
         # move every free workspace to the currently focused desktop
         busy_workspaces = set(
-            mon["activeWorkspace"]["id"]
+            mon["activeWorkspace"]["name"]
             for mon in cast(list[dict], await self.hyprctlJSON("monitors"))
             if mon["name"] != monitor_id
         )
         workspaces = [
-            w["id"]
+            w["name"]
             for w in cast(list[dict], await self.hyprctlJSON("workspaces"))
             if w["id"] > 0
         ]
 
         batch: list[str | list[str]] = []
         for n in workspaces:
-            if n in busy_workspaces or n == workspace_id:
+            if n in busy_workspaces or n == workspace_name:
                 continue
-            batch.append(f"moveworkspacetomonitor {n} {monitor_id}")
+            batch.append(f"moveworkspacetomonitor name:{n} {monitor_id}")
         await self.hyprctl(batch)
 
     async def run_change_workspace(self, direction: str):
         """<+1/-1> Switch workspaces of current monitor, avoiding displayed workspaces"""
         increment = int(direction)
         # get focused screen info
         monitors = await self.hyprctlJSON("monitors")
```

### Comparing `pyprland-2.2.5/pyproject.toml` & `pyprland-2.2.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyprland"
-version = "2.2.5"
+version = "2.2.6"
 description = "Hyperland plugin system - batteries included"
 authors = ["fdev31 <fdev31@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pyprland"}]
 homepage = "https://github.com/hyprland-community/pyprland/"
```

### Comparing `pyprland-2.2.5/PKG-INFO` & `pyprland-2.2.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprland
-Version: 2.2.5
+Version: 2.2.6
 Summary: Hyperland plugin system - batteries included
 Home-page: https://github.com/hyprland-community/pyprland/
 License: MIT
 Author: fdev31
 Author-email: fdev31@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -38,20 +38,20 @@
 - ["It just works very very well" - The Linux Cast (video)](https://youtu.be/Cjn0SFyyucY?si=hGb0TM9IDvlbcD6A&t=131) - February 2024
 - [You NEED This in your Hyprland Config - LibrePhoenix (video)](https://www.youtube.com/watch?v=CwGlm-rpok4) - October 2023 (*Now [TOML](https://toml.io/en/) format is preferred over [JSON](https://www.w3schools.com/js/js_json_intro.asp))
 
 ## Contributing
 
 Check out the [creating a pull request](https://docs.github.com/fr/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) document for guidance.
 
-- Report bugs or propose features [here](https://github.com/hyprland-community/pyprland/issues).
+- Report bugs or propose features [here](https://github.com/hyprland-community/pyprland/issues)
 - Improve our [wiki](https://github.com/hyprland-community/pyprland/wiki)
 
 and if you have coding skills you can also
 
-- Enhance test coverage in our [tests](https://github.com/hyprland-community/pyprland/tree/main/tests).
+- Enhance the coverage of our [tests](https://github.com/hyprland-community/pyprland/tree/main/tests)
 - Propose & write new plugins or enhancements
 
 ## Dependencies
 
 - **Hyprland** >= 0.37
 - **Python** >= 3.11
     - **aiofiles**
@@ -63,15 +63,15 @@
 
 ### 2.2
 
 - Added [wallpapers](https://github.com/hyprland-community/pyprland/wiki/wallpapers) and [system_notifier](https://github.com/hyprland-community/pyprland/wiki/system_notifier) plugins.
 - Refactor in 2.2.5
   - updated the syntax for [wallpapers](https://github.com/hyprland-community/pyprland/wiki/wallpapers)
   - deprecated `class_match` in [scratchpads](https://github.com/hyprland-community/pyprland/wiki/scratchpads)
-
+- Added [gbar](https://github.com/hyprland-community/pyprland/wiki/gbar) in 2.2.6
 ### 2.1
 
 - Requires Hyprland >= 0.37
 - [Monitors](https://github.com/hyprland-community/pyprland/wiki/monitors) plugin improvements.
 
 ### 2.0
```

