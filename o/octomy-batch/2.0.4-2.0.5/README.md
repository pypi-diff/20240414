# Comparing `tmp/octomy-batch-2.0.4.tar.gz` & `tmp/octomy-batch-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octomy-batch-2.0.4.tar", last modified: Wed Apr 10 23:48:01 2024, max compression
+gzip compressed data, was "octomy-batch-2.0.5.tar", last modified: Sat Apr 13 21:52:24 2024, max compression
```

## Comparing `octomy-batch-2.0.4.tar` & `octomy-batch-2.0.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:48:01.870838 octomy-batch-2.0.4/
--rw-r--r--   0 leo       (1000) leo       (1000)      496 2021-12-17 22:49:10.000000 octomy-batch-2.0.4/.gitignore
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:48:01.866838 octomy-batch-2.0.4/.gitlab/
--rw-r--r--   0 leo       (1000) leo       (1000)      804 2021-11-09 04:03:42.000000 octomy-batch-2.0.4/.gitlab/ci.yaml
--rw-r--r--   0 leo       (1000) leo       (1000)     2021 2024-04-01 18:16:40.000000 octomy-batch-2.0.4/LICENSE
--rw-r--r--   0 leo       (1000) leo       (1000)      284 2024-04-01 17:02:28.000000 octomy-batch-2.0.4/Makefile
--rw-r--r--   0 leo       (1000) leo       (1000)     3130 2024-04-10 23:48:01.870838 octomy-batch-2.0.4/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)     2292 2024-04-01 18:15:51.000000 octomy-batch-2.0.4/README.md
--rw-r--r--   0 leo       (1000) leo       (1000)        6 2024-04-10 23:47:25.000000 octomy-batch-2.0.4/VERSION
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:48:01.866838 octomy-batch-2.0.4/bin/
--rwxr-xr-x   0 leo       (1000) leo       (1000)     3257 2024-04-06 21:53:07.000000 octomy-batch-2.0.4/bin/octomy-batch
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:48:01.866838 octomy-batch-2.0.4/code_quality/
--rw-rw-r--   0 leo       (1000) leo       (1000)      136 2020-03-25 22:47:14.000000 octomy-batch-2.0.4/code_quality/.flake8
--rw-r--r--   0 leo       (1000) leo       (1000)     1919 2021-11-09 04:03:42.000000 octomy-batch-2.0.4/code_quality/Makefile
--rw-rw-r--   0 leo       (1000) leo       (1000)      117 2020-03-25 22:44:52.000000 octomy-batch-2.0.4/code_quality/mypy.ini
--rw-rw-r--   0 leo       (1000) leo       (1000)    11867 2020-03-25 22:43:04.000000 octomy-batch-2.0.4/code_quality/pylintrc
--rw-r--r--   0 leo       (1000) leo       (1000)     2789 2021-11-09 04:03:47.000000 octomy-batch-2.0.4/config.json
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:48:01.858838 octomy-batch-2.0.4/octomy/
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:48:01.862838 octomy-batch-2.0.4/octomy/batch/
--rw-r--r--   0 leo       (1000) leo       (1000)    20286 2024-04-10 23:37:03.000000 octomy-batch-2.0.4/octomy/batch/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:48:01.862838 octomy-batch-2.0.4/octomy/batch/filters/
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2024-04-06 13:13:35.000000 octomy-batch-2.0.4/octomy/batch/filters/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:48:01.862838 octomy-batch-2.0.4/octomy/batch/filters/base/
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2021-11-09 04:03:42.000000 octomy-batch-2.0.4/octomy/batch/filters/base/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      302 2024-04-01 17:33:21.000000 octomy-batch-2.0.4/octomy/batch/filters/base/hello.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:48:01.862838 octomy-batch-2.0.4/octomy/batch/filters/utils/
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2021-11-09 04:03:42.000000 octomy-batch-2.0.4/octomy/batch/filters/utils/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      697 2024-04-01 20:23:49.000000 octomy-batch-2.0.4/octomy/batch/filters/utils/ping.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1285 2024-04-07 18:05:17.000000 octomy-batch-2.0.4/octomy/batch/filters/utils/test.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:48:01.862838 octomy-batch-2.0.4/octomy/batch/server/
--rw-rw-r--   0 leo       (1000) leo       (1000)     4381 2024-03-22 18:00:16.000000 octomy-batch-2.0.4/octomy/batch/server/WebsiteIO.py
--rw-r--r--   0 leo       (1000) leo       (1000)     2254 2024-04-06 21:57:46.000000 octomy-batch-2.0.4/octomy/batch/server/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     4451 2024-04-10 23:07:15.000000 octomy-batch-2.0.4/octomy/batch/types.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:48:01.866838 octomy-batch-2.0.4/octomy_batch.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)     3130 2024-04-10 23:48:01.000000 octomy-batch-2.0.4/octomy_batch.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)     1301 2024-04-10 23:48:01.000000 octomy-batch-2.0.4/octomy_batch.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2024-04-10 23:48:01.000000 octomy-batch-2.0.4/octomy_batch.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-10 23:48:01.000000 octomy-batch-2.0.4/octomy_batch.egg-info/namespace_packages.txt
--rw-r--r--   0 leo       (1000) leo       (1000)       21 2024-04-10 23:48:01.000000 octomy-batch-2.0.4/octomy_batch.egg-info/requires.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-10 23:48:01.000000 octomy-batch-2.0.4/octomy_batch.egg-info/top_level.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2020-11-28 23:26:57.000000 octomy-batch-2.0.4/octomy_batch.egg-info/zip-safe
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:48:01.866838 octomy-batch-2.0.4/requirements/
--rw-r--r--   0 leo       (1000) leo       (1000)       21 2024-04-06 23:31:18.000000 octomy-batch-2.0.4/requirements/requirements.in
--rw-r--r--   0 leo       (1000) leo       (1000)     1743 2024-04-06 23:33:41.000000 octomy-batch-2.0.4/requirements/requirements.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      215 2021-11-09 04:03:42.000000 octomy-batch-2.0.4/requirements/test_requirements.in
--rw-r--r--   0 leo       (1000) leo       (1000)     2903 2023-08-28 22:19:16.000000 octomy-batch-2.0.4/requirements/test_requirements.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      166 2024-04-10 23:48:01.870838 octomy-batch-2.0.4/setup.cfg
--rwxr-xr-x   0 leo       (1000) leo       (1000)     7024 2024-04-06 13:28:48.000000 octomy-batch-2.0.4/setup.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:48:01.866838 octomy-batch-2.0.4/tests/
--rw-rw-r--   0 leo       (1000) leo       (1000)     1097 2020-03-19 22:34:38.000000 octomy-batch-2.0.4/tests/Makefile
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-19 20:39:36.000000 octomy-batch-2.0.4/tests/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:48:01.866838 octomy-batch-2.0.4/tests/integration/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-batch-2.0.4/tests/integration/__init__.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      130 2020-03-20 01:43:26.000000 octomy-batch-2.0.4/tests/integration/test_integration.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:48:01.866838 octomy-batch-2.0.4/tests/load/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-12-15 04:59:08.000000 octomy-batch-2.0.4/tests/load/__init__.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      123 2020-03-20 01:43:18.000000 octomy-batch-2.0.4/tests/load/test_load.py
--rw-r--r--   0 leo       (1000) leo       (1000)      339 2022-01-12 22:37:26.000000 octomy-batch-2.0.4/tests/pytest.ini
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:48:01.870838 octomy-batch-2.0.4/tests/regressions/
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2020-12-15 04:59:10.000000 octomy-batch-2.0.4/tests/regressions/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      130 2020-12-15 04:57:55.000000 octomy-batch-2.0.4/tests/regressions/test_regressions.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-10 23:48:01.870838 octomy-batch-2.0.4/tests/unit/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-batch-2.0.4/tests/unit/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      202 2022-01-12 22:37:26.000000 octomy-batch-2.0.4/tests/unit/test_batch_processor.py
--rw-r--r--   0 leo       (1000) leo       (1000)      190 2022-01-12 22:37:26.000000 octomy-batch-2.0.4/tests/unit/test_server.py
--rw-r--r--   0 leo       (1000) leo       (1000)     3502 2022-01-12 22:37:26.000000 octomy-batch-2.0.4/tests/unit/test_unit.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:52:24.333243 octomy-batch-2.0.5/
+-rw-r--r--   0 leo       (1000) leo       (1000)      496 2021-12-17 22:49:10.000000 octomy-batch-2.0.5/.gitignore
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:52:24.325243 octomy-batch-2.0.5/.gitlab/
+-rw-r--r--   0 leo       (1000) leo       (1000)      804 2021-11-09 04:03:42.000000 octomy-batch-2.0.5/.gitlab/ci.yaml
+-rw-r--r--   0 leo       (1000) leo       (1000)     2021 2024-04-01 18:16:40.000000 octomy-batch-2.0.5/LICENSE
+-rw-r--r--   0 leo       (1000) leo       (1000)      284 2024-04-01 17:02:28.000000 octomy-batch-2.0.5/Makefile
+-rw-r--r--   0 leo       (1000) leo       (1000)     3129 2024-04-13 21:52:24.333243 octomy-batch-2.0.5/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)     2292 2024-04-01 18:15:51.000000 octomy-batch-2.0.5/README.md
+-rw-r--r--   0 leo       (1000) leo       (1000)        6 2024-04-13 21:49:26.000000 octomy-batch-2.0.5/VERSION
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:52:24.325243 octomy-batch-2.0.5/bin/
+-rwxr-xr-x   0 leo       (1000) leo       (1000)     3257 2024-04-06 21:53:07.000000 octomy-batch-2.0.5/bin/octomy-batch
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:52:24.325243 octomy-batch-2.0.5/code_quality/
+-rw-rw-r--   0 leo       (1000) leo       (1000)      136 2020-03-25 22:47:14.000000 octomy-batch-2.0.5/code_quality/.flake8
+-rw-r--r--   0 leo       (1000) leo       (1000)     1919 2021-11-09 04:03:42.000000 octomy-batch-2.0.5/code_quality/Makefile
+-rw-rw-r--   0 leo       (1000) leo       (1000)      117 2020-03-25 22:44:52.000000 octomy-batch-2.0.5/code_quality/mypy.ini
+-rw-rw-r--   0 leo       (1000) leo       (1000)    11867 2020-03-25 22:43:04.000000 octomy-batch-2.0.5/code_quality/pylintrc
+-rw-r--r--   0 leo       (1000) leo       (1000)     2789 2021-11-09 04:03:47.000000 octomy-batch-2.0.5/config.json
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:52:24.305243 octomy-batch-2.0.5/octomy/
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:52:24.313243 octomy-batch-2.0.5/octomy/batch/
+-rw-r--r--   0 leo       (1000) leo       (1000)    20884 2024-04-13 21:48:00.000000 octomy-batch-2.0.5/octomy/batch/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:52:24.313243 octomy-batch-2.0.5/octomy/batch/filters/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2024-04-06 13:13:35.000000 octomy-batch-2.0.5/octomy/batch/filters/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:52:24.317243 octomy-batch-2.0.5/octomy/batch/filters/base/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2021-11-09 04:03:42.000000 octomy-batch-2.0.5/octomy/batch/filters/base/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      302 2024-04-01 17:33:21.000000 octomy-batch-2.0.5/octomy/batch/filters/base/hello.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:52:24.321243 octomy-batch-2.0.5/octomy/batch/filters/utils/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2021-11-09 04:03:42.000000 octomy-batch-2.0.5/octomy/batch/filters/utils/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      697 2024-04-01 20:23:49.000000 octomy-batch-2.0.5/octomy/batch/filters/utils/ping.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1285 2024-04-07 18:05:17.000000 octomy-batch-2.0.5/octomy/batch/filters/utils/test.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:52:24.325243 octomy-batch-2.0.5/octomy/batch/server/
+-rw-rw-r--   0 leo       (1000) leo       (1000)     4381 2024-03-22 18:00:16.000000 octomy-batch-2.0.5/octomy/batch/server/WebsiteIO.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2254 2024-04-06 21:57:46.000000 octomy-batch-2.0.5/octomy/batch/server/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     4487 2024-04-11 00:20:42.000000 octomy-batch-2.0.5/octomy/batch/types.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:52:24.325243 octomy-batch-2.0.5/octomy_batch.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)     3129 2024-04-13 21:52:24.000000 octomy-batch-2.0.5/octomy_batch.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)     1301 2024-04-13 21:52:24.000000 octomy-batch-2.0.5/octomy_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2024-04-13 21:52:24.000000 octomy-batch-2.0.5/octomy_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-13 21:52:24.000000 octomy-batch-2.0.5/octomy_batch.egg-info/namespace_packages.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       21 2024-04-13 21:52:24.000000 octomy-batch-2.0.5/octomy_batch.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-13 21:52:24.000000 octomy-batch-2.0.5/octomy_batch.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2020-11-28 23:26:57.000000 octomy-batch-2.0.5/octomy_batch.egg-info/zip-safe
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:52:24.329243 octomy-batch-2.0.5/requirements/
+-rw-r--r--   0 leo       (1000) leo       (1000)       21 2024-04-13 21:50:16.000000 octomy-batch-2.0.5/requirements/requirements.in
+-rw-r--r--   0 leo       (1000) leo       (1000)     1743 2024-04-13 21:52:09.000000 octomy-batch-2.0.5/requirements/requirements.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      215 2021-11-09 04:03:42.000000 octomy-batch-2.0.5/requirements/test_requirements.in
+-rw-r--r--   0 leo       (1000) leo       (1000)     2903 2023-08-28 22:19:16.000000 octomy-batch-2.0.5/requirements/test_requirements.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      166 2024-04-13 21:52:24.333243 octomy-batch-2.0.5/setup.cfg
+-rwxr-xr-x   0 leo       (1000) leo       (1000)     7479 2024-04-11 00:17:44.000000 octomy-batch-2.0.5/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:52:24.329243 octomy-batch-2.0.5/tests/
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1097 2020-03-19 22:34:38.000000 octomy-batch-2.0.5/tests/Makefile
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-19 20:39:36.000000 octomy-batch-2.0.5/tests/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:52:24.329243 octomy-batch-2.0.5/tests/integration/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-batch-2.0.5/tests/integration/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      125 2024-04-13 19:27:35.000000 octomy-batch-2.0.5/tests/integration/test_integration.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:52:24.329243 octomy-batch-2.0.5/tests/load/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-12-15 04:59:08.000000 octomy-batch-2.0.5/tests/load/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      118 2024-04-13 19:27:44.000000 octomy-batch-2.0.5/tests/load/test_load.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      339 2022-01-12 22:37:26.000000 octomy-batch-2.0.5/tests/pytest.ini
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:52:24.329243 octomy-batch-2.0.5/tests/regressions/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2020-12-15 04:59:10.000000 octomy-batch-2.0.5/tests/regressions/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      125 2024-04-13 19:27:26.000000 octomy-batch-2.0.5/tests/regressions/test_regressions.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:52:24.333243 octomy-batch-2.0.5/tests/unit/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-batch-2.0.5/tests/unit/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1188 2024-04-13 21:48:19.000000 octomy-batch-2.0.5/tests/unit/test_batch_processor.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      178 2024-04-13 14:03:03.000000 octomy-batch-2.0.5/tests/unit/test_server.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2828 2024-04-13 14:24:05.000000 octomy-batch-2.0.5/tests/unit/test_unit.py
```

### Comparing `octomy-batch-2.0.4/.gitlab/ci.yaml` & `octomy-batch-2.0.5/.gitlab/ci.yaml`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.4/LICENSE` & `octomy-batch-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.4/PKG-INFO` & `octomy-batch-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octomy-batch
-Version: 2.0.4
+Version: 2.0.5
 Summary: ('octomy/batch',)
 Home-page: https://gitlab.com/octomy/batch
 Author: OctoMY
 Author-email: pypi@octomy.org
 Maintainer: OctoMY
 Maintainer-email: pypi@octomy.org
 License: Proprietary Software License
@@ -78,8 +78,7 @@
 
 batch is an scalable asynchronous task execution system similar to cellery but tailored to the needs of OctoMY.
 
 
 FK_CLI_OUTPUT=""
 FK_CLI_EXECUTABLE="true"
 FK_HAS_CLI_EXECUTABLE="false"
-
```

