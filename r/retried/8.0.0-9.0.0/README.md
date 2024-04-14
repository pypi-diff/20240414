# Comparing `tmp/retried-8.0.0.tar.gz` & `tmp/retried-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retried-8.0.0.tar", last modified: Sat Apr 13 23:13:20 2024, max compression
+gzip compressed data, was "retried-9.0.0.tar", last modified: Sun Apr 14 03:02:24 2024, max compression
```

## Comparing `retried-8.0.0.tar` & `retried-9.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      102 2024-04-13 23:13:03.933806 retried-8.0.0/README.md
--rw-r--r--   0        0        0     1061 2024-04-13 23:13:20.734152 retried-8.0.0/pyproject.toml
--rw-r--r--   0        0        0      224 2024-04-13 23:13:03.933806 retried-8.0.0/src/retried/__init__.py
--rw-r--r--   0        0        0       18 2024-04-13 23:13:03.933806 retried-8.0.0/src/retried/__version__.py
--rw-r--r--   0        0        0     2290 2024-04-13 23:13:03.933806 retried-8.0.0/src/retried/aretry.py
--rw-r--r--   0        0        0     4018 2024-04-13 23:13:03.933806 retried-8.0.0/src/retried/retry.py
--rw-r--r--   0        0        0      189 2024-04-13 23:13:03.933806 retried-8.0.0/src/retried/utils.py
--rw-r--r--   0        0        0        0 2024-04-13 23:13:03.933806 retried-8.0.0/tests/__init__.py
--rw-r--r--   0        0        0      657 2024-04-13 23:13:03.933806 retried-8.0.0/tests/test_aretry.py
--rw-r--r--   0        0        0      276 1970-01-01 00:00:00.000000 retried-8.0.0/PKG-INFO
+-rw-r--r--   0        0        0      102 2024-04-14 03:02:03.194994 retried-9.0.0/README.md
+-rw-r--r--   0        0        0     1061 2024-04-14 03:02:24.910920 retried-9.0.0/pyproject.toml
+-rw-r--r--   0        0        0      224 2024-04-14 03:02:03.198994 retried-9.0.0/src/retried/__init__.py
+-rw-r--r--   0        0        0       18 2024-04-14 03:02:03.198994 retried-9.0.0/src/retried/__version__.py
+-rw-r--r--   0        0        0     2290 2024-04-14 03:02:03.198994 retried-9.0.0/src/retried/aretry.py
+-rw-r--r--   0        0        0     4137 2024-04-14 03:02:03.198994 retried-9.0.0/src/retried/retry.py
+-rw-r--r--   0        0        0      528 2024-04-14 03:02:03.198994 retried-9.0.0/src/retried/utils.py
+-rw-r--r--   0        0        0        0 2024-04-14 03:02:03.198994 retried-9.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      657 2024-04-14 03:02:03.198994 retried-9.0.0/tests/test_aretry.py
+-rw-r--r--   0        0        0      276 1970-01-01 00:00:00.000000 retried-9.0.0/PKG-INFO
```

### Comparing `retried-8.0.0/pyproject.toml` & `retried-9.0.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "retried"
-version = "8.0.0"
+version = "9.0.0"
 requires-python = ">=3.9"
 description = "A simple and powerful retrying library for Python"
 readme = "README.md"
 dependencies = []
 
 [build-system]
 requires = [
```

### Comparing `retried-8.0.0/src/retried/aretry.py` & `retried-9.0.0/src/retried/aretry.py`

 * *Files identical despite different names*

### Comparing `retried-8.0.0/tests/test_aretry.py` & `retried-9.0.0/tests/test_aretry.py`

 * *Files identical despite different names*

