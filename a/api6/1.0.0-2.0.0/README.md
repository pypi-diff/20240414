# Comparing `tmp/api6-1.0.0.tar.gz` & `tmp/api6-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api6-1.0.0.tar", last modified: Fri Apr 12 12:51:35 2024, max compression
+gzip compressed data, was "api6-2.0.0.tar", last modified: Sun Apr 14 19:41:49 2024, max compression
```

## Comparing `api6-1.0.0.tar` & `api6-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-12 12:51:35.303336 api6-1.0.0/
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)     1091 2024-04-04 15:04:40.000000 api6-1.0.0/LICENCE
--rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)      596 2024-04-12 12:51:35.303336 api6-1.0.0/PKG-INFO
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)      170 2024-04-05 07:30:12.000000 api6-1.0.0/README.md
-drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-12 12:51:35.303336 api6-1.0.0/api6/
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)     6823 2024-04-12 12:39:54.000000 api6-1.0.0/api6/Encryption.py
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)       25 2024-04-12 12:38:40.000000 api6-1.0.0/api6/__init__.py
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)    35588 2024-04-12 12:41:24.000000 api6-1.0.0/api6/client.py
-drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-12 12:51:35.303336 api6-1.0.0/api6.egg-info/
--rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)      596 2024-04-12 12:51:35.000000 api6-1.0.0/api6.egg-info/PKG-INFO
--rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)      189 2024-04-12 12:51:35.000000 api6-1.0.0/api6.egg-info/SOURCES.txt
--rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)        1 2024-04-12 12:51:35.000000 api6-1.0.0/api6.egg-info/dependency_links.txt
--rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)        5 2024-04-12 12:51:35.000000 api6-1.0.0/api6.egg-info/top_level.txt
--rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)       38 2024-04-12 12:51:35.303336 api6-1.0.0/setup.cfg
--rw-rw----   0 rubinoss  (3771) rubinoss  (3775)      568 2024-04-12 12:49:07.000000 api6-1.0.0/setup.py
+drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-14 19:41:49.341411 api6-2.0.0/
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)     1091 2024-04-04 15:04:40.000000 api6-2.0.0/LICENCE
+-rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)      596 2024-04-14 19:41:49.341411 api6-2.0.0/PKG-INFO
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)      170 2024-04-05 07:30:12.000000 api6-2.0.0/README.md
+drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-14 19:41:49.340411 api6-2.0.0/api6/
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)     6823 2024-04-12 12:39:54.000000 api6-2.0.0/api6/Encryption.py
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)       25 2024-04-12 12:38:40.000000 api6-2.0.0/api6/__init__.py
+-rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)    37206 2024-04-14 19:38:10.000000 api6-2.0.0/api6/client.py
+drwxrwxr-x   0 rubinoss  (3771) rubinoss  (3775)        0 2024-04-14 19:41:49.341411 api6-2.0.0/api6.egg-info/
+-rw-r--r--   0 rubinoss  (3771) rubinoss  (3775)      596 2024-04-14 19:41:49.000000 api6-2.0.0/api6.egg-info/PKG-INFO
+-rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)      189 2024-04-14 19:41:49.000000 api6-2.0.0/api6.egg-info/SOURCES.txt
+-rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)        1 2024-04-14 19:41:49.000000 api6-2.0.0/api6.egg-info/dependency_links.txt
+-rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)        5 2024-04-14 19:41:49.000000 api6-2.0.0/api6.egg-info/top_level.txt
+-rw-rw-r--   0 rubinoss  (3771) rubinoss  (3775)       38 2024-04-14 19:41:49.341411 api6-2.0.0/setup.cfg
+-rw-rw----   0 rubinoss  (3771) rubinoss  (3775)      568 2024-04-14 19:37:11.000000 api6-2.0.0/setup.py
```

### Comparing `api6-1.0.0/LICENCE` & `api6-2.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `api6-1.0.0/PKG-INFO` & `api6-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api6
-Version: 1.0.0
+Version: 2.0.0
 Summary: Luis Rubika Bot to Rubika api 6
 Home-page: https://guides.github.com/features/mastering-markdown/
 Author: Luis
 Author-email: mm12mok18@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `api6-1.0.0/api6/Encryption.py` & `api6-2.0.0/api6/Encryption.py`

 * *Files identical despite different names*

### Comparing `api6-1.0.0/api6/client.py` & `api6-2.0.0/api6/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,123 +16,125 @@
 from pathlib import Path
 import time
 from tqdm import tqdm
 import os
 from urllib3 import PoolManager, ProxyManager
 import asyncio
 class Client:
