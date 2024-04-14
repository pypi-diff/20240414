# Comparing `tmp/cdk-events-notify-2.2.96.tar.gz` & `tmp/cdk-events-notify-2.2.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-events-notify-2.2.96.tar", last modified: Sat Apr 13 00:11:05 2024, max compression
+gzip compressed data, was "cdk-events-notify-2.2.97.tar", last modified: Sun Apr 14 00:15:41 2024, max compression
```

## Comparing `cdk-events-notify-2.2.96.tar` & `cdk-events-notify-2.2.97.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:11:05.694396 cdk-events-notify-2.2.96/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-13 00:10:55.000000 cdk-events-notify-2.2.96/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-13 00:10:55.000000 cdk-events-notify-2.2.96/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-13 00:11:05.694396 cdk-events-notify-2.2.96/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-13 00:10:55.000000 cdk-events-notify-2.2.96/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-13 00:10:55.000000 cdk-events-notify-2.2.96/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 00:11:05.694396 cdk-events-notify-2.2.96/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-13 00:10:55.000000 cdk-events-notify-2.2.96/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:11:05.690396 cdk-events-notify-2.2.96/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:11:05.690396 cdk-events-notify-2.2.96/src/cdk_events_notify/
--rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-04-13 00:10:55.000000 cdk-events-notify-2.2.96/src/cdk_events_notify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:11:05.694396 cdk-events-notify-2.2.96/src/cdk_events_notify/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-13 00:10:55.000000 cdk-events-notify-2.2.96/src/cdk_events_notify/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24938 2024-04-13 00:10:55.000000 cdk-events-notify-2.2.96/src/cdk_events_notify/_jsii/cdk-events-notify@2.2.96.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 00:10:55.000000 cdk-events-notify-2.2.96/src/cdk_events_notify/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:11:05.694396 cdk-events-notify-2.2.96/src/cdk_events_notify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-13 00:11:05.000000 cdk-events-notify-2.2.96/src/cdk_events_notify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-13 00:11:05.000000 cdk-events-notify-2.2.96/src/cdk_events_notify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 00:11:05.000000 cdk-events-notify-2.2.96/src/cdk_events_notify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-13 00:11:05.000000 cdk-events-notify-2.2.96/src/cdk_events_notify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-13 00:11:05.000000 cdk-events-notify-2.2.96/src/cdk_events_notify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:15:41.990027 cdk-events-notify-2.2.97/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-14 00:15:26.000000 cdk-events-notify-2.2.97/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-14 00:15:26.000000 cdk-events-notify-2.2.97/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-14 00:15:41.990027 cdk-events-notify-2.2.97/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-04-14 00:15:26.000000 cdk-events-notify-2.2.97/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-14 00:15:26.000000 cdk-events-notify-2.2.97/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 00:15:41.994027 cdk-events-notify-2.2.97/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-14 00:15:26.000000 cdk-events-notify-2.2.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:15:41.990027 cdk-events-notify-2.2.97/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:15:41.990027 cdk-events-notify-2.2.97/src/cdk_events_notify/
+-rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-04-14 00:15:26.000000 cdk-events-notify-2.2.97/src/cdk_events_notify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:15:41.990027 cdk-events-notify-2.2.97/src/cdk_events_notify/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-14 00:15:26.000000 cdk-events-notify-2.2.97/src/cdk_events_notify/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24938 2024-04-14 00:15:26.000000 cdk-events-notify-2.2.97/src/cdk_events_notify/_jsii/cdk-events-notify@2.2.97.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 00:15:26.000000 cdk-events-notify-2.2.97/src/cdk_events_notify/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:15:41.990027 cdk-events-notify-2.2.97/src/cdk_events_notify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-14 00:15:41.000000 cdk-events-notify-2.2.97/src/cdk_events_notify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-14 00:15:41.000000 cdk-events-notify-2.2.97/src/cdk_events_notify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 00:15:41.000000 cdk-events-notify-2.2.97/src/cdk_events_notify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-14 00:15:41.000000 cdk-events-notify-2.2.97/src/cdk_events_notify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-14 00:15:41.000000 cdk-events-notify-2.2.97/src/cdk_events_notify.egg-info/top_level.txt
```

### Comparing `cdk-events-notify-2.2.96/LICENSE` & `cdk-events-notify-2.2.97/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-events-notify-2.2.96/PKG-INFO` & `cdk-events-notify-2.2.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-events-notify
-Version: 2.2.96
+Version: 2.2.97
 Summary: The Events Notify AWS Construct lib for AWS CDK
 Home-page: https://github.com/neilkuan/cdk-events-notify.git
 Author: Neil Kuan<guan840912@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neilkuan/cdk-events-notify.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-events-notify-2.2.96/README.md` & `cdk-events-notify-2.2.97/README.md`

 * *Files identical despite different names*

### Comparing `cdk-events-notify-2.2.96/setup.py` & `cdk-events-notify-2.2.97/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-events-notify",
-    "version": "2.2.96",
+    "version": "2.2.97",
     "description": "The Events Notify AWS Construct lib for AWS CDK",
     "license": "Apache-2.0",
     "url": "https://github.com/neilkuan/cdk-events-notify.git",
     "long_description_content_type": "text/markdown",
     "author": "Neil Kuan<guan840912@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_events_notify",
         "cdk_events_notify._jsii"
     ],
     "package_data": {
         "cdk_events_notify._jsii": [
-            "cdk-events-notify@2.2.96.jsii.tgz"
+            "cdk-events-notify@2.2.97.jsii.tgz"
         ],
         "cdk_events_notify": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-events-notify-2.2.96/src/cdk_events_notify/__init__.py` & `cdk-events-notify-2.2.97/src/cdk_events_notify/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-events-notify-2.2.96/src/cdk_events_notify.egg-info/PKG-INFO` & `cdk-events-notify-2.2.97/src/cdk_events_notify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-events-notify
-Version: 2.2.96
+Version: 2.2.97
 Summary: The Events Notify AWS Construct lib for AWS CDK
 Home-page: https://github.com/neilkuan/cdk-events-notify.git
 Author: Neil Kuan<guan840912@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neilkuan/cdk-events-notify.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

