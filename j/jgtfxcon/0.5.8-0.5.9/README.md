# Comparing `tmp/jgtfxcon-0.5.8.tar.gz` & `tmp/jgtfxcon-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jgtfxcon-0.5.8.tar", last modified: Tue Mar 26 03:54:49 2024, max compression
+gzip compressed data, was "jgtfxcon-0.5.9.tar", last modified: Tue Mar 26 23:25:49 2024, max compression
```

## Comparing `jgtfxcon-0.5.8.tar` & `jgtfxcon-0.5.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-03-26 03:54:49.948967 jgtfxcon-0.5.8/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/LICENSE
--rw-r--r--   0 jgi       (1000) jgi       (1000)     2203 2024-03-26 03:54:49.948967 jgtfxcon-0.5.8/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      666 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/README.md
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      345 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/README.rst
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-03-26 03:54:49.940967 jgtfxcon-0.5.8/jgtfxcon/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     5560 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/JGTCloudFS.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1423 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/JGTConfig.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     3207 2024-03-26 03:54:46.000000 jgtfxcon-0.5.8/jgtfxcon/JGTCore.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2586 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/JGTImage.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      269 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/JGTLoader.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     9417 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/JGTPDHelper.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)    14561 2024-03-26 03:54:00.000000 jgtfxcon-0.5.8/jgtfxcon/JGTPDS.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      384 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/JGTPDS.test.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     5906 2024-03-16 21:59:27.000000 jgtfxcon-0.5.8/jgtfxcon/JGTPDSSvc.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     4656 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/__init__.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        5 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/__main__.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     4058 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/dl_properties.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-03-26 03:54:49.944967 jgtfxcon-0.5.8/jgtfxcon/forexconnect/
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1649 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/forexconnect/EachRowListener.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)    25755 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/forexconnect/ForexConnect.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     9925 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/forexconnect/LiveHistory.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     8003 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/forexconnect/ResponseListener.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     4783 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/forexconnect/SessionStatusListener.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     5900 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/forexconnect/TableListener.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     3121 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/forexconnect/TableManagerListener.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2125 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/forexconnect/__init__.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)    19128 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/forexconnect/common.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      931 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/forexconnect/errors.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      437 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/forexconnect/x-pyd.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1214 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/fsserver.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)    25491 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/iprops.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      723 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/jgt2312.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2090 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/jgtbtetl1.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     4495 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/jgtbtetl2.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2901 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/jgtdotenv.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1400 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/jgtetl.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       36 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/jgtflags.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     9156 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/jgtfxc.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      282 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/jgtfxc.test.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     3942 2024-03-16 21:57:26.000000 jgtfxcon-0.5.8/jgtfxcon/jgtfxcli.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)    31434 2024-03-16 20:05:07.000000 jgtfxcon-0.5.8/jgtfxcon/jgtfxcommon.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     4626 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/pdsserver.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        0 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/test_JGTPDS.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2012 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/test_jgtfxc.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      673 2024-01-14 01:04:03.000000 jgtfxcon-0.5.8/jgtfxcon/wsl-run-command.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-03-26 03:54:49.944967 jgtfxcon-0.5.8/jgtfxcon.egg-info/
--rw-r--r--   0 jgi       (1000) jgi       (1000)     2203 2024-03-26 03:54:49.000000 jgtfxcon-0.5.8/jgtfxcon.egg-info/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1292 2024-03-26 03:54:49.000000 jgtfxcon-0.5.8/jgtfxcon.egg-info/SOURCES.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-03-26 03:54:49.000000 jgtfxcon-0.5.8/jgtfxcon.egg-info/dependency_links.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       52 2024-03-26 03:54:49.000000 jgtfxcon-0.5.8/jgtfxcon.egg-info/entry_points.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      342 2024-03-26 03:54:49.000000 jgtfxcon-0.5.8/jgtfxcon.egg-info/requires.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        9 2024-03-26 03:54:49.000000 jgtfxcon-0.5.8/jgtfxcon.egg-info/top_level.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      697 2024-03-26 03:54:46.000000 jgtfxcon-0.5.8/pyproject.toml
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      103 2024-03-26 03:54:49.948967 jgtfxcon-0.5.8/setup.cfg
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1770 2024-03-26 02:12:56.000000 jgtfxcon-0.5.8/setup.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-03-26 23:25:49.394066 jgtfxcon-0.5.9/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1086 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/LICENSE
+-rw-r--r--   0 jgi       (1000) jgi       (1000)     2203 2024-03-26 23:25:49.394066 jgtfxcon-0.5.9/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      666 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/README.md
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      345 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/README.rst
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-03-26 23:25:49.386066 jgtfxcon-0.5.9/jgtfxcon/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     5560 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/JGTCloudFS.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1423 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/JGTConfig.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     3207 2024-03-26 23:25:44.000000 jgtfxcon-0.5.9/jgtfxcon/JGTCore.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2586 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/JGTImage.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      269 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/JGTLoader.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     9417 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/JGTPDHelper.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)    14561 2024-03-26 03:54:00.000000 jgtfxcon-0.5.9/jgtfxcon/JGTPDS.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      384 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/JGTPDS.test.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     5906 2024-03-16 21:59:27.000000 jgtfxcon-0.5.9/jgtfxcon/JGTPDSSvc.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     4656 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/__init__.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        5 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/__main__.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     4058 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/dl_properties.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-03-26 23:25:49.390066 jgtfxcon-0.5.9/jgtfxcon/forexconnect/
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1649 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/forexconnect/EachRowListener.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)    25755 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/forexconnect/ForexConnect.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     9925 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/forexconnect/LiveHistory.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     8003 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/forexconnect/ResponseListener.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     4783 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/forexconnect/SessionStatusListener.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     5900 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/forexconnect/TableListener.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     3121 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/forexconnect/TableManagerListener.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2125 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/forexconnect/__init__.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)    19128 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/forexconnect/common.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      931 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/forexconnect/errors.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      437 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/forexconnect/x-pyd.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1214 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/fsserver.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)    25491 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/iprops.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      723 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/jgt2312.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2090 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/jgtbtetl1.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     4495 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/jgtbtetl2.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2901 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/jgtdotenv.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1400 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/jgtetl.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       36 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/jgtflags.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     9156 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/jgtfxc.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      282 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/jgtfxc.test.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     3942 2024-03-16 21:57:26.000000 jgtfxcon-0.5.9/jgtfxcon/jgtfxcli.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)    31434 2024-03-16 20:05:07.000000 jgtfxcon-0.5.9/jgtfxcon/jgtfxcommon.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     4626 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/pdsserver.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        0 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/test_JGTPDS.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2012 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/test_jgtfxc.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      673 2024-01-14 01:04:03.000000 jgtfxcon-0.5.9/jgtfxcon/wsl-run-command.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-03-26 23:25:49.390066 jgtfxcon-0.5.9/jgtfxcon.egg-info/
+-rw-r--r--   0 jgi       (1000) jgi       (1000)     2203 2024-03-26 23:25:49.000000 jgtfxcon-0.5.9/jgtfxcon.egg-info/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1292 2024-03-26 23:25:49.000000 jgtfxcon-0.5.9/jgtfxcon.egg-info/SOURCES.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-03-26 23:25:49.000000 jgtfxcon-0.5.9/jgtfxcon.egg-info/dependency_links.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       52 2024-03-26 23:25:49.000000 jgtfxcon-0.5.9/jgtfxcon.egg-info/entry_points.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      342 2024-03-26 23:25:49.000000 jgtfxcon-0.5.9/jgtfxcon.egg-info/requires.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        9 2024-03-26 23:25:49.000000 jgtfxcon-0.5.9/jgtfxcon.egg-info/top_level.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      689 2024-03-26 23:25:44.000000 jgtfxcon-0.5.9/pyproject.toml
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      103 2024-03-26 23:25:49.394066 jgtfxcon-0.5.9/setup.cfg
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1770 2024-03-26 23:25:22.000000 jgtfxcon-0.5.9/setup.py
```

### Comparing `jgtfxcon-0.5.8/LICENSE` & `jgtfxcon-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/PKG-INFO` & `jgtfxcon-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jgtfxcon
-Version: 0.5.8
+Version: 0.5.9
 Summary: PDS Services
 Home-page: https://github.com/jgwill/jgtfxcon
 Author: GUillaume Isabelle
 Author-email: Guillaume Isabelle <jgi@jgwill.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jgwill/jgtfxcon
 Project-URL: Bug Tracker, https://github.com/jgwill/jgtfxcon/issues
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas>=0.25.1
 Requires-Dist: python-dotenv>=0.19.2
