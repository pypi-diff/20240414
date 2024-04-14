# Comparing `tmp/THISDLChatBot-2.0.1.tar.gz` & `tmp/THISDLChatBot-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "THISDLChatBot-2.0.1.tar", last modified: Sun Apr 14 07:45:01 2024, max compression
+gzip compressed data, was "THISDLChatBot-2.0.2.tar", last modified: Sun Apr 14 09:50:52 2024, max compression
```

## Comparing `THISDLChatBot-2.0.1.tar` & `THISDLChatBot-2.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 07:45:01.748430 THISDLChatBot-2.0.1/
--rwxrwxrwx   0 root         (0) root         (0)    35149 2024-04-14 03:22:44.000000 THISDLChatBot-2.0.1/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      371 2024-04-14 07:45:01.748215 THISDLChatBot-2.0.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1131 2024-04-14 03:22:44.000000 THISDLChatBot-2.0.1/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 07:45:01.746924 THISDLChatBot-2.0.1/THISDLChatBot/
--rwxrwxrwx   0 root         (0) root         (0)    30959 2024-04-14 07:42:35.000000 THISDLChatBot-2.0.1/THISDLChatBot/Bot.py
--rwxrwxrwx   0 root         (0) root         (0)      467 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.1/THISDLChatBot/CommandProcessor.py
--rwxrwxrwx   0 root         (0) root         (0)     5050 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.1/THISDLChatBot/Config.py
--rwxrwxrwx   0 root         (0) root         (0)      103 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.1/THISDLChatBot/Exceptions.py
--rwxrwxrwx   0 root         (0) root         (0)      594 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.1/THISDLChatBot/Friend.py
--rwxrwxrwx   0 root         (0) root         (0)      914 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.1/THISDLChatBot/Group.py
--rwxrwxrwx   0 root         (0) root         (0)     2818 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.1/THISDLChatBot/Logger.py
--rwxrwxrwx   0 root         (0) root         (0)     2658 2024-04-14 07:43:55.000000 THISDLChatBot-2.0.1/THISDLChatBot/Message.py
--rwxrwxrwx   0 root         (0) root         (0)      391 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.1/THISDLChatBot/MessageProcessor.py
--rwxrwxrwx   0 root         (0) root         (0)      856 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.1/THISDLChatBot/Plugin.py
--rwxrwxrwx   0 root         (0) root         (0)      102 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.1/THISDLChatBot/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 07:45:01.747969 THISDLChatBot-2.0.1/THISDLChatBot.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)      371 2024-04-14 07:45:01.000000 THISDLChatBot-2.0.1/THISDLChatBot.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      497 2024-04-14 07:45:01.000000 THISDLChatBot-2.0.1/THISDLChatBot.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-14 07:45:01.000000 THISDLChatBot-2.0.1/THISDLChatBot.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       46 2024-04-14 07:45:01.000000 THISDLChatBot-2.0.1/THISDLChatBot.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       14 2024-04-14 07:45:01.000000 THISDLChatBot-2.0.1/THISDLChatBot.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-14 07:45:01.748473 THISDLChatBot-2.0.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      400 2024-04-14 07:44:44.000000 THISDLChatBot-2.0.1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 09:50:52.926740 THISDLChatBot-2.0.2/
+-rwxrwxrwx   0 root         (0) root         (0)    35149 2024-04-14 03:22:44.000000 THISDLChatBot-2.0.2/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      347 2024-04-14 09:50:52.926510 THISDLChatBot-2.0.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1220 2024-04-14 09:11:13.000000 THISDLChatBot-2.0.2/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 09:50:52.925240 THISDLChatBot-2.0.2/THISDLChatBot/
+-rwxrwxrwx   0 root         (0) root         (0)    31138 2024-04-14 09:39:36.000000 THISDLChatBot-2.0.2/THISDLChatBot/Bot.py
+-rwxrwxrwx   0 root         (0) root         (0)      467 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.2/THISDLChatBot/CommandProcessor.py
+-rwxrwxrwx   0 root         (0) root         (0)     5050 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.2/THISDLChatBot/Config.py
+-rwxrwxrwx   0 root         (0) root         (0)      103 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.2/THISDLChatBot/Exceptions.py
+-rwxrwxrwx   0 root         (0) root         (0)      594 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.2/THISDLChatBot/Friend.py
+-rwxrwxrwx   0 root         (0) root         (0)      914 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.2/THISDLChatBot/Group.py
+-rwxrwxrwx   0 root         (0) root         (0)     2818 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.2/THISDLChatBot/Logger.py
+-rwxrwxrwx   0 root         (0) root         (0)     2658 2024-04-14 07:43:55.000000 THISDLChatBot-2.0.2/THISDLChatBot/Message.py
+-rwxrwxrwx   0 root         (0) root         (0)      391 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.2/THISDLChatBot/MessageProcessor.py
+-rwxrwxrwx   0 root         (0) root         (0)      856 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.2/THISDLChatBot/Plugin.py
+-rwxrwxrwx   0 root         (0) root         (0)      102 2024-04-14 03:30:26.000000 THISDLChatBot-2.0.2/THISDLChatBot/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-14 09:50:52.926203 THISDLChatBot-2.0.2/THISDLChatBot.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)      347 2024-04-14 09:50:52.000000 THISDLChatBot-2.0.2/THISDLChatBot.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      497 2024-04-14 09:50:52.000000 THISDLChatBot-2.0.2/THISDLChatBot.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-14 09:50:52.000000 THISDLChatBot-2.0.2/THISDLChatBot.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       37 2024-04-14 09:50:52.000000 THISDLChatBot-2.0.2/THISDLChatBot.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       14 2024-04-14 09:50:52.000000 THISDLChatBot-2.0.2/THISDLChatBot.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-14 09:50:52.926787 THISDLChatBot-2.0.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      388 2024-04-14 09:50:31.000000 THISDLChatBot-2.0.2/setup.py
```

### Comparing `THISDLChatBot-2.0.1/LICENSE` & `THISDLChatBot-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.1/THISDLChatBot/Bot.py` & `THISDLChatBot-2.0.2/THISDLChatBot/Bot.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,16 @@
             for RawMessage in messages:
                 message = Message(RawMessage, self)
                 await self._UpdatePointer(message)
                 if (await message.GetFromUser()).GetUserId() == self.userid:
                     continue
                 if message.IsCommand():
                     await self._CommandProcessor(message)
