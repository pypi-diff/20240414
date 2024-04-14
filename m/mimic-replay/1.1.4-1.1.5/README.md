# Comparing `tmp/mimic_replay-1.1.4.tar.gz` & `tmp/mimic_replay-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimic_replay-1.1.4.tar", last modified: Sun Apr  7 17:18:14 2024, max compression
+gzip compressed data, was "mimic_replay-1.1.5.tar", last modified: Sun Apr 14 01:47:13 2024, max compression
```

## Comparing `mimic_replay-1.1.4.tar` & `mimic_replay-1.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-07 17:18:14.810368 mimic_replay-1.1.4/
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1062 2024-03-29 16:37:37.000000 mimic_replay-1.1.4/LICENSE
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1214 2024-04-07 17:18:14.810368 mimic_replay-1.1.4/PKG-INFO
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      458 2024-04-04 19:03:46.000000 mimic_replay-1.1.4/README.md
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      869 2024-04-07 17:18:05.000000 mimic_replay-1.1.4/pyproject.toml
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       38 2024-04-07 17:18:14.810368 mimic_replay-1.1.4/setup.cfg
-drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-07 17:18:14.800368 mimic_replay-1.1.4/src/
-drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-07 17:18:14.810368 mimic_replay-1.1.4/src/mimic_replay/
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-03-29 16:39:06.000000 mimic_replay-1.1.4/src/mimic_replay/__init__.py
--rw-rw-r--   0 veronika_todd  (1000) veronika_todd  (1000)     9039 2024-03-29 20:07:26.000000 mimic_replay-1.1.4/src/mimic_replay/config.py
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1202 2024-04-04 19:06:47.000000 mimic_replay-1.1.4/src/mimic_replay/injector.py
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     3120 2024-04-07 17:13:30.000000 mimic_replay-1.1.4/src/mimic_replay/install.py
-drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-07 17:18:14.810368 mimic_replay-1.1.4/src/mimic_replay.egg-info/
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1214 2024-04-07 17:18:14.000000 mimic_replay-1.1.4/src/mimic_replay.egg-info/PKG-INFO
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      344 2024-04-07 17:18:14.000000 mimic_replay-1.1.4/src/mimic_replay.egg-info/SOURCES.txt
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)        1 2024-04-07 17:18:14.000000 mimic_replay-1.1.4/src/mimic_replay.egg-info/dependency_links.txt
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       25 2024-04-07 17:18:14.000000 mimic_replay-1.1.4/src/mimic_replay.egg-info/requires.txt
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       13 2024-04-07 17:18:14.000000 mimic_replay-1.1.4/src/mimic_replay.egg-info/top_level.txt
+drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-14 01:47:12.990975 mimic_replay-1.1.5/
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1062 2024-04-08 22:59:40.000000 mimic_replay-1.1.5/LICENSE
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1229 2024-04-14 01:47:12.990975 mimic_replay-1.1.5/PKG-INFO
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      458 2024-04-08 22:59:40.000000 mimic_replay-1.1.5/README.md
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      884 2024-04-14 01:44:46.000000 mimic_replay-1.1.5/pyproject.toml
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       38 2024-04-14 01:47:12.990975 mimic_replay-1.1.5/setup.cfg
+drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-14 01:47:12.980975 mimic_replay-1.1.5/src/
+drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-14 01:47:12.980975 mimic_replay-1.1.5/src/mimic_replay/
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-08 22:59:40.000000 mimic_replay-1.1.5/src/mimic_replay/__init__.py
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     9039 2024-04-08 22:59:40.000000 mimic_replay-1.1.5/src/mimic_replay/config.py
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1261 2024-04-14 01:36:06.000000 mimic_replay-1.1.5/src/mimic_replay/injector.py
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     3120 2024-04-08 22:59:40.000000 mimic_replay-1.1.5/src/mimic_replay/install.py
+drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-14 01:47:12.990975 mimic_replay-1.1.5/src/mimic_replay.egg-info/
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1229 2024-04-14 01:47:12.000000 mimic_replay-1.1.5/src/mimic_replay.egg-info/PKG-INFO
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      344 2024-04-14 01:47:12.000000 mimic_replay-1.1.5/src/mimic_replay.egg-info/SOURCES.txt
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)        1 2024-04-14 01:47:12.000000 mimic_replay-1.1.5/src/mimic_replay.egg-info/dependency_links.txt
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       43 2024-04-14 01:47:12.000000 mimic_replay-1.1.5/src/mimic_replay.egg-info/requires.txt
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       13 2024-04-14 01:47:12.000000 mimic_replay-1.1.5/src/mimic_replay.egg-info/top_level.txt
```

### Comparing `mimic_replay-1.1.4/LICENSE` & `mimic_replay-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mimic_replay-1.1.4/PKG-INFO` & `mimic_replay-1.1.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mimic_replay
-Version: 1.1.4
+Version: 1.1.5
 Summary: MIMIC installation script, which enables your application to communicate with your MIMIC server.
 Author-email: Veronika Todd <veronika.todd@gmail.com>, Lucas Sorribes <lucas.sorribes@gmail.com>, Erik Wiens <erik.wiens@gmail.com>, Louis Mascari <lmascari16@gmail.com>
 Project-URL: MIMIC, https://mimic-replay.com
