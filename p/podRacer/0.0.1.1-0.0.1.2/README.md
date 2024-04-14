# Comparing `tmp/podRacer-0.0.1.1.tar.gz` & `tmp/podRacer-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podRacer-0.0.1.1.tar", last modified: Fri Nov 10 22:28:15 2023, max compression
+gzip compressed data, was "podRacer-0.0.1.2.tar", last modified: Sun Apr 14 04:39:09 2024, max compression
```

## Comparing `podRacer-0.0.1.1.tar` & `podRacer-0.0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 afshari    (501) staff       (20)        0 2023-11-10 22:28:15.761828 podRacer-0.0.1.1/
--rw-r--r--   0 afshari    (501) staff       (20)      724 2023-11-10 22:28:15.761703 podRacer-0.0.1.1/PKG-INFO
--rw-r--r--   0 afshari    (501) staff       (20)      338 2023-11-10 20:02:44.000000 podRacer-0.0.1.1/README.md
-drwxr-xr-x   0 afshari    (501) staff       (20)        0 2023-11-10 22:28:15.760939 podRacer-0.0.1.1/podRacer/
--rw-r--r--   0 afshari    (501) staff       (20)      168 2023-11-10 20:34:17.000000 podRacer-0.0.1.1/podRacer/__init__.py
--rw-r--r--   0 afshari    (501) staff       (20)     2004 2023-11-10 20:02:44.000000 podRacer-0.0.1.1/podRacer/_appdata.py
--rw-r--r--   0 afshari    (501) staff       (20)     3780 2023-11-10 22:10:29.000000 podRacer-0.0.1.1/podRacer/download.py
--rw-r--r--   0 afshari    (501) staff       (20)     7113 2023-11-10 20:31:47.000000 podRacer-0.0.1.1/podRacer/download_queue.py
--rw-r--r--   0 afshari    (501) staff       (20)     8799 2023-11-10 20:02:44.000000 podRacer-0.0.1.1/podRacer/organize.py
--rw-r--r--   0 afshari    (501) staff       (20)     7406 2023-11-10 20:31:36.000000 podRacer-0.0.1.1/podRacer/process.py
--rw-r--r--   0 afshari    (501) staff       (20)     2766 2023-11-10 20:02:44.000000 podRacer-0.0.1.1/podRacer/settings.py
-drwxr-xr-x   0 afshari    (501) staff       (20)        0 2023-11-10 22:28:15.761450 podRacer-0.0.1.1/podRacer.egg-info/
--rw-r--r--   0 afshari    (501) staff       (20)      724 2023-11-10 22:28:15.000000 podRacer-0.0.1.1/podRacer.egg-info/PKG-INFO
--rw-r--r--   0 afshari    (501) staff       (20)      329 2023-11-10 22:28:15.000000 podRacer-0.0.1.1/podRacer.egg-info/SOURCES.txt
--rw-r--r--   0 afshari    (501) staff       (20)        1 2023-11-10 22:28:15.000000 podRacer-0.0.1.1/podRacer.egg-info/dependency_links.txt
--rw-r--r--   0 afshari    (501) staff       (20)      155 2023-11-10 22:28:15.000000 podRacer-0.0.1.1/podRacer.egg-info/requires.txt
--rw-r--r--   0 afshari    (501) staff       (20)        9 2023-11-10 22:28:15.000000 podRacer-0.0.1.1/podRacer.egg-info/top_level.txt
--rw-r--r--   0 afshari    (501) staff       (20)       38 2023-11-10 22:28:15.761869 podRacer-0.0.1.1/setup.cfg
--rw-r--r--   0 afshari    (501) staff       (20)      717 2023-11-10 22:27:47.000000 podRacer-0.0.1.1/setup.py
+drwxr-xr-x   0 afshari    (501) staff       (20)        0 2024-04-14 04:39:09.145781 podRacer-0.0.1.2/
+-rw-r--r--   0 afshari    (501) staff       (20)      724 2024-04-14 04:39:09.145672 podRacer-0.0.1.2/PKG-INFO
+-rw-r--r--   0 afshari    (501) staff       (20)      338 2023-11-10 20:02:44.000000 podRacer-0.0.1.2/README.md
+drwxr-xr-x   0 afshari    (501) staff       (20)        0 2024-04-14 04:39:09.144941 podRacer-0.0.1.2/podRacer/
+-rw-r--r--   0 afshari    (501) staff       (20)      168 2023-11-10 20:34:17.000000 podRacer-0.0.1.2/podRacer/__init__.py
+-rw-r--r--   0 afshari    (501) staff       (20)     1529 2024-04-11 20:45:55.000000 podRacer-0.0.1.2/podRacer/_appdata.py
+-rw-r--r--   0 afshari    (501) staff       (20)     9101 2024-04-11 23:28:14.000000 podRacer-0.0.1.2/podRacer/download.py
+-rw-r--r--   0 afshari    (501) staff       (20)     9648 2024-04-11 23:28:30.000000 podRacer-0.0.1.2/podRacer/download_queue.py
+-rw-r--r--   0 afshari    (501) staff       (20)     9966 2024-04-11 23:28:35.000000 podRacer-0.0.1.2/podRacer/organize.py
+-rw-r--r--   0 afshari    (501) staff       (20)     7134 2024-04-11 23:28:45.000000 podRacer-0.0.1.2/podRacer/process.py
+-rw-r--r--   0 afshari    (501) staff       (20)     2766 2023-11-10 20:02:44.000000 podRacer-0.0.1.2/podRacer/settings.py
+drwxr-xr-x   0 afshari    (501) staff       (20)        0 2024-04-14 04:39:09.145520 podRacer-0.0.1.2/podRacer.egg-info/
+-rw-r--r--   0 afshari    (501) staff       (20)      724 2024-04-14 04:39:08.000000 podRacer-0.0.1.2/podRacer.egg-info/PKG-INFO
+-rw-r--r--   0 afshari    (501) staff       (20)      329 2024-04-14 04:39:09.000000 podRacer-0.0.1.2/podRacer.egg-info/SOURCES.txt
+-rw-r--r--   0 afshari    (501) staff       (20)        1 2024-04-14 04:39:08.000000 podRacer-0.0.1.2/podRacer.egg-info/dependency_links.txt
+-rw-r--r--   0 afshari    (501) staff       (20)      155 2024-04-14 04:39:09.000000 podRacer-0.0.1.2/podRacer.egg-info/requires.txt
+-rw-r--r--   0 afshari    (501) staff       (20)        9 2024-04-14 04:39:09.000000 podRacer-0.0.1.2/podRacer.egg-info/top_level.txt
+-rw-r--r--   0 afshari    (501) staff       (20)       38 2024-04-14 04:39:09.145816 podRacer-0.0.1.2/setup.cfg
+-rw-r--r--   0 afshari    (501) staff       (20)      717 2024-04-14 04:10:07.000000 podRacer-0.0.1.2/setup.py
```

### Comparing `podRacer-0.0.1.1/PKG-INFO` & `podRacer-0.0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podRacer
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: A library for interacting with podcasts
 Author: Mike Afshari
 Author-email: theneed4swede@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: podRacer Version: 0.0.1.1 Summary: A library for
