# Comparing `tmp/gixpy-1.5.tar.gz` & `tmp/gixpy-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gixpy-1.5.tar", last modified: Fri Apr 12 02:15:11 2024, max compression
+gzip compressed data, was "gixpy-1.6.tar", last modified: Sun Apr 14 02:22:37 2024, max compression
```

## Comparing `gixpy-1.5.tar` & `gixpy-1.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 02:15:11.091960 gixpy-1.5/
--rw-rw-rw-   0        0        0      433 2024-04-12 02:15:11.087647 gixpy-1.5/PKG-INFO
--rw-rw-rw-   0        0        0    19662 2024-04-12 02:07:17.000000 gixpy-1.5/gixpy.c
-drwxrwxrwx   0        0        0        0 2024-04-12 02:15:11.078839 gixpy-1.5/gixpy.egg-info/
--rw-rw-rw-   0        0        0      433 2024-04-12 02:15:10.000000 gixpy-1.5/gixpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      147 2024-04-12 02:15:10.000000 gixpy-1.5/gixpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 02:15:10.000000 gixpy-1.5/gixpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-12 02:15:10.000000 gixpy-1.5/gixpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      644 2024-04-12 02:14:46.000000 gixpy-1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-12 02:15:11.092470 gixpy-1.5/setup.cfg
--rw-rw-rw-   0        0        0      793 2024-04-12 02:14:00.000000 gixpy-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 02:22:37.497596 gixpy-1.6/
+-rw-rw-rw-   0        0        0      433 2024-04-14 02:22:37.494745 gixpy-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    19713 2024-04-14 02:21:13.000000 gixpy-1.6/gixpy.c
+drwxrwxrwx   0        0        0        0 2024-04-14 02:22:37.483610 gixpy-1.6/gixpy.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-04-14 02:22:37.000000 gixpy-1.6/gixpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      147 2024-04-14 02:22:37.000000 gixpy-1.6/gixpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 02:22:37.000000 gixpy-1.6/gixpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-14 02:22:37.000000 gixpy-1.6/gixpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      644 2024-04-14 02:21:14.000000 gixpy-1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-14 02:22:37.497596 gixpy-1.6/setup.cfg
+-rw-rw-rw-   0        0        0      793 2024-04-14 02:21:15.000000 gixpy-1.6/setup.py
```

### Comparing `gixpy-1.5/gixpy.c` & `gixpy-1.6/gixpy.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION
 #define PY_SSIZE_T_CLEAN
 #include <Python.h>
 #include <numpy/arrayobject.h>
 #include <math.h>
 #include <float.h>
 
 const float DEG2RAD = 0.0174532925199432957692369076848861271344287188854;
@@ -265,15 +266,15 @@
         PyObject* return_list = PyList_New(num_images);
         for (Py_ssize_t ii = 0; ii < num_images; ++ii) {
             PyList_SET_ITEM(return_list, ii, transformed_array_obj_ptr[ii]);
         }
         return_array = PyList_AsTuple(return_list);
     }
     
-    PyObject* beam_center_tuple = PyTuple_Pack(2, PyFloat_FromDouble(beam_center_t.y), PyFloat_FromDouble(beam_center_t.y));
+    PyObject* beam_center_tuple = PyTuple_Pack(2, PyFloat_FromDouble(beam_center_t.y), PyFloat_FromDouble(beam_center_t.x));
 
     free(r_arr);
     free(pixel_info);
     free(transformed_array_obj_ptr);
     free(transformed_data_ptr);
     free(data_array_obj_ptr);
     free(data_array_ptr);
@@ -426,15 +427,15 @@
  * Initialize gixpy. May be called multiple times, so avoid
  * using static state.
  */
 int exec_gixpy(PyObject *module) {
     PyModule_AddFunctions(module, gixpy_functions);
 
     PyModule_AddStringConstant(module, "__author__", "Teddy Tortorici");
-    PyModule_AddStringConstant(module, "__version__", "1.5");
+    PyModule_AddStringConstant(module, "__version__", "1.6");
     PyModule_AddIntConstant(module, "year", 2024);
 
     return 0; /* success */
 }
 
 /*
  * Documentation for gixpy.
```

### Comparing `gixpy-1.5/pyproject.toml` & `gixpy-1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel", "numpy"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gixpy"
-version = "1.5"
+version = "1.6"
 authors = [
   { name="Teddy Tortorici", email="edward.tortorici@colorado.edu" },
 ]
 description = "Transform GIWAXS images"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 classifiers = [
```

### Comparing `gixpy-1.5/setup.py` & `gixpy-1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         ],
     library_dirs=["\\root\\project"],
     language="c",
 )
 
 setup(
     name='gixpy',
-    version="1.5",
+    version="1.6",
     description="Python package to quickly transform GIWAXS images using C",
     long_description="Visit github.com/etortorici/gixpy for details",
     author_email='edward.tortorici@colorado.edu',
     license='GPL',
     ext_modules=[gp_module],
     install_requires=["numpy"],
 )
```

