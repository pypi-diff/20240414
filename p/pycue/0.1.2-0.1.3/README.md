# Comparing `tmp/pycue-0.1.2.tar.gz` & `tmp/pycue-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycue-0.1.2.tar", last modified: Sun Feb 26 08:55:11 2023, max compression
+gzip compressed data, was "pycue-0.1.3.tar", last modified: Sun Apr 14 08:48:19 2024, max compression
```

## Comparing `pycue-0.1.2.tar` & `pycue-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2023-02-26 08:55:11.788648 pycue-0.1.2/
--rw-r--r--   0 miki      (1000) miki      (1000)     1051 2023-02-26 08:44:07.000000 pycue-0.1.2/LICENSE.txt
--rw-r--r--   0 miki      (1000) miki      (1000)      130 2023-02-26 08:46:23.000000 pycue-0.1.2/MANIFEST.in
--rw-r--r--   0 miki      (1000) miki      (1000)     1425 2023-02-26 08:55:11.788648 pycue-0.1.2/PKG-INFO
--rw-r--r--   0 miki      (1000) miki      (1000)      707 2023-02-26 08:44:07.000000 pycue-0.1.2/README.md
--rw-r--r--   0 miki      (1000) miki      (1000)     1850 2023-02-26 08:46:55.000000 pycue-0.1.2/cue.py
--rw-r--r--   0 miki      (1000) miki      (1000)       66 2023-02-26 08:44:07.000000 pycue-0.1.2/dev-requirements.txt
-drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2023-02-26 08:55:11.788648 pycue-0.1.2/pycue.egg-info/
--rw-r--r--   0 miki      (1000) miki      (1000)     1425 2023-02-26 08:55:11.000000 pycue-0.1.2/pycue.egg-info/PKG-INFO
--rw-r--r--   0 miki      (1000) miki      (1000)      359 2023-02-26 08:55:11.000000 pycue-0.1.2/pycue.egg-info/SOURCES.txt
--rw-r--r--   0 miki      (1000) miki      (1000)        1 2023-02-26 08:55:11.000000 pycue-0.1.2/pycue.egg-info/dependency_links.txt
--rw-r--r--   0 miki      (1000) miki      (1000)       12 2023-02-26 08:55:11.000000 pycue-0.1.2/pycue.egg-info/requires.txt
--rw-r--r--   0 miki      (1000) miki      (1000)        4 2023-02-26 08:55:11.000000 pycue-0.1.2/pycue.egg-info/top_level.txt
--rw-r--r--   0 miki      (1000) miki      (1000)       12 2023-02-26 08:44:07.000000 pycue-0.1.2/requirements.txt
--rw-r--r--   0 miki      (1000) miki      (1000)       38 2023-02-26 08:55:11.788648 pycue-0.1.2/setup.cfg
--rw-r--r--   0 miki      (1000) miki      (1000)     1603 2023-02-26 08:44:07.000000 pycue-0.1.2/setup.py
-drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2023-02-26 08:55:11.788648 pycue-0.1.2/tests/
-drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2023-02-26 08:55:11.788648 pycue-0.1.2/tests/__pycache__/
--rw-r--r--   0 miki      (1000) miki      (1000)     5175 2023-02-26 08:53:25.000000 pycue-0.1.2/tests/__pycache__/test_cue.cpython-311-pytest-7.2.1.pyc
--rw-r--r--   0 miki      (1000) miki      (1000)      101 2023-02-26 08:44:07.000000 pycue-0.1.2/tests/data_bad.yml
--rw-r--r--   0 miki      (1000) miki      (1000)      103 2023-02-26 08:44:07.000000 pycue-0.1.2/tests/data_ok.yml
--rw-r--r--   0 miki      (1000) miki      (1000)      115 2023-02-26 08:44:07.000000 pycue-0.1.2/tests/schema.cue
--rw-r--r--   0 miki      (1000) miki      (1000)     1321 2023-02-26 08:44:07.000000 pycue-0.1.2/tests/test_cue.py
+drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2024-04-14 08:48:19.361795 pycue-0.1.3/
+-rw-r--r--   0 miki      (1000) miki      (1000)    11342 2024-04-14 08:47:29.000000 pycue-0.1.3/LICENSE
+-rw-r--r--   0 miki      (1000) miki      (1000)     1051 2024-04-14 08:37:26.000000 pycue-0.1.3/LICENSE.txt
+-rw-r--r--   0 miki      (1000) miki      (1000)      130 2024-04-14 08:37:26.000000 pycue-0.1.3/MANIFEST.in
+-rw-r--r--   0 miki      (1000) miki      (1000)     6325 2024-04-14 08:48:19.361795 pycue-0.1.3/PKG-INFO
+-rw-r--r--   0 miki      (1000) miki      (1000)     5558 2021-05-25 13:09:38.000000 pycue-0.1.3/README.md
+-rw-r--r--   0 miki      (1000) miki      (1000)     1877 2024-04-14 08:46:18.000000 pycue-0.1.3/cue.py
+-rw-r--r--   0 miki      (1000) miki      (1000)       47 2024-04-14 08:42:36.000000 pycue-0.1.3/dev-requirements.txt
+drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2024-04-14 08:48:19.361795 pycue-0.1.3/pycue.egg-info/
+-rw-r--r--   0 miki      (1000) miki      (1000)     6325 2024-04-14 08:48:19.000000 pycue-0.1.3/pycue.egg-info/PKG-INFO
+-rw-r--r--   0 miki      (1000) miki      (1000)      367 2024-04-14 08:48:19.000000 pycue-0.1.3/pycue.egg-info/SOURCES.txt
+-rw-r--r--   0 miki      (1000) miki      (1000)        1 2024-04-14 08:48:19.000000 pycue-0.1.3/pycue.egg-info/dependency_links.txt
+-rw-r--r--   0 miki      (1000) miki      (1000)       12 2024-04-14 08:48:19.000000 pycue-0.1.3/pycue.egg-info/requires.txt
+-rw-r--r--   0 miki      (1000) miki      (1000)        4 2024-04-14 08:48:19.000000 pycue-0.1.3/pycue.egg-info/top_level.txt
+-rw-r--r--   0 miki      (1000) miki      (1000)       14 2024-04-14 08:38:26.000000 pycue-0.1.3/requirements.txt
+-rw-r--r--   0 miki      (1000) miki      (1000)       38 2024-04-14 08:48:19.361795 pycue-0.1.3/setup.cfg
+-rw-r--r--   0 miki      (1000) miki      (1000)     1603 2024-04-14 08:37:26.000000 pycue-0.1.3/setup.py
+drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2024-04-14 08:48:19.361795 pycue-0.1.3/tests/
+drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2024-04-14 08:48:19.361795 pycue-0.1.3/tests/__pycache__/
+-rw-r--r--   0 miki      (1000) miki      (1000)     4279 2024-04-14 08:44:40.000000 pycue-0.1.3/tests/__pycache__/test_cue.cpython-312-pytest-8.1.1.pyc
+-rw-r--r--   0 miki      (1000) miki      (1000)      101 2024-04-14 08:37:26.000000 pycue-0.1.3/tests/data_bad.yml
+-rw-r--r--   0 miki      (1000) miki      (1000)      103 2024-04-14 08:37:26.000000 pycue-0.1.3/tests/data_ok.yml
+-rw-r--r--   0 miki      (1000) miki      (1000)      115 2024-04-14 08:37:26.000000 pycue-0.1.3/tests/schema.cue
+-rw-r--r--   0 miki      (1000) miki      (1000)     1321 2024-04-14 08:37:26.000000 pycue-0.1.3/tests/test_cue.py
```

### Comparing `pycue-0.1.2/LICENSE.txt` & `pycue-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycue-0.1.2/cue.py` & `pycue-0.1.3/cue.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """cue is a Python wrapper for https://cuelang.org"""
 from os import environ
 from subprocess import run
 from tempfile import NamedTemporaryFile
 
 import yaml
 
-__version__ = '0.1.2'
+__version__ = '0.1.3'
+__cue__version__ = '0.4.0'
 
 
 class Error(Exception):
     pass
 
 
 cue_exe = environ.get('CUE_EXE', 'cue')
```

### Comparing `pycue-0.1.2/setup.py` & `pycue-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `pycue-0.1.2/tests/test_cue.py` & `pycue-0.1.3/tests/test_cue.py`

 * *Files identical despite different names*

