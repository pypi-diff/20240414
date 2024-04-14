# Comparing `tmp/Sentinel_2_band_downloader-0.3.1.tar.gz` & `tmp/sentinel_2_band_downloader-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Sentinel_2_band_downloader-0.3.1.tar", last modified: Mon Feb 19 17:10:55 2024, max compression
+gzip compressed data, was "sentinel_2_band_downloader-0.3.2.tar", last modified: Sun Apr 14 15:34:07 2024, max compression
```

## Comparing `Sentinel_2_band_downloader-0.3.1.tar` & `sentinel_2_band_downloader-0.3.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        0 2024-02-19 17:10:55.317340 Sentinel_2_band_downloader-0.3.1/
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     1068 2024-01-31 16:01:25.000000 Sentinel_2_band_downloader-0.3.1/LICENSE
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     3078 2024-02-19 17:10:55.317340 Sentinel_2_band_downloader-0.3.1/PKG-INFO
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     2687 2024-02-19 17:09:42.000000 Sentinel_2_band_downloader-0.3.1/README.md
-drwxr-xr-x   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        0 2024-02-19 17:10:55.317340 Sentinel_2_band_downloader-0.3.1/Sentinel_2_band_downloader.egg-info/
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     3078 2024-02-19 17:10:55.000000 Sentinel_2_band_downloader-0.3.1/Sentinel_2_band_downloader.egg-info/PKG-INFO
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)      683 2024-02-19 17:10:55.000000 Sentinel_2_band_downloader-0.3.1/Sentinel_2_band_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        1 2024-02-19 17:10:55.000000 Sentinel_2_band_downloader-0.3.1/Sentinel_2_band_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)       44 2024-02-19 17:10:55.000000 Sentinel_2_band_downloader-0.3.1/Sentinel_2_band_downloader.egg-info/requires.txt
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        4 2024-02-19 17:10:55.000000 Sentinel_2_band_downloader-0.3.1/Sentinel_2_band_downloader.egg-info/top_level.txt
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)      457 2024-02-19 17:09:50.000000 Sentinel_2_band_downloader-0.3.1/pyproject.toml
-drwxr-xr-x   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        0 2024-02-19 17:10:55.307340 Sentinel_2_band_downloader-0.3.1/scr/
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        0 2024-02-07 16:18:21.000000 Sentinel_2_band_downloader-0.3.1/scr/__init__.py
-drwxr-xr-x   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        0 2024-02-19 17:10:55.307340 Sentinel_2_band_downloader-0.3.1/scr/example/
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        0 2024-01-18 23:59:05.000000 Sentinel_2_band_downloader-0.3.1/scr/example/__init__.py
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     1941 2024-02-19 17:08:51.000000 Sentinel_2_band_downloader-0.3.1/scr/example/sentinel_2_band_downloader_example.py
-drwxr-xr-x   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        0 2024-02-19 17:10:55.317340 Sentinel_2_band_downloader-0.3.1/scr/main/
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        0 2024-01-30 17:52:31.000000 Sentinel_2_band_downloader-0.3.1/scr/main/__init__.py
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     5048 2024-02-12 13:37:47.000000 Sentinel_2_band_downloader-0.3.1/scr/main/sentinel_2_band_downloader.py
-drwxr-xr-x   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        0 2024-02-19 17:10:55.317340 Sentinel_2_band_downloader-0.3.1/scr/misc/
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)       36 2024-01-23 21:08:56.000000 Sentinel_2_band_downloader-0.3.1/scr/misc/__init__.py
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)    24101 2024-02-12 13:57:48.000000 Sentinel_2_band_downloader-0.3.1/scr/misc/connections.py
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)      681 2024-02-05 18:12:39.000000 Sentinel_2_band_downloader-0.3.1/scr/misc/dates.py
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     5103 2024-02-02 17:59:29.000000 Sentinel_2_band_downloader-0.3.1/scr/misc/files.py
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     6100 2024-02-07 14:59:04.000000 Sentinel_2_band_downloader-0.3.1/scr/misc/utils.py
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)       38 2024-02-19 17:10:55.317340 Sentinel_2_band_downloader-0.3.1/setup.cfg
-drwxr-xr-x   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        0 2024-02-19 17:10:55.317340 Sentinel_2_band_downloader-0.3.1/test/
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     1759 2024-01-30 16:09:51.000000 Sentinel_2_band_downloader-0.3.1/test/test_connect_to_api.py
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     3630 2024-01-30 16:10:01.000000 Sentinel_2_band_downloader-0.3.1/test/test_construct_query.py
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     1974 2024-01-30 16:10:07.000000 Sentinel_2_band_downloader-0.3.1/test/test_get_products_info.py
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     1416 2024-01-30 16:10:38.000000 Sentinel_2_band_downloader-0.3.1/test/test_output_folder.py
--rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     3946 2024-01-30 16:10:27.000000 Sentinel_2_band_downloader-0.3.1/test/test_products_from_sentinel_2.py
+drwxr-xr-x   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        0 2024-04-14 15:34:07.124047 sentinel_2_band_downloader-0.3.2/
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     1068 2024-01-31 16:01:25.000000 sentinel_2_band_downloader-0.3.2/LICENSE
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     3078 2024-04-14 15:34:07.124047 sentinel_2_band_downloader-0.3.2/PKG-INFO
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     2687 2024-02-19 17:09:42.000000 sentinel_2_band_downloader-0.3.2/README.md
+drwxr-xr-x   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        0 2024-04-14 15:34:07.124047 sentinel_2_band_downloader-0.3.2/Sentinel_2_band_downloader.egg-info/
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     3078 2024-04-14 15:34:07.000000 sentinel_2_band_downloader-0.3.2/Sentinel_2_band_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)      683 2024-04-14 15:34:07.000000 sentinel_2_band_downloader-0.3.2/Sentinel_2_band_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        1 2024-04-14 15:34:07.000000 sentinel_2_band_downloader-0.3.2/Sentinel_2_band_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)       44 2024-04-14 15:34:07.000000 sentinel_2_band_downloader-0.3.2/Sentinel_2_band_downloader.egg-info/requires.txt
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        4 2024-04-14 15:34:07.000000 sentinel_2_band_downloader-0.3.2/Sentinel_2_band_downloader.egg-info/top_level.txt
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)      457 2024-04-14 15:32:33.000000 sentinel_2_band_downloader-0.3.2/pyproject.toml
+drwxr-xr-x   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        0 2024-04-14 15:34:07.124047 sentinel_2_band_downloader-0.3.2/scr/
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        0 2024-02-07 16:18:21.000000 sentinel_2_band_downloader-0.3.2/scr/__init__.py
+drwxr-xr-x   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        0 2024-04-14 15:34:07.124047 sentinel_2_band_downloader-0.3.2/scr/example/
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        0 2024-01-18 23:59:05.000000 sentinel_2_band_downloader-0.3.2/scr/example/__init__.py
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     1941 2024-02-19 17:08:51.000000 sentinel_2_band_downloader-0.3.2/scr/example/sentinel_2_band_downloader_example.py
+drwxr-xr-x   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        0 2024-04-14 15:34:07.124047 sentinel_2_band_downloader-0.3.2/scr/main/
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        0 2024-01-30 17:52:31.000000 sentinel_2_band_downloader-0.3.2/scr/main/__init__.py
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     5048 2024-02-12 13:37:47.000000 sentinel_2_band_downloader-0.3.2/scr/main/sentinel_2_band_downloader.py
+drwxr-xr-x   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        0 2024-04-14 15:34:07.124047 sentinel_2_band_downloader-0.3.2/scr/misc/
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)       36 2024-01-23 21:08:56.000000 sentinel_2_band_downloader-0.3.2/scr/misc/__init__.py
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)    24101 2024-02-12 13:57:48.000000 sentinel_2_band_downloader-0.3.2/scr/misc/connections.py
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)      681 2024-02-05 18:12:39.000000 sentinel_2_band_downloader-0.3.2/scr/misc/dates.py
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     5103 2024-02-02 17:59:29.000000 sentinel_2_band_downloader-0.3.2/scr/misc/files.py
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     6100 2024-02-07 14:59:04.000000 sentinel_2_band_downloader-0.3.2/scr/misc/utils.py
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)       38 2024-04-14 15:34:07.124047 sentinel_2_band_downloader-0.3.2/setup.cfg
+drwxr-xr-x   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)        0 2024-04-14 15:34:07.124047 sentinel_2_band_downloader-0.3.2/test/
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     1759 2024-01-30 16:09:51.000000 sentinel_2_band_downloader-0.3.2/test/test_connect_to_api.py
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     3630 2024-01-30 16:10:01.000000 sentinel_2_band_downloader-0.3.2/test/test_construct_query.py
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     1974 2024-01-30 16:10:07.000000 sentinel_2_band_downloader-0.3.2/test/test_get_products_info.py
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     1416 2024-01-30 16:10:38.000000 sentinel_2_band_downloader-0.3.2/test/test_output_folder.py
+-rw-r--r--   0 beatrizgiscaruso  (1000) beatrizgiscaruso  (1000)     3946 2024-01-30 16:10:27.000000 sentinel_2_band_downloader-0.3.2/test/test_products_from_sentinel_2.py
```

### Comparing `Sentinel_2_band_downloader-0.3.1/LICENSE` & `sentinel_2_band_downloader-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Sentinel_2_band_downloader-0.3.1/PKG-INFO` & `sentinel_2_band_downloader-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: Sentinel_2_band_downloader
-Version: 0.3.1
+Version: 0.3.2
 Summary: Utility for searching and downloading satellite images of Sentinel 2
 Author-email: Beatriz Nattrodt DAvila <beatriznattrodt@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
