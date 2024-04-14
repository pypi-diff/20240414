# Comparing `tmp/geoquanta-0.0.2.tar.gz` & `tmp/geoquanta-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoquanta-0.0.2.tar", last modified: Mon Feb 26 16:03:58 2024, max compression
+gzip compressed data, was "geoquanta-0.0.3.tar", last modified: Sun Apr 14 06:57:03 2024, max compression
```

## Comparing `geoquanta-0.0.2.tar` & `geoquanta-0.0.3.tar`

### file list

```diff
@@ -1,52 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:03:58.121081 geoquanta-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-26 16:03:43.000000 geoquanta-0.0.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:03:58.113081 geoquanta-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:03:58.117081 geoquanta-0.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-02-26 16:03:43.000000 geoquanta-0.0.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-02-26 16:03:43.000000 geoquanta-0.0.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-26 16:03:43.000000 geoquanta-0.0.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:03:58.117081 geoquanta-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-02-26 16:03:43.000000 geoquanta-0.0.2/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-02-26 16:03:43.000000 geoquanta-0.0.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-02-26 16:03:43.000000 geoquanta-0.0.2/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-02-26 16:03:43.000000 geoquanta-0.0.2/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-02-26 16:03:43.000000 geoquanta-0.0.2/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-02-26 16:03:43.000000 geoquanta-0.0.2/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-02-26 16:03:43.000000 geoquanta-0.0.2/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-02-26 16:03:43.000000 geoquanta-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 16:03:43.000000 geoquanta-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-26 16:03:43.000000 geoquanta-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-02-26 16:03:58.121081 geoquanta-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-02-26 16:03:43.000000 geoquanta-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:03:58.121081 geoquanta-0.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-26 16:03:43.000000 geoquanta-0.0.2/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-26 16:03:43.000000 geoquanta-0.0.2/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-02-26 16:03:43.000000 geoquanta-0.0.2/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:03:58.121081 geoquanta-0.0.2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-26 16:03:43.000000 geoquanta-0.0.2/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-26 16:03:43.000000 geoquanta-0.0.2/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-26 16:03:43.000000 geoquanta-0.0.2/docs/geoquanta.md
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-02-26 16:03:43.000000 geoquanta-0.0.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-02-26 16:03:43.000000 geoquanta-0.0.2/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:03:58.121081 geoquanta-0.0.2/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-26 16:03:43.000000 geoquanta-0.0.2/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-26 16:03:43.000000 geoquanta-0.0.2/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:03:58.121081 geoquanta-0.0.2/geoquanta/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-26 16:03:43.000000 geoquanta-0.0.2/geoquanta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-02-26 16:03:43.000000 geoquanta-0.0.2/geoquanta/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-26 16:03:43.000000 geoquanta-0.0.2/geoquanta/geoquanta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:03:58.121081 geoquanta-0.0.2/geoquanta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-02-26 16:03:58.000000 geoquanta-0.0.2/geoquanta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-02-26 16:03:58.000000 geoquanta-0.0.2/geoquanta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 16:03:58.000000 geoquanta-0.0.2/geoquanta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-26 16:03:58.000000 geoquanta-0.0.2/geoquanta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-26 16:03:58.000000 geoquanta-0.0.2/geoquanta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-26 16:03:58.000000 geoquanta-0.0.2/geoquanta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-02-26 16:03:43.000000 geoquanta-0.0.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-02-26 16:03:43.000000 geoquanta-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-26 16:03:43.000000 geoquanta-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-26 16:03:43.000000 geoquanta-0.0.2/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 16:03:58.121081 geoquanta-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 16:03:58.121081 geoquanta-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-26 16:03:43.000000 geoquanta-0.0.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-26 16:03:43.000000 geoquanta-0.0.2/tests/test_geoquanta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:57:03.296081 geoquanta-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-14 06:56:51.000000 geoquanta-0.0.3/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:57:03.284081 geoquanta-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:57:03.284081 geoquanta-0.0.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-14 06:56:51.000000 geoquanta-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-14 06:56:51.000000 geoquanta-0.0.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-14 06:56:51.000000 geoquanta-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:57:03.288081 geoquanta-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-14 06:56:51.000000 geoquanta-0.0.3/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-14 06:56:51.000000 geoquanta-0.0.3/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-14 06:56:51.000000 geoquanta-0.0.3/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-14 06:56:51.000000 geoquanta-0.0.3/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-14 06:56:51.000000 geoquanta-0.0.3/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-14 06:56:51.000000 geoquanta-0.0.3/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-14 06:56:51.000000 geoquanta-0.0.3/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-14 06:56:51.000000 geoquanta-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 06:56:51.000000 geoquanta-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-14 06:56:51.000000 geoquanta-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-14 06:57:03.296081 geoquanta-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-14 06:56:51.000000 geoquanta-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:57:03.288081 geoquanta-0.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:57:03.288081 geoquanta-0.0.3/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/examples/Add_Basemaps_and_Tile_Layers.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/examples/Geoquanta.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/examples/Vector.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:57:03.292081 geoquanta-0.0.3/docs/examples/countries/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/examples/countries/countries.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/examples/countries/countries.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    91209 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/examples/countries/countries.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)   241236 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/examples/countries/countries.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)   241236 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/examples/countries/countries.json
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/examples/countries/countries.prj
+-rw-r--r--   0 runner    (1001) docker     (127)   171476 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/examples/countries/countries.shp
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/examples/countries/countries.shx
+-rw-r--r--   0 runner    (1001) docker     (127)   232511 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/examples/countries/countries.zip
+-rw-r--r--   0 runner    (1001) docker     (127)   117900 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/examples/countries/europe_110.geo.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/examples/csv.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/examples/random.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/geoquanta.md
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:57:03.292081 geoquanta-0.0.3/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:57:03.296081 geoquanta-0.0.3/docs/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     4928 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/python/00_getting_started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/python/01_introduction_to_python.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/python/02_variables.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/python/03_data_types.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/python/04_operators.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4339 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/python/05_input_output.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/python/06_conditional_statements.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/python/07_loops.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/python/08_functions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    12092 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/python/09_data_structures.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/python/10_modules_and_packages.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/python/11_error_handling.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/python/12_file_handling.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7033 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/python/13_oop.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5743 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/python/14_special_methods.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-14 06:56:51.000000 geoquanta-0.0.3/docs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:57:03.296081 geoquanta-0.0.3/geoquanta/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-14 06:56:51.000000 geoquanta-0.0.3/geoquanta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-14 06:56:51.000000 geoquanta-0.0.3/geoquanta/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-14 06:56:51.000000 geoquanta-0.0.3/geoquanta/geoquanta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 06:56:51.000000 geoquanta-0.0.3/geoquanta/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:57:03.296081 geoquanta-0.0.3/geoquanta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-14 06:57:03.000000 geoquanta-0.0.3/geoquanta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-14 06:57:03.000000 geoquanta-0.0.3/geoquanta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 06:57:03.000000 geoquanta-0.0.3/geoquanta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-14 06:57:03.000000 geoquanta-0.0.3/geoquanta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-14 06:57:03.000000 geoquanta-0.0.3/geoquanta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 06:57:03.000000 geoquanta-0.0.3/geoquanta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-14 06:56:51.000000 geoquanta-0.0.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-14 06:56:51.000000 geoquanta-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-14 06:56:51.000000 geoquanta-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-14 06:56:51.000000 geoquanta-0.0.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 06:57:03.296081 geoquanta-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:57:03.296081 geoquanta-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-14 06:56:51.000000 geoquanta-0.0.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-14 06:56:51.000000 geoquanta-0.0.3/tests/test_geoquanta.py
```

### Comparing `geoquanta-0.0.2/.github/workflows/docs-build.yml` & `geoquanta-0.0.3/.github/workflows/docs-build.yml`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                   gdalinfo --version
             - name: Install dependencies
               run: |
                   pip install --no-cache-dir Cython
                   pip install -r requirements.txt -r requirements_dev.txt
                   pip install .
             - name: Discover typos with codespell
-              run: codespell --skip="*.csv,*.geojson,*.json,*.js,*.html,*cff,*.pdf,./.git" --ignore-words-list="aci,acount,hist"
+              run: codespell --skip="*.csv,*.geojson,*.json,*.js,*.html,*cff,*.pdf,./.git,*.txt" --ignore-words-list="aci,acount,hist"
             - name: PKG-TEST
               run: |
                   python -m unittest discover tests/
             - name: Build docs
               run: |
                   mkdocs build
             # - name: Deploy to Netlify
```

