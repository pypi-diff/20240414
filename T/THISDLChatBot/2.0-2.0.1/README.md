# Comparing `tmp/THISDLChatBot-2.0.tar.gz` & `tmp/THISDLChatBot-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "THISDLChatBot-2.0.tar", last modified: Sun Apr 14 03:58:40 2024, max compression
+gzip compressed data, was "THISDLChatBot-2.0.1.tar", last modified: Sun Apr 14 07:45:01 2024, max compression
```

## Comparing `THISDLChatBot-2.0.tar` & `THISDLChatBot-2.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 03:58:40.413402 THISDLChatBot-2.0/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2024-04-14 03:22:44.000000 THISDLChatBot-2.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      369 2024-04-14 03:58:40.413149 THISDLChatBot-2.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1131 2024-04-14 03:22:44.000000 THISDLChatBot-2.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 03:58:40.411916 THISDLChatBot-2.0/THISDLChatBot/
--rwxrwxrwx   0 root         (0) root         (0)    30858 2024-04-14 03:54:16.000000 THISDLChatBot-2.0/THISDLChatBot/Bot.py
--rwxrwxrwx   0 root         (0) root         (0)      467 2024-04-14 03:30:26.000000 THISDLChatBot-2.0/THISDLChatBot/CommandProcessor.py
--rwxrwxrwx   0 root         (0) root         (0)     5050 2024-04-14 03:30:26.000000 THISDLChatBot-2.0/THISDLChatBot/Config.py
--rwxrwxrwx   0 root         (0) root         (0)      103 2024-04-14 03:30:26.000000 THISDLChatBot-2.0/THISDLChatBot/Exceptions.py
--rwxrwxrwx   0 root         (0) root         (0)      594 2024-04-14 03:30:26.000000 THISDLChatBot-2.0/THISDLChatBot/Friend.py
--rwxrwxrwx   0 root         (0) root         (0)      914 2024-04-14 03:30:26.000000 THISDLChatBot-2.0/THISDLChatBot/Group.py
--rwxrwxrwx   0 root         (0) root         (0)     2818 2024-04-14 03:30:26.000000 THISDLChatBot-2.0/THISDLChatBot/Logger.py
--rwxrwxrwx   0 root         (0) root         (0)     2675 2024-04-14 03:40:28.000000 THISDLChatBot-2.0/THISDLChatBot/Message.py
--rwxrwxrwx   0 root         (0) root         (0)      391 2024-04-14 03:30:26.000000 THISDLChatBot-2.0/THISDLChatBot/MessageProcessor.py
--rwxrwxrwx   0 root         (0) root         (0)      856 2024-04-14 03:30:26.000000 THISDLChatBot-2.0/THISDLChatBot/Plugin.py
--rwxrwxrwx   0 root         (0) root         (0)      102 2024-04-14 03:30:26.000000 THISDLChatBot-2.0/THISDLChatBot/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 03:58:40.412811 THISDLChatBot-2.0/THISDLChatBot.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      369 2024-04-14 03:58:40.000000 THISDLChatBot-2.0/THISDLChatBot.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      497 2024-04-14 03:58:40.000000 THISDLChatBot-2.0/THISDLChatBot.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-14 03:58:40.000000 THISDLChatBot-2.0/THISDLChatBot.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       46 2024-04-14 03:58:40.000000 THISDLChatBot-2.0/THISDLChatBot.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       14 2024-04-14 03:58:40.000000 THISDLChatBot-2.0/THISDLChatBot.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-14 03:58:40.413456 THISDLChatBot-2.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      398 2024-04-14 03:58:33.000000 THISDLChatBot-2.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 07:45:01.748430 THISDLChatBot-2.0.1/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2024-04-14 03:22:44.000000 THISDLChatBot-2.0.1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      371 2024-04-14 07:45:01.748215 THISDLChatBot-2.0.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1131 2024-04-14 03:22:44.000000 THISDLChatBot-2.0.1/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 07:45:01.746924 THISDLChatBot-2.0.1/THISDLChatBot/
+-rwxrwxrwx   0 root         (0) root         (0)    30959 2024-04-14 07:42:35.000000 THISDLChatBot-2.0.1/THISDLChatBot/Bot.py
+-rwxrwxrwx   0 root         (0) root         (0)      467 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.1/THISDLChatBot/CommandProcessor.py
+-rwxrwxrwx   0 root         (0) root         (0)     5050 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.1/THISDLChatBot/Config.py
+-rwxrwxrwx   0 root         (0) root         (0)      103 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.1/THISDLChatBot/Exceptions.py
+-rwxrwxrwx   0 root         (0) root         (0)      594 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.1/THISDLChatBot/Friend.py
+-rwxrwxrwx   0 root         (0) root         (0)      914 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.1/THISDLChatBot/Group.py
+-rwxrwxrwx   0 root         (0) root         (0)     2818 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.1/THISDLChatBot/Logger.py
+-rwxrwxrwx   0 root         (0) root         (0)     2658 2024-04-14 07:43:55.000000 THISDLChatBot-2.0.1/THISDLChatBot/Message.py
+-rwxrwxrwx   0 root         (0) root         (0)      391 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.1/THISDLChatBot/MessageProcessor.py
+-rwxrwxrwx   0 root         (0) root         (0)      856 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.1/THISDLChatBot/Plugin.py
+-rwxrwxrwx   0 root         (0) root         (0)      102 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.1/THISDLChatBot/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 07:45:01.747969 THISDLChatBot-2.0.1/THISDLChatBot.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      371 2024-04-14 07:45:01.000000 THISDLChatBot-2.0.1/THISDLChatBot.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      497 2024-04-14 07:45:01.000000 THISDLChatBot-2.0.1/THISDLChatBot.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-14 07:45:01.000000 THISDLChatBot-2.0.1/THISDLChatBot.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       46 2024-04-14 07:45:01.000000 THISDLChatBot-2.0.1/THISDLChatBot.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       14 2024-04-14 07:45:01.000000 THISDLChatBot-2.0.1/THISDLChatBot.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-14 07:45:01.748473 THISDLChatBot-2.0.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      400 2024-04-14 07:44:44.000000 THISDLChatBot-2.0.1/setup.py
```

### Comparing `THISDLChatBot-2.0/LICENSE` & `THISDLChatBot-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0/README.md` & `THISDLChatBot-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0/THISDLChatBot/Bot.py` & `THISDLChatBot-2.0.1/THISDLChatBot/Bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 
     async def _start(self):
         while True:
             messages = await self._GetMessages()
             for RawMessage in messages:
                 message = Message(RawMessage, self)
                 await self._UpdatePointer(message)
