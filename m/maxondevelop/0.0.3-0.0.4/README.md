# Comparing `tmp/maxondevelop-0.0.3.tar.gz` & `tmp/maxondevelop-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maxondevelop-0.0.3.tar", last modified: Sun Apr 14 14:52:09 2024, max compression
+gzip compressed data, was "maxondevelop-0.0.4.tar", last modified: Sun Apr 14 15:22:10 2024, max compression
```

## Comparing `maxondevelop-0.0.3.tar` & `maxondevelop-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 maxondevelop   (501) staff       (20)        0 2024-04-14 14:52:09.365124 maxondevelop-0.0.3/
--rw-r--r--   0 maxondevelop   (501) staff       (20)     1069 2024-04-14 13:17:07.000000 maxondevelop-0.0.3/LICENSE
--rw-r--r--   0 maxondevelop   (501) staff       (20)       78 2024-04-14 14:52:09.364861 maxondevelop-0.0.3/PKG-INFO
--rw-r--r--   0 maxondevelop   (501) staff       (20)       16 2024-04-14 13:17:07.000000 maxondevelop-0.0.3/README.md
-drwxr-xr-x   0 maxondevelop   (501) staff       (20)        0 2024-04-14 14:52:09.364086 maxondevelop-0.0.3/maxondevelop/
--rw-r--r--   0 maxondevelop   (501) staff       (20)       23 2024-04-14 13:37:51.000000 maxondevelop-0.0.3/maxondevelop/__init__.py
--rw-r--r--   0 maxondevelop   (501) staff       (20)       39 2024-04-14 13:18:13.000000 maxondevelop-0.0.3/maxondevelop/main.py
-drwxr-xr-x   0 maxondevelop   (501) staff       (20)        0 2024-04-14 14:52:09.364669 maxondevelop-0.0.3/maxondevelop.egg-info/
--rw-r--r--   0 maxondevelop   (501) staff       (20)       78 2024-04-14 14:52:09.000000 maxondevelop-0.0.3/maxondevelop.egg-info/PKG-INFO
--rw-r--r--   0 maxondevelop   (501) staff       (20)      216 2024-04-14 14:52:09.000000 maxondevelop-0.0.3/maxondevelop.egg-info/SOURCES.txt
--rw-r--r--   0 maxondevelop   (501) staff       (20)        1 2024-04-14 14:52:09.000000 maxondevelop-0.0.3/maxondevelop.egg-info/dependency_links.txt
--rw-r--r--   0 maxondevelop   (501) staff       (20)       13 2024-04-14 14:52:09.000000 maxondevelop-0.0.3/maxondevelop.egg-info/top_level.txt
--rw-r--r--   0 maxondevelop   (501) staff       (20)       38 2024-04-14 14:52:09.365164 maxondevelop-0.0.3/setup.cfg
--rw-r--r--   0 maxondevelop   (501) staff       (20)      145 2024-04-14 14:50:48.000000 maxondevelop-0.0.3/setup.py
+drwxr-xr-x   0 maxondevelop   (501) staff       (20)        0 2024-04-14 15:22:10.563655 maxondevelop-0.0.4/
+-rw-r--r--   0 maxondevelop   (501) staff       (20)     1069 2024-04-14 13:17:07.000000 maxondevelop-0.0.4/LICENSE
+-rw-r--r--   0 maxondevelop   (501) staff       (20)       78 2024-04-14 15:22:10.563419 maxondevelop-0.0.4/PKG-INFO
+-rw-r--r--   0 maxondevelop   (501) staff       (20)       16 2024-04-14 13:17:07.000000 maxondevelop-0.0.4/README.md
+drwxr-xr-x   0 maxondevelop   (501) staff       (20)        0 2024-04-14 15:22:10.562541 maxondevelop-0.0.4/maxondevelop/
+-rw-r--r--   0 maxondevelop   (501) staff       (20)       30 2024-04-14 15:20:23.000000 maxondevelop-0.0.4/maxondevelop/__init__.py
+-rw-r--r--   0 maxondevelop   (501) staff       (20)       32 2024-04-14 15:20:37.000000 maxondevelop-0.0.4/maxondevelop/main.py
+drwxr-xr-x   0 maxondevelop   (501) staff       (20)        0 2024-04-14 15:22:10.563220 maxondevelop-0.0.4/maxondevelop.egg-info/
+-rw-r--r--   0 maxondevelop   (501) staff       (20)       78 2024-04-14 15:22:10.000000 maxondevelop-0.0.4/maxondevelop.egg-info/PKG-INFO
+-rw-r--r--   0 maxondevelop   (501) staff       (20)      216 2024-04-14 15:22:10.000000 maxondevelop-0.0.4/maxondevelop.egg-info/SOURCES.txt
+-rw-r--r--   0 maxondevelop   (501) staff       (20)        1 2024-04-14 15:22:10.000000 maxondevelop-0.0.4/maxondevelop.egg-info/dependency_links.txt
+-rw-r--r--   0 maxondevelop   (501) staff       (20)       13 2024-04-14 15:22:10.000000 maxondevelop-0.0.4/maxondevelop.egg-info/top_level.txt
+-rw-r--r--   0 maxondevelop   (501) staff       (20)       38 2024-04-14 15:22:10.563694 maxondevelop-0.0.4/setup.cfg
+-rw-r--r--   0 maxondevelop   (501) staff       (20)      145 2024-04-14 15:22:07.000000 maxondevelop-0.0.4/setup.py
```

### Comparing `maxondevelop-0.0.3/LICENSE` & `maxondevelop-0.0.4/LICENSE`

 * *Files identical despite different names*

