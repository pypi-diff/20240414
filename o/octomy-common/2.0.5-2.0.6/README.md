# Comparing `tmp/octomy-common-2.0.5.tar.gz` & `tmp/octomy-common-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octomy-common-2.0.5.tar", last modified: Sat Apr  6 23:31:22 2024, max compression
+gzip compressed data, was "octomy-common-2.0.6.tar", last modified: Sat Apr 13 21:50:12 2024, max compression
```

## Comparing `octomy-common-2.0.5.tar` & `octomy-common-2.0.6.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.365911 octomy-common-2.0.5/
--rw-r--r--   0 leo       (1000) leo       (1000)      735 2021-12-02 17:02:15.000000 octomy-common-2.0.5/.gitignore
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.361911 octomy-common-2.0.5/.gitlab/
--rw-r--r--   0 leo       (1000) leo       (1000)      771 2021-12-02 17:02:15.000000 octomy-common-2.0.5/.gitlab/ci.yaml
--rw-r--r--   0 leo       (1000) leo       (1000)     2021 2024-04-06 09:06:50.000000 octomy-common-2.0.5/LICENSE
--rw-r--r--   0 leo       (1000) leo       (1000)      284 2024-04-06 08:33:37.000000 octomy-common-2.0.5/Makefile
--rw-r--r--   0 leo       (1000) leo       (1000)     8436 2024-04-06 23:31:22.365911 octomy-common-2.0.5/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)     7595 2024-04-06 08:34:18.000000 octomy-common-2.0.5/README.md
--rw-r--r--   0 leo       (1000) leo       (1000)        6 2024-04-06 23:29:56.000000 octomy-common-2.0.5/VERSION
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.361911 octomy-common-2.0.5/code_quality/
--rw-r--r--   0 leo       (1000) leo       (1000)      214 2021-12-02 17:02:15.000000 octomy-common-2.0.5/code_quality/.flake8
--rw-r--r--   0 leo       (1000) leo       (1000)     2492 2021-12-28 02:40:34.000000 octomy-common-2.0.5/code_quality/Makefile
--rw-r--r--   0 leo       (1000) leo       (1000)      135 2021-12-02 17:02:15.000000 octomy-common-2.0.5/code_quality/mypy.ini
--rw-rw-r--   0 leo       (1000) leo       (1000)    11867 2020-03-02 23:49:28.000000 octomy-common-2.0.5/code_quality/pylintrc
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.361911 octomy-common-2.0.5/design/
--rw-r--r--   0 leo       (1000) leo       (1000)    62298 2021-12-02 17:02:15.000000 octomy-common-2.0.5/design/logo-1024.png
--rw-r--r--   0 leo       (1000) leo       (1000)     7427 2021-12-02 17:02:15.000000 octomy-common-2.0.5/design/logo-1024.svg
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.349911 octomy-common-2.0.5/octomy/
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.353911 octomy-common-2.0.5/octomy/access/
--rw-r--r--   0 leo       (1000) leo       (1000)    11927 2024-04-06 10:41:55.000000 octomy-common-2.0.5/octomy/access/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.353911 octomy-common-2.0.5/octomy/cad/
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.353911 octomy-common-2.0.5/octomy/cad/generators/
--rw-r--r--   0 leo       (1000) leo       (1000)     4653 2024-03-21 20:06:58.000000 octomy-common-2.0.5/octomy/cad/generators/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2023-12-09 21:11:36.000000 octomy-common-2.0.5/octomy/cad/generators/common.py
--rw-r--r--   0 leo       (1000) leo       (1000)       74 2023-12-09 21:13:26.000000 octomy-common-2.0.5/octomy/cad/generators/ntop.py
--rw-r--r--   0 leo       (1000) leo       (1000)     6642 2024-03-21 20:05:55.000000 octomy-common-2.0.5/octomy/cad/generators/openscad.py
--rw-r--r--   0 leo       (1000) leo       (1000)    15524 2024-04-06 12:29:11.000000 octomy-common-2.0.5/octomy/cad/ntop.py
--rw-r--r--   0 leo       (1000) leo       (1000)    28147 2024-04-06 12:29:00.000000 octomy-common-2.0.5/octomy/cad/openscad.py
--rw-r--r--   0 leo       (1000) leo       (1000)    20669 2024-03-21 19:38:26.000000 octomy-common-2.0.5/octomy/cad/parts.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.353911 octomy-common-2.0.5/octomy/cad/types/
--rw-r--r--   0 leo       (1000) leo       (1000)     3633 2023-12-09 22:30:55.000000 octomy-common-2.0.5/octomy/cad/types/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.353911 octomy-common-2.0.5/octomy/config/
--rw-r--r--   0 leo       (1000) leo       (1000)    13118 2024-04-06 09:12:51.000000 octomy-common-2.0.5/octomy/config/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.357911 octomy-common-2.0.5/octomy/db/
--rw-rw-r--   0 leo       (1000) leo       (1000)    12172 2024-04-06 23:29:13.000000 octomy-common-2.0.5/octomy/db/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      841 2024-04-06 17:40:11.000000 octomy-common-2.0.5/octomy/db/check.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.357911 octomy-common-2.0.5/octomy/log/
--rw-rw-r--   0 leo       (1000) leo       (1000)     1477 2024-04-06 08:54:24.000000 octomy-common-2.0.5/octomy/log/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.357911 octomy-common-2.0.5/octomy/storage/
--rw-r--r--   0 leo       (1000) leo       (1000)        0 2023-12-09 19:06:16.000000 octomy-common-2.0.5/octomy/storage/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)    11978 2023-12-09 18:40:20.000000 octomy-common-2.0.5/octomy/storage/google_drive.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.357911 octomy-common-2.0.5/octomy/utils/
--rw-rw-r--   0 leo       (1000) leo       (1000)      129 2024-04-06 09:03:01.000000 octomy-common-2.0.5/octomy/utils/Context.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      896 2024-04-06 09:04:17.000000 octomy-common-2.0.5/octomy/utils/Profiler.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      788 2024-04-06 09:04:22.000000 octomy-common-2.0.5/octomy/utils/Svg.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      683 2024-04-06 09:04:29.000000 octomy-common-2.0.5/octomy/utils/Watchdog.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     4963 2024-04-06 09:04:36.000000 octomy-common-2.0.5/octomy/utils/WorkerPool.py
--rw-r--r--   0 leo       (1000) leo       (1000)    13893 2024-04-06 15:00:59.000000 octomy-common-2.0.5/octomy/utils/__init__.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     1623 2024-04-06 09:02:56.000000 octomy-common-2.0.5/octomy/utils/click.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     3333 2024-04-06 09:03:16.000000 octomy-common-2.0.5/octomy/utils/credentials.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     2087 2024-04-06 09:03:27.000000 octomy-common-2.0.5/octomy/utils/csv_to_db.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      587 2024-04-06 09:03:38.000000 octomy-common-2.0.5/octomy/utils/debug_view.py
--rw-rw-r--   0 leo       (1000) leo       (1000)      944 2024-04-06 09:03:47.000000 octomy-common-2.0.5/octomy/utils/excavator.py
--rw-rw-r--   0 leo       (1000) leo       (1000)     2622 2024-04-06 09:04:08.000000 octomy-common-2.0.5/octomy/utils/expiry_cache.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.361911 octomy-common-2.0.5/octomy/version/
--rw-r--r--   0 leo       (1000) leo       (1000)      257 2024-04-06 09:05:07.000000 octomy-common-2.0.5/octomy/version/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.361911 octomy-common-2.0.5/octomy/web/
--rw-r--r--   0 leo       (1000) leo       (1000)     4318 2024-03-24 15:23:44.000000 octomy-common-2.0.5/octomy/web/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     4390 2024-04-06 09:13:34.000000 octomy-common-2.0.5/octomy/web/autoroute.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.361911 octomy-common-2.0.5/octomy/web/context/
--rw-r--r--   0 leo       (1000) leo       (1000)     2247 2024-03-24 20:06:54.000000 octomy-common-2.0.5/octomy/web/context/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.361911 octomy-common-2.0.5/octomy/web/search/
--rw-r--r--   0 leo       (1000) leo       (1000)     3870 2023-04-10 21:13:22.000000 octomy-common-2.0.5/octomy/web/search/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.361911 octomy-common-2.0.5/octomy_common.egg-info/
--rw-r--r--   0 leo       (1000) leo       (1000)     8436 2024-04-06 23:31:22.000000 octomy-common-2.0.5/octomy_common.egg-info/PKG-INFO
--rw-r--r--   0 leo       (1000) leo       (1000)     1736 2024-04-06 23:31:22.000000 octomy-common-2.0.5/octomy_common.egg-info/SOURCES.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2024-04-06 23:31:22.000000 octomy-common-2.0.5/octomy_common.egg-info/dependency_links.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-06 23:31:22.000000 octomy-common-2.0.5/octomy_common.egg-info/namespace_packages.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      325 2024-04-06 23:31:22.000000 octomy-common-2.0.5/octomy_common.egg-info/requires.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-06 23:31:22.000000 octomy-common-2.0.5/octomy_common.egg-info/top_level.txt
--rw-r--r--   0 leo       (1000) leo       (1000)        1 2020-11-26 02:00:43.000000 octomy-common-2.0.5/octomy_common.egg-info/zip-safe
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.365911 octomy-common-2.0.5/requirements/
--rw-r--r--   0 leo       (1000) leo       (1000)      325 2024-04-06 17:42:08.000000 octomy-common-2.0.5/requirements/requirements.in
--rw-r--r--   0 leo       (1000) leo       (1000)     1757 2024-04-06 17:42:10.000000 octomy-common-2.0.5/requirements/requirements.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      271 2023-08-28 21:54:48.000000 octomy-common-2.0.5/requirements/test_requirements.in
--rw-r--r--   0 leo       (1000) leo       (1000)     3299 2024-01-27 21:44:17.000000 octomy-common-2.0.5/requirements/test_requirements.txt
--rw-r--r--   0 leo       (1000) leo       (1000)      166 2024-04-06 23:31:22.365911 octomy-common-2.0.5/setup.cfg
--rwxr-xr-x   0 leo       (1000) leo       (1000)     7025 2024-04-06 09:26:59.000000 octomy-common-2.0.5/setup.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.365911 octomy-common-2.0.5/tests/
--rw-r--r--   0 leo       (1000) leo       (1000)      935 2021-12-02 17:02:15.000000 octomy-common-2.0.5/tests/Makefile
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.5/tests/__init__.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.365911 octomy-common-2.0.5/tests/integration/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.5/tests/integration/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      154 2021-12-02 17:02:15.000000 octomy-common-2.0.5/tests/integration/test_true.py
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.365911 octomy-common-2.0.5/tests/load/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.5/tests/load/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)      147 2021-12-02 17:02:15.000000 octomy-common-2.0.5/tests/load/test_true.py
--rw-r--r--   0 leo       (1000) leo       (1000)      361 2023-08-28 21:54:48.000000 octomy-common-2.0.5/tests/pytest.ini
-drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 23:31:22.365911 octomy-common-2.0.5/tests/unit/
--rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.5/tests/unit/__init__.py
--rw-r--r--   0 leo       (1000) leo       (1000)     1411 2023-08-28 21:54:48.000000 octomy-common-2.0.5/tests/unit/test_util.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.897294 octomy-common-2.0.6/
+-rw-r--r--   0 leo       (1000) leo       (1000)      735 2021-12-02 17:02:15.000000 octomy-common-2.0.6/.gitignore
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.885295 octomy-common-2.0.6/.gitlab/
+-rw-r--r--   0 leo       (1000) leo       (1000)      771 2021-12-02 17:02:15.000000 octomy-common-2.0.6/.gitlab/ci.yaml
+-rw-r--r--   0 leo       (1000) leo       (1000)     2021 2024-04-06 09:06:50.000000 octomy-common-2.0.6/LICENSE
+-rw-r--r--   0 leo       (1000) leo       (1000)      284 2024-04-06 08:33:37.000000 octomy-common-2.0.6/Makefile
+-rw-r--r--   0 leo       (1000) leo       (1000)     8435 2024-04-13 21:50:12.897294 octomy-common-2.0.6/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)     7595 2024-04-06 08:34:18.000000 octomy-common-2.0.6/README.md
+-rw-r--r--   0 leo       (1000) leo       (1000)        6 2024-04-13 21:49:16.000000 octomy-common-2.0.6/VERSION
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.893294 octomy-common-2.0.6/code_quality/
+-rw-r--r--   0 leo       (1000) leo       (1000)      214 2021-12-02 17:02:15.000000 octomy-common-2.0.6/code_quality/.flake8
+-rw-r--r--   0 leo       (1000) leo       (1000)     2492 2021-12-28 02:40:34.000000 octomy-common-2.0.6/code_quality/Makefile
+-rw-r--r--   0 leo       (1000) leo       (1000)      135 2021-12-02 17:02:15.000000 octomy-common-2.0.6/code_quality/mypy.ini
+-rw-rw-r--   0 leo       (1000) leo       (1000)    11867 2020-03-02 23:49:28.000000 octomy-common-2.0.6/code_quality/pylintrc
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.893294 octomy-common-2.0.6/design/
+-rw-r--r--   0 leo       (1000) leo       (1000)    62298 2021-12-02 17:02:15.000000 octomy-common-2.0.6/design/logo-1024.png
+-rw-r--r--   0 leo       (1000) leo       (1000)     7427 2021-12-02 17:02:15.000000 octomy-common-2.0.6/design/logo-1024.svg
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.865295 octomy-common-2.0.6/octomy/
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.869295 octomy-common-2.0.6/octomy/access/
+-rw-r--r--   0 leo       (1000) leo       (1000)    11927 2024-04-06 10:41:55.000000 octomy-common-2.0.6/octomy/access/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.869295 octomy-common-2.0.6/octomy/cad/
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.877294 octomy-common-2.0.6/octomy/cad/generators/
+-rw-r--r--   0 leo       (1000) leo       (1000)     4653 2024-03-21 20:06:58.000000 octomy-common-2.0.6/octomy/cad/generators/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2023-12-09 21:11:36.000000 octomy-common-2.0.6/octomy/cad/generators/common.py
+-rw-r--r--   0 leo       (1000) leo       (1000)       74 2023-12-09 21:13:26.000000 octomy-common-2.0.6/octomy/cad/generators/ntop.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     6642 2024-03-21 20:05:55.000000 octomy-common-2.0.6/octomy/cad/generators/openscad.py
+-rw-r--r--   0 leo       (1000) leo       (1000)    15524 2024-04-06 12:29:11.000000 octomy-common-2.0.6/octomy/cad/ntop.py
+-rw-r--r--   0 leo       (1000) leo       (1000)    28147 2024-04-06 12:29:00.000000 octomy-common-2.0.6/octomy/cad/openscad.py
+-rw-r--r--   0 leo       (1000) leo       (1000)    20669 2024-03-21 19:38:26.000000 octomy-common-2.0.6/octomy/cad/parts.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.877294 octomy-common-2.0.6/octomy/cad/types/
+-rw-r--r--   0 leo       (1000) leo       (1000)     3633 2023-12-09 22:30:55.000000 octomy-common-2.0.6/octomy/cad/types/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.877294 octomy-common-2.0.6/octomy/config/
+-rw-r--r--   0 leo       (1000) leo       (1000)    13118 2024-04-06 09:12:51.000000 octomy-common-2.0.6/octomy/config/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.881294 octomy-common-2.0.6/octomy/db/
+-rw-rw-r--   0 leo       (1000) leo       (1000)    17964 2024-04-13 21:45:20.000000 octomy-common-2.0.6/octomy/db/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      841 2024-04-06 17:40:11.000000 octomy-common-2.0.6/octomy/db/check.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.881294 octomy-common-2.0.6/octomy/log/
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1477 2024-04-06 08:54:24.000000 octomy-common-2.0.6/octomy/log/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.881294 octomy-common-2.0.6/octomy/storage/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2023-12-09 19:06:16.000000 octomy-common-2.0.6/octomy/storage/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)    11978 2023-12-09 18:40:20.000000 octomy-common-2.0.6/octomy/storage/google_drive.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.881294 octomy-common-2.0.6/octomy/utils/
+-rw-rw-r--   0 leo       (1000) leo       (1000)      129 2024-04-06 09:03:01.000000 octomy-common-2.0.6/octomy/utils/Context.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      896 2024-04-06 09:04:17.000000 octomy-common-2.0.6/octomy/utils/Profiler.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      788 2024-04-06 09:04:22.000000 octomy-common-2.0.6/octomy/utils/Svg.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      683 2024-04-06 09:04:29.000000 octomy-common-2.0.6/octomy/utils/Watchdog.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     4963 2024-04-06 09:04:36.000000 octomy-common-2.0.6/octomy/utils/WorkerPool.py
+-rw-r--r--   0 leo       (1000) leo       (1000)    13893 2024-04-06 15:00:59.000000 octomy-common-2.0.6/octomy/utils/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1623 2024-04-06 09:02:56.000000 octomy-common-2.0.6/octomy/utils/click.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     3333 2024-04-06 09:03:16.000000 octomy-common-2.0.6/octomy/utils/credentials.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     2087 2024-04-06 09:03:27.000000 octomy-common-2.0.6/octomy/utils/csv_to_db.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      587 2024-04-06 09:03:38.000000 octomy-common-2.0.6/octomy/utils/debug_view.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      944 2024-04-06 09:03:47.000000 octomy-common-2.0.6/octomy/utils/excavator.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)     2622 2024-04-06 09:04:08.000000 octomy-common-2.0.6/octomy/utils/expiry_cache.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.881294 octomy-common-2.0.6/octomy/version/
+-rw-r--r--   0 leo       (1000) leo       (1000)      257 2024-04-06 09:05:07.000000 octomy-common-2.0.6/octomy/version/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.885295 octomy-common-2.0.6/octomy/web/
+-rw-r--r--   0 leo       (1000) leo       (1000)     4318 2024-03-24 15:23:44.000000 octomy-common-2.0.6/octomy/web/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     4390 2024-04-06 09:13:34.000000 octomy-common-2.0.6/octomy/web/autoroute.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.885295 octomy-common-2.0.6/octomy/web/context/
+-rw-r--r--   0 leo       (1000) leo       (1000)     2247 2024-03-24 20:06:54.000000 octomy-common-2.0.6/octomy/web/context/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.885295 octomy-common-2.0.6/octomy/web/search/
+-rw-r--r--   0 leo       (1000) leo       (1000)     3870 2023-04-10 21:13:22.000000 octomy-common-2.0.6/octomy/web/search/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.885295 octomy-common-2.0.6/octomy_common.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)     8435 2024-04-13 21:50:12.000000 octomy-common-2.0.6/octomy_common.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)     1736 2024-04-13 21:50:12.000000 octomy-common-2.0.6/octomy_common.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2024-04-13 21:50:12.000000 octomy-common-2.0.6/octomy_common.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-13 21:50:12.000000 octomy-common-2.0.6/octomy_common.egg-info/namespace_packages.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      325 2024-04-13 21:50:12.000000 octomy-common-2.0.6/octomy_common.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-13 21:50:12.000000 octomy-common-2.0.6/octomy_common.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2020-11-26 02:00:43.000000 octomy-common-2.0.6/octomy_common.egg-info/zip-safe
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.897294 octomy-common-2.0.6/requirements/
+-rw-r--r--   0 leo       (1000) leo       (1000)      325 2024-04-06 17:42:08.000000 octomy-common-2.0.6/requirements/requirements.in
+-rw-r--r--   0 leo       (1000) leo       (1000)     1757 2024-04-06 17:42:10.000000 octomy-common-2.0.6/requirements/requirements.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      271 2023-08-28 21:54:48.000000 octomy-common-2.0.6/requirements/test_requirements.in
+-rw-r--r--   0 leo       (1000) leo       (1000)     3299 2024-01-27 21:44:17.000000 octomy-common-2.0.6/requirements/test_requirements.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      166 2024-04-13 21:50:12.897294 octomy-common-2.0.6/setup.cfg
+-rwxr-xr-x   0 leo       (1000) leo       (1000)     7025 2024-04-06 09:26:59.000000 octomy-common-2.0.6/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.897294 octomy-common-2.0.6/tests/
+-rw-r--r--   0 leo       (1000) leo       (1000)      935 2021-12-02 17:02:15.000000 octomy-common-2.0.6/tests/Makefile
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.6/tests/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.897294 octomy-common-2.0.6/tests/integration/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.6/tests/integration/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      154 2021-12-02 17:02:15.000000 octomy-common-2.0.6/tests/integration/test_true.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.897294 octomy-common-2.0.6/tests/load/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.6/tests/load/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      147 2021-12-02 17:02:15.000000 octomy-common-2.0.6/tests/load/test_true.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      361 2023-08-28 21:54:48.000000 octomy-common-2.0.6/tests/pytest.ini
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-13 21:50:12.897294 octomy-common-2.0.6/tests/unit/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-common-2.0.6/tests/unit/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1411 2023-08-28 21:54:48.000000 octomy-common-2.0.6/tests/unit/test_util.py
```

### Comparing `octomy-common-2.0.5/.gitignore` & `octomy-common-2.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/.gitlab/ci.yaml` & `octomy-common-2.0.6/.gitlab/ci.yaml`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/LICENSE` & `octomy-common-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/PKG-INFO` & `octomy-common-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octomy-common
-Version: 2.0.5
+Version: 2.0.6
 Summary: ('octomy/common',)
 Home-page: https://gitlab.com/octomy/common
 Author: OctoMY
 Author-email: pypi@octomy.org
 Maintainer: OctoMY
 Maintainer-email: pypi@octomy.org
 License: Proprietary Software License
@@ -159,8 +159,7 @@
 | docker-push     | Push the docker image with correct version tags to registry    |
 | pypi-build      | Build the pypi package with correct version                    |
 | pypi-push       | Push the pypi package with correct version to PyPi repository. NOTE: Should only be called for production branch  |
 
 ## Example implementation
 
 This octomy-common project will follow the rules above and will contain the Makefile targets that can be used as a reference for other projects.
-
```

