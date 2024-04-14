# Comparing `tmp/esa-2scm-0.2.4.tar.gz` & `tmp/esa-2scm-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esa-2scm-0.2.4.tar", last modified: Wed Apr  3 17:59:52 2024, max compression
+gzip compressed data, was "esa-2scm-0.2.5.tar", last modified: Sun Apr 14 19:17:04 2024, max compression
```

## Comparing `esa-2scm-0.2.4.tar` & `esa-2scm-0.2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-03 17:59:52.539755 esa-2scm-0.2.4/
--rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-28 16:38:21.000000 esa-2scm-0.2.4/LICENSE
--rw-r--r--   0 soli      (1000) soli      (1000)       87 2024-01-25 20:49:15.000000 esa-2scm-0.2.4/MANIFEST.in
--rw-r--r--   0 soli      (1000) soli      (1000)     6213 2024-04-03 17:59:52.539755 esa-2scm-0.2.4/PKG-INFO
--rw-r--r--   0 soli      (1000) soli      (1000)     5926 2024-04-03 17:57:51.000000 esa-2scm-0.2.4/README.md
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-03 17:59:52.539755 esa-2scm-0.2.4/esa_2scm/
--rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-28 16:05:50.000000 esa-2scm-0.2.4/esa_2scm/LICENSE
--rw-r--r--   0 soli      (1000) soli      (1000)      559 2024-04-03 17:58:57.000000 esa-2scm-0.2.4/esa_2scm/__init__.py
--rw-r--r--   0 soli      (1000) soli      (1000)     7824 2024-04-02 10:47:30.000000 esa-2scm-0.2.4/esa_2scm/models.py
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-03 17:59:52.539755 esa-2scm-0.2.4/esa_2scm/syniv/
--rw-r--r--   0 soli      (1000) soli      (1000)      541 2024-04-02 10:47:01.000000 esa-2scm-0.2.4/esa_2scm/syniv/__init__.py
--rw-r--r--   0 soli      (1000) soli      (1000)     5155 2024-04-02 10:47:08.000000 esa-2scm-0.2.4/esa_2scm/syniv/esa.py
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-03 17:59:52.539755 esa-2scm-0.2.4/esa_2scm.egg-info/
--rw-r--r--   0 soli      (1000) soli      (1000)     6213 2024-04-03 17:59:52.000000 esa-2scm-0.2.4/esa_2scm.egg-info/PKG-INFO
--rw-r--r--   0 soli      (1000) soli      (1000)      364 2024-04-03 17:59:52.000000 esa-2scm-0.2.4/esa_2scm.egg-info/SOURCES.txt
--rw-r--r--   0 soli      (1000) soli      (1000)        1 2024-04-03 17:59:52.000000 esa-2scm-0.2.4/esa_2scm.egg-info/dependency_links.txt
--rw-r--r--   0 soli      (1000) soli      (1000)       32 2024-04-03 17:59:52.000000 esa-2scm-0.2.4/esa_2scm.egg-info/requires.txt
--rw-r--r--   0 soli      (1000) soli      (1000)        9 2024-04-03 17:59:52.000000 esa-2scm-0.2.4/esa_2scm.egg-info/top_level.txt
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-03 17:59:52.539755 esa-2scm-0.2.4/examples/
--rw-r--r--   0 soli      (1000) soli      (1000)   133015 2024-04-02 11:23:33.000000 esa-2scm-0.2.4/examples/example.ipynb
--rw-r--r--   0 soli      (1000) soli      (1000)       38 2024-04-03 17:59:52.539755 esa-2scm-0.2.4/setup.cfg
--rw-r--r--   0 soli      (1000) soli      (1000)     1173 2024-04-03 17:58:59.000000 esa-2scm-0.2.4/setup.py
-drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-03 17:59:52.539755 esa-2scm-0.2.4/test/
--rw-r--r--   0 soli      (1000) soli      (1000)     2101 2024-03-28 16:37:14.000000 esa-2scm-0.2.4/test/test_model.py
--rw-r--r--   0 soli      (1000) soli      (1000)     2627 2024-03-23 19:40:59.000000 esa-2scm-0.2.4/test/test_syniv.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 19:17:04.445683 esa-2scm-0.2.5/
+-rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-28 16:38:21.000000 esa-2scm-0.2.5/LICENSE
+-rw-r--r--   0 soli      (1000) soli      (1000)       87 2024-01-25 20:49:15.000000 esa-2scm-0.2.5/MANIFEST.in
+-rw-r--r--   0 soli      (1000) soli      (1000)     6309 2024-04-14 19:17:04.445683 esa-2scm-0.2.5/PKG-INFO
+-rw-r--r--   0 soli      (1000) soli      (1000)     6022 2024-04-14 19:14:57.000000 esa-2scm-0.2.5/README.md
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 19:17:04.445683 esa-2scm-0.2.5/esa_2scm/
+-rw-r--r--   0 soli      (1000) soli      (1000)     1077 2024-03-28 16:05:50.000000 esa-2scm-0.2.5/esa_2scm/LICENSE
+-rw-r--r--   0 soli      (1000) soli      (1000)      559 2024-04-14 19:15:15.000000 esa-2scm-0.2.5/esa_2scm/__init__.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     7824 2024-04-02 10:47:30.000000 esa-2scm-0.2.5/esa_2scm/models.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 19:17:04.445683 esa-2scm-0.2.5/esa_2scm/syniv/
+-rw-r--r--   0 soli      (1000) soli      (1000)      541 2024-04-02 10:47:01.000000 esa-2scm-0.2.5/esa_2scm/syniv/__init__.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     5155 2024-04-02 10:47:08.000000 esa-2scm-0.2.5/esa_2scm/syniv/esa.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 19:17:04.445683 esa-2scm-0.2.5/esa_2scm.egg-info/
+-rw-r--r--   0 soli      (1000) soli      (1000)     6309 2024-04-14 19:17:04.000000 esa-2scm-0.2.5/esa_2scm.egg-info/PKG-INFO
+-rw-r--r--   0 soli      (1000) soli      (1000)      364 2024-04-14 19:17:04.000000 esa-2scm-0.2.5/esa_2scm.egg-info/SOURCES.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)        1 2024-04-14 19:17:04.000000 esa-2scm-0.2.5/esa_2scm.egg-info/dependency_links.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)       19 2024-04-14 19:17:04.000000 esa-2scm-0.2.5/esa_2scm.egg-info/requires.txt
+-rw-r--r--   0 soli      (1000) soli      (1000)        9 2024-04-14 19:17:04.000000 esa-2scm-0.2.5/esa_2scm.egg-info/top_level.txt
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 19:17:04.445683 esa-2scm-0.2.5/examples/
+-rw-r--r--   0 soli      (1000) soli      (1000)   133015 2024-04-02 11:23:33.000000 esa-2scm-0.2.5/examples/example.ipynb
+-rw-r--r--   0 soli      (1000) soli      (1000)       38 2024-04-14 19:17:04.445683 esa-2scm-0.2.5/setup.cfg
+-rw-r--r--   0 soli      (1000) soli      (1000)     1157 2024-04-14 19:15:09.000000 esa-2scm-0.2.5/setup.py
+drwxr-xr-x   0 soli      (1000) soli      (1000)        0 2024-04-14 19:17:04.445683 esa-2scm-0.2.5/test/
+-rw-r--r--   0 soli      (1000) soli      (1000)     2101 2024-03-28 16:37:14.000000 esa-2scm-0.2.5/test/test_model.py
+-rw-r--r--   0 soli      (1000) soli      (1000)     2627 2024-03-23 19:40:59.000000 esa-2scm-0.2.5/test/test_syniv.py
```

### Comparing `esa-2scm-0.2.4/LICENSE` & `esa-2scm-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `esa-2scm-0.2.4/PKG-INFO` & `esa-2scm-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: esa-2scm
-Version: 0.2.4
+Version: 0.2.5
 Summary: ESA-2SCM Python Package for Causal Discovery
 Home-page: https://github.com/DSsoli/esa-2scm.git
 Author: Sanghoon Lee (DSsoli)
 Author-email: solisoli3197@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ESA-2SCM: Elastic Segment Allocation-based 2SLS Structural Causal Model for Causal Discovery
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/DSsoli/esa-2scm/blob/main/LICENSE)
+[![PyPI - Version](https://img.shields.io/pypi/v/esa-2scm)](https://pypi.org/project/esa-2scm/)
 
 ESA-2SCM is a new method for detecting causality based on Elastic Segment Allocation-based synthetic instrumental variables with 2SLS application for estimating structural causal models. 
 <br>
 <br>
 For details of the model design, please refer to my Original Article:
 
 * [Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 21. <snbperi.org/article/230>](http://www.snbperi.org/article/230)
```

