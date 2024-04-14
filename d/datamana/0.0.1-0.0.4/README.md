# Comparing `tmp/datamana-0.0.1.tar.gz` & `tmp/datamana-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datamana-0.0.1.tar", last modified: Sat Apr  6 01:23:34 2024, max compression
+gzip compressed data, was "datamana-0.0.4.tar", last modified: Sun Apr 14 09:23:27 2024, max compression
```

## Comparing `datamana-0.0.1.tar` & `datamana-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:23:34.260304 datamana-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-06 01:23:29.000000 datamana-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-06 01:23:34.260304 datamana-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 01:23:29.000000 datamana-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:23:34.256304 datamana-0.0.1/datamana/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 01:23:29.000000 datamana-0.0.1/datamana/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-06 01:23:29.000000 datamana-0.0.1/datamana/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:23:34.256304 datamana-0.0.1/datamana.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-06 01:23:34.000000 datamana-0.0.1/datamana.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-06 01:23:34.000000 datamana-0.0.1/datamana.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 01:23:34.000000 datamana-0.0.1/datamana.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-06 01:23:34.000000 datamana-0.0.1/datamana.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-06 01:23:34.000000 datamana-0.0.1/datamana.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 01:23:34.260304 datamana-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-06 01:23:29.000000 datamana-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:23:27.972068 datamana-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-14 09:23:17.000000 datamana-0.0.4/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-14 09:23:17.000000 datamana-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-14 09:23:27.968068 datamana-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 09:23:17.000000 datamana-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:23:27.968068 datamana-0.0.4/csrc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 09:23:17.000000 datamana-0.0.4/csrc/mqueue.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-14 09:23:17.000000 datamana-0.0.4/csrc/semaphore.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:23:27.968068 datamana-0.0.4/datamana/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 09:23:17.000000 datamana-0.0.4/datamana/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 09:23:17.000000 datamana-0.0.4/datamana/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-14 09:23:17.000000 datamana-0.0.4/datamana/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 09:23:27.968068 datamana-0.0.4/datamana.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-14 09:23:27.000000 datamana-0.0.4/datamana.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-14 09:23:27.000000 datamana-0.0.4/datamana.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 09:23:27.000000 datamana-0.0.4/datamana.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 09:23:27.000000 datamana-0.0.4/datamana.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 09:23:27.000000 datamana-0.0.4/datamana.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-14 09:23:17.000000 datamana-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 09:23:27.972068 datamana-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-14 09:23:17.000000 datamana-0.0.4/setup.py
```

### Comparing `datamana-0.0.1/LICENSE` & `datamana-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datamana-0.0.1/datamana/torch.py` & `datamana-0.0.4/datamana/torch.py`

 * *Files identical despite different names*

