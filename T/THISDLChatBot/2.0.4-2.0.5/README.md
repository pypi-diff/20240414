# Comparing `tmp/THISDLChatBot-2.0.4.tar.gz` & `tmp/THISDLChatBot-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "THISDLChatBot-2.0.4.tar", last modified: Sun Apr 14 10:06:15 2024, max compression
+gzip compressed data, was "THISDLChatBot-2.0.5.tar", last modified: Sun Apr 14 10:08:01 2024, max compression
```

## Comparing `THISDLChatBot-2.0.4.tar` & `THISDLChatBot-2.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 10:06:15.160949 THISDLChatBot-2.0.4/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2024-04-14 03:22:44.000000 THISDLChatBot-2.0.4/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      347 2024-04-14 10:06:15.160552 THISDLChatBot-2.0.4/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1220 2024-04-14 09:11:13.000000 THISDLChatBot-2.0.4/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 10:06:15.158908 THISDLChatBot-2.0.4/THISDLChatBot/
--rwxrwxrwx   0 root         (0) root         (0)    31089 2024-04-14 10:05:50.000000 THISDLChatBot-2.0.4/THISDLChatBot/Bot.py
--rwxrwxrwx   0 root         (0) root         (0)      462 2024-04-14 09:53:31.000000 THISDLChatBot-2.0.4/THISDLChatBot/CommandProcessor.py
--rwxrwxrwx   0 root         (0) root         (0)     5050 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.4/THISDLChatBot/Config.py
--rwxrwxrwx   0 root         (0) root         (0)      103 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.4/THISDLChatBot/Exceptions.py
--rwxrwxrwx   0 root         (0) root         (0)      594 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.4/THISDLChatBot/Friend.py
--rwxrwxrwx   0 root         (0) root         (0)      914 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.4/THISDLChatBot/Group.py
--rwxrwxrwx   0 root         (0) root         (0)     2818 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.4/THISDLChatBot/Logger.py
--rwxrwxrwx   0 root         (0) root         (0)     2658 2024-04-14 07:43:55.000000 THISDLChatBot-2.0.4/THISDLChatBot/Message.py
--rwxrwxrwx   0 root         (0) root         (0)      391 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.4/THISDLChatBot/MessageProcessor.py
--rwxrwxrwx   0 root         (0) root         (0)      856 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.4/THISDLChatBot/Plugin.py
--rwxrwxrwx   0 root         (0) root         (0)      102 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.4/THISDLChatBot/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 10:06:15.160060 THISDLChatBot-2.0.4/THISDLChatBot.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      347 2024-04-14 10:06:15.000000 THISDLChatBot-2.0.4/THISDLChatBot.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      497 2024-04-14 10:06:15.000000 THISDLChatBot-2.0.4/THISDLChatBot.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-14 10:06:15.000000 THISDLChatBot-2.0.4/THISDLChatBot.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       37 2024-04-14 10:06:15.000000 THISDLChatBot-2.0.4/THISDLChatBot.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       14 2024-04-14 10:06:15.000000 THISDLChatBot-2.0.4/THISDLChatBot.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-14 10:06:15.161012 THISDLChatBot-2.0.4/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      388 2024-04-14 10:06:07.000000 THISDLChatBot-2.0.4/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 10:08:01.326343 THISDLChatBot-2.0.5/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2024-04-14 03:22:44.000000 THISDLChatBot-2.0.5/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      347 2024-04-14 10:08:01.326023 THISDLChatBot-2.0.5/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1220 2024-04-14 09:11:13.000000 THISDLChatBot-2.0.5/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 10:08:01.324571 THISDLChatBot-2.0.5/THISDLChatBot/
+-rwxrwxrwx   0 root         (0) root         (0)    31074 2024-04-14 10:07:44.000000 THISDLChatBot-2.0.5/THISDLChatBot/Bot.py
+-rwxrwxrwx   0 root         (0) root         (0)      462 2024-04-14 09:53:31.000000 THISDLChatBot-2.0.5/THISDLChatBot/CommandProcessor.py
+-rwxrwxrwx   0 root         (0) root         (0)     5050 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.5/THISDLChatBot/Config.py
+-rwxrwxrwx   0 root         (0) root         (0)      103 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.5/THISDLChatBot/Exceptions.py
+-rwxrwxrwx   0 root         (0) root         (0)      594 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.5/THISDLChatBot/Friend.py
+-rwxrwxrwx   0 root         (0) root         (0)      914 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.5/THISDLChatBot/Group.py
+-rwxrwxrwx   0 root         (0) root         (0)     2818 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.5/THISDLChatBot/Logger.py
+-rwxrwxrwx   0 root         (0) root         (0)     2658 2024-04-14 07:43:55.000000 THISDLChatBot-2.0.5/THISDLChatBot/Message.py
+-rwxrwxrwx   0 root         (0) root         (0)      391 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.5/THISDLChatBot/MessageProcessor.py
+-rwxrwxrwx   0 root         (0) root         (0)      856 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.5/THISDLChatBot/Plugin.py
+-rwxrwxrwx   0 root         (0) root         (0)      102 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.5/THISDLChatBot/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 10:08:01.325586 THISDLChatBot-2.0.5/THISDLChatBot.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      347 2024-04-14 10:08:01.000000 THISDLChatBot-2.0.5/THISDLChatBot.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      497 2024-04-14 10:08:01.000000 THISDLChatBot-2.0.5/THISDLChatBot.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-14 10:08:01.000000 THISDLChatBot-2.0.5/THISDLChatBot.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       37 2024-04-14 10:08:01.000000 THISDLChatBot-2.0.5/THISDLChatBot.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       14 2024-04-14 10:08:01.000000 THISDLChatBot-2.0.5/THISDLChatBot.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-14 10:08:01.326403 THISDLChatBot-2.0.5/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      388 2024-04-14 10:07:44.000000 THISDLChatBot-2.0.5/setup.py
```

### Comparing `THISDLChatBot-2.0.4/LICENSE` & `THISDLChatBot-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.4/README.md` & `THISDLChatBot-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.4/THISDLChatBot/Bot.py` & `THISDLChatBot-2.0.5/THISDLChatBot/Bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
             for friend in response.json()['body']['friends']:
                 if friend['profile']['userId'] != self.userid:
                     friends.append(self.GetFriendProfile(friend['profile']['userId']))
         except KeyError:
             return []
         return friends
 
-    async def GetGroups(self) -> list[Group]:
+    async def GetGroups(self):
         response = await self._httpclient.post(
             'http://chat.thisit.cc/index.php?action=api.group.list&body_format=json&lang=1', json={
                 "action": "api.group.list",
                 "body": {
                     "@type": "type.googleapis.com/site.ApiGroupListRequest",
                     "offset": 0,
                     "count": 200
```

### Comparing `THISDLChatBot-2.0.4/THISDLChatBot/Config.py` & `THISDLChatBot-2.0.5/THISDLChatBot/Config.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.4/THISDLChatBot/Friend.py` & `THISDLChatBot-2.0.5/THISDLChatBot/Friend.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.4/THISDLChatBot/Group.py` & `THISDLChatBot-2.0.5/THISDLChatBot/Group.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.4/THISDLChatBot/Logger.py` & `THISDLChatBot-2.0.5/THISDLChatBot/Logger.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.4/THISDLChatBot/Message.py` & `THISDLChatBot-2.0.5/THISDLChatBot/Message.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.4/THISDLChatBot/Plugin.py` & `THISDLChatBot-2.0.5/THISDLChatBot/Plugin.py`

 * *Files identical despite different names*

