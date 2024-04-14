# Comparing `tmp/jgtpy-0.4.8.tar.gz` & `tmp/jgtpy-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jgtpy-0.4.8.tar", last modified: Fri Mar  8 15:24:52 2024, max compression
+gzip compressed data, was "jgtpy-0.4.9.tar", last modified: Fri Mar  8 15:27:43 2024, max compression
```

## Comparing `jgtpy-0.4.8.tar` & `jgtpy-0.4.9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-03-08 15:24:52.742234 jgtpy-0.4.8/
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)       45 2024-03-08 01:55:02.000000 jgtpy-0.4.8/AUTHORS
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)     1066 2024-01-14 01:10:05.000000 jgtpy-0.4.8/LICENSE
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)      152 2024-01-14 01:10:05.000000 jgtpy-0.4.8/MANIFEST.in
--rw-r--r--   0 jgi       (1000) jgi       (1000)     2751 2024-03-08 15:24:52.742234 jgtpy-0.4.8/PKG-INFO
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)      779 2024-01-14 01:10:39.000000 jgtpy-0.4.8/README.md
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)      755 2024-01-14 01:10:05.000000 jgtpy-0.4.8/README.rst
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-03-08 15:24:52.734234 jgtpy-0.4.8/jgtpy/
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)    38564 2024-03-08 11:57:20.000000 jgtpy-0.4.8/jgtpy/JGTADS.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     3284 2024-03-08 07:39:02.000000 jgtpy-0.4.8/jgtpy/JGTADSRequest.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      193 2024-03-08 07:39:18.000000 jgtpy-0.4.8/jgtpy/JGTBaseRequest.py
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)    11461 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/JGTCDS.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      166 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/JGTCDS.test.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      438 2024-03-08 07:39:36.000000 jgtpy-0.4.8/jgtpy/JGTCDSRequest.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     8396 2024-03-08 07:39:11.000000 jgtpy-0.4.8/jgtpy/JGTChartConfig.py
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)     5552 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/JGTCloudFS.py
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)     1970 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/JGTConfig.py
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)     3003 2024-03-08 15:24:44.000000 jgtpy-0.4.8/jgtpy/JGTCore.py
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)    38355 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/JGTIDS.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     5175 2024-03-08 07:39:29.000000 jgtpy-0.4.8/jgtpy/JGTIDSRequest.py
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)     2586 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/JGTImage.py
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)      269 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/JGTLoader.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)    17415 2024-03-08 15:07:09.000000 jgtpy-0.4.8/jgtpy/JGTMKSG.py
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)     9417 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/JGTPDHelper.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)    10326 2024-03-08 15:02:30.000000 jgtpy-0.4.8/jgtpy/JGTPDSP.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1660 2024-03-08 08:00:24.000000 jgtpy-0.4.8/jgtpy/JGTPDSRequest.py
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)     2789 2024-03-08 06:55:56.000000 jgtpy-0.4.8/jgtpy/__init__.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        5 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/__main__.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     6106 2024-03-08 06:44:42.000000 jgtpy-0.4.8/jgtpy/adshelper.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     4300 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/aohelper.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     5596 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/fe-formulation_of_target_variable_for_ML_in_FTS.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1245 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/fsserver.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     3147 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/idsserver.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      723 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/jgt2312.py
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)     1996 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/jgtbtetl1.py
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)     4495 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/jgtbtetl2.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     5527 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/jgtcli.py
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)     2901 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/jgtdotenv.py
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)     1400 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/jgtetl.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       36 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/jgtflags.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2550 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/pdsclient.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2927 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/pto-panel-240209.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2359 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/pto__ao_divergence_finder.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      816 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/pto_featdim5.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      365 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/pto_feathelper.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2311 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/test_JGTADS.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1625 2024-03-08 04:25:54.000000 jgtpy-0.4.8/jgtpy/test_JGTIDS.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        0 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/test_JGTPDSP.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1471 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/test_jgtcli.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     2787 2024-03-08 04:26:47.000000 jgtpy-0.4.8/jgtpy/test_jgtcommon.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      512 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/test_jgtos.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1569 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/test_jgtwslhelper.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)   193650 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/testmock_IDS.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      711 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/testpdsclient-cli.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      893 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/testpdsclient-h.py
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1088 2024-03-08 01:59:24.000000 jgtpy-0.4.8/jgtpy/testpdsclient-iprop.py
-drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-03-08 15:24:52.738234 jgtpy-0.4.8/jgtpy.egg-info/
--rw-r--r--   0 jgi       (1000) jgi       (1000)     2751 2024-03-08 15:24:52.000000 jgtpy-0.4.8/jgtpy.egg-info/PKG-INFO
--rw-rw-r--   0 jgi       (1000) jgi       (1000)     1291 2024-03-08 15:24:52.000000 jgtpy-0.4.8/jgtpy.egg-info/SOURCES.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-03-08 15:24:52.000000 jgtpy-0.4.8/jgtpy.egg-info/dependency_links.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)       74 2024-03-08 15:24:52.000000 jgtpy-0.4.8/jgtpy.egg-info/entry_points.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)      540 2024-03-08 15:24:52.000000 jgtpy-0.4.8/jgtpy.egg-info/requires.txt
--rw-rw-r--   0 jgi       (1000) jgi       (1000)        6 2024-03-08 15:24:52.000000 jgtpy-0.4.8/jgtpy.egg-info/top_level.txt
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)      879 2024-03-08 15:24:44.000000 jgtpy-0.4.8/pyproject.toml
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)      103 2024-03-08 15:24:52.742234 jgtpy-0.4.8/setup.cfg
--rwxrwxr-x   0 jgi       (1000) jgi       (1000)     2006 2024-03-08 01:55:24.000000 jgtpy-0.4.8/setup.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-03-08 15:27:43.517258 jgtpy-0.4.9/
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)       45 2024-03-08 01:55:02.000000 jgtpy-0.4.9/AUTHORS
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)     1066 2024-01-14 01:10:05.000000 jgtpy-0.4.9/LICENSE
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)      152 2024-01-14 01:10:05.000000 jgtpy-0.4.9/MANIFEST.in
+-rw-r--r--   0 jgi       (1000) jgi       (1000)     2751 2024-03-08 15:27:43.517258 jgtpy-0.4.9/PKG-INFO
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)      779 2024-01-14 01:10:39.000000 jgtpy-0.4.9/README.md
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)      755 2024-01-14 01:10:05.000000 jgtpy-0.4.9/README.rst
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-03-08 15:27:43.509258 jgtpy-0.4.9/jgtpy/
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)    38564 2024-03-08 11:57:20.000000 jgtpy-0.4.9/jgtpy/JGTADS.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     3284 2024-03-08 07:39:02.000000 jgtpy-0.4.9/jgtpy/JGTADSRequest.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      193 2024-03-08 07:39:18.000000 jgtpy-0.4.9/jgtpy/JGTBaseRequest.py
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)    11461 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/JGTCDS.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      166 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/JGTCDS.test.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      438 2024-03-08 07:39:36.000000 jgtpy-0.4.9/jgtpy/JGTCDSRequest.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     8396 2024-03-08 07:39:11.000000 jgtpy-0.4.9/jgtpy/JGTChartConfig.py
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)     5552 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/JGTCloudFS.py
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)     1970 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/JGTConfig.py
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)     3003 2024-03-08 15:27:35.000000 jgtpy-0.4.9/jgtpy/JGTCore.py
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)    38355 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/JGTIDS.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     5175 2024-03-08 07:39:29.000000 jgtpy-0.4.9/jgtpy/JGTIDSRequest.py
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)     2586 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/JGTImage.py
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)      269 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/JGTLoader.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)    17415 2024-03-08 15:07:09.000000 jgtpy-0.4.9/jgtpy/JGTMKSG.py
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)     9417 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/JGTPDHelper.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)    10326 2024-03-08 15:02:30.000000 jgtpy-0.4.9/jgtpy/JGTPDSP.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1660 2024-03-08 08:00:24.000000 jgtpy-0.4.9/jgtpy/JGTPDSRequest.py
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)     2789 2024-03-08 06:55:56.000000 jgtpy-0.4.9/jgtpy/__init__.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        5 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/__main__.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     6106 2024-03-08 06:44:42.000000 jgtpy-0.4.9/jgtpy/adshelper.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     4300 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/aohelper.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     5596 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/fe-formulation_of_target_variable_for_ML_in_FTS.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1245 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/fsserver.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     3147 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/idsserver.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      723 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/jgt2312.py
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)     1996 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/jgtbtetl1.py
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)     4495 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/jgtbtetl2.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     5527 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/jgtcli.py
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)     2901 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/jgtdotenv.py
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)     1400 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/jgtetl.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       36 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/jgtflags.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2550 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/pdsclient.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2927 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/pto-panel-240209.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2359 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/pto__ao_divergence_finder.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      816 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/pto_featdim5.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      365 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/pto_feathelper.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2311 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/test_JGTADS.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1625 2024-03-08 04:25:54.000000 jgtpy-0.4.9/jgtpy/test_JGTIDS.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        0 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/test_JGTPDSP.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1471 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/test_jgtcli.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     2787 2024-03-08 04:26:47.000000 jgtpy-0.4.9/jgtpy/test_jgtcommon.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      512 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/test_jgtos.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1569 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/test_jgtwslhelper.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)   193650 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/testmock_IDS.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      711 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/testpdsclient-cli.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      893 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/testpdsclient-h.py
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1088 2024-03-08 01:59:24.000000 jgtpy-0.4.9/jgtpy/testpdsclient-iprop.py
+drwxrwxr-x   0 jgi       (1000) jgi       (1000)        0 2024-03-08 15:27:43.513258 jgtpy-0.4.9/jgtpy.egg-info/
+-rw-r--r--   0 jgi       (1000) jgi       (1000)     2751 2024-03-08 15:27:43.000000 jgtpy-0.4.9/jgtpy.egg-info/PKG-INFO
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)     1291 2024-03-08 15:27:43.000000 jgtpy-0.4.9/jgtpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        1 2024-03-08 15:27:43.000000 jgtpy-0.4.9/jgtpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)       74 2024-03-08 15:27:43.000000 jgtpy-0.4.9/jgtpy.egg-info/entry_points.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)      540 2024-03-08 15:27:43.000000 jgtpy-0.4.9/jgtpy.egg-info/requires.txt
+-rw-rw-r--   0 jgi       (1000) jgi       (1000)        6 2024-03-08 15:27:43.000000 jgtpy-0.4.9/jgtpy.egg-info/top_level.txt
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)      879 2024-03-08 15:27:35.000000 jgtpy-0.4.9/pyproject.toml
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)      103 2024-03-08 15:27:43.517258 jgtpy-0.4.9/setup.cfg
+-rwxrwxr-x   0 jgi       (1000) jgi       (1000)     2044 2024-03-08 15:27:21.000000 jgtpy-0.4.9/setup.py
```

### Comparing `jgtpy-0.4.8/LICENSE` & `jgtpy-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/PKG-INFO` & `jgtpy-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jgtpy
-Version: 0.4.8
+Version: 0.4.9
 Summary: Enhanced JGTPy CDS, IDS, PDSP Services
 Home-page: https://github.com/jgwill/jgtpy
 Author: GUillaume Isabelle
 Author-email: Guillaume Isabelle <jgi@jgwill.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jgwill/jgtpy
 Project-URL: Bug Tracker, https://github.com/jgwill/jgtpy/issues
