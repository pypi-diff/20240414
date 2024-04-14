# Comparing `tmp/asgebsmanager-0.1.tar.gz` & `tmp/asgebsmanager-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgebsmanager-0.1.tar", last modified: Sun Apr 14 09:50:04 2024, max compression
+gzip compressed data, was "asgebsmanager-0.2.tar", last modified: Sun Apr 14 09:56:08 2024, max compression
```

## Comparing `asgebsmanager-0.1.tar` & `asgebsmanager-0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 09:50:04.761583 asgebsmanager-0.1/
--rw-r--r--   0 raghavgupta   (501) staff       (20)      513 2024-04-14 09:50:04.761099 asgebsmanager-0.1/PKG-INFO
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 09:50:04.759846 asgebsmanager-0.1/asgebsmanager.egg-info/
--rw-r--r--   0 raghavgupta   (501) staff       (20)      513 2024-04-14 09:50:04.000000 asgebsmanager-0.1/asgebsmanager.egg-info/PKG-INFO
--rw-r--r--   0 raghavgupta   (501) staff       (20)      232 2024-04-14 09:50:04.000000 asgebsmanager-0.1/asgebsmanager.egg-info/SOURCES.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 09:50:04.000000 asgebsmanager-0.1/asgebsmanager.egg-info/dependency_links.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       62 2024-04-14 09:50:04.000000 asgebsmanager-0.1/asgebsmanager.egg-info/entry_points.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)      195 2024-04-14 09:50:04.000000 asgebsmanager-0.1/asgebsmanager.egg-info/requires.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 09:50:04.000000 asgebsmanager-0.1/asgebsmanager.egg-info/top_level.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       38 2024-04-14 09:50:04.761697 asgebsmanager-0.1/setup.cfg
--rw-r--r--   0 raghavgupta   (501) staff       (20)      755 2024-04-14 09:49:58.000000 asgebsmanager-0.1/setup.py
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 09:56:08.978779 asgebsmanager-0.2/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 09:56:08.978289 asgebsmanager-0.2/PKG-INFO
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 09:56:08.977660 asgebsmanager-0.2/asgebsmanager.egg-info/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 09:56:08.000000 asgebsmanager-0.2/asgebsmanager.egg-info/PKG-INFO
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      232 2024-04-14 09:56:08.000000 asgebsmanager-0.2/asgebsmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 09:56:08.000000 asgebsmanager-0.2/asgebsmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       62 2024-04-14 09:56:08.000000 asgebsmanager-0.2/asgebsmanager.egg-info/entry_points.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      188 2024-04-14 09:56:08.000000 asgebsmanager-0.2/asgebsmanager.egg-info/requires.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 09:56:08.000000 asgebsmanager-0.2/asgebsmanager.egg-info/top_level.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       38 2024-04-14 09:56:08.978903 asgebsmanager-0.2/setup.cfg
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      748 2024-04-14 09:56:06.000000 asgebsmanager-0.2/setup.py
```

### Comparing `asgebsmanager-0.1/setup.py` & `asgebsmanager-0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'asgebsmanager',
-    version = "0.1",
+    version = "0.2",
     author = 'Raghav Gupta',
     description = 'AWS Asg ebs manager',
     packages = find_packages(include=["src","VERSION","requirements.txt"]),
     install_requires = [
         "boto3==1.34.84",
         "botocore==1.34.84",
         "certifi==2024.2.2",
         "charset-normalizer==3.3.2",
         "idna==3.7",
         "jmespath==1.0.1",
         "python-dateutil==2.9.0.post0",
         "requests==2.31.0",
         "s3transfer==0.10.1",
         "six==1.16.0",
-        "urllib3==2.2.1"
+        "urllib3"
     ],
     classifiers=[
         "Programming Language :: Python :: 3"
     ],
     entry_points = {'console_scripts': ['asgebsmanager = asgebsmanager.__main__:main'],}
 )
```