-	def __init__(self, auth:str,key:str=None,palqform:str='Android',pak:str='app.rbmain.a',v:str="3.4.3"):
+	def __init__(self, auth:str,key:str=None,palqform:str='Android',pak:str='app.rbmain.a',v:str="3.4.3",type:str="rubika"):
 		self.palqform = palqform
 		self.v = v
 		self.requ = PoolManager()
 		self.pak = pak
 		self.auth = auth
 		self.auth_send = Encryption.authSet(auth)
 		self.t = "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"
 		if key == None:
 			self.key = None
 		else:
 			privateKey = key.replace('=','')
 			self.key = privateKey
+		if type == "rubika":
+			self.url = "https://messengerg2c58.iranlms.ir/"
+		else:
+			 if type == "shad":
+			 	self.url = "https://shadmessenger32.iranlms.ir/"
 	def requests(self, input, method):
 	   client = {"app_name": "Main", "package": self.pak, "app_version": self.v, "lang_code": "fa", "platform": self.palqform}
 	   method_payload = {"input": input, "method": method, "client": client}
 	   method_payload = dumps(method_payload)
 	   data_enc = Encryption.encrypt(method_payload, self.auth)
 	   sign = Encryption.sign_rsa(self.key, data_enc)
 	   data = {"api_version": "6", "data_enc": data_enc, "sign": sign, "auth": self.auth_send}
-	   url = "https://messengerg2c58.iranlms.ir/"
-	   Luis =  loads(self.requ.request("POST", url=url, body=dumps(data)).data.decode('utf-8'))
+	   Luis =  loads(self.requ.request("POST", url=self.url, body=dumps(data)).data.decode('utf-8'))
 	   data_enc = Luis['data_enc']
 	   data = Encryption.decode(data_enc, self.auth)
 	   data = loads(data)
 	   return data
 	def getUser(self):
 		return self.requests({},"getUserInfo")
 	def joinGroup(self,link:str):
 		return self.requests({"hash_link":link},'joinGroup')
-	def sendMessage(self,goid:str,text:str):
-		return self.requests({"object_guid":goid,"text":text,"rnd":str(randint(9282873, 102662617171))},"sendMessage")
+	def sendMessage(self,goid:str,text:str,id:str=None):
+		return self.requests({"object_guid":goid,"text":text,"rnd":str(randint(9282873, 102662617171)),"reply_to_message_id":id},"sendMessage")
 	def leaveGroup(self,goid):
 		return self.requests({"group_guid":goid},"leaveGroup")
 	def joinChannelAction(self,goid):
 		return self.requests({"channel_guid":goid,"action":"join"},"joinChannelAction")
 	def leaveChannelAction(self,goid):
 		return self.requests({"channel_guid":goid,"action":"Leave"},"joinChannelAction")
 	def getServiceInfo(self):
 		return self.requests({"service_guid":"s0B0e8da28a4fde394257f518e64e800"},"getServiceInfo")
 	def deleteMessages(self,goid,id):
-		return self.requests({"object_guid":Goid,"message_ids":[id],"type":"Local"},"deleteMessages")
+		return self.requests({"object_guid":goid,"message_ids":[id],"type":"Local"},"deleteMessages")
 	def deleteMessagesAcon(self,goid,id):