+                if (await message.GetFromUser()).GetUserId() == self.userid:
+                    continue
                 if message.IsCommand():
                     await self._CommandProcessor(message)
                 await self._MessageProcessor(message)
             await asyncio.sleep(self.config['wait_time'] / 1000)
 
     async def _CommandProcessor(self, message: Message):
         for plugin in self.plugins:
@@ -119,22 +121,22 @@
                 await self._login()
                 return await self._GetMessages()
             else:
                 pass
 
     async def _UpLoadFile(self, File: _io.BufferedReader, FileType: int, FileName: str) -> str:
         JsonData = {
-            'fileType': str(FileType),
+            'fileType': FileType,
             'isMessageAttachment': 'true'
         }
         file = {
             'file': (FileName, File, 'application/octet-stream')
         }
         response = await self._httpclient.post('http://chat.thisit.cc/index.php?action=http.file.uploadWeb', files=file,
-                                               json=JsonData, cookies={'zaly_site_user': self.token})
+                                               data=JsonData, cookies={'zaly_site_user': self.token})
         if response.json()['errorInfo'] != '':
             raise UpLoadFileFailedException(response.json()['errorInfo'])
         return response.json()['fileId']
 
     async def _GetPreSessionId(self) -> str:
         LoginData = {
             "action": "api.passport.passwordLogin",
```

### Comparing `THISDLChatBot-2.0/THISDLChatBot/Config.py` & `THISDLChatBot-2.0.1/THISDLChatBot/Config.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0/THISDLChatBot/Friend.py` & `THISDLChatBot-2.0.1/THISDLChatBot/Friend.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0/THISDLChatBot/Group.py` & `THISDLChatBot-2.0.1/THISDLChatBot/Group.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0/THISDLChatBot/Logger.py` & `THISDLChatBot-2.0.1/THISDLChatBot/Logger.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0/THISDLChatBot/Message.py` & `THISDLChatBot-2.0.1/THISDLChatBot/Message.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 class Message:
     def __init__(self, RawMessage: dict, bot) -> None:
-        self._RawMessage = RawMessage
+        self.RawMessage = RawMessage
         self.bot = bot
 
     def __str__(self) -> str:
-        return str(self._RawMessage)
+        return str(self.RawMessage)
 
     def GetMessageId(self):
-        return self._RawMessage.get('msgId')
+        return self.RawMessage.get('msgId')
 
     def GetType(self):
-        return self._RawMessage['type']
+        return self.RawMessage['type']
 
     def GetRoomType(self):
-        if self._RawMessage['msgId'].startswith('G'):
+        if self.RawMessage['msgId'].startswith('G'):
             return 'Group'
         return 'Private'
 
     async def GetFromUser(self):
-        return await self.bot.GetFriendProfile(self._RawMessage.get('fromUserId'))
+        return await self.bot.GetFriendProfile(self.RawMessage.get('fromUserId'))
 
     def GetPointer(self) -> str:
-        return self._RawMessage['pointer']
+        return self.RawMessage['pointer']
 
     async def GetFromGroup(self):
-        return await self.bot.GetGroupProfile(self._RawMessage.get('toGroupId'))
+        return await self.bot.GetGroupProfile(self.RawMessage.get('toGroupId'))
 
     def GetData(self):
         if self.GetType() == 'MessageText':
-            return self._RawMessage['text']['body']
+            return self.RawMessage['text']['body']
         if self.GetType() == 'MessageEventFriendRequest':
             return self.bot.config['auto_accept']
         if self.GetType() == 'MessageNotice':
-            return self._RawMessage['notice']['body']
+            return self.RawMessage['notice']['body']
         if self.GetType() == 'MessageWeb':
-            if self._RawMessage['web']['title'] == 'GIF':
+            if self.RawMessage['web']['title'] == 'GIF':
                 ImageUrl = ('http://chat.thisit.cc/'
-                            + self._RawMessage['web']['code'].split('<img src=\"')[1].split('\"')[0])
+                            + self.RawMessage['web']['code'].split('<img src=\"')[1].split('\"')[0])
                 return self.bot.loop.run_until_complete(self.bot.DownLoadFile(ImageUrl))
