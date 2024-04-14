# Comparing `tmp/h3-4.0.0b3.tar.gz` & `tmp/h3-4.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h3-4.0.0b3.tar", last modified: Tue Mar 12 20:47:17 2024, max compression
+gzip compressed data, was "h3-4.0.0b4.tar", last modified: Sun Apr 14 17:44:12 2024, max compression
```

## Comparing `h3-4.0.0b3.tar` & `h3-4.0.0b4.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:47:17.290313 h3-4.0.0b3/
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-03-12 20:47:08.000000 h3-4.0.0b3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-12 20:47:08.000000 h3-4.0.0b3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-12 20:47:08.000000 h3-4.0.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-03-12 20:47:17.290313 h3-4.0.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-12 20:47:08.000000 h3-4.0.0b3/makefile
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-12 20:47:08.000000 h3-4.0.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3517 2024-03-12 20:47:08.000000 h3-4.0.0b3/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-12 20:47:08.000000 h3-4.0.0b3/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 20:47:17.290313 h3-4.0.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-12 20:47:08.000000 h3-4.0.0b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:47:17.274314 h3-4.0.0b3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:47:17.278313 h3-4.0.0b3/src/h3/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:47:17.282313 h3-4.0.0b3/src/h3/_cy/
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/_cy/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/_cy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/_cy/cells.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/_cy/cells.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/_cy/edges.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/_cy/edges.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/_cy/error_system.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/_cy/error_system.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/_cy/h3lib.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/_cy/latlng.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/_cy/latlng.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/_cy/memory.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/_cy/memory.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/_cy/to_multipoly.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/_cy/util.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/_cy/util.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     7673 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/_h3shape.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:47:17.282313 h3-4.0.0b3/src/h3/api/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:47:17.282313 h3-4.0.0b3/src/h3/api/basic_int/
--rw-r--r--   0 runner    (1001) docker     (127)    19659 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/api/basic_int/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/api/basic_int/_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:47:17.282313 h3-4.0.0b3/src/h3/api/basic_str/
--rw-r--r--   0 runner    (1001) docker     (127)    19659 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/api/basic_str/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/api/basic_str/_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:47:17.282313 h3-4.0.0b3/src/h3/api/memview_int/
--rw-r--r--   0 runner    (1001) docker     (127)    19659 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/api/memview_int/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/api/memview_int/_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:47:17.282313 h3-4.0.0b3/src/h3/api/numpy_int/
--rw-r--r--   0 runner    (1001) docker     (127)    19659 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/api/numpy_int/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-12 20:47:08.000000 h3-4.0.0b3/src/h3/api/numpy_int/_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:47:17.290313 h3-4.0.0b3/src/h3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5079 2024-03-12 20:47:17.000000 h3-4.0.0b3/src/h3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-03-12 20:47:17.000000 h3-4.0.0b3/src/h3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 20:47:17.000000 h3-4.0.0b3/src/h3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-12 20:47:17.000000 h3-4.0.0b3/src/h3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-03-12 20:47:17.000000 h3-4.0.0b3/src/h3.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:47:17.282313 h3-4.0.0b3/src/h3lib/
--rw-r--r--   0 runner    (1001) docker     (127)    24480 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:47:17.282313 h3-4.0.0b3/src/h3lib/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/cmake/Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/cmake/TestWrapValgrind.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/cmake/toolchain.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:47:17.274314 h3-4.0.0b3/src/h3lib/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:47:17.274314 h3-4.0.0b3/src/h3lib/src/h3lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:47:17.286313 h3-4.0.0b3/src/h3lib/src/h3lib/include/
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/include/algos.h
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/include/alloc.h
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/include/baseCells.h
--rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/include/bbox.h
--rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/include/constants.h
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/include/coordijk.h
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/include/directedEdge.h
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/include/faceijk.h
--rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/include/h3Index.h
--rw-r--r--   0 runner    (1001) docker     (127)    24086 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/include/h3api.h.in
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/include/iterators.h
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/include/latLng.h
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/include/linkedGeo.h
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/include/localij.h
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/include/mathExtensions.h
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/include/polygon.h
--rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/include/polygonAlgos.h
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/include/vec2d.h
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/include/vec3d.h
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/include/vertex.h
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/include/vertexGraph.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:47:17.290313 h3-4.0.0b3/src/h3lib/src/h3lib/lib/
--rw-r--r--   0 runner    (1001) docker     (127)    44976 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/lib/algos.c
--rw-r--r--   0 runner    (1001) docker     (127)    37631 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/lib/baseCells.c
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/lib/bbox.c
--rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/lib/coordijk.c
--rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/lib/directedEdge.c
--rw-r--r--   0 runner    (1001) docker     (127)    34564 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/lib/faceijk.c
--rw-r--r--   0 runner    (1001) docker     (127)    36580 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/lib/h3Index.c
--rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/lib/iterators.c
--rw-r--r--   0 runner    (1001) docker     (127)    14183 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/lib/latLng.c
--rw-r--r--   0 runner    (1001) docker     (127)    12607 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/lib/linkedGeo.c
--rw-r--r--   0 runner    (1001) docker     (127)    26327 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/lib/localij.c
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/lib/mathExtensions.c
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/lib/polygon.c
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/lib/vec2d.c
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/lib/vec3d.c
--rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/lib/vertex.c
--rw-r--r--   0 runner    (1001) docker     (127)     7231 2024-03-12 20:47:10.000000 h3-4.0.0b3/src/h3lib/src/h3lib/lib/vertexGraph.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 20:47:17.290313 h3-4.0.0b3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    16108 2024-03-12 20:47:08.000000 h3-4.0.0b3/tests/test_cells_and_edges.py
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-03-12 20:47:08.000000 h3-4.0.0b3/tests/test_error_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9353 2024-03-12 20:47:08.000000 h3-4.0.0b3/tests/test_h3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-03-12 20:47:08.000000 h3-4.0.0b3/tests/test_length_area.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.255481 h3-4.0.0b4/
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-04-14 17:44:03.000000 h3-4.0.0b4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-14 17:44:03.000000 h3-4.0.0b4/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-14 17:44:03.000000 h3-4.0.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-14 17:44:12.255481 h3-4.0.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-14 17:44:03.000000 h3-4.0.0b4/makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-14 17:44:03.000000 h3-4.0.0b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-14 17:44:03.000000 h3-4.0.0b4/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-14 17:44:03.000000 h3-4.0.0b4/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 17:44:12.255481 h3-4.0.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-14 17:44:03.000000 h3-4.0.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.239481 h3-4.0.0b4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.239481 h3-4.0.0b4/src/h3/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.243481 h3-4.0.0b4/src/h3/_cy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/cells.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     9676 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/cells.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/edges.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/edges.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/error_system.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/error_system.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     6205 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/h3lib.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/latlng.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/latlng.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/memory.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/memory.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/to_multipoly.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/util.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     2159 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_cy/util.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     7673 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_h3shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.243481 h3-4.0.0b4/src/h3/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.243481 h3-4.0.0b4/src/h3/api/basic_int/
+-rw-r--r--   0 runner    (1001) docker     (127)    19659 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/api/basic_int/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/api/basic_int/_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.243481 h3-4.0.0b4/src/h3/api/basic_str/
+-rw-r--r--   0 runner    (1001) docker     (127)    19659 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/api/basic_str/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/api/basic_str/_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.247481 h3-4.0.0b4/src/h3/api/memview_int/
+-rw-r--r--   0 runner    (1001) docker     (127)    19659 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/api/memview_int/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/api/memview_int/_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.247481 h3-4.0.0b4/src/h3/api/numpy_int/
+-rw-r--r--   0 runner    (1001) docker     (127)    19659 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/api/numpy_int/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-14 17:44:03.000000 h3-4.0.0b4/src/h3/api/numpy_int/_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.255481 h3-4.0.0b4/src/h3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-14 17:44:12.000000 h3-4.0.0b4/src/h3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-04-14 17:44:12.000000 h3-4.0.0b4/src/h3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 17:44:12.000000 h3-4.0.0b4/src/h3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-14 17:44:12.000000 h3-4.0.0b4/src/h3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-14 17:44:12.000000 h3-4.0.0b4/src/h3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.247481 h3-4.0.0b4/src/h3lib/
+-rw-r--r--   0 runner    (1001) docker     (127)    24480 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.247481 h3-4.0.0b4/src/h3lib/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/cmake/Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/cmake/TestWrapValgrind.cmake
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/cmake/toolchain.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.239481 h3-4.0.0b4/src/h3lib/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.239481 h3-4.0.0b4/src/h3lib/src/h3lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.251481 h3-4.0.0b4/src/h3lib/src/h3lib/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/algos.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/alloc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/baseCells.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/bbox.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/constants.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/coordijk.h
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/directedEdge.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/faceijk.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5829 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/h3Index.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24086 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/h3api.h.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/iterators.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/latLng.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/linkedGeo.h
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/localij.h
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/mathExtensions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/polygon.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/polygonAlgos.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/vec2d.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/vec3d.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/vertex.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/include/vertexGraph.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.255481 h3-4.0.0b4/src/h3lib/src/h3lib/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)    44976 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/algos.c
+-rw-r--r--   0 runner    (1001) docker     (127)    37631 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/baseCells.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/bbox.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13658 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/coordijk.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/directedEdge.c
+-rw-r--r--   0 runner    (1001) docker     (127)    34564 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/faceijk.c
+-rw-r--r--   0 runner    (1001) docker     (127)    36580 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/h3Index.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11007 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/iterators.c
+-rw-r--r--   0 runner    (1001) docker     (127)    14183 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/latLng.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12607 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/linkedGeo.c
+-rw-r--r--   0 runner    (1001) docker     (127)    26327 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/localij.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/mathExtensions.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/polygon.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/vec2d.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/vec3d.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13367 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/vertex.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7231 2024-04-14 17:44:05.000000 h3-4.0.0b4/src/h3lib/src/h3lib/lib/vertexGraph.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 17:44:12.255481 h3-4.0.0b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    16108 2024-04-14 17:44:03.000000 h3-4.0.0b4/tests/test_cells_and_edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-14 17:44:03.000000 h3-4.0.0b4/tests/test_error_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9353 2024-04-14 17:44:03.000000 h3-4.0.0b4/tests/test_h3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-04-14 17:44:03.000000 h3-4.0.0b4/tests/test_length_area.py
```

### Comparing `h3-4.0.0b3/CHANGELOG.md` & `h3-4.0.0b4/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-# Versioning
+# CHANGELOG
+
+## Versioning
 
 The H3 core library adheres to [Semantic Versioning](http://semver.org/).
 H3-Py has a `major.minor.patch` version scheme. The major and minor version
 numbers of H3-Py are the major and minor version of the bound core library,
 respectively. The patch version is incremented independently of the core
 library.
 
@@ -12,14 +14,18 @@
 avoid adding features or APIs which do not map onto the
 [H3 core API](https://uber.github.io/h3/#/documentation/api-reference/).
 
 ## Unreleased
 
 - None
 
+## [4.0.0b4] - 2024-04-14
+
+No changes, just testing: #360
+
 ## [4.0.0b3] - 2024-03-11
 
 - Change supported Python versions to 3.7, 3.8, 3.9, 3.10, 3.11, 3.12 (#324, #325, #347, #348)
 - New `h3.Polygon()`/GeoJSON interface (#301)
 - Use functions instead of methods for the interface functions (#334)
 - Use `list` instead of `set` for unordered Python outputs (#339)
```

### Comparing `h3-4.0.0b3/CMakeLists.txt` & `h3-4.0.0b4/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/LICENSE` & `h3-4.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/PKG-INFO` & `h3-4.0.0b4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h3
-Version: 4.0.0b3
+Version: 4.0.0b4
 Summary: Hierarchical hexagonal geospatial indexing system
 Home-page: https://github.com/uber/h3-py
 Author: Uber Technologies
 Author-email: AJ Friend <ajfriend@gmail.com>
 License: Apache 2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -49,27 +49,29 @@
 [![conda](https://img.shields.io/conda/vn/conda-forge/h3-py.svg)](https://anaconda.org/conda-forge/h3-py)
 [![version](https://img.shields.io/badge/h3-v3.7.1-blue.svg)](https://github.com/uber/h3/releases/tag/v3.7.1)
 [![version](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/uber/h3-py/blob/master/LICENSE)
 
 [![Tests](https://github.com/uber/h3-py/workflows/tests/badge.svg)](https://github.com/uber/h3-py/actions)
 [![codecov](https://codecov.io/gh/uber/h3-py/branch/master/graph/badge.svg)](https://codecov.io/gh/uber/h3-py)
 
+
 ----
-### ANNOUNCEMENT: v4.0.0 beta released!
+## ANNOUNCEMENT: v4.0.0 beta released!
 Install the latest beta version with `pip install h3 --pre`
 or with
-`pip install 'h3==4.0.0b2'`. <br>
+`pip install 'h3==4.0.0b3'`. <br>
 Feedback is welcome via
 [Issues](https://github.com/uber/h3-py/issues/new),
 [Discussions](https://github.com/uber/h3/discussions),
 and
 [Slack](https://join.slack.com/t/h3-core/shared_invite/zt-g6u5r1hf-W_~uVJmfeiWtMQuBGc1NNg).
 
 ----
 
+
 Python bindings for the [H3 core library](https://h3geo.org/).
 
 - Documentation: [uber.github.io/h3-py](https://uber.github.io/h3-py)
 - GitHub repo: [github.com/uber/h3-py](https://github.com/uber/h3-py)
 
 ## Installation
```

### Comparing `h3-4.0.0b3/makefile` & `h3-4.0.0b4/makefile`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .PHONY: init clear rebuild purge test lint lab ipython
 
 PYTHON=$(shell command -v python || command -v python3)
 
 
 build-docs:
+	./env/bin/pip install -r requirements-dev.txt
 	./env/bin/jupyter-book build docs/ --warningiserror --keep-going --all
 
 open:
 	open docs/_build/html/index.html
 
 init: purge
 	git submodule update --init
```

### Comparing `h3-4.0.0b3/readme.md` & `h3-4.0.0b4/readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,27 +9,29 @@
 [![conda](https://img.shields.io/conda/vn/conda-forge/h3-py.svg)](https://anaconda.org/conda-forge/h3-py)
 [![version](https://img.shields.io/badge/h3-v3.7.1-blue.svg)](https://github.com/uber/h3/releases/tag/v3.7.1)
 [![version](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/uber/h3-py/blob/master/LICENSE)
 
 [![Tests](https://github.com/uber/h3-py/workflows/tests/badge.svg)](https://github.com/uber/h3-py/actions)
 [![codecov](https://codecov.io/gh/uber/h3-py/branch/master/graph/badge.svg)](https://codecov.io/gh/uber/h3-py)
 
+
 ----
-### ANNOUNCEMENT: v4.0.0 beta released!
+## ANNOUNCEMENT: v4.0.0 beta released!
 Install the latest beta version with `pip install h3 --pre`
 or with
-`pip install 'h3==4.0.0b2'`. <br>
+`pip install 'h3==4.0.0b3'`. <br>
 Feedback is welcome via
 [Issues](https://github.com/uber/h3-py/issues/new),
 [Discussions](https://github.com/uber/h3/discussions),
 and
 [Slack](https://join.slack.com/t/h3-core/shared_invite/zt-g6u5r1hf-W_~uVJmfeiWtMQuBGc1NNg).
 
 ----
 
+
 Python bindings for the [H3 core library](https://h3geo.org/).
 
 - Documentation: [uber.github.io/h3-py](https://uber.github.io/h3-py)
 - GitHub repo: [github.com/uber/h3-py](https://github.com/uber/h3-py)
 
 ## Installation
```

### Comparing `h3-4.0.0b3/setup.py` & `h3-4.0.0b4/setup.py`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3/__init__.py` & `h3-4.0.0b4/src/h3/__init__.py`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3/_cy/CMakeLists.txt` & `h3-4.0.0b4/src/h3/_cy/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3/_cy/__init__.py` & `h3-4.0.0b4/src/h3/_cy/__init__.py`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3/_cy/cells.pxd` & `h3-4.0.0b4/src/h3/_cy/cells.pxd`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3/_cy/cells.pyx` & `h3-4.0.0b4/src/h3/_cy/cells.pyx`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3/_cy/edges.pxd` & `h3-4.0.0b4/src/h3/_cy/edges.pxd`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3/_cy/edges.pyx` & `h3-4.0.0b4/src/h3/_cy/edges.pyx`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3/_cy/error_system.pyx` & `h3-4.0.0b4/src/h3/_cy/error_system.pyx`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3/_cy/h3lib.pxd` & `h3-4.0.0b4/src/h3/_cy/h3lib.pxd`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3/_cy/latlng.pyx` & `h3-4.0.0b4/src/h3/_cy/latlng.pyx`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3/_cy/memory.pyx` & `h3-4.0.0b4/src/h3/_cy/memory.pyx`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3/_cy/to_multipoly.pyx` & `h3-4.0.0b4/src/h3/_cy/to_multipoly.pyx`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3/_cy/util.pyx` & `h3-4.0.0b4/src/h3/_cy/util.pyx`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3/_h3shape.py` & `h3-4.0.0b4/src/h3/_h3shape.py`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3/_version.py` & `h3-4.0.0b4/src/h3/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '4.0.0b3'
+__version__ = '4.0.0b4'
 __description__ = 'Hierarchical hexagonal geospatial indexing system'
 __url__ = 'https://github.com/uber/h3-py'
 __license__ = 'Apache 2.0 License'
 __author__ = 'Uber Technologies'
 __author_email__ = 'AJ Friend <ajfriend@gmail.com>'
 __classifiers__ = [
     'Development Status :: 5 - Production/Stable',
```

### Comparing `h3-4.0.0b3/src/h3/api/basic_int/__init__.py` & `h3-4.0.0b4/src/h3/api/basic_int/__init__.py`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3/api/basic_str/__init__.py` & `h3-4.0.0b4/src/h3/api/basic_str/__init__.py`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3/api/memview_int/__init__.py` & `h3-4.0.0b4/src/h3/api/memview_int/__init__.py`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3/api/numpy_int/__init__.py` & `h3-4.0.0b4/src/h3/api/numpy_int/__init__.py`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3.egg-info/PKG-INFO` & `h3-4.0.0b4/src/h3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h3
-Version: 4.0.0b3
+Version: 4.0.0b4
 Summary: Hierarchical hexagonal geospatial indexing system
 Home-page: https://github.com/uber/h3-py
 Author: Uber Technologies
 Author-email: AJ Friend <ajfriend@gmail.com>
 License: Apache 2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -49,27 +49,29 @@
 [![conda](https://img.shields.io/conda/vn/conda-forge/h3-py.svg)](https://anaconda.org/conda-forge/h3-py)
 [![version](https://img.shields.io/badge/h3-v3.7.1-blue.svg)](https://github.com/uber/h3/releases/tag/v3.7.1)
 [![version](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://github.com/uber/h3-py/blob/master/LICENSE)
 
 [![Tests](https://github.com/uber/h3-py/workflows/tests/badge.svg)](https://github.com/uber/h3-py/actions)
 [![codecov](https://codecov.io/gh/uber/h3-py/branch/master/graph/badge.svg)](https://codecov.io/gh/uber/h3-py)
 
+
 ----
-### ANNOUNCEMENT: v4.0.0 beta released!
+## ANNOUNCEMENT: v4.0.0 beta released!
 Install the latest beta version with `pip install h3 --pre`
 or with
-`pip install 'h3==4.0.0b2'`. <br>
+`pip install 'h3==4.0.0b3'`. <br>
 Feedback is welcome via
 [Issues](https://github.com/uber/h3-py/issues/new),
 [Discussions](https://github.com/uber/h3/discussions),
 and
 [Slack](https://join.slack.com/t/h3-core/shared_invite/zt-g6u5r1hf-W_~uVJmfeiWtMQuBGc1NNg).
 
 ----
 
+
 Python bindings for the [H3 core library](https://h3geo.org/).
 
 - Documentation: [uber.github.io/h3-py](https://uber.github.io/h3-py)
 - GitHub repo: [github.com/uber/h3-py](https://github.com/uber/h3-py)
 
 ## Installation
```

### Comparing `h3-4.0.0b3/src/h3.egg-info/SOURCES.txt` & `h3-4.0.0b4/src/h3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/CMakeLists.txt` & `h3-4.0.0b4/src/h3lib/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/LICENSE` & `h3-4.0.0b4/src/h3lib/LICENSE`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/README.md` & `h3-4.0.0b4/src/h3lib/README.md`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/cmake/TestWrapValgrind.cmake` & `h3-4.0.0b4/src/h3lib/cmake/TestWrapValgrind.cmake`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/cmake/toolchain.cmake` & `h3-4.0.0b4/src/h3lib/cmake/toolchain.cmake`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/include/algos.h` & `h3-4.0.0b4/src/h3lib/src/h3lib/include/algos.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/include/alloc.h` & `h3-4.0.0b4/src/h3lib/src/h3lib/include/alloc.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/include/baseCells.h` & `h3-4.0.0b4/src/h3lib/src/h3lib/include/baseCells.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/include/bbox.h` & `h3-4.0.0b4/src/h3lib/src/h3lib/include/bbox.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/include/constants.h` & `h3-4.0.0b4/src/h3lib/src/h3lib/include/constants.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/include/coordijk.h` & `h3-4.0.0b4/src/h3lib/src/h3lib/include/coordijk.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/include/directedEdge.h` & `h3-4.0.0b4/src/h3lib/src/h3lib/include/directedEdge.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/include/faceijk.h` & `h3-4.0.0b4/src/h3lib/src/h3lib/include/faceijk.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/include/h3Index.h` & `h3-4.0.0b4/src/h3lib/src/h3lib/include/h3Index.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/include/h3api.h.in` & `h3-4.0.0b4/src/h3lib/src/h3lib/include/h3api.h.in`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/include/iterators.h` & `h3-4.0.0b4/src/h3lib/src/h3lib/include/iterators.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/include/latLng.h` & `h3-4.0.0b4/src/h3lib/src/h3lib/include/latLng.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/include/linkedGeo.h` & `h3-4.0.0b4/src/h3lib/src/h3lib/include/linkedGeo.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/include/localij.h` & `h3-4.0.0b4/src/h3lib/src/h3lib/include/localij.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/include/mathExtensions.h` & `h3-4.0.0b4/src/h3lib/src/h3lib/include/mathExtensions.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/include/polygon.h` & `h3-4.0.0b4/src/h3lib/src/h3lib/include/polygon.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/include/polygonAlgos.h` & `h3-4.0.0b4/src/h3lib/src/h3lib/include/polygonAlgos.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/include/vec2d.h` & `h3-4.0.0b4/src/h3lib/src/h3lib/include/vec2d.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/include/vec3d.h` & `h3-4.0.0b4/src/h3lib/src/h3lib/include/vec3d.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/include/vertex.h` & `h3-4.0.0b4/src/h3lib/src/h3lib/include/vertex.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/include/vertexGraph.h` & `h3-4.0.0b4/src/h3lib/src/h3lib/include/vertexGraph.h`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/lib/algos.c` & `h3-4.0.0b4/src/h3lib/src/h3lib/lib/algos.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/lib/baseCells.c` & `h3-4.0.0b4/src/h3lib/src/h3lib/lib/baseCells.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/lib/bbox.c` & `h3-4.0.0b4/src/h3lib/src/h3lib/lib/bbox.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/lib/coordijk.c` & `h3-4.0.0b4/src/h3lib/src/h3lib/lib/coordijk.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/lib/directedEdge.c` & `h3-4.0.0b4/src/h3lib/src/h3lib/lib/directedEdge.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/lib/faceijk.c` & `h3-4.0.0b4/src/h3lib/src/h3lib/lib/faceijk.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/lib/h3Index.c` & `h3-4.0.0b4/src/h3lib/src/h3lib/lib/h3Index.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/lib/iterators.c` & `h3-4.0.0b4/src/h3lib/src/h3lib/lib/iterators.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/lib/latLng.c` & `h3-4.0.0b4/src/h3lib/src/h3lib/lib/latLng.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/lib/linkedGeo.c` & `h3-4.0.0b4/src/h3lib/src/h3lib/lib/linkedGeo.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/lib/localij.c` & `h3-4.0.0b4/src/h3lib/src/h3lib/lib/localij.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/lib/mathExtensions.c` & `h3-4.0.0b4/src/h3lib/src/h3lib/lib/mathExtensions.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/lib/polygon.c` & `h3-4.0.0b4/src/h3lib/src/h3lib/lib/polygon.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/lib/vec2d.c` & `h3-4.0.0b4/src/h3lib/src/h3lib/lib/vec2d.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/lib/vec3d.c` & `h3-4.0.0b4/src/h3lib/src/h3lib/lib/vec3d.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/lib/vertex.c` & `h3-4.0.0b4/src/h3lib/src/h3lib/lib/vertex.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/src/h3lib/src/h3lib/lib/vertexGraph.c` & `h3-4.0.0b4/src/h3lib/src/h3lib/lib/vertexGraph.c`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/tests/test_cells_and_edges.py` & `h3-4.0.0b4/tests/test_cells_and_edges.py`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/tests/test_error_codes.py` & `h3-4.0.0b4/tests/test_error_codes.py`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/tests/test_h3.py` & `h3-4.0.0b4/tests/test_h3.py`

 * *Files identical despite different names*

### Comparing `h3-4.0.0b3/tests/test_length_area.py` & `h3-4.0.0b4/tests/test_length_area.py`

 * *Files identical despite different names*