-		return self.requests({"object_guid":Goid,"message_ids":[id],"type":"Global"},"deleteMessages")
+		return self.requests({"object_guid":goid,"message_ids":[id],"type":"Global"},"deleteMessages")
 	def getGroupInfo(self, goid:str):
 		return self.requests({"group_guid":goid},"getGroupInfo")
 	def groupPreviewByJoinLink(self, link:str):
 		return self.requests({"hash_link":link},"groupPreviewByJoinLink")
 	def channelPreviewByJoinLink(self, link:str):
 		return self.requests({"hash_link":link},"channelPreviewByJoinLink")
 	def updateUsername(self, id:str):
 		return self.requests({"username":id},updateUsername)
-	def getGroupAllMembers(self, goid:str):
-		return self.requests({"group_guid":goid,"search_text":None,"start_id":None},"getGroupAllMembers")
+	def getGroupAllMembers(self, goid:str,start_id=None):
+		return self.requests({"group_guid":goid,"search_text":None,"start_id":start_id},"getGroupAllMembers")
 	def searchGlobalObjects(self, text):
 		return self.requests({"search_text":text},"searchGlobalObjects")
 	def updateProfile(self,name,bio):
 		return self.requests({"first_name":name,"bio":bio,"updated_parameters":["first_name","bio"]},"updateProfile")
 	def getObjectByUsername(self,user):
 		return self.requests({"username":user},"getObjectByUsername")
 	def getUserInfo(self,user):
 		return self.requests({"user_guid":user},"getUserInfo")
-	def getChats(self):
-		return self.requests({"start_id":"null"},"getChats")
+	def getChats(self,start_id=None):
+		return self.requests({"start_id":start_id},"getChats")
 	def getChannelInfo(self,goid):
 		return self.requests({"channel_guid":goid},"getChannelInfo")
 	def joinChannelByLink(self,link):
 		return self.requests({"hash_link":link},"joinChannelByLink")
 	def setChannelAdmin(self,goid,goidm):
 		return self.requests({"channel_guid":goid,"member_guid":goidm,"action":"SetAdmin","access_list":["ChangeInfo","ViewMembers","ViewAdmins","PinMessages","SendMessages","EditAllMessages","DeleteGlobalAllMessages","AddMember","SetJoinLink","SetAdmin"]},"setChannelAdmin")
 	def requestChangeObjectOwner(self,goid,goidm):
 		return self.requests({"object_guid":goid,"new_owner_user_guid":goidm},"requestChangeObjectOwner")
 	def getMySessions(self):
 		return self.requests({},"getMySessions")
 	def terminateOtherSessions(self):
 		return self.requests({},"terminateOtherSessions")
 	def getLinkFromAppUrl(self,link):
 		return self.requests({"app_url":link},"getLinkFromAppUrl")
-	def forwardMessages(self,goid,togoid,id):
-		return self.requests({"from_object_guid":goid,"to_object_guid":togoid,"message_ids":[id],"rnd":str(randint(9282873, 102662617171))},"forwardMessages")
-	def getMessages(self,goid,id:int):
-		return self.requests({"object_guid":goid,"min_id":id,"sort":"FromMin","filter_type":None},"getMessages")
-	def getMessagess(self,goid):
-		return self.requests({"object_guid":goid,"max_id":None,"sort":"FromMin","filter_type":None},"getMessages")
+	def forwardMessages(self,goid,togoid,id:list):
+		return self.requests({"from_object_guid":goid,"to_object_guid":togoid,"message_ids":id,"rnd":str(randint(9282873, 102662617171))},"forwardMessages")
+	def getMessages(self,goid,id:int=None,type="Min"):
+		return self.requests({"object_guid":goid,f"{type.lower()}_id":id,"sort":f"From{type}","filter_type":None},"getMessages")
 	def votePoll(self,id,num:int):
 		num = num - 1
 		return self.requests({"poll_id":id,"selection_index":num},"votePoll")
 	def editMessage(self,goid,id,text):
 		return self.requests({"object_guid":goid,"message_id":id,"text":text},"editMessage")
