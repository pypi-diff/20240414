# Comparing `tmp/sprinko-0.0.12.tar.gz` & `tmp/sprinko-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprinko-0.0.12.tar", last modified: Thu Mar 14 19:46:06 2024, max compression
+gzip compressed data, was "sprinko-0.0.14.tar", last modified: Thu Mar 14 19:50:59 2024, max compression
```

## Comparing `sprinko-0.0.12.tar` & `sprinko-0.0.14.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 19:46:06.954504 sprinko-0.0.12/
--rw-rw-rw-   0        0        0     1085 2024-03-13 15:27:07.000000 sprinko-0.0.12/LICENSE
--rw-rw-rw-   0        0        0      209 2024-03-14 19:46:06.953505 sprinko-0.0.12/PKG-INFO
--rw-rw-rw-   0        0        0       10 2024-03-14 19:28:42.000000 sprinko-0.0.12/README.md
--rw-rw-rw-   0        0        0       75 2024-03-14 19:40:34.000000 sprinko-0.0.12/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-14 19:46:06.954504 sprinko-0.0.12/setup.cfg
--rw-rw-rw-   0        0        0      802 2024-03-14 19:42:20.000000 sprinko-0.0.12/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-14 19:46:06.947504 sprinko-0.0.12/sprinko/
--rw-rw-rw-   0        0        0     3009 2024-03-14 19:44:16.000000 sprinko-0.0.12/sprinko/cli.py
-drwxrwxrwx   0        0        0        0 2024-03-14 19:46:06.952504 sprinko-0.0.12/sprinko/core/
--rw-rw-rw-   0        0        0      172 2024-03-13 18:39:49.000000 sprinko-0.0.12/sprinko/core/__base__.py
--rw-rw-rw-   0        0        0      106 2024-03-14 19:45:38.000000 sprinko-0.0.12/sprinko/core/__init__.py
--rw-rw-rw-   0        0        0     1553 2024-03-14 19:45:30.000000 sprinko-0.0.12/sprinko/core/ctx.py
--rw-rw-rw-   0        0        0     8300 2024-03-14 18:50:42.000000 sprinko-0.0.12/sprinko/core/ko.py
--rw-rw-rw-   0        0        0     3676 2024-03-14 19:32:59.000000 sprinko-0.0.12/sprinko/core/sprinko.py
--rw-rw-rw-   0        0        0     1193 2024-03-13 21:55:31.000000 sprinko-0.0.12/sprinko/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-14 19:46:06.953505 sprinko-0.0.12/sprinko.egg-info/
--rw-rw-rw-   0        0        0      209 2024-03-14 19:46:06.000000 sprinko-0.0.12/sprinko.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2024-03-14 19:46:06.000000 sprinko-0.0.12/sprinko.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 19:46:06.000000 sprinko-0.0.12/sprinko.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-03-14 19:46:06.000000 sprinko-0.0.12/sprinko.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       49 2024-03-14 19:46:06.000000 sprinko-0.0.12/sprinko.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-14 19:46:06.000000 sprinko-0.0.12/sprinko.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-14 19:50:59.762679 sprinko-0.0.14/
+-rw-rw-rw-   0        0        0     1085 2024-03-13 15:27:07.000000 sprinko-0.0.14/LICENSE
+-rw-rw-rw-   0        0        0      209 2024-03-14 19:50:59.762679 sprinko-0.0.14/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2024-03-14 19:28:42.000000 sprinko-0.0.14/README.md
+-rw-rw-rw-   0        0        0       75 2024-03-14 19:40:34.000000 sprinko-0.0.14/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-03-14 19:50:59.762679 sprinko-0.0.14/setup.cfg
+-rw-rw-rw-   0        0        0      802 2024-03-14 19:42:20.000000 sprinko-0.0.14/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-14 19:50:59.756677 sprinko-0.0.14/sprinko/
+-rw-rw-rw-   0        0        0     3009 2024-03-14 19:44:16.000000 sprinko-0.0.14/sprinko/cli.py
+drwxrwxrwx   0        0        0        0 2024-03-14 19:50:59.761679 sprinko-0.0.14/sprinko/core/
+-rw-rw-rw-   0        0        0      172 2024-03-13 18:39:49.000000 sprinko-0.0.14/sprinko/core/__base__.py
+-rw-rw-rw-   0        0        0      106 2024-03-14 19:50:22.000000 sprinko-0.0.14/sprinko/core/__init__.py
+-rw-rw-rw-   0        0        0     1553 2024-03-14 19:45:30.000000 sprinko-0.0.14/sprinko/core/ctx.py
+-rw-rw-rw-   0        0        0     8300 2024-03-14 18:50:42.000000 sprinko-0.0.14/sprinko/core/ko.py
+-rw-rw-rw-   0        0        0     3676 2024-03-14 19:32:59.000000 sprinko-0.0.14/sprinko/core/sprinko.py
+-rw-rw-rw-   0        0        0     1193 2024-03-13 21:55:31.000000 sprinko-0.0.14/sprinko/utils.py
+drwxrwxrwx   0        0        0        0 2024-03-14 19:50:59.761679 sprinko-0.0.14/sprinko.egg-info/
+-rw-rw-rw-   0        0        0      209 2024-03-14 19:50:59.000000 sprinko-0.0.14/sprinko.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2024-03-14 19:50:59.000000 sprinko-0.0.14/sprinko.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-14 19:50:59.000000 sprinko-0.0.14/sprinko.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-03-14 19:50:59.000000 sprinko-0.0.14/sprinko.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       49 2024-03-14 19:50:59.000000 sprinko-0.0.14/sprinko.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-03-14 19:50:59.000000 sprinko-0.0.14/sprinko.egg-info/top_level.txt
```

### Comparing `sprinko-0.0.12/LICENSE` & `sprinko-0.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `sprinko-0.0.12/setup.py` & `sprinko-0.0.14/setup.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.0.12/sprinko/cli.py` & `sprinko-0.0.14/sprinko/cli.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.0.12/sprinko/core/ctx.py` & `sprinko-0.0.14/sprinko/core/ctx.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.0.12/sprinko/core/ko.py` & `sprinko-0.0.14/sprinko/core/ko.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.0.12/sprinko/core/sprinko.py` & `sprinko-0.0.14/sprinko/core/sprinko.py`

 * *Files identical despite different names*

### Comparing `sprinko-0.0.12/sprinko/utils.py` & `sprinko-0.0.14/sprinko/utils.py`

 * *Files identical despite different names*

