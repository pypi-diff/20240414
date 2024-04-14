# Comparing `tmp/emergingtrajectories-0.2.8.tar.gz` & `tmp/emergingtrajectories-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emergingtrajectories-0.2.8.tar", last modified: Tue Mar 26 02:09:31 2024, max compression
+gzip compressed data, was "emergingtrajectories-0.2.9.tar", last modified: Wed Mar 27 19:54:41 2024, max compression
```

## Comparing `emergingtrajectories-0.2.8.tar` & `emergingtrajectories-0.2.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 wojciech   (501) staff       (20)        0 2024-03-26 02:09:31.804558 emergingtrajectories-0.2.8/
--rw-r--r--   0 wojciech   (501) staff       (20)     1083 2024-03-24 03:42:14.000000 emergingtrajectories-0.2.8/LICENSE
--rw-r--r--   0 wojciech   (501) staff       (20)      676 2024-03-26 02:09:31.804449 emergingtrajectories-0.2.8/PKG-INFO
--rw-r--r--   0 wojciech   (501) staff       (20)      303 2024-03-24 03:42:14.000000 emergingtrajectories-0.2.8/README.md
-drwxr-xr-x   0 wojciech   (501) staff       (20)        0 2024-03-26 02:09:31.803696 emergingtrajectories-0.2.8/emergingtrajectories/
--rw-r--r--   0 wojciech   (501) staff       (20)     7471 2024-03-24 03:42:14.000000 emergingtrajectories-0.2.8/emergingtrajectories/__init__.py
--rw-r--r--   0 wojciech   (501) staff       (20)    16878 2024-03-24 03:42:14.000000 emergingtrajectories-0.2.8/emergingtrajectories/agents.py
--rw-r--r--   0 wojciech   (501) staff       (20)    20415 2024-03-24 03:42:14.000000 emergingtrajectories-0.2.8/emergingtrajectories/citationagents.py
--rw-r--r--   0 wojciech   (501) staff       (20)     3754 2024-03-24 03:42:14.000000 emergingtrajectories-0.2.8/emergingtrajectories/crawlers.py
--rw-r--r--   0 wojciech   (501) staff       (20)    18008 2024-03-24 03:42:14.000000 emergingtrajectories-0.2.8/emergingtrajectories/facts.py
--rw-r--r--   0 wojciech   (501) staff       (20)     9603 2024-03-24 03:42:14.000000 emergingtrajectories-0.2.8/emergingtrajectories/factsforecaster.py
--rw-r--r--   0 wojciech   (501) staff       (20)    23702 2024-03-26 01:58:58.000000 emergingtrajectories-0.2.8/emergingtrajectories/factsrag.py
--rw-r--r--   0 wojciech   (501) staff       (20)     9634 2024-03-25 22:24:08.000000 emergingtrajectories-0.2.8/emergingtrajectories/factsragforecaster.py
--rw-r--r--   0 wojciech   (501) staff       (20)     8909 2024-03-24 03:42:14.000000 emergingtrajectories-0.2.8/emergingtrajectories/knowledge.py
--rw-r--r--   0 wojciech   (501) staff       (20)     1388 2024-03-26 02:00:27.000000 emergingtrajectories-0.2.8/emergingtrajectories/news.py
--rw-r--r--   0 wojciech   (501) staff       (20)      971 2024-03-24 20:02:22.000000 emergingtrajectories-0.2.8/emergingtrajectories/prompts.py
--rw-r--r--   0 wojciech   (501) staff       (20)    14352 2024-03-24 03:42:14.000000 emergingtrajectories-0.2.8/emergingtrajectories/recursiveagent.py
--rw-r--r--   0 wojciech   (501) staff       (20)     4520 2024-03-24 03:42:14.000000 emergingtrajectories-0.2.8/emergingtrajectories/utils.py
-drwxr-xr-x   0 wojciech   (501) staff       (20)        0 2024-03-26 02:09:31.804293 emergingtrajectories-0.2.8/emergingtrajectories.egg-info/
--rw-r--r--   0 wojciech   (501) staff       (20)      676 2024-03-26 02:09:31.000000 emergingtrajectories-0.2.8/emergingtrajectories.egg-info/PKG-INFO
--rw-r--r--   0 wojciech   (501) staff       (20)      691 2024-03-26 02:09:31.000000 emergingtrajectories-0.2.8/emergingtrajectories.egg-info/SOURCES.txt
--rw-r--r--   0 wojciech   (501) staff       (20)        1 2024-03-26 02:09:31.000000 emergingtrajectories-0.2.8/emergingtrajectories.egg-info/dependency_links.txt
--rw-r--r--   0 wojciech   (501) staff       (20)      148 2024-03-26 02:09:31.000000 emergingtrajectories-0.2.8/emergingtrajectories.egg-info/requires.txt
--rw-r--r--   0 wojciech   (501) staff       (20)       21 2024-03-26 02:09:31.000000 emergingtrajectories-0.2.8/emergingtrajectories.egg-info/top_level.txt
--rw-r--r--   0 wojciech   (501) staff       (20)       38 2024-03-26 02:09:31.804601 emergingtrajectories-0.2.8/setup.cfg
--rw-r--r--   0 wojciech   (501) staff       (20)      948 2024-03-24 03:42:14.000000 emergingtrajectories-0.2.8/setup.py
+drwxr-xr-x   0 wojciech   (501) staff       (20)        0 2024-03-27 19:54:41.674540 emergingtrajectories-0.2.9/
+-rw-r--r--   0 wojciech   (501) staff       (20)     1083 2024-03-27 19:51:10.000000 emergingtrajectories-0.2.9/LICENSE
+-rw-r--r--   0 wojciech   (501) staff       (20)      676 2024-03-27 19:54:41.674413 emergingtrajectories-0.2.9/PKG-INFO
+-rw-r--r--   0 wojciech   (501) staff       (20)      303 2024-03-27 19:51:10.000000 emergingtrajectories-0.2.9/README.md
+drwxr-xr-x   0 wojciech   (501) staff       (20)        0 2024-03-27 19:54:41.673388 emergingtrajectories-0.2.9/emergingtrajectories/
+-rw-r--r--   0 wojciech   (501) staff       (20)     7471 2024-03-27 19:51:10.000000 emergingtrajectories-0.2.9/emergingtrajectories/__init__.py
+-rw-r--r--   0 wojciech   (501) staff       (20)    16878 2024-03-27 19:51:10.000000 emergingtrajectories-0.2.9/emergingtrajectories/agents.py
+-rw-r--r--   0 wojciech   (501) staff       (20)    20415 2024-03-27 19:51:10.000000 emergingtrajectories-0.2.9/emergingtrajectories/citationagents.py
+-rw-r--r--   0 wojciech   (501) staff       (20)     3754 2024-03-27 19:51:10.000000 emergingtrajectories-0.2.9/emergingtrajectories/crawlers.py
+-rw-r--r--   0 wojciech   (501) staff       (20)    18008 2024-03-27 19:51:10.000000 emergingtrajectories-0.2.9/emergingtrajectories/facts.py
+-rw-r--r--   0 wojciech   (501) staff       (20)     9603 2024-03-27 19:51:10.000000 emergingtrajectories-0.2.9/emergingtrajectories/factsforecaster.py
+-rw-r--r--   0 wojciech   (501) staff       (20)    23702 2024-03-27 19:51:10.000000 emergingtrajectories-0.2.9/emergingtrajectories/factsrag.py
+-rw-r--r--   0 wojciech   (501) staff       (20)     9634 2024-03-27 19:51:10.000000 emergingtrajectories-0.2.9/emergingtrajectories/factsragforecaster.py
+-rw-r--r--   0 wojciech   (501) staff       (20)     8909 2024-03-27 19:51:10.000000 emergingtrajectories-0.2.9/emergingtrajectories/knowledge.py
+-rw-r--r--   0 wojciech   (501) staff       (20)     1388 2024-03-27 19:51:10.000000 emergingtrajectories-0.2.9/emergingtrajectories/news.py
+-rw-r--r--   0 wojciech   (501) staff       (20)      971 2024-03-27 19:51:10.000000 emergingtrajectories-0.2.9/emergingtrajectories/prompts.py
+-rw-r--r--   0 wojciech   (501) staff       (20)    14352 2024-03-27 19:51:10.000000 emergingtrajectories-0.2.9/emergingtrajectories/recursiveagent.py
+-rw-r--r--   0 wojciech   (501) staff       (20)     4520 2024-03-27 19:51:10.000000 emergingtrajectories-0.2.9/emergingtrajectories/utils.py
+drwxr-xr-x   0 wojciech   (501) staff       (20)        0 2024-03-27 19:54:41.674219 emergingtrajectories-0.2.9/emergingtrajectories.egg-info/
+-rw-r--r--   0 wojciech   (501) staff       (20)      676 2024-03-27 19:54:41.000000 emergingtrajectories-0.2.9/emergingtrajectories.egg-info/PKG-INFO
+-rw-r--r--   0 wojciech   (501) staff       (20)      691 2024-03-27 19:54:41.000000 emergingtrajectories-0.2.9/emergingtrajectories.egg-info/SOURCES.txt
+-rw-r--r--   0 wojciech   (501) staff       (20)        1 2024-03-27 19:54:41.000000 emergingtrajectories-0.2.9/emergingtrajectories.egg-info/dependency_links.txt
+-rw-r--r--   0 wojciech   (501) staff       (20)      208 2024-03-27 19:54:41.000000 emergingtrajectories-0.2.9/emergingtrajectories.egg-info/requires.txt
+-rw-r--r--   0 wojciech   (501) staff       (20)       21 2024-03-27 19:54:41.000000 emergingtrajectories-0.2.9/emergingtrajectories.egg-info/top_level.txt
+-rw-r--r--   0 wojciech   (501) staff       (20)       38 2024-03-27 19:54:41.674587 emergingtrajectories-0.2.9/setup.cfg
+-rw-r--r--   0 wojciech   (501) staff       (20)     1089 2024-03-27 19:52:49.000000 emergingtrajectories-0.2.9/setup.py
```

### Comparing `emergingtrajectories-0.2.8/LICENSE` & `emergingtrajectories-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `emergingtrajectories-0.2.8/PKG-INFO` & `emergingtrajectories-0.2.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emergingtrajectories
-Version: 0.2.8
+Version: 0.2.9
 Summary: Open source library for tracking and saving forecasts of political, economic, and social events.
 Home-page: UNKNOWN
 Author: Wojciech Gryc
 Author-email: hello@phaseai.com
 License: MIT
 Keywords: llm,nlp,ai,social,politics,economics
 Platform: UNKNOWN
```

