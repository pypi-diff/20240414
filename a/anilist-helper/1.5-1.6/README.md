# Comparing `tmp/anilist-helper-1.5.tar.gz` & `tmp/anilist_helper-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anilist-helper-1.5.tar", last modified: Sat Apr 13 00:51:34 2024, max compression
+gzip compressed data, was "anilist_helper-1.6.tar", last modified: Sun Apr 14 09:05:42 2024, max compression
```

## Comparing `anilist-helper-1.5.tar` & `anilist_helper-1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:51:34.167762 anilist-helper-1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-13 00:51:19.000000 anilist-helper-1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-13 00:51:34.167762 anilist-helper-1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6341 2024-04-13 00:51:19.000000 anilist-helper-1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:51:34.167762 anilist-helper-1.5/anilist_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-13 00:51:34.000000 anilist-helper-1.5/anilist_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-13 00:51:34.000000 anilist-helper-1.5/anilist_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 00:51:34.000000 anilist-helper-1.5/anilist_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-13 00:51:34.000000 anilist-helper-1.5/anilist_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-13 00:51:34.000000 anilist-helper-1.5/anilist_helper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:51:34.167762 anilist-helper-1.5/anilisthelper/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-13 00:51:19.000000 anilist-helper-1.5/anilisthelper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19023 2024-04-13 00:51:19.000000 anilist-helper-1.5/anilisthelper/anilist_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-13 00:51:19.000000 anilist-helper-1.5/anilisthelper/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-13 00:51:19.000000 anilist-helper-1.5/anilisthelper/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-13 00:51:19.000000 anilist-helper-1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 00:51:34.167762 anilist-helper-1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-13 00:51:19.000000 anilist-helper-1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:05:42.544222 anilist_helper-1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35129 2024-04-14 09:05:35.000000 anilist_helper-1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-04-14 09:05:42.544222 anilist_helper-1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7015 2024-04-14 09:05:35.000000 anilist_helper-1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:05:42.544222 anilist_helper-1.6/anilist_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-04-14 09:05:42.000000 anilist_helper-1.6/anilist_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-14 09:05:42.000000 anilist_helper-1.6/anilist_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 09:05:42.000000 anilist_helper-1.6/anilist_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-14 09:05:42.000000 anilist_helper-1.6/anilist_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-14 09:05:42.000000 anilist_helper-1.6/anilist_helper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:05:42.544222 anilist_helper-1.6/anilisthelper/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-14 09:05:35.000000 anilist_helper-1.6/anilisthelper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19223 2024-04-14 09:05:35.000000 anilist_helper-1.6/anilisthelper/anilist_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-14 09:05:35.000000 anilist_helper-1.6/anilisthelper/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-14 09:05:35.000000 anilist_helper-1.6/anilisthelper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-14 09:05:35.000000 anilist_helper-1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 09:05:42.544222 anilist_helper-1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-14 09:05:35.000000 anilist_helper-1.6/setup.py
```

### Comparing `anilist-helper-1.5/LICENSE` & `anilist_helper-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `anilist-helper-1.5/PKG-INFO` & `anilist_helper-1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anilist-helper
-Version: 1.5
+Version: 1.6
 Summary: A simple library to help you fetch data from AniList.
 Author: Dominik Procházka
 Maintainer: Dominik Procházka
 Project-URL: Homepage, https://github.com/ProchyGaming/anilist-helper
 Project-URL: Documentation, https://github.com/ProchyGaming/anilist-helper/wiki
 Project-URL: Source, https://github.com/ProchyGaming/anilist-helper
 Keywords: python,anilist
@@ -85,14 +85,19 @@
 * After that the library is successfully set-up and ready for use.
 
 ## Help
 
 If you encounter any issues, feel free to open a new issue. If you have any new ideas or fixes, please open a pull request, they are more than welcome!
 
 ## Version History
+* [1.06](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.06)
+    * [get_id(): Make sure we actually return None](https://github.com/ProchyGaming/anilist-helper/commit/0aa230077ab7a3733508f5473a1f7e4d35096989)
+    * [anilist_helper: Create dir for config](https://github.com/ProchyGaming/anilist-helper/commit/db3940710e7a6866d97293d7067f26aab60f09f5)
+    * [check_status_in_cache(): generate upcoming ep if not known](https://github.com/ProchyGaming/anilist-helper/commit/3b3ef0a269866eb11938cb5fe23191aea57804bd)
+    * [anilist_helper: drop unnecessary imports](https://github.com/ProchyGaming/anilist-helper/commit/f651a08cf50e1c82ef9d3ce94c1499f0e89fb65c)
 * [1.05](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.05)
     * [get_all_anime_for_user(): Allow list as status](https://github.com/ProchyGaming/anilist-helper/commit/ae0906ae17940de5511b044abe4de957ef28a2b9)
     * [anilist_helper(): Add support for external api key](https://github.com/ProchyGaming/anilist-helper/commit/95ed72aa2f43a385ae8a40ed27b7c42fbe3b1c5d)
     * [anilist_helper: add MAL_ID into collected data](https://github.com/ProchyGaming/anilist-helper/commit/3c05821fa6ccfb3411ab3c4287ce47255da87fde)
     * [anilist_helper: Rewrite](https://github.com/ProchyGaming/anilist-helper/commit/d19059c2ef805d5d3cff318afd0bcc119608a8b6)
     * [anilist_helper: Add is_sus flag](https://github.com/ProchyGaming/anilist-helper/commit/5b6b2bfe14f09dbf3bb06d1a8f2dea80fa1e5f16)
 * [1.042](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.042)
```