### Comparing `geoquanta-0.0.2/.github/workflows/docs.yml` & `geoquanta-0.0.3/.github/workflows/docs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -17,13 +17,13 @@
               run: |
                   python -m pip install --upgrade pip
                   pip install --user --no-cache-dir Cython
                   pip install --user -r requirements.txt -r requirements_dev.txt
                   pip install .
             - name: Discover typos with codespell
               run: |
-                  codespell --skip="*.csv,*.geojson,*.json,*.js,*.html,*cff,./.git" --ignore-words-list="aci,hist"
+                  codespell --skip="*.csv,*.geojson,*.json,*.js,*.html,*cff,./.git,*.txt" --ignore-words-list="aci,hist"
             - name: PKG-TEST
               run: |
                   python -m unittest discover tests/
             - run: mkdocs gh-deploy --force
```

### Comparing `geoquanta-0.0.2/.github/workflows/installation.yml` & `geoquanta-0.0.3/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `geoquanta-0.0.2/.github/workflows/macos.yml` & `geoquanta-0.0.3/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `geoquanta-0.0.2/.github/workflows/pypi.yml` & `geoquanta-0.0.3/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `geoquanta-0.0.2/.github/workflows/ubuntu.yml` & `geoquanta-0.0.3/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `geoquanta-0.0.2/.github/workflows/windows.yml` & `geoquanta-0.0.3/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `geoquanta-0.0.2/.gitignore` & `geoquanta-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `geoquanta-0.0.2/PKG-INFO` & `geoquanta-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoquanta
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python package for geospatial analysis, offering a wide range of tools and functionalities for working with geographic data.
 Author-email: Chaitanya Joshi <chaitanyaj14@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/chaitanyaj14/geoquanta
 Keywords: geoquanta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