+Metadata-Version: 2.1 Name: podRacer Version: 0.0.1.2 Summary: A library for
 interacting with podcasts Author: Mike Afshari Author-email:
 theneed4swede@gmail.com License: MIT Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown
                           **Now this is podRacing!**
     ______________________________________________________________________
```

### Comparing `podRacer-0.0.1.1/podRacer/download_queue.py` & `podRacer-0.0.1.2/podRacer/download_queue.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,16 +10,16 @@
         import requests                                     # handles various web requests
         from tqdm import tqdm                               # handles progress bars for various operations
 
     if 'Local File':
         from .organize import Organize                       # podRacer lib - handles various organization tasks
         from .settings import Settings                       # podRacer lib - handles lib usage settings, such as error logging
 
-## HANDLES WORKER FUNCTIONS
-class Queue:
+## DOWNLOAD QUEUE FOR PODCAST AUDIO FILES
+class AudioQueue:
 
     ## INITIALIZE THE QUEUE WITH A NUMBER OF WORKERS
     def __init__(self, max_workers=1):
 
         ## INIT CLASSES
         self.organize = Organize()
         self.settings = Settings()
@@ -185,7 +185,81 @@
         ## WAIT FOR EACH FUTURE TO COMPLETE AND UPDATE PROGRESS BAR
         for future in as_completed(self.futures):
             result = future.result()  # OPTIONAL: HANDLE RESULT
             progress_bar.update(1)
 
         ## CLOSE THE PROGRESS BAR ONCE ALL DOWNLOADS ARE COMPLETE
         progress_bar.close()
