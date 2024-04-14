# Comparing `tmp/scmopy-0.0.1.tar.gz` & `tmp/scmopy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scmopy-0.0.1.tar", last modified: Mon Mar 18 08:59:01 2024, max compression
+gzip compressed data, was "scmopy-0.0.2.tar", last modified: Sun Apr 14 18:20:40 2024, max compression
```

## Comparing `scmopy-0.0.1.tar` & `scmopy-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,23 @@
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-03-18 08:59:01.633151 scmopy-0.0.1/
--rw-r--r--   0 soli      (1000) soli      (1000)       82 2024-03-18 08:59:01.633151 scmopy-0.0.1/PKG-INFO
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-03-18 08:59:01.633151 scmopy-0.0.1/scmopy.egg-info/
--rw-r--r--   0 soli      (1000) soli      (1000)       82 2024-03-18 08:59:01.000000 scmopy-0.0.1/scmopy.egg-info/PKG-INFO
--rw-r--r--   0 soli      (1000) soli      (1000)      128 2024-03-18 08:59:01.000000 scmopy-0.0.1/scmopy.egg-info/SOURCES.txt
--rw-r--r--   0 soli      (1000) soli      (1000)        1 2024-03-18 08:59:01.000000 scmopy-0.0.1/scmopy.egg-info/dependency_links.txt
--rw-r--r--   0 soli      (1000) soli      (1000)        1 2024-03-18 08:59:01.000000 scmopy-0.0.1/scmopy.egg-info/top_level.txt
--rw-r--r--   0 soli      (1000) soli      (1000)       38 2024-03-18 08:59:01.633151 scmopy-0.0.1/setup.cfg
--rw-r--r--   0 soli      (1000) soli      (1000)      207 2024-03-18 08:58:01.000000 scmopy-0.0.1/setup.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 18:20:40.766681 scmopy-0.0.2/
+-rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-30 13:55:39.000000 scmopy-0.0.2/LICENSE
+-rw-r--r--   0 soli      (1000) soli      (1000)       85 2024-04-14 17:50:35.000000 scmopy-0.0.2/MANIFEST.in
+-rw-r--r--   0 soli      (1000) soli      (1000)    21230 2024-04-14 18:20:40.766681 scmopy-0.0.2/PKG-INFO
+-rw-r--r--   0 soli      (1000) soli      (1000)    20914 2024-04-14 18:14:26.000000 scmopy-0.0.2/README.md
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 18:20:40.766681 scmopy-0.0.2/scmopy/
+-rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-30 10:40:19.000000 scmopy-0.0.2/scmopy/LICENSE
+-rw-r--r--   0 soli      (1000) soli      (1000)      891 2024-04-14 18:20:01.000000 scmopy-0.0.2/scmopy/__init__.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     2036 2024-04-14 17:43:02.000000 scmopy-0.0.2/scmopy/base.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 18:20:40.766681 scmopy-0.0.2/scmopy/components/
+-rw-r--r--   0 soli      (1000) soli      (1000)      905 2024-04-14 17:41:40.000000 scmopy-0.0.2/scmopy/components/__init__.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     5517 2024-04-14 17:42:11.000000 scmopy-0.0.2/scmopy/components/syniv.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     7089 2024-04-14 17:43:09.000000 scmopy-0.0.2/scmopy/gaussian_scm.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     5227 2024-04-14 17:43:16.000000 scmopy-0.0.2/scmopy/model_selection.py
+-rw-r--r--   0 soli      (1000) soli      (1000)    14355 2024-04-14 17:43:56.000000 scmopy-0.0.2/scmopy/nongaussian_scm.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 18:20:40.766681 scmopy-0.0.2/scmopy.egg-info/
+-rw-r--r--   0 soli      (1000) soli      (1000)    21230 2024-04-14 18:20:40.000000 scmopy-0.0.2/scmopy.egg-info/PKG-INFO
+-rw-r--r--   0 soli      (1000) soli      (1000)      368 2024-04-14 18:20:40.000000 scmopy-0.0.2/scmopy.egg-info/SOURCES.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)        1 2024-04-14 18:20:40.000000 scmopy-0.0.2/scmopy.egg-info/dependency_links.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)       19 2024-04-14 18:20:40.000000 scmopy-0.0.2/scmopy.egg-info/requires.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)        7 2024-04-14 18:20:40.000000 scmopy-0.0.2/scmopy.egg-info/top_level.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)       38 2024-04-14 18:20:40.766681 scmopy-0.0.2/setup.cfg
+-rw-r--r--   0 soli      (1000) soli      (1000)     1542 2024-04-14 18:20:12.000000 scmopy-0.0.2/setup.py
```

