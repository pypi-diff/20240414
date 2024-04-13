# Comparing `tmp/zrb_noto-0.0.4.tar.gz` & `tmp/zrb_noto-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zrb_noto-0.0.4.tar", max compression
+gzip compressed data, was "zrb_noto-0.0.5.tar", max compression
```

## Comparing `zrb_noto-0.0.4.tar` & `zrb_noto-0.0.5.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     1165 2024-04-11 12:19:34.722909 zrb_noto-0.0.4/README.md
--rw-r--r--   0        0        0      755 2024-04-11 12:37:51.016873 zrb_noto-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      758 2024-04-11 12:19:34.762909 zrb_noto-0.0.4/src/zrb_noto/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 12:19:34.772909 zrb_noto-0.0.4/src/zrb_noto/__main__.py
--rw-r--r--   0        0        0     1039 2024-04-11 12:19:34.762909 zrb_noto-0.0.4/src/zrb_noto/_config.py
--rw-r--r--   0        0        0      242 2024-04-11 12:19:34.782909 zrb_noto-0.0.4/src/zrb_noto/_env.py
--rw-r--r--   0        0        0      148 2024-04-11 12:19:34.792909 zrb_noto-0.0.4/src/zrb_noto/_group.py
--rw-r--r--   0        0        0      127 2024-04-11 12:19:34.802909 zrb_noto-0.0.4/src/zrb_noto/_helper.py
--rw-r--r--   0        0        0      419 2024-04-11 12:19:34.782909 zrb_noto-0.0.4/src/zrb_noto/lint.py
--rw-r--r--   0        0        0       45 2024-04-11 12:19:34.842909 zrb_noto-0.0.4/src/zrb_noto/lint.sh
--rw-r--r--   0        0        0      695 2024-04-11 12:28:46.966901 zrb_noto-0.0.4/src/zrb_noto/list.py
--rw-r--r--   0        0        0      141 2024-04-11 12:19:34.792909 zrb_noto-0.0.4/src/zrb_noto/log/__init__.py
--rw-r--r--   0        0        0       86 2024-04-11 12:19:34.792909 zrb_noto-0.0.4/src/zrb_noto/log/_group.py
--rw-r--r--   0        0        0     2207 2024-04-11 12:19:34.802909 zrb_noto-0.0.4/src/zrb_noto/log/_helper.py
--rw-r--r--   0        0        0      994 2024-04-11 12:27:13.646173 zrb_noto-0.0.4/src/zrb_noto/log/add.py
--rw-r--r--   0        0        0      902 2024-04-11 12:27:50.860635 zrb_noto-0.0.4/src/zrb_noto/log/list.py
--rw-r--r--   0        0        0     1531 2024-04-11 12:25:19.223647 zrb_noto-0.0.4/src/zrb_noto/sync.py
--rw-r--r--   0        0        0     1580 2024-04-11 12:37:35.157181 zrb_noto-0.0.4/src/zrb_noto/sync.sh
--rw-r--r--   0        0        0      489 2024-04-11 12:19:34.802909 zrb_noto-0.0.4/src/zrb_noto/todo/__init__.py
--rw-r--r--   0        0        0    10420 2024-04-11 12:19:34.842909 zrb_noto-0.0.4/src/zrb_noto/todo/_data.py
--rw-r--r--   0        0        0       81 2024-04-11 12:19:34.822909 zrb_noto-0.0.4/src/zrb_noto/todo/_group.py
--rw-r--r--   0        0        0     6130 2024-04-11 12:19:34.832909 zrb_noto-0.0.4/src/zrb_noto/todo/_helper.py
--rw-r--r--   0        0        0     1204 2024-04-11 12:19:34.812909 zrb_noto-0.0.4/src/zrb_noto/todo/_input.py
--rw-r--r--   0        0        0     2737 2024-04-11 12:26:13.243337 zrb_noto-0.0.4/src/zrb_noto/todo/add.py
--rw-r--r--   0        0        0     1723 2024-04-11 12:31:34.213284 zrb_noto-0.0.4/src/zrb_noto/todo/complete.py
--rw-r--r--   0        0        0     1506 2024-04-11 12:34:18.586663 zrb_noto-0.0.4/src/zrb_noto/todo/delete.py
--rw-r--r--   0        0        0     3244 2024-04-11 12:32:49.162135 zrb_noto-0.0.4/src/zrb_noto/todo/edit.py
--rw-r--r--   0        0        0     1165 2024-04-11 12:30:34.264715 zrb_noto-0.0.4/src/zrb_noto/todo/find.py
--rw-r--r--   0        0        0       52 2024-04-11 12:19:34.812909 zrb_noto-0.0.4/src/zrb_noto/todo/kanban/__init__.py
--rw-r--r--   0        0        0     3759 2024-04-11 12:19:34.822909 zrb_noto-0.0.4/src/zrb_noto/todo/kanban/_helper.py
--rw-r--r--   0        0        0      621 2024-04-11 12:19:34.812909 zrb_noto-0.0.4/src/zrb_noto/todo/kanban/kanban.py
--rw-r--r--   0        0        0      539 2024-04-11 12:29:31.650165 zrb_noto-0.0.4/src/zrb_noto/todo/list.py
--rw-r--r--   0        0        0     1689 2024-04-11 12:35:59.958293 zrb_noto-0.0.4/src/zrb_noto/todo/start.py
--rw-r--r--   0        0        0     1706 2024-04-11 12:34:54.744324 zrb_noto-0.0.4/src/zrb_noto/todo/stop.py
--rw-r--r--   0        0        0      341 2024-04-11 12:19:34.782909 zrb_noto-0.0.4/src/zrb_noto/wiki.py
--rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 zrb_noto-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1165 2024-04-13 00:18:51.452685 zrb_noto-0.0.5/README.md
+-rw-r--r--   0        0        0      755 2024-04-13 23:19:24.848195 zrb_noto-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      796 2024-04-13 23:07:15.366681 zrb_noto-0.0.5/src/zrb_noto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 00:18:51.512683 zrb_noto-0.0.5/src/zrb_noto/__main__.py
+-rw-r--r--   0        0        0     1154 2024-04-13 02:23:48.982743 zrb_noto-0.0.5/src/zrb_noto/_config.py
+-rw-r--r--   0        0        0      242 2024-04-13 00:18:51.522683 zrb_noto-0.0.5/src/zrb_noto/_env.py
+-rw-r--r--   0        0        0      148 2024-04-13 00:18:51.542683 zrb_noto-0.0.5/src/zrb_noto/_group.py
+-rw-r--r--   0        0        0      127 2024-04-13 00:18:51.562682 zrb_noto-0.0.5/src/zrb_noto/_helper.py
+-rw-r--r--   0        0        0      419 2024-04-13 00:18:51.532683 zrb_noto-0.0.5/src/zrb_noto/lint.py
+-rw-r--r--   0        0        0       45 2024-04-13 00:18:51.582682 zrb_noto-0.0.5/src/zrb_noto/lint.sh
+-rw-r--r--   0        0        0      736 2024-04-13 10:36:05.467455 zrb_noto-0.0.5/src/zrb_noto/list.py
+-rw-r--r--   0        0        0      141 2024-04-13 00:18:51.542683 zrb_noto-0.0.5/src/zrb_noto/log/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-13 00:18:51.552682 zrb_noto-0.0.5/src/zrb_noto/log/_group.py
+-rw-r--r--   0        0        0     2289 2024-04-13 22:46:44.792866 zrb_noto-0.0.5/src/zrb_noto/log/_helper.py
+-rw-r--r--   0        0        0     1266 2024-04-13 02:26:54.718345 zrb_noto-0.0.5/src/zrb_noto/log/add.py
+-rw-r--r--   0        0        0      937 2024-04-13 10:35:06.620761 zrb_noto-0.0.5/src/zrb_noto/log/list.py
+-rw-r--r--   0        0        0     1407 2024-04-13 00:18:51.532683 zrb_noto-0.0.5/src/zrb_noto/sync.py
+-rw-r--r--   0        0        0     1580 2024-04-13 00:18:51.592681 zrb_noto-0.0.5/src/zrb_noto/sync.sh
+-rw-r--r--   0        0        0      543 2024-04-13 23:06:50.382852 zrb_noto-0.0.5/src/zrb_noto/todo/__init__.py
+-rw-r--r--   0        0        0    10498 2024-04-13 22:38:39.588287 zrb_noto-0.0.5/src/zrb_noto/todo/_data.py
+-rw-r--r--   0        0        0       81 2024-04-13 00:18:51.572682 zrb_noto-0.0.5/src/zrb_noto/todo/_group.py
+-rw-r--r--   0        0        0     6122 2024-04-13 23:04:04.330171 zrb_noto-0.0.5/src/zrb_noto/todo/_helper.py
+-rw-r--r--   0        0        0     1197 2024-04-13 00:18:51.562682 zrb_noto-0.0.5/src/zrb_noto/todo/_input.py
+-rw-r--r--   0        0        0     3208 2024-04-13 22:43:19.141379 zrb_noto-0.0.5/src/zrb_noto/todo/add.py
+-rw-r--r--   0        0        0     1676 2024-04-13 23:06:25.189727 zrb_noto-0.0.5/src/zrb_noto/todo/archive.py
+-rw-r--r--   0        0        0     1955 2024-04-13 22:38:54.258764 zrb_noto-0.0.5/src/zrb_noto/todo/complete.py
+-rw-r--r--   0        0        0     1893 2024-04-13 22:44:04.193308 zrb_noto-0.0.5/src/zrb_noto/todo/delete.py
+-rw-r--r--   0        0        0     3581 2024-04-13 22:43:59.252570 zrb_noto-0.0.5/src/zrb_noto/todo/edit.py
+-rw-r--r--   0        0        0     1221 2024-04-13 14:37:04.962328 zrb_noto-0.0.5/src/zrb_noto/todo/find.py
+-rw-r--r--   0        0        0       52 2024-04-13 00:18:51.562682 zrb_noto-0.0.5/src/zrb_noto/todo/kanban/__init__.py
+-rw-r--r--   0        0        0     3759 2024-04-13 00:18:51.572682 zrb_noto-0.0.5/src/zrb_noto/todo/kanban/_helper.py
+-rw-r--r--   0        0        0      756 2024-04-13 10:39:46.235073 zrb_noto-0.0.5/src/zrb_noto/todo/kanban/kanban.py
+-rw-r--r--   0        0        0      595 2024-04-13 14:37:30.714417 zrb_noto-0.0.5/src/zrb_noto/todo/list.py
+-rw-r--r--   0        0        0     1913 2024-04-13 22:39:27.614985 zrb_noto-0.0.5/src/zrb_noto/todo/start.py
+-rw-r--r--   0        0        0     1928 2024-04-13 22:39:43.494665 zrb_noto-0.0.5/src/zrb_noto/todo/stop.py
+-rw-r--r--   0        0        0      341 2024-04-13 00:18:51.522683 zrb_noto-0.0.5/src/zrb_noto/wiki.py
+-rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 zrb_noto-0.0.5/PKG-INFO
```

### Comparing `zrb_noto-0.0.4/README.md` & `zrb_noto-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `zrb_noto-0.0.4/pyproject.toml` & `zrb_noto-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zrb-noto"
-version = "0.0.4"
+version = "0.0.5"
 description = "Personal todo and logging management"
 authors = ["Go Frendi Gunawan <gofrendiasgard@gmail.com>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/state-alchemists/noto"
 repository = "https://github.com/state-alchemists/noto"
 documentation = "https://github.com/state-alchemists/noto"
```

