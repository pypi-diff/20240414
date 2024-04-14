# Comparing `tmp/gp2040ce-binary-tools-0.7.0.tar.gz` & `tmp/gp2040ce_binary_tools-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gp2040ce-binary-tools-0.7.0.tar", last modified: Mon Apr  8 15:50:28 2024, max compression
+gzip compressed data, was "gp2040ce_binary_tools-0.8.0.tar", last modified: Sun Apr 14 04:34:29 2024, max compression
```

## Comparing `gp2040ce-binary-tools-0.7.0.tar` & `gp2040ce_binary_tools-0.8.0.tar`

### file list

```diff
@@ -1,63 +1,68 @@
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-08 15:50:28.882169 gp2040ce-binary-tools-0.7.0/
--rw-r--r--   0 bss       (1026) bss       (1000)       12 2023-06-20 20:02:15.000000 gp2040ce-binary-tools-0.7.0/.gitattributes
--rw-r--r--   0 bss       (1026) bss       (1000)     3138 2023-06-20 20:30:00.000000 gp2040ce-binary-tools-0.7.0/.gitignore
--rw-r--r--   0 bss       (1026) bss       (1000)     4294 2024-01-09 15:49:59.000000 gp2040ce-binary-tools-0.7.0/CHANGELOG.md
--rw-r--r--   0 bss       (1026) bss       (1000)     1392 2024-03-07 15:19:40.000000 gp2040ce-binary-tools-0.7.0/CONTRIBUTING.md
--rw-r--r--   0 bss       (1026) bss       (1000)     1366 2024-01-02 21:16:25.000000 gp2040ce-binary-tools-0.7.0/DCO.txt
--rw-r--r--   0 bss       (1026) bss       (1000)    35149 2024-03-07 15:11:36.000000 gp2040ce-binary-tools-0.7.0/LICENSE
--rw-r--r--   0 bss       (1026) bss       (1000)      428 2024-01-02 21:16:25.000000 gp2040ce-binary-tools-0.7.0/MAINTAINERS.md
--rw-r--r--   0 bss       (1026) bss       (1000)    51143 2024-04-08 15:50:28.882169 gp2040ce-binary-tools-0.7.0/PKG-INFO
--rw-r--r--   0 bss       (1026) bss       (1000)     8815 2024-04-08 13:57:12.000000 gp2040ce-binary-tools-0.7.0/README.md
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-08 15:50:28.881168 gp2040ce-binary-tools-0.7.0/gp2040ce_binary_tools.egg-info/
--rw-r--r--   0 bss       (1026) bss       (1000)    51143 2024-04-08 15:50:28.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_binary_tools.egg-info/PKG-INFO
--rw-r--r--   0 bss       (1026) bss       (1000)     1664 2024-04-08 15:50:28.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_binary_tools.egg-info/SOURCES.txt
--rw-r--r--   0 bss       (1026) bss       (1000)        1 2024-04-08 15:50:28.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_binary_tools.egg-info/dependency_links.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      282 2024-04-08 15:50:28.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_binary_tools.egg-info/entry_points.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      289 2024-04-08 15:50:28.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_binary_tools.egg-info/requires.txt
--rw-r--r--   0 bss       (1026) bss       (1000)       18 2024-04-08 15:50:28.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_binary_tools.egg-info/top_level.txt
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-08 15:50:28.868168 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/
--rw-r--r--   0 bss       (1026) bss       (1000)     2861 2024-03-07 15:08:57.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/__init__.py
--rw-r--r--   0 bss       (1026) bss       (1000)      411 2024-04-08 15:50:28.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/_version.py
--rw-r--r--   0 bss       (1026) bss       (1000)    14971 2024-03-25 16:36:51.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/builder.py
--rw-r--r--   0 bss       (1026) bss       (1000)      968 2024-03-26 17:28:23.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/config_tree.css
--rw-r--r--   0 bss       (1026) bss       (1000)    22958 2024-03-26 17:49:27.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/gui.py
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-08 15:50:28.869169 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/
--rw-r--r--   0 bss       (1026) bss       (1000)      407 2024-03-07 15:08:57.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/__init__.py
--rw-r--r--   0 bss       (1026) bss       (1000)    23813 2024-04-08 13:57:12.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/config.proto
--rw-r--r--   0 bss       (1026) bss       (1000)    43224 2024-04-08 13:57:12.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/config_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     9696 2024-04-08 13:57:12.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/enums.proto
--rw-r--r--   0 bss       (1026) bss       (1000)    15272 2024-04-08 13:57:12.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/enums_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     7099 2024-04-08 13:35:15.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/nanopb.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     4619 2024-04-08 13:35:48.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/nanopb_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     9212 2024-03-07 15:08:57.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/rp2040.py
--rw-r--r--   0 bss       (1026) bss       (1000)    14826 2024-03-25 15:03:42.000000 gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/storage.py
--rw-r--r--   0 bss       (1026) bss       (1000)     2687 2024-03-07 15:17:10.000000 gp2040ce-binary-tools-0.7.0/pyproject.toml
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-08 15:50:28.869169 gp2040ce-binary-tools-0.7.0/requirements/
--rw-r--r--   0 bss       (1026) bss       (1000)     4047 2024-04-08 14:07:50.000000 gp2040ce-binary-tools-0.7.0/requirements/requirements-dev.txt
--rw-r--r--   0 bss       (1026) bss       (1000)      906 2024-04-08 14:07:50.000000 gp2040ce-binary-tools-0.7.0/requirements/requirements.txt
--rw-r--r--   0 bss       (1026) bss       (1000)       38 2024-04-08 15:50:28.882169 gp2040ce-binary-tools-0.7.0/setup.cfg
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-08 15:50:28.869169 gp2040ce-binary-tools-0.7.0/tests/
--rw-r--r--   0 bss       (1026) bss       (1000)     2029 2024-03-07 15:08:57.000000 gp2040ce-binary-tools-0.7.0/tests/conftest.py
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-08 15:50:28.871168 gp2040ce-binary-tools-0.7.0/tests/test-files/
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-08 15:50:28.881168 gp2040ce-binary-tools-0.7.0/tests/test-files/pb2-files/
--rw-r--r--   0 bss       (1026) bss       (1000)    43224 2024-04-08 14:01:25.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/pb2-files/config_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)    15272 2024-04-08 14:01:25.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/pb2-files/enums_pb2.py
--rw-r--r--   0 bss       (1026) bss       (1000)     4619 2024-04-08 14:00:25.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/pb2-files/nanopb_pb2.py
-drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-08 15:50:28.881168 gp2040ce-binary-tools-0.7.0/tests/test-files/proto-files/
--rw-r--r--   0 bss       (1026) bss       (1000)    23813 2024-04-08 14:01:25.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/proto-files/config.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     9696 2024-04-08 14:01:25.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/proto-files/enums.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     7099 2024-04-08 14:00:09.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/proto-files/nanopb.proto
--rw-r--r--   0 bss       (1026) bss       (1000)     3770 2024-01-03 19:02:39.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/test-binary-source-of-json-config.bin
--rw-r--r--   0 bss       (1026) bss       (1000)     3321 2023-11-06 22:22:53.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/test-config.bin
--rw-r--r--   0 bss       (1026) bss       (1000)    27879 2024-04-08 14:07:47.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/test-config.json
--rw-r--r--   0 bss       (1026) bss       (1000)   816968 2023-11-06 22:20:55.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/test-firmware.bin
--rw-r--r--   0 bss       (1026) bss       (1000)    16384 2023-11-06 22:20:55.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/test-storage-area.bin
--rw-r--r--   0 bss       (1026) bss       (1000)  2097152 2024-01-06 22:53:09.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/test-whole-board-with-board-config.bin
--rw-r--r--   0 bss       (1026) bss       (1000) 16777216 2023-11-06 22:20:55.000000 gp2040ce-binary-tools-0.7.0/tests/test-files/test-whole-board.bin
--rw-r--r--   0 bss       (1026) bss       (1000)    14262 2024-03-25 16:41:58.000000 gp2040ce-binary-tools-0.7.0/tests/test_builder.py
--rw-r--r--   0 bss       (1026) bss       (1000)     3684 2024-03-07 15:08:57.000000 gp2040ce-binary-tools-0.7.0/tests/test_commands.py
--rw-r--r--   0 bss       (1026) bss       (1000)     9870 2024-03-26 18:47:23.000000 gp2040ce-binary-tools-0.7.0/tests/test_gui.py
--rw-r--r--   0 bss       (1026) bss       (1000)     1508 2024-04-08 13:56:04.000000 gp2040ce-binary-tools-0.7.0/tests/test_package.py
--rw-r--r--   0 bss       (1026) bss       (1000)    11088 2024-03-07 15:08:57.000000 gp2040ce-binary-tools-0.7.0/tests/test_rp2040.py
--rw-r--r--   0 bss       (1026) bss       (1000)     9532 2024-03-25 14:19:49.000000 gp2040ce-binary-tools-0.7.0/tests/test_storage.py
--rw-r--r--   0 bss       (1026) bss       (1000)     1628 2024-01-09 16:29:24.000000 gp2040ce-binary-tools-0.7.0/tox.ini
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-14 04:34:29.555307 gp2040ce_binary_tools-0.8.0/
+-rw-r--r--   0 bss       (1026) bss       (1000)       12 2023-06-20 20:02:15.000000 gp2040ce_binary_tools-0.8.0/.gitattributes
+-rw-r--r--   0 bss       (1026) bss       (1000)     3138 2023-06-20 20:30:00.000000 gp2040ce_binary_tools-0.8.0/.gitignore
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-14 04:34:29.539307 gp2040ce_binary_tools-0.8.0/.reuse/
+-rw-r--r--   0 bss       (1026) bss       (1000)     1123 2024-04-12 12:56:02.000000 gp2040ce_binary_tools-0.8.0/.reuse/dep5
+-rw-r--r--   0 bss       (1026) bss       (1000)     5973 2024-04-14 04:20:23.000000 gp2040ce_binary_tools-0.8.0/CHANGELOG.md
+-rw-r--r--   0 bss       (1026) bss       (1000)     2726 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 bss       (1026) bss       (1000)    34893 2024-04-12 12:38:58.000000 gp2040ce_binary_tools-0.8.0/LICENSE.md
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-14 04:34:29.540307 gp2040ce_binary_tools-0.8.0/LICENSES/
+-rw-r--r--   0 bss       (1026) bss       (1000)    18375 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.0/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)    34674 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.0/LICENSES/GPL-3.0-or-later.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)     1078 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.0/LICENSES/MIT.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      428 2024-01-02 21:16:25.000000 gp2040ce_binary_tools-0.8.0/MAINTAINERS.md
+-rw-r--r--   0 bss       (1026) bss       (1000)    11186 2024-04-14 04:34:29.555307 gp2040ce_binary_tools-0.8.0/PKG-INFO
+-rw-r--r--   0 bss       (1026) bss       (1000)     9343 2024-04-13 01:04:00.000000 gp2040ce_binary_tools-0.8.0/README.md
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-14 04:34:29.554307 gp2040ce_binary_tools-0.8.0/gp2040ce_binary_tools.egg-info/
+-rw-r--r--   0 bss       (1026) bss       (1000)    11186 2024-04-14 04:34:29.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_binary_tools.egg-info/PKG-INFO
+-rw-r--r--   0 bss       (1026) bss       (1000)     1744 2024-04-14 04:34:29.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_binary_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)        1 2024-04-14 04:34:29.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_binary_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      347 2024-04-14 04:34:29.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_binary_tools.egg-info/entry_points.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      295 2024-04-14 04:34:29.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_binary_tools.egg-info/requires.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)       18 2024-04-14 04:34:29.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_binary_tools.egg-info/top_level.txt
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-14 04:34:29.541307 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/
+-rw-r--r--   0 bss       (1026) bss       (1000)     2861 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/__init__.py
+-rw-r--r--   0 bss       (1026) bss       (1000)      411 2024-04-14 04:34:29.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/_version.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    18569 2024-04-13 01:06:37.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/builder.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     1095 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/config_tree.css
+-rw-r--r--   0 bss       (1026) bss       (1000)    22721 2024-04-13 01:01:20.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/gui.py
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-14 04:34:29.541307 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/
+-rw-r--r--   0 bss       (1026) bss       (1000)      407 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/__init__.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    23813 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/config.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)    43224 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/config_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     9696 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/enums.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)    15272 2024-04-08 13:57:12.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/enums_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     7099 2024-04-08 13:35:15.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/nanopb.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     4619 2024-04-08 13:35:48.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/nanopb_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     9212 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/rp2040.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    16797 2024-04-13 01:01:20.000000 gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/storage.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     2871 2024-04-14 04:28:56.000000 gp2040ce_binary_tools-0.8.0/pyproject.toml
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-14 04:34:29.541307 gp2040ce_binary_tools-0.8.0/requirements/
+-rw-r--r--   0 bss       (1026) bss       (1000)     4407 2024-04-12 12:38:22.000000 gp2040ce_binary_tools-0.8.0/requirements/requirements-dev.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)      906 2024-04-08 14:07:50.000000 gp2040ce_binary_tools-0.8.0/requirements/requirements.txt
+-rw-r--r--   0 bss       (1026) bss       (1000)       38 2024-04-14 04:34:29.555307 gp2040ce_binary_tools-0.8.0/setup.cfg
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-14 04:34:29.542307 gp2040ce_binary_tools-0.8.0/tests/
+-rw-r--r--   0 bss       (1026) bss       (1000)     2029 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.0/tests/conftest.py
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-14 04:34:29.544307 gp2040ce_binary_tools-0.8.0/tests/test-files/
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-14 04:34:29.553307 gp2040ce_binary_tools-0.8.0/tests/test-files/pb2-files/
+-rw-r--r--   0 bss       (1026) bss       (1000)    43224 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/pb2-files/config_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    15272 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/pb2-files/enums_pb2.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     4619 2024-04-08 14:00:25.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/pb2-files/nanopb_pb2.py
+drwxr-xr-x   0 bss       (1026) bss       (1000)        0 2024-04-14 04:34:29.553307 gp2040ce_binary_tools-0.8.0/tests/test-files/proto-files/
+-rw-r--r--   0 bss       (1026) bss       (1000)    23813 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/proto-files/config.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     9696 2024-04-08 14:01:25.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/proto-files/enums.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     7099 2024-04-08 14:00:09.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/proto-files/nanopb.proto
+-rw-r--r--   0 bss       (1026) bss       (1000)     3770 2024-01-03 19:02:39.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/test-binary-source-of-json-config.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)     3321 2023-11-06 22:22:53.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/test-config.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)    27879 2024-04-08 14:07:47.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/test-config.json
+-rw-r--r--   0 bss       (1026) bss       (1000)   816968 2023-11-06 22:20:55.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/test-firmware.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)    16384 2023-11-06 22:20:55.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/test-storage-area.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)  2097152 2024-01-06 22:53:09.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/test-whole-board-with-board-config.bin
+-rw-r--r--   0 bss       (1026) bss       (1000) 16777216 2023-11-06 22:20:55.000000 gp2040ce_binary_tools-0.8.0/tests/test-files/test-whole-board.bin
+-rw-r--r--   0 bss       (1026) bss       (1000)    16077 2024-04-13 01:08:25.000000 gp2040ce_binary_tools-0.8.0/tests/test_builder.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     3979 2024-04-13 01:01:20.000000 gp2040ce_binary_tools-0.8.0/tests/test_commands.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    11360 2024-04-13 01:01:20.000000 gp2040ce_binary_tools-0.8.0/tests/test_gui.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     1508 2024-04-08 13:56:04.000000 gp2040ce_binary_tools-0.8.0/tests/test_package.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    11088 2024-03-07 15:08:57.000000 gp2040ce_binary_tools-0.8.0/tests/test_rp2040.py
+-rw-r--r--   0 bss       (1026) bss       (1000)    11220 2024-04-13 01:01:20.000000 gp2040ce_binary_tools-0.8.0/tests/test_storage.py
+-rw-r--r--   0 bss       (1026) bss       (1000)     1707 2024-04-13 01:13:16.000000 gp2040ce_binary_tools-0.8.0/tox.ini
```

### Comparing `gp2040ce-binary-tools-0.7.0/.gitignore` & `gp2040ce_binary_tools-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/CHANGELOG.md` & `gp2040ce_binary_tools-0.8.0/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,54 @@
 # CHANGELOG
 
 Included is a summary of changes to the project. For full details, especially on behind-the-scenes code changes and
 development tools, see the commit history.
 
+## v0.8.0
+
+### Features
+
+* New command, `summarize-gp2040ce`, to get info about a board image or USB device. Details are limited at the moment,
+  but more will come as we need them.
+* `dump-config` can now dump the board config rather than only the user config.
+
+### Improvements
+
+* `visualize-config` can now read UF2 files in addition to raw binary files.
+    * `visualize-config` is the new name of what was formerly `visualize-storage`, to keep things consistent-ish.
+* `concatenate`'s output flag is now `--new-filename`.
+
+### Miscellaneous
+
+* Increased test coverage, especially in the TUI, to stay at 90% despite not being able to cover some USB stuff.
+* The repository is now compliant with the REUSE specification.
+    * This included moving the DCO and making the license a Markdown file, for cleanliness.
+* Some minor docs updates.
+* The SPDX descriptor is used in `pyproject.toml` as that displays better.
+
+## v0.7.0
+
+### Features
+
+* New configurations can be saved as .bin/.uf2 files via "Save As..." in the TUI editor. This allows for making files of
+  different configurations that can be applied on top of one another simply by dragging the tiny UF2 onto the device.
+  This is useful for backup purposes and might also be a handy way to apply different configurations in a networkless
+  environment.
+
+### Improvements
+
+* The GP2040-CE configuration structure has been updated to v0.7.8-RC2.
+* There's a small About screen now in the TUI, but I didn't get around to adding online help yet.
+* TUI tweaks, none of which are earthshattering.
+
+### Miscellaneous
+
+* The license has been changed to GPLv3 (or later).
+* Library/dependency version bumps, a couple times.
+
 ## v0.6.0
 
 ### Added
 
 * Preliminary support for reading and writing "board config"s in the GP2040-CE binary. This will replace the precompiled
   configuration for a particular board by way of `BoardConfig.h` with a second protobuf section of the flash that is
   read from when a user config is not corrupt. `dump-config` can read that section, and `concatenate` can now write it;
```

### Comparing `gp2040ce-binary-tools-0.7.0/CONTRIBUTING.md` & `gp2040ce_binary_tools-0.8.0/CONTRIBUTING.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,55 @@
 # Contributing Guidelines
 
 gp2040ce-binary-tools is made available under the GPLv3 (or later). Contributions are welcome via pull requests.  This
 document outlines the process to get your contribution accepted.
 
 ## Sign Offs/Custody of Contributions
 
