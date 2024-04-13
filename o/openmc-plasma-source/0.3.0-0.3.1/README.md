# Comparing `tmp/openmc_plasma_source-0.3.0.tar.gz` & `tmp/openmc_plasma_source-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmc_plasma_source-0.3.0.tar", last modified: Fri Dec  1 14:54:12 2023, max compression
+gzip compressed data, was "openmc_plasma_source-0.3.1.tar", last modified: Sat Apr 13 22:38:58 2024, max compression
```

## Comparing `openmc_plasma_source-0.3.0.tar` & `openmc_plasma_source-0.3.1.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 14:54:12.811833 openmc_plasma_source-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 14:54:12.807833 openmc_plasma_source-0.3.0/.circleci/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/.circleci/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 14:54:12.803833 openmc_plasma_source-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 14:54:12.807833 openmc_plasma_source-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      971 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/.github/workflows/anaconda-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      606 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (127)      702 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      589 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2023-12-01 14:54:12.811833 openmc_plasma_source-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 14:54:12.807833 openmc_plasma_source-0.3.0/conda/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/conda/conda_build_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/conda/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 14:54:12.807833 openmc_plasma_source-0.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/examples/point_source_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/examples/ring_source_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/examples/tokamak_source_example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 14:54:12.807833 openmc_plasma_source-0.3.0/openmc_plasma_source/
--rw-r--r--   0 runner    (1001) docker     (127)      525 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/openmc_plasma_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-01 14:54:12.000000 openmc_plasma_source-0.3.0/openmc_plasma_source/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/openmc_plasma_source/fuel_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 14:54:12.807833 openmc_plasma_source-0.3.0/openmc_plasma_source/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/openmc_plasma_source/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/openmc_plasma_source/plotting/plot_tokamak_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/openmc_plasma_source/point_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/openmc_plasma_source/ring_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    15712 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/openmc_plasma_source/tokamak_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 14:54:12.811833 openmc_plasma_source-0.3.0/openmc_plasma_source.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2023-12-01 14:54:12.000000 openmc_plasma_source-0.3.0/openmc_plasma_source.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2023-12-01 14:54:12.000000 openmc_plasma_source-0.3.0/openmc_plasma_source.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-01 14:54:12.000000 openmc_plasma_source-0.3.0/openmc_plasma_source.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-01 14:54:12.000000 openmc_plasma_source-0.3.0/openmc_plasma_source.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-12-01 14:54:12.000000 openmc_plasma_source-0.3.0/openmc_plasma_source.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2023-12-01 14:54:12.811833 openmc_plasma_source-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-01 14:54:12.811833 openmc_plasma_source-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/tests/test_fuel_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9478 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/tests/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/tests/test_point_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/tests/test_ring_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    13749 2023-12-01 14:53:57.000000 openmc_plasma_source-0.3.0/tests/test_tokamak_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:38:58.979075 openmc_plasma_source-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:38:58.971075 openmc_plasma_source-0.3.1/.circleci/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/.circleci/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:38:58.971075 openmc_plasma_source-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:38:58.971075 openmc_plasma_source-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/.github/workflows/anaconda-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-13 22:38:58.979075 openmc_plasma_source-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:38:58.971075 openmc_plasma_source-0.3.1/conda/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/conda/conda_build_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/conda/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:38:58.975075 openmc_plasma_source-0.3.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/examples/cross_sections.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/examples/point_source_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/examples/ring_source_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/examples/tokamak_source_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 22:38:58.979075 openmc_plasma_source-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:38:58.975075 openmc_plasma_source-0.3.1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-13 22:38:58.000000 openmc_plasma_source-0.3.1/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:38:58.975075 openmc_plasma_source-0.3.1/src/openmc_plasma_source/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/src/openmc_plasma_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/src/openmc_plasma_source/fuel_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:38:58.975075 openmc_plasma_source-0.3.1/src/openmc_plasma_source/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/src/openmc_plasma_source/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/src/openmc_plasma_source/plotting/plot_tokamak_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/src/openmc_plasma_source/point_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/src/openmc_plasma_source/ring_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16037 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/src/openmc_plasma_source/tokamak_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:38:58.975075 openmc_plasma_source-0.3.1/src/openmc_plasma_source.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-04-13 22:38:58.000000 openmc_plasma_source-0.3.1/src/openmc_plasma_source.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-04-13 22:38:58.000000 openmc_plasma_source-0.3.1/src/openmc_plasma_source.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 22:38:58.000000 openmc_plasma_source-0.3.1/src/openmc_plasma_source.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-13 22:38:58.000000 openmc_plasma_source-0.3.1/src/openmc_plasma_source.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-13 22:38:58.000000 openmc_plasma_source-0.3.1/src/openmc_plasma_source.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 22:38:58.975075 openmc_plasma_source-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/tests/test_fuel_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9478 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/tests/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/tests/test_point_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/tests/test_ring_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13752 2024-04-13 22:38:54.000000 openmc_plasma_source-0.3.1/tests/test_tokamak_source.py
```

### Comparing `openmc_plasma_source-0.3.0/.circleci/config.yml` & `openmc_plasma_source-0.3.1/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `openmc_plasma_source-0.3.0/.github/workflows/anaconda-publish.yml` & `openmc_plasma_source-0.3.1/.github/workflows/anaconda-publish.yml`

 * *Files identical despite different names*

