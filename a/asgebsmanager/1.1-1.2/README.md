# Comparing `tmp/asgebsmanager-1.1.tar.gz` & `tmp/asgebsmanager-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgebsmanager-1.1.tar", last modified: Sun Apr 14 10:41:28 2024, max compression
+gzip compressed data, was "asgebsmanager-1.2.tar", last modified: Sun Apr 14 10:43:42 2024, max compression
```

## Comparing `asgebsmanager-1.1.tar` & `asgebsmanager-1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:41:28.766338 asgebsmanager-1.1/
--rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:41:28.765803 asgebsmanager-1.1/PKG-INFO
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:41:28.765094 asgebsmanager-1.1/asgebsmanager.egg-info/
--rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:41:28.000000 asgebsmanager-1.1/asgebsmanager.egg-info/PKG-INFO
--rw-r--r--   0 raghavgupta   (501) staff       (20)      356 2024-04-14 10:41:28.000000 asgebsmanager-1.1/asgebsmanager.egg-info/SOURCES.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 10:41:28.000000 asgebsmanager-1.1/asgebsmanager.egg-info/dependency_links.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       62 2024-04-14 10:41:28.000000 asgebsmanager-1.1/asgebsmanager.egg-info/entry_points.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)      188 2024-04-14 10:41:28.000000 asgebsmanager-1.1/asgebsmanager.egg-info/requires.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       14 2024-04-14 10:41:28.000000 asgebsmanager-1.1/asgebsmanager.egg-info/top_level.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       38 2024-04-14 10:41:28.766461 asgebsmanager-1.1/setup.cfg
--rw-r--r--   0 raghavgupta   (501) staff       (20)      807 2024-04-14 10:41:26.000000 asgebsmanager-1.1/setup.py
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:41:28.759303 asgebsmanager-1.1/src/
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:41:28.764391 asgebsmanager-1.1/src/asgebsmanager/
--rw-r--r--   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:26:40.000000 asgebsmanager-1.1/src/asgebsmanager/__init__.py
--rw-r--r--   0 raghavgupta   (501) staff       (20)     1291 2024-04-14 10:12:34.000000 asgebsmanager-1.1/src/asgebsmanager/__main__.py
--rw-r--r--   0 raghavgupta   (501) staff       (20)     8843 2024-04-14 10:40:50.000000 asgebsmanager-1.1/src/asgebsmanager/ebs_manager.py
--rw-r--r--   0 raghavgupta   (501) staff       (20)     1620 2024-04-14 10:40:38.000000 asgebsmanager-1.1/src/asgebsmanager/mds_utils.py
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:43:42.807692 asgebsmanager-1.2/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:43:42.807147 asgebsmanager-1.2/PKG-INFO
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:43:42.806510 asgebsmanager-1.2/asgebsmanager.egg-info/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:43:42.000000 asgebsmanager-1.2/asgebsmanager.egg-info/PKG-INFO
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      356 2024-04-14 10:43:42.000000 asgebsmanager-1.2/asgebsmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 10:43:42.000000 asgebsmanager-1.2/asgebsmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       62 2024-04-14 10:43:42.000000 asgebsmanager-1.2/asgebsmanager.egg-info/entry_points.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      188 2024-04-14 10:43:42.000000 asgebsmanager-1.2/asgebsmanager.egg-info/requires.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       14 2024-04-14 10:43:42.000000 asgebsmanager-1.2/asgebsmanager.egg-info/top_level.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       38 2024-04-14 10:43:42.807834 asgebsmanager-1.2/setup.cfg
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      807 2024-04-14 10:43:26.000000 asgebsmanager-1.2/setup.py
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:43:42.801895 asgebsmanager-1.2/src/
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:43:42.806027 asgebsmanager-1.2/src/asgebsmanager/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:26:40.000000 asgebsmanager-1.2/src/asgebsmanager/__init__.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     1291 2024-04-14 10:12:34.000000 asgebsmanager-1.2/src/asgebsmanager/__main__.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     8848 2024-04-14 10:43:18.000000 asgebsmanager-1.2/src/asgebsmanager/ebs_manager.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     1620 2024-04-14 10:40:38.000000 asgebsmanager-1.2/src/asgebsmanager/mds_utils.py
```

### Comparing `asgebsmanager-1.1/setup.py` & `asgebsmanager-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os 
 
 setup(
     name = 'asgebsmanager',
-    version = "1.1",
+    version = "1.2",
     author = 'Raghav Gupta',
     description = 'AWS Asg ebs manager',
     packages = find_packages("src"),
     package_dir= {
         "asgebsmanager": os.path.join("src","asgebsmanager")
     },
     install_requires = [
```

### Comparing `asgebsmanager-1.1/src/asgebsmanager/__main__.py` & `asgebsmanager-1.2/src/asgebsmanager/__main__.py`

 * *Files identical despite different names*

### Comparing `asgebsmanager-1.1/src/asgebsmanager/ebs_manager.py` & `asgebsmanager-1.2/src/asgebsmanager/ebs_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         self.asg_name = asg_name
         self.session = boto3.Session(region_name=region)
         self.ec2_client = self.session.client('ec2')
 
     def __get_name():
         return 'AsgEbsManager'
     
-    def latest_volume(self,az,state):
+    def latest_volume(self,az,state=None):
         status = ["available","in-use"] if state is None else [state]
         volumes = self.ec2_client.client.describe_volumes(
             Filters=[
                 {
                     'Name': 'tag:BelongsTo',
                     'Values': [
                         self.asg_name,
```

### Comparing `asgebsmanager-1.1/src/asgebsmanager/mds_utils.py` & `asgebsmanager-1.2/src/asgebsmanager/mds_utils.py`

 * *Files identical despite different names*

