# Comparing `tmp/testasteca-0.5.5.tar.gz` & `tmp/testasteca-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testasteca-0.5.5.tar", max compression
+gzip compressed data, was "testasteca-0.5.6.tar", max compression
```

## Comparing `testasteca-0.5.5.tar` & `testasteca-0.5.6.tar`

### file list

```diff
@@ -1,4 +1,21 @@
--rw-r--r--   0        0        0     1071 2024-01-17 13:11:31.936959 testasteca-0.5.5/LICENSE.txt
--rw-r--r--   0        0        0     1168 2024-01-17 12:49:09.904793 testasteca-0.5.5/README.md
--rw-r--r--   0        0        0      621 2024-04-14 14:58:33.675943 testasteca-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 testasteca-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-01-17 13:11:31.936958 testasteca-0.5.6/LICENSE.txt
+-rw-r--r--   0        0        0     1168 2024-01-17 12:49:09.904792 testasteca-0.5.6/README.md
+-rw-r--r--   0        0        0      622 2024-04-14 15:06:05.670916 testasteca-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     1147 2024-04-12 19:41:45.687388 testasteca-0.5.6/testasteca/__init__.py
+-rw-r--r--   0        0        0     5210 2024-04-11 15:06:07.537776 testasteca-0.5.6/testasteca/cluster.py
+-rw-r--r--   0        0        0     4500 2024-04-06 12:59:39.883072 testasteca-0.5.6/testasteca/isochrones.py
+-rw-r--r--   0        0        0     3034 2024-04-06 12:59:39.867071 testasteca-0.5.6/testasteca/likelihood.py
+-rw-r--r--   0        0        0        0 2017-08-07 21:46:26.427264 testasteca-0.5.6/testasteca/modules/__init__.py
+-rw-r--r--   0        0        0      181 2024-04-14 14:04:42.250786 testasteca-0.5.6/testasteca/modules/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4671 2024-04-14 14:04:43.298823 testasteca-0.5.6/testasteca/modules/__pycache__/imfs.cpython-311.pyc
+-rw-r--r--   0        0        0    22255 2024-04-14 14:04:42.254786 testasteca-0.5.6/testasteca/modules/__pycache__/isochrones_priv.cpython-311.pyc
+-rw-r--r--   0        0        0    10795 2024-04-14 14:04:43.758839 testasteca-0.5.6/testasteca/modules/__pycache__/likelihood_priv.cpython-311.pyc
+-rw-r--r--   0        0        0     9736 2024-04-14 14:04:43.302823 testasteca-0.5.6/testasteca/modules/__pycache__/mass_binary.cpython-311.pyc
+-rw-r--r--   0        0        0    31633 2024-04-14 14:04:42.954811 testasteca-0.5.6/testasteca/modules/__pycache__/synth_cluster_priv.cpython-311.pyc
+-rw-r--r--   0        0        0     3725 2024-04-13 14:53:07.514535 testasteca-0.5.6/testasteca/modules/imfs.py
+-rw-r--r--   0        0        0    17615 2024-04-06 12:59:40.319079 testasteca-0.5.6/testasteca/modules/isochrones_priv.py
+-rw-r--r--   0        0        0     9947 2024-04-06 12:59:40.119075 testasteca-0.5.6/testasteca/modules/likelihood_priv.py
+-rw-r--r--   0        0        0     7845 2024-04-13 14:53:07.526535 testasteca-0.5.6/testasteca/modules/mass_binary.py
+-rw-r--r--   0        0        0    32517 2024-04-13 14:44:29.560876 testasteca-0.5.6/testasteca/modules/synth_cluster_priv.py
+-rw-r--r--   0        0        0    17822 2024-04-14 13:07:56.970990 testasteca-0.5.6/testasteca/synthetic.py
+-rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 testasteca-0.5.6/PKG-INFO
```

### Comparing `testasteca-0.5.5/LICENSE.txt` & `testasteca-0.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `testasteca-0.5.5/README.md` & `testasteca-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `testasteca-0.5.5/pyproject.toml` & `testasteca-0.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "testasteca"
-version = "0.5.5"
+version = "0.5.6"
 description = "Stellar cluster analysis package"
 authors = ["Gabriel I Perren <gabrielperren@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 keywords = ["cluster", "astrophysics"]
 homepage = "https://asteca.github.io/"
 repository = "https://github.com/asteca/ASteCA"
@@ -16,10 +16,11 @@
 matplotlib = "^3.8.4"
 scipy = "^1.13.0"
 astropy = "^6.0.1"
 pandas = "^2.2.2"
 fast-histogram = "^0.12"
 
 
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `testasteca-0.5.5/PKG-INFO` & `testasteca-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testasteca
-Version: 0.5.5
+Version: 0.5.6
 Summary: Stellar cluster analysis package
 Home-page: https://asteca.github.io/
 License: MIT
 Keywords: cluster,astrophysics
 Author: Gabriel I Perren
 Author-email: gabrielperren@gmail.com
 Requires-Python: >=3.11,<4.0
```

