# Comparing `tmp/twikit-1.4.7.tar.gz` & `tmp/twikit-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twikit-1.4.7.tar", last modified: Fri Apr 12 13:44:07 2024, max compression
+gzip compressed data, was "twikit-1.4.8.tar", last modified: Sat Apr 13 14:30:21 2024, max compression
```

## Comparing `twikit-1.4.7.tar` & `twikit-1.4.8.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 13:44:07.539001 twikit-1.4.7/
--rw-rw-rw-   0        0        0     1079 2024-04-06 11:03:16.000000 twikit-1.4.7/LICENSE
--rw-rw-rw-   0        0        0     3863 2024-04-12 13:44:07.536010 twikit-1.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     3590 2024-04-08 13:45:07.000000 twikit-1.4.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-12 13:44:07.539001 twikit-1.4.7/setup.cfg
--rw-rw-rw-   0        0        0      694 2024-04-08 07:44:57.000000 twikit-1.4.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:44:07.463204 twikit-1.4.7/twikit/
--rw-rw-rw-   0        0        0      509 2024-04-12 13:42:19.000000 twikit-1.4.7/twikit/__init__.py
--rw-rw-rw-   0        0        0   112236 2024-04-12 13:32:55.000000 twikit-1.4.7/twikit/client.py
--rw-rw-rw-   0        0        0     2380 2024-04-06 04:29:07.000000 twikit-1.4.7/twikit/errors.py
--rw-rw-rw-   0        0        0     7305 2024-04-08 14:07:28.000000 twikit-1.4.7/twikit/group.py
--rw-rw-rw-   0        0        0     1913 2024-04-06 04:28:27.000000 twikit-1.4.7/twikit/http.py
--rw-rw-rw-   0        0        0     7617 2024-04-08 13:03:12.000000 twikit-1.4.7/twikit/list.py
--rw-rw-rw-   0        0        0     3908 2024-04-06 13:37:31.000000 twikit-1.4.7/twikit/message.py
--rw-rw-rw-   0        0        0     1439 2024-04-06 13:37:50.000000 twikit-1.4.7/twikit/notification.py
--rw-rw-rw-   0        0        0     1070 2024-04-08 13:03:49.000000 twikit-1.4.7/twikit/trend.py
--rw-rw-rw-   0        0        0    20706 2024-04-12 09:14:00.000000 twikit-1.4.7/twikit/tweet.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:44:07.533018 twikit-1.4.7/twikit/twikit_async/
--rw-rw-rw-   0        0        0      461 2024-04-10 11:59:51.000000 twikit-1.4.7/twikit/twikit_async/__init__.py
--rw-rw-rw-   0        0        0   114259 2024-04-12 13:16:46.000000 twikit-1.4.7/twikit/twikit_async/client.py
--rw-rw-rw-   0        0        0      875 2024-03-23 06:08:25.000000 twikit-1.4.7/twikit/twikit_async/errors.py
--rw-rw-rw-   0        0        0     7509 2024-04-08 14:09:21.000000 twikit-1.4.7/twikit/twikit_async/group.py
--rw-rw-rw-   0        0        0     1955 2024-04-06 04:28:33.000000 twikit-1.4.7/twikit/twikit_async/http.py
--rw-rw-rw-   0        0        0     7780 2024-04-08 13:08:52.000000 twikit-1.4.7/twikit/twikit_async/list.py
--rw-rw-rw-   0        0        0     3974 2024-04-06 13:49:04.000000 twikit-1.4.7/twikit/twikit_async/message.py
--rw-rw-rw-   0        0        0     1439 2024-04-06 13:49:28.000000 twikit-1.4.7/twikit/twikit_async/notification.py
--rw-rw-rw-   0        0        0     1079 2024-04-06 13:49:39.000000 twikit-1.4.7/twikit/twikit_async/trend.py
--rw-rw-rw-   0        0        0    20105 2024-04-09 11:54:15.000000 twikit-1.4.7/twikit/twikit_async/tweet.py
--rw-rw-rw-   0        0        0    14677 2024-04-08 13:10:20.000000 twikit-1.4.7/twikit/twikit_async/user.py
--rw-rw-rw-   0        0        0     3390 2024-04-06 13:55:17.000000 twikit-1.4.7/twikit/twikit_async/utils.py
--rw-rw-rw-   0        0        0    14454 2024-04-08 13:05:19.000000 twikit-1.4.7/twikit/user.py
--rw-rw-rw-   0        0        0    21797 2024-04-12 12:58:43.000000 twikit-1.4.7/twikit/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-12 13:44:07.483150 twikit-1.4.7/twikit.egg-info/
--rw-rw-rw-   0        0        0     3863 2024-04-12 13:44:07.000000 twikit-1.4.7/twikit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      737 2024-04-12 13:44:07.000000 twikit-1.4.7/twikit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 13:44:07.000000 twikit-1.4.7/twikit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-12 13:44:07.000000 twikit-1.4.7/twikit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-12 13:44:07.000000 twikit-1.4.7/twikit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 14:30:21.579847 twikit-1.4.8/
+-rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:36.000000 twikit-1.4.8/LICENSE
+-rw-rw-rw-   0        0        0     3863 2024-04-13 14:30:21.577854 twikit-1.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3590 2024-04-13 12:42:36.000000 twikit-1.4.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-13 14:30:21.579847 twikit-1.4.8/setup.cfg
+-rw-rw-rw-   0        0        0      694 2024-04-13 12:42:36.000000 twikit-1.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 14:30:21.473135 twikit-1.4.8/twikit/
+-rw-rw-rw-   0        0        0      509 2024-04-13 14:18:06.000000 twikit-1.4.8/twikit/__init__.py
+-rw-rw-rw-   0        0        0   112871 2024-04-13 14:14:20.000000 twikit-1.4.8/twikit/client.py
+-rw-rw-rw-   0        0        0     2380 2024-04-13 12:42:36.000000 twikit-1.4.8/twikit/errors.py
+-rw-rw-rw-   0        0        0     7305 2024-04-13 12:42:36.000000 twikit-1.4.8/twikit/group.py
+-rw-rw-rw-   0        0        0     1913 2024-04-13 14:12:05.000000 twikit-1.4.8/twikit/http.py
+-rw-rw-rw-   0        0        0     7617 2024-04-13 12:42:37.000000 twikit-1.4.8/twikit/list.py
+-rw-rw-rw-   0        0        0     3908 2024-04-13 12:42:37.000000 twikit-1.4.8/twikit/message.py
+-rw-rw-rw-   0        0        0     1439 2024-04-13 12:42:37.000000 twikit-1.4.8/twikit/notification.py
+-rw-rw-rw-   0        0        0     1070 2024-04-13 12:42:37.000000 twikit-1.4.8/twikit/trend.py
+-rw-rw-rw-   0        0        0    20706 2024-04-13 12:42:37.000000 twikit-1.4.8/twikit/tweet.py
+drwxrwxrwx   0        0        0        0 2024-04-13 14:30:21.573863 twikit-1.4.8/twikit/twikit_async/
+-rw-rw-rw-   0        0        0      461 2024-04-13 12:42:37.000000 twikit-1.4.8/twikit/twikit_async/__init__.py
+-rw-rw-rw-   0        0        0   114836 2024-04-13 14:14:04.000000 twikit-1.4.8/twikit/twikit_async/client.py
+-rw-rw-rw-   0        0        0      875 2024-04-13 12:42:37.000000 twikit-1.4.8/twikit/twikit_async/errors.py
+-rw-rw-rw-   0        0        0     7509 2024-04-13 12:42:37.000000 twikit-1.4.8/twikit/twikit_async/group.py
+-rw-rw-rw-   0        0        0     1955 2024-04-13 12:42:37.000000 twikit-1.4.8/twikit/twikit_async/http.py
+-rw-rw-rw-   0        0        0     7780 2024-04-13 12:42:37.000000 twikit-1.4.8/twikit/twikit_async/list.py
+-rw-rw-rw-   0        0        0     3974 2024-04-13 12:42:37.000000 twikit-1.4.8/twikit/twikit_async/message.py
+-rw-rw-rw-   0        0        0     1439 2024-04-13 12:42:37.000000 twikit-1.4.8/twikit/twikit_async/notification.py
+-rw-rw-rw-   0        0        0     1079 2024-04-13 12:42:37.000000 twikit-1.4.8/twikit/twikit_async/trend.py
+-rw-rw-rw-   0        0        0    20105 2024-04-13 12:42:37.000000 twikit-1.4.8/twikit/twikit_async/tweet.py
+-rw-rw-rw-   0        0        0    14677 2024-04-13 12:42:37.000000 twikit-1.4.8/twikit/twikit_async/user.py
+-rw-rw-rw-   0        0        0     3390 2024-04-13 12:42:37.000000 twikit-1.4.8/twikit/twikit_async/utils.py
+-rw-rw-rw-   0        0        0    14454 2024-04-13 12:42:37.000000 twikit-1.4.8/twikit/user.py
+-rw-rw-rw-   0        0        0    21797 2024-04-13 12:42:37.000000 twikit-1.4.8/twikit/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-13 14:30:21.490088 twikit-1.4.8/twikit.egg-info/
+-rw-rw-rw-   0        0        0     3863 2024-04-13 14:30:21.000000 twikit-1.4.8/twikit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      737 2024-04-13 14:30:21.000000 twikit-1.4.8/twikit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 14:30:21.000000 twikit-1.4.8/twikit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-13 14:30:21.000000 twikit-1.4.8/twikit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-13 14:30:21.000000 twikit-1.4.8/twikit.egg-info/top_level.txt
```

### Comparing `twikit-1.4.7/LICENSE` & `twikit-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `twikit-1.4.7/PKG-INFO` & `twikit-1.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.4.7
+Version: 1.4.8
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.4.7/README.md` & `twikit-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `twikit-1.4.7/setup.py` & `twikit-1.4.8/setup.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.7/twikit/client.py` & `twikit-1.4.8/twikit/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import io
 import json
 import time
