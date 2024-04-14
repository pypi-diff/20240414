# Comparing `tmp/geonum-1.5.0.dev11.tar.gz` & `tmp/geonum-1.5.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geonum-1.5.0.dev11.tar", last modified: Sun Apr 14 12:22:07 2024, max compression
+gzip compressed data, was "geonum-1.5.0.dev9.tar", last modified: Sat May 13 11:22:18 2023, max compression
```

## Comparing `geonum-1.5.0.dev11.tar` & `geonum-1.5.0.dev9.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:22:07.465671 geonum-1.5.0.dev11/
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-14 12:22:07.465671 geonum-1.5.0.dev11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-14 12:22:04.000000 geonum-1.5.0.dev11/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:22:07.461670 geonum-1.5.0.dev11/geonum/
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/geonum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/geonum/_init_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17180 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/geonum/atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/geonum/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    26403 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/geonum/elevationprofile.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/geonum/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23189 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/geonum/geopoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    27825 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/geonum/geosetup.py
--rw-r--r--   0 runner    (1001) docker     (127)    11325 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/geonum/geovector3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     6928 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/geonum/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/geonum/lineongrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    36515 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/geonum/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     6743 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/geonum/plot_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18351 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/geonum/topoaccessbase.py
--rw-r--r--   0 runner    (1001) docker     (127)    13699 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/geonum/topodata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/geonum/topodataaccess.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/geonum/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:22:07.465671 geonum-1.5.0.dev11/geonum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-14 12:22:07.000000 geonum-1.5.0.dev11/geonum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-14 12:22:07.000000 geonum-1.5.0.dev11/geonum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 12:22:07.000000 geonum-1.5.0.dev11/geonum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-14 12:22:07.000000 geonum-1.5.0.dev11/geonum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-14 12:22:07.000000 geonum-1.5.0.dev11/geonum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 12:22:07.465671 geonum-1.5.0.dev11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:22:07.465671 geonum-1.5.0.dev11/test/
--rw-r--r--   0 runner    (1001) docker     (127)    10776 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/test/test_atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/test/test_base_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8819 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/test/test_elevationprofile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8476 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/test/test_geopoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    12595 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/test/test_geosetup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/test/test_geovector3d.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/test/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/test/test_lineongrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/test/test_plot_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/test/test_srtmpy_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/test/test_topoaccessbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/test/test_topodata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/test/test_topodataaccess.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-14 12:21:52.000000 geonum-1.5.0.dev11/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:22:18.418721 geonum-1.5.0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-13 11:22:18.414720 geonum-1.5.0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:22:18.414720 geonum-1.5.0.dev9/geonum/
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/geonum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/geonum/_init_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17180 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/geonum/atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/geonum/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26403 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/geonum/elevationprofile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/geonum/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23189 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/geonum/geopoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27825 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/geonum/geosetup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/geonum/geovector3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6928 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/geonum/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/geonum/lineongrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36515 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/geonum/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/geonum/plot_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18351 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/geonum/topoaccessbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13699 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/geonum/topodata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/geonum/topodataaccess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/geonum/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:22:18.414720 geonum-1.5.0.dev9/geonum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-05-13 11:22:18.000000 geonum-1.5.0.dev9/geonum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-13 11:22:18.000000 geonum-1.5.0.dev9/geonum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 11:22:18.000000 geonum-1.5.0.dev9/geonum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-13 11:22:18.000000 geonum-1.5.0.dev9/geonum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 11:22:18.418721 geonum-1.5.0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 11:22:18.414720 geonum-1.5.0.dev9/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10776 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/test/test_atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/test/test_base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8819 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/test/test_elevationprofile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8476 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/test/test_geopoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12595 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/test/test_geosetup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/test/test_geovector3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/test/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/test/test_lineongrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/test/test_plot_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/test/test_srtmpy_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/test/test_topoaccessbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/test/test_topodata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/test/test_topodataaccess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-13 11:22:07.000000 geonum-1.5.0.dev9/test/test_utils.py
```

### Comparing `geonum-1.5.0.dev11/LICENSE` & `geonum-1.5.0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/PKG-INFO` & `geonum-1.5.0.dev9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 Metadata-Version: 2.1
 Name: geonum
-Version: 1.5.0.dev11
+Version: 1.5.0.dev9
 Summary: Toolbox for 3D geonumerical calculations and atmospheric composition
-Author-email: Jonas Gliss <jonasgliss@gmail.com>
-License: GPLv3+
-Project-URL: Homepage, https://github.com/jgliss/geonum
-Project-URL: Documentation, https://geonum.readthedocs.io/en/latest/
+Home-page: https://github.com/jgliss/geonum
+Author: Jonas Gliss
+Author-email: jonasgliss@gmail.com
+License: GPLv3
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: scipy
-Requires-Dist: matplotlib
-Requires-Dist: LatLon23
-Requires-Dist: SRTM.py
-Requires-Dist: cartopy
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: netcdf4; extra == "test"
 
 |CI| |docs| |cov| |code-quality|
 
 geonum: a python library for geo-numerical calculations
 =========================================================
 
 All you need to know: https://geonum.readthedocs.io/en/latest/
@@ -38,7 +30,8 @@
 
 .. |cov| image:: https://codecov.io/gh/jgliss/geonum/branch/main-dev/graph/badge.svg?token=802DAZA1W9
     :target: https://codecov.io/gh/jgliss/geonum
 
 .. |code-quality| image:: https://www.codefactor.io/repository/github/jgliss/geonum/badge
    :target: https://www.codefactor.io/repository/github/jgliss/geonum
    :alt: Code quality
