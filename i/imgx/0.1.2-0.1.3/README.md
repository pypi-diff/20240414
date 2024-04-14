# Comparing `tmp/imgx-0.1.2.tar.gz` & `tmp/imgx-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imgx-0.1.2.tar", last modified: Fri Apr 12 10:42:24 2024, max compression
+gzip compressed data, was "imgx-0.1.3.tar", last modified: Sun Apr 14 05:56:29 2024, max compression
```

## Comparing `imgx-0.1.2.tar` & `imgx-0.1.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 mina       (501) staff       (20)        0 2024-04-12 10:42:24.053250 imgx-0.1.2/
--rw-r--r--   0 mina       (501) staff       (20)      156 2024-04-05 10:34:18.000000 imgx-0.1.2/AUTHORS.rst
--rw-r--r--   0 mina       (501) staff       (20)     3469 2024-04-05 10:34:18.000000 imgx-0.1.2/CONTRIBUTING.rst
--rw-r--r--   0 mina       (501) staff       (20)       89 2024-04-05 10:34:18.000000 imgx-0.1.2/HISTORY.rst
--rw-r--r--   0 mina       (501) staff       (20)     1068 2024-04-05 10:34:18.000000 imgx-0.1.2/LICENSE
--rw-r--r--   0 mina       (501) staff       (20)      262 2024-04-05 10:34:18.000000 imgx-0.1.2/MANIFEST.in
--rw-r--r--   0 mina       (501) staff       (20)     1569 2024-04-12 10:42:24.053470 imgx-0.1.2/PKG-INFO
--rw-r--r--   0 mina       (501) staff       (20)      810 2024-04-05 10:34:18.000000 imgx-0.1.2/README.rst
-drwxr-xr-x   0 mina       (501) staff       (20)        0 2024-04-12 10:42:24.043888 imgx-0.1.2/docs/
--rw-r--r--   0 mina       (501) staff       (20)      605 2024-04-05 10:34:18.000000 imgx-0.1.2/docs/Makefile
--rw-r--r--   0 mina       (501) staff       (20)       28 2024-04-05 10:34:18.000000 imgx-0.1.2/docs/authors.rst
--rwxr-xr-x   0 mina       (501) staff       (20)     4730 2024-04-05 10:34:18.000000 imgx-0.1.2/docs/conf.py
--rw-r--r--   0 mina       (501) staff       (20)       33 2024-04-05 10:34:18.000000 imgx-0.1.2/docs/contributing.rst
--rw-r--r--   0 mina       (501) staff       (20)       28 2024-04-05 10:34:18.000000 imgx-0.1.2/docs/history.rst
--rw-r--r--   0 mina       (501) staff       (20)      301 2024-04-05 10:34:18.000000 imgx-0.1.2/docs/index.rst
--rw-r--r--   0 mina       (501) staff       (20)     1086 2024-04-05 10:34:18.000000 imgx-0.1.2/docs/installation.rst
--rw-r--r--   0 mina       (501) staff       (20)      802 2024-04-05 10:34:18.000000 imgx-0.1.2/docs/make.bat
--rw-r--r--   0 mina       (501) staff       (20)       27 2024-04-05 10:34:18.000000 imgx-0.1.2/docs/readme.rst
--rw-r--r--   0 mina       (501) staff       (20)       63 2024-04-05 10:34:18.000000 imgx-0.1.2/docs/usage.rst
-drwxr-xr-x   0 mina       (501) staff       (20)        0 2024-04-12 10:42:24.046524 imgx-0.1.2/imgx/
--rw-r--r--   0 mina       (501) staff       (20)      122 2024-04-05 10:34:18.000000 imgx-0.1.2/imgx/__init__.py
--rw-r--r--   0 mina       (501) staff       (20)      576 2024-04-12 10:10:53.000000 imgx-0.1.2/imgx/cli.py
--rw-r--r--   0 mina       (501) staff       (20)       19 2024-04-05 10:34:18.000000 imgx-0.1.2/imgx/imgx.py
--rw-r--r--   0 mina       (501) staff       (20)     4515 2024-04-12 10:40:26.000000 imgx-0.1.2/imgx/process_module.py
-drwxr-xr-x   0 mina       (501) staff       (20)        0 2024-04-12 10:42:24.051259 imgx-0.1.2/imgx.egg-info/
--rw-r--r--   0 mina       (501) staff       (20)     1569 2024-04-12 10:42:23.000000 imgx-0.1.2/imgx.egg-info/PKG-INFO
--rw-r--r--   0 mina       (501) staff       (20)      554 2024-04-12 10:42:23.000000 imgx-0.1.2/imgx.egg-info/SOURCES.txt
--rw-r--r--   0 mina       (501) staff       (20)        1 2024-04-12 10:42:23.000000 imgx-0.1.2/imgx.egg-info/dependency_links.txt
--rw-r--r--   0 mina       (501) staff       (20)       39 2024-04-12 10:42:23.000000 imgx-0.1.2/imgx.egg-info/entry_points.txt
--rw-r--r--   0 mina       (501) staff       (20)        1 2024-04-05 10:37:39.000000 imgx-0.1.2/imgx.egg-info/not-zip-safe
--rw-r--r--   0 mina       (501) staff       (20)       45 2024-04-12 10:42:23.000000 imgx-0.1.2/imgx.egg-info/requires.txt
--rw-r--r--   0 mina       (501) staff       (20)        5 2024-04-12 10:42:23.000000 imgx-0.1.2/imgx.egg-info/top_level.txt
--rw-r--r--   0 mina       (501) staff       (20)      419 2024-04-12 10:42:24.054635 imgx-0.1.2/setup.cfg
--rw-r--r--   0 mina       (501) staff       (20)     1380 2024-04-12 10:41:22.000000 imgx-0.1.2/setup.py
-drwxr-xr-x   0 mina       (501) staff       (20)        0 2024-04-12 10:42:24.052634 imgx-0.1.2/tests/
--rw-r--r--   0 mina       (501) staff       (20)       34 2024-04-05 10:34:18.000000 imgx-0.1.2/tests/__init__.py
--rw-r--r--   0 mina       (501) staff       (20)      964 2024-04-05 10:34:18.000000 imgx-0.1.2/tests/test_imgx.py
+drwxr-xr-x   0 mina       (501) staff       (20)        0 2024-04-14 05:56:29.745354 imgx-0.1.3/
+-rw-r--r--   0 mina       (501) staff       (20)      156 2024-04-05 10:34:18.000000 imgx-0.1.3/AUTHORS.rst
+-rw-r--r--   0 mina       (501) staff       (20)     3469 2024-04-05 10:34:18.000000 imgx-0.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 mina       (501) staff       (20)       89 2024-04-05 10:34:18.000000 imgx-0.1.3/HISTORY.rst
+-rw-r--r--   0 mina       (501) staff       (20)     1068 2024-04-05 10:34:18.000000 imgx-0.1.3/LICENSE
+-rw-r--r--   0 mina       (501) staff       (20)      262 2024-04-05 10:34:18.000000 imgx-0.1.3/MANIFEST.in
+-rw-r--r--   0 mina       (501) staff       (20)     3059 2024-04-14 05:56:29.745603 imgx-0.1.3/PKG-INFO
+-rw-r--r--   0 mina       (501) staff       (20)     2300 2024-04-14 05:55:58.000000 imgx-0.1.3/README.rst
+drwxr-xr-x   0 mina       (501) staff       (20)        0 2024-04-14 05:56:29.733987 imgx-0.1.3/docs/
+-rw-r--r--   0 mina       (501) staff       (20)      605 2024-04-05 10:34:18.000000 imgx-0.1.3/docs/Makefile
+-rw-r--r--   0 mina       (501) staff       (20)       28 2024-04-05 10:34:18.000000 imgx-0.1.3/docs/authors.rst
+-rwxr-xr-x   0 mina       (501) staff       (20)     4730 2024-04-05 10:34:18.000000 imgx-0.1.3/docs/conf.py
+-rw-r--r--   0 mina       (501) staff       (20)       33 2024-04-05 10:34:18.000000 imgx-0.1.3/docs/contributing.rst
+-rw-r--r--   0 mina       (501) staff       (20)       28 2024-04-05 10:34:18.000000 imgx-0.1.3/docs/history.rst
+-rw-r--r--   0 mina       (501) staff       (20)      301 2024-04-05 10:34:18.000000 imgx-0.1.3/docs/index.rst
+-rw-r--r--   0 mina       (501) staff       (20)     1086 2024-04-05 10:34:18.000000 imgx-0.1.3/docs/installation.rst
+-rw-r--r--   0 mina       (501) staff       (20)      802 2024-04-05 10:34:18.000000 imgx-0.1.3/docs/make.bat
+-rw-r--r--   0 mina       (501) staff       (20)       27 2024-04-05 10:34:18.000000 imgx-0.1.3/docs/readme.rst
+-rw-r--r--   0 mina       (501) staff       (20)       63 2024-04-05 10:34:18.000000 imgx-0.1.3/docs/usage.rst
+drwxr-xr-x   0 mina       (501) staff       (20)        0 2024-04-14 05:56:29.736864 imgx-0.1.3/imgx/
+-rw-r--r--   0 mina       (501) staff       (20)      122 2024-04-05 10:34:18.000000 imgx-0.1.3/imgx/__init__.py
+-rw-r--r--   0 mina       (501) staff       (20)      576 2024-04-12 10:10:53.000000 imgx-0.1.3/imgx/cli.py
+-rw-r--r--   0 mina       (501) staff       (20)       19 2024-04-05 10:34:18.000000 imgx-0.1.3/imgx/imgx.py
+-rw-r--r--   0 mina       (501) staff       (20)     4515 2024-04-12 10:40:26.000000 imgx-0.1.3/imgx/process_module.py
+drwxr-xr-x   0 mina       (501) staff       (20)        0 2024-04-14 05:56:29.742064 imgx-0.1.3/imgx.egg-info/
+-rw-r--r--   0 mina       (501) staff       (20)     3059 2024-04-14 05:56:29.000000 imgx-0.1.3/imgx.egg-info/PKG-INFO
+-rw-r--r--   0 mina       (501) staff       (20)      554 2024-04-14 05:56:29.000000 imgx-0.1.3/imgx.egg-info/SOURCES.txt
+-rw-r--r--   0 mina       (501) staff       (20)        1 2024-04-14 05:56:29.000000 imgx-0.1.3/imgx.egg-info/dependency_links.txt
+-rw-r--r--   0 mina       (501) staff       (20)       39 2024-04-14 05:56:29.000000 imgx-0.1.3/imgx.egg-info/entry_points.txt
+-rw-r--r--   0 mina       (501) staff       (20)        1 2024-04-05 10:37:39.000000 imgx-0.1.3/imgx.egg-info/not-zip-safe
+-rw-r--r--   0 mina       (501) staff       (20)       45 2024-04-14 05:56:29.000000 imgx-0.1.3/imgx.egg-info/requires.txt
+-rw-r--r--   0 mina       (501) staff       (20)        5 2024-04-14 05:56:29.000000 imgx-0.1.3/imgx.egg-info/top_level.txt
+-rw-r--r--   0 mina       (501) staff       (20)      419 2024-04-14 05:56:29.746964 imgx-0.1.3/setup.cfg
+-rw-r--r--   0 mina       (501) staff       (20)     1380 2024-04-14 05:56:08.000000 imgx-0.1.3/setup.py
+drwxr-xr-x   0 mina       (501) staff       (20)        0 2024-04-14 05:56:29.744194 imgx-0.1.3/tests/
+-rw-r--r--   0 mina       (501) staff       (20)       34 2024-04-05 10:34:18.000000 imgx-0.1.3/tests/__init__.py
+-rw-r--r--   0 mina       (501) staff       (20)      964 2024-04-05 10:34:18.000000 imgx-0.1.3/tests/test_imgx.py
```

### Comparing `imgx-0.1.2/CONTRIBUTING.rst` & `imgx-0.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `imgx-0.1.2/LICENSE` & `imgx-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `imgx-0.1.2/docs/Makefile` & `imgx-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `imgx-0.1.2/docs/conf.py` & `imgx-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `imgx-0.1.2/docs/installation.rst` & `imgx-0.1.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `imgx-0.1.2/docs/make.bat` & `imgx-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `imgx-0.1.2/imgx/cli.py` & `imgx-0.1.3/imgx/cli.py`

 * *Files identical despite different names*

### Comparing `imgx-0.1.2/imgx/process_module.py` & `imgx-0.1.3/imgx/process_module.py`

 * *Files identical despite different names*

### Comparing `imgx-0.1.2/imgx.egg-info/SOURCES.txt` & `imgx-0.1.3/imgx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `imgx-0.1.2/setup.py` & `imgx-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,10 +40,10 @@
     include_package_data=True,
     keywords='imgx',
     name='imgx',
     packages=find_packages(include=['imgx', 'imgx.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/M-Farag/imgx',
-    version='0.1.2',
+    version='0.1.3',
     zip_safe=False,
 )
```

### Comparing `imgx-0.1.2/tests/test_imgx.py` & `imgx-0.1.3/tests/test_imgx.py`

 * *Files identical despite different names*