-The Developer Certificate of Origin (DCO) is a way for contributors to certify that they wrote or otherwise have the
-right to license their code contributions to the project. The full text of the DCO can be found
-[here](https://developercertificate.org/) or in `DCO.txt`. Contributors must sign-off that they adhere to these
-requirements by adding a `Signed-off-by` line to their commit message, and/or, for frequent contributors, by signing off
-on their entry in `MAINTAINERS.md`.
+The [Developer Certificate of Origin (DCO)](https://developercertificate.org/), reproduced below, is a way for
+contributors to certify that they wrote or otherwise have the right to license their code contributions to the project.
+Contributors must sign-off that they adhere to these requirements by adding a `Signed-off-by` line to their commit
+message, and/or, for frequent contributors, by signing off on their entry in `MAINTAINERS.md`.
+
+```
+Developer Certificate of Origin
+Version 1.1
+
+Copyright (C) 2004, 2006 The Linux Foundation and its contributors.
+
+Everyone is permitted to copy and distribute verbatim copies of this
+license document, but changing it is not allowed.
+
+
+Developer's Certificate of Origin 1.1
+
+By making a contribution to this project, I certify that:
+
+(a) The contribution was created in whole or in part by me and I
+    have the right to submit it under the open source license
+    indicated in the file; or
+
+(b) The contribution is based upon previous work that, to the best
+    of my knowledge, is covered under an appropriate open source
+    license and I have the right under that license to submit that
+    work with modifications, whether created in whole or in part
+    by me, under the same open source license (unless I am
+    permitted to submit under a different license), as indicated
+    in the file; or
+
+(c) The contribution was provided directly to me by some other
+    person who certified (a), (b) or (c) and I have not modified
+    it.
+
+(d) I understand and agree that this project and the contribution
+    are public and that a record of the contribution (including all
+    personal information I submit with it, including my sign-off) is
+    maintained indefinitely and may be redistributed consistent with
+    this project or the open source license(s) involved.
+```
 
 This process is followed by a number of open source projects, most notably the Linux kernel. Here's the gist of it:
 
 ```
 [Your normal Git commit message here.]
 
 Signed-off-by: Random J Developer <random@developer.example.org>
```

### Comparing `gp2040ce-binary-tools-0.7.0/LICENSE` & `gp2040ce_binary_tools-0.8.0/LICENSE.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,674 +1,675 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
+# GNU GENERAL PUBLIC LICENSE
 
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
+Version 3, 29 June 2007
 
-                            Preamble
+Copyright (C) 2007 Free Software Foundation, Inc.
+<https://fsf.org/>
 
-  The GNU General Public License is a free, copyleft license for
+Everyone is permitted to copy and distribute verbatim copies of this
+license document, but changing it is not allowed.
+
+## Preamble
+
+The GNU General Public License is a free, copyleft license for
 software and other kinds of works.
 
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
+The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works. By contrast,
+the GNU General Public License is intended to guarantee your freedom
+to share and change all versions of a program--to make sure it remains
+free software for all its users. We, the Free Software Foundation, use
+the GNU General Public License for most of our software; it applies
+also to any other work released this way by its authors. You can apply
+it to your programs, too.
 
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
+When we speak of free software, we are referring to freedom, not
+price. Our General Public Licenses are designed to make sure that you
 have the freedom to distribute copies of free software (and charge for
 them if you wish), that you receive source code or can get it if you
 want it, that you can change the software or use pieces of it in new
 free programs, and that you know you can do these things.
 
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
+To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights. Therefore, you
+have certain responsibilities if you distribute copies of the
+software, or if you modify it: responsibilities to respect the freedom
+of others.
 
-  For example, if you distribute copies of such a program, whether
+For example, if you distribute copies of such a program, whether
 gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
+freedoms that you received. You must make sure that they, too, receive
+or can get the source code. And you must show them these terms so they
 know their rights.
 
-  Developers that use the GNU GPL protect your rights with two steps:
+Developers that use the GNU GPL protect your rights with two steps:
 (1) assert copyright on the software, and (2) offer you this License
 giving you legal permission to copy, distribute and/or modify it.
 
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
+For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software. For both users' and
 authors' sake, the GPL requires that modified versions be marked as
 changed, so that their problems will not be attributed erroneously to
 authors of previous versions.
 
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
+Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the
+manufacturer can do so. This is fundamentally incompatible with the
+aim of protecting users' freedom to change the software. The
+systematic pattern of such abuse occurs in the area of products for
+individuals to use, which is precisely where it is most unacceptable.
+Therefore, we have designed this version of the GPL to prohibit the
+practice for those products. If such problems arise substantially in
+other domains, we stand ready to extend this provision to those
+domains in future versions of the GPL, as needed to protect the
+freedom of users.
 
-  Finally, every program is threatened constantly by software patents.
+Finally, every program is threatened constantly by software patents.
 States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
+software on general-purpose computers, but in those that do, we wish
+to avoid the special danger that patents applied to a free program
+could make it effectively proprietary. To prevent this, the GPL
+assures that patents cannot be used to render the program non-free.
 
-  The precise terms and conditions for copying, distribution and
+The precise terms and conditions for copying, distribution and
 modification follow.
 
-                       TERMS AND CONDITIONS
+## TERMS AND CONDITIONS
 
-  0. Definitions.
+### 0. Definitions.
 
-  "This License" refers to version 3 of the GNU General Public License.
+"This License" refers to version 3 of the GNU General Public License.
 
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
+"Copyright" also means copyright-like laws that apply to other kinds
+of works, such as semiconductor masks.
 
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
+"The Program" refers to any copyrightable work licensed under this
+License. Each licensee is addressed as "you". "Licensees" and
 "recipients" may be individuals or organizations.
 
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
+To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of
+an exact copy. The resulting work is called a "modified version" of
+the earlier work or a work "based on" the earlier work.
 
-  A "covered work" means either the unmodified Program or a work based
+A "covered work" means either the unmodified Program or a work based
 on the Program.
 
-  To "propagate" a work means to do anything with it that, without
+To "propagate" a work means to do anything with it that, without
 permission, would make you directly or secondarily liable for
 infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
+computer or modifying a private copy. Propagation includes copying,
 distribution (with or without modification), making available to the
 public, and in some countries other activities as well.
 
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
+To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies. Mere interaction with a user
+through a computer network, with no transfer of a copy, is not
+conveying.
 
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
+An interactive user interface displays "Appropriate Legal Notices" to
+the extent that it includes a convenient and prominently visible
 feature that (1) displays an appropriate copyright notice, and (2)
 tells the user that there is no warranty for the work (except to the
 extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
+work under this License, and how to view a copy of this License. If
 the interface presents a list of user commands or options, such as a
 menu, a prominent item in the list meets this criterion.
 
-  1. Source Code.
+### 1. Source Code.
 
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
+The "source code" for a work means the preferred form of the work for
+making modifications to it. "Object code" means any non-source form of
+a work.
 
-  A "Standard Interface" means an interface that either is an official
+A "Standard Interface" means an interface that either is an official
 standard defined by a recognized standards body, or, in the case of
 interfaces specified for a particular programming language, one that
 is widely used among developers working in that language.
 
-  The "System Libraries" of an executable work include anything, other
+The "System Libraries" of an executable work include anything, other
 than the work as a whole, that (a) is included in the normal form of
 packaging a Major Component, but which is not part of that Major
 Component, and (b) serves only to enable use of the work with that
 Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
+implementation is available to the public in source code form. A
 "Major Component", in this context, means a major essential component
 (kernel, window system, and so on) of the specific operating system
 (if any) on which the executable work runs, or a compiler used to
 produce the work, or an object code interpreter used to run it.
 
-  The "Corresponding Source" for a work in object code form means all
+The "Corresponding Source" for a work in object code form means all
 the source code needed to generate, install, and (for an executable
 work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
+control those activities. However, it does not include the work's
 System Libraries, or general-purpose tools or generally available free
 programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
+which are not part of the work. For example, Corresponding Source
 includes interface definition files associated with source files for
 the work, and the source code for shared libraries and dynamically
 linked subprograms that the work is specifically designed to require,
 such as by intimate data communication or control flow between those
 subprograms and other parts of the work.
 
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
+The Corresponding Source need not include anything that users can
+regenerate automatically from other parts of the Corresponding Source.
 
-  The Corresponding Source for a work in source code form is that
-same work.
+The Corresponding Source for a work in source code form is that same
+work.
 
-  2. Basic Permissions.
+### 2. Basic Permissions.
 
-  All rights granted under this License are granted for the term of
+All rights granted under this License are granted for the term of
 copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
+conditions are met. This License explicitly affirms your unlimited
+permission to run the unmodified Program. The output from running a
 covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
+content, constitutes a covered work. This License acknowledges your
 rights of fair use or other equivalent, as provided by copyright law.
 
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
+You may make, run and propagate covered works that you do not convey,
+without conditions so long as your license otherwise remains in force.
+You may convey covered works to others for the sole purpose of having
+them make modifications exclusively for you, or provide you with
+facilities for running those works, provided that you comply with the
+terms of this License in conveying all material for which you do not
+control copyright. Those thus making or running the covered works for
+you must do so exclusively on your behalf, under your direction and
+control, on terms that prohibit them from making any copies of your
+copyrighted material outside their relationship with you.
+
+Conveying under any other circumstances is permitted solely under the
+conditions stated below. Sublicensing is not allowed; section 10 makes
+it unnecessary.
 
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+### 3. Protecting Users' Legal Rights From Anti-Circumvention Law.
 
-  No covered work shall be deemed part of an effective technological
+No covered work shall be deemed part of an effective technological
 measure under any applicable law fulfilling obligations under article
 11 of the WIPO copyright treaty adopted on 20 December 1996, or
 similar laws prohibiting or restricting circumvention of such
 measures.
 
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
+When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such
+circumvention is effected by exercising rights under this License with
+respect to the covered work, and you disclaim any intention to limit
+operation or modification of the work as a means of enforcing, against
+the work's users, your or third parties' legal rights to forbid
+circumvention of technological measures.
 
-  4. Conveying Verbatim Copies.
+### 4. Conveying Verbatim Copies.
 
-  You may convey verbatim copies of the Program's source code as you
+You may convey verbatim copies of the Program's source code as you
 receive it, in any medium, provided that you conspicuously and
 appropriately publish on each copy an appropriate copyright notice;
 keep intact all notices stating that this License and any
 non-permissive terms added in accord with section 7 apply to the code;
 keep intact all notices of the absence of any warranty; and give all
 recipients a copy of this License along with the Program.
 
-  You may charge any price or no price for each copy that you convey,
+You may charge any price or no price for each copy that you convey,
 and you may offer support or warranty protection for a fee.
 
-  5. Conveying Modified Source Versions.
+### 5. Conveying Modified Source Versions.
 
-  You may convey a work based on the Program, or the modifications to
+You may convey a work based on the Program, or the modifications to
 produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
+terms of section 4, provided that you also meet all of these
+conditions:
 
-    a) The work must carry prominent notices stating that you modified
+-   a) The work must carry prominent notices stating that you modified
     it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
+-   b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under
+    section 7. This requirement modifies the requirement in section 4
+    to "keep intact all notices".
+-   c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy. This
     License will therefore apply, along with any applicable section 7
     additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
+    regardless of how they are packaged. This License gives no
     permission to license the work in any other way, but it does not
     invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
+-   d) If the work has interactive user interfaces, each must display
     Appropriate Legal Notices; however, if the Program has interactive
     interfaces that do not display Appropriate Legal Notices, your
     work need not make them do so.
 
-  A compilation of a covered work with other separate and independent
+A compilation of a covered work with other separate and independent
 works, which are not by their nature extensions of the covered work,
 and which are not combined with it such as to form a larger program,
 in or on a volume of a storage or distribution medium, is called an
 "aggregate" if the compilation and its resulting copyright are not
 used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
+beyond what the individual works permit. Inclusion of a covered work
 in an aggregate does not cause this License to apply to the other
 parts of the aggregate.
 
-  6. Conveying Non-Source Forms.
+### 6. Conveying Non-Source Forms.
 
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
+You may convey a covered work in object code form under the terms of
+sections 4 and 5, provided that you also convey the machine-readable
+Corresponding Source under the terms of this License, in one of these
+ways:
 
-    a) Convey the object code in, or embodied in, a physical product
+-   a) Convey the object code in, or embodied in, a physical product
     (including a physical distribution medium), accompanied by the
     Corresponding Source fixed on a durable physical medium
     customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
+-   b) Convey the object code in, or embodied in, a physical product
     (including a physical distribution medium), accompanied by a
     written offer, valid for at least three years and valid for as
     long as you offer spare parts or customer support for that product
     model, to give anyone who possesses the object code either (1) a
     copy of the Corresponding Source for all the software in the
     product that is covered by this License, on a durable physical
     medium customarily used for software interchange, for a price no
     more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
+    conveying of source, or (2) access to copy the Corresponding
+    Source from a network server at no charge.
+-   c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source. This
     alternative is allowed only occasionally and noncommercially, and
     only if you received the object code with such an offer, in accord
     with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
+-   d) Convey the object code by offering access from a designated
     place (gratis or for a charge), and offer equivalent access to the
     Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
+    further charge. You need not require recipients to copy the
+    Corresponding Source along with the object code. If the place to
     copy the object code is a network server, the Corresponding Source
     may be on a different server (operated by you or a third party)
     that supports equivalent copying facilities, provided you maintain
     clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source. Regardless of what server hosts the
     Corresponding Source, you remain obligated to ensure that it is
     available for as long as needed to satisfy these requirements.
+-   e) Convey the object code using peer-to-peer transmission,
+    provided you inform other peers where the object code and
+    Corresponding Source of the work are being offered to the general
+    public at no charge under subsection 6d.
 
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
+A separable portion of the object code, whose source code is excluded
 from the Corresponding Source as a System Library, need not be
 included in conveying the object code work.
 
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
+A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal,
+family, or household purposes, or (2) anything designed or sold for
+incorporation into a dwelling. In determining whether a product is a
+consumer product, doubtful cases shall be resolved in favor of
+coverage. For a particular product received by a particular user,
+"normally used" refers to a typical or common use of that class of
+product, regardless of the status of the particular user or of the way
+in which the particular user actually uses, or expects or is expected
+to use, the product. A product is a consumer product regardless of
+whether the product has substantial commercial, industrial or
+non-consumer uses, unless such uses represent the only significant
+mode of use of the product.
+
+"Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to
+install and execute modified versions of a covered work in that User
+Product from a modified version of its Corresponding Source. The
+information must suffice to ensure that the continued functioning of
+the modified object code is in no case prevented or interfered with
+solely because modification has been made.
 
-  If you convey an object code work under this section in, or with, or
+If you convey an object code work under this section in, or with, or
 specifically for use in, a User Product, and the conveying occurs as
 part of a transaction in which the right of possession and use of the
 User Product is transferred to the recipient in perpetuity or for a
 fixed term (regardless of how the transaction is characterized), the
 Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
+by the Installation Information. But this requirement does not apply
 if neither you nor any third party retains the ability to install
 modified object code on the User Product (for example, the work has
 been installed in ROM).
 
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
+The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or
+updates for a work that has been modified or installed by the
+recipient, or for the User Product in which it has been modified or
+installed. Access to a network may be denied when the modification
+itself materially and adversely affects the operation of the network
+or violates the rules and protocols for communication across the
+network.
 
-  Corresponding Source conveyed, and Installation Information provided,
+Corresponding Source conveyed, and Installation Information provided,
 in accord with this section must be in a format that is publicly
 documented (and with an implementation available to the public in
 source code form), and must require no special password or key for
 unpacking, reading or copying.
 
-  7. Additional Terms.
+### 7. Additional Terms.
 
-  "Additional permissions" are terms that supplement the terms of this
+"Additional permissions" are terms that supplement the terms of this
 License by making exceptions from one or more of its conditions.
 Additional permissions that are applicable to the entire Program shall
 be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
+that they are valid under applicable law. If additional permissions
 apply only to part of the Program, that part may be used separately
 under those permissions, but the entire Program remains governed by
 this License without regard to the additional permissions.
 
-  When you convey a copy of a covered work, you may at your option
+When you convey a copy of a covered work, you may at your option
 remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
+it. (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.) You may place
 additional permissions on material, added by you to a covered work,
 for which you have or can give appropriate copyright permission.
 
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
+Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders
+of that material) supplement the terms of this License with terms:
 
-    a) Disclaiming warranty or limiting liability differently from the
+-   a) Disclaiming warranty or limiting liability differently from the
     terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
+-   b) Requiring preservation of specified reasonable legal notices or
     author attributions in that material or in the Appropriate Legal
     Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
+-   c) Prohibiting misrepresentation of the origin of that material,
+    or requiring that modified versions of such material be marked in
     reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
+-   d) Limiting the use for publicity purposes of names of licensors
+    or authors of the material; or
+-   e) Declining to grant rights under trademark law for use of some
     trade names, trademarks, or service marks; or
+-   f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions
+    of it) with contractual assumptions of liability to the recipient,
+    for any liability that these contractual assumptions directly
+    impose on those licensors and authors.
 
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
+All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10. If the Program as you
 received it, or any part of it, contains a notice stating that it is
 governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
+restriction, you may remove that term. If a license document contains
 a further restriction but permits relicensing or conveying under this
 License, you may add to a covered work material governed by the terms
 of that license document, provided that the further restriction does
 not survive such relicensing or conveying.
 
-  If you add terms to a covered work in accord with this section, you
+If you add terms to a covered work in accord with this section, you
 must place, in the relevant source files, a statement of the
 additional terms that apply to those files, or a notice indicating
 where to find the applicable terms.
 
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
+Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions; the
+above requirements apply either way.
 
-  8. Termination.
+### 8. Termination.
 
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
+You may not propagate or modify a covered work except as expressly
+provided under this License. Any attempt otherwise to propagate or
 modify it is void, and will automatically terminate your rights under
 this License (including any patent licenses granted under the third
 paragraph of section 11).
 
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
+However, if you cease all violation of this License, then your license
+from a particular copyright holder is reinstated (a) provisionally,
+unless and until the copyright holder explicitly and finally
+terminates your license, and (b) permanently, if the copyright holder
+fails to notify you of the violation by some reasonable means prior to
+60 days after the cessation.
 
-  Moreover, your license from a particular copyright holder is
+Moreover, your license from a particular copyright holder is
 reinstated permanently if the copyright holder notifies you of the
 violation by some reasonable means, this is the first time you have
 received notice of violation of this License (for any work) from that
 copyright holder, and you cure the violation prior to 30 days after
 your receipt of the notice.
 
-  Termination of your rights under this section does not terminate the
+Termination of your rights under this section does not terminate the
 licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
+this License. If your rights have been terminated and not permanently
 reinstated, you do not qualify to receive new licenses for the same
 material under section 10.
 
-  9. Acceptance Not Required for Having Copies.
+### 9. Acceptance Not Required for Having Copies.
 
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
+You are not required to accept this License in order to receive or run
+a copy of the Program. Ancillary propagation of a covered work
 occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
+to receive a copy likewise does not require acceptance. However,
 nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
+modify any covered work. These actions infringe copyright if you do
+not accept this License. Therefore, by modifying or propagating a
 covered work, you indicate your acceptance of this License to do so.
 
-  10. Automatic Licensing of Downstream Recipients.
+### 10. Automatic Licensing of Downstream Recipients.
 
-  Each time you convey a covered work, the recipient automatically
+Each time you convey a covered work, the recipient automatically
 receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
+propagate that work, subject to this License. You are not responsible
 for enforcing compliance by third parties with this License.
 
-  An "entity transaction" is a transaction transferring control of an
+An "entity transaction" is a transaction transferring control of an
 organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
+organization, or merging organizations. If propagation of a covered
 work results from an entity transaction, each party to that
 transaction who receives a copy of the work also receives whatever
 licenses to the work the party's predecessor in interest had or could
 give under the previous paragraph, plus a right to possession of the
 Corresponding Source of the work from the predecessor in interest, if
 the predecessor has it or can get it with reasonable efforts.
 
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
+You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License. For example, you may
 not impose a license fee, royalty, or other charge for exercise of
 rights granted under this License, and you may not initiate litigation
 (including a cross-claim or counterclaim in a lawsuit) alleging that
 any patent claim is infringed by making, using, selling, offering for
 sale, or importing the Program or any portion of it.
 
-  11. Patents.
+### 11. Patents.
 
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
+A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based. The
 work thus licensed is called the contributor's "contributor version".
 
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
+A contributor's "essential patent claims" are all patent claims owned
+or controlled by the contributor, whether already acquired or
 hereafter acquired, that would be infringed by some manner, permitted
 by this License, of making, using, or selling its contributor version,
 but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
+consequence of further modification of the contributor version. For
 purposes of this definition, "control" includes the right to grant
 patent sublicenses in a manner consistent with the requirements of
 this License.
 
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
+Each contributor grants you a non-exclusive, worldwide, royalty-free
 patent license under the contributor's essential patent claims, to
 make, use, sell, offer for sale, import and otherwise run, modify and
 propagate the contents of its contributor version.
 
-  In the following three paragraphs, a "patent license" is any express
+In the following three paragraphs, a "patent license" is any express
 agreement or commitment, however denominated, not to enforce a patent
 (such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
+sue for patent infringement). To "grant" such a patent license to a
 party means to make such an agreement or commitment not to enforce a
 patent against the party.
 
-  If you convey a covered work, knowingly relying on a patent license,
+If you convey a covered work, knowingly relying on a patent license,
 and the Corresponding Source of the work is not available for anyone
 to copy, free of charge and under the terms of this License, through a
 publicly available network server or other readily accessible means,
 then you must either (1) cause the Corresponding Source to be so
 available, or (2) arrange to deprive yourself of the benefit of the
 patent license for this particular work, or (3) arrange, in a manner
 consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
+license to downstream recipients. "Knowingly relying" means you have
 actual knowledge that, but for the patent license, your conveying the
 covered work in a country, or your recipient's use of the covered work
 in a country, would infringe one or more identifiable patents in that
 country that you have reason to believe are valid.
 
-  If, pursuant to or in connection with a single transaction or
+If, pursuant to or in connection with a single transaction or
 arrangement, you convey, or propagate by procuring conveyance of, a
 covered work, and grant a patent license to some of the parties
 receiving the covered work authorizing them to use, propagate, modify
 or convey a specific copy of the covered work, then the patent license
 you grant is automatically extended to all recipients of the covered
 work and works based on it.
 
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
+A patent license is "discriminatory" if it does not include within the
+scope of its coverage, prohibits the exercise of, or is conditioned on
+the non-exercise of one or more of the rights that are specifically
+granted under this License. You may not convey a covered work if you
+are a party to an arrangement with a third party that is in the
+business of distributing software, under which you make payment to the
+third party based on the extent of your activity of conveying the
+work, and under which the third party grants, to any of the parties
+who would receive the covered work from you, a discriminatory patent
+license (a) in connection with copies of the covered work conveyed by
+you (or copies made from those copies), or (b) primarily for and in
+connection with specific products or compilations that contain the
+covered work, unless you entered into that arrangement, or that patent
+license was granted, prior to 28 March 2007.
 
-  Nothing in this License shall be construed as excluding or limiting
+Nothing in this License shall be construed as excluding or limiting
 any implied license or other defenses to infringement that may
 otherwise be available to you under applicable patent law.
 
-  12. No Surrender of Others' Freedom.
+### 12. No Surrender of Others' Freedom.
 
