# Comparing `tmp/asgebsmanager-0.6.tar.gz` & `tmp/asgebsmanager-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgebsmanager-0.6.tar", last modified: Sun Apr 14 10:18:28 2024, max compression
+gzip compressed data, was "asgebsmanager-0.7.tar", last modified: Sun Apr 14 10:34:14 2024, max compression
```

## Comparing `asgebsmanager-0.6.tar` & `asgebsmanager-0.7.tar`

### file list

```diff
@@ -1,11 +1,17 @@
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:18:28.437597 asgebsmanager-0.6/
--rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:18:28.437093 asgebsmanager-0.6/PKG-INFO
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:18:28.436493 asgebsmanager-0.6/asgebsmanager.egg-info/
--rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:18:28.000000 asgebsmanager-0.6/asgebsmanager.egg-info/PKG-INFO
--rw-r--r--   0 raghavgupta   (501) staff       (20)      232 2024-04-14 10:18:28.000000 asgebsmanager-0.6/asgebsmanager.egg-info/SOURCES.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 10:18:28.000000 asgebsmanager-0.6/asgebsmanager.egg-info/dependency_links.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       62 2024-04-14 10:18:28.000000 asgebsmanager-0.6/asgebsmanager.egg-info/entry_points.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)      188 2024-04-14 10:18:28.000000 asgebsmanager-0.6/asgebsmanager.egg-info/requires.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 10:18:28.000000 asgebsmanager-0.6/asgebsmanager.egg-info/top_level.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       38 2024-04-14 10:18:28.437962 asgebsmanager-0.6/setup.cfg
--rw-r--r--   0 raghavgupta   (501) staff       (20)      704 2024-04-14 10:18:25.000000 asgebsmanager-0.6/setup.py
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:34:14.484361 asgebsmanager-0.7/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:34:14.483887 asgebsmanager-0.7/PKG-INFO
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:34:14.483286 asgebsmanager-0.7/asgebsmanager.egg-info/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:34:14.000000 asgebsmanager-0.7/asgebsmanager.egg-info/PKG-INFO
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      356 2024-04-14 10:34:14.000000 asgebsmanager-0.7/asgebsmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 10:34:14.000000 asgebsmanager-0.7/asgebsmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       62 2024-04-14 10:34:14.000000 asgebsmanager-0.7/asgebsmanager.egg-info/entry_points.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      188 2024-04-14 10:34:14.000000 asgebsmanager-0.7/asgebsmanager.egg-info/requires.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       14 2024-04-14 10:34:14.000000 asgebsmanager-0.7/asgebsmanager.egg-info/top_level.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       38 2024-04-14 10:34:14.484466 asgebsmanager-0.7/setup.cfg
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      807 2024-04-14 10:34:07.000000 asgebsmanager-0.7/setup.py
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:34:14.478027 asgebsmanager-0.7/src/
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:34:14.482793 asgebsmanager-0.7/src/asgebsmanager/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:26:40.000000 asgebsmanager-0.7/src/asgebsmanager/__init__.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     1291 2024-04-14 10:12:34.000000 asgebsmanager-0.7/src/asgebsmanager/__main__.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     8843 2024-04-14 10:04:04.000000 asgebsmanager-0.7/src/asgebsmanager/ebs_manager.py
+-rw-r--r--   0 raghavgupta   (501) staff       (20)     1620 2024-04-14 10:33:58.000000 asgebsmanager-0.7/src/asgebsmanager/mds_utils.py
```