+import warnings
 from functools import partial
 from typing import Literal
 
 import filetype
 from fake_useragent import UserAgent
 from httpx import Response
 
@@ -55,18 +56,21 @@
     >>> client.login(
     ...     auth_info_1='example_user',
     ...     auth_info_2='email@example.com',
     ...     password='00000000'
     ... )
     """
 
-    def __init__(self, language: str | None = None, **kwargs) -> None:
+    def __init__(
+        self, language: str | None = None,
+        proxies: dict | None = None, **kwargs
+    ) -> None:
         self._token = TOKEN
         self.language = language
-        self.http = HTTPClient(**kwargs)
+        self.http = HTTPClient(proxies=proxies, **kwargs)
         self._user_id = None
         self._user_agent = UserAgent().random.strip()
         self._act_as = None
 
     def _get_guest_token(self) -> str:
         headers = self._base_headers
         headers.pop('X-Twitter-Active-User')
@@ -2358,15 +2362,16 @@
         return response
 
     def get_trends(
         self,
         category: Literal[
             'trending', 'for-you', 'news', 'sports', 'entertainment'
         ],
-        count: int = 20
+        count: int = 20,
+        retry: bool = True
     ) -> list[Trend]:
         """
         Retrieves trending topics on Twitter.
 
         Parameters
         ----------
         category : {'trending', 'for-you', 'news', 'sports', 'entertainment'}
