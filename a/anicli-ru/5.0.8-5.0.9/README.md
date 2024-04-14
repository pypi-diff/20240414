# Comparing `tmp/anicli_ru-5.0.8.tar.gz` & `tmp/anicli_ru-5.0.9.tar.gz`

## Comparing `anicli_ru-5.0.8.tar` & `anicli_ru-5.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 anicli_ru-5.0.8/app.py
--rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 anicli_ru-5.0.8/anicli/__init__.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 anicli_ru-5.0.8/anicli/_completion.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 anicli_ru-5.0.8/anicli/_validator.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 anicli_ru-5.0.8/anicli/cli_utlis.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 anicli_ru-5.0.8/anicli/log.py
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 anicli_ru-5.0.8/anicli/utils.py
--rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 anicli_ru-5.0.8/anicli/views.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 anicli_ru-5.0.8/anicli/cli/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anicli_ru-5.0.8/anicli/cli/compat.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 anicli_ru-5.0.8/anicli/cli/config.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 anicli_ru-5.0.8/anicli/cli/events.py
--rw-r--r--   0        0        0     7530 2020-02-02 00:00:00.000000 anicli_ru-5.0.8/anicli/cli/ongoing.py
--rw-r--r--   0        0        0     6942 2020-02-02 00:00:00.000000 anicli_ru-5.0.8/anicli/cli/player.py
--rw-r--r--   0        0        0     7686 2020-02-02 00:00:00.000000 anicli_ru-5.0.8/anicli/cli/search.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 anicli_ru-5.0.8/anicli/cli/slice_play.py
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 anicli_ru-5.0.8/anicli/cli/video_utils.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 anicli_ru-5.0.8/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 anicli_ru-5.0.8/LICENSE
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 anicli_ru-5.0.8/README.md
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 anicli_ru-5.0.8/pyproject.toml
--rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 anicli_ru-5.0.8/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 anicli_ru-5.0.9/app.py
+-rw-r--r--   0        0        0     3177 2020-02-02 00:00:00.000000 anicli_ru-5.0.9/anicli/__init__.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 anicli_ru-5.0.9/anicli/_completion.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 anicli_ru-5.0.9/anicli/_validator.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 anicli_ru-5.0.9/anicli/cli_utlis.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 anicli_ru-5.0.9/anicli/log.py
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 anicli_ru-5.0.9/anicli/utils.py
+-rw-r--r--   0        0        0     4236 2020-02-02 00:00:00.000000 anicli_ru-5.0.9/anicli/views.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 anicli_ru-5.0.9/anicli/cli/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 anicli_ru-5.0.9/anicli/cli/compat.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 anicli_ru-5.0.9/anicli/cli/config.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 anicli_ru-5.0.9/anicli/cli/events.py
+-rw-r--r--   0        0        0     7530 2020-02-02 00:00:00.000000 anicli_ru-5.0.9/anicli/cli/ongoing.py
+-rw-r--r--   0        0        0     6942 2020-02-02 00:00:00.000000 anicli_ru-5.0.9/anicli/cli/player.py
+-rw-r--r--   0        0        0     7686 2020-02-02 00:00:00.000000 anicli_ru-5.0.9/anicli/cli/search.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 anicli_ru-5.0.9/anicli/cli/slice_play.py
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 anicli_ru-5.0.9/anicli/cli/video_utils.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 anicli_ru-5.0.9/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 anicli_ru-5.0.9/LICENSE
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 anicli_ru-5.0.9/README.md
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 anicli_ru-5.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4936 2020-02-02 00:00:00.000000 anicli_ru-5.0.9/PKG-INFO
```

### Comparing `anicli_ru-5.0.8/anicli/__init__.py` & `anicli_ru-5.0.9/anicli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import importlib
 import warnings
 
 import pkg_resources
 
 from anicli.cli import APP
 
-__version__ = "5.0.8"
+__version__ = "5.0.9"
 
 
 def _get_version():
     return f"""anicli-ru {__version__}; anicli-api {pkg_resources.get_distribution("anicli-api").version}"""
 
 
 def get_modules(package_name='anicli_api.source'):
```

### Comparing `anicli_ru-5.0.8/anicli/_completion.py` & `anicli_ru-5.0.9/anicli/_completion.py`

 * *Files identical despite different names*

### Comparing `anicli_ru-5.0.8/anicli/_validator.py` & `anicli_ru-5.0.9/anicli/_validator.py`

 * *Files identical despite different names*

### Comparing `anicli_ru-5.0.8/anicli/cli_utlis.py` & `anicli_ru-5.0.9/anicli/cli_utlis.py`

 * *Files identical despite different names*

### Comparing `anicli_ru-5.0.8/anicli/utils.py` & `anicli_ru-5.0.9/anicli/utils.py`

 * *Files identical despite different names*

### Comparing `anicli_ru-5.0.8/anicli/views.py` & `anicli_ru-5.0.9/anicli/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from dataclasses import asdict
+from attr import asdict
+
 from typing import TYPE_CHECKING, Any, List
 
 from prompt_toolkit import HTML, print_formatted_text
 from prompt_toolkit.application import Application
 from prompt_toolkit.formatted_text import FormattedText
 from prompt_toolkit.key_binding import KeyBindings
 from prompt_toolkit.layout.containers import HSplit, Window
```

### Comparing `anicli_ru-5.0.8/anicli/cli/config.py` & `anicli_ru-5.0.9/anicli/cli/config.py`

 * *Files identical despite different names*

### Comparing `anicli_ru-5.0.8/anicli/cli/events.py` & `anicli_ru-5.0.9/anicli/cli/events.py`

 * *Files identical despite different names*

### Comparing `anicli_ru-5.0.8/anicli/cli/ongoing.py` & `anicli_ru-5.0.9/anicli/cli/ongoing.py`

 * *Files identical despite different names*

### Comparing `anicli_ru-5.0.8/anicli/cli/player.py` & `anicli_ru-5.0.9/anicli/cli/player.py`

 * *Files identical despite different names*

### Comparing `anicli_ru-5.0.8/anicli/cli/search.py` & `anicli_ru-5.0.9/anicli/cli/search.py`

 * *Files identical despite different names*

### Comparing `anicli_ru-5.0.8/anicli/cli/slice_play.py` & `anicli_ru-5.0.9/anicli/cli/slice_play.py`

 * *Files identical despite different names*

### Comparing `anicli_ru-5.0.8/anicli/cli/video_utils.py` & `anicli_ru-5.0.9/anicli/cli/video_utils.py`

 * *Files identical despite different names*

### Comparing `anicli_ru-5.0.8/.gitignore` & `anicli_ru-5.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `anicli_ru-5.0.8/LICENSE` & `anicli_ru-5.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `anicli_ru-5.0.8/README.md` & `anicli_ru-5.0.9/README.md`

 * *Files identical despite different names*

### Comparing `anicli_ru-5.0.8/pyproject.toml` & `anicli_ru-5.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anicli_ru-5.0.8/PKG-INFO` & `anicli_ru-5.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anicli-ru
-Version: 5.0.8
+Version: 5.0.9
 Summary: cli tool for watching anime
 Project-URL: Documentation, https://github.com/vypivshiy/ani-cli-ru#readme
 Project-URL: Issues, https://github.com/vypivshiy/ani-cli-ru/issues
 Project-URL: Source, https://github.com/vypivshiy/ani-cli-ru
 Author: vypivshiy
 License-Expression: MIT
 License-File: LICENSE
```

