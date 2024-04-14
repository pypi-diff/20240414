# Comparing `tmp/moddb-0.8.1.tar.gz` & `tmp/moddb-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moddb-0.8.1.tar", last modified: Sat Jan 14 18:10:16 2023, max compression
+gzip compressed data, was "moddb-0.9.0.tar", last modified: Fri Aug 25 07:31:46 2023, max compression
```

## Comparing `moddb-0.8.1.tar` & `moddb-0.9.0.tar`

### file list

```diff
@@ -1,36 +1,60 @@
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-01-14 18:10:16.879970 moddb-0.8.1/
--rw-r--r--   0 clement   (1000) clement   (1000)     1063 2022-06-21 14:40:09.000000 moddb-0.8.1/LICENSE
--rw-rw-r--   0 clement   (1000) clement   (1000)     2883 2023-01-14 18:10:16.879970 moddb-0.8.1/PKG-INFO
--rw-r--r--   0 clement   (1000) clement   (1000)     2613 2022-06-07 19:13:41.000000 moddb-0.8.1/README.md
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-01-14 18:10:16.867970 moddb-0.8.1/moddb/
--rw-r--r--   0 clement   (1000) clement   (1000)      300 2023-01-14 11:00:41.000000 moddb-0.8.1/moddb/__init__.py
--rw-r--r--   0 clement   (1000) clement   (1000)     5930 2022-06-07 19:13:41.000000 moddb-0.8.1/moddb/base.py
--rw-r--r--   0 clement   (1000) clement   (1000)    42106 2023-01-14 12:00:19.000000 moddb-0.8.1/moddb/boxes.py
--rw-r--r--   0 clement   (1000) clement   (1000)    34662 2023-01-14 09:36:02.000000 moddb-0.8.1/moddb/client.py
--rw-r--r--   0 clement   (1000) clement   (1000)     9087 2022-06-11 20:54:29.000000 moddb-0.8.1/moddb/enums.py
--rw-r--r--   0 clement   (1000) clement   (1000)      318 2022-06-07 19:13:41.000000 moddb-0.8.1/moddb/errors.py
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-01-14 18:10:16.879970 moddb-0.8.1/moddb/pages/
--rw-r--r--   0 clement   (1000) clement   (1000)      620 2022-06-07 19:13:41.000000 moddb-0.8.1/moddb/pages/__init__.py
--rw-r--r--   0 clement   (1000) clement   (1000)     6716 2022-06-07 19:13:41.000000 moddb-0.8.1/moddb/pages/article.py
--rw-r--r--   0 clement   (1000) clement   (1000)    21950 2022-06-07 19:13:41.000000 moddb-0.8.1/moddb/pages/base.py
--rw-r--r--   0 clement   (1000) clement   (1000)     1789 2022-06-07 19:13:41.000000 moddb-0.8.1/moddb/pages/engine.py
--rw-r--r--   0 clement   (1000) clement   (1000)    17551 2022-06-07 19:13:41.000000 moddb-0.8.1/moddb/pages/entity.py
--rw-r--r--   0 clement   (1000) clement   (1000)    13326 2023-01-14 11:00:45.000000 moddb-0.8.1/moddb/pages/file.py
--rw-r--r--   0 clement   (1000) clement   (1000)     4714 2022-06-21 14:40:09.000000 moddb-0.8.1/moddb/pages/fp.py
--rw-r--r--   0 clement   (1000) clement   (1000)     1717 2022-06-07 19:13:41.000000 moddb-0.8.1/moddb/pages/game.py
--rw-r--r--   0 clement   (1000) clement   (1000)     3650 2022-06-21 14:40:09.000000 moddb-0.8.1/moddb/pages/job.py
--rw-r--r--   0 clement   (1000) clement   (1000)    19439 2022-06-07 19:13:41.000000 moddb-0.8.1/moddb/pages/mixins.py
--rw-r--r--   0 clement   (1000) clement   (1000)     1787 2022-06-07 19:13:41.000000 moddb-0.8.1/moddb/pages/mod.py
--rw-r--r--   0 clement   (1000) clement   (1000)     6270 2022-06-07 19:13:41.000000 moddb-0.8.1/moddb/pages/opinion.py
--rw-r--r--   0 clement   (1000) clement   (1000)     6149 2022-06-07 19:13:41.000000 moddb-0.8.1/moddb/pages/platform.py
--rw-r--r--   0 clement   (1000) clement   (1000)     6416 2022-06-07 19:13:41.000000 moddb-0.8.1/moddb/pages/ware.py
--rw-r--r--   0 clement   (1000) clement   (1000)    13771 2022-06-21 14:40:09.000000 moddb-0.8.1/moddb/utils.py
-drwxrwxr-x   0 clement   (1000) clement   (1000)        0 2023-01-14 18:10:16.871970 moddb-0.8.1/moddb.egg-info/
--rw-rw-r--   0 clement   (1000) clement   (1000)     2883 2023-01-14 18:10:16.000000 moddb-0.8.1/moddb.egg-info/PKG-INFO
--rw-rw-r--   0 clement   (1000) clement   (1000)      590 2023-01-14 18:10:16.000000 moddb-0.8.1/moddb.egg-info/SOURCES.txt
--rw-rw-r--   0 clement   (1000) clement   (1000)        1 2023-01-14 18:10:16.000000 moddb-0.8.1/moddb.egg-info/dependency_links.txt
--rw-rw-r--   0 clement   (1000) clement   (1000)       75 2023-01-14 18:10:16.000000 moddb-0.8.1/moddb.egg-info/requires.txt
--rw-rw-r--   0 clement   (1000) clement   (1000)        6 2023-01-14 18:10:16.000000 moddb-0.8.1/moddb.egg-info/top_level.txt
--rw-r--r--   0 clement   (1000) clement   (1000)      174 2022-06-07 19:13:41.000000 moddb-0.8.1/pyproject.toml
--rw-rw-r--   0 clement   (1000) clement   (1000)       38 2023-01-14 18:10:16.879970 moddb-0.8.1/setup.cfg
--rw-r--r--   0 clement   (1000) clement   (1000)      891 2022-06-07 19:13:41.000000 moddb-0.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-25 07:31:46.650381 moddb-0.9.0/
+-rw-rw-rw-   0        0        0     1089 2023-08-25 07:21:49.000000 moddb-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0       48 2023-08-25 07:30:39.000000 moddb-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2707 2023-08-25 07:31:46.649379 moddb-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2427 2023-08-25 07:21:49.000000 moddb-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-25 07:31:46.581379 moddb-0.9.0/moddb/
+-rw-rw-rw-   0        0        0      324 2023-08-25 07:21:49.000000 moddb-0.9.0/moddb/__init__.py
+-rw-rw-rw-   0        0        0     6724 2023-08-25 07:21:49.000000 moddb-0.9.0/moddb/base.py
+-rw-rw-rw-   0        0        0    46431 2023-08-25 07:21:49.000000 moddb-0.9.0/moddb/boxes.py
+-rw-rw-rw-   0        0        0    37213 2023-08-25 07:21:49.000000 moddb-0.9.0/moddb/client.py
+-rw-rw-rw-   0        0        0     9576 2023-06-12 11:48:33.000000 moddb-0.9.0/moddb/enums.py
+-rw-rw-rw-   0        0        0      330 2023-06-12 11:48:33.000000 moddb-0.9.0/moddb/errors.py
+drwxrwxrwx   0        0        0        0 2023-08-25 07:31:46.614382 moddb-0.9.0/moddb/pages/
+-rw-rw-rw-   0        0        0      653 2023-08-25 07:21:49.000000 moddb-0.9.0/moddb/pages/__init__.py
+-rw-rw-rw-   0        0        0     7067 2023-08-25 07:21:49.000000 moddb-0.9.0/moddb/pages/article.py
+-rw-rw-rw-   0        0        0    22961 2023-08-25 07:21:49.000000 moddb-0.9.0/moddb/pages/base.py
+-rw-rw-rw-   0        0        0     1840 2023-08-25 07:21:49.000000 moddb-0.9.0/moddb/pages/engine.py
+-rw-rw-rw-   0        0        0    18350 2023-08-25 07:21:49.000000 moddb-0.9.0/moddb/pages/entity.py
+-rw-rw-rw-   0        0        0    13816 2023-08-25 07:21:49.000000 moddb-0.9.0/moddb/pages/file.py
+-rw-rw-rw-   0        0        0     4864 2023-08-25 07:21:49.000000 moddb-0.9.0/moddb/pages/fp.py
+-rw-rw-rw-   0        0        0     1763 2023-08-25 07:21:49.000000 moddb-0.9.0/moddb/pages/game.py
+-rw-rw-rw-   0        0        0     3911 2023-08-25 07:21:49.000000 moddb-0.9.0/moddb/pages/job.py
+-rw-rw-rw-   0        0        0    20715 2023-08-25 07:21:49.000000 moddb-0.9.0/moddb/pages/mixins.py
+-rw-rw-rw-   0        0        0     1947 2023-08-25 07:21:49.000000 moddb-0.9.0/moddb/pages/mod.py
+-rw-rw-rw-   0        0        0     6708 2023-08-25 07:21:49.000000 moddb-0.9.0/moddb/pages/opinion.py
+-rw-rw-rw-   0        0        0     6513 2023-08-25 07:21:49.000000 moddb-0.9.0/moddb/pages/platform.py
+-rw-rw-rw-   0        0        0     6786 2023-08-25 07:21:49.000000 moddb-0.9.0/moddb/pages/ware.py
+-rw-rw-rw-   0        0        0    14736 2023-08-25 07:21:49.000000 moddb-0.9.0/moddb/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-25 07:31:46.593379 moddb-0.9.0/moddb.egg-info/
+-rw-rw-rw-   0        0        0     2707 2023-08-25 07:31:46.000000 moddb-0.9.0/moddb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1054 2023-08-25 07:31:46.000000 moddb-0.9.0/moddb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-25 07:31:46.000000 moddb-0.9.0/moddb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-08-25 07:31:46.000000 moddb-0.9.0/moddb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-25 07:31:46.000000 moddb-0.9.0/moddb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      163 2023-08-25 07:21:49.000000 moddb-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0       88 2023-08-25 07:21:49.000000 moddb-0.9.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-25 07:31:46.650381 moddb-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1012 2023-08-25 07:30:49.000000 moddb-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-25 07:31:46.648380 moddb-0.9.0/tests/
+-rw-rw-rw-   0        0        0      686 2023-08-25 07:21:49.000000 moddb-0.9.0/tests/test_addon.py
+-rw-rw-rw-   0        0        0      607 2023-08-25 07:21:49.000000 moddb-0.9.0/tests/test_article.py
+-rw-rw-rw-   0        0        0     2489 2023-08-25 07:21:49.000000 moddb-0.9.0/tests/test_base.py
+-rw-rw-rw-   0        0        0     2479 2023-08-25 07:21:50.000000 moddb-0.9.0/tests/test_client.py
+-rw-rw-rw-   0        0        0      272 2023-06-12 11:50:07.000000 moddb-0.9.0/tests/test_config.py
+-rw-rw-rw-   0        0        0      248 2023-08-25 07:21:50.000000 moddb-0.9.0/tests/test_config_template.py
+-rw-rw-rw-   0        0        0     2054 2023-08-25 07:21:50.000000 moddb-0.9.0/tests/test_engine.py
+-rw-rw-rw-   0        0        0      644 2023-08-25 07:21:50.000000 moddb-0.9.0/tests/test_file.py
+-rw-rw-rw-   0        0        0     2437 2023-08-25 07:21:50.000000 moddb-0.9.0/tests/test_game.py
+-rw-rw-rw-   0        0        0     2160 2023-08-25 07:21:50.000000 moddb-0.9.0/tests/test_group.py
+-rw-rw-rw-   0        0        0     2665 2023-08-25 07:21:50.000000 moddb-0.9.0/tests/test_hardware.py
+-rw-rw-rw-   0        0        0      637 2023-08-25 07:21:50.000000 moddb-0.9.0/tests/test_job.py
+-rw-rw-rw-   0        0        0     6417 2023-08-25 07:21:50.000000 moddb-0.9.0/tests/test_main.py
+-rw-rw-rw-   0        0        0      593 2023-08-25 07:21:50.000000 moddb-0.9.0/tests/test_media.py
+-rw-rw-rw-   0        0        0     3394 2023-08-25 07:21:50.000000 moddb-0.9.0/tests/test_member.py
+-rw-rw-rw-   0        0        0     2205 2023-08-25 07:21:50.000000 moddb-0.9.0/tests/test_mod.py
+-rw-rw-rw-   0        0        0     3985 2023-08-25 07:21:50.000000 moddb-0.9.0/tests/test_parse.py
+-rw-rw-rw-   0        0        0     1572 2023-08-25 07:21:50.000000 moddb-0.9.0/tests/test_platform.py
+-rw-rw-rw-   0        0        0      590 2023-08-25 07:21:50.000000 moddb-0.9.0/tests/test_poll.py
+-rw-rw-rw-   0        0        0     2073 2023-08-25 07:21:50.000000 moddb-0.9.0/tests/test_software.py
+-rw-rw-rw-   0        0        0     3074 2023-08-25 07:21:50.000000 moddb-0.9.0/tests/test_team.py
```

### Comparing `moddb-0.8.1/LICENSE` & `moddb-0.9.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Clement
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2023 Clement Julia
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `moddb-0.8.1/PKG-INFO` & `moddb-0.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,73 @@
-Metadata-Version: 2.1
-Name: moddb
-Version: 0.8.1
-Summary: A scrapper for ModDB Mod and Game pages
-Home-page: https://github.com/ClementJ18/moddb
-Author: Clement Julia
-Author-email: clement.julia13@gmail.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ModDB Reader
-**Library is now stable**
-
-The goal of the library is to be able to navigate ModDB purely programmatically through scraping and parsing of the various models present on the website. This is based off a command of my bot which can parse either a game or a mod, this command gave birth to the original library which was extremely limited in its abilities and only able to parse a few pages with inconsistencies. This library is a much more mature and professional attempt at the whole idea, adding on a much deeper understanding of OOP.
-
-## Basic Usage
-The simplest way to use this library is to simply pass a ModDB url to the parse function and let the magic happen.
-```py
-import moddb
-mod = moddb.parse_page("http://www.moddb.com/mods/edain-mod")
-print(mod.name) #Edain Mod
-```
-The library tries to get the type of the url you are passing on its own but due to inconsistencies in the ModDB site this is not always correct, if you desire to be more specific you can pass a ThumbnailType to the function.
-```py
-import moddb
-mod = moddb.parse_page("http://www.moddb.com/mods/edain-mod", page_type=moddb.ThumbnailType.mod)
-print(mod.name) #Edain Mod
-```
-
-## Advanced Usage
-Check out the [documentation](https://moddb.readthedocs.io) for more information
-
-[Support](https://discord.gg/Ape8bZt)
-
-## Installing
-You can get it from pypi: https://pypi.org/project/moddb
-
-```
-pip install moddb
-```
-
-## Models
-* [x] Mod
-* [x] Game  
-* [x] Engine
-* [x] File
-* [x] Media
-* [x] Addon
-* [x] Article
-* [x] Blog
-* [x] User
-* [x] Team
-* [x] Group
-* [x] Job
-* [x] Search Page
-* [x] Front Page
-* [x] Platforms
-* [x] Software
-* [x] HardwAre
-* [x] Updates
-* [x] Friend Requests
-* [ ] Watchers
-* [ ] Tags
-
-Maybe
-* [ ] Messages
-* [ ] Threads
-
-## Glossary
-* **Partial[Model]**: A version of the model which does not contain all the attributes of the full model. Mainly because that model is being displayed as a preview in another page. Not to confuse with Thumbnails, Thumbnails are only guaranteed to contain a name and url of the page.
-* **Boxes**: Containers present on pages, a **div** tag which contains information around a certain theme and as such have been grouped into Box Models of such.
-* **Pages**: Another name for Models.
-* **Thumbnails**: A very widely used model meant to represent models which are references but not expanded onto. Usually the model in question will only include a url and the name of the page. This is transformed into a thumbnail and the user can then parse it with the built-in method.
-
-## Development
-requirement.txt file contains the necessary additional libraries for develompment
+Metadata-Version: 2.1
+Name: moddb
+Version: 0.9.0
+Summary: A scrapper for ModDB Mod and Game pages
+Home-page: https://github.com/ClementJ18/moddb
+Author: Clement Julia
+Author-email: clement.julia13@gmail.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ModDB Reader
+**Library is now stable**
+
+The goal of the library is to be able to navigate ModDB purely programmatically through scraping and parsing of the various models present on the website. This is based off a command of my bot which can parse either a game or a mod, this command gave birth to the original library which was extremely limited in its abilities and only able to parse a few pages with inconsistencies. This library is a much more mature and professional attempt at the whole idea, adding on a much deeper understanding of OOP.
+
+## Basic Usage
+The simplest way to use this library is to simply pass a ModDB url to the parse function and let the magic happen.
+```py
+import moddb
+mod = moddb.parse_page("http://www.moddb.com/mods/edain-mod")
+print(mod.name) #Edain Mod
+```
+
+## Advanced Usage
+Check out the [documentation](https://moddb.readthedocs.io) for more information
+
+[Support](https://discord.gg/Ape8bZt)
+
+## Installing
+You can get it from pypi: https://pypi.org/project/moddb
+
+```
+pip install moddb
+```
+
+## Models
+* [x] Mod
+* [x] Game  
+* [x] Engine
+* [x] File
+* [x] Media
+* [x] Addon
+* [x] Article
+* [x] Blog
+* [x] User
+* [x] Team
+* [x] Group
+* [x] Job
+* [x] Search Page
+* [x] Front Page
+* [x] Platforms
+* [x] Software
+* [x] HardwAre
+* [x] Updates
+* [x] Friend Requests
+* [x] Watchers
+* [x] Tags
+
+Maybe
+* [ ] Messages
+* [ ] Threads
+
+## Glossary
+* **Partial[Model]**: A version of the model which does not contain all the attributes of the full model. Mainly because that model is being displayed as a preview in another page. Not to confuse with Thumbnails, Thumbnails are only guaranteed to contain a name and url of the page.
+* **Boxes**: Containers present on pages, a **div** tag which contains information around a certain theme and as such have been grouped into Box Models of such.
+* **Pages**: Another name for Models.
+* **Thumbnails**: A very widely used model meant to represent models which are references but not expanded onto. Usually the model in question will only include a url and the name of the page. This is transformed into a thumbnail and the user can then parse it with the built-in method.
+
+## Development
+The necessary dependencies are stored in requirements.txt and requirements-dev.txt and can be installed with the following command
+```
+python -m pip install -r requirements.txt -r requirements-dev.txt
+```
```

### Comparing `moddb-0.8.1/README.md` & `moddb-0.9.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,66 +1,63 @@
-# ModDB Reader
-**Library is now stable**
-
-The goal of the library is to be able to navigate ModDB purely programmatically through scraping and parsing of the various models present on the website. This is based off a command of my bot which can parse either a game or a mod, this command gave birth to the original library which was extremely limited in its abilities and only able to parse a few pages with inconsistencies. This library is a much more mature and professional attempt at the whole idea, adding on a much deeper understanding of OOP.
-
-## Basic Usage
-The simplest way to use this library is to simply pass a ModDB url to the parse function and let the magic happen.
-```py
-import moddb
-mod = moddb.parse_page("http://www.moddb.com/mods/edain-mod")
-print(mod.name) #Edain Mod
-```
-The library tries to get the type of the url you are passing on its own but due to inconsistencies in the ModDB site this is not always correct, if you desire to be more specific you can pass a ThumbnailType to the function.
-```py
-import moddb
-mod = moddb.parse_page("http://www.moddb.com/mods/edain-mod", page_type=moddb.ThumbnailType.mod)
-print(mod.name) #Edain Mod
-```
-
-## Advanced Usage
-Check out the [documentation](https://moddb.readthedocs.io) for more information
-
-[Support](https://discord.gg/Ape8bZt)
-
-## Installing
-You can get it from pypi: https://pypi.org/project/moddb
-
-```
-pip install moddb
-```
-
-## Models
-* [x] Mod
-* [x] Game  
-* [x] Engine
-* [x] File
-* [x] Media
-* [x] Addon
-* [x] Article
-* [x] Blog
-* [x] User
-* [x] Team
-* [x] Group
-* [x] Job
-* [x] Search Page
-* [x] Front Page
-* [x] Platforms
-* [x] Software
-* [x] HardwAre
-* [x] Updates
-* [x] Friend Requests
-* [ ] Watchers
-* [ ] Tags
-
-Maybe
-* [ ] Messages
-* [ ] Threads
-
-## Glossary
-* **Partial[Model]**: A version of the model which does not contain all the attributes of the full model. Mainly because that model is being displayed as a preview in another page. Not to confuse with Thumbnails, Thumbnails are only guaranteed to contain a name and url of the page.
-* **Boxes**: Containers present on pages, a **div** tag which contains information around a certain theme and as such have been grouped into Box Models of such.
-* **Pages**: Another name for Models.
-* **Thumbnails**: A very widely used model meant to represent models which are references but not expanded onto. Usually the model in question will only include a url and the name of the page. This is transformed into a thumbnail and the user can then parse it with the built-in method.
-
-## Development
-requirement.txt file contains the necessary additional libraries for develompment
+# ModDB Reader
+**Library is now stable**
+
+The goal of the library is to be able to navigate ModDB purely programmatically through scraping and parsing of the various models present on the website. This is based off a command of my bot which can parse either a game or a mod, this command gave birth to the original library which was extremely limited in its abilities and only able to parse a few pages with inconsistencies. This library is a much more mature and professional attempt at the whole idea, adding on a much deeper understanding of OOP.
+
+## Basic Usage
+The simplest way to use this library is to simply pass a ModDB url to the parse function and let the magic happen.
+```py
+import moddb
+mod = moddb.parse_page("http://www.moddb.com/mods/edain-mod")
+print(mod.name) #Edain Mod
+```
+
+## Advanced Usage
+Check out the [documentation](https://moddb.readthedocs.io) for more information
+
+[Support](https://discord.gg/Ape8bZt)
+
+## Installing
+You can get it from pypi: https://pypi.org/project/moddb
+
+```
+pip install moddb
+```
+
+## Models
+* [x] Mod
+* [x] Game  
+* [x] Engine
+* [x] File
+* [x] Media
+* [x] Addon
+* [x] Article
+* [x] Blog
+* [x] User
+* [x] Team
+* [x] Group
+* [x] Job
+* [x] Search Page
+* [x] Front Page
+* [x] Platforms
+* [x] Software
+* [x] HardwAre
+* [x] Updates
+* [x] Friend Requests
+* [x] Watchers
+* [x] Tags
+
+Maybe
+* [ ] Messages
+* [ ] Threads
+
+## Glossary
+* **Partial[Model]**: A version of the model which does not contain all the attributes of the full model. Mainly because that model is being displayed as a preview in another page. Not to confuse with Thumbnails, Thumbnails are only guaranteed to contain a name and url of the page.
+* **Boxes**: Containers present on pages, a **div** tag which contains information around a certain theme and as such have been grouped into Box Models of such.
+* **Pages**: Another name for Models.
+* **Thumbnails**: A very widely used model meant to represent models which are references but not expanded onto. Usually the model in question will only include a url and the name of the page. This is transformed into a thumbnail and the user can then parse it with the built-in method.
+
+## Development
+The necessary dependencies are stored in requirements.txt and requirements-dev.txt and can be installed with the following command
+```
+python -m pip install -r requirements.txt -r requirements-dev.txt
+```
```

### Comparing `moddb-0.8.1/moddb/boxes.py` & `moddb-0.9.0/moddb/boxes.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1230 +1,1335 @@
-from .enums import (
-    ThumbnailType,
-    SearchCategory,
-    Membership,
-    Licence,
-    Genre,
-    Theme,
-    PlayerStyle,
-    Scope,
-    ArticleCategory,
-    HardwareCategory,
-    Status,
-    SoftwareCategory,
-    AddonCategory,
-    GroupCategory,
-    TeamCategory,
-)
-
-from .utils import (
-    get_date,
-    get_list_stats,
-    get_page,
-    get_views,
-    join,
-    normalize,
-    LOGGER,
-    time_mapping,
-    get_page_type,
-    get,
-)
-
-import re
-import sys
-import toolz
-import datetime
-import collections
-from typing import List, Any, Tuple, Union
-
-__all__ = [
-    "Statistics",
-    "Profile",
-    "Style",
-    "Thumbnail",
-    "Comment",
-    "MissingComment",
-    "MemberProfile",
-    "MemberStatistics",
-    "PlatformStatistics",
-    "PartialArticle",
-    "Option",
-    "Mirror",
-    "ResultList",
-    "CommentList",
-]
-
-
-class Statistics:
-    """The stats box, on pages that have one. This represents total stats and daily stats in one
-    neat package.
-
-    Attributes
-    ----------
-    files : int
-        The number of files this page has uploaded
-    articles : int
-        The number of articles this page has uploaded
-    reviews : int
-        The number of reviews this page has been given
-    watchers : int
-        The number of people following this page
-    mods : int
-        The number of mods this page is related too (only applies to games, members and teams)
-    addons : int
-        The number of addons this page has uploaded
-    members : int
-        The number of members a group has (only applies to groups and teams)
-    visits : int
-        The total number of times this page has been viewed
-    today : int
-        The number of times this page has been viewed today
-    rank : int
-        The current rank of the page against all other pages of the same type
-    total : int
-        The maximum rank number
-    updated : datetime.datetime
-        The last time this page was updated
-    """
-
-    def __init__(self, html):
-        misc = html.find_all(
-            "h5",
-            string=(
-                "Files",
-                "Articles",
-                "Reviews",
-                "Watchers",
-                "Mods",
-                "Addons",
-                "Members",
-            ),
-        )
-        self.__dict__.update({stat.string.lower(): int(normalize(stat.parent.a.string)) for stat in misc})
-
-        visits = normalize(html.find("h5", string="Visits").parent.a.string)
-        self.visits, self.today = get_views(visits)
-
-        rank = normalize(html.find("h5", string="Rank").parent.a.string).split("of")
-        self.rank = int(rank[0].replace(",", ""))
-        self.total = int(rank[1].replace(",", ""))
-
-        try:
-            self.updated = get_date(html.find("time", itemprop="dateModified")["datetime"])
-        except TypeError:
-            self.updated = None
-
-    def __repr__(self):
-        return f"<Statistics rank={self.rank}/{self.total}>"
-
-
-class Profile:
-    """The profile object is used for several models and as such attribute vary based on which model
-    the profile is attached too. Profiles are only present on Mod, Game, Member, Addon, Engine, Company,
-    Hardware, Software and Group pages.
-
-    Parameters
-    -----------
-    html : bs4.BeautifulSoup
-        The html to parse. Allows for finer control.
-
-    Attributes
-    -----------
-    category : Union[AddonCategory, HardwareCategory, SoftwareCategory, TeamCategory, GroupCategory, SearchCategory]
-        The category the page falls under within the context of what the page is. E.g the page is an Addon category
-        will be an AddonCategory enum. If the category of the page doesn't fall under any of the above mentionned
-        the attribute will be of type SearchCategory.
-    contact : str
-        The url to contact the page owner
-    follow : str
-        The url to click to follow the mod
-    share : dict
-        A dictionnary of share links with the place they will be shared as the key and the url
-        for sharing as the value.
-    private : bool
-        Exclusive to Group and Team, True if the group is private, else False
-    membership : Membership
-        Exclusive to Group and Team, represents the join procedure (invitation only, private, public)
-    icon : str
-        Exclusive to Game, Mod and Addon pages. URL of the icon image
-    developers : dict
-        Exclusive to Game, Mods, Engine and Addon pages. Dictionnary of member/team like thumbnails as
-        values and the role of the member/team as the key (creator, publisher, developer, ect...)
-    release : datetime.datetime
-        Exclusive to Game, Mods, Engine and Addon pages. Datetime object of when the page was
-        released, can be None if the page hasn't seen a release yet.
-    homepage : str
-        Present on all pages but Group pages. URL to the page's homepage. Can be None
-    engine : Thumbnail
-        Exclusive to Game and Addon pages. Engine like thumbnails representing the engine the addon/game
-        was built for.
-    game : Thumbnail
-        Exclusive to Mod pages. Game like thumbnail representing the game the mod was built for.
-    licence : Licence
-        Exclusive to Engine and Addon pages. Object representing the licence the engine operates under.
-    platforms : List[Thumbnail]
-        Exclusive to Game, Engine and Addon pages. List of platform like thumbnails representing
-        the plaftorms the software was built for.
-    status : Status
-        Exclusive to Games, Mods, Addons, Engines, Hardware .Whether the thing is released, unreleased, ect...
-
-    """
-
-    def __init__(self, html):
-        try:
-            _name = html.find("a", itemprop="mainEntityOfPage").string
-        except AttributeError:
-            try:
-                _name = html.find("span", itemprop="headline").string
-            except AttributeError:
-                _name = html.find("div", class_="title").h2.a.string
-        try:
-            url = html.find("meta", property="og:url")["content"]
-        except TypeError:
-            url = join(html.find("a", string=self.name)["href"])
-
-        regex = r"\/([a-z]+)\/"
-        matches = re.findall(regex, url)
-        matches.reverse()
-        page_type = SearchCategory[matches[0] if matches[0].endswith("s") else matches[0] + "s"]
-
-        self.category = page_type
-        profile_raw = html.find("span", string="Profile").parent.parent.parent.find(
-            "div", class_="table tablemenu"
-        )
-        self.contact = join(html.find("h5", string="Contact").parent.span.a["href"])
-        self.follow = join(
-            profile_raw.find_all(
-                "h5",
-                string=[
-                    "Mod watch",
-                    "Game watch",
-                    "Group watch",
-                    "Engine watch",
-                    "Hardware watch",
-                    "Software watch",
-                ],
-            )[0].parent.span.a["href"]
-        )
-
-        try:
-            share = profile_raw.find("h5", string="Share").parent.span.find_all("a")
-            self.share = {
-                "reddit": share[0]["href"],
-                "mail": share[1]["href"],
-                "twitter": share[2]["href"],
-                "facebook": share[3]["href"],
-            }
-        except (AttributeError, IndexError):
-            LOGGER.info("Something funky about share box of %s %s", page_type.name, _name)
-            self.share = None
-
-        if page_type in [SearchCategory.developers, SearchCategory.groups]:
-            self.private = profile_raw.find("h5", string="Privacy").parent.span.string.strip() != "Public"
-
-            membership = profile_raw.find("h5", string="Subscription").parent.span.string.strip()
-            if membership == "Open to all members":
-                self.membership = Membership(3)
-            elif membership == "Must apply to join":
-                self.membership = Membership(2)
-            else:
-                self.membership = Membership(1)
-
-        if page_type in [
-            SearchCategory.games,
-            SearchCategory.mods,
-            SearchCategory.addons,
-        ]:
-            try:
-                self.icon = profile_raw.find("h5", string="Icon").parent.span.img["src"]
-            except AttributeError:
-                self.icon = None
-                LOGGER.info("%s '%s' does not have an icon", page_type, _name)
-
-        if page_type in [
-            SearchCategory.games,
-            SearchCategory.mods,
-            SearchCategory.engines,
-            SearchCategory.addons,
-            SearchCategory.hardwares,
-            SearchCategory.softwares,
-        ]:
-            people = profile_raw.find_all(
-                "h5",
-                string=[
-                    "Developer",
-                    "Publisher",
-                    "Developer & Publisher",
-                    "Creator",
-                    "Company",
-                ],
-            )
-            self.developers = {
-                x.string.lower(): Thumbnail(
-                    url=x.parent.a["href"],
-                    name=x.parent.a.string,
-                    type=ThumbnailType.team if x.string != "Creator" else ThumbnailType.member,
-                )
-                for x in people
-            }
-
-            try:
-                d = profile_raw.find("h5", string="Release date").parent.span.time
-                self.release = get_date(d["datetime"])
-            except KeyError:
-                LOGGER.info("%s %s has not been released", page_type.name, _name)
-                self.release = None
-
-            if "Coming" in d.string:
-                self.status = Status.coming_soon
-            elif "Early" in d.string:
-                self.status = Status.early_access
-            elif "Released" in d.string:
-                self.status = Status.released
-            else:
-                self.status = Status.unreleased
-
-            if page_type != SearchCategory.mods:
-                platforms = profile_raw.find("h5", string="Platforms").parent.span.find_all("a")
-                self.platforms = [
-                    Thumbnail(name=x.string, url=x["href"], type=ThumbnailType.platform) for x in platforms
-                ]
-
-        if page_type != SearchCategory.groups:
-            try:
-                self.homepage = html.find("h5", string="Homepage").parent.span.a["href"]
-            except AttributeError:
-                self.homepage = None
-                LOGGER.info("%s %s has no homepage", page_type.name, _name)
-
-        if page_type in [SearchCategory.games, SearchCategory.addons]:
-            engine = profile_raw.find("h5", string="Engine")
-            url = engine.parent.span.a["href"]
-            name = engine.parent.span.a.string
-            self.engine = Thumbnail(url=url, name=name, type=ThumbnailType.engine)
-
-        if page_type == SearchCategory.mods:
-            game = profile_raw.find("h5", string="Game")
-            url = game.parent.span.a["href"]
-            name = game.parent.span.a.string
-            self.game = Thumbnail(url=url, name=name, type=ThumbnailType.game)
-
-        if page_type in [SearchCategory.engines, SearchCategory.addons]:
-            self.licence = Licence(
-                int(profile_raw.find("h5", string="Licence").parent.span.a["href"].split("=")[-1])
-            )
-
-        if page_type == SearchCategory.hardwares:
-            self.category = HardwareCategory(
-                int(profile_raw.find("h5", string="Category").parent.span.a["href"].split("=")[-1])
-            )
-
-        if page_type == SearchCategory.softwares:
-            self.category = SoftwareCategory(
-                int(profile_raw.find("h5", string="Category").parent.span.a["href"].split("=")[-1])
-            )
-
-        if page_type == SearchCategory.addons:
-            self.category = AddonCategory(
-                int(profile_raw.find("h5", string="Category").parent.span.a["href"].split("=")[-1])
-            )
-
-        if page_type == SearchCategory.developers:
-            category = html.find("h3").string.strip().lower()
-            try:
-                self.category = TeamCategory[category]
-            except KeyError:
-                self.category = TeamCategory(7)
-
-        if page_type == SearchCategory.groups:
-            category = html.find("h3").string.strip().lower().replace(" & ", "_")
-            self.category = GroupCategory[category]
-
-    def __repr__(self):
-        return f"<Profile category={self.category.name}>"
-
-
-class Style:
-    """Represents semantic information on the page's theme.
-
-    Parameters
-    -----------
-    html : bs4.BeautifulSoup
-        The html to parse. Allows for finer control.
-
-    Attributes
-    ----------
-    theme : Theme
-        fantasy, sci-fi, ect...
-    genre : Genre
-        fps, rpg, moba, ect...
-    players : PlayerStyle
-        Singplayer, multiplayer, ect...
-    scope : Scope
-        Triple A games or indie
-    boxart : str
-        URL of the boxart for the page.
-    """
-
-    def __init__(self, html):
-        misc = html.find_all("h5", string=("Theme", "Genre", "Players"))
-        styles = {style.string.lower(): re.findall(r"(\d*)$", style.parent.a["href"])[0] for style in misc}
-
-        self.theme = Theme(int(styles["theme"]))
-        self.genre = Genre(int(styles["genre"]))
-        self.players = PlayerStyle(int(styles["theme"]))
-
-        try:
-            self.scope = Scope(int(html.find("h5", string="Project").parent.a["href"][-1]))
-        except AttributeError:
-            LOGGER.info("Has no scope")
-
-        try:
-            self.boxart = html.find("h5", string="Boxart").parent.span.a.img["src"]
-        except AttributeError:
-            LOGGER.info("Has no boxart")
-
-    def __repr__(self):
-        return f"<Style genre={self.genre.name} theme={self.theme.name} players={str(self.players)}>"
-
-
-class Thumbnail:
-    """Thumbnail objects are minature version of ModDB models. They can be parsed to return the full
-    version of the model.
-
-    Attributes
-    -----------
-    url : str
-        The url to the full model, mandatory attribute.
-    name : str
-        The name of the model
-    image : str
-        The optional thumbnail image of the model
-    summary : str
-        Optional bit of fluff
-    date : datetime.datetime
-        A date related to this timestamp if it exists. Can be None
-    type : ThumbnailType
-        The type of the resource, mandatory attribute
-
-    """
-
-    def __init__(self, **attrs):
-        self.url = join(attrs.get("url"))
-        self.name = attrs.get("name", None)
-        self.image = attrs.get("image", None)
-        self.summary = attrs.get("summary", None)
-        self.date = attrs.get("date", None)
-        self.type = attrs.get("type")
-
-    def __repr__(self):
-        return f"<Thumbnail name={self.name} type={self.type.name}>"
-
-    def parse(self) -> Any:
-        """Uses the Thumbnail's mandatory attributes to get the full html of the
-        model and parse them with the appropriate object.
-
-        Returns
-        --------
-        Any
-            The model that was parsed, can be any model from the list of the ThumbnailType
-            enum.
-        """
-        return getattr(sys.modules["moddb"], self.type.name.title())(get_page(self.url))
-
-
-def _parse_results(html):
-    result_box = html.find("div", class_="normalbox browsebox")
-    try:
-        search_raws = (
-            result_box.find("div", class_="inner")
-            .find("div", class_="table")
-            .find_all("div", class_=["rowcontent"])
-        )
-    except AttributeError:
-        return [], 1, 1, 0
-
-    results = []
-    try:
-        for obj in search_raws:
-            date = obj.find("time")
-            summary = obj.find("p")
-            results.append(
-                Thumbnail(
-                    name=obj.a["title"],
-                    url=obj.a["href"],
-                    image=obj.a.img["src"],
-                    type=get_page_type(join(obj.a["href"])),
-                    summary=summary.string if summary else None,
-                    date=get_date(date["datetime"]) if date else None,
-                )
-            )
-    except (TypeError, KeyError):
-        # parse as a title-content pair of articles
-        LOGGER.info("Parsing articles as key-pair list")
-        for title, content in zip(search_raws[::2], search_raws[1::2]):
-            date = title.find("time")
-            url = title.find("h4").a
-            results.append(
-                Thumbnail(
-                    name=url.text,
-                    url=url["href"],
-                    image=None,
-                    type=get_page_type(join(url["href"])),
-                    summary=content.text,
-                    date=get_date(date["datetime"]) if date else None,
-                )
-            )
-
-    current_page, total_page, total_results = get_list_stats(result_box)
-    if total_results is None:
-        total_results = len(results)
-
-    return results, current_page, total_page, total_results
-
-
-def _parse_comments(html):
-    comments = []
-    comment_box = html.find("div", id="comments")
-    if comment_box is None:
-        return [], 1, 1, 0
-
-    current_page, total_page, total_results = get_list_stats(comment_box)
-
-    try:
-        url = html.find("meta", property="og:url")["content"]
-    except TypeError:
-        url = join(html.find("a", itemprop="mainEntityOfPage")["href"])
-
-    comments_raw = comment_box.find("div", class_=["tablecomments"]).find_all(
-        "div", class_="row", recursive=False
-    )
-    if total_results is None:
-        total_results = len(comments_raw)
-
-    for raw in comments_raw:
-        comment = Comment(raw)
-        comment._url = f"{url}/page/{current_page}"
-        if comment.position == 1:
-            try:
-                comments[-1].children.append(comment)
-            except IndexError:
-                comments.append(MissingComment(0))
-                comments[-1].children.append(comment)
-        elif comment.position == 2:
-            try:
-                comments[-1].children[-1].children.append(comment)
-            except IndexError:
-                comments[-1].children.append(MissingComment(1))
-                comments[-1].children[-1].children.append(comment)
-        else:
-            comments.append(comment)
-
-    return comments, current_page, total_page, total_results
-
-
-class Comment:
-    """A moddb comment object.
-
-    Parameters
-    -----------
-    html : bs4.Tag
-        The html to parse into the object. Must be the exact div of the comment.
-
-    Attributes
-    -----------
-    id : int
-        The ID of the comment
-    author : Thumbnail
-        A member like thumbnail of the member who posted the comment
-    date : datetime.datetime
-        Date and time of the comment creation
-    position : int
-        Ranging from 0-2 represents the nested level of the comment.
-    children : int
-        Comment object replying directly to this one. If the comment is
-        parsed on its own it will be null. It is only populated if originating
-        from a CommentList
-    content : str
-        Text of the comment can be none if the comment only contains embeds
-    embeds : list
-        List of urls that have been embeded
-    karma : int
-        The current karma count
-    upvote : str
-        Link to upvote the comment
-    downvote : str
-        Link to downvote the comment
-    approved : bool
-        Whether or not the comment is still waiting for admin approval and is visible to the guest members
-    developer : bool
-        Whether or not the comment was posted one of the page creators
-    staff : bool
-        Wether or not the comment was posted by one of moddb's staff members
-    subscriber : bool
-        Whether or not the comment was posted by a moddb subscriber
-    guest : bool
-        Whether or not the comment was posted by a guest user
-    location : Thumbnail
-        Thumbnail of the place the comment is, only available when getting comments from get_member_comments. This
-        thumbnail does not guarantee that you will find the comment if you parse it, since the url does not
-        contain the page number.
-    """
-
-    def __init__(self, html):
-        author = html.find("a", class_="avatar")
-        self.id = int(html["id"])
-        self.author = Thumbnail(
-            name=author["title"],
-            url=author["href"],
-            image=author.img["src"],
-            type=ThumbnailType.member,
-        )
-        self.date = get_date(html.find("time")["datetime"])
-        actions = html.find("span", class_="actions")
-        self._fetch_time = datetime.datetime.utcnow()
-
-        position = html["class"]
-        if "reply1" in position:
-            self.position = 1
-        elif "reply2" in position:
-            self.position = 2
-        else:
-            self.position = 0
-        self.children = []
-
-        try:
-            links = html.find("div", class_="comment").find_all("a")
-            for link in links:
-                link.string = link["href"]
-            self.content = html.find("div", class_="comment").text
-        except AttributeError:
-            LOGGER.info(
-                "Comment %s by %s has no content, likely embed",
-                self.id,
-                self.author.name,
-            )
-            self.content = None
-
-        try:
-            karma = actions.span.string
-            self.karma = int(re.findall(r"[+-]?\d", karma)[0].replace(",", ""))
-            self.upvote = join(actions.find_all("a")[1]["href"])
-            self.downvote = join(actions.find_all("a")[2]["href"])
-            self.approved = True
-        except AttributeError:
-            self.karma = 0
-            self.upvote = None
-            self.downvote = None
-            self.approved = False
-        except IndexError:
-            self.downvote = None
-            self.approved = True
-
-        self.developer = bool(html.find("span", class_="developer"))
-        self.staff = bool(html.find("span", class_="staff"))
-        self.subscriber = bool(html.find("span", class_="subscriber"))
-        self.guest = self.author.name.lower() == "guest"
-
-        self.embeds = [x["src"] for x in html.find_all("iframe")]
-
-        self.location = html.find("a", class_="related")
-        if self.location is not None:
-            url = join(self.location["href"])
-            page_type = get_page_type(url)
-            self.location = Thumbnail(name=self.location.string, url=url, type=page_type)
-
-        try:
-            self._hash = html.find("a", title=("Delete", "Undelete"))["href"].split("=")[-1]
-        except TypeError:
-            self._hash = None
-
-    def is_stale(self):
-        """Comments are very volatile. If they are pushed onto another page by other comments
-        it becomes impossible to use objects with the previous page number. In addition,
-        calculating the new page number is no possible. Pages do not have a defined size but
-        rather grow and shrink based on sizes of individual comments. Finally, comments
-        also have token that can be used to modify them. These tokens have a hard life of
-        30 minutes from the time of the request. This function puts in place several mechanism
-        to verify wether or not the object can still be trusted.
-
-
-        Returns
-        --------
-        bool
-            True, the comment is stale and you should fetch a new version, False you **should**
-            be good to continue using it.
-        """
-
-        return self._fetch_time + datetime.timedelta(minute=30) > datetime.datetime.utcnow()
-
-    def __repr__(self):
-        return f"<Comment author={self.author.name} position={self.position} approved={self.approved}>"
-
-
-class MissingComment:
-    """An object to represent a missing comment. This used in the cases where a parent comment with
-    children is deleted so that the children may still be accessible, missing comment will have the
-    same attributes as a :class:`.Comment` but they will all be equal to None or False apart from children
-    and the comment position, which will have the children of the comment that was deleted attached to it."""
-
-    def __init__(self, position):
-        self.id = None
-        self.author = None
-        self.date = None
-        self.position = position
-        self.content = None
-        self.karma = 0
-        self.upvote = None
-        self.downvote = None
-        self.approved = False
-        self.children = []
-
-        self.developer = False
-        self.staff = False
-        self.subscriber = False
-        self.guest = False
-        self.embeds = []
-        self.location = None
-
-    def __repr__(self):
-        return f"<MissingComment position={self.position}>"
-
-    def is_stale(self):
-        return True
-
-
-class MemberProfile:
-    """Member profiles are separate entities because they share nothing with the other profile boxes. Where as all
-    other profile boxes share at least 4 attributes, a member shares none.
-
-    Parameters
-    -----------
-    html : bs4.BeautifulSoup
-        The html to parse. Allows for finer control.
-
-    Attributes
-    -----------
-    name : str
-        Name of the member
-    level : int
-        Current level
-    progress : float
-        Percentage progress to next level
-    title : str
-        Member title
-    avatar : str
-        Url of the member avatar
-    online : bool
-        Whether or not the member is currently online
-    last_online :  datetime.datetime
-        None if the member is currently online, datetime the user was last seen online
-    gender : str
-        Gender of the member, can be None
-    homepage : str
-        URL of the member's homepage
-    country : str
-        The member's chosen country
-    follow : str
-        Link to follow a member
-    """
-
-    def __init__(self, html):
-        profile_raw = html.find("span", string="Profile").parent.parent.parent.find(
-            "div", class_="table tablemenu"
-        )
-        level_raw = profile_raw.find("h5", string="Level").parent.span.div
-        self.name = html.find("meta", property="og:title")["content"]
-
-        self.level = int(level_raw.find("span", class_="level").string)
-        self.progress = float("0." + level_raw.find("span", class_="info").strong.string.replace("%", ""))
-        self.title = level_raw.find("span", class_="info").a.string
-
-        self.avatar = profile_raw.find("div", class_="avatarinfo").img["src"]
-        self.online = bool(profile_raw.find("h5", string="Status"))
-        last_online = profile_raw.find("h5", string="Last Online")
-        self.last_online = get_date(last_online.parent.span.time["datetime"]) if last_online else None
-
-        try:
-            self.gender = profile_raw.find("h5", string="Gender").parent.span.string.strip()
-        except AttributeError:
-            LOGGER.info("Member %s has not publicized their gender", self.name)
-            self.gender = None
-
-        try:
-            self.homepage = html.find("h5", string="Homepage").parent.span.a["href"]
-        except AttributeError:
-            self.homepage = None
-            LOGGER.info("Member %s has no homepage", self.name)
-
-        self.country = profile_raw.find("h5", string="Country").parent.span.string.strip()
-
-        try:
-            self.follow = join(profile_raw.find("h5", string="Member watch").parent.span.a["href"])
-        except AttributeError:
-            LOGGER.info("Can't watch yourself, narcissist...")
-            self.follow = None
-
-    def __repr__(self):
-        return f"<MemberProfile name={self.name}>"
-
-
-class MemberStatistics:
-    """Similarly, a member statistics shared no common ground with other stats and therefore there was a
-    need for a separate object.
-
-    Parameters
-    -----------
-    html : bs4.BeautifulSoup
-        The html to parse. Allows for finer control.
-
-    Attributes
-    -----------
-    watchers : int
-        How many members are following this member
-    acivity_points : int
-        Activity points
-    comments : int
-        How many comments the member has made
-    tags : int
-        How many tags the member has created
-    visits : int
-        How many people have viewed this page
-    site_visits : int
-        How many time this user has visited the site
-    today : int
-        How many people have viewed this page today
-    time : int
-        How many seconds the member has spent online
-    rank : int
-        The member's current rank (compared to other members)
-    total : int
-        the maximum rank
-    """
-
-    def __init__(self, html):
-        def get(parent):
-            return parent.a.string.strip() if parent.a else parent.span.string.strip()
-
-        name = html.find("meta", property="og:title")["content"]
-        misc = html.find_all(
-            "h5",
-            string=("Watchers", "Activity Points", "Comments", "Tags", "Site visits"),
-        )
-        self.__dict__.update(
-            {stat.string.lower().replace(" ", "_"): int(normalize(get(stat.parent))) for stat in misc}
-        )
-
-        visits = normalize(html.find("h5", string="Visitors").parent.a.string)
-        self.visits, self.today = get_views(visits)
-
-        time, mapping = html.find("h5", string="Time Online").parent.span.string.strip().split(" ")
-        self.time = time_mapping[mapping.replace("s", "")] * int(time)
-
-        try:
-            rank = normalize(html.find("h5", string="Rank").parent.span.string).split("of")
-            self.rank = int(rank[0].replace(",", ""))
-            self.total = int(rank[1].replace(",", ""))
-        except AttributeError:
-            self.rank = 0
-            self.total = 0
-            LOGGER.info("Member %s has no rank", name)
-
-    def __repr__(self):
-        return f"<MemberStatistics rank={self.rank}/{self.total}>"
-
-
-class PlatformStatistics:
-    """Stats for platform pages.
-
-    Parameters
-    -----------
-    html : bs4.BeautifulSoup
-        The html to parse. Allows for finer control.
-
-    Attributes
-    -----------
-    hardware : int
-        Number of harware created for this platform
-    software : int
-        Number of software created for this platform
-    engines : int
-        Number of engines created for this platform
-    games : int
-        Number of games created for this platform
-    mods : int
-        Number of mods created for this platform
-    """
-
-    def __init__(self, html):
-        headings = ("Hardware", "Software", "Engines", "Games", "Mods")
-        html_headings = html.find_all("h5", string=headings)
-        self.__dict__.update(
-            {
-                headings[html_headings.index(x)].lower(): int(normalize(x.parent.span.a.string))
-                for x in html_headings
-            }
-        )
-
-    def __repr__(self):
-        return "<PlatformStatistics>"
-
-
-class PartialArticle:
-    """A partial article is an article object missing attributes due to being parsed from the front page
-    intead of from the article page itself. In general, it' is simple enough for previewing the article
-    but if you need a full article with comments, profile, ect... Then parse it with the method
-
-    Parameters
-    -----------
-    html : bs4.BeautifulSoup
-        The html to parse. Allows for finer control.
-
-    Attributes
-    -----------
-    name : str
-        Name of the articles
-    url : str
-        Link to the article
-    date : datetime.datetime
-        Date the article was published
-    type : ArticleCategory
-        Type of the article
-    content : str
-        html of the article content
-    plaintext : str
-        plaintext of the article content (without html)
-    """
-
-    def __init__(self, html):
-        meta_raw = html.find("div", class_="row rowcontent rownoimage clear")
-
-        self.name = meta_raw.h4.a.string
-        self.url = join(meta_raw.h4.a["href"])
-        self.date = get_date(meta_raw.find("time")["datetime"])
-        try:
-            self.type = ArticleCategory[
-                meta_raw.find("span", class_="subheading").text.strip().split(" ")[0].lower()
-            ]
-        except KeyError:
-            self.type = ArticleCategory.news
-
-        content = html.find("div", class_="row rowcontent rowcontentnext clear")
-        self.content = str(content)
-        self.plaintext = content.text
-
-    def __repr__(self):
-        return f"<PartialArticle title={self.name}>"
-
-    def get_article(self) -> "Article":
-        """Returns the full article object of this article.
-
-        Returns
-        --------
-        Article
-            The complete article object
-        """
-        return getattr(sys.modules["moddb"], "Article")(get_page(self.url))
-
-
-class Option:
-    """Represents one of the choice from the poll they are attached to, should not be created
-    manually, prefer relying on the Poll.
-
-    Attributes
-    -----------
-    id : int
-        The id of the option, can be None and will be None in most cases.
-    text : str
-        The option's text
-    votes : int
-        The number of votes that have been cast on this option
-    percent : int
-        The percent of all votes that have been cast on this option
-    """
-
-    def __init__(self, **kwargs):
-        self.id = kwargs.get("id", None)
-        self.text = kwargs.get("text")
-        self.votes = kwargs.get("votes")
-        self.percent = kwargs.get("percent")
-
-    def __repr__(self):
-        return f"<Option text={self.text}>"
-
-
-class ModDBList(collections.abc.MutableSequence):
-    """Base List type for the lib
-
-    Attributes
-    -----------
-    current_page : int
-        The page of results this objects represents
-    total_pages : int
-        The total amount of result pages available
-    total_results : int
-        The total amount of results available
-    """
-
-    def __init__(self, **kwargs):
-        self._results = kwargs.pop("results")
-        self._params = kwargs.pop("params", {})
-        self._url = kwargs.pop("url")
-        self.total_pages = kwargs.pop("total_pages")
-        self.current_page = kwargs.pop("current_page")
-        self.total_results = kwargs.pop("total_results")
-
-    def _parse_method(self, html):
-        raise NotImplementedError
-
-    def _do_request(self, **kwargs):
-        page = kwargs.pop("page", self.current_page)
-        params = {**self._params, **kwargs}
-
-        html = get_page(f"{self._url}/page/{page}", params=params)
-        results, current_page, total_pages, total_results = self._parse_method(html)
-
-        return self.__class__(
-            results=results,
-            params=params,
-            url=self._url,
-            total_pages=total_pages,
-            current_page=current_page,
-            total_results=total_results,
-        )
-
-    def next_page(self) -> Union["ResultList", "CommentList"]:
-        """Returns the next page of results as either a CommentList if you are retriving comments or
-        as a ResultList if it's literally anything else.
-
-        Returns
-        --------
-        Union[ResultList, CommentList]
-            The new search objects containing a new set of results.
-
-        Raises
-        -------
-        ValueError
-            There is no next page
-        """
-        if self.current_page == self.total_pages:
-            raise ValueError("Reached last page already")
-
-        return self.to_page(self.current_page + 1)
-
-    def previous_page(self) -> Union["ResultList", "CommentList"]:
-        """Returns the previous page of results as either a CommentList if you are retriving comments or
-        as a ResultList if it's literally anything else.
-
-        Returns
-        --------
-        Union[ResultList, CommentList]
-            The new list-like object of results.
-
-        Raises
-        -------
-        ValueError
-            There is no previous page
-        """
-        if self.current_page == 1:
-            raise ValueError("Reached first page already")
-
-        return self.to_page(self.current_page - 1)
-
-    def to_page(self, page: int) -> Union["ResultList", "CommentList"]:
-        """Returns the desired page of results as either a CommentList if you are retriving comments or
-        as a ResultList if it's literally anything else.
-
-        Parameters
-        -----------
-        page : int
-            A page number within the range 1 - max_page inclusive
-
-        Returns
-        --------
-        Union[ResultList, CommentList]
-            The new list-like object of results.
-
-        Raises
-        -------
-        ValueError
-            This page does not exist
-        """
-        if page < 1 or page > self.total_pages:
-            raise ValueError(f"Please pick a page between 1 and {self.total_pages}")
-
-        return self._do_request(page=page)
-
-    def get_all_results(self):
-        """An expensive methods that iterates over every page of the result query and returns all
-        the results. This may return more results than you expected if new page have fit the criteria
-        while iterating.
-
-        Returns
-        --------
-        Union[CommentList[Any], ResultList[Any]]
-            The list of things you were searching for
-        """
-        search = self.to_page(1)
-        results = list(search)
-
-        while True:
-            try:
-                search = search.next_page()
-            except ValueError:
-                break
-            else:
-                results.extend(search)
-                LOGGER.info("Parsed page %s/%s", search.current_page, search.total_pages)
-
-        def key_check(element):
-            if isinstance(element, Comment):
-                return element.id
-            else:
-                return element.name
-
-        search._results = list(toolz.unique(results, key=key_check))
-        return search
-
-    def __repr__(self):
-        return f"<{self.__class__.__name__} pages={self.current_page}/{self.total_pages}, results={self._results}>"
-
-    def __getitem__(self, element):
-        return self._results.__getitem__(element)
-
-    def __delitem__(self, element):
-        self._results.__delitem__(element)
-
-    def __len__(self):
-        return self._results.__len__()
-
-    def __setitem__(self, key, value):
-        self._results.__setitem__(key, value)
-
-    def insert(self, index, value):
-        self._results.insert(index, value)
-
-
-class ResultList(ModDBList):
-    """Represents a list of result gotten from one of the many get methods the library uses. This is returned
-    over a regular list because it has additional methods that allow for easily go through all the results. In
-    the same way that the moddb site works, you don't have to re-run the query manually to get the next page,
-    you simply click a button, same here, you don't have to recall the base get method, simply use on of the
-    methods here to traverse the results. This emulates a list and will behave like one, so you
-    can use any of the regular list operators in addition to the methods defined below
-
-    Attributes
-    -----------
-    current_page : int
-        The page of results this objects represents
-    total_pages : int
-        The total amount of result pages available
-    total_results : int
-        The total amount of results available
-    """
-
-    def _parse_method(self, html):
-        return _parse_results(html)
-
-    def resort(self, new_sort: Tuple[str, str]) -> "ResultList":
-        """Allows you to sort the whole search by a new sorting parameters. Returns a new search object.
-
-        Parameters
-        -----------
-        new_sort : Tuple[str, str]
-            The new sorting tuple to check by
-
-        Returns
-        -------
-        ResultList
-            The new set of results with the updated sort order
-        """
-        return self._do_request(sort=f"{new_sort[0]}-{new_sort[1]}")
-
-    def __contains__(self, element):
-        return get(self._results, name=element.name) is not None
-
-
-class CommentList(ModDBList):
-    """Represents a list of comments. This emulates a list and will behave like one, so you
-    can use any of the regular list operators in addition to the methods defined below.
-
-    Attributes
-    -----------
-    current_page : int
-        The page of results this objects represents
-    total_pages : int
-        The total amount of result pages available
-    total_results : int
-        The total amount of results available
-    """
-
-    def _parse_method(self, html):
-        return _parse_comments(html)
-
-    def __contains__(self, element):
-        return get(self._results, name=element.name) is not None
-
-    def flatten(self) -> List[Comment]:
-        """Returns a 'flattened' list of comments where children of comments are added right
-        after the parent comment so:
-
-        [ Comment1 ]
-            ├── Comment2\n
-            |   ├── Comment3\n
-            |   └── Comment4\n
-            └── Comment5
-
-        would become:
-
-        [Comment1, Comment2, Comment3, Comment4, Comment5]
-
-        Returns
-        --------
-        List[Comment]
-            The flattened list of comments
-        """
-        top_list = []
-        for comment in self._results:
-            top_list.append(comment)
-            for child in comment.children:
-                top_list.append(child)
-                top_list.extend(child.children)
-
-        return top_list
-
-
-class Mirror:
-    """Represents a download mirror from which the user can download a file
-
-    Attributes
-    -----------
-    name : str
-        The name of the mirror
-    index : int
-        The index of the mirror, as multiple mirrors
-        have the same name. Index starts at 1
-    city : str
-        Alpha 2 code, or full name, of the city the server is located
-        in. Sometimes represents a country.
-    country : str
-        Alpha 2 code for the country the server is
-        located in. Sometimes represents a continent.
-    served : int
-        How many downloads of this file this mirror has
-        served
-    capacity : float
-        The current capacity of this server as a percentage.
-        E.g. 35.5 -> 35.5%. Lower is better for speed.
-    """
-
-    def __init__(self, **kwargs):
-        self.name = kwargs.get("name")
-        self.index = kwargs.get("index")
-        self.city = kwargs.get("city")
-        self.country = kwargs.get("country")
-        self.served = kwargs.get("served")
-        self.capacity = kwargs.get("capacity")
-        self._url = kwargs.get("url")
-
-    def __repr__(self):
-        return f"<Mirror name={self.name} index={self.index} >"
+from __future__ import annotations
+
+import collections
+import datetime
+import re
+import sys
+from typing import TYPE_CHECKING, Any, List, Tuple, Union
+
+import toolz
+from bs4 import BeautifulSoup
+
+from .enums import (
+    AddonCategory,
+    ArticleCategory,
+    Genre,
+    GroupCategory,
+    HardwareCategory,
+    Licence,
+    Membership,
+    PlayerStyle,
+    Scope,
+    SearchCategory,
+    SoftwareCategory,
+    Status,
+    TeamCategory,
+    Theme,
+    ThumbnailType,
+)
+from .utils import (
+    BASE_URL,
+    LOGGER,
+    generate_hash,
+    get,
+    get_date,
+    get_list_stats,
+    get_page,
+    get_page_type,
+    get_siteareaid,
+    get_views,
+    join,
+    normalize,
+    time_mapping,
+)
+
+if TYPE_CHECKING:
+    from .pages.article import Article
+
+__all__ = [
+    "Statistics",
+    "Profile",
+    "Style",
+    "Thumbnail",
+    "Comment",
+    "MissingComment",
+    "MemberProfile",
+    "MemberStatistics",
+    "PlatformStatistics",
+    "PartialArticle",
+    "Option",
+    "Mirror",
+    "ResultList",
+    "CommentList",
+]
+
+
+class Statistics:
+    """The stats box, on pages that have one. This represents total stats and daily stats in one
+    neat package.
+
+    Attributes
+    ----------
+    files : int
+        The number of files this page has uploaded
+    articles : int
+        The number of articles this page has uploaded
+    reviews : int
+        The number of reviews this page has been given
+    watchers : int
+        The number of people following this page
+    mods : int
+        The number of mods this page is related too (only applies to games, members and teams)
+    addons : int
+        The number of addons this page has uploaded
+    members : int
+        The number of members a group has (only applies to groups and teams)
+    visits : int
+        The total number of times this page has been viewed
+    today : int
+        The number of times this page has been viewed today
+    rank : int
+        The current rank of the page against all other pages of the same type
+    total : int
+        The maximum rank number
+    updated : datetime.datetime
+        The last time this page was updated
+    """
+
+    def __init__(self, html: BeautifulSoup):
+        misc = html.find_all(
+            "h5",
+            string=(
+                "Files",
+                "Articles",
+                "Reviews",
+                "Watchers",
+                "Mods",
+                "Addons",
+                "Members",
+            ),
+        )
+        self.__dict__.update(
+            {stat.string.lower(): int(normalize(stat.parent.a.string)) for stat in misc}
+        )
+
+        visits = normalize(html.find("h5", string="Visits").parent.a.string)
+        self.visits, self.today = get_views(visits)
+
+        rank = normalize(html.find("h5", string="Rank").parent.a.string).split("of")
+        self.rank = int(rank[0].replace(",", ""))
+        self.total = int(rank[1].replace(",", ""))
+
+        try:
+            self.updated = get_date(html.find("time", itemprop="dateModified")["datetime"])
+        except TypeError:
+            self.updated = None
+
+    def __repr__(self):
+        return f"<Statistics rank={self.rank}/{self.total}>"
+
+
+class Profile:
+    """The profile object is used for several models and as such attribute vary based on which model
+    the profile is attached too. Profiles are only present on Mod, Game, Member, Addon, Engine, Company,
+    Hardware, Software and Group pages.
+
+    Parameters
+    -----------
+    html : bs4.BeautifulSoup
+        The html to parse. Allows for finer control.
+
+    Attributes
+    -----------
+    category : Union[AddonCategory, HardwareCategory, SoftwareCategory, TeamCategory, GroupCategory, SearchCategory]
+        The category the page falls under within the context of what the page is. E.g the page is an Addon category
+        will be an AddonCategory enum. If the category of the page doesn't fall under any of the above mentionned
+        the attribute will be of type SearchCategory.
+    contact : str
+        The url to contact the page owner
+    follow : str
+        The url to click to follow the mod
+    share : dict
+        A dictionnary of share links with the place they will be shared as the key and the url
+        for sharing as the value.
+    private : bool
+        Exclusive to Group and Team, True if the group is private, else False
+    membership : Membership
+        Exclusive to Group and Team, represents the join procedure (invitation only, private, public)
+    icon : str
+        Exclusive to Game, Mod and Addon pages. URL of the icon image
+    developers : dict
+        Exclusive to Game, Mods, Engine and Addon pages. Dictionnary of member/team like thumbnails as
+        values and the role of the member/team as the key (creator, publisher, developer, ect...)
+    release : datetime.datetime
+        Exclusive to Game, Mods, Engine and Addon pages. Datetime object of when the page was
+        released, can be None if the page hasn't seen a release yet.
+    homepage : str
+        Present on all pages but Group pages. URL to the page's homepage. Can be None
+    engine : Thumbnail
+        Exclusive to Game and Addon pages. Engine like thumbnails representing the engine the addon/game
+        was built for.
+    game : Thumbnail
+        Exclusive to Mod pages. Game like thumbnail representing the game the mod was built for.
+    licence : Licence
+        Exclusive to Engine and Addon pages. Object representing the licence the engine operates under.
+    platforms : List[Thumbnail]
+        Exclusive to Game, Engine and Addon pages. List of platform like thumbnails representing
+        the plaftorms the software was built for.
+    status : Status
+        Exclusive to Games, Mods, Addons, Engines, Hardware .Whether the thing is released, unreleased, ect...
+
+    """
+
+    def __init__(self, html: BeautifulSoup):
+        try:
+            _name = html.find("a", itemprop="mainEntityOfPage").string
+        except AttributeError:
+            try:
+                _name = html.find("span", itemprop="headline").string
+            except AttributeError:
+                _name = html.find("div", class_="title").h2.a.string
+        try:
+            url = html.find("meta", property="og:url")["content"]
+        except TypeError:
+            url = join(html.find("a", string=self.name)["href"])
+
+        regex = r"\/([a-z]+)\/"
+        matches = re.findall(regex, url)
+        matches.reverse()
+        page_type = SearchCategory[matches[0] if matches[0].endswith("s") else matches[0] + "s"]
+
+        self.category = page_type
+        profile_raw = html.find("span", string="Profile").parent.parent.parent.find(
+            "div", class_="table tablemenu"
+        )
+        self.contact = join(html.find("h5", string="Contact").parent.span.a["href"])
+        self.follow = join(
+            profile_raw.find_all(
+                "h5",
+                string=[
+                    "Mod watch",
+                    "Game watch",
+                    "Group watch",
+                    "Engine watch",
+                    "Hardware watch",
+                    "Software watch",
+                ],
+            )[0].parent.span.a["href"]
+        )
+
+        try:
+            share = profile_raw.find("h5", string="Share").parent.span.find_all("a")
+            self.share = {
+                "reddit": share[0]["href"],
+                "mail": share[1]["href"],
+                "twitter": share[2]["href"],
+                "facebook": share[3]["href"],
+            }
+        except (AttributeError, IndexError):
+            LOGGER.info("Something funky about share box of %s %s", page_type.name, _name)
+            self.share = None
+
+        if page_type in [SearchCategory.developers, SearchCategory.groups]:
+            self.private = (
+                profile_raw.find("h5", string="Privacy").parent.span.string.strip() != "Public"
+            )
+
+            membership = profile_raw.find("h5", string="Subscription").parent.span.string.strip()
+            if membership == "Open to all members":
+                self.membership = Membership(3)
+            elif membership == "Must apply to join":
+                self.membership = Membership(2)
+            else:
+                self.membership = Membership(1)
+
+        if page_type in [
+            SearchCategory.games,
+            SearchCategory.mods,
+            SearchCategory.addons,
+        ]:
+            try:
+                self.icon = profile_raw.find("h5", string="Icon").parent.span.img["src"]
+            except AttributeError:
+                self.icon = None
+                LOGGER.info("%s '%s' does not have an icon", page_type, _name)
+
+        if page_type in [
+            SearchCategory.games,
+            SearchCategory.mods,
+            SearchCategory.engines,
+            SearchCategory.addons,
+            SearchCategory.hardwares,
+            SearchCategory.softwares,
+        ]:
+            people = profile_raw.find_all(
+                "h5",
+                string=[
+                    "Developer",
+                    "Publisher",
+                    "Developer & Publisher",
+                    "Creator",
+                    "Company",
+                ],
+            )
+            self.developers = {
+                x.string.lower(): Thumbnail(
+                    url=x.parent.a["href"],
+                    name=x.parent.a.string,
+                    type=ThumbnailType.team if x.string != "Creator" else ThumbnailType.member,
+                )
+                for x in people
+            }
+
+            try:
+                d = profile_raw.find("h5", string="Release date").parent.span.time
+                self.release = get_date(d["datetime"])
+            except KeyError:
+                LOGGER.info("%s %s has not been released", page_type.name, _name)
+                self.release = None
+
+            if "Coming" in d.string:
+                self.status = Status.coming_soon
+            elif "Early" in d.string:
+                self.status = Status.early_access
+            elif "Released" in d.string:
+                self.status = Status.released
+            else:
+                self.status = Status.unreleased
+
+            if page_type != SearchCategory.mods:
+                platforms = profile_raw.find("h5", string="Platforms").parent.span.find_all("a")
+                self.platforms = [
+                    Thumbnail(name=x.string, url=x["href"], type=ThumbnailType.platform)
+                    for x in platforms
+                ]
+
+        if page_type != SearchCategory.groups:
+            try:
+                self.homepage = html.find("h5", string="Homepage").parent.span.a["href"]
+            except AttributeError:
+                self.homepage = None
+                LOGGER.info("%s %s has no homepage", page_type.name, _name)
+
+        if page_type in [SearchCategory.games, SearchCategory.addons]:
+            engine = profile_raw.find("h5", string="Engine")
+            url = engine.parent.span.a["href"]
+            name = engine.parent.span.a.string
+            self.engine = Thumbnail(url=url, name=name, type=ThumbnailType.engine)
+
+        if page_type == SearchCategory.mods:
+            game = profile_raw.find("h5", string="Game")
+            url = game.parent.span.a["href"]
+            name = game.parent.span.a.string
+            self.game = Thumbnail(url=url, name=name, type=ThumbnailType.game)
+
+        if page_type in [SearchCategory.engines, SearchCategory.addons]:
+            self.licence = Licence(
+                int(profile_raw.find("h5", string="Licence").parent.span.a["href"].split("=")[-1])
+            )
+
+        if page_type == SearchCategory.hardwares:
+            self.category = HardwareCategory(
+                int(profile_raw.find("h5", string="Category").parent.span.a["href"].split("=")[-1])
+            )
+
+        if page_type == SearchCategory.softwares:
+            self.category = SoftwareCategory(
+                int(profile_raw.find("h5", string="Category").parent.span.a["href"].split("=")[-1])
+            )
+
+        if page_type == SearchCategory.addons:
+            self.category = AddonCategory(
+                int(profile_raw.find("h5", string="Category").parent.span.a["href"].split("=")[-1])
+            )
+
+        if page_type == SearchCategory.developers:
+            category = html.find("h3").string.strip().lower()
+            try:
+                self.category = TeamCategory[category]
+            except KeyError:
+                self.category = TeamCategory(7)
+
+        if page_type == SearchCategory.groups:
+            category = html.find("h3").string.strip().lower().replace(" & ", "_")
+            self.category = GroupCategory[category]
+
+    def __repr__(self):
+        return f"<Profile category={self.category.name}>"
+
+
+class Style:
+    """Represents semantic information on the page's theme.
+
+    Parameters
+    -----------
+    html : bs4.BeautifulSoup
+        The html to parse. Allows for finer control.
+
+    Attributes
+    ----------
+    theme : Theme
+        fantasy, sci-fi, ect...
+    genre : Genre
+        fps, rpg, moba, ect...
+    players : PlayerStyle
+        Singplayer, multiplayer, ect...
+    scope : Scope
+        Triple A games or indie
+    boxart : str
+        URL of the boxart for the page.
+    """
+
+    def __init__(self, html: BeautifulSoup):
+        misc = html.find_all("h5", string=("Theme", "Genre", "Players"))
+        styles = {
+            style.string.lower(): re.findall(r"(\d*)$", style.parent.a["href"])[0] for style in misc
+        }
+
+        self.theme = Theme(int(styles["theme"]))
+        self.genre = Genre(int(styles["genre"]))
+        self.players = PlayerStyle(int(styles["theme"]))
+
+        try:
+            self.scope = Scope(int(html.find("h5", string="Project").parent.a["href"][-1]))
+        except AttributeError:
+            LOGGER.info("Has no scope")
+
+        try:
+            self.boxart = html.find("h5", string="Boxart").parent.span.a.img["src"]
+        except AttributeError:
+            LOGGER.info("Has no boxart")
+
+    def __repr__(self):
+        return (
+            f"<Style genre={self.genre.name} theme={self.theme.name} players={str(self.players)}>"
+        )
+
+
+class Thumbnail:
+    """Thumbnail objects are minature version of ModDB models. They can be parsed to return the full
+    version of the model.
+
+    Attributes
+    -----------
+    url : str
+        The url to the full model, mandatory attribute.
+    name : str
+        The name of the model
+    image : str
+        The optional thumbnail image of the model
+    summary : str
+        Optional bit of fluff
+    date : datetime.datetime
+        A date related to this timestamp if it exists. Can be None
+    type : ThumbnailType
+        The type of the resource, mandatory attribute
+
+    """
+
+    def __init__(self, **attrs):
+        self.url = join(attrs.get("url"))
+        self.name = attrs.get("name", None)
+        self.image = attrs.get("image", None)
+        self.summary = attrs.get("summary", None)
+        self.date = attrs.get("date", None)
+        self.type = attrs.get("type")
+
+    def __repr__(self):
+        return f"<Thumbnail name={self.name} type={self.type.name}>"
+
+    def parse(self) -> Any:
+        """Uses the Thumbnail's mandatory attributes to get the full html of the
+        model and parse them with the appropriate object.
+
+        Returns
+        --------
+        Any
+            The model that was parsed, can be any model from the list of the ThumbnailType
+            enum.
+        """
+        return getattr(sys.modules["moddb"], self.type.name.title())(get_page(self.url))
+
+
+def _parse_results(html):
+    result_box = html.find("div", class_="normalbox browsebox")
+    try:
+        search_raws = (
+            result_box.find("div", class_="inner")
+            .find("div", class_="table")
+            .find_all("div", class_=["rowcontent"])
+        )
+    except AttributeError:
+        return [], 1, 1, 0
+
+    results = []
+    try:
+        for obj in search_raws:
+            date = obj.find("time")
+            summary = obj.find("p")
+            results.append(
+                Thumbnail(
+                    name=obj.a["title"],
+                    url=obj.a["href"],
+                    image=obj.a.img["src"],
+                    type=get_page_type(join(obj.a["href"])),
+                    summary=summary.string if summary else None,
+                    date=get_date(date["datetime"]) if date else None,
+                )
+            )
+    except (TypeError, KeyError):
+        # parse as a title-content pair of articles
+        LOGGER.info("Parsing articles as key-pair list")
+        for title, content in zip(search_raws[::2], search_raws[1::2]):
+            date = title.find("time")
+            url = title.find("h4").a
+            results.append(
+                Thumbnail(
+                    name=url.text,
+                    url=url["href"],
+                    image=None,
+                    type=get_page_type(join(url["href"])),
+                    summary=content.text,
+                    date=get_date(date["datetime"]) if date else None,
+                )
+            )
+
+    current_page, total_page, total_results = get_list_stats(result_box)
+    if total_results is None:
+        total_results = len(results)
+
+    return results, current_page, total_page, total_results
+
+
+def _parse_comments(html):
+    comments = []
+    comment_box = html.find("div", id="comments")
+    if comment_box is None:
+        return [], 1, 1, 0
+
+    current_page, total_page, total_results = get_list_stats(comment_box)
+
+    try:
+        url = html.find("meta", property="og:url")["content"]
+    except TypeError:
+        url = join(html.find("a", itemprop="mainEntityOfPage")["href"])
+
+    comments_raw = comment_box.find("div", class_=["tablecomments"]).find_all(
+        "div", class_="row", recursive=False
+    )
+    if total_results is None:
+        total_results = len(comments_raw)
+
+    for raw in comments_raw:
+        comment = Comment(raw)
+        comment._url = f"{url}/page/{current_page}"
+        if comment.position == 1:
+            try:
+                comments[-1].children.append(comment)
+            except IndexError:
+                comments.append(MissingComment(0))
+                comments[-1].children.append(comment)
+        elif comment.position == 2:
+            try:
+                comments[-1].children[-1].children.append(comment)
+            except IndexError:
+                comments[-1].children.append(MissingComment(1))
+                comments[-1].children[-1].children.append(comment)
+        else:
+            comments.append(comment)
+
+    return comments, current_page, total_page, total_results
+
+
+class Comment:
+    """A moddb comment object.
+
+    Parameters
+    -----------
+    html : bs4.Tag
+        The html to parse into the object. Must be the exact div of the comment.
+
+    Attributes
+    -----------
+    id : int
+        The ID of the comment
+    author : Thumbnail
+        A member like thumbnail of the member who posted the comment
+    date : datetime.datetime
+        Date and time of the comment creation
+    position : int
+        Ranging from 0-2 represents the nested level of the comment.
+    children : int
+        Comment object replying directly to this one. If the comment is
+        parsed on its own it will be null. It is only populated if originating
+        from a CommentList
+    content : str
+        Text of the comment can be none if the comment only contains embeds
+    embeds : list
+        List of urls that have been embeded
+    karma : int
+        The current karma count
+    upvote : str
+        Link to upvote the comment
+    downvote : str
+        Link to downvote the comment
+    approved : bool
+        Whether or not the comment is still waiting for admin approval and is visible to the guest members
+    developer : bool
+        Whether or not the comment was posted one of the page creators
+    staff : bool
+        Wether or not the comment was posted by one of moddb's staff members
+    subscriber : bool
+        Whether or not the comment was posted by a moddb subscriber
+    guest : bool
+        Whether or not the comment was posted by a guest user
+    location : Thumbnail
+        Thumbnail of the place the comment is, only available when getting comments from get_member_comments. This
+        thumbnail does not guarantee that you will find the comment if you parse it, since the url does not
+        contain the page number.
+    """
+
+    def __init__(self, html: BeautifulSoup):
+        author = html.find("a", class_="avatar")
+        self.id = int(html["id"])
+        self.author = Thumbnail(
+            name=author["title"],
+            url=author["href"],
+            image=author.img["src"],
+            type=ThumbnailType.member,
+        )
+        self.date = get_date(html.find("time")["datetime"])
+        actions = html.find("span", class_="actions")
+        self._fetch_time = datetime.datetime.utcnow()
+
+        position = html["class"]
+        if "reply1" in position:
+            self.position = 1
+        elif "reply2" in position:
+            self.position = 2
+        else:
+            self.position = 0
+        self.children = []
+
+        try:
+            links = html.find("div", class_="comment").find_all("a")
+            for link in links:
+                link.string = link["href"]
+            self.content = html.find("div", class_="comment").text
+        except AttributeError:
+            LOGGER.info(
+                "Comment %s by %s has no content, likely embed",
+                self.id,
+                self.author.name,
+            )
+            self.content = None
+
+        try:
+            karma = actions.span.string
+            self.karma = int(re.findall(r"[+-]?\d", karma)[0].replace(",", ""))
+            self.upvote = join(actions.find_all("a")[1]["href"])
+            self.downvote = join(actions.find_all("a")[2]["href"])
+            self.approved = True
+        except AttributeError:
+            self.karma = 0
+            self.upvote = None
+            self.downvote = None
+            self.approved = False
+        except IndexError:
+            self.downvote = None
+            self.approved = True
+
+        self.developer = bool(html.find("span", class_="developer"))
+        self.staff = bool(html.find("span", class_="staff"))
+        self.subscriber = bool(html.find("span", class_="subscriber"))
+        self.guest = self.author.name.lower() == "guest"
+
+        self.embeds = [x["src"] for x in html.find_all("iframe")]
+
+        self.location = html.find("a", class_="related")
+        if self.location is not None:
+            url = join(self.location["href"])
+            page_type = get_page_type(url)
+            self.location = Thumbnail(name=self.location.string, url=url, type=page_type)
+
+        try:
+            self._hash = html.find("a", title=("Delete", "Undelete"))["href"].split("=")[-1]
+        except TypeError:
+            self._hash = None
+
+    def is_stale(self):
+        """Comments are very volatile. If they are pushed onto another page by other comments
+        it becomes impossible to use objects with the previous page number. In addition,
+        calculating the new page number is not possible. Pages do not have a defined size but
+        rather grow and shrink based on sizes of individual comments. Finally, comments
+        also have token that can be used to modify them. These tokens have a hard life of
+        30 minutes from the time of the request. This function puts in place several mechanism
+        to verify wether or not the object can still be trusted.
+
+
+        Returns
+        --------
+        bool
+            True, the comment is stale and you should fetch a new version, False you **should**
+            be good to continue using it.
+        """
+
+        return self._fetch_time + datetime.timedelta(minute=30) > datetime.datetime.utcnow()
+
+    def __repr__(self):
+        return (
+            f"<Comment author={self.author.name} position={self.position} approved={self.approved}>"
+        )
+
+
+class MissingComment:
+    """An object to represent a missing comment. This is used in the cases where a parent comment with
+    children is deleted so that the children may still be accessible, missing comment will have the
+    same attributes as a :class:`.Comment` but they will all be equal to None or False apart from children
+    and the comment position, which will have the children of the comment that was deleted attached to it.
+    """
+
+    def __init__(self, position):
+        self.id = None
+        self.author = None
+        self.date = None
+        self.position = position
+        self.content = None
+        self.karma = 0
+        self.upvote = None
+        self.downvote = None
+        self.approved = False
+        self.children = []
+
+        self.developer = False
+        self.staff = False
+        self.subscriber = False
+        self.guest = False
+        self.embeds = []
+        self.location = None
+
+    def __repr__(self):
+        return f"<MissingComment position={self.position}>"
+
+    def is_stale(self):
+        return True
+
+
+class MemberProfile:
+    """Member profiles are separate entities because they share nothing with the other profile boxes. Where as all
+    other profile boxes share at least 4 attributes, a member shares none.
+
+    Parameters
+    -----------
+    html : bs4.BeautifulSoup
+        The html to parse. Allows for finer control.
+
+    Attributes
+    -----------
+    name : str
+        Name of the member
+    level : int
+        Current level
+    progress : float
+        Percentage progress to next level
+    title : str
+        Member title
+    avatar : str
+        Url of the member avatar
+    online : bool
+        Whether or not the member is currently online
+    last_online :  datetime.datetime
+        None if the member is currently online, datetime the user was last seen online
+    gender : str
+        Gender of the member, can be None
+    homepage : str
+        URL of the member's homepage
+    country : str
+        The member's chosen country
+    follow : str
+        Link to follow a member
+    """
+
+    def __init__(self, html: BeautifulSoup):
+        profile_raw = html.find("span", string="Profile").parent.parent.parent.find(
+            "div", class_="table tablemenu"
+        )
+        level_raw = profile_raw.find("h5", string="Level").parent.span.div
+        self.name = html.find("meta", property="og:title")["content"]
+
+        self.level = int(level_raw.find("span", class_="level").string)
+        self.progress = float(
+            "0." + level_raw.find("span", class_="info").strong.string.replace("%", "")
+        )
+        self.title = level_raw.find("span", class_="info").a.string
+
+        self.avatar = profile_raw.find("div", class_="avatarinfo").img["src"]
+        self.online = bool(profile_raw.find("h5", string="Status"))
+        last_online = profile_raw.find("h5", string="Last Online")
+        self.last_online = (
+            get_date(last_online.parent.span.time["datetime"]) if last_online else None
+        )
+
+        try:
+            self.gender = profile_raw.find("h5", string="Gender").parent.span.string.strip()
+        except AttributeError:
+            LOGGER.info("Member %s has not publicized their gender", self.name)
+            self.gender = None
+
+        try:
+            self.homepage = html.find("h5", string="Homepage").parent.span.a["href"]
+        except AttributeError:
+            self.homepage = None
+            LOGGER.info("Member %s has no homepage", self.name)
+
+        self.country = profile_raw.find("h5", string="Country").parent.span.string.strip()
+
+        try:
+            self.follow = join(profile_raw.find("h5", string="Member watch").parent.span.a["href"])
+        except AttributeError:
+            LOGGER.info("Can't watch yourself, narcissist...")
+            self.follow = None
+
+    def __repr__(self):
+        return f"<MemberProfile name={self.name}>"
+
+
+class MemberStatistics:
+    """Similarly, a member statistics shared no common ground with other stats and therefore there was a
+    need for a separate object.
+
+    Parameters
+    -----------
+    html : bs4.BeautifulSoup
+        The html to parse. Allows for finer control.
+
+    Attributes
+    -----------
+    watchers : int
+        How many members are following this member
+    acivity_points : int
+        Activity points
+    comments : int
+        How many comments the member has made
+    tags : int
+        How many tags the member has created
+    visits : int
+        How many people have viewed this page
+    site_visits : int
+        How many time this user has visited the site
+    today : int
+        How many people have viewed this page today
+    time : int
+        How many seconds the member has spent online
+    rank : int
+        The member's current rank (compared to other members)
+    total : int
+        the maximum rank
+    """
+
+    def __init__(self, html: BeautifulSoup):
+        def get(parent):
+            return parent.a.string.strip() if parent.a else parent.span.string.strip()
+
+        name = html.find("meta", property="og:title")["content"]
+        misc = html.find_all(
+            "h5",
+            string=("Watchers", "Activity Points", "Comments", "Tags", "Site visits"),
+        )
+        self.__dict__.update(
+            {
+                stat.string.lower().replace(" ", "_"): int(normalize(get(stat.parent)))
+                for stat in misc
+            }
+        )
+
+        visits = normalize(html.find("h5", string="Visitors").parent.a.string)
+        self.visits, self.today = get_views(visits)
+
+        time, mapping = html.find("h5", string="Time Online").parent.span.string.strip().split(" ")
+        self.time = time_mapping[mapping.replace("s", "")] * int(time)
+
+        try:
+            rank = normalize(html.find("h5", string="Rank").parent.span.string).split("of")
+            self.rank = int(rank[0].replace(",", ""))
+            self.total = int(rank[1].replace(",", ""))
+        except AttributeError:
+            self.rank = 0
+            self.total = 0
+            LOGGER.info("Member %s has no rank", name)
+
+    def __repr__(self):
+        return f"<MemberStatistics rank={self.rank}/{self.total}>"
+
+
+class PlatformStatistics:
+    """Stats for platform pages.
+
+    Parameters
+    -----------
+    html : bs4.BeautifulSoup
+        The html to parse. Allows for finer control.
+
+    Attributes
+    -----------
+    hardware : int
+        Number of harware created for this platform
+    software : int
+        Number of software created for this platform
+    engines : int
+        Number of engines created for this platform
+    games : int
+        Number of games created for this platform
+    mods : int
+        Number of mods created for this platform
+    """
+
+    def __init__(self, html: BeautifulSoup):
+        headings = ("Hardware", "Software", "Engines", "Games", "Mods")
+        html_headings = html.find_all("h5", string=headings)
+        self.__dict__.update(
+            {
+                headings[html_headings.index(x)].lower(): int(normalize(x.parent.span.a.string))
+                for x in html_headings
+            }
+        )
+
+    def __repr__(self):
+        return "<PlatformStatistics>"
+
+
+class PartialArticle:
+    """A partial article is an article object missing attributes due to being parsed from the front page
+    intead of from the article page itself. In general, it' is simple enough for previewing the article
+    but if you need a full article with comments, profile, ect... Then parse it with the method
+
+    Parameters
+    -----------
+    html : bs4.BeautifulSoup
+        The html to parse. Allows for finer control.
+
+    Attributes
+    -----------
+    name : str
+        Name of the articles
+    url : str
+        Link to the article
+    date : datetime.datetime
+        Date the article was published
+    type : ArticleCategory
+        Type of the article
+    content : str
+        html of the article content
+    plaintext : str
+        plaintext of the article content (without html)
+    """
+
+    def __init__(self, html: BeautifulSoup):
+        meta_raw = html.find("div", class_="row rowcontent rownoimage clear")
+
+        self.name = meta_raw.h4.a.string
+        self.url = join(meta_raw.h4.a["href"])
+        self.date = get_date(meta_raw.find("time")["datetime"])
+        try:
+            self.type = ArticleCategory[
+                meta_raw.find("span", class_="subheading").text.strip().split(" ")[0].lower()
+            ]
+        except KeyError:
+            self.type = ArticleCategory.news
+
+        content = html.find("div", class_="row rowcontent rowcontentnext clear")
+        self.content = str(content)
+        self.plaintext = content.text
+
+    def __repr__(self):
+        return f"<PartialArticle title={self.name}>"
+
+    def get_article(self) -> Article:
+        """Returns the full article object of this article.
+
+        Returns
+        --------
+        Article
+            The complete article object
+        """
+        from .pages.article import Article
+
+        return Article(get_page(self.url))
+
+
+class Option:
+    """Represents one of the choice from the poll they are attached to, should not be created
+    manually, prefer relying on the Poll.
+
+    Attributes
+    -----------
+    id : int
+        The id of the option, can be None and will be None in most cases.
+    text : str
+        The option's text
+    votes : int
+        The number of votes that have been cast on this option
+    percent : int
+        The percent of all votes that have been cast on this option
+    """
+
+    def __init__(self, **kwargs):
+        self.id = kwargs.get("id", None)
+        self.text = kwargs.get("text")
+        self.votes = kwargs.get("votes")
+        self.percent = kwargs.get("percent")
+
+    def __repr__(self):
+        return f"<Option text={self.text}>"
+
+
+class ModDBList(collections.abc.MutableSequence):
+    """Base List type for the lib
+
+    Attributes
+    -----------
+    current_page : int
+        The page of results this objects represents
+    total_pages : int
+        The total amount of result pages available
+    total_results : int
+        The total amount of results available
+    """
+
+    def __init__(self, **kwargs):
+        self._results = kwargs.pop("results")
+        self._params = kwargs.pop("params", {})
+        self._url = kwargs.pop("url")
+        self.total_pages = kwargs.pop("total_pages")
+        self.current_page = kwargs.pop("current_page")
+        self.total_results = kwargs.pop("total_results")
+
+    def _parse_method(self, html: BeautifulSoup):
+        raise NotImplementedError
+
+    def _do_request(self, **kwargs):
+        page = kwargs.pop("page", self.current_page)
+        params = {**self._params, **kwargs}
+
+        html = get_page(f"{self._url}/page/{page}", params=params)
+        results, current_page, total_pages, total_results = self._parse_method(html)
+
+        return self.__class__(
+            results=results,
+            params=params,
+            url=self._url,
+            total_pages=total_pages,
+            current_page=current_page,
+            total_results=total_results,
+        )
+
+    def next_page(self) -> Union["ResultList", "CommentList"]:
+        """Returns the next page of results as either a CommentList if you are retriving comments or
+        as a ResultList if it's literally anything else.
+
+        Returns
+        --------
+        Union[ResultList, CommentList]
+            The new search objects containing a new set of results.
+
+        Raises
+        -------
+        ValueError
+            There is no next page
+        """
+        if self.current_page == self.total_pages:
+            raise ValueError("Reached last page already")
+
+        return self.to_page(self.current_page + 1)
+
+    def previous_page(self) -> Union["ResultList", "CommentList"]:
+        """Returns the previous page of results as either a CommentList if you are retriving comments or
+        as a ResultList if it's literally anything else.
+
+        Returns
+        --------
+        Union[ResultList, CommentList]
+            The new list-like object of results.
+
+        Raises
+        -------
+        ValueError
+            There is no previous page
+        """
+        if self.current_page == 1:
+            raise ValueError("Reached first page already")
+
+        return self.to_page(self.current_page - 1)
+
+    def to_page(self, page: int) -> Union["ResultList", "CommentList"]:
+        """Returns the desired page of results as either a CommentList if you are retriving comments or
+        as a ResultList if it's literally anything else.
+
+        Parameters
+        -----------
+        page : int
+            A page number within the range 1 - max_page inclusive
+
+        Returns
+        --------
+        Union[ResultList, CommentList]
+            The new list-like object of results.
+
+        Raises
+        -------
+        ValueError
+            This page does not exist
+        """
+        if page < 1 or page > self.total_pages:
+            raise ValueError(f"Please pick a page between 1 and {self.total_pages}")
+
+        return self._do_request(page=page)
+
+    def get_all_results(self):
+        """An expensive methods that iterates over every page of the result query and returns all
+        the results. This may return more results than you expected if new page have fit the criteria
+        while iterating.
+
+        Returns
+        --------
+        Union[CommentList[Any], ResultList[Any]]
+            The list of things you were searching for
+        """
+        search = self.to_page(1)
+        results = list(search)
+
+        while True:
+            try:
+                search = search.next_page()
+            except ValueError:
+                break
+            else:
+                results.extend(search)
+                LOGGER.info("Parsed page %s/%s", search.current_page, search.total_pages)
+
+        def key_check(element):
+            if isinstance(element, Comment):
+                return element.id
+            else:
+                return element.name
+
+        search._results = list(toolz.unique(results, key=key_check))
+        return search
+
+    def __repr__(self):
+        return f"<{self.__class__.__name__} pages={self.current_page}/{self.total_pages}, results={self._results}>"
+
+    def __getitem__(self, element):
+        return self._results.__getitem__(element)
+
+    def __delitem__(self, element):
+        self._results.__delitem__(element)
+
+    def __len__(self):
+        return self._results.__len__()
+
+    def __setitem__(self, key, value):
+        self._results.__setitem__(key, value)
+
+    def insert(self, index, value):
+        self._results.insert(index, value)
+
+
+class ResultList(ModDBList):
+    """Represents a list of result gotten from one of the many get methods the library uses. This is returned
+    over a regular list because it has additional methods that allow for easily go through all the results. In
+    the same way that the moddb site works, you don't have to re-run the query manually to get the next page,
+    you simply click a button, same here, you don't have to recall the base get method, simply use on of the
+    methods here to traverse the results. This emulates a list and will behave like one, so you
+    can use any of the regular list operators in addition to the methods defined below
+
+    Attributes
+    -----------
+    current_page : int
+        The page of results this objects represents
+    total_pages : int
+        The total amount of result pages available
+    total_results : int
+        The total amount of results available
+    """
+
+    def _parse_method(self, html: BeautifulSoup):
+        return _parse_results(html)
+
+    def resort(self, new_sort: Tuple[str, str]) -> "ResultList":
+        """Allows you to sort the whole search by a new sorting parameters. Returns a new search object.
+
+        Parameters
+        -----------
+        new_sort : Tuple[str, str]
+            The new sorting tuple to check by
+
+        Returns
+        -------
+        ResultList
+            The new set of results with the updated sort order
+        """
+        return self._do_request(sort=f"{new_sort[0]}-{new_sort[1]}")
+
+    def __contains__(self, element):
+        return get(self._results, name=element.name) is not None
+
+
+class CommentList(ModDBList):
+    """Represents a list of comments. This emulates a list and will behave like one, so you
+    can use any of the regular list operators in addition to the methods defined below.
+
+    Attributes
+    -----------
+    current_page : int
+        The page of results this objects represents
+    total_pages : int
+        The total amount of result pages available
+    total_results : int
+        The total amount of results available
+    """
+
+    def _parse_method(self, html: BeautifulSoup):
+        return _parse_comments(html)
+
+    def __contains__(self, element):
+        return get(self._results, name=element.name) is not None
+
+    def flatten(self) -> List[Comment]:
+        """Returns a 'flattened' list of comments where children of comments are added right
+        after the parent comment so:
+
+        [ Comment1 ]
+            ├── Comment2\n
+            |   ├── Comment3\n
+            |   └── Comment4\n
+            └── Comment5
+
+        would become:
+
+        [Comment1, Comment2, Comment3, Comment4, Comment5]
+
+        Returns
+        --------
+        List[Comment]
+            The flattened list of comments
+        """
+        top_list = []
+        for comment in self._results:
+            top_list.append(comment)
+            for child in comment.children:
+                top_list.append(child)
+                top_list.extend(child.children)
+
+        return top_list
+
+
+class Mirror:
+    """Represents a download mirror from which the user can download a file
+
+    Attributes
+    -----------
+    name : str
+        The name of the mirror
+    index : int
+        The index of the mirror, as multiple mirrors
+        have the same name. Index starts at 1
+    city : str
+        Alpha 2 code, or full name, of the city the server is located
+        in. Sometimes represents a country.
+    country : str
+        Alpha 2 code for the country the server is
+        located in. Sometimes represents a continent.
+    served : int
+        How many downloads of this file this mirror has
+        served
+    capacity : float
+        The current capacity of this server as a percentage.
+        E.g. 35.5 -> 35.5%. Lower is better for speed.
+    """
+
+    def __init__(self, **kwargs):
+        self.name = kwargs.get("name")
+        self.index = kwargs.get("index")
+        self.city = kwargs.get("city")
+        self.country = kwargs.get("country")
+        self.served = kwargs.get("served")
+        self.capacity = kwargs.get("capacity")
+        self._url = kwargs.get("url")
+
+    def __repr__(self):
+        return f"<Mirror name={self.name} index={self.index} >"
+
+
+PartialTag = collections.namedtuple("PartialTag", "name name_id url")
+
+
+class Tag:
+    """Represents a tag, useful to vote on stuff
+
+    Parameters
+    -----------
+    id : Optional[int]
+        ID of the tag. None if obtained from parsing a page
+    name_id : str
+        Name id of the tag
+    name : str
+        Name of the tag
+    date : Optional[datetime.datetime]
+        Creation date of the tag. None if obtained from parsing a page
+    official : Optional[bool]
+        Whether the tag is official or user created. None if obtained from parsing a page
+    sitearea : int
+        Site area
+    siteareaid : int
+        Site area id
+    positive : int
+        Number of positive votes
+    negative : int
+        Number of negative votes
+    rank : Optiona[int]
+        Rank of the tag in trending. None if obtained from parsing a page
+    url : str
+        Url to the tag
+    """
+
+    def __init__(self, **kwargs):
+        self.id = int(kwargs.pop("id"))
+        self.date = datetime.datetime.fromtimestamp(int(kwargs.pop("date")))
+        self.official = kwargs.pop("official") == "1"
+        self.sitearea = int(kwargs.pop("sitearea"))
+        self.siteareaid = int(kwargs.pop("siteareaid"))
+
+        self.positive = int(kwargs.pop("positive"))
+        self.negative = int(kwargs.pop("negative"))
+
+        self.name_id = kwargs.pop("tagid")
+        self.name = kwargs.pop("tag")
+        self.rank = int(kwargs.pop("trending"))
+        self.url = f"{BASE_URL}/tags/{self.name_id}"
+
+    def __repr__(self) -> str:
+        return f"< Tag id={self.id} name_id={self.name_id} >"
+
+    def _get_members(self):
+        """Get a list of the members that have voted for this tag
+
+        Returns
+        ---------
+        List[Thumbnail]
+            List of member typed thumbnail
+        """
+        LOGGER.warning("_get_members is undocumented and unreliable for the time being")
+        params = {
+            "ajax": "t",
+            "tag": self.name_id,
+            "sitearea": get_siteareaid(self.sitearea),
+            "siteareaid": self.siteareaid,
+            "hash": generate_hash(),
+        }
+
+        resp = get_page(f"{BASE_URL}/tags/ajax/who", params=params)
+
+        return [
+            Thumbnail(url=join(thumb["href"]), name=thumb.string, type=ThumbnailType.member)
+            for thumb in resp.find("div", class_="successboxachtung").find_all("a")
+        ]
```

### Comparing `moddb-0.8.1/moddb/client.py` & `moddb-0.9.0/moddb/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,1110 +1,1174 @@
-import re
-import sys
-import random
-from typing import Any, List, Tuple, Union
-from pyrate_limiter import Duration, Limiter, RequestRate
-import requests
-
-from .utils import (
-    concat_docs,
-    generate_login_cookies,
-    join,
-    soup,
-    get_page_type,
-    get_date,
-    BASE_URL,
-    generate_hash,
-    get,
-    LOGGER,
-    user_agent_list,
-    raise_for_status,
-    LIMITER,
-)
-from .boxes import Thumbnail, Comment, ResultList, _parse_results
-from .pages import Member, Review, Mod, Game, Engine, Group, Team
-from .enums import ThumbnailType, WatchType, Status
-from .errors import ModdbException
-from .base import parse_page
-
-COMMENT_LIMITER = Limiter(RequestRate(1, Duration.MINUTE))
-
-
-class Message:
-    """A single message within a thread.
-
-    Attributes
-    ----------
-    id : int
-        The id of the message
-    member : Thumbnail
-        A member type thumbnail representing the member
-        who sent the message
-    timestamp : datetime.datetime
-        Message send date
-    text : str
-        The html text of the message
-    """
-
-    def __init__(self, html):
-        member = html.find("a", class_="avatar")
-
-        self.id = int(html["id"])
-        self.member = Thumbnail(url=member["href"], type=ThumbnailType.member, name=member["title"])
-        self.timestamp = get_date(html.find("time")["datetime"])
-        self.text = html.find("div", class_="comment").text
-
-    def __repr__(self):
-        return f"< Message member={self.member} >"
-
-
-class Thread:
-    """A thread is a conversation between two or more members in which
-    one or more messages can be sent.
-
-    Sorting
-    --------
-        * **id** - when the message was sent, asc is oldest, desc is most recent
-        * **name** - order alphabetically, asc is a-z, desc is z-a
-        * **hasread** - order by whether or the message has been read, asc is unread first, desc is read first
-        * **hasreplied** - order by whether or not you have replied to the message, asc us unreplied first, desc is replied first
-
-    Attributes
-    -----------
-    name : str
-        Name of the thread
-    id : int
-        Id of the thread
-    count : int
-        The number of messages in this thread
-    members : List[Tumbnail]
-        All the members participating in the thread. Note: The
-        thumbnail of the member who fetched the message will always
-        be first and will have their name attribute be 'you' instead
-        of the username
-    message : List[Message]
-        The messages associated to this thread
-    """
-
-    def __init__(self, html):
-        thread = html.find("div", id="firstmessage")
-        header = thread.find("div", class_="normalcorner")
-
-        header_string = header.find("span", class_="heading").string
-        header_match = re.match(r"(.*) \(([0-9]*) messages?\)", header_string)
-        if header_match is None:
-            self.name = header_string
-            self.count = 1
-        else:
-            self.name = header_match.group(1)
-            self.count = int(header_match.group(2))
-
-        members = thread.find("p", class_="introduction").strong.find_all("a")
-        option = header.find("a", class_=["deleteicon"])
-        messages = thread.find("div", class_=["tablecomments"]).find_all("div", recursive=False)
-
-        self.id = int(option["href"][option["href"].index("=") + 1 :])
-        self.members = [
-            Thumbnail(url=member["href"], name=member.string, type=ThumbnailType.member) for member in members
-        ]
-        self.messages = [Message(message) for message in messages]
-
-    def __repr__(self):
-        return f"< Thread name={self.name} count={self.count} >"
-
-
-class ThreadThumbnail:
-    """The thumbnail of a thread, these represent partial objects that
-    must be parsed using a client to get the full thread.
-
-    Attributes
-    -----------
-    name : str
-        The name of the thread
-    id : int
-        The id of the thread
-    url : str
-        The url for the thread
-    last_messager : Thumbnail
-        A thumbnail representig the user that sent the
-        last message
-    timestamp : datetime.datetime
-        Datetime of the last message
-    content : str
-        Content of the last message. Useful for checking
-        the last message without having to parse the thread.
-    """
-
-    def __init__(self, **kwargs):
-        self.name = kwargs.get("name")
-        self.url = join(kwargs.get("url"))
-        self.last_messager = kwargs.get("last_messager")
-        self.timestamp = kwargs.get("timestamp")
-        self.content = kwargs.get("content")
-        self.id = int(self.url.split("/")[-1])
-
-    def __repr__(self):
-        return f"< ThreadThumbnail name={self.name} last_messager={self.last_messager} >"
-
-
-@concat_docs
-class Update(Thumbnail):
-    """An update object. Which is basically just a fancy thumbnail with a couple extra attributes and
-    methods.
-
-    Attributes
-    -----------
-    updates : List[Thumbnail]
-        A list of thumbnail objects of the things thave have been posted (new files, new images)
-    """
-
-    def __init__(self, **attrs):
-        super().__init__(**attrs)
-
-        self.updates = attrs.get("updates")
-        self._unfollow_url = join(attrs.get("unfollow"))
-        self._clear_url = join(attrs.get("clear"))
-        self._client = attrs.get("client")
-
-    def __repr__(self):
-        return f"<Update name={self.name} type={self.type.name} updates={len(self.updates)}>"
-
-    def clear(self) -> bool:
-        """Clears all updates
-
-        Raises
-        -------
-        ModdbException
-            An error has occured while trying to clear the updates for this page
-
-        Returns
-        --------
-        bool
-            True if the updates were successfully cleared
-        """
-        r = self._client._request("POST", self._clear_url, data={"ajax": "t"})
-
-        return "successfully removed" in r.json()["text"]
-
-    def unfollow(self) -> bool:
-        """Unfollows the page. This will also clear the updates
-
-        Raises
-        -------
-        ModdbException
-            An error has occured while trying to unfollow this page
-
-        Returns
-        --------
-        bool
-            True if the page was successfully unfollowed
-        """
-        r = self._client._request("POST", self._unfollow_url, data={"ajax": "t"})
-
-        return "no longer watching" in r.json()["text"]
-
-
-@concat_docs
-class Request(Thumbnail):
-    """A thumbnail with two extra methods used to clear and accept requests.
-
-    Attributes
-    -----------
-    """
-
-    def __init__(self, **attrs):
-        super().__init__(**attrs)
-
-        self._decline = join(attrs.get("decline"))
-        self._accept = join(attrs.get("accept"))
-        self._client = attrs.get("client")
-
-    def accept(self) -> bool:
-        """Accept the friend request.
-
-        Raises
-        -------
-        ModdbException
-            An error has occured while trying to accept the request
-
-        Returns
-        --------
-        bool
-            True if the request was successfully accepted
-        """
-        r = self._client._request("POST", self._accept, data={"ajax": "t"})
-
-        return "now friends with" in r.json()["text"]
-
-    def decline(self) -> bool:
-        """Decline the friend request
-
-        Raises
-        -------
-        ModdbException
-            An error has occured while trying to decline the request
-
-        Returns
-        --------
-        bool
-            True if the page was successfully declined
-        """
-        r = self._client._request("POST", self._decline, data={"ajax": "t"})
-
-        return "successfully removed" in r.json()["text"]
-
-    def __repr__(self):
-        return f"<Request from={self.name}>"
-
-
-class Client:
-    """Login the user to moddb through the library, this allows user to see guest comments and see
-    private groups they are part of. In addition, this can be used for a lot of the operation
-
-    Parameters
-    -----------
-    username : str
-        The username of the user
-
-    password : str
-        The password associated to that username
-
-    Raises
-    -------
-    ValueError
-        The password or username was incorrect
-
-    Attributes
-    ----------
-    member : Member
-        The member objects this client instance represents
-    """
-
-    def __init__(self, username: str, password: str):
-        session = requests.Session()
-        session.cookies = generate_login_cookies(username, password)
-        self._session = session
-        LOGGER.info("Login successful for %s", username)
-
-        self.member = Member(
-            soup(self._request("GET", f"{BASE_URL}/members/{username.replace('_', '-')}").text)
-        )
-
-    def __repr__(self):
-        return f"<Client username={self.member.name} level={self.member.profile.level}>"
-
-    def __enter__(self):
-        self._fake_session = sys.modules["moddb"].SESSION
-        sys.modules["moddb"].SESSION = self._session
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        sys.modules["moddb"].SESSION = self._fake_session
-        delattr(self, "_fake_session")
-
-    @LIMITER.ratelimit("moddb", delay=True)
-    def _request(self, method, url, **kwargs):
-        """Making sure we do our request with the cookies from this client rather than the cookies
-        of the library."""
-        cookies = cookies = requests.utils.dict_from_cookiejar(self._session.cookies)
-        headers = {
-            **kwargs.pop("headers", {}),
-            "User-Agent": random.choice(user_agent_list),
-        }
-
-        req = requests.Request(method, url, headers=headers, cookies=cookies, data=kwargs.pop("data", {}))
-        prepped = self._session.prepare_request(req)
-        LOGGER.info("Request: %s", prepped.url)
-
-        r = self._session.send(prepped, allow_redirects=kwargs.pop("allow_redirects", True))
-        raise_for_status(r)
-
-        return r
-
-    def get_updates(self) -> List[Update]:
-        """Get the current updates the user has for models they are subscribed to.
-
-        Returns
-        --------
-        List[Update]
-            List of updates (thumbnail like objects with extra methods and an extra attribute)
-        """
-        r = self._request("GET", f"{BASE_URL}/messages/updates")
-        html = soup(r.text)
-        updates = []
-
-        strings = (
-            "Mods Watch",
-            "Members Watch",
-            "Engines Watch",
-            "Groups Watch",
-            "Games Watch",
-        )
-        raw = html.find_all("span", string=strings)
-        objects = [
-            e.parent.parent.parent.find("div", class_="table").find_all("div", recursive=False) for e in raw
-        ]
-
-        objects_raw = [item for sublist in objects for item in sublist[:-1]]
-        for update in objects_raw:
-            thumbnail = update.find("a")
-            unfollow = update.find("a", title="Stop Watching")["href"]
-            clear = update.find("a", title="Clear")["href"]
-            updates_raw = update.find("p").find_all("a")
-
-            updates.append(
-                Update(
-                    name=thumbnail["title"],
-                    url=thumbnail["href"],
-                    type=get_page_type(thumbnail["href"]),
-                    image=thumbnail.img["src"],
-                    client=self,
-                    unfollow=unfollow,
-                    clear=clear,
-                    updates=[
-                        Thumbnail(name=x.string, url=x["href"], type=get_page_type(x["href"]))
-                        for x in updates_raw
-                    ],
-                    date=get_date(update.find("time")["datetime"]),
-                )
-            )
-
-        return updates
-
-    def clear_updates(self, category: WatchType) -> bool:
-        """Clear all updates for a specific category of
-        watched. This method will conduct two requests because
-        the clear update request requires a hash generated by
-        moddb.
-
-        Parameters
-        -----------
-        category: WatchType
-            The category of watched to clear
-
-        Returns
-        --------
-        bool
-            Whether or not the clear was successful
-        """
-        hash_page = self._request("GET", f"{BASE_URL}/messages/updates")
-        html = soup(hash_page.text)
-        pattern = re.compile(rf".*\/clearall\/(.*)\/1\/{category.name}s")
-        link = html.find("a", href=pattern)
-        if link is None:
-            return True
-
-        r = self._request("POST", f'{BASE_URL}{link["href"]}', data={"ajax": "t"})
-
-        return "updates were cleared" in r.json()["text"]
-
-    def get_friend_requests(self) -> List[Request]:
-        """Get the current friend requests the user has.
-
-        Returns
-        --------
-        List[Request]
-            List of requests (thumbnail like objects with extra methods)
-        """
-        r = self._request("GET", f"{BASE_URL}/messages/updates")
-        html = soup(r.text)
-        requests = []
-        raw = html.find("span", string="Friend Requests")
-        raw_requests = raw.parent.parent.parent.find("div", class_="table").find_all("div", recursive=False)
-
-        for request in raw_requests[:-1]:
-            thumbnail = request.find("a")
-            accept = request.find("a", title="Accept")["href"]
-            decline = request.find("a", title="Decline")["href"]
-
-            requests.append(
-                Request(
-                    name=thumbnail["title"],
-                    url=thumbnail["href"],
-                    type=get_page_type(thumbnail["href"]),
-                    image=thumbnail.img["src"],
-                    client=self,
-                    accept=accept,
-                    decline=decline,
-                    date=get_date(request.find("time")["datetime"]),
-                )
-            )
-
-        return requests
-
-    def get_watched(self, category: WatchType, page: int = 1) -> ResultList:
-        """Get a list of thumbnails of watched items based on the type parameters. Eventually, you'll also be
-        able to paginate your mods.
-
-        Parameters
-        -----------
-        category : WatchType
-            The type of watched thing you wanna get (mod, games, engines)
-        page : int
-            The page number you want to get
-
-        Returns
-        --------
-        ResultList[Thumbnail]
-            List of watched things
-
-        """
-        url = f"{BASE_URL}/messages/watching/{category.name}s"
-        html = soup(self._request("GET", f"{url}/page/{page}").text)
-        results, current_page, total_pages, total_results = _parse_results(html)
-
-        return ResultList(
-            results=results,
-            url=url,
-            current_page=current_page,
-            total_pages=total_pages,
-            total_results=total_results,
-        )
-
-    def tracking(self, page: Union[Mod, Game, Engine, Group, Member]) -> bool:
-        """Follow/unfollow this page.
-
-        Parameters
-        -----------
-        page : Union[Mod, Game, Engine, Group, Member]
-            The page you wish to watch/unwatch
-
-        Raises
-        -------
-        ModdbException
-            An error has occured while trying to follow/unfollow the page
-
-        Returns
-        --------
-        bool
-            True if the page has been successfully followed, False if it has been successfully unfollowed
-        """
-        r = self._request(
-            "POST",
-            f"{BASE_URL}/messages/ajax/action/",
-            data={
-                "ajax": "t",
-                "action": "watch",
-                "sitearea": page.url.split("/")[-2],
-                "siteareaid": page.id,
-            },
-            allow_redirects=False,
-        )
-
-        return "be notified" in r.json()["text"]
-
-    def like_comment(self, comment: Comment) -> bool:
-        """Like a comment, if the comment has already been liked nothing will happen.
-
-        Parameters
-        -----------
-        comment : Comment
-            The comment to like
-
-        Raises
-        -------
-        ModdbException
-            An error has occured while trying to like the comment
-
-        Returns
-        --------
-        bool
-            True if the comment has been successfully liked
-        """
-        r = self._request(
-            "POST",
-            f"{BASE_URL}/messages/ajax/action/",
-            data={
-                "ajax": "t",
-                "action": "karmagood",
-                "sitearea": "comment",
-                "siteareaid": comment.id,
-            },
-            allow_redirects=False,
-        )
-
-        return "successfully issued" in r.json()["text"]
-
-    def dislike_comment(self, comment: Comment) -> bool:
-        """Dislike a comment, if the comment has already been disliked nothing will happen.
-
-        Parameters
-        -----------
-        comment : Comment
-            The comment to dislike
-
-        Raises
-        -------
-        ModdbException
-            An error has occured while trying to dislike the comment
-
-        Returns
-        --------
-        bool
-            True if comment has been successfully disliked.
-        """
-        if not hasattr(comment, "downvote"):
-            raise TypeError("Argument must be a Comment-like object")
-
-        r = self._request(
-            "POST",
-            f"{BASE_URL}/messages/ajax/action/",
-            data={
-                "ajax": "t",
-                "action": "karmabad",
-                "sitearea": "comment",
-                "siteareaid": comment.id,
-            },
-            allow_redirects=False,
-        )
-
-        return "successfully issued" in r.json()["text"]
-
-    def membership(self, page: Union[Group, Team]) -> bool:
-        """Join/leave a team
-
-        Parameters
-        -----------
-        page : Union[Group, Team]
-            The team/group you want to join. Will not work if you don't have permissions
-
-        Raises
-        -------
-        ModdbException
-            An error has occured while trying to join/leave the group/team
-
-        Returns
-        --------
-        bool
-            True if the group/team has been successfully joined, False if the group/team has been
-            successfully left.
-
-        """
-        r = self._request(
-            "POST",
-            f"{BASE_URL}/groups/ajax/members/change/{page.id}",
-            data={"ajax": "t"},
-            allow_redirects=False,
-        )
-
-        return "successfully joined" in r.json()["text"]
-
-    def report(self, page: Any) -> bool:
-        """Report a page. This can take any object that has an id and url attribute.
-
-        Parameters
-        -----------
-        page : Any
-            The page to report
-
-        Raises
-        -------
-        ModdbException
-            An error has occured while trying to report the page
-
-        Returns
-        --------
-        bool
-            True if the page has been successfully reported
-        """
-        r = self._request(
-            "POST",
-            f"{BASE_URL}/messages/ajax/action/",
-            data={
-                "ajax": "t",
-                "action": "report",
-                "sitearea": page.url.split("/")[-2],
-                "siteareaid": page.id,
-            },
-            allow_redirects=False,
-        )
-
-        return "already reported this content" not in r.json()["text"]
-
-    def unfriend(self, member: Member) -> bool:
-        """Unfriend this member if you are friends with them.
-
-        Parameters
-        -----------
-        member : Member
-            The member you wish to unfriend
-
-        Raises
-        -------
-        ModdbException
-            An error has occured trying to unfriend this user
-
-        Returns
-        --------
-        bool
-            True if the user was succesfully unfriended
-        """
-        r = self._request(
-            "POST",
-            f"{BASE_URL}/members/ajax/friends/delete/{member.id}",
-            data={"ajax": "t"},
-            allow_redirects=False,
-        )
-
-        return "no longer friends with this member" in r.json()["text"]
-
-    def send_request(self, member: Member) -> bool:
-        """Send a friend request to a user. You will not instantly become friends with them,
-        they will have to accept the friend request you sent them first.
-
-        Parameters
-        -----------
-        member : Member
-            The member you wish to send a friend request to
-
-        Raises
-        -------
-        ModdbException
-            An error has occured trying to send a friend request to that user
-
-        Returns
-        --------
-        bool
-            True if the user was succesfully sent a friend request
-        """
-        r = self._request(
-            "POST",
-            f"{BASE_URL}/members/ajax/friends/add/{member.id}",
-            data={"ajax": "t"},
-            allow_redirects=False,
-        )
-
-        return "friend request has been sent" in r.json()["text"]
-
-    def add_comment(self, page: Any, text: str, *, comment: str = None) -> Any:
-        """Add a comment to a page.
-
-        Parameters
-        -----------
-        page : Any
-            Must be a moddb.page, the page you wish to add the comment to.
-        test : str
-            The content of the comment you wish to post
-        comment : Optional[Comment]
-            If you wish to reply to another comment you must provide the comment
-            object for it there.
-
-        Returns
-        --------
-        Any
-            The page's updated object containing the new comment and any other new data that
-            has been posted since then
-        """
-        COMMENT_LIMITER.try_acquire(self.member.name_id, delay=True)
-        r = self._request(
-            "POST",
-            page.url,
-            data={
-                "formhash": generate_hash(),
-                "replyid": comment.id if comment else 0,
-                "page": 1,
-                "summary": text,
-                "comment": "Save comment",
-            },
-        )
-
-        return page.__class__(soup(r.text))
-
-    def _comment_state_update(self, comment):
-        if comment is None:
-            raise ModdbException(
-                "This comment no longer exists or is no longer on the page it was initially retrieved from."
-            )
-
-        r = self._request(
-            "POST",
-            f"{BASE_URL}/messages/ajax/action/",
-            data={
-                "ajax": "t",
-                "action": "delete",
-                "sitearea": "comment",
-                "siteareaid": comment.id,
-                "hash": comment._hash,
-            },
-            allow_redirects=False,
-        )
-
-        return r
-
-    def delete_comment(self, comment: Comment) -> bool:
-        """This will delete the supplied comment provided you have the correct permissions.
-        This is an expensive request because if how moddb works. It needs to make two requests
-        in order to get the correct hash to delete the comment. In addition, it may fail if the
-        comment has changed location (page number) from what the object says. It is recommended
-        to use a newly created comment object that is less than 30 minutes old.
-
-        Parameters
-        -----------
-        comment : Comment
-            The comment to delete
-
-        Raises
-        -------
-        ModdbException
-            An error occured while trying to delete the comment
-
-        Returns
-        --------
-        bool
-            True if the comment was successfully deleted
-        """
-        with self:
-            page = parse_page(comment._url)
-            updated_comment = get(page.comments, id=comment.id)
-
-        r = self._comment_state_update(updated_comment)
-
-        return "You have <u>deleted</u> this comment" in r.json()["text"]
-
-    def undelete_comment(self, comment: Comment) -> bool:
-        """This will undelete the supplied comment provided you have the correct permissions.
-        This is an expensive request because of how moddb works. It needs to make three requests
-        in order to get the correct hash to undelete the comment. In addition, it may fail if the
-        comment has changed location (page number) from what the object says. It is recommended
-        to use a newly created comment object that is less than 30 minutes old.
-
-        Parameters
-        -----------
-        comment : Comment
-            The comment to undelete
-
-        Raises
-        -------
-        ModdbException
-            An error occured while trying to undelete the comment
-
-        Returns
-        --------
-        bool
-            True if the comment was successfully undeleted
-        """
-        with self:
-            page = parse_page(comment._url)
-            updated_comment = get(
-                page._get_comments_from_url(comment._url, show_deleted=True),
-                id=comment.id,
-            )
-
-        r = self._comment_state_update(updated_comment)
-
-        return "You have <u>authorized</u> this comment" in r.json()["text"]
-
-    def edit_comment(self, comment: Comment, new_text: str) -> bool:
-        """Edit the contents of a comment. You can only edit your comment 120 minutes after it has
-        been posted
-
-        Parameters
-        -----------
-        comment : Comment
-            The comment to edit
-        new_text : str
-            The new content of the comment
-
-        Raises
-        -------
-        ModdbException
-            An error has occured trying to edit the comment
-
-        Returns
-        --------
-        bool
-            True if the comment was successfully edited
-        """
-        r = self._request(
-            "POST",
-            f"{BASE_URL}/comment/ajax/post",
-            data={"ajax": "t", "id": comment.id, "summary": new_text},
-        )
-
-        return "Your comment has been saved" in r.json()["text"]
-
-    def add_review(self, page: Any, rating: int, *, text: str = None, has_spoilers: bool = False) -> bool:
-        """Rate and review a page. If you rating is below 3 or above 8 you will be asked
-        to also provide a review or else the request will not be made. This is also
-        used to edit existing reviews.
-
-        Parameters
-        -----------
-        page : Union[Mod, Game, Engine, Hardware, Software, Platform]
-            The page you wish to review
-        rating : int
-            The rating from 1 to 10
-        text : str
-            The text review you are giving of this page
-        has_spoilers : bool
-            Whether or not this review contains spoilers.
-
-        Raises
-        -------
-        ModdbException
-            An error occured trying to review the page.
-
-        Returns
-        --------
-        bool
-            True of the review was successfuly submitted.
-
-        """
-        if not (2 < rating < 9) and text is None:
-            raise ModdbException("Please include a review to justify such a low/high rating.")
-
-        with self:
-            page = parse_page(page.url)
-
-        r = self._request(
-            "POST",
-            f"{BASE_URL}/reviews/ajax",
-            data={
-                "ajax": "t",
-                "sitearea": page.url.split("/")[-2],
-                "siteareaid": page.id,
-                "hash": page._review_hash,
-                "earlyaccess": int(page.profile.status == Status.early_access),
-                "rating": rating,
-                "summary": text,
-                "spoiler": int(has_spoilers),
-            },
-            allow_redirects=False,
-        )
-
-        return "Your rating has been saved" in r.json()["text"]
-
-    def delete_review(self, review: Review) -> bool:
-        """Delete your review on the given page. This function will do two requests in order
-        to delete your review.
-
-        Parameters
-        -----------
-        review : Review
-            The review you wish to delete
-
-        Raises
-        -------
-        ModdbException
-            An error occured while trying to delete the review
-
-        Returns
-        --------
-        bool
-            True if the review was successfully deleted
-        """
-        with self:
-            hash_review = self.member.get_reviews()[0]
-
-        r = self._request(
-            "POST",
-            f"{BASE_URL}/messages/ajax/action/",
-            data={
-                "ajax": "t",
-                "action": "delete",
-                "sitearea": "reviews",
-                "siteareaid": review.id,
-                "hash": hash_review._hash,
-                "ispd": 1,
-            },
-            allow_redirects=False,
-        )
-
-        return "You have <u>deleted</u> this review." in r.json()["text"]
-
-    def get_threads(
-        self,
-        query: str = None,
-        read: bool = None,
-        replied: bool = None,
-        sent_items: bool = False,
-        sort: Tuple[str, str] = None,
-    ) -> List[ThreadThumbnail]:
-        """Get all the messages this user has sent or received. This does not return threads you
-        have left.
-
-        Parameters
-        -----------
-        query : Optional[str]
-            Optional query to filter messages
-        read : Optional[bool]
-            True to filter only read message, false to filter unread, None to allow both
-        replied : Optional[bool]
-            True to filter messages where you are the last message, False for messages
-            where another user is the last message, None for both.
-        sent_items:
-            Get only the threads you have started
-        sort : Tuple[str, str]
-            Optional sort tuple to order threads
-
-        Returns
-        --------
-        List[ThreadThumbnail]
-            Thread typed thumbnails
-        """
-        if sent_items:
-            url = f"{BASE_URL}/messages/sentitems"
-        else:
-            url = f"{BASE_URL}/messages/inbox"
-
-        r = self._request(
-            "GET",
-            url,
-            params={
-                "filter": "t",
-                "kw": query,
-                "hasread": int(read) if read is not None else read,
-                "hasreplied": int(replied) if replied is not None else replied,
-                "sort": f"{sort[0]}-{sort[1]}" if sort is not None else sort,
-            },
-        )
-        html = soup(r.text)
-
-        threads_raw = html.find_all("div", class_=["tabinbox"])[-1].find_all("div", class_=["rowcontent"])
-        threads = []
-        for thread in threads_raw:
-            member = thread.find("span", class_="subheading").find_all("a")[0]
-            threads.append(
-                ThreadThumbnail(
-                    url=thread.a["href"],
-                    name=thread.a["title"],
-                    last_messager=Thumbnail(
-                        type=ThumbnailType.member, name=member.string, url=member["href"]
-                    ),
-                    timestamp=get_date(thread.find("time")["datetime"]),
-                    content=thread.find("div", class_="content").find("p").string,
-                )
-            )
-
-        return threads
-
-    def parse_thread(self, thread: ThreadThumbnail) -> Thread:
-        """Parse a thread thumbnail into a full thread object.
-
-        Parameters
-        ----------
-        thread : ThreadThumbnail
-            The thumbnail to parse
-
-        Returns
-        --------
-        Thread
-            The parsed thread and its messages
-        """
-        r = self._request("GET", thread.url)
-
-        return Thread(soup(r.text))
-
-    def send_message(self, members: List[Member], name: str, message: str) -> Thread:
-        """Send a message and start a thread with one or more members
-
-        Parameters
-        ----------
-        member : List[Member]
-            The members to send the message to and start the
-            thread with
-        name : str
-            The subject of the message
-        message : str
-            The message to send
-
-        Returns
-        --------
-        Thread
-            The thread started from sending this message
-        """
-        r = self._request(
-            "POST",
-            f"{BASE_URL}/messages/compose/",
-            data={
-                "formhash": generate_hash(),
-                "membersto": ",".join(member.name for member in members),
-                "name": name,
-                "description": message,
-                "messages": "Send+message",
-            },
-        )
-
-        return Thread(soup(r.text))
-
-    def reply_to_thread(self, thread: Union[Thread, ThreadThumbnail], text: str) -> Thread:
-        """Add an additional message to an exiting thread
-
-        Parameters
-        -----------
-        thread : Union[Thread, ThreadThumbnail]
-            The thread to add the message to
-        text : str
-            The text to send
-
-        Returns
-        --------
-        Thread
-            The updated thread containing the new message. It is
-            recommended to use this object as it also contains
-            a new hash for sending another message
-        """
-        r = self._request(
-            "POST",
-            f"{BASE_URL}/messages/inbox/{thread.id}",
-            data={"formhash": generate_hash(), "description": text, "messages": "Send+message"},
-        )
-
-        return Thread(soup(r.text))
-
-    def add_member_to_thread(self, thread: Union[Thread, ThreadThumbnail], member: Member) -> bool:
-        """Add a member to a conversation
-
-        Parameters
-        -----------
-        thread : Union[Thread, ThreadThumbnail]
-            The thread to add add a member to
-        member : Member
-            The member to add
-
-        Returns
-        --------
-        bool
-            Whether adding the member was succesful. This
-            will not update the thread.
-        """
-        r = self._request(
-            "POST",
-            f"{BASE_URL}/messages/ajax/members/invite/{thread.id}",
-            data={"ajax": "t", "username": member.name, "member": "0"},
-            allow_redirects=False,
-        )
-
-        return "has been successfully added" in r.json()["text"]
-
-    def leave_thread(self, thread: Union[Thread, ThreadThumbnail]) -> bool:
-        """Leave a thread, you will not get any more notifications on this thread.
-
-        Parameters
-        ----------
-        thread : Union[Thread, ThreadThumbnail]
-            The thread to leave
-
-        Returns
-        --------
-        bool
-            Whether leaving the thread was successful
-        """
-        r = self._request(
-            "POST",
-            f"{BASE_URL}/messages/ajax/delete/",
-            data={"ajax": "t", "thread": thread.id},
-            allow_redirects=False,
-        )
-
-        return "You have successfully deleted the requested thread" in r.json()["text"]
-
-    def mark_all_read(self) -> bool:
-        """Mark all threads as read.
-
-        Returns
-        --------
-        bool
-            True if all threads have been marked as read
-        """
-        r = self._request("POST", f"{BASE_URL}/messages/ajax/markallread", data={"ajax": "t"})
-
-        return "All messages marked as read" in r.json()["text"]
+from __future__ import annotations
+
+import random
+import re
+import sys
+from typing import TYPE_CHECKING, Any, List, Tuple, Union
+
+import requests
+from bs4 import BeautifulSoup
+from pyrate_limiter import Duration, Limiter, RequestRate
+
+from .base import parse_page
+from .boxes import ResultList, Thumbnail, _parse_results
+from .enums import Status, ThumbnailType
+from .errors import ModdbException
+from .pages import Member
+from .utils import (
+    BASE_URL,
+    LIMITER,
+    LOGGER,
+    concat_docs,
+    generate_hash,
+    generate_login_cookies,
+    get,
+    get_date,
+    get_page_type,
+    get_sitearea,
+    get_siteareaid,
+    join,
+    raise_for_status,
+    soup,
+    user_agent_list,
+)
+
+if TYPE_CHECKING:
+    from .boxes import Comment, Tag
+    from .enums import WatchType
+    from .pages import Engine, Game, Group, Mod, Review, Team
+
+COMMENT_LIMITER = Limiter(RequestRate(1, Duration.MINUTE))
+
+
+class Message:
+    """A single message within a thread.
+
+    Attributes
+    ----------
+    id : int
+        The id of the message
+    member : Thumbnail
+        A member type thumbnail representing the member
+        who sent the message
+    timestamp : datetime.datetime
+        Message send date
+    text : str
+        The html text of the message
+    """
+
+    def __init__(self, html: BeautifulSoup):
+        member = html.find("a", class_="avatar")
+
+        self.id = int(html["id"])
+        self.member = Thumbnail(url=member["href"], type=ThumbnailType.member, name=member["title"])
+        self.timestamp = get_date(html.find("time")["datetime"])
+        self.text = html.find("div", class_="comment").text
+
+    def __repr__(self):
+        return f"< Message member={self.member} >"
+
+
+class Thread:
+    """A thread is a conversation between two or more members in which
+    one or more messages can be sent.
+
+    Sorting
+    --------
+        * **id** - when the message was sent, asc is oldest, desc is most recent
+        * **name** - order alphabetically, asc is a-z, desc is z-a
+        * **hasread** - order by whether or the message has been read, asc is unread first, desc is read first
+        * **hasreplied** - order by whether or not you have replied to the message, asc us unreplied first, desc is replied first
+
+    Attributes
+    -----------
+    name : str
+        Name of the thread
+    id : int
+        Id of the thread
+    count : int
+        The number of messages in this thread
+    members : List[Tumbnail]
+        All the members participating in the thread. Note: The
+        thumbnail of the member who fetched the message will always
+        be first and will have their name attribute be 'you' instead
+        of the username
+    message : List[Message]
+        The messages associated to this thread
+    """
+
+    def __init__(self, html: BeautifulSoup):
+        thread = html.find("div", id="firstmessage")
+        header = thread.find("div", class_="normalcorner")
+
+        header_string = header.find("span", class_="heading").string
+        header_match = re.match(r"(.*) \(([0-9]*) messages?\)", header_string)
+        if header_match is None:
+            self.name = header_string
+            self.count = 1
+        else:
+            self.name = header_match.group(1)
+            self.count = int(header_match.group(2))
+
+        members = thread.find("p", class_="introduction").strong.find_all("a")
+        option = header.find("a", class_=["deleteicon"])
+        messages = thread.find("div", class_=["tablecomments"]).find_all("div", recursive=False)
+
+        self.id = int(option["href"][option["href"].index("=") + 1 :])
+        self.members = [
+            Thumbnail(url=member["href"], name=member.string, type=ThumbnailType.member)
+            for member in members
+        ]
+        self.messages = [Message(message) for message in messages]
+
+    def __repr__(self):
+        return f"< Thread name={self.name} count={self.count} >"
+
+
+class ThreadThumbnail:
+    """The thumbnail of a thread, these represent partial objects that
+    must be parsed using a client to get the full thread.
+
+    Attributes
+    -----------
+    name : str
+        The name of the thread
+    id : int
+        The id of the thread
+    url : str
+        The url for the thread
+    last_messager : Thumbnail
+        A thumbnail representig the user that sent the
+        last message
+    timestamp : datetime.datetime
+        Datetime of the last message
+    content : str
+        Content of the last message. Useful for checking
+        the last message without having to parse the thread.
+    """
+
+    def __init__(self, **kwargs):
+        self.name = kwargs.get("name")
+        self.url = join(kwargs.get("url"))
+        self.last_messager = kwargs.get("last_messager")
+        self.timestamp = kwargs.get("timestamp")
+        self.content = kwargs.get("content")
+        self.id = int(self.url.split("/")[-1])
+
+    def __repr__(self):
+        return f"< ThreadThumbnail name={self.name} last_messager={self.last_messager} >"
+
+
+@concat_docs
+class Update(Thumbnail):
+    """An update object. Which is basically just a fancy thumbnail with a couple extra attributes and
+    methods.
+
+    Attributes
+    -----------
+    updates : List[Thumbnail]
+        A list of thumbnail objects of the things thave have been posted (new files, new images)
+    """
+
+    def __init__(self, **attrs):
+        super().__init__(**attrs)
+
+        self.updates = attrs.get("updates")
+        self._unfollow_url = join(attrs.get("unfollow"))
+        self._clear_url = join(attrs.get("clear"))
+        self._client = attrs.get("client")
+
+    def __repr__(self):
+        return f"<Update name={self.name} type={self.type.name} updates={len(self.updates)}>"
+
+    def clear(self) -> bool:
+        """Clears all updates
+
+        Raises
+        -------
+        ModdbException
+            An error has occured while trying to clear the updates for this page
+
+        Returns
+        --------
+        bool
+            True if the updates were successfully cleared
+        """
+        r = self._client._request("POST", self._clear_url, data={"ajax": "t"})
+
+        return "successfully removed" in r.json()["text"]
+
+    def unfollow(self) -> bool:
+        """Unfollows the page. This will also clear the updates
+
+        Raises
+        -------
+        ModdbException
+            An error has occured while trying to unfollow this page
+
+        Returns
+        --------
+        bool
+            True if the page was successfully unfollowed
+        """
+        r = self._client._request("POST", self._unfollow_url, data={"ajax": "t"})
+
+        return "no longer watching" in r.json()["text"]
+
+
+@concat_docs
+class Request(Thumbnail):
+    """A thumbnail with two extra methods used to clear and accept requests.
+
+    Attributes
+    -----------
+    """
+
+    def __init__(self, **attrs):
+        super().__init__(**attrs)
+
+        self._decline = join(attrs.get("decline"))
+        self._accept = join(attrs.get("accept"))
+        self._client = attrs.get("client")
+
+    def accept(self) -> bool:
+        """Accept the friend request.
+
+        Raises
+        -------
+        ModdbException
+            An error has occured while trying to accept the request
+
+        Returns
+        --------
+        bool
+            True if the request was successfully accepted
+        """
+        r = self._client._request("POST", self._accept, data={"ajax": "t"})
+
+        return "now friends with" in r.json()["text"]
+
+    def decline(self) -> bool:
+        """Decline the friend request
+
+        Raises
+        -------
+        ModdbException
+            An error has occured while trying to decline the request
+
+        Returns
+        --------
+        bool
+            True if the page was successfully declined
+        """
+        r = self._client._request("POST", self._decline, data={"ajax": "t"})
+
+        return "successfully removed" in r.json()["text"]
+
+    def __repr__(self):
+        return f"<Request from={self.name}>"
+
+
+class Client:
+    """Login the user to moddb through the library, this allows user to see guest comments and see
+    private groups they are part of. In addition, this can be used for a lot of the operation
+
+    Parameters
+    -----------
+    username : str
+        The username of the user
+
+    password : str
+        The password associated to that username
+
+    Raises
+    -------
+    ValueError
+        The password or username was incorrect
+
+    Attributes
+    ----------
+    member : Member
+        The member objects this client instance represents
+    """
+
+    def __init__(self, username: str, password: str):
+        session = requests.Session()
+        session.cookies = generate_login_cookies(username, password)
+        self._session = session
+        LOGGER.info("Login successful for %s", username)
+
+        self.member = Member(
+            soup(self._request("GET", f"{BASE_URL}/members/{username.replace('_', '-')}").text)
+        )
+
+    def __repr__(self):
+        return f"<Client username={self.member.name} level={self.member.profile.level}>"
+
+    def __enter__(self):
+        self._fake_session = sys.modules["moddb"].SESSION
+        sys.modules["moddb"].SESSION = self._session
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        sys.modules["moddb"].SESSION = self._fake_session
+        delattr(self, "_fake_session")
+
+    @LIMITER.ratelimit("moddb", delay=True)
+    def _request(self, method, url, **kwargs):
+        """Making sure we do our request with the cookies from this client rather than the cookies
+        of the library."""
+        cookies = cookies = requests.utils.dict_from_cookiejar(self._session.cookies)
+        headers = {
+            **kwargs.pop("headers", {}),
+            "User-Agent": random.choice(user_agent_list),
+        }
+
+        req = requests.Request(
+            method, url, headers=headers, cookies=cookies, data=kwargs.pop("data", {})
+        )
+        prepped = self._session.prepare_request(req)
+        LOGGER.info("Request: %s", prepped.url)
+
+        r = self._session.send(prepped, allow_redirects=kwargs.pop("allow_redirects", True))
+        raise_for_status(r)
+
+        return r
+
+    def get_updates(self) -> List[Update]:
+        """Get the current updates the user has for models they are subscribed to.
+
+        Returns
+        --------
+        List[Update]
+            List of updates (thumbnail like objects with extra methods and an extra attribute)
+        """
+        r = self._request("GET", f"{BASE_URL}/messages/updates")
+        html = soup(r.text)
+        updates = []
+
+        strings = (
+            "Mods Watch",
+            "Members Watch",
+            "Engines Watch",
+            "Groups Watch",
+            "Games Watch",
+        )
+        raw = html.find_all("span", string=strings)
+        objects = [
+            e.parent.parent.parent.find("div", class_="table").find_all("div", recursive=False)
+            for e in raw
+        ]
+
+        objects_raw = [item for sublist in objects for item in sublist[:-1]]
+        for update in objects_raw:
+            thumbnail = update.find("a")
+            unfollow = update.find("a", title="Stop Watching")["href"]
+            clear = update.find("a", title="Clear")["href"]
+            updates_raw = update.find("p").find_all("a")
+
+            updates.append(
+                Update(
+                    name=thumbnail["title"],
+                    url=thumbnail["href"],
+                    type=get_page_type(thumbnail["href"]),
+                    image=thumbnail.img["src"],
+                    client=self,
+                    unfollow=unfollow,
+                    clear=clear,
+                    updates=[
+                        Thumbnail(name=x.string, url=x["href"], type=get_page_type(x["href"]))
+                        for x in updates_raw
+                    ],
+                    date=get_date(update.find("time")["datetime"]),
+                )
+            )
+
+        return updates
+
+    def clear_updates(self, category: WatchType) -> bool:
+        """Clear all updates for a specific category of
+        watched. This method will conduct two requests because
+        the clear update request requires a hash generated by
+        moddb.
+
+        Parameters
+        -----------
+        category: WatchType
+            The category of watched to clear
+
+        Returns
+        --------
+        bool
+            Whether or not the clear was successful
+        """
+        hash_page = self._request("GET", f"{BASE_URL}/messages/updates")
+        html = soup(hash_page.text)
+        pattern = re.compile(rf".*\/clearall\/(.*)\/1\/{category.name}s")
+        link = html.find("a", href=pattern)
+        if link is None:
+            return True
+
+        r = self._request("POST", f'{BASE_URL}{link["href"]}', data={"ajax": "t"})
+
+        return "updates were cleared" in r.json()["text"]
+
+    def get_friend_requests(self) -> List[Request]:
+        """Get the current friend requests the user has.
+
+        Returns
+        --------
+        List[Request]
+            List of requests (thumbnail like objects with extra methods)
+        """
+        r = self._request("GET", f"{BASE_URL}/messages/updates")
+        html = soup(r.text)
+        requests = []
+        raw = html.find("span", string="Friend Requests")
+        raw_requests = raw.parent.parent.parent.find("div", class_="table").find_all(
+            "div", recursive=False
+        )
+
+        for request in raw_requests[:-1]:
+            thumbnail = request.find("a")
+            accept = request.find("a", title="Accept")["href"]
+            decline = request.find("a", title="Decline")["href"]
+
+            requests.append(
+                Request(
+                    name=thumbnail["title"],
+                    url=thumbnail["href"],
+                    type=get_page_type(thumbnail["href"]),
+                    image=thumbnail.img["src"],
+                    client=self,
+                    accept=accept,
+                    decline=decline,
+                    date=get_date(request.find("time")["datetime"]),
+                )
+            )
+
+        return requests
+
+    def get_watched(self, category: WatchType, page: int = 1) -> ResultList:
+        """Get a list of thumbnails of watched items based on the type parameters. Eventually, you'll also be
+        able to paginate your mods.
+
+        Parameters
+        -----------
+        category : WatchType
+            The type of watched thing you wanna get (mod, games, engines)
+        page : int
+            The page number you want to get
+
+        Returns
+        --------
+        ResultList[Thumbnail]
+            List of watched things
+
+        """
+        url = f"{BASE_URL}/messages/watching/{category.name}s"
+        html = soup(self._request("GET", f"{url}/page/{page}").text)
+        results, current_page, total_pages, total_results = _parse_results(html)
+
+        return ResultList(
+            results=results,
+            url=url,
+            current_page=current_page,
+            total_pages=total_pages,
+            total_results=total_results,
+        )
+
+    def tracking(self, page: Union[Mod, Game, Engine, Group, Member]) -> bool:
+        """Follow/unfollow this page.
+
+        Parameters
+        -----------
+        page : Union[Mod, Game, Engine, Group, Member]
+            The page you wish to watch/unwatch
+
+        Raises
+        -------
+        ModdbException
+            An error has occured while trying to follow/unfollow the page
+
+        Returns
+        --------
+        bool
+            True if the page has been successfully followed, False if it has been successfully unfollowed
+        """
+        r = self._request(
+            "POST",
+            f"{BASE_URL}/messages/ajax/action/",
+            data={
+                "ajax": "t",
+                "action": "watch",
+                "sitearea": get_sitearea(page.url),
+                "siteareaid": page.id,
+            },
+            allow_redirects=False,
+        )
+
+        return "be notified" in r.json()["text"]
+
+    def like_comment(self, comment: Comment) -> bool:
+        """Like a comment, if the comment has already been liked nothing will happen.
+
+        Parameters
+        -----------
+        comment : Comment
+            The comment to like
+
+        Raises
+        -------
+        ModdbException
+            An error has occured while trying to like the comment
+
+        Returns
+        --------
+        bool
+            True if the comment has been successfully liked
+        """
+        r = self._request(
+            "POST",
+            f"{BASE_URL}/messages/ajax/action/",
+            data={
+                "ajax": "t",
+                "action": "karmagood",
+                "sitearea": "comment",
+                "siteareaid": comment.id,
+            },
+            allow_redirects=False,
+        )
+
+        return "successfully issued" in r.json()["text"]
+
+    def dislike_comment(self, comment: Comment) -> bool:
+        """Dislike a comment, if the comment has already been disliked nothing will happen.
+
+        Parameters
+        -----------
+        comment : Comment
+            The comment to dislike
+
+        Raises
+        -------
+        ModdbException
+            An error has occured while trying to dislike the comment
+
+        Returns
+        --------
+        bool
+            True if comment has been successfully disliked.
+        """
+        if not hasattr(comment, "downvote"):
+            raise TypeError("Argument must be a Comment-like object")
+
+        r = self._request(
+            "POST",
+            f"{BASE_URL}/messages/ajax/action/",
+            data={
+                "ajax": "t",
+                "action": "karmabad",
+                "sitearea": "comment",
+                "siteareaid": comment.id,
+            },
+            allow_redirects=False,
+        )
+
+        return "successfully issued" in r.json()["text"]
+
+    def membership(self, page: Union[Group, Team]) -> bool:
+        """Join/leave a team
+
+        Parameters
+        -----------
+        page : Union[Group, Team]
+            The team/group you want to join. Will not work if you don't have permissions
+
+        Raises
+        -------
+        ModdbException
+            An error has occured while trying to join/leave the group/team
+
+        Returns
+        --------
+        bool
+            True if the group/team has been successfully joined, False if the group/team has been
+            successfully left.
+
+        """
+        r = self._request(
+            "POST",
+            f"{BASE_URL}/groups/ajax/members/change/{page.id}",
+            data={"ajax": "t"},
+            allow_redirects=False,
+        )
+
+        return "successfully joined" in r.json()["text"]
+
+    def report(self, page: Any) -> bool:
+        """Report a page. This can take any object that has an id and url attribute.
+
+        Parameters
+        -----------
+        page : Any
+            The page to report
+
+        Raises
+        -------
+        ModdbException
+            An error has occured while trying to report the page
+
+        Returns
+        --------
+        bool
+            True if the page has been successfully reported
+        """
+        r = self._request(
+            "POST",
+            f"{BASE_URL}/messages/ajax/action/",
+            data={
+                "ajax": "t",
+                "action": "report",
+                "sitearea": get_sitearea(page.url),
+                "siteareaid": page.id,
+            },
+            allow_redirects=False,
+        )
+
+        return "already reported this content" not in r.json()["text"]
+
+    def unfriend(self, member: Member) -> bool:
+        """Unfriend this member if you are friends with them.
+
+        Parameters
+        -----------
+        member : Member
+            The member you wish to unfriend
+
+        Raises
+        -------
+        ModdbException
+            An error has occured trying to unfriend this user
+
+        Returns
+        --------
+        bool
+            True if the user was succesfully unfriended
+        """
+        r = self._request(
+            "POST",
+            f"{BASE_URL}/members/ajax/friends/delete/{member.id}",
+            data={"ajax": "t"},
+            allow_redirects=False,
+        )
+
+        return "no longer friends with this member" in r.json()["text"]
+
+    def send_request(self, member: Member) -> bool:
+        """Send a friend request to a user. You will not instantly become friends with them,
+        they will have to accept the friend request you sent them first.
+
+        Parameters
+        -----------
+        member : Member
+            The member you wish to send a friend request to
+
+        Raises
+        -------
+        ModdbException
+            An error has occured trying to send a friend request to that user
+
+        Returns
+        --------
+        bool
+            True if the user was succesfully sent a friend request
+        """
+        r = self._request(
+            "POST",
+            f"{BASE_URL}/members/ajax/friends/add/{member.id}",
+            data={"ajax": "t"},
+            allow_redirects=False,
+        )
+
+        return "friend request has been sent" in r.json()["text"]
+
+    def add_comment(self, page: Any, text: str, *, comment: str = None) -> Any:
+        """Add a comment to a page.
+
+        Parameters
+        -----------
+        page : Any
+            Must be a moddb.page, the page you wish to add the comment to.
+        test : str
+            The content of the comment you wish to post
+        comment : Optional[Comment]
+            If you wish to reply to another comment you must provide the comment
+            object for it there.
+
+        Returns
+        --------
+        Any
+            The page's updated object containing the new comment and any other new data that
+            has been posted since then
+        """
+        COMMENT_LIMITER.try_acquire(self.member.name_id, delay=True)
+        r = self._request(
+            "POST",
+            page.url,
+            data={
+                "formhash": generate_hash(),
+                "replyid": comment.id if comment else 0,
+                "page": 1,
+                "summary": text,
+                "comment": "Save comment",
+            },
+        )
+
+        return page.__class__(soup(r.text))
+
+    def _comment_state_update(self, comment):
+        if comment is None:
+            raise ModdbException(
+                "This comment no longer exists or is no longer on the page it was initially retrieved from."
+            )
+
+        r = self._request(
+            "POST",
+            f"{BASE_URL}/messages/ajax/action/",
+            data={
+                "ajax": "t",
+                "action": "delete",
+                "sitearea": "comment",
+                "siteareaid": comment.id,
+                "hash": comment._hash,
+            },
+            allow_redirects=False,
+        )
+
+        return r
+
+    def delete_comment(self, comment: Comment) -> bool:
+        """This will delete the supplied comment provided you have the correct permissions.
+        This is an expensive request because if how moddb works. It needs to make two requests
+        in order to get the correct hash to delete the comment. In addition, it may fail if the
+        comment has changed location (page number) from what the object says. It is recommended
+        to use a newly created comment object that is less than 30 minutes old.
+
+        Parameters
+        -----------
+        comment : Comment
+            The comment to delete
+
+        Raises
+        -------
+        ModdbException
+            An error occured while trying to delete the comment
+
+        Returns
+        --------
+        bool
+            True if the comment was successfully deleted
+        """
+        with self:
+            page = parse_page(comment._url)
+            updated_comment = get(page.comments, id=comment.id)
+
+        r = self._comment_state_update(updated_comment)
+
+        return "You have <u>deleted</u> this comment" in r.json()["text"]
+
+    def undelete_comment(self, comment: Comment) -> bool:
+        """This will undelete the supplied comment provided you have the correct permissions.
+        This is an expensive request because of how moddb works. It needs to make three requests
+        in order to get the correct hash to undelete the comment. In addition, it may fail if the
+        comment has changed location (page number) from what the object says. It is recommended
+        to use a newly created comment object that is less than 30 minutes old.
+
+        Parameters
+        -----------
+        comment : Comment
+            The comment to undelete
+
+        Raises
+        -------
+        ModdbException
+            An error occured while trying to undelete the comment
+
+        Returns
+        --------
+        bool
+            True if the comment was successfully undeleted
+        """
+        with self:
+            page = parse_page(comment._url)
+            updated_comment = get(
+                page._get_comments_from_url(comment._url, show_deleted=True),
+                id=comment.id,
+            )
+
+        r = self._comment_state_update(updated_comment)
+
+        return "You have <u>authorized</u> this comment" in r.json()["text"]
+
+    def edit_comment(self, comment: Comment, new_text: str) -> bool:
+        """Edit the contents of a comment. You can only edit your comment 120 minutes after it has
+        been posted
+
+        Parameters
+        -----------
+        comment : Comment
+            The comment to edit
+        new_text : str
+            The new content of the comment
+
+        Raises
+        -------
+        ModdbException
+            An error has occured trying to edit the comment
+
+        Returns
+        --------
+        bool
+            True if the comment was successfully edited
+        """
+        r = self._request(
+            "POST",
+            f"{BASE_URL}/comment/ajax/post",
+            data={"ajax": "t", "id": comment.id, "summary": new_text},
+        )
+
+        return "Your comment has been saved" in r.json()["text"]
+
+    def add_review(
+        self, page: Any, rating: int, *, text: str = None, has_spoilers: bool = False
+    ) -> bool:
+        """Rate and review a page. If you rating is below 3 or above 8 you will be asked
+        to also provide a review or else the request will not be made. This is also
+        used to edit existing reviews.
+
+        Parameters
+        -----------
+        page : Union[Mod, Game, Engine, Hardware, Software, Platform]
+            The page you wish to review
+        rating : int
+            The rating from 1 to 10
+        text : str
+            The text review you are giving of this page
+        has_spoilers : bool
+            Whether or not this review contains spoilers.
+
+        Raises
+        -------
+        ModdbException
+            An error occured trying to review the page.
+
+        Returns
+        --------
+        bool
+            True of the review was successfuly submitted.
+
+        """
+        if not (2 < rating < 9) and text is None:
+            raise ModdbException("Please include a review to justify such a low/high rating.")
+
+        with self:
+            page = parse_page(page.url)
+
+        r = self._request(
+            "POST",
+            f"{BASE_URL}/reviews/ajax",
+            data={
+                "ajax": "t",
+                "sitearea": get_sitearea(page.url),
+                "siteareaid": page.id,
+                "hash": page._review_hash,
+                "earlyaccess": int(page.profile.status == Status.early_access),
+                "rating": rating,
+                "summary": text,
+                "spoiler": int(has_spoilers),
+            },
+            allow_redirects=False,
+        )
+
+        return "Your rating has been saved" in r.json()["text"]
+
+    def delete_review(self, review: Review) -> bool:
+        """Delete your review on the given page. This function will do two requests in order
+        to delete your review.
+
+        Parameters
+        -----------
+        review : Review
+            The review you wish to delete
+
+        Raises
+        -------
+        ModdbException
+            An error occured while trying to delete the review
+
+        Returns
+        --------
+        bool
+            True if the review was successfully deleted
+        """
+        with self:
+            hash_review = self.member.get_reviews()[0]
+
+        r = self._request(
+            "POST",
+            f"{BASE_URL}/messages/ajax/action/",
+            data={
+                "ajax": "t",
+                "action": "delete",
+                "sitearea": "reviews",
+                "siteareaid": review.id,
+                "hash": hash_review._hash,
+                "ispd": 1,
+            },
+            allow_redirects=False,
+        )
+
+        return "You have <u>deleted</u> this review." in r.json()["text"]
+
+    def get_threads(
+        self,
+        query: str = None,
+        read: bool = None,
+        replied: bool = None,
+        sent_items: bool = False,
+        sort: Tuple[str, str] = None,
+    ) -> List[ThreadThumbnail]:
+        """Get all the messages this user has sent or received. This does not return threads you
+        have left.
+
+        Parameters
+        -----------
+        query : Optional[str]
+            Optional query to filter messages
+        read : Optional[bool]
+            True to filter only read message, false to filter unread, None to allow both
+        replied : Optional[bool]
+            True to filter messages where you are the last message, False for messages
+            where another user is the last message, None for both.
+        sent_items:
+            Get only the threads you have started
+        sort : Tuple[str, str]
+            Optional sort tuple to order threads
+
+        Returns
+        --------
+        List[ThreadThumbnail]
+            Thread typed thumbnails
+        """
+        if sent_items:
+            url = f"{BASE_URL}/messages/sentitems"
+        else:
+            url = f"{BASE_URL}/messages/inbox"
+
+        r = self._request(
+            "GET",
+            url,
+            params={
+                "filter": "t",
+                "kw": query,
+                "hasread": int(read) if read is not None else read,
+                "hasreplied": int(replied) if replied is not None else replied,
+                "sort": f"{sort[0]}-{sort[1]}" if sort is not None else sort,
+            },
+        )
+        html = soup(r.text)
+
+        threads_raw = html.find_all("div", class_=["tabinbox"])[-1].find_all(
+            "div", class_=["rowcontent"]
+        )
+        threads = []
+        for thread in threads_raw:
+            member = thread.find("span", class_="subheading").find_all("a")[0]
+            threads.append(
+                ThreadThumbnail(
+                    url=thread.a["href"],
+                    name=thread.a["title"],
+                    last_messager=Thumbnail(
+                        type=ThumbnailType.member, name=member.string, url=member["href"]
+                    ),
+                    timestamp=get_date(thread.find("time")["datetime"]),
+                    content=thread.find("div", class_="content").find("p").string,
+                )
+            )
+
+        return threads
+
+    def parse_thread(self, thread: ThreadThumbnail) -> Thread:
+        """Parse a thread thumbnail into a full thread object.
+
+        Parameters
+        ----------
+        thread : ThreadThumbnail
+            The thumbnail to parse
+
+        Returns
+        --------
+        Thread
+            The parsed thread and its messages
+        """
+        r = self._request("GET", thread.url)
+
+        return Thread(soup(r.text))
+
+    def send_message(self, members: List[Member], name: str, message: str) -> Thread:
+        """Send a message and start a thread with one or more members
+
+        Parameters
+        ----------
+        member : List[Member]
+            The members to send the message to and start the
+            thread with
+        name : str
+            The subject of the message
+        message : str
+            The message to send
+
+        Returns
+        --------
+        Thread
+            The thread started from sending this message
+        """
+        r = self._request(
+            "POST",
+            f"{BASE_URL}/messages/compose/",
+            data={
+                "formhash": generate_hash(),
+                "membersto": ",".join(member.name for member in members),
+                "name": name,
+                "description": message,
+                "messages": "Send+message",
+            },
+        )
+
+        return Thread(soup(r.text))
+
+    def reply_to_thread(self, thread: Union[Thread, ThreadThumbnail], text: str) -> Thread:
+        """Add an additional message to an exiting thread
+
+        Parameters
+        -----------
+        thread : Union[Thread, ThreadThumbnail]
+            The thread to add the message to
+        text : str
+            The text to send
+
+        Returns
+        --------
+        Thread
+            The updated thread containing the new message. It is
+            recommended to use this object as it also contains
+            a new hash for sending another message
+        """
+        r = self._request(
+            "POST",
+            f"{BASE_URL}/messages/inbox/{thread.id}",
+            data={"formhash": generate_hash(), "description": text, "messages": "Send+message"},
+        )
+
+        return Thread(soup(r.text))
+
+    def add_member_to_thread(self, thread: Union[Thread, ThreadThumbnail], member: Member) -> bool:
+        """Add a member to a conversation
+
+        Parameters
+        -----------
+        thread : Union[Thread, ThreadThumbnail]
+            The thread to add add a member to
+        member : Member
+            The member to add
+
+        Returns
+        --------
+        bool
+            Whether adding the member was succesful. This
+            will not update the thread.
+        """
+        r = self._request(
+            "POST",
+            f"{BASE_URL}/messages/ajax/members/invite/{thread.id}",
+            data={"ajax": "t", "username": member.name, "member": "0"},
+            allow_redirects=False,
+        )
+
+        return "has been successfully added" in r.json()["text"]
+
+    def leave_thread(self, thread: Union[Thread, ThreadThumbnail]) -> bool:
+        """Leave a thread, you will not get any more notifications on this thread.
+
+        Parameters
+        ----------
+        thread : Union[Thread, ThreadThumbnail]
+            The thread to leave
+
+        Returns
+        --------
+        bool
+            Whether leaving the thread was successful
+        """
+        r = self._request(
+            "POST",
+            f"{BASE_URL}/messages/ajax/delete/",
+            data={"ajax": "t", "thread": thread.id},
+            allow_redirects=False,
+        )
+
+        return "You have successfully deleted the requested thread" in r.json()["text"]
+
+    def mark_all_read(self) -> bool:
+        """Mark all threads as read.
+
+        Returns
+        --------
+        bool
+            True if all threads have been marked as read
+        """
+        r = self._request("POST", f"{BASE_URL}/messages/ajax/markallread", data={"ajax": "t"})
+
+        return "All messages marked as read" in r.json()["text"]
+
+    def _vote_tag(self, tag: Tag, negative: int):
+        params = {
+            "ajax": "t",
+            "tag": tag.name_id,
+            "sitearea": get_siteareaid(tag.sitearea),
+            "siteareadid": tag.siteareaid,
+            "hash": generate_hash(),
+            "negative": str(negative),
+        }
+
+        resp = self._request("POST", f"{BASE_URL}/tags/ajax/add", data=params)
+        return resp.json()["success"]
+
+    def upvote_tag(self, tag: Tag) -> bool:
+        """Upvote a tag
+
+        Parameters
+        -----------
+        tag : Tag
+            The tag to upvote
+
+        Returns
+        --------
+        bool
+            Whether the upvote was successful
+        """
+        return self._vote_tag(tag, 0)
+
+    def downvote_tag(self, tag: Tag) -> bool:
+        """Downvote a tag
+
+        Parameters
+        -----------
+        tag : Tag
+            The tag to downvote
+
+        Returns
+        --------
+        bool
+            Whether the downvote was successful
+        """
+        return self._vote_tag(tag, 1)
```

### Comparing `moddb-0.8.1/moddb/pages/__init__.py` & `moddb-0.9.0/moddb/pages/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from .fp import FrontPage
-from .mod import Mod
-from .game import Game
-from .engine import Engine
-from .article import Article, Blog
-from .entity import Team, Group, Member
-from .file import File, Addon, Media
-from .opinion import Poll, Review, ReviewList
-from .platform import Platform
-from .ware import Hardware, Software
-from .job import Job
-
-__all__ = [
-    "Mod",
-    "Game",
-    "Engine",
-    "File",
-    "Addon",
-    "Media",
-    "Article",
-    "Team",
-    "Group",
-    "Job",
-    "Blog",
-    "Member",
-    "FrontPage",
-    "Review",
-    "Platform",
-    "Poll",
-    "Software",
-    "Hardware",
-    "ReviewList",
-]
+from .article import Article, Blog
+from .engine import Engine
+from .entity import Group, Member, Team
+from .file import Addon, File, Media
+from .fp import FrontPage
+from .game import Game
+from .job import Job
+from .mod import Mod
+from .opinion import Poll, Review, ReviewList
+from .platform import Platform
+from .ware import Hardware, Software
+
+__all__ = [
+    "Mod",
+    "Game",
+    "Engine",
+    "File",
+    "Addon",
+    "Media",
+    "Article",
+    "Team",
+    "Group",
+    "Job",
+    "Blog",
+    "Member",
+    "FrontPage",
+    "Review",
+    "Platform",
+    "Poll",
+    "Software",
+    "Hardware",
+    "ReviewList",
+]
```

### Comparing `moddb-0.8.1/moddb/pages/article.py` & `moddb-0.9.0/moddb/pages/article.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,170 +1,178 @@
-import bs4
-from .base import BaseMetaClass
-from ..utils import concat_docs, LOGGER, join, get_views, get_date
-from ..enums import ArticleCategory, ThumbnailType, TutorialCategory, Difficulty
-from ..boxes import Profile, Thumbnail
-
-
-@concat_docs
-class Article(BaseMetaClass):
-    """This object represents an news article, a tutorial or a feature.
-
-    Parameters
-    -----------
-    html : bs4.BeautifulSoup
-        The html to parse. Allows for finer control.
-
-    Filtering
-    ----------
-    category : :class:`.ArticleCategory`
-        Type of the article (news, feature)
-    timeframe : :class:`.TimeFrame`
-        The time period this was released in (last 24hr, last week, last month)
-    game : Union[:class:`.Game`, :class:`.Object`]
-        An game object or an object with an id attribute which represents the
-        game the article belongs to.
-
-    Sorting
-    --------
-        * **ranktoday** - order by daily ranking, asc is highest ranked, desc is lowest rank
-        * **visitstotal** - order by most views, asc is highest views, desc is lowest views
-        * **dateup** - order by article date, asc is most recent first, desc is oldest first
-        * **name** - order alphabetically, asc is a-z, desc is z-a
-        * **member** - order by member???
-        * **date** - order by upload date, asc is most recent first, desc is oldest first
-
-        Exclusive to tutorials
-        * **meta** - sort by difficulty, asc is most difficult, desc is least difficult
-        * **subtype** - sort by the area the tutorial covers
-
-    Attributes
-    -----------
-    category : ArticleCategory
-        Whether this article is a news article, a tutorial or a feature
-    name : str
-        The name of the article
-    profile : Profile
-        The profile object of the moddb model the article is for (engine, game, mod...). Can be none if it is not
-        rattached to anything, such as for site news.
-    tags : dict{str : str}
-        A dictionary of tags with the tag names as the key and the url to the tag
-        as the value.
-    views : int
-        Total amount of times this article was viewed
-    today : int
-        amount of time the article has been viewed today
-    intro : int
-        The intro/teaser paragraph of the article
-    author : Thumbnail
-        A member type thumbnail of the member who published the article
-    date : datetime.datetime
-        The date the article was published
-    html : str
-        The html of the article
-    plaintext : str
-        The article text without any html
-    summary : str
-        plaintext intro to the article
-    tutorial_category : TutorialCategory
-        If the article category is tutorial, this represents the area the tutorial covers, else it is None
-    difficulty : Difficulty
-        If the article category is tutorial, this represents how hard the tutorial is.
-    """
-
-    def __init__(self, html: bs4.BeautifulSoup):
-        try:
-            self.name = html.find("span", itemprop="headline").string
-        except AttributeError:
-            self.name = html.find("span", itemprop="heading").string
-
-        super().__init__(html)
-
-        raw_type = html.find("h5", string="Browse").parent.span.a.string
-        self.category = ArticleCategory[raw_type.lower()]
-
-        try:
-            raw = html.find("span", string=raw_type[0:-1]).parent.parent.parent.find(
-                "div", class_="table tablemenu"
-            )
-        except AttributeError:
-            raw = html.find("span", string=raw_type).parent.parent.parent.find(
-                "div", class_="table tablemenu"
-            )
-
-        try:
-            self.profile = Profile(html)
-        except AttributeError:
-            LOGGER.info("'%s' has no profile", self.name)
-            self.profile = None
-
-        try:
-            raw_tags = html.find("form", attrs={"name": "tagsform"}).find_all("a")
-            self.tags = {x.string: join(x["href"]) for x in raw_tags if x.string is not None}
-        except AttributeError:
-            self.tags = {}
-            LOGGER.info("'%s' '%s' has no tags", self.__class__.__name__, self.name)
-
-        views_raw = raw.find("h5", string="Views").parent.span.a.string
-        self.views, self.today = get_views(views_raw)
-
-        self.intro = html.find("p", itemprop="description").string
-        author = html.find("span", itemprop="author").span.a
-        self.author = Thumbnail(name=author.string, url=author["href"], type=ThumbnailType.member)
-
-        self.date = get_date(html.find("time", itemprop="datePublished")["datetime"])
-        self.html = str(html.find("div", itemprop="articleBody"))
-        self.plaintext = html.find("div", itemprop="articleBody").text
-
-        self.summary = html.find("p", class_="introductiontext").string
-
-        if self.category == ArticleCategory.tutorials:
-            cat = html.find("span", itemprop="proficiencyLevel").nextSibling.strip()
-            self.tutorial_category = TutorialCategory[cat.replace("/", "_").replace(" ", "_").lower()]
-            self.difficulty = Difficulty[html.find("span", itemprop="proficiencyLevel").string.lower()]
-
-    def __repr__(self):
-        return f"<Article title={self.name} type={self.category.name}>"
-
-
-@concat_docs
-class Blog(BaseMetaClass):
-    """Object used to represent a member blog.
-
-    Filtering
-    ----------
-    timeframe : :class:`.TimeFrame`
-        The time period this was released in (last 24hr, last week, last month)
-
-    Sorting
-    --------
-        * **ranktoday** - order by daily ranking, asc is highest ranked, desc is lowest rank
-        * **visitstotal** - order by most views, asc is highest views, desc is lowest views
-        * **dateup** - order by blog date, asc is most recent first, desc is oldest first
-        * **name** - order alphabetically, asc is a-z, desc is z-a
-        * **member** - order by member???
-        * **date** - order by upload date, asc is most recent first, desc is oldest first
-
-    Attributes
-    -----------
-    name_id : str
-        The name_id of the member, cannot be changed, it's a mix of the original username lowercased with
-        spaces removed and shortened.
-
-    """
-
-    def __init__(self, *, heading, text):
-        author = heading.find("span", class_="subheading").a
-        self.author = Thumbnail(url=author["href"], name=author.string, type=ThumbnailType.member)
-
-        self.date = get_date(heading.find("span", class_="date").time["datetime"])
-
-        title = heading.div.h4.a
-        self.name = title.string
-        self.url = join(title["href"])
-        self.name_id = self.url.split("/")[0]
-
-        self.html = str(text.content)
-        self.plaintext = text.text
-
-    def __repr__(self):
-        return f"<Blog title={self.name}>"
+import bs4
+
+from ..boxes import PartialTag, Profile, Thumbnail
+from ..enums import ArticleCategory, Difficulty, ThumbnailType, TutorialCategory
+from ..utils import LOGGER, concat_docs, get_date, get_views, join
+from .base import BaseMetaClass
+
+
+@concat_docs
+class Article(BaseMetaClass):
+    """This object represents an news article, a tutorial or a feature.
+
+    Parameters
+    -----------
+    html : bs4.BeautifulSoup
+        The html to parse. Allows for finer control.
+
+    Filtering
+    ----------
+    category : :class:`.ArticleCategory`
+        Type of the article (news, feature)
+    timeframe : :class:`.TimeFrame`
+        The time period this was released in (last 24hr, last week, last month)
+    game : Union[:class:`.Game`, :class:`.Object`]
+        An game object or an object with an id attribute which represents the
+        game the article belongs to.
+
+    Sorting
+    --------
+        * **ranktoday** - order by daily ranking, asc is highest ranked, desc is lowest rank
+        * **visitstotal** - order by most views, asc is highest views, desc is lowest views
+        * **dateup** - order by article date, asc is most recent first, desc is oldest first
+        * **name** - order alphabetically, asc is a-z, desc is z-a
+        * **member** - order by member???
+        * **date** - order by upload date, asc is most recent first, desc is oldest first
+
+        Exclusive to tutorials
+        * **meta** - sort by difficulty, asc is most difficult, desc is least difficult
+        * **subtype** - sort by the area the tutorial covers
+
+    Attributes
+    -----------
+    category : ArticleCategory
+        Whether this article is a news article, a tutorial or a feature
+    name : str
+        The name of the article
+    profile : Profile
+        The profile object of the moddb model the article is for (engine, game, mod...). Can be none if it is not
+        rattached to anything, such as for site news.
+    tags : List[PartialTag]
+         A list of partial tags. You can use `get_tags` and then use the name id to get the right one.
+    views : int
+        Total amount of times this article was viewed
+    today : int
+        amount of time the article has been viewed today
+    intro : int
+        The intro/teaser paragraph of the article
+    author : Thumbnail
+        A member type thumbnail of the member who published the article
+    date : datetime.datetime
+        The date the article was published
+    html : str
+        The html of the article
+    plaintext : str
+        The article text without any html
+    summary : str
+        plaintext intro to the article
+    tutorial_category : TutorialCategory
+        If the article category is tutorial, this represents the area the tutorial covers, else it is None
+    difficulty : Difficulty
+        If the article category is tutorial, this represents how hard the tutorial is.
+    """
+
+    def __init__(self, html: bs4.BeautifulSoup):
+        try:
+            self.name = html.find("span", itemprop="headline").string
+        except AttributeError:
+            self.name = html.find("span", itemprop="heading").string
+
+        super().__init__(html)
+
+        raw_type = html.find("h5", string="Browse").parent.span.a.string
+        self.category = ArticleCategory[raw_type.lower()]
+
+        try:
+            raw = html.find("span", string=raw_type[0:-1]).parent.parent.parent.find(
+                "div", class_="table tablemenu"
+            )
+        except AttributeError:
+            raw = html.find("span", string=raw_type).parent.parent.parent.find(
+                "div", class_="table tablemenu"
+            )
+
+        try:
+            self.profile = Profile(html)
+        except AttributeError:
+            LOGGER.info("'%s' has no profile", self.name)
+            self.profile = None
+
+        try:
+            raw_tags = html.find("form", attrs={"name": "tagsform"}).find_all("a")
+            self.tags = [
+                PartialTag(x.string, join(x["href"]), x["href"].split("/")[-1])
+                for x in raw_tags
+                if x.string is not None
+            ]
+        except AttributeError:
+            self.tags = []
+            LOGGER.info("'%s' '%s' has no tags", self.__class__.__name__, self.name)
+
+        views_raw = raw.find("h5", string="Views").parent.span.a.string
+        self.views, self.today = get_views(views_raw)
+
+        self.intro = html.find("p", itemprop="description").string
+        author = html.find("span", itemprop="author").span.a
+        self.author = Thumbnail(name=author.string, url=author["href"], type=ThumbnailType.member)
+
+        self.date = get_date(html.find("time", itemprop="datePublished")["datetime"])
+        self.html = str(html.find("div", itemprop="articleBody"))
+        self.plaintext = html.find("div", itemprop="articleBody").text
+
+        self.summary = html.find("p", class_="introductiontext").string
+
+        if self.category == ArticleCategory.tutorials:
+            cat = html.find("span", itemprop="proficiencyLevel").nextSibling.strip()
+            self.tutorial_category = TutorialCategory[
+                cat.replace("/", "_").replace(" ", "_").lower()
+            ]
+            self.difficulty = Difficulty[
+                html.find("span", itemprop="proficiencyLevel").string.lower()
+            ]
+
+    def __repr__(self):
+        return f"<Article title={self.name} type={self.category.name}>"
+
+
+@concat_docs
+class Blog(BaseMetaClass):
+    """Object used to represent a member blog.
+
+    Filtering
+    ----------
+    timeframe : :class:`.TimeFrame`
+        The time period this was released in (last 24hr, last week, last month)
+
+    Sorting
+    --------
+        * **ranktoday** - order by daily ranking, asc is highest ranked, desc is lowest rank
+        * **visitstotal** - order by most views, asc is highest views, desc is lowest views
+        * **dateup** - order by blog date, asc is most recent first, desc is oldest first
+        * **name** - order alphabetically, asc is a-z, desc is z-a
+        * **member** - order by member???
+        * **date** - order by upload date, asc is most recent first, desc is oldest first
+
+    Attributes
+    -----------
+    name_id : str
+        The name_id of the member, cannot be changed, it's a mix of the original username lowercased with
+        spaces removed and shortened.
+
+    """
+
+    def __init__(self, *, heading, text):
+        author = heading.find("span", class_="subheading").a
+        self.author = Thumbnail(url=author["href"], name=author.string, type=ThumbnailType.member)
+
+        self.date = get_date(heading.find("span", class_="date").time["datetime"])
+
+        title = heading.div.h4.a
+        self.name = title.string
+        self.url = join(title["href"])
+        self.name_id = self.url.split("/")[0]
+
+        self.html = str(text.content)
+        self.plaintext = text.text
+
+    def __repr__(self):
+        return f"<Blog title={self.name}>"
```

### Comparing `moddb-0.8.1/moddb/pages/base.py` & `moddb-0.9.0/moddb/pages/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,619 +1,632 @@
-import re
-import bs4
-from typing import List
-
-from ..utils import (
-    join,
-    LOGGER,
-    get_page,
-    get_media_type,
-    get_page_type,
-)
-from ..boxes import (
-    CommentList,
-    Thumbnail,
-    ResultList,
-    Profile,
-    Statistics,
-    PartialArticle,
-    Style,
-    _parse_comments,
-    _parse_results,
-)
-from ..enums import ThumbnailType, SearchCategory
-from .mixins import SharedMethodsMixin, RSSFeedMixin, GetWatchersMixin
-
-
-class BaseMetaClass:
-    """An abstract class that implements the attributes present on nearly every page. In addition, it implements
-    some shared hidden methods and the top level get_comments method.
-
-    Parameters
-    -----------
-    html : bs4.BeautifulSoup
-        The html containing the comments
-
-    Attributes
-    -----------
-    id : int
-        The id of the page
-    name_id : str
-        The name_id of the entity, cannot be changed, it's a mix of the original username lowercased with
-        spaces removed and shortened.
-    url : str
-        The url of the page
-    comments : CommentList[Comment]
-        The comments scrapped on this list in order.
-    report : str
-        URL to report the page
-    """
-
-    def __init__(self, html):
-        if not getattr(self, "name", None):
-            try:
-                self.name = html.find("a", itemprop="mainEntityOfPage").string
-            except AttributeError:
-                self.name = html.find("meta", property="og:title")["content"]
-
-        try:
-            self.id = int(re.search(r"siteareaid=(\d*)", html.find("a", class_=["reporticon"])["href"])[1])
-        except TypeError:
-            try:
-                self.id = int(html.find("input", attrs={"name": "siteareaid"})["value"])
-            except (AttributeError, TypeError):
-                # really scratching the bottom here but a lot of "official" groups don't have the regular ID
-                self.id = int(html.find("meta", property="og:image")["content"].split("/")[-2])
-
-        try:
-            self.url = html.find("meta", property="og:url")["content"]
-        except TypeError:
-            self.url = join(html.find("a", string=self.name)["href"])
-
-        self.name_id = self.url.split("/")[-1]
-
-        try:
-            self.report = join(html.find("a", string="Report")["href"])
-        except TypeError:
-            self.report = None
-            LOGGER.info("'%s' '%s' cannot be reported", self.__class__.__name__, self.name)
-
-        self.comments = self._get_comments(html)
-
-        self._html = html
-
-    def __repr__(self):
-        return f"<{self.__class__.__name__} name={self.name}>"
-
-    def _get_comments(self, html: bs4.BeautifulSoup) -> CommentList:
-        """Extracts the comments from an html page and adds them to a CommentList.
-
-        Parameters
-        -----------
-        html : bs4.BeautifulSoup
-            The html containing the comments
-
-        Returns
-        --------
-        CommentList
-            The list of parsed comments
-        """
-        results, current_page, total_pages, total_results = _parse_comments(html)
-
-        return CommentList(
-            results=results,
-            current_page=current_page,
-            total_pages=total_pages,
-            url=self.url,
-            total_results=total_results,
-        )
-
-    def _get(self, url: str, *, params: dict = {}) -> ResultList:
-        """This function takes a list of thumbnails of `object_type` in html and returns
-        a list of Thumbnail of that object type.
-
-        Parameters
-        -----------
-        url : str
-            The url with the list
-        object_type : ThumbnailType
-            The type of objects to be expected. Easier to pass and hardcode then to guess
-        params : dict
-            A dictionnary of filters to pass on to the soup function used to filter the results.
-
-        Returns
-        -------
-        ResultList[Thumbnail]
-            The list of objects present on the page as a list of thumbnails.
-        """
-        html = get_page(url, params=params)
-        results, current_page, total_pages, total_results = _parse_results(html)
-
-        return ResultList(
-            results=results,
-            params=params,
-            url=url,
-            current_page=current_page,
-            total_pages=total_pages,
-            total_results=total_results,
-        )
-
-    def _get_media(self, index: int, *, html) -> List[Thumbnail]:
-        """Hidden method used to parse media content from the page. Since the only difference is that pages
-        with videos have one extra script that tells the window not do any sort of video playing assistance.
-        Also used to cached all media on a page.
-
-        Parameters
-        ----------
-        index : int
-            The index of the script containing the cached objects. 1 if it's only images, 2 if videos are
-            also included
-
-        Returns
-        --------
-        List[Thumbnail]
-            List of media like thumbnails that can be parsed individually. Can be a very long list.
-        """
-        script = html.find_all("script", text=True)[index]
-        regex = r'new Array\(0, "(\S*)", "(\S*)"'
-        matches = re.findall(regex, script.text)
-
-        name_finder = r"\/([a-z0-9-]*)#imagebox"
-        return [
-            Thumbnail(
-                name=re.search(name_finder, match[0])[1],
-                url=match[0],
-                type=ThumbnailType.media,
-                image=match[1],
-            )
-            for match in matches
-        ]
-
-    def get_comments(self, index: int = 1, *, show_deleted=False) -> CommentList:
-        """Used to get comments on the model regardless of what page they may be present in. The function
-        itself simply relies on two other to make the request and parse the table.
-
-        Parameters
-        ----------
-        index : int
-            The page of the model to get the comments for.
-        show_deleted : Optional[bool]
-            Pass true to show deleted user comments. Only works if it is a page
-            you have permissions on.
-
-        Returns
-        --------
-        CommentList[Comment]
-            A list-like object containing the comments and additional methods
-        """
-        params = {"deleted": "t" if show_deleted else None}
-        return self._get_comments(get_page(f"{self.url}/page/{index}", params=params))
-
-
-class PageMetaClass(BaseMetaClass, SharedMethodsMixin, RSSFeedMixin, GetWatchersMixin):
-    """The common class representing the page for either a Mod, Game, Engine or a Member. Mostly used to be inherited by
-    those classes.
-
-    Parameters
-    -----------
-    html : bs4.BeautifulSoup
-        The page to be parsed.
-
-    page_type : ThumbnailType
-        The type of pages, this is passed down be the base class to help with the parsing of
-
-    Attributes
-    -----------
-    name : str
-        The name of the page
-    profile : Profile
-        The object with the content of the page's profile box.
-    stats : Statistics
-        The object containg stat data on the page such as views, followers, ect...
-    style : Style
-        The object containing data relevant to the type of the page, not valid for Engines. Multiplayer, singleplayer,
-        ect...
-    suggestions : List[Thumbnail]
-        A list of thumbnail object representing moddb's suggestion of similar pages for the visiting member.
-    files : List[Thumbnail]
-        A list of thumbnails representing a possible partial list of all the files. To get a guaranteed full
-        list either compare with statistics.files to see if the length of the list matches the number of files in the
-        stats or use get_files, although that will still not return the whole list if there are multiple pages of
-        files.
-    articles : List[Thumbnail]
-        A list of thumbnail objects representing articles present on the page. Usually 3 or 4 articles long.
-    article :  PartialArticle
-        A partial representation of the frong page article. This does not include things like comments or any
-        of the sideba elements found in a full article. Can be parsed to return the complete Article object.
-    tags : dict{str : str}
-        A dict of key-values pair where the key is the name of the tag and the value is the url.
-    imagebox : List[Thumbnail]
-        A list of Thumbnail objects representing the image, videos and audio clips that are presented in the
-        image box on the front page.
-    embed : str
-        The html necessary to embed the a widget of the page.
-    rating : float
-        A float out of ten representing the average rating for the page
-    medias : List[Thumbnail]
-        list of thumbnails representing all the combined media objects of a page (videos and images)
-    summary : str
-        Short description of the page, in plaintext.
-    description : str
-        The full description of the page, contains html
-    plaintext : str
-        Plaintext version of the full description
-    """
-
-    def __init__(self, html: bs4.BeautifulSoup, page_type: SearchCategory):
-        super().__init__(html)
-        self._type = page_type
-
-        # boxes
-        if page_type != SearchCategory.members:
-            self.profile = Profile(html)
-
-            try:
-                self.stats = Statistics(html)
-            except AttributeError:
-                LOGGER.info("Entity '%s' has no stats (idk why, ask moddb)", self.name)
-                self.stats = None
-
-            if page_type != SearchCategory.engines:
-                self.style = Style(html)
-
-            # thumbnails
-            self.suggestions = self._get_suggestions(html)
-
-            # misc
-            try:
-                self.embed = html.find("input", type="text", class_="text textembed")["value"]
-            except TypeError:
-                self.embed = str(html.find_all("textarea")[1].a)
-
-        try:
-            self.files = self._get_files(html)
-        except AttributeError:
-            LOGGER.info("'%s' '%s' has no files", self.__class__.__name__, self.name)
-            self.files = []
-
-        articles_raw = None
-        try:
-            raw = html.find("span", string="Articles") or html.find("span", string="Related Articles")
-            articles_raw = raw.parent.parent.parent.find("div", class_="table")
-            thumbnails = articles_raw.find_all("div", class_="row rowcontent clear")
-            self.articles = [
-                Thumbnail(
-                    name=x.a["title"],
-                    url=x.a["href"],
-                    image=x.a.img["src"] if x.a.img else None,
-                    summary=x.find("p").string,
-                    date=x.find("time")["datetime"],
-                    type=ThumbnailType.article,
-                )
-                for x in thumbnails
-            ]
-        except AttributeError:
-            LOGGER.info(
-                "'%s' '%s' has no article suggestions",
-                self.__class__.__name__,
-                self.name,
-            )
-            self.articles = []
-
-        # main page article
-        if articles_raw:
-            self.article = PartialArticle(articles_raw)
-        else:
-            self.article = None
-            LOGGER.info(
-                "'%s' '%s' has no front page article",
-                self.__class__.__name__,
-                self.name,
-            )
-
-        try:
-            raw_tags = html.find("form", attrs={"name": "tagsform"}).find_all("a")
-            self.tags = {x.string: join(x["href"]) for x in raw_tags if x.string is not None}
-        except AttributeError:
-            self.tags = {}
-            LOGGER.info("'%s' '%s' has no tags", self.__class__.__name__, self.name)
-
-        # imagebox
-        try:
-            imagebox = html.find("ul", id="imagebox").find_all("li")[1:-2]
-            self.imagebox = [
-                Thumbnail(
-                    name=x.a["title"],
-                    url=x.a["href"],
-                    image=x.a.img["src"],
-                    type=ThumbnailType(get_media_type(x.a.img)),
-                )
-                for x in imagebox
-                if x.a
-            ]
-        except (AttributeError, TypeError):
-            LOGGER.info("'%s' '%s' has no images", self.__class__.__name__, self.name)
-            self.imagebox = []
-
-        try:
-            self.rating = float(
-                html.find("div", class_="score").find("meta", itemprop="ratingValue")["content"]
-            )
-        except AttributeError:
-            self.rating = 0.0
-            LOGGER.info("'%s' '%s' is not rated", self.__class__.__name__, self.name)
-
-        try:
-            self._review_hash = html.find("form", class_="ratingform").find("input", {"name": "hash"})[
-                "value"
-            ]
-        except AttributeError:
-            self._review_hash = None
-
-        self.medias = self._get_media(2, html=html)
-
-        try:
-            self.summary = html.find("meta", itemprop="description")["content"]
-        except TypeError:
-            self.summary = None
-            LOGGER.info("'%s' '%s' has no summary", self.__class__.__name__, self.name)
-
-        self.description = str(html.find("div", id="profiledescription"))
-
-        try:
-            self.description = str(html.find("div", id="profiledescription"))
-            self.plaintext = html.find("div", id="profiledescription").text
-        except AttributeError:
-            LOGGER.info(
-                "'%s' '%s' has no extended description",
-                self.__class__.__name__,
-                self.name,
-            )
-            self.description = None
-            self.plaintext = None
-
-    def _get_suggestions(self, html: bs4.BeautifulSoup) -> List[Thumbnail]:
-        """Hidden method used to get the list of suggestions on the page. As with most things, this list of suggestions
-        will be a list of Thumbnail objects that can be parsed individually.
-
-        Parameters
-        -----------
-        html : bs4.BeautifulSoup
-            The html page we are trying to parse the suggestions for
-
-        Returns
-        --------
-        List[Thumbnail]
-            The list of suggestions as thumbnails.
-        """
-        suggestions_raw = (
-            html.find("span", string="You may also like")
-            .parent.parent.parent.find("div", class_="table")
-            .find_all("div", recursive=False)
-        )
-        suggestions = []
-        for x in suggestions_raw:
-            try:
-                link = x.find("a", class_="image")
-                suggestion_type = get_page_type(link["href"])
-                suggestion = Thumbnail(
-                    name=link["title"],
-                    url=link["href"],
-                    image=link.img["src"],
-                    type=suggestion_type,
-                )
-                suggestions.append(suggestion)
-            except (AttributeError, TypeError):
-                pass
-
-        return suggestions
-
-    def _get_games(self, html: bs4.BeautifulSoup) -> List[Thumbnail]:
-        """Used both for Teams and Engines, returns a list of games  present on the page
-        as Thumbnail objects.
-
-        Parameters
-        ----------
-        html : bs4.BeautifulSoup
-            The html to extract the list of games from
-
-        Returns
-        -------
-        List[Thumbnail]
-            The list of games on the page as Thumbnail objects.
-        """
-        games_raw = html.find(string="Games").parent.parent.parent.parent.find_all(
-            class_="row rowcontent clear"
-        )
-        games = []
-        for x in games_raw:
-            link = x.find("div", class_="content").h4.a
-            image_url = link.parent.parent.parent.find("img")["src"]
-            game = Thumbnail(
-                name=link.string,
-                url=link["href"],
-                image=image_url,
-                type=ThumbnailType.game,
-            )
-            games.append(game)
-
-        return games
-
-    def _get_files(self, html: bs4.BeautifulSoup) -> List[Thumbnail]:
-        """Cache the files present on the page. Up to 5 files might be present
-
-        Parameters
-        -----------
-        html : bs4.BeautifulSoup
-            The page to cache the files from
-
-        Returns
-        -------
-        List[Thumbnail]
-            The list of file like thumbnails
-        """
-
-        files_raw = html.find(string="Files").parent.parent.parent.parent.find_all(
-            class_="row rowcontent clear"
-        )
-        files = []
-        for x in files_raw:
-            link = x.find("div", class_="content").h4.a
-            try:
-                image_url = link.parent.parent.parent.find("img")["src"]
-            except TypeError:
-                image_url = None
-
-            file = Thumbnail(
-                name=link.string,
-                url=link["href"],
-                image=image_url,
-                type=ThumbnailType.file,
-            )
-            files.append(file)
-
-        return files
-
-    def _get_engines(self, html):
-        """Hidden method to get the engines showed currently on the page as a list of engine like thumbnails. Takes
-        an entire page of html and sorts it out
-
-        Parameters
-        -----------
-        html : bs4.BeautifulSoup
-            The page to cache the engines from
-
-        Returns
-        -------
-        List[Thumbnail]
-            The list of engine like thumbnail objects
-        """
-        engines_raw = html.find(string="Engines").parent.parent.parent.parent.find_all(
-            class_="row rowcontent clear"
-        )
-        engines = []
-        for x in engines_raw:
-            link = x.find("div", class_="content").h4.a
-            image_url = link.parent.parent.parent.find("img")["src"]
-            engine = Thumbnail(
-                name=link.string,
-                url=link["href"],
-                image=image_url,
-                type=ThumbnailType.engine,
-            )
-            engines.append(engine)
-
-        return engines
-
-    def __repr__(self):
-        return f"<{self.__class__.__name__} name={self.name}>"
-
-
-class HardwareSoftwareMetaClass(BaseMetaClass, SharedMethodsMixin, RSSFeedMixin, GetWatchersMixin):
-    """Shared class for Hardware and Software
-
-    Attributes
-    -----------
-    description : str
-        Description of the page
-    profile : Profile
-        The page's profile
-    stats : Statistics
-        The page's stats
-    rating : float
-        The rating of the item
-    articles : List[Thumbnail]
-        List of article type thumbnails from the recommended articles
-    article : PartialArticle
-        The partial article presented on the front page
-    tags : Dict{str : str}
-        Dict of tags with the name as the key and the url as the value
-    medias : List[Thumbnail]
-        list of thumbnails representing all the combined media objects of a page (videos and images)
-    suggestions : List[Thumbnail]
-        list of suggested software/hardware type thumbnails
-    """
-
-    def __init__(self, html):
-        super().__init__(html)
-        try:
-            self.description = html.find("div", id="profiledescription").p.string
-        except AttributeError:
-            self.description = html.find("p", itemprop="description").string
-
-        self.profile = Profile(html)
-
-        try:
-            self.stats = Statistics(html)
-        except AttributeError:
-            LOGGER.info("Entity '%s' has no stats (idk why, ask moddb)", self.name)
-            self.stats = None
-
-        try:
-            self.rating = float(
-                html.find("div", class_="score").find("meta", itemprop="ratingValue")["content"]
-            )
-        except AttributeError:
-            self.rating = 0.0
-            LOGGER.info("'%s' '%s' is not rated", self.profile.category.name, self.name)
-
-        try:
-            self._review_hash = html.find("form", class_="ratingform").find("input", {"name": "hash"})[
-                "value"
-            ]
-        except AttributeError:
-            self._review_hash = None
-
-        articles_raw = None
-        try:
-            articles_raw = html.find("span", string="Related Articles").parent.parent.parent.find(
-                "div", class_="table"
-            )
-            thumbnails = articles_raw.find_all("div", class_="row rowcontent clear")
-            self.articles = [
-                Thumbnail(
-                    name=x.a["title"],
-                    url=x.a["href"],
-                    image=x.a.img["src"] if x.a.img else None,
-                    summary=x.find("p").string,
-                    date=x.find("time")["datetime"],
-                    type=ThumbnailType.article,
-                )
-                for x in thumbnails
-            ]
-        except AttributeError:
-            LOGGER.info(
-                "'%s' '%s' has no article suggestions",
-                self.profile.category.name,
-                self.name,
-            )
-            self.articles = []
-
-        if articles_raw:
-            self.article = PartialArticle(articles_raw)
-        else:
-            self.article = None
-            LOGGER.info(
-                "'%s' '%s' has no front page article",
-                self.profile.category.name,
-                self.name,
-            )
-
-        try:
-            raw_tags = html.find("form", attrs={"name": "tagsform"}).find_all("a")
-            self.tags = {x.string: join(x["href"]) for x in raw_tags if x.string is not None}
-        except AttributeError:
-            self.tags = {}
-            LOGGER.info("Hardware '%s' has no tags", self.name)
-
-        self.medias = self._get_media(1, html=html)
-
-        try:
-            t = ThumbnailType[self.__class__.__name__.lower()]
-            suggestions = html.find("span", string="You may also like").parent.parent.parent.find_all(
-                "a", class_="image"
-            )
-            self.suggestions = [
-                Thumbnail(url=x["href"], name=x["title"], type=t, image=x.img["src"]) for x in suggestions
-            ]
-        except AttributeError:
-            LOGGER.info("'%s' '%s' has no suggestions", self.__class__.__name__, self.name)
+import re
+from typing import List
+
+from bs4 import BeautifulSoup
+
+from ..boxes import (
+    CommentList,
+    PartialArticle,
+    PartialTag,
+    Profile,
+    ResultList,
+    Statistics,
+    Style,
+    Thumbnail,
+    _parse_comments,
+    _parse_results,
+)
+from ..enums import SearchCategory, ThumbnailType
+from ..utils import LOGGER, get_media_type, get_page, get_page_type, join
+from .mixins import GetTagsMixin, GetWatchersMixin, RSSFeedMixin, SharedMethodsMixin
+
+
+class BaseMetaClass:
+    """An abstract class that implements the attributes present on nearly every page. In addition, it implements
+    some shared hidden methods and the top level get_comments method.
+
+    Parameters
+    -----------
+    html : BeautifulSoup
+        The html containing the comments
+
+    Attributes
+    -----------
+    id : int
+        The id of the page
+    name_id : str
+        The name_id of the entity, cannot be changed, it's a mix of the original username lowercased with
+        spaces removed and shortened.
+    url : str
+        The url of the page
+    comments : CommentList[Comment]
+        The comments scrapped on this list in order.
+    report : str
+        URL to report the page
+    """
+
+    def __init__(self, html: BeautifulSoup):
+        if not getattr(self, "name", None):
+            try:
+                self.name = html.find("a", itemprop="mainEntityOfPage").string
+            except AttributeError:
+                self.name = html.find("meta", property="og:title")["content"]
+
+        try:
+            self.id = int(
+                re.search(r"siteareaid=(\d*)", html.find("a", class_=["reporticon"])["href"])[1]
+            )
+        except TypeError:
+            try:
+                self.id = int(html.find("input", attrs={"name": "siteareaid"})["value"])
+            except (AttributeError, TypeError):
+                # really scratching the bottom here but a lot of "official" groups don't have the regular ID
+                self.id = int(html.find("meta", property="og:image")["content"].split("/")[-2])
+
+        try:
+            self.url = html.find("meta", property="og:url")["content"]
+        except TypeError:
+            self.url = join(html.find("a", string=self.name)["href"])
+
+        self.name_id = self.url.split("/")[-1]
+
+        try:
+            self.report = join(html.find("a", string="Report")["href"])
+        except TypeError:
+            self.report = None
+            LOGGER.info("'%s' '%s' cannot be reported", self.__class__.__name__, self.name)
+
+        self.comments = self._get_comments(html)
+
+        self._html = html
+
+    def __repr__(self):
+        return f"<{self.__class__.__name__} name={self.name}>"
+
+    def _get_comments(self, html: BeautifulSoup) -> CommentList:
+        """Extracts the comments from an html page and adds them to a CommentList.
+
+        Parameters
+        -----------
+        html : BeautifulSoup
+            The html containing the comments
+
+        Returns
+        --------
+        CommentList
+            The list of parsed comments
+        """
+        results, current_page, total_pages, total_results = _parse_comments(html)
+
+        return CommentList(
+            results=results,
+            current_page=current_page,
+            total_pages=total_pages,
+            url=self.url,
+            total_results=total_results,
+        )
+
+    def _get(self, url: str, *, params: dict = {}) -> ResultList:
+        """This function takes a list of thumbnails of `object_type` in html and returns
+        a list of Thumbnail of that object type.
+
+        Parameters
+        -----------
+        url : str
+            The url with the list
+        object_type : ThumbnailType
+            The type of objects to be expected. Easier to pass and hardcode then to guess
+        params : dict
+            A dictionnary of filters to pass on to the soup function used to filter the results.
+
+        Returns
+        -------
+        ResultList[Thumbnail]
+            The list of objects present on the page as a list of thumbnails.
+        """
+        html = get_page(url, params=params)
+        results, current_page, total_pages, total_results = _parse_results(html)
+
+        return ResultList(
+            results=results,
+            params=params,
+            url=url,
+            current_page=current_page,
+            total_pages=total_pages,
+            total_results=total_results,
+        )
+
+    def _get_media(self, index: int, *, html) -> List[Thumbnail]:
+        """Hidden method used to parse media content from the page. Since the only difference is that pages
+        with videos have one extra script that tells the window not do any sort of video playing assistance.
+        Also used to cached all media on a page.
+
+        Parameters
+        ----------
+        index : int
+            The index of the script containing the cached objects. 1 if it's only images, 2 if videos are
+            also included
+
+        Returns
+        --------
+        List[Thumbnail]
+            List of media like thumbnails that can be parsed individually. Can be a very long list.
+        """
+        script = html.find_all("script", string=True)[index]
+        regex = r'new Array\(0, "(\S*)", "(\S*)"'
+        matches = re.findall(regex, script.text)
+
+        name_finder = r"\/([a-z0-9-]*)#imagebox"
+        return [
+            Thumbnail(
+                name=re.search(name_finder, match[0])[1],
+                url=match[0],
+                type=ThumbnailType.media,
+                image=match[1],
+            )
+            for match in matches
+        ]
+
+    def get_comments(self, index: int = 1, *, show_deleted=False) -> CommentList:
+        """Used to get comments on the model regardless of what page they may be present in. The function
+        itself simply relies on two other to make the request and parse the table.
+
+        Parameters
+        ----------
+        index : int
+            The page of the model to get the comments for.
+        show_deleted : Optional[bool]
+            Pass true to show deleted user comments. Only works if it is a page
+            you have permissions on.
+
+        Returns
+        --------
+        CommentList[Comment]
+            A list-like object containing the comments and additional methods
+        """
+        params = {"deleted": "t" if show_deleted else None}
+        return self._get_comments(get_page(f"{self.url}/page/{index}", params=params))
+
+
+class PageMetaClass(
+    BaseMetaClass, SharedMethodsMixin, RSSFeedMixin, GetWatchersMixin, GetTagsMixin
+):
+    """The common class representing the page for either a Mod, Game, Engine or a Member. Mostly used to be inherited by
+    those classes.
+
+    Parameters
+    -----------
+    html : BeautifulSoup
+        The page to be parsed.
+
+    page_type : ThumbnailType
+        The type of pages, this is passed down be the base class to help with the parsing of
+
+    Attributes
+    -----------
+    name : str
+        The name of the page
+    profile : Profile
+        The object with the content of the page's profile box.
+    stats : Statistics
+        The object containg stat data on the page such as views, followers, ect...
+    style : Style
+        The object containing data relevant to the type of the page, not valid for Engines. Multiplayer, singleplayer,
+        ect...
+    suggestions : List[Thumbnail]
+        A list of thumbnail object representing moddb's suggestion of similar pages for the visiting member.
+    files : List[Thumbnail]
+        A list of thumbnails representing a possible partial list of all the files. To get a guaranteed full
+        list either compare with statistics.files to see if the length of the list matches the number of files in the
+        stats or use get_files, although that will still not return the whole list if there are multiple pages of
+        files.
+    articles : List[Thumbnail]
+        A list of thumbnail objects representing articles present on the page. Usually 3 or 4 articles long.
+    article :  PartialArticle
+        A partial representation of the frong page article. This does not include things like comments or any
+        of the sideba elements found in a full article. Can be parsed to return the complete Article object.
+    tags : List[PartialTag]
+        A list of partial tags. You can use `get_tags` and then use the name id to get the right one.
+    imagebox : List[Thumbnail]
+        A list of Thumbnail objects representing the image, videos and audio clips that are presented in the
+        image box on the front page.
+    embed : str
+        The html necessary to embed the a widget of the page.
+    rating : float
+        A float out of ten representing the average rating for the page
+    medias : List[Thumbnail]
+        list of thumbnails representing all the combined media objects of a page (videos and images)
+    summary : str
+        Short description of the page, in plaintext.
+    description : str
+        The full description of the page, contains html
+    plaintext : str
+        Plaintext version of the full description
+    """
+
+    def __init__(self, html: BeautifulSoup, page_type: SearchCategory):
+        super().__init__(html)
+        self._type = page_type
+
+        # boxes
+        if page_type != SearchCategory.members:
+            self.profile = Profile(html)
+
+            try:
+                self.stats = Statistics(html)
+            except AttributeError:
+                LOGGER.info("Entity '%s' has no stats (idk why, ask moddb)", self.name)
+                self.stats = None
+
+            if page_type != SearchCategory.engines:
+                self.style = Style(html)
+
+            # thumbnails
+            self.suggestions = self._get_suggestions(html)
+
+            # misc
+            try:
+                self.embed = html.find("input", type="text", class_="text textembed")["value"]
+            except TypeError:
+                self.embed = str(html.find_all("textarea")[1].a)
+
+        try:
+            self.files = self._get_files(html)
+        except AttributeError:
+            LOGGER.info("'%s' '%s' has no files", self.__class__.__name__, self.name)
+            self.files = []
+
+        articles_raw = None
+        try:
+            raw = html.find("span", string="Articles") or html.find(
+                "span", string="Related Articles"
+            )
+            articles_raw = raw.parent.parent.parent.find("div", class_="table")
+            thumbnails = articles_raw.find_all("div", class_="row rowcontent clear")
+            self.articles = [
+                Thumbnail(
+                    name=x.a["title"],
+                    url=x.a["href"],
+                    image=x.a.img["src"] if x.a.img else None,
+                    summary=x.find("p").string,
+                    date=x.find("time")["datetime"],
+                    type=ThumbnailType.article,
+                )
+                for x in thumbnails
+            ]
+        except AttributeError:
+            LOGGER.info(
+                "'%s' '%s' has no article suggestions",
+                self.__class__.__name__,
+                self.name,
+            )
+            self.articles = []
+
+        # main page article
+        if articles_raw:
+            self.article = PartialArticle(articles_raw)
+        else:
+            self.article = None
+            LOGGER.info(
+                "'%s' '%s' has no front page article",
+                self.__class__.__name__,
+                self.name,
+            )
+
+        try:
+            raw_tags = html.find("form", attrs={"name": "tagsform"}).find_all("a")
+            self.tags = [
+                PartialTag(x.string, join(x["href"]), x["href"].split("/")[-1])
+                for x in raw_tags
+                if x.string is not None
+            ]
+        except AttributeError:
+            self.tags = []
+            LOGGER.info("'%s' '%s' has no tags", self.__class__.__name__, self.name)
+
+        # imagebox
+        try:
+            imagebox = html.find("ul", id="imagebox").find_all("li")[1:-2]
+            self.imagebox = [
+                Thumbnail(
+                    name=x.a["title"],
+                    url=x.a["href"],
+                    image=x.a.img["src"],
+                    type=ThumbnailType(get_media_type(x.a.img)),
+                )
+                for x in imagebox
+                if x.a
+            ]
+        except (AttributeError, TypeError):
+            LOGGER.info("'%s' '%s' has no images", self.__class__.__name__, self.name)
+            self.imagebox = []
+
+        try:
+            self.rating = float(
+                html.find("div", class_="score").find("meta", itemprop="ratingValue")["content"]
+            )
+        except AttributeError:
+            self.rating = 0.0
+            LOGGER.info("'%s' '%s' is not rated", self.__class__.__name__, self.name)
+
+        try:
+            self._review_hash = html.find("form", class_="ratingform").find(
+                "input", {"name": "hash"}
+            )["value"]
+        except AttributeError:
+            self._review_hash = None
+
+        self.medias = self._get_media(2, html=html)
+
+        try:
+            self.summary = html.find("meta", itemprop="description")["content"]
+        except TypeError:
+            self.summary = None
+            LOGGER.info("'%s' '%s' has no summary", self.__class__.__name__, self.name)
+
+        self.description = str(html.find("div", id="profiledescription"))
+
+        try:
+            self.description = str(html.find("div", id="profiledescription"))
+            self.plaintext = html.find("div", id="profiledescription").text
+        except AttributeError:
+            LOGGER.info(
+                "'%s' '%s' has no extended description",
+                self.__class__.__name__,
+                self.name,
+            )
+            self.description = None
+            self.plaintext = None
+
+    def _get_suggestions(self, html: BeautifulSoup) -> List[Thumbnail]:
+        """Hidden method used to get the list of suggestions on the page. As with most things, this list of suggestions
+        will be a list of Thumbnail objects that can be parsed individually.
+
+        Parameters
+        -----------
+        html : BeautifulSoup
+            The html page we are trying to parse the suggestions for
+
+        Returns
+        --------
+        List[Thumbnail]
+            The list of suggestions as thumbnails.
+        """
+        suggestions_raw = (
+            html.find("span", string="You may also like")
+            .parent.parent.parent.find("div", class_="table")
+            .find_all("div", recursive=False)
+        )
+        suggestions = []
+        for x in suggestions_raw:
+            try:
+                link = x.find("a", class_="image")
+                suggestion_type = get_page_type(link["href"])
+                suggestion = Thumbnail(
+                    name=link["title"],
+                    url=link["href"],
+                    image=link.img["src"],
+                    type=suggestion_type,
+                )
+                suggestions.append(suggestion)
+            except (AttributeError, TypeError):
+                pass
+
+        return suggestions
+
+    def _get_games(self, html: BeautifulSoup) -> List[Thumbnail]:
+        """Used both for Teams and Engines, returns a list of games  present on the page
+        as Thumbnail objects.
+
+        Parameters
+        ----------
+        html : BeautifulSoup
+            The html to extract the list of games from
+
+        Returns
+        -------
+        List[Thumbnail]
+            The list of games on the page as Thumbnail objects.
+        """
+        games_raw = html.find(string="Games").parent.parent.parent.parent.find_all(
+            class_="row rowcontent clear"
+        )
+        games = []
+        for x in games_raw:
+            link = x.find("div", class_="content").h4.a
+            image_url = link.parent.parent.parent.find("img")["src"]
+            game = Thumbnail(
+                name=link.string,
+                url=link["href"],
+                image=image_url,
+                type=ThumbnailType.game,
+            )
+            games.append(game)
+
+        return games
+
+    def _get_files(self, html: BeautifulSoup) -> List[Thumbnail]:
+        """Cache the files present on the page. Up to 5 files might be present
+
+        Parameters
+        -----------
+        html : BeautifulSoup
+            The page to cache the files from
+
+        Returns
+        -------
+        List[Thumbnail]
+            The list of file like thumbnails
+        """
+
+        files_raw = html.find(string="Files").parent.parent.parent.parent.find_all(
+            class_="row rowcontent clear"
+        )
+        files = []
+        for x in files_raw:
+            link = x.find("div", class_="content").h4.a
+            try:
+                image_url = link.parent.parent.parent.find("img")["src"]
+            except TypeError:
+                image_url = None
+
+            file = Thumbnail(
+                name=link.string,
+                url=link["href"],
+                image=image_url,
+                type=ThumbnailType.file,
+            )
+            files.append(file)
+
+        return files
+
+    def _get_engines(self, html: BeautifulSoup):
+        """Hidden method to get the engines showed currently on the page as a list of engine like thumbnails. Takes
+        an entire page of html and sorts it out
+
+        Parameters
+        -----------
+        html : BeautifulSoup
+            The page to cache the engines from
+
+        Returns
+        -------
+        List[Thumbnail]
+            The list of engine like thumbnail objects
+        """
+        engines_raw = html.find(string="Engines").parent.parent.parent.parent.find_all(
+            class_="row rowcontent clear"
+        )
+        engines = []
+        for x in engines_raw:
+            link = x.find("div", class_="content").h4.a
+            image_url = link.parent.parent.parent.find("img")["src"]
+            engine = Thumbnail(
+                name=link.string,
+                url=link["href"],
+                image=image_url,
+                type=ThumbnailType.engine,
+            )
+            engines.append(engine)
+
+        return engines
+
+    def __repr__(self):
+        return f"<{self.__class__.__name__} name={self.name}>"
+
+
+class HardwareSoftwareMetaClass(
+    BaseMetaClass, SharedMethodsMixin, RSSFeedMixin, GetWatchersMixin, GetTagsMixin
+):
+    """Shared class for Hardware and Software
+
+    Attributes
+    -----------
+    description : str
+        Description of the page
+    profile : Profile
+        The page's profile
+    stats : Statistics
+        The page's stats
+    rating : float
+        The rating of the item
+    articles : List[Thumbnail]
+        List of article type thumbnails from the recommended articles
+    article : PartialArticle
+        The partial article presented on the front page
+    tags : List[PartialTag]
+         A list of partial tags. You can use `get_tags` and then use the name id to get the right one.
+    medias : List[Thumbnail]
+        list of thumbnails representing all the combined media objects of a page (videos and images)
+    suggestions : List[Thumbnail]
+        list of suggested software/hardware type thumbnails
+    """
+
+    def __init__(self, html: BeautifulSoup):
+        super().__init__(html)
+        try:
+            self.description = html.find("div", id="profiledescription").p.string
+        except AttributeError:
+            self.description = html.find("p", itemprop="description").string
+
+        self.profile = Profile(html)
+
+        try:
+            self.stats = Statistics(html)
+        except AttributeError:
+            LOGGER.info("Entity '%s' has no stats (idk why, ask moddb)", self.name)
+            self.stats = None
+
+        try:
+            self.rating = float(
+                html.find("div", class_="score").find("meta", itemprop="ratingValue")["content"]
+            )
+        except AttributeError:
+            self.rating = 0.0
+            LOGGER.info("'%s' '%s' is not rated", self.profile.category.name, self.name)
+
+        try:
+            self._review_hash = html.find("form", class_="ratingform").find(
+                "input", {"name": "hash"}
+            )["value"]
+        except AttributeError:
+            self._review_hash = None
+
+        articles_raw = None
+        try:
+            articles_raw = html.find("span", string="Related Articles").parent.parent.parent.find(
+                "div", class_="table"
+            )
+            thumbnails = articles_raw.find_all("div", class_="row rowcontent clear")
+            self.articles = [
+                Thumbnail(
+                    name=x.a["title"],
+                    url=x.a["href"],
+                    image=x.a.img["src"] if x.a.img else None,
+                    summary=x.find("p").string,
+                    date=x.find("time")["datetime"],
+                    type=ThumbnailType.article,
+                )
+                for x in thumbnails
+            ]
+        except AttributeError:
+            LOGGER.info(
+                "'%s' '%s' has no article suggestions",
+                self.profile.category.name,
+                self.name,
+            )
+            self.articles = []
+
+        if articles_raw:
+            self.article = PartialArticle(articles_raw)
+        else:
+            self.article = None
+            LOGGER.info(
+                "'%s' '%s' has no front page article",
+                self.profile.category.name,
+                self.name,
+            )
+
+        try:
+            raw_tags = html.find("form", attrs={"name": "tagsform"}).find_all("a")
+            self.tags = [
+                PartialTag(x.string, join(x["href"]), x["href"].split("/")[-1])
+                for x in raw_tags
+                if x.string is not None
+            ]
+        except AttributeError:
+            self.tags = []
+            LOGGER.info("Hardware '%s' has no tags", self.name)
+
+        self.medias = self._get_media(1, html=html)
+
+        try:
+            t = ThumbnailType[self.__class__.__name__.lower()]
+            suggestions = html.find(
+                "span", string="You may also like"
+            ).parent.parent.parent.find_all("a", class_="image")
+            self.suggestions = [
+                Thumbnail(url=x["href"], name=x["title"], type=t, image=x.img["src"])
+                for x in suggestions
+            ]
+        except AttributeError:
+            LOGGER.info("'%s' '%s' has no suggestions", self.__class__.__name__, self.name)
```

### Comparing `moddb-0.8.1/moddb/pages/engine.py` & `moddb-0.9.0/moddb/pages/engine.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import bs4
-
-from ..utils import concat_docs, LOGGER
-from .base import PageMetaClass
-from .mixins import GetGamesMixin
-from ..enums import SearchCategory
-
-
-@concat_docs
-class Engine(PageMetaClass, GetGamesMixin):
-    """A subclass of Page, however, it does not have the files attribute
-
-    Parameters
-    -----------
-    html : bs4.BeautifulSoup
-        The html to parse. Allows for finer control.
-
-    Filtering
-    -----------
-    released : :class:`.Status`
-        The status of the engine (released, unreleased)
-    licence : :class:`.Licence`
-        The license of the engine
-    timeframe : :class:`.TimeFrame`
-        The time period this was released in (last 24hr, last week, last month)
-
-    Sorting
-    --------
-        * **released** - when the object was released, asc is oldest, desc is most recent
-        * **id** - when it was added to moddb, asc is oldest, desc is most recent
-        * **ranktoday** - order by daily ranking, asc is highest ranked, desc is lowest rank
-        * **visitstotal** - order by most views, asc is highest views, desc is lowest views
-        * **rating** - order by rating, asc is highest rating, desc is lowest rating
-        * **name** - order alphabetically, asc is a-z, desc is z-a
-        * **dateup** - order by latest update, asc is most recent update first, desc is oldest update first
-
-    Attributes
-    -----------
-    games : List[Thumbnail]
-        A list of games suggested on the engine main page.
-    """
-
-    def __init__(self, html: bs4.BeautifulSoup):
-        super().__init__(html, SearchCategory.engines)
-        delattr(self, "files")
-
-        try:
-            self.games = self._get_games(html)
-        except AttributeError:
-            LOGGER.info("Engine '%s' has no games", self.name)
-            self.games = []
+import bs4
+
+from ..enums import SearchCategory
+from ..utils import LOGGER, concat_docs
+from .base import PageMetaClass
+from .mixins import GetGamesMixin
+
+
+@concat_docs
+class Engine(PageMetaClass, GetGamesMixin):
+    """A subclass of Page, however, it does not have the files attribute
+
+    Parameters
+    -----------
+    html : bs4.BeautifulSoup
+        The html to parse. Allows for finer control.
+
+    Filtering
+    -----------
+    released : :class:`.Status`
+        The status of the engine (released, unreleased)
+    licence : :class:`.Licence`
+        The license of the engine
+    timeframe : :class:`.TimeFrame`
+        The time period this was released in (last 24hr, last week, last month)
+
+    Sorting
+    --------
+        * **released** - when the object was released, asc is oldest, desc is most recent
+        * **id** - when it was added to moddb, asc is oldest, desc is most recent
+        * **ranktoday** - order by daily ranking, asc is highest ranked, desc is lowest rank
+        * **visitstotal** - order by most views, asc is highest views, desc is lowest views
+        * **rating** - order by rating, asc is highest rating, desc is lowest rating
+        * **name** - order alphabetically, asc is a-z, desc is z-a
+        * **dateup** - order by latest update, asc is most recent update first, desc is oldest update first
+
+    Attributes
+    -----------
+    games : List[Thumbnail]
+        A list of games suggested on the engine main page.
+    """
+
+    def __init__(self, html: bs4.BeautifulSoup):
+        super().__init__(html, SearchCategory.engines)
+        delattr(self, "files")
+
+        try:
+            self.games = self._get_games(html)
+        except AttributeError:
+            LOGGER.info("Engine '%s' has no games", self.name)
+            self.games = []
```

### Comparing `moddb-0.8.1/moddb/pages/entity.py` & `moddb-0.9.0/moddb/pages/entity.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,495 +1,505 @@
-import bs4
-from typing import List, Tuple
-
-from ..utils import concat_docs, LOGGER, join, get_page
-from .base import PageMetaClass, BaseMetaClass
-from .mixins import (
-    GetAddonsMixin,
-    GetEnginesMixin,
-    GetGamesMixin,
-    GetModsMixin,
-    GetWaresMixin,
-)
-from ..boxes import (
-    Profile,
-    Statistics,
-    Thumbnail,
-    MemberProfile,
-    MemberStatistics,
-    ResultList,
-    CommentList,
-    _parse_results,
-)
-from ..enums import ThumbnailType, SearchCategory, TimeFrame, Membership, GroupCategory
-from .article import Blog
-
-
-@concat_docs
-class Group(PageMetaClass, GetAddonsMixin):
-    """This object represents the group model of  Certain attributes can be None if the group
-    has been set to private. If you wish to see a group you have access to then you can login with the
-    login
-
-    Parameters
-    -----------
-    html : bs4.BeautifulSoup
-        The html to parse. Allows for finer control.
-
-    Filtering
-    ----------
-    subscriptions : :class:`.Membership`
-        The subscription system of the group (private, invitation)
-    category : :class:`.GroupCategory`
-        The category of the group (funny, literature)
-
-    Sorting
-    --------
-        * **id** - order group by date, asc is most recent first, desc is oldest first
-        * **ranktoday** - order by daily ranking, asc is highest ranked, desc is lowest rank
-        * **visitstotal** - order by most views, asc is highest views, desc is lowest views
-        * **name** - order alphabetically, asc is a-z, desc is z-a
-        * **membercount** - order by number of members, asc is most members first, desc is lest member first
-
-    Attributes
-    -----------
-    name : str
-        The name of the group
-    private : bool
-        Whether or not the group is private
-    profile : Profile
-        The profile object for the group
-    stats : Statistics
-        The stats of the Group
-    tags : dict{str, str}
-        A dictionnary of tags where the key is the tag name and the value is the tag url
-    embed : str
-        The html for athe group embed
-    medias : List[Thumbnail]
-        A list of media like thumbnail objects representing all the images, videos and audio
-        clips that a group has published.
-    suggestions : List[Thumbnail]
-        A list of group like thumbnail objects representing the suggestions made by moddb to
-        members visiting this group
-    articles : List[Thumbnail]
-        A list of article like thumbnail objects representing some of the articles published
-        by the group
-    description : str
-        The plaintext description of the group
-    """
-
-    get_reviews = None
-
-    def __init__(self, html: bs4.BeautifulSoup):
-        self.name = html.find("div", class_="title").h2.a.string
-        BaseMetaClass.__init__(self, html)
-        self.private = False
-
-        try:
-            self.profile = Profile(html)
-        except AttributeError:
-            LOGGER.info("Entity '%s' has no profile (private)", self.name)
-            self.profile = None
-            self.private = True
-
-        try:
-            self.stats = Statistics(html)
-        except AttributeError:
-            LOGGER.info("Entity '%s' has no stats (private)", self.name)
-            self.stats = None
-
-        try:
-            raw_tags = html.find("form", attrs={"name": "tagsform"}).find_all("a")
-            self.tags = {x.string: join(x["href"]) for x in raw_tags if x.string is not None}
-        except AttributeError:
-            LOGGER.info("Entity '%s' has no tags (private)", self.name)
-            self.tags = {}
-
-        try:
-            self.embed = html.find("input", type="text", class_="text textembed")["value"]
-        except TypeError:
-            try:
-                self.embed = str(html.find_all("textarea")[1].a)
-            except IndexError:
-                LOGGER.info("Group '%s' has no embed", self.name)
-                self.embed = None
-
-        self.suggestions = self._get_suggestions(html)
-
-        try:
-            articles_raw = html.find("span", string="Articles").parent.parent.parent.find(
-                "div", class_="table"
-            )
-            thumbnails = articles_raw.find_all("div", class_="row rowcontent clear", recursive=False)
-            self.articles = [
-                Thumbnail(
-                    name=x.a["title"],
-                    url=x.a["href"],
-                    image=x.a.img["src"],
-                    summary=x.find("p").string,
-                    date=x.find("time")["datetime"],
-                    type=ThumbnailType.article,
-                )
-                for x in thumbnails
-            ]
-        except AttributeError:
-            LOGGER.info("Group '%s' has no article suggestions", self.name)
-            self.articles = []
-
-        try:
-            self.description = html.find("div", id="profiledescription").text
-        except AttributeError:
-            self.description = (
-                html.find("div", class_=["column", "span-all"]).find("div", class_="tooltip").parent.text
-            )
-
-        self.medias = self._get_media(2, html=html)
-
-    def _get_suggestions(self, html: bs4.BeautifulSoup) -> List[Thumbnail]:
-        """Hidden method used to get the list of suggestions on the page. As with most things, this list of suggestions
-        will be a list of Thumbnail objects that can be parsed individually. Slightly modified to fit a group
-
-        Parameters
-        -----------
-        html : bs4.BeautifulSoup
-            The html page we are trying to parse the suggestions for
-
-        Returns
-        --------
-        List[Thumbnail]
-            The list of suggestions as thumbnails.
-        """
-        try:
-            suggestions_raw = (
-                html.find("span", string=("You may also like", "Popular Articles"))
-                .parent.parent.parent.find("div", class_="table")
-                .find_all("div", recursive=False)
-            )
-        except AttributeError:
-            LOGGER.info("Group '%s' has no sidebar suggestions", self.name)
-            return []
-
-        suggestions = []
-        for x in suggestions_raw:
-            try:
-                link = x.find("a", class_="image")
-                suggestion_type = link["href"].split("/")[1].replace("s", "")
-                suggestion = Thumbnail(
-                    name=link["title"],
-                    url=link["href"],
-                    image=link.img["src"],
-                    type=ThumbnailType[suggestion_type],
-                )
-                suggestions.append(suggestion)
-            except (AttributeError, TypeError):
-                pass
-
-        return suggestions
-
-    def __repr__(self):
-        return f"<Group name={self.name}>"
-
-
-@concat_docs
-class Team(Group, GetEnginesMixin, GetGamesMixin, GetModsMixin, GetWaresMixin):
-    """A team is a group of people, which are the author of a game, a mod or an engine. A group has members which all
-    have rights on those page. Like a member but instead of a single person authoring various mods and games it's several.
-
-    Parameters
-    ------------
-    html : bs4.BeautifulSoup
-        The html to parse. Allows for finer control.
-
-    Filtering
-    ----------
-    subscriptions : :class:`.Membership`
-        The subscription system of the company (private, invitation)
-    category : :class:`.TeamCategory`
-        What does the team do (publisher, developer)
-
-    Sorting
-    --------
-        * **id** - order by creation, desc is most recent first, asc is oldest first
-        * **ranktoday** - order by daily ranking, asc is highest ranked, desc is lowest rank
-        * **visitstotal** - order by most views, asc is highest views, desc is lowest views
-        * **name** - order alphabetically, asc is a-z, desc is z-a
-        * **game** - order by game???
-        * **dateup** - order by latest update, asc is most recent update first, desc is oldest update first
-
-    Attributes
-    -----------
-    games : List[Thumbnail]
-        A list of game like thumbnails that the team has authored.
-    engines : List[Thumbnail]
-        A list of engine like objects that the team has authored.
-
-    """
-
-    def __init__(self, html: bs4.BeautifulSoup):
-        super().__init__(html)
-        try:
-            self.games = self._get_games(html)
-        except AttributeError:
-            LOGGER.info("Team '%s' has no games", self.name)
-            self.games = []
-
-        try:
-            self.engines = self._get_engines(html)
-        except AttributeError:
-            LOGGER.info("Team '%s' has no engines", self.name)
-            self.engines = []
-        try:
-            mods = (
-                html.find("span", string="Popular Mods")
-                .parent.parent.parent.find("div", class_="table")
-                .find_all("div", recursive=False)[1:]
-            )
-            self.mods = [
-                Thumbnail(
-                    name=x.a["title"],
-                    url=x.a["href"],
-                    type=ThumbnailType.mod,
-                    image=x.a.img["src"],
-                )
-                for x in mods
-            ]
-        except AttributeError:
-            LOGGER.info("Team '%s' has no mods", self.name)
-            self.mods = []
-
-
-@concat_docs
-class Member(PageMetaClass, GetGamesMixin, GetModsMixin, GetAddonsMixin):
-    """The object to represent an individual member on ModDB
-
-    Parameters
-    -----------
-    html : bs4.BeautifulSoup
-        The html to parse. Allows for finer control.
-
-    Sorting
-    --------
-    * **username** - sort alphabetically by username, asc is z-a and desc is a-z
-    * **id** - sort by member creation date, asc is most recent, desc is oldest
-    * **online** - sort by last online, asc is most recently seen online and desc is least recently
-
-    Attributes
-    -----------
-    profile : MemberProfile
-        Since member profile boxes have no overlap with other profiles, they are a separate object type
-        but serve the same function of making the side box "Profile" into an object, except exclusively
-        for a member page.
-    stats : MemberStatistics
-        Since member statistics have no overlap with regular statistic pages, they are a separate object type
-        but serve the same function of making the side box "Statistics" into an object, but exclusively for
-        the member page.
-    description : str
-        Description written on the member profile
-    groups : List[Thumbnail]
-        A list of group/team like thumbnail objects representing both the Teams the member is part of and the
-        Groups the member is part of.
-    blog : Blog
-        The front page blog shown on the member page
-    blogs : List[Thumbnail]
-        A list of blog like thumbnails representing the blog suggestion of a member's frontpage
-    friends : List[Thumnails]
-        A list of member like thumbnails representing some of the friends shown on the member's front
-        page
-    """
-
-    def __init__(self, html: bs4.BeautifulSoup):
-        super().__init__(html, SearchCategory.members)
-        try:
-            self.profile = MemberProfile(html)
-        except AttributeError:
-            LOGGER.info("Member '%s' has no profile (private)", self.name)
-            self.profile = None
-
-        try:
-            self.stats = MemberStatistics(html)
-        except AttributeError:
-            LOGGER.info("Member '%s' has no stats (private)", self.name)
-            self.stats = None
-
-        try:
-            self.description = html.find("div", id="profiledescription").p.string
-        except AttributeError:
-            LOGGER.info("Member '%s' has no description", self.name)
-            self.description = None
-
-        try:
-            groups_raw = (
-                html.find("span", string="Groups")
-                .parent.parent.parent.find("div", class_="table")
-                .find_all("div", recursive=False)[:-2]
-            )
-            self.groups = [
-                Thumbnail(name=div.a["title"], url=div.a["href"], type=ThumbnailType.group)
-                for div in groups_raw
-            ]
-        except AttributeError:
-            LOGGER.info("Member '%s' doesn't have any groups", self.name)
-            self.groups = []
-
-        try:
-            blogs_raw = (
-                html.find("span", string="My Blogs")
-                .parent.parent.parent.find("div", class_="table")
-                .find_all("div", recursive=False)
-            )
-            self.blog = Blog(heading=blogs_raw.pop(0), text=blogs_raw.pop(0))
-        except (TypeError, AttributeError):
-            self.blog = None
-            LOGGER.info("Member '%s' has no front page blog", self.name)
-
-        try:
-            blogs_raw = (
-                html.find("span", string="My Blogs")
-                .parent.parent.parent.find("div", class_="table")
-                .find_all("div", recursive=False)
-            )
-            self.blogs = [
-                Thumbnail(name=blog.a.string, url=blog.a["href"], type=ThumbnailType.blog)
-                for blog in blogs_raw[:-2]
-            ]
-        except (TypeError, AttributeError):
-            self.blogs = []
-            LOGGER.info("Member '%s' has no blog suggestions", self.name)
-
-        try:
-            friends = html.find("div", class_="table tablerelated").find_all("div", recursive=False)[1:]
-            self.friends = [
-                Thumbnail(
-                    name=friend.a["title"],
-                    url=friend.a["href"],
-                    type=ThumbnailType.member,
-                )
-                for friend in friends
-            ]
-        except AttributeError:
-            self.friends = []
-            LOGGER.info("Member '%s' has no friends ;(", self.name)
-
-    def __repr__(self):
-        return f"<Member name={self.name} level={self.profile.level}>"
-
-    def get_blogs(
-        self,
-        index: int = 1,
-        *,
-        query: str = None,
-        timeframe: TimeFrame = None,
-        sort: Tuple[str, str] = None,
-    ) -> ResultList:
-        """Search through a member's blogs one page at a time with certain filters.
-
-        Parameters
-        -----------
-        index : int
-            The page index you wish to get the blogs for, allows to hop around.
-        timeframe : TimeFrame
-            The date the blog was added, optional
-        query : str
-            The string to look for in the blog title, optional.
-        sort : Tuple[str, str]
-            The sorting tuple to sort by
-
-        Returns
-        --------
-        ResultList[Blog]
-            The list of blogs on this page.
-        """
-        params = {
-            "filter": "t",
-            "kw": query,
-            "timeframe": timeframe.value if timeframe else None,
-            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
-        }
-
-        url = f"{self.url}/blogs"
-        html = get_page(f"{url}/page/{index}", params=params)
-        results, current_page, total_pages, total_results = _parse_results(html)
-
-        return ResultList(
-            results=results,
-            params=params,
-            url=url,
-            current_page=current_page,
-            total_pages=total_pages,
-            total_results=total_results,
-        )
-
-    def get_member_comments(self, index: int = 1, *, show_deleted: bool = False) -> CommentList:
-        """Gets a page of all the comments a member has posted.
-
-        Parameters
-        -----------
-        index : int
-            The page number to get the comments from.
-        show_deleted : Optional[bool]
-            Pass true to show deleted user comments. Only works if it is a page
-            you have permissions on.
-
-        Returns
-        --------
-        CommentList[Comment]
-            A list of the comments made by the user.
-
-        """
-        params = {"deleted": "t" if show_deleted else None}
-
-        html = get_page(f"{self.url}/comments/page/{index}", params=params)
-        return self._get_comments(html)
-
-    def get_friends(self, index: int = 1, *, username: str = None) -> ResultList:
-        """Get a page of the friends of the member
-
-        Parameters
-        -----------
-        index : int
-            The page number to get the friends from.
-        username : Optional[str]
-            The username of the user you are looking for
-
-        Returns
-        --------
-        ResultList[Thumbnail]
-            A list of member like thumbnails of the member's friends
-        """
-        params = {"filter": "t", "username": username}
-
-        return self._get(f"{self.url}/friends/page/{index}", params=params)
-
-    def get_groups(
-        self,
-        index: int = 1,
-        *,
-        query: str = None,
-        subscription: Membership = None,
-        category: GroupCategory = None,
-    ) -> ResultList:
-        """Get a page of the groups and teams a member is part of.
-
-        Parameters
-        -----------
-        index : int
-            The page number to get the friends from.
-        query : Optional[str]
-            The text to look for in the group's name
-        subscription : Optional[Membership]
-            The membership rules
-        category : Optional[GroupCategory]
-            The category of groups to search for
-
-        Returns
-        --------
-        ResultList[Thumbnail]
-            A list of team/group like thumbnails the member is part of
-        """
-        params = {
-            "filter": "t",
-            "kw": query,
-            "subscription": subscription.value if subscription else None,
-            "category": category.value if category else None,
-        }
-
-        return self._get(f"{self.url}/groups/page/{index}", params=params)
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, List, Tuple
+
+from ..boxes import (
+    MemberProfile,
+    MemberStatistics,
+    PartialTag,
+    Profile,
+    ResultList,
+    Statistics,
+    Thumbnail,
+    _parse_results,
+)
+from ..enums import GroupCategory, Membership, SearchCategory, ThumbnailType, TimeFrame
+from ..utils import LOGGER, concat_docs, get_page, join
+from .article import Blog
+from .base import BaseMetaClass, PageMetaClass
+from .mixins import GetAddonsMixin, GetEnginesMixin, GetGamesMixin, GetModsMixin, GetWaresMixin
+
+if TYPE_CHECKING:
+    import bs4
+
+    from ..boxes import CommentList
+
+
+@concat_docs
+class Group(PageMetaClass, GetAddonsMixin):
+    """This object represents the group model of  Certain attributes can be None if the group
+    has been set to private. If you wish to see a group you have access to then you can login with the
+    login
+
+    Parameters
+    -----------
+    html : bs4.BeautifulSoup
+        The html to parse. Allows for finer control.
+
+    Filtering
+    ----------
+    subscriptions : :class:`.Membership`
+        The subscription system of the group (private, invitation)
+    category : :class:`.GroupCategory`
+        The category of the group (funny, literature)
+
+    Sorting
+    --------
+        * **id** - order group by date, asc is most recent first, desc is oldest first
+        * **ranktoday** - order by daily ranking, asc is highest ranked, desc is lowest rank
+        * **visitstotal** - order by most views, asc is highest views, desc is lowest views
+        * **name** - order alphabetically, asc is a-z, desc is z-a
+        * **membercount** - order by number of members, asc is most members first, desc is lest member first
+
+    Attributes
+    -----------
+    name : str
+        The name of the group
+    private : bool
+        Whether or not the group is private
+    profile : Profile
+        The profile object for the group
+    stats : Statistics
+        The stats of the Group
+    tags : List[PartialTag]
+        A list of partial tags. You can use `get_tags` and then use the name id to get the right one.
+    embed : str
+        The html for athe group embed
+    medias : List[Thumbnail]
+        A list of media like thumbnail objects representing all the images, videos and audio
+        clips that a group has published.
+    suggestions : List[Thumbnail]
+        A list of group like thumbnail objects representing the suggestions made by moddb to
+        members visiting this group
+    articles : List[Thumbnail]
+        A list of article like thumbnail objects representing some of the articles published
+        by the group
+    description : str
+        The plaintext description of the group
+    """
+
+    get_reviews = None
+
+    def __init__(self, html: bs4.BeautifulSoup):
+        self.name = html.find("div", class_="title").h2.a.string
+        BaseMetaClass.__init__(self, html)
+        self.private = False
+
+        try:
+            self.profile = Profile(html)
+        except AttributeError:
+            LOGGER.info("Entity '%s' has no profile (private)", self.name)
+            self.profile = None
+            self.private = True
+
+        try:
+            self.stats = Statistics(html)
+        except AttributeError:
+            LOGGER.info("Entity '%s' has no stats (private)", self.name)
+            self.stats = None
+
+        try:
+            raw_tags = html.find("form", attrs={"name": "tagsform"}).find_all("a")
+            self.tags = [
+                PartialTag(x.string, join(x["href"]), x["href"].split("/")[-1])
+                for x in raw_tags
+                if x.string is not None
+            ]
+        except AttributeError:
+            LOGGER.info("Entity '%s' has no tags (private)", self.name)
+            self.tags = []
+
+        try:
+            self.embed = html.find("input", type="text", class_="text textembed")["value"]
+        except TypeError:
+            try:
+                self.embed = str(html.find_all("textarea")[1].a)
+            except IndexError:
+                LOGGER.info("Group '%s' has no embed", self.name)
+                self.embed = None
+
+        self.suggestions = self._get_suggestions(html)
+
+        try:
+            articles_raw = html.find("span", string="Articles").parent.parent.parent.find(
+                "div", class_="table"
+            )
+            thumbnails = articles_raw.find_all(
+                "div", class_="row rowcontent clear", recursive=False
+            )
+            self.articles = [
+                Thumbnail(
+                    name=x.a["title"],
+                    url=x.a["href"],
+                    image=x.a.img["src"],
+                    summary=x.find("p").string,
+                    date=x.find("time")["datetime"],
+                    type=ThumbnailType.article,
+                )
+                for x in thumbnails
+            ]
+        except AttributeError:
+            LOGGER.info("Group '%s' has no article suggestions", self.name)
+            self.articles = []
+
+        try:
+            self.description = html.find("div", id="profiledescription").text
+        except AttributeError:
+            self.description = (
+                html.find("div", class_=["column", "span-all"])
+                .find("div", class_="tooltip")
+                .parent.text
+            )
+
+        self.medias = self._get_media(2, html=html)
+
+    def _get_suggestions(self, html: bs4.BeautifulSoup) -> List[Thumbnail]:
+        """Hidden method used to get the list of suggestions on the page. As with most things, this list of suggestions
+        will be a list of Thumbnail objects that can be parsed individually. Slightly modified to fit a group
+
+        Parameters
+        -----------
+        html : bs4.BeautifulSoup
+            The html page we are trying to parse the suggestions for
+
+        Returns
+        --------
+        List[Thumbnail]
+            The list of suggestions as thumbnails.
+        """
+        try:
+            suggestions_raw = (
+                html.find("span", string=("You may also like", "Popular Articles"))
+                .parent.parent.parent.find("div", class_="table")
+                .find_all("div", recursive=False)
+            )
+        except AttributeError:
+            LOGGER.info("Group '%s' has no sidebar suggestions", self.name)
+            return []
+
+        suggestions = []
+        for x in suggestions_raw:
+            try:
+                link = x.find("a", class_="image")
+                suggestion_type = link["href"].split("/")[1].replace("s", "")
+                suggestion = Thumbnail(
+                    name=link["title"],
+                    url=link["href"],
+                    image=link.img["src"],
+                    type=ThumbnailType[suggestion_type],
+                )
+                suggestions.append(suggestion)
+            except (AttributeError, TypeError):
+                pass
+
+        return suggestions
+
+    def __repr__(self):
+        return f"<Group name={self.name}>"
+
+
+@concat_docs
+class Team(Group, GetEnginesMixin, GetGamesMixin, GetModsMixin, GetWaresMixin):
+    """A team is a group of people, which are the author of a game, a mod or an engine. A group has members which all
+    have rights on those page. Like a member but instead of a single person authoring various mods and games it's several.
+
+    Parameters
+    ------------
+    html : bs4.BeautifulSoup
+        The html to parse. Allows for finer control.
+
+    Filtering
+    ----------
+    subscriptions : :class:`.Membership`
+        The subscription system of the company (private, invitation)
+    category : :class:`.TeamCategory`
+        What does the team do (publisher, developer)
+
+    Sorting
+    --------
+        * **id** - order by creation, desc is most recent first, asc is oldest first
+        * **ranktoday** - order by daily ranking, asc is highest ranked, desc is lowest rank
+        * **visitstotal** - order by most views, asc is highest views, desc is lowest views
+        * **name** - order alphabetically, asc is a-z, desc is z-a
+        * **game** - order by game???
+        * **dateup** - order by latest update, asc is most recent update first, desc is oldest update first
+
+    Attributes
+    -----------
+    games : List[Thumbnail]
+        A list of game like thumbnails that the team has authored.
+    engines : List[Thumbnail]
+        A list of engine like objects that the team has authored.
+
+    """
+
+    def __init__(self, html: bs4.BeautifulSoup):
+        super().__init__(html)
+        try:
+            self.games = self._get_games(html)
+        except AttributeError:
+            LOGGER.info("Team '%s' has no games", self.name)
+            self.games = []
+
+        try:
+            self.engines = self._get_engines(html)
+        except AttributeError:
+            LOGGER.info("Team '%s' has no engines", self.name)
+            self.engines = []
+        try:
+            mods = (
+                html.find("span", string="Popular Mods")
+                .parent.parent.parent.find("div", class_="table")
+                .find_all("div", recursive=False)[1:]
+            )
+            self.mods = [
+                Thumbnail(
+                    name=x.a["title"],
+                    url=x.a["href"],
+                    type=ThumbnailType.mod,
+                    image=x.a.img["src"],
+                )
+                for x in mods
+            ]
+        except AttributeError:
+            LOGGER.info("Team '%s' has no mods", self.name)
+            self.mods = []
+
+
+@concat_docs
+class Member(PageMetaClass, GetGamesMixin, GetModsMixin, GetAddonsMixin):
+    """The object to represent an individual member on ModDB
+
+    Parameters
+    -----------
+    html : bs4.BeautifulSoup
+        The html to parse. Allows for finer control.
+
+    Sorting
+    --------
+    * **username** - sort alphabetically by username, asc is z-a and desc is a-z
+    * **id** - sort by member creation date, asc is most recent, desc is oldest
+    * **online** - sort by last online, asc is most recently seen online and desc is least recently
+
+    Attributes
+    -----------
+    profile : MemberProfile
+        Since member profile boxes have no overlap with other profiles, they are a separate object type
+        but serve the same function of making the side box "Profile" into an object, except exclusively
+        for a member page.
+    stats : MemberStatistics
+        Since member statistics have no overlap with regular statistic pages, they are a separate object type
+        but serve the same function of making the side box "Statistics" into an object, but exclusively for
+        the member page.
+    description : str
+        Description written on the member profile
+    groups : List[Thumbnail]
+        A list of group/team like thumbnail objects representing both the Teams the member is part of and the
+        Groups the member is part of.
+    blog : Blog
+        The front page blog shown on the member page
+    blogs : List[Thumbnail]
+        A list of blog like thumbnails representing the blog suggestion of a member's frontpage
+    friends : List[Thumnails]
+        A list of member like thumbnails representing some of the friends shown on the member's front
+        page
+    """
+
+    def __init__(self, html: bs4.BeautifulSoup):
+        super().__init__(html, SearchCategory.members)
+        try:
+            self.profile = MemberProfile(html)
+        except AttributeError:
+            LOGGER.info("Member '%s' has no profile (private)", self.name)
+            self.profile = None
+
+        try:
+            self.stats = MemberStatistics(html)
+        except AttributeError:
+            LOGGER.info("Member '%s' has no stats (private)", self.name)
+            self.stats = None
+
+        try:
+            self.description = html.find("div", id="profiledescription").p.string
+        except AttributeError:
+            LOGGER.info("Member '%s' has no description", self.name)
+            self.description = None
+
+        try:
+            groups_raw = (
+                html.find("span", string="Groups")
+                .parent.parent.parent.find("div", class_="table")
+                .find_all("div", recursive=False)[:-2]
+            )
+            self.groups = [
+                Thumbnail(name=div.a["title"], url=div.a["href"], type=ThumbnailType.group)
+                for div in groups_raw
+            ]
+        except AttributeError:
+            LOGGER.info("Member '%s' doesn't have any groups", self.name)
+            self.groups = []
+
+        try:
+            blogs_raw = (
+                html.find("span", string="My Blogs")
+                .parent.parent.parent.find("div", class_="table")
+                .find_all("div", recursive=False)
+            )
+            self.blog = Blog(heading=blogs_raw.pop(0), text=blogs_raw.pop(0))
+        except (TypeError, AttributeError):
+            self.blog = None
+            LOGGER.info("Member '%s' has no front page blog", self.name)
+
+        try:
+            blogs_raw = (
+                html.find("span", string="My Blogs")
+                .parent.parent.parent.find("div", class_="table")
+                .find_all("div", recursive=False)
+            )
+            self.blogs = [
+                Thumbnail(name=blog.a.string, url=blog.a["href"], type=ThumbnailType.blog)
+                for blog in blogs_raw[:-2]
+            ]
+        except (TypeError, AttributeError):
+            self.blogs = []
+            LOGGER.info("Member '%s' has no blog suggestions", self.name)
+
+        try:
+            friends = html.find("div", class_="table tablerelated").find_all(
+                "div", recursive=False
+            )[1:]
+            self.friends = [
+                Thumbnail(
+                    name=friend.a["title"],
+                    url=friend.a["href"],
+                    type=ThumbnailType.member,
+                )
+                for friend in friends
+            ]
+        except AttributeError:
+            self.friends = []
+            LOGGER.info("Member '%s' has no friends ;(", self.name)
+
+    def __repr__(self):
+        return f"<Member name={self.name} level={self.profile.level}>"
+
+    def get_blogs(
+        self,
+        index: int = 1,
+        *,
+        query: str = None,
+        timeframe: TimeFrame = None,
+        sort: Tuple[str, str] = None,
+    ) -> ResultList:
+        """Search through a member's blogs one page at a time with certain filters.
+
+        Parameters
+        -----------
+        index : int
+            The page index you wish to get the blogs for, allows to hop around.
+        timeframe : TimeFrame
+            The date the blog was added, optional
+        query : str
+            The string to look for in the blog title, optional.
+        sort : Tuple[str, str]
+            The sorting tuple to sort by
+
+        Returns
+        --------
+        ResultList[Blog]
+            The list of blogs on this page.
+        """
+        params = {
+            "filter": "t",
+            "kw": query,
+            "timeframe": timeframe.value if timeframe else None,
+            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
+        }
+
+        url = f"{self.url}/blogs"
+        html = get_page(f"{url}/page/{index}", params=params)
+        results, current_page, total_pages, total_results = _parse_results(html)
+
+        return ResultList(
+            results=results,
+            params=params,
+            url=url,
+            current_page=current_page,
+            total_pages=total_pages,
+            total_results=total_results,
+        )
+
+    def get_member_comments(self, index: int = 1, *, show_deleted: bool = False) -> CommentList:
+        """Gets a page of all the comments a member has posted.
+
+        Parameters
+        -----------
+        index : int
+            The page number to get the comments from.
+        show_deleted : Optional[bool]
+            Pass true to show deleted user comments. Only works if it is a page
+            you have permissions on.
+
+        Returns
+        --------
+        CommentList[Comment]
+            A list of the comments made by the user.
+
+        """
+        params = {"deleted": "t" if show_deleted else None}
+
+        html = get_page(f"{self.url}/comments/page/{index}", params=params)
+        return self._get_comments(html)
+
+    def get_friends(self, index: int = 1, *, username: str = None) -> ResultList:
+        """Get a page of the friends of the member
+
+        Parameters
+        -----------
+        index : int
+            The page number to get the friends from.
+        username : Optional[str]
+            The username of the user you are looking for
+
+        Returns
+        --------
+        ResultList[Thumbnail]
+            A list of member like thumbnails of the member's friends
+        """
+        params = {"filter": "t", "username": username}
+
+        return self._get(f"{self.url}/friends/page/{index}", params=params)
+
+    def get_groups(
+        self,
+        index: int = 1,
+        *,
+        query: str = None,
+        subscription: Membership = None,
+        category: GroupCategory = None,
+    ) -> ResultList:
+        """Get a page of the groups and teams a member is part of.
+
+        Parameters
+        -----------
+        index : int
+            The page number to get the friends from.
+        query : Optional[str]
+            The text to look for in the group's name
+        subscription : Optional[Membership]
+            The membership rules
+        category : Optional[GroupCategory]
+            The category of groups to search for
+
+        Returns
+        --------
+        ResultList[Thumbnail]
+            A list of team/group like thumbnails the member is part of
+        """
+        params = {
+            "filter": "t",
+            "kw": query,
+            "subscription": subscription.value if subscription else None,
+            "category": category.value if category else None,
+        }
+
+        return self._get(f"{self.url}/groups/page/{index}", params=params)
```

### Comparing `moddb-0.8.1/moddb/pages/file.py` & `moddb-0.9.0/moddb/pages/file.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,350 +1,361 @@
-import re
-import bs4
-import sys
-import datetime
-import requests
-
-from ..utils import (
-    BASE_URL,
-    concat_docs,
-    get_date,
-    get_page,
-    raise_for_status,
-    join,
-    get_views,
-    prepare_request,
-)
-from .base import BaseMetaClass
-from ..enums import FileCategory, AddonCategory, ThumbnailType, MediaCategory
-from ..boxes import Mirror, Thumbnail
-
-
-@concat_docs
-class File(BaseMetaClass):
-    """An oject representing a file on ModDB, a file is something posted by the page owner which is directly linked
-    to the page. It is endorsed by the page owner and they should do everythign they can to make sure that it is safe.
-    As compared to an addon that may be added by fans to the page and that are files meant to work with the page but
-    that are not directly related to the page. E.x the file of a mod page would be the mod files used to install the
-    mod whereas an addon could be something like a fan-made texture pack for the mod or a map.
-
-    Parameters
-    -----------
-    html : bs4.BeautifulSoup
-        The html to parse. Allows for finer control.
-
-    Filtering
-    ----------
-    category  : :class:`.FileCategory`
-        The type of file (audio, video, demo, full version....)
-    categoryaddon : :class:`.AddonCategory`
-        The type of addon (map, textures, ect...)
-    game : Union[:class:`.Game`, :class:`.Object`]
-        An game object or an object with an id attribute which represents the
-        game the file belongs to.
-    timeframe : :class:`.TimeFrame`
-        The time period this was released in (last 24hr, last week, last month)
-
-    Sorting
-    --------
-        * **released** - when the object was released, asc is oldest, desc is most recent
-        * **id** - when it was added to moddb, asc is oldest, desc is most recent
-        * **ranktoday** - order by daily ranking, asc is highest ranked, desc is lowest rank
-        * **visitstotal** - order by most views, asc is highest views, desc is lowest views
-        * **rating** - order by rating, asc is highest rating, desc is lowest rating
-        * **name** - order alphabetically, asc is a-z, desc is z-a
-        * **date** - order by upload date, asc is most recent first, desc is oldest first
-
-    Attributes
-    -----------
-    filename : str
-        The name of the file
-    hash : str
-        The MD5 hash of the file
-    name : str
-        The name of the page
-    size : int
-        the file size in bytes
-    today : int
-        The number of downloads today
-    downloads : int
-        The total number of times this file has been downloaded
-    category : FileCategory
-        The category of the file
-    author : Thumbnail
-        A member type thumbnail of the member who uploaded the file
-    date : datetime.datetime
-        The date the file was uploaded
-    button : str
-        html code for the embed button
-    widget : str
-        html code for the embed widget
-    description : str
-        Description of the file, as written by the author
-    preview : str
-        URL of the preview image for the file
-    """
-
-    def __init__(self, html: bs4.BeautifulSoup):
-        if html.find("span", string="File Deleted", class_="heading"):
-            raise ValueError("This file has been removed")
-
-        info = html.find("div", class_="table tablemenu")
-        file = {
-            x.string.lower(): x.parent.span.string.strip()
-            for x in info.find_all("h5", string=("Filename", "Size", "MD5 Hash"))
-        }
-        self.name = html.find("a", title="Report").parent.parent.find("span", class_="heading").string
-        self.filename = file["filename"]
-        super().__init__(html)
-
-        self.hash = file["md5 hash"]
-        self.size = int(re.sub(r"[(),bytes]", "", file["size"].split(" ")[1]))
-
-        downloads = html.find("h5", string="Downloads").parent.a.string
-        self.today = int(re.sub(r"[(),today]", "", downloads.split(" ")[1]))
-        self.downloads = int(downloads.split(" ")[0].replace(",", ""))
-
-        try:
-            self.category = FileCategory(
-                int(info.find("h5", string="Category").parent.a["href"].split("=")[-1])
-            )
-        except ValueError:
-            self.category = AddonCategory(
-                int(info.find("h5", string="Category").parent.a["href"].split("=")[-1])
-            )
-
-        uploader = info.find("h5", string="Uploader").parent.a
-        self.author = Thumbnail(url=uploader["href"], name=uploader.string, type=ThumbnailType.member)
-
-        self.date = get_date(info.find("h5", string="Added").parent.span.time["datetime"])
-        self.button = info.find("h5", string="Embed Button").parent.span.input["value"]
-        self.widget = info.find("h5", string="Embed Widget").parent.span.input["value"]
-
-        self.description = html.find("p", id="downloadsummary").string
-
-        self.preview = html.find_all("img", src=True)[0]["src"]
-
-    def __repr__(self):
-        return f"<{self.__class__.__name__} name={self.name} type={self.category.name}>"
-
-    def save(self, file_obj, *, mirror=None):
-        """Save the file to an object. This functions makes
-        two requests. If you pass a valid mirror it will
-        make only one request.
-
-        Parameters
-        -----------
-        file_obj : typing.BinaryIO
-            The file obj to save the file to. The binary data
-            will be streamed to that object.
-        mirror : Optional[Mirror]
-            An optional mirror object to download the
-            file from a specific moddb mirror
-
-        """
-        if mirror is None:
-            download = get_page(f"{BASE_URL}/downloads/start/{self.id}")
-            url = download.find("a", string=f"download {self.filename}")["href"]
-        else:
-            url = mirror._url
-
-        SESSION = sys.modules["moddb"].SESSION
-        prepped = prepare_request(requests.Request("GET", join(url)), SESSION)
-        with SESSION.send(prepped, stream=True) as r:
-            raise_for_status(r)
-            for chunk in r.iter_content(chunk_size=8192):
-                file_obj.write(chunk)
-
-    def get_mirrors(self):
-        """Get all the mirrors from which a file can be downloaded. This
-        can then be passed to File.save to download from a specific mirror.
-
-
-        Returns
-        --------
-        List[Mirror]
-            A list of Mirror objects"""
-
-        html = get_page(f"https://www.moddb.com/downloads/start/{self.id}/all")
-        mirrors_div = html.find("div", class_="mirrors").find_all("div", recursive=False)
-        mirrors = []
-        for mirror in mirrors_div:
-            mirror_match = re.match(r"(.*) #([0-9]*) \((\w+), (\w+)\)", mirror.div.p.contents[-1].strip())
-            stats_match = re.match(
-                r"([0-9,]*) downloads? served, ([0-9.]*)% capacity",
-                mirror.div.span.string,
-            )
-
-            mirrors.append(
-                Mirror(
-                    name=mirror_match.group(1),
-                    index=int(mirror_match.group(2)),
-                    city=mirror_match.group(3),
-                    country=mirror_match.group(4),
-                    served=int(stats_match.group(1).replace(",", "")),
-                    capacity=float(stats_match.group(2)),
-                    url=mirror.div.p.a["href"],
-                )
-            )
-
-        return mirrors
-
-
-@concat_docs
-class Addon(File):
-    """Object representing an addon. Seemingly the only difference between an addon and a file is in
-    the semantics. A file often represents something official released by the page, e.g. the mod installation
-    or an official guide where as addons are often fan made and might not be directly endorsed by the page owners
-    even if it is allowed. They literally add on to the page's content without becoming part of it. There is a slight
-    difference in their profiles but nothing beyond that.
-
-    Parameters
-    -----------
-    html : bs4.BeautifulSoup
-        The html to parse. Allows for finer control.
-
-    Filtering
-    ----------
-    categoryaddon : :class:`.AddonCategory`
-        The type of addon (map, textures, ect...)
-    licence : :class:`.Licence`
-        The licence of the addon
-    game : Union[:class:`.Game`, :class:`.Object`]
-        An game object or an object with an id attribute which represents the
-        game the addon belongs to.
-    timeframe : :class:`.TimeFrame`
-        The time period this was released in (last 24hr, last week, last month)
-
-    Sorting
-    --------
-        * **released** - when the object was released, asc is oldest, desc is most recent
-        * **id** - when it was added to moddb, asc is oldest, desc is most recent
-        * **ranktoday** - order by daily ranking, asc is highest ranked, desc is lowest rank
-        * **visitstotal** - order by most views, asc is highest views, desc is lowest views
-        * **rating** - order by rating, asc is highest rating, desc is lowest rating
-        * **name** - order alphabetically, asc is a-z, desc is z-a
-        * **licence** - order based on licence
-        * **date** - order by upload date, asc is most recent first, desc is oldest first
-
-
-    """
-
-    pass
-
-
-@concat_docs
-class Media(BaseMetaClass):
-    """Represents an image, audio file or video file on
-
-    Parameters
-    -----------
-    html : bs4.BeautifulSoup
-        The html to parse. Allows for finer control.
-
-    Filtering
-    -----------
-    sitearea : :class:`.Category`
-        The type of model the media belongs to. Category.downloads is not valid for this.
-
-    Sorting
-    --------
-        * **ranktoday** - order by daily ranking, asc is highest ranked, desc is lowest rank
-        * **visitstotal** - order by most views, asc is highest views, desc is lowest views
-        * **name** - order alphabetically, asc is a-z, desc is z-a
-        * **id** - order by upload date, asc is most recent first, desc is oldest first
-
-        Exclusive to videos and audios
-        * **duration** - order by duration, asc is shortest to longest, desc is longest first
-
-    Attributes
-    -----------
-    date : datetime.datetime
-        The date the media was uploaded
-    name : str
-        The name of the media
-    author : Thumbnail
-        Member type thumbnail of the media uploader
-    duration : datetime.timedelta
-        Duration of the media in seconds, 0 if it's an image
-    size : int
-        Size of the files in bytes
-    views : int
-        Total amount of views
-    today : int
-        Amount of views today
-    filename : str
-        The name of the file for the media
-    fileurl : str
-        The url of the file for the media
-    category : MediaCategory
-        Whether the media is an image, a video or an audio
-    description : str
-        The description of the file as given by the file uploader.
-    """
-
-    def __init__(self, html: bs4.BeautifulSoup):
-        try:
-            self.name = html.find("meta", itemprop="name")["content"]
-        except TypeError:
-            self.name = html.find("img", id="mediaimage")["title"]
-
-        super().__init__(html)
-        medias = html.find_all("h5", string=("Date", "By", "Duration", "Size", "Views", "Filename"))
-        raw_media = {media.string.lower(): media.parent for media in medias}
-
-        self.date = get_date(raw_media["date"].span.time["datetime"])
-
-        author = raw_media["by"].span.a
-        self.author = Thumbnail(url=author["href"], name=author.string.strip(), type=ThumbnailType.member)
-
-        if "duration" in raw_media:
-            duration = raw_media["duration"].span.time.string.strip().split(":")
-            duration.reverse()
-            times = ["seconds", "minutes", "hours"]
-            self.duration = datetime.timedelta(**{times[duration.index(x)]: int(x) for x in duration})
-        else:
-            self.duration = 0
-
-        if "size" in raw_media:
-            self.size = tuple(raw_media["size"].span.string.strip().split("×"))
-
-        self.views, self.today = get_views(raw_media["views"].a.string)
-        media_player = html.find("video", id="mediaplayer")
-
-        if not media_player:
-            self.category = MediaCategory.image
-            self.fileurl = html.find("meta", property="og:image")["content"]
-        else:
-            self.fileurl = media_player.source["src"]
-            if "audio" in media_player.source["type"]:
-                self.category = MediaCategory.audio
-            else:
-                self.category = MediaCategory.video
-
-        if "filename" in raw_media:
-            self.filename = raw_media["filename"].span.string.strip()
-        else:
-            self.filename = self.fileurl.split("/")[-1]
-
-        self.description = html.find("meta", {"name": "description"})["content"]
-
-    def __repr__(self):
-        return f"<Media name={self.name} type={self.category.name}>"
-
-    def save(self, file_obj):
-        """Save the media to an object.
-
-        Parameters
-        -----------
-        file_obj : typing.BinaryIO
-            The file obj to save the file to. The binary data
-            will be streamed to that object.
-
-        """
-        SESSION = sys.modules["moddb"].SESSION
-        prepped = prepare_request(requests.Request("GET", self.fileurl), SESSION)
-
-        with SESSION.send(prepped, stream=True) as r:
-            raise_for_status(r)
-            for chunk in r.iter_content(chunk_size=8192):
-                file_obj.write(chunk)
+import datetime
+import re
+import sys
+
+import bs4
+import requests
+
+from ..boxes import Mirror, Thumbnail
+from ..enums import AddonCategory, FileCategory, MediaCategory, ThumbnailType
+from ..utils import (
+    BASE_URL,
+    concat_docs,
+    get_date,
+    get_page,
+    get_views,
+    join,
+    prepare_request,
+    raise_for_status,
+)
+from .base import BaseMetaClass
+
+
+@concat_docs
+class File(BaseMetaClass):
+    """An oject representing a file on ModDB, a file is something posted by the page owner which is directly linked
+    to the page. It is endorsed by the page owner and they should do everythign they can to make sure that it is safe.
+    As compared to an addon that may be added by fans to the page and that are files meant to work with the page but
+    that are not directly related to the page. E.x the file of a mod page would be the mod files used to install the
+    mod whereas an addon could be something like a fan-made texture pack for the mod or a map.
+
+    Parameters
+    -----------
+    html : bs4.BeautifulSoup
+        The html to parse. Allows for finer control.
+
+    Filtering
+    ----------
+    category  : :class:`.FileCategory`
+        The type of file (audio, video, demo, full version....)
+    categoryaddon : :class:`.AddonCategory`
+        The type of addon (map, textures, ect...)
+    game : Union[:class:`.Game`, :class:`.Object`]
+        An game object or an object with an id attribute which represents the
+        game the file belongs to.
+    timeframe : :class:`.TimeFrame`
+        The time period this was released in (last 24hr, last week, last month)
+
+    Sorting
+    --------
+        * **released** - when the object was released, asc is oldest, desc is most recent
+        * **id** - when it was added to moddb, asc is oldest, desc is most recent
+        * **ranktoday** - order by daily ranking, asc is highest ranked, desc is lowest rank
+        * **visitstotal** - order by most views, asc is highest views, desc is lowest views
+        * **rating** - order by rating, asc is highest rating, desc is lowest rating
+        * **name** - order alphabetically, asc is a-z, desc is z-a
+        * **date** - order by upload date, asc is most recent first, desc is oldest first
+
+    Attributes
+    -----------
+    filename : str
+        The name of the file
+    hash : str
+        The MD5 hash of the file
+    name : str
+        The name of the page
+    size : int
+        the file size in bytes
+    today : int
+        The number of downloads today
+    downloads : int
+        The total number of times this file has been downloaded
+    category : FileCategory
+        The category of the file
+    author : Thumbnail
+        A member type thumbnail of the member who uploaded the file
+    date : datetime.datetime
+        The date the file was uploaded
+    button : str
+        html code for the embed button
+    widget : str
+        html code for the embed widget
+    description : str
+        Description of the file, as written by the author
+    preview : str
+        URL of the preview image for the file
+    """
+
+    def __init__(self, html: bs4.BeautifulSoup):
+        if html.find("span", string="File Deleted", class_="heading"):
+            raise ValueError("This file has been removed")
+
+        info = html.find("div", class_="table tablemenu")
+        file = {
+            x.string.lower(): x.parent.span.string.strip()
+            for x in info.find_all("h5", string=("Filename", "Size", "MD5 Hash"))
+        }
+        self.name = (
+            html.find("a", title="Report").parent.parent.find("span", class_="heading").string
+        )
+        self.filename = file["filename"]
+        super().__init__(html)
+
+        self.hash = file["md5 hash"]
+        self.size = int(re.sub(r"[(),bytes]", "", file["size"].split(" ")[1]))
+
+        downloads = html.find("h5", string="Downloads").parent.a.string
+        self.today = int(re.sub(r"[(),today]", "", downloads.split(" ")[1]))
+        self.downloads = int(downloads.split(" ")[0].replace(",", ""))
+
+        try:
+            self.category = FileCategory(
+                int(info.find("h5", string="Category").parent.a["href"].split("=")[-1])
+            )
+        except ValueError:
+            self.category = AddonCategory(
+                int(info.find("h5", string="Category").parent.a["href"].split("=")[-1])
+            )
+
+        uploader = info.find("h5", string="Uploader").parent.a
+        self.author = Thumbnail(
+            url=uploader["href"], name=uploader.string, type=ThumbnailType.member
+        )
+
+        self.date = get_date(info.find("h5", string="Added").parent.span.time["datetime"])
+        self.button = info.find("h5", string="Embed Button").parent.span.input["value"]
+        self.widget = info.find("h5", string="Embed Widget").parent.span.input["value"]
+
+        self.description = html.find("p", id="downloadsummary").string
+
+        self.preview = html.find_all("img", src=True)[0]["src"]
+
+    def __repr__(self):
+        return f"<{self.__class__.__name__} name={self.name} type={self.category.name}>"
+
+    def save(self, file_obj, *, mirror=None):
+        """Save the file to an object. This functions makes
+        two requests. If you pass a valid mirror it will
+        make only one request.
+
+        Parameters
+        -----------
+        file_obj : typing.BinaryIO
+            The file obj to save the file to. The binary data
+            will be streamed to that object.
+        mirror : Optional[Mirror]
+            An optional mirror object to download the
+            file from a specific moddb mirror
+
+        """
+        if mirror is None:
+            download = get_page(f"{BASE_URL}/downloads/start/{self.id}")
+            url = download.find("a", string=f"download {self.filename}")["href"]
+        else:
+            url = mirror._url
+
+        SESSION = sys.modules["moddb"].SESSION
+        prepped = prepare_request(requests.Request("GET", join(url)), SESSION)
+        with SESSION.send(prepped, stream=True) as r:
+            raise_for_status(r)
+            for chunk in r.iter_content(chunk_size=8192):
+                file_obj.write(chunk)
+
+    def get_mirrors(self):
+        """Get all the mirrors from which a file can be downloaded. This
+        can then be passed to File.save to download from a specific mirror.
+
+
+        Returns
+        --------
+        List[Mirror]
+            A list of Mirror objects"""
+
+        html = get_page(f"https://www.moddb.com/downloads/start/{self.id}/all")
+        mirrors_div = html.find("div", class_="mirrors").find_all("div", recursive=False)
+        mirrors = []
+        for mirror in mirrors_div:
+            mirror_match = re.match(
+                r"(.*) #([0-9]*) \((\w+), (\w+)\)", mirror.div.p.contents[-1].strip()
+            )
+            stats_match = re.match(
+                r"([0-9,]*) downloads? served, ([0-9.]*)% capacity",
+                mirror.div.span.string,
+            )
+
+            mirrors.append(
+                Mirror(
+                    name=mirror_match.group(1),
+                    index=int(mirror_match.group(2)),
+                    city=mirror_match.group(3),
+                    country=mirror_match.group(4),
+                    served=int(stats_match.group(1).replace(",", "")),
+                    capacity=float(stats_match.group(2)),
+                    url=mirror.div.p.a["href"],
+                )
+            )
+
+        return mirrors
+
+
+@concat_docs
+class Addon(File):
+    """Object representing an addon. Seemingly the only difference between an addon and a file is in
+    the semantics. A file often represents something official released by the page, e.g. the mod installation
+    or an official guide where as addons are often fan made and might not be directly endorsed by the page owners
+    even if it is allowed. They literally add on to the page's content without becoming part of it. There is a slight
+    difference in their profiles but nothing beyond that.
+
+    Parameters
+    -----------
+    html : bs4.BeautifulSoup
+        The html to parse. Allows for finer control.
+
+    Filtering
+    ----------
+    categoryaddon : :class:`.AddonCategory`
+        The type of addon (map, textures, ect...)
+    licence : :class:`.Licence`
+        The licence of the addon
+    game : Union[:class:`.Game`, :class:`.Object`]
+        An game object or an object with an id attribute which represents the
+        game the addon belongs to.
+    timeframe : :class:`.TimeFrame`
+        The time period this was released in (last 24hr, last week, last month)
+
+    Sorting
+    --------
+        * **released** - when the object was released, asc is oldest, desc is most recent
+        * **id** - when it was added to moddb, asc is oldest, desc is most recent
+        * **ranktoday** - order by daily ranking, asc is highest ranked, desc is lowest rank
+        * **visitstotal** - order by most views, asc is highest views, desc is lowest views
+        * **rating** - order by rating, asc is highest rating, desc is lowest rating
+        * **name** - order alphabetically, asc is a-z, desc is z-a
+        * **licence** - order based on licence
+        * **date** - order by upload date, asc is most recent first, desc is oldest first
+
+
+    """
+
+    pass
+
+
+@concat_docs
+class Media(BaseMetaClass):
+    """Represents an image, audio file or video file on
+
+    Parameters
+    -----------
+    html : bs4.BeautifulSoup
+        The html to parse. Allows for finer control.
+
+    Filtering
+    -----------
+    sitearea : :class:`.Category`
+        The type of model the media belongs to. Category.downloads is not valid for this.
+
+    Sorting
+    --------
+        * **ranktoday** - order by daily ranking, asc is highest ranked, desc is lowest rank
+        * **visitstotal** - order by most views, asc is highest views, desc is lowest views
+        * **name** - order alphabetically, asc is a-z, desc is z-a
+        * **id** - order by upload date, asc is most recent first, desc is oldest first
+
+        Exclusive to videos and audios
+        * **duration** - order by duration, asc is shortest to longest, desc is longest first
+
+    Attributes
+    -----------
+    date : datetime.datetime
+        The date the media was uploaded
+    name : str
+        The name of the media
+    author : Thumbnail
+        Member type thumbnail of the media uploader
+    duration : datetime.timedelta
+        Duration of the media in seconds, 0 if it's an image
+    size : int
+        Size of the files in bytes
+    views : int
+        Total amount of views
+    today : int
+        Amount of views today
+    filename : str
+        The name of the file for the media
+    fileurl : str
+        The url of the file for the media
+    category : MediaCategory
+        Whether the media is an image, a video or an audio
+    description : str
+        The description of the file as given by the file uploader.
+    """
+
+    def __init__(self, html: bs4.BeautifulSoup):
+        try:
+            self.name = html.find("meta", itemprop="name")["content"]
+        except TypeError:
+            self.name = html.find("img", id="mediaimage")["title"]
+
+        super().__init__(html)
+        medias = html.find_all("h5", string=("Date", "By", "Duration", "Size", "Views", "Filename"))
+        raw_media = {media.string.lower(): media.parent for media in medias}
+
+        self.date = get_date(raw_media["date"].span.time["datetime"])
+
+        author = raw_media["by"].span.a
+        self.author = Thumbnail(
+            url=author["href"], name=author.string.strip(), type=ThumbnailType.member
+        )
+
+        if "duration" in raw_media:
+            duration = raw_media["duration"].span.time.string.strip().split(":")
+            duration.reverse()
+            times = ["seconds", "minutes", "hours"]
+            self.duration = datetime.timedelta(
+                **{times[duration.index(x)]: int(x) for x in duration}
+            )
+        else:
+            self.duration = 0
+
+        if "size" in raw_media:
+            self.size = tuple(raw_media["size"].span.string.strip().split("×"))
+
+        self.views, self.today = get_views(raw_media["views"].a.string)
+        media_player = html.find("video", id="mediaplayer")
+
+        if not media_player:
+            self.category = MediaCategory.image
+            self.fileurl = html.find("meta", property="og:image")["content"]
+        else:
+            self.fileurl = media_player.source["src"]
+            if "audio" in media_player.source["type"]:
+                self.category = MediaCategory.audio
+            else:
+                self.category = MediaCategory.video
+
+        if "filename" in raw_media:
+            self.filename = raw_media["filename"].span.string.strip()
+        else:
+            self.filename = self.fileurl.split("/")[-1]
+
+        self.description = html.find("meta", {"name": "description"})["content"]
+
+    def __repr__(self):
+        return f"<Media name={self.name} type={self.category.name}>"
+
+    def save(self, file_obj):
+        """Save the media to an object.
+
+        Parameters
+        -----------
+        file_obj : typing.BinaryIO
+            The file obj to save the file to. The binary data
+            will be streamed to that object.
+
+        """
+        SESSION = sys.modules["moddb"].SESSION
+        prepped = prepare_request(requests.Request("GET", self.fileurl), SESSION)
+
+        with SESSION.send(prepped, stream=True) as r:
+            raise_for_status(r)
+            for chunk in r.iter_content(chunk_size=8192):
+                file_obj.write(chunk)
```

### Comparing `moddb-0.8.1/moddb/pages/fp.py` & `moddb-0.9.0/moddb/pages/fp.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,148 +1,149 @@
-import bs4
-import re
-
-from ..boxes import Thumbnail
-from ..enums import ThumbnailType
-from ..utils import get_page_type, get_page
-from . import opinion
-
-
-class FrontPage:
-    """An object representing the front page of  More of less just a long suggestion of the hottest mods,
-    games, articles and files of the moment
-
-    Parameters
-    -----------
-    html : bs4.BeautifulSoup
-        The html to parse. Allows for finer control.
-
-    Attributes
-    -----------
-    slider : List[Thumnail]
-        A list of object like thumbnails presented by the slider present on
-        the front page, this is a catered list of promoted content, can contain
-        any type of object.
-    articles : List[Thumbnail]
-        A list of article like thumbnail objects representing the suggested
-        articles on the front page.
-    mods : List[Thumbnail]
-        A list of mod like thumbnail objects representing the suggested
-        mods on the front page.
-    games : List[Thumbnail]
-        A list of game like thumbnail objects representing the suggested
-        games on the front page.
-    files : List[Thumbnail]
-        A list of file like thumbnail objects representing the suggested
-        files on the front page.
-    poll : Poll
-        The current ongoing moddb poll. Currently cannot be voted on.
-
-    """
-
-    def __init__(self, html: bs4.BeautifulSoup):
-        slider = html.find("div", class_="rotatorholder").find_all("div", class_="rotatorbox")
-        self.slider = []
-        for x in slider:
-            name = x.a.find("h2")
-            summary = x.a.find("p")
-
-            image = None
-            if "style" in x.div:
-                re_search = re.search(r"\((.*)\)", x.div["style"])
-                if re_search:
-                    image = re_search.group(1)
-            elif "data-bg" in x.div:
-                image = x.div["data-bg"]
-
-            thumbnail = Thumbnail(
-                name=name.string if name else None,
-                url=x.a["href"],
-                summary=summary.string if summary else None,
-                image=image,
-                type=get_page_type(x.a["href"]),
-            )
-
-            self.slider.append(thumbnail)
-
-        articles = (
-            html.find("span", string="Latest Articles")
-            .parent.parent.parent.find("div", class_="table")
-            .find_all("div", recursive=False)[:-1]
-        )
-        self.articles = [
-            Thumbnail(
-                name=x.a["title"],
-                url=x.a["href"],
-                type=ThumbnailType.article,
-                image=x.a.img["src"],
-                summary=x.find("p").string,
-                date=x.find("time")["datetime"],
-            )
-            for x in articles
-        ]
-
-        mods = (
-            html.find("span", string="Popular Mods")
-            .parent.parent.parent.find("div", class_="table")
-            .find_all("div", recursive=False)[1:]
-        )
-        self.mods = [
-            Thumbnail(
-                name=x.a["title"],
-                url=x.a["href"],
-                type=ThumbnailType.mod,
-                image=x.a.img["src"],
-            )
-            for x in mods
-        ]
-
-        games = (
-            html.find("span", string="Popular Games")
-            .parent.parent.parent.find("div", class_="table")
-            .find_all("div", recursive=False)[1:]
-        )
-        self.games = [
-            Thumbnail(
-                name=x.a["title"],
-                url=x.a["href"],
-                type=ThumbnailType.game,
-                image=x.a.img["src"],
-            )
-            for x in games
-        ]
-
-        jobs = (
-            html.find("span", string="Jobs")
-            .parent.parent.parent.find("div", class_="table")
-            .find_all("div", recursive=False)[1:]
-        )
-        self.jobs = [
-            Thumbnail(
-                name=x.find("a").string,
-                url=x.find("a")["href"],
-                type=ThumbnailType.job,
-            )
-            for x in jobs
-        ]
-
-        files = (
-            html.find("span", string="Popular Files")
-            .parent.parent.parent.find("div", class_="table")
-            .find_all("div", recursive=False)[1:]
-        )
-        self.files = [
-            Thumbnail(
-                name=x.a["title"],
-                url=x.a["href"],
-                type=ThumbnailType.file,
-                image=x.a.img["src"],
-            )
-            for x in files
-        ]
-
-        self.poll = opinion.Poll(get_page(html.find("div", class_="poll").form["action"]))
-
-        self._html = html
-
-    def __repr__(self):
-        return f"<FrontPage articles={len(self.articles)} mods={len(self.mods)} games={len(self.games)} files={len(self.files)}>"
+import re
+
+import bs4
+
+from ..boxes import Thumbnail
+from ..enums import ThumbnailType
+from ..utils import get_page, get_page_type
+from . import opinion
+
+
+class FrontPage:
+    """An object representing the front page of  More of less just a long suggestion of the hottest mods,
+    games, articles and files of the moment
+
+    Parameters
+    -----------
+    html : bs4.BeautifulSoup
+        The html to parse. Allows for finer control.
+
+    Attributes
+    -----------
+    slider : List[Thumnail]
+        A list of object like thumbnails presented by the slider present on
+        the front page, this is a catered list of promoted content, can contain
+        any type of object.
+    articles : List[Thumbnail]
+        A list of article like thumbnail objects representing the suggested
+        articles on the front page.
+    mods : List[Thumbnail]
+        A list of mod like thumbnail objects representing the suggested
+        mods on the front page.
+    games : List[Thumbnail]
+        A list of game like thumbnail objects representing the suggested
+        games on the front page.
+    files : List[Thumbnail]
+        A list of file like thumbnail objects representing the suggested
+        files on the front page.
+    poll : Poll
+        The current ongoing moddb poll. Currently cannot be voted on.
+
+    """
+
+    def __init__(self, html: bs4.BeautifulSoup):
+        slider = html.find("div", class_="rotatorholder").find_all("div", class_="rotatorbox")
+        self.slider = []
+        for x in slider:
+            name = x.a.find("h2")
+            summary = x.a.find("p")
+
+            image = None
+            if "style" in x.div:
+                re_search = re.search(r"\((.*)\)", x.div["style"])
+                if re_search:
+                    image = re_search.group(1)
+            elif "data-bg" in x.div:
+                image = x.div["data-bg"]
+
+            thumbnail = Thumbnail(
+                name=name.string if name else None,
+                url=x.a["href"],
+                summary=summary.string if summary else None,
+                image=image,
+                type=get_page_type(x.a["href"]),
+            )
+
+            self.slider.append(thumbnail)
+
+        articles = (
+            html.find("span", string="Latest Articles")
+            .parent.parent.parent.find("div", class_="table")
+            .find_all("div", recursive=False)[:-1]
+        )
+        self.articles = [
+            Thumbnail(
+                name=x.a["title"],
+                url=x.a["href"],
+                type=ThumbnailType.article,
+                image=x.a.img["src"],
+                summary=x.find("p").string,
+                date=x.find("time")["datetime"],
+            )
+            for x in articles
+        ]
+
+        mods = (
+            html.find("span", string="Popular Mods")
+            .parent.parent.parent.find("div", class_="table")
+            .find_all("div", recursive=False)[1:]
+        )
+        self.mods = [
+            Thumbnail(
+                name=x.a["title"],
+                url=x.a["href"],
+                type=ThumbnailType.mod,
+                image=x.a.img["src"],
+            )
+            for x in mods
+        ]
+
+        games = (
+            html.find("span", string="Popular Games")
+            .parent.parent.parent.find("div", class_="table")
+            .find_all("div", recursive=False)[1:]
+        )
+        self.games = [
+            Thumbnail(
+                name=x.a["title"],
+                url=x.a["href"],
+                type=ThumbnailType.game,
+                image=x.a.img["src"],
+            )
+            for x in games
+        ]
+
+        jobs = (
+            html.find("span", string="Jobs")
+            .parent.parent.parent.find("div", class_="table")
+            .find_all("div", recursive=False)[1:]
+        )
+        self.jobs = [
+            Thumbnail(
+                name=x.find("a").string,
+                url=x.find("a")["href"],
+                type=ThumbnailType.job,
+            )
+            for x in jobs
+        ]
+
+        files = (
+            html.find("span", string="Popular Files")
+            .parent.parent.parent.find("div", class_="table")
+            .find_all("div", recursive=False)[1:]
+        )
+        self.files = [
+            Thumbnail(
+                name=x.a["title"],
+                url=x.a["href"],
+                type=ThumbnailType.file,
+                image=x.a.img["src"],
+            )
+            for x in files
+        ]
+
+        self.poll = opinion.Poll(get_page(html.find("div", class_="poll").form["action"]))
+
+        self._html = html
+
+    def __repr__(self):
+        return f"<FrontPage articles={len(self.articles)} mods={len(self.mods)} games={len(self.games)} files={len(self.files)}>"
```

### Comparing `moddb-0.8.1/moddb/pages/game.py` & `moddb-0.9.0/moddb/pages/game.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-import bs4
-
-from ..utils import concat_docs
-from .base import PageMetaClass
-from .mixins import GetModsMixin, GetAddonsMixin
-from ..enums import SearchCategory
-
-
-@concat_docs
-class Game(PageMetaClass, GetModsMixin, GetAddonsMixin):
-    """A subclass of Page plus a method to get all the mods.
-
-    Parameters
-    -----------
-    html : bs4.BeautifulSoup
-        The html to parse. Allows for finer control.
-
-
-    Filtering
-    ----------
-    released : :class:`.Status`
-        The status of the game (released, unreleased)
-    genre : :class:`.Genre`
-        The genre of the game (fps, tower defense)
-    theme : :class:`.Theme`
-        The theme of the game (fantasy, action)
-    indie : :class:`.Scope`
-        Whether the game is triple AAA or indie
-    players : :class:`.PlayerStyle`
-        Player styles of the game (co-op, singleplayer)
-    timeframe : :class:`.TimeFrame`
-        The time period this was released in (last 24hr, last week, last month)
-
-    Sorting
-    --------
-        * **released** - when the object was released, asc is oldest, desc is most recent
-        * **id** - when it was added to moddb, asc is oldest, desc is most recent
-        * **ranktoday** - order by daily ranking, asc is highest ranked, desc is lowest rank
-        * **visitstotal** - order by most views, asc is highest views, desc is lowest views
-        * **rating** - order by rating, asc is highest rating, desc is lowest rating
-        * **name** - order alphabetically, asc is a-z, desc is z-a
-        * **dateup** - order by latest update, asc is most recent update first, desc is oldest update first
-    """
-
-    def __init__(self, html: bs4.BeautifulSoup):
-        super().__init__(html, SearchCategory.games)
+import bs4
+
+from ..enums import SearchCategory
+from ..utils import concat_docs
+from .base import PageMetaClass
+from .mixins import GetAddonsMixin, GetModsMixin
+
+
+@concat_docs
+class Game(PageMetaClass, GetModsMixin, GetAddonsMixin):
+    """A subclass of Page plus a method to get all the mods.
+
+    Parameters
+    -----------
+    html : bs4.BeautifulSoup
+        The html to parse. Allows for finer control.
+
+
+    Filtering
+    ----------
+    released : :class:`.Status`
+        The status of the game (released, unreleased)
+    genre : :class:`.Genre`
+        The genre of the game (fps, tower defense)
+    theme : :class:`.Theme`
+        The theme of the game (fantasy, action)
+    indie : :class:`.Scope`
+        Whether the game is triple AAA or indie
+    players : :class:`.PlayerStyle`
+        Player styles of the game (co-op, singleplayer)
+    timeframe : :class:`.TimeFrame`
+        The time period this was released in (last 24hr, last week, last month)
+
+    Sorting
+    --------
+        * **released** - when the object was released, asc is oldest, desc is most recent
+        * **id** - when it was added to moddb, asc is oldest, desc is most recent
+        * **ranktoday** - order by daily ranking, asc is highest ranked, desc is lowest rank
+        * **visitstotal** - order by most views, asc is highest views, desc is lowest views
+        * **rating** - order by rating, asc is highest rating, desc is lowest rating
+        * **name** - order alphabetically, asc is a-z, desc is z-a
+        * **dateup** - order by latest update, asc is most recent update first, desc is oldest update first
+    """
+
+    def __init__(self, html: bs4.BeautifulSoup):
+        super().__init__(html, SearchCategory.games)
```

### Comparing `moddb-0.8.1/moddb/pages/job.py` & `moddb-0.9.0/moddb/pages/job.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,105 +1,112 @@
-import bs4
-import json
-import re
-
-from ..utils import join, LOGGER
-from ..boxes import Thumbnail
-from ..enums import ThumbnailType, JobSkill
-
-
-class Job:
-    """Model representing a job proposed on ModDB
-
-    Parameters
-    -----------
-    html : bs4.BeautifulSoup
-        The html to parse. Allows for finer control.
-
-    Filtering
-    ----------
-    skill : :class:`.JobSkill`
-        The job skill looked for
-    earn : :class:`.bool`
-        Whether or not the job is paid
-
-    Sorting
-    --------
-        * **location** - order by the location of the job
-        * **name** - order alphabetically, asc is a-z, desc is z-a
-        * **skill** - order by the skill required
-        * **id** - order by upload date, asc is most recent, desc is oldest first
-
-    Attributes
-    -----------
-    id : int
-        id of the job
-    name_id : str
-        The name_id of the member, cannot be changed, it's a mix of the original username lowercased with
-        spaces removed and shortened.
-    author : Thumbnail
-        A member like thumbnail representing the poster of the job. Can be none if they desire to remain private.
-    paid : bool
-        Whether or not the job is paid
-    tags : dict{str : str}
-        A dict of key-values pair where the key is the name of the tag and the value is the url.
-    skill : JobSkill
-        the skill demanded for the job
-    location : str
-        The location the job will be at
-    name : str
-        The name of the job
-    text : str
-        The description of the job
-    related : List[Thumbnail]
-        A list of team like thumbnails of companies related to the job poster
-
-    """
-
-    def __init__(self, html: bs4.BeautifulSoup):
-        breadcrumb = json.loads(html.find("script", type="application/ld+json").string)["itemListElement"][
-            -1
-        ]["Item"]
-        self.name = breadcrumb["name"]
-        self.url = breadcrumb["@id"]
-        self.name_id = self.url.split("/")[0]
-        self.text = html.find("div", id="articlecontent").text
-
-        profile_raw = html.find("span", string="Jobs").parent.parent.parent.find(
-            "div", class_="table tablemenu"
-        )
-
-        self.id = int(re.search(r"siteareaid=(\d*)", html.find("a", string="Report")["href"])[1])
-
-        try:
-            author = profile_raw.find("h5", string="Author").parent.span.a
-            self.author = Thumbnail(url=author["href"], name=author.string, type=ThumbnailType.member)
-        except AttributeError:
-            LOGGER.info("Job '%s' has no author", self.name)
-            self.author = None
-
-        self.paid = profile_raw.find("h5", string="Paid").parent.a.string == "Yes"
-
-        try:
-            raw_tags = html.find("form", attrs={"name": "tagsform"}).find_all("a")
-            self.tags = {x.string: join(x["href"]) for x in raw_tags if x.string is not None}
-        except AttributeError:
-            self.tags = {}
-            LOGGER.info("'%s' '%s' has no tags", self.__class__.__name__, self.name)
-
-        self.skill = JobSkill(int(profile_raw.find("h5", string="Skill").parent.span.a["href"][-1]))
-
-        self.location = profile_raw.find("h5", string="Location").parent.span.string.strip()
-
-        try:
-            related = html.find("div", class_="tablerelated").find_all("a", class_="image")
-            self.related = [
-                Thumbnail(url=x["href"], name=x["title"], type=ThumbnailType.team) for x in related
-            ]
-        except AttributeError:
-            LOGGER.info("Job '%s' has no related companies", self.name)
-            self.related = []
-
-        self._html = html
-
-    def __repr__(self):
-        return f"<Job name={self.name}>"
+import json
+import re
+
+import bs4
+
+from ..boxes import PartialTag, Thumbnail
+from ..enums import JobSkill, ThumbnailType
+from ..utils import LOGGER, join
+
+
+class Job:
+    """Model representing a job proposed on ModDB
+
+    Parameters
+    -----------
+    html : bs4.BeautifulSoup
+        The html to parse. Allows for finer control.
+
+    Filtering
+    ----------
+    skill : :class:`.JobSkill`
+        The job skill looked for
+    earn : :class:`.bool`
+        Whether or not the job is paid
+
+    Sorting
+    --------
+        * **location** - order by the location of the job
+        * **name** - order alphabetically, asc is a-z, desc is z-a
+        * **skill** - order by the skill required
+        * **id** - order by upload date, asc is most recent, desc is oldest first
+
+    Attributes
+    -----------
+    id : int
+        id of the job
+    name_id : str
+        The name_id of the member, cannot be changed, it's a mix of the original username lowercased with
+        spaces removed and shortened.
+    author : Thumbnail
+        A member like thumbnail representing the poster of the job. Can be none if they desire to remain private.
+    paid : bool
+        Whether or not the job is paid
+    tags : List[PartialTag]
+        A list of partial tags. You can use `get_tags` and then use the name id to get the right one.
+    skill : JobSkill
+        the skill demanded for the job
+    location : str
+        The location the job will be at
+    name : str
+        The name of the job
+    text : str
+        The description of the job
+    related : List[Thumbnail]
+        A list of team like thumbnails of companies related to the job poster
+
+    """
+
+    def __init__(self, html: bs4.BeautifulSoup):
+        breadcrumb = json.loads(html.find("script", type="application/ld+json").string)[
+            "itemListElement"
+        ][-1]["Item"]
+        self.name = breadcrumb["name"]
+        self.url = breadcrumb["@id"]
+        self.name_id = self.url.split("/")[0]
+        self.text = html.find("div", id="articlecontent").text
+
+        profile_raw = html.find("span", string="Jobs").parent.parent.parent.find(
+            "div", class_="table tablemenu"
+        )
+
+        self.id = int(re.search(r"siteareaid=(\d*)", html.find("a", string="Report")["href"])[1])
+
+        try:
+            author = profile_raw.find("h5", string="Author").parent.span.a
+            self.author = Thumbnail(
+                url=author["href"], name=author.string, type=ThumbnailType.member
+            )
+        except AttributeError:
+            LOGGER.info("Job '%s' has no author", self.name)
+            self.author = None
+
+        self.paid = profile_raw.find("h5", string="Paid").parent.a.string == "Yes"
+
+        try:
+            raw_tags = html.find("form", attrs={"name": "tagsform"}).find_all("a")
+            self.tags = [
+                PartialTag(x.string, join(x["href"]), x["href"].split("/")[-1])
+                for x in raw_tags
+                if x.string is not None
+            ]
+        except AttributeError:
+            self.tags = []
+            LOGGER.info("'%s' '%s' has no tags", self.__class__.__name__, self.name)
+
+        self.skill = JobSkill(int(profile_raw.find("h5", string="Skill").parent.span.a["href"][-1]))
+
+        self.location = profile_raw.find("h5", string="Location").parent.span.string.strip()
+
+        try:
+            related = html.find("div", class_="tablerelated").find_all("a", class_="image")
+            self.related = [
+                Thumbnail(url=x["href"], name=x["title"], type=ThumbnailType.team) for x in related
+            ]
+        except AttributeError:
+            LOGGER.info("Job '%s' has no related companies", self.name)
+            self.related = []
+
+        self._html = html
+
+    def __repr__(self):
+        return f"<Job name={self.name}>"
```

### Comparing `moddb-0.8.1/moddb/pages/mixins.py` & `moddb-0.9.0/moddb/pages/mixins.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,566 +1,592 @@
-from typing import Tuple, Union, List
-
-from . import opinion
-
-from ..utils import get_page, Object
-from ..boxes import ResultList, Thumbnail
-from ..enums import (
-    Status,
-    Genre,
-    Theme,
-    Scope,
-    PlayerStyle,
-    TimeFrame,
-    Licence,
-    ArticleCategory,
-    FileCategory,
-    AddonCategory,
-    Difficulty,
-    TutorialCategory,
-    HardwareCategory,
-    SoftwareCategory,
-    RSSType,
-)
-
-
-class GetGamesMixin:
-    """Abstract class containing the get_games method"""
-
-    def get_games(
-        self,
-        index: int = 1,
-        *,
-        query: str = None,
-        status: Status = None,
-        genre: Genre = None,
-        theme: Theme = None,
-        scope: Scope = None,
-        players: PlayerStyle = None,
-        timeframe: TimeFrame = None,
-        sort: Tuple[str, str] = None,
-    ) -> ResultList:
-        """Get a page of games for the model. Each page will yield up to 30 games.
-
-        Parameters
-        -----------
-        index : Optional[int]
-            The page number to get the games for.
-        query : Optional[str]
-            The text to look for in the game names.
-        status : Optional[Status]
-            The status of the game (unreleased, released, early access, ect...)
-        genre : Optional[Genre]
-            The genre of the game (fps, tower defense)
-        theme : Optional[Theme]
-            The theme of the game (fantasy, action)
-        scope : Optional[Scope]
-            The scope of the game (AAA, indie)
-        players : Optional[PlayerStyle]
-            Player styles of the game (co-op, singleplayer)
-        timeframe : Optional[TimeFrame]
-            The time period this was released in (last 24hr, last week, last month)
-        sort : Optional[Tuple[str, str]]
-            The sorting tuple to sort by the results
-
-        Returns
-        --------
-        ResultList[Thumbnail]
-            List of game like thumbnails that can be parsed individually.
-        """
-        params = {
-            "filter": "t",
-            "kw": query,
-            "released": status.value if status else None,
-            "genre": genre.value if genre else None,
-            "theme": theme.value if theme else None,
-            "indie": scope.value if scope else None,
-            "players": players.value if players else None,
-            "timeframe": timeframe.value if timeframe else None,
-            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
-        }
-
-        return self._get(f"{self.url}/games/page/{index}", params=params)
-
-
-class GetModsMixin:
-    """Abstract class containing the get_mod method"""
-
-    def get_mods(
-        self,
-        index: int = 1,
-        *,
-        query: str = None,
-        status: Status = None,
-        genre: Genre = None,
-        theme: Theme = None,
-        players: PlayerStyle = None,
-        timeframe: TimeFrame = None,
-        game: Union["Game", Object] = None,
-        sort: Tuple[str, str] = None,
-    ) -> ResultList:
-        """Get a page of mods for the game. Each page will yield up to 30 mods.
-
-        Parameters
-        -----------
-        index : int
-            The page number to get the mods from.
-        query : Optional[str]
-            The text to look for in the mod names.
-        status : Optional[Status]
-            The status of the mod (unreleased, released, early access, ect...)
-        genre : Optional[Genre]
-            The genre of the mod (fps, tower defense)
-        theme : Optional[Theme]
-            The theme of the mod (fantasy, action)
-        players : Optional[PlayerStyle]
-            Player styles of the mod (co-op, singleplayer)
-        timeframe : Optional[TimeFrame]
-            The time period this was released in (last 24hr, last week, last month)
-        game : Union[mod, Object]
-            An mod object or an object with an id attribute which represents the
-            mod the mod belongs to.
-        sort : Optional[Tuple[str, str]]
-            The sorting tuple to sort by the results
-
-        Returns
-        --------
-        ResultList[Thumbnail]
-            The list of mods type thumbnails parsed from the game
-        """
-        params = {
-            "filter": "t",
-            "kw": query,
-            "released": status.value if status else None,
-            "genre": genre.value if genre else None,
-            "theme": theme.value if theme else None,
-            "players": players.value if players else None,
-            "timeframe": timeframe.value if timeframe else None,
-            "game": game.id if game else None,
-            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
-        }
-
-        return self._get(f"{self.url}/mods/page/{index}", params=params)
-
-
-class GetEnginesMixin:
-    """Abstract class containing the get_engines method"""
-
-    def get_engines(
-        self,
-        index: int = 1,
-        *,
-        query: str = None,
-        status: Status = None,
-        licence: Licence = None,
-        timeframe: TimeFrame = None,
-        sort: Tuple[str, str] = None,
-    ) -> ResultList:
-        """Get a page of engines for the game. Each page will yield up to 30 engines.
-
-        Parameters
-        -----------
-        index : int
-            The page number to get the engines from.
-        query : Optional[str]
-            The text to look for in the engine names.
-        status : Optional[Status]
-            The status of the game (unreleased, released, early access, ect...)
-        licence : Optional[Licence]
-            The licence of the engine (open source, proprietary, ect...)
-        timeframe : Optional[TimeFrame]
-            The time period this was released in (last 24hr, last week, last month)
-        sort : Optional[Tuple[str, str]]
-            The sorting tuple to sort by the results
-        Returns
-        --------
-        ResultList[Thumbnail]
-            The list of engine type thumbnails parsed from the game
-        """
-        params = {
-            "filter": "t",
-            "kw": query,
-            "released": status.value if status else None,
-            "licence": licence.value if licence else None,
-            "timeframe": timeframe.value if timeframe else None,
-            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
-        }
-
-        return self._get(f"{self.url}/engines/page/{index}", params=params)
-
-
-class SharedMethodsMixin:
-    """Abstract class that implements a certain amount of top level methods shared between Pages
-    and Hardware"""
-
-    def get_reviews(
-        self,
-        index: int = 1,
-        *,
-        query: str = None,
-        rating: int = None,
-        sort: Tuple[str, str] = None,
-    ) -> ResultList:
-        """Get a page of reviews for the page. Each page will yield up to 10 reviews.
-
-        Parameters
-        -----------
-        index : Optional[int]
-            The page number to get the reviews from.
-        query : Optional[str]
-            The string to look for in the review, optional.
-        rating : Optiona[int]
-            A number between 1 and 10 to get the ratings
-        sort : Optional[Tuple[str, str]]
-            The sorting tuple to sort by the results
-
-        Returns
-        --------
-        ResultList[Review]
-            The list of reviews parsed from the page
-        """
-        params = {
-            "filter": "t",
-            "kw": query,
-            "rating": rating,
-            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
-        }
-
-        base_url = f"{self.url}/reviews"
-        url = f"{base_url}/page/{index}"
-        html = get_page(url, params=params)
-        results, current_page, total_pages, total_results = opinion.parse_reviews(html)
-
-        return opinion.ReviewList(
-            results=results,
-            url=base_url,
-            total_results=total_results,
-            params=params,
-            current_page=current_page,
-            total_pages=total_pages,
-        )
-
-    def get_articles(
-        self,
-        index: int = 1,
-        *,
-        query: str = None,
-        category: ArticleCategory = None,
-        timeframe: TimeFrame = None,
-        sort: Tuple[str, str] = None,
-    ) -> ResultList:
-        """Get a page of articles for the page. Each page will yield up to 30 articles.
-
-        Parameters
-        -----------
-        index : Optional[int]
-            The page number to get the articles from.
-        query : Optional[str]
-            The string query to search for in the article name, optional.
-        category : Optional[ArticleCategory]
-            Type enum defining what the article is, optional
-        timeframe : Optional[TimeFrame]
-            The time period this was released in (last 24hr, last week, last month)
-        sort : Optional[Tuple[str, str]]
-            The sorting tuple to sort by the results
-
-        Returns
-        --------
-        ResultList[Thumbnail]
-            The list of article type thumbnails parsed from the page
-        """
-        params = {
-            "filter": "t",
-            "kw": query,
-            "type": category.value if category else None,
-            "timeframe": timeframe.value if timeframe else None,
-            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
-        }
-
-        return self._get(f"{self.url}/articles/page/{index}", params=params)
-
-    def get_files(
-        self,
-        index: int = 1,
-        *,
-        query: str = None,
-        category: FileCategory = None,
-        addon_type: AddonCategory = None,
-        timeframe: TimeFrame = None,
-        sort: Tuple[str, str] = None,
-    ) -> ResultList:
-        """Get a page of files for the page. Each page will yield up to 30 files.
-
-        Parameters
-        -----------
-        index : Optional[int]
-            The page number to get the files from.
-        query : Optional[str]
-            The string query to search for in the file name, optional.
-        category : [FileCategory]
-            Type enum defining what the file is, optional
-        addon_type : Optional[AddonCategory]
-            Type enum defining what category the file is.
-        timeframe : Optional[TimeFrame]
-            The time period this was released in (last 24hr, last week, last month)
-        sort : Optional[Tuple[str, str]]
-            The sorting tuple to sort by the results
-
-        Returns
-        --------
-        ResultList[Thumbnail]
-            The list of file type thumbnails parsed from the page
-        """
-        params = {
-            "filter": "t",
-            "kw": query,
-            "category": category.value if category else None,
-            "categoryaddon": addon_type.value if addon_type else None,
-            "timeframe": timeframe.value if timeframe else None,
-            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
-        }
-
-        return self._get(f"{self.url}/downloads/page/{index}", params=params)
-
-    def get_images(self) -> List[Thumbnail]:
-        """Get all the images a page has uploaded. Literally all of them. As thumbnails. ModDB's imagebox
-        caches all the urls for images on the page so this grabs them all. Lists might be long, but this
-        is all the images. They can be invidually parsed to get full fledged media objects from them.
-
-        Returns
-        --------
-        List[Thumbnail]
-            The list of image type thumbnails parsed from the page
-        """
-        html = get_page(f"{self.url}/images")
-        return self._get_media(1, html=html)
-
-    def get_videos(self) -> List[Thumbnail]:
-        """Get all the videos a page has uploaded. Literally all of them. As thumbnails. ModDB's imagebox
-        caches all the urls for videos on the page so this grabs them all. Lists might be long, but this
-        is all the videos. They can be invidually parsed to get full fledged media objects from them.
-
-        Returns
-        --------
-        List[Thumbnail]
-            The list of video type thumbnails parsed from the page
-        """
-        html = get_page(f"{self.url}/videos")
-        return self._get_media(2, html=html)
-
-    def get_tutorials(
-        self,
-        index: int = 1,
-        *,
-        query: str = None,
-        difficulty: Difficulty = None,
-        tutorial_type: TutorialCategory = None,
-        sort: Tuple[str, str] = None,
-    ) -> ResultList:
-        """Get a page of tutorial for the page. Each page will yield up to 30 tutorials.
-
-        Parameters
-        -----------
-        index : Optional[int]
-            The page number to get the tutorials from.
-        query : Optional[str]
-            The string query to look for in the tutorial title, optional.
-        difficulty : Optional[Difficulty]
-            Enum type representing the difficulty of the tutorial, optional.
-        tutorial_type : Optional[TutorialCategory]
-            Enum type representing the theme/type/category of the tutorial, optional.
-        sort : Optional[Tuple[str, str]]
-            The sorting tuple to sort by the results
-
-        Returns
-        --------
-        ResultList[Thumbnail]
-            The list of article type thumbnails parsed from the page
-        """
-        params = {
-            "filter": "t",
-            "kw": query,
-            "subtype": tutorial_type.value if tutorial_type else None,
-            "meta": difficulty.value if difficulty else None,
-            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
-        }
-
-        return self._get(f"{self.url}/tutorials/page/{index}", params=params)
-
-
-class GetWaresMixin:
-    """Abstrac class implementing get_software and get_hardware"""
-
-    def get_hardware(
-        self,
-        index: int = 1,
-        *,
-        query: str = None,
-        status: Status = None,
-        category: HardwareCategory = None,
-        timeframe: TimeFrame = None,
-        sort: Tuple[str, str] = None,
-    ) -> ResultList:
-        """Get a page of hardware for the platform. Each page will yield up to 30 hardware.
-
-        Parameters
-        -----------
-        index : Optional[int]
-            The page number to get the hardware for.
-        query : Optional[str]
-            The text to look for in the hardware's names
-        status : Optional[Status]
-            Status of the hardware (released, unreleased, early access...)
-        category : Optional[HardwareCategory]
-            Category of the hardware (headset, controller, ect...)
-        timeframe : Optional[TimeFrame]
-            The time period this was released in (last 24hr, last week, last month)
-        sort : Optional[Tuple[str, str]]
-            The sorting tuple to sort by
-
-        Returns
-        --------
-        ResultList[Thumbnail]
-            List of hardware like thumbnails that can be parsed individually.
-        """
-        params = {
-            "filter": "t",
-            "kw": query,
-            "released": status.value if status else None,
-            "category": category.value if category else None,
-            "timeframe": timeframe.value if timeframe else None,
-            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
-        }
-
-        return self._get(f"{self.url}/hardware/page/{index}", params=params)
-
-    def get_software(
-        self,
-        index: int = 1,
-        *,
-        query: str = None,
-        status: Status = None,
-        category: SoftwareCategory = None,
-        timeframe: TimeFrame = None,
-        sort: Tuple[str, str] = None,
-    ) -> ResultList:
-        """Get a page of software for the platform. Each page will yield up to 30 software.
-
-        Parameters
-        -----------
-        index : Optional[int]
-            The page number to get the software for.
-        query : Optional[str]
-            The text to look for in the hardware's names
-        status : Optional[Status]
-            Status of the hardware (released, unreleased, early access...)
-        category : Optional[SoftwareCategory]
-            Category of the hardware (headset, controller, ect...)
-        timeframe : Optional[TimeFrame]
-            The time period this was released in (last 24hr, last week, last month)
-        sort : Optional[Tuple[str, str]]
-            The sorting tuple to sort by
-
-        Returns
-        --------
-        ResultList[Thumbnail]
-            List of software like thumbnails that can be parsed individually.
-        """
-        params = {
-            "filter": "t",
-            "kw": query,
-            "released": status.value if status else None,
-            "category": category.value if category else None,
-            "timeframe": timeframe.value if timeframe else None,
-            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
-        }
-
-        return self._get(f"{self.url}/software/page/{index}", params=params)
-
-
-class RSSFeedMixin:
-    def rss(self, type: RSSType):
-        """Get the RSS feed url for the page depending on which feed type you want
-
-        Parameters
-        -----------
-        type : RSSType
-            The type of feed you desire to get
-
-        Returns
-        --------
-        str
-            URL for the feed type
-        """
-        return f"https://rss.moddb.com/{self._type.name}/{self.name_id}/{type.name}/feed/rss.xml"
-
-
-class GetAddonsMixin:
-    def get_addons(
-        self,
-        index: int = 1,
-        *,
-        query: str = None,
-        addon_type: AddonCategory = None,
-        timeframe: TimeFrame = None,
-        licence: Licence = None,
-        sort: Tuple[str, str] = None,
-    ) -> ResultList:
-        """Get a page of addons for the page. Each page will yield up to 30 addons.
-
-        Parameters
-        -----------
-        index : Optional[int]
-            The page number to get the addons from.
-        query : Optional[str]
-            The string query to search for in the addon name, optional.
-        addon_type : Optional[AddonCategory]
-            Type enum defining what category the file is.
-        timeframe : Optional[TimeFrame]
-            Time frame of when the file was added, optional
-        licence : Optional[Licence]
-            The licence for the addon, optional
-        sort : Optional[Tuple[str, str]]
-            The sorting tuple to sort by the results
-
-        Returns
-        --------
-        ResultList[Thumbnail]
-            The list of addon type thumbnails parsed from the page
-        """
-        params = {
-            "filter": "t",
-            "kw": query,
-            "category": addon_type.value if addon_type else None,
-            "timeframe": timeframe.value if timeframe else None,
-            "licence": licence.value if licence else None,
-            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
-        }
-        return self._get(f"{self.url}/addons/page/{index}", params=params)
-
-
-class GetWatchersMixin:
-    def get_watchers(self, index: int = 1, *, query: str = None, sort: Tuple[str, str] = None) -> ResultList:
-        """Get a page of watchers for the page. Each page will yield up to 30 members.
-
-        Parameters
-        -----------
-        index : Optional[int]
-            The page number to get the watchers from.
-        query : Optional[str]
-            The string query to search for in the watcher name, optional.
-        sort : Optional[Tuple[str, str]]
-            The sorting tuple to sort by the results
-
-        Returns
-        --------
-        ResultList[Thumbnail]
-            The list of member type thumbnails parsed from the page
-        """
-
-        params = {
-            "filter": "t",
-            "kw": query,
-            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
-        }
-
-        return self._get(f"{self.url}/watchers/page/{index}", params=params)
+from __future__ import annotations
+
+from typing import TYPE_CHECKING, List, Tuple, Union
+
+from ..boxes import Tag
+from ..utils import BASE_URL, get_page, get_sitearea
+
+if TYPE_CHECKING:
+    from ..boxes import ResultList, Thumbnail
+    from ..enums import (
+        AddonCategory,
+        ArticleCategory,
+        Difficulty,
+        FileCategory,
+        Genre,
+        HardwareCategory,
+        Licence,
+        PlayerStyle,
+        RSSType,
+        Scope,
+        SoftwareCategory,
+        Status,
+        Theme,
+        TimeFrame,
+        TutorialCategory,
+    )
+    from ..utils import Object
+    from .game import Game
+
+
+class GetGamesMixin:
+    """Abstract class containing the get_games method"""
+
+    def get_games(
+        self,
+        index: int = 1,
+        *,
+        query: str = None,
+        status: Status = None,
+        genre: Genre = None,
+        theme: Theme = None,
+        scope: Scope = None,
+        players: PlayerStyle = None,
+        timeframe: TimeFrame = None,
+        sort: Tuple[str, str] = None,
+    ) -> ResultList:
+        """Get a page of games for the model. Each page will yield up to 30 games.
+
+        Parameters
+        -----------
+        index : Optional[int]
+            The page number to get the games for.
+        query : Optional[str]
+            The text to look for in the game names.
+        status : Optional[Status]
+            The status of the game (unreleased, released, early access, ect...)
+        genre : Optional[Genre]
+            The genre of the game (fps, tower defense)
+        theme : Optional[Theme]
+            The theme of the game (fantasy, action)
+        scope : Optional[Scope]
+            The scope of the game (AAA, indie)
+        players : Optional[PlayerStyle]
+            Player styles of the game (co-op, singleplayer)
+        timeframe : Optional[TimeFrame]
+            The time period this was released in (last 24hr, last week, last month)
+        sort : Optional[Tuple[str, str]]
+            The sorting tuple to sort by the results
+
+        Returns
+        --------
+        ResultList[Thumbnail]
+            List of game like thumbnails that can be parsed individually.
+        """
+        params = {
+            "filter": "t",
+            "kw": query,
+            "released": status.value if status else None,
+            "genre": genre.value if genre else None,
+            "theme": theme.value if theme else None,
+            "indie": scope.value if scope else None,
+            "players": players.value if players else None,
+            "timeframe": timeframe.value if timeframe else None,
+            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
+        }
+
+        return self._get(f"{self.url}/games/page/{index}", params=params)
+
+
+class GetModsMixin:
+    """Abstract class containing the get_mod method"""
+
+    def get_mods(
+        self,
+        index: int = 1,
+        *,
+        query: str = None,
+        status: Status = None,
+        genre: Genre = None,
+        theme: Theme = None,
+        players: PlayerStyle = None,
+        timeframe: TimeFrame = None,
+        game: Union[Game, Object] = None,
+        sort: Tuple[str, str] = None,
+    ) -> ResultList:
+        """Get a page of mods for the game. Each page will yield up to 30 mods.
+
+        Parameters
+        -----------
+        index : int
+            The page number to get the mods from.
+        query : Optional[str]
+            The text to look for in the mod names.
+        status : Optional[Status]
+            The status of the mod (unreleased, released, early access, ect...)
+        genre : Optional[Genre]
+            The genre of the mod (fps, tower defense)
+        theme : Optional[Theme]
+            The theme of the mod (fantasy, action)
+        players : Optional[PlayerStyle]
+            Player styles of the mod (co-op, singleplayer)
+        timeframe : Optional[TimeFrame]
+            The time period this was released in (last 24hr, last week, last month)
+        game : Union[mod, Object]
+            An mod object or an object with an id attribute which represents the
+            mod the mod belongs to.
+        sort : Optional[Tuple[str, str]]
+            The sorting tuple to sort by the results
+
+        Returns
+        --------
+        ResultList[Thumbnail]
+            The list of mods type thumbnails parsed from the game
+        """
+        params = {
+            "filter": "t",
+            "kw": query,
+            "released": status.value if status else None,
+            "genre": genre.value if genre else None,
+            "theme": theme.value if theme else None,
+            "players": players.value if players else None,
+            "timeframe": timeframe.value if timeframe else None,
+            "game": game.id if game else None,
+            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
+        }
+
+        return self._get(f"{self.url}/mods/page/{index}", params=params)
+
+
+class GetEnginesMixin:
+    """Abstract class containing the get_engines method"""
+
+    def get_engines(
+        self,
+        index: int = 1,
+        *,
+        query: str = None,
+        status: Status = None,
+        licence: Licence = None,
+        timeframe: TimeFrame = None,
+        sort: Tuple[str, str] = None,
+    ) -> ResultList:
+        """Get a page of engines for the game. Each page will yield up to 30 engines.
+
+        Parameters
+        -----------
+        index : int
+            The page number to get the engines from.
+        query : Optional[str]
+            The text to look for in the engine names.
+        status : Optional[Status]
+            The status of the game (unreleased, released, early access, ect...)
+        licence : Optional[Licence]
+            The licence of the engine (open source, proprietary, ect...)
+        timeframe : Optional[TimeFrame]
+            The time period this was released in (last 24hr, last week, last month)
+        sort : Optional[Tuple[str, str]]
+            The sorting tuple to sort by the results
+        Returns
+        --------
+        ResultList[Thumbnail]
+            The list of engine type thumbnails parsed from the game
+        """
+        params = {
+            "filter": "t",
+            "kw": query,
+            "released": status.value if status else None,
+            "licence": licence.value if licence else None,
+            "timeframe": timeframe.value if timeframe else None,
+            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
+        }
+
+        return self._get(f"{self.url}/engines/page/{index}", params=params)
+
+
+class SharedMethodsMixin:
+    """Abstract class that implements a certain amount of top level methods shared between Pages
+    and Hardware"""
+
+    def get_reviews(
+        self,
+        index: int = 1,
+        *,
+        query: str = None,
+        rating: int = None,
+        sort: Tuple[str, str] = None,
+    ) -> ResultList:
+        """Get a page of reviews for the page. Each page will yield up to 10 reviews.
+
+        Parameters
+        -----------
+        index : Optional[int]
+            The page number to get the reviews from.
+        query : Optional[str]
+            The string to look for in the review, optional.
+        rating : Optiona[int]
+            A number between 1 and 10 to get the ratings
+        sort : Optional[Tuple[str, str]]
+            The sorting tuple to sort by the results
+
+        Returns
+        --------
+        ResultList[Review]
+            The list of reviews parsed from the page
+        """
+        from .opinion import ReviewList, parse_reviews
+
+        params = {
+            "filter": "t",
+            "kw": query,
+            "rating": rating,
+            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
+        }
+
+        base_url = f"{self.url}/reviews"
+        url = f"{base_url}/page/{index}"
+        html = get_page(url, params=params)
+        results, current_page, total_pages, total_results = parse_reviews(html)
+
+        return ReviewList(
+            results=results,
+            url=base_url,
+            total_results=total_results,
+            params=params,
+            current_page=current_page,
+            total_pages=total_pages,
+        )
+
+    def get_articles(
+        self,
+        index: int = 1,
+        *,
+        query: str = None,
+        category: ArticleCategory = None,
+        timeframe: TimeFrame = None,
+        sort: Tuple[str, str] = None,
+    ) -> ResultList:
+        """Get a page of articles for the page. Each page will yield up to 30 articles.
+
+        Parameters
+        -----------
+        index : Optional[int]
+            The page number to get the articles from.
+        query : Optional[str]
+            The string query to search for in the article name, optional.
+        category : Optional[ArticleCategory]
+            Type enum defining what the article is, optional
+        timeframe : Optional[TimeFrame]
+            The time period this was released in (last 24hr, last week, last month)
+        sort : Optional[Tuple[str, str]]
+            The sorting tuple to sort by the results
+
+        Returns
+        --------
+        ResultList[Thumbnail]
+            The list of article type thumbnails parsed from the page
+        """
+        params = {
+            "filter": "t",
+            "kw": query,
+            "type": category.value if category else None,
+            "timeframe": timeframe.value if timeframe else None,
+            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
+        }
+
+        return self._get(f"{self.url}/articles/page/{index}", params=params)
+
+    def get_files(
+        self,
+        index: int = 1,
+        *,
+        query: str = None,
+        category: FileCategory = None,
+        addon_type: AddonCategory = None,
+        timeframe: TimeFrame = None,
+        sort: Tuple[str, str] = None,
+    ) -> ResultList:
+        """Get a page of files for the page. Each page will yield up to 30 files.
+
+        Parameters
+        -----------
+        index : Optional[int]
+            The page number to get the files from.
+        query : Optional[str]
+            The string query to search for in the file name, optional.
+        category : [FileCategory]
+            Type enum defining what the file is, optional
+        addon_type : Optional[AddonCategory]
+            Type enum defining what category the file is.
+        timeframe : Optional[TimeFrame]
+            The time period this was released in (last 24hr, last week, last month)
+        sort : Optional[Tuple[str, str]]
+            The sorting tuple to sort by the results
+
+        Returns
+        --------
+        ResultList[Thumbnail]
+            The list of file type thumbnails parsed from the page
+        """
+        params = {
+            "filter": "t",
+            "kw": query,
+            "category": category.value if category else None,
+            "categoryaddon": addon_type.value if addon_type else None,
+            "timeframe": timeframe.value if timeframe else None,
+            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
+        }
+
+        return self._get(f"{self.url}/downloads/page/{index}", params=params)
+
+    def get_images(self) -> List[Thumbnail]:
+        """Get all the images a page has uploaded. Literally all of them. As thumbnails. ModDB's imagebox
+        caches all the urls for images on the page so this grabs them all. Lists might be long, but this
+        is all the images. They can be invidually parsed to get full fledged media objects from them.
+
+        Returns
+        --------
+        List[Thumbnail]
+            The list of image type thumbnails parsed from the page
+        """
+        html = get_page(f"{self.url}/images")
+        return self._get_media(1, html=html)
+
+    def get_videos(self) -> List[Thumbnail]:
+        """Get all the videos a page has uploaded. Literally all of them. As thumbnails. ModDB's imagebox
+        caches all the urls for videos on the page so this grabs them all. Lists might be long, but this
+        is all the videos. They can be invidually parsed to get full fledged media objects from them.
+
+        Returns
+        --------
+        List[Thumbnail]
+            The list of video type thumbnails parsed from the page
+        """
+        html = get_page(f"{self.url}/videos")
+        return self._get_media(2, html=html)
+
+    def get_tutorials(
+        self,
+        index: int = 1,
+        *,
+        query: str = None,
+        difficulty: Difficulty = None,
+        tutorial_type: TutorialCategory = None,
+        sort: Tuple[str, str] = None,
+    ) -> ResultList:
+        """Get a page of tutorial for the page. Each page will yield up to 30 tutorials.
+
+        Parameters
+        -----------
+        index : Optional[int]
+            The page number to get the tutorials from.
+        query : Optional[str]
+            The string query to look for in the tutorial title, optional.
+        difficulty : Optional[Difficulty]
+            Enum type representing the difficulty of the tutorial, optional.
+        tutorial_type : Optional[TutorialCategory]
+            Enum type representing the theme/type/category of the tutorial, optional.
+        sort : Optional[Tuple[str, str]]
+            The sorting tuple to sort by the results
+
+        Returns
+        --------
+        ResultList[Thumbnail]
+            The list of article type thumbnails parsed from the page
+        """
+        params = {
+            "filter": "t",
+            "kw": query,
+            "subtype": tutorial_type.value if tutorial_type else None,
+            "meta": difficulty.value if difficulty else None,
+            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
+        }
+
+        return self._get(f"{self.url}/tutorials/page/{index}", params=params)
+
+
+class GetWaresMixin:
+    """Abstrac class implementing get_software and get_hardware"""
+
+    def get_hardware(
+        self,
+        index: int = 1,
+        *,
+        query: str = None,
+        status: Status = None,
+        category: HardwareCategory = None,
+        timeframe: TimeFrame = None,
+        sort: Tuple[str, str] = None,
+    ) -> ResultList:
+        """Get a page of hardware for the platform. Each page will yield up to 30 hardware.
+
+        Parameters
+        -----------
+        index : Optional[int]
+            The page number to get the hardware for.
+        query : Optional[str]
+            The text to look for in the hardware's names
+        status : Optional[Status]
+            Status of the hardware (released, unreleased, early access...)
+        category : Optional[HardwareCategory]
+            Category of the hardware (headset, controller, ect...)
+        timeframe : Optional[TimeFrame]
+            The time period this was released in (last 24hr, last week, last month)
+        sort : Optional[Tuple[str, str]]
+            The sorting tuple to sort by
+
+        Returns
+        --------
+        ResultList[Thumbnail]
+            List of hardware like thumbnails that can be parsed individually.
+        """
+        params = {
+            "filter": "t",
+            "kw": query,
+            "released": status.value if status else None,
+            "category": category.value if category else None,
+            "timeframe": timeframe.value if timeframe else None,
+            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
+        }
+
+        return self._get(f"{self.url}/hardware/page/{index}", params=params)
+
+    def get_software(
+        self,
+        index: int = 1,
+        *,
+        query: str = None,
+        status: Status = None,
+        category: SoftwareCategory = None,
+        timeframe: TimeFrame = None,
+        sort: Tuple[str, str] = None,
+    ) -> ResultList:
+        """Get a page of software for the platform. Each page will yield up to 30 software.
+
+        Parameters
+        -----------
+        index : Optional[int]
+            The page number to get the software for.
+        query : Optional[str]
+            The text to look for in the hardware's names
+        status : Optional[Status]
+            Status of the hardware (released, unreleased, early access...)
+        category : Optional[SoftwareCategory]
+            Category of the hardware (headset, controller, ect...)
+        timeframe : Optional[TimeFrame]
+            The time period this was released in (last 24hr, last week, last month)
+        sort : Optional[Tuple[str, str]]
+            The sorting tuple to sort by
+
+        Returns
+        --------
+        ResultList[Thumbnail]
+            List of software like thumbnails that can be parsed individually.
+        """
+        params = {
+            "filter": "t",
+            "kw": query,
+            "released": status.value if status else None,
+            "category": category.value if category else None,
+            "timeframe": timeframe.value if timeframe else None,
+            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
+        }
+
+        return self._get(f"{self.url}/software/page/{index}", params=params)
+
+
+class RSSFeedMixin:
+    def rss(self, type: RSSType):
+        """Get the RSS feed url for the page depending on which feed type you want
+
+        Parameters
+        -----------
+        type : RSSType
+            The type of feed you desire to get
+
+        Returns
+        --------
+        str
+            URL for the feed type
+        """
+        return f"https://rss.moddb.com/{self._type.name}/{self.name_id}/{type.name}/feed/rss.xml"
+
+
+class GetAddonsMixin:
+    def get_addons(
+        self,
+        index: int = 1,
+        *,
+        query: str = None,
+        addon_type: AddonCategory = None,
+        timeframe: TimeFrame = None,
+        licence: Licence = None,
+        sort: Tuple[str, str] = None,
+    ) -> ResultList:
+        """Get a page of addons for the page. Each page will yield up to 30 addons.
+
+        Parameters
+        -----------
+        index : Optional[int]
+            The page number to get the addons from.
+        query : Optional[str]
+            The string query to search for in the addon name, optional.
+        addon_type : Optional[AddonCategory]
+            Type enum defining what category the file is.
+        timeframe : Optional[TimeFrame]
+            Time frame of when the file was added, optional
+        licence : Optional[Licence]
+            The licence for the addon, optional
+        sort : Optional[Tuple[str, str]]
+            The sorting tuple to sort by the results
+
+        Returns
+        --------
+        ResultList[Thumbnail]
+            The list of addon type thumbnails parsed from the page
+        """
+        params = {
+            "filter": "t",
+            "kw": query,
+            "category": addon_type.value if addon_type else None,
+            "timeframe": timeframe.value if timeframe else None,
+            "licence": licence.value if licence else None,
+            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
+        }
+        return self._get(f"{self.url}/addons/page/{index}", params=params)
+
+
+class GetWatchersMixin:
+    def get_watchers(
+        self, index: int = 1, *, query: str = None, sort: Tuple[str, str] = None
+    ) -> ResultList:
+        """Get a page of watchers for the page. Each page will yield up to 30 members.
+
+        Parameters
+        -----------
+        index : Optional[int]
+            The page number to get the watchers from.
+        query : Optional[str]
+            The string query to search for in the watcher name, optional.
+        sort : Optional[Tuple[str, str]]
+            The sorting tuple to sort by the results
+
+        Returns
+        --------
+        ResultList[Thumbnail]
+            The list of member type thumbnails parsed from the page
+        """
+
+        params = {
+            "filter": "t",
+            "kw": query,
+            "sort": f"{sort[0]}-{sort[1]}" if sort else None,
+        }
+
+        return self._get(f"{self.url}/watchers/page/{index}", params=params)
+
+
+class GetTagsMixin:
+    def get_tags(self):
+        """Get more tags for a page.
+
+        Returns
+        --------
+        List[Tag]
+            List of returned tags
+        """
+
+        params = {"ajax": "t", "sitearea": get_sitearea(self.url), "siteareaid": self.id}
+
+        resp = get_page(f"{BASE_URL}/tags/ajax/more", params=params, json=True)
+
+        return [Tag(**tag) for tag in resp["tags"].values()]
```

### Comparing `moddb-0.8.1/moddb/pages/mod.py` & `moddb-0.9.0/moddb/pages/mod.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,53 @@
-import bs4
-
-from ..utils import concat_docs
-from .base import PageMetaClass
-from .mixins import GetAddonsMixin
-from ..enums import SearchCategory
-
-
-@concat_docs
-class Mod(PageMetaClass, GetAddonsMixin):
-    """Basically just a subclass of Page
-
-    Parameters
-    -----------
-    html : bs4.BeautifulSoup
-        The html to parse. Allows for finer control.
-
-    Filtering
-    ----------
-    released : :class:`.Status`
-        The status of the mod (released, unreleased)
-    genre : :class:`.Genre`
-        The genre of the mod (fps, tower defense)
-    theme : :class:`.Theme`
-        The theme of the mod (fantasy, action)
-    players : :class:`.PlayerStyle`
-        Player styles of the mod (co-op, singleplayer)
-    timeframe : :class:`.TimeFrame`
-        The time period this was released in (last 24hr, last week, last month)
-    game : Union[:class:`.Game`, :class:`.Object`]
-        An game object or an object with an id attribute which represents the
-        game the mod belongs to.
-
-    Sorting
-    --------
-        * **released** - when the object was released, asc is oldest, desc is most recent
-        * **id** - when it was added to moddb, asc is oldest, desc is most recent
-        * **ranktoday** - order by daily ranking, asc is highest ranked, desc is lowest rank
-        * **visitstotal** - order by most views, asc is highest views, desc is lowest views
-        * **rating** - order by rating, asc is highest rating, desc is lowest rating
-        * **name** - order alphabetically, asc is a-z, desc is z-a
-        * **game** - order by game???
-        * **dateup** - order by latest update, asc is most recent update first, desc is oldest update first
-
-    """
-
-    def __init__(self, html: bs4.BeautifulSoup):
-        super().__init__(html, SearchCategory.mods)
+from __future__ import annotations
+
+from typing import TYPE_CHECKING
+
+from ..enums import SearchCategory
+from ..utils import concat_docs
+from .base import PageMetaClass
+from .mixins import GetAddonsMixin
+
+if TYPE_CHECKING:
+    from bs4 import BeautifulSoup
+
+
+@concat_docs
+class Mod(PageMetaClass, GetAddonsMixin):
+    """Basically just a subclass of Page
+
+    Parameters
+    -----------
+    html : bs4.BeautifulSoup
+        The html to parse. Allows for finer control.
+
+    Filtering
+    ----------
+    released : :class:`.Status`
+        The status of the mod (released, unreleased)
+    genre : :class:`.Genre`
+        The genre of the mod (fps, tower defense)
+    theme : :class:`.Theme`
+        The theme of the mod (fantasy, action)
+    players : :class:`.PlayerStyle`
+        Player styles of the mod (co-op, singleplayer)
+    timeframe : :class:`.TimeFrame`
+        The time period this was released in (last 24hr, last week, last month)
+    game : Union[:class:`.Game`, :class:`.Object`]
+        An game object or an object with an id attribute which represents the
+        game the mod belongs to.
+
+    Sorting
+    --------
+        * **released** - when the object was released, asc is oldest, desc is most recent
+        * **id** - when it was added to moddb, asc is oldest, desc is most recent
+        * **ranktoday** - order by daily ranking, asc is highest ranked, desc is lowest rank
+        * **visitstotal** - order by most views, asc is highest views, desc is lowest views
+        * **rating** - order by rating, asc is highest rating, desc is lowest rating
+        * **name** - order alphabetically, asc is a-z, desc is z-a
+        * **game** - order by game???
+        * **dateup** - order by latest update, asc is most recent update first, desc is oldest update first
+
+    """
+
+    def __init__(self, html: BeautifulSoup):
+        super().__init__(html, SearchCategory.mods)
```

### Comparing `moddb-0.8.1/moddb/pages/opinion.py` & `moddb-0.9.0/moddb/pages/opinion.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,188 +1,200 @@
-import re
-
-from ..utils import concat_docs, get_date, get_list_stats, join
-from ..boxes import ModDBList, Thumbnail, Option
-from ..enums import ThumbnailType
-from .base import BaseMetaClass
-
-
-class ReviewList(ModDBList):
-    """Represents a list of reviews
-
-    Attributes
-    -----------
-    current_page : int
-        The page of results this objects represents
-    total_pages : int
-        The total amount of result pages available
-    total_results : int
-        The total amount of results available
-    """
-
-    def _parse_method(self, html):
-        return parse_reviews(html)
-
-
-def parse_reviews(html):
-    review_box = html.find("div", class_="normalbox browsebox")
-
-    try:
-        raw_ratings = (
-            review_box.find("div", class_="inner")
-            .find("div", class_="table")
-            .find_all("div", class_=["rowrating"], recursive=False)
-        )
-    except AttributeError:
-        return [], 1, 1, 0
-
-    reviews = []
-    for rating in raw_ratings:
-        next_sibling = rating.find_next_sibling("div", class_=["rowcontent"])
-        if next_sibling is not None and "rowcontentnext" in next_sibling["class"]:
-            reviews.append(Review(rating=rating, text=next_sibling))
-        else:
-            reviews.append(Review(rating=rating))
-
-    return reviews, *get_list_stats(review_box, 10)
-
-
-@concat_docs
-class Review:
-    """Represents a review.
-
-    Filtering
-    -----------
-    rating : int
-        A value from 1 to 10 denoting the rating number you're looking for
-    sitearea : Category
-        The type of model the rating is for (mod, engine, game)
-
-    Sorting
-    --------
-        * **ratingalt** - rating number, desc is biggest to lowest, asc is lowest to biggest
-        * **memberipid** - sort reviewer account age, asc is oldest reviewer first
-        * **positive** - how many people agree with it, desc is most to least people agreeing
-        * **negative** - how many people disagree with it, desc is most to least people disagreeing
-        * **id** - when it was added to moddb, asc is oldest, desc is most recent
-
-    Attributes
-    -----------
-    id : int
-        The review id
-    text : str
-        The contents of the review. Can be none if the member hasn't left any
-    rating : int
-        An int out of 10 representing the rating left with this review.
-    author : Thumbnail
-        A member like thumbnail of the member who left the review
-    date : datetime.datetime
-        Date and time of the review creation
-    agree : str
-            Link to agree with the review
-    disagree : str
-        Link to disagree with the review
-    """
-
-    def __init__(self, **attrs):
-        text = attrs.get("text")
-        if text:
-            self.text = text.text
-        else:
-            self.text = None
-
-        review = attrs.get("rating")
-        self.rating = int(review.span.string)
-
-        # id and hash are none if the review doesn't have content
-        try:
-            strings = ("Agree", "Delete", "Disagree")
-            self.id = int(re.findall(r"siteareaid=(\d*)", review.find("a", title=strings)["href"])[0])
-        except TypeError:
-            self.id = None
-
-        try:
-            self._hash = re.findall(r"hash=(.*)&", review.find("a", title="Delete")["href"])[0]
-        except TypeError:
-            self._hash = None
-
-        author = review.div.a
-        self.author = Thumbnail(
-            url=author["href"],
-            name=author.string.split(" ")[0],
-            type=ThumbnailType.member,
-        )
-        self.date = get_date(review.div.span.time["datetime"])
-
-        try:
-            self.agree = join(review.find("a", title="Agree")["href"])
-            self.disagree = join(review.find("a", title="Disagree")["href"])
-        except TypeError:
-            self.agree = None
-            self.disagree = None
-
-    def __repr__(self):
-        return f"<Review author={self.author.name} rating={self.rating}>"
-
-
-@concat_docs
-class Poll(BaseMetaClass):
-    """Represents a poll. Cannot be voted for due to restrictions implemented by the website.
-
-    Parameters
-    -----------
-    html : bs4.BeautifulSoup
-        The html to parse. Allows for finer control.
-
-    Filtering
-    ----------
-        month : Month
-            The month the poll you're looking for should be from
-        year : int
-            A int representing a year between 2002 and now. Anything below or above 2002 will
-            always return zero results.
-
-    Sorting
-    --------
-        * **totalvotes** - how many people voted on the poll, desc is most to least
-        * **name** - sort the poll alphabetically by name, asc is a-z
-        * **date** - when it was added to moddb, asc is oldest, desc is most recent
-
-    Attributes
-    -----------
-    question : str
-        The question of the poll
-    author : Thumbnail
-        A member like thumbnail of the member who posted the poll, usually ModDB staff
-    total : int
-        The total number of votes that have been cast
-    options : List[Option]
-        The list of available options for the poll
-    """
-
-    def __init__(self, html):
-        poll = html.find("div", class_="poll")
-        self.question = (
-            poll.parent.parent.parent.find("div", class_="normalcorner").find("span", class_="heading").string
-        )
-        self.name = self.question
-        super().__init__(html)
-        author = poll.find("p", class_="question").find("a")
-        self.author = Thumbnail(name=author.string, url=author["href"], type=ThumbnailType.member)
-
-        self.total = int(
-            re.search(r"([\d,]*) votes", poll.find("p", class_="question").text)[1].replace(",", "")
-        )
-
-        percentage = poll.find_all("div", class_="barouter")
-        rest = poll.find_all("p")[1:]
-
-        self.options = []
-        for index, _ in enumerate(percentage):
-            raw = percentage[index].div.string.replace("%", "").replace("\xa0", "")
-            percent = float(f"0.{raw}")
-            text = re.sub(r"\([\d,]* vote(s)?\)", "", rest[index].text)
-            votes = int(re.search(r"([\d,]*) vote(s)?", rest[index].span.string)[1].replace(",", ""))
-            self.options.append(Option(text=text, votes=votes, percent=percent))
-
-    def __repr__(self):
-        return f"<Poll question={self.question}>"
+from __future__ import annotations
+
+import re
+from typing import TYPE_CHECKING
+
+from ..boxes import ModDBList, Option, Thumbnail
+from ..enums import ThumbnailType
+from ..utils import concat_docs, get_date, get_list_stats, join
+from .base import BaseMetaClass
+
+if TYPE_CHECKING:
+    from bs4 import BeautifulSoup
+
+
+class ReviewList(ModDBList):
+    """Represents a list of reviews
+
+    Attributes
+    -----------
+    current_page : int
+        The page of results this objects represents
+    total_pages : int
+        The total amount of result pages available
+    total_results : int
+        The total amount of results available
+    """
+
+    def _parse_method(self, html: BeautifulSoup):
+        return parse_reviews(html)
+
+
+def parse_reviews(html):
+    review_box = html.find("div", class_="normalbox browsebox")
+
+    try:
+        raw_ratings = (
+            review_box.find("div", class_="inner")
+            .find("div", class_="table")
+            .find_all("div", class_=["rowrating"], recursive=False)
+        )
+    except AttributeError:
+        return [], 1, 1, 0
+
+    reviews = []
+    for rating in raw_ratings:
+        next_sibling = rating.find_next_sibling("div", class_=["rowcontent"])
+        if next_sibling is not None and "rowcontentnext" in next_sibling["class"]:
+            reviews.append(Review(rating=rating, text=next_sibling))
+        else:
+            reviews.append(Review(rating=rating))
+
+    return reviews, *get_list_stats(review_box, 10)
+
+
+@concat_docs
+class Review:
+    """Represents a review.
+
+    Filtering
+    -----------
+    rating : int
+        A value from 1 to 10 denoting the rating number you're looking for
+    sitearea : Category
+        The type of model the rating is for (mod, engine, game)
+
+    Sorting
+    --------
+        * **ratingalt** - rating number, desc is biggest to lowest, asc is lowest to biggest
+        * **memberipid** - sort reviewer account age, asc is oldest reviewer first
+        * **positive** - how many people agree with it, desc is most to least people agreeing
+        * **negative** - how many people disagree with it, desc is most to least people disagreeing
+        * **id** - when it was added to moddb, asc is oldest, desc is most recent
+
+    Attributes
+    -----------
+    id : int
+        The review id
+    text : str
+        The contents of the review. Can be none if the member hasn't left any
+    rating : int
+        An int out of 10 representing the rating left with this review.
+    author : Thumbnail
+        A member like thumbnail of the member who left the review
+    date : datetime.datetime
+        Date and time of the review creation
+    agree : str
+            Link to agree with the review
+    disagree : str
+        Link to disagree with the review
+    """
+
+    def __init__(self, **attrs):
+        text = attrs.get("text")
+        if text:
+            self.text = text.text
+        else:
+            self.text = None
+
+        review = attrs.get("rating")
+        self.rating = int(review.span.string)
+
+        # id and hash are none if the review doesn't have content
+        try:
+            strings = ("Agree", "Delete", "Disagree")
+            self.id = int(
+                re.findall(r"siteareaid=(\d*)", review.find("a", title=strings)["href"])[0]
+            )
+        except TypeError:
+            self.id = None
+
+        try:
+            self._hash = re.findall(r"hash=(.*)&", review.find("a", title="Delete")["href"])[0]
+        except TypeError:
+            self._hash = None
+
+        author = review.div.a
+        self.author = Thumbnail(
+            url=author["href"],
+            name=author.string.split(" ")[0],
+            type=ThumbnailType.member,
+        )
+        self.date = get_date(review.div.span.time["datetime"])
+
+        try:
+            self.agree = join(review.find("a", title="Agree")["href"])
+            self.disagree = join(review.find("a", title="Disagree")["href"])
+        except TypeError:
+            self.agree = None
+            self.disagree = None
+
+    def __repr__(self):
+        return f"<Review author={self.author.name} rating={self.rating}>"
+
+
+@concat_docs
+class Poll(BaseMetaClass):
+    """Represents a poll. Cannot be voted for due to restrictions implemented by the website.
+
+    Parameters
+    -----------
+    html : bs4.BeautifulSoup
+        The html to parse. Allows for finer control.
+
+    Filtering
+    ----------
+        month : Month
+            The month the poll you're looking for should be from
+        year : int
+            A int representing a year between 2002 and now. Anything below or above 2002 will
+            always return zero results.
+
+    Sorting
+    --------
+        * **totalvotes** - how many people voted on the poll, desc is most to least
+        * **name** - sort the poll alphabetically by name, asc is a-z
+        * **date** - when it was added to moddb, asc is oldest, desc is most recent
+
+    Attributes
+    -----------
+    question : str
+        The question of the poll
+    author : Thumbnail
+        A member like thumbnail of the member who posted the poll, usually ModDB staff
+    total : int
+        The total number of votes that have been cast
+    options : List[Option]
+        The list of available options for the poll
+    """
+
+    def __init__(self, html: BeautifulSoup):
+        poll = html.find("div", class_="poll")
+        self.question = (
+            poll.parent.parent.parent.find("div", class_="normalcorner")
+            .find("span", class_="heading")
+            .string
+        )
+        self.name = self.question
+        super().__init__(html)
+        author = poll.find("p", class_="question").find("a")
+        self.author = Thumbnail(name=author.string, url=author["href"], type=ThumbnailType.member)
+
+        self.total = int(
+            re.search(r"([\d,]*) votes", poll.find("p", class_="question").text)[1].replace(",", "")
+        )
+
+        percentage = poll.find_all("div", class_="barouter")
+        rest = poll.find_all("p")[1:]
+
+        self.options = []
+        for index, _ in enumerate(percentage):
+            raw = percentage[index].div.string.replace("%", "").replace("\xa0", "")
+            percent = float(f"0.{raw}")
+            text = re.sub(r"\([\d,]* vote(s)?\)", "", rest[index].text)
+            votes = int(
+                re.search(r"([\d,]*) vote(s)?", rest[index].span.string)[1].replace(",", "")
+            )
+            self.options.append(Option(text=text, votes=votes, percent=percent))
+
+    def __repr__(self):
+        return f"<Poll question={self.question}>"
```

### Comparing `moddb-0.8.1/moddb/utils.py` & `moddb-0.9.0/moddb/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,458 +1,480 @@
-import bs4
-from .enums import ThumbnailType
-from .errors import ModdbException, AwaitingAuthorisation
-
-import re
-import sys
-import uuid
-import json
-import random
-import inspect
-import logging
-import datetime
-import requests
-from typing import Tuple
-from urllib.parse import urljoin
-from bs4 import BeautifulSoup, Tag
-from pyrate_limiter import Duration, Limiter, RequestRate
-
-LOGGER = logging.getLogger("moddb")
-BASE_URL = "https://www.moddb.com"
-LIMITER = Limiter(
-    # request stuff slowly, like a human
-    RequestRate(1, Duration.SECOND * 2.5),
-    # take breaks when requesting stuff, like a human
-    RequestRate(60, Duration.MINUTE * 5),
-)
-
-time_mapping = {
-    "year": 125798400,
-    "month": 2419200,
-    "week": 604800,
-    "day": 86400,
-    "hour": 3600,
-    "minute": 60,
-    "econd": 1,
-}
-
-user_agent_list = [
-    # Chrome
-    "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/60.0.3112.113 Safari/537.36",
-    "Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/60.0.3112.90 Safari/537.36",
-    "Mozilla/5.0 (Windows NT 5.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/60.0.3112.90 Safari/537.36",
-    "Mozilla/5.0 (Windows NT 6.2; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/60.0.3112.90 Safari/537.36",
-    "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/44.0.2403.157 Safari/537.36",
-    "Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/60.0.3112.113 Safari/537.36",
-    "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/57.0.2987.133 Safari/537.36",
-    "Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/57.0.2987.133 Safari/537.36",
-    "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/55.0.2883.87 Safari/537.36",
-    "Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/55.0.2883.87 Safari/537.36",
-    # Firefox
-    "Mozilla/4.0 (compatible; MSIE 9.0; Windows NT 6.1)",
-    "Mozilla/5.0 (Windows NT 6.1; WOW64; Trident/7.0; rv:11.0) like Gecko",
-    "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; WOW64; Trident/5.0)",
-    "Mozilla/5.0 (Windows NT 6.1; Trident/7.0; rv:11.0) like Gecko",
-    "Mozilla/5.0 (Windows NT 6.2; WOW64; Trident/7.0; rv:11.0) like Gecko",
-    "Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; rv:11.0) like Gecko",
-    "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.0; Trident/5.0)",
-    "Mozilla/5.0 (Windows NT 6.3; WOW64; Trident/7.0; rv:11.0) like Gecko",
-    "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Trident/5.0)",
-    "Mozilla/5.0 (Windows NT 6.1; Win64; x64; Trident/7.0; rv:11.0) like Gecko",
-    "Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.1; WOW64; Trident/6.0)",
-    "Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.1; Trident/6.0)",
-    "Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 5.1; Trident/4.0; .NET CLR 2.0.50727; .NET CLR 3.0.4506.2152; .NET CLR 3.5.30729)",
-]
-
-
-def concat_docs(cls):
-    """Does it look like I'm enjoying this?"""
-    attributes = []
-
-    def get_docs(parent):
-        nonlocal attributes
-        if parent.__name__ == "object":
-            return
-
-        docs = parent.__doc__.splitlines()
-        if "    Attributes" in docs:
-            attributes = docs[docs.index("    Attributes") + 2 :] + attributes
-
-        source = inspect.getsource(parent.__init__)
-        source = source[source.index("):") :]
-
-        if "super().__init__" in source:
-            get_docs(parent.__base__)
-        elif "__init__" in source:
-            get_docs(parent.__base__.__base__)
-
-    get_docs(cls)
-    original = cls.__doc__.splitlines()
-    if "    Attributes" not in original:
-        original.append("    Attributes")
-        original.append("    -----------")
-
-    final = original[: original.index("    Attributes") + 2]
-    final.extend([x for x in attributes if x.strip()])
-    cls.__doc__ = "\n".join(final)
-
-    return cls
-
-
-def get_date(d: str) -> datetime.datetime:
-    """A helper function that takes a ModDB string representation of time and returns an equivalent
-    datetime.datetime object. This can range from a datetime with the full year to
-    second to just a year and a month.
-
-    Parameters
-    -----------
-    d : str
-        String representation of a datetime
-
-    Returns
-    -------
-    datetime.datetime
-        The datetime object for the given string
-    """
-    try:
-        return datetime.datetime.strptime(d[:-3] + d[-2:], "%Y-%m-%dT%H:%M:%S%z")
-    except ValueError:
-        pass
-
-    try:
-        return datetime.datetime.strptime(d, "%Y-%m-%d")
-    except ValueError:
-        pass
-
-    return datetime.datetime.strptime(d, "%Y-%m")
-
-
-def prepare_request(req: requests.Request, session):
-    """Prepared a request with the appropriate cookies"""
-    cookies = requests.utils.dict_from_cookiejar(session.cookies)
-
-    if req.cookies is not None:
-        req.cookies = {**req.cookies, **cookies}
-    else:
-        req.cookies = cookies
-
-    req.headers["User-Agent"] = random.choice(user_agent_list)
-
-    prepped = session.prepare_request(req)
-    return prepped
-
-
-def raise_for_status(response):
-    """Raise any error that could have occured"""
-    try:
-        text = response.json()
-        if text.get("error", False):
-            LOGGER.error(text["text"])
-            LOGGER.error(response.request.url)
-            LOGGER.error(response.request.body)
-            raise ModdbException(text["text"])
-    except json.decoder.JSONDecodeError:
-        response.raise_for_status()
-
-    if (
-        "is currently awaiting authorisation, which can take a couple of days while a"
-        in response.text.lower()
-    ):
-        raise AwaitingAuthorisation("This page is still await authorisation and cannot currently be parsed")
-
-
-def generate_login_cookies(username, password):
-    """Log a user in and return the `freeman` cookie containing the login hash"""
-    resp = requests.get(f"{BASE_URL}/members/login")
-    html = soup(resp.text)
-    form = html.find("form", attrs={"name": "membersform"})
-
-    username_input = form.find("input", id="membersusername")
-    botcatcher = form.find("input", type="text", id=False)
-
-    data = {
-        "referer": "",
-        username_input["name"]: username,
-        botcatcher["name"]: "",
-        "password": password,
-        "rememberme": ["1"],
-        "members": "Sign in",
-    }
-
-    login = requests.post(
-        f"{BASE_URL}/members/login",
-        data=data,
-        cookies=resp.cookies,
-        allow_redirects=False,
-    )
-
-    if "freeman" not in login.cookies:
-        raise ValueError(f"Login failed for user {username}")
-
-    return login.cookies
-
-
-@LIMITER.ratelimit("moddb", delay=True)
-def request(req: requests.Request):
-    """Helper function to make get/post requests with the current SESSION object.
-
-    Parameters
-    -----------
-    req : requests.Request
-        The request to perform
-
-    Return
-    -------
-    requests.Response
-        The returned response object
-
-    """
-    SESSION = sys.modules["moddb"].SESSION
-    prepped = prepare_request(req, SESSION)
-    r = SESSION.send(prepped)
-
-    raise_for_status(r)
-    return r
-
-
-def soup(html: str) -> BeautifulSoup:
-    """Simple helper function that takes a string representation of an html page and
-    returns a beautiful soup object"""
-
-    return BeautifulSoup(html, "html.parser")
-
-
-def get_page(url: str, *, params: dict = {}):
-    """A helper function that takes a url and returns a beautiful soup objects. This is used to center
-    the request making section of the library. Can also be passed a set of paramaters, used for sorting
-    and filtering in the search function.
-
-    Parameters
-    -----------
-    url : str
-        The url to get
-
-    params : dict
-        A dictionnary of filters and sorting key-value pairs.
-
-    Returns
-    -------
-    bs4.BeautifulSoup
-    """
-    r = request(requests.Request("GET", url, params=params))
-    return soup(r.text)
-
-
-def get_views(string: str) -> Tuple[int, int]:
-    """A helper function that takes a string reresentation of total something and
-    daily amount of that same thing and returns both as a tuple of ints.
-
-    Parameters
-    ------------
-    string : str
-        The string containing the numbers both total and daily
-
-    Returns
-    --------
-    Tuple[int, int]
-        Tuple contains the total views (first element) and the daily views (second element)
-    """
-    matches = re.search(r"^([0-9,]*) \(([0-9,]*) today\)$", string)
-    views = int(matches.group(1).replace(",", ""))
-    today = int(matches.group(2).replace(",", ""))
-
-    return views, today
-
-
-def join(path: str) -> str:
-    """Joins a partial moddb url with the base url and returns the combined url
-
-    Parameters
-    -----------
-    path : str
-        the url to join
-
-    Return
-    -------
-    str
-        The full url.
-
-    """
-    if not path.startswith(BASE_URL):
-        return urljoin(BASE_URL, path)
-
-    return path
-
-
-def normalize(string: str) -> str:
-    """Removes all extra fluff from a text to get the barebone content"""
-    return string.replace(",", "").replace("members", "").replace("member", "").strip()
-
-
-def get_media_type(img: Tag) -> int:
-    """Determines the type of the image through some very hacky stuff, might break"""
-    if img is None:
-        return 2
-    elif img["src"][-8:-5] == ".mp4":
-        return 0
-    else:
-        return 1
-
-
-def get_page_type(url: str) -> "ThumbnailType":
-    """Get the page type based on a url.
-
-    Parameters
-    -----------
-    url : str
-        The url to get
-
-    Return
-    -------
-    ThumbnailType
-        The type of the page
-    """
-    regex = r"\/((?!page|pages\b)\b\w+)\/"
-    type_mapping = {
-        "new": "article",
-        "feature": "article",
-        "tutorial": "article",
-        "download": "file",
-        "image": "media",
-        "audio": " media",
-        "video": "media",
-    }
-
-    matches = re.findall(regex, url)
-    match = matches[-1][0:-1] if matches[0].endswith("s") else matches[0]
-
-    try:
-        page_type = ThumbnailType[match]
-    except KeyError:
-        page_type = ThumbnailType[type_mapping[match]]
-
-    LOGGER.info("%s is type %s", url, page_type)
-    return page_type
-
-
-def ceildiv(a: int, b: int) -> int:
-    "Like a // b but rounded up instead of down."
-    return -(a // -b)
-
-
-def get_list_stats(result_box: bs4.BeautifulSoup, per_page: int = 30) -> Tuple[int, int, int]:
-    """Get the current page, total pages and total results from
-    a result list"""
-    stats = re.match(
-        r".*\(([0-9,]*) - ([0-9,]*) of ([0-9,]*)\)",
-        result_box.find("div", class_="normalcorner")
-        .find("div", class_="title")
-        .find("span", class_="heading")
-        .string,
-    )
-
-    if not stats:  # less than a page
-        return 1, 1, None
-
-    max_results = int(stats.group(2).replace(",", ""))
-    all_results = int(stats.group(3).replace(",", ""))
-    max_page = ceildiv(all_results, per_page)
-    current_page = ceildiv(max_results, per_page)
-
-    return current_page, max_page, all_results
-
-
-class Object:
-    """A dud objects that will transform every kwarg given into an attribute"""
-
-    def __init__(self, **kwargs):
-        self.__dict__.update(kwargs)
-
-
-def find(predicate, seq):
-    """A helper to return the first element found in the sequence
-    that meets the predicate. For example: ::
-
-        comment = find(lambda comment: comment.author.name == 'SilverElf', mod.comments.flatten())
-
-    would find the first :class:`.Comment` whose author's name is 'SilverElf' and return it.
-    If no entry is found, then ``None`` is returned.
-
-    This is different from `filter`_ due to the fact it stops the moment it finds
-    a valid entry.
-
-    .. _filter: https://docs.python.org/3.6/library/functions.html#filter
-
-    Parameters
-    -----------
-    predicate
-        A function that returns a boolean-like result.
-    seq : iterable
-        The iterable to search through.
-    """
-
-    for element in seq:
-        if predicate(element):
-            return element
-    return None
-
-
-def get(iterable, **attrs):
-    r"""A helper that returns the first element in the iterable that meets
-    all the traits passed in ``attrs``. This is an alternative for
-    :func:`moddb.utils.find`.
-
-    When multiple attributes are specified, they are checked using
-    logical AND, not logical OR. Meaning they have to meet every
-    attribute passed in and not one of them.
-
-    To have a nested attribute search (i.e. search by ``x.y``) then
-    pass in ``x__y`` as the keyword argument.
-
-    If nothing is found that matches the attributes passed, then
-    ``None`` is returned.
-
-    Examples
-    ---------
-
-    Basic usage:
-
-    .. code-block:: python3
-
-        article = moddb.utils.get(mod.get_articles(), name='Version 3.5 Released')
-
-    Multiple attribute matching:
-
-    .. code-block:: python3
-
-        comment = moddb.utils.get(mod.get_comments(2), content='Test', karma=3)
-
-    Nested attribute matching:
-
-    .. code-block:: python3
-
-        comment = moddb.utils.get(article.get_comments(), author__name='SilverElf', content='Best article ever')
-
-    Parameters
-    -----------
-    iterable
-        An iterable to search through.
-    \*\*attrs
-        Keyword arguments that denote attributes to search with.
-    """
-
-    def predicate(elem):
-        for attr, val in attrs.items():
-            nested = attr.split("__")
-            obj = elem
-            for attribute in nested:
-                obj = getattr(obj, attribute)
-
-            if obj != val:
-                return False
-        return True
-
-    return find(predicate, iterable)
-
-
-def generate_hash():
-    return uuid.uuid4().hex
+import datetime
+import inspect
+import logging
+import random
+import re
+import sys
+import uuid
+from typing import Tuple
+from urllib.parse import urljoin
+
+import bs4
+import requests
+from bs4 import BeautifulSoup, Tag
+from pyrate_limiter import Duration, Limiter, RequestRate
+
+from .enums import ThumbnailType
+from .errors import AwaitingAuthorisation, ModdbException
+
+LOGGER = logging.getLogger("moddb")
+BASE_URL = "https://www.moddb.com"
+LIMITER = Limiter(
+    # request stuff slowly, like a human
+    RequestRate(1, Duration.SECOND * 1),
+    # take breaks when requesting stuff, like a human
+    RequestRate(40, Duration.MINUTE * 5),
+)
+
+time_mapping = {
+    "year": 125798400,
+    "month": 2419200,
+    "week": 604800,
+    "day": 86400,
+    "hour": 3600,
+    "minute": 60,
+    "econd": 1,
+}
+
+user_agent_list = [
+    # Chrome
+    "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/60.0.3112.113 Safari/537.36",
+    "Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/60.0.3112.90 Safari/537.36",
+    "Mozilla/5.0 (Windows NT 5.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/60.0.3112.90 Safari/537.36",
+    "Mozilla/5.0 (Windows NT 6.2; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/60.0.3112.90 Safari/537.36",
+    "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/44.0.2403.157 Safari/537.36",
+    "Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/60.0.3112.113 Safari/537.36",
+    "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/57.0.2987.133 Safari/537.36",
+    "Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/57.0.2987.133 Safari/537.36",
+    "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/55.0.2883.87 Safari/537.36",
+    "Mozilla/5.0 (Windows NT 6.1; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/55.0.2883.87 Safari/537.36",
+    # Firefox
+    "Mozilla/4.0 (compatible; MSIE 9.0; Windows NT 6.1)",
+    "Mozilla/5.0 (Windows NT 6.1; WOW64; Trident/7.0; rv:11.0) like Gecko",
+    "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; WOW64; Trident/5.0)",
+    "Mozilla/5.0 (Windows NT 6.1; Trident/7.0; rv:11.0) like Gecko",
+    "Mozilla/5.0 (Windows NT 6.2; WOW64; Trident/7.0; rv:11.0) like Gecko",
+    "Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; rv:11.0) like Gecko",
+    "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.0; Trident/5.0)",
+    "Mozilla/5.0 (Windows NT 6.3; WOW64; Trident/7.0; rv:11.0) like Gecko",
+    "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; Trident/5.0)",
+    "Mozilla/5.0 (Windows NT 6.1; Win64; x64; Trident/7.0; rv:11.0) like Gecko",
+    "Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.1; WOW64; Trident/6.0)",
+    "Mozilla/5.0 (compatible; MSIE 10.0; Windows NT 6.1; Trident/6.0)",
+    "Mozilla/4.0 (compatible; MSIE 8.0; Windows NT 5.1; Trident/4.0; .NET CLR 2.0.50727; .NET CLR 3.0.4506.2152; .NET CLR 3.5.30729)",
+]
+
+
+def concat_docs(cls):
+    """Does it look like I'm enjoying this?"""
+    attributes = []
+
+    def get_docs(parent):
+        nonlocal attributes
+        if parent.__name__ == "object":
+            return
+
+        docs = parent.__doc__.splitlines()
+        if "    Attributes" in docs:
+            attributes = docs[docs.index("    Attributes") + 2 :] + attributes
+
+        source = inspect.getsource(parent.__init__)
+        source = source[source.index("):") :]
+
+        if "super().__init__" in source:
+            get_docs(parent.__base__)
+        elif "__init__" in source:
+            get_docs(parent.__base__.__base__)
+
+    get_docs(cls)
+    original = cls.__doc__.splitlines()
+    if "    Attributes" not in original:
+        original.append("    Attributes")
+        original.append("    -----------")
+
+    final = original[: original.index("    Attributes") + 2]
+    final.extend([x for x in attributes if x.strip()])
+    cls.__doc__ = "\n".join(final)
+
+    return cls
+
+
+def get_date(d: str) -> datetime.datetime:
+    """A helper function that takes a ModDB string representation of time and returns an equivalent
+    datetime.datetime object. This can range from a datetime with the full year to
+    second to just a year and a month.
+
+    Parameters
+    -----------
+    d : str
+        String representation of a datetime
+
+    Returns
+    -------
+    datetime.datetime
+        The datetime object for the given string
+    """
+    try:
+        return datetime.datetime.strptime(d[:-3] + d[-2:], "%Y-%m-%dT%H:%M:%S%z")
+    except ValueError:
+        pass
+
+    try:
+        return datetime.datetime.strptime(d, "%Y-%m-%d")
+    except ValueError:
+        pass
+
+    return datetime.datetime.strptime(d, "%Y-%m")
+
+
+def prepare_request(req: requests.Request, session):
+    """Prepared a request with the appropriate cookies"""
+    cookies = requests.utils.dict_from_cookiejar(session.cookies)
+
+    if req.cookies is not None:
+        req.cookies = {**req.cookies, **cookies}
+    else:
+        req.cookies = cookies
+
+    req.headers["User-Agent"] = random.choice(user_agent_list)
+
+    prepped = session.prepare_request(req)
+    return prepped
+
+
+def raise_for_status(response):
+    """Raise any error that could have occured"""
+    try:
+        text = response.json()
+        if text.get("error", False):
+            LOGGER.error(text["text"])
+            LOGGER.error(response.request.url)
+            LOGGER.error(response.request.body)
+            raise ModdbException(text["text"])
+    except requests.exceptions.JSONDecodeError:
+        response.raise_for_status()
+
+    if (
+        "is currently awaiting authorisation, which can take a couple of days while a"
+        in response.text.lower()
+    ):
+        raise AwaitingAuthorisation(
+            "This page is still await authorisation and cannot currently be parsed"
+        )
+
+
+def generate_login_cookies(username, password):
+    """Log a user in and return the `freeman` cookie containing the login hash"""
+    resp = requests.get(f"{BASE_URL}/members/login")
+    html = soup(resp.text)
+    form = html.find("form", attrs={"name": "membersform"})
+
+    username_input = form.find("input", id="membersusername")
+    botcatcher = form.find("input", type="text", id=False)
+
+    data = {
+        "referer": "",
+        username_input["name"]: username,
+        botcatcher["name"]: "",
+        "password": password,
+        "rememberme": ["1"],
+        "members": "Sign in",
+    }
+
+    login = requests.post(
+        f"{BASE_URL}/members/login",
+        data=data,
+        cookies=resp.cookies,
+        allow_redirects=False,
+    )
+
+    if "freeman" not in login.cookies:
+        raise ValueError(f"Login failed for user {username}")
+
+    return login.cookies
+
+
+@LIMITER.ratelimit("moddb", delay=True)
+def request(req: requests.Request):
+    """Helper function to make get/post requests with the current SESSION object.
+
+    Parameters
+    -----------
+    req : requests.Request
+        The request to perform
+
+    Return
+    -------
+    requests.Response
+        The returned response object
+
+    """
+    SESSION = sys.modules["moddb"].SESSION
+    prepped = prepare_request(req, SESSION)
+    r = SESSION.send(prepped)
+
+    raise_for_status(r)
+    return r
+
+
+def soup(html: str) -> BeautifulSoup:
+    """Simple helper function that takes a string representation of an html page and
+    returns a beautiful soup object"""
+
+    return BeautifulSoup(html, "html.parser")
+
+
+def get_page(url: str, *, params: dict = {}, json: bool = False):
+    """A helper function that takes a url and returns a beautiful soup objects. This is used to center
+    the request making section of the library. Can also be passed a set of paramaters, used for sorting
+    and filtering in the search function.
+
+    Parameters
+    -----------
+    url : str
+        The url to get
+    params : dict
+        A dictionnary of filters and sorting key-value pairs.
+    json : Optional[bool]
+        Whether the expected response is json, in which case it will not be soup'd
+
+    Returns
+    -------
+    bs4.BeautifulSoup
+    """
+    resp = request(requests.Request("GET", url, params=params))
+    if json:
+        return resp.json()
+
+    return soup(resp.text)
+
+
+def get_views(string: str) -> Tuple[int, int]:
+    """A helper function that takes a string reresentation of total something and
+    daily amount of that same thing and returns both as a tuple of ints.
+
+    Parameters
+    ------------
+    string : str
+        The string containing the numbers both total and daily
+
+    Returns
+    --------
+    Tuple[int, int]
+        Tuple contains the total views (first element) and the daily views (second element)
+    """
+    matches = re.search(r"^([0-9,]*) \(([0-9,]*) today\)$", string)
+    views = int(matches.group(1).replace(",", ""))
+    today = int(matches.group(2).replace(",", ""))
+
+    return views, today
+
+
+def join(path: str) -> str:
+    """Joins a partial moddb url with the base url and returns the combined url
+
+    Parameters
+    -----------
+    path : str
+        the url to join
+
+    Return
+    -------
+    str
+        The full url.
+
+    """
+    if not path.startswith(BASE_URL):
+        return urljoin(BASE_URL, path)
+
+    return path
+
+
+def normalize(string: str) -> str:
+    """Removes all extra fluff from a text to get the barebone content"""
+    return string.replace(",", "").replace("members", "").replace("member", "").strip()
+
+
+def get_media_type(img: Tag) -> int:
+    """Determines the type of the image through some very hacky stuff, might break"""
+    if img is None:
+        return 2
+    elif img["src"][-8:-5] == ".mp4":
+        return 0
+    else:
+        return 1
+
+
+def get_page_type(url: str) -> "ThumbnailType":
+    """Get the page type based on a url.
+
+    Parameters
+    -----------
+    url : str
+        The url to get
+
+    Return
+    -------
+    ThumbnailType
+        The type of the page
+    """
+    regex = r"\/((?!page|pages\b)\b\w+)\/"
+    type_mapping = {
+        "new": "article",
+        "feature": "article",
+        "tutorial": "article",
+        "download": "file",
+        "image": "media",
+        "audio": " media",
+        "video": "media",
+    }
+
+    matches = re.findall(regex, url)
+    match = matches[-1][0:-1] if matches[0].endswith("s") else matches[0]
+
+    try:
+        page_type = ThumbnailType[match]
+    except KeyError:
+        page_type = ThumbnailType[type_mapping[match]]
+
+    LOGGER.info("%s is type %s", url, page_type)
+    return page_type
+
+
+def ceildiv(a: int, b: int) -> int:
+    "Like a // b but rounded up instead of down."
+    return -(a // -b)
+
+
+def get_list_stats(result_box: bs4.BeautifulSoup, per_page: int = 30) -> Tuple[int, int, int]:
+    """Get the current page, total pages and total results from
+    a result list"""
+    stats = re.match(
+        r".*\(([0-9,]*) - ([0-9,]*) of ([0-9,]*)\)",
+        result_box.find("div", class_="normalcorner")
+        .find("div", class_="title")
+        .find("span", class_="heading")
+        .string,
+    )
+
+    if not stats:  # less than a page
+        return 1, 1, None
+
+    max_results = int(stats.group(2).replace(",", ""))
+    all_results = int(stats.group(3).replace(",", ""))
+    max_page = ceildiv(all_results, per_page)
+    current_page = ceildiv(max_results, per_page)
+
+    return current_page, max_page, all_results
+
+
+class Object:
+    """A dud objects that will transform every kwarg given into an attribute"""
+
+    def __init__(self, **kwargs):
+        self.__dict__.update(kwargs)
+
+
+def find(predicate, seq):
+    """A helper to return the first element found in the sequence
+    that meets the predicate. For example: ::
+
+        comment = find(lambda comment: comment.author.name == 'SilverElf', mod.comments.flatten())
+
+    would find the first :class:`.Comment` whose author's name is 'SilverElf' and return it.
+    If no entry is found, then ``None`` is returned.
+
+    This is different from `filter`_ due to the fact it stops the moment it finds
+    a valid entry.
+
+    .. _filter: https://docs.python.org/3.6/library/functions.html#filter
+
+    Parameters
+    -----------
+    predicate
+        A function that returns a boolean-like result.
+    seq : iterable
+        The iterable to search through.
+    """
+
+    for element in seq:
+        if predicate(element):
+            return element
+    return None
+
+
+def get(iterable, **attrs):
+    r"""A helper that returns the first element in the iterable that meets
+    all the traits passed in ``attrs``. This is an alternative for
+    :func:`moddb.utils.find`.
+
+    When multiple attributes are specified, they are checked using
+    logical AND, not logical OR. Meaning they have to meet every
+    attribute passed in and not one of them.
+
+    To have a nested attribute search (i.e. search by ``x.y``) then
+    pass in ``x__y`` as the keyword argument.
+
+    If nothing is found that matches the attributes passed, then
+    ``None`` is returned.
+
+    Examples
+    ---------
+
+    Basic usage:
+
+    .. code-block:: python3
+
+        article = moddb.utils.get(mod.get_articles(), name='Version 3.5 Released')
+
+    Multiple attribute matching:
+
+    .. code-block:: python3
+
+        comment = moddb.utils.get(mod.get_comments(2), content='Test', karma=3)
+
+    Nested attribute matching:
+
+    .. code-block:: python3
+
+        comment = moddb.utils.get(article.get_comments(), author__name='SilverElf', content='Best article ever')
+
+    Parameters
+    -----------
+    iterable
+        An iterable to search through.
+    \*\*attrs
+        Keyword arguments that denote attributes to search with.
+    """
+
+    def predicate(elem):
+        for attr, val in attrs.items():
+            nested = attr.split("__")
+            obj = elem
+            for attribute in nested:
+                obj = getattr(obj, attribute)
+
+            if obj != val:
+                return False
+        return True
+
+    return find(predicate, iterable)
+
+
+def generate_hash():
+    return uuid.uuid4().hex
+
+
+def get_sitearea(url: str) -> str:
+    """Get the site area from a url"""
+    return url.split("/")[-2]
+
+
+siteareaid_mapping = {
+    "3": "mods",
+    "2": "games",
+}
+
+
+def get_siteareaid(key: str):
+    """Get the sitearea id from an int"""
+    return siteareaid_mapping.get(str(key), "none")
```

### Comparing `moddb-0.8.1/moddb.egg-info/PKG-INFO` & `moddb-0.9.0/moddb.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,73 @@
-Metadata-Version: 2.1
-Name: moddb
-Version: 0.8.1
-Summary: A scrapper for ModDB Mod and Game pages
-Home-page: https://github.com/ClementJ18/moddb
-Author: Clement Julia
-Author-email: clement.julia13@gmail.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# ModDB Reader
-**Library is now stable**
-
-The goal of the library is to be able to navigate ModDB purely programmatically through scraping and parsing of the various models present on the website. This is based off a command of my bot which can parse either a game or a mod, this command gave birth to the original library which was extremely limited in its abilities and only able to parse a few pages with inconsistencies. This library is a much more mature and professional attempt at the whole idea, adding on a much deeper understanding of OOP.
-
-## Basic Usage
-The simplest way to use this library is to simply pass a ModDB url to the parse function and let the magic happen.
-```py
-import moddb
-mod = moddb.parse_page("http://www.moddb.com/mods/edain-mod")
-print(mod.name) #Edain Mod
-```
-The library tries to get the type of the url you are passing on its own but due to inconsistencies in the ModDB site this is not always correct, if you desire to be more specific you can pass a ThumbnailType to the function.
-```py
-import moddb
-mod = moddb.parse_page("http://www.moddb.com/mods/edain-mod", page_type=moddb.ThumbnailType.mod)
-print(mod.name) #Edain Mod
-```
-
-## Advanced Usage
-Check out the [documentation](https://moddb.readthedocs.io) for more information
-
-[Support](https://discord.gg/Ape8bZt)
-
-## Installing
-You can get it from pypi: https://pypi.org/project/moddb
-
-```
-pip install moddb
-```
-
-## Models
-* [x] Mod
-* [x] Game  
-* [x] Engine
-* [x] File
-* [x] Media
-* [x] Addon
-* [x] Article
-* [x] Blog
-* [x] User
-* [x] Team
-* [x] Group
-* [x] Job
-* [x] Search Page
-* [x] Front Page
-* [x] Platforms
-* [x] Software
-* [x] HardwAre
-* [x] Updates
-* [x] Friend Requests
-* [ ] Watchers
-* [ ] Tags
-
-Maybe
-* [ ] Messages
-* [ ] Threads
-
-## Glossary
-* **Partial[Model]**: A version of the model which does not contain all the attributes of the full model. Mainly because that model is being displayed as a preview in another page. Not to confuse with Thumbnails, Thumbnails are only guaranteed to contain a name and url of the page.
-* **Boxes**: Containers present on pages, a **div** tag which contains information around a certain theme and as such have been grouped into Box Models of such.
-* **Pages**: Another name for Models.
-* **Thumbnails**: A very widely used model meant to represent models which are references but not expanded onto. Usually the model in question will only include a url and the name of the page. This is transformed into a thumbnail and the user can then parse it with the built-in method.
-
-## Development
-requirement.txt file contains the necessary additional libraries for develompment
+Metadata-Version: 2.1
+Name: moddb
+Version: 0.9.0
+Summary: A scrapper for ModDB Mod and Game pages
+Home-page: https://github.com/ClementJ18/moddb
+Author: Clement Julia
+Author-email: clement.julia13@gmail.com
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# ModDB Reader
+**Library is now stable**
+
+The goal of the library is to be able to navigate ModDB purely programmatically through scraping and parsing of the various models present on the website. This is based off a command of my bot which can parse either a game or a mod, this command gave birth to the original library which was extremely limited in its abilities and only able to parse a few pages with inconsistencies. This library is a much more mature and professional attempt at the whole idea, adding on a much deeper understanding of OOP.
+
+## Basic Usage
+The simplest way to use this library is to simply pass a ModDB url to the parse function and let the magic happen.
+```py
+import moddb
+mod = moddb.parse_page("http://www.moddb.com/mods/edain-mod")
+print(mod.name) #Edain Mod
+```
+
+## Advanced Usage
+Check out the [documentation](https://moddb.readthedocs.io) for more information
+
+[Support](https://discord.gg/Ape8bZt)
+
+## Installing
+You can get it from pypi: https://pypi.org/project/moddb
+
+```
+pip install moddb
+```
+
+## Models
+* [x] Mod
+* [x] Game  
+* [x] Engine
+* [x] File
+* [x] Media
+* [x] Addon
+* [x] Article
+* [x] Blog
+* [x] User
+* [x] Team
+* [x] Group
+* [x] Job
+* [x] Search Page
+* [x] Front Page
+* [x] Platforms
+* [x] Software
+* [x] HardwAre
+* [x] Updates
+* [x] Friend Requests
+* [x] Watchers
+* [x] Tags
+
+Maybe
+* [ ] Messages
+* [ ] Threads
+
+## Glossary
+* **Partial[Model]**: A version of the model which does not contain all the attributes of the full model. Mainly because that model is being displayed as a preview in another page. Not to confuse with Thumbnails, Thumbnails are only guaranteed to contain a name and url of the page.
+* **Boxes**: Containers present on pages, a **div** tag which contains information around a certain theme and as such have been grouped into Box Models of such.
+* **Pages**: Another name for Models.
+* **Thumbnails**: A very widely used model meant to represent models which are references but not expanded onto. Usually the model in question will only include a url and the name of the page. This is transformed into a thumbnail and the user can then parse it with the built-in method.
+
+## Development
+The necessary dependencies are stored in requirements.txt and requirements-dev.txt and can be installed with the following command
+```
+python -m pip install -r requirements.txt -r requirements-dev.txt
+```
```

