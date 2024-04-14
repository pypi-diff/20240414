# Comparing `tmp/mocket-3.9.42.tar.gz` & `tmp/mocket-3.9.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mocket-3.9.42.tar", last modified: Thu Jun 10 12:26:00 2021, max compression
+gzip compressed data, was "mocket-3.9.44.tar", last modified: Tue Aug 31 10:59:25 2021, max compression
```

## Comparing `mocket-3.9.42.tar` & `mocket-3.9.44.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 drizzt    (1000) drizzt    (1000)        0 2021-06-10 12:26:00.610983 mocket-3.9.42/
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     1539 2021-03-20 18:51:56.000000 mocket-3.9.42/LICENSE
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      153 2021-03-20 18:51:56.000000 mocket-3.9.42/MANIFEST.in
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)    12120 2021-06-10 12:26:00.610983 mocket-3.9.42/PKG-INFO
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)    10987 2021-03-20 18:51:56.000000 mocket-3.9.42/README.rst
-drwxrwxr-x   0 drizzt    (1000) drizzt    (1000)        0 2021-06-10 12:26:00.608983 mocket-3.9.42/mocket/
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      157 2021-06-10 12:22:06.000000 mocket-3.9.42/mocket/__init__.py
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      502 2021-06-10 12:17:58.000000 mocket-3.9.42/mocket/async_mocket.py
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      910 2021-03-20 18:51:56.000000 mocket-3.9.42/mocket/compat.py
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)    20310 2021-06-10 12:17:58.000000 mocket-3.9.42/mocket/mocket.py
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     7811 2021-03-20 18:51:56.000000 mocket-3.9.42/mocket/mockhttp.py
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     2708 2021-03-20 18:51:56.000000 mocket-3.9.42/mocket/mockredis.py
-drwxrwxr-x   0 drizzt    (1000) drizzt    (1000)        0 2021-06-10 12:26:00.608983 mocket-3.9.42/mocket/plugins/
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)        0 2021-03-20 18:51:56.000000 mocket-3.9.42/mocket/plugins/__init__.py
-drwxrwxr-x   0 drizzt    (1000) drizzt    (1000)        0 2021-06-10 12:26:00.608983 mocket-3.9.42/mocket/plugins/httpretty/
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     3354 2021-03-20 18:51:56.000000 mocket-3.9.42/mocket/plugins/httpretty/__init__.py
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)       77 2021-03-20 18:51:56.000000 mocket-3.9.42/mocket/plugins/httpretty/core.py
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     1927 2021-03-20 18:51:56.000000 mocket-3.9.42/mocket/plugins/pook_mock_engine.py
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      942 2021-06-10 12:09:29.000000 mocket-3.9.42/mocket/utils.py
-drwxrwxr-x   0 drizzt    (1000) drizzt    (1000)        0 2021-06-10 12:26:00.608983 mocket-3.9.42/mocket.egg-info/
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)    12120 2021-06-10 12:26:00.000000 mocket-3.9.42/mocket.egg-info/PKG-INFO
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     1267 2021-06-10 12:26:00.000000 mocket-3.9.42/mocket.egg-info/SOURCES.txt
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)        1 2021-06-10 12:26:00.000000 mocket-3.9.42/mocket.egg-info/dependency_links.txt
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      242 2021-06-10 12:26:00.000000 mocket-3.9.42/mocket.egg-info/requires.txt
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)        7 2021-06-10 12:26:00.000000 mocket-3.9.42/mocket.egg-info/top_level.txt
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)       75 2021-06-10 12:25:58.000000 mocket-3.9.42/requirements.txt
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)       38 2021-06-10 12:26:00.610983 mocket-3.9.42/setup.cfg
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     2281 2021-03-20 18:51:56.000000 mocket-3.9.42/setup.py
-drwxrwxr-x   0 drizzt    (1000) drizzt    (1000)        0 2021-06-10 12:26:00.608983 mocket-3.9.42/tests/
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      291 2021-03-20 18:51:56.000000 mocket-3.9.42/tests/__init__.py
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)    40976 2021-03-20 18:51:56.000000 mocket-3.9.42/tests/fluidicon.png
-drwxrwxr-x   0 drizzt    (1000) drizzt    (1000)        0 2021-06-10 12:26:00.609983 mocket-3.9.42/tests/main/
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)        0 2021-03-20 18:51:56.000000 mocket-3.9.42/tests/main/__init__.py
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)    14757 2021-03-20 18:51:56.000000 mocket-3.9.42/tests/main/test_http.py
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      162 2021-03-20 18:51:56.000000 mocket-3.9.42/tests/main/test_http_gevent.py
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      842 2021-03-20 18:51:56.000000 mocket-3.9.42/tests/main/test_http_with_xxhash.py
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)    12504 2021-06-06 18:03:57.000000 mocket-3.9.42/tests/main/test_httpretty.py
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     1986 2021-06-09 17:11:33.000000 mocket-3.9.42/tests/main/test_https.py
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     5714 2021-05-21 09:06:01.000000 mocket-3.9.42/tests/main/test_mocket.py
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      614 2021-03-20 18:51:56.000000 mocket-3.9.42/tests/main/test_pook.py
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     8754 2021-03-20 18:51:56.000000 mocket-3.9.42/tests/main/test_redis.py
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     2801 2021-03-20 18:51:56.000000 mocket-3.9.42/tests/main/tests.main.test_http.HttpEntryTestCase.test_truesendall_with_dump_from_recording.json
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     3784 2021-03-20 18:51:56.000000 mocket-3.9.42/tests/main/tests.main.test_http_gevent.GeventHttpEntryTestCase.test_truesendall_with_dump_from_recording.json
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     2753 2021-03-20 18:51:56.000000 mocket-3.9.42/tests/main/tests.main.test_http_with_xxhash.HttpEntryTestCase.test_truesendall_with_dump_from_recording.json
-drwxrwxr-x   0 drizzt    (1000) drizzt    (1000)        0 2021-06-10 12:26:00.609983 mocket-3.9.42/tests/tests35/
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      116 2021-03-20 18:51:56.000000 mocket-3.9.42/tests/tests35/README.txt
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)        0 2021-03-20 18:51:56.000000 mocket-3.9.42/tests/tests35/__init__.py
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     3132 2021-03-20 18:51:56.000000 mocket-3.9.42/tests/tests35/test_http_aiohttp.py
-drwxrwxr-x   0 drizzt    (1000) drizzt    (1000)        0 2021-06-10 12:26:00.609983 mocket-3.9.42/tests/tests37/
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     1299 2021-03-20 18:51:56.000000 mocket-3.9.42/tests/tests37/test_asyncio.py
-drwxrwxr-x   0 drizzt    (1000) drizzt    (1000)        0 2021-06-10 12:26:00.610983 mocket-3.9.42/tests/tests38/
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      132 2021-03-20 18:51:56.000000 mocket-3.9.42/tests/tests38/README.txt
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)        0 2021-03-20 18:51:56.000000 mocket-3.9.42/tests/tests38/__init__.py
--rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     2692 2021-03-20 18:51:56.000000 mocket-3.9.42/tests/tests38/test_http_aiohttp.py
+drwxrwxr-x   0 drizzt    (1000) drizzt    (1000)        0 2021-08-31 10:59:25.871479 mocket-3.9.44/
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     1539 2021-03-20 18:51:56.000000 mocket-3.9.44/LICENSE
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      153 2021-03-20 18:51:56.000000 mocket-3.9.44/MANIFEST.in
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)    12121 2021-08-31 10:59:25.871479 mocket-3.9.44/PKG-INFO
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)    10988 2021-08-31 10:37:51.000000 mocket-3.9.44/README.rst
+drwxrwxr-x   0 drizzt    (1000) drizzt    (1000)        0 2021-08-31 10:59:25.870479 mocket-3.9.44/mocket/
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      157 2021-08-31 10:59:11.000000 mocket-3.9.44/mocket/__init__.py
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      791 2021-08-31 10:41:08.000000 mocket-3.9.44/mocket/async_mocket.py
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      910 2021-03-20 18:51:56.000000 mocket-3.9.44/mocket/compat.py
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)    20449 2021-08-31 10:41:08.000000 mocket-3.9.44/mocket/mocket.py
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     7811 2021-03-20 18:51:56.000000 mocket-3.9.44/mocket/mockhttp.py
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     2708 2021-03-20 18:51:56.000000 mocket-3.9.44/mocket/mockredis.py
+drwxrwxr-x   0 drizzt    (1000) drizzt    (1000)        0 2021-08-31 10:59:25.870479 mocket-3.9.44/mocket/plugins/
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)        0 2021-03-20 18:51:56.000000 mocket-3.9.44/mocket/plugins/__init__.py
+drwxrwxr-x   0 drizzt    (1000) drizzt    (1000)        0 2021-08-31 10:59:25.870479 mocket-3.9.44/mocket/plugins/httpretty/
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     3269 2021-08-31 10:41:08.000000 mocket-3.9.44/mocket/plugins/httpretty/__init__.py
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)       77 2021-03-20 18:51:56.000000 mocket-3.9.44/mocket/plugins/httpretty/core.py
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     1927 2021-03-20 18:51:56.000000 mocket-3.9.44/mocket/plugins/pook_mock_engine.py
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      942 2021-08-31 10:37:51.000000 mocket-3.9.44/mocket/utils.py
+drwxrwxr-x   0 drizzt    (1000) drizzt    (1000)        0 2021-08-31 10:59:25.870479 mocket-3.9.44/mocket.egg-info/
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)    12121 2021-08-31 10:59:25.000000 mocket-3.9.44/mocket.egg-info/PKG-INFO
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     1267 2021-08-31 10:59:25.000000 mocket-3.9.44/mocket.egg-info/SOURCES.txt
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)        1 2021-08-31 10:59:25.000000 mocket-3.9.44/mocket.egg-info/dependency_links.txt
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      239 2021-08-31 10:59:25.000000 mocket-3.9.44/mocket.egg-info/requires.txt
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)        7 2021-08-31 10:59:25.000000 mocket-3.9.44/mocket.egg-info/top_level.txt
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)       72 2021-08-31 10:59:23.000000 mocket-3.9.44/requirements.txt
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)       38 2021-08-31 10:59:25.871479 mocket-3.9.44/setup.cfg
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     2281 2021-03-20 18:51:56.000000 mocket-3.9.44/setup.py
+drwxrwxr-x   0 drizzt    (1000) drizzt    (1000)        0 2021-08-31 10:59:25.870479 mocket-3.9.44/tests/
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      291 2021-03-20 18:51:56.000000 mocket-3.9.44/tests/__init__.py
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)    40976 2021-03-20 18:51:56.000000 mocket-3.9.44/tests/fluidicon.png
+drwxrwxr-x   0 drizzt    (1000) drizzt    (1000)        0 2021-08-31 10:59:25.871479 mocket-3.9.44/tests/main/
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)        0 2021-03-20 18:51:56.000000 mocket-3.9.44/tests/main/__init__.py
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)    14757 2021-03-20 18:51:56.000000 mocket-3.9.44/tests/main/test_http.py
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      162 2021-03-20 18:51:56.000000 mocket-3.9.44/tests/main/test_http_gevent.py
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      842 2021-03-20 18:51:56.000000 mocket-3.9.44/tests/main/test_http_with_xxhash.py
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)    12504 2021-06-06 18:03:57.000000 mocket-3.9.44/tests/main/test_httpretty.py
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     1986 2021-06-09 17:11:33.000000 mocket-3.9.44/tests/main/test_https.py
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     5714 2021-08-31 10:37:51.000000 mocket-3.9.44/tests/main/test_mocket.py
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      614 2021-03-20 18:51:56.000000 mocket-3.9.44/tests/main/test_pook.py
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     8754 2021-03-20 18:51:56.000000 mocket-3.9.44/tests/main/test_redis.py
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     2801 2021-03-20 18:51:56.000000 mocket-3.9.44/tests/main/tests.main.test_http.HttpEntryTestCase.test_truesendall_with_dump_from_recording.json
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     3784 2021-03-20 18:51:56.000000 mocket-3.9.44/tests/main/tests.main.test_http_gevent.GeventHttpEntryTestCase.test_truesendall_with_dump_from_recording.json
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     2753 2021-03-20 18:51:56.000000 mocket-3.9.44/tests/main/tests.main.test_http_with_xxhash.HttpEntryTestCase.test_truesendall_with_dump_from_recording.json
+drwxrwxr-x   0 drizzt    (1000) drizzt    (1000)        0 2021-08-31 10:59:25.871479 mocket-3.9.44/tests/tests35/
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      116 2021-03-20 18:51:56.000000 mocket-3.9.44/tests/tests35/README.txt
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)        0 2021-03-20 18:51:56.000000 mocket-3.9.44/tests/tests35/__init__.py
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     3132 2021-03-20 18:51:56.000000 mocket-3.9.44/tests/tests35/test_http_aiohttp.py
+drwxrwxr-x   0 drizzt    (1000) drizzt    (1000)        0 2021-08-31 10:59:25.871479 mocket-3.9.44/tests/tests37/
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     1299 2021-08-31 10:37:51.000000 mocket-3.9.44/tests/tests37/test_asyncio.py
+drwxrwxr-x   0 drizzt    (1000) drizzt    (1000)        0 2021-08-31 10:59:25.871479 mocket-3.9.44/tests/tests38/
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)      132 2021-03-20 18:51:56.000000 mocket-3.9.44/tests/tests38/README.txt
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)        0 2021-03-20 18:51:56.000000 mocket-3.9.44/tests/tests38/__init__.py
+-rw-rw-r--   0 drizzt    (1000) drizzt    (1000)     2692 2021-08-30 21:46:19.000000 mocket-3.9.44/tests/tests38/test_http_aiohttp.py
```

### Comparing `mocket-3.9.42/LICENSE` & `mocket-3.9.44/LICENSE`

 * *Files identical despite different names*

### Comparing `mocket-3.9.42/PKG-INFO` & `mocket-3.9.44/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocket
-Version: 3.9.42
+Version: 3.9.44
 Summary: Socket Mock Framework - for all kinds of socket animals, web-clients included -         with gevent/asyncio/SSL support
 Home-page: https://github.com/mindflayer/python-mocket
 Author: Giorgio Salluzzo
 Author-email: giorgio.salluzzo@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
