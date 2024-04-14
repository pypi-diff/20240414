# Comparing `tmp/bitrix24-rest-1.1.1.tar.gz` & `tmp/bitrix24_rest-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bitrix24-rest-1.1.1.tar", last modified: Tue Oct 29 05:23:13 2019, max compression
+gzip compressed data, was "bitrix24_rest-2.0.0.tar", last modified: Sun Apr 14 00:50:36 2024, max compression
```

## Comparing `bitrix24-rest-1.1.1.tar` & `bitrix24_rest-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxr-xr-x   0 akopkesheshyan   (501) staff       (20)        0 2019-10-29 05:23:13.000000 bitrix24-rest-1.1.1/
--rw-r--r--   0 akopkesheshyan   (501) staff       (20)     1072 2019-10-29 05:08:38.000000 bitrix24-rest-1.1.1/LICENSE
--rw-r--r--   0 akopkesheshyan   (501) staff       (20)       51 2019-10-29 05:08:38.000000 bitrix24-rest-1.1.1/MANIFEST.in
--rw-r--r--   0 akopkesheshyan   (501) staff       (20)     3222 2019-10-29 05:23:13.000000 bitrix24-rest-1.1.1/PKG-INFO
--rw-r--r--   0 akopkesheshyan   (501) staff       (20)     1417 2019-10-29 05:08:38.000000 bitrix24-rest-1.1.1/README.md
-drwxr-xr-x   0 akopkesheshyan   (501) staff       (20)        0 2019-10-29 05:23:13.000000 bitrix24-rest-1.1.1/bitrix24/
--rw-r--r--   0 akopkesheshyan   (501) staff       (20)      936 2019-10-29 05:21:01.000000 bitrix24-rest-1.1.1/bitrix24/__init__.py
--rw-r--r--   0 akopkesheshyan   (501) staff       (20)     4162 2019-10-29 05:21:01.000000 bitrix24-rest-1.1.1/bitrix24/bitrix24.py
--rw-r--r--   0 akopkesheshyan   (501) staff       (20)      336 2019-10-29 05:08:38.000000 bitrix24-rest-1.1.1/bitrix24/exceptions.py
-drwxr-xr-x   0 akopkesheshyan   (501) staff       (20)        0 2019-10-29 05:23:13.000000 bitrix24-rest-1.1.1/bitrix24_rest.egg-info/
--rw-r--r--   0 akopkesheshyan   (501) staff       (20)     3222 2019-10-29 05:23:13.000000 bitrix24-rest-1.1.1/bitrix24_rest.egg-info/PKG-INFO
--rw-r--r--   0 akopkesheshyan   (501) staff       (20)      328 2019-10-29 05:23:13.000000 bitrix24-rest-1.1.1/bitrix24_rest.egg-info/SOURCES.txt
--rw-r--r--   0 akopkesheshyan   (501) staff       (20)        1 2019-10-29 05:23:13.000000 bitrix24-rest-1.1.1/bitrix24_rest.egg-info/dependency_links.txt
--rw-r--r--   0 akopkesheshyan   (501) staff       (20)        9 2019-10-29 05:23:13.000000 bitrix24-rest-1.1.1/bitrix24_rest.egg-info/requires.txt
--rw-r--r--   0 akopkesheshyan   (501) staff       (20)       15 2019-10-29 05:23:13.000000 bitrix24-rest-1.1.1/bitrix24_rest.egg-info/top_level.txt
--rw-r--r--   0 akopkesheshyan   (501) staff       (20)       38 2019-10-29 05:23:13.000000 bitrix24-rest-1.1.1/setup.cfg
--rw-r--r--   0 akopkesheshyan   (501) staff       (20)     2581 2019-10-29 05:21:01.000000 bitrix24-rest-1.1.1/setup.py
-drwxr-xr-x   0 akopkesheshyan   (501) staff       (20)        0 2019-10-29 05:23:13.000000 bitrix24-rest-1.1.1/tests/
--rw-r--r--   0 akopkesheshyan   (501) staff       (20)        0 2019-10-29 05:08:38.000000 bitrix24-rest-1.1.1/tests/__init__.py
--rw-r--r--   0 akopkesheshyan   (501) staff       (20)     2912 2019-10-29 05:08:38.000000 bitrix24-rest-1.1.1/tests/test_bitrix24.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:50:36.623272 bitrix24_rest-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-14 00:50:30.000000 bitrix24_rest-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-14 00:50:30.000000 bitrix24_rest-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-14 00:50:36.623272 bitrix24_rest-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-14 00:50:30.000000 bitrix24_rest-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:50:36.623272 bitrix24_rest-2.0.0/bitrix24/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-14 00:50:30.000000 bitrix24_rest-2.0.0/bitrix24/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-04-14 00:50:30.000000 bitrix24_rest-2.0.0/bitrix24/bitrix24.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-14 00:50:30.000000 bitrix24_rest-2.0.0/bitrix24/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:50:36.623272 bitrix24_rest-2.0.0/bitrix24_rest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-04-14 00:50:36.000000 bitrix24_rest-2.0.0/bitrix24_rest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-14 00:50:36.000000 bitrix24_rest-2.0.0/bitrix24_rest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 00:50:36.000000 bitrix24_rest-2.0.0/bitrix24_rest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-14 00:50:36.000000 bitrix24_rest-2.0.0/bitrix24_rest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-14 00:50:36.000000 bitrix24_rest-2.0.0/bitrix24_rest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 00:50:36.623272 bitrix24_rest-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-14 00:50:30.000000 bitrix24_rest-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:50:36.623272 bitrix24_rest-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 00:50:30.000000 bitrix24_rest-2.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-14 00:50:30.000000 bitrix24_rest-2.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-14 00:50:30.000000 bitrix24_rest-2.0.0/tests/test_async_call_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-14 00:50:30.000000 bitrix24_rest-2.0.0/tests/test_bitrix24.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-14 00:50:30.000000 bitrix24_rest-2.0.0/tests/test_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-14 00:50:30.000000 bitrix24_rest-2.0.0/tests/test_params_preparation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-14 00:50:30.000000 bitrix24_rest-2.0.0/tests/test_request_retry.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bitrix24-rest-1.1.1/LICENSE` & `bitrix24_rest-2.0.0/LICENSE`

 * *Files identical despite different names*