### Comparing `octomy-batch-2.0.4/README.md` & `octomy-batch-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.4/bin/octomy-batch` & `octomy-batch-2.0.5/bin/octomy-batch`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.4/code_quality/Makefile` & `octomy-batch-2.0.5/code_quality/Makefile`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.4/code_quality/pylintrc` & `octomy-batch-2.0.5/code_quality/pylintrc`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.4/config.json` & `octomy-batch-2.0.5/config.json`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.4/octomy/batch/__init__.py` & `octomy-batch-2.0.5/octomy/batch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #from octomy.batch.db import Database
 from octomy.batch.types import *
 from octomy.utils import human_delta
-from pathlib import Path
+import pathlib
 import datetime
 import octomy.utils
 import octomy.utils.Watchdog
 import glob
 import importlib
 import importlib.util
 import json
@@ -48,46 +48,58 @@
 
 
 def random_token(length=10):
 	alphabet = string.ascii_letters + string.digits
 	return "".join(random.choice(alphabet) for i in range(length))
 
 
+def get_package_relative_dir():
+	path = pathlib.Path(__file__).resolve()
+	logger.info(f"get_package_relative_dir file: '{path}' is file: {path.is_file()}")
+	path = path.parent.parent.parent
+	logger.info(f"get_package_relative_dir path: '{path}' is dir: {path.is_dir()}")
+	return path
+
 
 class Processor:
 	batch_sql_base:str = "octomy.batch"
 	