-	def getContacts(self):
-		return self.requests({"start_id":"null"},"getContacts")
+	def getContacts(self,start_id=None):
+		return self.requests({"start_id":start_id},"getContacts")
 	def getAvailableReactions(self):
 		return self.requests({},"getAvailableReactions")
 	def getMyGifSet(self):
 		return self.requests({},"getMyGifSet")
-	def getBlockedUsers(self):
-		return self.requests({"start_id":"null"},"getBlockedUsers")
+	def getBlockedUsers(self,start_id=None):
+		return self.requests({"start_id":start_id},"getBlockedUsers")
 	def getPrivacySetting(self):
 		return self.requests({},"getPrivacySetting")
 	def getMessagesInterval(self,goid,id):
 		return self.requests({"object_guid":goid,"middle_message_id":id,"filter_type":None},"getMessagesInterval")
-	def getTimeUp(self):
+	def getTime(self):
 		return self.requests({},'getTime')
 	def getChatsUpdates(self):
-		data = self.getTimeUp()["data"]['time']
+		data = self.getTime()["data"]['time']
 		p = {"state":data}
 		return self.requests(p,"getChatsUpdates")
 	def getMessagesUpdates(self, goid):
-		time = self.getTimeUp['data']['time']
+		time = self.getTime()['data']['time']
 		return self.requests({"object_guid":goid,"state":time},'getMessagesUpdates')
 	def getTopChatUsers(self):
 		return self.requests({},"getTopChatUsers")
 	def removeFromTopChatUsers(self,guid:str):
 		return self.requests({"user_guid":guid},"removeFromTopChatUsers")
 	def getChatLink(self,guid:str):
 		type = self.getType(guid)
@@ -416,36 +418,50 @@
 		name = "discardCall"
 		input = {
                 "call_id": id,
                 "duration": None,
                 "reason":"Missed"
             }
 		return self.requests(input,name)
+	def sendMessageHyperLink(self,guid,text,link,id:str=None):
+		input = {"object_guid":guid,"rnd":str(randint(9282873, 102662617171)),"text":text,"reply_to_message_id":id,"metadata":{"meta_data_parts":[{"from_index":0,"length":len(text),"link":{"hyperlink_data":{"url":link},"type":"hyperlink"},"type":"Link"}]}}
+		return self.requests(input,"sendMessage")
+	def sendMessageMentionText(self,guid,text,id=None):
+		input = {"object_guid":guid,"text":text,"rnd":str(randint(9282873, 102662617171)),"reply_to_message_id":id,"metadata":{"meta_data_parts":[{"type":"MentionText","mention_text_object_guid":guid,"from_index":0,"length":len(text),"mention_text_object_type":"User"}]}}
+		return self.requests(input,"sendMessage")
 	def getMessageAllGroup(self,guid,number:int=10):
 		last = self.getGroupInfo(guid)['data']['chat']['last_message']['message_id']
 		list = []
-		for x in range(number):
-			p = self.getMessagesInterval(guid,last)
-			mass = p['data']['messages']
-			to = int(len(mass)) - 1
-			last = mass[to]['message_id']
-			list  = list + mass
+		for x in range(int(number)):
+				p = self.getMessages(guid,last,"Max")
+				if "new_max_id" in p['data']:
+					last = p['data']['new_max_id']
+				list += p['data']['messages']
 		return list
 	def getMessageAllChannel(self,guid,number:int=10):
 			last = self.getChannelInfo(guid)['data']['chat']['last_message_id']
-			list = [None]
-			for x in range(number):
-				p = self.getMessagesInterval(guid,last)
-			mass = p['data']['messages']
-			to = int(len(mass)) - 1
-			last = mass[to]['message_id']
-			for m in mass:
-				list.append(m)
+			list =[]
+			for x in range(int(number)):
+				p = self.getMessages(guid,last,"Max")
+				if "new_max_id" in p['data']:
+					last = p['data']['new_max_id']
+				list += p['data']['messages']
 			return list
