# Comparing `tmp/librecell-layout-0.0.8.tar.gz` & `tmp/librecell-layout-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/librecell-layout-0.0.8.tar", last modified: Wed Dec 30 17:35:42 2020, max compression
+gzip compressed data, was "dist/librecell-layout-0.0.9.tar", last modified: Wed Dec 30 17:45:38 2020, max compression
```

## Comparing `librecell-layout-0.0.8.tar` & `librecell-layout-0.0.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:35:42.000000 librecell-layout-0.0.8/
--rw-r--r--   0 kramert   (1000) kramert   (1000)     1574 2020-12-30 17:35:42.000000 librecell-layout-0.0.8/PKG-INFO
--rw-r--r--   0 kramert   (1000) kramert   (1000)      841 2019-10-05 16:43:05.000000 librecell-layout-0.0.8/README.md
-drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:35:42.000000 librecell-layout-0.0.8/lclayout/
--rw-r--r--   0 kramert   (1000) kramert   (1000)      552 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/__init__.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     3478 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/data_types.py
-drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:35:42.000000 librecell-layout-0.0.8/lclayout/drc_cleaner/
--rw-r--r--   0 kramert   (1000) kramert   (1000)      552 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/drc_cleaner/__init__.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)    19867 2020-12-10 17:57:02.000000 librecell-layout-0.0.8/lclayout/drc_cleaner/base.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)    18329 2020-12-10 17:57:02.000000 librecell-layout-0.0.8/lclayout/drc_cleaner/drc_cleaner.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     2957 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/drc_cleaner/drc_theorem_proofs.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     3133 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/drc_cleaner/standalone.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     1621 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/extrema.py
-drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:35:42.000000 librecell-layout-0.0.8/lclayout/graphrouter/
--rw-r--r--   0 kramert   (1000) kramert   (1000)      552 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/graphrouter/__init__.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     1695 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/graphrouter/graphrouter.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     8929 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/graphrouter/hv_router.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)    14183 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/graphrouter/lp_router.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     2043 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/graphrouter/min_area_router.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     3264 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/graphrouter/multi_via_router.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)    14846 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/graphrouter/pathfinder.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     2250 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/graphrouter/pyo3_graphrouter.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)    14550 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/graphrouter/signal_router.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)    10772 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/graphrouter/smt_router.py
-drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:35:42.000000 librecell-layout-0.0.8/lclayout/layout/
--rw-r--r--   0 kramert   (1000) kramert   (1000)      552 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/layout/__init__.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     2174 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/layout/cell_template.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     2296 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/layout/geometry_helpers.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     5959 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/layout/grid.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     1025 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/layout/grid_helpers.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     4685 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/layout/layers.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     1479 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/layout/notch_removal.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     8878 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/layout/transistor.py
-drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:35:42.000000 librecell-layout-0.0.8/lclayout/lef/
--rw-r--r--   0 kramert   (1000) kramert   (1000)      552 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/lef/__init__.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     9801 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/lef/types.py
-drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:35:42.000000 librecell-layout-0.0.8/lclayout/lvs/
--rw-r--r--   0 kramert   (1000) kramert   (1000)      552 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/lvs/__init__.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     7816 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/lvs/lvs.py
-drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:35:42.000000 librecell-layout-0.0.8/lclayout/place/
--rw-r--r--   0 kramert   (1000) kramert   (1000)      552 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/place/__init__.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)    23858 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/place/euler_placer.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     6965 2020-12-10 17:57:02.000000 librecell-layout-0.0.8/lclayout/place/eulertours.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     1762 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/place/partition.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)      712 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/place/place.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     8772 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/place/smt_placer.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)    15668 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/routing_graph.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)    32493 2020-11-29 12:06:00.000000 librecell-layout-0.0.8/lclayout/standalone.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     1474 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/tech_util.py
-drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:35:42.000000 librecell-layout-0.0.8/lclayout/writer/
--rw-r--r--   0 kramert   (1000) kramert   (1000)      552 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/writer/__init__.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     2016 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/writer/gds_writer.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     7358 2020-12-10 17:57:02.000000 librecell-layout-0.0.8/lclayout/writer/lef_writer.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     8481 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/writer/magic_writer.py
--rw-r--r--   0 kramert   (1000) kramert   (1000)     2556 2020-07-09 17:09:02.000000 librecell-layout-0.0.8/lclayout/writer/writer.py
-drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:35:42.000000 librecell-layout-0.0.8/librecell_layout.egg-info/
--rw-r--r--   0 kramert   (1000) kramert   (1000)     1574 2020-12-30 17:35:42.000000 librecell-layout-0.0.8/librecell_layout.egg-info/PKG-INFO
--rw-r--r--   0 kramert   (1000) kramert   (1000)     1625 2020-12-30 17:35:42.000000 librecell-layout-0.0.8/librecell_layout.egg-info/SOURCES.txt
--rw-r--r--   0 kramert   (1000) kramert   (1000)        1 2020-12-30 17:35:42.000000 librecell-layout-0.0.8/librecell_layout.egg-info/dependency_links.txt
--rw-r--r--   0 kramert   (1000) kramert   (1000)       55 2020-12-30 17:35:42.000000 librecell-layout-0.0.8/librecell_layout.egg-info/entry_points.txt
--rw-r--r--   0 kramert   (1000) kramert   (1000)        1 2019-10-11 19:52:20.000000 librecell-layout-0.0.8/librecell_layout.egg-info/not-zip-safe
--rw-r--r--   0 kramert   (1000) kramert   (1000)      158 2020-12-30 17:35:42.000000 librecell-layout-0.0.8/librecell_layout.egg-info/requires.txt
--rw-r--r--   0 kramert   (1000) kramert   (1000)        9 2020-12-30 17:35:42.000000 librecell-layout-0.0.8/librecell_layout.egg-info/top_level.txt
--rw-r--r--   0 kramert   (1000) kramert   (1000)       38 2020-12-30 17:35:42.000000 librecell-layout-0.0.8/setup.cfg
--rw-r--r--   0 kramert   (1000) kramert   (1000)     2084 2020-12-30 17:33:04.000000 librecell-layout-0.0.8/setup.py
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:45:38.000000 librecell-layout-0.0.9/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     1574 2020-12-30 17:45:38.000000 librecell-layout-0.0.9/PKG-INFO
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      841 2019-10-05 16:43:05.000000 librecell-layout-0.0.9/README.md
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:45:38.000000 librecell-layout-0.0.9/lclayout/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      552 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/__init__.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     3478 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/data_types.py
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:45:38.000000 librecell-layout-0.0.9/lclayout/drc_cleaner/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      552 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/drc_cleaner/__init__.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)    19867 2020-12-10 17:57:02.000000 librecell-layout-0.0.9/lclayout/drc_cleaner/base.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)    18329 2020-12-10 17:57:02.000000 librecell-layout-0.0.9/lclayout/drc_cleaner/drc_cleaner.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     2957 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/drc_cleaner/drc_theorem_proofs.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     3133 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/drc_cleaner/standalone.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     1621 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/extrema.py
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:45:38.000000 librecell-layout-0.0.9/lclayout/graphrouter/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      552 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/graphrouter/__init__.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     1695 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/graphrouter/graphrouter.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     8929 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/graphrouter/hv_router.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)    14183 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/graphrouter/lp_router.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     2043 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/graphrouter/min_area_router.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     3264 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/graphrouter/multi_via_router.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)    14846 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/graphrouter/pathfinder.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     2250 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/graphrouter/pyo3_graphrouter.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)    14550 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/graphrouter/signal_router.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)    10772 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/graphrouter/smt_router.py
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:45:38.000000 librecell-layout-0.0.9/lclayout/layout/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      552 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/layout/__init__.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     2174 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/layout/cell_template.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     2296 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/layout/geometry_helpers.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     5959 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/layout/grid.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     1025 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/layout/grid_helpers.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     4685 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/layout/layers.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     1479 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/layout/notch_removal.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     8878 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/layout/transistor.py
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:45:38.000000 librecell-layout-0.0.9/lclayout/lef/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      552 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/lef/__init__.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     9801 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/lef/types.py
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:45:38.000000 librecell-layout-0.0.9/lclayout/lvs/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      552 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/lvs/__init__.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     7816 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/lvs/lvs.py
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:45:38.000000 librecell-layout-0.0.9/lclayout/place/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      552 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/place/__init__.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)    23858 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/place/euler_placer.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     6965 2020-12-10 17:57:02.000000 librecell-layout-0.0.9/lclayout/place/eulertours.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     1762 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/place/partition.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      712 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/place/place.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     8772 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/place/smt_placer.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)    15668 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/routing_graph.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)    32493 2020-11-29 12:06:00.000000 librecell-layout-0.0.9/lclayout/standalone.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     1474 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/tech_util.py
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:45:38.000000 librecell-layout-0.0.9/lclayout/writer/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      552 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/writer/__init__.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     2016 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/writer/gds_writer.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     7358 2020-12-10 17:57:02.000000 librecell-layout-0.0.9/lclayout/writer/lef_writer.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     8481 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/writer/magic_writer.py
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     2556 2020-07-09 17:09:02.000000 librecell-layout-0.0.9/lclayout/writer/writer.py
+drwxr-xr-x   0 kramert   (1000) kramert   (1000)        0 2020-12-30 17:45:38.000000 librecell-layout-0.0.9/librecell_layout.egg-info/
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     1574 2020-12-30 17:45:38.000000 librecell-layout-0.0.9/librecell_layout.egg-info/PKG-INFO
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     1625 2020-12-30 17:45:38.000000 librecell-layout-0.0.9/librecell_layout.egg-info/SOURCES.txt
+-rw-r--r--   0 kramert   (1000) kramert   (1000)        1 2020-12-30 17:45:38.000000 librecell-layout-0.0.9/librecell_layout.egg-info/dependency_links.txt
+-rw-r--r--   0 kramert   (1000) kramert   (1000)       55 2020-12-30 17:45:38.000000 librecell-layout-0.0.9/librecell_layout.egg-info/entry_points.txt
+-rw-r--r--   0 kramert   (1000) kramert   (1000)        1 2019-10-11 19:52:20.000000 librecell-layout-0.0.9/librecell_layout.egg-info/not-zip-safe
+-rw-r--r--   0 kramert   (1000) kramert   (1000)      158 2020-12-30 17:45:38.000000 librecell-layout-0.0.9/librecell_layout.egg-info/requires.txt
+-rw-r--r--   0 kramert   (1000) kramert   (1000)        9 2020-12-30 17:45:38.000000 librecell-layout-0.0.9/librecell_layout.egg-info/top_level.txt
+-rw-r--r--   0 kramert   (1000) kramert   (1000)       38 2020-12-30 17:45:38.000000 librecell-layout-0.0.9/setup.cfg
+-rw-r--r--   0 kramert   (1000) kramert   (1000)     2084 2020-12-30 17:44:08.000000 librecell-layout-0.0.9/setup.py
```

### Comparing `librecell-layout-0.0.8/PKG-INFO` & `librecell-layout-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: librecell-layout
-Version: 0.0.8
+Version: 0.0.9
 Summary: CMOS standard cell layout generator.
 Home-page: https://codeberg.org/tok/librecell
 Author: T. Kramer
 Author-email: code@tkramer.ch
 License: OHL-S v2.0
 Description: # LibreCell - Layout
         CMOS Standard Cell layout generator.