+                if message.GetType() == 'MessageEventFriendRequest' and self.config['auto_accept']:
+                    await self.Accept(True, (await message.GetFromUser()).GetUserId())
                 await self._MessageProcessor(message)
             await asyncio.sleep(self.config['wait_time'] / 1000)
 
     async def _CommandProcessor(self, message: Message):
         for plugin in self.plugins:
             for commandProcessor in plugin.CommandProcessors:
                 if (message.GetData() + ' ').startswith(f'/{commandProcessor.command} '):
@@ -120,23 +122,23 @@
                 self.logger.error('重新登录...')
                 await self._login()
                 return await self._GetMessages()
             else:
                 pass
 
     async def _UpLoadFile(self, File: _io.BufferedReader, FileType: int, FileName: str) -> str:
-        JsonData = {
+        Data = {
             'fileType': FileType,
             'isMessageAttachment': 'true'
         }
         file = {
             'file': (FileName, File, 'application/octet-stream')
         }
         response = await self._httpclient.post('http://chat.thisit.cc/index.php?action=http.file.uploadWeb', files=file,
-                                               data=JsonData, cookies={'zaly_site_user': self.token})
+                                               data=Data, cookies={'zaly_site_user': self.token})
         if response.json()['errorInfo'] != '':
             raise UpLoadFileFailedException(response.json()['errorInfo'])
         return response.json()['fileId']
 
     async def _GetPreSessionId(self) -> str:
         LoginData = {
             "action": "api.passport.passwordLogin",
```

### Comparing `THISDLChatBot-2.0.1/THISDLChatBot/Config.py` & `THISDLChatBot-2.0.2/THISDLChatBot/Config.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.1/THISDLChatBot/Friend.py` & `THISDLChatBot-2.0.2/THISDLChatBot/Friend.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.1/THISDLChatBot/Group.py` & `THISDLChatBot-2.0.2/THISDLChatBot/Group.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.1/THISDLChatBot/Logger.py` & `THISDLChatBot-2.0.2/THISDLChatBot/Logger.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.1/THISDLChatBot/Message.py` & `THISDLChatBot-2.0.2/THISDLChatBot/Message.py`

 * *Files identical despite different names*

### Comparing `THISDLChatBot-2.0.1/THISDLChatBot/Plugin.py` & `THISDLChatBot-2.0.2/THISDLChatBot/Plugin.py`

 * *Files identical despite different names*

