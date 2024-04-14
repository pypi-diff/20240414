# Comparing `tmp/datapools-0.1.9.tar.gz` & `tmp/datapools-1.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapools-0.1.9.tar", last modified: Mon Nov  6 16:50:35 2023, max compression
+gzip compressed data, was "datapools-1.0.41.tar", last modified: Sun Apr 14 20:18:20 2024, max compression
```

## Comparing `datapools-0.1.9.tar` & `datapools-1.0.41.tar`

### file list

```diff
@@ -1,73 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 16:50:35.764563 datapools-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-11-06 16:50:22.000000 datapools-0.1.9/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2023-11-06 16:50:22.000000 datapools-0.1.9/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2023-11-06 16:50:22.000000 datapools-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      113 2023-11-06 16:50:22.000000 datapools-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2023-11-06 16:50:35.764563 datapools-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      792 2023-11-06 16:50:22.000000 datapools-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 16:50:35.752563 datapools-0.1.9/datapools/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      136 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 16:50:35.756563 datapools-0.1.9/datapools/common/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/common/backend_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/common/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 16:50:35.756563 datapools-0.1.9/datapools/common/queues/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/common/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7874 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/common/queues/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/common/queues/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/common/stoppable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 16:50:35.756563 datapools-0.1.9/datapools/common/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/common/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/common/storage/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/common/storage/file_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 16:50:35.756563 datapools-0.1.9/datapools/common/tasks_db/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/common/tasks_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/common/tasks_db/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/common/tasks_db/tasks_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/common/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 16:50:35.756563 datapools-0.1.9/datapools/producer/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/producer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5975 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/producer/base_producer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/producer/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     6261 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 16:50:35.756563 datapools-0.1.9/datapools/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/worker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 16:50:35.760563 datapools-0.1.9/datapools/worker/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/worker/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/worker/plugins/base_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 16:50:35.760563 datapools-0.1.9/datapools/worker/plugins/dataphoenix_info/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/worker/plugins/dataphoenix_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 16:50:35.760563 datapools-0.1.9/datapools/worker/plugins/default/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/worker/plugins/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/worker/plugins/default/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 16:50:35.760563 datapools-0.1.9/datapools/worker/plugins/google_drive/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/worker/plugins/google_drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7297 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/worker/plugins/google_drive/google_drive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 16:50:35.760563 datapools-0.1.9/datapools/worker/plugins/imageshack/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/worker/plugins/imageshack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/worker/plugins/imageshack/imageshack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 16:50:35.760563 datapools-0.1.9/datapools/worker/plugins/s3/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/worker/plugins/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/worker/plugins/s3/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 16:50:35.760563 datapools-0.1.9/datapools/worker/plugins/youtube_channel/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/worker/plugins/youtube_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6948 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/worker/plugins/youtube_channel/youtube_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/worker/scheduler_api.py.bak
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-11-06 16:50:22.000000 datapools-0.1.9/datapools/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 16:50:35.756563 datapools-0.1.9/datapools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2023-11-06 16:50:35.000000 datapools-0.1.9/datapools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2023-11-06 16:50:35.000000 datapools-0.1.9/datapools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-06 16:50:35.000000 datapools-0.1.9/datapools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-11-06 16:50:35.000000 datapools-0.1.9/datapools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      181 2023-11-06 16:50:35.000000 datapools-0.1.9/datapools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-06 16:50:35.000000 datapools-0.1.9/datapools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-06 16:50:35.764563 datapools-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2023-11-06 16:50:22.000000 datapools-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-06 16:50:35.760563 datapools-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-06 16:50:22.000000 datapools-0.1.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2023-11-06 16:50:22.000000 datapools-0.1.9/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-11-06 16:50:22.000000 datapools-0.1.9/tests/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:20.423143 datapools-1.0.41/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-14 20:18:11.000000 datapools-1.0.41/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:11.000000 datapools-1.0.41/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-04-14 20:18:11.000000 datapools-1.0.41/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-14 20:18:11.000000 datapools-1.0.41/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-14 20:18:20.423143 datapools-1.0.41/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-14 20:18:11.000000 datapools-1.0.41/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:20.407143 datapools-1.0.41/datapools/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:20.411143 datapools-1.0.41/datapools/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/common/backend_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/common/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:20.411143 datapools-1.0.41/datapools/common/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/common/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12803 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/common/queues/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/common/queues/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/common/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/common/stoppable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:20.411143 datapools-1.0.41/datapools/common/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/common/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/common/storage/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/common/storage/file_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:20.411143 datapools-1.0.41/datapools/common/tasks_db/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/common/tasks_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/common/tasks_db/redis.py.bak
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/common/tasks_db/tasks_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8887 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:20.411143 datapools-1.0.41/datapools/producer/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/producer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5876 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/producer/base_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:20.411143 datapools-1.0.41/datapools/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10858 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:20.415143 datapools-1.0.41/datapools/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:20.415143 datapools-1.0.41/datapools/worker/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/plugins/base_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:20.415143 datapools-1.0.41/datapools/worker/plugins/dataphoenix_info/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/plugins/dataphoenix_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:20.415143 datapools-1.0.41/datapools/worker/plugins/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/plugins/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9025 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/plugins/default/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:20.415143 datapools-1.0.41/datapools/worker/plugins/deutsche_welle/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/plugins/deutsche_welle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:20.415143 datapools-1.0.41/datapools/worker/plugins/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/plugins/google_drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8140 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/plugins/google_drive/google_drive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:20.415143 datapools-1.0.41/datapools/worker/plugins/imageshack/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/plugins/imageshack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11282 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/plugins/imageshack/imageshack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:20.419143 datapools-1.0.41/datapools/worker/plugins/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/plugins/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/plugins/s3/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:20.419143 datapools-1.0.41/datapools/worker/plugins/theguardian/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/plugins/theguardian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/plugins/theguardian/theguardian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:20.419143 datapools-1.0.41/datapools/worker/plugins/washingtonpost/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/plugins/washingtonpost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/plugins/washingtonpost/washingtonpost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:20.419143 datapools-1.0.41/datapools/worker/plugins/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/plugins/wikipedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7338 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/plugins/wikipedia/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:20.419143 datapools-1.0.41/datapools/worker/plugins/youtube_channel/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/plugins/youtube_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/plugins/youtube_channel/youtube_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16055 2024-04-14 20:18:11.000000 datapools-1.0.41/datapools/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:20.423143 datapools-1.0.41/datapools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-14 20:18:20.000000 datapools-1.0.41/datapools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-14 20:18:20.000000 datapools-1.0.41/datapools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 20:18:20.000000 datapools-1.0.41/datapools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-14 20:18:20.000000 datapools-1.0.41/datapools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-14 20:18:20.000000 datapools-1.0.41/datapools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 20:18:20.000000 datapools-1.0.41/datapools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 20:18:20.423143 datapools-1.0.41/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-04-14 20:18:11.000000 datapools-1.0.41/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:20.419143 datapools-1.0.41/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 20:18:11.000000 datapools-1.0.41/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-14 20:18:11.000000 datapools-1.0.41/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-14 20:18:11.000000 datapools-1.0.41/tests/test_base.py
```

### Comparing `datapools-0.1.9/LICENSE` & `datapools-1.0.41/LICENSE`

 * *Files identical despite different names*

### Comparing `datapools-0.1.9/README.md` & `datapools-1.0.41/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 ```bash
 pip install datapools
 ```
 
 ## Usage
 
 ```python
-from datapools import datapool
-
-datapool('id').crawl()
+from datapools import crawl
+...
+await crawl(datapool_id=1)
 ```
 
 ```bash
-$ python -m datapools
+$ python3 -m datapools --id=1
 #or
 $ datapools
 ```
 
 ## Documentation
 Documentation is available at [docs.openlicense.ai](https://docs.openlicense.ai)
-
+ 
 
 ## Development
 
 Read the [CONTRIBUTING.md](https://github.com/openlicenseai/datapools/blob/master/CONTRIBUTING.md) file.
```

### Comparing `datapools-0.1.9/datapools/common/backend_api.py` & `datapools-1.0.41/datapools/common/backend_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,62 @@
+from typing import List
+
 import httpx
 from pydantic import BaseModel
 
 from ..common.logger import logger
-from ..common.types import CrawlerHintURLStatus, DatapoolRules
+from ..common.types import CrawlerHintURLStatus  # , DatapoolRules
 
 
-class TagDatapools(BaseModel):
-    id: int
-    content_rules: DatapoolRules
+# class TagDatapool(BaseModel):
+#     id: int
+#     rules: DatapoolRules
 
-    class Config:
-        validate_assignment = True
+#     class Config:
+#         validate_assignment = True
 
 
 class BackendAPI:
     def __init__(self, url):
         self.url = url
 
     async def get_hint_urls(self, limit):
-        return await self.get_uri("get-hint-urls", {"limit": limit})
+        res = await self.get_uri("get-hint-urls", {"limit": limit})
+        return res if res is not None else []
 
-    async def set_hint_url_status(self, id, status: CrawlerHintURLStatus):
+    async def set_hint_url_status(self, hint_id, status: CrawlerHintURLStatus, session_id=None):
         return await self.get_uri(
-            "set-hint-url-status", {"id": id, "status": status.value}
+            "set-hint-url-status", {"id": hint_id, "status": status.value, "session_id": session_id}
         )
 
     # async def add_crawler_contents( self, contents: dict ):
     #     return await self.get_uri( 'add-crawler-contents', { 'contents': contents } )
 
     # async def get_crawled_contents(self, limit):
     #     return await self.get_uri( 'get-crawled-contents', { 'limit': limit } )
 
-    async def add_datapool_content(self, data):
-        return await self.get_uri("add-datapool-content", data)
+    async def add_crawled_content(self, data):
+        return await self.get_uri("add-crawled-content", data)
 
-    async def get_tag_datapools(self, tag_id) -> TagDatapools:
-        return await self.get_uri(
-            "get-tag-datapools", {"filter": {"tag_id": tag_id}}
-        )
+    # async def get_tag_datapools(self, tag_id) -> List[TagDatapool]:
+    #     res = await self.get_uri(
+    #         "get-tag-datapools", {"filter": {"tag_id": tag_id}}
+    #     )
+    #     # logger.info( f"get_tag_datapools {res=}")
+    #     for i in range(len(res)):
+    #         res[i] = TagDatapool.parse_obj(res[i])
+    #     return res
 
     async def get_uri(self, uri, data={}):
         async with httpx.AsyncClient() as client:
             url = self.url + uri
-            logger.info(f"posting to {url=} {data=}")
+            logger.debug(f"posting to {url=} {data=}")
 
-            r = await client.post(url, json=data)
-            if r.status_code == 200:
-                return r.json()
-            else:
-                logger.error(f"Non 200 http response {r=}")
-                raise Exception("non 200 response")
+            try:
+                r = await client.post(url, json=data)
+                if r.status_code == 200:
+                    return r.json()
+                else:
+                    logger.error(f"Non 200 http response {r=}")
+                    raise Exception("non 200 response")
+            except httpx.ConnectError as e:
+                logger.error( f'Failed connect Backend API server: {e}')
```

### Comparing `datapools-0.1.9/datapools/common/queues/types.py` & `datapools-1.0.41/datapools/common/queues/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 import json
 from enum import Enum
 
-#from ..logger import logger
+# from ..logger import logger
 
 
 class QueueRole(Enum):
     Publisher = 1
     Receiver = 2
 
 
 class QueueMessageType(Enum):
     Task = 1
     Report = 2
     StorageInvalidation = 3
+    Stop = 4
 
 
 class QueueMessage:
-    def __init__(self, type: QueueMessageType, data):
-        self.type = type
+    def __init__(self, session_id: str, message_type: QueueMessageType, data=None):
+        self.session_id = session_id
+        self.type = message_type
         self.data = data
 
     def encode(self):
         # logger.info( f'encoding {self.type=} {self.data=}')
         return json.dumps(
-            {"type": self.type.value, "data": json.dumps(self.data)}
+            {"session_id": self.session_id, "type": self.type.value, "data": json.dumps(self.data)}
         ).encode()
 
     @staticmethod
     def decode(binary):
         j = json.loads(binary.decode())
-        res = QueueMessage(
-            type=QueueMessageType(j["type"]), data=json.loads(j["data"])
+        res = QueueMessage( 
+            session_id=j['session_id'],
+            message_type=QueueMessageType(j["type"]), 
+            data=json.loads(j["data"])
         )
         return res
 
 
 class QueueTopicMessage:
     def __init__(self, topic, data):
         self.topic = topic.split(".")
```

### Comparing `datapools-0.1.9/datapools/common/stoppable.py` & `datapools-1.0.41/datapools/common/stoppable.py`

 * *Files identical despite different names*

### Comparing `datapools-0.1.9/datapools/common/storage/file_storage.py` & `datapools-1.0.41/datapools/common/storage/file_storage.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import os
 
-#from ..logger import logger
+from ..logger import logger
 from .base_storage import BaseStorage
 
 
 class FileStorage(BaseStorage):
     def __init__(self, dst_path):
         self.dst_path = dst_path
 
     async def put(self, storage_id, content):
-        f = open(self.get_path(storage_id), "wb")
-        if type(content) is str:
-            content = content.encode()
-        f.write(content)
-        f.close()
+        with open(self.get_path(storage_id), "wb") as f:
+            if type(content) is str:
+                content = content.encode()
+            f.write(content)
 
     async def get(self, storage_id):
-        f = open(self.get_path(storage_id), "rb")
-        res = f.read()
-        f.close()
-        return res
+        with open(self.get_path(storage_id), "rb") as f:
+            res = f.read()
+            return res
 
     async def remove(self, storage_id):
-        os.unlink(self.get_path(storage_id))
+        path = self.get_path(storage_id)
+        logger.info(f"unlink {path=}")
+        os.unlink(path)
+        
+    async def has( self, storage_id):
+        path = self.get_path(storage_id)
+        return os.path.exists( path )
 
     def get_path(self, storage_id):
         return os.path.join(self.dst_path, storage_id)
```

### Comparing `datapools-0.1.9/datapools/common/tasks_db/redis.py` & `datapools-1.0.41/datapools/common/tasks_db/redis.py.bak`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 import json
 import time
-from typing import Union, Literal
+from typing import Literal, Union
 
 import redis
 
 from ..logger import logger
-from .tasks_db import TasksDB, Hash, TaskOrNone, TasksInProgress, TaskInProgress, Task
+from .tasks_db import (
+    Hash,
+    Task,
+    TaskInProgress,
+    TaskOrNone,
+    TasksDB,
+    TasksInProgress,
+)
 
 URL_HASHES_KEY = "tasks_url_hashes"  # sorted set
 URL_DONE_HASHES_KEY = "tasks_url_done_hashes"  # set
 TASKS_QUEUE_KEY = "tasks_queue"  # hash
 TASKS_IN_PROGRESS_KEY = "tasks_in_progress"  # hash
 
 
@@ -100,24 +107,23 @@
             else:
                 break
 
         return None
 
     def get_progress_list(self, offset, limit) -> TasksInProgress:
         keys = self.redis.hkeys(TASKS_IN_PROGRESS_KEY)
-        keys = keys[offset:offset + limit]
+        keys = keys[offset : offset + limit]
         if len(keys) > 0:
             tasks = self.redis.hmget(TASKS_IN_PROGRESS_KEY, keys)
             for i in range(0, len(tasks)):
                 tasks[i] = json.loads(tasks[i])
             res = dict(zip(keys, tasks))
         else:
             res = {}
         return res
-        
 
     def _remove_progress(self, hash) -> TaskInProgress:
         # start transaction
         pipe = self.redis.pipeline()
 
         # 1. get from progress list and remove value
         pipe.hget(TASKS_IN_PROGRESS_KEY, hash)
```

### Comparing `datapools-0.1.9/datapools/common/tasks_db/tasks_db.py` & `datapools-1.0.41/datapools/common/tasks_db/tasks_db.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # from pydantic import Dict
 from hashlib import md5
-from typing import Dict, TypeAlias, Union, Literal
+from typing import Dict, Literal, TypeAlias, Union
 
 
 class TasksDBException(Exception):
     pass
 
+
 # class Task:
 #     pass
 
 # class TaskInProgress:
 #     pass
 
 Hash: TypeAlias = str
@@ -21,15 +22,15 @@
 
 class TasksDB:
     def __init__(self):
         pass
 
     def add(
         self, task, score=0, ignore_existing=False, ignore_done=False
-    ) -> Union[Hash, Literal[False] ]:
+    ) -> Union[Hash, Literal[False]]:
         # puts new url to the queue
         # score may define priority of the task
         # should return False if url is already in the queue
         raise TasksDBException("implement add()")
 
     def has(self, task) -> bool:
         # checks if URL is not in the queue already
```

### Comparing `datapools-0.1.9/datapools/producer/base_producer.py` & `datapools-1.0.41/datapools/producer/base_producer.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,151 +1,155 @@
 import asyncio
+
 # import importlib
 # import inspect
-# import os
+import os
+
 # import sys
 import traceback
-# from enum import Enum
-from typing import Optional
 
-import aio_pika
-# from pydantic import BaseModel
+# from enum import Enum
+from typing import List, Optional
 
-from ..common.backend_api import BackendAPI, TagDatapools
+from ..common.backend_api import BackendAPI  # , TagDatapool
 from ..common.logger import logger
 from ..common.queues import (
+    GenericQueue,
     QueueMessage,
     QueueMessageType,
     QueueRole,
     QueueTopicMessage,
-    RabbitmqParams,
-    RabbitmqQueue,
 )
 from ..common.stoppable import Stoppable
 from ..common.storage.file_storage import FileStorage
-from ..common.types import BaseProducerSettings, QUEUE_EVAL_TASKS, QUEUE_WORKER_TASKS, DatapoolRuleMatch, DatapoolRules, TOPICS_EXCHANGE_NAME
-from ..worker import CrawlerWorker
-from .rules import DatapoolRulesChecker
+
+from ..common.types import (
+    BaseProducerSettings,
+    InvalidUsageException,
+)
+from ..worker.utils import get_storage_invalidation_topic
+from ..common.session_manager import SessionManager
+# from .rules import DatapoolRulesChecker
 
 
 class BaseProducer(Stoppable):
     def __init__(self, cfg: Optional[BaseProducerSettings] = None):
         super().__init__()
         self.cfg = cfg if cfg is not None else BaseProducerSettings()
-        self.api = BackendAPI(url=self.cfg.BACKEND_API_URL)
-        self.storage = FileStorage(self.cfg.STORAGE_PATH)
+        self.session_manager = SessionManager(
+            self.cfg.REDIS_HOST, self.cfg.REDIS_PORT)
 
-        # receives tasks from workers
-        self.eval_queue = RabbitmqQueue(
-            QueueRole.Receiver,
-            self.cfg.RABBITMQ_CONNECTION_URL,
-            QUEUE_EVAL_TASKS,
-        )
+        if not self.cfg.CLI_MODE:
+            self.api = BackendAPI(url=self.cfg.BACKEND_API_URL)
 
-        # will wait messages from workers
-        self.todo_queue = RabbitmqQueue(
-            QueueRole.Publisher,
-            self.cfg.RABBITMQ_CONNECTION_URL,
-            QUEUE_WORKER_TASKS,
+        # receives tasks from workers
+        self.eval_queue = GenericQueue(
+            role=QueueRole.Receiver,
+            url=self.cfg.QUEUE_CONNECTION_URL,
+            name=self.cfg.EVAL_TASKS_QUEUE_NAME,
         )
+        logger.info("created receiver eval_tasks")
 
         # will invalidate worker cache entries
-        self.topics_queue = RabbitmqQueue(
-            QueueRole.Publisher,
-            self.cfg.RABBITMQ_CONNECTION_URL,
-            None,
-            RabbitmqParams(
-                exchange_type=aio_pika.ExchangeType.TOPIC,
-                exchange_name=TOPICS_EXCHANGE_NAME,
-            ),
+        self.topics_queue = GenericQueue(
+            role=QueueRole.Publisher,
+            url=self.cfg.QUEUE_CONNECTION_URL,
+            name=self.cfg.TOPICS_QUEUE_NAME,
+            topic=True,  # for Rabbitmq publisher
         )
-        self.datapool_rules_checker = DatapoolRulesChecker()
+        logger.info("created publisher worker_tasks")
+        if self.cfg.CLI_MODE is True:
+            self.stop_task_received = asyncio.Event()
+
+        # self.datapool_rules_checker = DatapoolRulesChecker()
 
     def run(self):
         self.tasks.append(asyncio.create_task(self.router_loop()))
         self.eval_queue.run()
         self.topics_queue.run()
         super().run()
 
+    async def wait(self):
+        if self.cfg.CLI_MODE is False:
+            logger.error('baseproducer invalid usage')
+            raise InvalidUsageException("not a cli mode")
+
+        logger.info('BaseProducer wait()')
+        await self.stop_task_received.wait()
+        logger.info('BaseProducer stop_task_received')
+        waiters = (
+            self.eval_queue.until_empty(),
+            self.topics_queue.until_empty(),
+        )
+        await asyncio.gather(*waiters)
+        logger.info('BaseProducer wait done')
+
     async def stop(self):
         await self.eval_queue.stop()
         await self.topics_queue.stop()
         await super().stop()
+        logger.info("BaseProducer stopped")
 
     async def router_loop(self):
         try:
             while not await self.is_stopped():
                 message = await self.eval_queue.pop(timeout=1)
                 if message:
                     qm = QueueMessage.decode(message.body)
                     try:
-                        assert qm.type == QueueMessageType.Task
-
-                        task = qm.data
-                        logger.info(f"Producer got: {task}")
-
-                        # TODO: this storage must be associated with the worker!
-                        #   For example, storage path or url can be formatted accordingly to worker id
-                        worker_storage = FileStorage(
-                            self.cfg.WORKER_STORAGE_PATH
-                        )
-                        raw_data = await worker_storage.get(task["storage_id"])
-
-                        datapools = await self._get_tag_datapools(
-                            task["tag_id"]
-                        )
-                        logger.info(f"tag_id {task['tag_id']} in {datapools=}")
-                        for datapool_data in datapools:
-                            logger.info(
-                                f"matching content for {datapool_data['id']=}"
-                            )
-                            against = DatapoolRuleMatch(
-                                content_type=task[
-                                    "type"
-                                ],  # DatapoolContentType
-                                url=task[
-                                    "parent_url"
-                                ],  # for image it should be site image, not image src itself
+                        if qm.type == QueueMessageType.Task:
+                            task = qm.data
+                            logger.info(f"Producer got: {task}")
+
+                            # TODO: this storage must be associated with the worker!
+                            #   For example, storage path or url can be formatted accordingly to worker id
+                            worker_storage = FileStorage(
+                                self.cfg.WORKER_STORAGE_PATH
                             )
-                            content_rules = DatapoolRules(
-                                **datapool_data["rules"]
-                            )
-                            if self.datapool_rules_checker.match(
-                                content_rules, against
-                            ):
-                                logger.info("matched")
-                                await self.process_content(
-                                    datapool_data["id"], raw_data, task
-                                )
-                            else:
-                                logger.info("not matched")
+                            raw_data = await worker_storage.get(task["storage_id"])
+                            await self.process_content(qm.session_id, raw_data, task)
 
-                        # tell worker that his storage item can be removed
-                        await self.topics_queue.push(
-                            QueueTopicMessage(
-                                CrawlerWorker.get_storage_invalidation_topic(
-                                    task["worker_id"]
-                                ),
-                                {"storage_id": task["storage_id"]},
-                            )
-                        )
+                            if not self.is_shared_storage():
+                                # tell worker that his storage item can be removed
+                                await self.topics_queue.push(
+                                    QueueTopicMessage(
+                                        get_storage_invalidation_topic(
+                                            task["worker_id"]
+                                        ),
+                                        {"storage_id": task["storage_id"]},
+                                    )
+                                )
+                        elif qm.type == QueueMessageType.Stop:
+                            logger.info('base_producer: stop task received')
+                            self.stop_task_received.set()
+                        else:
+                            raise Exception(
+                                f"!!!!!!!!!!!!!!! BUG: unexpected {message=} {qm=}")
 
                         await self.eval_queue.mark_done(message)
                     except Exception as e:
                         logger.error(f"Catched: {traceback.format_exc()}")
                         logger.error(f"failed evaluate {e}")
                         await self.eval_queue.reject(message)
 
         except Exception as e:
             logger.error(f"Catched: {traceback.format_exc()}")
             logger.error(f"!!!!!!! Exception in Datapools::router_loop() {e}")
 
-    async def _get_tag_datapools(self, tag_id) -> TagDatapools:
-        # TODO: tag_id: datapool_ids pairs should be cached with cache TTL:
-        #   CACHE CONSIDERATION: user may leave datapool while datapool_id may still be associated with tag_id in cache
-        return await self.api.get_tag_datapools(tag_id)
-
-    async def process_content(self, datapool_id, raw_data, task):
-        # put data into persistent storage
-        await self.storage.put(
-            task["storage_id"], raw_data
-        )  # TODO: consider using datapool_id
+    async def process_content(self, session_id, raw_data, task):
+        # path = os.path.join(self.cfg.STORAGE_PATH, str(datapool_id))
+        if not self.is_shared_storage():
+            path = self.cfg.STORAGE_PATH
+            if not os.path.exists(path):
+                os.mkdir(path)
+            storage = FileStorage(path)
+            # put data into persistent storage
+            await storage.put(
+                task["storage_id"], raw_data
+            )
+
+        if self.session_manager.has(session_id):
+            session = self.session_manager.get(session_id)
+            session.inc_evaluated_content()
+
+    def is_shared_storage(self):
+        return self.cfg.STORAGE_PATH is None or self.cfg.WORKER_STORAGE_PATH == self.cfg.STORAGE_PATH
```

### Comparing `datapools-0.1.9/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py` & `datapools-1.0.41/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,83 +1,93 @@
 import asyncio
 import json
 import re
-#import traceback
 
-#from bs4 import BeautifulSoup
-#from playwright.async_api import Locator, Page
+# from bs4 import BeautifulSoup
+# from playwright.async_api import Locator, Page
 from playwright.async_api import TimeoutError as PlaywriteTimeoutError
 from playwright.async_api import async_playwright, expect
 
 from ....common.logger import logger
 from ....common.storage import BaseStorage
 from ....common.types import (
     CrawlerBackTask,
     CrawlerContent,
     CrawlerNop,
     DatapoolContentType,
 )
-from ..base_plugin import BasePlugin
+from ..base_plugin import BasePlugin, WorkerTask
+
+# import traceback
 
 
 class DataPhoenixInfoPlugin(BasePlugin):
-    def __init__(self, storage):
-        super().__init__(storage)
+    def __init__(self, ctx):
+        super().__init__(ctx)
         self.header_tag_id = None
 
-    def is_supported(self, url):
-        u = self.parse_url(url)
+    @staticmethod
+    def is_supported(url):
+        u = BasePlugin.parse_url(url)
         # logger.info( f'dataphoenix.info {u=}')
         return u.netloc == "dataphoenix.info"
 
-    async def process(self, url):
-        logger.info(f"dataphoenix_info::process({url})")
+    async def process(self, task: WorkerTask):
+        logger.info(f"dataphoenix_info::process({task.url})")
 
         async with async_playwright() as playwright:
-            self.webkit = playwright.webkit
+            self.webkit = playwright.chromium
             self.browser = await self.webkit.launch()
             self.context = await self.browser.new_context()
             self.page = await self.context.new_page()
 
             # async with httpx.AsyncClient() as client:
             #     logger.info( f'loading url {url}')
 
             #     r = await client.get( url )
             #     #logger.info( f'got Response {r}')
             #     r = r.text
-            logger.info(f"loading url {url}")
-            await self.page.goto(url)  # "https://dataphoenix.info/news/"
-            logger.info(f"loaded {url=}")
+            logger.info(f"loading url {task.url}")
+            await self.page.goto(str(task.url))  # "https://dataphoenix.info/news/"
 
             # check if <meta/> tag exists with our tag
-            self.header_tag_id = await BasePlugin.parse_meta_tag(self.page, 'robots')
+            self.header_tag_id = await BasePlugin.parse_meta_tag(
+                self.page, "robots"
+            )
+            logger.info(f"{self.header_tag_id=}")
+
             if not self.header_tag_id:
-                logger.info("No <meta> tag found, give up")
+                logger.info("No <meta> tag found")
                 return
 
-            logger.info(f"{self.header_tag_id=}")
+            if self.header_tag_id.is_crawling_allowed() is False:
+                logger.info("crawling disabled")
+                return
 
             if re.match(
                 "^http(s?)://dataphoenix.info/(news|papers|articles|videos)(?:$|/)",
-                url,
+                str(task.url),  #linter..
             ):
                 logger.info("parsing feed")
-                async for yielded in self._process_feed(url):
+                async for yielded in self._process_feed(task.url):
                     yield yielded
             else:
                 logger.info("parsing single page")
-                async for yielded in self._process_single_page(url):
+                async for yielded in self._process_single_page(task.url):
                     yield yielded
 
     async def _process_single_page(self, url):
         # article consists of header, excerpt and body
         # TODO: support video
         header = await self.page.locator("h1.c-post-header__title").all()
         if len(header) == 0:
             logger.error("Not parsable page (header)")
+            # await self.page.screenshot(
+            #     path="/app/tmp/not_parsable_page_header.png"
+            # )
             return
         header = await header[0].inner_text()
 
         # optional Excerpt
         excerpt = await self.page.locator("p.c-post-header__excerpt").all()
         if len(excerpt) > 0:
             excerpt = await excerpt[0].inner_text()
@@ -88,21 +98,21 @@
         ps = await self.page.locator("section.c-content > p").all()
         for p in ps:
             body += await p.inner_text() + "\n"
 
         storage_id = BaseStorage.gen_id(url)
         logger.info(f"putting article into {storage_id=}")
 
-        await self.storage.put(
+        await self.ctx.storage.put(
             storage_id,
-            json.dumps({"header": header, "excerpt": excerpt, "body": body}),
+            BasePlugin.make_text_storage_value(body, header=header, excerpt=excerpt )
         )
 
         yield CrawlerContent(
-            tag_id=self.header_tag_id,
+            tag_id=str(self.header_tag_id),
             type=DatapoolContentType.Text,
             storage_id=storage_id,
             url=url,
         )
 
     async def _process_feed(self, url):
         total_news = 0
@@ -143,23 +153,23 @@
                 except PlaywriteTimeoutError:
                     # logger.info( e )
                     # logger.info( traceback.format_exc() )
                     await self._try_remove_banner()
 
             if not ready:
                 logger.error("ready wait failed error")
-                await self.page.screenshot(path="/app/tmp/screenshot.png")
+                # await self.page.screenshot(path="/app/tmp/screenshot.png")
                 break
 
             try:
                 await button.click(no_wait_after=True, timeout=10000)
                 # logger.info( "clicked More Posts")
             except PlaywriteTimeoutError:
                 logger.error("click More Posts timeout")
-                await self.page.screenshot(path="/app/tmp/screenshot.png")
+                # await self.page.screenshot(path="/app/tmp/screenshot.png")
                 break
 
             button = self.page.locator("button.js-load-posts.c-btn--loading")
             await button.wait_for()
             logger.info("button changed to Loading")
 
             button = self.page.locator(
```

### Comparing `datapools-0.1.9/datapools/worker/plugins/google_drive/google_drive.py` & `datapools-1.0.41/datapools/worker/plugins/google_drive/google_drive.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,169 +1,195 @@
-#import os
-import asyncio
-import io
+# import os
+# import asyncio
+# import io
 import traceback
 
-#from google.auth.transport.requests import Request
-#from google.oauth2.credentials import Credentials
-#from google_auth_oauthlib.flow import InstalledAppFlow
-from googleapiclient.discovery import build
-#from googleapiclient.errors import HttpError
-
 from google.auth.api_key import Credentials
-from googleapiclient.http import MediaIoBaseDownload
 
-from ..base_plugin import BasePlugin, BasePluginException
-from ....common.storage import BaseStorage
+# from google.auth.transport.requests import Request
+# from google.oauth2.credentials import Credentials
+# from google_auth_oauthlib.flow import InstalledAppFlow
+from googleapiclient.discovery import build
+# from googleapiclient.http import MediaIoBaseDownload
+
 from ....common.logger import logger
-from ....common.types import (
-    CrawlerContent,
-)
+from ....common.storage import BaseStorage
+from ....common.types import CrawlerContent, DatapoolContentType
+from ..base_plugin import BasePlugin, BasePluginException, WorkerTask
+
+# from googleapiclient.errors import HttpError
 
 
 # If modifying these scopes, delete the file token.json.
-#SCOPES = ['https://www.googleapis.com/auth/drive.metadata.readonly']
+# SCOPES = ['https://www.googleapis.com/auth/drive.metadata.readonly']
+
 
 class GoogleDrivePlugin(BasePlugin):
-    def __init__(self, storage, api_key ):
-        super().__init__(storage)
+    def __init__(self, ctx, api_key):
+        super().__init__(ctx)
         self.creds = Credentials(api_key)
 
-#https://drive.google.com/drive/folders/1CPDmula2V83KWOocJR9jVvsTk6tVSpKd?usp=sharing
+    # https://drive.google.com/drive/folders/1CPDmula2V83KWOocJR9jVvsTk6tVSpKd?usp=sharing
 
-    def is_supported( self, url ):
-        u = self.parse_url(url)
-        if u.netloc == 'drive.google.com':
-            if u.path[0:15] == '/drive/folders/':
+    @staticmethod
+    def is_supported(url):
+        u = BasePlugin.parse_url(url)
+        if u.netloc == "drive.google.com":
+            if u.path[0:15] == "/drive/folders/":
                 return True
-            
-        return False    
-        
-
-    async def process(self, url):
-        u = self.parse_url(url)
-        folder_id = u.path.split('/')[3]
-        
+
+        return False
+
+    async def process(self, task: WorkerTask):
+        u = self.parse_url(task.url)
+        folder_id = u.path.split("/")[3]
+
         try:
-            with build('drive', 'v3', credentials=self.creds) as drive:
-                self.tag_id = await self.find_license( folder_id, drive )
-                if self.tag_id:
-                    async for msg in self.scan_folder( folder_id, drive ):
+            with build("drive", "v3", credentials=self.creds) as drive:
+                self.tag_id = await self.find_license(folder_id, drive)
+                if self.tag_id and self.tag_id.is_crawling_allowed():
+                    async for msg in self.scan_folder(folder_id, drive):
                         yield msg
         except Exception as e:
-            logger.error(f'GoogleDrivePlugin exception {e}')
-            logger.error( traceback.format_exc())
-            
+            logger.error(f"GoogleDrivePlugin exception {e}")
+            logger.error(traceback.format_exc())
+
     def _get_download_url(self, file_id):
-        #this url can be placed on site for preview
-        return f'https://drive.google.com/uc?id={file_id}'
-        
-        #return f"https://www.googleapis.com/drive/v3/files/{file_id}?alt=media&key={self.creds.token}"
-    
-    async def find_license( self, folder_id, drive ):
-        try:        
-            license = drive.files().list(q = f"name='{BasePlugin.license_filename}' and '{folder_id}' in parents", pageSize=1, fields="files(id)").execute()
-            file_id = license.get('files')[0]['id']
-            
+        # this url can be placed on site for preview
+        return f"https://drive.google.com/uc?id={file_id}"
+
+        # return f"https://www.googleapis.com/drive/v3/files/{file_id}?alt=media&key={self.creds.token}"
+
+    async def find_license(self, folder_id, drive):
+        try:
+            license = (
+                drive.files().list(
+                    q=f"name='{BasePlugin.license_filename}' and '{folder_id}' in parents",
+                    pageSize=1, fields="files(id)",).execute())
+            file_id = license.get("files")[0]["id"]
+
             url = self._get_download_url(file_id)
             # headers = { "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,*/*;q=0.8",
-			#             "Accept-Encoding":"gzip, deflate, br",
-			#             "Accept-Language":"en-US,en;q=0.5",
-			#             "Connection":"keep-alive",
+            #             "Accept-Encoding":"gzip, deflate, br",
+            #             "Accept-Language":"en-US,en;q=0.5",
+            #             "Connection":"keep-alive",
             #             "Sec-Fetch-Dest":"document",
-			#             "Sec-Fetch-Mode":"navigate",
-			#             "Sec-Fetch-Site":"none",
-			#             "Sec-Fetch-User":"?1",
-			#             "TE":"trailers",
-			#             "Upgrade-Insecure-Requests":"1",
-			#             "User-Agent":"Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/118.0"
-			# }
+            #             "Sec-Fetch-Mode":"navigate",
+            #             "Sec-Fetch-Site":"none",
+            #             "Sec-Fetch-User":"?1",
+            #             "TE":"trailers",
+            #             "Upgrade-Insecure-Requests":"1",
+            #             "User-Agent":"Mozilla/5.0 (X11; Ubuntu; Linux x86_64; rv:109.0) Gecko/20100101 Firefox/118.0"
+            # }
             headers = {}
-            tag_id = await self.download( url, headers )
-            logger.info(f'download {tag_id=}')
+            tag_id = await self.download(url, headers)
+            logger.info(f"download {tag_id=}")
             tag_id = await BasePlugin.parse_tag_in(tag_id.decode())
-            logger.info( f'{tag_id=}')
+            logger.info(f"{tag_id=}")
             return tag_id
-            
-            # file = drive.files().get( fileId=file_id ).execute()                    
-            
+
+            # file = drive.files().get( fileId=file_id ).execute()
+
             # logger.info( f'downloading file {file_id} {file["name"]}')
             # fileRequest = drive.files().get_media(fileId=file_id)
             # fh = io.BytesIO()
             # downloader = MediaIoBaseDownload(fh, fileRequest)
             # done = False
             # while done is False:
             #     status, done = downloader.next_chunk()
             # fh.seek(0)
             # tag_id = fh.read().strip()
             # tag_id = await BasePlugin.parse_tag_in(tag_id)
-            
+
             # logger.info( f'{tag_id=}')
-            
-            #return tag_id            
+
+            # return tag_id
         except Exception:
             pass
-        
-        
-    async def scan_folder( self, folder_id, drive ):
-        logger.info( f'scanning folder {folder_id}')
-        #print(folder_id)
+
+    async def scan_folder(self, folder_id, drive):
+        logger.info(f"scanning folder {folder_id}")
+        # print(folder_id)
         # this gives us a list of all folders with that name
-        #folder = drive.files().get( fileId=folder_id ).execute()
+        # folder = drive.files().get( fileId=folder_id ).execute()
         # print(type(folder))
-        
+
         page_token = None
         while True:
-            results = drive.files().list(q = "'" + folder_id + "' in parents", pageSize=10, pageToken=page_token, fields="nextPageToken, files(id, name)").execute()
-            items = results.get('files', [])
-            page_token = results.get( 'nextPageToken', None )
+            results = (
+                drive.files()
+                .list(
+                    q="'" + folder_id + "' in parents",
+                    pageSize=10,
+                    pageToken=page_token,
+                    fields="nextPageToken, files(id, name)",
+                )
+                .execute()
+            )
+            items = results.get("files", [])
+            page_token = results.get("nextPageToken", None)
 
             # Now we can loop through each file in that folder, and do whatever (in this case, download them and open them as images in OpenCV)
             for f in range(0, len(items)):
-                #print( items[f])
-                
-                file_id = items[f].get('id')
-                logger.info(f'{file_id=}')
-                
-                file = drive.files().get( fileId=file_id ).execute()
+                # print( items[f])
+
+                file_id = items[f].get("id")
+                logger.info(f"{file_id=}")
+
+                file = drive.files().get(fileId=file_id).execute()
                 logger.info(f"{file['mimeType']=}")
-                
-                if file[ 'mimeType' ] == 'application/vnd.google-apps.folder':
-                    async for yielded in self.scan_folder( file_id, drive ):
+
+                if file["mimeType"] == "application/vnd.google-apps.folder":
+                    async for yielded in self.scan_folder(file_id, drive):
                         yield yielded
                 else:
                     try:
-                        datapool_content_type = BasePlugin.get_content_type_by_mime_type( file[ 'mimeType' ] )
+                        datapool_content_type = (
+                            BasePlugin.get_content_type_by_mime_type(
+                                file["mimeType"]
+                            )
+                        )
                     except BasePluginException:
-                        logger.error( f'Not supported mime type {file["mimeType"]}')
-                    
-                    logger.info( f'downloading file {file_id} {file["name"]}')
-                        #TODO: this works too, but is getting blocked  when running from lsrv2
-                        # fileRequest = drive.files().get_media(fileId=file_id)
-                        # fh = io.BytesIO()
-                        # downloader = MediaIoBaseDownload(fh, fileRequest)
-                        # done = False
-                        # while done is False:
-                        #     status, done = downloader.next_chunk()
-                        # fh.seek(0)
-                        # content = fh.read()
-                    #direct url seems to work better than API access
+                        logger.error(
+                            f'Not supported mime type {file["mimeType"]}'
+                        )
+
+                    logger.info(f'downloading file {file_id} {file["name"]}')
+                    # TODO: this works too, but is getting blocked  when running from lsrv2
+                    # fileRequest = drive.files().get_media(fileId=file_id)
+                    # fh = io.BytesIO()
+                    # downloader = MediaIoBaseDownload(fh, fileRequest)
+                    # done = False
+                    # while done is False:
+                    #     status, done = downloader.next_chunk()
+                    # fh.seek(0)
+                    # content = fh.read()
+                    # direct url seems to work better than API access
                     url = self._get_download_url(file_id)
-                    content = await self.download( url )
-                    
-                    print( f'file size={len(content)}')
-                    
-                    #obj_url = f'https://drive.google.com/file/d/{file_id}/view'
-                    obj_url = url
-                    storage_id = BaseStorage.gen_id(obj_url)
-                    await self.storage.put( storage_id, content )
-                    
-                    yield CrawlerContent(tag_id=self.tag_id,
-                                            type=datapool_content_type,
-                                            storage_id=storage_id,
-                                            url=obj_url)
-                    
-                
-                #baseImage = cv2.imdecode(np.fromstring(fhContents, dtype=np.uint8), cv2.IMREAD_COLOR)
+                    content = await self.download(url)
+                    if content is not None:
+                        logger.info(f"file size={len(content)}")
+
+                        image_tag = None
+                        if datapool_content_type == DatapoolContentType.Image:
+                            image_tag = BasePlugin.parse_image_tag(content)
+                            if image_tag is not None and image_tag.is_crawling_allowed() is False:
+                                logger.info(
+                                    f'crawling is disabled by image tag: {str(image_tag)}')
+                                continue
+
+                        # obj_url = f'https://drive.google.com/file/d/{file_id}/view'
+                        obj_url = url
+                        storage_id = BaseStorage.gen_id(obj_url)
+                        await self.ctx.storage.put(storage_id, content)
+
+                        yield CrawlerContent(
+                            tag_id=str(image_tag) if image_tag is not None else None,
+                            copyright_tag_id=str(self.tag_id),
+                            type=datapool_content_type,
+                            storage_id=storage_id,
+                            url=obj_url,
+                        )
+
+                # baseImage = cv2.imdecode(np.fromstring(fhContents, dtype=np.uint8), cv2.IMREAD_COLOR)
             if page_token is None:
                 break
-
```

### Comparing `datapools-0.1.9/datapools/worker/plugins/s3/s3.py` & `datapools-1.0.41/datapools/worker/plugins/s3/s3.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,124 +1,157 @@
-import asyncio
+# import asyncio
+import tempfile
 import traceback
+
 import boto3
+import filetype
 from botocore import UNSIGNED
-from botocore.exceptions import ClientError
 from botocore.client import Config
-import filetype
-import tempfile
+from botocore.exceptions import ClientError
 
-from ..base_plugin import BasePlugin, BasePluginException
-from ....common.storage import BaseStorage
 from ....common.logger import logger
-from ....common.types import (
-#    CrawlerBackTask,
-    CrawlerContent,
-    CrawlerNop,
-    DatapoolContentType,
-)
+from ....common.storage import BaseStorage
+
+# from ....common.types import CrawlerNop  # CrawlerBackTask,
+from ....common.types import CrawlerContent, DatapoolContentType
+from ..base_plugin import BasePlugin, BasePluginException, WorkerTask
+
 
 class S3Exception(BasePluginException):
     pass
 
+
 class S3Plugin(BasePlugin):
-    def __init__(self, storage, aws_access_key_id=None, aws_secret_access_key=None):
-        super().__init__(storage)
-        
-        logger.info( f'{aws_access_key_id=}')
-        logger.info( f'{aws_secret_access_key=}')
-        
-        #empty key means bucket is public
-        if aws_access_key_id == '':
+    def __init__(
+        self, ctx, aws_access_key_id=None, aws_secret_access_key=None
+    ):
+        super().__init__(ctx)
+
+        logger.info(f"{aws_access_key_id=}")
+        logger.info(f"{aws_secret_access_key=}")
+
+        # empty key means bucket is public
+        if aws_access_key_id == "":
             self.is_public_bucket = True
-            self.s3_client = boto3.client('s3', config=Config(signature_version=UNSIGNED))
-            self.s3 = boto3.resource('s3', config=Config(signature_version=UNSIGNED))
+            self.s3_client = boto3.client(
+                "s3", config=Config(signature_version=UNSIGNED)
+            )
+            self.s3 = boto3.resource(
+                "s3", config=Config(signature_version=UNSIGNED)
+            )
         else:
             self.is_public_bucket = False
-            self.s3_client = boto3.client('s3', aws_access_key_id=aws_access_key_id, aws_secret_access_key=aws_secret_access_key)    
-            self.s3 = boto3.resource('s3', aws_access_key_id=aws_access_key_id, aws_secret_access_key=aws_secret_access_key)
-        
-        
-
-    def is_supported(self, url):
-        u = self.parse_url(url)
-        logger.info( f'============ s3 {u=} =====================================')
-        if u.netloc == 's3.console.aws.amazon.com':
-            logger.info( 'netloc ok')
-            if u.path[0:12] == '/s3/buckets/':
-                logger.info( 'path ok')
+            self.s3_client = boto3.client(
+                "s3",
+                aws_access_key_id=aws_access_key_id,
+                aws_secret_access_key=aws_secret_access_key,
+            )
+            self.s3 = boto3.resource(
+                "s3",
+                aws_access_key_id=aws_access_key_id,
+                aws_secret_access_key=aws_secret_access_key,
+            )
+
+    @staticmethod
+    def is_supported(url):
+        u = BasePlugin.parse_url(url)
+        # logger.info( f'============ s3 {u=} =====================================')
+        if u.netloc == "s3.console.aws.amazon.com":
+            # logger.info( 'netloc ok')
+            if u.path[0:12] == "/s3/buckets/":
+                # logger.info( 'path ok')
                 return True
             # elif u.path[0:6] == '/watch' and u.query[0:2] == 'v=':
             #     self.video_id = u.query[2:13]
             #     return True
-            
-        return False    
-    
-    
-    async def process(self, url):
-        logger.info(f"s3::process({url})")
-        
-        u = self.parse_url(url)
-        self.bucket_name = u.path.split('/')[3]
-        logger.info( f'{self.bucket_name=}')
-        
-        bucket = self.s3.Bucket( self.bucket_name )
-        
+
+        return False
+
+    async def process(self, task: WorkerTask):
+        logger.info(f"s3::process({task.url})")
+
+        u = self.parse_url(task.url)
+        self.bucket_name = u.path.split("/")[3]
+        logger.info(f"{self.bucket_name=}")
+
+        bucket = self.s3.Bucket(self.bucket_name)
+
         try:
-            tag_id = self._download( BasePlugin.license_filename )
-            tag_id = await BasePlugin.parse_tag_in(tag_id.decode())
-            logger.info( f'found license: {tag_id}')
+            copyright_tag_id = self._download(BasePlugin.license_filename)
+            copyright_tag = await BasePlugin.parse_tag_in(copyright_tag_id.decode())
+            logger.info(f"found license: {copyright_tag_id}")
+            if copyright_tag is not None and copyright_tag.is_crawling_allowed() is False:
+                logger.info('crawling disabled by copyright owner')
+                return
         except S3Exception:
-            logger.error( 'bucket does not contain license.txt, cannot process(1)')
-            logger.error( traceback.format_exc())
+            logger.error(
+                "bucket does not contain license.txt, cannot process(1)"
+            )
+            logger.error(traceback.format_exc())
             return
         except ClientError:
-            logger.error( 'bucket does not contain license.txt, cannot process(2)')
-            logger.error( traceback.format_exc())
+            logger.error(
+                "bucket does not contain license.txt, cannot process(2)"
+            )
+            logger.error(traceback.format_exc())
             return
 
         for obj in bucket.objects.all():
-            logger.info( f'{obj=}')
-            
+            logger.info(f"{obj=}")
+
             if obj.key == BasePlugin.license_filename:
                 continue
-            
+
             if self.is_public_bucket is False:
-                #THIS IS PURE API ACCESS URL
-                obj_url = f'https://s3.console.aws.amazon.com/s3/buckets/{self.bucket_name}/{obj.key}'
+                # THIS IS PURE API ACCESS URL
+                obj_url = f"https://s3.console.aws.amazon.com/s3/buckets/{self.bucket_name}/{obj.key}"
             else:
-                #THIS IS DIRECT URL ( FOR PUBLIC BUCKETS )
-                #TODO: region?
-                obj_url = f'https://{self.bucket_name}.s3.amazonaws.com/{obj.key}'
+                # THIS IS DIRECT URL ( FOR PUBLIC BUCKETS )
+                # TODO: region?
+                obj_url = (
+                    f"https://{self.bucket_name}.s3.amazonaws.com/{obj.key}"
+                )
 
             storage_id = BaseStorage.gen_id(obj_url)
-            
-            content = self._download( obj.key )
-            
+
+            content = self._download(obj.key)
+
             try:
                 type = self._get_datapool_content_type(content)
-                
-                await self.storage.put(
-                            storage_id,
-                            content
-                        )
-                
-                yield CrawlerContent(tag_id=tag_id,
-                                            type=type,
-                                            storage_id=storage_id,
-                                            url=obj_url)            
+
+                if type == DatapoolContentType.Image:
+                    image_tag = BasePlugin.parse_image_tag(content)
+                    if image_tag is not None:
+                        if image_tag.is_crawling_allowed() is False:
+                            logger.info(
+                                f'crawling is disabled by image tag: {str(image_tag)}')
+                            continue
+                    else:
+                        if copyright_tag is None:
+                            logger.info(
+                                'no image tag, nor copyright tag, skipped')
+                            continue
+
+                await self.ctx.storage.put(storage_id, content)
+
+                yield CrawlerContent(
+                    tag_id=str(image_tag) if image_tag is not None else None,
+                    copyright_tag_id=str(copyright_tag) if copyright_tag is not None else None,
+                    type=type,
+                    storage_id=storage_id,
+                    url=obj_url,
+                )
             except S3Exception as e:
-                logger.info( f"mime type not supported/detected: {e}" )
+                logger.info(f"mime type not supported/detected: {e}")
 
-    def _download( self, key ):
+    def _download(self, key):
         with tempfile.NamedTemporaryFile() as tmp:
-            self.s3_client.download_fileobj( self.bucket_name, key, tmp )
-            
-            tmp.seek(0,0)
+            self.s3_client.download_fileobj(self.bucket_name, key, tmp)
+
+            tmp.seek(0, 0)
             return tmp.read()
-        
+
     def _get_datapool_content_type(self, content):
-        type = filetype.guess( content )
+        type = filetype.guess(content)
         if type is None:
-            raise S3Exception(f"unknown file type")
-        return BasePlugin.get_content_type_by_mime_type( type.mime )
-        
+            raise S3Exception("unknown file type")
+        return BasePlugin.get_content_type_by_mime_type(type.mime)
```

### Comparing `datapools-0.1.9/datapools/worker/worker.py` & `datapools-1.0.41/datapools/scheduler/scheduler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,274 +1,280 @@
 import asyncio
-import importlib
-import inspect
-import os
-# import sys
+
+# import json
 # import time
 import traceback
-import uuid
 from typing import Optional
 
-import aio_pika
-# import httpx
-
+from ..common.backend_api import BackendAPI
 from ..common.logger import logger
 from ..common.queues import (
+    GenericQueue,
     QueueMessage,
     QueueMessageType,
     QueueRole,
-    QueueTopicMessage,
-    RabbitmqParams,
-    RabbitmqQueue,
 )
 from ..common.stoppable import Stoppable
-from ..common.storage import FileStorage
-from ..common.types import WorkerSettings, QUEUE_WORKER_TASKS, QUEUE_REPORTS, QUEUE_EVAL_TASKS, TOPICS_EXCHANGE_NAME,\
-    CrawlerContent, CrawlerHintURLStatus, DatapoolContentType, CrawlerBackTask, CrawlerNop
 
+# from .common.tasks_db import Hash
+# from .common.tasks_db.redis import RedisTasksDB
+from ..common.session_manager import SessionManager
+from ..common.types import (
+    DatapoolContentType,
+    CrawlerHintURLStatus,
+    SchedulerSettings,
+    InvalidUsageException,
+)
+
+# import httpx
+
+
+class CrawlerScheduler(Stoppable):
+    # 1. task:
+    #   - get hint urls from the backend, put into tasks_db, status is changed at the backend at once
+    #   - check "processing" tasks: ping worker. If it's dead then task is moved back to the queue
+    # 2. api: get urls from workers, put into tasks_db
+    #   tips:
+    #   - reject existing urls: request redis by url hash
+    # 3. api: worker gets a new task(s?) from queue:
+    #   tips:
+    #   - tasks_db: (redis) task should be moved into a separate key as "in progress", worker ID/IP/etc should be remembered to be able to ping
+    # 4. api: worker notifies about finished task
+    #    - remove task from "processing"
+    #    - if it's a backend hint url, then update its status by calling backend api
+
+    cli_tasks: Optional[asyncio.Queue] = None
 
-class CrawlerWorker(Stoppable):
-    def __init__(self, cfg: Optional[WorkerSettings] = None):
+    def __init__(self, cfg: Optional[SchedulerSettings] = None):
         super().__init__()
-        self.cfg = cfg if cfg is not None else WorkerSettings()
-        self.id = uuid.uuid4().hex
-        logger.info(f"worker id={self.id}")
-        self.storage = FileStorage(self.cfg.STORAGE_PATH)
-        self.init_plugins()
-        self.todo_queue = RabbitmqQueue(
-            QueueRole.Receiver,
-            self.cfg.RABBITMQ_CONNECTION_URL,
-            QUEUE_WORKER_TASKS,
-        )
-        self.reports_queue = RabbitmqQueue(
-            QueueRole.Publisher,
-            self.cfg.RABBITMQ_CONNECTION_URL,
-            QUEUE_REPORTS,
+        self.cfg = cfg if cfg is not None else SchedulerSettings()
+
+        if self.cfg.CLI_MODE is True:
+            self.cli_tasks = asyncio.Queue()
+        else:
+            self.api = BackendAPI(url=self.cfg.BACKEND_API_URL)
+
+        self.session_manager = SessionManager(
+            self.cfg.REDIS_HOST, self.cfg.REDIS_PORT)
+
+        # self.tasks_db = RedisTasksDB(
+        #     host=self.cfg.REDIS_HOST, port=self.cfg.REDIS_PORT
+        # )
+        self.todo_queue = GenericQueue(
+            role=QueueRole.Publisher,
+            url=self.cfg.QUEUE_CONNECTION_URL,
+            name=self.cfg.WORKER_TASKS_QUEUE_NAME,
         )
-        self.producer_queue = RabbitmqQueue(
-            QueueRole.Publisher,
-            self.cfg.RABBITMQ_CONNECTION_URL,
-            QUEUE_EVAL_TASKS,
+        logger.info("created publisher worker_tasks")
+        self.reports_queue = GenericQueue(
+            role=QueueRole.Receiver,
+            url=self.cfg.QUEUE_CONNECTION_URL,
+            name=self.cfg.WORKER_REPORTS_QUEUE_NAME,
         )
-        self.topics_queue = RabbitmqQueue(
-            QueueRole.Receiver,
-            self.cfg.RABBITMQ_CONNECTION_URL,
-            "",
-            RabbitmqParams(
-                exchange_type=aio_pika.ExchangeType.TOPIC,
-                exchange_name=TOPICS_EXCHANGE_NAME,
-                routing_key=CrawlerWorker.get_storage_invalidation_topic(
-                    self.id
-                ),
-            ),
+        logger.info("created receiver reports")
+
+        if self.cfg.CLI_MODE:
+            self.cli_session = self.session_manager.create()
+            logger.info(f'created session {self.cli_session.id}')
+
+            # TODO: this mechanism will not work for multiple workers/producers
+            self.stop_task_processed = asyncio.Event()
+
+    async def wait(self):
+        """for CLI mode usage only"""
+        if not self.cfg.CLI_MODE:
+            logger.error('scheduler invalid usage')
+            raise InvalidUsageException("not a cli mode")
+
+        await self.stop_task_processed.wait()
+
+        waiters = (
+            self.todo_queue.until_empty(),
+            self.reports_queue.until_empty(),
         )
+        await asyncio.gather(*waiters)
+        logger.info('scheduler wait done')
 
     def run(self):
-        # self.tasks.append( asyncio.create_task( self.tasks_fetcher_loop() ) )
+        self.tasks.append(asyncio.create_task(self.hints_loop()))
+        self.tasks.append(asyncio.create_task(self.reports_loop()))
         self.todo_queue.run()
         self.reports_queue.run()
-        self.producer_queue.run()
-        self.topics_queue.run()
-        self.tasks.append(asyncio.create_task(self.worker_loop()))
-        self.tasks.append(asyncio.create_task(self.topics_loop()))
         super().run()
 
     async def stop(self):
+        logger.info("scheduler stopping")
         await self.todo_queue.stop()
+        logger.info("todo_queue stopped")
         await self.reports_queue.stop()
-        await self.producer_queue.stop()
-        await self.topics_queue.stop()
+        logger.info("reports_queue stopped")
         await super().stop()
+        logger.info("super stopped")
+
+    async def _set_task_status(self, session_id, data):
+        # hash, status: CrawlerHintURLStatus, contents
+        logger.info(f"set_task_status: {session_id=} {data=}")
+
+        session = self.session_manager.get(session_id)
+
+        meta = session.get_meta()
+        logger.info(f'{meta=}')
+        if not meta:
+            return False
+
+        status = CrawlerHintURLStatus(data["status"])
+
+        if status in (
+                CrawlerHintURLStatus.Success, CrawlerHintURLStatus.Failure,
+                CrawlerHintURLStatus.Rejected):
+            if status == CrawlerHintURLStatus.Success:
+                session.inc_complete_urls()
+            elif status == CrawlerHintURLStatus.Failure:
+                session.inc_failed_urls()
+            else:
+                session.inc_rejected_urls()
+
+            if (meta['total_tasks'] == meta['complete_tasks'] + meta['failed_tasks'] + meta['rejected_tasks'] + 1
+                # and meta[ 'crawled_content'] == meta[ 'evaluated_content']      <--- this will not work here, because producer will evaluate later than task is complete
+                    and meta['hint_id'] is not None):
+                # this is hint url from server => have to update status on the backend
+                if not self.cfg.CLI_MODE:
+                    await self.api.set_hint_url_status(meta["hint_id"], status, session_id)
+
+    async def _add_task(self, session_id, task: dict):
+        if not self.session_manager.has(session_id):
+            logger.error(f'Session not found: {session_id=}')
+            return False
+
+        session = self.session_manager.get(session_id)
+
+        if 'url' in task:
+            if not session.has_url(task['url']):
+                session.add_url(task['url'])
 
-    def init_plugins(self):
-        self.plugins = []
-        plugins_dir = os.path.join(os.path.dirname(__file__), "plugins")
-        logger.info( f'{plugins_dir=}')
-
-        for dir in os.listdir(plugins_dir):
-            if dir != "__pycache__" and os.path.isdir(
-                os.path.join(plugins_dir, dir)
-            ):
-                logger.info(f"loading module {dir}")
-                module = importlib.import_module(
-                    f"datapools.worker.plugins.{dir}"
+                await self.todo_queue.push(
+                    QueueMessage(session_id, QueueMessageType.Task, data=task)
                 )
-                clsmembers = inspect.getmembers(module, inspect.isclass)
-                # logger.info( f'{clsmembers=}')
+            else:
+                logger.info('task exists, ignored')
+                return False
+        elif 'stop_running' in task:
+            await self.todo_queue.push(
+                QueueMessage(session_id, QueueMessageType.Stop)
+            )
+        else:
+            raise Exception(f'unsupported {task=}')
 
-                for cls in clsmembers:
-                    for base in cls[1].__bases__:
-                        # logger.info( f'{base=}')
-                        if base.__name__ == "BasePlugin":
-                            # logger.info( f'valid plugin class {cls[1]}')
-                            self.plugins.append(cls)
-                            break
+        # logger.info( 'pushed')
+        return True
+        # return hash
+
+    # return False
+
+    async def add_download_task(self, url, content_type: Optional[DatapoolContentType] = None):
+        """for cli mode: pushing url to the queue. Scheduler will run until empty string is added"""
+        if self.cli_tasks is None:
+            logger.error('scheduler invalid usage')
+            raise InvalidUsageException("not a cli mode")
+        await self.cli_tasks.put((url, content_type))
+
+    async def _get_hints(self):
+        hints = None
+        if not self.cfg.CLI_MODE:
+            # deployment mode
+            try:
+                hints = await self.api.get_hint_urls(limit=10)
+                for hint in hints:
+                    session = self.session_manager.create(
+                        hint_id=hint.get('id', 0),
+                        url=hint.get('url', '')
+                    )
+                    hint['session_id'] = session.id
+
+            except Exception as e:
+                logger.error(f"Failed get hints: {e}")
+        else:
+            # cli mode
+            try:
+                (url, content_type) = await asyncio.wait_for(self.cli_tasks.get(), timeout=1)
+                if len(url) > 0:
+                    hints = [{"url": url, "content_type": content_type,
+                              "session_id": self.cli_session.id}]
+                else:
+                    hints = [{'stop_running': True,
+                              "session_id": self.cli_session.id}]
+            except asyncio.TimeoutError:
+                pass
+        return hints
 
-    async def topics_loop(self):
-        # receives storage_id which content can be removed from Evaluator
+    async def hints_loop(self):
+        # infinitely fetching URL hints by calling backend api
         try:
             while not await self.is_stopped():
-                message = await self.topics_queue.pop(timeout=1)
-                if message:
-                    qm = QueueTopicMessage.decode(
-                        message.routing_key, message.body
-                    )
-                    if (
-                        message.routing_key
-                        == CrawlerWorker.get_storage_invalidation_topic(
-                            self.id
-                        )
-                    ):
-                        logger.info(
-                            f"invalidating storage {qm.data[ 'storage_id' ]}"
-                        )
-                        await self.storage.remove(qm.data["storage_id"])
-
-                        await self.topics_queue.mark_done(message)
-                    else:
-                        logger.error(
-                            f"!!!!!!!!!!!!!!! BUG: unexpected topic {message=} {qm=}"
-                        )
-                        await self.topics_queue.reject(message)
+                if self.session_manager.is_ready():
+                    hints = await self._get_hints()
+                    if hints is not None:
+                        for hint in hints:
+                            logger.info(f"got hint: {hint}")
+
+                            if await self._add_task(
+                                hint.get('session_id'),
+                                hint
+                            ):
+                                if "id" in hint:
+                                    await self.api.set_hint_url_status(
+                                        hint["id"],
+                                        CrawlerHintURLStatus.Processing,
+                                        hint['session_id']
+                                    )
+                            else:
+                                logger.error('failed add task, REJECTING')
+                                if "id" in hint:
+                                    await self.api.set_hint_url_status(
+                                        hint["id"],
+                                        CrawlerHintURLStatus.Rejected,
+                                    )
+                                    self.session_manager.remove(
+                                        hint['session_id'])
+
+                    if not self.cfg.CLI_MODE:
+                        await asyncio.sleep(self.cfg.BACKEND_HINTS_PERIOD)
+                else:
+                    await asyncio.sleep(1)
         except Exception as e:
-            logger.error(f"!!!!!!!!Exception in topics_loop() {e}")
+            logger.error(
+                f"!!!!!!! Exception in CrawlerScheduler::hints_loop() {e}"
+            )
             logger.error(traceback.format_exc())
 
-    async def worker_loop(self):
-        # fetches urls one by one from the queue and scans them using available plugins
+    async def reports_loop(self):
+        # receive reports from workers
         try:
             while not await self.is_stopped():
-                message = await self.todo_queue.pop(timeout=1)
+                message = await self.reports_queue.pop(timeout=1)
                 if message:
-                    qm = QueueMessage.decode(message.body)
-
-                    if qm.type == QueueMessageType.Task:
-                        task = qm.data
-                        logger.info(f"got {task=}")
-                        url = task["url"]
-                        logger.info(f"processing {url=}")
-
-                        plugin = self.get_url_plugin(url)
-                        logger.info(f"suitable {plugin=}")
-
-                        done = False
-                        for attempt in range(0, self.cfg.ATTEMPTS_PER_URL):
-                            if attempt > 0:
-                                logger.info(f"{attempt=}")
-
-                            try:
-                                async for content_or_task in plugin.process(
-                                    url
-                                ):
-                                    # logger.info( f'{type( content_or_task )=}')
-                                    t = type(content_or_task)
-                                    # logger.info( f'{(t is CrawlerNop)=}')
-                                    if t is CrawlerContent:
-                                        await self._set_task_status(
-                                            task,
-                                            CrawlerHintURLStatus.Processing,
-                                        )
-
-                                        # notifying datapool pipeline about new crawled data
-                                        await self.producer_queue.push(
-                                            QueueMessage(
-                                                QueueMessageType.Task,
-                                                {
-                                                    "parent_url": url,
-                                                    "url": content_or_task.url,
-                                                    "storage_id": content_or_task.storage_id,
-                                                    "tag_id": content_or_task.tag_id,
-                                                    "type": DatapoolContentType(
-                                                        content_or_task.type
-                                                    ).value,
-                                                    "worker_id": self.id,
-                                                },
-                                            )
-                                        )
-
-                                    elif t is CrawlerBackTask:
-                                        await self._add_back_task(
-                                            content_or_task
-                                        )
-                                    elif t is CrawlerNop:
-                                        pass
-                                    else:
-                                        raise Exception(
-                                            f"unknown {content_or_task=}"
-                                        )
-                                    # logger.info( '=================================== process iteration done')
-
-                                logger.info("plugin.process done")
-                                await self._set_task_status(
-                                    task, CrawlerHintURLStatus.Success
-                                )
-
-                                done = True
-                                break
-                            except Exception as e:
-                                logger.error(f"failed get url: {e}")
-                                logger.error(traceback.format_exc())
-                                await asyncio.sleep(self.cfg.ATTEMPTS_DELAY)
-                            if done:
-                                break
-                        if done:
-                            logger.info(
-                                f"sending ack for {message.message_id}"
-                            )
-                            await self.todo_queue.mark_done(message)
+                    try:
+                        qm = QueueMessage.decode(message.body)
+                        if qm.type == QueueMessageType.Task:
+                            # logger.info("new task from worker")
+                            # logger.info(f"{qm=}")
+                            await self._add_task(qm.session_id, qm.data)
+                        elif qm.type == QueueMessageType.Report:
+                            await self._set_task_status(qm.session_id, qm.data)
+                        elif qm.type == QueueMessageType.Stop:
+                            logger.info('scheduler: got stop from worker')
+                            self.stop_task_processed.set()
                         else:
-                            await self.todo_queue.reject(message)
-                            await self._set_task_status(
-                                task, CrawlerHintURLStatus.Failure
-                            )
-                    else:
-                        logger.error(
-                            f"!!!!!!!!!!!!!!! BUG: unexpected {message=} {qm=}"
-                        )
-                        await self.todo_queue.reject(message)
+                            logger.error(f"Unsupported QueueMessage {qm=}")
 
-        except Exception as e:
-            logger.error(f"!!!!!!!!Exception in worker_loop() {e}")
-            logger.error(traceback.format_exc())
+                    except Exception as e:
+                        logger.error(f"Failed decode {message.body=} {message=}")
+                        logger.error(traceback.format_exc())
+                        await asyncio.sleep(1)
 
-    # async def _set_task_status( self, task, status: CrawlerHintURLStatus, contents = None ):
-    #     await self.reports_queue.push( QueueMessage( QueueMessageType.Report, { 'task': task, 'status': status.value, 'contents': contents } ) )
+                    await self.reports_queue.mark_done(message)
 
-    async def _set_task_status(self, task, status: CrawlerHintURLStatus):
-        await self.reports_queue.push(
-            QueueMessage(
-                QueueMessageType.Report, {"task": task, "status": status.value}
+        except Exception as e:
+            logger.error(
+                f"!!!!!!! Exception in CrawlerScheduler::reports_loop() {e}"
             )
-        )
-
-    async def _add_back_task(self, task: CrawlerBackTask):
-        await self.reports_queue.push(
-            QueueMessage(QueueMessageType.Task, task.to_dict())
-        )
-
-    def get_url_plugin(self, url):
-        default_obj = None
-        for cls in self.plugins:
-            args = [self.storage]
-            
-            logger.info( f'get url plugin {cls=}')
-            
-            if cls[0] == 'S3Plugin':
-                #TODO: this is wrong: key/secret should be passed alogn with url somehow..
-                args.append( self.cfg.S3_IMAGESHACK_ACCESS_KEY)
-                args.append( self.cfg.S3_IMAGESHACK_ACCESS_SECRET)
-            elif cls[0] == 'GoogleDrivePlugin':
-                args.append( self.cfg.GOOGLE_DRIVE_API_KEY )
-                
-            obj = cls[1](*args)
-            if cls[0] != "DefaultPlugin":
-                if obj.is_supported(url):
-                    return obj
-            else:
-                default_obj = obj
-        return default_obj
-
-    @staticmethod
-    def get_storage_invalidation_topic(id):
-        return (
-            f"worker.id_{id}.type_{QueueMessageType.StorageInvalidation.value}"
-        )
+            logger.error(traceback.format_exc())
```

### Comparing `datapools-0.1.9/datapools.egg-info/SOURCES.txt` & `datapools-1.0.41/datapools.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,52 +3,62 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 datapools/VERSION
 datapools/__init__.py
 datapools/__main__.py
+datapools/api.py
 datapools/cli.py
-datapools/scheduler.py
 datapools.egg-info/PKG-INFO
 datapools.egg-info/SOURCES.txt
 datapools.egg-info/dependency_links.txt
 datapools.egg-info/entry_points.txt
 datapools.egg-info/requires.txt
 datapools.egg-info/top_level.txt
 datapools/common/__init__.py
 datapools/common/backend_api.py
 datapools/common/logger.py
+datapools/common/session_manager.py
 datapools/common/stoppable.py
 datapools/common/types.py
 datapools/common/queues/__init__.py
 datapools/common/queues/rabbitmq.py
 datapools/common/queues/types.py
 datapools/common/storage/__init__.py
 datapools/common/storage/base_storage.py
 datapools/common/storage/file_storage.py
 datapools/common/tasks_db/__init__.py
-datapools/common/tasks_db/redis.py
+datapools/common/tasks_db/redis.py.bak
 datapools/common/tasks_db/tasks_db.py
 datapools/producer/__init__.py
 datapools/producer/base_producer.py
-datapools/producer/rules.py
+datapools/scheduler/__init__.py
+datapools/scheduler/scheduler.py
 datapools/worker/__init__.py
-datapools/worker/scheduler_api.py.bak
+datapools/worker/utils.py
 datapools/worker/worker.py
 datapools/worker/plugins/__init__.py
 datapools/worker/plugins/base_plugin.py
 datapools/worker/plugins/dataphoenix_info/__init__.py
 datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
 datapools/worker/plugins/default/__init__.py
 datapools/worker/plugins/default/default.py
+datapools/worker/plugins/deutsche_welle/__init__.py
+datapools/worker/plugins/deutsche_welle/deutsche_welle.py
 datapools/worker/plugins/google_drive/__init__.py
 datapools/worker/plugins/google_drive/google_drive.py
 datapools/worker/plugins/imageshack/__init__.py
 datapools/worker/plugins/imageshack/imageshack.py
 datapools/worker/plugins/s3/__init__.py
 datapools/worker/plugins/s3/s3.py
+datapools/worker/plugins/theguardian/__init__.py
+datapools/worker/plugins/theguardian/theguardian.py
+datapools/worker/plugins/washingtonpost/__init__.py
+datapools/worker/plugins/washingtonpost/washingtonpost.py
+datapools/worker/plugins/wikipedia/__init__.py
+datapools/worker/plugins/wikipedia/wikipedia.py
 datapools/worker/plugins/youtube_channel/__init__.py
 datapools/worker/plugins/youtube_channel/youtube_channel.py
 tests/__init__.py
 tests/conftest.py
 tests/test_base.py
```

### Comparing `datapools-0.1.9/setup.py` & `datapools-1.0.41/setup.py`

 * *Files identical despite different names*

