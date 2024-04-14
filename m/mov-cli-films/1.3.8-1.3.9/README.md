# Comparing `tmp/mov-cli-films-1.3.8.tar.gz` & `tmp/mov-cli-films-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov-cli-films-1.3.8.tar", last modified: Wed Apr 10 20:40:08 2024, max compression
+gzip compressed data, was "mov-cli-films-1.3.9.tar", last modified: Thu Apr 11 05:59:59 2024, max compression
```

## Comparing `mov-cli-films-1.3.8.tar` & `mov-cli-films-1.3.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-10 20:40:08.233701 mov-cli-films-1.3.8/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 22:34:31.000000 mov-cli-films-1.3.8/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2915 2024-04-10 20:40:08.230368 mov-cli-films-1.3.8/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      569 2024-04-09 23:47:16.000000 mov-cli-films-1.3.8/README.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-10 20:40:08.227035 mov-cli-films-1.3.8/mov_cli_films/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      579 2024-04-10 20:39:52.000000 mov-cli-films-1.3.8/mov_cli_films/__init__.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-10 20:40:08.230368 mov-cli-films-1.3.8/mov_cli_films/vadapav/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-04-10 00:49:50.000000 mov-cli-films-1.3.8/mov_cli_films/vadapav/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     7060 2024-04-10 20:36:40.000000 mov-cli-films-1.3.8/mov_cli_films/vadapav/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-10 20:40:08.230368 mov-cli-films-1.3.8/mov_cli_films/vidsrcme/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-03-14 20:16:52.000000 mov-cli-films-1.3.8/mov_cli_films/vidsrcme/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4364 2024-04-10 00:48:41.000000 mov-cli-films-1.3.8/mov_cli_films/vidsrcme/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-10 20:40:08.230368 mov-cli-films-1.3.8/mov_cli_films/vidsrcto/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-03-09 16:43:29.000000 mov-cli-films-1.3.8/mov_cli_films/vidsrcto/__init__.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-10 20:40:08.230368 mov-cli-films-1.3.8/mov_cli_films/vidsrcto/ext/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-03-27 21:59:37.000000 mov-cli-films-1.3.8/mov_cli_films/vidsrcto/ext/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4019 2024-03-27 21:59:49.000000 mov-cli-films-1.3.8/mov_cli_films/vidsrcto/ext/vidplay.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4508 2024-04-10 00:47:28.000000 mov-cli-films-1.3.8/mov_cli_films/vidsrcto/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-04-10 20:40:08.230368 mov-cli-films-1.3.8/mov_cli_films.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2915 2024-04-10 20:40:08.000000 mov-cli-films-1.3.8/mov_cli_films.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      524 2024-04-10 20:40:08.000000 mov-cli-films-1.3.8/mov_cli_films.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-04-10 20:40:08.000000 mov-cli-films-1.3.8/mov_cli_films.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       88 2024-04-10 20:40:08.000000 mov-cli-films-1.3.8/mov_cli_films.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       14 2024-04-10 20:40:08.000000 mov-cli-films-1.3.8/mov_cli_films.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1326 2024-04-03 21:05:40.000000 mov-cli-films-1.3.8/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-04-10 20:40:08.233701 mov-cli-films-1.3.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-11 05:59:59.694267 mov-cli-films-1.3.9/
+-rw-rw-rw-   0        0        0     1085 2024-04-10 00:53:38.000000 mov-cli-films-1.3.9/LICENSE
+-rw-rw-rw-   0        0        0     2996 2024-04-11 05:59:59.693270 mov-cli-films-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0      601 2024-04-10 00:53:38.000000 mov-cli-films-1.3.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 05:59:59.670331 mov-cli-films-1.3.9/mov_cli_films/
+-rw-rw-rw-   0        0        0      600 2024-04-11 05:59:44.000000 mov-cli-films-1.3.9/mov_cli_films/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 05:59:59.686289 mov-cli-films-1.3.9/mov_cli_films/vadapav/
+-rw-rw-rw-   0        0        0       22 2024-04-10 00:53:38.000000 mov-cli-films-1.3.9/mov_cli_films/vadapav/__init__.py
+-rw-rw-rw-   0        0        0     7259 2024-04-11 05:13:33.000000 mov-cli-films-1.3.9/mov_cli_films/vadapav/scraper.py
+drwxrwxrwx   0        0        0        0 2024-04-11 05:59:59.688283 mov-cli-films-1.3.9/mov_cli_films/vidsrcme/
+-rw-rw-rw-   0        0        0       22 2024-04-10 00:53:38.000000 mov-cli-films-1.3.9/mov_cli_films/vidsrcme/__init__.py
+-rw-rw-rw-   0        0        0     4496 2024-04-10 00:53:38.000000 mov-cli-films-1.3.9/mov_cli_films/vidsrcme/scraper.py
+drwxrwxrwx   0        0        0        0 2024-04-11 05:59:59.689280 mov-cli-films-1.3.9/mov_cli_films/vidsrcto/
+-rw-rw-rw-   0        0        0       22 2024-04-10 00:53:38.000000 mov-cli-films-1.3.9/mov_cli_films/vidsrcto/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 05:59:59.691275 mov-cli-films-1.3.9/mov_cli_films/vidsrcto/ext/
+-rw-rw-rw-   0        0        0       22 2024-04-10 00:53:38.000000 mov-cli-films-1.3.9/mov_cli_films/vidsrcto/ext/__init__.py
+-rw-rw-rw-   0        0        0     4140 2024-04-10 00:53:38.000000 mov-cli-films-1.3.9/mov_cli_films/vidsrcto/ext/vidplay.py
+-rw-rw-rw-   0        0        0     4642 2024-04-10 00:53:38.000000 mov-cli-films-1.3.9/mov_cli_films/vidsrcto/scraper.py
+drwxrwxrwx   0        0        0        0 2024-04-11 05:59:59.692273 mov-cli-films-1.3.9/mov_cli_films.egg-info/
+-rw-rw-rw-   0        0        0     2996 2024-04-11 05:59:59.000000 mov-cli-films-1.3.9/mov_cli_films.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      524 2024-04-11 05:59:59.000000 mov-cli-films-1.3.9/mov_cli_films.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 05:59:59.000000 mov-cli-films-1.3.9/mov_cli_films.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-04-11 05:59:59.000000 mov-cli-films-1.3.9/mov_cli_films.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-11 05:59:59.000000 mov-cli-films-1.3.9/mov_cli_films.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1376 2024-04-10 00:53:38.000000 mov-cli-films-1.3.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 05:59:59.694267 mov-cli-films-1.3.9/setup.cfg
```

### Comparing `mov-cli-films-1.3.8/PKG-INFO` & `mov-cli-films-1.3.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-Metadata-Version: 2.1
-Name: mov-cli-films
-Version: 1.3.8
-Summary: A mov-cli v4 plugin for watching Films and Shows.
-Author-email: Ananas <ananas@r3tr0ananas.lol>
-License: MIT License
-        
-        Copyright (c) 2024 mov-cli
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: GitHub, https://github.com/JDALab/mov-cli-films
-Project-URL: BugTracker, https://github.com/JDALab/mov-cli-films/issues
-Keywords: amazing mov-cli plugin
-Classifier: Operating System :: Microsoft :: Windows :: Windows 11
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Operating System :: POSIX :: Linux
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: mov-cli>=4.0.3
-Provides-Extra: dev
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: build; extra == "dev"
-
-<div align="center">
-
-  # mov-cli-films 
-  <sub>A mov-cli v4 plugin for watching Films and Shows.</sub>
-
-  <img src="https://github.com/mov-cli/mov-cli-vadapav/assets/132799819/6406133d-f840-424b-a1c9-04599fadb0a7">
-
-</div>
-
-> [!NOTE]
-> Searching for maintainers
-
-## Installation
-Here's how to install and add the plugin to mov-cli.
-
-1. Install the pip package.
-```sh
-pip install mov-cli-films 
-```
-2. Then add the plugin to your mov-cli config.
-```sh
-mov-cli -e
-```
-```toml
-[mov-cli.plugins]
-films = "mov-cli-films"
-```
-
-## Usage
-```sh
-mov-cli -s films the rookie
-```
+Metadata-Version: 2.1
+Name: mov-cli-films
+Version: 1.3.9
+Summary: A mov-cli v4 plugin for watching Films and Shows.
+Author-email: Ananas <ananas@r3tr0ananas.lol>
+License: MIT License
+        
+        Copyright (c) 2024 mov-cli
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: GitHub, https://github.com/JDALab/mov-cli-films
+Project-URL: BugTracker, https://github.com/JDALab/mov-cli-films/issues
+Keywords: amazing mov-cli plugin
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: POSIX :: Linux
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: mov-cli>=4.0.3
+Provides-Extra: dev
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: build; extra == "dev"
+
+<div align="center">
+
+  # mov-cli-films 
+  <sub>A mov-cli v4 plugin for watching Films and Shows.</sub>
+
+  <img src="https://github.com/mov-cli/mov-cli-vadapav/assets/132799819/6406133d-f840-424b-a1c9-04599fadb0a7">
+
+</div>
+
+> [!NOTE]
+> Searching for maintainers
+
+## Installation
+Here's how to install and add the plugin to mov-cli.
+
+1. Install the pip package.
+```sh
+pip install mov-cli-films 
+```
+2. Then add the plugin to your mov-cli config.
+```sh
+mov-cli -e
+```
+```toml
+[mov-cli.plugins]
+films = "mov-cli-films"
+```
+
+## Usage
+```sh
+mov-cli -s films the rookie
+```
```

### Comparing `mov-cli-films-1.3.8/mov_cli_films/__init__.py` & `mov-cli-films-1.3.9/mov_cli_films/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from mov_cli.plugins import PluginHookData
-
-from .vidsrcme import *
-from .vidsrcto import *
-from .vadapav import *
-
-plugin: PluginHookData = {
-    "version": 1,
-    "package_name": "mov-cli-films", # Required for the plugin update checker.
-    "scrapers": {
-        "DEFAULT": VadapavScraper,
-        "vidsrcme": VidSrcMeScraper,
-        "vadapav": VadapavScraper,
-        "vidsrcto": VidSrcToScraper
-    } # NOTE: WE ARE IN NEED OF GOOD AND STABLE PROVIDERS 😭
-}
-
-__version__ = "1.3.8"
+from __future__ import annotations
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from mov_cli.plugins import PluginHookData
+
+from .vidsrcme import *
+from .vidsrcto import *
+from .vadapav import *
+
+plugin: PluginHookData = {
+    "version": 1,
+    "package_name": "mov-cli-films", # Required for the plugin update checker.
+    "scrapers": {
+        "DEFAULT": VadapavScraper,
+        "vidsrcme": VidSrcMeScraper,
+        "vadapav": VadapavScraper,
+        "vidsrcto": VidSrcToScraper
+    } # NOTE: WE ARE IN NEED OF GOOD AND STABLE PROVIDERS 😭
+}
+
+__version__ = "1.3.9"
```

### Comparing `mov-cli-films-1.3.8/mov_cli_films/vadapav/scraper.py` & `mov-cli-films-1.3.9/mov_cli_films/vadapav/scraper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,191 +1,191 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    from typing import Iterable, Optional
-
-    from bs4 import ResultSet, Tag
-    from mov_cli import Config
-    from mov_cli.http_client import HTTPClient
-    from mov_cli.scraper import ScraperOptionsT
-
-import re
-
-from mov_cli import utils
-from mov_cli.scraper import Scraper
-from mov_cli import Multi, Single, Metadata, MetadataType
-
-__all__ = ("VadapavScraper",)
-
-class VadapavScraper(Scraper):
-    def __init__(self, config: Config, http_client: HTTPClient, options: Optional[ScraperOptionsT] = None) -> None:
-        self.base_url = "https://vadapav.mov"
-        super().__init__(config, http_client, options)
-
-    def search(self, query: str, limit: int = 15) -> Iterable[Metadata]:
-        search_url = f"{self.base_url}/s/{query}"
-        search_html = self.http_client.get(search_url)
-        search_results_soup = self.soup(search_html)
-        # In this site, all movies are appended with its release year.
-        # So it can be used as an inexpensive way to determine the type of media
-        # movie_pattern = r".*\(\d{4}\)$"
-
-        index = 0
-
-        for search_result_item in search_results_soup.find_all("a", {"class": "directory-entry"}):
-            if index > limit:
-                break
-
-            item_url = search_result_item.get("href")
-
-            r = self.http_client.get(self.base_url + item_url)
-            item_page = self.soup(r.text)
-
-            item_directory_path: ResultSet[Tag] = item_page.find("div", {"class": "directory"}).find("div").find_all("span")
-
-            item_type = None
-            item_name = None
-            item_year = None
-
-            for dir_path in item_directory_path:
-
-                if dir_path.text.startswith(("Movies",)):
-                    item_type = MetadataType.SINGLE
-                    item_year = search_result_item.string[-5:-1]
-                    item_name = search_result_item.string[:-6]
-                    break
-
-                elif dir_path.text.startswith(("TV", "TV Shows")):
-                    item_type = MetadataType.MULTI
-                    item_name = search_result_item.string
-                    break
-
-            if item_type is None:
-                continue
-
-            index =+ 1
-
-            yield Metadata(
-                id=item_url.strip("/"),
-                title=item_name,
-                type=item_type,
-                year=item_year,
-            )
-
-    def scrape_episodes(self, metadata: Metadata):
-        seasons_html = self.http_client.get(f"{self.base_url}/{metadata.id}")
-        seasons_soup = self.soup(seasons_html)
-        season_dirs = [
-            dir
-            for dir in seasons_soup.find_all("a", {"class": "directory-entry"})
-            if "Season" in dir.string
-        ]
-        result = {}
-        for i, season in enumerate(season_dirs):
-            season_html = self.http_client.get(self.base_url + season.get("href"))
-            season_soup = self.soup(season_html)
-            episodes_entries = [
-                episode
-                for episode in season_soup.find_all("a", {"class": "file-entry"})
-                if episode.string[-4:] not in [".srt", ".txt"]
-            ]
-            result[i + 1] = len(episodes_entries)
-        return result
-
-    def extract_resolution(self, filename):
-        # Regular expression to extract resolution information
-        match = re.search(r"(\d+)p|4K", filename)
-        if match:
-            if match.group(1):  # If a numeric resolution is found (e.g., "720p")
-                return int(match.group(1))
-            else:  # If "4K" is found
-                return 2160  # Assumed resolution for 4K
-        else:
-            return 0  # Default to 0 if resolution is not found
-
-    def scrape(self, metadata: Metadata, episode: utils.EpisodeSelector) -> Multi | Single:
-
-        if metadata.type == MetadataType.MOVIE:
-            mov_dir_html = self.http_client.get(f"{self.base_url}/{metadata.id}")
-            movie_soup = self.soup(mov_dir_html)
-            mov_files = [
-                x
-                for x in movie_soup.find_all("a", {"class": "file-entry"})
-                if x.string[-4:] not in [".srt", ".txt"]
-            ]
-
-            subtitles = [
-                x
-                for x in movie_soup.find_all("a", {"class": "file-entry"})
-                if x.string[-4:] == ".srt"
-            ]
-            subtitle_url = (
-                {
-                    "en": self.base_url
-                    + (subtitles[0].get("data-href") or subtitles.get("href"))
-                }
-                if subtitles
-                else None
-            )
-
-            # Always select greatest resolution when there are multiple files
-            # Starting with a resolution that's lower than any possible resolution
-            movie_url, max_resolution = "", -1
-            for mov_file in mov_files:
-                resolution = self.extract_resolution(mov_file.string)
-                if resolution > max_resolution:
-                    max_resolution = resolution
-                    movie_url = mov_file.get("data-href") or mov_file.get("href")
-
-            series_url = self.base_url + movie_url
-
-            return Single(
-                series_url,
-                title=metadata.title,
-                referrer=self.base_url,
-                year=metadata.year,
-                subtitles=subtitle_url,
-            )
-
-        season_no = int(episode.season)
-        episode_no = int(episode.episode)
-
-        season_str = "S" + str(season_no) if season_no > 9 else "S0" + str(season_no)
-        season_dir_name = (
-            "Season " + str(season_no) if season_no > 9 else "Season 0" + str(season_no)
-        )
-        episode_str = (
-            "E" + str(episode_no) if episode_no > 9 else "E0" + str(episode_no)
-        )
-
-        series_dir_html = self.http_client.get(f"{self.base_url}/{metadata.id}")
-        series_soup = self.soup(series_dir_html)
-        season_directories = series_soup.find_all("a", {"class": "directory-entry"})[1:]
-
-        for season_dir in season_directories:
-            if season_dir.string == season_dir_name:
-                season_dir_html = self.http_client.get(
-                    self.base_url + season_dir.get("href")
-                )
-                season_soup = self.soup(season_dir_html)
-                episode_files = [
-                    file_entry
-                    for file_entry in season_soup.find_all("a", {"class": "file-entry"})
-                    if file_entry.string[-4:] != ".srt"
-                ]
-                break
-
-        for episode_file in episode_files:
-            if season_str + episode_str in episode_file.string:
-                episode_url = self.base_url + (
-                    episode_file.get("data-href") or episode_file.get("href")
-                )
-                break
-
-        return Multi(
-            episode_url,
-            title=metadata.title,
-            referrer=self.base_url,
-            episode=episode,
-            subtitles=None,
-        )
+from __future__ import annotations
+from typing import TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from typing import Iterable, Optional
+
+    from bs4 import ResultSet, Tag
+    from mov_cli import Config
+    from mov_cli.http_client import HTTPClient
+    from mov_cli.scraper import ScraperOptionsT
+
+import re
+
+from mov_cli import utils
+from mov_cli.scraper import Scraper
+from mov_cli import Multi, Single, Metadata, MetadataType
+
+__all__ = ("VadapavScraper",)
+
+class VadapavScraper(Scraper):
+    def __init__(self, config: Config, http_client: HTTPClient, options: Optional[ScraperOptionsT] = None) -> None:
+        self.base_url = "https://vadapav.mov"
+        super().__init__(config, http_client, options)
+
+    def search(self, query: str, limit: int = 15) -> Iterable[Metadata]:
+        search_url = f"{self.base_url}/s/{query}"
+        search_html = self.http_client.get(search_url)
+        search_results_soup = self.soup(search_html)
+        # In this site, all movies are appended with its release year.
+        # So it can be used as an inexpensive way to determine the type of media
+        # movie_pattern = r".*\(\d{4}\)$"
+
+        index = 0
+
+        for search_result_item in search_results_soup.find_all("a", {"class": "directory-entry"}):
+            if index > limit:
+                break
+
+            item_url = search_result_item.get("href")
+
+            r = self.http_client.get(self.base_url + item_url)
+            item_page = self.soup(r.text)
+
+            item_directory_path: ResultSet[Tag] = item_page.find("div", {"class": "directory"}).find("div").find_all("span")
+
+            item_type = None
+            item_name = None
+            item_year = None
+
+            for dir_path in item_directory_path:
+
+                if dir_path.text.startswith(("Movies",)):
+                    item_type = MetadataType.SINGLE
+                    item_year = search_result_item.string[-5:-1]
+                    item_name = search_result_item.string[:-6]
+                    break
+
+                elif dir_path.text.startswith(("TV", "TV Shows")):
+                    item_type = MetadataType.MULTI
+                    item_name = search_result_item.string
+                    break
+
+            if item_type is None:
+                continue
+
+            index =+ 1
+
+            yield Metadata(
+                id=item_url.strip("/"),
+                title=item_name,
+                type=item_type,
+                year=item_year,
+            )
+
+    def scrape_episodes(self, metadata: Metadata):
+        seasons_html = self.http_client.get(f"{self.base_url}/{metadata.id}")
+        seasons_soup = self.soup(seasons_html)
+        season_dirs = [
+            dir
+            for dir in seasons_soup.find_all("a", {"class": "directory-entry"})
+            if "Season" in dir.string
+        ]
+        result = {}
+        for i, season in enumerate(season_dirs):
+            season_html = self.http_client.get(self.base_url + season.get("href"))
+            season_soup = self.soup(season_html)
+            episodes_entries = [
+                episode
+                for episode in season_soup.find_all("a", {"class": "file-entry"})
+                if episode.string[-4:] not in [".srt", ".txt"]
+            ]
+            result[i + 1] = len(episodes_entries)
+        return result
+
+    def extract_resolution(self, filename):
+        # Regular expression to extract resolution information
+        match = re.search(r"(\d+)p|4K", filename)
+        if match:
+            if match.group(1):  # If a numeric resolution is found (e.g., "720p")
+                return int(match.group(1))
+            else:  # If "4K" is found
+                return 2160  # Assumed resolution for 4K
+        else:
+            return 0  # Default to 0 if resolution is not found
+
+    def scrape(self, metadata: Metadata, episode: utils.EpisodeSelector) -> Multi | Single:
+
+        if metadata.type == MetadataType.MOVIE:
+            mov_dir_html = self.http_client.get(f"{self.base_url}/{metadata.id}")
+            movie_soup = self.soup(mov_dir_html)
+            mov_files = [
+                x
+                for x in movie_soup.find_all("a", {"class": "file-entry"})
+                if x.string[-4:] not in [".srt", ".txt"]
+            ]
+
+            subtitles = [
+                x
+                for x in movie_soup.find_all("a", {"class": "file-entry"})
+                if x.string[-4:] == ".srt"
+            ]
+            subtitle_url = (
+                {
+                    "en": self.base_url
+                    + (subtitles[0].get("data-href") or subtitles.get("href"))
+                }
+                if subtitles
+                else None
+            )
+
+            # Always select greatest resolution when there are multiple files
+            # Starting with a resolution that's lower than any possible resolution
+            movie_url, max_resolution = "", -1
+            for mov_file in mov_files:
+                resolution = self.extract_resolution(mov_file.string)
+                if resolution > max_resolution:
+                    max_resolution = resolution
+                    movie_url = mov_file.get("data-href") or mov_file.get("href")
+
+            series_url = self.base_url + movie_url
+
+            return Single(
+                series_url,
+                title=metadata.title,
+                referrer=self.base_url,
+                year=metadata.year,
+                subtitles=subtitle_url,
+            )
+
+        season_no = int(episode.season)
+        episode_no = int(episode.episode)
+
+        season_str = "S" + str(season_no) if season_no > 9 else "S0" + str(season_no)
+        season_dir_name = (
+            "Season " + str(season_no) if season_no > 9 else "Season 0" + str(season_no)
+        )
+        episode_str = (
+            "E" + str(episode_no) if episode_no > 9 else "E0" + str(episode_no)
+        )
+
+        series_dir_html = self.http_client.get(f"{self.base_url}/{metadata.id}")
+        series_soup = self.soup(series_dir_html)
+        season_directories = series_soup.find_all("a", {"class": "directory-entry"})[1:]
+
+        for season_dir in season_directories:
+            if season_dir.string == season_dir_name:
+                season_dir_html = self.http_client.get(
+                    self.base_url + season_dir.get("href")
+                )
+                season_soup = self.soup(season_dir_html)
+                episode_files = [
+                    file_entry
+                    for file_entry in season_soup.find_all("a", {"class": "file-entry"})
+                    if file_entry.string[-4:] != ".srt"
+                ]
+                break
+
+        for episode_file in episode_files:
+            if season_str + episode_str in episode_file.string.upper():
+                episode_url = self.base_url + (
+                    episode_file.get("data-href") or episode_file.get("href")
+                )
+                break
+
+        return Multi(
+            episode_url,
+            title=metadata.title,
+            referrer=self.base_url,
+            episode=episode,
+            subtitles=None,
+        )
```

### Comparing `mov-cli-films-1.3.8/mov_cli_films/vidsrcme/scraper.py` & `mov-cli-films-1.3.9/mov_cli_films/vidsrcme/scraper.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING, Dict, Iterable
-
-if TYPE_CHECKING:
-    from typing import Dict, Literal, Optional
-
-    from mov_cli import Config
-    from httpx import Response
-    from mov_cli.http_client import HTTPClient
-    from mov_cli.scraper import ScraperOptionsT
-
-import re
-
-from mov_cli.scraper import Scraper
-from mov_cli import Multi, Single, Metadata, MetadataType
-from mov_cli.utils.scraper import TheMovieDB
-from mov_cli.utils import EpisodeSelector
-
-import base64
-
-
-__all__ = ("VidSrcMeScraper",)
-
-class VidSrcMeScraper(Scraper):
-    def __init__(self, config: Config, http_client: HTTPClient, options: Optional[ScraperOptionsT] = None) -> None:
-        self.base_url = "https://vidsrc.net"
-        self.tmdb = TheMovieDB(http_client)
-
-        self.MAX_TRIES = 10
-        super().__init__(config, http_client, options)
-
-    def search(self, query: str, limit: int = 10) -> Iterable[Metadata]:
-        for search_result in self.tmdb.search(query, limit):
-            embed_response = self.__get_embed(search_result, EpisodeSelector())
-
-            if embed_response.status_code == 404: # don't include media that isn't available on the provider.
-                continue
-
-            yield search_result
-
-    def scrape_episodes(self, metadata: Metadata) -> Dict[int, int] | Dict[None, Literal[1]]:
-        return self.tmdb.scrape_episodes(metadata)
-
-    def __deobfstr(self, hash, index):
-        result = ""
-        for i in range(0, len(hash), 2):
-            j = hash[i:i+2]
-            result += chr(int(j, 16) ^ ord(index[i // 2 % len(index)]))
-        return result
-
-    def __get_url(self, prourl: str):
-        url = None
-        
-        for _ in range(self.MAX_TRIES):
-            prorcp = self.http_client.get(prourl, headers={"Referer": "https://vidsrc.stream/"})
-
-            if prorcp.status_code == 503:
-                continue
-            
-            hls_url = re.search(r'file:"([^"]*)"', prorcp.text).group(1)
-            hls_url = re.sub(r'\/\/\S+?=', '', hls_url)[2:]     
-            hls_url = re.sub(r"\/@#@\/[^=\/]+==", "", hls_url)
-
-            hls_url = hls_url.replace('_', '/').replace('-', '+')
-
-            try:
-                hls_url = bytearray(base64.b64decode(hls_url))
-                hls_url = hls_url.decode('utf-8')
-            except UnicodeDecodeError:
-                hls_url = None
-
-            if hls_url is not None:
-                url = hls_url
-                break
-
-        return url
-
-    def __get_embed(self, metadata: Metadata, episode: EpisodeSelector) -> Response:
-        media_type = "tv" if metadata.type == MetadataType.SERIES else "movie"
-
-        url = f"{self.base_url}/embed/{media_type}/{metadata.id}"
-
-        if metadata.type == MetadataType.SERIES:
-            url += f"/{episode.season}/{episode.episode}"
-
-        return self.http_client.get(url)
-
-    def scrape(self, metadata: Metadata, episode: EpisodeSelector) -> Multi | Single:        
-        for _ in range(self.MAX_TRIES):
-            vidsrc = self.__get_embed(metadata, EpisodeSelector())
-
-            if vidsrc.status_code != 503:
-                break
-
-        print(self.soup(vidsrc).prettify())
-
-        iframeurl = "https:" + self.soup(vidsrc).select("iframe#player_iframe")[0]["src"]
-
-        for _ in range(self.MAX_TRIES):
-            doc = self.http_client.get(iframeurl, headers={"Referer": vidsrc})
-
-            if doc.status_code != 503:
-                break
-
-        doc = self.soup(doc)
-
-        index = doc.select("body")[0]["data-i"]
-        hash = doc.select("div#hidden")[0]["data-h"]
-
-        srcrcp = "https:" + self.__deobfstr(hash, index).replace("vidsrc.stream", "vidsrc.net")
-
-        for _ in range(self.MAX_TRIES):
-            prourl = self.http_client.get(srcrcp, headers={"Referer": "https://vidsrc.stream/"}).headers.get("Location", None)
-
-            if prourl is not None:
-                break
-
-        url = self.__get_url(prourl)
-
-        if metadata.type == MetadataType.MOVIE:
-            return Single(
-                url = url,
-                title = metadata.title,
-                referrer = "https://vidsrc.stream/",
-                year = metadata.year
-            )
-
-        return Multi(
-            url = url,
-            title = metadata.title,
-            referrer = "https://vidsrc.stream/",
-            episode = episode
+from __future__ import annotations
+from typing import TYPE_CHECKING, Dict, Iterable
+
+if TYPE_CHECKING:
+    from typing import Dict, Literal, Optional
+
+    from mov_cli import Config
+    from httpx import Response
+    from mov_cli.http_client import HTTPClient
+    from mov_cli.scraper import ScraperOptionsT
+
+import re
+
+from mov_cli.scraper import Scraper
+from mov_cli import Multi, Single, Metadata, MetadataType
+from mov_cli.utils.scraper import TheMovieDB
+from mov_cli.utils import EpisodeSelector
+
+import base64
+
+
+__all__ = ("VidSrcMeScraper",)
+
+class VidSrcMeScraper(Scraper):
+    def __init__(self, config: Config, http_client: HTTPClient, options: Optional[ScraperOptionsT] = None) -> None:
+        self.base_url = "https://vidsrc.net"
+        self.tmdb = TheMovieDB(http_client)
+
+        self.MAX_TRIES = 10
+        super().__init__(config, http_client, options)
+
+    def search(self, query: str, limit: int = 10) -> Iterable[Metadata]:
+        for search_result in self.tmdb.search(query, limit):
+            embed_response = self.__get_embed(search_result, EpisodeSelector())
+
+            if embed_response.status_code == 404: # don't include media that isn't available on the provider.
+                continue
+
+            yield search_result
+
+    def scrape_episodes(self, metadata: Metadata) -> Dict[int, int] | Dict[None, Literal[1]]:
+        return self.tmdb.scrape_episodes(metadata)
+
+    def __deobfstr(self, hash, index):
+        result = ""
+        for i in range(0, len(hash), 2):
+            j = hash[i:i+2]
+            result += chr(int(j, 16) ^ ord(index[i // 2 % len(index)]))
+        return result
+
+    def __get_url(self, prourl: str):
+        url = None
+        
+        for _ in range(self.MAX_TRIES):
+            prorcp = self.http_client.get(prourl, headers={"Referer": "https://vidsrc.stream/"})
+
+            if prorcp.status_code == 503:
+                continue
+            
+            hls_url = re.search(r'file:"([^"]*)"', prorcp.text).group(1)
+            hls_url = re.sub(r'\/\/\S+?=', '', hls_url)[2:]     
+            hls_url = re.sub(r"\/@#@\/[^=\/]+==", "", hls_url)
+
+            hls_url = hls_url.replace('_', '/').replace('-', '+')
+
+            try:
+                hls_url = bytearray(base64.b64decode(hls_url))
+                hls_url = hls_url.decode('utf-8')
+            except UnicodeDecodeError:
+                hls_url = None
+
+            if hls_url is not None:
+                url = hls_url
+                break
+
+        return url
+
+    def __get_embed(self, metadata: Metadata, episode: EpisodeSelector) -> Response:
+        media_type = "tv" if metadata.type == MetadataType.SERIES else "movie"
+
+        url = f"{self.base_url}/embed/{media_type}/{metadata.id}"
+
+        if metadata.type == MetadataType.SERIES:
+            url += f"/{episode.season}/{episode.episode}"
+
+        return self.http_client.get(url)
+
+    def scrape(self, metadata: Metadata, episode: EpisodeSelector) -> Multi | Single:        
+        for _ in range(self.MAX_TRIES):
+            vidsrc = self.__get_embed(metadata, EpisodeSelector())
+
+            if vidsrc.status_code != 503:
+                break
+
+        print(self.soup(vidsrc).prettify())
+
+        iframeurl = "https:" + self.soup(vidsrc).select("iframe#player_iframe")[0]["src"]
+
+        for _ in range(self.MAX_TRIES):
+            doc = self.http_client.get(iframeurl, headers={"Referer": vidsrc})
+
+            if doc.status_code != 503:
+                break
+
+        doc = self.soup(doc)
+
+        index = doc.select("body")[0]["data-i"]
+        hash = doc.select("div#hidden")[0]["data-h"]
+
+        srcrcp = "https:" + self.__deobfstr(hash, index).replace("vidsrc.stream", "vidsrc.net")
+
+        for _ in range(self.MAX_TRIES):
+            prourl = self.http_client.get(srcrcp, headers={"Referer": "https://vidsrc.stream/"}).headers.get("Location", None)
+
+            if prourl is not None:
+                break
+
+        url = self.__get_url(prourl)
+
+        if metadata.type == MetadataType.MOVIE:
+            return Single(
+                url = url,
+                title = metadata.title,
+                referrer = "https://vidsrc.stream/",
+                year = metadata.year
+            )
+
+        return Multi(
+            url = url,
+            title = metadata.title,
+            referrer = "https://vidsrc.stream/",
+            episode = episode
         )
```

### Comparing `mov-cli-films-1.3.8/mov_cli_films/vidsrcto/ext/vidplay.py` & `mov-cli-films-1.3.9/mov_cli_films/vidsrcto/ext/vidplay.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-"""Code from: https://github.com/Ciarands/vidsrc-to-resolver"""
-from __future__ import annotations
-from typing import TYPE_CHECKING, Dict
-
-if TYPE_CHECKING:
-    from typing import Dict, Optional, Union, Tuple, List
-
-    from mov_cli.http_client import HTTPClient
-
-import re
-import base64
-import json
-from mov_cli.errors import MovCliException
-
-__all__ = (
-    "VidPlay",
-)
-
-class VidPlay():
-    def __init__(self, http_client: HTTPClient) -> None:
-        self.KEY_URL : str = "https://github.com/Ciarands/vidsrc-keys/blob/main/keys.json"
-        self.http_client = http_client
-    
-    def decode_data(self, key: str, data: Union[bytearray, str]) -> bytearray:
-        key_bytes = bytes(key, 'utf-8')
-        s = bytearray(range(256))
-        j = 0
-
-        for i in range(256):
-            j = (j + s[i] + key_bytes[i % len(key_bytes)]) & 0xff
-            s[i], s[j] = s[j], s[i]
-
-        decoded = bytearray(len(data))
-        i = 0
-        k = 0
-
-        for index in range(len(data)):
-            i = (i + 1) & 0xff
-            k = (k + s[i]) & 0xff
-            s[i], s[k] = s[k], s[i]
-            t = (s[i] + s[k]) & 0xff
-
-            if isinstance(data[index], str):
-                decoded[index] = ord(data[index]) ^ s[t]
-            elif isinstance(data[index], int):
-                decoded[index] = data[index] ^ s[t]
-            else:
-                raise RC4DecodeFailure("Unsupported data type in the input")
-
-        return decoded
-    
-    def int_2_base(self, x: int, base: int) -> str:
-        charset = "0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ+/"
-
-        if x < 0:
-            sign = -1
-        elif x == 0:
-            return 0
-        else:
-            sign = 1
-
-        x *= sign
-        digits = []
-
-        while x:
-            digits.append(charset[int(x % base)])
-            x = int(x / base)
-        
-        if sign < 0:
-            digits.append('-')
-        digits.reverse()
-
-        return ''.join(digits)
-    
-    def decode_base64_url_safe(s: str) -> bytearray:
-        standardized_input = s.replace('_', '/').replace('-', '+')
-        binary_data = base64.b64decode(standardized_input)
-        return bytearray(binary_data)
-
-    def get_futoken(self, key: str, url: str, provider_url: str) -> str:
-        req = self.http_client.get(f"{provider_url}/futoken", {"Referer": url})
-        fu_key = re.search(r"var\s+k\s*=\s*'([^']+)'", req.text).group(1)
-        
-        return f"{fu_key},{','.join([str(ord(fu_key[i % len(fu_key)]) + ord(key[i])) for i in range(len(key))])}"
-
-    def encode_id(self, v_id: str) -> str:
-        req = self.http_client.get(self.KEY_URL)
-        
-        matches = re.search(r"\"rawLines\":\s*\[\"(.+)\"\]", req.text)
-
-        key1, key2 = json.loads(matches.group(1).replace("\\", ""))
-        decoded_id = self.decode_data(key1, v_id)
-        encoded_result = self.decode_data(key2, decoded_id)
-        
-        encoded_base64 = base64.b64encode(encoded_result)
-        decoded_result = encoded_base64.decode("utf-8")
-
-        return decoded_result.replace("/", "_")
-    
-    def resolve_source(self, url: str, provider_url: str = "https://vidplay.online") -> Tuple[Optional[List], Optional[Dict]]:
-        url_data = url.split("?")
-
-        key = self.encode_id(url_data[0].split("/e/")[-1])
-        futoken = self.get_futoken(key, url, provider_url)
-        
-        req = self.http_client.get(f"{provider_url}/mediainfo/{futoken}?{url_data[1]}&autostart=true", headers={"Referer": url})
-        if req.status_code != 200:
-            return None, None
-
-        req_data = req.json()
-        if (req_data.get("result")) and isinstance(req_data.get("result"), dict):
-            sources = req_data.get("result").get("sources")
-            return [value.get("file") for value in sources]
-        
-        return None, None
-
-class RC4DecodeFailure(MovCliException):
-    """Raised when failure on decoding RC4 data."""
-    def __init__(self) -> None:
-        super().__init__(
-            "Failed to decode RC4 Data."
+"""Code from: https://github.com/Ciarands/vidsrc-to-resolver"""
+from __future__ import annotations
+from typing import TYPE_CHECKING, Dict
+
+if TYPE_CHECKING:
+    from typing import Dict, Optional, Union, Tuple, List
+
+    from mov_cli.http_client import HTTPClient
+
+import re
+import base64
+import json
+from mov_cli.errors import MovCliException
+
+__all__ = (
+    "VidPlay",
+)
+
+class VidPlay():
+    def __init__(self, http_client: HTTPClient) -> None:
+        self.KEY_URL : str = "https://github.com/Ciarands/vidsrc-keys/blob/main/keys.json"
+        self.http_client = http_client
+    
+    def decode_data(self, key: str, data: Union[bytearray, str]) -> bytearray:
+        key_bytes = bytes(key, 'utf-8')
+        s = bytearray(range(256))
+        j = 0
+
+        for i in range(256):
+            j = (j + s[i] + key_bytes[i % len(key_bytes)]) & 0xff
+            s[i], s[j] = s[j], s[i]
+
+        decoded = bytearray(len(data))
+        i = 0
+        k = 0
+
+        for index in range(len(data)):
+            i = (i + 1) & 0xff
+            k = (k + s[i]) & 0xff
+            s[i], s[k] = s[k], s[i]
+            t = (s[i] + s[k]) & 0xff
+
+            if isinstance(data[index], str):
+                decoded[index] = ord(data[index]) ^ s[t]
+            elif isinstance(data[index], int):
+                decoded[index] = data[index] ^ s[t]
+            else:
+                raise RC4DecodeFailure("Unsupported data type in the input")
+
+        return decoded
+    
+    def int_2_base(self, x: int, base: int) -> str:
+        charset = "0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ+/"
+
+        if x < 0:
+            sign = -1
+        elif x == 0:
+            return 0
+        else:
+            sign = 1
+
+        x *= sign
+        digits = []
+
+        while x:
+            digits.append(charset[int(x % base)])
+            x = int(x / base)
+        
+        if sign < 0:
+            digits.append('-')
+        digits.reverse()
+
+        return ''.join(digits)
+    
+    def decode_base64_url_safe(s: str) -> bytearray:
+        standardized_input = s.replace('_', '/').replace('-', '+')
+        binary_data = base64.b64decode(standardized_input)
+        return bytearray(binary_data)
+
+    def get_futoken(self, key: str, url: str, provider_url: str) -> str:
+        req = self.http_client.get(f"{provider_url}/futoken", {"Referer": url})
+        fu_key = re.search(r"var\s+k\s*=\s*'([^']+)'", req.text).group(1)
+        
+        return f"{fu_key},{','.join([str(ord(fu_key[i % len(fu_key)]) + ord(key[i])) for i in range(len(key))])}"
+
+    def encode_id(self, v_id: str) -> str:
+        req = self.http_client.get(self.KEY_URL)
+        
+        matches = re.search(r"\"rawLines\":\s*\[\"(.+)\"\]", req.text)
+
+        key1, key2 = json.loads(matches.group(1).replace("\\", ""))
+        decoded_id = self.decode_data(key1, v_id)
+        encoded_result = self.decode_data(key2, decoded_id)
+        
+        encoded_base64 = base64.b64encode(encoded_result)
+        decoded_result = encoded_base64.decode("utf-8")
+
+        return decoded_result.replace("/", "_")
+    
+    def resolve_source(self, url: str, provider_url: str = "https://vidplay.online") -> Tuple[Optional[List], Optional[Dict]]:
+        url_data = url.split("?")
+
+        key = self.encode_id(url_data[0].split("/e/")[-1])
+        futoken = self.get_futoken(key, url, provider_url)
+        
+        req = self.http_client.get(f"{provider_url}/mediainfo/{futoken}?{url_data[1]}&autostart=true", headers={"Referer": url})
+        if req.status_code != 200:
+            return None, None
+
+        req_data = req.json()
+        if (req_data.get("result")) and isinstance(req_data.get("result"), dict):
+            sources = req_data.get("result").get("sources")
+            return [value.get("file") for value in sources]
+        
+        return None, None
+
+class RC4DecodeFailure(MovCliException):
+    """Raised when failure on decoding RC4 data."""
+    def __init__(self) -> None:
+        super().__init__(
+            "Failed to decode RC4 Data."
         )
```

### Comparing `mov-cli-films-1.3.8/mov_cli_films.egg-info/PKG-INFO` & `mov-cli-films-1.3.9/mov_cli_films.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-Metadata-Version: 2.1
-Name: mov-cli-films
-Version: 1.3.8
-Summary: A mov-cli v4 plugin for watching Films and Shows.
-Author-email: Ananas <ananas@r3tr0ananas.lol>
-License: MIT License
-        
-        Copyright (c) 2024 mov-cli
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: GitHub, https://github.com/JDALab/mov-cli-films
-Project-URL: BugTracker, https://github.com/JDALab/mov-cli-films/issues
-Keywords: amazing mov-cli plugin
-Classifier: Operating System :: Microsoft :: Windows :: Windows 11
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Operating System :: POSIX :: Linux
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: mov-cli>=4.0.3
-Provides-Extra: dev
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: build; extra == "dev"
-
-<div align="center">
-
-  # mov-cli-films 
-  <sub>A mov-cli v4 plugin for watching Films and Shows.</sub>
-
-  <img src="https://github.com/mov-cli/mov-cli-vadapav/assets/132799819/6406133d-f840-424b-a1c9-04599fadb0a7">
-
-</div>
-
-> [!NOTE]
-> Searching for maintainers
-
-## Installation
-Here's how to install and add the plugin to mov-cli.
-
-1. Install the pip package.
-```sh
-pip install mov-cli-films 
-```
-2. Then add the plugin to your mov-cli config.
-```sh
-mov-cli -e
-```
-```toml
-[mov-cli.plugins]
-films = "mov-cli-films"
-```
-
-## Usage
-```sh
-mov-cli -s films the rookie
-```
+Metadata-Version: 2.1
+Name: mov-cli-films
+Version: 1.3.9
+Summary: A mov-cli v4 plugin for watching Films and Shows.
+Author-email: Ananas <ananas@r3tr0ananas.lol>
+License: MIT License
+        
+        Copyright (c) 2024 mov-cli
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: GitHub, https://github.com/JDALab/mov-cli-films
+Project-URL: BugTracker, https://github.com/JDALab/mov-cli-films/issues
+Keywords: amazing mov-cli plugin
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: POSIX :: Linux
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: mov-cli>=4.0.3
+Provides-Extra: dev
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: build; extra == "dev"
+
+<div align="center">
+
+  # mov-cli-films 
+  <sub>A mov-cli v4 plugin for watching Films and Shows.</sub>
+
+  <img src="https://github.com/mov-cli/mov-cli-vadapav/assets/132799819/6406133d-f840-424b-a1c9-04599fadb0a7">
+
+</div>
+
+> [!NOTE]
+> Searching for maintainers
+
+## Installation
+Here's how to install and add the plugin to mov-cli.
+
+1. Install the pip package.
+```sh
+pip install mov-cli-films 
+```
+2. Then add the plugin to your mov-cli config.
+```sh
+mov-cli -e
+```
+```toml
+[mov-cli.plugins]
+films = "mov-cli-films"
+```
+
+## Usage
+```sh
+mov-cli -s films the rookie
+```
```

### Comparing `mov-cli-films-1.3.8/mov_cli_films.egg-info/SOURCES.txt` & `mov-cli-films-1.3.9/mov_cli_films.egg-info/SOURCES.txt`

 * *Files identical despite different names*