### Comparing `esa-2scm-0.2.4/README.md` & `esa-2scm-0.2.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # ESA-2SCM: Elastic Segment Allocation-based 2SLS Structural Causal Model for Causal Discovery
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/DSsoli/esa-2scm/blob/main/LICENSE)
+[![PyPI - Version](https://img.shields.io/pypi/v/esa-2scm)](https://pypi.org/project/esa-2scm/)
 
 ESA-2SCM is a new method for detecting causality based on Elastic Segment Allocation-based synthetic instrumental variables with 2SLS application for estimating structural causal models. 
 <br>
 <br>
 For details of the model design, please refer to my Original Article:
 
 * [Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 21. <snbperi.org/article/230>](http://www.snbperi.org/article/230)
```

### Comparing `esa-2scm-0.2.4/esa_2scm/LICENSE` & `esa-2scm-0.2.5/esa_2scm/LICENSE`

 * *Files identical despite different names*

### Comparing `esa-2scm-0.2.4/esa_2scm/__init__.py` & `esa-2scm-0.2.5/esa_2scm/syniv/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,10 +3,8 @@
 For documentation and algorithm/methodology details, please refer to my original article: http://www.snbperi.org/article/230
 
 Should you use this package, I kindly request you to cite my article:
 Lee, Sanghoon (2024). ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable, SnB Political and Economic Research Institute, 1, 21. <snbperi.org/article/230>
 """
 
 
-__version__ = "0.2.4"
-
-from .models import Esa2Scm
+from .esa import SynIV, r2_score
```

### Comparing `esa-2scm-0.2.4/esa_2scm/models.py` & `esa-2scm-0.2.5/esa_2scm/models.py`

 * *Files identical despite different names*

### Comparing `esa-2scm-0.2.4/esa_2scm/syniv/__init__.py` & `esa-2scm-0.2.5/esa_2scm/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,8 +3,10 @@
 For documentation and algorithm/methodology details, please refer to my original article: http://www.snbperi.org/article/230
 
 Should you use this package, I kindly request you to cite my article:
 Lee, Sanghoon (2024). ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable, SnB Political and Economic Research Institute, 1, 21. <snbperi.org/article/230>
 """
 
 
-from .esa import SynIV, r2_score
+__version__ = "0.2.5"
+
+from .models import Esa2Scm
```

### Comparing `esa-2scm-0.2.4/esa_2scm/syniv/esa.py` & `esa-2scm-0.2.5/esa_2scm/syniv/esa.py`

 * *Files identical despite different names*

### Comparing `esa-2scm-0.2.4/esa_2scm.egg-info/PKG-INFO` & `esa-2scm-0.2.5/esa_2scm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: esa-2scm
-Version: 0.2.4
+Version: 0.2.5
 Summary: ESA-2SCM Python Package for Causal Discovery
 Home-page: https://github.com/DSsoli/esa-2scm.git
 Author: Sanghoon Lee (DSsoli)
 Author-email: solisoli3197@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ESA-2SCM: Elastic Segment Allocation-based 2SLS Structural Causal Model for Causal Discovery
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/DSsoli/esa-2scm/blob/main/LICENSE)
+[![PyPI - Version](https://img.shields.io/pypi/v/esa-2scm)](https://pypi.org/project/esa-2scm/)
 
 ESA-2SCM is a new method for detecting causality based on Elastic Segment Allocation-based synthetic instrumental variables with 2SLS application for estimating structural causal models. 
 <br>
 <br>
 For details of the model design, please refer to my Original Article:
 
 * [Lee, Sanghoon (2024). **ESA-2SCM for Causal Discovery: Causal Modeling with Elastic Segmentation-based Synthetic Instrumental Variable**, *SnB Political and Economic Research Institute,* *1,* 21. <snbperi.org/article/230>](http://www.snbperi.org/article/230)
```

### Comparing `esa-2scm-0.2.4/examples/example.ipynb` & `esa-2scm-0.2.5/examples/example.ipynb`

 * *Files identical despite different names*

### Comparing `esa-2scm-0.2.4/setup.py` & `esa-2scm-0.2.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 with open("README.md", "r", encoding='utf-8') as fh:
     README = fh.read()
 
 setup(
     author="Sanghoon Lee (DSsoli)",
     author_email="solisoli3197@gmail.com",
     name="esa-2scm",
-    version="0.2.4",
+    version="0.2.5",
     description="ESA-2SCM Python Package for Causal Discovery",
     long_description=README,
     long_description_content_type="text/markdown",
-    install_requires=["numpy", "pandas", "scipy", "scikit-learn"],
+    install_requires=["numpy", "pandas", "scipy"],
     url="https://github.com/DSsoli/esa-2scm.git",
     packages=find_packages(include=['esa_2scm', 'esa_2scm.*']),
     package_data={"esa_2scm": ['LICENSE', 'examples/*']},
     include_package_data=True
 )
```

### Comparing `esa-2scm-0.2.4/test/test_model.py` & `esa-2scm-0.2.5/test/test_model.py`

 * *Files identical despite different names*

### Comparing `esa-2scm-0.2.4/test/test_syniv.py` & `esa-2scm-0.2.5/test/test_syniv.py`

 * *Files identical despite different names*