-  If conditions are imposed on you (whether by court order, agreement or
+If conditions are imposed on you (whether by court order, agreement or
 otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
+excuse you from the conditions of this License. If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under
+this License and any other pertinent obligations, then as a
+consequence you may not convey it at all. For example, if you agree to
+terms that obligate you to collect a royalty for further conveying
+from those to whom you convey the Program, the only way you could
+satisfy both those terms and this License would be to refrain entirely
+from conveying the Program.
 
-  13. Use with the GNU Affero General Public License.
+### 13. Use with the GNU Affero General Public License.
 
-  Notwithstanding any other provision of this License, you have
+Notwithstanding any other provision of this License, you have
 permission to link or combine any covered work with a work licensed
 under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
+combined work, and to convey the resulting work. The terms of this
 License will continue to apply to the part which is the covered work,
 but the special requirements of the GNU Affero General Public License,
 section 13, concerning interaction through a network will apply to the
 combination as such.
 
-  14. Revised Versions of this License.
+### 14. Revised Versions of this License.
 
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
+The Free Software Foundation may publish revised and/or new versions
+of the GNU General Public License from time to time. Such new versions
+will be similar in spirit to the present version, but may differ in
+detail to address new problems or concerns.
+
+Each version is given a distinguishing version number. If the Program
+specifies that a certain numbered version of the GNU General Public
+License "or any later version" applies to it, you have the option of
+following the terms and conditions either of that numbered version or
+of any later version published by the Free Software Foundation. If the
+Program does not specify a version number of the GNU General Public
+License, you may choose any version ever published by the Free
+Software Foundation.
+
+If the Program specifies that a proxy can decide which future versions
+of the GNU General Public License can be used, that proxy's public
+statement of acceptance of a version permanently authorizes you to
+choose that version for the Program.
 
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
+Later license versions may give you additional or different
+permissions. However, no additional obligations are imposed on any
 author or copyright holder as a result of your choosing to follow a
 later version.
 
-  15. Disclaimer of Warranty.
+### 15. Disclaimer of Warranty.
 
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
+THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT
+WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT
+LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
+A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND
+PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE
+DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR
+CORRECTION.
+
+### 16. Limitation of Liability.
+
+IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR
+CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES,
+INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES
+ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT
+NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR
+LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM
+TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER
+PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
 
-  17. Interpretation of Sections 15 and 16.
+### 17. Interpretation of Sections 15 and 16.
 
-  If the disclaimer of warranty and limitation of liability provided
+If the disclaimer of warranty and limitation of liability provided
 above cannot be given local legal effect according to their terms,
 reviewing courts shall apply local law that most closely approximates
 an absolute waiver of all civil liability in connection with the
 Program, unless a warranty or assumption of liability accompanies a
 copy of the Program in return for a fee.
 
-                     END OF TERMS AND CONDITIONS
+END OF TERMS AND CONDITIONS
 
-            How to Apply These Terms to Your New Programs
+## How to Apply These Terms to Your New Programs
 
-  If you develop a new program, and you want it to be of the greatest
+If you develop a new program, and you want it to be of the greatest
 possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
+free software which everyone can redistribute and change under these
+terms.
 
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
+To do so, attach the following notices to the program. It is safest to
+attach them to the start of each source file to most effectively state
+the exclusion of warranty; and each file should have at least the
+"copyright" line and a pointer to where the full notice is found.
+
+        <one line to give the program's name and a brief idea of what it does.>
+        Copyright (C) <year>  <name of author>
+
+        This program is free software: you can redistribute it and/or modify
+        it under the terms of the GNU General Public License as published by
+        the Free Software Foundation, either version 3 of the License, or
+        (at your option) any later version.
+
+        This program is distributed in the hope that it will be useful,
+        but WITHOUT ANY WARRANTY; without even the implied warranty of
+        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+        GNU General Public License for more details.
 
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+        You should have received a copy of the GNU General Public License
+        along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-Also add information on how to contact you by electronic and paper mail.
+Also add information on how to contact you by electronic and paper
+mail.
 
-  If the program does terminal interaction, make it output a short
+If the program does terminal interaction, make it output a short
 notice like this when it starts in an interactive mode:
 
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
+        <program>  Copyright (C) <year>  <name of author>
+        This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+        This is free software, and you are welcome to redistribute it
+        under certain conditions; type `show c' for details.
+
+The hypothetical commands \`show w' and \`show c' should show the
+appropriate parts of the General Public License. Of course, your
+program's commands might be different; for a GUI interface, you would
+use an "about box".
+
+You should also get your employer (if you work as a programmer) or
+school, if any, to sign a "copyright disclaimer" for the program, if
+necessary. For more information on this, and how to apply and follow
+the GNU GPL, see <https://www.gnu.org/licenses/>.
+
+The GNU General Public License does not permit incorporating your
+program into proprietary programs. If your program is a subroutine
+library, you may consider it more useful to permit linking proprietary
+applications with the library. If this is what you want to do, use the
+GNU Lesser General Public License instead of this License. But first,
+please read <https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `gp2040ce-binary-tools-0.7.0/PKG-INFO` & `gp2040ce_binary_tools-0.8.0/LICENSES/GPL-3.0-or-later.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,959 +1,232 @@
-Metadata-Version: 2.1
-Name: gp2040ce-binary-tools
-Version: 0.7.0
-Summary: Tools for working with GP2040-CE firmware and storage binaries.
-Author-email: "Brian S. Stephan" <bss@incorporeal.org>
-License:                     GNU GENERAL PUBLIC LICENSE
-                               Version 3, 29 June 2007
-        
-         Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
-         Everyone is permitted to copy and distribute verbatim copies
-         of this license document, but changing it is not allowed.
-        
-                                    Preamble
-        
-          The GNU General Public License is a free, copyleft license for
-        software and other kinds of works.
-        
-          The licenses for most software and other practical works are designed
-        to take away your freedom to share and change the works.  By contrast,
-        the GNU General Public License is intended to guarantee your freedom to
-        share and change all versions of a program--to make sure it remains free
-        software for all its users.  We, the Free Software Foundation, use the
-        GNU General Public License for most of our software; it applies also to
-        any other work released this way by its authors.  You can apply it to
-        your programs, too.
-        
-          When we speak of free software, we are referring to freedom, not
-        price.  Our General Public Licenses are designed to make sure that you
-        have the freedom to distribute copies of free software (and charge for
-        them if you wish), that you receive source code or can get it if you
-        want it, that you can change the software or use pieces of it in new
-        free programs, and that you know you can do these things.
-        
-          To protect your rights, we need to prevent others from denying you
-        these rights or asking you to surrender the rights.  Therefore, you have
-        certain responsibilities if you distribute copies of the software, or if
-        you modify it: responsibilities to respect the freedom of others.
-        
-          For example, if you distribute copies of such a program, whether
-        gratis or for a fee, you must pass on to the recipients the same
-        freedoms that you received.  You must make sure that they, too, receive
-        or can get the source code.  And you must show them these terms so they
-        know their rights.
-        
-          Developers that use the GNU GPL protect your rights with two steps:
-        (1) assert copyright on the software, and (2) offer you this License
-        giving you legal permission to copy, distribute and/or modify it.
-        
-          For the developers' and authors' protection, the GPL clearly explains
-        that there is no warranty for this free software.  For both users' and
-        authors' sake, the GPL requires that modified versions be marked as
-        changed, so that their problems will not be attributed erroneously to
-        authors of previous versions.
-        
-          Some devices are designed to deny users access to install or run
-        modified versions of the software inside them, although the manufacturer
-        can do so.  This is fundamentally incompatible with the aim of
-        protecting users' freedom to change the software.  The systematic
-        pattern of such abuse occurs in the area of products for individuals to
-        use, which is precisely where it is most unacceptable.  Therefore, we
-        have designed this version of the GPL to prohibit the practice for those
-        products.  If such problems arise substantially in other domains, we
-        stand ready to extend this provision to those domains in future versions
-        of the GPL, as needed to protect the freedom of users.
-        
-          Finally, every program is threatened constantly by software patents.
-        States should not allow patents to restrict development and use of
-        software on general-purpose computers, but in those that do, we wish to
-        avoid the special danger that patents applied to a free program could
-        make it effectively proprietary.  To prevent this, the GPL assures that
-        patents cannot be used to render the program non-free.
-        
-          The precise terms and conditions for copying, distribution and
-        modification follow.
-        
-                               TERMS AND CONDITIONS
-        
-          0. Definitions.
-        
-          "This License" refers to version 3 of the GNU General Public License.
-        
-          "Copyright" also means copyright-like laws that apply to other kinds of
-        works, such as semiconductor masks.
-        
-          "The Program" refers to any copyrightable work licensed under this
-        License.  Each licensee is addressed as "you".  "Licensees" and
-        "recipients" may be individuals or organizations.
-        
-          To "modify" a work means to copy from or adapt all or part of the work
-        in a fashion requiring copyright permission, other than the making of an
-        exact copy.  The resulting work is called a "modified version" of the
-        earlier work or a work "based on" the earlier work.
-        
-          A "covered work" means either the unmodified Program or a work based
-        on the Program.
-        
-          To "propagate" a work means to do anything with it that, without
-        permission, would make you directly or secondarily liable for
-        infringement under applicable copyright law, except executing it on a
-        computer or modifying a private copy.  Propagation includes copying,
-        distribution (with or without modification), making available to the
-        public, and in some countries other activities as well.
-        
-          To "convey" a work means any kind of propagation that enables other
-        parties to make or receive copies.  Mere interaction with a user through
-        a computer network, with no transfer of a copy, is not conveying.
-        
-          An interactive user interface displays "Appropriate Legal Notices"
-        to the extent that it includes a convenient and prominently visible
-        feature that (1) displays an appropriate copyright notice, and (2)
-        tells the user that there is no warranty for the work (except to the
-        extent that warranties are provided), that licensees may convey the
-        work under this License, and how to view a copy of this License.  If
-        the interface presents a list of user commands or options, such as a
-        menu, a prominent item in the list meets this criterion.
-        
-          1. Source Code.
-        
-          The "source code" for a work means the preferred form of the work
-        for making modifications to it.  "Object code" means any non-source
-        form of a work.
-        
-          A "Standard Interface" means an interface that either is an official
-        standard defined by a recognized standards body, or, in the case of
-        interfaces specified for a particular programming language, one that
-        is widely used among developers working in that language.
-        
-          The "System Libraries" of an executable work include anything, other
-        than the work as a whole, that (a) is included in the normal form of
-        packaging a Major Component, but which is not part of that Major
-        Component, and (b) serves only to enable use of the work with that
-        Major Component, or to implement a Standard Interface for which an
-        implementation is available to the public in source code form.  A
-        "Major Component", in this context, means a major essential component
-        (kernel, window system, and so on) of the specific operating system
-        (if any) on which the executable work runs, or a compiler used to
-        produce the work, or an object code interpreter used to run it.
-        
-          The "Corresponding Source" for a work in object code form means all
-        the source code needed to generate, install, and (for an executable
-        work) run the object code and to modify the work, including scripts to
-        control those activities.  However, it does not include the work's
-        System Libraries, or general-purpose tools or generally available free
-        programs which are used unmodified in performing those activities but
-        which are not part of the work.  For example, Corresponding Source
-        includes interface definition files associated with source files for
-        the work, and the source code for shared libraries and dynamically
-        linked subprograms that the work is specifically designed to require,
-        such as by intimate data communication or control flow between those
-        subprograms and other parts of the work.
-        
-          The Corresponding Source need not include anything that users
-        can regenerate automatically from other parts of the Corresponding
-        Source.
-        
-          The Corresponding Source for a work in source code form is that
-        same work.
-        
-          2. Basic Permissions.
-        
-          All rights granted under this License are granted for the term of
-        copyright on the Program, and are irrevocable provided the stated
-        conditions are met.  This License explicitly affirms your unlimited
-        permission to run the unmodified Program.  The output from running a
-        covered work is covered by this License only if the output, given its
-        content, constitutes a covered work.  This License acknowledges your
-        rights of fair use or other equivalent, as provided by copyright law.
-        
-          You may make, run and propagate covered works that you do not
-        convey, without conditions so long as your license otherwise remains
-        in force.  You may convey covered works to others for the sole purpose
-        of having them make modifications exclusively for you, or provide you
-        with facilities for running those works, provided that you comply with
-        the terms of this License in conveying all material for which you do
-        not control copyright.  Those thus making or running the covered works
-        for you must do so exclusively on your behalf, under your direction
-        and control, on terms that prohibit them from making any copies of
-        your copyrighted material outside their relationship with you.
-        
-          Conveying under any other circumstances is permitted solely under
-        the conditions stated below.  Sublicensing is not allowed; section 10
-        makes it unnecessary.
-        
-          3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-        
-          No covered work shall be deemed part of an effective technological
-        measure under any applicable law fulfilling obligations under article
-        11 of the WIPO copyright treaty adopted on 20 December 1996, or
-        similar laws prohibiting or restricting circumvention of such
-        measures.
-        
-          When you convey a covered work, you waive any legal power to forbid
-        circumvention of technological measures to the extent such circumvention
-        is effected by exercising rights under this License with respect to
-        the covered work, and you disclaim any intention to limit operation or
-        modification of the work as a means of enforcing, against the work's
-        users, your or third parties' legal rights to forbid circumvention of
-        technological measures.
-        
-          4. Conveying Verbatim Copies.
-        
-          You may convey verbatim copies of the Program's source code as you
-        receive it, in any medium, provided that you conspicuously and
-        appropriately publish on each copy an appropriate copyright notice;
-        keep intact all notices stating that this License and any
-        non-permissive terms added in accord with section 7 apply to the code;
-        keep intact all notices of the absence of any warranty; and give all
-        recipients a copy of this License along with the Program.
-        
-          You may charge any price or no price for each copy that you convey,
-        and you may offer support or warranty protection for a fee.
-        
-          5. Conveying Modified Source Versions.
-        
-          You may convey a work based on the Program, or the modifications to
-        produce it from the Program, in the form of source code under the
-        terms of section 4, provided that you also meet all of these conditions:
-        
-            a) The work must carry prominent notices stating that you modified
-            it, and giving a relevant date.
-        
-            b) The work must carry prominent notices stating that it is
-            released under this License and any conditions added under section
-            7.  This requirement modifies the requirement in section 4 to
-            "keep intact all notices".
-        
-            c) You must license the entire work, as a whole, under this
-            License to anyone who comes into possession of a copy.  This
-            License will therefore apply, along with any applicable section 7
-            additional terms, to the whole of the work, and all its parts,
-            regardless of how they are packaged.  This License gives no
-            permission to license the work in any other way, but it does not
-            invalidate such permission if you have separately received it.
-        
-            d) If the work has interactive user interfaces, each must display
-            Appropriate Legal Notices; however, if the Program has interactive
-            interfaces that do not display Appropriate Legal Notices, your
-            work need not make them do so.
-        
-          A compilation of a covered work with other separate and independent
-        works, which are not by their nature extensions of the covered work,
-        and which are not combined with it such as to form a larger program,
-        in or on a volume of a storage or distribution medium, is called an
-        "aggregate" if the compilation and its resulting copyright are not
-        used to limit the access or legal rights of the compilation's users
-        beyond what the individual works permit.  Inclusion of a covered work
-        in an aggregate does not cause this License to apply to the other
-        parts of the aggregate.
-        
-          6. Conveying Non-Source Forms.
-        
-          You may convey a covered work in object code form under the terms
-        of sections 4 and 5, provided that you also convey the
-        machine-readable Corresponding Source under the terms of this License,
-        in one of these ways:
-        
-            a) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by the
-            Corresponding Source fixed on a durable physical medium
-            customarily used for software interchange.
-        
-            b) Convey the object code in, or embodied in, a physical product
-            (including a physical distribution medium), accompanied by a
-            written offer, valid for at least three years and valid for as
-            long as you offer spare parts or customer support for that product
-            model, to give anyone who possesses the object code either (1) a
-            copy of the Corresponding Source for all the software in the
-            product that is covered by this License, on a durable physical
-            medium customarily used for software interchange, for a price no
-            more than your reasonable cost of physically performing this
-            conveying of source, or (2) access to copy the
-            Corresponding Source from a network server at no charge.
-        
-            c) Convey individual copies of the object code with a copy of the
-            written offer to provide the Corresponding Source.  This
-            alternative is allowed only occasionally and noncommercially, and
-            only if you received the object code with such an offer, in accord
-            with subsection 6b.
-        
-            d) Convey the object code by offering access from a designated
-            place (gratis or for a charge), and offer equivalent access to the
-            Corresponding Source in the same way through the same place at no
-            further charge.  You need not require recipients to copy the
-            Corresponding Source along with the object code.  If the place to
-            copy the object code is a network server, the Corresponding Source
-            may be on a different server (operated by you or a third party)
-            that supports equivalent copying facilities, provided you maintain
-            clear directions next to the object code saying where to find the
-            Corresponding Source.  Regardless of what server hosts the
-            Corresponding Source, you remain obligated to ensure that it is
-            available for as long as needed to satisfy these requirements.
-        
-            e) Convey the object code using peer-to-peer transmission, provided
-            you inform other peers where the object code and Corresponding
-            Source of the work are being offered to the general public at no
-            charge under subsection 6d.
-        
-          A separable portion of the object code, whose source code is excluded
-        from the Corresponding Source as a System Library, need not be
-        included in conveying the object code work.
-        
-          A "User Product" is either (1) a "consumer product", which means any
-        tangible personal property which is normally used for personal, family,
-        or household purposes, or (2) anything designed or sold for incorporation
-        into a dwelling.  In determining whether a product is a consumer product,
-        doubtful cases shall be resolved in favor of coverage.  For a particular
-        product received by a particular user, "normally used" refers to a
-        typical or common use of that class of product, regardless of the status
-        of the particular user or of the way in which the particular user
-        actually uses, or expects or is expected to use, the product.  A product
-        is a consumer product regardless of whether the product has substantial
-        commercial, industrial or non-consumer uses, unless such uses represent
-        the only significant mode of use of the product.
-        
-          "Installation Information" for a User Product means any methods,
-        procedures, authorization keys, or other information required to install
-        and execute modified versions of a covered work in that User Product from
-        a modified version of its Corresponding Source.  The information must
-        suffice to ensure that the continued functioning of the modified object
-        code is in no case prevented or interfered with solely because
-        modification has been made.
-        
-          If you convey an object code work under this section in, or with, or
-        specifically for use in, a User Product, and the conveying occurs as
-        part of a transaction in which the right of possession and use of the
-        User Product is transferred to the recipient in perpetuity or for a
-        fixed term (regardless of how the transaction is characterized), the
-        Corresponding Source conveyed under this section must be accompanied
-        by the Installation Information.  But this requirement does not apply
-        if neither you nor any third party retains the ability to install
-        modified object code on the User Product (for example, the work has
-        been installed in ROM).
-        
-          The requirement to provide Installation Information does not include a
-        requirement to continue to provide support service, warranty, or updates
-        for a work that has been modified or installed by the recipient, or for
-        the User Product in which it has been modified or installed.  Access to a
-        network may be denied when the modification itself materially and
-        adversely affects the operation of the network or violates the rules and
-        protocols for communication across the network.
-        
-          Corresponding Source conveyed, and Installation Information provided,
-        in accord with this section must be in a format that is publicly
-        documented (and with an implementation available to the public in
-        source code form), and must require no special password or key for
-        unpacking, reading or copying.
-        
-          7. Additional Terms.
-        
-          "Additional permissions" are terms that supplement the terms of this
-        License by making exceptions from one or more of its conditions.
-        Additional permissions that are applicable to the entire Program shall
-        be treated as though they were included in this License, to the extent
-        that they are valid under applicable law.  If additional permissions
-        apply only to part of the Program, that part may be used separately
-        under those permissions, but the entire Program remains governed by
-        this License without regard to the additional permissions.
-        
-          When you convey a copy of a covered work, you may at your option
-        remove any additional permissions from that copy, or from any part of
-        it.  (Additional permissions may be written to require their own
-        removal in certain cases when you modify the work.)  You may place
-        additional permissions on material, added by you to a covered work,
-        for which you have or can give appropriate copyright permission.
-        
-          Notwithstanding any other provision of this License, for material you
-        add to a covered work, you may (if authorized by the copyright holders of
-        that material) supplement the terms of this License with terms:
-        
-            a) Disclaiming warranty or limiting liability differently from the
-            terms of sections 15 and 16 of this License; or
-        
-            b) Requiring preservation of specified reasonable legal notices or
-            author attributions in that material or in the Appropriate Legal
-            Notices displayed by works containing it; or
-        
-            c) Prohibiting misrepresentation of the origin of that material, or
-            requiring that modified versions of such material be marked in
-            reasonable ways as different from the original version; or
-        
-            d) Limiting the use for publicity purposes of names of licensors or
-            authors of the material; or
-        
-            e) Declining to grant rights under trademark law for use of some
-            trade names, trademarks, or service marks; or
-        
-            f) Requiring indemnification of licensors and authors of that
-            material by anyone who conveys the material (or modified versions of
-            it) with contractual assumptions of liability to the recipient, for
-            any liability that these contractual assumptions directly impose on
-            those licensors and authors.
-        
-          All other non-permissive additional terms are considered "further
-        restrictions" within the meaning of section 10.  If the Program as you
-        received it, or any part of it, contains a notice stating that it is
-        governed by this License along with a term that is a further
-        restriction, you may remove that term.  If a license document contains
-        a further restriction but permits relicensing or conveying under this
-        License, you may add to a covered work material governed by the terms
-        of that license document, provided that the further restriction does
-        not survive such relicensing or conveying.
-        
-          If you add terms to a covered work in accord with this section, you
-        must place, in the relevant source files, a statement of the
-        additional terms that apply to those files, or a notice indicating
-        where to find the applicable terms.
-        
-          Additional terms, permissive or non-permissive, may be stated in the
-        form of a separately written license, or stated as exceptions;
-        the above requirements apply either way.
-        
-          8. Termination.
-        
-          You may not propagate or modify a covered work except as expressly
-        provided under this License.  Any attempt otherwise to propagate or
-        modify it is void, and will automatically terminate your rights under
-        this License (including any patent licenses granted under the third
-        paragraph of section 11).
-        
-          However, if you cease all violation of this License, then your
-        license from a particular copyright holder is reinstated (a)
-        provisionally, unless and until the copyright holder explicitly and
-        finally terminates your license, and (b) permanently, if the copyright
-        holder fails to notify you of the violation by some reasonable means
-        prior to 60 days after the cessation.
-        
-          Moreover, your license from a particular copyright holder is
-        reinstated permanently if the copyright holder notifies you of the
-        violation by some reasonable means, this is the first time you have
-        received notice of violation of this License (for any work) from that
-        copyright holder, and you cure the violation prior to 30 days after
-        your receipt of the notice.
-        
-          Termination of your rights under this section does not terminate the
-        licenses of parties who have received copies or rights from you under
-        this License.  If your rights have been terminated and not permanently
-        reinstated, you do not qualify to receive new licenses for the same
-        material under section 10.
-        
-          9. Acceptance Not Required for Having Copies.
-        
-          You are not required to accept this License in order to receive or
-        run a copy of the Program.  Ancillary propagation of a covered work
-        occurring solely as a consequence of using peer-to-peer transmission
-        to receive a copy likewise does not require acceptance.  However,
-        nothing other than this License grants you permission to propagate or
-        modify any covered work.  These actions infringe copyright if you do
-        not accept this License.  Therefore, by modifying or propagating a
-        covered work, you indicate your acceptance of this License to do so.
-        
-          10. Automatic Licensing of Downstream Recipients.
-        
-          Each time you convey a covered work, the recipient automatically
-        receives a license from the original licensors, to run, modify and
-        propagate that work, subject to this License.  You are not responsible
-        for enforcing compliance by third parties with this License.
-        
-          An "entity transaction" is a transaction transferring control of an
-        organization, or substantially all assets of one, or subdividing an
-        organization, or merging organizations.  If propagation of a covered
-        work results from an entity transaction, each party to that
-        transaction who receives a copy of the work also receives whatever
-        licenses to the work the party's predecessor in interest had or could
-        give under the previous paragraph, plus a right to possession of the
-        Corresponding Source of the work from the predecessor in interest, if
-        the predecessor has it or can get it with reasonable efforts.
-        
-          You may not impose any further restrictions on the exercise of the
-        rights granted or affirmed under this License.  For example, you may
-        not impose a license fee, royalty, or other charge for exercise of
-        rights granted under this License, and you may not initiate litigation
-        (including a cross-claim or counterclaim in a lawsuit) alleging that
-        any patent claim is infringed by making, using, selling, offering for
-        sale, or importing the Program or any portion of it.
-        
-          11. Patents.
-        
-          A "contributor" is a copyright holder who authorizes use under this
-        License of the Program or a work on which the Program is based.  The
-        work thus licensed is called the contributor's "contributor version".
-        
-          A contributor's "essential patent claims" are all patent claims
-        owned or controlled by the contributor, whether already acquired or
-        hereafter acquired, that would be infringed by some manner, permitted
-        by this License, of making, using, or selling its contributor version,
-        but do not include claims that would be infringed only as a
-        consequence of further modification of the contributor version.  For
-        purposes of this definition, "control" includes the right to grant
-        patent sublicenses in a manner consistent with the requirements of
-        this License.
-        
-          Each contributor grants you a non-exclusive, worldwide, royalty-free
-        patent license under the contributor's essential patent claims, to
-        make, use, sell, offer for sale, import and otherwise run, modify and
-        propagate the contents of its contributor version.
-        
-          In the following three paragraphs, a "patent license" is any express
-        agreement or commitment, however denominated, not to enforce a patent
-        (such as an express permission to practice a patent or covenant not to
-        sue for patent infringement).  To "grant" such a patent license to a
-        party means to make such an agreement or commitment not to enforce a
-        patent against the party.
-        
-          If you convey a covered work, knowingly relying on a patent license,
-        and the Corresponding Source of the work is not available for anyone
-        to copy, free of charge and under the terms of this License, through a
-        publicly available network server or other readily accessible means,
-        then you must either (1) cause the Corresponding Source to be so
-        available, or (2) arrange to deprive yourself of the benefit of the
-        patent license for this particular work, or (3) arrange, in a manner
-        consistent with the requirements of this License, to extend the patent
-        license to downstream recipients.  "Knowingly relying" means you have
-        actual knowledge that, but for the patent license, your conveying the
-        covered work in a country, or your recipient's use of the covered work
-        in a country, would infringe one or more identifiable patents in that
-        country that you have reason to believe are valid.
-        
-          If, pursuant to or in connection with a single transaction or
-        arrangement, you convey, or propagate by procuring conveyance of, a
-        covered work, and grant a patent license to some of the parties
-        receiving the covered work authorizing them to use, propagate, modify
-        or convey a specific copy of the covered work, then the patent license
-        you grant is automatically extended to all recipients of the covered
-        work and works based on it.
-        
-          A patent license is "discriminatory" if it does not include within
-        the scope of its coverage, prohibits the exercise of, or is
-        conditioned on the non-exercise of one or more of the rights that are
-        specifically granted under this License.  You may not convey a covered
-        work if you are a party to an arrangement with a third party that is
-        in the business of distributing software, under which you make payment
-        to the third party based on the extent of your activity of conveying
-        the work, and under which the third party grants, to any of the
-        parties who would receive the covered work from you, a discriminatory
-        patent license (a) in connection with copies of the covered work
-        conveyed by you (or copies made from those copies), or (b) primarily
-        for and in connection with specific products or compilations that
-        contain the covered work, unless you entered into that arrangement,
-        or that patent license was granted, prior to 28 March 2007.
-        
-          Nothing in this License shall be construed as excluding or limiting
-        any implied license or other defenses to infringement that may
-        otherwise be available to you under applicable patent law.
-        
-          12. No Surrender of Others' Freedom.
-        
-          If conditions are imposed on you (whether by court order, agreement or
-        otherwise) that contradict the conditions of this License, they do not
-        excuse you from the conditions of this License.  If you cannot convey a
-        covered work so as to satisfy simultaneously your obligations under this
-        License and any other pertinent obligations, then as a consequence you may
-        not convey it at all.  For example, if you agree to terms that obligate you
-        to collect a royalty for further conveying from those to whom you convey
-        the Program, the only way you could satisfy both those terms and this
-        License would be to refrain entirely from conveying the Program.
-        
-          13. Use with the GNU Affero General Public License.
-        
-          Notwithstanding any other provision of this License, you have
-        permission to link or combine any covered work with a work licensed
-        under version 3 of the GNU Affero General Public License into a single
-        combined work, and to convey the resulting work.  The terms of this
-        License will continue to apply to the part which is the covered work,
-        but the special requirements of the GNU Affero General Public License,
-        section 13, concerning interaction through a network will apply to the
-        combination as such.
-        
-          14. Revised Versions of this License.
-        
-          The Free Software Foundation may publish revised and/or new versions of
-        the GNU General Public License from time to time.  Such new versions will
-        be similar in spirit to the present version, but may differ in detail to
-        address new problems or concerns.
-        
-          Each version is given a distinguishing version number.  If the
-        Program specifies that a certain numbered version of the GNU General
-        Public License "or any later version" applies to it, you have the
-        option of following the terms and conditions either of that numbered
-        version or of any later version published by the Free Software
-        Foundation.  If the Program does not specify a version number of the
-        GNU General Public License, you may choose any version ever published
-        by the Free Software Foundation.
-        
-          If the Program specifies that a proxy can decide which future
-        versions of the GNU General Public License can be used, that proxy's
-        public statement of acceptance of a version permanently authorizes you
-        to choose that version for the Program.
-        
-          Later license versions may give you additional or different
-        permissions.  However, no additional obligations are imposed on any
-        author or copyright holder as a result of your choosing to follow a
-        later version.
-        
-          15. Disclaimer of Warranty.
-        
-          THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-        APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-        HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-        OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-        THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-        PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-        IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-        ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-        
-          16. Limitation of Liability.
-        
-          IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-        WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-        THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-        GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-        USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-        DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-        PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-        EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-        SUCH DAMAGES.
-        
-          17. Interpretation of Sections 15 and 16.
-        
-          If the disclaimer of warranty and limitation of liability provided
-        above cannot be given local legal effect according to their terms,
-        reviewing courts shall apply local law that most closely approximates
-        an absolute waiver of all civil liability in connection with the
-        Program, unless a warranty or assumption of liability accompanies a
-        copy of the Program in return for a fee.
-        
-                             END OF TERMS AND CONDITIONS
-        
-                    How to Apply These Terms to Your New Programs
-        
-          If you develop a new program, and you want it to be of the greatest
-        possible use to the public, the best way to achieve this is to make it
-        free software which everyone can redistribute and change under these terms.
-        
-          To do so, attach the following notices to the program.  It is safest
-        to attach them to the start of each source file to most effectively
-        state the exclusion of warranty; and each file should have at least
-        the "copyright" line and a pointer to where the full notice is found.
-        
-            <one line to give the program's name and a brief idea of what it does.>
-            Copyright (C) <year>  <name of author>
-        
-            This program is free software: you can redistribute it and/or modify
-            it under the terms of the GNU General Public License as published by
-            the Free Software Foundation, either version 3 of the License, or
-            (at your option) any later version.
-        
-            This program is distributed in the hope that it will be useful,
-            but WITHOUT ANY WARRANTY; without even the implied warranty of
-            MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-            GNU General Public License for more details.
-        
-            You should have received a copy of the GNU General Public License
-            along with this program.  If not, see <https://www.gnu.org/licenses/>.
-        
-        Also add information on how to contact you by electronic and paper mail.
-        
-          If the program does terminal interaction, make it output a short
-        notice like this when it starts in an interactive mode:
-        
-            <program>  Copyright (C) <year>  <name of author>
-            This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-            This is free software, and you are welcome to redistribute it
-            under certain conditions; type `show c' for details.
-        
-        The hypothetical commands `show w' and `show c' should show the appropriate
-        parts of the General Public License.  Of course, your program's commands
-        might be different; for a GUI interface, you would use an "about box".
-        
-          You should also get your employer (if you work as a programmer) or school,
-        if any, to sign a "copyright disclaimer" for the program, if necessary.
-        For more information on this, and how to apply and follow the GNU GPL, see
-        <https://www.gnu.org/licenses/>.
-        
-          The GNU General Public License does not permit incorporating your program
-        into proprietary programs.  If your program is a subroutine library, you
-        may consider it more useful to permit linking proprietary applications with
-        the library.  If this is what you want to do, use the GNU Lesser General
-        Public License instead of this License.  But first, please read
-        <https://www.gnu.org/licenses/why-not-lgpl.html>.
-        
-Project-URL: Homepage, https://github.com/OpenStickCommunity/gp2040ce-binary-tools
-Project-URL: Changelog, https://github.com/OpenStickCommunity/gp2040ce-binary-tools/blob/main/CHANGELOG.md
-Project-URL: Bug Tracker, https://github.com/OpenStickCommunity/gp2040ce-binary-tools/issues
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Utilities
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: grpcio-tools
-Requires-Dist: pyusb
-Requires-Dist: textual
-Provides-Extra: dev
-Requires-Dist: bandit; extra == "dev"
-Requires-Dist: decorator; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: flake8-blind-except; extra == "dev"
-Requires-Dist: flake8-builtins; extra == "dev"
-Requires-Dist: flake8-docstrings; extra == "dev"
-Requires-Dist: flake8-executable; extra == "dev"
-Requires-Dist: flake8-fixme; extra == "dev"
-Requires-Dist: flake8-isort; extra == "dev"
-Requires-Dist: flake8-logging-format; extra == "dev"
-Requires-Dist: flake8-mutable; extra == "dev"
-Requires-Dist: flake8-pyproject; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: pip-tools; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: pytest-asyncio; extra == "dev"
-Requires-Dist: pytest-cov; extra == "dev"
-Requires-Dist: setuptools-scm; extra == "dev"
-Requires-Dist: textual-dev; extra == "dev"
-Requires-Dist: tox; extra == "dev"
-
-# GP2040-CE Binary Tools
-
-Tools for working with GP2040-CE binary dumps.
-
-## Dependencies
-
-While not necessary for most tools, you may want [picotool](https://github.com/raspberrypi/picotool) as an alternative
-way to dump binary data from the board. These dumps can be created with `gp2040ce-binary-tools` natively, but having an
-alternative way to create a binary dump can be helpful, as these tools work as well (or better) with a binary dump as
-over USB.
-
-### Protobuf Files
-
-All tools take `-P PATH` flag(s) in order to import Protobuf files (either precompiled Python files or raw .proto files)
-if you have them locally, in order to work with the latest (or development) version of the configuration. That said,
-this tool also includes a precompiled fallback version of the config structure if you cannot supply these files. Be
-aware, however, that they are a point in time snapshot, and may lag the real format in undesirable ways. Supply the
-latest Protobuf files if you can.
-
-An example of this invocation is:
-
-`visualize-storage -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto --filename memory.bin`
-
-## Installation
-
-```
-% pip install gp2040ce-binary-tools
-```
-
-### Development Installation
-
-```
-% git clone [URL to this repository]
-% cd gp2040ce-binary-tools
-% python -m venv venv
-% source ./venv/bin/activate
-% pip install -e .
-% pip install -Ur requirements/requirements-dev.txt
-```
-
-## Tools
-
-In all cases, online help can be retrieved by providing the `-h` or ``--help`` flags to the below programs.
-
-### Config Editor
-
-[![asciicast](https://asciinema.org/a/67hELtUNkKCit4dFwYeAUa2fo.svg)](https://asciinema.org/a/67hELtUNkKCit4dFwYeAUa2fo)
-
-A terminal UI config editor, capable of viewing and editing existing configurations, can be launched via
-`edit-config`. It supports navigation both via the keyboard or the mouse, and can view and edit either a binary file
-made via `picotool` or configuration directly on the board in BOOTSEL mode over USB.
-
-Simple usage:
-
-| Key(s)                | Action                                                 |
-|-----------------------|--------------------------------------------------------|
-| Up, Down              | Move up and down the config tree                       |
-| Left, Right           | Scroll the tree left and right (when content is long)  |
-| Space                 | Expand a tree node to show its children                |
-| Enter                 | Expand a tree node, or edit a leaf node (bools toggle) |
-| Tab (in edit popup)   | Cycle highlight between input field and buttons        |
-| Enter (in edit popup) | Choose dropdown option or activate button              |
-| S                     | Save the config to the opened file                     |
-| Q                     | Quit without saving                                    |
-
-A quick demonstration of the editor is available [on asciinema.org](https://asciinema.org/a/67hELtUNkKCit4dFwYeAUa2fo).
-
-### concatenate
-
-`concatenate` combines a GP2040-CE firmware .bin file (such as from a fresh build) with:
-
-* a GP2040-CE board config, in the form of
-    * a config section .bin (with footer) (optionally padded) (`--binary-board-config-filename`) or
-    * a JSON file representing the config (`--json-board-config-filename`)
-* and/or a GP2040-CE user config, in the form of
-    * a config section .bin (with footer) (optionally padded) (`--binary-user-config-filename`) or
-    * a JSON file representing the config (`--json-user-config-filename`)
-
-...and produces a properly-offset firmware file suitable for flashing to a board with the provided config(s). This may
-be useful to ensure the board is flashed with a particular configuration, for instances such as producing a binary to
-flash many boards with a particular configuration (specific customizations, etc.), creating a file suitable for the
-initial install of a fresh board (a "board config"), or keeping documented backups of what you're testing with during
-development.
-
-The `--...-board-config-filename` flags allow for shipping a default configuration as part of the binary, replacing
-the need for generating these board configurations at compile time. This allows for more custom builds and less
-dependency on the build jobs, and is a feature in progress in the core firmware.
-
-The produced firmware + config(s) can be written to a file with `--new-binary-filename FILENAME` or straight to a RP2040
-in BOOTSEL mode with `--usb`. The output file is a direct binary representation by default, but if `FILENAME` ends in
-".uf2", it will be written in the UF2 format, which is generally more convenient to the end user.
-
-Sample usage:
-
-```
-% concatenate build/GP2040-CE_foo_bar.bin --binary-user-config-filename storage-dump.bin \
-    --new-binary-filename new-firmware-with-config.bin
-```
-
-### dump-config
-
-`dump-config` replaces the need for picotool in order to make a copy of the GP2040-CE configuration as a binary file.
-This could be used with the other tools, or just to keep a backup.
-
-Sample usage:
-
-```
-% dump-config `date +%Y%m%d`-config-backup.bin
-```
-
-### dump-gp2040ce
-
-`dump-gp2040ce` replaces the need for picotool in order to make a copy of a board's full GP2040-CE image as a binary file.
-This could be used with the other tools, or just to keep a backup.
-
-Sample usage:
-
-```
-% dump-gp2040ce `date +%Y%m%d`-backup.bin
-```
-
-### visualize-storage
-
-`visualize-storage` reads a GP2040-CE board's configuration, either over USB or from a dump of the board's flash
-storage section, and prints it out for visual inspection or diffing with other tools. It can also find the storage
-section from a GP2040-CE whole board dump, if you have that instead. Usage is simple; just connect your board in BOOTSEL
-mode or pass the tool your binary file to analyze along with the path to the Protobuf files.
-
-Sample output:
-
-```
-% visualize-storage --usb
-boardVersion: "v0.7.2"
-gamepadOptions {
-  inputMode: INPUT_MODE_HID
-  dpadMode: DPAD_MODE_DIGITAL
-  socdMode: SOCD_MODE_SECOND_INPUT_PRIORITY
-  invertXAxis: false
-  invertYAxis: false
-  switchTpShareForDs4: true
-  lockHotkeys: false
-}
-hotkeyOptions {
-  hotkeyF1Up {
-    dpadMask: 1
-    action: HOTKEY_SOCD_UP_PRIORITY
-  }
-  hotkeyF1Down {
-    dpadMask: 2
-    action: HOTKEY_SOCD_NEUTRAL
-  }
-  ...[and so on]...
-}
-pinMappings {
-  pinDpadUp: 19
-  pinDpadDown: 18
-  pinDpadLeft: 16
-  pinDpadRight: 17
-  pinButtonB1: 8
-  pinButtonB2: 7
-  pinButtonB3: 12
-  pinButtonB4: 11
-  pinButtonL1: 9
-  pinButtonR1: 10
-  pinButtonL2: 5
-  pinButtonR2: 6
-  pinButtonS1: 15
-  pinButtonS2: 13
-  pinButtonL3: 21
-  pinButtonR3: 22
-  pinButtonA1: 14
-  pinButtonA2: 20
-}
-...[and so on]...
-addonOptions {
-  bootselButtonOptions {
-    enabled: false
-    buttonMap: 0
-  }
-  ...[and so on]...
-  dualDirectionalOptions {
-    enabled: true
-    upPin: 23
-    downPin: 27
-    leftPin: 26
-    rightPin: 24
-    dpadMode: DPAD_MODE_DIGITAL
-    combineMode: 3
-  }
-  ...[and so on]...
-}
-forcedSetupOptions {
-  mode: FORCED_SETUP_MODE_OFF
-}
-```
-
-## Miscellaneous
-
-### Version information
-
-The GP2040-CE configuration is still changing, so the tools are changing accordingly. This project doesn't currently make
-a huge effort to be backwards compatible, so instead, refer to this:
-
-#### Flash Layouts
-
-* `gp2040ce-binary-tools >=v0.6.0` supports both board and user configs still being developed in `GP2040-CE`.
-* `gp2040ce-binary-tools >=v0.5.1` supported the increased user config size in `GP2040-CE >=v0.7.5`.
-* `gp2040ce-binary-tools <=v0.5.0` supported the smaller user config size in `GP2040-CE <v0.7.5`.
-
-#### Config Structures
-
-The latest update of the configuration snapshot is from **v0.7.8-RC2**.
-
-### Dumping the GP2040-CE board with picotool
-
-Some of these tools require a dump of your GP2040-CE board, either the storage section or the whole board, depending on
-the context. The storage section of a GP2040-CE board is a reserved 16 KB starting at `0x101FC000`. To dump your board's
-storage with picotool:
-
-```
-% picotool save -r 101FC000 10200000 memory.bin
-```
-
-And to dump your whole board:
-
-```
-% picotool save -a whole-board.bin
-```
-
-## Author and Licensing
-
-Written by and copyright Brian S. Stephan (<bss@incorporeal.org>).
-
-gp2040ce-binary-tools is free software: you can redistribute it and/or modify it under the terms of the GNU General
-Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any
-later version.
-
-gp2040ce-binary-tools is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the
-implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more
-details.
+GNU GENERAL PUBLIC LICENSE
+Version 3, 29 June 2007
 
-You should have received a copy of the GNU General Public License along with gp2040ce-binary-tools. If not, see
-<https://www.gnu.org/licenses/>.
+Copyright © 2007 Free Software Foundation, Inc. <https://fsf.org/>
+
+Everyone is permitted to copy and distribute verbatim copies of this license document, but changing it is not allowed.
+
+Preamble
+
+The GNU General Public License is a free, copyleft license for software and other kinds of works.
+
+The licenses for most software and other practical works are designed to take away your freedom to share and change the works. By contrast, the GNU General Public License is intended to guarantee your freedom to share and change all versions of a program--to make sure it remains free software for all its users. We, the Free Software Foundation, use the GNU General Public License for most of our software; it applies also to any other work released this way by its authors. You can apply it to your programs, too.
+
+When we speak of free software, we are referring to freedom, not price. Our General Public Licenses are designed to make sure that you have the freedom to distribute copies of free software (and charge for them if you wish), that you receive source code or can get it if you want it, that you can change the software or use pieces of it in new free programs, and that you know you can do these things.
+
+To protect your rights, we need to prevent others from denying you these rights or asking you to surrender the rights. Therefore, you have certain responsibilities if you distribute copies of the software, or if you modify it: responsibilities to respect the freedom of others.
+
+For example, if you distribute copies of such a program, whether gratis or for a fee, you must pass on to the recipients the same freedoms that you received. You must make sure that they, too, receive or can get the source code. And you must show them these terms so they know their rights.
+
+Developers that use the GNU GPL protect your rights with two steps: (1) assert copyright on the software, and (2) offer you this License giving you legal permission to copy, distribute and/or modify it.
+
+For the developers' and authors' protection, the GPL clearly explains that there is no warranty for this free software. For both users' and authors' sake, the GPL requires that modified versions be marked as changed, so that their problems will not be attributed erroneously to authors of previous versions.
+
+Some devices are designed to deny users access to install or run modified versions of the software inside them, although the manufacturer can do so. This is fundamentally incompatible with the aim of protecting users' freedom to change the software. The systematic pattern of such abuse occurs in the area of products for individuals to use, which is precisely where it is most unacceptable. Therefore, we have designed this version of the GPL to prohibit the practice for those products. If such problems arise substantially in other domains, we stand ready to extend this provision to those domains in future versions of the GPL, as needed to protect the freedom of users.
+
+Finally, every program is threatened constantly by software patents. States should not allow patents to restrict development and use of software on general-purpose computers, but in those that do, we wish to avoid the special danger that patents applied to a free program could make it effectively proprietary. To prevent this, the GPL assures that patents cannot be used to render the program non-free.
+
+The precise terms and conditions for copying, distribution and modification follow.
+
+TERMS AND CONDITIONS
+
+0. Definitions.
+
+“This License” refers to version 3 of the GNU General Public License.
+
+“Copyright” also means copyright-like laws that apply to other kinds of works, such as semiconductor masks.
+
+“The Program” refers to any copyrightable work licensed under this License. Each licensee is addressed as “you”. “Licensees” and “recipients” may be individuals or organizations.
+
+To “modify” a work means to copy from or adapt all or part of the work in a fashion requiring copyright permission, other than the making of an exact copy. The resulting work is called a “modified version” of the earlier work or a work “based on” the earlier work.
+
+A “covered work” means either the unmodified Program or a work based on the Program.
+
+To “propagate” a work means to do anything with it that, without permission, would make you directly or secondarily liable for infringement under applicable copyright law, except executing it on a computer or modifying a private copy. Propagation includes copying, distribution (with or without modification), making available to the public, and in some countries other activities as well.
+
+To “convey” a work means any kind of propagation that enables other parties to make or receive copies. Mere interaction with a user through a computer network, with no transfer of a copy, is not conveying.
+
+An interactive user interface displays “Appropriate Legal Notices” to the extent that it includes a convenient and prominently visible feature that (1) displays an appropriate copyright notice, and (2) tells the user that there is no warranty for the work (except to the extent that warranties are provided), that licensees may convey the work under this License, and how to view a copy of this License. If the interface presents a list of user commands or options, such as a menu, a prominent item in the list meets this criterion.
+
+1. Source Code.
+The “source code” for a work means the preferred form of the work for making modifications to it. “Object code” means any non-source form of a work.
+
+A “Standard Interface” means an interface that either is an official standard defined by a recognized standards body, or, in the case of interfaces specified for a particular programming language, one that is widely used among developers working in that language.
+
+The “System Libraries” of an executable work include anything, other than the work as a whole, that (a) is included in the normal form of packaging a Major Component, but which is not part of that Major Component, and (b) serves only to enable use of the work with that Major Component, or to implement a Standard Interface for which an implementation is available to the public in source code form. A “Major Component”, in this context, means a major essential component (kernel, window system, and so on) of the specific operating system (if any) on which the executable work runs, or a compiler used to produce the work, or an object code interpreter used to run it.
+
+The “Corresponding Source” for a work in object code form means all the source code needed to generate, install, and (for an executable work) run the object code and to modify the work, including scripts to control those activities. However, it does not include the work's System Libraries, or general-purpose tools or generally available free programs which are used unmodified in performing those activities but which are not part of the work. For example, Corresponding Source includes interface definition files associated with source files for the work, and the source code for shared libraries and dynamically linked subprograms that the work is specifically designed to require, such as by intimate data communication or control flow between those subprograms and other parts of the work.
+
+The Corresponding Source need not include anything that users can regenerate automatically from other parts of the Corresponding Source.
+
+The Corresponding Source for a work in source code form is that same work.
+
+2. Basic Permissions.
+All rights granted under this License are granted for the term of copyright on the Program, and are irrevocable provided the stated conditions are met. This License explicitly affirms your unlimited permission to run the unmodified Program. The output from running a covered work is covered by this License only if the output, given its content, constitutes a covered work. This License acknowledges your rights of fair use or other equivalent, as provided by copyright law.
+
+You may make, run and propagate covered works that you do not convey, without conditions so long as your license otherwise remains in force. You may convey covered works to others for the sole purpose of having them make modifications exclusively for you, or provide you with facilities for running those works, provided that you comply with the terms of this License in conveying all material for which you do not control copyright. Those thus making or running the covered works for you must do so exclusively on your behalf, under your direction and control, on terms that prohibit them from making any copies of your copyrighted material outside their relationship with you.
+
+Conveying under any other circumstances is permitted solely under the conditions stated below. Sublicensing is not allowed; section 10 makes it unnecessary.
+
+3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+No covered work shall be deemed part of an effective technological measure under any applicable law fulfilling obligations under article 11 of the WIPO copyright treaty adopted on 20 December 1996, or similar laws prohibiting or restricting circumvention of such measures.
+
+When you convey a covered work, you waive any legal power to forbid circumvention of technological measures to the extent such circumvention is effected by exercising rights under this License with respect to the covered work, and you disclaim any intention to limit operation or modification of the work as a means of enforcing, against the work's users, your or third parties' legal rights to forbid circumvention of technological measures.
+
+4. Conveying Verbatim Copies.
+You may convey verbatim copies of the Program's source code as you receive it, in any medium, provided that you conspicuously and appropriately publish on each copy an appropriate copyright notice; keep intact all notices stating that this License and any non-permissive terms added in accord with section 7 apply to the code; keep intact all notices of the absence of any warranty; and give all recipients a copy of this License along with the Program.
+
+You may charge any price or no price for each copy that you convey, and you may offer support or warranty protection for a fee.
+
+5. Conveying Modified Source Versions.
+You may convey a work based on the Program, or the modifications to produce it from the Program, in the form of source code under the terms of section 4, provided that you also meet all of these conditions:
+
+     a) The work must carry prominent notices stating that you modified it, and giving a relevant date.
+
+     b) The work must carry prominent notices stating that it is released under this License and any conditions added under section 7. This requirement modifies the requirement in section 4 to “keep intact all notices”.
+
+     c) You must license the entire work, as a whole, under this License to anyone who comes into possession of a copy. This License will therefore apply, along with any applicable section 7 additional terms, to the whole of the work, and all its parts, regardless of how they are packaged. This License gives no permission to license the work in any other way, but it does not invalidate such permission if you have separately received it.
+
+     d) If the work has interactive user interfaces, each must display Appropriate Legal Notices; however, if the Program has interactive interfaces that do not display Appropriate Legal Notices, your work need not make them do so.
+
+A compilation of a covered work with other separate and independent works, which are not by their nature extensions of the covered work, and which are not combined with it such as to form a larger program, in or on a volume of a storage or distribution medium, is called an “aggregate” if the compilation and its resulting copyright are not used to limit the access or legal rights of the compilation's users beyond what the individual works permit. Inclusion of a covered work in an aggregate does not cause this License to apply to the other parts of the aggregate.
+
+6. Conveying Non-Source Forms.
+You may convey a covered work in object code form under the terms of sections 4 and 5, provided that you also convey the machine-readable Corresponding Source under the terms of this License, in one of these ways:
+
+     a) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by the Corresponding Source fixed on a durable physical medium customarily used for software interchange.
+
+     b) Convey the object code in, or embodied in, a physical product (including a physical distribution medium), accompanied by a written offer, valid for at least three years and valid for as long as you offer spare parts or customer support for that product model, to give anyone who possesses the object code either (1) a copy of the Corresponding Source for all the software in the product that is covered by this License, on a durable physical medium customarily used for software interchange, for a price no more than your reasonable cost of physically performing this conveying of source, or (2) access to copy the Corresponding Source from a network server at no charge.
+
+     c) Convey individual copies of the object code with a copy of the written offer to provide the Corresponding Source. This alternative is allowed only occasionally and noncommercially, and only if you received the object code with such an offer, in accord with subsection 6b.
+
+     d) Convey the object code by offering access from a designated place (gratis or for a charge), and offer equivalent access to the Corresponding Source in the same way through the same place at no further charge. You need not require recipients to copy the Corresponding Source along with the object code. If the place to copy the object code is a network server, the Corresponding Source may be on a different server (operated by you or a third party) that supports equivalent copying facilities, provided you maintain clear directions next to the object code saying where to find the Corresponding Source. Regardless of what server hosts the Corresponding Source, you remain obligated to ensure that it is available for as long as needed to satisfy these requirements.
+
+     e) Convey the object code using peer-to-peer transmission, provided you inform other peers where the object code and Corresponding Source of the work are being offered to the general public at no charge under subsection 6d.
+
+A separable portion of the object code, whose source code is excluded from the Corresponding Source as a System Library, need not be included in conveying the object code work.
+
+A “User Product” is either (1) a “consumer product”, which means any tangible personal property which is normally used for personal, family, or household purposes, or (2) anything designed or sold for incorporation into a dwelling. In determining whether a product is a consumer product, doubtful cases shall be resolved in favor of coverage. For a particular product received by a particular user, “normally used” refers to a typical or common use of that class of product, regardless of the status of the particular user or of the way in which the particular user actually uses, or expects or is expected to use, the product. A product is a consumer product regardless of whether the product has substantial commercial, industrial or non-consumer uses, unless such uses represent the only significant mode of use of the product.
+
+“Installation Information” for a User Product means any methods, procedures, authorization keys, or other information required to install and execute modified versions of a covered work in that User Product from a modified version of its Corresponding Source. The information must suffice to ensure that the continued functioning of the modified object code is in no case prevented or interfered with solely because modification has been made.
+
+If you convey an object code work under this section in, or with, or specifically for use in, a User Product, and the conveying occurs as part of a transaction in which the right of possession and use of the User Product is transferred to the recipient in perpetuity or for a fixed term (regardless of how the transaction is characterized), the Corresponding Source conveyed under this section must be accompanied by the Installation Information. But this requirement does not apply if neither you nor any third party retains the ability to install modified object code on the User Product (for example, the work has been installed in ROM).
+
+The requirement to provide Installation Information does not include a requirement to continue to provide support service, warranty, or updates for a work that has been modified or installed by the recipient, or for the User Product in which it has been modified or installed. Access to a network may be denied when the modification itself materially and adversely affects the operation of the network or violates the rules and protocols for communication across the network.
+
+Corresponding Source conveyed, and Installation Information provided, in accord with this section must be in a format that is publicly documented (and with an implementation available to the public in source code form), and must require no special password or key for unpacking, reading or copying.
+
+7. Additional Terms.
+“Additional permissions” are terms that supplement the terms of this License by making exceptions from one or more of its conditions. Additional permissions that are applicable to the entire Program shall be treated as though they were included in this License, to the extent that they are valid under applicable law. If additional permissions apply only to part of the Program, that part may be used separately under those permissions, but the entire Program remains governed by this License without regard to the additional permissions.
+
+When you convey a copy of a covered work, you may at your option remove any additional permissions from that copy, or from any part of it. (Additional permissions may be written to require their own removal in certain cases when you modify the work.) You may place additional permissions on material, added by you to a covered work, for which you have or can give appropriate copyright permission.
+
+Notwithstanding any other provision of this License, for material you add to a covered work, you may (if authorized by the copyright holders of that material) supplement the terms of this License with terms:
+
+     a) Disclaiming warranty or limiting liability differently from the terms of sections 15 and 16 of this License; or
+
+     b) Requiring preservation of specified reasonable legal notices or author attributions in that material or in the Appropriate Legal Notices displayed by works containing it; or
+
+     c) Prohibiting misrepresentation of the origin of that material, or requiring that modified versions of such material be marked in reasonable ways as different from the original version; or
+
+     d) Limiting the use for publicity purposes of names of licensors or authors of the material; or
+
+     e) Declining to grant rights under trademark law for use of some trade names, trademarks, or service marks; or
+
+     f) Requiring indemnification of licensors and authors of that material by anyone who conveys the material (or modified versions of it) with contractual assumptions of liability to the recipient, for any liability that these contractual assumptions directly impose on those licensors and authors.
+
+All other non-permissive additional terms are considered “further restrictions” within the meaning of section 10. If the Program as you received it, or any part of it, contains a notice stating that it is governed by this License along with a term that is a further restriction, you may remove that term. If a license document contains a further restriction but permits relicensing or conveying under this License, you may add to a covered work material governed by the terms of that license document, provided that the further restriction does not survive such relicensing or conveying.
+
+If you add terms to a covered work in accord with this section, you must place, in the relevant source files, a statement of the additional terms that apply to those files, or a notice indicating where to find the applicable terms.
+
+Additional terms, permissive or non-permissive, may be stated in the form of a separately written license, or stated as exceptions; the above requirements apply either way.
+
+8. Termination.
+You may not propagate or modify a covered work except as expressly provided under this License. Any attempt otherwise to propagate or modify it is void, and will automatically terminate your rights under this License (including any patent licenses granted under the third paragraph of section 11).
+
+However, if you cease all violation of this License, then your license from a particular copyright holder is reinstated (a) provisionally, unless and until the copyright holder explicitly and finally terminates your license, and (b) permanently, if the copyright holder fails to notify you of the violation by some reasonable means prior to 60 days after the cessation.
+
+Moreover, your license from a particular copyright holder is reinstated permanently if the copyright holder notifies you of the violation by some reasonable means, this is the first time you have received notice of violation of this License (for any work) from that copyright holder, and you cure the violation prior to 30 days after your receipt of the notice.
+
+Termination of your rights under this section does not terminate the licenses of parties who have received copies or rights from you under this License. If your rights have been terminated and not permanently reinstated, you do not qualify to receive new licenses for the same material under section 10.
+
+9. Acceptance Not Required for Having Copies.
+You are not required to accept this License in order to receive or run a copy of the Program. Ancillary propagation of a covered work occurring solely as a consequence of using peer-to-peer transmission to receive a copy likewise does not require acceptance. However, nothing other than this License grants you permission to propagate or modify any covered work. These actions infringe copyright if you do not accept this License. Therefore, by modifying or propagating a covered work, you indicate your acceptance of this License to do so.
+
+10. Automatic Licensing of Downstream Recipients.
+Each time you convey a covered work, the recipient automatically receives a license from the original licensors, to run, modify and propagate that work, subject to this License. You are not responsible for enforcing compliance by third parties with this License.
+
+An “entity transaction” is a transaction transferring control of an organization, or substantially all assets of one, or subdividing an organization, or merging organizations. If propagation of a covered work results from an entity transaction, each party to that transaction who receives a copy of the work also receives whatever licenses to the work the party's predecessor in interest had or could give under the previous paragraph, plus a right to possession of the Corresponding Source of the work from the predecessor in interest, if the predecessor has it or can get it with reasonable efforts.
+
+You may not impose any further restrictions on the exercise of the rights granted or affirmed under this License. For example, you may not impose a license fee, royalty, or other charge for exercise of rights granted under this License, and you may not initiate litigation (including a cross-claim or counterclaim in a lawsuit) alleging that any patent claim is infringed by making, using, selling, offering for sale, or importing the Program or any portion of it.
+
+11. Patents.
+A “contributor” is a copyright holder who authorizes use under this License of the Program or a work on which the Program is based. The work thus licensed is called the contributor's “contributor version”.
+
+A contributor's “essential patent claims” are all patent claims owned or controlled by the contributor, whether already acquired or hereafter acquired, that would be infringed by some manner, permitted by this License, of making, using, or selling its contributor version, but do not include claims that would be infringed only as a consequence of further modification of the contributor version. For purposes of this definition, “control” includes the right to grant patent sublicenses in a manner consistent with the requirements of this License.
+
+Each contributor grants you a non-exclusive, worldwide, royalty-free patent license under the contributor's essential patent claims, to make, use, sell, offer for sale, import and otherwise run, modify and propagate the contents of its contributor version.
+
+In the following three paragraphs, a “patent license” is any express agreement or commitment, however denominated, not to enforce a patent (such as an express permission to practice a patent or covenant not to sue for patent infringement). To “grant” such a patent license to a party means to make such an agreement or commitment not to enforce a patent against the party.
+
+If you convey a covered work, knowingly relying on a patent license, and the Corresponding Source of the work is not available for anyone to copy, free of charge and under the terms of this License, through a publicly available network server or other readily accessible means, then you must either (1) cause the Corresponding Source to be so available, or (2) arrange to deprive yourself of the benefit of the patent license for this particular work, or (3) arrange, in a manner consistent with the requirements of this License, to extend the patent license to downstream recipients. “Knowingly relying” means you have actual knowledge that, but for the patent license, your conveying the covered work in a country, or your recipient's use of the covered work in a country, would infringe one or more identifiable patents in that country that you have reason to believe are valid.
+
+If, pursuant to or in connection with a single transaction or arrangement, you convey, or propagate by procuring conveyance of, a covered work, and grant a patent license to some of the parties receiving the covered work authorizing them to use, propagate, modify or convey a specific copy of the covered work, then the patent license you grant is automatically extended to all recipients of the covered work and works based on it.
+
+A patent license is “discriminatory” if it does not include within the scope of its coverage, prohibits the exercise of, or is conditioned on the non-exercise of one or more of the rights that are specifically granted under this License. You may not convey a covered work if you are a party to an arrangement with a third party that is in the business of distributing software, under which you make payment to the third party based on the extent of your activity of conveying the work, and under which the third party grants, to any of the parties who would receive the covered work from you, a discriminatory patent license (a) in connection with copies of the covered work conveyed by you (or copies made from those copies), or (b) primarily for and in connection with specific products or compilations that contain the covered work, unless you entered into that arrangement, or that patent license was granted, prior to 28 March 2007.
+
+Nothing in this License shall be construed as excluding or limiting any implied license or other defenses to infringement that may otherwise be available to you under applicable patent law.
+
+12. No Surrender of Others' Freedom.
+If conditions are imposed on you (whether by court order, agreement or otherwise) that contradict the conditions of this License, they do not excuse you from the conditions of this License. If you cannot convey a covered work so as to satisfy simultaneously your obligations under this License and any other pertinent obligations, then as a consequence you may not convey it at all. For example, if you agree to terms that obligate you to collect a royalty for further conveying from those to whom you convey the Program, the only way you could satisfy both those terms and this License would be to refrain entirely from conveying the Program.
+
+13. Use with the GNU Affero General Public License.
+Notwithstanding any other provision of this License, you have permission to link or combine any covered work with a work licensed under version 3 of the GNU Affero General Public License into a single combined work, and to convey the resulting work. The terms of this License will continue to apply to the part which is the covered work, but the special requirements of the GNU Affero General Public License, section 13, concerning interaction through a network will apply to the combination as such.
+
+14. Revised Versions of this License.
+The Free Software Foundation may publish revised and/or new versions of the GNU General Public License from time to time. Such new versions will be similar in spirit to the present version, but may differ in detail to address new problems or concerns.
+
+Each version is given a distinguishing version number. If the Program specifies that a certain numbered version of the GNU General Public License “or any later version” applies to it, you have the option of following the terms and conditions either of that numbered version or of any later version published by the Free Software Foundation. If the Program does not specify a version number of the GNU General Public License, you may choose any version ever published by the Free Software Foundation.
+
+If the Program specifies that a proxy can decide which future versions of the GNU General Public License can be used, that proxy's public statement of acceptance of a version permanently authorizes you to choose that version for the Program.
+
+Later license versions may give you additional or different permissions. However, no additional obligations are imposed on any author or copyright holder as a result of your choosing to follow a later version.
+
+15. Disclaimer of Warranty.
+THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM “AS IS” WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+16. Limitation of Liability.
+IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
+
+17. Interpretation of Sections 15 and 16.
+If the disclaimer of warranty and limitation of liability provided above cannot be given local legal effect according to their terms, reviewing courts shall apply local law that most closely approximates an absolute waiver of all civil liability in connection with the Program, unless a warranty or assumption of liability accompanies a copy of the Program in return for a fee.
+
+END OF TERMS AND CONDITIONS
+
+How to Apply These Terms to Your New Programs
+
+If you develop a new program, and you want it to be of the greatest possible use to the public, the best way to achieve this is to make it free software which everyone can redistribute and change under these terms.
+
+To do so, attach the following notices to the program. It is safest to attach them to the start of each source file to most effectively state the exclusion of warranty; and each file should have at least the “copyright” line and a pointer to where the full notice is found.
+
+     <one line to give the program's name and a brief idea of what it does.>
+     Copyright (C) <year>  <name of author>
+
+     This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.
+
+     This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more details.
+
+     You should have received a copy of the GNU General Public License along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+If the program does terminal interaction, make it output a short notice like this when it starts in an interactive mode:
+
+     <program>  Copyright (C) <year>  <name of author>
+     This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+     This is free software, and you are welcome to redistribute it under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate parts of the General Public License. Of course, your program's commands might be different; for a GUI interface, you would use an “about box”.
+
+You should also get your employer (if you work as a programmer) or school, if any, to sign a “copyright disclaimer” for the program, if necessary. For more information on this, and how to apply and follow the GNU GPL, see <https://www.gnu.org/licenses/>.
+
+The GNU General Public License does not permit incorporating your program into proprietary programs. If your program is a subroutine library, you may consider it more useful to permit linking proprietary applications with the library. If this is what you want to do, use the GNU Lesser General Public License instead of this License. But first, please read <https://www.gnu.org/philosophy/why-not-lgpl.html>.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gp2040ce-binary-tools-0.7.0/README.md` & `gp2040ce_binary_tools-0.8.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 if you have them locally, in order to work with the latest (or development) version of the configuration. That said,
 this tool also includes a precompiled fallback version of the config structure if you cannot supply these files. Be
 aware, however, that they are a point in time snapshot, and may lag the real format in undesirable ways. Supply the
 latest Protobuf files if you can.
 
 An example of this invocation is:
 