-	def requestCall(self,guid,type):
+	def getChatsAll(self):
+		input = {"start_id":None}
+		list = []
+		re = self.requests(input,"getChats")
+		num=0
+		for x in range(int(10)):
+			start_id = int(len(re)) + int(num)
+			if "data" in re:
+				list += re['data']['chats']
+			re = self.requests({"start_id":start_id},"getChats")
+		return list
+	def requestCall(self,guid,type=None):
 		name = "requestCall"
 		input = {
                 "call_type": type,
                 "library_versions": ["2.7.7","2.4.4"],
                 "max_layer": 92,
                 "min_layer": 65,
                 "sip_version": 1,
@@ -458,14 +474,15 @@
 		input = {
                 "object_guid": guid,
                 "report_description": text,
                 "report_type": 100,
                 "report_type_object": "Object"
             }
 		return self.requests(input,name)
+	
 	def getType(self, guid:str):
 		user = guid[0]
 		if user == "u":
 			return "User"
 		if user == "c":
 			return "Channel"
 		if user == "g":
@@ -533,20 +550,24 @@
 	def uploadAvatarBogGroup(self,file:str,files:str,link):
 		goid = self.joinGroup()['data']['group']['group_guid']
 		hash_rec = self.uplodFile(file)
 		to = self.uplodFile(files)
 		input = {"object_guid":goid,"thumbnail_file_id":hash_rec['id'],"main_file_id":to['id']}
 		return self.requests(input,'uploadAvatar')
 	def postTmp(self, input,name):
-		client = {"app_name":"Main","package":"app.rbmain.a","app_version":"3.4.3","lang_code":"fa","platform":"Android"}
+		client = {"app_name":"Main","package":self.pak,"app_version":self.v,"lang_code":"fa","platform":self.palqform}
 		method = {"client":client,"input":input,"method":name}
 		dataEnc = Encryption.encrypt(method,selg.auth)
 		api = {"api_version":"6","tmp_session":self.auth,"auth":None,"data_enc":dataEnc}
-		p = post(url="https://messengerg2c58.iranlms.ir/",json=api)
+		p = post(url=self.url,json=api)
 		return loads(Encryption.decode(loads(p.text)['data_enc'],self.auth))
+	def registerDevice(self):
+		rnd = str(randint(9282873, 10266261277277171))
+		input = {"app_version":"MA_3.4.3","device_hash":rnd,"device_model":"api6","is_multi_account":False,"lang_code":"fa","system_version":"SDK 28","token":"","token_type":"Firebase"}
+		return self.requests(input,'registerDevice')
 	def sendCode(self, phone):
 		phone = "##" + str(phone)
 		phone = phone.replace('##0','')
 		phone = phone.replace('##','')
 		phone = '98'+ phone
 		input = {"phone_number":str(phone),"send_type":"SMS"}
 		return self.postTmp(input,'sendCode')['data']['phone_code_hash']
@@ -572,14 +593,17 @@
 		"phone_code_hash": str(hash),
 		"phone_code": str(code),
 		"public_key": pubic_key,
 		}
 		p = self.postTmp(input,'signIn')
 		authOld = p['data']['auth']
 		auth = Encryption.decrypt_rsa(authOld,private_key)
+		self.auth = auth
+		self.key = private_key
+		m = self.registerDevice()
 		return [auth,private_key]
 	def sendViceBog(self,goid,file:str):
 		rnd = str(randint(9282873, 102662617171))
 		p = self.uplodFile(file=file)
 		input = {"file_inline":{"dc_id":p['dc'],"file_id":p['id'],"file_name":p['name'],"size":p['size'],"mime":p['mime'],"access_hash_rec":p['hash'],"type":"Voice","is_spoil":False,"time":10000000009900000},"object_guid":goid,"rnd":rnd}
 		p = self.requests(input,"sendMessage")
 		return p