### Comparing `openmc_plasma_source-0.3.0/.github/workflows/black.yml` & `openmc_plasma_source-0.3.1/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `openmc_plasma_source-0.3.0/.gitignore` & `openmc_plasma_source-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `openmc_plasma_source-0.3.0/CITATION.cff` & `openmc_plasma_source-0.3.1/CITATION.cff`

 * *Files 26% similar despite different names*

```diff
@@ -10,10 +10,10 @@
 - family-names: "Pattinson"
   given-names: "Liam"
 - family-names: "Pranto"
   given-names: "Ariful Islam"
 - family-names: "Faisal"
   given-names: "Mohammed"
 title: "OpenMC Plasma Source"
-version: 0.2.4
-date-released: 2022-01-31
+version: 0.3.0
+date-released: 2023-01-12
 url: "https://github.com/fusion-energy/openmc-plasma-source"
```

### Comparing `openmc_plasma_source-0.3.0/LICENSE.txt` & `openmc_plasma_source-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `openmc_plasma_source-0.3.0/PKG-INFO` & `openmc_plasma_source-0.3.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 Metadata-Version: 2.1
 Name: openmc_plasma_source
-Version: 0.3.0
-Summary: Creates tokamak plasma sources for OpenMC
-Home-page: https://github.com/fusion-energy/openmc-plasma-source
-Author: The openmc-plasma-source Development Team
-Author-email: rdelaportemathurin@gmail.com
-License: MIT
-Project-URL: Source, https://github.com/fusion-energy/openmc-plasma-source
-Project-URL: Tracker, https://github.com/fusion-energy/openmc-plasma-source/issues
-Classifier: Natural Language :: English
-Classifier: Topic :: Scientific/Engineering
+Version: 0.3.1
+Summary: Creates tokamak and ICF plasma sources for OpenMC
+Author: Rémi Delaporte-Mathurin
+Project-URL: Homepage, https://github.com/fusion-energy/openmc-plasma-source
+Project-URL: Bug Tracker, https://github.com/fusion-energy/openmc-plasma-source/issues
+Keywords: python,neutron,fusion,source,openmc,energy,tokamak
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy>=1.9
 Requires-Dist: matplotlib>=3.2.2