-`visualize-storage -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto --filename memory.bin`
+`visualize-config -P ~/proj/GP2040-CE/proto -P ~/proj/GP2040-CE/lib/nanopb/generator/proto --filename memory.bin`
 
 ## Installation
 
 ```
 % pip install gp2040ce-binary-tools
 ```
 
@@ -82,23 +82,23 @@
 initial install of a fresh board (a "board config"), or keeping documented backups of what you're testing with during
 development.
 
 The `--...-board-config-filename` flags allow for shipping a default configuration as part of the binary, replacing
 the need for generating these board configurations at compile time. This allows for more custom builds and less
 dependency on the build jobs, and is a feature in progress in the core firmware.
 
-The produced firmware + config(s) can be written to a file with `--new-binary-filename FILENAME` or straight to a RP2040
+The produced firmware + config(s) can be written to a file with `--new-filename FILENAME` or straight to a RP2040
 in BOOTSEL mode with `--usb`. The output file is a direct binary representation by default, but if `FILENAME` ends in
 ".uf2", it will be written in the UF2 format, which is generally more convenient to the end user.
 
 Sample usage:
 
 ```
 % concatenate build/GP2040-CE_foo_bar.bin --binary-user-config-filename storage-dump.bin \
-    --new-binary-filename new-firmware-with-config.bin
+    --new-filename new-firmware-with-config.bin
 ```
 
 ### dump-config
 
 `dump-config` replaces the need for picotool in order to make a copy of the GP2040-CE configuration as a binary file.
 This could be used with the other tools, or just to keep a backup.
 
