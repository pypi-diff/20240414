# Comparing `tmp/MLXpress-0.1.8.7.tar.gz` & `tmp/MLXpress-0.1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLXpress-0.1.8.7.tar", last modified: Thu Dec 14 15:55:03 2023, max compression
+gzip compressed data, was "MLXpress-0.1.8.8.tar", last modified: Sun Apr 14 12:06:56 2024, max compression
```

## Comparing `MLXpress-0.1.8.7.tar` & `MLXpress-0.1.8.8.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 vinilg7    (501) staff       (20)        0 2023-12-14 15:55:03.489340 MLXpress-0.1.8.7/
-drwxr-xr-x   0 vinilg7    (501) staff       (20)        0 2023-12-14 15:55:03.487893 MLXpress-0.1.8.7/MLXpress/
--rw-rw-r--   0 vinilg7    (501) staff       (20)        0 2023-07-14 01:21:38.000000 MLXpress-0.1.8.7/MLXpress/__init__.py
--rw-r--r--   0 vinilg7    (501) staff       (20)     5478 2023-12-13 11:57:53.000000 MLXpress-0.1.8.7/MLXpress/bigdata.py
--rw-rw-r--   0 vinilg7    (501) staff       (20)     2338 2023-07-16 23:45:14.000000 MLXpress-0.1.8.7/MLXpress/diabetes.py
--rw-r--r--   0 vinilg7    (501) staff       (20)     3360 2023-12-14 13:36:32.000000 MLXpress-0.1.8.7/MLXpress/help.py
--rw-rw-r--   0 vinilg7    (501) staff       (20)     4011 2023-07-17 06:11:02.000000 MLXpress-0.1.8.7/MLXpress/iris.py
--rw-r--r--   0 vinilg7    (501) staff       (20)     3240 2023-12-13 09:58:20.000000 MLXpress-0.1.8.7/MLXpress/math.py
--rw-r--r--   0 vinilg7    (501) staff       (20)    28135 2023-12-13 09:58:20.000000 MLXpress-0.1.8.7/MLXpress/ml.py
--rw-rw-r--   0 vinilg7    (501) staff       (20)     5030 2023-07-17 05:03:38.000000 MLXpress-0.1.8.7/MLXpress/preprocessing.py
--rw-rw-r--   0 vinilg7    (501) staff       (20)     1870 2023-07-17 05:24:56.000000 MLXpress-0.1.8.7/MLXpress/stats.py
--rw-rw-r--   0 vinilg7    (501) staff       (20)     2733 2023-07-17 06:10:32.000000 MLXpress-0.1.8.7/MLXpress/wine.py
-drwxr-xr-x   0 vinilg7    (501) staff       (20)        0 2023-12-14 15:55:03.488777 MLXpress-0.1.8.7/MLXpress.egg-info/
--rw-r--r--   0 vinilg7    (501) staff       (20)     2355 2023-12-14 15:55:03.000000 MLXpress-0.1.8.7/MLXpress.egg-info/PKG-INFO
--rw-r--r--   0 vinilg7    (501) staff       (20)      366 2023-12-14 15:55:03.000000 MLXpress-0.1.8.7/MLXpress.egg-info/SOURCES.txt
--rw-rw-r--   0 vinilg7    (501) staff       (20)        1 2023-12-14 15:55:03.000000 MLXpress-0.1.8.7/MLXpress.egg-info/dependency_links.txt
--rw-rw-r--   0 vinilg7    (501) staff       (20)       51 2023-12-14 15:55:03.000000 MLXpress-0.1.8.7/MLXpress.egg-info/requires.txt
--rw-rw-r--   0 vinilg7    (501) staff       (20)        9 2023-12-14 15:55:03.000000 MLXpress-0.1.8.7/MLXpress.egg-info/top_level.txt
--rw-r--r--   0 vinilg7    (501) staff       (20)     2355 2023-12-14 15:55:03.489119 MLXpress-0.1.8.7/PKG-INFO
--rw-rw-r--   0 vinilg7    (501) staff       (20)     1718 2023-07-16 07:37:28.000000 MLXpress-0.1.8.7/README.md
--rw-r--r--   0 vinilg7    (501) staff       (20)       38 2023-12-14 15:55:03.489390 MLXpress-0.1.8.7/setup.cfg
--rw-r--r--   0 vinilg7    (501) staff       (20)      890 2023-12-14 15:54:52.000000 MLXpress-0.1.8.7/setup.py
+drwxr-xr-x   0 vinilg7    (501) staff       (20)        0 2024-04-14 12:06:56.305877 MLXpress-0.1.8.8/
+drwxr-xr-x   0 vinilg7    (501) staff       (20)        0 2024-04-14 12:06:56.304334 MLXpress-0.1.8.8/MLXpress/
+-rw-rw-r--   0 vinilg7    (501) staff       (20)        0 2023-07-14 01:21:38.000000 MLXpress-0.1.8.8/MLXpress/__init__.py
+-rw-r--r--   0 vinilg7    (501) staff       (20)     5478 2023-12-13 11:57:53.000000 MLXpress-0.1.8.8/MLXpress/bigdata.py
+-rw-rw-r--   0 vinilg7    (501) staff       (20)     2338 2023-07-16 23:45:14.000000 MLXpress-0.1.8.8/MLXpress/diabetes.py
+-rw-r--r--   0 vinilg7    (501) staff       (20)     6232 2024-04-14 12:01:28.000000 MLXpress-0.1.8.8/MLXpress/getdata.py
+-rw-r--r--   0 vinilg7    (501) staff       (20)     3360 2023-12-14 13:36:32.000000 MLXpress-0.1.8.8/MLXpress/help.py
+-rw-rw-r--   0 vinilg7    (501) staff       (20)     4011 2023-07-17 06:11:02.000000 MLXpress-0.1.8.8/MLXpress/iris.py
+-rw-r--r--   0 vinilg7    (501) staff       (20)     3240 2023-12-13 09:58:20.000000 MLXpress-0.1.8.8/MLXpress/math.py
+-rw-r--r--   0 vinilg7    (501) staff       (20)    28135 2023-12-13 09:58:20.000000 MLXpress-0.1.8.8/MLXpress/ml.py
+-rw-rw-r--   0 vinilg7    (501) staff       (20)     5030 2023-07-17 05:03:38.000000 MLXpress-0.1.8.8/MLXpress/preprocessing.py
+-rw-rw-r--   0 vinilg7    (501) staff       (20)     1870 2023-07-17 05:24:56.000000 MLXpress-0.1.8.8/MLXpress/stats.py
+-rw-rw-r--   0 vinilg7    (501) staff       (20)     2733 2023-07-17 06:10:32.000000 MLXpress-0.1.8.8/MLXpress/wine.py
+drwxr-xr-x   0 vinilg7    (501) staff       (20)        0 2024-04-14 12:06:56.305304 MLXpress-0.1.8.8/MLXpress.egg-info/
+-rw-r--r--   0 vinilg7    (501) staff       (20)     2461 2024-04-14 12:06:56.000000 MLXpress-0.1.8.8/MLXpress.egg-info/PKG-INFO
+-rw-r--r--   0 vinilg7    (501) staff       (20)      386 2024-04-14 12:06:56.000000 MLXpress-0.1.8.8/MLXpress.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinilg7    (501) staff       (20)        1 2024-04-14 12:06:56.000000 MLXpress-0.1.8.8/MLXpress.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinilg7    (501) staff       (20)       97 2024-04-14 12:06:56.000000 MLXpress-0.1.8.8/MLXpress.egg-info/requires.txt
+-rw-rw-r--   0 vinilg7    (501) staff       (20)        9 2024-04-14 12:06:56.000000 MLXpress-0.1.8.8/MLXpress.egg-info/top_level.txt
+-rw-r--r--   0 vinilg7    (501) staff       (20)     2461 2024-04-14 12:06:56.305655 MLXpress-0.1.8.8/PKG-INFO
+-rw-rw-r--   0 vinilg7    (501) staff       (20)     1718 2023-07-16 07:37:28.000000 MLXpress-0.1.8.8/README.md
+-rw-r--r--   0 vinilg7    (501) staff       (20)       38 2024-04-14 12:06:56.305928 MLXpress-0.1.8.8/setup.cfg
+-rw-r--r--   0 vinilg7    (501) staff       (20)      981 2024-04-14 12:05:51.000000 MLXpress-0.1.8.8/setup.py
```

### Comparing `MLXpress-0.1.8.7/MLXpress/bigdata.py` & `MLXpress-0.1.8.8/MLXpress/bigdata.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.8.7/MLXpress/diabetes.py` & `MLXpress-0.1.8.8/MLXpress/diabetes.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.8.7/MLXpress/help.py` & `MLXpress-0.1.8.8/MLXpress/help.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.8.7/MLXpress/iris.py` & `MLXpress-0.1.8.8/MLXpress/iris.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.8.7/MLXpress/math.py` & `MLXpress-0.1.8.8/MLXpress/math.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.8.7/MLXpress/ml.py` & `MLXpress-0.1.8.8/MLXpress/ml.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.8.7/MLXpress/preprocessing.py` & `MLXpress-0.1.8.8/MLXpress/preprocessing.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.8.7/MLXpress/stats.py` & `MLXpress-0.1.8.8/MLXpress/stats.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.8.7/MLXpress/wine.py` & `MLXpress-0.1.8.8/MLXpress/wine.py`

 * *Files identical despite different names*

### Comparing `MLXpress-0.1.8.7/MLXpress.egg-info/PKG-INFO` & `MLXpress-0.1.8.8/MLXpress.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLXpress
-Version: 0.1.8.7
+Version: 0.1.8.8
 Summary: A powerful and user-friendly machine learning toolkit for data science and ML professionals to accelerate their workflow
 Author: vinilg7
 Author-email: vinilg7@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,18 @@
 Description-Content-Type: text/markdown
 Requires-Dist: scikit-learn
 Requires-Dist: pandas
 Requires-Dist: seaborn
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: scipy
+Requires-Dist: yfinance
+Requires-Dist: ccxt
+Requires-Dist: forex_python.converter
+Requires-Dist: datetime
 
 MLXpress is a comprehensive and intuitive machine learning toolkit that simplifies the development and deployment of machine learning models. It offers a wide range of essential functionalities for data science and ML professionals, enabling a streamlined and efficient workflow. With MLXpress, you can easily implement commonly used data science and ML functionality, making complex tasks simpler and more accessible.
 ### Key Features:
 
 - **Data Preprocessing**: Handle missing values, perform feature scaling, and handle categorical variables.
 - **Feature Selection**: Select the most relevant features using statistical tests and evaluation metrics.
 - **Model Evaluation**: Evaluate model performance using various metrics like accuracy, precision, recall, and F1 score.
