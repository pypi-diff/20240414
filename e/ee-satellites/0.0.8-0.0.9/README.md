# Comparing `tmp/ee_satellites-0.0.8.tar.gz` & `tmp/ee_satellites-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ee_satellites-0.0.8.tar", last modified: Wed Aug 30 13:21:54 2023, max compression
+gzip compressed data, was "ee_satellites-0.0.9.tar", last modified: Wed Aug 30 13:34:36 2023, max compression
```

## Comparing `ee_satellites-0.0.8.tar` & `ee_satellites-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 francesco   (501) staff       (20)        0 2023-08-30 13:21:54.228889 ee_satellites-0.0.8/
--rwxr-xr-x   0 francesco   (501) staff       (20)     1071 2023-07-11 07:39:43.000000 ee_satellites-0.0.8/LICENSE
--rw-r--r--   0 francesco   (501) staff       (20)     8296 2023-08-30 13:21:54.229092 ee_satellites-0.0.8/PKG-INFO
--rwxr-xr-x   0 francesco   (501) staff       (20)     7518 2023-08-30 13:05:19.000000 ee_satellites-0.0.8/README.md
-drwxr-xr-x   0 francesco   (501) staff       (20)        0 2023-08-30 13:21:54.228417 ee_satellites-0.0.8/ee_satellites.egg-info/
--rw-r--r--   0 francesco   (501) staff       (20)     8296 2023-08-30 13:21:54.000000 ee_satellites-0.0.8/ee_satellites.egg-info/PKG-INFO
--rw-r--r--   0 francesco   (501) staff       (20)      281 2023-08-30 13:21:54.000000 ee_satellites-0.0.8/ee_satellites.egg-info/SOURCES.txt
--rw-r--r--   0 francesco   (501) staff       (20)        1 2023-08-30 13:21:54.000000 ee_satellites-0.0.8/ee_satellites.egg-info/dependency_links.txt
--rw-r--r--   0 francesco   (501) staff       (20)       23 2023-08-30 13:21:54.000000 ee_satellites-0.0.8/ee_satellites.egg-info/requires.txt
--rw-r--r--   0 francesco   (501) staff       (20)       43 2023-08-30 13:21:54.000000 ee_satellites-0.0.8/ee_satellites.egg-info/top_level.txt
--rwxr-xr-x   0 francesco   (501) staff       (20)    18541 2023-07-11 12:47:07.000000 ee_satellites-0.0.8/ee_satellites.py
--rwxr-xr-x   0 francesco   (501) staff       (20)     2040 2023-07-11 12:13:24.000000 ee_satellites-0.0.8/landsat8.py
--rw-r--r--   0 francesco   (501) staff       (20)       89 2023-07-11 07:39:43.000000 ee_satellites-0.0.8/pyproject.toml
--rwxr-xr-x   0 francesco   (501) staff       (20)     7982 2023-07-11 07:39:43.000000 ee_satellites-0.0.8/sentinel1.py
--rwxr-xr-x   0 francesco   (501) staff       (20)    20297 2023-07-11 12:50:38.000000 ee_satellites-0.0.8/sentinel2.py
--rw-r--r--   0 francesco   (501) staff       (20)      883 2023-08-30 13:21:54.230340 ee_satellites-0.0.8/setup.cfg
+drwxr-xr-x   0 francesco   (501) staff       (20)        0 2023-08-30 13:34:36.820653 ee_satellites-0.0.9/
+-rwxr-xr-x   0 francesco   (501) staff       (20)     1071 2023-07-11 07:39:43.000000 ee_satellites-0.0.9/LICENSE
+-rw-r--r--   0 francesco   (501) staff       (20)     8301 2023-08-30 13:34:36.820820 ee_satellites-0.0.9/PKG-INFO
+-rwxr-xr-x   0 francesco   (501) staff       (20)     7523 2023-08-30 13:32:52.000000 ee_satellites-0.0.9/README.md
+drwxr-xr-x   0 francesco   (501) staff       (20)        0 2023-08-30 13:34:36.820140 ee_satellites-0.0.9/ee_satellites.egg-info/
+-rw-r--r--   0 francesco   (501) staff       (20)     8301 2023-08-30 13:34:36.000000 ee_satellites-0.0.9/ee_satellites.egg-info/PKG-INFO
+-rw-r--r--   0 francesco   (501) staff       (20)      281 2023-08-30 13:34:36.000000 ee_satellites-0.0.9/ee_satellites.egg-info/SOURCES.txt
+-rw-r--r--   0 francesco   (501) staff       (20)        1 2023-08-30 13:34:36.000000 ee_satellites-0.0.9/ee_satellites.egg-info/dependency_links.txt
+-rw-r--r--   0 francesco   (501) staff       (20)       23 2023-08-30 13:34:36.000000 ee_satellites-0.0.9/ee_satellites.egg-info/requires.txt
+-rw-r--r--   0 francesco   (501) staff       (20)       43 2023-08-30 13:34:36.000000 ee_satellites-0.0.9/ee_satellites.egg-info/top_level.txt
+-rwxr-xr-x   0 francesco   (501) staff       (20)    18541 2023-07-11 12:47:07.000000 ee_satellites-0.0.9/ee_satellites.py
+-rwxr-xr-x   0 francesco   (501) staff       (20)     2040 2023-07-11 12:13:24.000000 ee_satellites-0.0.9/landsat8.py
+-rw-r--r--   0 francesco   (501) staff       (20)       89 2023-07-11 07:39:43.000000 ee_satellites-0.0.9/pyproject.toml
+-rwxr-xr-x   0 francesco   (501) staff       (20)     7982 2023-07-11 07:39:43.000000 ee_satellites-0.0.9/sentinel1.py
+-rwxr-xr-x   0 francesco   (501) staff       (20)    20297 2023-07-11 12:50:38.000000 ee_satellites-0.0.9/sentinel2.py
+-rw-r--r--   0 francesco   (501) staff       (20)      883 2023-08-30 13:34:36.821417 ee_satellites-0.0.9/setup.cfg
```

### Comparing `ee_satellites-0.0.8/LICENSE` & `ee_satellites-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ee_satellites-0.0.8/PKG-INFO` & `ee_satellites-0.0.9/ee_satellites.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ee_satellites
-Version: 0.0.8
+Name: ee-satellites
+Version: 0.0.9
 Summary: A Python library that allows to extract data from satellites, exploiting machine parallelism and relying on Google Earth Engine APIs.
 Home-page: https://github.com/Amatofrancesco99/master-thesis/tree/main/Notebooks/1-features-extraction/utils
 Author: Francesco Amato
 Author-email: amatofrancesco99@gmail.com
 License: mit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,15 +22,15 @@
 
 <img src="https://i.ibb.co/bPMchfz/logo.png" alt="logo" border="0"><br>
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-yellow.svg)](https://github.com/Amatofrancesco99/master-thesis/blob/main/Notebooks/1-features-extraction/utils/LICENSE)
 ![maintained](https://img.shields.io/badge/maintained%3F-YES-green.svg)
 ![stars](https://img.shields.io/github/stars/Amatofrancesco99/master-thesis.svg)
 ![forks](https://img.shields.io/github/forks/Amatofrancesco99/master-thesis.svg)
-![watchers](https://img.shields.io/github/watchers/Amatofrancesco99/master-thesis.svg)
+![watchers](https://img.shields.io/github/watchers/Amatofrancesco99/master-thesis.svg) <br>
 ![GitHub last commit](https://img.shields.io/github/last-commit/Amatofrancesco99/master-thesis)
 ![GitHub contributors](https://img.shields.io/github/contributors/Amatofrancesco99/master-thesis)
 ![GitHub issues](https://img.shields.io/github/issues/Amatofrancesco99/master-thesis)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/Amatofrancesco99/master-thesis)
 
 </div><br>
 
@@ -41,15 +41,15 @@
 
 ### **Installation**
 The easiest way to install `ee-satellites` is by using `pip`:
 ```bash
 $ pip install ee-satellites
 ```
 
-*(Disclaimer: This project is currently under development.)*
+*(Disclaimer: This library is under continous development.)*
 
 ## **Functions** 
 Expand the function you wish to grasp more details about.
     <details> 
         <summary><b>`get_features()`</b></summary>
 
 It allows to get from an [input pandas DataFrame](#input-dataframe) composed of fields information, [an output DataFrame](#output-dataframe) that contains for each time a [selected satellite](#how-to-execute-it) (sentinel-1, sentinel-2 or landsat-8) passed over the specified fields, within a given time period, all the mean values of some of the most used indexes (optical, radar or thermal).
```

### Comparing `ee_satellites-0.0.8/README.md` & `ee_satellites-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 <img src="https://i.ibb.co/bPMchfz/logo.png" alt="logo" border="0"><br>
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-yellow.svg)](https://github.com/Amatofrancesco99/master-thesis/blob/main/Notebooks/1-features-extraction/utils/LICENSE)
 ![maintained](https://img.shields.io/badge/maintained%3F-YES-green.svg)
 ![stars](https://img.shields.io/github/stars/Amatofrancesco99/master-thesis.svg)
 ![forks](https://img.shields.io/github/forks/Amatofrancesco99/master-thesis.svg)
-![watchers](https://img.shields.io/github/watchers/Amatofrancesco99/master-thesis.svg)
+![watchers](https://img.shields.io/github/watchers/Amatofrancesco99/master-thesis.svg) <br>
 ![GitHub last commit](https://img.shields.io/github/last-commit/Amatofrancesco99/master-thesis)
 ![GitHub contributors](https://img.shields.io/github/contributors/Amatofrancesco99/master-thesis)
 ![GitHub issues](https://img.shields.io/github/issues/Amatofrancesco99/master-thesis)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/Amatofrancesco99/master-thesis)
 
 </div><br>
 
@@ -23,15 +23,15 @@
 
 ### **Installation**
 The easiest way to install `ee-satellites` is by using `pip`:
 ```bash
 $ pip install ee-satellites
 ```
 
-*(Disclaimer: This project is currently under development.)*
+*(Disclaimer: This library is under continous development.)*
 
 ## **Functions** 
 Expand the function you wish to grasp more details about.
     <details> 
         <summary><b>`get_features()`</b></summary>
 
 It allows to get from an [input pandas DataFrame](#input-dataframe) composed of fields information, [an output DataFrame](#output-dataframe) that contains for each time a [selected satellite](#how-to-execute-it) (sentinel-1, sentinel-2 or landsat-8) passed over the specified fields, within a given time period, all the mean values of some of the most used indexes (optical, radar or thermal).
```

### Comparing `ee_satellites-0.0.8/ee_satellites.egg-info/PKG-INFO` & `ee_satellites-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ee-satellites
-Version: 0.0.8
+Name: ee_satellites
+Version: 0.0.9
 Summary: A Python library that allows to extract data from satellites, exploiting machine parallelism and relying on Google Earth Engine APIs.
 Home-page: https://github.com/Amatofrancesco99/master-thesis/tree/main/Notebooks/1-features-extraction/utils
 Author: Francesco Amato
 Author-email: amatofrancesco99@gmail.com
 License: mit
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -22,15 +22,15 @@
 
 <img src="https://i.ibb.co/bPMchfz/logo.png" alt="logo" border="0"><br>
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-yellow.svg)](https://github.com/Amatofrancesco99/master-thesis/blob/main/Notebooks/1-features-extraction/utils/LICENSE)
 ![maintained](https://img.shields.io/badge/maintained%3F-YES-green.svg)
 ![stars](https://img.shields.io/github/stars/Amatofrancesco99/master-thesis.svg)
 ![forks](https://img.shields.io/github/forks/Amatofrancesco99/master-thesis.svg)
-![watchers](https://img.shields.io/github/watchers/Amatofrancesco99/master-thesis.svg)
+![watchers](https://img.shields.io/github/watchers/Amatofrancesco99/master-thesis.svg) <br>
 ![GitHub last commit](https://img.shields.io/github/last-commit/Amatofrancesco99/master-thesis)
 ![GitHub contributors](https://img.shields.io/github/contributors/Amatofrancesco99/master-thesis)
 ![GitHub issues](https://img.shields.io/github/issues/Amatofrancesco99/master-thesis)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/Amatofrancesco99/master-thesis)
 
 </div><br>
 
@@ -41,15 +41,15 @@
 
 ### **Installation**
 The easiest way to install `ee-satellites` is by using `pip`:
 ```bash
 $ pip install ee-satellites
 ```
 
-*(Disclaimer: This project is currently under development.)*
+*(Disclaimer: This library is under continous development.)*
 
 ## **Functions** 
 Expand the function you wish to grasp more details about.
     <details> 
         <summary><b>`get_features()`</b></summary>
 
 It allows to get from an [input pandas DataFrame](#input-dataframe) composed of fields information, [an output DataFrame](#output-dataframe) that contains for each time a [selected satellite](#how-to-execute-it) (sentinel-1, sentinel-2 or landsat-8) passed over the specified fields, within a given time period, all the mean values of some of the most used indexes (optical, radar or thermal).
```

### Comparing `ee_satellites-0.0.8/ee_satellites.py` & `ee_satellites-0.0.9/ee_satellites.py`

 * *Files identical despite different names*

### Comparing `ee_satellites-0.0.8/landsat8.py` & `ee_satellites-0.0.9/landsat8.py`

 * *Files identical despite different names*

### Comparing `ee_satellites-0.0.8/sentinel1.py` & `ee_satellites-0.0.9/sentinel1.py`

 * *Files identical despite different names*

### Comparing `ee_satellites-0.0.8/sentinel2.py` & `ee_satellites-0.0.9/sentinel2.py`

 * *Files identical despite different names*

### Comparing `ee_satellites-0.0.8/setup.cfg` & `ee_satellites-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ee_satellites
-version = 0.0.8
+version = 0.0.9
 author = Francesco Amato
 author_email = amatofrancesco99@gmail.com
 description = A Python library that allows to extract data from satellites, exploiting machine parallelism and relying on Google Earth Engine APIs.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = mit
 url = https://github.com/Amatofrancesco99/master-thesis/tree/main/Notebooks/1-features-extraction/utils
```

