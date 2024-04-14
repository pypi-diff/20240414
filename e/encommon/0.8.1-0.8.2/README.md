# Comparing `tmp/encommon-0.8.1.tar.gz` & `tmp/encommon-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encommon-0.8.1.tar", last modified: Mon Apr  8 05:22:50 2024, max compression
+gzip compressed data, was "encommon-0.8.2.tar", last modified: Sun Apr 14 04:45:34 2024, max compression
```

## Comparing `encommon-0.8.1.tar` & `encommon-0.8.2.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-08 05:22:50.536667 encommon-0.8.1/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1071 2024-03-20 05:52:00.000000 encommon-0.8.1/LICENSE
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       32 2023-12-31 23:18:53.000000 encommon-0.8.1/MANIFEST.in
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2671 2024-04-08 05:22:50.536667 encommon-0.8.1/PKG-INFO
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2177 2024-03-31 14:52:08.000000 encommon-0.8.1/README.md
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-08 05:22:50.533667 encommon-0.8.1/encommon/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/__init__.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-08 05:22:50.534667 encommon-0.8.1/encommon/config/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      859 2024-04-07 23:12:30.000000 encommon-0.8.1/encommon/config/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2099 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/config/common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4802 2024-04-08 05:21:36.000000 encommon-0.8.1/encommon/config/config.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2388 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/config/files.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    13488 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/config/logger.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1806 2024-04-07 23:12:30.000000 encommon-0.8.1/encommon/config/params.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2535 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/config/paths.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-08 05:22:50.534667 encommon-0.8.1/encommon/config/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/config/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1069 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/config/test/test_common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2329 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/config/test/test_config.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2230 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/config/test/test_files.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     5135 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/config/test/test_logger.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2568 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/config/test/test_paths.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1810 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/conftest.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-08 05:22:50.534667 encommon-0.8.1/encommon/crypts/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      371 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/crypts/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3540 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/crypts/crypts.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3075 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/crypts/hashes.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      590 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/crypts/params.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-08 05:22:50.534667 encommon-0.8.1/encommon/crypts/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/crypts/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2655 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/crypts/test/test_crypts.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1129 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/crypts/test/test_hashes.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2023-12-31 23:18:53.000000 encommon-0.8.1/encommon/py.typed
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-08 05:22:50.535667 encommon-0.8.1/encommon/times/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      638 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/times/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3635 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/times/common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    10033 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/times/duration.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6153 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/times/parse.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-08 05:22:50.535667 encommon-0.8.1/encommon/times/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/times/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2059 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/times/test/test_common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4161 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/times/test/test_duration.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4055 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/times/test/test_parse.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3075 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/times/test/test_timers.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1691 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/times/test/test_times.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     5411 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/times/test/test_window.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6663 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/times/timers.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     9696 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/times/times.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7975 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/times/window.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-08 05:22:50.535667 encommon-0.8.1/encommon/types/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      420 2024-04-07 10:25:51.000000 encommon-0.8.1/encommon/types/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2265 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/types/dicts.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2739 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/types/empty.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      632 2024-04-07 10:25:51.000000 encommon-0.8.1/encommon/types/strings.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-08 05:22:50.535667 encommon-0.8.1/encommon/types/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/types/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2678 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/types/test/test_dicts.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      971 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/types/test/test_empty.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      406 2024-04-07 10:25:51.000000 encommon-0.8.1/encommon/types/test/test_strings.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-08 05:22:50.536667 encommon-0.8.1/encommon/utils/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      927 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/utils/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1355 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/utils/common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2471 2024-04-07 23:12:30.000000 encommon-0.8.1/encommon/utils/match.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3545 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/utils/paths.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3230 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/utils/sample.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7531 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/utils/stdout.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-08 05:22:50.536667 encommon-0.8.1/encommon/utils/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/utils/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      681 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/utils/test/test_common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1124 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/utils/test/test_match.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1919 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/utils/test/test_paths.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1710 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/utils/test/test_sample.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4878 2024-04-07 10:21:05.000000 encommon-0.8.1/encommon/utils/test/test_stdout.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        6 2024-04-08 05:21:49.000000 encommon-0.8.1/encommon/version.txt
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-08 05:22:50.536667 encommon-0.8.1/encommon.egg-info/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2671 2024-04-08 05:22:50.000000 encommon-0.8.1/encommon.egg-info/PKG-INFO
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1926 2024-04-08 05:22:50.000000 encommon-0.8.1/encommon.egg-info/SOURCES.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        1 2024-04-08 05:22:50.000000 encommon-0.8.1/encommon.egg-info/dependency_links.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       63 2024-04-08 05:22:50.000000 encommon-0.8.1/encommon.egg-info/requires.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        9 2024-04-08 05:22:50.000000 encommon-0.8.1/encommon.egg-info/top_level.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2023-12-31 23:18:53.000000 encommon-0.8.1/pyproject.toml
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       63 2024-01-01 10:25:04.000000 encommon-0.8.1/reqs-install.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      558 2024-04-08 05:22:50.536667 encommon-0.8.1/setup.cfg
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.075637 encommon-0.8.2/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1071 2024-03-20 05:52:00.000000 encommon-0.8.2/LICENSE
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       32 2023-12-31 23:18:53.000000 encommon-0.8.2/MANIFEST.in
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2917 2024-04-14 04:45:34.075637 encommon-0.8.2/PKG-INFO
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2423 2024-04-11 05:09:20.000000 encommon-0.8.2/README.md
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.072637 encommon-0.8.2/encommon/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/__init__.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.073637 encommon-0.8.2/encommon/config/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      859 2024-04-07 23:12:30.000000 encommon-0.8.2/encommon/config/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2099 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/config/common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4802 2024-04-08 05:21:36.000000 encommon-0.8.2/encommon/config/config.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2388 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/config/files.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    13488 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/config/logger.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1806 2024-04-07 23:12:30.000000 encommon-0.8.2/encommon/config/params.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2535 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/config/paths.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.073637 encommon-0.8.2/encommon/config/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/config/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1069 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/config/test/test_common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2325 2024-04-14 04:37:18.000000 encommon-0.8.2/encommon/config/test/test_config.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2240 2024-04-14 04:37:18.000000 encommon-0.8.2/encommon/config/test/test_files.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     5131 2024-04-14 04:37:18.000000 encommon-0.8.2/encommon/config/test/test_logger.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2578 2024-04-14 04:37:18.000000 encommon-0.8.2/encommon/config/test/test_paths.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1810 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/conftest.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.073637 encommon-0.8.2/encommon/crypts/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      371 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/crypts/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3540 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/crypts/crypts.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3075 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/crypts/hashes.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      590 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/crypts/params.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.073637 encommon-0.8.2/encommon/crypts/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/crypts/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2651 2024-04-14 04:37:18.000000 encommon-0.8.2/encommon/crypts/test/test_crypts.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1125 2024-04-14 04:37:18.000000 encommon-0.8.2/encommon/crypts/test/test_hashes.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2023-12-31 23:18:53.000000 encommon-0.8.2/encommon/py.typed
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.074638 encommon-0.8.2/encommon/times/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      638 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/times/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3635 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/times/common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    10794 2024-04-14 04:37:18.000000 encommon-0.8.2/encommon/times/duration.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6153 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/times/parse.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.074638 encommon-0.8.2/encommon/times/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/times/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2059 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/times/test/test_common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4161 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/times/test/test_duration.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4055 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/times/test/test_parse.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3073 2024-04-14 04:37:18.000000 encommon-0.8.2/encommon/times/test/test_timers.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1691 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/times/test/test_times.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     5409 2024-04-14 04:37:18.000000 encommon-0.8.2/encommon/times/test/test_window.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6603 2024-04-14 04:37:18.000000 encommon-0.8.2/encommon/times/timers.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     9696 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/times/times.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7975 2024-04-14 03:50:15.000000 encommon-0.8.2/encommon/times/window.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.074638 encommon-0.8.2/encommon/types/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      420 2024-04-07 10:25:51.000000 encommon-0.8.2/encommon/types/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2265 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/types/dicts.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2739 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/types/empty.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      632 2024-04-07 10:25:51.000000 encommon-0.8.2/encommon/types/strings.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.074638 encommon-0.8.2/encommon/types/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/types/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2678 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/types/test/test_dicts.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      973 2024-04-14 04:37:18.000000 encommon-0.8.2/encommon/types/test/test_empty.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      406 2024-04-07 10:25:51.000000 encommon-0.8.2/encommon/types/test/test_strings.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.075637 encommon-0.8.2/encommon/utils/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      927 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/utils/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1355 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/utils/common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2471 2024-04-07 23:12:30.000000 encommon-0.8.2/encommon/utils/match.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3545 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/utils/paths.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3230 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/utils/sample.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7531 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/utils/stdout.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.075637 encommon-0.8.2/encommon/utils/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/utils/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      681 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/utils/test/test_common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1124 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/utils/test/test_match.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1919 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/utils/test/test_paths.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1710 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/utils/test/test_sample.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4878 2024-04-07 10:21:05.000000 encommon-0.8.2/encommon/utils/test/test_stdout.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        6 2024-04-14 04:41:22.000000 encommon-0.8.2/encommon/version.txt
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-14 04:45:34.075637 encommon-0.8.2/encommon.egg-info/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2917 2024-04-14 04:45:34.000000 encommon-0.8.2/encommon.egg-info/PKG-INFO
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1926 2024-04-14 04:45:34.000000 encommon-0.8.2/encommon.egg-info/SOURCES.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        1 2024-04-14 04:45:34.000000 encommon-0.8.2/encommon.egg-info/dependency_links.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       63 2024-04-14 04:45:34.000000 encommon-0.8.2/encommon.egg-info/requires.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        9 2024-04-14 04:45:34.000000 encommon-0.8.2/encommon.egg-info/top_level.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2023-12-31 23:18:53.000000 encommon-0.8.2/pyproject.toml
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       63 2024-01-01 10:25:04.000000 encommon-0.8.2/reqs-install.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      558 2024-04-14 04:45:34.075637 encommon-0.8.2/setup.cfg
```

### Comparing `encommon-0.8.1/LICENSE` & `encommon-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/PKG-INFO` & `encommon-0.8.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encommon
-Version: 0.8.1
+Version: 0.8.2
 Summary: Enasis Network Common Library
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -14,38 +14,43 @@
 Requires-Dist: pydantic
 Requires-Dist: python-dateutil
 Requires-Dist: pyyaml
 Requires-Dist: snaptime
 
 # Enasis Network Common Library
 