### Comparing `anilist-helper-1.5/README.md` & `anilist_helper-1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,19 @@
 * After that the library is successfully set-up and ready for use.
 
 ## Help
 
 If you encounter any issues, feel free to open a new issue. If you have any new ideas or fixes, please open a pull request, they are more than welcome!
 
 ## Version History
+* [1.06](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.06)
+    * [get_id(): Make sure we actually return None](https://github.com/ProchyGaming/anilist-helper/commit/0aa230077ab7a3733508f5473a1f7e4d35096989)
+    * [anilist_helper: Create dir for config](https://github.com/ProchyGaming/anilist-helper/commit/db3940710e7a6866d97293d7067f26aab60f09f5)
+    * [check_status_in_cache(): generate upcoming ep if not known](https://github.com/ProchyGaming/anilist-helper/commit/3b3ef0a269866eb11938cb5fe23191aea57804bd)
+    * [anilist_helper: drop unnecessary imports](https://github.com/ProchyGaming/anilist-helper/commit/f651a08cf50e1c82ef9d3ce94c1499f0e89fb65c)
 * [1.05](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.05)
     * [get_all_anime_for_user(): Allow list as status](https://github.com/ProchyGaming/anilist-helper/commit/ae0906ae17940de5511b044abe4de957ef28a2b9)
     * [anilist_helper(): Add support for external api key](https://github.com/ProchyGaming/anilist-helper/commit/95ed72aa2f43a385ae8a40ed27b7c42fbe3b1c5d)
     * [anilist_helper: add MAL_ID into collected data](https://github.com/ProchyGaming/anilist-helper/commit/3c05821fa6ccfb3411ab3c4287ce47255da87fde)
     * [anilist_helper: Rewrite](https://github.com/ProchyGaming/anilist-helper/commit/d19059c2ef805d5d3cff318afd0bcc119608a8b6)
     * [anilist_helper: Add is_sus flag](https://github.com/ProchyGaming/anilist-helper/commit/5b6b2bfe14f09dbf3bb06d1a8f2dea80fa1e5f16)
 * [1.042](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.042)
```

### Comparing `anilist-helper-1.5/anilist_helper.egg-info/PKG-INFO` & `anilist_helper-1.6/anilist_helper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anilist-helper
-Version: 1.5
+Version: 1.6
 Summary: A simple library to help you fetch data from AniList.
 Author: Dominik Procházka
 Maintainer: Dominik Procházka
 Project-URL: Homepage, https://github.com/ProchyGaming/anilist-helper
 Project-URL: Documentation, https://github.com/ProchyGaming/anilist-helper/wiki
 Project-URL: Source, https://github.com/ProchyGaming/anilist-helper
 Keywords: python,anilist
@@ -85,14 +85,19 @@
 * After that the library is successfully set-up and ready for use.
 
 ## Help
 
 If you encounter any issues, feel free to open a new issue. If you have any new ideas or fixes, please open a pull request, they are more than welcome!
 
 ## Version History
+* [1.06](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.06)
+    * [get_id(): Make sure we actually return None](https://github.com/ProchyGaming/anilist-helper/commit/0aa230077ab7a3733508f5473a1f7e4d35096989)
+    * [anilist_helper: Create dir for config](https://github.com/ProchyGaming/anilist-helper/commit/db3940710e7a6866d97293d7067f26aab60f09f5)
+    * [check_status_in_cache(): generate upcoming ep if not known](https://github.com/ProchyGaming/anilist-helper/commit/3b3ef0a269866eb11938cb5fe23191aea57804bd)
+    * [anilist_helper: drop unnecessary imports](https://github.com/ProchyGaming/anilist-helper/commit/f651a08cf50e1c82ef9d3ce94c1499f0e89fb65c)
 * [1.05](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.05)
     * [get_all_anime_for_user(): Allow list as status](https://github.com/ProchyGaming/anilist-helper/commit/ae0906ae17940de5511b044abe4de957ef28a2b9)
     * [anilist_helper(): Add support for external api key](https://github.com/ProchyGaming/anilist-helper/commit/95ed72aa2f43a385ae8a40ed27b7c42fbe3b1c5d)
     * [anilist_helper: add MAL_ID into collected data](https://github.com/ProchyGaming/anilist-helper/commit/3c05821fa6ccfb3411ab3c4287ce47255da87fde)
     * [anilist_helper: Rewrite](https://github.com/ProchyGaming/anilist-helper/commit/d19059c2ef805d5d3cff318afd0bcc119608a8b6)
     * [anilist_helper: Add is_sus flag](https://github.com/ProchyGaming/anilist-helper/commit/5b6b2bfe14f09dbf3bb06d1a8f2dea80fa1e5f16)
 * [1.042](https://github.com/ProchyGaming/anilist-helper/releases/tag/v1.042)
```

### Comparing `anilist-helper-1.5/anilisthelper/anilist_helper.py` & `anilist_helper-1.6/anilisthelper/anilist_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-import requests, time, json, os, webbrowser, copy
+import requests, time, os, copy, math
 from datetime import datetime, timedelta
-from flask import Flask, request, jsonify, send_file
-from gevent.pywsgi import WSGIServer
 from .utils import utils_save_json, utils_read_json
 from .config_utils import config_setup
 
 total_user = {}
 user_entries = {}
 script_path = os.path.dirname(os.path.abspath(__file__))
 anilist_id_cache_path = os.path.join(script_path, 'cache', 'anilist_id_cache.json')
@@ -46,22 +44,26 @@
         end_date = datetime.strptime(cache[anime]['end_date'], '%Y-%m-%d').date()
       except:
         end_date = None
       if not release_date and not end_date:
         continue
       status = cache[anime]['status']
       if status == 'RELEASING':
-        next_ep_date = release_date + timedelta(cache[anime]['upcoming_ep'] * 7)
-        if end_date:
-          if current_date > end_date:
+          try:
+            upcoming_ep = cache[anime]['upcoming_ep']
+          except:
+            upcoming_ep = math.ceil(int((current_date - release_date).days)/7) + 1
+          next_ep_date = release_date + timedelta( * 7)
+          if end_date:
+            if current_date > end_date:
+              updated_info = get_anime_info(anime, True)
+              cache.update(updated_info)
+          if current_date > next_ep_date:
             updated_info = get_anime_info(anime, True)
             cache.update(updated_info)
-        if current_date > next_ep_date:
-          updated_info = get_anime_info(anime, True)
-          cache.update(updated_info)
       elif status == 'NOT_YET_RELEASED':
         if release_date:
           if current_date > release_date:
             cache.update(get_anime_info(anime, True))
     config_dict['checked_date'] = current_date.strftime('%Y-%m-%d')
     utils_save_json(config_path, config_dict)
     utils_save_json(anilist_id_cache_path, cache, True)
@@ -80,14 +82,16 @@
 # Functions
 
 def make_graphql_request(query, variables=None, anilist_token=None):
   if anilist_token:
     pass
   elif 'anilist_key' in os.environ:
     anilist_token = os.getenv('anilist_key')
+    if not os.path.exists(config_path):
+      os.makedirs(os.path.dirname(config_path))
   else:
     anilist_token = load_config()
 
   # Constants for GraphQL endpoint and headers
   ANILIST_API_URL = 'https://graphql.anilist.co'
   HEADERS = {'Content-Type': 'application/json', 'Authorization': f'Bearer {anilist_token}'}
 
@@ -518,24 +522,24 @@
   return anime_data
 
 def get_id(name, anilist_token=None):
   search_cache = utils_read_json(anilist_search_cache_path)
   
   def fetch_from_anilist():
     # Fetch anime info from Anilist API or any other source
-    anime_info = str(anilist_fetch_id(name))
+    anime_info = str(anilist_fetch_id(name)) if anilist_fetch_id(name) else None
     if anime_info:
       ani_dict = get_anime_info(anime_info, False, anilist_token)
       status = ani_dict[anime_info]['status']
       if status == 'NOT_YET_RELEASED':
         anime_info = None
-    json_out = {name: anime_info}
-    utils_save_json(anilist_search_cache_path, json_out, False)
-    return anime_info
-  
+      json_out = {name: anime_info}
+      utils_save_json(anilist_search_cache_path, json_out, False)
+      return anime_info
+    return None
   # Check if anime_id exists in cache
   try:
     if search_cache and name in search_cache:
         print("Returning cached result for search query:", name)
         return str(search_cache[name])
     else:
         return fetch_from_anilist()
```

### Comparing `anilist-helper-1.5/anilisthelper/config_utils.py` & `anilist_helper-1.6/anilisthelper/config_utils.py`

 * *Files identical despite different names*

### Comparing `anilist-helper-1.5/anilisthelper/utils.py` & `anilist_helper-1.6/anilisthelper/utils.py`

 * *Files identical despite different names*

### Comparing `anilist-helper-1.5/pyproject.toml` & `anilist_helper-1.6/pyproject.toml`

 * *Files identical despite different names*

