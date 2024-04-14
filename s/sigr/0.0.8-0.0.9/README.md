# Comparing `tmp/sigr-0.0.8.tar.gz` & `tmp/sigr-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigr-0.0.8.tar", last modified: Sat Mar 16 17:17:47 2024, max compression
+gzip compressed data, was "sigr-0.0.9.tar", last modified: Sun Mar 17 17:03:00 2024, max compression
```

## Comparing `sigr-0.0.8.tar` & `sigr-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-16 17:17:47.264306 sigr-0.0.8/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2024-02-16 20:20:17.000000 sigr-0.0.8/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2024-02-16 20:20:17.000000 sigr-0.0.8/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     1989 2024-03-16 17:17:47.264175 sigr-0.0.8/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1431 2024-02-24 20:30:35.000000 sigr-0.0.8/README.md
--rw-r--r--   0 solst      (501) staff       (20)      735 2024-03-11 20:32:35.000000 sigr-0.0.8/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2024-03-16 17:17:47.264346 sigr-0.0.8/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2580 2024-02-16 20:20:17.000000 sigr-0.0.8/setup.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-16 17:17:47.262900 sigr-0.0.8/sigr/
--rw-r--r--   0 solst      (501) staff       (20)      946 2024-03-16 17:17:44.000000 sigr-0.0.8/sigr/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    10982 2024-03-16 17:17:44.000000 sigr-0.0.8/sigr/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     1671 2024-03-16 17:17:44.000000 sigr-0.0.8/sigr/attr.py
--rw-r--r--   0 solst      (501) staff       (20)     1655 2024-03-16 17:17:44.000000 sigr-0.0.8/sigr/bcls.py
--rw-r--r--   0 solst      (501) staff       (20)    10962 2024-03-16 17:17:44.000000 sigr-0.0.8/sigr/bnds.py
--rw-r--r--   0 solst      (501) staff       (20)     2078 2024-03-16 17:17:44.000000 sigr-0.0.8/sigr/cons.py
--rw-r--r--   0 solst      (501) staff       (20)     8736 2024-03-16 17:17:44.000000 sigr-0.0.8/sigr/deco.py
--rw-r--r--   0 solst      (501) staff       (20)    10883 2024-03-16 17:17:44.000000 sigr-0.0.8/sigr/enum.py
--rw-r--r--   0 solst      (501) staff       (20)     3835 2024-03-16 17:17:44.000000 sigr-0.0.8/sigr/grds.py
--rw-r--r--   0 solst      (501) staff       (20)    15096 2024-03-16 17:17:44.000000 sigr-0.0.8/sigr/sigs.py
--rw-r--r--   0 solst      (501) staff       (20)    14949 2024-03-16 17:17:44.000000 sigr-0.0.8/sigr/type.py
--rw-r--r--   0 solst      (501) staff       (20)    21104 2024-03-16 17:17:44.000000 sigr-0.0.8/sigr/util.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-16 17:17:47.263862 sigr-0.0.8/sigr.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     1989 2024-03-16 17:17:47.000000 sigr-0.0.8/sigr.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      411 2024-03-16 17:17:47.000000 sigr-0.0.8/sigr.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-16 17:17:47.000000 sigr-0.0.8/sigr.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2024-03-16 17:17:47.000000 sigr-0.0.8/sigr.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-02-24 20:27:32.000000 sigr-0.0.8/sigr.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)        7 2024-03-16 17:17:47.000000 sigr-0.0.8/sigr.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2024-03-16 17:17:47.000000 sigr-0.0.8/sigr.egg-info/top_level.txt
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-17 17:03:00.613389 sigr-0.0.9/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2024-02-16 20:20:17.000000 sigr-0.0.9/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2024-02-16 20:20:17.000000 sigr-0.0.9/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     1989 2024-03-17 17:03:00.613253 sigr-0.0.9/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1431 2024-02-24 20:30:35.000000 sigr-0.0.9/README.md
+-rw-r--r--   0 solst      (501) staff       (20)      735 2024-03-16 17:18:51.000000 sigr-0.0.9/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2024-03-17 17:03:00.613428 sigr-0.0.9/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2580 2024-02-16 20:20:17.000000 sigr-0.0.9/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-17 17:03:00.612032 sigr-0.0.9/sigr/
+-rw-r--r--   0 solst      (501) staff       (20)      946 2024-03-17 17:02:58.000000 sigr-0.0.9/sigr/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    10982 2024-03-17 17:02:58.000000 sigr-0.0.9/sigr/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     1671 2024-03-17 17:02:58.000000 sigr-0.0.9/sigr/attr.py
+-rw-r--r--   0 solst      (501) staff       (20)     1655 2024-03-17 17:02:58.000000 sigr-0.0.9/sigr/bcls.py
+-rw-r--r--   0 solst      (501) staff       (20)    10962 2024-03-17 17:02:58.000000 sigr-0.0.9/sigr/bnds.py
+-rw-r--r--   0 solst      (501) staff       (20)     2078 2024-03-17 17:02:58.000000 sigr-0.0.9/sigr/cons.py
+-rw-r--r--   0 solst      (501) staff       (20)     8736 2024-03-17 17:02:58.000000 sigr-0.0.9/sigr/deco.py
+-rw-r--r--   0 solst      (501) staff       (20)    10883 2024-03-17 17:02:58.000000 sigr-0.0.9/sigr/enum.py
+-rw-r--r--   0 solst      (501) staff       (20)     4031 2024-03-17 17:02:58.000000 sigr-0.0.9/sigr/grds.py
+-rw-r--r--   0 solst      (501) staff       (20)    15096 2024-03-17 17:02:58.000000 sigr-0.0.9/sigr/sigs.py
+-rw-r--r--   0 solst      (501) staff       (20)    14949 2024-03-17 17:02:58.000000 sigr-0.0.9/sigr/type.py
+-rw-r--r--   0 solst      (501) staff       (20)    21104 2024-03-17 17:02:58.000000 sigr-0.0.9/sigr/util.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-17 17:03:00.613094 sigr-0.0.9/sigr.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     1989 2024-03-17 17:03:00.000000 sigr-0.0.9/sigr.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      411 2024-03-17 17:03:00.000000 sigr-0.0.9/sigr.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-17 17:03:00.000000 sigr-0.0.9/sigr.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2024-03-17 17:03:00.000000 sigr-0.0.9/sigr.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-02-24 20:27:32.000000 sigr-0.0.9/sigr.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)        7 2024-03-17 17:03:00.000000 sigr-0.0.9/sigr.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2024-03-17 17:03:00.000000 sigr-0.0.9/sigr.egg-info/top_level.txt
```

### Comparing `sigr-0.0.8/LICENSE` & `sigr-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sigr-0.0.8/PKG-INFO` & `sigr-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigr
-Version: 0.0.8
+Version: 0.0.9
 Summary: sigr
 Home-page: https://github.com/dsm-72/sigr
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: sigr
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sigr-0.0.8/README.md` & `sigr-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sigr-0.0.8/settings.ini` & `sigr-0.0.9/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = sigr
 lib_name = sigr