### Comparing `octomy-common-2.0.5/README.md` & `octomy-common-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/code_quality/Makefile` & `octomy-common-2.0.6/code_quality/Makefile`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/code_quality/pylintrc` & `octomy-common-2.0.6/code_quality/pylintrc`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/design/logo-1024.png` & `octomy-common-2.0.6/design/logo-1024.png`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/design/logo-1024.svg` & `octomy-common-2.0.6/design/logo-1024.svg`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/access/__init__.py` & `octomy-common-2.0.6/octomy/access/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/cad/generators/__init__.py` & `octomy-common-2.0.6/octomy/cad/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/cad/generators/openscad.py` & `octomy-common-2.0.6/octomy/cad/generators/openscad.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/cad/ntop.py` & `octomy-common-2.0.6/octomy/cad/ntop.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/cad/openscad.py` & `octomy-common-2.0.6/octomy/cad/openscad.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/cad/parts.py` & `octomy-common-2.0.6/octomy/cad/parts.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/cad/types/__init__.py` & `octomy-common-2.0.6/octomy/cad/types/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/config/__init__.py` & `octomy-common-2.0.6/octomy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/db/check.py` & `octomy-common-2.0.6/octomy/db/check.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/log/__init__.py` & `octomy-common-2.0.6/octomy/log/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/storage/google_drive.py` & `octomy-common-2.0.6/octomy/storage/google_drive.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/utils/Profiler.py` & `octomy-common-2.0.6/octomy/utils/Profiler.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/utils/Svg.py` & `octomy-common-2.0.6/octomy/utils/Svg.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/utils/Watchdog.py` & `octomy-common-2.0.6/octomy/utils/Watchdog.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/utils/WorkerPool.py` & `octomy-common-2.0.6/octomy/utils/WorkerPool.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/utils/__init__.py` & `octomy-common-2.0.6/octomy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/utils/click.py` & `octomy-common-2.0.6/octomy/utils/click.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/utils/credentials.py` & `octomy-common-2.0.6/octomy/utils/credentials.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/utils/csv_to_db.py` & `octomy-common-2.0.6/octomy/utils/csv_to_db.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/utils/debug_view.py` & `octomy-common-2.0.6/octomy/utils/debug_view.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/utils/excavator.py` & `octomy-common-2.0.6/octomy/utils/excavator.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/utils/expiry_cache.py` & `octomy-common-2.0.6/octomy/utils/expiry_cache.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/web/__init__.py` & `octomy-common-2.0.6/octomy/web/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/web/autoroute.py` & `octomy-common-2.0.6/octomy/web/autoroute.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/web/context/__init__.py` & `octomy-common-2.0.6/octomy/web/context/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy/web/search/__init__.py` & `octomy-common-2.0.6/octomy/web/search/__init__.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/octomy_common.egg-info/PKG-INFO` & `octomy-common-2.0.6/octomy_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octomy-common
-Version: 2.0.5
+Version: 2.0.6
 Summary: ('octomy/common',)
 Home-page: https://gitlab.com/octomy/common
 Author: OctoMY
 Author-email: pypi@octomy.org
 Maintainer: OctoMY
 Maintainer-email: pypi@octomy.org
 License: Proprietary Software License
@@ -159,8 +159,7 @@
 | docker-push     | Push the docker image with correct version tags to registry    |
 | pypi-build      | Build the pypi package with correct version                    |
 | pypi-push       | Push the pypi package with correct version to PyPi repository. NOTE: Should only be called for production branch  |
 
 ## Example implementation
 
 This octomy-common project will follow the rules above and will contain the Makefile targets that can be used as a reference for other projects.
-
```

### Comparing `octomy-common-2.0.5/octomy_common.egg-info/SOURCES.txt` & `octomy-common-2.0.6/octomy_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/requirements/requirements.txt` & `octomy-common-2.0.6/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/requirements/test_requirements.txt` & `octomy-common-2.0.6/requirements/test_requirements.txt`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/setup.py` & `octomy-common-2.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/tests/Makefile` & `octomy-common-2.0.6/tests/Makefile`

 * *Files identical despite different names*

### Comparing `octomy-common-2.0.5/tests/unit/test_util.py` & `octomy-common-2.0.6/tests/unit/test_util.py`

 * *Files identical despite different names*