```

### Comparing `librecell-layout-0.0.8/README.md` & `librecell-layout-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/__init__.py` & `librecell-layout-0.0.9/lclayout/__init__.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/data_types.py` & `librecell-layout-0.0.9/lclayout/data_types.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/drc_cleaner/__init__.py` & `librecell-layout-0.0.9/lclayout/drc_cleaner/__init__.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/drc_cleaner/base.py` & `librecell-layout-0.0.9/lclayout/drc_cleaner/base.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/drc_cleaner/drc_cleaner.py` & `librecell-layout-0.0.9/lclayout/drc_cleaner/drc_cleaner.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/drc_cleaner/drc_theorem_proofs.py` & `librecell-layout-0.0.9/lclayout/drc_cleaner/drc_theorem_proofs.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/drc_cleaner/standalone.py` & `librecell-layout-0.0.9/lclayout/drc_cleaner/standalone.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/extrema.py` & `librecell-layout-0.0.9/lclayout/extrema.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/graphrouter/__init__.py` & `librecell-layout-0.0.9/lclayout/graphrouter/__init__.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/graphrouter/graphrouter.py` & `librecell-layout-0.0.9/lclayout/graphrouter/graphrouter.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/graphrouter/hv_router.py` & `librecell-layout-0.0.9/lclayout/graphrouter/hv_router.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/graphrouter/lp_router.py` & `librecell-layout-0.0.9/lclayout/graphrouter/lp_router.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/graphrouter/min_area_router.py` & `librecell-layout-0.0.9/lclayout/graphrouter/min_area_router.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/graphrouter/multi_via_router.py` & `librecell-layout-0.0.9/lclayout/graphrouter/multi_via_router.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/graphrouter/pathfinder.py` & `librecell-layout-0.0.9/lclayout/graphrouter/pathfinder.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/graphrouter/pyo3_graphrouter.py` & `librecell-layout-0.0.9/lclayout/graphrouter/pyo3_graphrouter.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/graphrouter/signal_router.py` & `librecell-layout-0.0.9/lclayout/graphrouter/signal_router.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/graphrouter/smt_router.py` & `librecell-layout-0.0.9/lclayout/graphrouter/smt_router.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/layout/__init__.py` & `librecell-layout-0.0.9/lclayout/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/layout/cell_template.py` & `librecell-layout-0.0.9/lclayout/layout/cell_template.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/layout/geometry_helpers.py` & `librecell-layout-0.0.9/lclayout/layout/geometry_helpers.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/layout/grid.py` & `librecell-layout-0.0.9/lclayout/layout/grid.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/layout/grid_helpers.py` & `librecell-layout-0.0.9/lclayout/layout/grid_helpers.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/layout/layers.py` & `librecell-layout-0.0.9/lclayout/layout/layers.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/layout/notch_removal.py` & `librecell-layout-0.0.9/lclayout/layout/notch_removal.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/layout/transistor.py` & `librecell-layout-0.0.9/lclayout/layout/transistor.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/lef/__init__.py` & `librecell-layout-0.0.9/lclayout/lef/__init__.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/lef/types.py` & `librecell-layout-0.0.9/lclayout/lef/types.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/lvs/__init__.py` & `librecell-layout-0.0.9/lclayout/lvs/__init__.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/lvs/lvs.py` & `librecell-layout-0.0.9/lclayout/lvs/lvs.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/place/__init__.py` & `librecell-layout-0.0.9/lclayout/place/__init__.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/place/euler_placer.py` & `librecell-layout-0.0.9/lclayout/place/euler_placer.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/place/eulertours.py` & `librecell-layout-0.0.9/lclayout/place/eulertours.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/place/partition.py` & `librecell-layout-0.0.9/lclayout/place/partition.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/place/place.py` & `librecell-layout-0.0.9/lclayout/place/place.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/place/smt_placer.py` & `librecell-layout-0.0.9/lclayout/place/smt_placer.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/routing_graph.py` & `librecell-layout-0.0.9/lclayout/routing_graph.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/standalone.py` & `librecell-layout-0.0.9/lclayout/standalone.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/tech_util.py` & `librecell-layout-0.0.9/lclayout/tech_util.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/writer/__init__.py` & `librecell-layout-0.0.9/lclayout/writer/__init__.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/writer/gds_writer.py` & `librecell-layout-0.0.9/lclayout/writer/gds_writer.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/writer/lef_writer.py` & `librecell-layout-0.0.9/lclayout/writer/lef_writer.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/writer/magic_writer.py` & `librecell-layout-0.0.9/lclayout/writer/magic_writer.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/lclayout/writer/writer.py` & `librecell-layout-0.0.9/lclayout/writer/writer.py`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/librecell_layout.egg-info/PKG-INFO` & `librecell-layout-0.0.9/librecell_layout.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: librecell-layout
-Version: 0.0.8
+Version: 0.0.9
 Summary: CMOS standard cell layout generator.
 Home-page: https://codeberg.org/tok/librecell
 Author: T. Kramer
 Author-email: code@tkramer.ch
 License: OHL-S v2.0
 Description: # LibreCell - Layout
         CMOS Standard Cell layout generator.
```

