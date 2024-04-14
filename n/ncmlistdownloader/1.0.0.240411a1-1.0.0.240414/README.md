# Comparing `tmp/ncmlistdownloader-1.0.0.240411a1.tar.gz` & `tmp/ncmlistdownloader-1.0.0.240414.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncmlistdownloader-1.0.0.240411a1.tar", last modified: Thu Apr 11 14:57:45 2024, max compression
+gzip compressed data, was "ncmlistdownloader-1.0.0.240414.tar", last modified: Sun Apr 14 14:46:02 2024, max compression
```

## Comparing `ncmlistdownloader-1.0.0.240411a1.tar` & `ncmlistdownloader-1.0.0.240414.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 14:57:45.419854 ncmlistdownloader-1.0.0.240411a1/
--rw-rw-rw-   0        0        0    35181 2024-03-07 09:37:50.000000 ncmlistdownloader-1.0.0.240411a1/LICENSE
--rw-rw-rw-   0        0        0     1424 2024-04-11 14:57:45.419854 ncmlistdownloader-1.0.0.240411a1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-11 14:57:45.357376 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/
--rw-rw-rw-   0        0        0     1264 2024-04-08 14:52:37.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 14:57:45.372996 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/cmd/
--rw-rw-rw-   0        0        0     2700 2024-04-11 14:57:18.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/cmd/__init__.py
--rw-rw-rw-   0        0        0     1182 2024-04-11 14:57:22.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/cmd/module.py
-drwxrwxrwx   0        0        0        0 2024-04-11 14:57:45.388612 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/common/
--rw-rw-rw-   0        0        0     2859 2024-04-10 14:43:02.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/common/__init__.py
--rw-rw-rw-   0        0        0     2325 2024-04-10 09:59:47.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/common/encode_sec_key.py
--rw-rw-rw-   0        0        0     2213 2024-04-10 10:20:01.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/common/global_args.py
--rw-rw-rw-   0        0        0     1784 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/common/thread_test.py
-drwxrwxrwx   0        0        0        0 2024-04-11 14:57:45.404472 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/downloader/
--rw-rw-rw-   0        0        0     6526 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/downloader/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 14:57:45.404472 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/editer/
--rw-rw-rw-   0        0        0     3929 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/editer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 14:57:45.404472 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/playlist/
--rw-rw-rw-   0        0        0     1814 2024-04-11 14:57:28.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/playlist/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 14:57:45.404472 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/song/
--rw-rw-rw-   0        0        0     7424 2024-04-10 10:20:08.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/song/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 14:57:45.419854 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader.egg-info/
--rw-rw-rw-   0        0        0     1424 2024-04-11 14:57:45.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      672 2024-04-11 14:57:45.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 14:57:45.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-11 14:57:45.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       46 2024-04-11 14:57:45.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-11 14:57:45.000000 ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 14:57:45.419854 ncmlistdownloader-1.0.0.240411a1/setup.cfg
--rw-rw-rw-   0        0        0     1711 2024-04-11 14:56:54.000000 ncmlistdownloader-1.0.0.240411a1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 14:46:02.837665 ncmlistdownloader-1.0.0.240414/
+-rw-rw-rw-   0        0        0    35181 2024-03-07 09:37:50.000000 ncmlistdownloader-1.0.0.240414/LICENSE
+-rw-rw-rw-   0        0        0     1409 2024-04-14 14:46:02.822032 ncmlistdownloader-1.0.0.240414/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-14 14:46:02.784289 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/
+-rw-rw-rw-   0        0        0     1263 2024-04-14 14:42:21.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 14:46:02.799906 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/cmd/
+-rw-rw-rw-   0        0        0        0 2024-04-13 04:27:21.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/cmd/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-13 04:27:37.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/cmd/module.py
+drwxrwxrwx   0        0        0        0 2024-04-14 14:46:02.822032 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/common/
+-rw-rw-rw-   0        0        0     2859 2024-04-10 14:43:02.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/common/__init__.py
+-rw-rw-rw-   0        0        0     2325 2024-04-14 14:36:25.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/common/encode_sec_key.py
+-rw-rw-rw-   0        0        0     2184 2024-04-14 14:42:02.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/common/global_args.py
+-rw-rw-rw-   0        0        0     1784 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/common/thread_test.py
+drwxrwxrwx   0        0        0        0 2024-04-14 14:46:02.822032 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/downloader/
+-rw-rw-rw-   0        0        0     6526 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/downloader/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 14:46:02.822032 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/editer/
+-rw-rw-rw-   0        0        0     3929 2024-04-06 14:26:30.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/editer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 14:46:02.822032 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/playlist/
+-rw-rw-rw-   0        0        0     1956 2024-04-14 14:42:29.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/playlist/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 14:46:02.822032 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/song/
+-rw-rw-rw-   0        0        0     7481 2024-04-12 15:08:55.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader/song/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 14:46:02.822032 ncmlistdownloader-1.0.0.240414/ncmlistdownloader.egg-info/
+-rw-rw-rw-   0        0        0     1409 2024-04-14 14:46:02.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      672 2024-04-14 14:46:02.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 14:46:02.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-14 14:46:02.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       37 2024-04-14 14:46:02.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-14 14:46:02.000000 ncmlistdownloader-1.0.0.240414/ncmlistdownloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 14:46:02.837665 ncmlistdownloader-1.0.0.240414/setup.cfg
+-rw-rw-rw-   0        0        0     1756 2024-04-14 14:39:59.000000 ncmlistdownloader-1.0.0.240414/setup.py
```

### Comparing `ncmlistdownloader-1.0.0.240411a1/LICENSE` & `ncmlistdownloader-1.0.0.240414/LICENSE`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240411a1/PKG-INFO` & `ncmlistdownloader-1.0.0.240414/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.0.240411a1
+Version: 1.0.0.240414
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Graphics
@@ -25,8 +25,7 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
 Requires-Dist: pycryptodome
 Requires-Dist: pillow
 Requires-Dist: mutagen
 Requires-Dist: requests
-Requires-Dist: keyboard
```

