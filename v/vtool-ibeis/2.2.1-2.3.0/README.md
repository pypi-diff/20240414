# Comparing `tmp/vtool_ibeis-2.2.1.tar.gz` & `tmp/vtool_ibeis-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtool_ibeis-2.2.1.tar", last modified: Sun Jan 29 18:27:07 2023, max compression
+gzip compressed data, was "vtool_ibeis-2.3.0.tar", last modified: Sun Apr 14 05:54:18 2024, max compression
```

## Comparing `vtool_ibeis-2.2.1.tar` & `vtool_ibeis-2.3.0.tar`

### file list

```diff
@@ -1,51 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 18:27:07.234852 vtool_ibeis-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-01-29 18:27:07.234852 vtool_ibeis-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-29 18:27:07.234852 vtool_ibeis-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9362 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 18:27:07.234852 vtool_ibeis-2.2.1/vtool_ibeis/
--rwxr-xr-x   0 runner    (1001) docker     (123)    37732 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/_pyflann_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/_rhomb_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/blend.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15699 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/chip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30788 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/clustering2.py
--rw-r--r--   0 runner    (1001) docker     (123)    40883 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/confusion.py
--rw-r--r--   0 runner    (1001) docker     (123)    13263 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/coverage_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19203 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/coverage_kpts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    40928 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/demodata.py
--rw-r--r--   0 runner    (1001) docker     (123)    25083 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/distance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15439 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/ellipse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13256 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/exif.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13434 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/fontdemo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18885 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/geometry.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    40094 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/histogram.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   106295 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/image.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6918 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/image_filters.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      449 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/image_shared.py
--rw-r--r--   0 runner    (1001) docker     (123)    13155 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/inspect_matches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81177 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/keypoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21111 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/linalg.py
--rw-r--r--   0 runner    (1001) docker     (123)    73427 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/matching.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29606 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/nearest_neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11689 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    88733 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/other.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    54760 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/quality_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    68619 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/score_normalization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10210 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/segmentation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47898 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/spatial_verification.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3728 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/sver_c_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6227 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/symbolic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      739 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/trig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24177 2023-01-29 18:26:59.000000 vtool_ibeis-2.2.1/vtool_ibeis/util_math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 18:27:07.234852 vtool_ibeis-2.2.1/vtool_ibeis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-01-29 18:27:07.000000 vtool_ibeis-2.2.1/vtool_ibeis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-01-29 18:27:07.000000 vtool_ibeis-2.2.1/vtool_ibeis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-29 18:27:07.000000 vtool_ibeis-2.2.1/vtool_ibeis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13571 2023-01-29 18:27:07.000000 vtool_ibeis-2.2.1/vtool_ibeis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-29 18:27:07.000000 vtool_ibeis-2.2.1/vtool_ibeis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:54:18.396973 vtool_ibeis-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    51706 2024-04-14 05:54:18.396973 vtool_ibeis-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 05:54:18.396973 vtool_ibeis-2.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9836 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:54:18.312972 vtool_ibeis-2.3.0/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2591 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/tests/test_akmeans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/tests/test_coverage_max_reduce.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5212 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/tests/test_draw_keypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/tests/test_import.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12184 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/tests/test_pyflann.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7633 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/tests/test_spatial_verification.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1265 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/tests/test_vtool.py
+-rw-r--r--   0 runner    (1001) docker     (127)   356339 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/tests/testdata_nondeterm_sver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:54:18.320972 vtool_ibeis-2.3.0/vtool_ibeis/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37732 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/_pyflann_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11919 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/_rhomb_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13566 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/blend.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15699 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/chip.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30788 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/clustering2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40883 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/confusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13259 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/coverage_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19250 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/coverage_kpts.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    40928 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/demodata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25083 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/distance.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15439 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/ellipse.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13256 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/exif.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13343 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/fontdemo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18710 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/geometry.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    40088 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/histogram.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   106216 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/image.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7179 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/image_filters.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      449 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/image_shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13155 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/inspect_matches.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    81177 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/keypoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21111 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/linalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73612 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/matching.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29722 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/nearest_neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11689 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88733 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/other.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    54174 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/quality_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68619 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/score_normalization.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10206 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/segmentation.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    47775 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/spatial_verification.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3728 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/sver_c_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/symbolic.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      739 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/trig.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24177 2024-04-14 05:53:28.000000 vtool_ibeis-2.3.0/vtool_ibeis/util_math.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 05:54:18.324972 vtool_ibeis-2.3.0/vtool_ibeis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    51706 2024-04-14 05:54:18.000000 vtool_ibeis-2.3.0/vtool_ibeis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-14 05:54:18.000000 vtool_ibeis-2.3.0/vtool_ibeis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 05:54:18.000000 vtool_ibeis-2.3.0/vtool_ibeis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18776 2024-04-14 05:54:18.000000 vtool_ibeis-2.3.0/vtool_ibeis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-14 05:54:18.000000 vtool_ibeis-2.3.0/vtool_ibeis.egg-info/top_level.txt
```

### Comparing `vtool_ibeis-2.2.1/LICENSE` & `vtool_ibeis-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vtool_ibeis-2.2.1/README.rst` & `vtool_ibeis-2.3.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 vtool_ibeis
 ===========
 
-|Pypi| |Downloads| |Codecov| |Travis| |Appveyor| 
+|Pypi| |Downloads| |Codecov|
 
 Vision Tools - tools for computer vision. Part of the WildMe / IBEIS Project.
 
 
 Repos relevant to the ibeis project:
 
 * https://github.com/Erotemic/plottool_ibeis
@@ -23,20 +23,14 @@
 * https://github.com/Erotemic/pyhesaff
 
 * https://github.com/Erotemic/utool
 
 * https://github.com/Erotemic/ibeis
 
 
-.. |CircleCI| image:: https://circleci.com/gh/Erotemic/vtool_ibeis.svg?style=svg
-    :target: https://circleci.com/gh/Erotemic/vtool_ibeis
-.. |Travis| image:: https://img.shields.io/travis/Erotemic/vtool_ibeis/master.svg?label=Travis%20CI
-   :target: https://travis-ci.org/Erotemic/vtool_ibeis?branch=master
-.. |Appveyor| image:: https://ci.appveyor.com/api/projects/status/github/Erotemic/vtool_ibeis?branch=master&svg=True
-   :target: https://ci.appveyor.com/project/Erotemic/vtool_ibeis/branch/master
 .. |Codecov| image:: https://codecov.io/github/Erotemic/vtool_ibeis/badge.svg?branch=master&service=github
    :target: https://codecov.io/github/Erotemic/vtool_ibeis?branch=master
 .. |Pypi| image:: https://img.shields.io/pypi/v/vtool_ibeis.svg
    :target: https://pypi.python.org/pypi/vtool_ibeis
 .. |Downloads| image:: https://img.shields.io/pypi/dm/vtool_ibeis.svg
    :target: https://pypistats.org/packages/vtool_ibeis
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/vtool_ibeis/badge/?version=latest
```

### Comparing `vtool_ibeis-2.2.1/pyproject.toml` & `vtool_ibeis-2.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -11,24 +11,30 @@
 repo_name = "vtool_ibeis"
 url = "https://github.com/Erotemic/vtool_ibeis"
 description = "vision tools for IBEIS"
 os = [ "linux" ]
 ci_pypy_versions = []
 author = ['Jon Crall', 'Jason Parham', 'Hendrik Weideman', 'Avi Weinstock', 'Zackary Rutfield', 'Chuck Stewart']
 author_email="erotemic@gmail.com"
-min_python = 3.7
+min_python = 3.8
+max_python = 3.11
 version = "{mod_dpath}/__init__.py::__version__"
 license = "Apache 2"
 dev_status = "beta"
 
 
 [tool.pytest.ini_options]
-addopts = "-p no:doctest --xdoctest --xdoctest-style=google --ignore-glob=setup.py"
-norecursedirs = ".git ignore build __pycache__ dev _skbuild"
-filterwarnings = [ "default", "ignore:.*No cfgstr given in Cacher constructor or call.*:Warning", "ignore:.*Define the __nice__ method for.*:Warning", "ignore:.*private pytest class or function.*:Warning",]
+addopts = "-p no:doctest --xdoctest --xdoctest-style=google --ignore-glob=setup.py --ignore-glob=docs"
+norecursedirs = ".git ignore build __pycache__ dev _skbuild docs"
+filterwarnings = [
+    "default",
+    "ignore:.*No cfgstr given in Cacher constructor or call.*:Warning",
+    "ignore:.*Define the __nice__ method for.*:Warning",
+    "ignore:.*private pytest class or function.*:Warning",
+]
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 exclude_lines = [ "pragma: no cover", ".*  # pragma: no cover", ".*  # nocover", "def __repr__", "raise AssertionError", "raise NotImplementedError", "if 0:", "if trace is not None", "verbose = .*", "^ *raise", "^ *pass *$", "if _debug:", "if __name__ == .__main__.:", ".*if six.PY2:",]
 omit = [ "vtool_ibeis/__main__.py", "*/setup.py",]
```

### Comparing `vtool_ibeis-2.2.1/setup.py` & `vtool_ibeis-2.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # Generated by ~/code/xcookie/xcookie/builders/setup.py
 # based on part ~/code/xcookie/xcookie/rc/setup.py.in
 import sys
