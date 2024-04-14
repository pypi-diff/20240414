# Comparing `tmp/quotesgeneratorapi-wrapper-0.2.2.tar.gz` & `tmp/quotesgeneratorapi_wrapper-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quotesgeneratorapi-wrapper-0.2.2.tar", last modified: Tue Mar  5 18:46:59 2024, max compression
+gzip compressed data, was "quotesgeneratorapi_wrapper-0.2.3.tar", max compression
```

## Comparing `quotesgeneratorapi-wrapper-0.2.2.tar` & `quotesgeneratorapi_wrapper-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,6 @@
-drwxr-xr-x   0 anonym    (1000) anonym    (1000)        0 2024-03-05 18:46:59.827119 quotesgeneratorapi-wrapper-0.2.2/
--rw-r--r--   0 anonym    (1000) anonym    (1000)     1080 2024-03-05 18:28:23.000000 quotesgeneratorapi-wrapper-0.2.2/LICENSE
--rw-r--r--   0 anonym    (1000) anonym    (1000)      345 2024-03-05 18:46:59.827119 quotesgeneratorapi-wrapper-0.2.2/PKG-INFO
--rw-r--r--   0 anonym    (1000) anonym    (1000)       26 2024-03-05 18:28:23.000000 quotesgeneratorapi-wrapper-0.2.2/README.md
-drwxr-xr-x   0 anonym    (1000) anonym    (1000)        0 2024-03-05 18:46:59.827119 quotesgeneratorapi-wrapper-0.2.2/quotesgeneratorapi_wrapper/
--rw-r--r--   0 anonym    (1000) anonym    (1000)       65 2024-03-05 18:28:23.000000 quotesgeneratorapi-wrapper-0.2.2/quotesgeneratorapi_wrapper/__init__.py
--rw-r--r--   0 anonym    (1000) anonym    (1000)      654 2024-03-05 18:29:59.000000 quotesgeneratorapi-wrapper-0.2.2/quotesgeneratorapi_wrapper/quotesgenerator.py
-drwxr-xr-x   0 anonym    (1000) anonym    (1000)        0 2024-03-05 18:46:59.827119 quotesgeneratorapi-wrapper-0.2.2/quotesgeneratorapi_wrapper.egg-info/
--rw-r--r--   0 anonym    (1000) anonym    (1000)      345 2024-03-05 18:46:59.000000 quotesgeneratorapi-wrapper-0.2.2/quotesgeneratorapi_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 anonym    (1000) anonym    (1000)      360 2024-03-05 18:46:59.000000 quotesgeneratorapi-wrapper-0.2.2/quotesgeneratorapi_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 anonym    (1000) anonym    (1000)        1 2024-03-05 18:46:59.000000 quotesgeneratorapi-wrapper-0.2.2/quotesgeneratorapi_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 anonym    (1000) anonym    (1000)        9 2024-03-05 18:46:59.000000 quotesgeneratorapi-wrapper-0.2.2/quotesgeneratorapi_wrapper.egg-info/requires.txt
--rw-r--r--   0 anonym    (1000) anonym    (1000)       27 2024-03-05 18:46:59.000000 quotesgeneratorapi-wrapper-0.2.2/quotesgeneratorapi_wrapper.egg-info/top_level.txt
--rw-r--r--   0 anonym    (1000) anonym    (1000)       38 2024-03-05 18:46:59.827119 quotesgeneratorapi-wrapper-0.2.2/setup.cfg
--rw-r--r--   0 anonym    (1000) anonym    (1000)      815 2024-03-05 18:31:12.000000 quotesgeneratorapi-wrapper-0.2.2/setup.py
+-rw-r--r--   0        0        0     1080 2024-03-05 18:28:23.204977 quotesgeneratorapi_wrapper-0.2.3/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-14 20:50:25.840847 quotesgeneratorapi_wrapper-0.2.3/README.md
+-rw-r--r--   0        0        0      301 2024-04-14 21:00:56.230023 quotesgeneratorapi_wrapper-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-14 20:50:25.840847 quotesgeneratorapi_wrapper-0.2.3/quotesgeneratorapi_wrapper/__init__.py
+-rw-r--r--   0        0        0      491 2024-04-14 21:00:47.773846 quotesgeneratorapi_wrapper-0.2.3/quotesgeneratorapi_wrapper/quotesgenerator.py
+-rw-r--r--   0        0        0      371 1970-01-01 00:00:00.000000 quotesgeneratorapi_wrapper-0.2.3/PKG-INFO
```

### Comparing `quotesgeneratorapi-wrapper-0.2.2/LICENSE` & `quotesgeneratorapi_wrapper-0.2.3/LICENSE`

 * *Files identical despite different names*

