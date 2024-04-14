# Comparing `tmp/yahooproject-0.2.tar.gz` & `tmp/yahooproject-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yahooproject-0.2.tar", last modified: Sun Apr 14 09:33:50 2024, max compression
+gzip compressed data, was "yahooproject-0.3.tar", last modified: Sun Apr 14 09:43:14 2024, max compression
```

## Comparing `yahooproject-0.2.tar` & `yahooproject-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 09:33:50.815544 yahooproject-0.2/
--rw-rw-rw-   0        0        0     2112 2024-04-14 09:33:50.812175 yahooproject-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1722 2024-04-14 09:16:47.000000 yahooproject-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 09:33:50.742370 yahooproject-0.2/YahooProject/
--rw-rw-rw-   0        0        0       23 2024-04-14 09:32:41.000000 yahooproject-0.2/YahooProject/__intit__.py
-drwxrwxrwx   0        0        0        0 2024-04-14 09:33:50.806752 yahooproject-0.2/YahooProject.egg-info/
--rw-rw-rw-   0        0        0     2112 2024-04-14 09:33:50.000000 yahooproject-0.2/YahooProject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2024-04-14 09:33:50.000000 yahooproject-0.2/YahooProject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 09:33:50.000000 yahooproject-0.2/YahooProject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-04-14 09:33:50.000000 yahooproject-0.2/YahooProject.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-14 09:33:50.000000 yahooproject-0.2/YahooProject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 09:33:50.816725 yahooproject-0.2/setup.cfg
--rw-rw-rw-   0        0        0      585 2024-04-14 09:33:28.000000 yahooproject-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 09:43:14.487054 yahooproject-0.3/
+-rw-rw-rw-   0        0        0     2112 2024-04-14 09:43:14.479119 yahooproject-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1722 2024-04-14 09:16:47.000000 yahooproject-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 09:43:14.414183 yahooproject-0.3/YahooProject/
+-rw-rw-rw-   0        0        0     3209 2024-04-14 09:41:49.000000 yahooproject-0.3/YahooProject/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-14 09:43:14.475147 yahooproject-0.3/YahooProject.egg-info/
+-rw-rw-rw-   0        0        0     2112 2024-04-14 09:43:14.000000 yahooproject-0.3/YahooProject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2024-04-14 09:43:14.000000 yahooproject-0.3/YahooProject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 09:43:14.000000 yahooproject-0.3/YahooProject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-04-14 09:43:14.000000 yahooproject-0.3/YahooProject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-14 09:43:14.000000 yahooproject-0.3/YahooProject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 09:43:14.490950 yahooproject-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      585 2024-04-14 09:39:59.000000 yahooproject-0.3/setup.py
```

### Comparing `yahooproject-0.2/PKG-INFO` & `yahooproject-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YahooProject
-Version: 0.2
+Version: 0.3
 Summary: A package for scraping search results from Yahoo Search.
 Author: Nick37
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `yahooproject-0.2/README.md` & `yahooproject-0.3/README.md`

 * *Files identical despite different names*

### Comparing `yahooproject-0.2/YahooProject.egg-info/PKG-INFO` & `yahooproject-0.3/YahooProject.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YahooProject
-Version: 0.2
+Version: 0.3
 Summary: A package for scraping search results from Yahoo Search.
 Author: Nick37
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `yahooproject-0.2/setup.py` & `yahooproject-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='YahooProject',
-    version='0.2',
+    version='0.3',
     packages=['YahooProject'],
     install_requires=[
         'requests',
         'beautifulsoup4'
     ],
     author='Nick37',
     description='A package for scraping search results from Yahoo Search.',
```