-from os.path import exists
+import re
+from os.path import exists, dirname, join
 from setuptools import find_packages
 from setuptools import setup
 
 
 def parse_version(fpath):
     """
     Statically parse the version number from a python file
@@ -49,16 +50,14 @@
     """
     Parse the description in the README file
 
     CommandLine:
         pandoc --from=markdown --to=rst --output=README.rst README.md
         python -c "import setup; print(setup.parse_description())"
     """
-    from os.path import dirname, join, exists
-
     readme_fpath = join(dirname(__file__), "README.rst")
     # This breaks on pip install, so check that it exists.
     if exists(readme_fpath):
         with open(readme_fpath, "r") as f:
             text = f.read()
         return text
     return ""
@@ -73,18 +72,18 @@
         fname (str): path to requirements file
         versions (bool | str, default=False):
             If true include version specs.
             If strict, then pin to the minimum version.
 
     Returns:
         List[str]: list of requirements items
-    """
-    from os.path import exists, dirname, join
-    import re
 
+    CommandLine:
+        python -c "import setup, ubelt; print(ubelt.urepr(setup.parse_requirements()))"
+    """
     require_fpath = fname
 
     def parse_line(line, dpath=""):
         """
         Parse information from a line in a requirements text file
 
         line = 'git+https://a.com/somedep@sometag#egg=SomeDep'
@@ -194,62 +193,66 @@
 #             raise KeyError(versions)
 #     requirements = [r.replace(' ', '') for r in requirements]
 #     return requirements
 
 
 NAME = "vtool_ibeis"
 INIT_PATH = "vtool_ibeis/__init__.py"
-VERSION = parse_version("vtool_ibeis/__init__.py")
+VERSION = parse_version(INIT_PATH)
 
 if __name__ == "__main__":
     setupkw = {}
 
-    setupkw["install_requires"] = parse_requirements("requirements/runtime.txt")
+    setupkw["install_requires"] = parse_requirements(
+        "requirements/runtime.txt", versions="loose"
+    )
     setupkw["extras_require"] = {
-        "all": parse_requirements("requirements.txt"),
-        "tests": parse_requirements("requirements/tests.txt"),
-        "optional": parse_requirements("requirements/optional.txt"),
-        "headless": parse_requirements("requirements/headless.txt"),
-        "graphics": parse_requirements("requirements/graphics.txt"),
-        # Strict versions
+        "all": parse_requirements("requirements.txt", versions="loose"),
+        "headless": parse_requirements("requirements/headless.txt", versions="loose"),
+        "graphics": parse_requirements("requirements/graphics.txt", versions="loose"),
+        "build": parse_requirements("requirements/build.txt", versions="loose"),
+        "docs": parse_requirements("requirements/docs.txt", versions="loose"),
+        "optional": parse_requirements("requirements/optional.txt", versions="loose"),
+        "runtime": parse_requirements("requirements/runtime.txt", versions="loose"),
+        "tests": parse_requirements("requirements/tests.txt", versions="loose"),
+        "all-strict": parse_requirements("requirements.txt", versions="strict"),
         "headless-strict": parse_requirements(
             "requirements/headless.txt", versions="strict"
         ),
         "graphics-strict": parse_requirements(
             "requirements/graphics.txt", versions="strict"
         ),
-        "all-strict": parse_requirements("requirements.txt", versions="strict"),
+        "build-strict": parse_requirements("requirements/build.txt", versions="strict"),
+        "docs-strict": parse_requirements("requirements/docs.txt", versions="strict"),
+        "optional-strict": parse_requirements(
+            "requirements/optional.txt", versions="strict"
+        ),
         "runtime-strict": parse_requirements(
             "requirements/runtime.txt", versions="strict"
         ),
         "tests-strict": parse_requirements("requirements/tests.txt", versions="strict"),
-        "optional-strict": parse_requirements(
-            "requirements/optional.txt", versions="strict"
-        ),
     }
-
     setupkw["name"] = NAME
     setupkw["version"] = VERSION
     setupkw[
         "author"
     ] = "Jon Crall, Jason Parham, Hendrik Weideman, Avi Weinstock, Zackary Rutfield, Chuck Stewart"
     setupkw["author_email"] = "erotemic@gmail.com"
     setupkw["url"] = "https://github.com/Erotemic/vtool_ibeis"
     setupkw["description"] = "vision tools for IBEIS"
     setupkw["long_description"] = parse_description()
     setupkw["long_description_content_type"] = "text/x-rst"
     setupkw["license"] = "Apache 2"
     setupkw["packages"] = find_packages(".")