### Comparing `zrb_noto-0.0.4/src/zrb_noto/__init__.py` & `zrb_noto-0.0.5/src/zrb_noto/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from ._group import noto_group, noto_wiki_group
 from .lint import lint_noto
 from .list import list_noto
 from .log import add_log, list_log, noto_log_group
 from .sync import sync_noto
 from .todo import (
     add_todo,
+    archive_todo,
     complete_todo,
     delete_todo,
     edit_todo,
     find_todo,
     list_todo,
     noto_todo_group,
     show_kanban,
@@ -20,14 +21,15 @@
 assert noto_group
 assert noto_wiki_group
 assert noto_log_group
 assert add_log
 assert list_log
 assert noto_todo_group
 assert add_todo
+assert archive_todo
 assert complete_todo
 assert delete_todo
 assert edit_todo
 assert find_todo
 assert show_kanban
 assert list_todo
 assert start_todo
```

### Comparing `zrb_noto-0.0.4/src/zrb_noto/_config.py` & `zrb_noto-0.0.5/src/zrb_noto/_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 from datetime import datetime
+from zrb.helper.string.conversion import to_boolean
 
 _HOME_DIR = os.path.expanduser("~")
 _SYSTEM_USER = os.getenv("USER", "incognito")
 _DEFAULT_REMOTE_GIT_URL = f"git@github.com:{_SYSTEM_USER}/daily.git"
 
+IS_AUTO_SYNC = to_boolean(os.getenv("NOTO_AUTO_SYNC", "true"))
 REMOTE_GIT_URL = os.getenv("NOTO_REMOTE_GIT", _DEFAULT_REMOTE_GIT_URL)
 LOCAL_REPO_DIR = os.path.abspath(os.getenv("NOTO_LOCAL_REPO", f"{_HOME_DIR}/daily"))
 TODO_FILE_PATH = os.getenv("NOTO_TODO_FILE", "todo.txt")
 DONE_FILE_PATH = os.getenv("NOTO_DONE_FILE", "done.txt")
 WIKI_DIR_PATH = os.getenv("NOTO_WIKI_DIR", "wiki")
 LOG_DIR_PATH = os.getenv("NOTO_LOG_DIR", "log")
```

### Comparing `zrb_noto-0.0.4/src/zrb_noto/list.py` & `zrb_noto-0.0.5/src/zrb_noto/todo/list.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-from typing import Any
-
 from zrb import Task, python_task, runner
 from zrb.helper.task import show_lines
 
-from ._group import noto_group
-from .log._helper import get_pretty_log_lines
-from .sync import create_sync_noto_task
-from .todo._helper import get_pretty_todo_item_lines, get_todo_items
+from .._config import IS_AUTO_SYNC
+from ..sync import create_sync_noto_task
+from ._group import noto_todo_group
+from ._helper import get_pretty_todo_item_lines, get_todo_items
 
 
 @python_task(
     name="list",
-    group=noto_group,
-    description="List todo",
+    group=noto_todo_group,
     retry=0,
 )
-def list_noto(*args: Any, **kwargs: Any):
+def list_todo(*args, **kwargs):
     task: Task = kwargs.get("_task")
-    items = get_todo_items(completed=False)
     show_lines(
-        task, *get_pretty_log_lines(), "", *get_pretty_todo_item_lines(items)
+        task,
+        *get_pretty_todo_item_lines(get_todo_items()),
     )
 
 
-create_sync_noto_task(name="pre-sync") >> list_noto
-runner.register(list_noto)
+if IS_AUTO_SYNC:
+    create_sync_noto_task(name="pre-sync") >> list_todo
+runner.register(list_todo)
```

### Comparing `zrb_noto-0.0.4/src/zrb_noto/log/_helper.py` & `zrb_noto-0.0.5/src/zrb_noto/log/_helper.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,17 +5,20 @@
 from typing import List, Optional
 
 from zrb.helper.accessories.color import colored
 
 from .._config import CURRENT_TIME, LOG_ABS_DIR_PATH
 
 _STATUS_COLOR_MAP = {
-    "START": "cyan",
-    "COMPLETE": "green",
-    "STOP": "yellow",
+    "START": "light_cyan",
+    "COMPLETE": "light_green",
+    "STOP": "light_yellow",
+    "ADD": "cyan",
+    "EDIT": "green",
+    "DELETE": "yellow",
 }
 
 
 def get_log_file_name(current_time: datetime = CURRENT_TIME) -> str:
     year = current_time.year
     month = current_time.strftime("%m")
     date = current_time.strftime("%d")
```

### Comparing `zrb_noto-0.0.4/src/zrb_noto/log/add.py` & `zrb_noto-0.0.5/src/zrb_noto/log/add.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from zrb import StrInput, Task, python_task, runner
+from zrb.helper.accessories.color import colored
 from zrb.helper.task import show_lines
 
+from .._config import IS_AUTO_SYNC
 from ..sync import create_sync_noto_task
 from ._group import noto_log_group
 from ._helper import append_log_item, get_pretty_log_lines
 
 
 @python_task(
     name="add-item",
@@ -15,15 +17,17 @@
             prompt="Text",
             default="",
         ),
     ],
     retry=0,
 )
 def add_item(*args, **kwargs):