-Requires-Dist: loguru==0.7.0
-Requires-Dist: tqdm==4.66.0
+Requires-Dist: loguru==0.7.2
+Requires-Dist: tqdm==4.66.1
 
 # Sentinel-2 Band Downloader
 
 ## Overview
 
 Sentinel-2 Band Downloader is a simple Python package that allows users to download individual bands from Sentinel-2 satellite data.
```

### Comparing `Sentinel_2_band_downloader-0.3.1/README.md` & `sentinel_2_band_downloader-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `Sentinel_2_band_downloader-0.3.1/Sentinel_2_band_downloader.egg-info/PKG-INFO` & `sentinel_2_band_downloader-0.3.2/Sentinel_2_band_downloader.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: Sentinel_2_band_downloader
-Version: 0.3.1
+Version: 0.3.2
 Summary: Utility for searching and downloading satellite images of Sentinel 2
 Author-email: Beatriz Nattrodt DAvila <beatriznattrodt@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.31.0
-Requires-Dist: loguru==0.7.0
-Requires-Dist: tqdm==4.66.0
+Requires-Dist: loguru==0.7.2
+Requires-Dist: tqdm==4.66.1
 
 # Sentinel-2 Band Downloader
 
 ## Overview
 
 Sentinel-2 Band Downloader is a simple Python package that allows users to download individual bands from Sentinel-2 satellite data.
```