-Common classes and functions used in various public and private projects for
-[Enasis Network](https://github.com/enasisnetwork).
+> :children_crossing: This project has not released its first major version.
+
+Common classes and functions used in various public and private projects.
 
 [![](https://img.shields.io/github/actions/workflow/status/enasisnetwork/encommon/build.yml?style=flat-square&label=GitHub%20actions)](https://github.com/enasisnetwork/encommon/actions)<br>
-[![codecov](https://codecov.io/gh/enasisnetwork/encommon/graph/badge.svg?token=7PGOXKJU0E)](https://codecov.io/gh/enasisnetwork/encommon)<br>
-[![](https://img.shields.io/readthedocs/encommon?style=flat-square&label=Read%20the%20Docs)](https://encommon.readthedocs.io/en/stable)<br>
+[![codecov](https://img.shields.io/codecov/c/github/enasisnetwork/encommon?token=7PGOXKJU0E&style=flat-square&logoColor=FFFFFF&label=Coverage)](https://codecov.io/gh/enasisnetwork/encommon)<br>
+[![](https://img.shields.io/readthedocs/encommon?style=flat-square&label=Read%20the%20Docs)](https://encommon.readthedocs.io)<br>
 [![](https://img.shields.io/pypi/v/encommon.svg?style=flat-square&label=PyPi%20version)](https://pypi.org/project/encommon)<br>
 [![](https://img.shields.io/pypi/dm/encommon?style=flat-square&label=PyPi%20downloads)](https://pypi.org/project/encommon)
 
+## Documentation
+Documentation is on [Read the Docs](https://encommon.readthedocs.io).
+Should you venture into the sections below you will be able to use the
+`sphinx` recipe to build documention in the `docs/html` directory.
+
+## Projects using library
+- [Enasis Network Remote Connect](https://github.com/enasisnetwork/enconnect)
+- [Enasis Network Homie Automate](https://github.com/enasisnetwork/enhomie)
+
 ## Installing the package
 Installing stable from the PyPi repository
 ```
 pip install encommon
 ```
 Installing latest from GitHub repository
 ```
 pip install git+https://github.com/enasisnetwork/encommon
 ```
 
-## Documentation
-Documentation is on [Read the Docs](https://encommon.readthedocs.io).
-Should you venture into the sections below you will be able to use the
-`sphinx` recipe to build documention in the `docs/html` directory.
-
 ## Quick start for local development
 Start by cloning the repository to your local machine.
 ```
 git clone https://github.com/enasisnetwork/encommon.git
 ```
 Set up the Python virtual environments expected by the Makefile.
 ```
```

### Comparing `encommon-0.8.1/README.md` & `encommon-0.8.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 # Enasis Network Common Library
 
-Common classes and functions used in various public and private projects for
-[Enasis Network](https://github.com/enasisnetwork).
+> :children_crossing: This project has not released its first major version.
+
+Common classes and functions used in various public and private projects.
 
 [![](https://img.shields.io/github/actions/workflow/status/enasisnetwork/encommon/build.yml?style=flat-square&label=GitHub%20actions)](https://github.com/enasisnetwork/encommon/actions)<br>
-[![codecov](https://codecov.io/gh/enasisnetwork/encommon/graph/badge.svg?token=7PGOXKJU0E)](https://codecov.io/gh/enasisnetwork/encommon)<br>
-[![](https://img.shields.io/readthedocs/encommon?style=flat-square&label=Read%20the%20Docs)](https://encommon.readthedocs.io/en/stable)<br>
+[![codecov](https://img.shields.io/codecov/c/github/enasisnetwork/encommon?token=7PGOXKJU0E&style=flat-square&logoColor=FFFFFF&label=Coverage)](https://codecov.io/gh/enasisnetwork/encommon)<br>
+[![](https://img.shields.io/readthedocs/encommon?style=flat-square&label=Read%20the%20Docs)](https://encommon.readthedocs.io)<br>
 [![](https://img.shields.io/pypi/v/encommon.svg?style=flat-square&label=PyPi%20version)](https://pypi.org/project/encommon)<br>
 [![](https://img.shields.io/pypi/dm/encommon?style=flat-square&label=PyPi%20downloads)](https://pypi.org/project/encommon)
 
+## Documentation
+Documentation is on [Read the Docs](https://encommon.readthedocs.io).
+Should you venture into the sections below you will be able to use the
+`sphinx` recipe to build documention in the `docs/html` directory.
+
+## Projects using library
+- [Enasis Network Remote Connect](https://github.com/enasisnetwork/enconnect)
+- [Enasis Network Homie Automate](https://github.com/enasisnetwork/enhomie)
+
 ## Installing the package
 Installing stable from the PyPi repository
 ```
 pip install encommon
 ```
 Installing latest from GitHub repository
 ```
 pip install git+https://github.com/enasisnetwork/encommon
 ```
 
-## Documentation
-Documentation is on [Read the Docs](https://encommon.readthedocs.io).
-Should you venture into the sections below you will be able to use the
-`sphinx` recipe to build documention in the `docs/html` directory.
-
 ## Quick start for local development
 Start by cloning the repository to your local machine.
 ```
 git clone https://github.com/enasisnetwork/encommon.git
 ```
 Set up the Python virtual environments expected by the Makefile.
 ```
```

### Comparing `encommon-0.8.1/encommon/__init__.py` & `encommon-0.8.2/encommon/__init__.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/config/__init__.py` & `encommon-0.8.2/encommon/config/__init__.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/config/common.py` & `encommon-0.8.2/encommon/config/common.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/config/config.py` & `encommon-0.8.2/encommon/config/config.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/config/files.py` & `encommon-0.8.2/encommon/config/files.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/config/logger.py` & `encommon-0.8.2/encommon/config/logger.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/config/params.py` & `encommon-0.8.2/encommon/config/params.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/config/paths.py` & `encommon-0.8.2/encommon/config/paths.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/config/test/test_common.py` & `encommon-0.8.2/encommon/config/test/test_common.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/config/test/test_config.py` & `encommon-0.8.2/encommon/config/test/test_config.py`

 * *Files 19% similar despite different names*

```diff
@@ -44,21 +44,21 @@
         '_Config__cargs',
         '_Config__params',
         '_Config__paths',
         '_Config__logger',
         '_Config__crypts']
 
 
-    assert repr(config)[:23] == (
-        '<encommon.config.config')
+    assert 1 <= repr(config).find(
+        'config.Config object')
 
     assert hash(config) > 0
 
-    assert str(config)[:23] == (
-        '<encommon.config.config')
+    assert 1 <= str(config).find(
+        'config.Config object')
 
 
     assert 'ConfigFiles' in str(config.files)
 
     assert 'ConfigPaths' in str(config.paths)
 
     assert len(config.cargs) == 1
```

### Comparing `encommon-0.8.1/encommon/config/test/test_files.py` & `encommon-0.8.2/encommon/config/test/test_files.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,21 +50,21 @@
     attrs = list(file.__dict__)
 
     assert attrs == [
         'path',
         'config']
 
 
-    assert repr(file)[:22] == (
-        '<encommon.config.files')
+    assert 1 <= repr(file).find(
+        'files.ConfigFile object')
 
     assert hash(file) > 0
 
-    assert str(file)[:22] == (
-        '<encommon.config.files')
+    assert 1 <= str(file).find(
+        'files.ConfigFile object')
 
 
     assert file.path.name == 'config.yml'
 
     assert len(file.config) == 3
 
 
@@ -83,21 +83,21 @@
 
     assert attrs == [
         'paths',
         'config',
         '_ConfigFiles__merged']
 
 
-    assert repr(files)[:22] == (
-        '<encommon.config.files')
+    assert 1 <= repr(files).find(
+        'files.ConfigFiles object')
 
     assert hash(files) > 0
 
-    assert str(files)[:22] == (
-        '<encommon.config.files')
+    assert 1 <= str(files).find(
+        'files.ConfigFiles object')
 
 
     assert len(files.paths) == 2
 
     assert len(files.config) == 2
 
     assert files.merged == {
```

### Comparing `encommon-0.8.1/encommon/config/test/test_logger.py` & `encommon-0.8.2/encommon/config/test/test_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,21 +142,21 @@
         '_Logger__file_level',
         '_Logger__file_path',
         '_Logger__started',
         '_Logger__logr_stdo',
         '_Logger__logr_file']
 
 
-    assert repr(logger)[:23] == (
-        '<encommon.config.logger')
+    assert 1 <= repr(logger).find(
+        'logger.Logger object')
 
     assert hash(logger) > 0
 
-    assert str(logger)[:23] == (
-        '<encommon.config.logger')
+    assert 1 <= str(logger).find(
+        'logger.Logger object')
 
 
     assert logger.stdo_level == 'info'
 
     assert logger.file_level == 'info'
 
     assert logger.file_path is not None
```

### Comparing `encommon-0.8.1/encommon/config/test/test_paths.py` & `encommon-0.8.2/encommon/config/test/test_paths.py`

 * *Files 13% similar despite different names*

```diff
@@ -53,21 +53,21 @@
     attrs = list(path.__dict__)
 
     assert attrs == [
         'path',
         'config']
 
 
-    assert repr(path)[:22] == (
-        '<encommon.config.paths')
+    assert 1 <= repr(path).find(
+        'paths.ConfigPath object')
 
     assert hash(path) > 0
 
-    assert str(path)[:22] == (
-        '<encommon.config.paths')
+    assert 1 <= str(path).find(
+        'paths.ConfigPath object')
 
 
     assert 'test' in path.path.name
 
     assert len(path.config) == 1
 
 
@@ -85,21 +85,21 @@
     attrs = list(paths.__dict__)
 
     assert attrs == [
         'paths', 'config',
         '_ConfigPaths__merged']
 
 
-    assert repr(paths)[:22] == (
-        '<encommon.config.paths')
+    assert 1 <= repr(paths).find(
+        'paths.ConfigPaths object')
 
     assert hash(paths) > 0
 
-    assert str(paths)[:22] == (
-        '<encommon.config.paths')
+    assert 1 <= str(paths).find(
+        'paths.ConfigPaths object')
 
 
     assert len(paths.paths) == 2
 
     assert len(paths.config) == 2
```

### Comparing `encommon-0.8.1/encommon/conftest.py` & `encommon-0.8.2/encommon/conftest.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/crypts/crypts.py` & `encommon-0.8.2/encommon/crypts/crypts.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/crypts/hashes.py` & `encommon-0.8.2/encommon/crypts/hashes.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/crypts/params.py` & `encommon-0.8.2/encommon/crypts/params.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/crypts/test/test_crypts.py` & `encommon-0.8.2/encommon/crypts/test/test_crypts.py`

 * *Files 10% similar despite different names*

```diff
@@ -47,21 +47,21 @@
 
     attrs = list(crypts.__dict__)
 
     assert attrs == [
         '_Crypts__phrases']
 
 
-    assert repr(crypts)[:23] == (
-        '<encommon.crypts.crypts')
+    assert 1 <= repr(crypts).find(
+        'crypts.Crypts object')
 
     assert hash(crypts) > 0
 
-    assert str(crypts)[:23] == (
-        '<encommon.crypts.crypts')
+    assert 1 <= str(crypts).find(
+        'crypts.Crypts object')
 
 
     assert len(crypts.phrases) == 2
 
     assert len(crypts.keygen()) == 44
```

### Comparing `encommon-0.8.1/encommon/crypts/test/test_hashes.py` & `encommon-0.8.2/encommon/crypts/test/test_hashes.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 
     attrs = list(hashes.__dict__)
 
     assert attrs == [
         '_Hashes__string']
 
 
-    assert repr(hashes)[:23] == (
-        '<encommon.crypts.hashes')
+    assert 1 <= repr(hashes).find(
+        'hashes.Hashes object')
 
     assert hash(hashes) > 0
 
-    assert str(hashes)[:23] == (
-        '<encommon.crypts.hashes')
+    assert 1 <= str(hashes).find(
+        'hashes.Hashes object')
 
 
     assert hashes.string == 'string'
 
     assert hashes.md5[:3] == 'b45'
     assert hashes.md5[-2:] == '21'
```

### Comparing `encommon-0.8.1/encommon/times/__init__.py` & `encommon-0.8.2/encommon/times/__init__.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/times/common.py` & `encommon-0.8.2/encommon/times/common.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/times/duration.py` & `encommon-0.8.2/encommon/times/duration.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,29 +35,61 @@
 
 
 
 class Duration:
     """
     Convert the provided seconds in a human friendly format.
 
-    Example
-    -------
-    >>> Duration(86400 * 700).compact
+    Example: Common Methods
+    -----------------------
+    >>> durate = Duration(6048e4)
+    >>> durate.short
+    '1y 11mon 5d'
+    >>> durate.compact
     '1y11mon5d'
-
-    Example
-    -------
-    >>> Duration(86400 * 700).verbose
+    >>> durate.verbose
     '1 year, 11 months, 5 days'
 
-    Example
-    -------
-    >>> Duration(7201, False).verbose
+    Example: Dump the Units
+    -----------------------
+    >>> durate = Duration(6048e4)
+    >>> durate.units()
+    {'year': 1, 'month': 11, 'day': 5}
+
+    Example: Disable Smart Seconds
+    ------------------------------
+    >>> durate = Duration(7201, False)
+    >>> durate.compact
+    '2h1s'
+    >>> durate.verbose
     '2 hours, 1 second'
 
+    Example: Basic Operators
+    ------------------------
+    >>> durate1 = Duration(1000)
+    >>> durate2 = Duration(2000)
+    >>> durate1 == durate2
+    False
+    >>> durate1 != durate2
+    True
+    >>> durate1 > durate2
+    False
+    >>> durate1 >= durate2
+    False
+    >>> durate1 < durate2
+    True
+    >>> durate1 <= durate2
+    True
+    >>> durate1 + durate2
+    3000.0
+    >>> durate1 - durate2
+    -1000.0
+    >>> durate2 - durate1
+    1000.0
+
     :param seconds: Period in seconds that will be iterated.
     :param smart: Determines if we hide seconds after minute.
     :param groups: Determine the quantity of groups to show,
         ensuring larger units are returned before smaller.
     """
 
     __source: float
```

### Comparing `encommon-0.8.1/encommon/times/parse.py` & `encommon-0.8.2/encommon/times/parse.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/times/test/test_common.py` & `encommon-0.8.2/encommon/times/test/test_common.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/times/test/test_duration.py` & `encommon-0.8.2/encommon/times/test/test_duration.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/times/test/test_parse.py` & `encommon-0.8.2/encommon/times/test/test_parse.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/times/test/test_timers.py` & `encommon-0.8.2/encommon/times/test/test_timers.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,21 +50,21 @@
         '_Timers__config',
         '_Timers__sqlite',
         '_Timers__file',
         '_Timers__table',
         '_Timers__cache']
 
 
-    assert repr(timers)[:22] == (
-        '<encommon.times.timers')
+    assert 1 <= repr(timers).find(
+        'timers.Timers object')
 
     assert hash(timers) > 0
 
-    assert str(timers)[:22] == (
-        '<encommon.times.timers')
+    assert 1 <= str(timers).find(
+        'timers.Timers object')
 
 
     assert timers.timers == {'one': 1}
 
     assert timers.sqlite is not None
 
     assert timers.file[-8:] == 'cache.db'
```

### Comparing `encommon-0.8.1/encommon/times/test/test_times.py` & `encommon-0.8.2/encommon/times/test/test_times.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/times/test/test_window.py` & `encommon-0.8.2/encommon/times/test/test_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,21 +54,21 @@
         '_Window__anchor',
         '_Window__delay',
         '_Window__wilast',
         '_Window__winext',
         '_Window__walked']
 
 
-    assert repr(window)[:22] == (
-        '<encommon.times.window')
+    assert 1 <= repr(window).find(
+        'window.Window object')
 
     assert hash(window) > 0
 
-    assert str(window)[:22] == (
-        '<encommon.times.window')
+    assert 1 <= str(window).find(
+        'window.Window object')
 
 
     assert window.schedule == '* * * * *'
 
     assert window.start == '1970-01-01T00:05:30Z'
 
     assert window.stop == '1970-01-01T00:10:30Z'
```

### Comparing `encommon-0.8.1/encommon/times/timers.py` & `encommon-0.8.2/encommon/times/timers.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,22 @@
 
 This file is part of Enasis Network software eco-system. Distribution
 is permitted, for more information consult the project license file.
 """
 
 
 
+from sqlite3 import Connection
 from sqlite3 import connect as SQLite
 from typing import Optional
-from typing import TYPE_CHECKING
 
 from .common import NUMERIC
 from .common import PARSABLE
 from .times import Times
 
-if TYPE_CHECKING:
-    from sqlite3 import Connection
-
 
 
 CACHE_TABLE = (
     """
     create table if not exists
      {0} (
       "unique" text not null,
@@ -59,15 +56,15 @@
     :param timers: Seconds that are used for each of timers.
     :param file: Optional path to SQLite database for
         cache. This will allow for use between executions.
     :param table: Optional override default table name.
     """
 
     __config: _TIMERS
-    __sqlite: 'Connection'
+    __sqlite: Connection
     __file: str
     __table: str
     __cache: _CACHED
 
 
     def __init__(
         self,
@@ -187,15 +184,15 @@
 
         return dict(self.__config)
 
 
     @property
     def sqlite(
         self,
-    ) -> 'Connection':
+    ) -> Connection:
         """
         Return the value for the attribute from class instance.
 
         :returns: Value for the attribute from class instance.
         """
 
         return self.__sqlite
```

### Comparing `encommon-0.8.1/encommon/times/times.py` & `encommon-0.8.2/encommon/times/times.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/times/window.py` & `encommon-0.8.2/encommon/times/window.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/types/dicts.py` & `encommon-0.8.2/encommon/types/dicts.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/types/empty.py` & `encommon-0.8.2/encommon/types/empty.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/types/strings.py` & `encommon-0.8.2/encommon/types/strings.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/types/test/test_dicts.py` & `encommon-0.8.2/encommon/types/test/test_dicts.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/types/test/test_empty.py` & `encommon-0.8.2/encommon/types/test/test_empty.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,17 @@
     attrs = list(empty.__dict__)
 
     assert attrs == [
         '_EmptyType__empty']
 
 
     assert repr(empty) == 'Empty'
+
     assert hash(empty) > 0
+
     assert str(empty) == 'Empty'
 
 
     assert not (Empty or None)
     assert Empty is empty
     assert Empty is Empty
     assert Empty is EmptyType()
```

### Comparing `encommon-0.8.1/encommon/utils/__init__.py` & `encommon-0.8.2/encommon/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/utils/common.py` & `encommon-0.8.2/encommon/utils/common.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/utils/match.py` & `encommon-0.8.2/encommon/utils/match.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/utils/paths.py` & `encommon-0.8.2/encommon/utils/paths.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/utils/sample.py` & `encommon-0.8.2/encommon/utils/sample.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/utils/stdout.py` & `encommon-0.8.2/encommon/utils/stdout.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/utils/test/test_common.py` & `encommon-0.8.2/encommon/utils/test/test_common.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/utils/test/test_match.py` & `encommon-0.8.2/encommon/utils/test/test_match.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/utils/test/test_paths.py` & `encommon-0.8.2/encommon/utils/test/test_paths.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/utils/test/test_sample.py` & `encommon-0.8.2/encommon/utils/test/test_sample.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon/utils/test/test_stdout.py` & `encommon-0.8.2/encommon/utils/test/test_stdout.py`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/encommon.egg-info/PKG-INFO` & `encommon-0.8.2/encommon.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encommon
-Version: 0.8.1
+Version: 0.8.2
 Summary: Enasis Network Common Library
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -14,38 +14,43 @@
 Requires-Dist: pydantic
 Requires-Dist: python-dateutil
 Requires-Dist: pyyaml
 Requires-Dist: snaptime
 
 # Enasis Network Common Library
 
-Common classes and functions used in various public and private projects for
-[Enasis Network](https://github.com/enasisnetwork).
+> :children_crossing: This project has not released its first major version.
+
+Common classes and functions used in various public and private projects.
 
 [![](https://img.shields.io/github/actions/workflow/status/enasisnetwork/encommon/build.yml?style=flat-square&label=GitHub%20actions)](https://github.com/enasisnetwork/encommon/actions)<br>
-[![codecov](https://codecov.io/gh/enasisnetwork/encommon/graph/badge.svg?token=7PGOXKJU0E)](https://codecov.io/gh/enasisnetwork/encommon)<br>
-[![](https://img.shields.io/readthedocs/encommon?style=flat-square&label=Read%20the%20Docs)](https://encommon.readthedocs.io/en/stable)<br>
+[![codecov](https://img.shields.io/codecov/c/github/enasisnetwork/encommon?token=7PGOXKJU0E&style=flat-square&logoColor=FFFFFF&label=Coverage)](https://codecov.io/gh/enasisnetwork/encommon)<br>
+[![](https://img.shields.io/readthedocs/encommon?style=flat-square&label=Read%20the%20Docs)](https://encommon.readthedocs.io)<br>
 [![](https://img.shields.io/pypi/v/encommon.svg?style=flat-square&label=PyPi%20version)](https://pypi.org/project/encommon)<br>
 [![](https://img.shields.io/pypi/dm/encommon?style=flat-square&label=PyPi%20downloads)](https://pypi.org/project/encommon)
 
+## Documentation
+Documentation is on [Read the Docs](https://encommon.readthedocs.io).
+Should you venture into the sections below you will be able to use the
+`sphinx` recipe to build documention in the `docs/html` directory.
+
+## Projects using library
+- [Enasis Network Remote Connect](https://github.com/enasisnetwork/enconnect)
+- [Enasis Network Homie Automate](https://github.com/enasisnetwork/enhomie)
+
 ## Installing the package
 Installing stable from the PyPi repository
 ```
 pip install encommon
 ```
 Installing latest from GitHub repository
 ```
 pip install git+https://github.com/enasisnetwork/encommon
 ```
 
-## Documentation
-Documentation is on [Read the Docs](https://encommon.readthedocs.io).
-Should you venture into the sections below you will be able to use the
-`sphinx` recipe to build documention in the `docs/html` directory.
-
 ## Quick start for local development
 Start by cloning the repository to your local machine.
 ```
 git clone https://github.com/enasisnetwork/encommon.git
 ```
 Set up the Python virtual environments expected by the Makefile.
 ```
```

### Comparing `encommon-0.8.1/encommon.egg-info/SOURCES.txt` & `encommon-0.8.2/encommon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/pyproject.toml` & `encommon-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `encommon-0.8.1/setup.cfg` & `encommon-0.8.2/setup.cfg`

 * *Files identical despite different names*

