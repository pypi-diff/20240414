# Comparing `tmp/asgebsmanager-0.2.tar.gz` & `tmp/asgebsmanager-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgebsmanager-0.2.tar", last modified: Sun Apr 14 09:56:08 2024, max compression
+gzip compressed data, was "asgebsmanager-0.3.tar", last modified: Sun Apr 14 10:00:31 2024, max compression
```

## Comparing `asgebsmanager-0.2.tar` & `asgebsmanager-0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 09:56:08.978779 asgebsmanager-0.2/
--rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 09:56:08.978289 asgebsmanager-0.2/PKG-INFO
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 09:56:08.977660 asgebsmanager-0.2/asgebsmanager.egg-info/
--rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 09:56:08.000000 asgebsmanager-0.2/asgebsmanager.egg-info/PKG-INFO
--rw-r--r--   0 raghavgupta   (501) staff       (20)      232 2024-04-14 09:56:08.000000 asgebsmanager-0.2/asgebsmanager.egg-info/SOURCES.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 09:56:08.000000 asgebsmanager-0.2/asgebsmanager.egg-info/dependency_links.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       62 2024-04-14 09:56:08.000000 asgebsmanager-0.2/asgebsmanager.egg-info/entry_points.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)      188 2024-04-14 09:56:08.000000 asgebsmanager-0.2/asgebsmanager.egg-info/requires.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 09:56:08.000000 asgebsmanager-0.2/asgebsmanager.egg-info/top_level.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       38 2024-04-14 09:56:08.978903 asgebsmanager-0.2/setup.cfg
--rw-r--r--   0 raghavgupta   (501) staff       (20)      748 2024-04-14 09:56:06.000000 asgebsmanager-0.2/setup.py
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:00:31.468109 asgebsmanager-0.3/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:00:31.467605 asgebsmanager-0.3/PKG-INFO
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:00:31.466966 asgebsmanager-0.3/asgebsmanager.egg-info/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:00:31.000000 asgebsmanager-0.3/asgebsmanager.egg-info/PKG-INFO
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      232 2024-04-14 10:00:31.000000 asgebsmanager-0.3/asgebsmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 10:00:31.000000 asgebsmanager-0.3/asgebsmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       62 2024-04-14 10:00:31.000000 asgebsmanager-0.3/asgebsmanager.egg-info/entry_points.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      188 2024-04-14 10:00:31.000000 asgebsmanager-0.3/asgebsmanager.egg-info/requires.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 10:00:31.000000 asgebsmanager-0.3/asgebsmanager.egg-info/top_level.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       38 2024-04-14 10:00:31.468229 asgebsmanager-0.3/setup.cfg
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      748 2024-04-14 10:00:25.000000 asgebsmanager-0.3/setup.py
```

### Comparing `asgebsmanager-0.2/setup.py` & `asgebsmanager-0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'asgebsmanager',
-    version = "0.2",
+    version = "0.3",
     author = 'Raghav Gupta',
     description = 'AWS Asg ebs manager',
     packages = find_packages(include=["src","VERSION","requirements.txt"]),
     install_requires = [
         "boto3==1.34.84",
         "botocore==1.34.84",
         "certifi==2024.2.2",
```