@@ -115,25 +115,43 @@
 
 Sample usage:
 
 ```
 % dump-gp2040ce `date +%Y%m%d`-backup.bin
 ```
 
-### visualize-storage
+### summarize-gp2040ce
 
-`visualize-storage` reads a GP2040-CE board's configuration, either over USB or from a dump of the board's flash
+`summarize-gp2040ce` prints information regarding the provided USB device or file. It attempts to detect the firmware
+and/or board config and/or user config version, which might be useful for confirming files are built properly, or to
+determine the lineage of something.
+
+Sample usage:
+
+```
+% summarize-gp2040ce --usb
+USB device:
+
+GP2040-CE Information
+  detected GP2040-CE version:     v0.7.8-9-g59e2d19b-dirty
+  detected board config version:  v0.7.8-board-test
+  detected user config version:   v0.7.8-RC2-1-g882235b3
+```
+
+### visualize-config
+
+`visualize-config` reads a GP2040-CE board's configuration, either over USB or from a dump of the board's flash
 storage section, and prints it out for visual inspection or diffing with other tools. It can also find the storage
 section from a GP2040-CE whole board dump, if you have that instead. Usage is simple; just connect your board in BOOTSEL
 mode or pass the tool your binary file to analyze along with the path to the Protobuf files.
 
 Sample output:
 
 ```
-% visualize-storage --usb
+% visualize-config --usb
 boardVersion: "v0.7.2"
 gamepadOptions {
   inputMode: INPUT_MODE_HID
   dpadMode: DPAD_MODE_DIGITAL
   socdMode: SOCD_MODE_SECOND_INPUT_PRIORITY
   invertXAxis: false
   invertYAxis: false
@@ -205,15 +223,15 @@
 
 * `gp2040ce-binary-tools >=v0.6.0` supports both board and user configs still being developed in `GP2040-CE`.
 * `gp2040ce-binary-tools >=v0.5.1` supported the increased user config size in `GP2040-CE >=v0.7.5`.
 * `gp2040ce-binary-tools <=v0.5.0` supported the smaller user config size in `GP2040-CE <v0.7.5`.
 
 #### Config Structures
 
-The latest update of the configuration snapshot is from **v0.7.8-RC2**.
+The latest update of the configuration snapshot is from **v0.7.8**.
 
 ### Dumping the GP2040-CE board with picotool
 
 Some of these tools require a dump of your GP2040-CE board, either the storage section or the whole board, depending on
 the context. The storage section of a GP2040-CE board is a reserved 16 KB starting at `0x101FC000`. To dump your board's
 storage with picotool:
```