```

### Comparing `jgtpy-0.4.8/README.md` & `jgtpy-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/README.rst` & `jgtpy-0.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/JGTADS.py` & `jgtpy-0.4.9/jgtpy/JGTADS.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/JGTADSRequest.py` & `jgtpy-0.4.9/jgtpy/JGTADSRequest.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/JGTCDS.py` & `jgtpy-0.4.9/jgtpy/JGTCDS.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/JGTChartConfig.py` & `jgtpy-0.4.9/jgtpy/JGTChartConfig.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/JGTCloudFS.py` & `jgtpy-0.4.9/jgtpy/JGTCloudFS.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/JGTConfig.py` & `jgtpy-0.4.9/jgtpy/JGTConfig.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/JGTCore.py` & `jgtpy-0.4.9/jgtpy/JGTCore.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from collections import namedtuple
 from json import JSONEncoder
 import os
 import pathlib
 from pathlib import Path
 import pandas as pd
 
-__version__ = "0.4.8"
+__version__ = "0.4.9"
 
 from datetime import datetime
 from datetime import timedelta
 def offsetdt(time_str,nbhoursoffset=4,date_format_str= '%m/%d/%Y %H:%M:%S',output_dt_format='%Y-%m-%d %H:%M:%S'):
   given_time = datetime.strptime(time_str, date_format_str)
   final_time = given_time + timedelta(hours=nbhoursoffset)
   final_time_str = final_time.strftime(output_dt_format)
