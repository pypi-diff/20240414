# Comparing `tmp/asgebsmanager-0.7.tar.gz` & `tmp/asgebsmanager-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgebsmanager-0.7.tar", last modified: Sun Apr 14 10:34:14 2024, max compression
+gzip compressed data, was "asgebsmanager-0.8.tar", last modified: Sun Apr 14 10:36:03 2024, max compression
```

## Comparing `asgebsmanager-0.7.tar` & `asgebsmanager-0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:34:14.484361 asgebsmanager-0.7/
--rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:34:14.483887 asgebsmanager-0.7/PKG-INFO
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:34:14.483286 asgebsmanager-0.7/asgebsmanager.egg-info/
--rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:34:14.000000 asgebsmanager-0.7/asgebsmanager.egg-info/PKG-INFO
--rw-r--r--   0 raghavgupta   (501) staff       (20)      356 2024-04-14 10:34:14.000000 asgebsmanager-0.7/asgebsmanager.egg-info/SOURCES.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 10:34:14.000000 asgebsmanager-0.7/asgebsmanager.egg-info/dependency_links.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       62 2024-04-14 10:34:14.000000 asgebsmanager-0.7/asgebsmanager.egg-info/entry_points.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)      188 2024-04-14 10:34:14.000000 asgebsmanager-0.7/asgebsmanager.egg-info/requires.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       14 2024-04-14 10:34:14.000000 asgebsmanager-0.7/asgebsmanager.egg-info/top_level.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       38 2024-04-14 10:34:14.484466 asgebsmanager-0.7/setup.cfg
--rw-r--r--   0 raghavgupta   (501) staff       (20)      807 2024-04-14 10:34:07.000000 asgebsmanager-0.7/setup.py
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:34:14.478027 asgebsmanager-0.7/src/
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:34:14.482793 asgebsmanager-0.7/src/asgebsmanager/
--rw-r--r--   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:26:40.000000 asgebsmanager-0.7/src/asgebsmanager/__init__.py
--rw-r--r--   0 raghavgupta   (501) staff       (20)     1291 2024-04-14 10:12:34.000000 asgebsmanager-0.7/src/asgebsmanager/__main__.py
--rw-r--r--   0 raghavgupta   (501) staff       (20)     8843 2024-04-14 10:04:04.000000 asgebsmanager-0.7/src/asgebsmanager/ebs_manager.py
--rw-r--r--   0 raghavgupta   (501) staff       (20)     1620 2024-04-14 10:33:58.000000 asgebsmanager-0.7/src/asgebsmanager/mds_utils.py
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:36:03.547920 asgebsmanager-0.8/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:36:03.547341 asgebsmanager-0.8/PKG-INFO
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:36:03.546665 asgebsmanager-0.8/asgebsmanager.egg-info/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:36:03.000000 asgebsmanager-0.8/asgebsmanager.egg-info/PKG-INFO
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      356 2024-04-14 10:36:03.000000 asgebsmanager-0.8/asgebsmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 10:36:03.000000 asgebsmanager-0.8/asgebsmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       62 2024-04-14 10:36:03.000000 asgebsmanager-0.8/asgebsmanager.egg-info/entry_points.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      188 2024-04-14 10:36:03.000000 asgebsmanager-0.8/asgebsmanager.egg-info/requires.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       14 2024-04-14 10:36:03.000000 asgebsmanager-0.8/asgebsmanager.egg-info/top_level.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       38 2024-04-14 10:36:03.548056 asgebsmanager-0.8/setup.cfg
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      807 2024-04-14 10:35:55.000000 asgebsmanager-0.8/setup.py
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:36:03.541998 asgebsmanager-0.8/src/
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:36:03.546198 asgebsmanager-0.8/src/asgebsmanager/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:26:40.000000 asgebsmanager-0.8/src/asgebsmanager/__init__.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     1291 2024-04-14 10:12:34.000000 asgebsmanager-0.8/src/asgebsmanager/__main__.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     8843 2024-04-14 10:04:04.000000 asgebsmanager-0.8/src/asgebsmanager/ebs_manager.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     1674 2024-04-14 10:35:45.000000 asgebsmanager-0.8/src/asgebsmanager/mds_utils.py
```

### Comparing `asgebsmanager-0.7/setup.py` & `asgebsmanager-0.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os 
 
 setup(
     name = 'asgebsmanager',
-    version = "0.7",
+    version = "0.8",
     author = 'Raghav Gupta',
     description = 'AWS Asg ebs manager',
     packages = find_packages("src"),
     package_dir= {
         "asgebsmanager": os.path.join("src","asgebsmanager")
     },
     install_requires = [
```

### Comparing `asgebsmanager-0.7/src/asgebsmanager/__main__.py` & `asgebsmanager-0.8/src/asgebsmanager/__main__.py`

 * *Files identical despite different names*

### Comparing `asgebsmanager-0.7/src/asgebsmanager/ebs_manager.py` & `asgebsmanager-0.8/src/asgebsmanager/ebs_manager.py`

 * *Files identical despite different names*

### Comparing `asgebsmanager-0.7/src/asgebsmanager/mds_utils.py` & `asgebsmanager-0.8/src/asgebsmanager/mds_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     for attempt in range(retries):
         try:
             url = "http://169.254.169.254/latest/api/token"
             headers = {
                 "X-aws-ec2-metadata-token-ttl-seconds": "21600"
             }
             response = requests.put(url, headers=headers)
+            print(response.text,response.status_code)
             if response.status_code == 200:
                 return response.text
             else:
                 raise Exception("Failed to retrieve IMDS token")
         except Exception as e:
             print(f"Error: {e}. Retrying ({attempt + 1}/{retries}) in {delay} seconds...")
             time.sleep(delay)
```