-	def __init__(self, config, dbc, do_debug=False):
+	def __init__(self, config, dbc, do_debug = False):
 		self.do_debug = do_debug
 		self.worker_id = None
 		self.config = config
 		self.dbc = dbc
-		#self.db = octomy.batch.db.Database(config, dbc)
 		self.do_log = self.config.get("batch-log-logging", True)
 		self.last_cleanup_time = datetime.datetime.now()
 		self.task_filter = re.compile("^([0-9a-z\-_]+(\/[0-9a-z\-_]+)*)$")
 		self.last_status_time = None
 		self.callables = {}
 		self.callables_params = {}
 		self.entry_name = "batch_filter_entrypoint"
 		self.param_name = "batch_filter_parameters"
+		self.package_dir = get_package_relative_dir()
+		self.sql_dir = self.package_dir.joinpath('sql')
+		self.dbc.register_query_dir(self.sql_dir, do_preload = True, do_debug = do_debug)
+		if do_debug:
+			logger.warning(f"sql dir: {self.package_dir} is dir={self.package_dir.is_dir()}")
 
 	async def get_id(self):
 		if not self.worker_id:
 			self.worker_id = random_token(10)
 			logger.info(f"Batch Processor {self.worker_id} instanciated")
 		return self.worker_id
 
 	def __del__(self):
 		if self.worker_id:
 			logger.info(f"Batch Processor {self.worker_id} deleted")
 			self.worker_id = None
 
 
 	async def create_tables(self):
