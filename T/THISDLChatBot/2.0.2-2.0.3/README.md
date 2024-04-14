# Comparing `tmp/THISDLChatBot-2.0.2.tar.gz` & `tmp/THISDLChatBot-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "THISDLChatBot-2.0.2.tar", last modified: Sun Apr 14 09:50:52 2024, max compression
+gzip compressed data, was "THISDLChatBot-2.0.3.tar", last modified: Sun Apr 14 10:01:55 2024, max compression
```

## Comparing `THISDLChatBot-2.0.2.tar` & `THISDLChatBot-2.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 09:50:52.926740 THISDLChatBot-2.0.2/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2024-04-14 03:22:44.000000 THISDLChatBot-2.0.2/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      347 2024-04-14 09:50:52.926510 THISDLChatBot-2.0.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1220 2024-04-14 09:11:13.000000 THISDLChatBot-2.0.2/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 09:50:52.925240 THISDLChatBot-2.0.2/THISDLChatBot/
--rwxrwxrwx   0 root         (0) root         (0)    31138 2024-04-14 09:39:36.000000 THISDLChatBot-2.0.2/THISDLChatBot/Bot.py
--rwxrwxrwx   0 root         (0) root         (0)      467 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.2/THISDLChatBot/CommandProcessor.py
--rwxrwxrwx   0 root         (0) root         (0)     5050 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.2/THISDLChatBot/Config.py
--rwxrwxrwx   0 root         (0) root         (0)      103 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.2/THISDLChatBot/Exceptions.py
--rwxrwxrwx   0 root         (0) root         (0)      594 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.2/THISDLChatBot/Friend.py
--rwxrwxrwx   0 root         (0) root         (0)      914 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.2/THISDLChatBot/Group.py
--rwxrwxrwx   0 root         (0) root         (0)     2818 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.2/THISDLChatBot/Logger.py
--rwxrwxrwx   0 root         (0) root         (0)     2658 2024-04-14 07:43:55.000000 THISDLChatBot-2.0.2/THISDLChatBot/Message.py
--rwxrwxrwx   0 root         (0) root         (0)      391 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.2/THISDLChatBot/MessageProcessor.py
--rwxrwxrwx   0 root         (0) root         (0)      856 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.2/THISDLChatBot/Plugin.py
--rwxrwxrwx   0 root         (0) root         (0)      102 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.2/THISDLChatBot/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 09:50:52.926203 THISDLChatBot-2.0.2/THISDLChatBot.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      347 2024-04-14 09:50:52.000000 THISDLChatBot-2.0.2/THISDLChatBot.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      497 2024-04-14 09:50:52.000000 THISDLChatBot-2.0.2/THISDLChatBot.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-14 09:50:52.000000 THISDLChatBot-2.0.2/THISDLChatBot.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       37 2024-04-14 09:50:52.000000 THISDLChatBot-2.0.2/THISDLChatBot.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       14 2024-04-14 09:50:52.000000 THISDLChatBot-2.0.2/THISDLChatBot.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-14 09:50:52.926787 THISDLChatBot-2.0.2/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      388 2024-04-14 09:50:31.000000 THISDLChatBot-2.0.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 10:01:55.266300 THISDLChatBot-2.0.3/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2024-04-14 03:22:44.000000 THISDLChatBot-2.0.3/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      347 2024-04-14 10:01:55.266022 THISDLChatBot-2.0.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1220 2024-04-14 09:11:13.000000 THISDLChatBot-2.0.3/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 10:01:55.264629 THISDLChatBot-2.0.3/THISDLChatBot/
+-rwxrwxrwx   0 root         (0) root         (0)    31138 2024-04-14 09:39:36.000000 THISDLChatBot-2.0.3/THISDLChatBot/Bot.py
+-rwxrwxrwx   0 root         (0) root         (0)      462 2024-04-14 09:53:31.000000 THISDLChatBot-2.0.3/THISDLChatBot/CommandProcessor.py
+-rwxrwxrwx   0 root         (0) root         (0)     5050 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.3/THISDLChatBot/Config.py
+-rwxrwxrwx   0 root         (0) root         (0)      103 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.3/THISDLChatBot/Exceptions.py
+-rwxrwxrwx   0 root         (0) root         (0)      594 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.3/THISDLChatBot/Friend.py
+-rwxrwxrwx   0 root         (0) root         (0)      914 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.3/THISDLChatBot/Group.py
+-rwxrwxrwx   0 root         (0) root         (0)     2818 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.3/THISDLChatBot/Logger.py
+-rwxrwxrwx   0 root         (0) root         (0)     2658 2024-04-14 07:43:55.000000 THISDLChatBot-2.0.3/THISDLChatBot/Message.py
+-rwxrwxrwx   0 root         (0) root         (0)      391 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.3/THISDLChatBot/MessageProcessor.py
+-rwxrwxrwx   0 root         (0) root         (0)      856 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.3/THISDLChatBot/Plugin.py
+-rwxrwxrwx   0 root         (0) root         (0)      102 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.3/THISDLChatBot/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 10:01:55.265648 THISDLChatBot-2.0.3/THISDLChatBot.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      347 2024-04-14 10:01:55.000000 THISDLChatBot-2.0.3/THISDLChatBot.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      497 2024-04-14 10:01:55.000000 THISDLChatBot-2.0.3/THISDLChatBot.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-14 10:01:55.000000 THISDLChatBot-2.0.3/THISDLChatBot.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       37 2024-04-14 10:01:55.000000 THISDLChatBot-2.0.3/THISDLChatBot.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       14 2024-04-14 10:01:55.000000 THISDLChatBot-2.0.3/THISDLChatBot.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-14 10:01:55.266354 THISDLChatBot-2.0.3/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      388 2024-04-14 10:01:42.000000 THISDLChatBot-2.0.3/setup.py
```

### Comparing `THISDLChatBot-2.0.2/LICENSE` & `THISDLChatBot-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.2/README.md` & `THISDLChatBot-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.2/THISDLChatBot/Bot.py` & `THISDLChatBot-2.0.3/THISDLChatBot/Bot.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.2/THISDLChatBot/Config.py` & `THISDLChatBot-2.0.3/THISDLChatBot/Config.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.2/THISDLChatBot/Friend.py` & `THISDLChatBot-2.0.3/THISDLChatBot/Friend.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.2/THISDLChatBot/Group.py` & `THISDLChatBot-2.0.3/THISDLChatBot/Group.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.2/THISDLChatBot/Logger.py` & `THISDLChatBot-2.0.3/THISDLChatBot/Logger.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.2/THISDLChatBot/Message.py` & `THISDLChatBot-2.0.3/THISDLChatBot/Message.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.2/THISDLChatBot/Plugin.py` & `THISDLChatBot-2.0.3/THISDLChatBot/Plugin.py`

 * *Files identical despite different names*

