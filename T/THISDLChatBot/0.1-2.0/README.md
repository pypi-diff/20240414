# Comparing `tmp/THISDLChatBot-0.1.tar.gz` & `tmp/THISDLChatBot-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "THISDLChatBot-0.1.tar", last modified: Sun Apr 14 03:17:22 2024, max compression
+gzip compressed data, was "THISDLChatBot-2.0.tar", last modified: Sun Apr 14 03:58:40 2024, max compression
```

## Comparing `THISDLChatBot-0.1.tar` & `THISDLChatBot-2.0.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 03:17:22.000225 THISDLChatBot-0.1/
--rwxrwxrwx   0 root         (0) root         (0)      347 2024-04-14 03:17:21.999916 THISDLChatBot-0.1/PKG-INFO
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 03:17:21.998211 THISDLChatBot-0.1/THISDLChatBot/
--rwxrwxrwx   0 root         (0) root         (0)    30319 2024-04-14 03:16:42.000000 THISDLChatBot-0.1/THISDLChatBot/Bot.py
--rwxrwxrwx   0 root         (0) root         (0)      467 2024-04-14 03:16:42.000000 THISDLChatBot-0.1/THISDLChatBot/CommandProcessor.py
--rwxrwxrwx   0 root         (0) root         (0)     5050 2024-04-13 10:15:50.000000 THISDLChatBot-0.1/THISDLChatBot/Config.py
--rwxrwxrwx   0 root         (0) root         (0)      103 2024-04-13 07:23:27.000000 THISDLChatBot-0.1/THISDLChatBot/Exceptions.py
--rwxrwxrwx   0 root         (0) root         (0)      594 2024-04-13 12:57:36.000000 THISDLChatBot-0.1/THISDLChatBot/Friend.py
--rwxrwxrwx   0 root         (0) root         (0)      914 2024-04-13 13:35:37.000000 THISDLChatBot-0.1/THISDLChatBot/Group.py
--rwxrwxrwx   0 root         (0) root         (0)     2818 2024-04-14 02:07:08.000000 THISDLChatBot-0.1/THISDLChatBot/Logger.py
--rwxrwxrwx   0 root         (0) root         (0)     2974 2024-04-14 03:02:10.000000 THISDLChatBot-0.1/THISDLChatBot/Message.py
--rwxrwxrwx   0 root         (0) root         (0)      391 2024-04-14 03:16:42.000000 THISDLChatBot-0.1/THISDLChatBot/MessageProcessor.py
--rwxrwxrwx   0 root         (0) root         (0)      856 2024-04-14 03:16:42.000000 THISDLChatBot-0.1/THISDLChatBot/Plugin.py
--rwxrwxrwx   0 root         (0) root         (0)      102 2024-04-13 14:16:44.000000 THISDLChatBot-0.1/THISDLChatBot/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 03:17:21.999647 THISDLChatBot-0.1/THISDLChatBot.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      347 2024-04-14 03:17:21.000000 THISDLChatBot-0.1/THISDLChatBot.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      479 2024-04-14 03:17:21.000000 THISDLChatBot-0.1/THISDLChatBot.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-14 03:17:21.000000 THISDLChatBot-0.1/THISDLChatBot.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       46 2024-04-14 03:17:21.000000 THISDLChatBot-0.1/THISDLChatBot.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       14 2024-04-14 03:17:21.000000 THISDLChatBot-0.1/THISDLChatBot.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-14 03:17:22.000269 THISDLChatBot-0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      398 2024-04-13 02:05:56.000000 THISDLChatBot-0.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 03:58:40.413402 THISDLChatBot-2.0/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2024-04-14 03:22:44.000000 THISDLChatBot-2.0/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      369 2024-04-14 03:58:40.413149 THISDLChatBot-2.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1131 2024-04-14 03:22:44.000000 THISDLChatBot-2.0/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 03:58:40.411916 THISDLChatBot-2.0/THISDLChatBot/
+-rwxrwxrwx   0 root         (0) root         (0)    30858 2024-04-14 03:54:16.000000 THISDLChatBot-2.0/THISDLChatBot/Bot.py
+-rwxrwxrwx   0 root         (0) root         (0)      467 2024-04-14 03:30:26.000000 THISDLChatBot-2.0/THISDLChatBot/CommandProcessor.py
+-rwxrwxrwx   0 root         (0) root         (0)     5050 2024-04-14 03:30:26.000000 THISDLChatBot-2.0/THISDLChatBot/Config.py
+-rwxrwxrwx   0 root         (0) root         (0)      103 2024-04-14 03:30:26.000000 THISDLChatBot-2.0/THISDLChatBot/Exceptions.py
+-rwxrwxrwx   0 root         (0) root         (0)      594 2024-04-14 03:30:26.000000 THISDLChatBot-2.0/THISDLChatBot/Friend.py
+-rwxrwxrwx   0 root         (0) root         (0)      914 2024-04-14 03:30:26.000000 THISDLChatBot-2.0/THISDLChatBot/Group.py
+-rwxrwxrwx   0 root         (0) root         (0)     2818 2024-04-14 03:30:26.000000 THISDLChatBot-2.0/THISDLChatBot/Logger.py
+-rwxrwxrwx   0 root         (0) root         (0)     2675 2024-04-14 03:40:28.000000 THISDLChatBot-2.0/THISDLChatBot/Message.py
+-rwxrwxrwx   0 root         (0) root         (0)      391 2024-04-14 03:30:26.000000 THISDLChatBot-2.0/THISDLChatBot/MessageProcessor.py
+-rwxrwxrwx   0 root         (0) root         (0)      856 2024-04-14 03:30:26.000000 THISDLChatBot-2.0/THISDLChatBot/Plugin.py
+-rwxrwxrwx   0 root         (0) root         (0)      102 2024-04-14 03:30:26.000000 THISDLChatBot-2.0/THISDLChatBot/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 03:58:40.412811 THISDLChatBot-2.0/THISDLChatBot.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      369 2024-04-14 03:58:40.000000 THISDLChatBot-2.0/THISDLChatBot.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      497 2024-04-14 03:58:40.000000 THISDLChatBot-2.0/THISDLChatBot.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-14 03:58:40.000000 THISDLChatBot-2.0/THISDLChatBot.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       46 2024-04-14 03:58:40.000000 THISDLChatBot-2.0/THISDLChatBot.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       14 2024-04-14 03:58:40.000000 THISDLChatBot-2.0/THISDLChatBot.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-14 03:58:40.413456 THISDLChatBot-2.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      398 2024-04-14 03:58:33.000000 THISDLChatBot-2.0/setup.py
```

### Comparing `THISDLChatBot-0.1/THISDLChatBot/Bot.py` & `THISDLChatBot-2.0/THISDLChatBot/Bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,27 +16,27 @@
 
 
 class Bot:
 
     def __init__(self, config: Config, logger: Logger) -> None:
         self.logger = logger
         self.config = config
