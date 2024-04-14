# Comparing `tmp/maxondevelop-0.0.2.tar.gz` & `tmp/maxondevelop-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxondevelop-0.0.2.tar", last modified: Sun Apr 14 14:37:58 2024, max compression
+gzip compressed data, was "maxondevelop-0.0.3.tar", last modified: Sun Apr 14 14:52:09 2024, max compression
```

## Comparing `maxondevelop-0.0.2.tar` & `maxondevelop-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 maxondevelop   (501) staff       (20)        0 2024-04-14 14:37:58.799915 maxondevelop-0.0.2/
--rw-r--r--   0 maxondevelop   (501) staff       (20)     1069 2024-04-14 13:17:07.000000 maxondevelop-0.0.2/LICENSE
--rw-r--r--   0 maxondevelop   (501) staff       (20)       78 2024-04-14 14:37:58.799674 maxondevelop-0.0.2/PKG-INFO
--rw-r--r--   0 maxondevelop   (501) staff       (20)       16 2024-04-14 13:17:07.000000 maxondevelop-0.0.2/README.md
-drwxr-xr-x   0 maxondevelop   (501) staff       (20)        0 2024-04-14 14:37:58.798838 maxondevelop-0.0.2/maxondevelop/
--rw-r--r--   0 maxondevelop   (501) staff       (20)       23 2024-04-14 13:37:51.000000 maxondevelop-0.0.2/maxondevelop/__init__.py
--rw-r--r--   0 maxondevelop   (501) staff       (20)       39 2024-04-14 13:18:13.000000 maxondevelop-0.0.2/maxondevelop/main.py
-drwxr-xr-x   0 maxondevelop   (501) staff       (20)        0 2024-04-14 14:37:58.799521 maxondevelop-0.0.2/maxondevelop.egg-info/
--rw-r--r--   0 maxondevelop   (501) staff       (20)       78 2024-04-14 14:37:58.000000 maxondevelop-0.0.2/maxondevelop.egg-info/PKG-INFO
--rw-r--r--   0 maxondevelop   (501) staff       (20)      255 2024-04-14 14:37:58.000000 maxondevelop-0.0.2/maxondevelop.egg-info/SOURCES.txt
--rw-r--r--   0 maxondevelop   (501) staff       (20)        1 2024-04-14 14:37:58.000000 maxondevelop-0.0.2/maxondevelop.egg-info/dependency_links.txt
--rw-r--r--   0 maxondevelop   (501) staff       (20)       52 2024-04-14 14:37:58.000000 maxondevelop-0.0.2/maxondevelop.egg-info/entry_points.txt
--rw-r--r--   0 maxondevelop   (501) staff       (20)       13 2024-04-14 14:37:58.000000 maxondevelop-0.0.2/maxondevelop.egg-info/top_level.txt
--rw-r--r--   0 maxondevelop   (501) staff       (20)       38 2024-04-14 14:37:58.799956 maxondevelop-0.0.2/setup.cfg
--rw-r--r--   0 maxondevelop   (501) staff       (20)      233 2024-04-14 14:37:30.000000 maxondevelop-0.0.2/setup.py
+drwxr-xr-x   0 maxondevelop   (501) staff       (20)        0 2024-04-14 14:52:09.365124 maxondevelop-0.0.3/
+-rw-r--r--   0 maxondevelop   (501) staff       (20)     1069 2024-04-14 13:17:07.000000 maxondevelop-0.0.3/LICENSE
+-rw-r--r--   0 maxondevelop   (501) staff       (20)       78 2024-04-14 14:52:09.364861 maxondevelop-0.0.3/PKG-INFO
+-rw-r--r--   0 maxondevelop   (501) staff       (20)       16 2024-04-14 13:17:07.000000 maxondevelop-0.0.3/README.md
+drwxr-xr-x   0 maxondevelop   (501) staff       (20)        0 2024-04-14 14:52:09.364086 maxondevelop-0.0.3/maxondevelop/
+-rw-r--r--   0 maxondevelop   (501) staff       (20)       23 2024-04-14 13:37:51.000000 maxondevelop-0.0.3/maxondevelop/__init__.py
+-rw-r--r--   0 maxondevelop   (501) staff       (20)       39 2024-04-14 13:18:13.000000 maxondevelop-0.0.3/maxondevelop/main.py
+drwxr-xr-x   0 maxondevelop   (501) staff       (20)        0 2024-04-14 14:52:09.364669 maxondevelop-0.0.3/maxondevelop.egg-info/
+-rw-r--r--   0 maxondevelop   (501) staff       (20)       78 2024-04-14 14:52:09.000000 maxondevelop-0.0.3/maxondevelop.egg-info/PKG-INFO
+-rw-r--r--   0 maxondevelop   (501) staff       (20)      216 2024-04-14 14:52:09.000000 maxondevelop-0.0.3/maxondevelop.egg-info/SOURCES.txt
+-rw-r--r--   0 maxondevelop   (501) staff       (20)        1 2024-04-14 14:52:09.000000 maxondevelop-0.0.3/maxondevelop.egg-info/dependency_links.txt
+-rw-r--r--   0 maxondevelop   (501) staff       (20)       13 2024-04-14 14:52:09.000000 maxondevelop-0.0.3/maxondevelop.egg-info/top_level.txt
+-rw-r--r--   0 maxondevelop   (501) staff       (20)       38 2024-04-14 14:52:09.365164 maxondevelop-0.0.3/setup.cfg
+-rw-r--r--   0 maxondevelop   (501) staff       (20)      145 2024-04-14 14:50:48.000000 maxondevelop-0.0.3/setup.py
```

### Comparing `maxondevelop-0.0.2/LICENSE` & `maxondevelop-0.0.3/LICENSE`

 * *Files identical despite different names*