@@ -43,15 +43,15 @@
      :target: https://requires.io/github/mindflayer/python-mocket/requirements/?branch=master
      :alt: Requirements Status
 
 A socket mock framework
 -------------------------
     for all kinds of socket *animals*, web-clients included - with gevent/asyncio/SSL support
 
-...and then MicroPython's *urequest* (*mocket >= 3.9.1*)
+...and then MicroPython's *urequests* (*mocket >= 3.9.1*)
 
 
 Versioning
 ==========
 Starting from *3.7.0*, Mocket major version will follow the same numbering pattern as Python's and therefore indicate the most recent Python version that is supported.
 
 FYI: the last version compatible with Python 2.7 is *3.9.4*, bugfixing or backporting of features introduced after that release will only be available as commercial support.
```

### Comparing `mocket-3.9.42/README.rst` & `mocket-3.9.44/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
      :target: https://requires.io/github/mindflayer/python-mocket/requirements/?branch=master
      :alt: Requirements Status
 
 A socket mock framework
 -------------------------
     for all kinds of socket *animals*, web-clients included - with gevent/asyncio/SSL support
 
-...and then MicroPython's *urequest* (*mocket >= 3.9.1*)
+...and then MicroPython's *urequests* (*mocket >= 3.9.1*)
 
 
 Versioning
 ==========
 Starting from *3.7.0*, Mocket major version will follow the same numbering pattern as Python's and therefore indicate the most recent Python version that is supported.
 
 FYI: the last version compatible with Python 2.7 is *3.9.4*, bugfixing or backporting of features introduced after that release will only be available as commercial support.
