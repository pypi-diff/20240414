# Comparing `tmp/get_bibtex-1.0.0.tar.gz` & `tmp/get_bibtex-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get_bibtex-1.0.0.tar", last modified: Sun Apr 14 10:30:20 2024, max compression
+gzip compressed data, was "get_bibtex-1.0.1.tar", last modified: Sun Apr 14 12:04:37 2024, max compression
```

## Comparing `get_bibtex-1.0.0.tar` & `get_bibtex-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 10:30:20.741454 get_bibtex-1.0.0/
--rw-rw-rw-   0        0        0     1649 2024-04-14 10:30:20.739451 get_bibtex-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      731 2024-04-13 14:36:53.000000 get_bibtex-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-14 10:30:20.670451 get_bibtex-1.0.0/apiModels/
--rw-rw-rw-   0        0        0        0 2024-04-13 13:17:47.000000 get_bibtex-1.0.0/apiModels/__init__.py
--rw-rw-rw-   0        0        0     2925 2024-04-13 13:57:44.000000 get_bibtex-1.0.0/apiModels/get_bibtex_from_crossref.py
--rw-rw-rw-   0        0        0     3563 2024-04-13 14:18:07.000000 get_bibtex-1.0.0/apiModels/get_bibtex_from_google_scholar.py
-drwxrwxrwx   0        0        0        0 2024-04-14 10:30:20.708452 get_bibtex-1.0.0/get_bibtex.egg-info/
--rw-rw-rw-   0        0        0     1649 2024-04-14 10:30:20.000000 get_bibtex-1.0.0/get_bibtex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2024-04-14 10:30:20.000000 get_bibtex-1.0.0/get_bibtex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 10:30:20.000000 get_bibtex-1.0.0/get_bibtex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-14 10:30:20.000000 get_bibtex-1.0.0/get_bibtex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 10:30:20.741454 get_bibtex-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     3216 2024-04-14 10:28:50.000000 get_bibtex-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-14 10:30:20.737455 get_bibtex-1.0.0/utils/
--rw-rw-rw-   0        0        0        0 2024-04-13 13:59:03.000000 get_bibtex-1.0.0/utils/__init__.py
--rw-rw-rw-   0        0        0      349 2024-04-13 14:00:01.000000 get_bibtex-1.0.0/utils/get_bibtex_from_link.py
--rw-rw-rw-   0        0        0      633 2024-04-13 14:00:01.000000 get_bibtex-1.0.0/utils/verify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:04:37.359810 get_bibtex-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-14 12:04:37.359810 get_bibtex-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-14 12:04:29.000000 get_bibtex-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:04:37.359810 get_bibtex-1.0.1/apiModels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 12:04:29.000000 get_bibtex-1.0.1/apiModels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-14 12:04:29.000000 get_bibtex-1.0.1/apiModels/get_bibtex_from_crossref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-14 12:04:29.000000 get_bibtex-1.0.1/apiModels/get_bibtex_from_google_scholar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:04:37.359810 get_bibtex-1.0.1/get_bibtex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-14 12:04:37.000000 get_bibtex-1.0.1/get_bibtex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-14 12:04:37.000000 get_bibtex-1.0.1/get_bibtex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 12:04:37.000000 get_bibtex-1.0.1/get_bibtex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-14 12:04:37.000000 get_bibtex-1.0.1/get_bibtex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 12:04:37.359810 get_bibtex-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-04-14 12:04:29.000000 get_bibtex-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:04:37.359810 get_bibtex-1.0.1/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 12:04:29.000000 get_bibtex-1.0.1/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-14 12:04:29.000000 get_bibtex-1.0.1/utils/get_bibtex_from_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-14 12:04:29.000000 get_bibtex-1.0.1/utils/verify.py
```

### Comparing `get_bibtex-1.0.0/README.md` & `get_bibtex-1.0.1/README.md`

 * *Files identical despite different names*