@@ -2374,14 +2379,16 @@
             - 'trending': General trending topics.
             - 'for-you': Trends personalized for the user.
             - 'news': News-related trends.
             - 'sports': Sports-related trends.
             - 'entertainment': Entertainment-related trends.
         count : :class:`int`, default=20
             The number of trends to retrieve.
+        retry : :class:`bool`, default=True
+            If no trends are fetched continuously retry to fetch trends.
 
         Returns
         -------
         list[:class:`Trend`]
             A list of Trend objects representing the retrieved trends.
 
         Examples
@@ -2410,17 +2417,19 @@
         entry_id_prefix = 'trends' if category == 'trending' else 'Guide'
         entries = [
             i for i in find_dict(response, 'entries')[0]
             if i['entryId'].startswith(entry_id_prefix)
         ]
 
         if not entries:
+            if not retry:
+                return []
             # Recall the method again, as the trend information
             # may not be returned due to a Twitter error.
-            return self.get_trends(category, count)
+            return self.get_trends(category, count, retry)
 
         items = entries[-1]['content']['timelineModule']['items']
 
         results = []
         for item in items:
             trend_info = item['item']['content']['trend']
             results.append(Trend(self, trend_info))
@@ -2455,16 +2464,23 @@
         ).json()
 
         items = find_dict(response, 'entries')[0]
         results = []
         for item in items:
             entry_id = item['entryId']
             if entry_id.startswith('user'):
