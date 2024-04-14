# Comparing `tmp/scmopy-0.0.5.tar.gz` & `tmp/scmopy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scmopy-0.0.5.tar", last modified: Sun Apr 14 18:38:10 2024, max compression
+gzip compressed data, was "scmopy-0.0.6.tar", last modified: Sun Apr 14 18:46:49 2024, max compression
```

## Comparing `scmopy-0.0.5.tar` & `scmopy-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 18:38:10.903802 scmopy-0.0.5/
--rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-30 13:55:39.000000 scmopy-0.0.5/LICENSE
--rw-r--r--   0 soli      (1000) soli      (1000)       85 2024-04-14 17:50:35.000000 scmopy-0.0.5/MANIFEST.in
--rw-r--r--   0 soli      (1000) soli      (1000)    21227 2024-04-14 18:38:10.903802 scmopy-0.0.5/PKG-INFO
--rw-r--r--   0 soli      (1000) soli      (1000)    20911 2024-04-14 18:36:07.000000 scmopy-0.0.5/README.md
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 18:38:10.903802 scmopy-0.0.5/scmopy/
--rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-30 10:40:19.000000 scmopy-0.0.5/scmopy/LICENSE
--rw-r--r--   0 soli      (1000) soli      (1000)      891 2024-04-14 18:36:38.000000 scmopy-0.0.5/scmopy/__init__.py
--rw-r--r--   0 soli      (1000) soli      (1000)     2036 2024-04-14 17:43:02.000000 scmopy-0.0.5/scmopy/base.py
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 18:38:10.903802 scmopy-0.0.5/scmopy/components/
--rw-r--r--   0 soli      (1000) soli      (1000)      905 2024-04-14 17:41:40.000000 scmopy-0.0.5/scmopy/components/__init__.py
--rw-r--r--   0 soli      (1000) soli      (1000)     5517 2024-04-14 17:42:11.000000 scmopy-0.0.5/scmopy/components/syniv.py
--rw-r--r--   0 soli      (1000) soli      (1000)     7089 2024-04-14 17:43:09.000000 scmopy-0.0.5/scmopy/gaussian_scm.py
--rw-r--r--   0 soli      (1000) soli      (1000)     5227 2024-04-14 17:43:16.000000 scmopy-0.0.5/scmopy/model_selection.py
--rw-r--r--   0 soli      (1000) soli      (1000)    14355 2024-04-14 17:43:56.000000 scmopy-0.0.5/scmopy/nongaussian_scm.py
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 18:38:10.903802 scmopy-0.0.5/scmopy.egg-info/
--rw-r--r--   0 soli      (1000) soli      (1000)    21227 2024-04-14 18:38:10.000000 scmopy-0.0.5/scmopy.egg-info/PKG-INFO
--rw-r--r--   0 soli      (1000) soli      (1000)      368 2024-04-14 18:38:10.000000 scmopy-0.0.5/scmopy.egg-info/SOURCES.txt
--rw-r--r--   0 soli      (1000) soli      (1000)        1 2024-04-14 18:38:10.000000 scmopy-0.0.5/scmopy.egg-info/dependency_links.txt
--rw-r--r--   0 soli      (1000) soli      (1000)       19 2024-04-14 18:38:10.000000 scmopy-0.0.5/scmopy.egg-info/requires.txt
--rw-r--r--   0 soli      (1000) soli      (1000)        7 2024-04-14 18:38:10.000000 scmopy-0.0.5/scmopy.egg-info/top_level.txt
--rw-r--r--   0 soli      (1000) soli      (1000)       38 2024-04-14 18:38:10.903802 scmopy-0.0.5/setup.cfg
--rw-r--r--   0 soli      (1000) soli      (1000)     1542 2024-04-14 18:36:42.000000 scmopy-0.0.5/setup.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 18:46:49.008506 scmopy-0.0.6/
+-rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-30 13:55:39.000000 scmopy-0.0.6/LICENSE
+-rw-r--r--   0 soli      (1000) soli      (1000)       85 2024-04-14 17:50:35.000000 scmopy-0.0.6/MANIFEST.in
+-rw-r--r--   0 soli      (1000) soli      (1000)    21335 2024-04-14 18:46:49.008506 scmopy-0.0.6/PKG-INFO
+-rw-r--r--   0 soli      (1000) soli      (1000)    21019 2024-04-14 18:45:38.000000 scmopy-0.0.6/README.md
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 18:46:49.008506 scmopy-0.0.6/scmopy/
+-rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-30 10:40:19.000000 scmopy-0.0.6/scmopy/LICENSE
+-rw-r--r--   0 soli      (1000) soli      (1000)      891 2024-04-14 18:45:50.000000 scmopy-0.0.6/scmopy/__init__.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     2036 2024-04-14 17:43:02.000000 scmopy-0.0.6/scmopy/base.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 18:46:49.008506 scmopy-0.0.6/scmopy/components/
+-rw-r--r--   0 soli      (1000) soli      (1000)      905 2024-04-14 17:41:40.000000 scmopy-0.0.6/scmopy/components/__init__.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     5517 2024-04-14 17:42:11.000000 scmopy-0.0.6/scmopy/components/syniv.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     7089 2024-04-14 17:43:09.000000 scmopy-0.0.6/scmopy/gaussian_scm.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     5227 2024-04-14 17:43:16.000000 scmopy-0.0.6/scmopy/model_selection.py
+-rw-r--r--   0 soli      (1000) soli      (1000)    14355 2024-04-14 17:43:56.000000 scmopy-0.0.6/scmopy/nongaussian_scm.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 18:46:49.008506 scmopy-0.0.6/scmopy.egg-info/
+-rw-r--r--   0 soli      (1000) soli      (1000)    21335 2024-04-14 18:46:48.000000 scmopy-0.0.6/scmopy.egg-info/PKG-INFO
+-rw-r--r--   0 soli      (1000) soli      (1000)      368 2024-04-14 18:46:48.000000 scmopy-0.0.6/scmopy.egg-info/SOURCES.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)        1 2024-04-14 18:46:48.000000 scmopy-0.0.6/scmopy.egg-info/dependency_links.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)       19 2024-04-14 18:46:48.000000 scmopy-0.0.6/scmopy.egg-info/requires.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)        7 2024-04-14 18:46:48.000000 scmopy-0.0.6/scmopy.egg-info/top_level.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)       38 2024-04-14 18:46:49.008506 scmopy-0.0.6/setup.cfg
+-rw-r--r--   0 soli      (1000) soli      (1000)     1542 2024-04-14 18:45:58.000000 scmopy-0.0.6/setup.py
```

### Comparing `scmopy-0.0.5/LICENSE` & `scmopy-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scmopy-0.0.5/PKG-INFO` & `scmopy-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: scmopy
-Version: 0.0.5
+Version: 0.0.6
 Summary: scmopy: Distribution-Agnostic Structural Causal Models Optimization in Python
 Home-page: https://github.com/DSsoli/scmopy.git
 Author: Sanghoon Lee (DSsoli)
 Author-email: solisoli3197@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **scmopy**: Distribution-Agnostic Structural Causal Models Optimization in Python
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/DSsoli/scmopy/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/scmopy.svg)](https://pypi.org/project/scmopy/)
+[![PyPI version](https://img.shields.io/pypi/v/scmopy.svg?kill_cache=1)](https://pypi.org/project/scmopy/)
+
 
 scmopy is a composite package for causal discovery/analysis using several **novel** types of Structural Causal Models Optimization algorithms.
 <br>
 
 scmopy provides **Distribution-Agnostic** methods in identifying causality; in other words, distributional assumptions in typical SCM/SEM such as satisfying the normality conditions are *not* required.
 <br>
```

### Comparing `scmopy-0.0.5/README.md` & `scmopy-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # **scmopy**: Distribution-Agnostic Structural Causal Models Optimization in Python
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/DSsoli/scmopy/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/scmopy.svg)](https://pypi.org/project/scmopy/)
+[![PyPI version](https://img.shields.io/pypi/v/scmopy.svg?kill_cache=1)](https://pypi.org/project/scmopy/)
+
 
 scmopy is a composite package for causal discovery/analysis using several **novel** types of Structural Causal Models Optimization algorithms.
 <br>
 
 scmopy provides **Distribution-Agnostic** methods in identifying causality; in other words, distributional assumptions in typical SCM/SEM such as satisfying the normality conditions are *not* required.
 <br>
```

### Comparing `scmopy-0.0.5/scmopy/LICENSE` & `scmopy-0.0.6/scmopy/LICENSE`

 * *Files identical despite different names*

### Comparing `scmopy-0.0.5/scmopy/__init__.py` & `scmopy-0.0.6/scmopy/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 
 Should you use the scmopy package, please cite the following articles.
 - Lee, Sanghoon (2024). ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable, SnB Political and Economic Research Institute, 1, 21. <snbperi.org/article/230>.
 - S.Shimizu and Y.Kano (2008). Use of non-normality in structural equation modeling: Application to direction of causation, Journal of Statistical Planning and Inference, 138, 11, 3483-3491.
 
 """
 
-__version__ = '0.0.5'
+__version__ = '0.0.6'
```

### Comparing `scmopy-0.0.5/scmopy/base.py` & `scmopy-0.0.6/scmopy/base.py`

 * *Files identical despite different names*

### Comparing `scmopy-0.0.5/scmopy/components/__init__.py` & `scmopy-0.0.6/scmopy/components/__init__.py`

 * *Files identical despite different names*

### Comparing `scmopy-0.0.5/scmopy/components/syniv.py` & `scmopy-0.0.6/scmopy/components/syniv.py`

 * *Files identical despite different names*

### Comparing `scmopy-0.0.5/scmopy/gaussian_scm.py` & `scmopy-0.0.6/scmopy/gaussian_scm.py`

 * *Files identical despite different names*

### Comparing `scmopy-0.0.5/scmopy/model_selection.py` & `scmopy-0.0.6/scmopy/model_selection.py`

 * *Files identical despite different names*

### Comparing `scmopy-0.0.5/scmopy/nongaussian_scm.py` & `scmopy-0.0.6/scmopy/nongaussian_scm.py`

 * *Files identical despite different names*

### Comparing `scmopy-0.0.5/scmopy.egg-info/PKG-INFO` & `scmopy-0.0.6/scmopy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: scmopy
-Version: 0.0.5
+Version: 0.0.6
 Summary: scmopy: Distribution-Agnostic Structural Causal Models Optimization in Python
 Home-page: https://github.com/DSsoli/scmopy.git
 Author: Sanghoon Lee (DSsoli)
 Author-email: solisoli3197@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **scmopy**: Distribution-Agnostic Structural Causal Models Optimization in Python
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/DSsoli/scmopy/blob/main/LICENSE)
 [![PyPI version](https://badge.fury.io/py/scmopy.svg)](https://pypi.org/project/scmopy/)
+[![PyPI version](https://img.shields.io/pypi/v/scmopy.svg?kill_cache=1)](https://pypi.org/project/scmopy/)
+
 
 scmopy is a composite package for causal discovery/analysis using several **novel** types of Structural Causal Models Optimization algorithms.
 <br>
 
 scmopy provides **Distribution-Agnostic** methods in identifying causality; in other words, distributional assumptions in typical SCM/SEM such as satisfying the normality conditions are *not* required.
 <br>
```

### Comparing `scmopy-0.0.5/setup.py` & `scmopy-0.0.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 with open("README.md", "r", encoding='utf-8') as fh:
     README = fh.read()
 
 setup(
     author="Sanghoon Lee (DSsoli)",
     author_email="solisoli3197@gmail.com",
     name="scmopy",
-    version="0.0.5",
+    version="0.0.6",
     description="scmopy: Distribution-Agnostic Structural Causal Models Optimization in Python",
     long_description=README,
     long_description_content_type="text/markdown",
     install_requires=["numpy", "pandas", "scipy"],
     url="https://github.com/DSsoli/scmopy.git",
     packages=find_packages(include=['scmopy', 'scmopy.*']),
     package_data={"scmopy": ['LICENSE', 'examples/*']},
```

