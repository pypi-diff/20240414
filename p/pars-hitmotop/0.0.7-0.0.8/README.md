# Comparing `tmp/pars_hitmotop-0.0.7.tar.gz` & `tmp/pars_hitmotop-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pars_hitmotop-0.0.7.tar", last modified: Thu Mar 14 19:59:47 2024, max compression
+gzip compressed data, was "pars_hitmotop-0.0.8.tar", last modified: Sat Apr 13 22:17:35 2024, max compression
```

## Comparing `pars_hitmotop-0.0.7.tar` & `pars_hitmotop-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 19:59:47.000000 pars_hitmotop-0.0.7/
--rw-rw-rw-   0        0        0     4379 2024-03-14 19:59:47.000000 pars_hitmotop-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3320 2023-11-06 18:54:01.000000 pars_hitmotop-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-03-14 19:59:47.000000 pars_hitmotop-0.0.7/pars_hitmotop/
--rw-rw-rw-   0        0        0      180 2024-01-13 21:48:08.000000 pars_hitmotop-0.0.7/pars_hitmotop/__init__.py
--rw-rw-rw-   0        0        0     4871 2024-03-14 19:48:04.000000 pars_hitmotop-0.0.7/pars_hitmotop/entered_tracks.py
--rw-rw-rw-   0        0        0      524 2023-10-29 16:35:26.000000 pars_hitmotop-0.0.7/pars_hitmotop/excepts.py
--rw-rw-rw-   0        0        0     2084 2023-11-06 19:43:20.000000 pars_hitmotop-0.0.7/pars_hitmotop/how_to_use.py
--rw-rw-rw-   0        0        0     4296 2024-03-14 19:39:29.000000 pars_hitmotop-0.0.7/pars_hitmotop/rating_tracks_count.py
--rw-rw-rw-   0        0        0     6840 2024-03-14 19:44:32.000000 pars_hitmotop-0.0.7/pars_hitmotop/rating_tracks_page.py
-drwxrwxrwx   0        0        0        0 2024-03-14 19:59:47.000000 pars_hitmotop-0.0.7/pars_hitmotop.egg-info/
--rw-rw-rw-   0        0        0     4379 2024-03-14 19:59:46.000000 pars_hitmotop-0.0.7/pars_hitmotop.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2024-03-14 19:59:47.000000 pars_hitmotop-0.0.7/pars_hitmotop.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 19:59:46.000000 pars_hitmotop-0.0.7/pars_hitmotop.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-03-14 19:59:46.000000 pars_hitmotop-0.0.7/pars_hitmotop.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-14 19:59:46.000000 pars_hitmotop-0.0.7/pars_hitmotop.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-14 19:59:47.000000 pars_hitmotop-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      893 2024-03-14 19:57:35.000000 pars_hitmotop-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 22:17:35.539700 pars_hitmotop-0.0.8/
+-rw-rw-rw-   0        0        0     3911 2024-04-13 22:17:35.540698 pars_hitmotop-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3320 2023-11-06 18:54:01.000000 pars_hitmotop-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-13 22:17:35.506694 pars_hitmotop-0.0.8/pars_hitmotop/
+-rw-rw-rw-   0        0        0      180 2024-04-13 22:12:46.000000 pars_hitmotop-0.0.8/pars_hitmotop/__init__.py
+-rw-rw-rw-   0        0        0     4873 2024-04-13 22:13:39.000000 pars_hitmotop-0.0.8/pars_hitmotop/entered_tracks.py
+-rw-rw-rw-   0        0        0      524 2024-04-13 22:12:46.000000 pars_hitmotop-0.0.8/pars_hitmotop/excepts.py
+-rw-rw-rw-   0        0        0     2084 2024-04-13 22:12:46.000000 pars_hitmotop-0.0.8/pars_hitmotop/how_to_use.py
+-rw-rw-rw-   0        0        0     4296 2024-04-13 22:12:46.000000 pars_hitmotop-0.0.8/pars_hitmotop/rating_tracks_count.py
+-rw-rw-rw-   0        0        0     6840 2024-04-13 22:12:46.000000 pars_hitmotop-0.0.8/pars_hitmotop/rating_tracks_page.py
+drwxrwxrwx   0        0        0        0 2024-04-13 22:17:35.534696 pars_hitmotop-0.0.8/pars_hitmotop.egg-info/
+-rw-rw-rw-   0        0        0     3911 2024-04-13 22:17:35.000000 pars_hitmotop-0.0.8/pars_hitmotop.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2024-04-13 22:17:35.000000 pars_hitmotop-0.0.8/pars_hitmotop.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 22:17:35.000000 pars_hitmotop-0.0.8/pars_hitmotop.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-04-13 22:17:35.000000 pars_hitmotop-0.0.8/pars_hitmotop.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-13 22:17:35.000000 pars_hitmotop-0.0.8/pars_hitmotop.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-13 22:17:35.543697 pars_hitmotop-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      893 2024-04-13 22:17:05.000000 pars_hitmotop-0.0.8/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pars_hitmotop-0.0.7/PKG-INFO` & `pars_hitmotop-0.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,67 +1,64 @@
 Metadata-Version: 2.1
 Name: pars_hitmotop