-                user_info = find_dict(item, 'result')[0]
-                results.append(User(self, user_info))
+                user_info = find_dict(item, 'result')
+                if not user_info:
+                    warnings.warn(
+                        'Some followers are excluded because '
+                        '"Quality Filter" is enabled. To get all followers, '
+                        'turn this off this in the Twitter settings.'
+                    )
+                    continue
+                results.append(User(self, user_info[0]))
             elif entry_id.startswith('cursor-bottom'):
                 next_cursor = item['content']['value']
 
         return Result(
             results,
             partial(self._get_user_friendship,
                     user_id, count, endpoint, next_cursor),
```

### Comparing `twikit-1.4.7/twikit/errors.py` & `twikit-1.4.8/twikit/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.7/twikit/group.py` & `twikit-1.4.8/twikit/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.7/twikit/http.py` & `twikit-1.4.8/twikit/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.7/twikit/list.py` & `twikit-1.4.8/twikit/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.7/twikit/message.py` & `twikit-1.4.8/twikit/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.7/twikit/notification.py` & `twikit-1.4.8/twikit/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.7/twikit/trend.py` & `twikit-1.4.8/twikit/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.7/twikit/tweet.py` & `twikit-1.4.8/twikit/tweet.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.7/twikit/twikit_async/client.py` & `twikit-1.4.8/twikit/twikit_async/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import asyncio
 import io
 import json
+import warnings
 from functools import partial
 from typing import Literal
 
 import filetype
 from fake_useragent import UserAgent
 from httpx import Response
 
@@ -56,18 +57,21 @@
     >>> await client.login(
     ...     auth_info_1='example_user',
     ...     auth_info_2='email@example.com',
     ...     password='00000000'
     ... )
     """
 
-    def __init__(self, language: str | None = None, **kwargs) -> None:
+    def __init__(
+        self, language: str | None = None,
+        proxies: dict | None = None, **kwargs
+    ) -> None:
         self._token = TOKEN
         self.language = language
-        self.http = HTTPClient(**kwargs)
+        self.http = HTTPClient(proxies=proxies, **kwargs)
         self._user_id = None
         self._user_agent = UserAgent().random.strip()
         self._act_as = None
 
     async def _get_guest_token(self) -> str:
         headers = self._base_headers
         headers.pop('X-Twitter-Active-User')
@@ -2376,15 +2380,16 @@
         return response
 
     async def get_trends(
         self,
         category: Literal[
             'trending', 'for-you', 'news', 'sports', 'entertainment'
         ],
-        count: int = 20
+        count: int = 20,
+        retry: bool = True
     ) -> list[Trend]:
         """
         Retrieves trending topics on Twitter.
 
         Parameters
         ----------
         category : {'trending', 'for-you', 'news', 'sports', 'entertainment'}
@@ -2392,14 +2397,16 @@
             - 'trending': General trending topics.
             - 'for-you': Trends personalized for the user.
             - 'news': News-related trends.
             - 'sports': Sports-related trends.
             - 'entertainment': Entertainment-related trends.
         count : :class:`int`, default=20
             The number of trends to retrieve.
+        retry : :class:`bool`, default=True
+            If no trends are fetched continuously retry to fetch trends.
 
         Returns
         -------
         list[:class:`Trend`]
             A list of Trend objects representing the retrieved trends.
 
         Examples
@@ -2428,17 +2435,19 @@
         entry_id_prefix = 'trends' if category == 'trending' else 'Guide'
         entries = [
             i for i in find_dict(response, 'entries')[0]
             if i['entryId'].startswith(entry_id_prefix)
         ]
 
         if not entries:
+            if not retry:
+                return []
             # Recall the method again, as the trend information
             # may not be returned due to a Twitter error.
-            return await self.get_trends(category, count)
+            return await self.get_trends(category, count, retry)
 
         items = entries[-1]['content']['timelineModule']['items']
 
         results = []
         for item in items:
             trend_info = item['item']['content']['trend']
             results.append(Trend(self, trend_info))
@@ -2473,16 +2482,22 @@
         )).json()
 
         items = find_dict(response, 'entries')[0]
         results = []
         for item in items:
             entry_id = item['entryId']
             if entry_id.startswith('user'):