### Comparing `gp2040ce-binary-tools-0.7.0/gp2040ce_binary_tools.egg-info/SOURCES.txt` & `gp2040ce_binary_tools-0.8.0/gp2040ce_binary_tools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 .gitattributes
 .gitignore
 CHANGELOG.md
 CONTRIBUTING.md
-DCO.txt
-LICENSE
+LICENSE.md
 MAINTAINERS.md
 README.md
 pyproject.toml
 tox.ini
+.reuse/dep5
+LICENSES/CC-BY-SA-4.0.txt
+LICENSES/GPL-3.0-or-later.txt
+LICENSES/MIT.txt
 gp2040ce_binary_tools.egg-info/PKG-INFO
 gp2040ce_binary_tools.egg-info/SOURCES.txt
 gp2040ce_binary_tools.egg-info/dependency_links.txt
 gp2040ce_binary_tools.egg-info/entry_points.txt
 gp2040ce_binary_tools.egg-info/requires.txt
 gp2040ce_binary_tools.egg-info/top_level.txt
 gp2040ce_bintools/__init__.py
```

### Comparing `gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/__init__.py` & `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/__init__.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/builder.py` & `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/builder.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 
 SPDX-FileCopyrightText: © 2023 Brian S. Stephan <bss@incorporeal.org>
 SPDX-License-Identifier: GPL-3.0-or-later
 """
 import argparse
 import copy
 import logging
+import re
 from typing import Optional
 
 from google.protobuf.message import Message
 
+import gp2040ce_bintools.storage as storage
 from gp2040ce_bintools import core_parser
 from gp2040ce_bintools.rp2040 import get_bootsel_endpoints, read, write
-from gp2040ce_bintools.storage import (BOARD_CONFIG_BINARY_LOCATION, STORAGE_SIZE, USER_CONFIG_BINARY_LOCATION,
-                                       USER_CONFIG_BOOTSEL_ADDRESS, convert_binary_to_uf2, get_config_from_json,
-                                       pad_config_to_storage_size, serialize_config_with_footer)
 
 logger = logging.getLogger(__name__)
 
 GP2040CE_START_ADDRESS = 0x10000000
 GP2040CE_SIZE = 2 * 1024 * 1024
 
 
@@ -45,18 +44,18 @@
     """
     if not board_config_binary and not user_config_binary:
         raise ValueError("at least one config binary must be provided!")
 
     combined = copy.copy(firmware_binary)
     if board_config_binary:
         combined = (pad_binary_up_to_board_config(combined, or_truncate=replace_extra) +
-                    pad_config_to_storage_size(board_config_binary))
+                    storage.pad_config_to_storage_size(board_config_binary))
     if user_config_binary:
         combined = (pad_binary_up_to_user_config(combined, or_truncate=replace_extra) +
-                    pad_config_to_storage_size(user_config_binary))
+                    storage.pad_config_to_storage_size(user_config_binary))
     return combined
 
 
 def concatenate_firmware_and_storage_files(firmware_filename: str,
                                            binary_board_config_filename: Optional[str] = None,
                                            json_board_config_filename: Optional[str] = None,
                                            binary_user_config_filename: Optional[str] = None,
@@ -75,44 +74,80 @@
         replace_extra: if larger than normal firmware files should have their overage replaced
     """
     new_binary = bytearray([])
     board_config_binary = bytearray([])
     user_config_binary = bytearray([])
 
     if binary_board_config_filename:
-        with open(binary_board_config_filename, 'rb') as storage:
-            board_config_binary = bytearray(storage.read())
+        with open(binary_board_config_filename, 'rb') as binary_file:
+            board_config_binary = bytearray(binary_file.read())
     elif json_board_config_filename:
         with open(json_board_config_filename, 'r') as json_file:
-            config = get_config_from_json(json_file.read())
-            board_config_binary = serialize_config_with_footer(config)
+            config = storage.get_config_from_json(json_file.read())
+            board_config_binary = storage.serialize_config_with_footer(config)
 
     if binary_user_config_filename:
-        with open(binary_user_config_filename, 'rb') as storage:
-            user_config_binary = bytearray(storage.read())
+        with open(binary_user_config_filename, 'rb') as binary_file:
+            user_config_binary = bytearray(binary_file.read())
     elif json_user_config_filename:
         with open(json_user_config_filename, 'r') as json_file:
-            config = get_config_from_json(json_file.read())
-            user_config_binary = serialize_config_with_footer(config)
+            config = storage.get_config_from_json(json_file.read())
+            user_config_binary = storage.serialize_config_with_footer(config)
 
     with open(firmware_filename, 'rb') as firmware:
-        new_binary = combine_firmware_and_config(bytearray(firmware.read()), board_config_binary, user_config_binary,
+        firmware_binary = bytearray(firmware.read())
+
+    # create a sequential binary for .bin and USB uses, or index it for .uf2
+    if usb or combined_filename[-4:] != '.uf2':
+        new_binary = combine_firmware_and_config(firmware_binary, board_config_binary, user_config_binary,
                                                  replace_extra=replace_extra)
+    else:
+        # this was kind of fine, but combining multiple calls of convert_binary_to_uf2 produced
+        # incorrect total block counts in the file, which picotool handled with some squirrely
+        # double-output behavior that has me worried it'd cause a real issue, so doing the
+        # crude padding + write of empty blocks, for now...
+        #
+        # new_binary = convert_binary_to_uf2(firmware_binary)
+        # if board_config_binary:
+        #     new_binary += convert_binary_to_uf2(pad_config_to_storage_size(board_config_binary),
+        #                                         start=BOARD_CONFIG_BINARY_LOCATION)
+        # if user_config_binary:
+        #     new_binary += convert_binary_to_uf2(pad_config_to_storage_size(user_config_binary),
+        #                                         start=USER_CONFIG_BINARY_LOCATION)
+        #
+        # the correct way to do the above would be to pass a list of {offset,binary_data} to convert...,
+        # and have it calculate the total block size before starting to write, and then iterating over
+        # the three lists. doable, just not on the top of my mind right now
+        new_binary = storage.convert_binary_to_uf2(combine_firmware_and_config(firmware_binary, board_config_binary,
+                                                                               user_config_binary,
+                                                                               replace_extra=replace_extra))
 
     if combined_filename:
         with open(combined_filename, 'wb') as combined:
-            if combined_filename[-4:] == '.uf2':
-                combined.write(convert_binary_to_uf2(new_binary))
-            else:
-                combined.write(new_binary)
+            combined.write(new_binary)
+
     if usb:
         endpoint_out, endpoint_in = get_bootsel_endpoints()
         write(endpoint_out, endpoint_in, GP2040CE_START_ADDRESS, bytes(new_binary))
 
 
+def find_version_string_in_binary(binary: bytes) -> str:
+    """Search for a git describe style version string in a binary file.
+
+    Args:
+        binary: the binary to search
+    Returns:
+        the first found string, or None
+    """
+    match = re.search(b'v[0-9]+.[0-9]+.[0-9]+[A-Za-z0-9-+.]*', binary)
+    if match:
+        return match.group(0).decode(encoding='ascii')
+    return 'NONE'
+
+
 def get_gp2040ce_from_usb() -> tuple[bytes, object, object]:
     """Read the firmware + config sections from a USB device.
 
     Returns:
         the bytes from the board, along with the USB out and in endpoints for reference
     """
     # open the USB device and get the config
@@ -153,29 +188,29 @@
         firmware: the firmware binary to process
         or_truncate: if the firmware is longer than expected, just return the max size
     Returns:
         the resulting padded binary as a bytearray
     Raises:
         FirmwareLengthError: if the firmware is larger than the storage location
     """
-    return pad_binary_up_to_address(firmware, BOARD_CONFIG_BINARY_LOCATION, or_truncate)
+    return pad_binary_up_to_address(firmware, storage.BOARD_CONFIG_BINARY_LOCATION, or_truncate)
 
 
 def pad_binary_up_to_user_config(firmware: bytes, or_truncate: bool = False) -> bytearray:
     """Provide a copy of the firmware padded with zero bytes up to the user config position.
 
     Args:
         firmware: the firmware binary to process
         or_truncate: if the firmware is longer than expected, just return the max size
     Returns:
         the resulting padded binary as a bytearray
     Raises:
         FirmwareLengthError: if the firmware is larger than the storage location
     """
-    return pad_binary_up_to_address(firmware, USER_CONFIG_BINARY_LOCATION, or_truncate)
+    return pad_binary_up_to_address(firmware, storage.USER_CONFIG_BINARY_LOCATION, or_truncate)
 
 
 def replace_config_in_binary(board_binary: bytearray, config_binary: bytearray) -> bytearray:
     """Given (presumed) whole board and config binaries, combine the two to one, with proper offsets for GP2040-CE.
 
     Whatever is in the board binary is not sanity checked, and is overwritten. If it is
     too small to be a board dump, it is nonetheless expanded and overwritten to fit the
@@ -183,21 +218,22 @@
 
     Args:
         board_binary: binary data of a whole board dump from a GP2040-CE board
         config_binary: binary data of board config + footer, possibly padded to be a full storage section
     Returns:
         the resulting correctly-offset binary suitable for a GP2040-CE board
     """
-    if len(board_binary) < USER_CONFIG_BINARY_LOCATION + STORAGE_SIZE:
+    if len(board_binary) < storage.USER_CONFIG_BINARY_LOCATION + storage.STORAGE_SIZE:
         # this is functionally the same, since this doesn't sanity check the firmware
         return combine_firmware_and_config(board_binary, bytearray([]), config_binary)
     else:
         new_binary = bytearray(copy.copy(board_binary))
-        new_config = pad_config_to_storage_size(config_binary)
-        new_binary[USER_CONFIG_BINARY_LOCATION:(USER_CONFIG_BINARY_LOCATION + STORAGE_SIZE)] = new_config
+        new_config = storage.pad_config_to_storage_size(config_binary)
+        location_end = storage.USER_CONFIG_BINARY_LOCATION + storage.STORAGE_SIZE
+        new_binary[storage.USER_CONFIG_BINARY_LOCATION:location_end] = new_config
         return new_binary
 
 
 def write_new_config_to_filename(config: Message, filename: str, inject: bool = False) -> None:
     """Serialize the provided config to the specified file.
 
     The file may be replaced, creating a configuration section-only binary, or appended to
@@ -206,50 +242,51 @@
     Args:
         config: the Protobuf configuration to write to disk
         filename: the filename to write the serialized configuration to
         inject: if True, the file is read in and has its storage section replaced; if False,
                 the whole file is replaced
     """
     if inject:
-        config_binary = serialize_config_with_footer(config)
+        config_binary = storage.serialize_config_with_footer(config)
         with open(filename, 'rb') as file:
             existing_binary = file.read()
         binary = replace_config_in_binary(bytearray(existing_binary), config_binary)
         with open(filename, 'wb') as file:
             file.write(binary)
     else:
-        binary = serialize_config_with_footer(config)
+        binary = storage.serialize_config_with_footer(config)
         with open(filename, 'wb') as file:
             if filename[-4:] == '.uf2':
-                file.write(convert_binary_to_uf2(pad_config_to_storage_size(binary),
-                                                 start=USER_CONFIG_BINARY_LOCATION))
+                file.write(storage.convert_binary_to_uf2(storage.pad_config_to_storage_size(binary),
+                                                         start=storage.USER_CONFIG_BINARY_LOCATION))
             else:
                 file.write(binary)
 
 
 def write_new_config_to_usb(config: Message, endpoint_out: object, endpoint_in: object):
     """Serialize the provided config to a device over USB, in the proper location for a GP2040-CE board.
 
     Args:
         config: the Protobuf configuration to write to a RP2040 board in BOOTSEL mode
         endpoint_out: the USB endpoint to write to
         endpoint_in: the USB endpoint to read from
     """
-    serialized = serialize_config_with_footer(config)
+    serialized = storage.serialize_config_with_footer(config)
     # we don't write the whole area, just the minimum from the end of the storage section
     # nevertheless, the USB device needs writes to start at 256 byte boundaries
     logger.debug("serialized: %s", serialized)
     # not sure why this minimal padding isn't working but it leads to corruption
     # maybe claims that erase need to be on 4096 byte sectors?
     # padding = 256 - (len(serialized) % 256)
     padding = 4096 - (len(serialized) % 4096)
     logger.debug("length: %s with %s bytes of padding", len(serialized), padding)
     binary = bytearray(b'\x00' * padding) + serialized
     logger.debug("binary for writing: %s", binary)
-    write(endpoint_out, endpoint_in, USER_CONFIG_BOOTSEL_ADDRESS + (STORAGE_SIZE - len(binary)), bytes(binary))
+    write(endpoint_out, endpoint_in, storage.USER_CONFIG_BOOTSEL_ADDRESS + (storage.STORAGE_SIZE - len(binary)),
+          bytes(binary))
 
 
 ############
 # COMMANDS #
 ############
 
 
@@ -270,23 +307,23 @@
     board_config_group.add_argument('--json-board-config-filename', help=".json file of a GP2040-CE board config")
     user_config_group = parser.add_mutually_exclusive_group(required=False)
     user_config_group.add_argument('--binary-user-config-filename',
                                    help=".bin file of a GP2040-CE user config w/footer")
     user_config_group.add_argument('--json-user-config-filename', help=".json file of a GP2040-CE user config")
     output_group = parser.add_mutually_exclusive_group(required=True)
     output_group.add_argument('--usb', action='store_true', help="write the resulting firmware + storage to USB")
-    output_group.add_argument('--new-binary-filename', help="output .bin file of the resulting firmware + storage")
+    output_group.add_argument('--new-filename', help="output .bin or .uf2 file of the resulting firmware + storage")
 
     args, _ = parser.parse_known_args()
     concatenate_firmware_and_storage_files(args.firmware_filename,
                                            binary_board_config_filename=args.binary_board_config_filename,
                                            json_board_config_filename=args.json_board_config_filename,
                                            binary_user_config_filename=args.binary_user_config_filename,
                                            json_user_config_filename=args.json_user_config_filename,
-                                           combined_filename=args.new_binary_filename, usb=args.usb,
+                                           combined_filename=args.new_filename, usb=args.usb,
                                            replace_extra=args.replace_extra)
 
 
 def dump_gp2040ce():
     """Copy the whole GP2040-CE section off of a BOOTSEL mode board."""
     parser = argparse.ArgumentParser(
         description="Read the GP2040-CE firmware + storage section off of a connected USB RP2040 in BOOTSEL mode.",
@@ -294,7 +331,44 @@
     )
     parser.add_argument('binary_filename', help="output .bin file of the resulting firmware + storage")
 
     args, _ = parser.parse_known_args()
     content, _, _ = get_gp2040ce_from_usb()
     with open(args.binary_filename, 'wb') as out_file:
         out_file.write(content)
+
+
+def summarize_gp2040ce():
+    """Provide information on a dump or USB device."""
+    parser = argparse.ArgumentParser(
+        description="Read a file or USB device to determine what GP2040-CE parts are present.",
+        parents=[core_parser],
+    )
+    input_group = parser.add_mutually_exclusive_group(required=True)
+    input_group.add_argument('--usb', action='store_true', help="inspect the RP2040 device over USB")
+    input_group.add_argument('--filename', help="input .bin or .uf2 file to inspect")
+
+    args, _ = parser.parse_known_args()
+    if args.usb:
+        content, endpoint, _ = get_gp2040ce_from_usb()
+        print(f"USB device {hex(endpoint.device.idVendor)}:{hex(endpoint.device.idProduct)}:\n")
+    else:
+        with open(args.filename, 'rb') as file_:
+            content = file_.read()
+        print(f"File {args.filename}:\n")
+
+    gp2040ce_version = find_version_string_in_binary(content)
+    try:
+        board_config = storage.get_config(storage.get_board_storage_section(bytes(content)))
+        board_config_version = board_config.boardVersion if board_config.boardVersion else "NOT SPECIFIED"
+    except storage.ConfigReadError:
+        board_config_version = "NONE"
+    try:
+        user_config = storage.get_config(storage.get_user_storage_section(bytes(content)))
+        user_config_version = user_config.boardVersion if user_config.boardVersion else "NOT FOUND"
+    except storage.ConfigReadError:
+        user_config_version = "NONE"
+
+    print("GP2040-CE Information")
+    print(f"  detected GP2040-CE version:     {gp2040ce_version}")
+    print(f"  detected board config version:  {board_config_version}")
+    print(f"  detected user config version:   {user_config_version}")
```

### Comparing `gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/config_tree.css` & `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/config_tree.css`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+/**
+ * SPDX-FileCopyrightText: © 2023 Brian S. Stephan <bss@incorporeal.org>
+ * SPDX-License-Identifier: GPL-3.0-or-later
+ */
 Tree {
     padding: 1;
 }
 
 Button {
     border: round gray;
     content-align: center middle;
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/gui.py` & `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,17 +50,15 @@
         elif self.field_descriptor.type in (descriptor.FieldDescriptor.TYPE_INT32,
                                             descriptor.FieldDescriptor.TYPE_INT64,
                                             descriptor.FieldDescriptor.TYPE_UINT32,
                                             descriptor.FieldDescriptor.TYPE_UINT64):
             self.input_field = Input(value=repr(self.field_value), validators=[Number()], id='field-input')
         elif self.field_descriptor.type == descriptor.FieldDescriptor.TYPE_STRING:
             self.input_field = Input(value=self.field_value, id='field-input')
-        else:
-            # we don't handle whatever these are yet
-            self.input_field = Label(repr(self.field_value), id='field-input')
+
         yield Grid(
             Container(Label(self.field_descriptor.full_name, id='field-name'), id='field-name-container'),
             Container(self.input_field, id='input-field-container'),
             Container(Pretty('', id='input-errors', classes='hidden'), id='error-container'),
             Horizontal(Container(Button("Cancel", id='cancel-button'), id='cancel-button-container'),
                        Container(Button("Confirm", id='confirm-button'), id='confirm-button-container'),
                        id='button-container'),
@@ -87,25 +85,24 @@
         if event.button.id == 'confirm-button':
             logger.debug("calling _save")
             self._save()
         self.app.pop_screen()
 
     def _save(self):
         """Save the field value to the retained config item."""
-        if not isinstance(self.input_field, Label):
-            if self.field_descriptor.type in (descriptor.FieldDescriptor.TYPE_INT32,
-                                              descriptor.FieldDescriptor.TYPE_INT64,
-                                              descriptor.FieldDescriptor.TYPE_UINT32,
-                                              descriptor.FieldDescriptor.TYPE_UINT64):
-                field_value = int(self.input_field.value)
-            else:
-                field_value = self.input_field.value
-            setattr(self.parent_config, self.field_descriptor.name, field_value)
-            logger.debug("parent config post-change: %s", self.parent_config)
-            self.node.set_label(pb_field_to_node_label(self.field_descriptor, field_value))
+        if self.field_descriptor.type in (descriptor.FieldDescriptor.TYPE_INT32,
+                                          descriptor.FieldDescriptor.TYPE_INT64,
+                                          descriptor.FieldDescriptor.TYPE_UINT32,
+                                          descriptor.FieldDescriptor.TYPE_UINT64):
+            field_value = int(self.input_field.value)
+        else:
+            field_value = self.input_field.value
+        setattr(self.parent_config, self.field_descriptor.name, field_value)
+        logger.debug("parent config post-change: %s", self.parent_config)
+        self.node.set_label(pb_field_to_node_label(self.field_descriptor, field_value))
 
 
 class MessageScreen(ModalScreen):
     """Simple screen for displaying messages."""
 
     def __init__(self, text: str, *args, **kwargs):
         """Store the message for later display."""
```

### Comparing `gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/config.proto` & `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/config.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/config_pb2.py` & `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/config_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/enums.proto` & `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/enums.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/enums_pb2.py` & `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/enums_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/nanopb.proto` & `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/nanopb.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/proto_snapshot/nanopb_pb2.py` & `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/proto_snapshot/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/rp2040.py` & `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/rp2040.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/gp2040ce_bintools/storage.py` & `gp2040ce_binary_tools-0.8.0/gp2040ce_bintools/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,14 +82,52 @@
                            UF2_FAMILY_ID)                                   # family ID
         uf2 += binary[index:index+256] + bytearray(b'\x00' * pad_count)     # content
         uf2 += struct.pack('<L', UF2_MAGIC_FINAL)                           # final magic number
         index += 256
     return uf2
 
 