-Requires-Dist: importlib-metadata; python_version < "3.8"
 Provides-Extra: tests
 Requires-Dist: pytest>=5.4.3; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 
 [![CircleCI](https://circleci.com/gh/fusion-energy/openmc-plasma-source/tree/main.svg?style=svg)](https://circleci.com/gh/fusion-energy/openmc-plasma-source/tree/main) [![codecov](https://codecov.io/gh/fusion-energy/openmc-plasma-source/branch/main/graph/badge.svg?token=kDvWo6NGue)](https://codecov.io/gh/fusion-energy/openmc-plasma-source) [![PyPI version](https://badge.fury.io/py/openmc-plasma-source.svg)](https://badge.fury.io/py/openmc-plasma-source)
 
 # OpenMC-plasma-source
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openmc_plasma_source-0.3.0/README.md` & `openmc_plasma_source-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `openmc_plasma_source-0.3.0/conda/meta.yaml` & `openmc_plasma_source-0.3.1/conda/meta.yaml`

 * *Files identical despite different names*

### Comparing `openmc_plasma_source-0.3.0/examples/tokamak_source_example.py` & `openmc_plasma_source-0.3.1/examples/tokamak_source_example.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,19 @@
+from pathlib import Path
 import openmc
 from openmc_plasma_source import TokamakSource
 
+# just making use of a local cross section xml file, replace with your own cross sections or comment out
+openmc.config["cross_sections"] = Path(__file__).parent.resolve() / "cross_sections.xml"
+
+
+# minimal geometry
+sphere_surface = openmc.Sphere(r=1000.0, boundary_type="vacuum")
+cell = openmc.Cell(region=-sphere_surface)
+geometry = openmc.Geometry([cell])
 
 # create a plasma source
 my_plasma = TokamakSource(
     elongation=1.557,
     ion_density_centre=1.09e20,
     ion_density_peaking_factor=1,
     ion_density_pedestal=1.09e20,
@@ -18,47 +27,18 @@
     pedestal_radius=0.8 * 2.92258,
     mode="H",
     shafranov_factor=0.44789,
     triangularity=0.270,
     ion_temperature_beta=6,
 )
 
-
-# Create a single material
-iron = openmc.Material()
-iron.set_density("g/cm3", 5.0)
-iron.add_element("Fe", 1.0)
-mats = openmc.Materials([iron])
-
-# Create a 5 cm x 5 cm box filled with iron
-cells = []
-inner_box1 = openmc.ZCylinder(r=600.0)
-inner_box2 = openmc.ZCylinder(r=1400.0)
-outer_box = openmc.model.rectangular_prism(4000.0, 4000.0, boundary_type="vacuum")
-cells += [openmc.Cell(fill=iron, region=-inner_box1)]
-cells += [openmc.Cell(fill=None, region=+inner_box1 & -inner_box2)]
-cells += [openmc.Cell(fill=iron, region=+inner_box2 & outer_box)]
-geometry = openmc.Geometry(cells)
-
 # Tell OpenMC we're going to use our custom source
 settings = openmc.Settings()
 settings.run_mode = "fixed source"
 settings.batches = 10
 settings.particles = 1000
 settings.source = my_plasma.sources
 
-# Finally, define a mesh tally so that we can see the resulting flux
-mesh = openmc.RegularMesh()
-mesh.lower_left = (-2000.0, -2000.0)
-mesh.upper_right = (2000.0, 2000.0)
-mesh.dimension = (50, 50)
-
-tally = openmc.Tally()
-tally.filters = [openmc.MeshFilter(mesh)]
-tally.scores = ["flux"]
-tallies = openmc.Tallies([tally])
 
-model = openmc.model.Model(
-    materials=mats, geometry=geometry, settings=settings, tallies=tallies
-)
+model = openmc.model.Model(materials=None, geometry=geometry, settings=settings)
 
 model.run()
```

### Comparing `openmc_plasma_source-0.3.0/openmc_plasma_source/__init__.py` & `openmc_plasma_source-0.3.1/src/openmc_plasma_source/__init__.py`

 * *Files identical despite different names*

### Comparing `openmc_plasma_source-0.3.0/openmc_plasma_source/fuel_types.py` & `openmc_plasma_source-0.3.1/src/openmc_plasma_source/fuel_types.py`

 * *Files identical despite different names*

### Comparing `openmc_plasma_source-0.3.0/openmc_plasma_source/plotting/plot_tokamak_source.py` & `openmc_plasma_source-0.3.1/src/openmc_plasma_source/plotting/plot_tokamak_source.py`

 * *Files identical despite different names*

### Comparing `openmc_plasma_source-0.3.0/openmc_plasma_source/point_source.py` & `openmc_plasma_source-0.3.1/src/openmc_plasma_source/point_source.py`

 * *Files identical despite different names*

### Comparing `openmc_plasma_source-0.3.0/openmc_plasma_source/ring_source.py` & `openmc_plasma_source-0.3.1/src/openmc_plasma_source/ring_source.py`

 * *Files identical despite different names*

### Comparing `openmc_plasma_source-0.3.0/openmc_plasma_source/tokamak_source.py` & `openmc_plasma_source-0.3.1/src/openmc_plasma_source/tokamak_source.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,19 +37,21 @@
             (referred in [1] as ion temperature exponent beta_T)
         ion_temperature_pedestal (float): Ion temperature at pedestal (keV)
         ion_temperature_separatrix (float): Ion temperature at separatrix
             (keV)
         pedestal_radius (float): Minor radius at pedestal (cm)
         shafranov_factor (float): Shafranov factor (referred in [1] as esh)
             also known as outward radial displacement of magnetic surfaces
-            (m)
+            (cm)
         angles (iterable of floats): the start and stop angles of the ring in
             radians
-        sample_size (int, optional): number of neutron sources. Defaults
-            to 1000.
+        sample_size int: number of neutron sources. Defaults to 1000.
+        sample_seed int: the seed passed to numpy.random when sampling source
+            location. Numpy recommend a large int value. Defaults to
+            122807528840384100672342137672332424406
     """
 
     def __init__(
         self,
         major_radius: float,
         minor_radius: float,
         elongation: float,
@@ -64,14 +66,15 @@
         ion_temperature_beta: float,
         ion_temperature_pedestal: float,
         ion_temperature_separatrix: float,
         pedestal_radius: float,
         shafranov_factor: float,
         angles: Tuple[float, float] = (0, 2 * np.pi),
         sample_size: int = 1000,
+        sample_seed: int = 122807528840384100672342137672332424406,
     ) -> None:
         # Assign attributes
         self.major_radius = major_radius
         self.minor_radius = minor_radius
         self.elongation = elongation
         self.triangularity = triangularity
         self.ion_density_centre = ion_density_centre
@@ -84,14 +87,15 @@
         self.ion_temperature_peaking_factor = ion_temperature_peaking_factor
         self.ion_temperature_pedestal = ion_temperature_pedestal
         self.ion_temperature_separatrix = ion_temperature_separatrix
         self.ion_temperature_beta = ion_temperature_beta
         self.shafranov_factor = shafranov_factor
         self.angles = angles
         self.sample_size = sample_size
+        self.sample_seed = sample_seed
 
         # Perform sanity checks for inputs not caught by properties
         if self.minor_radius >= self.major_radius:
             raise ValueError("Minor radius must be smaller than major radius")
 
         if self.pedestal_radius >= self.minor_radius:
             raise ValueError("Pedestal radius must be smaller than minor radius")
@@ -337,16 +341,17 @@
 
     def sample_sources(self):
         """Samples self.sample_size neutrons and creates attributes .densities
         (ion density), .temperatures (ion temperature), .strengths
         (neutron source density) and .RZ (coordinates)
         """
         # create a sample of (a, alpha) coordinates
-        a = np.random.random(self.sample_size) * self.minor_radius
-        alpha = np.random.random(self.sample_size) * 2 * np.pi
+        rng = np.random.default_rng(self.sample_seed)
+        a = rng.random(self.sample_size) * self.minor_radius
+        alpha = rng.random(self.sample_size) * 2 * np.pi
 
         # compute densities, temperatures, neutron source densities and
         # convert coordinates
         self.densities = self.ion_density(a)
         self.temperatures = self.ion_temperature(a)
         self.neutron_source_density = neutron_source_density(
             self.densities, self.temperatures
```

### Comparing `openmc_plasma_source-0.3.0/openmc_plasma_source.egg-info/PKG-INFO` & `openmc_plasma_source-0.3.1/src/openmc_plasma_source.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 Metadata-Version: 2.1
-Name: openmc-plasma-source
-Version: 0.3.0
-Summary: Creates tokamak plasma sources for OpenMC
-Home-page: https://github.com/fusion-energy/openmc-plasma-source
-Author: The openmc-plasma-source Development Team
-Author-email: rdelaportemathurin@gmail.com
-License: MIT
-Project-URL: Source, https://github.com/fusion-energy/openmc-plasma-source
-Project-URL: Tracker, https://github.com/fusion-energy/openmc-plasma-source/issues
-Classifier: Natural Language :: English
-Classifier: Topic :: Scientific/Engineering
+Name: openmc_plasma_source
+Version: 0.3.1
+Summary: Creates tokamak and ICF plasma sources for OpenMC
+Author: Rémi Delaporte-Mathurin
+Project-URL: Homepage, https://github.com/fusion-energy/openmc-plasma-source
+Project-URL: Bug Tracker, https://github.com/fusion-energy/openmc-plasma-source/issues
+Keywords: python,neutron,fusion,source,openmc,energy,tokamak
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy>=1.9
 Requires-Dist: matplotlib>=3.2.2
-Requires-Dist: importlib-metadata; python_version < "3.8"
 Provides-Extra: tests
 Requires-Dist: pytest>=5.4.3; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 
 [![CircleCI](https://circleci.com/gh/fusion-energy/openmc-plasma-source/tree/main.svg?style=svg)](https://circleci.com/gh/fusion-energy/openmc-plasma-source/tree/main) [![codecov](https://codecov.io/gh/fusion-energy/openmc-plasma-source/branch/main/graph/badge.svg?token=kDvWo6NGue)](https://codecov.io/gh/fusion-energy/openmc-plasma-source) [![PyPI version](https://badge.fury.io/py/openmc-plasma-source.svg)](https://badge.fury.io/py/openmc-plasma-source)
 
 # OpenMC-plasma-source
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openmc_plasma_source-0.3.0/tests/test_fuel_types.py` & `openmc_plasma_source-0.3.1/tests/test_fuel_types.py`

 * *Files identical despite different names*

### Comparing `openmc_plasma_source-0.3.0/tests/test_plotting.py` & `openmc_plasma_source-0.3.1/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `openmc_plasma_source-0.3.0/tests/test_point_source.py` & `openmc_plasma_source-0.3.1/tests/test_point_source.py`

 * *Files identical despite different names*

### Comparing `openmc_plasma_source-0.3.0/tests/test_ring_source.py` & `openmc_plasma_source-0.3.1/tests/test_ring_source.py`

 * *Files identical despite different names*

### Comparing `openmc_plasma_source-0.3.0/tests/test_tokamak_source.py` & `openmc_plasma_source-0.3.1/tests/test_tokamak_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,23 +260,23 @@
     # Specify the base strategies for each geometry input
     major_radius = draw(st.floats(min_value=1e-5, max_value=100.0, **finites))
 
     minor_radius = draw(
         st.floats(
             min_value=1e-5 * major_radius,
             max_value=np.nextafter(major_radius, major_radius - 1),
-            **finites
+            **finites,
         )
     )
 
     pedestal_radius = draw(
         st.floats(
             min_value=0.8 * minor_radius,
             max_value=np.nextafter(minor_radius, minor_radius - 1),
-            **finites
+            **finites,
         )
     )
 
     elongation = draw(st.floats(min_value=1e-5, max_value=10.0, **finites))
 
     triangularity = draw(
         st.floats(
@@ -284,15 +284,15 @@
         )
     )
 
     shafranov_factor = draw(
         st.floats(
             min_value=np.nextafter(-0.5 * minor_radius, +1),
             max_value=np.nextafter(0.5 * minor_radius, -1),
-            **finites
+            **finites,
         )
     )
 
     return TokamakSource(
         elongation=elongation,
         triangularity=triangularity,
         major_radius=major_radius,
```