-Project-URL: Github, https://github.com/2401-Team-4/capstone
+Project-URL: Github, https://github.com/2401-Team-4/MIMIC
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: uuid
 Requires-Dist: requests
 Requires-Dist: bcrypt
-Requires-Dist: bs4
+Requires-Dist: BeautifulSoup>=4.11.0
 
 This installation package sets up and injects MIMIC's session replay recording functionality into your own application. Unfamiliar with MIMIC? Please visit our project links for more information!  
 
 To properly utilize this installation package:
 - Ensure your MIMIC backend is installed and running before proceeding.
 - In the root folder of the desired application, run the installation script with `python3 -m mimic_replay.install` and follow the prompts.
```

### Comparing `mimic_replay-1.1.4/pyproject.toml` & `mimic_replay-1.1.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mimic_replay"
-version = "1.1.4"
+version = "1.1.5"
 authors = [
   { name="Veronika Todd", email="veronika.todd@gmail.com" },
   { name="Lucas Sorribes", email="lucas.sorribes@gmail.com" },
   { name="Erik Wiens", email="erik.wiens@gmail.com" },
   { name="Louis Mascari", email="lmascari16@gmail.com" }
 ]
 dependencies = [
     "uuid",
     "requests",
     "bcrypt",
-    "bs4"
+    "BeautifulSoup>=4.11.0"
 ]
 description = "MIMIC installation script, which enables your application to communicate with your MIMIC server."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 MIMIC = "https://mimic-replay.com"
-Github = "https://github.com/2401-Team-4/capstone"
+Github = "https://github.com/2401-Team-4/MIMIC"
```

### Comparing `mimic_replay-1.1.4/src/mimic_replay/config.py` & `mimic_replay-1.1.5/src/mimic_replay/config.py`

 * *Files identical despite different names*

### Comparing `mimic_replay-1.1.4/src/mimic_replay/injector.py` & `mimic_replay-1.1.5/src/mimic_replay/injector.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,31 @@
-from bs4 import BeautifulSoup, Comment
+from bs4 import BeautifulSoup, Comment, formatter
 import glob, os
 
 root_dir = '.'
 
 def inject_scripts(raw_file):
   current_dir = os.path.dirname(raw_file)
   rel_dir = os.path.relpath(root_dir, current_dir)
 
   with open(raw_file, 'r') as file:
     html_content = file.read()
+    format = formatter.HTMLFormatter(indent=2)
     if "Mimic Start" in html_content: 
       return
 
     soup = BeautifulSoup(html_content, 'html.parser')
 
     rrweb_script = soup.new_tag('script') 
     rrweb_script['src'] = "https://cdn.jsdelivr.net/npm/rrweb@latest/dist/rrweb-all.min.js"
     rrweb_script['class'] = 'mimic'
     rrweb_script.attrs['defer'] = None
 
     mimic_script = soup.new_tag('script')
-    mimic_script['src'] = os.path.join(rel_dir, 'script.mimic.js') #"./script.mimic.js"
+    mimic_script['src'] = os.path.join(rel_dir, 'script.mimic.js')
     mimic_script['class'] = 'mimic'
     mimic_script.attrs['defer'] = None
 
     soup.head.extend([ 
       Comment('Mimic Start'),   
       '\n',
       rrweb_script, 
@@ -32,15 +33,15 @@
       mimic_script,   
       '\n',         
       Comment('Mimic End'),    
       '\n'
     ])
 
     with open(raw_file, 'w') as file:
-      file.write(str(soup))  
+      file.write(soup.prettify(formatter=format))  
 
 
 files = glob.glob('./**/*.html', recursive=True)
 for file in files:
   inject_scripts(file)
   
 print("🔹 Mimic script injected into html file(s)")
```

### Comparing `mimic_replay-1.1.4/src/mimic_replay/install.py` & `mimic_replay-1.1.5/src/mimic_replay/install.py`

 * *Files identical despite different names*

### Comparing `mimic_replay-1.1.4/src/mimic_replay.egg-info/PKG-INFO` & `mimic_replay-1.1.5/src/mimic_replay.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: mimic_replay
-Version: 1.1.4
+Version: 1.1.5
 Summary: MIMIC installation script, which enables your application to communicate with your MIMIC server.
 Author-email: Veronika Todd <veronika.todd@gmail.com>, Lucas Sorribes <lucas.sorribes@gmail.com>, Erik Wiens <erik.wiens@gmail.com>, Louis Mascari <lmascari16@gmail.com>
 Project-URL: MIMIC, https://mimic-replay.com
-Project-URL: Github, https://github.com/2401-Team-4/capstone
+Project-URL: Github, https://github.com/2401-Team-4/MIMIC
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: uuid
 Requires-Dist: requests
 Requires-Dist: bcrypt
-Requires-Dist: bs4
+Requires-Dist: BeautifulSoup>=4.11.0
 
 This installation package sets up and injects MIMIC's session replay recording functionality into your own application. Unfamiliar with MIMIC? Please visit our project links for more information!  
 
 To properly utilize this installation package:
 - Ensure your MIMIC backend is installed and running before proceeding.
 - In the root folder of the desired application, run the installation script with `python3 -m mimic_replay.install` and follow the prompts.
```

