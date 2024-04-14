# Comparing `tmp/testasteca-0.5.4.tar.gz` & `tmp/testasteca-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testasteca-0.5.4.tar", max compression
+gzip compressed data, was "testasteca-0.5.5.tar", max compression
```

## Comparing `testasteca-0.5.4.tar` & `testasteca-0.5.5.tar`

### file list

```diff
@@ -1,15 +1,4 @@
--rw-r--r--   0        0        0     1071 2024-01-17 13:11:31.936958 testasteca-0.5.4/LICENSE.txt
--rw-r--r--   0        0        0     1168 2024-01-17 12:49:09.904792 testasteca-0.5.4/README.md
--rw-r--r--   0        0        0      621 2024-04-14 14:45:55.575955 testasteca-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     1147 2024-04-12 19:41:45.687388 testasteca-0.5.4/testasteca/__init__.py
--rw-r--r--   0        0        0     5210 2024-04-11 15:06:07.537776 testasteca-0.5.4/testasteca/cluster.py
--rw-r--r--   0        0        0     4500 2024-04-06 12:59:39.883072 testasteca-0.5.4/testasteca/isochrones.py
--rw-r--r--   0        0        0     3034 2024-04-06 12:59:39.867071 testasteca-0.5.4/testasteca/likelihood.py
--rw-r--r--   0        0        0        0 2017-08-07 21:46:26.427264 testasteca-0.5.4/testasteca/modules/__init__.py
--rw-r--r--   0        0        0     3725 2024-04-13 14:53:07.514535 testasteca-0.5.4/testasteca/modules/imfs.py
--rw-r--r--   0        0        0    17615 2024-04-06 12:59:40.319079 testasteca-0.5.4/testasteca/modules/isochrones_priv.py
--rw-r--r--   0        0        0     9947 2024-04-06 12:59:40.119075 testasteca-0.5.4/testasteca/modules/likelihood_priv.py
--rw-r--r--   0        0        0     7845 2024-04-13 14:53:07.526535 testasteca-0.5.4/testasteca/modules/mass_binary.py
--rw-r--r--   0        0        0    32517 2024-04-13 14:44:29.560876 testasteca-0.5.4/testasteca/modules/synth_cluster_priv.py
--rw-r--r--   0        0        0    17822 2024-04-14 13:07:56.970990 testasteca-0.5.4/testasteca/synthetic.py
--rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 testasteca-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-01-17 13:11:31.936959 testasteca-0.5.5/LICENSE.txt
+-rw-r--r--   0        0        0     1168 2024-01-17 12:49:09.904793 testasteca-0.5.5/README.md
+-rw-r--r--   0        0        0      621 2024-04-14 14:58:33.675943 testasteca-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 testasteca-0.5.5/PKG-INFO
```

### Comparing `testasteca-0.5.4/LICENSE.txt` & `testasteca-0.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `testasteca-0.5.4/README.md` & `testasteca-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `testasteca-0.5.4/pyproject.toml` & `testasteca-0.5.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "testasteca"
-version = "0.5.4"
+version = "0.5.5"
 description = "Stellar cluster analysis package"
 authors = ["Gabriel I Perren <gabrielperren@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 keywords = ["cluster", "astrophysics"]
 homepage = "https://asteca.github.io/"
 repository = "https://github.com/asteca/ASteCA"
```

### Comparing `testasteca-0.5.4/PKG-INFO` & `testasteca-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testasteca
-Version: 0.5.4
+Version: 0.5.5
 Summary: Stellar cluster analysis package
 Home-page: https://asteca.github.io/
 License: MIT
 Keywords: cluster,astrophysics
 Author: Gabriel I Perren
 Author-email: gabrielperren@gmail.com
 Requires-Python: >=3.11,<4.0
```

