# Comparing `tmp/onebag-0.1.0.tar.gz` & `tmp/onebag-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onebag-0.1.0.tar", max compression
+gzip compressed data, was "onebag-0.1.1.tar", max compression
```

## Comparing `onebag-0.1.0.tar` & `onebag-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-04-13 20:13:19.118666 onebag-0.1.0/README.md
--rw-r--r--   0        0        0       48 2024-04-13 23:17:24.211769 onebag-0.1.0/onebag/__init__.py
--rw-r--r--   0        0        0     1593 2024-04-13 23:17:24.215621 onebag-0.1.0/onebag/functions.py
--rw-r--r--   0        0        0      412 2024-04-13 23:30:00.212185 onebag-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 onebag-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-13 20:13:19.118666 onebag-0.1.1/README.md
+-rw-r--r--   0        0        0       48 2024-04-13 23:17:24.211769 onebag-0.1.1/onebag/__init__.py
+-rw-r--r--   0        0        0     1593 2024-04-13 23:17:24.215621 onebag-0.1.1/onebag/functions.py
+-rw-r--r--   0        0        0      411 2024-04-14 00:22:31.057672 onebag-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 onebag-0.1.1/PKG-INFO
```

### Comparing `onebag-0.1.0/onebag/functions.py` & `onebag-0.1.1/onebag/functions.py`

 * *Files identical despite different names*

