# Comparing `tmp/my_playground-0.1.5.tar.gz` & `tmp/my_playground-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_playground-0.1.5.tar", last modified: Sun Apr 14 10:36:22 2024, max compression
+gzip compressed data, was "my_playground-0.1.6.tar", last modified: Sun Apr 14 10:43:27 2024, max compression
```

## Comparing `my_playground-0.1.5.tar` & `my_playground-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       13 2024-04-14 10:35:59.223008 my_playground-0.1.5/README.md
--rw-r--r--   0        0        0      413 2024-04-14 10:36:22.691328 my_playground-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       39 2024-04-14 10:35:59.223008 my_playground-0.1.5/src/playground/__init__.py
--rw-r--r--   0        0        0       44 2024-04-14 10:35:59.223008 my_playground-0.1.5/src/playground/hello.py
--rw-r--r--   0        0        0        0 2024-04-14 10:35:59.223008 my_playground-0.1.5/tests/__init__.py
--rw-r--r--   0        0        0      273 1970-01-01 00:00:00.000000 my_playground-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       13 2024-04-14 10:43:09.641142 my_playground-0.1.6/README.md
+-rw-r--r--   0        0        0      413 2024-04-14 10:43:27.309091 my_playground-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       39 2024-04-14 10:43:09.641142 my_playground-0.1.6/src/playground/__init__.py
+-rw-r--r--   0        0        0       44 2024-04-14 10:43:09.641142 my_playground-0.1.6/src/playground/hello.py
+-rw-r--r--   0        0        0        0 2024-04-14 10:43:09.641142 my_playground-0.1.6/tests/__init__.py
+-rw-r--r--   0        0        0      273 1970-01-01 00:00:00.000000 my_playground-0.1.6/PKG-INFO
```