```

### Comparing `mocket-3.9.42/mocket/compat.py` & `mocket-3.9.44/mocket/compat.py`

 * *Files identical despite different names*

### Comparing `mocket-3.9.42/mocket/mocket.py` & `mocket-3.9.44/mocket/mocket.py`

 * *Files 1% similar despite different names*

```diff
@@ -584,51 +584,63 @@
 
 class Mocketizer(object):
     def __init__(self, instance=None, namespace=None, truesocket_recording_dir=None):
         self.instance = instance
         self.truesocket_recording_dir = truesocket_recording_dir
         self.namespace = namespace or text_type(id(self))
 
-    def __enter__(self):
+    def enter(self):
         Mocket.enable(
             namespace=self.namespace,
             truesocket_recording_dir=self.truesocket_recording_dir,
         )
         if self.instance:
             self.check_and_call("mocketize_setup")
+
+    def __enter__(self):
+        self.enter()
         return self
 
-    def __exit__(self, type, value, tb):
+    def exit(self):
         if self.instance:
             self.check_and_call("mocketize_teardown")
         Mocket.disable()
 
+    def __exit__(self, type, value, tb):
+        self.exit()
+
+    async def __aenter__(self, *args, **kwargs):
+        self.enter()
+        return self
+
+    async def __aexit__(self, *args, **kwargs):
+        self.exit()
+
     def check_and_call(self, method):
         method = getattr(self.instance, method, None)
         if callable(method):
             method()
 