```

### Comparing `MLXpress-0.1.8.7/PKG-INFO` & `MLXpress-0.1.8.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MLXpress
-Version: 0.1.8.7
+Version: 0.1.8.8
 Summary: A powerful and user-friendly machine learning toolkit for data science and ML professionals to accelerate their workflow
 Author: vinilg7
 Author-email: vinilg7@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,18 @@
 Description-Content-Type: text/markdown
 Requires-Dist: scikit-learn
 Requires-Dist: pandas
 Requires-Dist: seaborn
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: scipy
+Requires-Dist: yfinance
+Requires-Dist: ccxt
+Requires-Dist: forex_python.converter
+Requires-Dist: datetime
 
 MLXpress is a comprehensive and intuitive machine learning toolkit that simplifies the development and deployment of machine learning models. It offers a wide range of essential functionalities for data science and ML professionals, enabling a streamlined and efficient workflow. With MLXpress, you can easily implement commonly used data science and ML functionality, making complex tasks simpler and more accessible.
 ### Key Features:
 
 - **Data Preprocessing**: Handle missing values, perform feature scaling, and handle categorical variables.
 - **Feature Selection**: Select the most relevant features using statistical tests and evaluation metrics.
 - **Model Evaluation**: Evaluate model performance using various metrics like accuracy, precision, recall, and F1 score.
```

### Comparing `MLXpress-0.1.8.7/README.md` & `MLXpress-0.1.8.8/README.md`

 * *Files identical despite different names*