-        self._loop = asyncio.get_event_loop()
+        self.loop = asyncio.get_event_loop()
         self.packageId = 1
         self.plugins = []
 
     async def _start(self):
         while True:
             messages = await self._GetMessages()
             for RawMessage in messages:
                 message = Message(RawMessage, self)
                 await self._UpdatePointer(message)
                 if message.IsCommand():
                     await self._CommandProcessor(message)
-
+                await self._MessageProcessor(message)
             await asyncio.sleep(self.config['wait_time'] / 1000)
 
     async def _CommandProcessor(self, message: Message):
         for plugin in self.plugins:
             for commandProcessor in plugin.CommandProcessors:
                 if (message.GetData() + ' ').startswith(f'/{commandProcessor.command} '):
                     await commandProcessor.Process((message.GetData() + ' ').split(' ')[1:], message, self)
@@ -106,15 +106,24 @@
                                                        "_6": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) "
                                                              "AppleWebKit/537.36 (KHTML, like Gecko) Chrome/115.0.0.0 "
                                                              "Safari/537.36"
                                                    },
                                                    "packageId": self.packageId
                                                })
         self.packageId += 1
-        return response.json()['body']['list'][:-1]
+        try:
+            return response.json()['body']['list'][:-1]
+        except KeyError:
+            self.logger.error('消息结构错误')
+            if self.config['auto_login']:
+                self.logger.error('重新登录...')
+                await self._login()
+                return await self._GetMessages()
+            else:
+                pass
 
     async def _UpLoadFile(self, File: _io.BufferedReader, FileType: int, FileName: str) -> str:
         JsonData = {
             'fileType': str(FileType),
             'isMessageAttachment': 'true'
         }
         file = {
@@ -176,14 +185,18 @@
             json=LoginData)
         try:
             self.userid = response.json()['body']['profile']['public']['userId']
             self.token = response.cookies['zaly_site_user']
         except KeyError:
             raise LoginFailedException(response.json())
 
