# Comparing `tmp/jgtutils-0.1.7.tar.gz` & `tmp/jgtutils-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jgtutils-0.1.7.tar", last modified: Fri Dec 29 02:24:46 2023, max compression
+gzip compressed data, was "jgtutils-0.1.8.tar", last modified: Fri Dec 29 02:26:10 2023, max compression
```

## Comparing `jgtutils-0.1.7.tar` & `jgtutils-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,30 @@
-drwxrwxrwx   0 jgi       (1000) jgi       (1000)        0 2023-12-29 02:24:46.309104 jgtutils-0.1.7/
--rwxrwxrwx   0 jgi       (1000) jgi       (1000)     1086 2023-12-28 01:42:09.000000 jgtutils-0.1.7/LICENSE
--rwxrwxrwx   0 jgi       (1000) jgi       (1000)     1613 2023-12-29 02:24:46.306339 jgtutils-0.1.7/PKG-INFO
--rwxrwxrwx   0 jgi       (1000) jgi       (1000)      807 2023-12-28 01:39:41.000000 jgtutils-0.1.7/README.md
-drwxrwxrwx   0 jgi       (1000) jgi       (1000)        0 2023-12-29 02:24:46.177122 jgtutils-0.1.7/jgtutils/
--rwxrwxrwx   0 jgi       (1000) jgi       (1000)       47 2023-12-29 02:24:41.000000 jgtutils-0.1.7/jgtutils/__init__.py
--rwxrwxrwx   0 jgi       (1000) jgi       (1000)     6105 2023-12-29 02:21:58.000000 jgtutils-0.1.7/jgtutils/fxcli2console.py
--rwxrwxrwx   0 jgi       (1000) jgi       (1000)    25491 2023-12-29 02:08:29.000000 jgtutils-0.1.7/jgtutils/iprops.py
--rwxrwxrwx   0 jgi       (1000) jgi       (1000)    13789 2023-12-28 03:12:12.000000 jgtutils-0.1.7/jgtutils/jgtcommon.py
--rwxrwxrwx   0 jgi       (1000) jgi       (1000)     7639 2023-12-28 01:47:05.000000 jgtutils-0.1.7/jgtutils/jgtconstants.py
--rwxrwxrwx   0 jgi       (1000) jgi       (1000)     5396 2023-12-28 02:09:53.000000 jgtutils-0.1.7/jgtutils/jgtos.py
--rwxrwxrwx   0 jgi       (1000) jgi       (1000)     5661 2023-12-28 02:12:55.000000 jgtutils-0.1.7/jgtutils/jgtwslhelper.py
--rwxrwxrwx   0 jgi       (1000) jgi       (1000)       45 2023-12-28 01:39:18.000000 jgtutils-0.1.7/jgtutils/module.py
-drwxrwxrwx   0 jgi       (1000) jgi       (1000)        0 2023-12-29 02:24:46.265962 jgtutils-0.1.7/jgtutils.egg-info/
--rwxrwxrwx   0 jgi       (1000) jgi       (1000)     1613 2023-12-29 02:24:45.000000 jgtutils-0.1.7/jgtutils.egg-info/PKG-INFO
--rwxrwxrwx   0 jgi       (1000) jgi       (1000)      385 2023-12-29 02:24:45.000000 jgtutils-0.1.7/jgtutils.egg-info/SOURCES.txt
--rwxrwxrwx   0 jgi       (1000) jgi       (1000)        1 2023-12-29 02:24:45.000000 jgtutils-0.1.7/jgtutils.egg-info/dependency_links.txt
--rwxrwxrwx   0 jgi       (1000) jgi       (1000)       62 2023-12-29 02:24:45.000000 jgtutils-0.1.7/jgtutils.egg-info/entry_points.txt
--rwxrwxrwx   0 jgi       (1000) jgi       (1000)        9 2023-12-29 02:24:45.000000 jgtutils-0.1.7/jgtutils.egg-info/top_level.txt
--rwxrwxrwx   0 jgi       (1000) jgi       (1000)       38 2023-12-29 02:24:46.310102 jgtutils-0.1.7/setup.cfg
--rwxrwxrwx   0 jgi       (1000) jgi       (1000)     1089 2023-12-29 02:24:41.000000 jgtutils-0.1.7/setup.py
-drwxrwxrwx   0 jgi       (1000) jgi       (1000)        0 2023-12-29 02:24:46.288330 jgtutils-0.1.7/tests/
--rwxrwxrwx   0 jgi       (1000) jgi       (1000)      234 2023-12-28 01:39:23.000000 jgtutils-0.1.7/tests/test_module.py
+drwxrwxrwx   0 jgi       (1000) jgi       (1000)        0 2023-12-29 02:26:10.689771 jgtutils-0.1.8/
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)     1086 2023-12-28 01:42:09.000000 jgtutils-0.1.8/LICENSE
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)     1613 2023-12-29 02:26:10.682771 jgtutils-0.1.8/PKG-INFO
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)      807 2023-12-28 01:39:41.000000 jgtutils-0.1.8/README.md
+drwxrwxrwx   0 jgi       (1000) jgi       (1000)        0 2023-12-29 02:26:10.212397 jgtutils-0.1.8/jgtutils/
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)       47 2023-12-29 02:26:05.000000 jgtutils-0.1.8/jgtutils/__init__.py
+drwxrwxrwx   0 jgi       (1000) jgi       (1000)        0 2023-12-29 02:26:10.619004 jgtutils-0.1.8/jgtutils/common_samples/
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)     3071 2023-12-25 21:04:07.000000 jgtutils-0.1.8/jgtutils/common_samples/BatchOrderMonitor.py
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)     6703 2023-12-25 21:04:07.000000 jgtutils-0.1.8/jgtutils/common_samples/OrderMonitor.py
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)     8058 2023-12-25 21:04:07.000000 jgtutils-0.1.8/jgtutils/common_samples/OrderMonitorNetting.py
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)     8841 2023-12-25 21:04:07.000000 jgtutils-0.1.8/jgtutils/common_samples/TableListenerContainer.py
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)     1286 2023-12-25 21:04:07.000000 jgtutils-0.1.8/jgtutils/common_samples/__init__.py
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)    10060 2023-12-25 21:26:12.000000 jgtutils-0.1.8/jgtutils/common_samples/common.py
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)     6105 2023-12-29 02:21:58.000000 jgtutils-0.1.8/jgtutils/fxcli2console.py
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)    25491 2023-12-29 02:08:29.000000 jgtutils-0.1.8/jgtutils/iprops.py
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)    13789 2023-12-28 03:12:12.000000 jgtutils-0.1.8/jgtutils/jgtcommon.py
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)     7639 2023-12-28 01:47:05.000000 jgtutils-0.1.8/jgtutils/jgtconstants.py
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)     5396 2023-12-28 02:09:53.000000 jgtutils-0.1.8/jgtutils/jgtos.py
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)     5661 2023-12-28 02:12:55.000000 jgtutils-0.1.8/jgtutils/jgtwslhelper.py
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)       45 2023-12-28 01:39:18.000000 jgtutils-0.1.8/jgtutils/module.py
+drwxrwxrwx   0 jgi       (1000) jgi       (1000)        0 2023-12-29 02:26:10.385398 jgtutils-0.1.8/jgtutils.egg-info/
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)     1613 2023-12-29 02:26:09.000000 jgtutils-0.1.8/jgtutils.egg-info/PKG-INFO
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)      637 2023-12-29 02:26:09.000000 jgtutils-0.1.8/jgtutils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)        1 2023-12-29 02:26:09.000000 jgtutils-0.1.8/jgtutils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)       62 2023-12-29 02:26:09.000000 jgtutils-0.1.8/jgtutils.egg-info/entry_points.txt
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)        9 2023-12-29 02:26:09.000000 jgtutils-0.1.8/jgtutils.egg-info/top_level.txt
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)       38 2023-12-29 02:26:10.690774 jgtutils-0.1.8/setup.cfg
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)     1089 2023-12-29 02:26:05.000000 jgtutils-0.1.8/setup.py
+drwxrwxrwx   0 jgi       (1000) jgi       (1000)        0 2023-12-29 02:26:10.653914 jgtutils-0.1.8/tests/
+-rwxrwxrwx   0 jgi       (1000) jgi       (1000)      234 2023-12-28 01:39:23.000000 jgtutils-0.1.8/tests/test_module.py
```

### Comparing `jgtutils-0.1.7/LICENSE` & `jgtutils-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jgtutils-0.1.7/PKG-INFO` & `jgtutils-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jgtutils
-Version: 0.1.7
+Version: 0.1.8
 Summary: A utility package common to other JGT projects.
 Home-page: https://github.com/jgwill/jgtutils
 Author: Guillaume Isabelle
 Author-email: jgi@jgwill.com
 Project-URL: Bug Reports, https://github.com/jgwill/jgtutils/issues
 Project-URL: Source, https://github.com/jgwill/jgtutils
 Keywords: utilities
