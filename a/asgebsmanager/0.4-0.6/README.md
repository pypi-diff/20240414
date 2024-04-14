# Comparing `tmp/asgebsmanager-0.4.tar.gz` & `tmp/asgebsmanager-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgebsmanager-0.4.tar", last modified: Sun Apr 14 10:07:38 2024, max compression
+gzip compressed data, was "asgebsmanager-0.6.tar", last modified: Sun Apr 14 10:18:28 2024, max compression
```

## Comparing `asgebsmanager-0.4.tar` & `asgebsmanager-0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:07:38.006919 asgebsmanager-0.4/
--rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:07:38.006501 asgebsmanager-0.4/PKG-INFO
-drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:07:38.005651 asgebsmanager-0.4/asgebsmanager.egg-info/
--rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:07:37.000000 asgebsmanager-0.4/asgebsmanager.egg-info/PKG-INFO
--rw-r--r--   0 raghavgupta   (501) staff       (20)      232 2024-04-14 10:07:37.000000 asgebsmanager-0.4/asgebsmanager.egg-info/SOURCES.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 10:07:37.000000 asgebsmanager-0.4/asgebsmanager.egg-info/dependency_links.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       48 2024-04-14 10:07:37.000000 asgebsmanager-0.4/asgebsmanager.egg-info/entry_points.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)      188 2024-04-14 10:07:37.000000 asgebsmanager-0.4/asgebsmanager.egg-info/requires.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 10:07:37.000000 asgebsmanager-0.4/asgebsmanager.egg-info/top_level.txt
--rw-r--r--   0 raghavgupta   (501) staff       (20)       38 2024-04-14 10:07:38.007218 asgebsmanager-0.4/setup.cfg
--rw-r--r--   0 raghavgupta   (501) staff       (20)      734 2024-04-14 10:07:35.000000 asgebsmanager-0.4/setup.py
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:18:28.437597 asgebsmanager-0.6/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:18:28.437093 asgebsmanager-0.6/PKG-INFO
+drwxr-xr-x   0 raghavgupta   (501) staff       (20)        0 2024-04-14 10:18:28.436493 asgebsmanager-0.6/asgebsmanager.egg-info/
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      506 2024-04-14 10:18:28.000000 asgebsmanager-0.6/asgebsmanager.egg-info/PKG-INFO
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      232 2024-04-14 10:18:28.000000 asgebsmanager-0.6/asgebsmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 10:18:28.000000 asgebsmanager-0.6/asgebsmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       62 2024-04-14 10:18:28.000000 asgebsmanager-0.6/asgebsmanager.egg-info/entry_points.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      188 2024-04-14 10:18:28.000000 asgebsmanager-0.6/asgebsmanager.egg-info/requires.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)        1 2024-04-14 10:18:28.000000 asgebsmanager-0.6/asgebsmanager.egg-info/top_level.txt
+-rw-r--r--   0 raghavgupta   (501) staff       (20)       38 2024-04-14 10:18:28.437962 asgebsmanager-0.6/setup.cfg
+-rw-r--r--   0 raghavgupta   (501) staff       (20)      704 2024-04-14 10:18:25.000000 asgebsmanager-0.6/setup.py
```

