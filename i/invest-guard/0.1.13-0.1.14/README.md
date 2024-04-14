# Comparing `tmp/invest_guard-0.1.13.tar.gz` & `tmp/invest_guard-0.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invest_guard-0.1.13.tar", last modified: Sun Apr 14 00:50:49 2024, max compression
+gzip compressed data, was "invest_guard-0.1.14.tar", last modified: Sun Apr 14 01:23:02 2024, max compression
```

## Comparing `invest_guard-0.1.13.tar` & `invest_guard-0.1.14.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-14 00:50:49.631168 invest_guard-0.1.13/
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     2590 2024-04-14 00:50:49.630835 invest_guard-0.1.13/PKG-INFO
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     1760 2024-04-13 22:01:49.000000 invest_guard-0.1.13/README.md
-drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-14 00:50:49.630490 invest_guard-0.1.13/invest_guard.egg-info/
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     2590 2024-04-14 00:50:49.000000 invest_guard-0.1.13/invest_guard.egg-info/PKG-INFO
--rw-r--r--   0 tracymuzembi   (501) staff       (20)      236 2024-04-14 00:50:49.000000 invest_guard-0.1.13/invest_guard.egg-info/SOURCES.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-14 00:50:49.000000 invest_guard-0.1.13/invest_guard.egg-info/dependency_links.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)       39 2024-04-14 00:50:49.000000 invest_guard-0.1.13/invest_guard.egg-info/entry_points.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)       41 2024-04-14 00:50:49.000000 invest_guard-0.1.13/invest_guard.egg-info/requires.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-14 00:50:49.000000 invest_guard-0.1.13/invest_guard.egg-info/top_level.txt
--rw-r--r--   0 tracymuzembi   (501) staff       (20)       38 2024-04-14 00:50:49.631229 invest_guard-0.1.13/setup.cfg
--rw-r--r--   0 tracymuzembi   (501) staff       (20)     1125 2024-04-14 00:50:46.000000 invest_guard-0.1.13/setup.py
+drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-14 01:23:02.224946 invest_guard-0.1.14/
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     2590 2024-04-14 01:23:02.224585 invest_guard-0.1.14/PKG-INFO
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     1760 2024-04-13 22:01:49.000000 invest_guard-0.1.14/README.md
+drwxr-xr-x   0 tracymuzembi   (501) staff       (20)        0 2024-04-14 01:23:02.224179 invest_guard-0.1.14/invest_guard.egg-info/
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     2590 2024-04-14 01:23:02.000000 invest_guard-0.1.14/invest_guard.egg-info/PKG-INFO
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)      236 2024-04-14 01:23:02.000000 invest_guard-0.1.14/invest_guard.egg-info/SOURCES.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-14 01:23:02.000000 invest_guard-0.1.14/invest_guard.egg-info/dependency_links.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)       36 2024-04-14 01:23:02.000000 invest_guard-0.1.14/invest_guard.egg-info/entry_points.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)       41 2024-04-14 01:23:02.000000 invest_guard-0.1.14/invest_guard.egg-info/requires.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)        1 2024-04-14 01:23:02.000000 invest_guard-0.1.14/invest_guard.egg-info/top_level.txt
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)       38 2024-04-14 01:23:02.225013 invest_guard-0.1.14/setup.cfg
+-rw-r--r--   0 tracymuzembi   (501) staff       (20)     1148 2024-04-14 01:22:06.000000 invest_guard-0.1.14/setup.py
```

### Comparing `invest_guard-0.1.13/PKG-INFO` & `invest_guard-0.1.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invest_guard
-Version: 0.1.13
+Version: 0.1.14
 Summary: Invest Guard is a command-line interface (CLI) tool for fetching and analyzing financial data from various sources. With Invest Guard, you can easily retrieve stock prices, market trends, and other relevant financial information directly from your terminal.
 Home-page: https://github.com/Work-With-Phoenix/invest-guard
 Author: Phoenix Interface
 Author-email: info@phoenixui.cloud
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `invest_guard-0.1.13/README.md` & `invest_guard-0.1.14/README.md`

 * *Files identical despite different names*

### Comparing `invest_guard-0.1.13/invest_guard.egg-info/PKG-INFO` & `invest_guard-0.1.14/invest_guard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invest_guard
-Version: 0.1.13
+Version: 0.1.14
 Summary: Invest Guard is a command-line interface (CLI) tool for fetching and analyzing financial data from various sources. With Invest Guard, you can easily retrieve stock prices, market trends, and other relevant financial information directly from your terminal.
 Home-page: https://github.com/Work-With-Phoenix/invest-guard
 Author: Phoenix Interface
 Author-email: info@phoenixui.cloud
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `invest_guard-0.1.13/setup.py` & `invest_guard-0.1.14/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
-
+from version import VERSION
 setup(
     name='invest_guard',
-    version='0.1.13',
+    version=VERSION,
     packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'guard = src.main:run'
+            'guard = guard:run'
         ]
     },
     install_requires=[
         'rich',
         'tabulate',
         'yfinance',
         'pandas',
```