### Comparing `ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/__init__.py` & `ncmlistdownloader-1.0.0.240414/ncmlistdownloader/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 '''
 ncmlistdownloader/__init__.py
-Core.Ver.1.0.0.240408a1
+Core.Ver.1.0.0.240414
 Author: CooooldWind_
 '''
 from pathlib import Path
 from ncmlistdownloader.playlist import *
 from ncmlistdownloader.common import *
 from ncmlistdownloader.common.global_args import *
 
 def main():
     for i in CMD_START_WORDS:
         print(i)
-    print('Core.Ver.1.0.0.240408a1')
+    print('[*]Core.Ver.1.0.0.240414')
     id = str(input("ID: "))
     p = Playlist(id)
     p.get_info()
     p.get_detail_info()
     print("Playlist info-reading succeed.")
     d = str(input("Dir: "))
     if d == '':
```

### Comparing `ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/common/__init__.py` & `ncmlistdownloader-1.0.0.240414/ncmlistdownloader/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/common/encode_sec_key.py` & `ncmlistdownloader-1.0.0.240414/ncmlistdownloader/common/encode_sec_key.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/common/global_args.py` & `ncmlistdownloader-1.0.0.240414/ncmlistdownloader/common/global_args.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,14 +38,13 @@
 PLAYLIST_API = json_file['PLAYLIST_API']
 SONG_INFO_API = json_file['SONG_INFO_API']
 SONG_FILE_API = json_file['SONG_FILE_API']
 SONG_FILE_API_2 = json_file['SONG_FILE_API_2']
 SEARCH_API = "https://music.163.com/weapi/cloudsearch/get/web?csrf_token="
 LYRIC_API = json_file['LYRIC_API']
 CMD_START_WORDS = [
-    "163ListDownloader CMD Ver.",
+    "163ListDownloader CMD Ver - Ver.1.0.0.240414",
     "Made by CooooldWind_",
-    "Warning: It's an Alpha Version. It may has a lot of bugs.",
-    "If you met them, click the links below:",
+    "Here's the Gitee/GitHub Page, click a star if you like it~",
     "Gitee: https://gitee.com/CooooldWind/163ListDownloader_NexT/issues",
     "GitHub: https://github.com/CooooldWind/163ListDownloader_NexT/issues",
 ]
```

### Comparing `ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/common/thread_test.py` & `ncmlistdownloader-1.0.0.240414/ncmlistdownloader/common/thread_test.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/downloader/__init__.py` & `ncmlistdownloader-1.0.0.240414/ncmlistdownloader/downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/editer/__init__.py` & `ncmlistdownloader-1.0.0.240414/ncmlistdownloader/editer/__init__.py`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/playlist/__init__.py` & `ncmlistdownloader-1.0.0.240414/ncmlistdownloader/playlist/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 ncmlistdownloader/playlist/__init__.py
-Core.Ver.1.0.0.240411a1
+Core.Ver.1.0.0.240414
 Author: CooooldWind_
 '''
 from ncmlistdownloader.common import *
 from ncmlistdownloader.common.encode_sec_key import *
 from ncmlistdownloader.common.global_args import *
 from ncmlistdownloader.song import *
 import threading
@@ -18,20 +18,20 @@
         self.creator_id = ""
         self.raw_info = {}
         self.track_count = int(0)
         self.creator = ""
         self.track_id = []
         self.title = ""
 
-    def get_info(self):
+    def get_info(self, cookies = None):
         self.raw_info = NeteaseParams(url = PLAYLIST_API,
                                       encode_data = {
                                           'csrf_token': '',
                                           'id': self.id,
-                                      }).get_resource()['playlist']
+                                      }).get_resource(cookies = cookies)['playlist']
         self.creator_id = self.raw_info['userId']
         self.track_count = self.raw_info['trackCount']
         self.creator = self.raw_info['creator']['nickname']
         self.title = self.raw_info['name']
         for i in self.raw_info['trackIds']:
             self.track_id.append(str(i['id']))
         for truck_id in self.track_id:
@@ -40,13 +40,18 @@
     
     def get_detail_info(self):
         threads: list[threading.Thread] = []
         for i in self.track:
             thread = threading.Thread(target = i.multi_get_info)
             thread.start()
             threads.append(thread)
-        for i in threads:
-            i.join()
 
     def auto_get_info(self):
         self.get_info()
-        self.get_detail_info()
+        self.get_detail_info()
+
+    def done_sum(self):
+        count = 0
+        for i in self.track:
+            if i.is_get == True:
+                count += 1
+        return count
```

### Comparing `ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader/song/__init__.py` & `ncmlistdownloader-1.0.0.240414/ncmlistdownloader/song/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 '''
 ncmlistdownloader/song/__init__.py
-Core.Ver.1.0.0.240410a1
+Core.Ver.1.0.0.240412a2
 Author: CooooldWind_
 '''
 
 from ncmlistdownloader.common import *
 from ncmlistdownloader.common.encode_sec_key import *
 from ncmlistdownloader.common.thread_test import best_thread
 from ncmlistdownloader.downloader import *
@@ -46,14 +46,15 @@
             'tv': -1,
         }
         self.raw_info = {}
         self.processed_info = {}
         self.url_info = {}
         self.filename_info = {}
         self.filename_format = '$title$ - $artist$'
+        self.is_get = False
 
     def __str__(self):
         '''
         返回存有歌曲信息的字符串。
         ----------
         无参数。
         如果直接`print`这个类就是调用这个函数了。
@@ -101,14 +102,15 @@
             'song_file': SONG_FILE_API + self.id,
         })
         self.filename_info.update({
             'song': self.get_formated_filename('mp3'),
             'pic': self.get_formated_filename('jpg'),
             'lyric': self.get_formated_filename('lrc'),
         })
+        self.is_get = True
         return self.raw_info
     
     def multi_get_info(self):
         '''
         获取歌曲信息（多线程用）
         ----------
         无参数。
```

### Comparing `ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader.egg-info/PKG-INFO` & `ncmlistdownloader-1.0.0.240414/ncmlistdownloader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: ncmlistdownloader
-Version: 1.0.0.240411a1
+Version: 1.0.0.240414
 Summary: 获取网易云音乐歌单数据，下载音乐，主动添加元信息。
 Home-page: https://gitee.com/Cooooldwind/163ListDownloader_NexT
 Author: CooooldWind_
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Internet
 Classifier: Topic :: Multimedia
 Classifier: Topic :: Multimedia :: Graphics
@@ -25,8 +25,7 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 License-File: LICENSE
 Requires-Dist: pycryptodome
 Requires-Dist: pillow
 Requires-Dist: mutagen
 Requires-Dist: requests
-Requires-Dist: keyboard
```

### Comparing `ncmlistdownloader-1.0.0.240411a1/ncmlistdownloader.egg-info/SOURCES.txt` & `ncmlistdownloader-1.0.0.240414/ncmlistdownloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ncmlistdownloader-1.0.0.240411a1/setup.py` & `ncmlistdownloader-1.0.0.240414/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from setuptools import setup, find_packages
 setup(
     classifiers = [
         # 发展时期
-        'Development Status :: 3 - Alpha',
+        # 'Development Status :: 3 - Alpha',
         # 'Development Status :: 4 - Beta',
+        'Development Status :: 5 - Production/Stable',
         # 开发的目标用户
         'Intended Audience :: Customer Service',
         'Intended Audience :: Developers',
         'Intended Audience :: End Users/Desktop',
         # 属于什么类型
         'Topic :: Communications :: File Sharing',
         'Topic :: Internet',
@@ -25,15 +26,15 @@
 		'Programming Language :: Python :: 3.8',
 		'Programming Language :: Python :: 3.9',
 		'Programming Language :: Python :: 3.10',
 		'Programming Language :: Python :: 3.11',
 		'Programming Language :: Python :: 3.12',
     ],
     name = 'ncmlistdownloader',
-    version = "1.0.0.240411a1",
+    version = "1.0.0.240414",
     description = '获取网易云音乐歌单数据，下载音乐，主动添加元信息。',
     author = 'CooooldWind_',
     url = 'https://gitee.com/Cooooldwind/163ListDownloader_NexT',
     packages = find_packages(),
-    install_requires = ['pycryptodome','pillow','mutagen','requests','keyboard',],
+    install_requires = ['pycryptodome','pillow','mutagen','requests',],
     entry_points = {'console_scripts': ['ncmlistdownloader = ncmlistdownloader.__init__:main']},
 )
```