+Requires-Dist: ipyleaflet
+Requires-Dist: pandas
 Provides-Extra: all
 Requires-Dist: geoquanta[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # geoquanta
 
@@ -35,8 +37,9 @@
 
 -   Free software: MIT License
 -   Documentation: https://chaitanyaj14.github.io/geoquanta
     
 
 ## Features
 
--   TODO
+-   Visualizing vector and raster data
+-   Analyzing vector and raster data
```

### Comparing `geoquanta-0.0.2/docs/contributing.md` & `geoquanta-0.0.3/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `geoquanta-0.0.2/docs/installation.md` & `geoquanta-0.0.3/docs/installation.md`

 * *Files identical despite different names*

### Comparing `geoquanta-0.0.2/geoquanta.egg-info/PKG-INFO` & `geoquanta-0.0.3/geoquanta.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoquanta
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python package for geospatial analysis, offering a wide range of tools and functionalities for working with geographic data.
 Author-email: Chaitanya Joshi <chaitanyaj14@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/chaitanyaj14/geoquanta
 Keywords: geoquanta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -14,14 +14,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
+Requires-Dist: ipyleaflet
+Requires-Dist: pandas
 Provides-Extra: all
 Requires-Dist: geoquanta[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # geoquanta
 
@@ -35,8 +37,9 @@
 
 -   Free software: MIT License
 -   Documentation: https://chaitanyaj14.github.io/geoquanta
     
 
 ## Features
 
--   TODO
+-   Visualizing vector and raster data
+-   Analyzing vector and raster data
```

### Comparing `geoquanta-0.0.2/pyproject.toml` & `geoquanta-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "geoquanta"
-version = "0.0.2"
+version = "0.0.3"
 dynamic = [
     "dependencies",
 ]
 description = "A python package for geospatial analysis, offering a wide range of tools and functionalities for working with geographic data."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.2"
+current_version = "0.0.3"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