### Comparing `emergingtrajectories-0.2.8/emergingtrajectories/__init__.py` & `emergingtrajectories-0.2.9/emergingtrajectories/__init__.py`

 * *Files identical despite different names*

### Comparing `emergingtrajectories-0.2.8/emergingtrajectories/agents.py` & `emergingtrajectories-0.2.9/emergingtrajectories/agents.py`

 * *Files identical despite different names*

### Comparing `emergingtrajectories-0.2.8/emergingtrajectories/citationagents.py` & `emergingtrajectories-0.2.9/emergingtrajectories/citationagents.py`

 * *Files identical despite different names*

### Comparing `emergingtrajectories-0.2.8/emergingtrajectories/crawlers.py` & `emergingtrajectories-0.2.9/emergingtrajectories/crawlers.py`

 * *Files identical despite different names*

### Comparing `emergingtrajectories-0.2.8/emergingtrajectories/facts.py` & `emergingtrajectories-0.2.9/emergingtrajectories/facts.py`

 * *Files identical despite different names*

### Comparing `emergingtrajectories-0.2.8/emergingtrajectories/factsforecaster.py` & `emergingtrajectories-0.2.9/emergingtrajectories/factsforecaster.py`

 * *Files identical despite different names*

### Comparing `emergingtrajectories-0.2.8/emergingtrajectories/factsrag.py` & `emergingtrajectories-0.2.9/emergingtrajectories/factsrag.py`

 * *Files identical despite different names*

