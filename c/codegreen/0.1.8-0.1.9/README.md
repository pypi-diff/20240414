# Comparing `tmp/codegreen-0.1.8.tar.gz` & `tmp/codegreen-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codegreen-0.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "codegreen-0.1.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `codegreen-0.1.8.tar` & `codegreen-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0    32422 2023-09-22 18:30:25.024705 codegreen-0.1.8/LICENSE
--rw-r--r--   0        0        0       47 2023-09-22 20:48:20.204900 codegreen-0.1.8/codegreen/__init__.py
--rw-r--r--   0        0        0      468 2023-09-22 20:49:01.265194 codegreen-0.1.8/codegreen/main.py
--rw-r--r--   0        0        0      430 2023-09-22 20:14:30.022618 codegreen-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 codegreen-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    32422 2023-09-22 18:30:25.024705 codegreen-0.1.9/LICENSE
+-rw-r--r--   0        0        0       47 2023-09-22 20:55:53.264163 codegreen-0.1.9/codegreen/__init__.py
+-rw-r--r--   0        0        0      466 2023-09-22 20:55:36.020038 codegreen-0.1.9/codegreen/main.py
+-rw-r--r--   0        0        0      430 2023-09-22 20:14:30.022618 codegreen-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 codegreen-0.1.9/PKG-INFO
```

### Comparing `codegreen-0.1.8/LICENSE` & `codegreen-0.1.9/LICENSE`

 * *Files identical despite different names*

