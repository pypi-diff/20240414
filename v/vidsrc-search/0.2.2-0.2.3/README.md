# Comparing `tmp/vidsrc_search-0.2.2.tar.gz` & `tmp/vidsrc_search-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vidsrc_search-0.2.2.tar", last modified: Fri Apr 12 20:11:42 2024, max compression
+gzip compressed data, was "vidsrc_search-0.2.3.tar", last modified: Sun Apr 14 05:40:58 2024, max compression
```

## Comparing `vidsrc_search-0.2.2.tar` & `vidsrc_search-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-12 20:11:42.163082 vidsrc_search-0.2.2/
--rw-r--r--   0 Dev        (502) staff       (20)     1053 2024-04-11 00:33:35.000000 vidsrc_search-0.2.2/LICENSE
--rw-r--r--   0 Dev        (502) staff       (20)     1958 2024-04-12 20:11:42.162789 vidsrc_search-0.2.2/PKG-INFO
--rw-r--r--   0 Dev        (502) staff       (20)     1075 2024-04-12 02:57:47.000000 vidsrc_search-0.2.2/README.md
--rw-r--r--   0 Dev        (502) staff       (20)      977 2024-04-12 19:43:26.000000 vidsrc_search-0.2.2/pyproject.toml
--rw-r--r--   0 Dev        (502) staff       (20)       38 2024-04-12 20:11:42.163140 vidsrc_search-0.2.2/setup.cfg
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-12 20:11:42.158385 vidsrc_search-0.2.2/src/
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-12 20:11:42.161112 vidsrc_search-0.2.2/src/vidsrc_search/
--rw-r--r--   0 Dev        (502) staff       (20)     1685 2024-04-12 17:43:36.000000 vidsrc_search-0.2.2/src/vidsrc_search/__main__.py
--rw-r--r--   0 Dev        (502) staff       (20)     2213 2024-04-12 06:17:23.000000 vidsrc_search-0.2.2/src/vidsrc_search/argparsing.py
--rw-r--r--   0 Dev        (502) staff       (20)     5314 2024-04-12 17:45:19.000000 vidsrc_search-0.2.2/src/vidsrc_search/library.py
--rw-r--r--   0 Dev        (502) staff       (20)     1763 2024-04-12 20:08:58.000000 vidsrc_search-0.2.2/src/vidsrc_search/modules.py
--rw-r--r--   0 Dev        (502) staff       (20)     7722 2024-04-12 17:42:32.000000 vidsrc_search-0.2.2/src/vidsrc_search/search.py
--rw-r--r--   0 Dev        (502) staff       (20)     8534 2024-04-12 20:10:31.000000 vidsrc_search-0.2.2/src/vidsrc_search/utils.py
-drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-12 20:11:42.162497 vidsrc_search-0.2.2/src/vidsrc_search.egg-info/
--rw-r--r--   0 Dev        (502) staff       (20)     1958 2024-04-12 20:11:42.000000 vidsrc_search-0.2.2/src/vidsrc_search.egg-info/PKG-INFO
--rw-r--r--   0 Dev        (502) staff       (20)      455 2024-04-12 20:11:42.000000 vidsrc_search-0.2.2/src/vidsrc_search.egg-info/SOURCES.txt
--rw-r--r--   0 Dev        (502) staff       (20)        1 2024-04-12 20:11:42.000000 vidsrc_search-0.2.2/src/vidsrc_search.egg-info/dependency_links.txt
--rw-r--r--   0 Dev        (502) staff       (20)       62 2024-04-12 20:11:42.000000 vidsrc_search-0.2.2/src/vidsrc_search.egg-info/entry_points.txt
--rw-r--r--   0 Dev        (502) staff       (20)       34 2024-04-12 20:11:42.000000 vidsrc_search-0.2.2/src/vidsrc_search.egg-info/requires.txt
--rw-r--r--   0 Dev        (502) staff       (20)       14 2024-04-12 20:11:42.000000 vidsrc_search-0.2.2/src/vidsrc_search.egg-info/top_level.txt
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-14 05:40:58.594907 vidsrc_search-0.2.3/
+-rw-r--r--   0 Dev        (502) staff       (20)     1053 2024-04-11 00:33:35.000000 vidsrc_search-0.2.3/LICENSE
+-rw-r--r--   0 Dev        (502) staff       (20)     1958 2024-04-14 05:40:58.594675 vidsrc_search-0.2.3/PKG-INFO
+-rw-r--r--   0 Dev        (502) staff       (20)     1075 2024-04-12 02:57:47.000000 vidsrc_search-0.2.3/README.md
+-rw-r--r--   0 Dev        (502) staff       (20)      977 2024-04-14 04:48:50.000000 vidsrc_search-0.2.3/pyproject.toml
+-rw-r--r--   0 Dev        (502) staff       (20)       38 2024-04-14 05:40:58.594956 vidsrc_search-0.2.3/setup.cfg
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-14 05:40:58.590431 vidsrc_search-0.2.3/src/
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-14 05:40:58.592412 vidsrc_search-0.2.3/src/vidsrc_search/
+-rw-r--r--   0 Dev        (502) staff       (20)     1238 2024-04-14 05:30:44.000000 vidsrc_search-0.2.3/src/vidsrc_search/__main__.py
+-rw-r--r--   0 Dev        (502) staff       (20)     2111 2024-04-14 05:33:44.000000 vidsrc_search-0.2.3/src/vidsrc_search/argparsing.py
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-14 05:40:58.594138 vidsrc_search-0.2.3/src/vidsrc_search/core/
+-rw-r--r--   0 Dev        (502) staff       (20)     2166 2024-04-14 01:25:38.000000 vidsrc_search-0.2.3/src/vidsrc_search/core/help.py
+-rw-r--r--   0 Dev        (502) staff       (20)     8120 2024-04-14 05:40:13.000000 vidsrc_search-0.2.3/src/vidsrc_search/core/library.py
+-rw-r--r--   0 Dev        (502) staff       (20)    10870 2024-04-14 05:39:44.000000 vidsrc_search-0.2.3/src/vidsrc_search/core/search.py
+-rw-r--r--   0 Dev        (502) staff       (20)      677 2024-04-14 04:48:41.000000 vidsrc_search-0.2.3/src/vidsrc_search/core/version.py
+-rw-r--r--   0 Dev        (502) staff       (20)      756 2024-04-14 01:08:30.000000 vidsrc_search-0.2.3/src/vidsrc_search/modules.py
+-rw-r--r--   0 Dev        (502) staff       (20)     6584 2024-04-14 05:39:16.000000 vidsrc_search-0.2.3/src/vidsrc_search/utils.py
+drwxr-xr-x   0 Dev        (502) staff       (20)        0 2024-04-14 05:40:58.594421 vidsrc_search-0.2.3/src/vidsrc_search.egg-info/
+-rw-r--r--   0 Dev        (502) staff       (20)     1958 2024-04-14 05:40:58.000000 vidsrc_search-0.2.3/src/vidsrc_search.egg-info/PKG-INFO
+-rw-r--r--   0 Dev        (502) staff       (20)      530 2024-04-14 05:40:58.000000 vidsrc_search-0.2.3/src/vidsrc_search.egg-info/SOURCES.txt
+-rw-r--r--   0 Dev        (502) staff       (20)        1 2024-04-14 05:40:58.000000 vidsrc_search-0.2.3/src/vidsrc_search.egg-info/dependency_links.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       62 2024-04-14 05:40:58.000000 vidsrc_search-0.2.3/src/vidsrc_search.egg-info/entry_points.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       34 2024-04-14 05:40:58.000000 vidsrc_search-0.2.3/src/vidsrc_search.egg-info/requires.txt
+-rw-r--r--   0 Dev        (502) staff       (20)       14 2024-04-14 05:40:58.000000 vidsrc_search-0.2.3/src/vidsrc_search.egg-info/top_level.txt
```

### Comparing `vidsrc_search-0.2.2/LICENSE` & `vidsrc_search-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vidsrc_search-0.2.2/PKG-INFO` & `vidsrc_search-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vidsrc-search
-Version: 0.2.2
+Version: 0.2.3
 Summary: A pirate movie watcher written in Python
 Project-URL: Homepage, https://github.com/SomedudeX/vidsrc-search
 Project-URL: License, https://github.com/SomedudeX/vidsrc-search/blob/main/LICENSE
 Project-URL: Changelog, https://github.com/SomedudeX/vidsrc-search/releases
 Keywords: movie,video,search
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `vidsrc_search-0.2.2/README.md` & `vidsrc_search-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `vidsrc_search-0.2.2/pyproject.toml` & `vidsrc_search-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vidsrc-search"
-version = "0.2.2"
+version = "0.2.3"
 description = "A pirate movie watcher written in Python"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `vidsrc_search-0.2.2/src/vidsrc_search/argparsing.py` & `vidsrc_search-0.2.3/src/vidsrc_search/argparsing.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,84 +1,71 @@
-from typing import List, Tuple, Dict, Any, Union
+from typing import Any, Dict, List, Tuple
 
 
 class ArgumentsError(Exception):
+    """An error encountered when parsing arguments"""
     def __init__(
         self,
         message: str,
         code: int = 1
     ) -> None:
+        """Initializes an ArgumentsError instance"""
         self.message = message
         self.code = code
         super().__init__()
+        return
 
 
 def is_flag(arg: str) -> bool:
-    assert len(arg) > 0
-    return arg[0] == "-"
+    """Whether an item from sys.argv is a flag"""
+    return len(arg) >= 1 and \
+           arg[0] == "-"
 
 
 def is_int(arg: str) -> bool:
-    if not isinstance(arg, str):
-        return False
-    return arg.isdigit()
+    """Whether an item from sys.argv is an integer"""
+    return len(arg) >= 1 and \
+           arg.isdigit()
 
 
 def is_stacked_flag(flag: str) -> bool:
-    if len(flag) <= 2:
-        return False
-    return flag[0] == "-" and flag[1] != "-"
-
-
-def process_bool_flag(flag: tuple) -> Union[int, str]:
-    if not is_int(flag[1]):
-        return flag[1]
-    return bool(int(flag[1]))
+    """Whether an argument is a stacked flag (e.g. -abc)"""
+    return len(flag) >= 2 and \
+           flag[0] == "-" and \
+           flag[1] != "-"
 
 
 def split_arguments(argv: List[str]) -> Tuple[Any, Any]:
-    for index, arg in enumerate(argv):
-        if is_flag(arg):
+    """Splits arguments into positionals and flags. This is responsible
+    for enforcing the structure of the arguments (positionals before flags)
+    """
+    for index, argument in enumerate(argv):
+        if is_flag(argument):
             flags = argv[index:]
             positionals = argv[:index]
-            return positionals, split_flags(flags)
+            return positionals, flags
     return argv, []
 
 
-def split_flags(flags: List[str]) -> List[Tuple]:
-    ret = []
-    for _ in range(len(flags)):
-        if len(flags) == 0:
-            break
-        current_flag = flags[0]
-        if current_flag[0] == "-":
-            option = current_flag
-            ret.append((option, True))
-            del flags[0]
-            continue
-        raise ArgumentsError(f"error parsing '{current_flag}' (unexpected trailing positional)", 1)
-    return ret
-
-
 def parse_arguments(argv: List[str]) -> Dict[str, Any]:
-    ret = {
+    """Parse the arguments from sys.argv into a dictionary"""
+    positionals, flags = split_arguments(argv[1:])
+    parsed_arguments = {
         "module": [""],
         "raw": False,
         "new": False
     }
 
-    positionals, flags = split_arguments(argv)
-
     if len(positionals) > 0:
-        ret["module"] = positionals
+        parsed_arguments["module"] = positionals
 
     for flag in flags:   # Mapping each command line flag to a dictionary key
-        if flag[0] == "--raw" or flag[0] == "-r":
-            ret["raw"] = process_bool_flag(flags[0])
+        if flag == "--raw" or flag == "-r":
+            parsed_arguments["raw"] = True
             continue
-        if flag[0] == "--new" or flag[0] == "-n":
-            ret["new"] = process_bool_flag(flags[0])
+        if flag == "--new" or flag == "-n":
+            parsed_arguments["new"] = True
             continue
-        if is_stacked_flag(flag[0]):
-            raise ArgumentsError(f"stacked flag '{flag[0]}' not allowed", 1)
-        raise ArgumentsError(f"invalid flag '{flag[0]}' received", 1)
-    return ret
+        if is_stacked_flag(flag):
+            raise ArgumentsError(f"stacked flag '{flag}' not allowed", 1)
+        raise ArgumentsError(f"invalid flag '{flag}' received", 1)
+    return parsed_arguments
```