+		await self.dbc.register_query_dir(self.package_dir, do_preload = True, do_debug = True)
 		await self.dbc.query_none("overwatch.batch.create_batch_status_enum", prepare=False)
 		await self.dbc.query_none("overwatch.batch.create_batch_items", prepare=False)
 		await self.dbc.query_none("overwatch.batch.create_gcra_throttle", prepare=False)
 
 	async def verify(self):
 		modules = await self.list_modules()
 		# logger.info(f"modules: {pprint.pformat(modules)}")
```

### Comparing `octomy-batch-2.0.4/octomy/batch/filters/utils/ping.py` & `octomy-batch-2.0.5/octomy/batch/filters/utils/ping.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.4/octomy/batch/filters/utils/test.py` & `octomy-batch-2.0.5/octomy/batch/filters/utils/test.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.4/octomy/batch/server/WebsiteIO.py` & `octomy-batch-2.0.5/octomy/batch/server/WebsiteIO.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.4/octomy/batch/server/__init__.py` & `octomy-batch-2.0.5/octomy/batch/server/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.4/octomy/batch/types.py` & `octomy-batch-2.0.5/octomy/batch/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 	, throttle_limit integer
 	, throttle_period integer
 	, source text
 	, error text
 	, worker_id varchar(63) default null
 	'''
 	priority:int
-	ttl_seconds:int | None = None
+	# ttl_seconds:int | None = None
+	ttl_seconds:Optional[int] = None
 	data:str | None = None
 	result:str | None = None
 	type: Annotated[str, pydantic.StringConstraints(max_length=255)] | None = None
 	status: JobStatusEnum | None = None
 	throttle_key: Annotated[str, pydantic.StringConstraints(max_length=63)] | None = None
 	throttle_limit:int | None = None
 	throttle_period:int | None = None
```

### Comparing `octomy-batch-2.0.4/octomy_batch.egg-info/PKG-INFO` & `octomy-batch-2.0.5/octomy_batch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octomy-batch
-Version: 2.0.4
+Version: 2.0.5
 Summary: ('octomy/batch',)
 Home-page: https://gitlab.com/octomy/batch
 Author: OctoMY
 Author-email: pypi@octomy.org
 Maintainer: OctoMY
 Maintainer-email: pypi@octomy.org
 License: Proprietary Software License
@@ -78,8 +78,7 @@
 
 batch is an scalable asynchronous task execution system similar to cellery but tailored to the needs of OctoMY.
 
 
 FK_CLI_OUTPUT=""
 FK_CLI_EXECUTABLE="true"
 FK_HAS_CLI_EXECUTABLE="false"
-
```

### Comparing `octomy-batch-2.0.4/octomy_batch.egg-info/SOURCES.txt` & `octomy-batch-2.0.5/octomy_batch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.4/requirements/requirements.txt` & `octomy-batch-2.0.5/requirements/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     # via octomy-common
 idna==2.10
     # via
     #   email-validator
     #   requests
 markupsafe==2.1.5
     # via octomy-common
-octomy-common==2.0.5
+octomy-common==2.0.6
     # via -r requirements.in
 orderedmultidict==1.0.1
     # via furl
 psycopg[binary,pool]==3.1.10
     # via octomy-common
 psycopg-binary==3.1.10
     # via psycopg
```

### Comparing `octomy-batch-2.0.4/requirements/test_requirements.txt` & `octomy-batch-2.0.5/requirements/test_requirements.txt`

 * *Files identical despite different names*

### Comparing `octomy-batch-2.0.4/setup.py` & `octomy-batch-2.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -179,14 +179,28 @@
 def get_license():
 	bob={
 		"license": "Proprietary",
 	}
 
 
 
+# Function to recursively list all files in a directory
+def list_files(directory):
+	paths = []
+	for (path, directories, filenames) in os.walk(directory):
+		for filename in filenames:
+			# Generate the path relative to the directory
+			paths.append(os.path.join('..', path, filename))
+	return paths
+
+
+# Assuming 'sql/' is directly inside 'your_package/'
+package_sql_files = list_files('sql')
+
+
 package = {
 	  "name": package_name
 	, "version": get_version_string()
 	, "author": author_name
 	, "author_email": author_email
 	, "maintainer": author_name
 	, "maintainer_email": author_email
@@ -205,15 +219,16 @@
 	# Allow flexible deps for install
 	, "install_requires": read_requirements_file("requirements/requirements.in")
 	# Use flexible deps for testing
 	, "tests_require": read_requirements_file("requirements/test_requirements.in")
 	, "test_suite": os.path.join(code_dir, "tests")
 	, "python_requires": ">=" + python_version
 	# Needed because installed package depends on this file to know it's version number
-	, "data_files": [(base_name, [version_file]), (base_name, [license_file])]
+	, "data_files": [(package_name, [version_file]), (package_name, [license_file])]
+	, "package_data": { package_name: package_sql_files, }
 	, "include_package_data": True
 	# From https://pypi.org/pypi?%3Aaction=list_classifiers
 	, "classifiers": [
 		  get_development_status()
 		, "Intended Audience :: Developers"
 		, "Intended Audience :: Information Technology"
 		, "Intended Audience :: Science/Research"
```

### Comparing `octomy-batch-2.0.4/tests/Makefile` & `octomy-batch-2.0.5/tests/Makefile`

 * *Files identical despite different names*