+    task: Task = kwargs.get("_task")
     text = kwargs.get("text")
+    task.print_out(colored(f"Adding log: {text}", color="yellow"))
     append_log_item(text)
 
 
 @python_task(
     name="add",
     group=noto_log_group,
     inputs=[
@@ -37,9 +41,18 @@
     retry=0,
 )
 def add_log(*args, **kwargs):
     task: Task = kwargs.get("_task")
     show_lines(task, *get_pretty_log_lines())
 
 
-create_sync_noto_task(name="pre-sync") >> add_item >> create_sync_noto_task(name="post-sync") >> add_log  # noqa
+if IS_AUTO_SYNC:
+    (
+        create_sync_noto_task(name="pre-sync")
+        >> add_item
+        >> create_sync_noto_task(name="post-sync")
+        >> add_log
+    )
+else:
+    add_item >> add_log
+
 runner.register(add_log)
```

### Comparing `zrb_noto-0.0.4/src/zrb_noto/log/list.py` & `zrb_noto-0.0.5/src/zrb_noto/log/list.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import datetime
 
 from zrb import StrInput, Task, python_task, runner
 from zrb.helper.task import show_lines
 
-from .._config import CURRENT_TIME
+from .._config import CURRENT_TIME, IS_AUTO_SYNC
 from ..sync import create_sync_noto_task
 from ._group import noto_log_group
 from ._helper import get_log_file_name, get_pretty_log_lines
 
 
 @python_task(
     name="list",
@@ -26,9 +26,10 @@
     task: Task = kwargs.get("_task")
     date_str = kwargs.get("date")
     current_time = datetime.strptime(date_str, "%Y-%m-%d")
     file_name = get_log_file_name(current_time)
     show_lines(task, *get_pretty_log_lines(file_name))
 
 
-create_sync_noto_task(name="pre-sync") >> list_log
+if IS_AUTO_SYNC:
+    create_sync_noto_task(name="pre-sync") >> list_log
 runner.register(list_log)
```

### Comparing `zrb_noto-0.0.4/src/zrb_noto/sync.py` & `zrb_noto-0.0.5/src/zrb_noto/sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,24 +21,16 @@
         name=name,
         group=group,
         description="Sync noto",
         upstreams=upstreams,
         envs=[
             LOCAL_REPO_DIR_ENV,
             REMOTE_GIT_URL_ENV,
-            Env(
-                name="IGNORE_ERROR",
-                os_name="",
-                default="1" if ignore_error else "0"
-            ),
-            Env(
-                name="COMMIT_MESSAGE",
-                os_name="",
-                default="{{input.commit_message}}"
-            ),
+            Env(name="IGNORE_ERROR", os_name="", default="1" if ignore_error else "0"),
+            Env(name="COMMIT_MESSAGE", os_name="", default="{{input.commit_message}}"),
         ],
         retry=retry,
         cmd_path=os.path.join(_CURRENT_DIR, "sync.sh"),
         should_show_cmd=False,
         should_print_cmd_result=False,
     )
     if custom_commit_message:
```

### Comparing `zrb_noto-0.0.4/src/zrb_noto/sync.sh` & `zrb_noto-0.0.5/src/zrb_noto/sync.sh`

 * *Files identical despite different names*

### Comparing `zrb_noto-0.0.4/src/zrb_noto/todo/_data.py` & `zrb_noto-0.0.5/src/zrb_noto/todo/_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,14 +206,17 @@
         )
 
     def _get_status_icon(self):
         status = self.get_status()
         status_str = STATUS_ICON_MAP.get(status)
         return status_str
 
