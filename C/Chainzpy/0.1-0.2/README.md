# Comparing `tmp/Chainzpy-0.1.tar.gz` & `tmp/Chainzpy-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Chainzpy-0.1.tar", last modified: Sun Apr 14 07:35:05 2024, max compression
+gzip compressed data, was "Chainzpy-0.2.tar", last modified: Sun Apr 14 17:16:00 2024, max compression
```

## Comparing `Chainzpy-0.1.tar` & `Chainzpy-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-14 07:35:05.822807 Chainzpy-0.1/
-drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-14 07:35:05.820649 Chainzpy-0.1/Chainzpy/
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      286 2024-04-14 07:31:35.000000 Chainzpy-0.1/Chainzpy/__init__.py
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)     3440 2024-04-14 07:28:23.000000 Chainzpy-0.1/Chainzpy/main.py
-drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-14 07:35:05.822057 Chainzpy-0.1/Chainzpy.egg-info/
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)       93 2024-04-14 07:35:05.000000 Chainzpy-0.1/Chainzpy.egg-info/PKG-INFO
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      215 2024-04-14 07:35:05.000000 Chainzpy-0.1/Chainzpy.egg-info/SOURCES.txt
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        1 2024-04-14 07:35:05.000000 Chainzpy-0.1/Chainzpy.egg-info/dependency_links.txt
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)       13 2024-04-14 07:35:05.000000 Chainzpy-0.1/Chainzpy.egg-info/requires.txt
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        9 2024-04-14 07:35:05.000000 Chainzpy-0.1/Chainzpy.egg-info/top_level.txt
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)       93 2024-04-14 07:35:05.822375 Chainzpy-0.1/PKG-INFO
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-14 07:29:26.000000 Chainzpy-0.1/README.md
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)       38 2024-04-14 07:35:05.822885 Chainzpy-0.1/setup.cfg
--rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      186 2024-04-14 07:33:30.000000 Chainzpy-0.1/setup.py
+drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-14 17:16:00.469199 Chainzpy-0.2/
+drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-14 17:16:00.466875 Chainzpy-0.2/Chainzpy/
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      328 2024-04-14 17:14:47.000000 Chainzpy-0.2/Chainzpy/__init__.py
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)     3440 2024-04-14 17:15:15.000000 Chainzpy-0.2/Chainzpy/main.py
+drwxr-xr-x   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-14 17:16:00.468407 Chainzpy-0.2/Chainzpy.egg-info/
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      148 2024-04-14 17:16:00.000000 Chainzpy-0.2/Chainzpy.egg-info/PKG-INFO
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      215 2024-04-14 17:16:00.000000 Chainzpy-0.2/Chainzpy.egg-info/SOURCES.txt
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        1 2024-04-14 17:16:00.000000 Chainzpy-0.2/Chainzpy.egg-info/dependency_links.txt
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)       13 2024-04-14 17:16:00.000000 Chainzpy-0.2/Chainzpy.egg-info/requires.txt
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        9 2024-04-14 17:16:00.000000 Chainzpy-0.2/Chainzpy.egg-info/top_level.txt
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      148 2024-04-14 17:16:00.468730 Chainzpy-0.2/PKG-INFO
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)        0 2024-04-14 07:29:26.000000 Chainzpy-0.2/README.md
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)       38 2024-04-14 17:16:00.469268 Chainzpy-0.2/setup.cfg
+-rw-r--r--   0 alexanderwilkerson   (501) staff       (20)      251 2024-04-14 17:15:06.000000 Chainzpy-0.2/setup.py
```

### Comparing `Chainzpy-0.1/Chainzpy/main.py` & `Chainzpy-0.2/Chainzpy/main.py`

 * *Files identical despite different names*