-                user_info = find_dict(item, 'result')[0]
-                results.append(User(self, user_info))
+                user_info = find_dict(item, 'result')
+                if not user_info:
+                    warnings.warn(
+                        'Some followers are excluded because '
+                        '"Quality Filter" is enabled. To get all followers, '
+                        'turn this off this in the Twitter settings.'
+                    )
+                    continue
             elif entry_id.startswith('cursor-bottom'):
                 next_cursor = item['content']['value']
 
         return Result(
             results,
             partial(self._get_user_friendship,
                     user_id, count, endpoint, next_cursor),
```

### Comparing `twikit-1.4.7/twikit/twikit_async/errors.py` & `twikit-1.4.8/twikit/twikit_async/errors.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.7/twikit/twikit_async/group.py` & `twikit-1.4.8/twikit/twikit_async/group.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.7/twikit/twikit_async/http.py` & `twikit-1.4.8/twikit/twikit_async/http.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.7/twikit/twikit_async/list.py` & `twikit-1.4.8/twikit/twikit_async/list.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.7/twikit/twikit_async/message.py` & `twikit-1.4.8/twikit/twikit_async/message.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.7/twikit/twikit_async/notification.py` & `twikit-1.4.8/twikit/twikit_async/notification.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.7/twikit/twikit_async/trend.py` & `twikit-1.4.8/twikit/twikit_async/trend.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.7/twikit/twikit_async/tweet.py` & `twikit-1.4.8/twikit/twikit_async/tweet.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.7/twikit/twikit_async/user.py` & `twikit-1.4.8/twikit/twikit_async/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.7/twikit/twikit_async/utils.py` & `twikit-1.4.8/twikit/twikit_async/utils.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.7/twikit/user.py` & `twikit-1.4.8/twikit/user.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.7/twikit/utils.py` & `twikit-1.4.8/twikit/utils.py`

 * *Files identical despite different names*

### Comparing `twikit-1.4.7/twikit.egg-info/PKG-INFO` & `twikit-1.4.8/twikit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twikit
-Version: 1.4.7
+Version: 1.4.8
 Summary: Twitter API wrapper for python with **no API key required**.
 Home-page: https://github.com/d60/twikit
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `twikit-1.4.7/twikit.egg-info/SOURCES.txt` & `twikit-1.4.8/twikit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