-    @classmethod
-    def wrap(cls, test=None, truesocket_recording_dir=None):
-        def wrapper(t, *args, **kw):
-            instance = args[0] if args else None
-            namespace = None
-            if truesocket_recording_dir:
-                namespace = ".".join(
-                    (
-                        instance.__class__.__module__,
-                        instance.__class__.__name__,
-                        t.__name__,
-                    )
-                )
-            with cls(
-                instance,
-                namespace=namespace,
-                truesocket_recording_dir=truesocket_recording_dir,
-            ):
-                t(*args, **kw)
-            return wrapper
 
-        return decorator.decorator(wrapper, test)
+def wrapper(test, cls=Mocketizer, truesocket_recording_dir=None, *args, **kwargs):
+    instance = args[0] if args else None
+    namespace = None
+    if truesocket_recording_dir:
+        namespace = ".".join(
+            (
+                instance.__class__.__module__,
+                instance.__class__.__name__,
+                test.__name__,
+            )
+        )
+    with cls(
+        instance,
+        namespace=namespace,
+        truesocket_recording_dir=truesocket_recording_dir,
+    ):
+        return test(*args, **kwargs)
 
 
-mocketize = Mocketizer.wrap
+if decorator.__version__ < "5":
+    mocketize = decorator.decorator(wrapper)
+else:
+    mocketize = decorator.decorator(wrapper, kwsyntax=True)
```

### Comparing `mocket-3.9.42/mocket/mockhttp.py` & `mocket-3.9.44/mocket/mockhttp.py`

 * *Files identical despite different names*

### Comparing `mocket-3.9.42/mocket/mockredis.py` & `mocket-3.9.44/mocket/mockredis.py`

 * *Files identical despite different names*

### Comparing `mocket-3.9.42/mocket/plugins/httpretty/__init__.py` & `mocket-3.9.44/mocket/plugins/httpretty/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from sys import version_info
-
 from mocket import Mocket, mocketize