### Comparing `vidsrc_search-0.2.2/src/vidsrc_search/search.py` & `vidsrc_search-0.2.3/src/vidsrc_search/core/library.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,221 +1,225 @@
+# Using classes for better organization
+
 import os
 import sys
 import json
-import requests
-import webbrowser
+import time
+import asyncio
 
-from . import utils
+import aiohttp
+import requests
 
-from typing import List, Tuple
+from typing import Any, List, Union
 
-from tabulate import tabulate
-from thefuzz.fuzz import partial_ratio, ratio
-from html.parser import HTMLParser
+from .. import utils
+from ..argparsing import ArgumentsError
 
 
-def similarity(str1: str, str2: str) -> float:
-    return (2 * partial_ratio(str1.lower(), str2.lower()) + 8 * ratio(str1.lower(), str2.lower())) / 10
+class Library:
+    """Properties of the library"""
+    root_path = os.path.expanduser("~/.local/vidsrc-search")
+    lib_path = os.path.expanduser("~/.local/vidsrc-search/lib.json")
+    cache_path = os.path.expanduser("~/.local/vidsrc-search/cache")
 
+    def check_library(
+        self,
+        exit_on_false: bool = True
+    ) -> bool:
+        """Checks whether the library exist or not"""
+        if os.path.exists(self.lib_path):
+            return True
+        if exit_on_false:
+            print("fatal: library does not exist")
+            print("fatal: please download the library first by using 'vidsrc-search library download'")
+            print("fatal: vidsrc-search terminating with exit code 2")
+            sys.exit(2)
+        return False
+
+class DownloadManager:
+    """A manager for library downloads"""
+
+    def __init__(
+        self,
+        types: List[str]
+    ) -> None:
+        """Initializes a download manager instance with the types of media
+        to be downloaded from vidsrc
+        """
+        self.types = types
+        self.time: float
 