```

### Comparing `jgtpy-0.4.8/jgtpy/JGTIDS.py` & `jgtpy-0.4.9/jgtpy/JGTIDS.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/JGTIDSRequest.py` & `jgtpy-0.4.9/jgtpy/JGTIDSRequest.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/JGTImage.py` & `jgtpy-0.4.9/jgtpy/JGTImage.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/JGTMKSG.py` & `jgtpy-0.4.9/jgtpy/JGTMKSG.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/JGTPDHelper.py` & `jgtpy-0.4.9/jgtpy/JGTPDHelper.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/JGTPDSP.py` & `jgtpy-0.4.9/jgtpy/JGTPDSP.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/JGTPDSRequest.py` & `jgtpy-0.4.9/jgtpy/JGTPDSRequest.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/__init__.py` & `jgtpy-0.4.9/jgtpy/__init__.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/adshelper.py` & `jgtpy-0.4.9/jgtpy/adshelper.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/aohelper.py` & `jgtpy-0.4.9/jgtpy/aohelper.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/fe-formulation_of_target_variable_for_ML_in_FTS.py` & `jgtpy-0.4.9/jgtpy/fe-formulation_of_target_variable_for_ML_in_FTS.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/fsserver.py` & `jgtpy-0.4.9/jgtpy/fsserver.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/idsserver.py` & `jgtpy-0.4.9/jgtpy/idsserver.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/jgt2312.py` & `jgtpy-0.4.9/jgtpy/jgt2312.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/jgtbtetl1.py` & `jgtpy-0.4.9/jgtpy/jgtbtetl1.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/jgtbtetl2.py` & `jgtpy-0.4.9/jgtpy/jgtbtetl2.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/jgtcli.py` & `jgtpy-0.4.9/jgtpy/jgtcli.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/jgtdotenv.py` & `jgtpy-0.4.9/jgtpy/jgtdotenv.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/jgtetl.py` & `jgtpy-0.4.9/jgtpy/jgtetl.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/pdsclient.py` & `jgtpy-0.4.9/jgtpy/pdsclient.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/pto-panel-240209.py` & `jgtpy-0.4.9/jgtpy/pto-panel-240209.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/pto__ao_divergence_finder.py` & `jgtpy-0.4.9/jgtpy/pto__ao_divergence_finder.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/pto_featdim5.py` & `jgtpy-0.4.9/jgtpy/pto_featdim5.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/test_JGTADS.py` & `jgtpy-0.4.9/jgtpy/test_JGTADS.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/test_JGTIDS.py` & `jgtpy-0.4.9/jgtpy/test_JGTIDS.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/test_jgtcli.py` & `jgtpy-0.4.9/jgtpy/test_jgtcli.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/test_jgtcommon.py` & `jgtpy-0.4.9/jgtpy/test_jgtcommon.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/test_jgtos.py` & `jgtpy-0.4.9/jgtpy/test_jgtos.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/test_jgtwslhelper.py` & `jgtpy-0.4.9/jgtpy/test_jgtwslhelper.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/testmock_IDS.py` & `jgtpy-0.4.9/jgtpy/testmock_IDS.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/testpdsclient-cli.py` & `jgtpy-0.4.9/jgtpy/testpdsclient-cli.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/testpdsclient-h.py` & `jgtpy-0.4.9/jgtpy/testpdsclient-h.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy/testpdsclient-iprop.py` & `jgtpy-0.4.9/jgtpy/testpdsclient-iprop.py`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy.egg-info/PKG-INFO` & `jgtpy-0.4.9/jgtpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jgtpy
-Version: 0.4.8
+Version: 0.4.9
 Summary: Enhanced JGTPy CDS, IDS, PDSP Services
 Home-page: https://github.com/jgwill/jgtpy
 Author: GUillaume Isabelle
 Author-email: Guillaume Isabelle <jgi@jgwill.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jgwill/jgtpy
 Project-URL: Bug Tracker, https://github.com/jgwill/jgtpy/issues
```

