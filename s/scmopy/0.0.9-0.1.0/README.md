# Comparing `tmp/scmopy-0.0.9.tar.gz` & `tmp/scmopy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scmopy-0.0.9.tar", last modified: Sun Apr 14 19:10:57 2024, max compression
+gzip compressed data, was "scmopy-0.1.0.tar", last modified: Sun Apr 14 19:27:51 2024, max compression
```

## Comparing `scmopy-0.0.9.tar` & `scmopy-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 19:10:57.760778 scmopy-0.0.9/
--rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-30 13:55:39.000000 scmopy-0.0.9/LICENSE
--rw-r--r--   0 soli      (1000) soli      (1000)       85 2024-04-14 17:50:35.000000 scmopy-0.0.9/MANIFEST.in
--rw-r--r--   0 soli      (1000) soli      (1000)    21235 2024-04-14 19:10:57.760778 scmopy-0.0.9/PKG-INFO
--rw-r--r--   0 soli      (1000) soli      (1000)    20919 2024-04-14 19:09:55.000000 scmopy-0.0.9/README.md
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 19:10:57.760778 scmopy-0.0.9/scmopy/
--rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-30 10:40:19.000000 scmopy-0.0.9/scmopy/LICENSE
--rw-r--r--   0 soli      (1000) soli      (1000)      891 2024-04-14 19:09:33.000000 scmopy-0.0.9/scmopy/__init__.py
--rw-r--r--   0 soli      (1000) soli      (1000)     2036 2024-04-14 17:43:02.000000 scmopy-0.0.9/scmopy/base.py
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 19:10:57.760778 scmopy-0.0.9/scmopy/components/
--rw-r--r--   0 soli      (1000) soli      (1000)      905 2024-04-14 17:41:40.000000 scmopy-0.0.9/scmopy/components/__init__.py
--rw-r--r--   0 soli      (1000) soli      (1000)     5517 2024-04-14 17:42:11.000000 scmopy-0.0.9/scmopy/components/syniv.py
--rw-r--r--   0 soli      (1000) soli      (1000)     7089 2024-04-14 17:43:09.000000 scmopy-0.0.9/scmopy/gaussian_scm.py
--rw-r--r--   0 soli      (1000) soli      (1000)     5227 2024-04-14 17:43:16.000000 scmopy-0.0.9/scmopy/model_selection.py
--rw-r--r--   0 soli      (1000) soli      (1000)    14355 2024-04-14 17:43:56.000000 scmopy-0.0.9/scmopy/nongaussian_scm.py
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 19:10:57.760778 scmopy-0.0.9/scmopy.egg-info/
--rw-r--r--   0 soli      (1000) soli      (1000)    21235 2024-04-14 19:10:57.000000 scmopy-0.0.9/scmopy.egg-info/PKG-INFO
--rw-r--r--   0 soli      (1000) soli      (1000)      368 2024-04-14 19:10:57.000000 scmopy-0.0.9/scmopy.egg-info/SOURCES.txt
--rw-r--r--   0 soli      (1000) soli      (1000)        1 2024-04-14 19:10:57.000000 scmopy-0.0.9/scmopy.egg-info/dependency_links.txt
--rw-r--r--   0 soli      (1000) soli      (1000)       19 2024-04-14 19:10:57.000000 scmopy-0.0.9/scmopy.egg-info/requires.txt
--rw-r--r--   0 soli      (1000) soli      (1000)        7 2024-04-14 19:10:57.000000 scmopy-0.0.9/scmopy.egg-info/top_level.txt
--rw-r--r--   0 soli      (1000) soli      (1000)       38 2024-04-14 19:10:57.760778 scmopy-0.0.9/setup.cfg
--rw-r--r--   0 soli      (1000) soli      (1000)     1542 2024-04-14 19:09:39.000000 scmopy-0.0.9/setup.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 19:27:51.785739 scmopy-0.1.0/
+-rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-30 13:55:39.000000 scmopy-0.1.0/LICENSE
+-rw-r--r--   0 soli      (1000) soli      (1000)       85 2024-04-14 17:50:35.000000 scmopy-0.1.0/MANIFEST.in
+-rw-r--r--   0 soli      (1000) soli      (1000)    21227 2024-04-14 19:27:51.785739 scmopy-0.1.0/PKG-INFO
+-rw-r--r--   0 soli      (1000) soli      (1000)    20911 2024-04-14 19:26:23.000000 scmopy-0.1.0/README.md
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 19:27:51.785739 scmopy-0.1.0/scmopy/
+-rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-30 10:40:19.000000 scmopy-0.1.0/scmopy/LICENSE
+-rw-r--r--   0 soli      (1000) soli      (1000)      891 2024-04-14 19:27:13.000000 scmopy-0.1.0/scmopy/__init__.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     2036 2024-04-14 17:43:02.000000 scmopy-0.1.0/scmopy/base.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 19:27:51.785739 scmopy-0.1.0/scmopy/components/
+-rw-r--r--   0 soli      (1000) soli      (1000)      905 2024-04-14 17:41:40.000000 scmopy-0.1.0/scmopy/components/__init__.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     5517 2024-04-14 17:42:11.000000 scmopy-0.1.0/scmopy/components/syniv.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     7089 2024-04-14 17:43:09.000000 scmopy-0.1.0/scmopy/gaussian_scm.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     5227 2024-04-14 17:43:16.000000 scmopy-0.1.0/scmopy/model_selection.py
+-rw-r--r--   0 soli      (1000) soli      (1000)    14355 2024-04-14 17:43:56.000000 scmopy-0.1.0/scmopy/nongaussian_scm.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 19:27:51.785739 scmopy-0.1.0/scmopy.egg-info/
+-rw-r--r--   0 soli      (1000) soli      (1000)    21227 2024-04-14 19:27:51.000000 scmopy-0.1.0/scmopy.egg-info/PKG-INFO
+-rw-r--r--   0 soli      (1000) soli      (1000)      368 2024-04-14 19:27:51.000000 scmopy-0.1.0/scmopy.egg-info/SOURCES.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)        1 2024-04-14 19:27:51.000000 scmopy-0.1.0/scmopy.egg-info/dependency_links.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)       19 2024-04-14 19:27:51.000000 scmopy-0.1.0/scmopy.egg-info/requires.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)        7 2024-04-14 19:27:51.000000 scmopy-0.1.0/scmopy.egg-info/top_level.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)       38 2024-04-14 19:27:51.785739 scmopy-0.1.0/setup.cfg
+-rw-r--r--   0 soli      (1000) soli      (1000)     1542 2024-04-14 19:27:01.000000 scmopy-0.1.0/setup.py
```

### Comparing `scmopy-0.0.9/LICENSE` & `scmopy-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scmopy-0.0.9/PKG-INFO` & `scmopy-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmopy
-Version: 0.0.9
+Version: 0.1.0
 Summary: scmopy: Distribution-Agnostic Structural Causal Models Optimization in Python
 Home-page: https://github.com/DSsoli/scmopy.git
 Author: Sanghoon Lee (DSsoli)
 Author-email: solisoli3197@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -530,18 +530,18 @@
 
 <br>
 
 Reference and detailed documentation for the ESA-2SCM algorithm:
 * Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 21. <snbperi.org/article/230> [[ARTICLE LINK]](http://www.snbperi.org/article/230)
 
 ## Examples
-Examples of running ESA-2SCM in Jupyter Notebook are included in [esa_2scm/examples](https://github.com/DSsoli/esa-2scm/tree/main/examples)
+Examples of running scmopy in Jupyter Notebook are included in [scmopy/examples](https://github.com/DSsoli/scmopy/tree/main/examples)
 
 ## License
-scmopy package is licensed under the terms of the [MIT license](https://github.com/DSsoli/esa-2scm/blob/main/LICENSE)
+scmopy package is licensed under the terms of the [MIT license](https://github.com/DSsoli/scmopy/blob/main/LICENSE)
 
 ## References
 
 ### scmopy Package
 
 Should you use the scmopy package to perform causal discovery, please kindly cite my original article and the original article by S.Shimizu and Y.Kano:
```

### Comparing `scmopy-0.0.9/README.md` & `scmopy-0.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -520,18 +520,18 @@
 
 <br>
 
 Reference and detailed documentation for the ESA-2SCM algorithm:
 * Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 21. <snbperi.org/article/230> [[ARTICLE LINK]](http://www.snbperi.org/article/230)
 
 ## Examples
-Examples of running ESA-2SCM in Jupyter Notebook are included in [esa_2scm/examples](https://github.com/DSsoli/esa-2scm/tree/main/examples)
+Examples of running scmopy in Jupyter Notebook are included in [scmopy/examples](https://github.com/DSsoli/scmopy/tree/main/examples)
 
 ## License
-scmopy package is licensed under the terms of the [MIT license](https://github.com/DSsoli/esa-2scm/blob/main/LICENSE)
+scmopy package is licensed under the terms of the [MIT license](https://github.com/DSsoli/scmopy/blob/main/LICENSE)
 
 ## References
 
 ### scmopy Package
 
 Should you use the scmopy package to perform causal discovery, please kindly cite my original article and the original article by S.Shimizu and Y.Kano:
```

### Comparing `scmopy-0.0.9/scmopy/LICENSE` & `scmopy-0.1.0/scmopy/LICENSE`

 * *Files identical despite different names*

### Comparing `scmopy-0.0.9/scmopy/__init__.py` & `scmopy-0.1.0/scmopy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 
 Should you use the scmopy package, please cite the following articles.
 - Lee, Sanghoon (2024). ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable, SnB Political and Economic Research Institute, 1, 21. <snbperi.org/article/230>.
 - S.Shimizu and Y.Kano (2008). Use of non-normality in structural equation modeling: Application to direction of causation, Journal of Statistical Planning and Inference, 138, 11, 3483-3491.
 
 """
 
-__version__ = '0.0.9'
+__version__ = '0.1.0'
```

### Comparing `scmopy-0.0.9/scmopy/base.py` & `scmopy-0.1.0/scmopy/base.py`

 * *Files identical despite different names*

### Comparing `scmopy-0.0.9/scmopy/components/__init__.py` & `scmopy-0.1.0/scmopy/components/__init__.py`

 * *Files identical despite different names*

### Comparing `scmopy-0.0.9/scmopy/components/syniv.py` & `scmopy-0.1.0/scmopy/components/syniv.py`

 * *Files identical despite different names*

### Comparing `scmopy-0.0.9/scmopy/gaussian_scm.py` & `scmopy-0.1.0/scmopy/gaussian_scm.py`

 * *Files identical despite different names*

### Comparing `scmopy-0.0.9/scmopy/model_selection.py` & `scmopy-0.1.0/scmopy/model_selection.py`

 * *Files identical despite different names*

### Comparing `scmopy-0.0.9/scmopy/nongaussian_scm.py` & `scmopy-0.1.0/scmopy/nongaussian_scm.py`

 * *Files identical despite different names*

### Comparing `scmopy-0.0.9/scmopy.egg-info/PKG-INFO` & `scmopy-0.1.0/scmopy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmopy
-Version: 0.0.9
+Version: 0.1.0
 Summary: scmopy: Distribution-Agnostic Structural Causal Models Optimization in Python
 Home-page: https://github.com/DSsoli/scmopy.git
 Author: Sanghoon Lee (DSsoli)
 Author-email: solisoli3197@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -530,18 +530,18 @@
 
 <br>
 
 Reference and detailed documentation for the ESA-2SCM algorithm:
 * Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 21. <snbperi.org/article/230> [[ARTICLE LINK]](http://www.snbperi.org/article/230)
 
 ## Examples
-Examples of running ESA-2SCM in Jupyter Notebook are included in [esa_2scm/examples](https://github.com/DSsoli/esa-2scm/tree/main/examples)
+Examples of running scmopy in Jupyter Notebook are included in [scmopy/examples](https://github.com/DSsoli/scmopy/tree/main/examples)
 
 ## License
-scmopy package is licensed under the terms of the [MIT license](https://github.com/DSsoli/esa-2scm/blob/main/LICENSE)
+scmopy package is licensed under the terms of the [MIT license](https://github.com/DSsoli/scmopy/blob/main/LICENSE)
 
 ## References
 
 ### scmopy Package
 
 Should you use the scmopy package to perform causal discovery, please kindly cite my original article and the original article by S.Shimizu and Y.Kano:
```

### Comparing `scmopy-0.0.9/setup.py` & `scmopy-0.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 with open("README.md", "r", encoding='utf-8') as fh:
     README = fh.read()
 
 setup(
     author="Sanghoon Lee (DSsoli)",
     author_email="solisoli3197@gmail.com",
     name="scmopy",
-    version="0.0.9",
+    version="0.1.0",
     description="scmopy: Distribution-Agnostic Structural Causal Models Optimization in Python",
     long_description=README,
     long_description_content_type="text/markdown",
     install_requires=["numpy", "pandas", "scipy"],
     url="https://github.com/DSsoli/scmopy.git",
     packages=find_packages(include=['scmopy', 'scmopy.*']),
     package_data={"scmopy": ['LICENSE', 'examples/*']},
```

