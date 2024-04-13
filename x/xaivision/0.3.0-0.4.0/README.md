# Comparing `tmp/xaivision-0.3.0.tar.gz` & `tmp/xaivision-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xaivision-0.3.0.tar", max compression
+gzip compressed data, was "xaivision-0.4.0.tar", max compression
```

## Comparing `xaivision-0.3.0.tar` & `xaivision-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1114 2024-04-11 11:21:56.989947 xaivision-0.3.0/README.md
--rw-r--r--   0        0        0      265 2024-04-13 22:39:38.482813 xaivision-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       61 2024-04-13 15:44:32.244089 xaivision-0.3.0/xaivision/__init__.py
--rw-r--r--   0        0        0     2847 2024-04-13 21:30:38.041957 xaivision-0.3.0/xaivision/nmf_func.py
--rw-r--r--   0        0        0    12632 2024-04-13 22:06:09.038199 xaivision-0.3.0/xaivision/utils.py
--rw-r--r--   0        0        0     6856 2024-04-13 22:02:31.965352 xaivision-0.3.0/xaivision/xai_tools.py
--rw-r--r--   0        0        0     1392 1970-01-01 00:00:00.000000 xaivision-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1114 2024-04-11 11:21:56.989947 xaivision-0.4.0/README.md
+-rw-r--r--   0        0        0      265 2024-04-13 22:47:53.255997 xaivision-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       61 2024-04-13 15:44:32.244089 xaivision-0.4.0/xaivision/__init__.py
+-rw-r--r--   0        0        0     2847 2024-04-13 21:30:38.041957 xaivision-0.4.0/xaivision/nmf_func.py
+-rw-r--r--   0        0        0    12632 2024-04-13 22:06:09.038199 xaivision-0.4.0/xaivision/utils.py
+-rw-r--r--   0        0        0     6856 2024-04-13 22:02:31.965352 xaivision-0.4.0/xaivision/xai_tools.py
+-rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 xaivision-0.4.0/PKG-INFO
```

### Comparing `xaivision-0.3.0/README.md` & `xaivision-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `xaivision-0.3.0/xaivision/nmf_func.py` & `xaivision-0.4.0/xaivision/nmf_func.py`

 * *Files identical despite different names*

### Comparing `xaivision-0.3.0/xaivision/utils.py` & `xaivision-0.4.0/xaivision/utils.py`

 * *Files identical despite different names*

### Comparing `xaivision-0.3.0/xaivision/xai_tools.py` & `xaivision-0.4.0/xaivision/xai_tools.py`

 * *Files identical despite different names*

### Comparing `xaivision-0.3.0/PKG-INFO` & `xaivision-0.4.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: xaivision
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 Author: philorfa
 Author-email: phil.orfa@gmail.com
-Requires-Python: >3.11
+Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 
 # Explainable AI (XAI)
 
 ## Introduction
```