+def convert_uf2_to_binary(uf2: bytearray) -> bytearray:
+    """Convert a Microsoft's UF2 payload to a raw binary.
+
+    https://github.com/microsoft/uf2/tree/master#overview
+
+    Args:
+        uf2: bytearray content to convert from a UF2 payload
+    Returns:
+        the content in sequential binary format
+    """
+    if len(uf2) % 512 != 0:
+        raise ValueError(f"provided binary is length {len(uf2)}, which isn't fully divisible by 512!")
+
+    binary = bytearray()
+    old_uf2_addr = None
+
+    for index in range(0, len(uf2), 512):
+        chunk = uf2[index:index+512]
+        _, _, _, uf2_addr, bytes_, block_num, block_count, _ = struct.unpack('<LLLLLLLL', chunk[0:32])
+        content = chunk[32:508]
+        if block_num != index // 512:
+            raise ValueError(f"inconsistent block number in reading UF2, got {block_num}, expected {index // 512}!")
+        if block_count != len(uf2) // 512:
+            raise ValueError(f"inconsistent block count in reading UF2, got {block_count}, expected {len(uf2) // 512}!")
+
+        # the UF2 is indexed, which we could convert to binary with padding 0s, but we don't yet
+        if old_uf2_addr and (uf2_addr != old_uf2_addr + 256):
+            raise ValueError("segmented UF2 files are not yet supported!")
+
+        binary += content[0:bytes_]
+        old_uf2_addr = uf2_addr
+
+    # when this is all done we should have counted the expected number of blocks
+    if block_count != block_num + 1:
+        raise ValueError(f"not all expected blocks ({block_count}) were found, only got {block_num + 1}!")
+    return binary
+
+
 def get_config(content: bytes) -> Message:
     """Read the config from a GP2040-CE storage section.
 
     Args:
         content: bytes from a GP2040-CE board's storage section
     Returns:
         the parsed configuration
@@ -174,15 +212,18 @@
         allow_no_file: if true, attempting to open a nonexistent file returns an empty config, else it errors
         board_config: if true, the board config is provided instead of the user config
     Returns:
         the parsed configuration
     """
     try:
         with open(filename, 'rb') as dump:
-            content = dump.read()
+            if filename[-4:] == '.uf2':
+                content = bytes(convert_uf2_to_binary(bytearray(dump.read())))
+            else:
+                content = dump.read()
     except FileNotFoundError:
         if not allow_no_file:
             raise
         config_pb2 = get_config_pb2()
         return config_pb2.Config()
 
     if whole_board:
@@ -320,18 +361,23 @@
 
 def dump_config():
     """Save the GP2040-CE's user configuration to a binary or UF2 file."""
     parser = argparse.ArgumentParser(
         description="Read the configuration section from a USB device and save it to a binary file.",
         parents=[core_parser],
     )
+    parser.add_argument('--board-config', action='store_true', default=False,
+                        help="dump the board config rather than the user config")
     parser.add_argument('filename', help="file to save the GP2040-CE board's config section to --- if the "
                                          "suffix is .uf2, it is saved in UF2 format, else it is a raw binary")
     args, _ = parser.parse_known_args()
-    config, _, _ = get_user_config_from_usb()
+    if args.board_config:
+        config, _, _ = get_board_config_from_usb()
+    else:
+        config, _, _ = get_user_config_from_usb()
     binary_config = serialize_config_with_footer(config)
     with open(args.filename, 'wb') as out_file:
         if args.filename[-4:] == '.uf2':
             # we must pad to storage start in order for the UF2 write addresses to make sense
             out_file.write(convert_binary_to_uf2(pad_config_to_storage_size(binary_config),
                                                  start=USER_CONFIG_BINARY_LOCATION))
         else:
```

### Comparing `gp2040ce-binary-tools-0.7.0/pyproject.toml` & `gp2040ce_binary_tools-0.8.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gp2040ce-binary-tools"
 description = "Tools for working with GP2040-CE firmware and storage binaries."
 readme = "README.md"
-license = {file = "LICENSE"}
+license = {text = "GPL-3.0-or-later"}
 authors = [
     {name = "Brian S. Stephan", email = "bss@incorporeal.org"},
 ]
 requires-python = ">=3.9"
 dependencies = ["grpcio-tools", "pyusb", "textual"]
 dynamic = ["version"]
 classifiers = [
@@ -26,23 +26,24 @@
 "Changelog" = "https://github.com/OpenStickCommunity/gp2040ce-binary-tools/blob/main/CHANGELOG.md"
 "Bug Tracker" = "https://github.com/OpenStickCommunity/gp2040ce-binary-tools/issues"
 
 
 [project.optional-dependencies]
 dev = ["bandit", "decorator", "flake8", "flake8-blind-except", "flake8-builtins", "flake8-docstrings",
        "flake8-executable", "flake8-fixme", "flake8-isort", "flake8-logging-format", "flake8-mutable",
-       "flake8-pyproject", "mypy", "pip-tools", "pytest", "pytest-asyncio", "pytest-cov", "setuptools-scm",
-       "textual-dev", "tox"]
+       "flake8-pyproject", "mypy", "pip-tools", "pytest", "pytest-asyncio", "pytest-cov", "reuse",
+       "setuptools-scm", "textual-dev", "tox"]
 
 [project.scripts]
 concatenate = "gp2040ce_bintools.builder:concatenate"
 dump-config = "gp2040ce_bintools.storage:dump_config"
 dump-gp2040ce = "gp2040ce_bintools.builder:dump_gp2040ce"
 edit-config = "gp2040ce_bintools.gui:edit_config"
-visualize-storage = "gp2040ce_bintools.storage:visualize"
+summarize-gp2040ce = "gp2040ce_bintools.builder:summarize_gp2040ce"
+visualize-config = "gp2040ce_bintools.storage:visualize"
 
 [tool.flake8]
 enable-extensions = "G,M"
 exclude = [".tox/", "venv/", "_version.py", "tests/test-files/", "config_pb2.py", "enums_pb2.py", "nanopb_pb2.py"]
 extend-ignore = "T101"
 max-complexity = 10
 max-line-length = 120
@@ -69,9 +70,15 @@
 [[tool.mypy.overrides]]
 module = "gp2040ce_bintools.gui"
 ignore_errors = true
 
 [tool.pytest]
 python_files = ["*_tests.py", "tests.py", "test_*.py"]
 
+[tool.setuptools]
+packages = [
+    "gp2040ce_bintools",
+    "gp2040ce_bintools.proto_snapshot",
+]
+
 [tool.setuptools_scm]
 write_to = "gp2040ce_bintools/_version.py"
```

### Comparing `gp2040ce-binary-tools-0.7.0/requirements/requirements-dev.txt` & `gp2040ce_binary_tools-0.8.0/requirements/requirements-dev.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,29 @@
     # via textual-dev
 aiosignal==1.3.1
     # via aiohttp
 attrs==23.2.0
     # via aiohttp
 bandit==1.7.8
     # via gp2040ce-binary-tools (pyproject.toml)
+binaryornot==0.4.4
+    # via reuse
+boolean-py==4.0
+    # via
+    #   license-expression
+    #   reuse
 build==1.2.1
     # via pip-tools
 cachetools==5.3.3
     # via tox
 chardet==5.2.0
-    # via tox
+    # via
+    #   binaryornot
+    #   python-debian
+    #   tox
 click==8.1.7
     # via
     #   pip-tools
     #   textual-dev
 colorama==0.4.6
     # via tox
 coverage[toml]==7.4.4
@@ -71,21 +80,27 @@
     # via gp2040ce-binary-tools (pyproject.toml)
 idna==3.6
     # via yarl
 iniconfig==2.0.0
     # via pytest
 isort==5.13.2
     # via flake8-isort
+jinja2==3.1.3
+    # via reuse
+license-expression==30.3.0
+    # via reuse
 linkify-it-py==2.0.3
     # via markdown-it-py
 markdown-it-py[linkify,plugins]==3.0.0
     # via
     #   mdit-py-plugins
     #   rich
     #   textual
+markupsafe==2.1.5
+    # via jinja2
 mccabe==0.7.0
     # via flake8
 mdit-py-plugins==0.4.0
     # via markdown-it-py
 mdurl==0.1.2
     # via markdown-it-py
 msgpack==1.0.8
@@ -138,18 +153,22 @@
     #   gp2040ce-binary-tools (pyproject.toml)
     #   pytest-asyncio
     #   pytest-cov
 pytest-asyncio==0.23.6
     # via gp2040ce-binary-tools (pyproject.toml)
 pytest-cov==5.0.0
     # via gp2040ce-binary-tools (pyproject.toml)
+python-debian==0.1.49
+    # via reuse
 pyusb==1.2.1
     # via gp2040ce-binary-tools (pyproject.toml)
 pyyaml==6.0.1
     # via bandit
+reuse==3.0.2
+    # via gp2040ce-binary-tools (pyproject.toml)
 rich==13.7.1
     # via
     #   bandit
     #   textual
 setuptools-scm==8.0.4
     # via gp2040ce-binary-tools (pyproject.toml)
 snowballstemmer==2.2.0
```

### Comparing `gp2040ce-binary-tools-0.7.0/requirements/requirements.txt` & `gp2040ce_binary_tools-0.8.0/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/tests/conftest.py` & `gp2040ce_binary_tools-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/tests/test-files/pb2-files/config_pb2.py` & `gp2040ce_binary_tools-0.8.0/tests/test-files/pb2-files/config_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/tests/test-files/pb2-files/enums_pb2.py` & `gp2040ce_binary_tools-0.8.0/tests/test-files/pb2-files/enums_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/tests/test-files/pb2-files/nanopb_pb2.py` & `gp2040ce_binary_tools-0.8.0/tests/test-files/pb2-files/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/tests/test-files/proto-files/config.proto` & `gp2040ce_binary_tools-0.8.0/tests/test-files/proto-files/config.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/tests/test-files/proto-files/enums.proto` & `gp2040ce_binary_tools-0.8.0/tests/test-files/proto-files/enums.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/tests/test-files/proto-files/nanopb.proto` & `gp2040ce_binary_tools-0.8.0/tests/test-files/proto-files/nanopb.proto`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/tests/test-files/test-binary-source-of-json-config.bin` & `gp2040ce_binary_tools-0.8.0/tests/test-files/test-binary-source-of-json-config.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/tests/test-files/test-config.bin` & `gp2040ce_binary_tools-0.8.0/tests/test-files/test-config.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/tests/test-files/test-config.json` & `gp2040ce_binary_tools-0.8.0/tests/test-files/test-config.json`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/tests/test-files/test-firmware.bin` & `gp2040ce_binary_tools-0.8.0/tests/test-files/test-firmware.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/tests/test-files/test-storage-area.bin` & `gp2040ce_binary_tools-0.8.0/tests/test-files/test-storage-area.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/tests/test-files/test-whole-board-with-board-config.bin` & `gp2040ce_binary_tools-0.8.0/tests/test-files/test-whole-board-with-board-config.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/tests/test-files/test-whole-board.bin` & `gp2040ce_binary_tools-0.8.0/tests/test-files/test-whole-board.bin`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/tests/test_builder.py` & `gp2040ce_binary_tools-0.8.0/tests/test_builder.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,19 +6,16 @@
 import os
 import sys
 import unittest.mock as mock
 
 import pytest
 from decorator import decorator
 
+import gp2040ce_bintools.builder as builder
 from gp2040ce_bintools import get_config_pb2
-from gp2040ce_bintools.builder import (FirmwareLengthError, combine_firmware_and_config,
-                                       concatenate_firmware_and_storage_files, get_gp2040ce_from_usb,
-                                       pad_binary_up_to_board_config, pad_binary_up_to_user_config,
-                                       replace_config_in_binary, write_new_config_to_filename, write_new_config_to_usb)
 from gp2040ce_bintools.storage import (STORAGE_SIZE, get_board_storage_section, get_config, get_config_footer,
                                        get_user_storage_section, serialize_config_with_footer)
 
 HERE = os.path.dirname(os.path.abspath(__file__))
 
 
 @decorator
@@ -34,40 +31,40 @@
 
 
 def test_concatenate_to_file(tmp_path):
     """Test that we write a file with firmware + binary user config as expected."""
     tmp_file = os.path.join(tmp_path, 'concat.bin')
     firmware_file = os.path.join(HERE, 'test-files', 'test-firmware.bin')
     config_file = os.path.join(HERE, 'test-files', 'test-config.bin')
-    concatenate_firmware_and_storage_files(firmware_file, binary_user_config_filename=config_file,
-                                           combined_filename=tmp_file)
+    builder.concatenate_firmware_and_storage_files(firmware_file, binary_user_config_filename=config_file,
+                                                   combined_filename=tmp_file)
     with open(tmp_file, 'rb') as file:
         content = file.read()
     assert len(content) == 2 * 1024 * 1024
 
 
 def test_concatenate_board_config_to_file(tmp_path):
     """Test that we write a file with firmware + binary board config as expected."""
     tmp_file = os.path.join(tmp_path, 'concat.bin')
     firmware_file = os.path.join(HERE, 'test-files', 'test-firmware.bin')
     config_file = os.path.join(HERE, 'test-files', 'test-config.bin')
-    concatenate_firmware_and_storage_files(firmware_file, binary_board_config_filename=config_file,
-                                           combined_filename=tmp_file)
+    builder.concatenate_firmware_and_storage_files(firmware_file, binary_board_config_filename=config_file,
+                                                   combined_filename=tmp_file)
     with open(tmp_file, 'rb') as file:
         content = file.read()
     assert len(content) == (2 * 1024 * 1024) - (16 * 1024)
 
 
 def test_concatenate_both_configs_to_file(tmp_path):
     """Test that we write a file with firmware + binary board + binary user config as expected."""
     tmp_file = os.path.join(tmp_path, 'concat.bin')
     firmware_file = os.path.join(HERE, 'test-files', 'test-firmware.bin')
     config_file = os.path.join(HERE, 'test-files', 'test-config.bin')
-    concatenate_firmware_and_storage_files(firmware_file, binary_board_config_filename=config_file,
-                                           binary_user_config_filename=config_file, combined_filename=tmp_file)
+    builder.concatenate_firmware_and_storage_files(firmware_file, binary_board_config_filename=config_file,
+                                                   binary_user_config_filename=config_file, combined_filename=tmp_file)
     with open(tmp_file, 'rb') as file:
         content = file.read()
     assert len(content) == 2 * 1024 * 1024
     storage = get_board_storage_section(content)
     footer_size, _, _ = get_config_footer(storage)
     assert footer_size == 3309
     storage = get_user_storage_section(content)
@@ -77,142 +74,179 @@
 
 @with_pb2s
 def test_concatenate_user_json_to_file(tmp_path):
     """Test that we write a file with firmware + JSON user config as expected."""
     tmp_file = os.path.join(tmp_path, 'concat.bin')
     firmware_file = os.path.join(HERE, 'test-files', 'test-firmware.bin')
     config_file = os.path.join(HERE, 'test-files', 'test-config.json')
-    concatenate_firmware_and_storage_files(firmware_file, json_user_config_filename=config_file,
-                                           combined_filename=tmp_file)
+    builder.concatenate_firmware_and_storage_files(firmware_file, json_user_config_filename=config_file,
+                                                   combined_filename=tmp_file)
     with open(tmp_file, 'rb') as file:
         content = file.read()
     assert len(content) == 2 * 1024 * 1024
 
 
 def test_concatenate_to_file_incomplete_args_is_error(tmp_path):
     """Test that we bail properly if we weren't given all the necessary arguments to make a binary."""
     tmp_file = os.path.join(tmp_path, 'concat.bin')
     firmware_file = os.path.join(HERE, 'test-files', 'test-firmware.bin')
     with pytest.raises(ValueError):
-        concatenate_firmware_and_storage_files(firmware_file, combined_filename=tmp_file)
+        builder.concatenate_firmware_and_storage_files(firmware_file, combined_filename=tmp_file)
 
 
 def test_concatenate_to_usb(tmp_path):
     """Test that we write a file as expected."""
     firmware_file = os.path.join(HERE, 'test-files', 'test-firmware.bin')
     config_file = os.path.join(HERE, 'test-files', 'test-config.bin')
     end_out, end_in = mock.MagicMock(), mock.MagicMock()
     with mock.patch('gp2040ce_bintools.builder.get_bootsel_endpoints', return_value=(end_out, end_in)):
         with mock.patch('gp2040ce_bintools.builder.write') as mock_write:
-            concatenate_firmware_and_storage_files(firmware_file, binary_user_config_filename=config_file,
-                                                   usb=True)
+            builder.concatenate_firmware_and_storage_files(firmware_file, binary_user_config_filename=config_file,
+                                                           usb=True)
 
     assert mock_write.call_args.args[2] == 0x10000000
     assert len(mock_write.call_args.args[3]) == 2 * 1024 * 1024
 
 
+def test_concatenate_to_uf2(tmp_path, firmware_binary, config_binary):
+    """Test that we write a UF2 file as expected."""
+    tmp_file = os.path.join(tmp_path, 'concat.uf2')
+    firmware_file = os.path.join(HERE, 'test-files', 'test-firmware.bin')
+    config_file = os.path.join(HERE, 'test-files', 'test-config.bin')
+    builder.concatenate_firmware_and_storage_files(firmware_file, binary_board_config_filename=config_file,
+                                                   binary_user_config_filename=config_file,
+                                                   combined_filename=tmp_file)
+    with open(tmp_file, 'rb') as file:
+        content = file.read()
+    # size of the file should be 2x the binary version, and the binary is 2 MB
+    assert len(content) == 2 * 2 * 1024 * 1024
+
+
+def test_concatenate_to_uf2_board_only(tmp_path, firmware_binary, config_binary):
+    """Test that we write a UF2 file as expected."""
+    tmp_file = os.path.join(tmp_path, 'concat.uf2')
+    firmware_file = os.path.join(HERE, 'test-files', 'test-firmware.bin')
+    config_file = os.path.join(HERE, 'test-files', 'test-config.bin')
+    builder.concatenate_firmware_and_storage_files(firmware_file, binary_board_config_filename=config_file,
+                                                   combined_filename=tmp_file)
+    with open(tmp_file, 'rb') as file:
+        content = file.read()
+    # size of the file should be 2x the binary version (minus user config space), and the binary is 2 MB - 16KB
+    assert len(content) == 2 * (2 * 1024 * 1024 - 16384)
+
+
+def test_find_version_string(firmware_binary):
+    """Test that we can find a version string in a binary."""
+    assert builder.find_version_string_in_binary(firmware_binary) == 'v0.7.5'
+
+
+def test_dont_always_find_version_string(firmware_binary):
+    """Test that we can find a version string in a binary."""
+    assert builder.find_version_string_in_binary(b'\x00') == 'NONE'
+
+
 def test_padding_firmware(firmware_binary):
     """Test that firmware is padded to the expected size."""
-    padded = pad_binary_up_to_user_config(firmware_binary)
+    padded = builder.pad_binary_up_to_user_config(firmware_binary)
     assert len(padded) == 2080768
 
 
 def test_padding_firmware_can_truncate():
     """Test that firmware is padded to the expected size."""
-    padded = pad_binary_up_to_user_config(bytearray(b'\x00' * 4 * 1024 * 1024), or_truncate=True)
+    padded = builder.pad_binary_up_to_user_config(bytearray(b'\x00' * 4 * 1024 * 1024), or_truncate=True)
     assert len(padded) == 2080768
 
 
 def test_padding_firmware_to_board(firmware_binary):
     """Test that firmware is padded to the expected size."""
-    padded = pad_binary_up_to_board_config(firmware_binary)
+    padded = builder.pad_binary_up_to_board_config(firmware_binary)
     assert len(padded) == 2080768 - (16 * 1024)
 
 
 def test_firmware_plus_storage_section(firmware_binary, storage_dump):
     """Test that combining firmware and storage produces a valid combined binary."""
-    whole_board = combine_firmware_and_config(firmware_binary, None, storage_dump)
+    whole_board = builder.combine_firmware_and_config(firmware_binary, None, storage_dump)
     # if this is valid, we should be able to find the storage and footer again
     storage = get_user_storage_section(whole_board)
     footer_size, _, _ = get_config_footer(storage)
     assert footer_size == 3309
 
 
 def test_firmware_plus_user_config_binary(firmware_binary, config_binary):
     """Test that combining firmware and user config produces a valid combined binary."""
-    whole_board = combine_firmware_and_config(firmware_binary, None, config_binary)
+    whole_board = builder.combine_firmware_and_config(firmware_binary, None, config_binary)
     # if this is valid, we should be able to find the storage and footer again
     storage = get_user_storage_section(whole_board)
     footer_size, _, _ = get_config_footer(storage)
     assert footer_size == 3309
 
 
 def test_chunky_firmware_plus_user_config_binary(config_binary):
     """Test that combining giant firmware and storage produces a valid combined binary."""
-    whole_board = combine_firmware_and_config(bytearray(b'\x00' * 4 * 1024 * 1024), None, config_binary,
-                                              replace_extra=True)
+    whole_board = builder.combine_firmware_and_config(bytearray(b'\x00' * 4 * 1024 * 1024), None, config_binary,
+                                                      replace_extra=True)
     # if this is valid, we should be able to find the storage and footer again
     storage = get_user_storage_section(whole_board)
     footer_size, _, _ = get_config_footer(storage)
     assert footer_size == 3309
 
 
 def test_firmware_plus_board_config_binary(firmware_binary, config_binary):
     """Test that combining firmware and board config produces a valid combined binary."""
-    almost_whole_board = combine_firmware_and_config(firmware_binary, config_binary, None)
+    almost_whole_board = builder.combine_firmware_and_config(firmware_binary, config_binary, None)
     assert len(almost_whole_board) == (2 * 1024 * 1024) - (16 * 1024)
     # if this is valid, we should be able to find the storage and footer again
     storage = get_board_storage_section(almost_whole_board)
     footer_size, _, _ = get_config_footer(storage)
     assert footer_size == 3309
 
 
 def test_firmware_plus_board_and_user_config_binary(firmware_binary, config_binary):
     """Test that combining firmware and both board and user configs produces a valid combined binary."""
-    whole_board = combine_firmware_and_config(firmware_binary, config_binary, config_binary)
+    whole_board = builder.combine_firmware_and_config(firmware_binary, config_binary, config_binary)
     assert len(whole_board) == 2 * 1024 * 1024
     # if this is valid, we should be able to find the storage and footer again
     storage = get_board_storage_section(whole_board)
     footer_size, _, _ = get_config_footer(storage)
     assert footer_size == 3309
     storage = get_user_storage_section(whole_board)
     footer_size, _, _ = get_config_footer(storage)
     assert footer_size == 3309
 
 
 def test_combine_must_get_at_least_one_config(firmware_binary):
     """Test that we error if we are asked to combine with nothing to combine."""
     with pytest.raises(ValueError):
-        combine_firmware_and_config(firmware_binary, None, None)
+        builder.combine_firmware_and_config(firmware_binary, None, None)
 
 
 def test_replace_config_in_binary(config_binary):
     """Test that a config binary is placed in the storage location of a source binary to overwrite."""
-    whole_board = replace_config_in_binary(bytearray(b'\x00' * 3 * 1024 * 1024), config_binary)
+    whole_board = builder.replace_config_in_binary(bytearray(b'\x00' * 3 * 1024 * 1024), config_binary)
     assert len(whole_board) == 3 * 1024 * 1024
     # if this is valid, we should be able to find the storage and footer again
     storage = get_user_storage_section(whole_board)
     footer_size, _, _ = get_config_footer(storage)
     assert footer_size == 3309
 
 
 def test_replace_config_in_binary_not_big_enough(config_binary):
     """Test that a config binary is placed in the storage location of a source binary to pad."""
-    whole_board = replace_config_in_binary(bytearray(b'\x00' * 1 * 1024 * 1024), config_binary)
+    whole_board = builder.replace_config_in_binary(bytearray(b'\x00' * 1 * 1024 * 1024), config_binary)
     assert len(whole_board) == 2 * 1024 * 1024
     # if this is valid, we should be able to find the storage and footer again
     storage = get_user_storage_section(whole_board)
     footer_size, _, _ = get_config_footer(storage)
     assert footer_size == 3309
 
 
 def test_padding_firmware_too_big(firmware_binary):
     """Test that firmware is padded to the expected size."""
-    with pytest.raises(FirmwareLengthError):
-        _ = pad_binary_up_to_user_config(firmware_binary + firmware_binary + firmware_binary)
+    with pytest.raises(builder.FirmwareLengthError):
+        _ = builder.pad_binary_up_to_user_config(firmware_binary + firmware_binary + firmware_binary)
 
 
 @with_pb2s
 def test_write_new_config_to_whole_board(whole_board_dump, tmp_path):
     """Test that the config can be overwritten on a whole board dump."""
     tmp_file = os.path.join(tmp_path, 'whole-board-dump-copy.bin')
     with open(tmp_file, 'wb') as file:
@@ -220,15 +254,15 @@
     # reread just in case
     with open(tmp_file, 'rb') as file:
         board_dump = file.read()
 
     config = get_config(get_user_storage_section(board_dump))
     assert config.boardVersion == 'v0.7.5'
     config.boardVersion = 'v0.7.5-COOL'
-    write_new_config_to_filename(config, tmp_file, inject=True)
+    builder.write_new_config_to_filename(config, tmp_file, inject=True)
 
     # read new file
     with open(tmp_file, 'rb') as file:
         new_board_dump = file.read()
     config = get_config(get_user_storage_section(new_board_dump))
     assert config.boardVersion == 'v0.7.5-COOL'
     assert len(board_dump) == len(new_board_dump)
@@ -240,15 +274,15 @@
     tmp_file = os.path.join(tmp_path, 'firmware-copy.bin')
     with open(tmp_file, 'wb') as file:
         file.write(firmware_binary)
 
     config_pb2 = get_config_pb2()
     config = config_pb2.Config()
     config.boardVersion = 'v0.7.5-COOL'
-    write_new_config_to_filename(config, tmp_file, inject=True)
+    builder.write_new_config_to_filename(config, tmp_file, inject=True)
 
     # read new file
     with open(tmp_file, 'rb') as file:
         new_board_dump = file.read()
     config = get_config(get_user_storage_section(new_board_dump))
     assert config.boardVersion == 'v0.7.5-COOL'
     assert len(new_board_dump) == 2 * 1024 * 1024
@@ -257,15 +291,15 @@
 @with_pb2s
 def test_write_new_config_to_config_bin(firmware_binary, tmp_path):
     """Test that the config can be written to a file."""
     tmp_file = os.path.join(tmp_path, 'config.bin')
     config_pb2 = get_config_pb2()
     config = config_pb2.Config()
     config.boardVersion = 'v0.7.5-COOL'
-    write_new_config_to_filename(config, tmp_file)
+    builder.write_new_config_to_filename(config, tmp_file)
 
     # read new file
     with open(tmp_file, 'rb') as file:
         config_dump = file.read()
     config = get_config(config_dump)
     config_size, _, _ = get_config_footer(config_dump)
     assert config.boardVersion == 'v0.7.5-COOL'
@@ -275,15 +309,15 @@
 @with_pb2s
 def test_write_new_config_to_config_uf2(firmware_binary, tmp_path):
     """Test that the config can be written to a file."""
     tmp_file = os.path.join(tmp_path, 'config.uf2')
     config_pb2 = get_config_pb2()
     config = config_pb2.Config()
     config.boardVersion = 'v0.7.5-COOL'
-    write_new_config_to_filename(config, tmp_file)
+    builder.write_new_config_to_filename(config, tmp_file)
 
     # read new file
     with open(tmp_file, 'rb') as file:
         config_dump = file.read()
     # the current implementation of UF2 writing does it in 256 blocks, so each 256 byte block of
     # binary is 512 bytes in the UF2
     assert len(config_dump) == STORAGE_SIZE * 2
@@ -292,15 +326,15 @@
 @with_pb2s
 def test_write_new_config_to_usb(config_binary):
     """Test that the config can be written to USB at the proper alignment."""
     config = get_config(config_binary)
     serialized = serialize_config_with_footer(config)
     end_out, end_in = mock.MagicMock(), mock.MagicMock()
     with mock.patch('gp2040ce_bintools.builder.write') as mock_write:
-        write_new_config_to_usb(config, end_out, end_in)
+        builder.write_new_config_to_usb(config, end_out, end_in)
 
     # check that it got padded
     assert len(serialized) == 3321
     padded_serialized = bytearray(b'\x00' * 775) + serialized
     assert mock_write.call_args.args[2] % 4096 == 0
     assert mock_write.call_args.args[3] == padded_serialized
 
@@ -311,11 +345,11 @@
     mock_out.device.idVendor = 0xbeef
     mock_out.device.idProduct = 0xcafe
     mock_out.device.bus = 1
     mock_out.device.address = 2
     mock_in = mock.MagicMock()
     with mock.patch('gp2040ce_bintools.builder.get_bootsel_endpoints', return_value=(mock_out, mock_in)) as mock_get:
         with mock.patch('gp2040ce_bintools.builder.read') as mock_read:
-            config, _, _ = get_gp2040ce_from_usb()
+            config, _, _ = builder.get_gp2040ce_from_usb()
 
     mock_get.assert_called_once()
     mock_read.assert_called_with(mock_out, mock_in, 0x10000000, 2 * 1024 * 1024)
```

