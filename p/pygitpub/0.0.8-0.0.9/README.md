# Comparing `tmp/pygitpub-0.0.8.tar.gz` & `tmp/pygitpub-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygitpub-0.0.8.tar", last modified: Thu Apr 28 00:20:09 2022, max compression
+gzip compressed data, was "pygitpub-0.0.9.tar", last modified: Thu Apr 28 00:24:02 2022, max compression
```

## Comparing `pygitpub-0.0.8.tar` & `pygitpub-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-04-28 00:20:09.144742 pygitpub-0.0.8/
--rw-r--r--   0 mark      (1000) mark      (1000)       25 2022-04-27 02:39:16.000000 pygitpub-0.0.8/MANIFEST.in
--rw-r--r--   0 mark      (1000) mark      (1000)     1293 2022-04-28 00:20:09.144742 pygitpub-0.0.8/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      315 2022-04-28 00:19:49.000000 pygitpub-0.0.8/README.rst
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-04-28 00:20:09.143742 pygitpub-0.0.8/pygitpub/
--rw-r--r--   0 mark      (1000) mark      (1000)       25 2022-04-27 23:11:28.000000 pygitpub-0.0.8/pygitpub/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)      357 2022-04-27 23:53:55.000000 pygitpub-0.0.8/pygitpub/configs.py
--rw-r--r--   0 mark      (1000) mark      (1000)     3008 2022-04-28 00:19:28.000000 pygitpub-0.0.8/pygitpub/main.py
--rw-r--r--   0 mark      (1000) mark      (1000)      172 2022-04-28 00:19:49.000000 pygitpub-0.0.8/pygitpub/static.py
--rw-r--r--   0 mark      (1000) mark      (1000)      587 2022-04-28 00:03:01.000000 pygitpub-0.0.8/pygitpub/utils.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-04-28 00:20:09.144742 pygitpub-0.0.8/pygitpub.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)     1293 2022-04-28 00:20:09.000000 pygitpub-0.0.8/pygitpub.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      330 2022-04-28 00:20:09.000000 pygitpub-0.0.8/pygitpub.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2022-04-28 00:20:09.000000 pygitpub-0.0.8/pygitpub.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       49 2022-04-28 00:20:09.000000 pygitpub-0.0.8/pygitpub.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       27 2022-04-28 00:20:09.000000 pygitpub-0.0.8/pygitpub.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        9 2022-04-28 00:20:09.000000 pygitpub-0.0.8/pygitpub.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       67 2022-04-28 00:20:09.144742 pygitpub-0.0.8/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)     1481 2022-04-28 00:19:49.000000 pygitpub-0.0.8/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-04-28 00:24:02.810986 pygitpub-0.0.9/
+-rw-r--r--   0 mark      (1000) mark      (1000)       25 2022-04-27 02:39:16.000000 pygitpub-0.0.9/MANIFEST.in
+-rw-r--r--   0 mark      (1000) mark      (1000)     1293 2022-04-28 00:24:02.810986 pygitpub-0.0.9/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      315 2022-04-28 00:23:34.000000 pygitpub-0.0.9/README.rst
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-04-28 00:24:02.809986 pygitpub-0.0.9/pygitpub/
+-rw-r--r--   0 mark      (1000) mark      (1000)       25 2022-04-27 23:11:28.000000 pygitpub-0.0.9/pygitpub/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      357 2022-04-27 23:53:55.000000 pygitpub-0.0.9/pygitpub/configs.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     3345 2022-04-28 00:23:18.000000 pygitpub-0.0.9/pygitpub/main.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      172 2022-04-28 00:23:34.000000 pygitpub-0.0.9/pygitpub/static.py
+-rw-r--r--   0 mark      (1000) mark      (1000)      587 2022-04-28 00:03:01.000000 pygitpub-0.0.9/pygitpub/utils.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-04-28 00:24:02.810986 pygitpub-0.0.9/pygitpub.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)     1293 2022-04-28 00:24:02.000000 pygitpub-0.0.9/pygitpub.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      330 2022-04-28 00:24:02.000000 pygitpub-0.0.9/pygitpub.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2022-04-28 00:24:02.000000 pygitpub-0.0.9/pygitpub.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       49 2022-04-28 00:24:02.000000 pygitpub-0.0.9/pygitpub.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       27 2022-04-28 00:24:02.000000 pygitpub-0.0.9/pygitpub.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        9 2022-04-28 00:24:02.000000 pygitpub-0.0.9/pygitpub.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       67 2022-04-28 00:24:02.810986 pygitpub-0.0.9/setup.cfg
+-rw-r--r--   0 mark      (1000) mark      (1000)     1481 2022-04-28 00:23:34.000000 pygitpub-0.0.9/setup.py
```

### Comparing `pygitpub-0.0.8/PKG-INFO` & `pygitpub-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygitpub
-Version: 0.0.8
+Version: 0.0.9
 Summary: help you work with github
 Home-page: https://veltzer.github.io/pygitpub
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
@@ -19,15 +19,15 @@
         
         .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
         
         project website: https://veltzer.github.io/pygitpub
         
         author: Mark Veltzer
         
-        version: 0.0.8
+        version: 0.0.9
         
         
         
 Keywords: github,pygithub
 Platform: python3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `pygitpub-0.0.8/pygitpub/main.py` & `pygitpub-0.0.9/pygitpub/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,27 @@
 def repos_list() -> None:
     g = github.Github(login_or_token=ConfigGithub.token)
     for repo in g.get_user(ConfigGithub.username).get_repos():
         print(repo.name)
 
 
 @register_endpoint(
+    description="List all private repos",
+    configs=[
+        ConfigGithub,
+    ],
+)
+def repos_list_private() -> None:
+    g = github.Github(login_or_token=ConfigGithub.token)
+    for repo in g.get_user(ConfigGithub.username).get_repos(type="private"):
+        if not repo.fork:
+            print(f"{repo.name}")
+
+
+@register_endpoint(
     description="Cleanup old failing or un-needed runs",
     configs=[
         ConfigGithub,
     ],
 )
 def runs_cleanup() -> None:
     g = github.Github(login_or_token=ConfigGithub.token)
```

### Comparing `pygitpub-0.0.8/pygitpub/utils.py` & `pygitpub-0.0.9/pygitpub/utils.py`

 * *Files identical despite different names*

### Comparing `pygitpub-0.0.8/pygitpub.egg-info/PKG-INFO` & `pygitpub-0.0.9/pygitpub.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygitpub
-Version: 0.0.8
+Version: 0.0.9
 Summary: help you work with github
 Home-page: https://veltzer.github.io/pygitpub
 Author: Mark Veltzer
 Author-email: mark.veltzer@gmail.com
 Maintainer: Mark Veltzer
 Maintainer-email: mark.veltzer@gmail.com
 License: MIT
@@ -19,15 +19,15 @@
         
         .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
         
         project website: https://veltzer.github.io/pygitpub
         
         author: Mark Veltzer
         
-        version: 0.0.8
+        version: 0.0.9
         
         
         
 Keywords: github,pygithub
 Platform: python3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `pygitpub-0.0.8/setup.py` & `pygitpub-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.rst') as f:
         return f.read()
 
 
 setuptools.setup(
     # the first three fields are a must according to the documentation
     name="pygitpub",
-    version="0.0.8",
+    version="0.0.9",
     packages=[
         'pygitpub',
     ],
     # from here all is optional
     description="help you work with github",
     long_description=get_readme(),
     long_description_content_type="text/x-rst",
```