+
+## GENERAL DOWNLOAD QUEUE
+class Queue:
+
+    ## INITIALIZE THE QUEUE WITH A NUMBER OF WORKERS
+    def __init__(self, max_workers=1):
+
+        ## INIT CLASSES
+        self.organize = Organize()
+        self.settings = Settings()
+
+        ## CREATE A THREAD POOL EXECUTOR
+        self.executor = ThreadPoolExecutor(max_workers=max_workers)
+
+        ## INITIALIZE A LIST TO TRACK FUTURE DOWNLOAD TASKS
+        self.futures = []
+
+    ## DOWNLOAD AN INDIVIDUAL FILE
+    def start(self, url, path):
+
+        ## ATTEMPT DOWNLOAD
+        try:
+
+            ## DOWNLOAD THE FILE
+            response = requests.get(url, stream=True)
+            with open(path, 'wb') as f:
+                for chunk in response.iter_content(chunk_size=1024):
+                    if chunk:
+                        f.write(chunk)
+
+            ## RETURN DOWNLOADED FILENAME
+            if os.path.getsize(path) > 0:
+                return str(url).split('/')[-1]
+            else:
+                self.settings.error("Download completed, but file is empty!",
+                        "Could happen if the download link wasn't parsed correctly, or if the server is unresponsive",
+                        path,
+                        "Title of the downloaded file",
+                        "Try running 'podRacer.Process.request()' and verify server response and check the links")
+                return None
+
+        ## HANDLE EXCEPTIONS
+        except Exception as error:
+            self.settings.error(error,
+                    caught_input=f"-",
+                message="Try running 'podRacer.Process.request()' and verify server response and check the links")
+            return None
+
+    ## ADD DOWNLOAD TO THE QUEUE
+    def add(self, url, path):
+
+        ## SUBMIT A DOWNLOAD TASK TO THE EXECUTOR
+        future = self.executor.submit(self.start, url, path)
+
+        ## APPEND THE FUTURE TO THE TRACKING LIST
+        self.futures.append(future)
+
+    ## DOWNLOAD PROGRESS BAR
+    def progress_bar(self, total_files, desc):
+
+        ## INITIALIZE A PROGRESS BAR
+        progress_bar = tqdm(
+            total=total_files,
+            desc="\033[1;33m" + desc + "\033[0m",  # Yellow and bold text
+            unit="ep"
+        )
+
+        ## WAIT FOR EACH FUTURE TO COMPLETE AND UPDATE PROGRESS BAR
+        for future in as_completed(self.futures):
+            result = future.result()  # OPTIONAL: HANDLE RESULT
+            progress_bar.update(1)
+
+        ## CLOSE THE PROGRESS BAR ONCE ALL DOWNLOADS ARE COMPLETE
+        progress_bar.close()
```

### Comparing `podRacer-0.0.1.1/podRacer/organize.py` & `podRacer-0.0.1.2/podRacer/organize.py`

 * *Files 10% similar despite different names*

```diff
@@ -75,22 +75,52 @@
                     base_dir.mkdir(parents=True, exist_ok=True)
                     create_sub_dirs(base_dir)
 
             ## ERROR
             else:
                 raise ValueError("The path and name of directories must be either both strings or both lists with the same length.")
 