### Comparing `Sentinel_2_band_downloader-0.3.1/Sentinel_2_band_downloader.egg-info/SOURCES.txt` & `sentinel_2_band_downloader-0.3.2/Sentinel_2_band_downloader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Sentinel_2_band_downloader-0.3.1/scr/example/sentinel_2_band_downloader_example.py` & `sentinel_2_band_downloader-0.3.2/scr/example/sentinel_2_band_downloader_example.py`

 * *Files identical despite different names*

### Comparing `Sentinel_2_band_downloader-0.3.1/scr/main/sentinel_2_band_downloader.py` & `sentinel_2_band_downloader-0.3.2/scr/main/sentinel_2_band_downloader.py`

 * *Files identical despite different names*

### Comparing `Sentinel_2_band_downloader-0.3.1/scr/misc/connections.py` & `sentinel_2_band_downloader-0.3.2/scr/misc/connections.py`

 * *Files identical despite different names*

### Comparing `Sentinel_2_band_downloader-0.3.1/scr/misc/dates.py` & `sentinel_2_band_downloader-0.3.2/scr/misc/dates.py`

 * *Files identical despite different names*

### Comparing `Sentinel_2_band_downloader-0.3.1/scr/misc/files.py` & `sentinel_2_band_downloader-0.3.2/scr/misc/files.py`

 * *Files identical despite different names*

### Comparing `Sentinel_2_band_downloader-0.3.1/scr/misc/utils.py` & `sentinel_2_band_downloader-0.3.2/scr/misc/utils.py`

 * *Files identical despite different names*

### Comparing `Sentinel_2_band_downloader-0.3.1/test/test_connect_to_api.py` & `sentinel_2_band_downloader-0.3.2/test/test_connect_to_api.py`

 * *Files identical despite different names*

### Comparing `Sentinel_2_band_downloader-0.3.1/test/test_construct_query.py` & `sentinel_2_band_downloader-0.3.2/test/test_construct_query.py`

 * *Files identical despite different names*

### Comparing `Sentinel_2_band_downloader-0.3.1/test/test_get_products_info.py` & `sentinel_2_band_downloader-0.3.2/test/test_get_products_info.py`

 * *Files identical despite different names*

### Comparing `Sentinel_2_band_downloader-0.3.1/test/test_output_folder.py` & `sentinel_2_band_downloader-0.3.2/test/test_output_folder.py`

 * *Files identical despite different names*

### Comparing `Sentinel_2_band_downloader-0.3.1/test/test_products_from_sentinel_2.py` & `sentinel_2_band_downloader-0.3.2/test/test_products_from_sentinel_2.py`

 * *Files identical despite different names*

