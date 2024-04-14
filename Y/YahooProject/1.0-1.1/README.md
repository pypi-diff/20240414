# Comparing `tmp/yahooproject-1.0.tar.gz` & `tmp/yahooproject-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yahooproject-1.0.tar", last modified: Sun Apr 14 09:53:20 2024, max compression
+gzip compressed data, was "yahooproject-1.1.tar", last modified: Sun Apr 14 10:08:34 2024, max compression
```

## Comparing `yahooproject-1.0.tar` & `yahooproject-1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 09:53:20.385017 yahooproject-1.0/
--rw-rw-rw-   0        0        0     2112 2024-04-14 09:53:20.383113 yahooproject-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1722 2024-04-14 09:16:47.000000 yahooproject-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 09:53:20.333182 yahooproject-1.0/YahooProject/
--rw-rw-rw-   0        0        0       25 2024-04-14 09:51:56.000000 yahooproject-1.0/YahooProject/__init__.py
--rw-rw-rw-   0        0        0     3209 2024-04-14 09:51:14.000000 yahooproject-1.0/YahooProject/search.py
-drwxrwxrwx   0        0        0        0 2024-04-14 09:53:20.371127 yahooproject-1.0/YahooProject.egg-info/
--rw-rw-rw-   0        0        0     2112 2024-04-14 09:53:20.000000 yahooproject-1.0/YahooProject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-04-14 09:53:20.000000 yahooproject-1.0/YahooProject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 09:53:20.000000 yahooproject-1.0/YahooProject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-14 09:53:20.000000 yahooproject-1.0/YahooProject.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-14 09:53:20.000000 yahooproject-1.0/YahooProject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 09:53:20.385605 yahooproject-1.0/setup.cfg
--rw-rw-rw-   0        0        0      585 2024-04-14 09:52:36.000000 yahooproject-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 10:08:34.735396 yahooproject-1.1/
+-rw-rw-rw-   0        0        0     2112 2024-04-14 10:08:34.732622 yahooproject-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1722 2024-04-14 09:16:47.000000 yahooproject-1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 10:08:34.655632 yahooproject-1.1/YahooProject/
+-rw-rw-rw-   0        0        0       26 2024-04-14 10:07:35.000000 yahooproject-1.1/YahooProject/__init__.py
+-rw-rw-rw-   0        0        0     3209 2024-04-14 09:51:14.000000 yahooproject-1.1/YahooProject/search.py
+drwxrwxrwx   0        0        0        0 2024-04-14 10:08:34.726075 yahooproject-1.1/YahooProject.egg-info/
+-rw-rw-rw-   0        0        0     2112 2024-04-14 10:08:34.000000 yahooproject-1.1/YahooProject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-04-14 10:08:34.000000 yahooproject-1.1/YahooProject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 10:08:34.000000 yahooproject-1.1/YahooProject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-14 10:08:34.000000 yahooproject-1.1/YahooProject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-14 10:08:34.000000 yahooproject-1.1/YahooProject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 10:08:34.736392 yahooproject-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      585 2024-04-14 10:08:01.000000 yahooproject-1.1/setup.py
```

### Comparing `yahooproject-1.0/PKG-INFO` & `yahooproject-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YahooProject
-Version: 1.0
+Version: 1.1
 Summary: A package for scraping search results from Yahoo Search.
 Author: Nick37
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `yahooproject-1.0/README.md` & `yahooproject-1.1/README.md`

 * *Files identical despite different names*

### Comparing `yahooproject-1.0/YahooProject/search.py` & `yahooproject-1.1/YahooProject/search.py`

 * *Files identical despite different names*

### Comparing `yahooproject-1.0/YahooProject.egg-info/PKG-INFO` & `yahooproject-1.1/YahooProject.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YahooProject
-Version: 1.0
+Version: 1.1
 Summary: A package for scraping search results from Yahoo Search.
 Author: Nick37
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `yahooproject-1.0/setup.py` & `yahooproject-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='YahooProject',
-    version='1.0',
+    version='1.1',
     packages=['YahooProject'],
     install_requires=[
         'requests',
         'beautifulsoup4'
     ],
     author='Nick37',
     description='A package for scraping search results from Yahoo Search.',
```