-Version: 0.0.7
-Summary: UNKNOWN
+Version: 0.0.8
 Home-page: https://github.com/PY079/pars_hitmotop
+Download-URL: https://github.com/PY079/pars_hitmotop/arhive/v0.0.8.zip
 Author: Joy_079
 Author-email: Prufu@yandex.ru
-License: UNKNOWN
-Download-URL: https://github.com/PY079/pars_hitmotop/arhive/v0.0.7.zip
-Description: # Оглавление
-        0. [Оглавление](https://github.com/PY079/pars_hitmotop#оглавление)
-        1. [Что именно парсит?](https://github.com/PY079/pars_hitmotop/blob/main/README.md#что-именно-парсит)
-        2. [Как использовать модуль entered_tracks](https://github.com/PY079/pars_hitmotop/blob/main/README.md#как-использовать-модуль-entered_tracks)
-        3. [Как использовать модуль rating_tracks_count](https://github.com/PY079/pars_hitmotop/blob/main/README.md#как-использовать-модуль-rating_tracks_count)
-        4. [Как использовать модуль rating_tracks_page](https://github.com/PY079/pars_hitmotop/blob/main/README.md#как-использовать-модуль-rating_tracks_page)
-        5. [Что можно достать при запросе?](https://github.com/PY079/pars_hitmotop/blob/main/README.md#что-можно-достать-при-запросе)
-        ____
-        Этот проект парсит [музыкальный сайт](https://rur.hitmotop.com/)
-        ____
-        # Что именно парсит?
-        1. [Рейтинговые треки](https://rur.hitmotop.com/songs/top-rated) от 1 до 48;
-        2. Тоже [рейтиновые треки](https://rur.hitmotop.com/songs/top-rated) но можно выбрать количество страниц, с которых будет произведен парсинг;
-        3. Треки введеные пользователем. Парсит от 1 трека до конечной страницы (на одной старнице 48 треков)
-        ____
-        ## Как использовать модуль *entered_tracks*
-        ```
-        from pars_hitmotop.entered_tracks import EnteredTrack
-        result=EnteredTrack('linkin park',10)
-        ```
-        1 аргументом (musci_name) передается название пенси или автора. 2 Аргументом (count) передается количество треков
-        ____
-        ## Как использовать модуль *rating_tracks_count*
-        ```
-        from pars_hitmotop.rating_tracks_count import RatingCount
-        result=RatingCount(10)
-        ```
-        1 аргументом (count) передается количество песен
-        ____
-        ## Как использовать модуль *rating_tracks_page*
-        ```
-        from pars_hitmotop.rating_tracks_page import RatingPage
-        result=RatingPage(10)
-        ```
-        1 аргументом (count) передается количество страниц (max 11)
-        ____
-        # Что можно достать при запросе?
-        Все вовзращается в виде list
-        | Метод | Описание |
-        |----------------|:---------|
-        | result.get_author | Получить автора трека|
-        |result.get_title| Получить название трека|
-        |result.get_url_down|Получить ссылку на скачивание трека|
-        |result.direct_download_link|Получть пряму ссылку на скачивание трека|
-        |result.get_duraction|Получить продолжительность трека|
-        |result.get_picture_url|Получить ссылку на обложку трека|
-        |result.get_url_track|Получить ссылку трек|
-        |result.get_all|Получить все данные в виде словаря|
-        
-        ____
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/markdown
+
+# Оглавление
+0. [Оглавление](https://github.com/PY079/pars_hitmotop#оглавление)
+1. [Что именно парсит?](https://github.com/PY079/pars_hitmotop/blob/main/README.md#что-именно-парсит)
+2. [Как использовать модуль entered_tracks](https://github.com/PY079/pars_hitmotop/blob/main/README.md#как-использовать-модуль-entered_tracks)
+3. [Как использовать модуль rating_tracks_count](https://github.com/PY079/pars_hitmotop/blob/main/README.md#как-использовать-модуль-rating_tracks_count)
+4. [Как использовать модуль rating_tracks_page](https://github.com/PY079/pars_hitmotop/blob/main/README.md#как-использовать-модуль-rating_tracks_page)
+5. [Что можно достать при запросе?](https://github.com/PY079/pars_hitmotop/blob/main/README.md#что-можно-достать-при-запросе)
+____
+Этот проект парсит [музыкальный сайт](https://rur.hitmotop.com/)
+____
+# Что именно парсит?
+1. [Рейтинговые треки](https://rur.hitmotop.com/songs/top-rated) от 1 до 48;
+2. Тоже [рейтиновые треки](https://rur.hitmotop.com/songs/top-rated) но можно выбрать количество страниц, с которых будет произведен парсинг;
+3. Треки введеные пользователем. Парсит от 1 трека до конечной страницы (на одной старнице 48 треков)
+____
+## Как использовать модуль *entered_tracks*
+```
+from pars_hitmotop.entered_tracks import EnteredTrack
+result=EnteredTrack('linkin park',10)
+```
+1 аргументом (musci_name) передается название пенси или автора. 2 Аргументом (count) передается количество треков
+____
+## Как использовать модуль *rating_tracks_count*
+```
+from pars_hitmotop.rating_tracks_count import RatingCount
+result=RatingCount(10)
+```
+1 аргументом (count) передается количество песен
+____
+## Как использовать модуль *rating_tracks_page*
+```
+from pars_hitmotop.rating_tracks_page import RatingPage
+result=RatingPage(10)
+```
+1 аргументом (count) передается количество страниц (max 11)
+____
+# Что можно достать при запросе?
+Все вовзращается в виде list
+| Метод | Описание |
+|----------------|:---------|
+| result.get_author | Получить автора трека|
+|result.get_title| Получить название трека|
+|result.get_url_down|Получить ссылку на скачивание трека|
+|result.direct_download_link|Получть пряму ссылку на скачивание трека|
+|result.get_duraction|Получить продолжительность трека|
+|result.get_picture_url|Получить ссылку на обложку трека|
+|result.get_url_track|Получить ссылку трек|
+|result.get_all|Получить все данные в виде словаря|
+
+____
```

### Comparing `pars_hitmotop-0.0.7/README.md` & `pars_hitmotop-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pars_hitmotop-0.0.7/pars_hitmotop/entered_tracks.py` & `pars_hitmotop-0.0.8/pars_hitmotop/entered_tracks.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
             # получаем информацию о треках
             _track_titles = [i.text.strip() for i in _soup.find_all("div", class_="track__title")]
             _track_artists = [i.text.strip() for i in _soup.find_all("div", class_="track__desc")]
             _track_duration = [i.text.strip() for i in _soup.find_all("div", class_="track__fulltime")]
             _track_pictures = [f"{i.get('style')[23:-3]}" for i in _soup.find_all("div", class_="track__img")]
             _track_urls_dow = [i.get('href') for i in _soup.find_all('a', class_='track__download-btn')]
-            _track_url = [f"{_url}{tra_url.get('href')}" for tra_url in _soup.find_all('a', class_='track__info-l')]
+            _track_url = [f"{__url1}{tra_url.get('href')}" for tra_url in _soup.find_all('a', class_='track__info-l')]
 
             _items = []
             for idx in range(min(len(_track_titles), self.amount)):
                 if self.get_redirect_url and len(_track_urls_dow[idx])>0:
                     direct_download_link = requests.get(_track_urls_dow[idx],headers=__headers,allow_redirects=True).url
                     print(f'Получил прямую ссылку: {direct_download_link}')
                 else: direct_download_link = None
```

### Comparing `pars_hitmotop-0.0.7/pars_hitmotop/excepts.py` & `pars_hitmotop-0.0.8/pars_hitmotop/excepts.py`

 * *Files identical despite different names*

### Comparing `pars_hitmotop-0.0.7/pars_hitmotop/how_to_use.py` & `pars_hitmotop-0.0.8/pars_hitmotop/how_to_use.py`

 * *Files identical despite different names*

### Comparing `pars_hitmotop-0.0.7/pars_hitmotop/rating_tracks_count.py` & `pars_hitmotop-0.0.8/pars_hitmotop/rating_tracks_count.py`

 * *Files identical despite different names*

### Comparing `pars_hitmotop-0.0.7/pars_hitmotop/rating_tracks_page.py` & `pars_hitmotop-0.0.8/pars_hitmotop/rating_tracks_page.py`

 * *Files identical despite different names*

### Comparing `pars_hitmotop-0.0.7/pars_hitmotop.egg-info/PKG-INFO` & `pars_hitmotop-0.0.8/pars_hitmotop.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,67 +1,64 @@
 Metadata-Version: 2.1
 Name: pars-hitmotop
-Version: 0.0.7
-Summary: UNKNOWN
+Version: 0.0.8
 Home-page: https://github.com/PY079/pars_hitmotop
+Download-URL: https://github.com/PY079/pars_hitmotop/arhive/v0.0.8.zip
 Author: Joy_079
 Author-email: Prufu@yandex.ru
-License: UNKNOWN
-Download-URL: https://github.com/PY079/pars_hitmotop/arhive/v0.0.7.zip
-Description: # Оглавление
-        0. [Оглавление](https://github.com/PY079/pars_hitmotop#оглавление)
-        1. [Что именно парсит?](https://github.com/PY079/pars_hitmotop/blob/main/README.md#что-именно-парсит)
-        2. [Как использовать модуль entered_tracks](https://github.com/PY079/pars_hitmotop/blob/main/README.md#как-использовать-модуль-entered_tracks)
-        3. [Как использовать модуль rating_tracks_count](https://github.com/PY079/pars_hitmotop/blob/main/README.md#как-использовать-модуль-rating_tracks_count)
-        4. [Как использовать модуль rating_tracks_page](https://github.com/PY079/pars_hitmotop/blob/main/README.md#как-использовать-модуль-rating_tracks_page)
-        5. [Что можно достать при запросе?](https://github.com/PY079/pars_hitmotop/blob/main/README.md#что-можно-достать-при-запросе)
-        ____
-        Этот проект парсит [музыкальный сайт](https://rur.hitmotop.com/)
-        ____
-        # Что именно парсит?
-        1. [Рейтинговые треки](https://rur.hitmotop.com/songs/top-rated) от 1 до 48;
-        2. Тоже [рейтиновые треки](https://rur.hitmotop.com/songs/top-rated) но можно выбрать количество страниц, с которых будет произведен парсинг;
-        3. Треки введеные пользователем. Парсит от 1 трека до конечной страницы (на одной старнице 48 треков)
-        ____
-        ## Как использовать модуль *entered_tracks*
-        ```
-        from pars_hitmotop.entered_tracks import EnteredTrack
-        result=EnteredTrack('linkin park',10)
-        ```
-        1 аргументом (musci_name) передается название пенси или автора. 2 Аргументом (count) передается количество треков
-        ____
-        ## Как использовать модуль *rating_tracks_count*
-        ```
-        from pars_hitmotop.rating_tracks_count import RatingCount
-        result=RatingCount(10)
-        ```
-        1 аргументом (count) передается количество песен
-        ____
-        ## Как использовать модуль *rating_tracks_page*
-        ```
-        from pars_hitmotop.rating_tracks_page import RatingPage
-        result=RatingPage(10)
-        ```
-        1 аргументом (count) передается количество страниц (max 11)
-        ____
-        # Что можно достать при запросе?
-        Все вовзращается в виде list
-        | Метод | Описание |
-        |----------------|:---------|
-        | result.get_author | Получить автора трека|
-        |result.get_title| Получить название трека|
-        |result.get_url_down|Получить ссылку на скачивание трека|
-        |result.direct_download_link|Получть пряму ссылку на скачивание трека|
-        |result.get_duraction|Получить продолжительность трека|
-        |result.get_picture_url|Получить ссылку на обложку трека|
-        |result.get_url_track|Получить ссылку трек|
-        |result.get_all|Получить все данные в виде словаря|
-        
-        ____
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/markdown
+
+# Оглавление
+0. [Оглавление](https://github.com/PY079/pars_hitmotop#оглавление)
+1. [Что именно парсит?](https://github.com/PY079/pars_hitmotop/blob/main/README.md#что-именно-парсит)
+2. [Как использовать модуль entered_tracks](https://github.com/PY079/pars_hitmotop/blob/main/README.md#как-использовать-модуль-entered_tracks)
+3. [Как использовать модуль rating_tracks_count](https://github.com/PY079/pars_hitmotop/blob/main/README.md#как-использовать-модуль-rating_tracks_count)
+4. [Как использовать модуль rating_tracks_page](https://github.com/PY079/pars_hitmotop/blob/main/README.md#как-использовать-модуль-rating_tracks_page)
+5. [Что можно достать при запросе?](https://github.com/PY079/pars_hitmotop/blob/main/README.md#что-можно-достать-при-запросе)
+____
+Этот проект парсит [музыкальный сайт](https://rur.hitmotop.com/)
+____
+# Что именно парсит?
+1. [Рейтинговые треки](https://rur.hitmotop.com/songs/top-rated) от 1 до 48;
+2. Тоже [рейтиновые треки](https://rur.hitmotop.com/songs/top-rated) но можно выбрать количество страниц, с которых будет произведен парсинг;
+3. Треки введеные пользователем. Парсит от 1 трека до конечной страницы (на одной старнице 48 треков)
+____
+## Как использовать модуль *entered_tracks*
+```
+from pars_hitmotop.entered_tracks import EnteredTrack
+result=EnteredTrack('linkin park',10)
+```
+1 аргументом (musci_name) передается название пенси или автора. 2 Аргументом (count) передается количество треков
+____
+## Как использовать модуль *rating_tracks_count*
+```
+from pars_hitmotop.rating_tracks_count import RatingCount
+result=RatingCount(10)
+```
+1 аргументом (count) передается количество песен
+____
+## Как использовать модуль *rating_tracks_page*
+```
+from pars_hitmotop.rating_tracks_page import RatingPage
+result=RatingPage(10)
+```
+1 аргументом (count) передается количество страниц (max 11)
+____
+# Что можно достать при запросе?
+Все вовзращается в виде list
+| Метод | Описание |
+|----------------|:---------|
+| result.get_author | Получить автора трека|
+|result.get_title| Получить название трека|
+|result.get_url_down|Получить ссылку на скачивание трека|
+|result.direct_download_link|Получть пряму ссылку на скачивание трека|
+|result.get_duraction|Получить продолжительность трека|
+|result.get_picture_url|Получить ссылку на обложку трека|
+|result.get_url_track|Получить ссылку трек|
+|result.get_all|Получить все данные в виде словаря|
+
+____
```

### Comparing `pars_hitmotop-0.0.7/setup.py` & `pars_hitmotop-0.0.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version='0.0.7'
+version='0.0.8'
 with open('README.md', encoding='utf-8') as f:
     long_description=f.read()
 
 setup(
     name='pars_hitmotop',
     version=version,
```

