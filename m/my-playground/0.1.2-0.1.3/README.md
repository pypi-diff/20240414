# Comparing `tmp/my_playground-0.1.2.tar.gz` & `tmp/my_playground-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_playground-0.1.2.tar", last modified: Sat Apr 13 15:26:13 2024, max compression
+gzip compressed data, was "my_playground-0.1.3.tar", last modified: Sat Apr 13 15:31:50 2024, max compression
```

## Comparing `my_playground-0.1.2.tar` & `my_playground-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       13 2024-04-13 15:25:59.983168 my_playground-0.1.2/README.md
--rw-r--r--   0        0        0      413 2024-04-13 15:26:13.207154 my_playground-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       38 2024-04-13 15:25:59.983168 my_playground-0.1.2/src/playground/__init__.py
--rw-r--r--   0        0        0       44 2024-04-13 15:25:59.983168 my_playground-0.1.2/src/playground/hello.py
--rw-r--r--   0        0        0        0 2024-04-13 15:25:59.983168 my_playground-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0      273 1970-01-01 00:00:00.000000 my_playground-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       13 2024-04-13 15:31:36.506899 my_playground-0.1.3/README.md
+-rw-r--r--   0        0        0      413 2024-04-13 15:31:50.090870 my_playground-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       24 2024-04-13 15:31:36.506899 my_playground-0.1.3/src/playground/__init__.py
+-rw-r--r--   0        0        0       44 2024-04-13 15:31:36.506899 my_playground-0.1.3/src/playground/hello.py
+-rw-r--r--   0        0        0        0 2024-04-13 15:31:36.506899 my_playground-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0      273 1970-01-01 00:00:00.000000 my_playground-0.1.3/PKG-INFO
```

