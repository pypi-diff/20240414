# Comparing `tmp/my_playground-0.1.7.tar.gz` & `tmp/my_playground-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_playground-0.1.7.tar", last modified: Sun Apr 14 10:52:55 2024, max compression
+gzip compressed data, was "my_playground-0.1.8.tar", last modified: Sun Apr 14 13:42:27 2024, max compression
```

## Comparing `my_playground-0.1.7.tar` & `my_playground-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       13 2024-04-14 10:52:34.014505 my_playground-0.1.7/README.md
--rw-r--r--   0        0        0      413 2024-04-14 10:52:55.706410 my_playground-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       35 2024-04-14 10:52:34.014505 my_playground-0.1.7/src/playground/__init__.py
--rw-r--r--   0        0        0       44 2024-04-14 10:52:34.014505 my_playground-0.1.7/src/playground/hello.py
--rw-r--r--   0        0        0        0 2024-04-14 10:52:34.014505 my_playground-0.1.7/tests/__init__.py
--rw-r--r--   0        0        0      273 1970-01-01 00:00:00.000000 my_playground-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       13 2024-04-14 13:42:11.296956 my_playground-0.1.8/README.md
+-rw-r--r--   0        0        0      413 2024-04-14 13:42:27.445016 my_playground-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       35 2024-04-14 13:42:11.296956 my_playground-0.1.8/src/playground/__init__.py
+-rw-r--r--   0        0        0       44 2024-04-14 13:42:11.296956 my_playground-0.1.8/src/playground/hello.py
+-rw-r--r--   0        0        0        0 2024-04-14 13:42:11.296956 my_playground-0.1.8/tests/__init__.py
+-rw-r--r--   0        0        0      273 1970-01-01 00:00:00.000000 my_playground-0.1.8/PKG-INFO
```