-    setupkw["python_requires"] = ">=3.7"
+    setupkw["python_requires"] = ">=3.8"
     setupkw["classifiers"] = [
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Utilities",
         "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ]
     setup(**setupkw)
```

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/__init__.py` & `vtool_ibeis-2.3.0/vtool_ibeis/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 VTool - Computer vision tools
 
 Autogenerate Command:
     mkinit vtool_ibeis -i
 """
 # flake8: noqa
-__version__ = '2.2.1'
+__version__ = '2.3.0'
 __author__ = 'Jon Crall, Avi Weinstock, Chuck Stewart, Hendrik Weideman, Jason Parham, Zackary Rutfield'
 __author_email__ = 'erotemic@gmail.com'
 __url__ = 'https://github.com/Erotemic/vtool_ibeis'
 
 
 
 __submodules__ = [
```

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/__main__.py` & `vtool_ibeis-2.3.0/vtool_ibeis/__main__.py`

 * *Files identical despite different names*

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/_pyflann_backend.py` & `vtool_ibeis-2.3.0/vtool_ibeis/_pyflann_backend.py`

 * *Files identical despite different names*

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/_rhomb_dist.py` & `vtool_ibeis-2.3.0/vtool_ibeis/_rhomb_dist.py`

 * *Files identical despite different names*

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/blend.py` & `vtool_ibeis-2.3.0/vtool_ibeis/blend.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 import utool as ut
 import ubelt as ub
 
 
 def testdata_blend(scale=128):
     import vtool_ibeis as vt
-    img_fpath = ut.grab_test_imgpath('lena.png')
+    img_fpath = ut.grab_test_imgpath('astro')
     img1 = vt.imread(img_fpath)
     rng = np.random.RandomState(0)
     img2 = vt.perlin_noise(img1.shape[0:2], scale=scale, rng=rng)[None, :].T
     img1 = vt.rectify_to_float01(img1)
     img2 = vt.rectify_to_float01(img2)
     return img1, img2
```

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/chip.py` & `vtool_ibeis-2.3.0/vtool_ibeis/chip.py`

 * *Files identical despite different names*

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/clustering2.py` & `vtool_ibeis-2.3.0/vtool_ibeis/clustering2.py`

 * *Files identical despite different names*

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/confusion.py` & `vtool_ibeis-2.3.0/vtool_ibeis/confusion.py`

 * *Files identical despite different names*

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/coverage_grid.py` & `vtool_ibeis-2.3.0/vtool_ibeis/coverage_grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         python -m vtool_ibeis.coverage_grid --test-make_grid_coverage_mask --show
 
     Example:
         >>> # DISABLE_DOCTEST
         >>> from vtool_ibeis.coverage_grid import *  # NOQA
         >>> import vtool_ibeis as vt
         >>> # build test data
-        >>> kpts, chipsize, weights = coverage_kpts.testdata_coverage('easy1.png')
+        >>> kpts, chipsize, weights = coverage_kpts.testdata_coverage('tsukuba_l')
         >>> pxl_per_bin = 4
         >>> grid_steps = 2
         >>> # execute function
         >>> weightgrid = make_grid_coverage_mask(kpts, chipsize, weights, pxl_per_bin, grid_steps)
         >>> # verify result
         >>> result = str(weightgrid)
         >>> print(result)
@@ -319,15 +319,15 @@
         >>> from vtool_ibeis.coverage_grid import *  # NOQA
         >>> import plottool_ibeis as pt
         >>> gridsearch_coverage_grid_mask()
         >>> pt.show_if_requested()
     """
     import plottool_ibeis as pt
     cfgdict_list, cfglbl_list = get_coverage_grid_gridsearch_configs()
-    kpts, chipsize, weights = coverage_kpts.testdata_coverage('easy1.png')
+    kpts, chipsize, weights = coverage_kpts.testdata_coverage('astro')
     gridmask_list = [
         255 *  make_grid_coverage_mask(kpts, chipsize, weights, **cfgdict)
         for cfgdict in ub.ProgIter(cfgdict_list, desc='coverage grid')
     ]
     NORMHACK = False
     if NORMHACK:
         gridmask_list = [
```

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/coverage_kpts.py` & `vtool_ibeis-2.3.0/vtool_ibeis/coverage_kpts.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     Example:
         >>> # ENABLE_DOCTEST
         >>> # xdoctest: +REQUIRES(module:plottool_ibeis)
         >>> # xdoctest: +REQUIRES(module:pyhesaff)
         >>> from vtool_ibeis.coverage_kpts import *  # NOQA
         >>> import vtool_ibeis as vt
         >>> import pyhesaff
-        >>> img_fpath = ut.grab_test_imgpath('carl.jpg')
+        >>> img_fpath = ut.grab_test_imgpath('carl')
         >>> (kpts, vecs) = pyhesaff.detect_feats(img_fpath)
         >>> chip = vt.imread(img_fpath)
         >>> kpts = kpts[0:100]
         >>> chipsize = chip.shape[0:2][::-1]
         >>> heatmask = make_kpts_heatmask(kpts, chipsize)
         >>> img1 = heatmask
         >>> img2 = chip
@@ -125,15 +125,15 @@
         >>> # ENABLE_DOCTEST
         >>> # xdoctest: +REQUIRES(module:plottool_ibeis)
         >>> # xdoctest: +REQUIRES(module:pyhesaff)
         >>> from vtool_ibeis.coverage_kpts import *  # NOQA
         >>> import vtool_ibeis as vt
         >>> import plottool_ibeis as pt
         >>> import pyhesaff
-        >>> img_fpath = ut.grab_test_imgpath('carl.jpg')
+        >>> img_fpath = ut.grab_test_imgpath('carl')
         >>> (kpts, vecs) = pyhesaff.detect_feats(img_fpath)
         >>> kpts = kpts[::10]
         >>> chip = vt.imread(img_fpath)
         >>> chipsize = chip.shape[0:2][::-1]
         >>> # execute function
         >>> dstimg, patch = make_kpts_coverage_mask(kpts, chipsize, resize=True, return_patch=True, cov_size_penalty_on=False, cov_blur_on=False)
         >>> # show results
@@ -206,15 +206,15 @@
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> # xdoctest: +REQUIRES(module:pyhesaff)
         >>> from vtool_ibeis.coverage_kpts import *  # NOQA
         >>> import vtool_ibeis as vt
         >>> import pyhesaff
-        >>> img_fpath    = ut.grab_test_imgpath('carl.jpg')
+        >>> img_fpath    = ut.grab_test_imgpath('carl')
         >>> (kpts, vecs) = pyhesaff.detect_feats(img_fpath)
         >>> kpts = kpts[::15]
         >>> chip = vt.imread(img_fpath)
         >>> chipshape = chip.shape
         >>> weights = np.ones(len(kpts))
         >>> cov_scale_factor = 1.0
         >>> srcshape = (19, 19)
@@ -430,15 +430,16 @@
         >>> from vtool_ibeis.coverage_kpts import *  # NOQA
         >>> import plottool_ibeis as pt
         >>> gridsearch_kpts_coverage_mask()
         >>> pt.show_if_requested()
     """
     import plottool_ibeis as pt
     cfgdict_list, cfglbl_list = get_coverage_kpts_gridsearch_configs()
-    kpts, chipsize, weights = testdata_coverage('easy1.png')
+    # kpts, chipsize, weights = testdata_coverage('easy1.png')
+    kpts, chipsize, weights = testdata_coverage('astro')
     imgmask_list = [
         255 *  make_kpts_coverage_mask(kpts, chipsize, weights,
                                        return_patch=False, **cfgdict)
         for cfgdict in ub.ProgIter(cfgdict_list, label='coverage grid')
     ]
     #NORMHACK = True
     #if NORMHACK:
@@ -455,26 +456,26 @@
 
 def testdata_coverage(fname=None):
     """ testing function """
     import vtool_ibeis as vt
     # build test data
     kpts, vecs = vt.demodata.get_testdata_kpts(fname, with_vecs=True)
     # HACK IN DISTINCTIVENESS
-    if fname is not None:
-        from ibeis.algo.hots import distinctiveness_normalizer
-        cachedir = ub.ensure_app_cache_dir('ibeis', 'distinctiveness_model')
-        species = 'zebra_plains'
-        dstcnvs_normer = distinctiveness_normalizer.DistinctivnessNormalizer(species, cachedir=cachedir)
-        dstcnvs_normer.load(cachedir)
-        weights = dstcnvs_normer.get_distinctiveness(vecs)
-    else:
-        kpts = np.vstack((kpts, [0, 0, 1, 1, 1, 0]))
-        kpts = np.vstack((kpts, [0.01, 10, 1, 1, 1, 0]))
-        kpts = np.vstack((kpts, [0.94, 11.5, 1, 1, 1, 0]))
-        weights = np.ones(len(kpts))
+    # if fname is not None:
+    #     from ibeis.algo.hots import distinctiveness_normalizer
+    #     cachedir = ub.ensure_app_cache_dir('ibeis', 'distinctiveness_model')
+    #     species = 'zebra_plains'
+    #     dstcnvs_normer = distinctiveness_normalizer.DistinctivnessNormalizer(species, cachedir=cachedir)
+    #     dstcnvs_normer.load(cachedir)
+    #     weights = dstcnvs_normer.get_distinctiveness(vecs)
+    # else:
+    kpts = np.vstack((kpts, [0, 0, 1, 1, 1, 0]))
+    kpts = np.vstack((kpts, [0.01, 10, 1, 1, 1, 0]))
+    kpts = np.vstack((kpts, [0.94, 11.5, 1, 1, 1, 0]))
+    weights = np.ones(len(kpts))
     chipsize = tuple(vt.iceil(vt.get_kpts_image_extent(kpts)[2:4]).tolist())
     return kpts, chipsize, weights
 
 
 def show_coverage_map(chip, mask, patch, kpts, fnum=None, ell_alpha=.6,
                       show_mask_kpts=False):
     """ testing function """
```

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/demodata.py` & `vtool_ibeis-2.3.0/vtool_ibeis/demodata.py`

 * *Files 0% similar despite different names*

```diff
@@ -629,15 +629,15 @@
         kpts, vecs = feattool.extract_features(fpath)
     if with_vecs:
         return kpts, vecs
     else:
         return kpts
 
 
-def testdata_ratio_matches(fname1='easy1.png', fname2='easy2.png', **kwargs):
+def testdata_ratio_matches(fname1='tsukuba_r', fname2='tsukuba_l', **kwargs):
     r"""
     Runs simple ratio-test matching between two images.
     Technically this is not demodata data.
 
     Args:
         fname1 (str):
         fname2 (str):
@@ -655,16 +655,16 @@
         python -m vtool_ibeis.demodata --test-testdata_ratio_matches --show --ratio_thresh=.625 --no-rotation_invariance --fname1 easy1.png --fname2 easy3.png
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> # xdoctest: +REQUIRES(module:pyhesaff)
         >>> from vtool_ibeis.demodata import *  # NOQA
         >>> import vtool_ibeis as vt
-        >>> fname1 = ut.get_argval('--fname1', type_=str, default='easy1.png')
-        >>> fname2 = ut.get_argval('--fname2', type_=str, default='easy2.png')
+        >>> fname1 = ut.get_argval('--fname1', type_=str, default='tsukuba_l')
+        >>> fname2 = ut.get_argval('--fname2', type_=str, default='tsukuba_r')
         >>> default_dict = vt.get_extract_features_default_params()
         >>> default_dict['ratio_thresh'] = .625
         >>> kwargs = ut.argparse_dict(default_dict)
         >>> matches_testtup = testdata_ratio_matches(fname1, fname2, **kwargs)
         >>> (kpts1, kpts2, fm_RAT, fs_RAT, rchip1, rchip2) = matches_testtup
         >>> # xdoctest: +REQUIRES(--show)
         >>> import plottool_ibeis as pt
```

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/distance.py` & `vtool_ibeis-2.3.0/vtool_ibeis/distance.py`

 * *Files identical despite different names*

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/ellipse.py` & `vtool_ibeis-2.3.0/vtool_ibeis/ellipse.py`

 * *Files identical despite different names*

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/exif.py` & `vtool_ibeis-2.3.0/vtool_ibeis/exif.py`

 * *Files identical despite different names*

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/features.py` & `vtool_ibeis-2.3.0/vtool_ibeis/features.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> # xdoctest: +REQUIRES(module:pyhesaff)
         >>> from vtool_ibeis.features import *  # NOQA
         >>> import vtool_ibeis as vt
         >>> # build test data
-        >>> img_fpath = ut.grab_test_imgpath(ut.get_argval('--fname', default='lena.png'))
+        >>> img_fpath = ut.grab_test_imgpath(ut.get_argval('--fname', default='astro'))
         >>> imgBGR = vt.imread(img_fpath)
         >>> feat_type = ub.argval('--feat_type', default='hesaff+sift')
         >>> import pyhesaff
         >>> kwargs = ut.parse_dict_from_argv(pyhesaff.get_hesaff_default_params())
         >>> # execute function
         >>> #(kpts, vecs) = extract_features(img_fpath)
         >>> (kpts, vecs) = extract_features(imgBGR, feat_type, **kwargs)
@@ -105,16 +105,15 @@
 
 
 def detect_opencv_keypoints():
     import cv2
     import vtool_ibeis as vt
     import numpy as np  # NOQA
 
-    #img_fpath = ut.grab_test_imgpath(ub.argval('--fname', default='lena.png'))
-    img_fpath = ut.grab_test_imgpath(ub.argval('--fname', default='zebra.png'))
+    img_fpath = ut.grab_test_imgpath(ub.argval('--fname', default='astro'))
     imgBGR = vt.imread(img_fpath)
     imgGray = cv2.cvtColor(imgBGR, cv2.COLOR_BGR2GRAY)
 
     def from_cv2_kpts(cv2_kp):
         kp = (cv2_kp.pt[0], cv2_kp.pt[1], cv2_kp.size, 0, cv2_kp.size, cv2_kp.angle)
         return kp
 
@@ -247,15 +246,15 @@
             return vt.get_kpts_eccentricity(self.kparr)
 
         def compress(self, flags, inplace=False):
             subarr = self.kparr.compress(flags, axis=0)
             info = {key: list(ub.compress(val, flags)) for key, val in self.info.items()}
             return Keypoints(subarr, info)
 
-    img_fpath = ut.grab_test_imgpath(ub.argval('--fname', default='zebra.png'))
+    img_fpath = ut.grab_test_imgpath(ub.argval('--fname', default='astro'))
     imgBGR = vt.imread(img_fpath)
     imgGray = cv2.cvtColor(imgBGR, cv2.COLOR_BGR2GRAY)
     # http://docs.opencv.org/master/d3/d28/classcv_1_1MSER.html#gsc.tab=0
     # http://stackoverflow.com/questions/17647500/exact-meaning-of-the-parameters-given-to-initialize-mser-in-opencv-2-4-x
     factory = cv2.MSER_create
     img_area = np.product(np.array(vt.get_size(imgGray)))
     _max_area = (img_area // 10)
```

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/fontdemo.py` & `vtool_ibeis-2.3.0/vtool_ibeis/fontdemo.py`

 * *Files identical despite different names*

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/geometry.py` & `vtool_ibeis-2.3.0/vtool_ibeis/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,14 @@
     Args:
         bbox (tuple):  bounding box in the format (x, y, w, h)
         close (bool): (default = False)
 
     Returns:
         list: verts
 
-    CommandLine:
-        python -m vtool_ibeis.geometry --test-verts_from_bbox
-
     Example:
         >>> # ENABLE_DOCTEST
         >>> from vtool_ibeis.geometry import *  # NOQA
         >>> bbox = (10, 10, 50, 50)
         >>> close = False
         >>> verts = verts_from_bbox(bbox, close)
         >>> result = ('verts = %s' % (str(verts),))
@@ -62,22 +59,19 @@
     r"""
     Args:
         img_in (ndarray[uint8_t, ndim=2]):  image data
         color (tuple): in bgr
         thickness (int):
         out (None):
 
-    CommandLine:
-        python -m vtool_ibeis.geometry --test-draw_border --show
-
     Example:
         >>> # ENABLE_DOCTEST
         >>> from vtool_ibeis.geometry import *  # NOQA
         >>> import vtool_ibeis as vt
-        >>> img_in = vt.imread(ut.grab_test_imgpath('carl.jpg'))
+        >>> img_in = vt.imread(ut.grab_test_imgpath('carl'))
         >>> color = (0, 128, 255)
         >>> thickness = 20
         >>> out = None
         >>> # xdoctest: +REQUIRES(module:plottool_ibeis)
         >>> img = draw_border(img_in, color, thickness, out)
         >>> # xdoctest: +REQUIRES(--show)
         >>> import plottool_ibeis as pt
@@ -117,15 +111,15 @@
     Example:
         >>> # ENABLE_DOCTEST
         >>> from vtool_ibeis.geometry import *  # NOQA
         >>> # xdoctest: +REQUIRES(--show)
         >>> import plottool_ibeis as pt
         >>> import vtool_ibeis as vt
         >>> # build test data
-        >>> img_in = vt.imread(ut.grab_test_imgpath('carl.jpg'))
+        >>> img_in = vt.imread(ut.grab_test_imgpath('carl'))
         >>> verts = ((10, 10), (10, 100), (100, 100), (100, 10))
         >>> color = (0, 128, 255)
         >>> thickness = 2
         >>> # execute function
         >>> out = None
         >>> img = draw_verts(img_in, verts, color, thickness, out)
         >>> assert img_in is not img
@@ -139,15 +133,15 @@
     Example1:
         >>> # ENABLE_DOCTEST
         >>> from vtool_ibeis.geometry import *  # NOQA
         >>> # xdoctest: +REQUIRES(--show)
         >>> import plottool_ibeis as pt
         >>> import vtool_ibeis as vt
         >>> # build test data
-        >>> img_in = vt.imread(ut.grab_test_imgpath('carl.jpg'))
+        >>> img_in = vt.imread(ut.grab_test_imgpath('carl'))
         >>> verts = ((10, 10), (10, 100), (100, 100), (100, 10))
         >>> color = (0, 128, 255)
         >>> thickness = 2
         >>> out = img_in
         >>> # execute function
         >>> img = draw_verts(img_in, verts, color, thickness, out)
         >>> assert img_in is img, 'should be in place'
```

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/histogram.py` & `vtool_ibeis-2.3.0/vtool_ibeis/histogram.py`

 * *Files 0% similar despite different names*

```diff
@@ -971,16 +971,16 @@
         >>> from vtool_ibeis.histogram import *  # NOQA
         >>> import plottool_ibeis as pt
         >>> import vtool_ibeis as vt
         >>> result = show_ori_image_ondisk()
         >>> pt.show_if_requested()
     """
     #if img_fpath is not None:
-    #    img_fpath = ut.get_argval('--fpath', type_=str, default=ut.grab_test_imgpath('star.png'))
-    #    img_fpath = ut.get_argval('--fpath', type_=str, default=ut.grab_test_imgpath('star.png'))
+    #    img_fpath = ut.get_argval('--fpath', type_=str, default=ut.grab_test_imgpath('astro'))
+    #    img_fpath = ut.get_argval('--fpath', type_=str, default=ut.grab_test_imgpath('astro'))
     #    img = vt.imread(img_fpath)
     #    ori_img_fpath     = ut.get_argval('--fpath-ori', type_=str,
     #    default=ut.augpath(img_fpath, '_ori'))
     #    weights_img_fpath = ut.get_argval('--fpath-weight', type_=str,
     #    default=ut.augpath(img_fpath, '_mag'))
     #    vt.imwrite(ori_img_fpath, vt.patch_ori(*vt.patch_gradient(img)))
     #    vt.imwrite(weights_img_fpath, vt.patch_mag(*vt.patch_gradient(img)))
```

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/image.py` & `vtool_ibeis-2.3.0/vtool_ibeis/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,20 +285,20 @@
     References:
         http://docs.opencv.org/modules/core/doc/utility_and_system_functions_and_macros.html#error
         http://stackoverflow.com/questions/23572241/cv2-threshold-error-210
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> from vtool_ibeis.image import *  # NOQA
-        >>> img_fpath = ut.grab_test_imgpath('carl.jpg')
+        >>> img_fpath = ut.grab_test_imgpath('astro')
         >>> imgBGR1 = imread(img_fpath, grayscale=False)
         >>> imgBGR2 = imread(img_fpath, grayscale=True)
         >>> imgBGR3 = imread(img_fpath, orient=True)
-        >>> assert imgBGR1.shape == (250, 300, 3)
-        >>> assert imgBGR2.shape == (250, 300)
+        >>> assert imgBGR1.shape == (512, 512, 3)
+        >>> assert imgBGR2.shape == (512, 512)
         >>> assert np.all(imgBGR1 == imgBGR3)
         >>> # xdoctest: +REQUIRES(--show)
         >>> import plottool_ibeis as pt
         >>> pt.imshow(imgBGR1, pnum=(2, 2, 1))
         >>> pt.imshow(imgBGR2, pnum=(2, 2, 2))
         >>> pt.imshow(imgBGR3, pnum=(2, 2, 3))
         >>> ut.show_if_requested()
@@ -328,15 +328,15 @@
         >>> kwplot.imshow(imgBGR1, pnum=(1, 3, 1))
         >>> kwplot.imshow(diffMag / diffMag.max(), pnum=(1, 3, 2))
         >>> kwplot.imshow(imgBGR2, pnum=(1, 3, 3))
         >>> kwplot.show_if_requested()
         (2736, 3648, 3)
 
     Example:
-        >>> # ENABLE_DOCTEST
+        >>> # xdoctest +SKIP("networking")
         >>> from vtool_ibeis.image import *  # NOQA
         >>> url = 'http://www.sherv.net/cm/emo/funny/2/big-dancing-banana-smiley-emoticon.gif'
         >>> img_fpath = ut.grab_file_url(url)
         >>> delete_if_corrupted = False
         >>> grayscale = False
         >>> imgBGR = imread(img_fpath, grayscale=grayscale)
         >>> # xdoctest: +REQUIRES(--show)
@@ -536,30 +536,30 @@
         python -m vtool_ibeis.image --exec-imwrite
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> from vtool_ibeis.image import *  # NOQA
         >>> import vtool_ibeis as vt
         >>> import utool as ut
-        >>> img_fpath1 = ut.grab_test_imgpath('zebra.png')
+        >>> img_fpath1 = ut.grab_test_imgpath('astro')
         >>> imgBGR = vt.imread(img_fpath1)
         >>> img_dpath = ub.ensure_app_cache_dir('vtool_ibeis', 'testwrite')
-        >>> img_fpath2 = ut.unixjoin(img_dpath, 'zebra.png')
+        >>> img_fpath2 = ut.unixjoin(img_dpath, 'astro.png')
         >>> fallback = False
         >>> imwrite(img_fpath2, imgBGR, fallback=fallback)
         >>> imgBGR2 = vt.imread(img_fpath2)
         >>> assert np.all(imgBGR2 == imgBGR)
     """
     try:
         cv2.imwrite(img_fpath, imgBGR)
     except Exception as ex:
         if fallback:
             try:
                 imwrite_fallback(img_fpath, imgBGR)
-            except Exception as ex:
+            except Exception:
                 pass
         msg = '[vt.image] ERROR writing: %s' % (img_fpath,)
         ut.printex(ex, msg, keys=['imgBGR.shape'])
         raise
 
 
 def imwrite_fallback(img_fpath, imgBGR):
@@ -653,19 +653,19 @@
         tuple: size (width, height)
 
     CommandLine:
         python -m vtool_ibeis.image --test-open_image_size
 
     Doctest:
         >>> from vtool_ibeis.image import *  # NOQA
-        >>> image_fpath = ut.grab_test_imgpath('patsy.jpg')
+        >>> image_fpath = ut.grab_test_imgpath('carl')
         >>> size = open_image_size(image_fpath)
         >>> result = ('size = %s' % (str(size),))
         >>> print(result)
-        size = (800, 441)
+        size = (328, 448)
 
     Ignore:
         # Confirm that Image.open is a lazy load
         import vtool_ibeis as vt
         import utool as ut
         import timeit
         setup = ut.codeblock(
@@ -726,15 +726,15 @@
     CommandLine:
         python -m vtool_ibeis.image --test-warpAffine --show
 
     Example:
         >>> # DISABLE_DOCTEST
         >>> from vtool_ibeis.image import *  # NOQA
         >>> import vtool_ibeis as vt
-        >>> img_fpath = ut.grab_test_imgpath('carl.jpg')
+        >>> img_fpath = ut.grab_test_imgpath('carl')
         >>> img = vt.imread(img_fpath)
         >>> Aff = vt.rotation_mat3x3(TAU / 8)
         >>> dsize = vt.get_size(img)
         >>> warped_img = warpAffine(img, Aff, dsize)
         >>> # xdoctest: +REQUIRES(--show)
         >>> import plottool_ibeis as pt
         >>> pt.imshow(warped_img)
@@ -1102,15 +1102,15 @@
     CommandLine:
         python -m vtool_ibeis.image --test-rotate_image_ondisk
 
     Example:
         >>> # DISABLE_DOCTEST
         >>> from vtool_ibeis.image import *  # NOQA
         >>> # build test data
-        >>> img_fpath = ut.grab_test_imgpath('star.png')
+        >>> img_fpath = ut.grab_test_imgpath('astro')
         >>> theta = TAU * 3 / 8
         >>> # execute function
         >>> out_fpath = None
         >>> out_fpath_ = rotate_image_ondisk(img_fpath, theta, out_fpath)
         >>> print(out_fpath_)
         >>> if ut.get_argflag('--show') or ut.inIPython():
         >>>     import plottool_ibeis as pt
@@ -1418,17 +1418,17 @@
     CommandLine:
         python -m vtool_ibeis.image convert_colorspace --show
 
     Example:
         >>> # DISABLE_DOCTEST
         >>> from vtool_ibeis.image import *  # NOQA
         >>> import vtool_ibeis as vt
-        >>> img_fpath = ut.grab_test_imgpath('zebra.png')
-        >>> img_fpath = ut.grab_file_url('http://itsnasb.com/wp-content/uploads/2013/03/lisa-frank-logo1.jpg')
-        >>> img_fpath = ut.grab_test_imgpath('carl.jpg')
+        >>> #img_fpath = ut.grab_file_url('http://itsnasb.com/wp-content/uploads/2013/03/lisa-frank-logo1.jpg')
+        >>> #img_fpath = ut.grab_test_imgpath('carl')
+        >>> img_fpath = ut.grab_test_imgpath('pm5644')
         >>> img = vt.imread(img_fpath)
         >>> img_float = vt.rectify_to_float01(img, np.float32)
         >>> colorspace = 'LAB'
         >>> src_colorspace = 'BGR'
         >>> imgLAB = convert_colorspace(img, colorspace, src_colorspace)
         >>> imgL = imgLAB[:, :, 0]
         >>> fillL = imgL.mean()
@@ -1504,17 +1504,17 @@
     CommandLine:
         python -m vtool_ibeis.image --test-padded_resize --show
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> from vtool_ibeis.image import *  # NOQA
         >>> import vtool_ibeis as vt
-        >>> imgA = vt.imread(ut.grab_test_imgpath('carl.jpg'))
-        >>> imgB = vt.imread(ut.grab_test_imgpath('ada.jpg'))
-        >>> imgC = vt.imread(ut.grab_test_imgpath('carl.jpg'), grayscale=True)
+        >>> imgA = vt.imread(ut.grab_test_imgpath('carl'))
+        >>> imgB = vt.imread(ut.grab_test_imgpath('astro'))
+        >>> imgC = vt.imread(ut.grab_test_imgpath('carl'), grayscale=True)
         >>> #target_size = (64, 64)
         >>> target_size = (1024, 1024)
         >>> img3_list = [padded_resize(img, target_size) for img in [imgA, imgB, imgC]]
         >>> # verify results
         >>> assert ut.allsame([vt.get_size(img3) for img3 in img3_list])
         >>> # xdoctest: +REQUIRES(--show)
         >>> import plottool_ibeis as pt
@@ -1550,15 +1550,15 @@
     CommandLine:
         python -m vtool_ibeis.image embed_in_square_image --show
 
     Example:
         >>> # DISABLE_DOCTEST
         >>> from vtool_ibeis.image import *  # NOQA
         >>> import vtool_ibeis as vt
-        >>> img_fpath = ut.grab_test_imgpath('carl.jpg')
+        >>> img_fpath = ut.grab_test_imgpath('carl')
         >>> img = vt.imread(img_fpath)
         >>> target_size = tuple(np.array(vt.get_size(img)) * 3)
         >>> img_origin = (.5, .5)
         >>> target_origin = (.5, .5)
         >>> img_square = embed_in_square_image(img, target_size, img_origin, target_origin)
         >>> assert img_square.sum() == img.sum()
         >>> assert vt.get_size(img_square) == target_size
@@ -1703,15 +1703,15 @@
     CommandLine:
         python -m vtool_ibeis.image --test-resize_to_maxdims --show
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> from vtool_ibeis.image import *  # NOQA
         >>> import vtool_ibeis as vt
-        >>> img_fpath = ut.grab_test_imgpath('carl.jpg')
+        >>> img_fpath = ut.grab_test_imgpath('carl')
         >>> img = vt.imread(img_fpath)
         >>> max_dsize = (1024, 1024)
         >>> img2 = resize_to_maxdims(img, max_dsize)
         >>> print('img.shape = %r' % (img.shape,))
         >>> print('img2.shape = %r' % (img2.shape,))
         >>> # verify results
         >>> # xdoctest: +REQUIRES(--show)
@@ -1733,15 +1733,15 @@
         python -m vtool_ibeis.image --test-resize_thumb --show
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> from vtool_ibeis.image import *  # NOQA
         >>> import vtool_ibeis as vt
         >>> # build test data
-        >>> img_fpath = ut.grab_test_imgpath('carl.jpg')
+        >>> img_fpath = ut.grab_test_imgpath('carl')
         >>> img = vt.imread(img_fpath)
         >>> max_dsize = (64, 64)
         >>> # execute function
         >>> img2 = resize_thumb(img, max_dsize)
         >>> print('img.shape = %r' % (img.shape,))
         >>> print('img2.shape = %r' % (img2.shape,))
         >>> # verify results
@@ -2004,19 +2004,19 @@
 
 # STACK IMAGES STUFF
 
 
 def testdata_imglist():
     # build test data
     import vtool_ibeis as vt
-    img1 = vt.imread(ut.grab_test_imgpath('carl.jpg'))
-    img2 = vt.imread(ut.grab_test_imgpath('astro.png'))
-    img3 = vt.imread(ut.grab_test_imgpath('ada.jpg'))
-    img4 = vt.imread(ut.grab_test_imgpath('jeff.png'))
-    img5 = vt.imread(ut.grab_test_imgpath('star.png'))
+    img1 = vt.imread(ut.grab_test_imgpath('carl'))
+    img2 = vt.imread(ut.grab_test_imgpath('astro'))
+    img3 = vt.imread(ut.grab_test_imgpath('stars'))
+    img4 = vt.imread(ut.grab_test_imgpath('pm5644'))
+    img5 = vt.imread(ut.grab_test_imgpath('parrot'))
     img_list = [img1, img2, img3, img4, img5]
     return img_list
 
 
 def stack_image_list_special(img1, img_list, num=1, vert=True, use_larger=True,
                              initial_sf=None, interpolation=None):
     r"""
@@ -2419,17 +2419,17 @@
     CommandLine:
         python -m vtool_ibeis.image --exec-ensure_3channel --show
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> from vtool_ibeis.image import *  # NOQA
         >>> import vtool_ibeis as vt
-        >>> patch1 = vt.imread(ut.grab_test_imgpath('astro.png'))[0:512, 0:500, :]
-        >>> patch2 = vt.imread(ut.grab_test_imgpath('ada.jpg'))[:, :, 0:1]
-        >>> patch3 = vt.imread(ut.grab_test_imgpath('jeff.png'))[0:390, 0:400, 0]
+        >>> patch1 = vt.imread(ut.grab_test_imgpath('astro'))[0:512, 0:500, :]
+        >>> patch2 = vt.imread(ut.grab_test_imgpath('carl'))[:, :, 0:1]
+        >>> patch3 = vt.imread(ut.grab_test_imgpath('paraview'))[0:390, 0:400, 0]
         >>> res1 = ensure_3channel(patch1)
         >>> res2 = ensure_3channel(patch2)
         >>> res3 = ensure_3channel(patch3)
         >>> assert res1.shape[0:2] == patch1.shape[0:2], 'failed test1'
         >>> assert res2.shape[0:2] == patch2.shape[0:2], 'failed test2'
         >>> assert res3.shape[0:2] == patch3.shape[0:2], 'failed test3'
         >>> assert res1.shape[-1] == 3
@@ -2485,16 +2485,16 @@
         python -m vtool_ibeis.image --test-stack_images --show
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> from vtool_ibeis.image import *  # NOQA
         >>> import vtool_ibeis as vt
         >>> # build test data
-        >>> img1 = vt.imread(ut.grab_test_imgpath('carl.jpg'))
-        >>> img2 = vt.imread(ut.grab_test_imgpath('astro.png'))
+        >>> img1 = vt.imread(ut.grab_test_imgpath('carl'))
+        >>> img2 = vt.imread(ut.grab_test_imgpath('astro'))
         >>> vert = True
         >>> modifysize = False
         >>> # execute function
         >>> return_sf = True
         >>> #(imgB, woff, hoff) = stack_images(img1, img2, vert, modifysize, return_sf=return_sf)
         >>> overlap = 100
         >>> imgB, offset2, sf_tup = stack_images(img1, img2, vert, modifysize,
@@ -2641,28 +2641,28 @@
         python -m vtool_ibeis.image --test-stack_image_recurse --show
 
     Example:
         >>> # DISABLE_DOCTEST
         >>> from vtool_ibeis.image import *  # NOQA
         >>> import vtool_ibeis as vt
         >>> # build test data
-        >>> img1 = vt.imread(ut.grab_test_imgpath('carl.jpg'))
-        >>> img2 = vt.imread(ut.grab_test_imgpath('astro.png'))
-        >>> img3 = vt.imread(ut.grab_test_imgpath('ada.jpg'))
-        >>> img4 = vt.imread(ut.grab_test_imgpath('jeff.png'))
-        >>> img5 = vt.imread(ut.grab_test_imgpath('star.png'))
+        >>> img1 = vt.imread(ut.grab_test_imgpath('carl'))
+        >>> img2 = vt.imread(ut.grab_test_imgpath('astro'))
+        >>> img3 = vt.imread(ut.grab_test_imgpath('paraview'))
+        >>> img4 = vt.imread(ut.grab_test_imgpath('lowcontrast'))
+        >>> img5 = vt.imread(ut.grab_test_imgpath('stars'))
         >>> img_list1 = [img1, img2, img3, img4, img5]
         >>> img_list2 = None
         >>> vert = True
         >>> # execute function
         >>> imgB = stack_image_recurse(img_list1, img_list2, vert)
         >>> # verify results
         >>> # xdoctest: +REQUIRES(--show)
         >>> import plottool_ibeis as pt
-        >>> imshow(imgB)
+        >>> pt.imshow(imgB)
         >>> #wh1 = img1.shape[0:2][::-1]
         >>> #wh2 = img2.shape[0:2][::-1]
         >>> #pt.draw_bbox((0, 0) + wh1, bbox_color=(1, 0, 0))
         >>> #pt.draw_bbox((woff, hoff) + wh2, bbox_color=(0, 1, 0))
         >>> pt.show_if_requested()
     """
     interpolation = _rectify_interpolation(interpolation, default=cv2.INTER_NEAREST)
@@ -2728,16 +2728,16 @@
         An MPO (Multi Picture Object) file is a stereoscopic image and contains
         two JPG images side-by-side, and allows them to be viewed as a single
         3D image.
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> from vtool_ibeis.image import *  # NOQA
-        >>> gpaths = [ut.grab_test_imgpath('carl.jpg'),
-        >>>           ut.grab_test_imgpath('astro.png')]
+        >>> gpaths = [ut.grab_test_imgpath('carl'),
+        >>>           ut.grab_test_imgpath('astro')]
         >>> flags = filterflags_valid_images(gpaths)
         >>> assert all(flags)
     """
     from PIL import Image
     from os.path import splitext
     #import operator
     #import itertools as it
```

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/image_filters.py` & `vtool_ibeis-2.3.0/vtool_ibeis/image_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
     CommandLine:
         python -m vtool_ibeis.image_filters IntensityPreproc --show
 
     Doctest:
         >>> from vtool_ibeis.image_filters import *
         >>> import vtool_ibeis as vt
-        >>> chipBGR = vt.imread(ut.grab_file_url('http://i.imgur.com/qVWQaex.jpg'))
+        >>> #chipBGR = vt.imread(ut.grab_file_url('http://i.imgur.com/qVWQaex.jpg'))
+        >>> chipBGR = vt.imread(ut.grab_test_imgpath('astro'))
         >>> filter_list = [
         >>>     ('medianblur', {}),
         >>>     ('adapteq', {}),
         >>> ]
         >>> self = IntensityPreproc()
         >>> chipBGR2 = self.preprocess(chipBGR, filter_list)
         >>> # xdoctest: +REQUIRES(--show)
@@ -67,15 +68,17 @@
     References:
         http://onlinelibrary.wiley.com/doi/10.1002/ece3.587/full
 
     Ignore:
         >>> from ibeis.core_annots import *  # NOQA
         >>> import ibeis
         >>> ibs = ibeis.opendb('Mantas')
-        >>> chipBGR = vt.imread(ut.grab_file_url('http://i.imgur.com/qVWQaex.jpg'))
+        >>> #chipBGR = vt.imread(ut.grab_file_url('http://i.imgur.com/qVWQaex.jpg'))
+        >>> chipBGR = vt.imread(ut.grab_test_imgpath('astro'))
+
     """
     chipLAB = cv2.cvtColor(chipBGR, cv2.COLOR_BGR2LAB)
 
     intensity = chipLAB[:, :, 0]
     # Median filter
     noise_thresh = 100
     ksize = 5 if intensity.std() > noise_thresh else 3
@@ -95,15 +98,16 @@
     """
     adaptive histogram equalization with CLAHE
 
     Example:
         >>> from vtool_ibeis.image_filters import *
         >>> import vtool_ibeis as vt
         >>> import utool as ut
-        >>> chipBGR = vt.imread(ut.grab_file_url('http://i.imgur.com/qVWQaex.jpg'))
+        >>> #chipBGR = vt.imread(ut.grab_file_url('http://i.imgur.com/qVWQaex.jpg'))
+        >>> chipBGR = vt.imread(ut.grab_test_imgpath('astro'))
         >>> chip2 = adapteq_fn(chipBGR)
         >>> # xdoctest: +REQUIRES(--show)
         >>> import plottool_ibeis as pt
         >>> pt.imshow(chipBGR, pnum=(1, 2, 1), fnum=1)
         >>> pt.imshow(chip2, pnum=(1, 2, 2), fnum=1)
         >>> ut.show_if_requested()
     """
@@ -120,16 +124,17 @@
     """
     median filtering
 
     Example:
         >>> from vtool_ibeis.image_filters import *
         >>> import vtool_ibeis as vt
         >>> import utool as ut
-        >>> chipBGR = vt.imread(ut.grab_file_url('http://i.imgur.com/qVWQaex.jpg'))
-        >>> chip2 = adapteq_fn(chipBGR)
+        >>> #chipBGR = vt.imread(ut.grab_file_url('http://i.imgur.com/qVWQaex.jpg'))
+        >>> chipBGR = vt.imread(ut.grab_test_imgpath('astro'))
+        >>> chip2 = medianfilter_fn(chipBGR)
         >>> # xdoctest: +REQUIRES(--show)
         >>> import plottool_ibeis as pt
         >>> pt.imshow(chipBGR, pnum=(1, 2, 1), fnum=1)
         >>> pt.imshow(chip2, pnum=(1, 2, 2), fnum=1)
         >>> ut.show_if_requested()
     """
     chipLAB = cv2.cvtColor(chipBGR, cv2.COLOR_BGR2LAB)
@@ -195,15 +200,14 @@
     chipHSV = np.array(chipHSV, dtype=float) / 255.0
     chipHSV[:, :, 2] *= chip_mask
     chipHSV = np.array(np.round(chipHSV * 255.0), dtype=np.uint8)
     seg_chipBGR = cv2.cvtColor(chipHSV, cv2.COLOR_HSV2BGR)
     return seg_chipBGR
 
 
-
 if __name__ == '__main__':
     """
     CommandLine:
         xdoctest -m vtool_ibeis.image_filters
     """
     import xdoctest
     xdoctest.doctest_module(__file__)
```

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/inspect_matches.py` & `vtool_ibeis-2.3.0/vtool_ibeis/inspect_matches.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,16 +65,16 @@
 
     Example:
         >>> # SCRIPT
         >>> from vtool_ibeis.inspect_matches import *  # NOQA
         >>> import vtool_ibeis as vt
         >>> gt.ensure_qapp()
         >>> ut.qtensure()
-        >>> annot1 = lazy_test_annot('easy1.png')
-        >>> annot2 = lazy_test_annot('easy2.png')
+        >>> annot1 = lazy_test_annot('tsukuba_r')
+        >>> annot2 = lazy_test_annot('tsukuba_l')
         >>> match = vt.PairwiseMatch(annot1, annot2)
         >>> self = MatchInspector(match=match)
         >>> self.show()
         >>> # xdoctest: +REQUIRES(--show)
         >>> #self.update()
         >>> gt.qtapp_loop(qwin=self, freq=10)
```

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/keypoint.py` & `vtool_ibeis-2.3.0/vtool_ibeis/keypoint.py`

 * *Files identical despite different names*

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/linalg.py` & `vtool_ibeis-2.3.0/vtool_ibeis/linalg.py`

 * *Files identical despite different names*

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/matching.py` & `vtool_ibeis-2.3.0/vtool_ibeis/matching.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,21 +98,21 @@
         use_cache = False
     function_sig = ut.get_func_sourcecode(vt.matching.PairwiseMatch)
     hashid = ut.hash_data(function_sig)
     ub.util_hash._HASHABLE_EXTENSIONS._register_agressive_extensions()
     cfgstr = ub.hash_data(cfgdict) + hashid
     cacher = ub.Cacher(
         'test_match_v5',
-        cfgstr=cfgstr,
+        depends=cfgstr,
         appname='vtool_ibeis',
         enabled=use_cache
     )
     match = cacher.tryload()
-    annot1 = lazy_test_annot('easy1.png')
-    annot2 = lazy_test_annot('easy2.png')
+    annot1 = lazy_test_annot('tsukuba_l')
+    annot2 = lazy_test_annot('tsukuba_r')
     if match is None or recompute:
         match = vt.PairwiseMatch(annot1, annot2)
         if apply:
             match.apply_all(cfgdict)
         cacher.save(match)
     else:
         match.annot1 = annot1
@@ -137,16 +137,18 @@
         Optional annotation attributes:
             aid, nid, flann, rchip, dlen_sqrd, weight
 
     Ignore:
         >>> # xdoctest: +REQUIRES(module:pyhesaff)
         >>> from vtool_ibeis.matching import *  # NOQA
         >>> import vtool_ibeis as vt
-        >>> imgR = vt.imread(ut.grab_test_imgpath('easy1.png'))
-        >>> imgL = vt.imread(ut.grab_test_imgpath('easy2.png'))
+        >>> #imgR = vt.imread(ut.grab_test_imgpath('easy1.png'))
+        >>> #imgL = vt.imread(ut.grab_test_imgpath('easy2.png'))
+        >>> imgR = vt.imread(ut.grab_test_imgpath('tsukuba_r'))
+        >>> imgL = vt.imread(ut.grab_test_imgpath('tsukuba_l'))
         >>> annot1 = {'rchip': imgR}
         >>> annot2 = {'rchip': imgL}
         >>> match = vt.PairwiseMatch(annot1, annot2)
         >>> match.apply_all({'refine_method': 'affine', 'affine_invariance': False, 'rotation_invariance': False})
         >>> dsize = imgR.shape[0:2][::-1]
         >>> imgR_warp = vt.warpHomog(imgR, match.H_12, dsize)
         >>> # xdoctest: +REQUIRES(--show)
@@ -158,16 +160,16 @@
         >>> kwplot.imshow(imgR_warp, pnum=(2, 1, 2))
         >>> # xdoctest: +REQUIRES(--gui)
         >>> import guitool_ibeis as gt
         >>> gt.ensure_qapp()
         >>> match.ishow()
         >>> from vtool_ibeis.matching import *  # NOQA
         >>> import vtool_ibeis as vt
-        >>> imgR = vt.imread(ut.grab_test_imgpath('easy1.png'))
-        >>> imgL = vt.imread(ut.grab_test_imgpath('easy2.png'))
+        >>> imgR = vt.imread(ut.grab_test_imgpath('tsukuba_r'))
+        >>> imgL = vt.imread(ut.grab_test_imgpath('tsukuba_l'))
         >>> annot1 = {'rchip': imgR}
         >>> annot2 = {'rchip': imgL}
         >>> match = vt.PairwiseMatch(annot1, annot2)
         >>> match.apply_all({'refine_method': 'affine', 'affine_invariance': False, 'rotation_invariance': False})
         >>> dsize = imgR.shape[0:2][::-1]
         >>> imgR_warp = vt.warpHomog(imgR, match.H_12, dsize)
         >>> # xdoctest: +REQUIRES(--show)
@@ -449,16 +451,18 @@
         """
         params = match._take_params(cfgdict, ['K', 'Knorm', 'symmetric',
                                               'checks', 'weight'])
         params = list(params)
         K, Knorm, symmetric, checks, weight_key = params
         annot1 = match.annot1
         annot2 = match.annot2
+        if verbose is None:
+            verbose = match.verbose
 
-        if match.verbose:
+        if verbose:
             print('[match] assign')
             print('[match] params = ' + ub.repr2(params))
 
         ensure_metadata_vsone(annot1, annot2, cfgdict)
 
         allow_shrink = True  # TODO: parameterize?
 
@@ -1443,15 +1447,15 @@
     CommandLine:
         python -m vtool_ibeis.matching --exec-ensure_metadata_feats
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> # xdoctest: +REQUIRES(module:pyhesaff)
         >>> from vtool_ibeis.matching import *  # NOQA
-        >>> rchip_fpath = ut.grab_test_imgpath('easy1.png')
+        >>> rchip_fpath = ut.grab_test_imgpath('astro')
         >>> annot = ut.LazyDict({'rchip_fpath': rchip_fpath})
         >>> cfgdict = {}
         >>> ensure_metadata_feats(annot, cfgdict)
         >>> assert len(annot._stored_results) == 1
         >>> annot['kpts']
         >>> assert len(annot._stored_results) >= 4
         >>> annot['vecs']
```

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/nearest_neighbors.py` & `vtool_ibeis-2.3.0/vtool_ibeis/nearest_neighbors.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,16 +105,18 @@
 
         ut.grab_zipped_url('https://priithon.googlecode.com/archive/a6117f5e81ec00abcfb037f0f9da2937bb2ea47f.tar.gz', download_dir='.')
     """
     import cv2
     from vtool_ibeis import demodata
     import plottool_ibeis as pt
     import vtool_ibeis as vt
-    img1 = vt.imread(ut.grab_test_imgpath('easy1.png'))
-    img2 = vt.imread(ut.grab_test_imgpath('easy2.png'))
+    # img1 = vt.imread(ut.grab_test_imgpath('easy1.png'))
+    # img2 = vt.imread(ut.grab_test_imgpath('easy2.png'))
+    img1 = vt.imread(ut.grab_test_imgpath('tsukuba_l'))
+    img2 = vt.imread(ut.grab_test_imgpath('tsukuba_r'))
 
     stereo = cv2.StereoBM_create(numDisparities=16, blockSize=15)
     disparity = stereo.compute(img1, img2)
     pt.imshow(disparity)
     pt.show()
 
     #cv2.estima
```

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/numpy_utils.py` & `vtool_ibeis-2.3.0/vtool_ibeis/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/other.py` & `vtool_ibeis-2.3.0/vtool_ibeis/other.py`

 * *Files identical despite different names*

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/patch.py` & `vtool_ibeis-2.3.0/vtool_ibeis/patch.py`

 * *Files 0% similar despite different names*

```diff
@@ -566,15 +566,15 @@
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> # xdoctest: +REQUIRES(module:pyhesaff)
         >>> from vtool_ibeis.patch import *  # NOQA
         >>> import vtool_ibeis as vt
         >>> # build test data
-        >>> img_fpath = ut.grab_test_imgpath('carl.jpg')
+        >>> img_fpath = ut.grab_test_imgpath('carl')
         >>> img = vt.imread(img_fpath)
         >>> use_cpp = ut.get_argflag('--use_cpp')
         >>> kpts, desc = vt.extract_features(img_fpath)
         >>> kpts = kpts[0:1]
         >>> flags = cv2.INTER_LANCZOS4
         >>> borderMode = cv2.BORDER_REPLICATE
         >>> # execute function
@@ -1061,52 +1061,40 @@
         >>> # DISABLE_DOCTEST
         >>> # xdoctest: +REQUIRES(module:pyhesaff)
         >>> import plottool_ibeis as pt
         >>> from vtool_ibeis.patch import *  # NOQA
         >>> draw_kp_ori_steps()
         >>> pt.show_if_requested()
     """
-    #from vtool_ibeis.patch import *  # NOQA
-    #import vtool_ibeis as vt
     # build test data
     import utool as ut
     import plottool_ibeis as pt
-    import vtool_ibeis as vt
 
     if True:
         from ibeis.scripts.thesis import TMP_RC
         import matplotlib as mpl
         mpl.rcParams.update(TMP_RC)
-    #import vtool_ibeis as vt
     np.random.seed(0)
     USE_COMMANLINE = True
     if USE_COMMANLINE:
         kpts, vecs, imgBGR = pt.viz_keypoints.testdata_kpts()
         fx = ut.get_argval('--fx', type_=int, default=0)
         kp = kpts[fx]
     else:
         fx = 0
-        USE_EXTERN_STAR = False
-        if USE_EXTERN_STAR:
-            img_fpath = ut.grab_test_imgpath('star.png')
-            imgBGR = vt.imread(img_fpath)
-            kpts, vecs = vt.extract_features(img_fpath)
-            kp = np.array([  3.14742985e+01,   2.95660381e+01,   1.96057682e+01, -5.11199608e-03,   2.05653343e+01,   0.00000000e+00],
-                          dtype=np.float32)
-        else:
-            #imgBGR = get_test_patch('stripe', jitter=True)
-            #imgBGR = get_test_patch('star', jitter=True)
-            imgBGR = get_test_patch('star2', jitter=True)
-            #imgBGR = get_test_patch('cross', jitter=False)
-            #imgBGR = cv2.resize(imgBGR, (41, 41), interpolation=cv2.INTER_LANCZOS4)
-            imgBGR = cv2.resize(imgBGR, (41, 41), interpolation=cv2.INTER_CUBIC)
-            theta = 0  # 3.4  # TAU / 16
-            #kpts = make_test_image_keypoints(imgBGR, scale=.9, theta=theta)
-            kpts = make_test_image_keypoints(imgBGR, scale=.3, theta=theta, shift=(.3, .1))
-            kp = kpts[0]
+        #imgBGR = get_test_patch('stripe', jitter=True)
+        #imgBGR = get_test_patch('star', jitter=True)
+        imgBGR = get_test_patch('star2', jitter=True)
+        #imgBGR = get_test_patch('cross', jitter=False)
+        #imgBGR = cv2.resize(imgBGR, (41, 41), interpolation=cv2.INTER_LANCZOS4)
+        imgBGR = cv2.resize(imgBGR, (41, 41), interpolation=cv2.INTER_CUBIC)
+        theta = 0  # 3.4  # TAU / 16
+        #kpts = make_test_image_keypoints(imgBGR, scale=.9, theta=theta)
+        kpts = make_test_image_keypoints(imgBGR, scale=.3, theta=theta, shift=(.3, .1))
+        kp = kpts[0]
     bins = 36
     maxima_thresh = .8
     converge_lists = []
 
     def exec_internals_find_patch_dominant_orientations(patch, bins, maxima_thresh, old_ori):
         # TODO: can use ut.exec_func_src instead
         # <HACKISH>
```

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/quality_classifier.py` & `vtool_ibeis-2.3.0/vtool_ibeis/quality_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     CommandLine:
         python -m vtool_ibeis.quality_classifier --exec-compute_average_contrast --show
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> from vtool_ibeis.quality_classifier import *  # NOQA
         >>> import vtool_ibeis as vt
-        >>> img_fpath = ut.grab_test_imgpath('carl.jpg')
+        >>> img_fpath = ut.grab_test_imgpath('carl')
         >>> img = vt.imread(img_fpath, grayscale=True)
         >>> average_contrast, gradmag_sqrd = compute_average_contrast(img)
         >>> # xdoctest: +REQUIRES(module:plottool_ibeis)
         >>> import plottool_ibeis as pt
         >>> # xdoctest: +REQUIRES(--show)
         >>> pt.figure(fnum=1)
         >>> pt.plt.imshow(gradmag_sqrd)
@@ -100,15 +100,15 @@
         http://opencv-python-tutroals.readthedocs.org/en/latest/py_tutorials/py_imgproc/py_transforms/py_fourier_transform/py_fourier_transform.html
         http://cns-alumni.bu.edu/~slehar/fourier/fourier.html
 
     Example:
         >>> # DISABLE_DOCTEST
         >>> from vtool_ibeis.quality_classifier import *  # NOQA
         >>> import vtool_ibeis as vt
-        >>> img_fpath = ut.grab_test_imgpath('carl.jpg')
+        >>> img_fpath = ut.grab_test_imgpath('carl')
         >>> img = vt.imread(img_fpath, grayscale=True)
         >>> magnitude_spectrum = fourier_devtest(img)
     """
     import plottool_ibeis as pt
     def pad_img(img):
         rows, cols = img.shape
         nrows = cv2.getOptimalDFTSize(rows)
```

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/score_normalization.py` & `vtool_ibeis-2.3.0/vtool_ibeis/score_normalization.py`

 * *Files identical despite different names*

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/segmentation.py` & `vtool_ibeis-2.3.0/vtool_ibeis/segmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     Example:
         >>> # DISABLE_DOCTEST
         >>> from vtool_ibeis.segmentation import *  # NOQA
         >>> # build test data
         >>> import utool as ut
         >>> import plottool_ibeis as pt
         >>> import vtool_ibeis as vt
-        >>> img_fpath = ut.grab_test_imgpath('easy1.png')
+        >>> img_fpath = ut.grab_test_imgpath('astro')
         >>> bgr_img = vt.imread(img_fpath)
         >>> # execute function
         >>> print(bgr_img.shape)
         >>> result = demo_grabcut(bgr_img)
         >>> # verify results
         >>> print(result)
         >>> ## xdoctest: +REQUIRES(--show)
```

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/spatial_verification.py` & `vtool_ibeis-2.3.0/vtool_ibeis/spatial_verification.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,16 +370,16 @@
     import vtool_ibeis as vt
     scale_thresh = 2.0
     xy_thresh = ut.get_argval('--xy-thresh', type_=float, default=.01)
     dlen_sqrd2 = 447271.015
     ori_thresh = 1.57
     xy_thresh_sqrd = dlen_sqrd2 * xy_thresh
     featkw = ut.argparse_dict(vt.get_extract_features_default_params())
-    fname1 = ut.get_argval('--fname1', type_=str, default='easy1.png')
-    fname2 = ut.get_argval('--fname2', type_=str, default='easy2.png')
+    fname1 = ut.get_argval('--fname1', type_=str, default='tsukuba_l')
+    fname2 = ut.get_argval('--fname2', type_=str, default='tsukuba_r')
     (kpts1, kpts2, fm, fs, rchip1, rchip2) = demodata.testdata_ratio_matches(fname1, fname2, **featkw)
     aff_inliers, aff_errors, Aff = get_best_affine_inliers_(
         kpts1, kpts2, fm, fs, xy_thresh_sqrd, scale_thresh, ori_thresh)
     return kpts1, kpts2, fm, aff_inliers, rchip1, rchip2, xy_thresh_sqrd
 
 
 def testdata_matching_affine_inliers_normalized():
@@ -954,16 +954,16 @@
 
     Example:
         >>> # ENABLE_DOCTEST
         >>> # xdoctest: +REQUIRES(module:pyhesaff)
         >>> from vtool_ibeis.spatial_verification import *
         >>> import vtool_ibeis.demodata as demodata
         >>> import vtool_ibeis as vt
-        >>> fname1 = ut.get_argval('--fname1', type_=str, default='easy1.png')
-        >>> fname2 = ut.get_argval('--fname2', type_=str, default='easy2.png')
+        >>> fname1 = ut.get_argval('--fname1', type_=str, default='tsukuba_r')
+        >>> fname2 = ut.get_argval('--fname2', type_=str, default='tsukuba_l')
         >>> default_dict = vt.get_extract_features_default_params()
         >>> default_dict['ratio_thresh'] = .625
         >>> kwargs = ut.argparse_dict(default_dict)
         >>> (kpts1, kpts2, fm, fs, rchip1, rchip2) = demodata.testdata_ratio_matches(fname1, fname2, **kwargs)
         >>> xy_thresh = .01
         >>> dlen_sqrd2 = 447271.015
         >>> ori_thresh = 1.57
@@ -989,16 +989,14 @@
         >>> print(result)
         >>> # xdoctest: +REQUIRES(--show)
         >>> import plottool_ibeis as pt
         >>> homog_tup = (refined_inliers, H)
         >>> aff_tup = (aff_inliers, Aff)
         >>> pt.draw_sv.show_sv(rchip1, rchip2, kpts1, kpts2, fm, aff_tup=aff_tup, homog_tup=homog_tup, refine_method=refine_method)
         >>> pt.show_if_requested()
-        tuple(numpy.ndarray, tuple(numpy.ndarray*3), numpy.ndarray, numpy.ndarray, tuple(numpy.ndarray*3), numpy.ndarray)
-
     """
     if len(fm) == 0:
         if VERBOSE_SVER:
             print('[sver] Cannot verify with no matches')
         svtup = None
         return svtup
     # Cast keypoints to float64 to avoid numerical issues
```

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/sver_c_wrapper.py` & `vtool_ibeis-2.3.0/vtool_ibeis/sver_c_wrapper.py`

 * *Files identical despite different names*

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/symbolic.py` & `vtool_ibeis-2.3.0/vtool_ibeis/symbolic.py`

 * *Files identical despite different names*

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/trig.py` & `vtool_ibeis-2.3.0/vtool_ibeis/trig.py`

 * *Files identical despite different names*

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis/util_math.py` & `vtool_ibeis-2.3.0/vtool_ibeis/util_math.py`

 * *Files identical despite different names*

### Comparing `vtool_ibeis-2.2.1/vtool_ibeis.egg-info/SOURCES.txt` & `vtool_ibeis-2.3.0/vtool_ibeis.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 LICENSE
 README.rst
 pyproject.toml
 setup.py
+tests/test_akmeans.py
+tests/test_coverage_max_reduce.py
+tests/test_draw_keypoint.py
+tests/test_import.py
+tests/test_pyflann.py
+tests/test_spatial_verification.py
+tests/test_vtool.py
+tests/testdata_nondeterm_sver.py
 vtool_ibeis/__init__.py
 vtool_ibeis/__main__.py
 vtool_ibeis/_pyflann_backend.py
 vtool_ibeis/_rhomb_dist.py
 vtool_ibeis/blend.py
 vtool_ibeis/chip.py
 vtool_ibeis/clustering2.py
```