```

### Comparing `jgtutils-0.1.7/README.md` & `jgtutils-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `jgtutils-0.1.7/jgtutils/fxcli2console.py` & `jgtutils-0.1.8/jgtutils/fxcli2console.py`

 * *Files identical despite different names*

### Comparing `jgtutils-0.1.7/jgtutils/iprops.py` & `jgtutils-0.1.8/jgtutils/iprops.py`

 * *Files identical despite different names*

### Comparing `jgtutils-0.1.7/jgtutils/jgtcommon.py` & `jgtutils-0.1.8/jgtutils/jgtcommon.py`

 * *Files identical despite different names*

### Comparing `jgtutils-0.1.7/jgtutils/jgtconstants.py` & `jgtutils-0.1.8/jgtutils/jgtconstants.py`

 * *Files identical despite different names*

### Comparing `jgtutils-0.1.7/jgtutils/jgtos.py` & `jgtutils-0.1.8/jgtutils/jgtos.py`

 * *Files identical despite different names*

### Comparing `jgtutils-0.1.7/jgtutils/jgtwslhelper.py` & `jgtutils-0.1.8/jgtutils/jgtwslhelper.py`

 * *Files identical despite different names*

### Comparing `jgtutils-0.1.7/jgtutils.egg-info/PKG-INFO` & `jgtutils-0.1.8/jgtutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jgtutils
-Version: 0.1.7
+Version: 0.1.8
 Summary: A utility package common to other JGT projects.
 Home-page: https://github.com/jgwill/jgtutils
 Author: Guillaume Isabelle
 Author-email: jgi@jgwill.com
 Project-URL: Bug Reports, https://github.com/jgwill/jgtutils/issues
 Project-URL: Source, https://github.com/jgwill/jgtutils
 Keywords: utilities
```

### Comparing `jgtutils-0.1.7/setup.py` & `jgtutils-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='jgtutils',
-    version='0.1.7',
+    version='0.1.8',
     packages=find_packages(),
     description='A utility package common to other JGT projects.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Guillaume Isabelle',
     author_email='jgi@jgwill.com',
     url='https://github.com/jgwill/jgtutils',
```