-def relevance_key(entry) -> float:
-    return float(entry["Match"])
+        self.final_size: int = 0
+        self.expected_size: int = 0
+        return
 
+    def handle_download_library(self) -> None:
+        """Handles the downloading of the library"""
+        self.start_download()
+        self.print_summary()
+        return
 
-def sort_results(result: list) -> list:
-    result.sort(key = relevance_key, reverse = True)
-    return result
+    def start_download(self) -> None:
+        """Starts the downloading of types specified in the constructor"""
+        utils.check_internet()
+
+        start_time = time.time()
+        for item in self.types:
+            size = DownloadManager.get_download_size(item)
+            asyncio.run(DownloadManager.download(size, item))
+
+            self.final_size += size * 15
+            self.expected_size += utils.unite_jsons(f"~/.local/vidsrc-search/{item}_buffer/", f"~/.local/vidsrc-search/{item}.json")
+        end_time = time.time()
+
+        RemovalManager.remove_library()   # Removing previously downloaded library
+        utils.unite_jsons(f"~/.local/vidsrc-search/", f"~/.local/vidsrc-search/lib.json", raw=False)
+        utils.cleanup()
+        self.time = start_time - end_time
+        return
 
+    def print_summary(self) -> None:
+        """Prints the summary of download"""
+        loss = 100 * ((self.expected_size - self.final_size) / self.expected_size)
+        if loss < 1:
+            loss = 0
+        print(f"info: total/estimated number of movies downloaded: {self.expected_size}/{self.final_size}")
+        print(f"info: estimated link loss from client/server connection issues: ~{loss:.2f}%")
+        print(f"info: operation took {self.time:.2f} seconds to complete")
+        print(f"info: library has been downloaded")
+        return
 