+    def get_id(self):
+        return self.keyval.get("id", "xxxx-xxxx-xxxx")
+
     def get_status(self):
         if self.completed:
             return "COMPLETED"
         status = self.keyval.get("status", "new").upper()
         if status not in STATUS_ICON_MAP:
             status = "NEW"
         return status
```

### Comparing `zrb_noto-0.0.4/src/zrb_noto/todo/_helper.py` & `zrb_noto-0.0.5/src/zrb_noto/todo/_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 
 def append_todo_item(item: Item, file_name: str = TODO_ABS_FILE_PATH) -> str:
     dir_path = Path(os.path.dirname(file_name))
     dir_path.mkdir(parents=True, exist_ok=True)
     items = get_todo_items(file_name=file_name)
     items.append(item)
-    _write_items(items, file_name)
+    save_items(items, file_name)
 
 
 def get_todo_items(
     contexts: List[str] = [],
     projects: List[str] = [],
     search: str = "",
     completed: Optional[bool] = None,
@@ -115,24 +115,24 @@
 
 def delete_todo_item(item: Item, file_name: str = TODO_ABS_FILE_PATH):
     items = [
         old_item
         for old_item in get_todo_items(file_name=file_name)
         if old_item.description != item.old_description
     ]
-    _write_items(items, file_name)
+    save_items(items, file_name)
 
 
 def replace_todo_item(item: Item, file_name: str = TODO_ABS_FILE_PATH):
     items = get_todo_items(file_name=file_name)
     for index, existing_item in enumerate(items):
         if item.old_description == existing_item.description:
             items[index] = item
             break
-    _write_items(items, file_name)
+    save_items(items, file_name)
 
 
 def get_existing_todo_contexts(file_name: str = TODO_ABS_FILE_PATH) -> List[str]:
     existing_contexts = set()
     items = get_todo_items(file_name=file_name)
     for item in items:
         existing_contexts.update(item.contexts)
@@ -167,15 +167,15 @@
         keyval_part = keyval_str.strip().split(":")
         if len(keyval_part) < 2:
             raise Exception(f"Invalid keyval: {keyval_str}")
         keyval[keyval_part[0]] = keyval_part[1]
     return keyval
 
 
-def _write_items(items: List[Item], file_name: str = TODO_ABS_FILE_PATH):
+def save_items(items: List[Item], file_name: str = TODO_ABS_FILE_PATH):
     items = _sort_items(items)
     with open(file_name, "w") as file:
         file.write("\n".join([item.as_str() for item in items]))
         file.write("\n")
 
 
 def _sort_items(items: List[Item]) -> List[Item]:
```

### Comparing `zrb_noto-0.0.4/src/zrb_noto/todo/_input.py` & `zrb_noto-0.0.5/src/zrb_noto/todo/_input.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,22 +5,21 @@
 
 _EXISTING_CONTEXT_STR = ",".join(get_existing_todo_contexts())
 _EXISTING_PROJECT_STR = ",".join(get_existing_todo_projects())
 
 task_input = StrInput(
     name="task",
     shortcut="t",
-    prompt="Task",
+    prompt="Task name or id",
     prompt_required=True,
     default="",
 )
 
 description_input = StrInput(
     name="description",
-    shortcut="t",
     prompt="Description",
     default="",
 )
 
 priority_input = StrInput(
     name="priority",
     prompt="Priority",
```

### Comparing `zrb_noto-0.0.4/src/zrb_noto/todo/add.py` & `zrb_noto-0.0.5/src/zrb_noto/todo/add.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,42 @@
-from zrb import Task, python_task, runner
+from zrb import StrInput, Task, python_task, runner
 from zrb.helper.accessories.color import colored
 from zrb.helper.task import show_lines
 
-from .._config import CURRENT_TIME
+from .._config import CURRENT_TIME, IS_AUTO_SYNC
+from ..log._helper import append_log_item, get_pretty_log_lines
 from ..sync import create_sync_noto_task
 from ._data import Item
 from ._group import noto_todo_group
 from ._helper import (
     append_todo_item,
     get_pretty_todo_item_lines,
     get_todo_items,
     read_keyval_input,
 )
 from ._input import (
     context_input,
     date_input,
-    description_input,
     keyval_input,
     priority_input,
     project_input,
 )
 
+new_description_input = StrInput(
+    name="description",
+    shortcut="t",
+    prompt="Description",
+    default="",
+)
+
 
 @python_task(
     name="add-item",
     inputs=[
-        description_input,
+        new_description_input,
         priority_input,
         project_input,
         context_input,
         keyval_input,
         date_input,
     ],
     retry=0,
@@ -75,30 +82,43 @@
         description=description,
         priority=priority,
         creation_date=CURRENT_TIME,
         contexts=contexts,
         projects=projects,
         keyval=keyval,
     )
+    task.print_out(colored(f"Adding task: {item.description}", color="yellow"))
     append_todo_item(item=item)
+    append_log_item(f"__ADD__ [{item.get_id()}] {item.description}")
 
 
 @python_task(
     name="add",
     group=noto_todo_group,
     inputs=[
-        description_input,
+        new_description_input,
         priority_input,
         project_input,
         context_input,
         keyval_input,
         date_input,
     ],
     retry=0,
 )
 def add_todo(*args, **kwargs):
     task: Task = kwargs.get("_task")
-    show_lines(task, *get_pretty_todo_item_lines(get_todo_items()))
+    show_lines(
+        task, *get_pretty_log_lines(), "", *get_pretty_todo_item_lines(get_todo_items())
+    )
 
 
-create_sync_noto_task(name="pre-sync") >> add_item >> create_sync_noto_task(name="post-sync") >> add_todo  # noqa
+if IS_AUTO_SYNC:
+    (
+        create_sync_noto_task(name="pre-sync")
+        >> add_item
+        >> create_sync_noto_task(name="post-sync")
+        >> add_todo
+    )
+else:
+    add_item >> add_todo
+
 runner.register(add_todo)
```

### Comparing `zrb_noto-0.0.4/src/zrb_noto/todo/complete.py` & `zrb_noto-0.0.5/src/zrb_noto/todo/complete.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from zrb import Task, python_task, runner
 from zrb.helper.accessories.color import colored
 from zrb.helper.task import show_lines
 
+from .._config import IS_AUTO_SYNC
 from ..log._helper import append_log_item, get_pretty_log_lines
 from ..sync import create_sync_noto_task
 from ._group import noto_todo_group
 from ._helper import complete_todo_item, get_pretty_todo_item_lines, get_todo_items
 from ._input import task_input
 
 
@@ -31,16 +32,17 @@
             task,
             colored("⚠️  NOT COMPLETED: Multiple task found", color="light_red"),
             "List of matched tasks:",
             *get_pretty_todo_item_lines(items),
         )
         return
     item = items[0]
+    task.print_out(colored(f"Completing task: {item.description}", color="yellow"))
     complete_todo_item(item)
-    append_log_item(f"__COMPLETE__ {item.description}")
+    append_log_item(f"__COMPLETE__ [{item.get_id()}] {item.description}")
 
 
 @python_task(
     name="complete",
     group=noto_todo_group,
     inputs=[task_input],
     retry=0,
@@ -48,9 +50,18 @@
 def complete_todo(*args, **kwargs):
     task: Task = kwargs.get("_task")
     show_lines(
         task, *get_pretty_log_lines(), "", *get_pretty_todo_item_lines(get_todo_items())
     )
 
 
-create_sync_noto_task(name="pre-sync") >> complete_item >> create_sync_noto_task(name="post-sync") >> complete_todo  # noqa
+if IS_AUTO_SYNC:
+    (
+        create_sync_noto_task(name="pre-sync")
+        >> complete_item
+        >> create_sync_noto_task(name="post-sync")
+        >> complete_todo
+    )
+else:
+    complete_item >> complete_todo
+
 runner.register(complete_todo)
```

### Comparing `zrb_noto-0.0.4/src/zrb_noto/todo/delete.py` & `zrb_noto-0.0.5/src/zrb_noto/todo/stop.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,68 @@
 from zrb import Task, python_task, runner
 from zrb.helper.accessories.color import colored
 from zrb.helper.task import show_lines
 
+from .._config import IS_AUTO_SYNC
+from ..log._helper import append_log_item, get_pretty_log_lines
 from ..sync import create_sync_noto_task
 from ._group import noto_todo_group
-from ._helper import delete_todo_item, get_pretty_todo_item_lines, get_todo_items
+from ._helper import get_pretty_todo_item_lines, get_todo_items, stop_todo_item
 from ._input import task_input
 
 
 @python_task(
-    name="delete-item",
+    name="stop-item",
+    group=noto_todo_group,
     inputs=[task_input],
     retry=0,
 )
-def delete_item(*args, **kwargs):
+def stop_item(*args, **kwargs):
     task: Task = kwargs.get("_task")
     search = kwargs.get("task")
-    items = get_todo_items(search=search)
+    items = get_todo_items(search=search, completed=False)
     if len(items) == 0:
         show_lines(
             task,
-            colored("⚠️  NOT DELETED: Task not found", color="light_red"),
+            colored("⚠️  NOT STOPPED: Task not found", color="light_red"),
             "List of available tasks:",
-            *get_pretty_todo_item_lines(get_todo_items()),
+            *get_pretty_todo_item_lines(get_todo_items(completed=False)),
         )
         return
     if len(items) > 1:
         show_lines(
             task,
-            colored("⚠️  NOT DELETED: Multiple task found", color="light_red"),
+            colored("⚠️  NOT STOPPED: Multiple task found", color="light_red"),
             "List of matched tasks:",
             *get_pretty_todo_item_lines(items),
         )
         return
     item = items[0]
-    delete_todo_item(item)
+    task.print_out(colored(f"Stopping task: {item.description}", color="yellow"))
+    stop_todo_item(item)
+    append_log_item(f"__STOP__ [{item.get_id()}] {item.description}")
 
 
 @python_task(
-    name="delete",
+    name="stop",
     group=noto_todo_group,
     inputs=[task_input],
     retry=0,
 )
-def delete_todo(*args, **kwargs):
+def stop_todo(*args, **kwargs):
     task: Task = kwargs.get("_task")
-    show_lines(task, *get_pretty_todo_item_lines(get_todo_items()))
-
+    show_lines(
+        task, *get_pretty_log_lines(), "", *get_pretty_todo_item_lines(get_todo_items())
+    )
+
+
+if IS_AUTO_SYNC:
+    (
+        create_sync_noto_task(name="pre-sync")
+        >> stop_item
+        >> create_sync_noto_task(name="post-sync")
+        >> stop_todo
+    )
+else:
+    stop_item >> stop_todo
 
-create_sync_noto_task(name="pre-sync") >> delete_item >> create_sync_noto_task(name="post-sync") >> delete_todo  # noqa
-runner.register(delete_todo)
+runner.register(stop_todo)
```

### Comparing `zrb_noto-0.0.4/src/zrb_noto/todo/edit.py` & `zrb_noto-0.0.5/src/zrb_noto/todo/edit.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from zrb import Task, python_task, runner
 from zrb.helper.accessories.color import colored
 from zrb.helper.task import show_lines
 
+from .._config import IS_AUTO_SYNC
+from ..log._helper import append_log_item, get_pretty_log_lines
 from ..log._helper import get_pretty_log_lines
 from ..sync import create_sync_noto_task
 from ._group import noto_todo_group
 from ._helper import (
     get_pretty_todo_item_lines,
     get_todo_items,
     read_keyval_input,
@@ -85,15 +87,17 @@
     if project_str.strip() != "":
         item.projects = [project.strip() for project in project_str.split(",")]
     # keyval
     keyval_input = kwargs.get("keyval")
     if keyval_input.strip() != "":
         item.set_keyval(read_keyval_input(keyval_input))
     # save item
+    task.print_out(colored(f"Editing task: {item.description}", color="yellow"))
     replace_todo_item(item)
+    append_log_item(f"__EDIT__ [{item.get_id()}] {item.description}")
 
 
 @python_task(
     name="edit",
     group=noto_todo_group,
     inputs=[
         task_input,
@@ -109,9 +113,18 @@
 def edit_todo(*args, **kwargs):
     task: Task = kwargs.get("_task")
     show_lines(
         task, *get_pretty_log_lines(), "", *get_pretty_todo_item_lines(get_todo_items())
     )
 
 
-create_sync_noto_task(name="pre-sync") >> edit_item >> create_sync_noto_task(name="post-sync") >> edit_todo  # noqa
+if IS_AUTO_SYNC:
+    (
+        create_sync_noto_task(name="pre-sync")
+        >> edit_item
+        >> create_sync_noto_task(name="post-sync")
+        >> edit_todo
+    )
+else:
+    edit_item >> edit_todo
+
 runner.register(edit_todo)
```

### Comparing `zrb_noto-0.0.4/src/zrb_noto/todo/find.py` & `zrb_noto-0.0.5/src/zrb_noto/todo/find.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from zrb import Task, python_task, runner
 from zrb.helper.task import show_lines
 
+from .._config import IS_AUTO_SYNC
 from ..sync import create_sync_noto_task
 from ._group import noto_todo_group
 from ._helper import get_pretty_todo_item_lines, get_todo_items
 from ._input import context_input, project_input, task_input
 
 
 @python_task(
@@ -31,9 +32,10 @@
         f"Search:   {search}",
         *get_pretty_todo_item_lines(
             get_todo_items(contexts=contexts, projects=projects, search=search)
         ),
     )
 
 
-create_sync_noto_task(name="pre-sync") >> find_todo
+if IS_AUTO_SYNC:
+    create_sync_noto_task(name="pre-sync") >> find_todo
 runner.register(find_todo)
```

### Comparing `zrb_noto-0.0.4/src/zrb_noto/todo/kanban/_helper.py` & `zrb_noto-0.0.5/src/zrb_noto/todo/kanban/_helper.py`

 * *Files identical despite different names*

### Comparing `zrb_noto-0.0.4/src/zrb_noto/todo/start.py` & `zrb_noto-0.0.5/src/zrb_noto/todo/start.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from zrb import Task, python_task, runner
 from zrb.helper.accessories.color import colored
 from zrb.helper.task import show_lines
 
+from .._config import IS_AUTO_SYNC
 from ..log._helper import append_log_item, get_pretty_log_lines
 from ..sync import create_sync_noto_task
 from ._group import noto_todo_group
 from ._helper import get_pretty_todo_item_lines, get_todo_items, start_todo_item
 from ._input import task_input
 
 
@@ -31,16 +32,17 @@
             task,
             colored("⚠️  NOT STARTED: Multiple task found", color="light_red"),
             "List of matched tasks:",
             *get_pretty_todo_item_lines(items),
         )
         return
     item = items[0]
+    task.print_out(colored(f"Starting task: {item.description}", color="yellow"))
     start_todo_item(item)
-    append_log_item(f"__START__ {item.description}")
+    append_log_item(f"__START__ [{item.get_id()}] {item.description}")
 
 
 @python_task(
     name="start",
     group=noto_todo_group,
     inputs=[task_input],
     retry=0,
@@ -48,9 +50,18 @@
 def start_todo(*args, **kwargs):
     task: Task = kwargs.get("_task")
     show_lines(
         task, *get_pretty_log_lines(), "", *get_pretty_todo_item_lines(get_todo_items())
     )
 
 
-create_sync_noto_task(name="pre-sync") >> start_item >> create_sync_noto_task(name="post-sync") >> start_todo  # noqa
+if IS_AUTO_SYNC:
+    (
+        create_sync_noto_task(name="pre-sync")
+        >> start_item
+        >> create_sync_noto_task(name="post-sync")
+        >> start_todo
+    )
+else:
+    start_item >> start_todo
+
 runner.register(start_todo)
```

### Comparing `zrb_noto-0.0.4/PKG-INFO` & `zrb_noto-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zrb-noto
-Version: 0.0.4
+Version: 0.0.5
 Summary: Personal todo and logging management
 Home-page: https://github.com/state-alchemists/noto
 License: AGPL-3.0-or-later
 Author: Go Frendi Gunawan
 Author-email: gofrendiasgard@gmail.com
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

