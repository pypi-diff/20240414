# Comparing `tmp/THISDLChatBot-2.0.5.tar.gz` & `tmp/THISDLChatBot-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "THISDLChatBot-2.0.5.tar", last modified: Sun Apr 14 10:08:01 2024, max compression
+gzip compressed data, was "THISDLChatBot-2.0.6.tar", last modified: Sun Apr 14 11:09:32 2024, max compression
```

## Comparing `THISDLChatBot-2.0.5.tar` & `THISDLChatBot-2.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 10:08:01.326343 THISDLChatBot-2.0.5/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2024-04-14 03:22:44.000000 THISDLChatBot-2.0.5/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      347 2024-04-14 10:08:01.326023 THISDLChatBot-2.0.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1220 2024-04-14 09:11:13.000000 THISDLChatBot-2.0.5/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 10:08:01.324571 THISDLChatBot-2.0.5/THISDLChatBot/
--rwxrwxrwx   0 root         (0) root         (0)    31074 2024-04-14 10:07:44.000000 THISDLChatBot-2.0.5/THISDLChatBot/Bot.py
--rwxrwxrwx   0 root         (0) root         (0)      462 2024-04-14 09:53:31.000000 THISDLChatBot-2.0.5/THISDLChatBot/CommandProcessor.py
--rwxrwxrwx   0 root         (0) root         (0)     5050 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.5/THISDLChatBot/Config.py
--rwxrwxrwx   0 root         (0) root         (0)      103 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.5/THISDLChatBot/Exceptions.py
--rwxrwxrwx   0 root         (0) root         (0)      594 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.5/THISDLChatBot/Friend.py
--rwxrwxrwx   0 root         (0) root         (0)      914 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.5/THISDLChatBot/Group.py
--rwxrwxrwx   0 root         (0) root         (0)     2818 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.5/THISDLChatBot/Logger.py
--rwxrwxrwx   0 root         (0) root         (0)     2658 2024-04-14 07:43:55.000000 THISDLChatBot-2.0.5/THISDLChatBot/Message.py
--rwxrwxrwx   0 root         (0) root         (0)      391 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.5/THISDLChatBot/MessageProcessor.py
--rwxrwxrwx   0 root         (0) root         (0)      856 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.5/THISDLChatBot/Plugin.py
--rwxrwxrwx   0 root         (0) root         (0)      102 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.5/THISDLChatBot/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 10:08:01.325586 THISDLChatBot-2.0.5/THISDLChatBot.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      347 2024-04-14 10:08:01.000000 THISDLChatBot-2.0.5/THISDLChatBot.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      497 2024-04-14 10:08:01.000000 THISDLChatBot-2.0.5/THISDLChatBot.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-14 10:08:01.000000 THISDLChatBot-2.0.5/THISDLChatBot.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       37 2024-04-14 10:08:01.000000 THISDLChatBot-2.0.5/THISDLChatBot.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       14 2024-04-14 10:08:01.000000 THISDLChatBot-2.0.5/THISDLChatBot.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-14 10:08:01.326403 THISDLChatBot-2.0.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      388 2024-04-14 10:07:44.000000 THISDLChatBot-2.0.5/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 11:09:32.254541 THISDLChatBot-2.0.6/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2024-04-14 03:22:44.000000 THISDLChatBot-2.0.6/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      347 2024-04-14 11:09:32.254319 THISDLChatBot-2.0.6/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1220 2024-04-14 09:11:13.000000 THISDLChatBot-2.0.6/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 11:09:32.252796 THISDLChatBot-2.0.6/THISDLChatBot/
+-rwxrwxrwx   0 root         (0) root         (0)    31074 2024-04-14 10:07:44.000000 THISDLChatBot-2.0.6/THISDLChatBot/Bot.py
+-rwxrwxrwx   0 root         (0) root         (0)      462 2024-04-14 09:53:31.000000 THISDLChatBot-2.0.6/THISDLChatBot/CommandProcessor.py
+-rwxrwxrwx   0 root         (0) root         (0)     5050 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.6/THISDLChatBot/Config.py
+-rwxrwxrwx   0 root         (0) root         (0)      103 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.6/THISDLChatBot/Exceptions.py
+-rwxrwxrwx   0 root         (0) root         (0)      594 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.6/THISDLChatBot/Friend.py
+-rwxrwxrwx   0 root         (0) root         (0)      914 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.6/THISDLChatBot/Group.py
+-rwxrwxrwx   0 root         (0) root         (0)     2818 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.6/THISDLChatBot/Logger.py
+-rwxrwxrwx   0 root         (0) root         (0)     2702 2024-04-14 11:09:26.000000 THISDLChatBot-2.0.6/THISDLChatBot/Message.py
+-rwxrwxrwx   0 root         (0) root         (0)      391 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.6/THISDLChatBot/MessageProcessor.py
+-rwxrwxrwx   0 root         (0) root         (0)      856 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.6/THISDLChatBot/Plugin.py
+-rwxrwxrwx   0 root         (0) root         (0)      102 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.6/THISDLChatBot/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 11:09:32.253981 THISDLChatBot-2.0.6/THISDLChatBot.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      347 2024-04-14 11:09:32.000000 THISDLChatBot-2.0.6/THISDLChatBot.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      497 2024-04-14 11:09:32.000000 THISDLChatBot-2.0.6/THISDLChatBot.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-14 11:09:32.000000 THISDLChatBot-2.0.6/THISDLChatBot.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       37 2024-04-14 11:09:32.000000 THISDLChatBot-2.0.6/THISDLChatBot.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       14 2024-04-14 11:09:32.000000 THISDLChatBot-2.0.6/THISDLChatBot.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-14 11:09:32.254590 THISDLChatBot-2.0.6/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      388 2024-04-14 11:09:26.000000 THISDLChatBot-2.0.6/setup.py
```

### Comparing `THISDLChatBot-2.0.5/LICENSE` & `THISDLChatBot-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.5/README.md` & `THISDLChatBot-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.5/THISDLChatBot/Bot.py` & `THISDLChatBot-2.0.6/THISDLChatBot/Bot.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.5/THISDLChatBot/Config.py` & `THISDLChatBot-2.0.6/THISDLChatBot/Config.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.5/THISDLChatBot/Friend.py` & `THISDLChatBot-2.0.6/THISDLChatBot/Friend.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.5/THISDLChatBot/Group.py` & `THISDLChatBot-2.0.6/THISDLChatBot/Group.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.5/THISDLChatBot/Logger.py` & `THISDLChatBot-2.0.6/THISDLChatBot/Logger.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.5/THISDLChatBot/Message.py` & `THISDLChatBot-2.0.6/THISDLChatBot/Message.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,22 +13,22 @@
         return self.RawMessage['type']
 
     def GetRoomType(self):
         if self.RawMessage['msgId'].startswith('G'):
             return 'Group'
         return 'Private'
 
-    async def GetFromUser(self):
-        return await self.bot.GetFriendProfile(self.RawMessage.get('fromUserId'))
+    def GetFromUser(self):
+        return self.bot.loop.run_until_complete(self.bot.GetFriendProfile(self.RawMessage.get('fromUserId')))
 
     def GetPointer(self) -> str:
         return self.RawMessage['pointer']
 
-    async def GetFromGroup(self):
-        return await self.bot.GetGroupProfile(self.RawMessage.get('toGroupId'))
+    def GetFromGroup(self):
+        return self.bot.loop.run_until_complete(self.bot.GetGroupProfile(self.RawMessage.get('toGroupId')))
 
     def GetData(self):
         if self.GetType() == 'MessageText':
             return self.RawMessage['text']['body']
         if self.GetType() == 'MessageEventFriendRequest':
             return self.bot.config['auto_accept']
         if self.GetType() == 'MessageNotice':
```

### Comparing `THISDLChatBot-2.0.5/THISDLChatBot/Plugin.py` & `THISDLChatBot-2.0.6/THISDLChatBot/Plugin.py`

 * *Files identical despite different names*