### Comparing `jgtpy-0.4.8/jgtpy.egg-info/SOURCES.txt` & `jgtpy-0.4.9/jgtpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/jgtpy.egg-info/requires.txt` & `jgtpy-0.4.9/jgtpy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `jgtpy-0.4.8/pyproject.toml` & `jgtpy-0.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jgtpy"
-version = "0.4.8"
+version = "0.4.9"
 authors = [
   { name="Guillaume Isabelle", email="jgi@jgwill.com" },
 ]
 
 description = "Enhanced JGTPy CDS, IDS, PDSP Services"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `jgtpy-0.4.8/setup.py` & `jgtpy-0.4.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     name="jgtpy",
     version=version,
     description="JGTrading Data maker' Dataframes",
     long_description=open("README.rst").read(),
     author="GUillaume Isabelle",
     author_email="jgi@jgwill.com",
     url="https://github.com/jgwill/jgtpy",
-    packages=find_packages(include=["jgtpy"], exclude=["*test*"]),
+    packages=find_packages(include=["jgtpy","test-*.py"], exclude=["test*log","*test*csv","*test*png"]),
     # packages=find_packages(include=['jgtpy', 'jgtpy.forexconnect', 'jgtpy.forexconnect.lib', 'jgtpy.forexconnect.lib.windows', 'jgtpy.forexconnect.lib.linux'], exclude=['*test*']),
     install_requires=INSTALL_REQUIRES,
     entry_points={
         "console_scripts": ["jgtcli=jgtpy.jgtcli:main","jgtmksg=jgtpy.JGTMKSG:main"],
     },
     extras_require={
         "dev": (EXTRAS_DEV_LINT + EXTRAS_DEV_TEST + EXTRAS_DEV_DOCS),
```