### Comparing `gp2040ce-binary-tools-0.7.0/tests/test_commands.py` & `gp2040ce_binary_tools-0.8.0/tests/test_commands.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,66 +25,73 @@
 
     sys.path.pop()
     del sys.modules['config_pb2']
 
 
 def test_version_flag():
     """Test that tools report the version."""
-    result = run(['visualize-storage', '-v'], capture_output=True, encoding='utf8')
+    result = run(['visualize-config', '-v'], capture_output=True, encoding='utf8')
     assert __version__ in result.stdout
 
 
 def test_help_flag():
     """Test that tools report the usage information."""
-    result = run(['visualize-storage', '-h'], capture_output=True, encoding='utf8')
-    assert 'usage: visualize-storage' in result.stdout
+    result = run(['visualize-config', '-h'], capture_output=True, encoding='utf8')
+    assert 'usage: visualize-config' in result.stdout
     assert 'Read the configuration section from a dump of a GP2040-CE board' in result.stdout
 
 
 def test_concatenate_invocation(tmpdir):
     """Test that a normal invocation against a dump works."""
     out_filename = os.path.join(tmpdir, 'out.bin')
     _ = run(['concatenate', 'tests/test-files/test-firmware.bin', '--binary-user-config-filename',
-             'tests/test-files/test-storage-area.bin', '--new-binary-filename', out_filename])
+             'tests/test-files/test-storage-area.bin', '--new-filename', out_filename])
     with open(out_filename, 'rb') as out_file, open('tests/test-files/test-storage-area.bin', 'rb') as storage_file:
         out = out_file.read()
         storage = storage_file.read()
     assert out[2080768:2097152] == storage
 
 
 def test_concatenate_invocation_json(tmpdir):
     """Test that a normal invocation with a firmware and a JSON file works."""
     out_filename = os.path.join(tmpdir, 'out.bin')
     _ = run(['concatenate', '-P', 'tests/test-files/proto-files', 'tests/test-files/test-firmware.bin',
-             '--json-user-config-filename', 'tests/test-files/test-config.json', '--new-binary-filename',
+             '--json-user-config-filename', 'tests/test-files/test-config.json', '--new-filename',
              out_filename])
     with open(out_filename, 'rb') as out_file, open('tests/test-files/test-binary-source-of-json-config.bin',
                                                     'rb') as storage_file:
         out = out_file.read()
         storage = storage_file.read()
     assert out[2093382:2097152] == storage
 
 
+def test_summarize_invocation(tmpdir):
+    """Test that we can get some summary information."""
+    result = run(['summarize-gp2040ce', '--filename', 'tests/test-files/test-firmware.bin'],
+                 capture_output=True, encoding='utf8')
+    assert 'detected GP2040-CE version:     v0.7.5' in result.stdout
+
+
 def test_storage_dump_invocation():
     """Test that a normal invocation against a dump works."""
-    result = run(['visualize-storage', '-P', 'tests/test-files/proto-files',
+    result = run(['visualize-config', '-P', 'tests/test-files/proto-files',
                   '--filename', 'tests/test-files/test-storage-area.bin'],
                  capture_output=True, encoding='utf8')
     assert 'boardVersion: "v0.7.5"' in result.stdout
 
 
 def test_debug_storage_dump_invocation():
     """Test that a normal invocation against a dump works."""
-    result = run(['visualize-storage', '-d', '-P', 'tests/test-files/proto-files',
+    result = run(['visualize-config', '-d', '-P', 'tests/test-files/proto-files',
                   '--filename', 'tests/test-files/test-storage-area.bin'],
                  capture_output=True, encoding='utf8')
     assert 'boardVersion: "v0.7.5"' in result.stdout
     assert 'length of content to look for footer in: 16384' in result.stderr
 
 
 def test_storage_dump_json_invocation():
     """Test that a normal invocation against a dump works."""
-    result = run(['visualize-storage', '-P', 'tests/test-files/proto-files', '--json',
+    result = run(['visualize-config', '-P', 'tests/test-files/proto-files', '--json',
                   '--filename', 'tests/test-files/test-storage-area.bin'],
                  capture_output=True, encoding='utf8')
     to_dict = json.loads(result.stdout)
     assert to_dict['boardVersion'] == 'v0.7.5'
```

### Comparing `gp2040ce-binary-tools-0.7.0/tests/test_gui.py` & `gp2040ce_binary_tools-0.8.0/tests/test_gui.py`

 * *Files 9% similar despite different names*

```diff
@@ -123,14 +123,49 @@
         await pilot.wait_for_scheduled_animations()
         await pilot.click('Button#confirm-button')
         assert pilot.app.config.displayOptions.deprecatedI2cSpeed == 5
 
 
 @pytest.mark.asyncio
 @with_pb2s
+async def test_cancel_simple_edit_via_input_field():
+    """Test that we can cancel out of saving an int via UI and see it reflected in the config."""
+    app = ConfigEditor(config_filename=os.path.join(HERE, 'test-files/test-config.bin'))
+    async with app.run_test() as pilot:
+        tree = pilot.app.query_one(Tree)
+        display_node = tree.root.children[5]
+        i2cspeed_node = display_node.children[4]
+        assert pilot.app.config.displayOptions.deprecatedI2cSpeed == 400000
+
+        tree.root.expand_all()
+        await pilot.wait_for_scheduled_animations()
+        tree.select_node(i2cspeed_node)
+        tree.action_select_cursor()
+        await pilot.wait_for_scheduled_animations()
+        await pilot.click('Input#field-input')
+        await pilot.wait_for_scheduled_animations()
+        await pilot.press('backspace', 'backspace', 'backspace', 'backspace', 'backspace', 'backspace', '5')
+        await pilot.wait_for_scheduled_animations()
+        await pilot.click('Button#cancel-button')
+        assert pilot.app.config.displayOptions.deprecatedI2cSpeed == 400000
+
+
+@pytest.mark.asyncio
+@with_pb2s
+async def test_about():
+    """Test that we can bring up the about box."""
+    app = ConfigEditor(config_filename=os.path.join(HERE, 'test-files/test-config.bin'))
+    async with app.run_test() as pilot:
+        await pilot.press('?')
+        await pilot.wait_for_scheduled_animations()
+        await pilot.click('Button#ok-button')
+
+
+@pytest.mark.asyncio
+@with_pb2s
 async def test_simple_edit_via_input_field_enum():
     """Test that we can change an enum via the UI and see it reflected in the config."""
     app = ConfigEditor(config_filename=os.path.join(HERE, 'test-files/test-config.bin'))
     async with app.run_test() as pilot:
         tree = pilot.app.query_one(Tree)
         gamepad_node = tree.root.children[7]
         dpadmode_node = gamepad_node.children[0]
```

### Comparing `gp2040ce-binary-tools-0.7.0/tests/test_package.py` & `gp2040ce_binary_tools-0.8.0/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/tests/test_rp2040.py` & `gp2040ce_binary_tools-0.8.0/tests/test_rp2040.py`

 * *Files identical despite different names*

### Comparing `gp2040ce-binary-tools-0.7.0/tests/test_storage.py` & `gp2040ce_binary_tools-0.8.0/tests/test_storage.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Unit tests for the storage module.
 
 SPDX-FileCopyrightText: © 2023 Brian S. Stephan <bss@incorporeal.org>
 SPDX-License-Identifier: GPL-3.0-or-later
 """
+import math
 import os
 import sys
 import unittest.mock as mock
 
 import pytest
 from decorator import decorator
 
@@ -135,23 +136,61 @@
     uf2 = storage.convert_binary_to_uf2(whole_board_with_board_config_dump)
     assert len(uf2) == 4194304                              # binary is 8192 256 byte chunks, UF2 is 512 b per chunk
     assert uf2[0:4] == b'\x55\x46\x32\x0a' == b'UF2\n'      # proper magic
     assert uf2[8:12] == bytearray(b'\x00\x20\x00\x00')      # family ID set
     assert uf2[524:528] == bytearray(b'\x00\x01\x00\x10')   # address to write the second chunk
 
 
+def test_convert_unaligned_binary_to_uf2(firmware_binary):
+    """Do some sanity checks in the attempt to convert a binary to a UF2."""
+    uf2 = storage.convert_binary_to_uf2(firmware_binary)
+    assert len(uf2) == math.ceil(len(firmware_binary)/256) * 512    # 256 byte complete/partial chunks -> 512 b chunks
+    assert uf2[0:4] == b'\x55\x46\x32\x0a' == b'UF2\n'      # proper magic
+    assert uf2[8:12] == bytearray(b'\x00\x20\x00\x00')      # family ID set
+    assert uf2[524:528] == bytearray(b'\x00\x01\x00\x10')   # address to write the second chunk
+
+
 def test_convert_binary_to_uf2_with_offsets(whole_board_with_board_config_dump):
     """Do some sanity checks in the attempt to convert a binary to a UF2."""
     uf2 = storage.convert_binary_to_uf2(whole_board_with_board_config_dump, start=storage.USER_CONFIG_BINARY_LOCATION)
     assert len(uf2) == 4194304                              # binary is 8192 256 byte chunks, UF2 is 512 b per chunk
     assert uf2[0:4] == b'\x55\x46\x32\x0a' == b'UF2\n'      # proper magic
     assert uf2[8:12] == bytearray(b'\x00\x20\x00\x00')      # family ID set
     assert uf2[524:528] == bytearray(b'\x00\xc1\x1f\x10')   # address to write the second chunk
 
 
+def test_convert_binary_to_uf2_to_binary(whole_board_with_board_config_dump):
+    """Do some sanity checks in the attempt to convert a binary to a UF2."""
+    uf2 = storage.convert_binary_to_uf2(whole_board_with_board_config_dump)
+    binary = storage.convert_uf2_to_binary(uf2)
+    assert len(binary) == 2097152
+    assert whole_board_with_board_config_dump == binary
+
+
+def test_malformed_uf2(whole_board_with_board_config_dump):
+    """Check that we expect a properly-formed UF2."""
+    uf2 = storage.convert_binary_to_uf2(whole_board_with_board_config_dump)
+
+    # truncated UF2 --- byte mismatch
+    with pytest.raises(ValueError):
+        storage.convert_uf2_to_binary(uf2[:-4])
+
+    # truncated uf2 --- counter is wrong
+    with pytest.raises(ValueError):
+        storage.convert_uf2_to_binary(uf2[512:])
+
+    # truncated uf2 --- total count is wrong
+    with pytest.raises(ValueError):
+        storage.convert_uf2_to_binary(uf2[:-512])
+
+    # malformed UF2 --- counter jumps in the middle, suggests total blocks is wrong
+    with pytest.raises(ValueError):
+        storage.convert_uf2_to_binary(uf2 + uf2)
+
+
 @with_pb2s
 def test_serialize_config_with_footer(storage_dump, config_binary):
     """Test that reserializing a read in config matches the original.
 
     Note that this isn't going to produce an *identical* result, because new message fields
     may have default values that get saved in the reserialized binary, so we can still only test
     some particular parts. But it should work.
```

### Comparing `gp2040ce-binary-tools-0.7.0/tox.ini` & `gp2040ce_binary_tools-0.8.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # tox (https://tox.readthedocs.io/) is a tool for running tests
 # in multiple virtualenvs. This configuration file will run the
 # test suite on all supported python versions. To use it, "pip install tox"
 # and then run "tox" from this directory.
 
 [tox]
 isolated_build = true
-envlist = begin,py39,py310,py311,coverage,bandit,lint
+envlist = begin,py39,py310,py311,coverage,bandit,lint,reuse
 
 [testenv]
 allow_externals = pytest, coverage
 
 deps =
     -rrequirements/requirements-dev.txt
 
@@ -53,14 +53,19 @@
 [testenv:lint]
 # run style checks
 commands =
     flake8
     mypy gp2040ce_bintools
     - flake8 --disable-noqa --ignore= --select=E,W,F,C,D,A,G,B,I,T,M,DUO
 
+[testenv:reuse]
+# check license documentation
+commands =
+    reuse lint
+
 [coverage:paths]
 source =
     ./
     .tox/**/site-packages/
 
 [coverage:run]
 branch = True
```

