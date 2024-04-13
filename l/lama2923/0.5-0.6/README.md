# Comparing `tmp/lama2923-0.5.tar.gz` & `tmp/lama2923-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lama2923-0.5.tar", last modified: Fri Apr 12 09:27:15 2024, max compression
+gzip compressed data, was "lama2923-0.6.tar", last modified: Sat Apr 13 18:04:56 2024, max compression
```

## Comparing `lama2923-0.5.tar` & `lama2923-0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 09:27:15.307841 lama2923-0.5/
--rw-rw-rw-   0        0        0      627 2024-04-12 09:27:15.301795 lama2923-0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-12 09:27:15.256698 lama2923-0.5/lama2923/
--rw-rw-rw-   0        0        0    19428 2024-04-12 09:25:37.000000 lama2923-0.5/lama2923/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 09:27:15.295024 lama2923-0.5/lama2923.egg-info/
--rw-rw-rw-   0        0        0      627 2024-04-12 09:27:14.000000 lama2923-0.5/lama2923.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-04-12 09:27:15.000000 lama2923-0.5/lama2923.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 09:27:14.000000 lama2923-0.5/lama2923.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-04-12 09:27:14.000000 lama2923-0.5/lama2923.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-12 09:27:14.000000 lama2923-0.5/lama2923.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 09:27:15.308380 lama2923-0.5/setup.cfg
--rw-rw-rw-   0        0        0      944 2024-04-12 09:26:56.000000 lama2923-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 18:04:56.499534 lama2923-0.6/
+-rw-rw-rw-   0        0        0      895 2024-04-13 18:04:56.497835 lama2923-0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-13 18:04:56.478834 lama2923-0.6/lama2923/
+-rw-rw-rw-   0        0        0    19506 2024-04-13 18:04:10.000000 lama2923-0.6/lama2923/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 18:04:56.494798 lama2923-0.6/lama2923.egg-info/
+-rw-rw-rw-   0        0        0      895 2024-04-13 18:04:56.000000 lama2923-0.6/lama2923.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-04-13 18:04:56.000000 lama2923-0.6/lama2923.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 18:04:56.000000 lama2923-0.6/lama2923.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-04-13 18:04:56.000000 lama2923-0.6/lama2923.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-13 18:04:56.000000 lama2923-0.6/lama2923.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-13 18:04:56.500049 lama2923-0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1233 2024-04-13 18:04:36.000000 lama2923-0.6/setup.py
```

### Comparing `lama2923-0.5/lama2923/__init__.py` & `lama2923-0.6/lama2923/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -406,52 +406,51 @@
                 'Authorization': str(self.token)
             }
             
             r = requests.get(f'https://discord.com/api/v9/channels/{Channel_id}/messages', headers=headers)
             
             if r.status_code == 200:
                 messages = r.json()
-                return messages
+                return [r.status_code, messages]
             else:
                 return r.status_code
             
         def get_specific_message(self, Channel_id, Message_id):
             headers = {'Authorization': str(self.token)}
             url = f'https://discord.com/api/v9/channels/{Channel_id}/messages/{Message_id}'
             response = requests.get(url, headers=headers)
             if response.status_code == 200:
-                return response.json()
+                return [response.status_code, response.json()]
             else:
                 return response.status_code
 
 
         def add_reaction(self, Channel_id, Message_id, emoji):
             headers = {'Authorization': str(self.token)}
-            # Discord requires emojis to be URL encoded
             emoji = requests.utils.quote(emoji)
             url = f'https://discord.com/api/v9/channels/{Channel_id}/messages/{Message_id}/reactions/{emoji}/@me'
             response = requests.put(url, headers=headers)
             return response.status_code
 
 
         def get_channel_info(self, Channel_id):
             headers = {'Authorization': str(self.token)}
             url = f'https://discord.com/api/v9/channels/{Channel_id}'
             response = requests.get(url, headers=headers)
             if response.status_code == 200:
-                return response.json()
+                return [response.status_code, response.json()]
             else:
                 return response.status_code
     
         def list_guild_channels(self, Guild_id):
             headers = {'Authorization': str(self.token)}
             url = f'https://discord.com/api/v9/guilds/{Guild_id}/channels'
             response = requests.get(url, headers=headers)
             if response.status_code == 200:
-                return response.json()
+                return [response.status_code, response.json()]
             else:
                 return response.status_code   
 
         def send_tts_message(self, Channel_id, Message):
             payload = {'content': str(Message), 'tts': True}
             headers = {'Authorization': str(self.token)}
             response = requests.post(f'https://discord.com/api/v9/channels/{Channel_id}/messages', data=payload, headers=headers)
@@ -513,15 +512,15 @@
                             with open(file_name, "rb") as file:
                                 files_data[os.path.basename(file_name)] = file.read()
                     response = requests.post(self.WebhookUrl, data=data, files=files_data)
                 else:
 
                     response = requests.post(self.WebhookUrl, json=data)
 
-                return response
+                return response.status_code
             
             else:
                 if files is not None and isinstance(files, list):
                     files_data = {}
                     for file_name in files:
                         if os.path.getsize(file_name) > 0:
                             with open(file_name, "rb") as file:
@@ -532,12 +531,15 @@
                     response = requests.post(self.WebhookUrl, json=data)
                     response2 = requests.post(self.WebhookUrl, json=data2, files=files_data)
                     return [response, response2]
                 else:
                     
                     response = requests.post(self.WebhookUrl, json=data)
                 
-                    return response
+                    return response.status_code
+                
+
+
```