-            return self._RawMessage['web']['code']
+            return self.RawMessage['web']['code']
         if self.GetType() == 'MessageDocument':
             FileUrl = (f"http://chat.thisit.cc/index.php?action=http.file.downloadFile&fileId="
-                       + self._RawMessage['document']['url']
+                       + self.RawMessage['document']['url']
                        + "&returnBase64=0&isGroupMessage=0&messageId="
-                       + self._RawMessage['msgId']
+                       + self.RawMessage['msgId']
                        + "&lang=1")
             return self.bot.DownLoadFile(FileUrl)
         if self.GetType() == 'MessageImage':
             ImageUrl = ("http://chat.thisit.cc/index.php?action=http.file.downloadFile&fileId="
-                        + self._RawMessage['image']['url']
+                        + self.RawMessage['image']['url']
                         + "&returnBase64=0&lang=1")
             return self.bot.loop.run_until_complete(self.bot.DownLoadFile(ImageUrl))
         if self.GetType() == 'MessageRecall':
-            result = {'msgId': self._RawMessage['recall']['msgId']}
+            result = {'msgId': self.RawMessage['recall']['msgId']}
             if self.GetRoomType() == 'Group':
                 result['Group'] = self.GetFromGroup()
             else:
                 result['Friend'] = self.GetFromUser()
             return result
 
     def IsCommand(self):
```

### Comparing `THISDLChatBot-2.0/THISDLChatBot/Plugin.py` & `THISDLChatBot-2.0.1/THISDLChatBot/Plugin.py`

 * *Files identical despite different names*