+    async def DownLoadFile(self, Url: str) -> bytes:
+        cookies = {'zaly_site_user': self.token}
+        return (await self._httpclient.get(Url, cookies=cookies)).content
+
     async def GetFriends(self) -> list[Any] | list[Coroutine[Any, Any, Friend]]:
         response = await self._httpclient.post(
             'http://chat.thisit.cc/index.php?action=api.friend.list&body_format=json&lang=1', json={
                 "action": "api.friend.list",
                 "body": {
                     "@type": "type.googleapis.com/site.ApiFriendListRequest",
                     "offset": 0,
@@ -584,15 +597,15 @@
                 "packageId": self.packageId
             })
         self.packageId += 1
         return response.json()['header']['_1'] == 'success'
 
     def start(self):
         self.logger.info('机器人启动...')
-        self._loop.run_until_complete(self._login())
+        self.loop.run_until_complete(self._login())
         self.logger.success('登录成功!')
-        self._loop.run_until_complete(self._start())
+        self.loop.run_until_complete(self._start())
 
     def LoadPlugin(self, plugin: Plugin):
         plugin.bot = self
         self.plugins.append(plugin)
-        self._loop.run_until_complete(plugin.OnLoad())
+        self.loop.run_until_complete(plugin.OnLoad())
```

### Comparing `THISDLChatBot-0.1/THISDLChatBot/Config.py` & `THISDLChatBot-2.0/THISDLChatBot/Config.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-0.1/THISDLChatBot/Friend.py` & `THISDLChatBot-2.0/THISDLChatBot/Friend.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-0.1/THISDLChatBot/Group.py` & `THISDLChatBot-2.0/THISDLChatBot/Group.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-0.1/THISDLChatBot/Logger.py` & `THISDLChatBot-2.0/THISDLChatBot/Logger.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-0.1/THISDLChatBot/Message.py` & `THISDLChatBot-2.0/THISDLChatBot/Message.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-from .Friend import Friend
-from .Group import Group
-import asyncio
-
-
 class Message:
     def __init__(self, RawMessage: dict, bot) -> None:
         self._RawMessage = RawMessage
         self.bot = bot
 
     def __str__(self) -> str:
         return str(self._RawMessage)
@@ -38,31 +33,28 @@
             return self.bot.config['auto_accept']
         if self.GetType() == 'MessageNotice':
             return self._RawMessage['notice']['body']
         if self.GetType() == 'MessageWeb':
             if self._RawMessage['web']['title'] == 'GIF':
                 ImageUrl = ('http://chat.thisit.cc/'
                             + self._RawMessage['web']['code'].split('<img src=\"')[1].split('\"')[0])
-                cookies = {'zaly_site_user': self.bot.token}
-                return asyncio.run(self.bot._httpclient.get(ImageUrl, cookies=cookies)).content
+                return self.bot.loop.run_until_complete(self.bot.DownLoadFile(ImageUrl))
             return self._RawMessage['web']['code']
         if self.GetType() == 'MessageDocument':
             FileUrl = (f"http://chat.thisit.cc/index.php?action=http.file.downloadFile&fileId="
                        + self._RawMessage['document']['url']
                        + "&returnBase64=0&isGroupMessage=0&messageId="
                        + self._RawMessage['msgId']
                        + "&lang=1")
-            cookies = {'zaly_site_user': self.bot.token}
-            return asyncio.run(self.bot._httpclient.get(FileUrl, cookies=cookies)).content
+            return self.bot.DownLoadFile(FileUrl)
         if self.GetType() == 'MessageImage':
             ImageUrl = ("http://chat.thisit.cc/index.php?action=http.file.downloadFile&fileId="
                         + self._RawMessage['image']['url']
                         + "&returnBase64=0&lang=1")
-            cookies = {'zaly_site_user': self.bot.token}
-            return asyncio.run(self.bot._httpclient.get(ImageUrl, cookies=cookies)).content
+            return self.bot.loop.run_until_complete(self.bot.DownLoadFile(ImageUrl))
         if self.GetType() == 'MessageRecall':
             result = {'msgId': self._RawMessage['recall']['msgId']}
             if self.GetRoomType() == 'Group':
                 result['Group'] = self.GetFromGroup()
             else:
                 result['Friend'] = self.GetFromUser()
             return result
```

### Comparing `THISDLChatBot-0.1/THISDLChatBot/Plugin.py` & `THISDLChatBot-2.0/THISDLChatBot/Plugin.py`

 * *Files identical despite different names*