-        def dir_paths(self, dir_path):
+        def dir_paths(self, dir_path, *create_dirs):
 
+            ## INITIALIZE DICTIONARY
             dir_paths = {}
 
+            ## ROOT DIRECTORY
             dir_paths['root'] = dir_path
+
+            ## MAIN SUBDIRECTORIES
             dir_paths['audio'] = os.path.join(dir_path, 'audio')
+            dir_paths['images'] = os.path.join(dir_path, 'images')
             dir_paths['metadata'] = os.path.join(dir_path, 'metadata')
 
+            ## METADATA SUBDIRECTORIES
+            dir_paths['links'] = os.path.join(dir_paths['metadata'], 'links')
+
+            ## CHECK IF CREATION ARGS ARE PROVIDED
+            if create_dirs:
+
+                ## INITIALIZE SET
+                dirs_to_create = set()
+
+                ## HANDLE BOTH LISTS AND SINGLE STRING ARGUMENTS
+                flattened_args = [item for sublist in create_dirs for item in (sublist if isinstance(sublist, list) else [sublist])]
+
+                ## CHECK IF ALL DIRECTORIES SHOULD BE CREATED
+                if 'all' in flattened_args:
+                    dirs_to_create = dir_paths.values()
+
+                ## CREATE SPECIFIC DIRECTORIES
+                else:
+                    dirs_to_create = {dir_paths[arg] for arg in flattened_args if arg in dir_paths}
+
+                ## CREATE DIRECTORIES
+                for path in dirs_to_create:
+                    os.makedirs(path, exist_ok=True)
+
+            ## RETURN DICTIONARY
             return dir_paths
 
     if 'Lists':
 
         ## GENERATES A FLAT LIST OF EPISODES TO DOWNLOAD
         def list_episodes_to_download(self, episode_args, total_episodes):
 
@@ -216,15 +246,15 @@
 
         ## REPLACE SPACES WITH UNDERSCORE
         def text_replace_spaces(self, text):
             return str(text).replace(' ', '_')
 
         ## REMOVES SPECIAL CHARACTERS AND DOUBLE SPACES
         def text_remove_specials(self, text):
-            text = re.sub(r"[^a-zA-Z0-9\s']", '', text)
+            text = re.sub(r'[^\w\s]', '', text, flags=re.UNICODE)
             text = re.sub(r'\s+', ' ', text).strip()
             return text
 
         ## STRIPS HTML TAGS FROM TEXT
         def text_strip_tags(self, text):
 
             ## PREVENT CDATA CONTENT FROM BEING STRIPPED
```

### Comparing `podRacer-0.0.1.1/podRacer/process.py` & `podRacer-0.0.1.2/podRacer/process.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,26 +8,32 @@
 
     if 'External Dependancy':
         import validators                   # validates links to see if they're valid URL's
 
     if 'Local File':
         from ._appdata import *                    # stores local application data, like global variables
         from .organize import Organize       # podRacer lib - handles various organization tasks
+        from .settings import Settings       # podRacer lib - handles lib usage settings, such as error logging
 
 ## HANDLES FETCH REQUESTS
 class Process:
 
     ## INITIALIZE CLASS
     def __init__(self):
         self.organize = Organize()
+        self.settings = Settings()
 
     ## PARSES RSS FEED
     def parse_feed(self, feed):
         if validators.url(feed):
-            return feedparser.parse(feed)
+            rss_feed = feedparser.parse(feed)
+            if rss_feed['bozo']:
+                self.settings.error("Invalid 'feed'", "The URL is either invalid or unreachable", f"{feed}", "https://rss.nytimes.com/services/xml/rss/nyt/US.xml")
+                return None
+            return rss_feed
         elif str(feed).endswith(('.xml', '.rss')):
             with open(feed, 'r', encoding='utf-8') as file:
                 content = file.read()
             return feedparser.parse(content)
         else:
             return None
 