-version = 0.0.8
+version = 0.0.9
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = sigr
 nbs_path = nbs
 recursive = True
```

### Comparing `sigr-0.0.8/setup.py` & `sigr-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `sigr-0.0.8/sigr/__init__.py` & `sigr-0.0.9/sigr/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00__init__.ipynb.
 
 # %% auto 0
 __all__ = ['loadmod']
 
 # %% ../nbs/00__init__.ipynb 3
 from itertools import chain
```

### Comparing `sigr-0.0.8/sigr/_modidx.py` & `sigr-0.0.9/sigr/_modidx.py`

 * *Files identical despite different names*

### Comparing `sigr-0.0.8/sigr/attr.py` & `sigr-0.0.9/sigr/attr.py`

 * *Files identical despite different names*

### Comparing `sigr-0.0.8/sigr/bcls.py` & `sigr-0.0.9/sigr/bcls.py`

 * *Files identical despite different names*

### Comparing `sigr-0.0.8/sigr/bnds.py` & `sigr-0.0.9/sigr/bnds.py`

 * *Files identical despite different names*

### Comparing `sigr-0.0.8/sigr/cons.py` & `sigr-0.0.9/sigr/cons.py`

 * *Files identical despite different names*

### Comparing `sigr-0.0.8/sigr/deco.py` & `sigr-0.0.9/sigr/deco.py`

 * *Files identical despite different names*

### Comparing `sigr-0.0.8/sigr/enum.py` & `sigr-0.0.9/sigr/enum.py`

 * *Files identical despite different names*

### Comparing `sigr-0.0.8/sigr/grds.py` & `sigr-0.0.9/sigr/grds.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,14 +100,17 @@
 def isemptyparam(x) -> TypeGuard[Parameter]:
     '''Check if `x` is a `Parameter` and that it's default value is `Parameter._empty`'''
     return isparam(x) and isempty(x.default)
 
 def iscallattr(obj, attr: str) -> TypeGuard[Callable]: 
     return callable(getattr(obj, attr, None))
 
-def isoptional(x) -> TypeGuard[T | None]:
+def isoptional(x, __ducktype: bool = True) -> TypeGuard[T | None]:
     "Check if `x` is an optional type"
-    isname = getattr(x, '__name__', None) == 'Optional'
+    isname = getattr(x,'__name__', None) == 'Optional'
     isgenr = isinstance(x, _UnionGenericAlias)
     args = get_args(x)
     isnone = False if not len(args) else args[-1] == NoneType
-    return isname and isgenr and isnone
+    optspec = str(getattr(x, '__species__', None)) == 'opt'
+    hasnone = NoneType in getattr(x, '__usetypes__', lambda : ())()
+    return (isname and isgenr and isnone) or ((optspec or hasnone) and __ducktype)
+
```

### Comparing `sigr-0.0.8/sigr/sigs.py` & `sigr-0.0.9/sigr/sigs.py`

 * *Files identical despite different names*

### Comparing `sigr-0.0.8/sigr/type.py` & `sigr-0.0.9/sigr/type.py`

 * *Files identical despite different names*

### Comparing `sigr-0.0.8/sigr/util.py` & `sigr-0.0.9/sigr/util.py`

 * *Files identical despite different names*

### Comparing `sigr-0.0.8/sigr.egg-info/PKG-INFO` & `sigr-0.0.9/sigr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigr
-Version: 0.0.8
+Version: 0.0.9
 Summary: sigr
 Home-page: https://github.com/dsm-72/sigr
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: sigr
 Classifier: Development Status :: 4 - Beta
```

