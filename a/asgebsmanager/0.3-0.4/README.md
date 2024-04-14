# Comparing `tmp/asgebsmanager-0.3.tar.gz` & `tmp/asgebsmanager-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgebsmanager-0.3.tar", last modified: Sun Apr 14 10:00:31 2024, max compression
+gzip compressed data, was "asgebsmanager-0.4.tar", last modified: Sun Apr 14 10:07:38 2024, max compression
```

## Comparing `asgebsmanager-0.3.tar` & `asgebsmanager-0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:00:31.468109 asgebsmanager-0.3/
--rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:00:31.467605 asgebsmanager-0.3/PKG-INFO
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:00:31.466966 asgebsmanager-0.3/asgebsmanager.egg-info/
--rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:00:31.000000 asgebsmanager-0.3/asgebsmanager.egg-info/PKG-INFO
--rw-r--r--   0 raghavgupta   (501) staff       (20)      232 2024-04-14 10:00:31.000000 asgebsmanager-0.3/asgebsmanager.egg-info/SOURCES.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 10:00:31.000000 asgebsmanager-0.3/asgebsmanager.egg-info/dependency_links.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       62 2024-04-14 10:00:31.000000 asgebsmanager-0.3/asgebsmanager.egg-info/entry_points.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)      188 2024-04-14 10:00:31.000000 asgebsmanager-0.3/asgebsmanager.egg-info/requires.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 10:00:31.000000 asgebsmanager-0.3/asgebsmanager.egg-info/top_level.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       38 2024-04-14 10:00:31.468229 asgebsmanager-0.3/setup.cfg
--rw-r--r--   0 raghavgupta   (501) staff       (20)      748 2024-04-14 10:00:25.000000 asgebsmanager-0.3/setup.py
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:07:38.006919 asgebsmanager-0.4/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:07:38.006501 asgebsmanager-0.4/PKG-INFO
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:07:38.005651 asgebsmanager-0.4/asgebsmanager.egg-info/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:07:37.000000 asgebsmanager-0.4/asgebsmanager.egg-info/PKG-INFO
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      232 2024-04-14 10:07:37.000000 asgebsmanager-0.4/asgebsmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 10:07:37.000000 asgebsmanager-0.4/asgebsmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       48 2024-04-14 10:07:37.000000 asgebsmanager-0.4/asgebsmanager.egg-info/entry_points.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      188 2024-04-14 10:07:37.000000 asgebsmanager-0.4/asgebsmanager.egg-info/requires.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 10:07:37.000000 asgebsmanager-0.4/asgebsmanager.egg-info/top_level.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       38 2024-04-14 10:07:38.007218 asgebsmanager-0.4/setup.cfg
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      734 2024-04-14 10:07:35.000000 asgebsmanager-0.4/setup.py
```

### Comparing `asgebsmanager-0.3/setup.py` & `asgebsmanager-0.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'asgebsmanager',
-    version = "0.3",
+    version = "0.4",
     author = 'Raghav Gupta',
     description = 'AWS Asg ebs manager',
     packages = find_packages(include=["src","VERSION","requirements.txt"]),
     install_requires = [
         "boto3==1.34.84",
         "botocore==1.34.84",
         "certifi==2024.2.2",
@@ -18,9 +18,9 @@
         "s3transfer==0.10.1",
         "six==1.16.0",
         "urllib3"
     ],
     classifiers=[
         "Programming Language :: Python :: 3"
     ],
-    entry_points = {'console_scripts': ['asgebsmanager = asgebsmanager.__main__:main'],}
+    entry_points = {'console_scripts': ['asgebsmanager = __main__:main'],}
 )
```

