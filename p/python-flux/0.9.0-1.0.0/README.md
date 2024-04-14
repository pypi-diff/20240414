# Comparing `tmp/python_flux-0.9.0.tar.gz` & `tmp/python_flux-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_flux-0.9.0.tar", max compression
+gzip compressed data, was "python_flux-1.0.0.tar", max compression
```

## Comparing `python_flux-0.9.0.tar` & `python_flux-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0      719 2024-04-11 04:42:26.800886 python_flux-0.9.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-0.9.0/python_flux/__init__.py
--rw-r--r--   0        0        0     7123 2024-04-11 02:03:51.782589 python_flux-0.9.0/python_flux/flux.py
--rw-r--r--   0        0        0     1182 2022-12-06 14:51:39.000000 python_flux-0.9.0/python_flux/producers.py
--rw-r--r--   0        0        0      858 2022-09-13 18:15:28.000000 python_flux-0.9.0/python_flux/subscribers.py
--rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 python_flux-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      719 2024-04-13 23:26:20.252584 python_flux-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-07-20 21:55:18.000000 python_flux-1.0.0/python_flux/__init__.py
+-rw-r--r--   0        0        0    14870 2024-04-14 00:16:09.911500 python_flux-1.0.0/python_flux/flux.py
+-rw-r--r--   0        0        0      736 2024-04-13 23:50:57.491246 python_flux-1.0.0/python_flux/flux_utilis.py
+-rw-r--r--   0        0        0     1522 2024-04-13 21:23:45.466753 python_flux-1.0.0/python_flux/producers.py
+-rw-r--r--   0        0        0     1248 2024-04-13 22:38:54.621949 python_flux-1.0.0/python_flux/subscribers.py
+-rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 python_flux-1.0.0/PKG-INFO
```

### Comparing `python_flux-0.9.0/pyproject.toml` & `python_flux-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-flux"
-version = "0.9.0"
+version = "1.0.0"
 description = "Librería que utiliza generadores de python para simular procesamiento de flujo de datos"
 authors = ["Juan Pablo Bochard <jbochard@gmail.com>"]
 license = "GPL-3.0-or-later"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
```

### Comparing `python_flux-0.9.0/PKG-INFO` & `python_flux-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-flux
-Version: 0.9.0
+Version: 1.0.0
 Summary: Librería que utiliza generadores de python para simular procesamiento de flujo de datos
 License: GPL-3.0-or-later
 Author: Juan Pablo Bochard
 Author-email: jbochard@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