+from mocket.async_mocket import async_mocketize
 from mocket.compat import byte_type, text_type
 from mocket.mockhttp import Entry as MocketHttpEntry
 from mocket.mockhttp import Request as MocketHttpRequest
 from mocket.mockhttp import Response as MocketHttpResponse
 
 
 def httprettifier_headers(headers):
@@ -40,20 +39,15 @@
 class Entry(MocketHttpEntry):
     request_cls = Request
     response_cls = Response
 
 
 activate = mocketize
 httprettified = mocketize
-
-major, minor = version_info[:2]
-if major == 3 and minor >= 5:
-    from mocket.async_mocket import get_async_mocketize
-
-    async_httprettified = get_async_mocketize()
+async_httprettified = async_mocketize
 
 enable = Mocket.enable
 disable = Mocket.disable
 reset = Mocket.reset
 
 GET = Entry.GET
 PUT = Entry.PUT
@@ -124,14 +118,15 @@
 HTTPretty = MocketHTTPretty()
 HTTPretty.register_uri = register_uri
 httpretty = HTTPretty
 
 __all__ = (
     "HTTPretty",
     "activate",
+    "async_httprettified",
     "httprettified",
     "enable",
     "disable",
     "reset",
     "Response",
     "GET",
     "PUT",
```

### Comparing `mocket-3.9.42/mocket/plugins/pook_mock_engine.py` & `mocket-3.9.44/mocket/plugins/pook_mock_engine.py`

 * *Files identical despite different names*

### Comparing `mocket-3.9.42/mocket/utils.py` & `mocket-3.9.44/mocket/utils.py`

 * *Files identical despite different names*

### Comparing `mocket-3.9.42/mocket.egg-info/PKG-INFO` & `mocket-3.9.44/mocket.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mocket
-Version: 3.9.42
+Version: 3.9.44
 Summary: Socket Mock Framework - for all kinds of socket animals, web-clients included -         with gevent/asyncio/SSL support
 Home-page: https://github.com/mindflayer/python-mocket
 Author: Giorgio Salluzzo
 Author-email: giorgio.salluzzo@gmail.com
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 6 - Mature
@@ -43,15 +43,15 @@
      :target: https://requires.io/github/mindflayer/python-mocket/requirements/?branch=master
      :alt: Requirements Status
 
 A socket mock framework
 -------------------------
     for all kinds of socket *animals*, web-clients included - with gevent/asyncio/SSL support
 
-...and then MicroPython's *urequest* (*mocket >= 3.9.1*)
+...and then MicroPython's *urequests* (*mocket >= 3.9.1*)
 
 
 Versioning
 ==========
 Starting from *3.7.0*, Mocket major version will follow the same numbering pattern as Python's and therefore indicate the most recent Python version that is supported.
 
 FYI: the last version compatible with Python 2.7 is *3.9.4*, bugfixing or backporting of features introduced after that release will only be available as commercial support.
```

### Comparing `mocket-3.9.42/mocket.egg-info/SOURCES.txt` & `mocket-3.9.44/mocket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mocket-3.9.42/setup.py` & `mocket-3.9.44/setup.py`

 * *Files identical despite different names*

### Comparing `mocket-3.9.42/tests/fluidicon.png` & `mocket-3.9.44/tests/fluidicon.png`

 * *Files identical despite different names*

### Comparing `mocket-3.9.42/tests/main/test_http.py` & `mocket-3.9.44/tests/main/test_http.py`

 * *Files identical despite different names*

### Comparing `mocket-3.9.42/tests/main/test_http_with_xxhash.py` & `mocket-3.9.44/tests/main/test_http_with_xxhash.py`

 * *Files identical despite different names*

### Comparing `mocket-3.9.42/tests/main/test_httpretty.py` & `mocket-3.9.44/tests/main/test_httpretty.py`

 * *Files identical despite different names*

### Comparing `mocket-3.9.42/tests/main/test_https.py` & `mocket-3.9.44/tests/main/test_https.py`

 * *Files identical despite different names*

### Comparing `mocket-3.9.42/tests/main/test_mocket.py` & `mocket-3.9.44/tests/main/test_mocket.py`

 * *Files identical despite different names*

### Comparing `mocket-3.9.42/tests/main/test_pook.py` & `mocket-3.9.44/tests/main/test_pook.py`

 * *Files identical despite different names*

### Comparing `mocket-3.9.42/tests/main/test_redis.py` & `mocket-3.9.44/tests/main/test_redis.py`

 * *Files identical despite different names*

### Comparing `mocket-3.9.42/tests/main/tests.main.test_http.HttpEntryTestCase.test_truesendall_with_dump_from_recording.json` & `mocket-3.9.44/tests/main/tests.main.test_http.HttpEntryTestCase.test_truesendall_with_dump_from_recording.json`

 * *Files identical despite different names*

### Comparing `mocket-3.9.42/tests/main/tests.main.test_http_gevent.GeventHttpEntryTestCase.test_truesendall_with_dump_from_recording.json` & `mocket-3.9.44/tests/main/tests.main.test_http_gevent.GeventHttpEntryTestCase.test_truesendall_with_dump_from_recording.json`

 * *Files identical despite different names*

### Comparing `mocket-3.9.42/tests/main/tests.main.test_http_with_xxhash.HttpEntryTestCase.test_truesendall_with_dump_from_recording.json` & `mocket-3.9.44/tests/main/tests.main.test_http_with_xxhash.HttpEntryTestCase.test_truesendall_with_dump_from_recording.json`

 * *Files identical despite different names*

### Comparing `mocket-3.9.42/tests/tests35/test_http_aiohttp.py` & `mocket-3.9.44/tests/tests35/test_http_aiohttp.py`

 * *Files identical despite different names*

### Comparing `mocket-3.9.42/tests/tests37/test_asyncio.py` & `mocket-3.9.44/tests/tests37/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `mocket-3.9.42/tests/tests38/test_http_aiohttp.py` & `mocket-3.9.44/tests/tests38/test_http_aiohttp.py`

 * *Files identical despite different names*