@@ -601,15 +625,15 @@
 		input = {"file_inline":{"dc_id":p['dc'],"file_id":p['id'],"file_name":p['name'],"size":99999999999999999,"mime":p['mime'],"access_hash_rec":p['hash'],"type":"File","is_spoil":False},"object_guid":goid,"rnd":rnd}
 		p = self.requests(input,"sendMessage")
 		return p
 	def sendGifBog(self,goid,file:str):
 		width, height = [100,100]
 		rnd = str(randint(9282873, 102662617171))
 		p = self.uplodFile(file=file)
-		input = {"file_inline":{"dc_id":p['dc'],"file_id":p['id'],"file_name":p['name'],"size":p['size'],"mime":p['mime'],"access_hash_rec":p['hash'],"type":"Gif","is_spoil":False,"time":999990990000,"height":height,"width":width,"a(uto_play":False,"thumb_inline":self.t},"object_guid":goid,"rnd":rnd}
+		input = {"file_inline":{"dc_id":p['dc'],"file_id":p['id'],"file_name":p['name'],"size":p['size'],"mime":p['mime'],"access_hash_rec":p['hash'],"type":"Gif","is_spoil":False,"time":999990990000,"height":height,"width":width,"auto_play":False,"thumb_inline":self.t},"object_guid":goid,"rnd":rnd}
 		p = self.requests(input,"sendMessage")
 		return p
 	def getVoiceDuration(bytes:bytes) -> int:
 	       file = BytesIO()
 	       file.write(bytes)
 	       file.seek(0)
 	       return mp3.MP3(file).info.length
@@ -706,28 +730,34 @@
 		headers= {
             "auth": self.auth,
             "access-hash-rec": accessHashRec,
             "dc-id": str(dcId),
             "file-id": str(fileId),
             "Host": f"messenger{dcId}.iranlms.ir",
             "client-app-name": "Main",
-            "client-app-version": "3.5.7",
-            "client-package": "app.rbmain.a",
-            "client-platform": "Android",
+            "client-app-version": self.v,
+            "client-package": self.pak,
+            "client-platform": self.palqform,
             "Connection": "Keep-Alive",
             "Content-Type": "application/json",
             "User-Agent": "okhttp/3.12.1"
         }
 		url = f"https://messenger{dcId}.iranlms.ir/GetFile.ashx"
 		response = self.requ.request("POST",preload_content=False,headers=headers,url=url)
 		type=fileName.split(".")[-1]
 		data:bytes = b""
 		num = 0
 		for x in response:
 			data += x
+			print(f"{ste(num)}/{len(response)}")
+		if path == None:
+			path = None
+		else:
+			with open(path, 'wb') as file:
+				file.write(data)
 		return data
 class rubino:
 	def  __init__(self, auth:str=None):
 		self.auth = auth
 	def method(auth,input,name,url= 'https://rubino5.iranlms.ir/'):
 		method = {"api_version":"0","auth":auth,"client":{"app_name":"Main","app_version":"3.6.4","lang_code":"fa","package":"app.rbmain.a","platform":"Android"},"data":input,"method":name}
 		p = post(url=url,json=method)
@@ -796,8 +826,9 @@
 class Luis(Client):...
 class BotX(Luis):...
 class client(Luis):...
 class auth(Luis):...
 class private(Luis):...
 class privateKey(Luis):...
 class key(Luis):...
-class methods(Luis):...
+class methods(Luis):...
+class shad(Luis):...
```

### Comparing `api6-1.0.0/api6.egg-info/PKG-INFO` & `api6-2.0.0/api6.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: api6
-Version: 1.0.0
+Version: 2.0.0
 Summary: Luis Rubika Bot to Rubika api 6
 Home-page: https://guides.github.com/features/mastering-markdown/
 Author: Luis
 Author-email: mm12mok18@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `api6-1.0.0/setup.py` & `api6-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name='api6',
-    version='1.0.0',
+    version='2.0.0',
     packages= ["api6"],
     url='https://guides.github.com/features/mastering-markdown/',
     license='MIT',
     author='Luis',
     author_email='mm12mok18@gmail.com',
     description='Luis Rubika Bot to Rubika api 6',
     long_description= open("README.md",'r').read(),
```

