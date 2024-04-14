# Comparing `tmp/libreppc-0.1.2.tar.gz` & `tmp/libreppc-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libreppc-0.1.2.tar", last modified: Sun Apr 14 17:21:23 2024, max compression
+gzip compressed data, was "libreppc-0.1.3.tar", last modified: Sun Apr 14 17:32:30 2024, max compression
```

## Comparing `libreppc-0.1.2.tar` & `libreppc-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 17:21:23.791953 libreppc-0.1.2/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1096 2024-02-23 10:09:06.000000 libreppc-0.1.2/LICENSE
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-14 17:21:23.791953 libreppc-0.1.2/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1500 2024-04-14 17:20:23.000000 libreppc-0.1.2/README.md
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 17:21:23.791953 libreppc-0.1.2/libreppc/
--rw-r--r--   0 warlock   (1000) warlock   (1000)       48 2024-04-14 17:16:50.000000 libreppc-0.1.2/libreppc/__init__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)      705 2024-04-14 17:18:08.000000 libreppc-0.1.2/libreppc/__main__.py
--rw-r--r--   0 warlock   (1000) warlock   (1000)     5531 2024-04-14 17:18:04.000000 libreppc-0.1.2/libreppc/libreppc.py
-drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 17:21:23.791953 libreppc-0.1.2/libreppc.egg-info/
--rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-14 17:21:23.000000 libreppc-0.1.2/libreppc.egg-info/PKG-INFO
--rw-r--r--   0 warlock   (1000) warlock   (1000)      248 2024-04-14 17:21:23.000000 libreppc-0.1.2/libreppc.egg-info/SOURCES.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-04-14 17:21:23.000000 libreppc-0.1.2/libreppc.egg-info/dependency_links.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       28 2024-04-14 17:21:23.000000 libreppc-0.1.2/libreppc.egg-info/requires.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)        9 2024-04-14 17:21:23.000000 libreppc-0.1.2/libreppc.egg-info/top_level.txt
--rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-04-14 17:21:23.791953 libreppc-0.1.2/setup.cfg
--rw-r--r--   0 warlock   (1000) warlock   (1000)     1070 2024-04-14 16:02:17.000000 libreppc-0.1.2/setup.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 17:32:30.261845 libreppc-0.1.3/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1096 2024-02-23 10:09:06.000000 libreppc-0.1.3/LICENSE
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-14 17:32:30.261845 libreppc-0.1.3/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1500 2024-04-14 17:20:23.000000 libreppc-0.1.3/README.md
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 17:32:30.261845 libreppc-0.1.3/libreppc/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       48 2024-04-14 17:31:42.000000 libreppc-0.1.3/libreppc/__init__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      705 2024-04-14 17:18:08.000000 libreppc-0.1.3/libreppc/__main__.py
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     5555 2024-04-14 17:31:16.000000 libreppc-0.1.3/libreppc/libreppc.py
+drwxr-xr-x   0 warlock   (1000) warlock   (1000)        0 2024-04-14 17:32:30.261845 libreppc-0.1.3/libreppc.egg-info/
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     2209 2024-04-14 17:32:30.000000 libreppc-0.1.3/libreppc.egg-info/PKG-INFO
+-rw-r--r--   0 warlock   (1000) warlock   (1000)      248 2024-04-14 17:32:30.000000 libreppc-0.1.3/libreppc.egg-info/SOURCES.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        1 2024-04-14 17:32:30.000000 libreppc-0.1.3/libreppc.egg-info/dependency_links.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       28 2024-04-14 17:32:30.000000 libreppc-0.1.3/libreppc.egg-info/requires.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)        9 2024-04-14 17:32:30.000000 libreppc-0.1.3/libreppc.egg-info/top_level.txt
+-rw-r--r--   0 warlock   (1000) warlock   (1000)       38 2024-04-14 17:32:30.261845 libreppc-0.1.3/setup.cfg
+-rw-r--r--   0 warlock   (1000) warlock   (1000)     1070 2024-04-14 16:02:17.000000 libreppc-0.1.3/setup.py
```

### Comparing `libreppc-0.1.2/LICENSE` & `libreppc-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.2/PKG-INFO` & `libreppc-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreppc
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple profile page creator.
 Home-page: https://codeberg.org/librehub/libreppc
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,profile,html,css,markdown,profile page,page,site,personal page
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `libreppc-0.1.2/README.md` & `libreppc-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.2/libreppc/__main__.py` & `libreppc-0.1.3/libreppc/__main__.py`

 * *Files identical despite different names*

### Comparing `libreppc-0.1.2/libreppc/libreppc.py` & `libreppc-0.1.3/libreppc/libreppc.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         blog_dir = self.data['blog_dir']
         postId = postId.replace('.html', '')
         with open(f'{blog_dir}/{postId}.md') as file:
             text = file.read()
 
         html = markdown.markdown(text, extensions=['fenced_code', 'nl2br', 'tables'])
         data = self.data.copy()
-        data['post'] = self.make_post_dict(postId, html) 
+        data['post'] = self.make_post_dict(postId, html)
 
         render = render_template("post.html", **data)
         render = render.replace("&lt;", "<")
         render = render.replace("&gt;", ">")
         return render
 
     def generate_rss(self) -> FeedGenerator:
@@ -150,9 +150,10 @@
                     file.write(self.render_post(postId))
 
         print("Generate rss...")
         fg = self.generate_rss()
         fg.atom_file("build/static/feed.atom")
 
         print("Copy styles...")
-        shutil.copy(f"{self.current_dir}/static/{self.data['theme']}.css", "build/static/style.css")
+        theme = self.data['theme']
+        shutil.copy(f"{self.current_dir}/static/{theme}.css", f"build/static/{theme}.css")
         print("Complete building!")
```

### Comparing `libreppc-0.1.2/libreppc.egg-info/PKG-INFO` & `libreppc-0.1.3/libreppc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libreppc
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple profile page creator.
 Home-page: https://codeberg.org/librehub/libreppc
 Author: loliconshik3
 Author-email: loliconshik3@gmail.com
 Keywords: python,profile,html,css,markdown,profile page,page,site,personal page
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `libreppc-0.1.2/setup.py` & `libreppc-0.1.3/setup.py`

 * *Files identical despite different names*

