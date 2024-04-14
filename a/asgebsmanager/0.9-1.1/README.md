# Comparing `tmp/asgebsmanager-0.9.tar.gz` & `tmp/asgebsmanager-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgebsmanager-0.9.tar", last modified: Sun Apr 14 10:38:08 2024, max compression
+gzip compressed data, was "asgebsmanager-1.1.tar", last modified: Sun Apr 14 10:41:28 2024, max compression
```

## Comparing `asgebsmanager-0.9.tar` & `asgebsmanager-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:38:08.873347 asgebsmanager-0.9/
--rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:38:08.872858 asgebsmanager-0.9/PKG-INFO
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:38:08.872101 asgebsmanager-0.9/asgebsmanager.egg-info/
--rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:38:08.000000 asgebsmanager-0.9/asgebsmanager.egg-info/PKG-INFO
--rw-r--r--   0 raghavgupta   (501) staff       (20)      356 2024-04-14 10:38:08.000000 asgebsmanager-0.9/asgebsmanager.egg-info/SOURCES.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 10:38:08.000000 asgebsmanager-0.9/asgebsmanager.egg-info/dependency_links.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       62 2024-04-14 10:38:08.000000 asgebsmanager-0.9/asgebsmanager.egg-info/entry_points.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)      188 2024-04-14 10:38:08.000000 asgebsmanager-0.9/asgebsmanager.egg-info/requires.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       14 2024-04-14 10:38:08.000000 asgebsmanager-0.9/asgebsmanager.egg-info/top_level.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       38 2024-04-14 10:38:08.873454 asgebsmanager-0.9/setup.cfg
--rw-r--r--   0 raghavgupta   (501) staff       (20)      807 2024-04-14 10:38:03.000000 asgebsmanager-0.9/setup.py
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:38:08.866998 asgebsmanager-0.9/src/
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:38:08.871587 asgebsmanager-0.9/src/asgebsmanager/
--rw-r--r--   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:26:40.000000 asgebsmanager-0.9/src/asgebsmanager/__init__.py
--rw-r--r--   0 raghavgupta   (501) staff       (20)     1291 2024-04-14 10:12:34.000000 asgebsmanager-0.9/src/asgebsmanager/__main__.py
--rw-r--r--   0 raghavgupta   (501) staff       (20)     8843 2024-04-14 10:04:04.000000 asgebsmanager-0.9/src/asgebsmanager/ebs_manager.py
--rw-r--r--   0 raghavgupta   (501) staff       (20)     1674 2024-04-14 10:37:33.000000 asgebsmanager-0.9/src/asgebsmanager/mds_utils.py
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:41:28.766338 asgebsmanager-1.1/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:41:28.765803 asgebsmanager-1.1/PKG-INFO
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:41:28.765094 asgebsmanager-1.1/asgebsmanager.egg-info/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:41:28.000000 asgebsmanager-1.1/asgebsmanager.egg-info/PKG-INFO
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      356 2024-04-14 10:41:28.000000 asgebsmanager-1.1/asgebsmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 10:41:28.000000 asgebsmanager-1.1/asgebsmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       62 2024-04-14 10:41:28.000000 asgebsmanager-1.1/asgebsmanager.egg-info/entry_points.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      188 2024-04-14 10:41:28.000000 asgebsmanager-1.1/asgebsmanager.egg-info/requires.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       14 2024-04-14 10:41:28.000000 asgebsmanager-1.1/asgebsmanager.egg-info/top_level.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       38 2024-04-14 10:41:28.766461 asgebsmanager-1.1/setup.cfg
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      807 2024-04-14 10:41:26.000000 asgebsmanager-1.1/setup.py
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:41:28.759303 asgebsmanager-1.1/src/
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:41:28.764391 asgebsmanager-1.1/src/asgebsmanager/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:26:40.000000 asgebsmanager-1.1/src/asgebsmanager/__init__.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     1291 2024-04-14 10:12:34.000000 asgebsmanager-1.1/src/asgebsmanager/__main__.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     8843 2024-04-14 10:40:50.000000 asgebsmanager-1.1/src/asgebsmanager/ebs_manager.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     1620 2024-04-14 10:40:38.000000 asgebsmanager-1.1/src/asgebsmanager/mds_utils.py
```

### Comparing `asgebsmanager-0.9/setup.py` & `asgebsmanager-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os 
 
 setup(
     name = 'asgebsmanager',
-    version = "0.9",
+    version = "1.1",
     author = 'Raghav Gupta',
     description = 'AWS Asg ebs manager',
     packages = find_packages("src"),
     package_dir= {
         "asgebsmanager": os.path.join("src","asgebsmanager")
     },
     install_requires = [
```

### Comparing `asgebsmanager-0.9/src/asgebsmanager/__main__.py` & `asgebsmanager-1.1/src/asgebsmanager/__main__.py`

 * *Files identical despite different names*

### Comparing `asgebsmanager-0.9/src/asgebsmanager/ebs_manager.py` & `asgebsmanager-1.1/src/asgebsmanager/ebs_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 def manage_ebs(args):
     asg_ebs_manager = AsgEbsManager(region=args.region,asg_name=args.asg_name)
 
     # get the current instance az and id
     mds_token = get_imds_token()
 
     az =  get_instance_metadata(mds_token,"placement/availability-zone")
-    instance_id =  get_instance_metadata(mds_token,"instance_id")
+    instance_id =  get_instance_metadata(mds_token,"instance-id")
 
     volume_id = asg_ebs_manager.latest_volume(az)
     # if volume_id is not None, there is chance we can get the available volume
     if volume_id is not None:
         # find the available volume
         volume_id = asg_ebs_manager.latest_volume(az,'available')
         # wait for some other volume to be available
```

### Comparing `asgebsmanager-0.9/src/asgebsmanager/mds_utils.py` & `asgebsmanager-1.1/src/asgebsmanager/mds_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     for attempt in range(retries):
         try:
             url = f"http://169.254.169.254/latest/meta-data/{metadata_key}"
             headers = {
                 "X-aws-ec2-metadata-token": token
             }
             response = requests.get(url, headers=headers)
-            print(response.text,response.status_code)
             if response.status_code == 200:
                 metadata = response.text
                 return metadata
             else:
                 raise Exception("Failed to retrieve instance metadata")
         except Exception as e:
             print(f"Error: {e}. Retrying ({attempt + 1}/{retries}) in {delay} seconds...")
```