-def search_library(search_query: str):
-    ret = []
-    lib_path = os.path.expanduser("~/.local/vidsrc-search/lib.json")
-    if not os.path.exists(lib_path):
-        print("fatal: library does not exist")
-        print("fatal: please download the library first by using 'vidsrc-search library download'")
-        print("fatal: vidsrc-search terminating with exit code 2")
-        sys.exit(2)
-
-    with open(lib_path, "r") as f: 
-        library = f.read()
-    library = json.loads(library) 
-
-    for entry in library: 
-        if similarity(entry["title"][:len(entry["title"]) - 7], search_query) >= 60:
-            ret.append({
-                "Index": None,
-                "Title": entry["title"], 
-                "IMDB ID": entry["imdb_id"][2:],
-                "Type": entry["type"], 
-                "URL": entry["embed_url_imdb"],
-                "Match": f"{similarity(entry['title'][:len(entry['title']) - 7], search_query):.2f}",
-            })
-
-    if len(ret) == 0: 
-        return None
-
-    ret = sort_results(ret)
-    while len(ret) > 20: 
-        del ret[len(ret) - 1]
-    index = 1
-    for result in ret:
-        result["Index"] = f"[{index}]"
-        result["Match"] += "%"
-        index += 1
-    ret.reverse()
-    return ret
-
-
-def ask_open_index(movies: list) -> int:
-    while True:
-        try:
-            open_index = int(input(" > choose an index to open in browser: "))
-            if open_index <= 0 or open_index > len(movies):
-                raise ValueError()
-            open_index = len(movies) - open_index
-            return open_index
-        except ValueError:
-            print("error: please enter a valid value")
-            continue
-
-
-def print_movies(movies: list) -> None:
-    print()
-    print(tabulate(movies, headers = "keys", tablefmt = "grid", maxcolwidths = [4, 36]))
-    print()
-    return
-
-
-def print_warning() -> None:
-    print()
-    print("warning: the content of the movie is hosted on a third party site. the")
-    print("         site is not endorsed by the author or checked for its quality, ")
-    print("         content, or authenticity. the author of vidsrc-search disclaims")
-    print("         any responsibility, express or implied, of the consequences ")
-    print("         as a result your usage or dependence on the website provided ")
-    print("         through this tool. ")
-    print("warning: the following window shown will be the cached contents of vidsrc.to\n")
-    affirm = input(" > i have read and understood the conditions above (Y/n) ")
-    print()
-    if not affirm == "Y":
-        print()
-        print("info: terminating per user request")
-        raise UserWarning
-    return
-
-
-def delete_substring(text, start_offset, end_offset):
-    deleted_text = text[:start_offset - 1] + text[end_offset + 1:]
-    return deleted_text
-
-
-def process_html(path: str) -> None:
-    print(f"info: processing html")
-    with open(path, "r") as f:
-        content = f.readlines()
-        content = ''.join(content)
-        while True:
-            parser = FileProcesser()
-            parser.feed(content)
-            if len(parser.positions_tag) == 0:
-                break
-            content = delete_substring(
-                content,
-                parser.start_positions[0][1] + 1,
-                parser.end_positions[0][1] + len(parser.positions_tag[0]) - 1
-            )
-
-    print(f"info: writing processed html")
-    with open(path, "w") as f:
-        f.write(content)
-
-
-def show_movie(index: int, results: list, raw: bool, recache: bool):
-    print_warning()
-    utils.check_internet()
-
-    number = index + 1
-    title = results[index]["Title"]
-    url = results[index]["URL"]
-    id = results[index]["IMDB ID"]
-
-    if raw:
-        print(f"info: opening #{number} '{title}' in new browser window")
-        webbrowser.open(url)
-        return
-
-    print()
-    print(f"info: checking for local cache")
-    if os.path.exists(os.path.expanduser(f"~/.local/vidsrc-search/cache/{id}.html")) and recache:
-        print(f"info: local cache found: recaching by requesting remote html per user request")
-        response = requests.get(url)
-        print(f"info: remote html request status code is {response.status_code}")
-        with open(os.path.expanduser(f"~/.local/vidsrc-search/cache/{id}.html"), "w") as f:
-            print(f"info: writing remote html content to local cache")
-            f.write(response.content.decode())
-            print(f"info: finished recaching html")
-    if not os.path.exists(os.path.expanduser(f"~/.local/vidsrc-search/cache/{id}.html")):
-        print(f"info: local cache not found: Caching by requesting remote html")
-        response = requests.get(url)
-        print(f"info: remote html request status code is {response.status_code}")
-        with open(os.path.expanduser(f"~/.local/vidsrc-search/cache/{id}.html"), "w") as f:
-            print(f"info: writing remote html content to local cache")
-            f.write(response.content.decode())
-            print(f"info: finished caching html")
-    process_html(os.path.expanduser(f"~/.local/vidsrc-search/cache/{id}.html"))
-    print(f"info: opening #{number} '{title}' in new browser window")
-    webbrowser.open("file://" + os.path.expanduser(f"~/.local/vidsrc-search/cache/{id}.html"))
-    return
-    
-
-def handle_search(query: str, raw: bool = True, recache: bool = False) -> None:
-    print(f"info: searching json library for '{query}'")
-    print(f"info: open raw website: {str(raw).lower()}")
-    print(f"info: recaching website: {str(recache).lower()}")
-    results = search_library(query)
-    if results == None:
-        print(f"info: '{query}' not found in movies library")
-        print(f"info: vidsrc-search terminating due to entry not found")
-        return
-    print_movies(results)
-    open_index = ask_open_index(results)
-    show_movie(open_index, results, raw, recache)
-    return
-
-
-class FileProcesser(HTMLParser):
-
-    def __init__(self, *, convert_charrefs: bool = True) -> None:
-        self.start_positions: List[Tuple] = []
-        self.end_positions: List[Tuple] = []
-        self.positions_tag: List[str] = []
-        self.current_bad_script = 0
-        self.current_bad_element = 0
-        super().__init__(convert_charrefs=convert_charrefs)
+    @staticmethod
+    def get_download_size(kind: str) -> int:
+        """Estimates the number of pages (links) of a download using binary
+        search.
+        """
+        print(f"info: estimating download size for {kind} items (this may take a while)")
+
+        index = 0
+        width = 2048
+        this_direction = 1
+        last_direction = 1
+        while width > 1:
+            url = f"https://vidsrc.to/vapi/{kind}/new/{index}"
+            file = requests.get(url)
+            if last_direction != this_direction:
+                width = width // 2
+            if len(file.content) > 50:
+                last_direction = this_direction
+                this_direction = 1
+                index += width * 1
+            if len(file.content) < 50:
+                last_direction = this_direction
+                this_direction = -1
+                index += width * -1
+        return index
 