-Requires-Dist: jgtutils>=0.1.46
+Requires-Dist: jgtutils>=0.1.47
 Requires-Dist: jgtfx2console
 Requires-Dist: tlid
 Requires-Dist: flask
 Provides-Extra: dev
 Requires-Dist: flake8<3.7.0,>=3.6.0; extra == "dev"
 Requires-Dist: isort<4.4.0,>=4.3.4; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
```

### Comparing `jgtfxcon-0.5.8/README.md` & `jgtfxcon-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/JGTCloudFS.py` & `jgtfxcon-0.5.9/jgtfxcon/JGTCloudFS.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/JGTConfig.py` & `jgtfxcon-0.5.9/jgtfxcon/JGTConfig.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/JGTCore.py` & `jgtfxcon-0.5.9/jgtfxcon/JGTCore.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from collections import namedtuple
 from json import JSONEncoder
 import os
 import pathlib
 from pathlib import Path
 import pandas as pd
 
-__version__ = "0.5.8"
+__version__ = "0.5.9"
 
 from datetime import datetime
 from datetime import timedelta
 
 
 def offsetdt(
     time_str,
```

### Comparing `jgtfxcon-0.5.8/jgtfxcon/JGTImage.py` & `jgtfxcon-0.5.9/jgtfxcon/JGTImage.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/JGTPDHelper.py` & `jgtfxcon-0.5.9/jgtfxcon/JGTPDHelper.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/JGTPDS.py` & `jgtfxcon-0.5.9/jgtfxcon/JGTPDS.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/JGTPDSSvc.py` & `jgtfxcon-0.5.9/jgtfxcon/JGTPDSSvc.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/__init__.py` & `jgtfxcon-0.5.9/jgtfxcon/__init__.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/dl_properties.py` & `jgtfxcon-0.5.9/jgtfxcon/dl_properties.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/forexconnect/EachRowListener.py` & `jgtfxcon-0.5.9/jgtfxcon/forexconnect/EachRowListener.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/forexconnect/ForexConnect.py` & `jgtfxcon-0.5.9/jgtfxcon/forexconnect/ForexConnect.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/forexconnect/LiveHistory.py` & `jgtfxcon-0.5.9/jgtfxcon/forexconnect/LiveHistory.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/forexconnect/ResponseListener.py` & `jgtfxcon-0.5.9/jgtfxcon/forexconnect/ResponseListener.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/forexconnect/SessionStatusListener.py` & `jgtfxcon-0.5.9/jgtfxcon/forexconnect/SessionStatusListener.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/forexconnect/TableListener.py` & `jgtfxcon-0.5.9/jgtfxcon/forexconnect/TableListener.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/forexconnect/TableManagerListener.py` & `jgtfxcon-0.5.9/jgtfxcon/forexconnect/TableManagerListener.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/forexconnect/__init__.py` & `jgtfxcon-0.5.9/jgtfxcon/forexconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/forexconnect/common.py` & `jgtfxcon-0.5.9/jgtfxcon/forexconnect/common.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/forexconnect/errors.py` & `jgtfxcon-0.5.9/jgtfxcon/forexconnect/errors.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/fsserver.py` & `jgtfxcon-0.5.9/jgtfxcon/fsserver.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/iprops.py` & `jgtfxcon-0.5.9/jgtfxcon/iprops.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/jgt2312.py` & `jgtfxcon-0.5.9/jgtfxcon/jgt2312.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/jgtbtetl1.py` & `jgtfxcon-0.5.9/jgtfxcon/jgtbtetl1.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/jgtbtetl2.py` & `jgtfxcon-0.5.9/jgtfxcon/jgtbtetl2.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/jgtdotenv.py` & `jgtfxcon-0.5.9/jgtfxcon/jgtdotenv.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/jgtetl.py` & `jgtfxcon-0.5.9/jgtfxcon/jgtetl.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/jgtfxc.py` & `jgtfxcon-0.5.9/jgtfxcon/jgtfxc.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/jgtfxcli.py` & `jgtfxcon-0.5.9/jgtfxcon/jgtfxcli.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/jgtfxcommon.py` & `jgtfxcon-0.5.9/jgtfxcon/jgtfxcommon.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/pdsserver.py` & `jgtfxcon-0.5.9/jgtfxcon/pdsserver.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/test_jgtfxc.py` & `jgtfxcon-0.5.9/jgtfxcon/test_jgtfxc.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon/wsl-run-command.py` & `jgtfxcon-0.5.9/jgtfxcon/wsl-run-command.py`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/jgtfxcon.egg-info/PKG-INFO` & `jgtfxcon-0.5.9/jgtfxcon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jgtfxcon
-Version: 0.5.8
+Version: 0.5.9
 Summary: PDS Services
 Home-page: https://github.com/jgwill/jgtfxcon
 Author: GUillaume Isabelle
 Author-email: Guillaume Isabelle <jgi@jgwill.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jgwill/jgtfxcon
 Project-URL: Bug Tracker, https://github.com/jgwill/jgtfxcon/issues
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas>=0.25.1
 Requires-Dist: python-dotenv>=0.19.2
-Requires-Dist: jgtutils>=0.1.46
+Requires-Dist: jgtutils>=0.1.47
 Requires-Dist: jgtfx2console
 Requires-Dist: tlid
 Requires-Dist: flask
 Provides-Extra: dev
 Requires-Dist: flake8<3.7.0,>=3.6.0; extra == "dev"
 Requires-Dist: isort<4.4.0,>=4.3.4; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
```

### Comparing `jgtfxcon-0.5.8/jgtfxcon.egg-info/SOURCES.txt` & `jgtfxcon-0.5.9/jgtfxcon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jgtfxcon-0.5.8/pyproject.toml` & `jgtfxcon-0.5.9/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,29 @@
 [build-system]
-requires = ["setuptools>=40.8.0","wheel"]
+requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jgtfxcon"
-version = "0.5.8"
-authors = [
-  { name="Guillaume Isabelle", email="jgi@jgwill.com" },
-]
+version = "0.5.9"
+authors = [{ name = "Guillaume Isabelle", email = "jgi@jgwill.com" }]
 
 description = "PDS Services"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
   'pandas>=0.25.1',
   'python-dotenv>=0.19.2',
-  'jgtutils>=0.1.46',
+  'jgtutils>=0.1.47',
   'jgtfx2console',
   'tlid',
-  'flask'
-]	
+  'flask',
+]
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/jgwill/jgtfxcon"
 "Bug Tracker" = "https://github.com/jgwill/jgtfxcon/issues"
-
-
```

### Comparing `jgtfxcon-0.5.8/setup.py` & `jgtfxcon-0.5.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 
 
 INSTALL_REQUIRES = [
     'pandas>=0.25.1',
     'python-dotenv>=0.19.2',
-    'jgtutils>=0.1.46',
+    'jgtutils>=0.1.47',
     'jgtfx2console',
     'tlid',
     'flask'
 ]
 
 EXTRAS_DEV_LINT = [
     "flake8>=3.6.0,<3.7.0",
```

