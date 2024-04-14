# Comparing `tmp/python-bmob-1.5.0.tar.gz` & `tmp/python-bmob-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\python-bmob-1.5.0.tar", last modified: Thu Apr 11 14:13:27 2024, max compression
+gzip compressed data, was "dist\python-bmob-1.6.0.tar", last modified: Sun Apr 14 10:10:44 2024, max compression
```

## Comparing `python-bmob-1.5.0.tar` & `python-bmob-1.6.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 14:13:27.326959 python-bmob-1.5.0/
--rw-rw-rw-   0        0        0      280 2024-04-11 14:13:27.326959 python-bmob-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-09 14:01:42.000000 python-bmob-1.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 14:13:27.311336 python-bmob-1.5.0/bmobpy/
--rw-rw-rw-   0        0        0       25 2024-04-09 14:54:42.000000 python-bmob-1.5.0/bmobpy/__init__.py
--rw-rw-rw-   0        0        0    19427 2024-04-11 10:47:48.000000 python-bmob-1.5.0/bmobpy/bmob.py
-drwxrwxrwx   0        0        0        0 2024-04-11 14:13:27.311336 python-bmob-1.5.0/python_bmob.egg-info/
--rw-rw-rw-   0        0        0      280 2024-04-11 14:13:27.000000 python-bmob-1.5.0/python_bmob.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2024-04-11 14:13:27.000000 python-bmob-1.5.0/python_bmob.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 14:13:27.000000 python-bmob-1.5.0/python_bmob.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-11 14:13:27.000000 python-bmob-1.5.0/python_bmob.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-11 14:13:27.326959 python-bmob-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0      393 2024-04-11 14:13:09.000000 python-bmob-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 10:10:44.531114 python-bmob-1.6.0/
+-rw-rw-rw-   0        0        0      280 2024-04-14 10:10:44.531114 python-bmob-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-09 14:01:42.000000 python-bmob-1.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 10:10:44.518174 python-bmob-1.6.0/bmobpy/
+-rw-rw-rw-   0        0        0       25 2024-04-09 14:54:42.000000 python-bmob-1.6.0/bmobpy/__init__.py
+-rw-rw-rw-   0        0        0    36073 2024-04-14 10:09:23.000000 python-bmob-1.6.0/bmobpy/bmob.py
+-rw-rw-rw-   0        0        0     4364 2024-04-14 09:53:19.000000 python-bmob-1.6.0/bmobpy/test.py
+drwxrwxrwx   0        0        0        0 2024-04-14 10:10:44.530114 python-bmob-1.6.0/python_bmob.egg-info/
+-rw-rw-rw-   0        0        0      280 2024-04-14 10:10:44.000000 python-bmob-1.6.0/python_bmob.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2024-04-14 10:10:44.000000 python-bmob-1.6.0/python_bmob.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 10:10:44.000000 python-bmob-1.6.0/python_bmob.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-14 10:10:44.000000 python-bmob-1.6.0/python_bmob.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 10:10:44.531114 python-bmob-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      393 2024-04-14 10:10:30.000000 python-bmob-1.6.0/setup.py
```