-    def handle_starttag(self, tag, attrs):
-        if tag not in ["script", "div"]:
+    @staticmethod
+    async def fetch_downloads(session: aiohttp.ClientSession, url: str, _tries: int = 3) -> Union[Any, None]:
+        """Asynchronously fetch a json file from a url, retrying if the response is not a json"""
+        async with session.get(url) as response:
+            if response.content_type == "application/json":
+                if _tries != 3:
+                    print(f"info: retry successful")
+                return await response.json()
+            if _tries != 0:
+                print(f"error: bad connection encountered, retrying ({_tries})")
+                return await DownloadManager.fetch_downloads(session, url, _tries - 1)
+            print(f"info: too many retries, omitting current link")
             return
-        for attr in attrs:
-            if self.bad_script(attr):
-                self.current_bad_script += 1
-                self.start_positions.append(self.getpos())
 
-    def handle_endtag(self, tag: str) -> None:
-        if tag not in ["script", "div"]:
-            return
-        if self.current_bad_script == 1:
-            self.current_bad_script = 0
-            self.end_positions.append(self.getpos())
-            self.positions_tag.append("</script>")
-        if self.current_bad_script != 0:
-            self.current_bad_script -= 1
-
-    @staticmethod
-    def bad_script(script_attr: tuple):
-        if script_attr[0] != "src":
-            return False
-        if "embed" in script_attr[1]:
-            return False
-        if "cloudflare" in script_attr[1]:
-            return False
-        return True
+    @staticmethod
+    async def download(total: int, type: str):
+        """Downloads the movie library into a buffer folder on disk"""
+        domain = f"https://vidsrc.to/vapi/{type}/new/"
+        folder = f"~/.local/vidsrc-search/{type}_buffer/"
+        urls = [f"{domain}{i}" for i in range(total)]
+        print(f"info: initialized {type} download with {total} links to jsons")
+        print(f"info: waiting for response(s) from {total} server requests")
+
+        async with aiohttp.ClientSession() as session:
+            tasks = [DownloadManager.fetch_downloads(session, url) for url in urls]
+            jsons = await asyncio.gather(*tasks)
+            folder = os.path.expanduser(folder)
+
+            print(f"info: writing json files to disk")
+            for index, file in enumerate(jsons):
+                f = open(f"{folder}{index}.json", "w")
+                f.write(json.dumps(file))
+                f.close()
+        return
+
+
+class RemovalManager:
+    """A manager for removing various items on disk"""
+
+    @staticmethod
+    def remove_library() -> None:
+        """Removes the library downloaded from vidsrc"""
+        utils.rmfile(Library.lib_path)
+        return
+
+    @staticmethod
+    def remove_cache() -> None:
+        """Removes the cached html storage"""
+        utils.rmdir_recurse(Library.cache_path)
+        return
+
+    @staticmethod
+    def remove_buffer() -> None:
+        """Removes the buffer storage"""
+        folders = utils.get_file(f"~/.local/vidsrc-search", "_buffer")
+        for folder in folders:
+            utils.rmdir_recurse(f"~/.local/vidsrc-search/" + folder)
+        return
+
+    def handle_remove_library(self) -> None:
+        """Handles the removal of library"""
+        if not os.path.exists(Library.lib_path):
+            print("fatal: library does not exist")
+            print("fatal: please download the library first by using 'vidsrc-search library download'")
+            print("fatal: vidsrc-search terminating with exit code 2")
+            sys.exit(2)
+        with open(Library.lib_path, "r") as f:
+            jsons = json.load(f)
+
+        confirm = input(f" > are you sure you want to remove ~{len(jsons) * 15} links to movies? (Y/n) ")
+        if not confirm == "Y":
+            print("info: user declined operation")
+            print("info: vidsrc-search terminating per user request")
+            sys.exit(0)
+        print(f"info: removing downloaded library")
+        print(f"info: removing cached html files")
+        RemovalManager.remove_library()
+        RemovalManager.remove_cache()
+        return
+
+
+class SizeManager:
+    """A manager for printing the size occupied by the program"""
+
+    def __init__(self) -> None:
+        """Initializes a SizeManager by calculating the library size"""
+        self.size = utils.get_folder_size_recursive(Library.root_path)
+        return
+
+    def print_size(self) -> None:
+        print(f"total disk usage by vidsrc-search: {self.size}")
+        return
+
+
+def run_module(arguments: List[str]) -> None:
+    """Runs the library module"""
+    if arguments == ["library", "download"]:
+        downloader = DownloadManager(["movie", "tv"])
+        downloader.handle_download_library()
+        return
+    if arguments == ["library", "remove"]:
+        remover = RemovalManager()
+        remover.handle_remove_library()
+        return
+    if arguments == ["library", "size"]:
+        sizer = SizeManager()
+        sizer.print_size()
+        return
+    raise ArgumentsError(f"invalid arguments for command 'library' received: {' '.join(arguments)}")
```

### Comparing `vidsrc_search-0.2.2/src/vidsrc_search.egg-info/PKG-INFO` & `vidsrc_search-0.2.3/src/vidsrc_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vidsrc-search
-Version: 0.2.2
+Version: 0.2.3
 Summary: A pirate movie watcher written in Python
 Project-URL: Homepage, https://github.com/SomedudeX/vidsrc-search
 Project-URL: License, https://github.com/SomedudeX/vidsrc-search/blob/main/LICENSE
 Project-URL: Changelog, https://github.com/SomedudeX/vidsrc-search/releases
 Keywords: movie,video,search
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: End Users/Desktop
```