### Comparing `librecell-layout-0.0.8/librecell_layout.egg-info/SOURCES.txt` & `librecell-layout-0.0.9/librecell_layout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `librecell-layout-0.0.8/setup.py` & `librecell-layout-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 def readme():
     with open("README.md", "r") as f:
         return f.read()
 
 
 setup(name='librecell-layout',
-      version='0.0.8',
+      version='0.0.9',
       description='CMOS standard cell layout generator.',
       long_description=readme(),
       long_description_content_type="text/markdown",
       keywords='cmos cell generator layout klayout vlsi asic',
       classifiers=[
           # 'License :: OSI Approved :: GNU Affero General Public License v3',
           'Development Status :: 3 - Alpha',
@@ -41,15 +41,15 @@
       entry_points={
           'console_scripts': [
               'lclayout = lclayout.standalone:main',
               # 'drc_cleaner = lclayout.drc_cleaner.standalone:main',
           ]
       },
       install_requires=[
-          'librecell-common==0.0.7',
+          'librecell-common>=0.0.9',
           'toml==0.10.*',
           'klayout==0.26.*',  # GPLv3
           'numpy==1.*',  # BSD
           'networkx==2.5',  # BSD
           'pyspice==1.4.3',  # GPLv3
           'scipy>=1.5.*',  # BSD
           'liberty-parser==0.0.8',  # GPLv3
```