### Comparing `emergingtrajectories-0.2.8/emergingtrajectories/factsragforecaster.py` & `emergingtrajectories-0.2.9/emergingtrajectories/factsragforecaster.py`

 * *Files identical despite different names*

### Comparing `emergingtrajectories-0.2.8/emergingtrajectories/knowledge.py` & `emergingtrajectories-0.2.9/emergingtrajectories/knowledge.py`

 * *Files identical despite different names*

### Comparing `emergingtrajectories-0.2.8/emergingtrajectories/news.py` & `emergingtrajectories-0.2.9/emergingtrajectories/news.py`

 * *Files identical despite different names*

### Comparing `emergingtrajectories-0.2.8/emergingtrajectories/prompts.py` & `emergingtrajectories-0.2.9/emergingtrajectories/prompts.py`

 * *Files identical despite different names*

### Comparing `emergingtrajectories-0.2.8/emergingtrajectories/recursiveagent.py` & `emergingtrajectories-0.2.9/emergingtrajectories/recursiveagent.py`

 * *Files identical despite different names*

### Comparing `emergingtrajectories-0.2.8/emergingtrajectories/utils.py` & `emergingtrajectories-0.2.9/emergingtrajectories/utils.py`

 * *Files identical despite different names*

### Comparing `emergingtrajectories-0.2.8/emergingtrajectories.egg-info/PKG-INFO` & `emergingtrajectories-0.2.9/emergingtrajectories.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emergingtrajectories
-Version: 0.2.8
+Version: 0.2.9
 Summary: Open source library for tracking and saving forecasts of political, economic, and social events.
 Home-page: UNKNOWN
 Author: Wojciech Gryc
 Author-email: hello@phaseai.com
 License: MIT
 Keywords: llm,nlp,ai,social,politics,economics
 Platform: UNKNOWN
```

### Comparing `emergingtrajectories-0.2.8/emergingtrajectories.egg-info/SOURCES.txt` & `emergingtrajectories-0.2.9/emergingtrajectories.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emergingtrajectories-0.2.8/setup.py` & `emergingtrajectories-0.2.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,15 +7,23 @@
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     author=AUTHOR,
     author_email="hello@phaseai.com",
     license="MIT",
     packages=find_packages(),
-    install_requires=["phasellm>=0.0.20", "Django>=5.0.0", "python-dotenv>=1.0.0"],
+    install_requires=[
+        "phasellm>=0.0.21", 
+        "Django>=5.0.0", 
+        "python-dotenv>=1.0.0", 
+        "dateparser>=1.2.0",
+        "pytest-playwright",
+        "beautifulsoup4",
+        "chromadb"
+        ],
     extras_require={
         "docs": [
             "furo",
             "sphinx>=7.1.2",
             "myst_parser>=2.0.0",
             "sphinx-autoapi>=2.1.1",
             "sphinx-autobuild>=2021.3.14",
```