@@ -141,53 +147,36 @@
 
         ## RETURN LIST
         return episodes
 
     ## GETS THE DATE OF THE MOST RECENT EPISODE
     def get_latest_episode_date(self, feed):
 
-        ## INITIALIZE LATEST_PUB_DATE AS EARLY AS POSSIBLE
-        latest_pub_date = datetime.min
+        ## INITIALIZE LATEST PUB DATE
+        latest_pub_date = None
 
         ## ITERATE THROUGH FEED ENTRIES
         for entry in feed.entries:
 
-            ## CHECK IF 'PUBLISHED_PARSED' IS AVAILABLE AND USE IT
-            if 'published_parsed' in entry:
-                pub_date = datetime(*entry.published_parsed[:6])
-
-            ## OTHERWISE, TRY TO PARSE 'PUBDATE' MANUALLY
-            elif 'pubDate' in entry:
-
-                ## TRY TO PARSE THE PUBDATE STRING TO A DATETIME OBJECT
+            ## TRY TO PARSE 'PUBDATE'
+            if 'pubDate' in entry:
                 try:
-                    pub_date = datetime.strptime(entry.pubDate, '%a, %d %b %Y %H:%M:%S %z')
-
-                ## IF PARSING FAILS, CONTINUE TO THE NEXT ENTRY
-                except ValueError:
-                    continue
-
-            ## IF NO VALID DATE IS FOUND, CONTINUE TO THE NEXT ENTRY
-            else:
-                continue
+                    latest_pub_date = datetime.strptime(entry.pubDate, '%a, %d %b %Y %H:%M:%S %z')
+                except (TypeError, ValueError):
+                    pass
 
-            ## UPDATE THE LATEST_PUB_DATE IF THIS ENTRY IS MORE RECENT
-            if pub_date > latest_pub_date:
-                latest_pub_date = pub_date
-
-        ## IF LATEST_PUB_DATE IS STILL DATETIME.MIN, NO VALID DATES WERE FOUND
-        if latest_pub_date == datetime.min:
-            latest_episode = 'Unknown'
-
-        ## OTHERWISE, FORMAT LATEST_PUB_DATE AS A STRING
-        else:
-            latest_episode = latest_pub_date.strftime('%a, %d %b %Y %H:%M:%S %z')
+            ## OTHERWISE, TRY TO PARSE 'PUBLISHED'
+            if not latest_pub_date and 'published' in entry:
+                try:
+                    latest_pub_date = entry.published
+                except (TypeError, ValueError):
+                    pass
 
         ## RETURN LATEST EPISODE DATE
-        return latest_episode
+        return latest_pub_date
 
     ## RETURNS LIST OF EPISODE LINKS
     def get_episode_links(self, feed):
 
         ## INITIALIZE LIST
         links = []
```

### Comparing `podRacer-0.0.1.1/podRacer/settings.py` & `podRacer-0.0.1.2/podRacer/settings.py`

 * *Files identical despite different names*

### Comparing `podRacer-0.0.1.1/podRacer.egg-info/PKG-INFO` & `podRacer-0.0.1.2/podRacer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podRacer
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: A library for interacting with podcasts
 Author: Mike Afshari
 Author-email: theneed4swede@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: podRacer Version: 0.0.1.1 Summary: A library for
+Metadata-Version: 2.1 Name: podRacer Version: 0.0.1.2 Summary: A library for
 interacting with podcasts Author: Mike Afshari Author-email:
 theneed4swede@gmail.com License: MIT Classifier: Programming Language :: Python
 :: 3 Classifier: License :: OSI Approved :: MIT License Classifier: Operating
 System :: OS Independent Requires-Python: >=3.6 Description-Content-Type: text/
 markdown
                           **Now this is podRacing!**
     ______________________________________________________________________
```

### Comparing `podRacer-0.0.1.1/setup.py` & `podRacer-0.0.1.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='podRacer',
-    version='0.0.1.1',
+    version='0.0.1.2',
     author='Mike Afshari',
     author_email='theneed4swede@gmail.com',
     description='A library for interacting with podcasts',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
     classifiers=[
```

