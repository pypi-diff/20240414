# Comparing `tmp/libreppc-0.1.1.tar.gz` & `tmp/libreppc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreppc-0.1.1.tar", last modified: Sun Apr 14 16:07:30 2024, max compression
+gzip compressed data, was "libreppc-0.1.2.tar", last modified: Sun Apr 14 17:21:23 2024, max compression
```

## Comparing `libreppc-0.1.1.tar` & `libreppc-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 16:07:30.342728 libreppc-0.1.1/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1096 2024-02-23 10:09:06.000000 libreppc-0.1.1/LICENSE
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2164 2024-04-14 16:07:30.342728 libreppc-0.1.1/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1455 2024-04-14 16:06:12.000000 libreppc-0.1.1/README.md
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 16:07:30.339395 libreppc-0.1.1/libreppc/
--rw-r--r--   0 warlock   (1000) warlock   (1000)       48 2024-04-14 16:06:37.000000 libreppc-0.1.1/libreppc/__init__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)      705 2024-04-14 15:53:52.000000 libreppc-0.1.1/libreppc/__main__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     5427 2024-04-14 15:58:57.000000 libreppc-0.1.1/libreppc/libreppc.py
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 16:07:30.339395 libreppc-0.1.1/libreppc.egg-info/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2164 2024-04-14 16:07:30.000000 libreppc-0.1.1/libreppc.egg-info/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)      248 2024-04-14 16:07:30.000000 libreppc-0.1.1/libreppc.egg-info/SOURCES.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-04-14 16:07:30.000000 libreppc-0.1.1/libreppc.egg-info/dependency_links.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       28 2024-04-14 16:07:30.000000 libreppc-0.1.1/libreppc.egg-info/requires.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        9 2024-04-14 16:07:30.000000 libreppc-0.1.1/libreppc.egg-info/top_level.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-04-14 16:07:30.342728 libreppc-0.1.1/setup.cfg
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1070 2024-04-14 16:02:17.000000 libreppc-0.1.1/setup.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 17:21:23.791953 libreppc-0.1.2/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1096 2024-02-23 10:09:06.000000 libreppc-0.1.2/LICENSE
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-14 17:21:23.791953 libreppc-0.1.2/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1500 2024-04-14 17:20:23.000000 libreppc-0.1.2/README.md
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 17:21:23.791953 libreppc-0.1.2/libreppc/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       48 2024-04-14 17:16:50.000000 libreppc-0.1.2/libreppc/__init__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      705 2024-04-14 17:18:08.000000 libreppc-0.1.2/libreppc/__main__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     5531 2024-04-14 17:18:04.000000 libreppc-0.1.2/libreppc/libreppc.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 17:21:23.791953 libreppc-0.1.2/libreppc.egg-info/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-14 17:21:23.000000 libreppc-0.1.2/libreppc.egg-info/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      248 2024-04-14 17:21:23.000000 libreppc-0.1.2/libreppc.egg-info/SOURCES.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-04-14 17:21:23.000000 libreppc-0.1.2/libreppc.egg-info/dependency_links.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       28 2024-04-14 17:21:23.000000 libreppc-0.1.2/libreppc.egg-info/requires.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        9 2024-04-14 17:21:23.000000 libreppc-0.1.2/libreppc.egg-info/top_level.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-04-14 17:21:23.791953 libreppc-0.1.2/setup.cfg
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1070 2024-04-14 16:02:17.000000 libreppc-0.1.2/setup.py
```

### Comparing `libreppc-0.1.1/LICENSE` & `libreppc-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.1/PKG-INFO` & `libreppc-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreppc
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple profile page creator.
 Home-page: https://codeberg.org/librehub/libreppc
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,profile,html,css,markdown,profile page,page,site,personal page
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -26,23 +26,24 @@
 ![example](resources/example.png "Profile example")
 
 ## Installation
 
 ```sh
 $ pip install libreppc
 $ python -m libreppc --serve
-``
+```
 
 ## Getting started
 
 You need to create `config.json`:
 
 **config.json** structure
 ```json
 {
+    "theme" : "CSS_FILE_NAME_WITHOUT_.css",
     "avatar" : "https://avatar-url.com",
     "username" : "yourusername",
     "description" : "yourdescription",
     "base_url" : "yourpageurl",
     "blog_dir" : "blog",
     "blog_title" : "Blog",
     "links" : [
```

### Comparing `libreppc-0.1.1/README.md` & `libreppc-0.1.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 ![example](resources/example.png "Profile example")
 
 ## Installation
 
 ```sh
 $ pip install libreppc
 $ python -m libreppc --serve
-``
+```
 
 ## Getting started
 
 You need to create `config.json`:
 
 **config.json** structure
 ```json
 {
+    "theme" : "CSS_FILE_NAME_WITHOUT_.css",
     "avatar" : "https://avatar-url.com",
     "username" : "yourusername",
     "description" : "yourdescription",
     "base_url" : "yourpageurl",
     "blog_dir" : "blog",
     "blog_title" : "Blog",
     "links" : [
```

### Comparing `libreppc-0.1.1/libreppc/__main__.py` & `libreppc-0.1.2/libreppc/__main__.py`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.1/libreppc/libreppc.py` & `libreppc-0.1.2/libreppc/libreppc.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,17 @@
     current_dir = os.path.dirname(__file__)
 
     def __init__(self, app) -> None:
         self.app = app
         self.data = json.load(open("config.json"))
         self.load_blog_previews()
 
+        if not 'theme' in self.data.keys():
+            self.data['theme'] = 'mastodon'
+
     def render_main(self) -> str:
         render = render_template("index.html", **self.data)
         render = render.replace("&lt;", "<")
         render = render.replace("&gt;", ">")
         return render
 
     def render_post(self, postId: str) -> str:
@@ -147,9 +150,9 @@
                     file.write(self.render_post(postId))
 
         print("Generate rss...")
         fg = self.generate_rss()
         fg.atom_file("build/static/feed.atom")
 
         print("Copy styles...")
-        shutil.copy(f"{self.current_dir}/static/style.css", "build/static/style.css")
+        shutil.copy(f"{self.current_dir}/static/{self.data['theme']}.css", "build/static/style.css")
         print("Complete building!")
```

### Comparing `libreppc-0.1.1/libreppc.egg-info/PKG-INFO` & `libreppc-0.1.2/libreppc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreppc
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple profile page creator.
 Home-page: https://codeberg.org/librehub/libreppc
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,profile,html,css,markdown,profile page,page,site,personal page
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
@@ -26,23 +26,24 @@
 ![example](resources/example.png "Profile example")
 
 ## Installation
 
 ```sh
 $ pip install libreppc
 $ python -m libreppc --serve
-``
+```
 
 ## Getting started
 
 You need to create `config.json`:
 
 **config.json** structure
 ```json
 {
+    "theme" : "CSS_FILE_NAME_WITHOUT_.css",
     "avatar" : "https://avatar-url.com",
     "username" : "yourusername",
     "description" : "yourdescription",
     "base_url" : "yourpageurl",
     "blog_dir" : "blog",
     "blog_title" : "Blog",
     "links" : [
```

### Comparing `libreppc-0.1.1/setup.py` & `libreppc-0.1.2/setup.py`

 * *Files identical despite different names*

