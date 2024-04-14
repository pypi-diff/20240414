# Comparing `tmp/movoid_function-1.4.1.tar.gz` & `tmp/movoid_function-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movoid_function-1.4.1.tar", last modified: Tue Feb 20 17:25:19 2024, max compression
+gzip compressed data, was "movoid_function-1.5.0.tar", last modified: Sun Apr 14 08:04:10 2024, max compression
```

## Comparing `movoid_function-1.4.1.tar` & `movoid_function-1.5.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-02-20 17:25:19.990540 movoid_function-1.4.1/
--rw-rw-rw-   0        0        0      213 2024-02-20 17:25:19.988541 movoid_function-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_function-1.4.1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-20 17:25:19.976549 movoid_function-1.4.1/movoid_function/
--rw-rw-rw-   0        0        0      530 2024-02-20 11:35:42.000000 movoid_function-1.4.1/movoid_function/__init__.py
--rw-rw-rw-   0        0        0     9812 2024-02-20 05:59:20.000000 movoid_function-1.4.1/movoid_function/check.py
--rw-rw-rw-   0        0        0    16565 2024-02-20 11:49:02.000000 movoid_function-1.4.1/movoid_function/decorator.py
--rw-rw-rw-   0        0        0    12734 2024-02-20 05:59:20.000000 movoid_function-1.4.1/movoid_function/type.py
-drwxrwxrwx   0        0        0        0 2024-02-20 17:25:19.987541 movoid_function-1.4.1/movoid_function.egg-info/
--rw-rw-rw-   0        0        0      213 2024-02-20 17:25:19.000000 movoid_function-1.4.1/movoid_function.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-02-20 17:25:19.000000 movoid_function-1.4.1/movoid_function.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-20 17:25:19.000000 movoid_function-1.4.1/movoid_function.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-02-20 17:25:19.000000 movoid_function-1.4.1/movoid_function.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-20 17:25:19.990540 movoid_function-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0      462 2024-02-20 17:24:08.000000 movoid_function-1.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 08:04:10.289501 movoid_function-1.5.0/
+-rw-rw-rw-   0        0        0      213 2024-04-14 08:04:10.288515 movoid_function-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2024-01-07 14:19:32.000000 movoid_function-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-14 08:04:10.278538 movoid_function-1.5.0/movoid_function/
+-rw-rw-rw-   0        0        0      562 2024-04-13 09:15:08.000000 movoid_function-1.5.0/movoid_function/__init__.py
+-rw-rw-rw-   0        0        0     9812 2024-02-20 05:59:20.000000 movoid_function-1.5.0/movoid_function/check.py
+-rw-rw-rw-   0        0        0    16565 2024-02-20 11:49:02.000000 movoid_function-1.5.0/movoid_function/decorator.py
+-rw-rw-rw-   0        0        0     1557 2024-04-14 08:03:48.000000 movoid_function-1.5.0/movoid_function/function.py
+-rw-rw-rw-   0        0        0    12734 2024-02-20 05:59:20.000000 movoid_function-1.5.0/movoid_function/type.py
+drwxrwxrwx   0        0        0        0 2024-04-14 08:04:10.287510 movoid_function-1.5.0/movoid_function.egg-info/
+-rw-rw-rw-   0        0        0      213 2024-04-14 08:04:10.000000 movoid_function-1.5.0/movoid_function.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2024-04-14 08:04:10.000000 movoid_function-1.5.0/movoid_function.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 08:04:10.000000 movoid_function-1.5.0/movoid_function.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-14 08:04:10.000000 movoid_function-1.5.0/movoid_function.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 08:04:10.289501 movoid_function-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      462 2024-04-14 07:24:11.000000 movoid_function-1.5.0/setup.py
```

### Comparing `movoid_function-1.4.1/movoid_function/__init__.py` & `movoid_function-1.5.0/movoid_function/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,7 +7,8 @@
 # Description   : 
 """
 from .decorator import recover_signature_from_function as wraps
 from .decorator import recover_signature_from_function_func as wraps_func
 from .decorator import recover_signature_from_function_only_kwargs as wraps_kw
 from .decorator import reset_function_default_value, analyse_args_value_from_function
 from .type import check_parameters_type
+from .function import Function
```

### Comparing `movoid_function-1.4.1/movoid_function/check.py` & `movoid_function-1.5.0/movoid_function/check.py`

 * *Files identical despite different names*

### Comparing `movoid_function-1.4.1/movoid_function/decorator.py` & `movoid_function-1.5.0/movoid_function/decorator.py`

 * *Files identical despite different names*

### Comparing `movoid_function-1.4.1/movoid_function/type.py` & `movoid_function-1.5.0/movoid_function/type.py`

 * *Files identical despite different names*