+
```

### Comparing `geonum-1.5.0.dev11/README.rst` & `geonum-1.5.0.dev9/README.rst`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/geonum/__init__.py` & `geonum-1.5.0.dev9/geonum/__init__.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/geonum/atmosphere.py` & `geonum-1.5.0.dev9/geonum/atmosphere.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/geonum/conftest.py` & `geonum-1.5.0.dev9/geonum/conftest.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/geonum/elevationprofile.py` & `geonum-1.5.0.dev9/geonum/elevationprofile.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/geonum/exceptions.py` & `geonum-1.5.0.dev9/geonum/exceptions.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/geonum/geopoint.py` & `geonum-1.5.0.dev9/geonum/geopoint.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/geonum/geosetup.py` & `geonum-1.5.0.dev9/geonum/geosetup.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/geonum/geovector3d.py` & `geonum-1.5.0.dev9/geonum/geovector3d.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/geonum/helpers.py` & `geonum-1.5.0.dev9/geonum/helpers.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/geonum/lineongrid.py` & `geonum-1.5.0.dev9/geonum/lineongrid.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/geonum/mapping.py` & `geonum-1.5.0.dev9/geonum/mapping.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/geonum/plot_helpers.py` & `geonum-1.5.0.dev9/geonum/plot_helpers.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/geonum/topoaccessbase.py` & `geonum-1.5.0.dev9/geonum/topoaccessbase.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/geonum/topodata.py` & `geonum-1.5.0.dev9/geonum/topodata.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/geonum/topodataaccess.py` & `geonum-1.5.0.dev9/geonum/topodataaccess.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/geonum.egg-info/PKG-INFO` & `geonum-1.5.0.dev9/geonum.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 Metadata-Version: 2.1
 Name: geonum
-Version: 1.5.0.dev11
+Version: 1.5.0.dev9
 Summary: Toolbox for 3D geonumerical calculations and atmospheric composition
-Author-email: Jonas Gliss <jonasgliss@gmail.com>
-License: GPLv3+
-Project-URL: Homepage, https://github.com/jgliss/geonum
-Project-URL: Documentation, https://geonum.readthedocs.io/en/latest/
+Home-page: https://github.com/jgliss/geonum
+Author: Jonas Gliss
+Author-email: jonasgliss@gmail.com
+License: GPLv3
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: scipy
-Requires-Dist: matplotlib
-Requires-Dist: LatLon23
-Requires-Dist: SRTM.py
-Requires-Dist: cartopy
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: netcdf4; extra == "test"
 
 |CI| |docs| |cov| |code-quality|
 
 geonum: a python library for geo-numerical calculations
 =========================================================
 
 All you need to know: https://geonum.readthedocs.io/en/latest/
@@ -38,7 +30,8 @@
 
 .. |cov| image:: https://codecov.io/gh/jgliss/geonum/branch/main-dev/graph/badge.svg?token=802DAZA1W9
     :target: https://codecov.io/gh/jgliss/geonum
 
 .. |code-quality| image:: https://www.codefactor.io/repository/github/jgliss/geonum/badge
    :target: https://www.codefactor.io/repository/github/jgliss/geonum
    :alt: Code quality
+
```

### Comparing `geonum-1.5.0.dev11/geonum.egg-info/SOURCES.txt` & `geonum-1.5.0.dev9/geonum.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
+MANIFEST.in
 README.rst
-VERSION
-pyproject.toml
 setup.py
 geonum/__init__.py
 geonum/_init_helpers.py
 geonum/atmosphere.py
 geonum/conftest.py
 geonum/elevationprofile.py
 geonum/exceptions.py
@@ -19,16 +18,16 @@
 geonum/topoaccessbase.py
 geonum/topodata.py
 geonum/topodataaccess.py
 geonum/utils.py
 geonum.egg-info/PKG-INFO
 geonum.egg-info/SOURCES.txt
 geonum.egg-info/dependency_links.txt
-geonum.egg-info/requires.txt
 geonum.egg-info/top_level.txt
+test/__init__.py
 test/test_atmosphere.py
 test/test_base_classes.py
 test/test_elevationprofile.py
 test/test_geopoint.py
 test/test_geosetup.py
 test/test_geovector3d.py
 test/test_helpers.py
```

### Comparing `geonum-1.5.0.dev11/test/test_atmosphere.py` & `geonum-1.5.0.dev9/test/test_atmosphere.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/test/test_base_classes.py` & `geonum-1.5.0.dev9/test/test_base_classes.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/test/test_elevationprofile.py` & `geonum-1.5.0.dev9/test/test_elevationprofile.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/test/test_geopoint.py` & `geonum-1.5.0.dev9/test/test_geopoint.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/test/test_geosetup.py` & `geonum-1.5.0.dev9/test/test_geosetup.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/test/test_geovector3d.py` & `geonum-1.5.0.dev9/test/test_geovector3d.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/test/test_helpers.py` & `geonum-1.5.0.dev9/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/test/test_lineongrid.py` & `geonum-1.5.0.dev9/test/test_lineongrid.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/test/test_plot_helpers.py` & `geonum-1.5.0.dev9/test/test_plot_helpers.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/test/test_srtmpy_lib.py` & `geonum-1.5.0.dev9/test/test_srtmpy_lib.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/test/test_topoaccessbase.py` & `geonum-1.5.0.dev9/test/test_topoaccessbase.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/test/test_topodata.py` & `geonum-1.5.0.dev9/test/test_topodata.py`

 * *Files identical despite different names*

### Comparing `geonum-1.5.0.dev11/test/test_topodataaccess.py` & `geonum-1.5.0.dev9/test/test_topodataaccess.py`

 * *Files identical despite different names*

