# Comparing `tmp/givapi-0.2.0.tar.gz` & `tmp/givapi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "givapi-0.2.0.tar", max compression
+gzip compressed data, was "givapi-0.3.0.tar", max compression
```

## Comparing `givapi-0.2.0.tar` & `givapi-0.3.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    35149 2024-04-01 16:32:19.487008 givapi-0.2.0/LICENSE
--rw-r--r--   0        0        0     3515 2024-04-01 16:32:19.487008 givapi-0.2.0/givapi.py
--rw-r--r--   0        0        0      396 2024-04-01 16:32:19.487008 givapi-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      704 1970-01-01 00:00:00.000000 givapi-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-14 16:41:58.683844 givapi-0.3.0/LICENSE
+-rw-r--r--   0        0        0     6412 2024-04-14 16:41:58.683844 givapi-0.3.0/givapi.py
+-rw-r--r--   0        0        0      417 2024-04-14 16:41:58.683844 givapi-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 givapi-0.3.0/PKG-INFO
```

### Comparing `givapi-0.2.0/LICENSE` & `givapi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `givapi-0.2.0/PKG-INFO` & `givapi-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: GivAPI
-Version: 0.2.0
-Summary: Pulls data from the GivEnergy API
+Version: 0.3.0
+Summary: Pulls data from or sends commands to the GivEnergy API
 License: GPL-3.0
 Author: Wilbur Williams
 Author-email: contact@wilburwilliams.uk
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

