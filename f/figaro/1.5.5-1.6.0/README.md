# Comparing `tmp/figaro-1.5.5.tar.gz` & `tmp/figaro-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "figaro-1.5.5.tar", last modified: Fri Mar 15 18:25:45 2024, max compression
+gzip compressed data, was "figaro-1.6.0.tar", last modified: Sun Apr 14 08:24:11 2024, max compression
```

## Comparing `figaro-1.5.5.tar` & `figaro-1.6.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-03-15 18:25:45.908072 figaro-1.5.5/
--rw-r--r--   0 rinaldi    (503) staff       (20)     1072 2023-11-15 13:14:25.000000 figaro-1.5.5/LICENSE
--rw-r--r--   0 rinaldi    (503) staff       (20)       67 2024-02-10 17:20:30.000000 figaro-1.5.5/MANIFEST.in
--rw-r--r--   0 rinaldi    (503) staff       (20)     6873 2024-03-15 18:25:45.907847 figaro-1.5.5/PKG-INFO
--rw-r--r--   0 rinaldi    (503) staff       (20)     4154 2024-02-15 08:23:51.000000 figaro-1.5.5/README.md
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-03-15 18:25:45.892272 figaro-1.5.5/docs/
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-03-15 18:25:45.897183 figaro-1.5.5/docs/source/
--rw-r--r--   0 rinaldi    (503) staff       (20)      317 2024-02-15 08:23:51.000000 figaro-1.5.5/docs/source/api.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/figaro.cosmology.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      159 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/figaro.credible_regions.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/figaro.cumulative.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/figaro.decorators.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/figaro.diagnostic.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      121 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/figaro.load.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      133 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/figaro.marginal.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      130 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/figaro.mixture.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/figaro.montecarlo.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      121 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/figaro.plot.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      293 2024-02-15 08:23:51.000000 figaro-1.5.5/docs/source/figaro.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/figaro.transform.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      124 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/figaro.utils.rst
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-03-15 18:25:45.899483 figaro-1.5.5/docs/source/generated/
--rw-r--r--   0 rinaldi    (503) staff       (20)      207 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/generated/figaro.cosmology.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      363 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/generated/figaro.credible_regions.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      231 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/generated/figaro.cumulative.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      263 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/generated/figaro.decorators.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      397 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/generated/figaro.diagnostic.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      267 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/generated/figaro.load.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      211 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/generated/figaro.marginal.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      225 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/generated/figaro.mixture.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      201 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/generated/figaro.montecarlo.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      357 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/generated/figaro.plot.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      385 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/generated/figaro.transform.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)      320 2023-11-15 13:14:25.000000 figaro-1.5.5/docs/source/generated/figaro.utils.rst
--rw-r--r--   0 rinaldi    (503) staff       (20)     1009 2024-02-15 08:23:51.000000 figaro-1.5.5/docs/source/index.rst
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-03-15 18:25:45.904584 figaro-1.5.5/figaro/
--rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-01-16 16:50:38.000000 figaro-1.5.5/figaro/__init__.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     5008 2024-02-10 17:20:30.000000 figaro-1.5.5/figaro/_likelihood.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     1612 2024-03-15 18:23:44.000000 figaro-1.5.5/figaro/_numba_functions.py
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-03-15 18:25:45.907127 figaro-1.5.5/figaro/_pipelines/
--rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-02-10 17:20:30.000000 figaro-1.5.5/figaro/_pipelines/__init__.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    13338 2024-02-29 13:56:42.000000 figaro-1.5.5/figaro/_pipelines/hierarchical_inference.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    18041 2024-02-29 13:56:45.000000 figaro-1.5.5/figaro/_pipelines/par_hierarchical_inference.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    10593 2024-02-29 13:56:24.000000 figaro-1.5.5/figaro/_pipelines/par_probability_density.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     9403 2024-02-29 13:56:08.000000 figaro-1.5.5/figaro/_pipelines/probability_density.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     2274 2024-02-10 17:20:30.000000 figaro-1.5.5/figaro/cosmology.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     7490 2024-02-10 17:20:30.000000 figaro-1.5.5/figaro/credible_regions.py
--rw-r--r--   0 rinaldi    (503) staff       (20)      785 2024-02-10 17:20:30.000000 figaro-1.5.5/figaro/cumulative.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     1304 2024-02-10 17:20:30.000000 figaro-1.5.5/figaro/decorators.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     8460 2024-02-10 17:20:30.000000 figaro-1.5.5/figaro/diagnostic.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     1249 2024-02-06 14:42:23.000000 figaro-1.5.5/figaro/exceptions.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    26716 2024-02-24 19:49:02.000000 figaro-1.5.5/figaro/load.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     6282 2024-02-24 19:48:07.000000 figaro-1.5.5/figaro/marginal.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    51240 2024-03-15 18:23:44.000000 figaro-1.5.5/figaro/mixture.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     2590 2024-02-10 17:20:30.000000 figaro-1.5.5/figaro/montecarlo.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    39214 2024-02-25 14:45:38.000000 figaro-1.5.5/figaro/plot.py
--rw-r--r--   0 rinaldi    (503) staff       (20)      933 2024-02-06 14:42:23.000000 figaro-1.5.5/figaro/plot_settings.py
--rw-r--r--   0 rinaldi    (503) staff       (20)     3462 2024-02-13 11:17:19.000000 figaro-1.5.5/figaro/transform.py
--rw-r--r--   0 rinaldi    (503) staff       (20)    16063 2024-02-15 08:43:15.000000 figaro-1.5.5/figaro/utils.py
-drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-03-15 18:25:45.907587 figaro-1.5.5/figaro.egg-info/
--rw-r--r--   0 rinaldi    (503) staff       (20)     6873 2024-03-15 18:25:45.000000 figaro-1.5.5/figaro.egg-info/PKG-INFO
--rw-r--r--   0 rinaldi    (503) staff       (20)     1746 2024-03-15 18:25:45.000000 figaro-1.5.5/figaro.egg-info/SOURCES.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)        1 2024-03-15 18:25:45.000000 figaro-1.5.5/figaro.egg-info/dependency_links.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)      290 2024-03-15 18:25:45.000000 figaro-1.5.5/figaro.egg-info/entry_points.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)       76 2024-03-15 18:25:45.000000 figaro-1.5.5/figaro.egg-info/requires.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)        7 2024-03-15 18:25:45.000000 figaro-1.5.5/figaro.egg-info/top_level.txt
--rw-r--r--   0 rinaldi    (503) staff       (20)     1988 2024-03-15 18:25:27.000000 figaro-1.5.5/pyproject.toml
--rw-r--r--   0 rinaldi    (503) staff       (20)       38 2024-03-15 18:25:45.908118 figaro-1.5.5/setup.cfg
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-14 08:24:11.959134 figaro-1.6.0/
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1072 2023-11-15 13:14:25.000000 figaro-1.6.0/LICENSE
+-rw-r--r--   0 rinaldi    (503) staff       (20)       67 2024-02-10 17:20:30.000000 figaro-1.6.0/MANIFEST.in
+-rw-r--r--   0 rinaldi    (503) staff       (20)     6873 2024-04-14 08:24:11.958908 figaro-1.6.0/PKG-INFO
+-rw-r--r--   0 rinaldi    (503) staff       (20)     4154 2024-02-15 08:23:51.000000 figaro-1.6.0/README.md
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-14 08:24:11.944293 figaro-1.6.0/docs/
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-14 08:24:11.949364 figaro-1.6.0/docs/source/
+-rw-r--r--   0 rinaldi    (503) staff       (20)      317 2024-02-15 08:23:51.000000 figaro-1.6.0/docs/source/api.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.cosmology.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      159 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.credible_regions.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.cumulative.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.decorators.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.diagnostic.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      121 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.load.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      133 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.marginal.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      130 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.mixture.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      139 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.montecarlo.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      121 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.plot.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      293 2024-02-15 08:23:51.000000 figaro-1.6.0/docs/source/figaro.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      136 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.transform.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      124 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/figaro.utils.rst
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-14 08:24:11.951787 figaro-1.6.0/docs/source/generated/
+-rw-r--r--   0 rinaldi    (503) staff       (20)      207 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.cosmology.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      363 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.credible_regions.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      231 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.cumulative.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      263 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.decorators.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      397 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.diagnostic.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      267 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.load.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      211 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.marginal.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      225 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.mixture.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      201 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.montecarlo.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      357 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.plot.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      385 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.transform.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)      320 2023-11-15 13:14:25.000000 figaro-1.6.0/docs/source/generated/figaro.utils.rst
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1009 2024-02-15 08:23:51.000000 figaro-1.6.0/docs/source/index.rst
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-14 08:24:11.956945 figaro-1.6.0/figaro/
+-rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-01-16 16:50:38.000000 figaro-1.6.0/figaro/__init__.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     5008 2024-04-09 08:31:38.000000 figaro-1.6.0/figaro/_likelihood.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1612 2024-03-15 18:23:44.000000 figaro-1.6.0/figaro/_numba_functions.py
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-14 08:24:11.958449 figaro-1.6.0/figaro/_pipelines/
+-rw-r--r--   0 rinaldi    (503) staff       (20)        0 2024-02-10 17:20:30.000000 figaro-1.6.0/figaro/_pipelines/__init__.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    13557 2024-04-10 10:07:14.000000 figaro-1.6.0/figaro/_pipelines/hierarchical_inference.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    18761 2024-04-10 10:07:14.000000 figaro-1.6.0/figaro/_pipelines/par_hierarchical_inference.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    10486 2024-04-10 10:07:14.000000 figaro-1.6.0/figaro/_pipelines/par_probability_density.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     9321 2024-04-10 10:07:14.000000 figaro-1.6.0/figaro/_pipelines/probability_density.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     2341 2024-04-10 10:07:12.000000 figaro-1.6.0/figaro/cosmology.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     7490 2024-02-10 17:20:30.000000 figaro-1.6.0/figaro/credible_regions.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)      785 2024-02-10 17:20:30.000000 figaro-1.6.0/figaro/cumulative.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1304 2024-02-10 17:20:30.000000 figaro-1.6.0/figaro/decorators.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     8460 2024-02-10 17:20:30.000000 figaro-1.6.0/figaro/diagnostic.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1249 2024-02-06 14:42:23.000000 figaro-1.6.0/figaro/exceptions.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    33823 2024-04-10 10:07:14.000000 figaro-1.6.0/figaro/load.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     6282 2024-02-24 19:48:07.000000 figaro-1.6.0/figaro/marginal.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    54015 2024-04-12 07:55:46.000000 figaro-1.6.0/figaro/mixture.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     2590 2024-02-10 17:20:30.000000 figaro-1.6.0/figaro/montecarlo.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    40056 2024-04-10 10:07:14.000000 figaro-1.6.0/figaro/plot.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)      933 2024-02-06 14:42:23.000000 figaro-1.6.0/figaro/plot_settings.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)     3462 2024-02-13 11:17:19.000000 figaro-1.6.0/figaro/transform.py
+-rw-r--r--   0 rinaldi    (503) staff       (20)    16060 2024-04-10 10:07:14.000000 figaro-1.6.0/figaro/utils.py
+drwxr-xr-x   0 rinaldi    (503) staff       (20)        0 2024-04-14 08:24:11.958648 figaro-1.6.0/figaro.egg-info/
+-rw-r--r--   0 rinaldi    (503) staff       (20)     6873 2024-04-14 08:24:11.000000 figaro-1.6.0/figaro.egg-info/PKG-INFO
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1746 2024-04-14 08:24:11.000000 figaro-1.6.0/figaro.egg-info/SOURCES.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)        1 2024-04-14 08:24:11.000000 figaro-1.6.0/figaro.egg-info/dependency_links.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)      290 2024-04-14 08:24:11.000000 figaro-1.6.0/figaro.egg-info/entry_points.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)       76 2024-04-14 08:24:11.000000 figaro-1.6.0/figaro.egg-info/requires.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)        7 2024-04-14 08:24:11.000000 figaro-1.6.0/figaro.egg-info/top_level.txt
+-rw-r--r--   0 rinaldi    (503) staff       (20)     1988 2024-04-14 08:23:36.000000 figaro-1.6.0/pyproject.toml
+-rw-r--r--   0 rinaldi    (503) staff       (20)       38 2024-04-14 08:24:11.959184 figaro-1.6.0/setup.cfg
```

### Comparing `figaro-1.5.5/LICENSE` & `figaro-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `figaro-1.5.5/PKG-INFO` & `figaro-1.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.5.5
+Version: 1.6.0
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Author-email: Stefano Rinaldi <stefano.rinaldi@uni-heidelberg.de>, Walter Del Pozzo <walter.delpozzo@unipi.it>, Daniele Sanfratello <daniele.sanfratello@studenti.unipi.it>
 License: MIT License
         
         Copyright (c) 2022 Stefano Rinaldi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `figaro-1.5.5/README.md` & `figaro-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `figaro-1.5.5/docs/source/index.rst` & `figaro-1.6.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `figaro-1.5.5/figaro/_likelihood.py` & `figaro-1.6.0/figaro/_likelihood.py`

 * *Files identical despite different names*

### Comparing `figaro-1.5.5/figaro/_numba_functions.py` & `figaro-1.6.0/figaro/_numba_functions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.5.5/figaro/_pipelines/hierarchical_inference.py` & `figaro-1.6.0/figaro/_pipelines/hierarchical_inference.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 from tqdm import tqdm
 
 from figaro.mixture import DPGMM, HDPGMM
 from figaro.transform import transform_to_probit
 from figaro.utils import save_options, load_options, get_priors
 from figaro.plot import plot_median_cr, plot_multidim
-from figaro.load import load_data, load_single_event, save_density, load_density, supported_pars
+from figaro.load import load_data, load_single_event, load_selection_function, save_density, load_density, supported_pars
 
 def main():
 
     parser = optparse.OptionParser(prog = 'figaro-hierarchical', description = 'Hierarchical probability density reconstruction')
     # Input/output
     parser.add_option("-i", "--input", type = "string", dest = "input", help = "Folder with single-event samples files", default = None)
     parser.add_option("-b", "--bounds", type = "string", dest = "bounds", help = "Density bounds. Must be a string formatted as '[[xmin, xmax], [ymin, ymax],...]'. For 1D distributions use '[xmin, xmax]'. Quotation marks are required and scientific notation is accepted", default = None)
@@ -39,16 +39,15 @@
     parser.add_option("--exclude_points", dest = "exclude_points", action = 'store_true', help = "Exclude points outside bounds from analysis", default = False)
     parser.add_option("--cosmology", type = "string", dest = "cosmology", help = "Cosmological parameters (h, om, ol). Default values from Planck (2021)", default = '0.674,0.315,0.685')
     parser.add_option("-e", "--events", dest = "run_events", action = 'store_false', help = "Skip single-event analysis", default = True)
     parser.add_option("--se_sigma_prior", dest = "se_sigma_prior", type = "string", help = "Expected standard deviation (prior) for single-event inference - single value or n-dim values. If None, it is estimated from samples", default = None)
     parser.add_option("--sigma_prior", dest = "sigma_prior", type = "string", help = "Expected standard deviation (prior) for hierarchical inference - single value or n-dim values. If None, it is estimated from samples", default = None)
     parser.add_option("--fraction", dest = "fraction", type = "float", help = "Fraction of samples standard deviation for sigma prior. Overrided by sigma_prior.", default = None)
     parser.add_option("--mc_draws", dest = "mc_draws", type = "int", help = "Number of draws for assignment MC integral", default = None)
-    parser.add_option("--snr_threshold", dest = "snr_threshold", type = "float", help = "SNR threshold for simulated GW datasets", default = None)
-    parser.add_option("--far_threshold", dest = "far_threshold", type = "float", help = "FAR threshold for simulated GW datasets", default = None)
+    parser.add_option("--far_threshold", dest = "far_threshold", type = "float", help = "FAR threshold for LVK sensitivity estimate injections", default = 1.)
     parser.add_option("--no_probit", dest = "probit", action = 'store_false', help = "Disable probit transformation", default = True)
     parser.add_option("--config", dest = "config", type = "string", help = "Config file. Warning: command line options override config options", default = None)
     
     (options, args) = parser.parse_args()
 
     if options.config is not None:
         options = load_options(options, parser)
@@ -72,15 +71,19 @@
         output_plots.mkdir()
     output_draws = Path(options.output, 'draws')
     if not output_draws.exists():
         output_draws.mkdir()
     # Read hierarchical name
     if options.hier_name is None:
         options.hier_name = options.output.parts[-1]
-        
+    if options.selfunc_file is None:
+        hier_name = 'observed_'+options.hier_name
+    else:
+        hier_name = 'intrinsic_'+options.hier_name
+
     if options.config is None:
         save_options(options, options.output, name = options.hier_name)
     
     # Read bounds
     if options.bounds is not None:
         options.bounds = np.array(np.atleast_2d(eval(options.bounds)), dtype = np.float64)
     elif options.bounds is None and not options.postprocess:
@@ -104,32 +107,33 @@
     inj_density = None
     if options.inj_density_file is not None:
         inj_file_name = Path(options.inj_density_file).parts[-1].split('.')[0]
         spec = importlib.util.spec_from_file_location(inj_file_name, options.inj_density_file)
         inj_module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(inj_module)
         inj_density = inj_module.density
-    #If provided, load selecton function
+    # If provided, load selecton function
     selfunc = None
+    inj_pdf = None
     if options.selfunc_file is not None:
-        selfunc_file_name = Path(options.selfunc_file).parts[-1].split('.')[0]
-        spec = importlib.util.spec_from_file_location(selfunc_file_name, options.selfunc_file)
-        selfunc_module = importlib.util.module_from_spec(spec)
-        spec.loader.exec_module(selfunc_module)
-        selfunc = selfunc_module.selection_function
+        selfunc, inj_pdf, n_total_inj = load_selection_function(options.selfunc_file, par = options.par, far_threshold = options.far_threshold)
+        if not callable(selfunc) and not options.probit:
+            # Keeping only the samples within bounds
+            selfunc = selfunc[np.where((np.prod(options.bounds[:,0] < selfunc, axis = 1) & np.prod(selfunc < options.bounds[:,1], axis = 1)))]
+            inj_pdf = inj_pdf[np.where((np.prod(options.bounds[:,0] < selfunc, axis = 1) & np.prod(selfunc < options.bounds[:,1], axis = 1)))]
     # If provided, load true values
     hier_samples = None
     if options.hier_samples is not None:
         options.hier_samples = Path(options.hier_samples).resolve()
         hier_samples, true_name = load_single_event(options.hier_samples, par = options.par, h = options.h, om = options.om, ol = options.ol, waveform = options.wf)
         if np.shape(hier_samples)[-1] == 1:
             hier_samples = hier_samples.flatten()
             
     # Load samples
-    events, names = load_data(options.input, par = options.par, n_samples = options.n_samples_dsp, h = options.h, om = options.om, ol = options.ol, waveform = options.wf, snr_threshold = options.snr_threshold, far_threshold = options.far_threshold)
+    events, names = load_data(options.input, par = options.par, n_samples = options.n_samples_dsp, h = options.h, om = options.om, ol = options.ol, waveform = options.wf)
     try:
         dim = np.shape(events[0][0])[-1]
     except IndexError:
         dim = 1
     if options.exclude_points:
         print("Ignoring points outside bounds.")
         for i, ev in enumerate(events):
@@ -181,21 +185,21 @@
         else:
             # Load pre-computed posteriors
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore", category=UserWarning)
                 posteriors = load_density(Path(output_draws, 'posteriors_single_event.'+options.ext), make_comp = False)
         # Run hierarchical analysis
         prior_pars = get_priors(options.bounds, samples = events, std = options.sigma_prior, scale = options.fraction, probit = options.probit, hierarchical = True)
-        mix        = HDPGMM(options.bounds, prior_pars = prior_pars, MC_draws = options.mc_draws, probit = options.probit)
+        mix        = HDPGMM(options.bounds, prior_pars = prior_pars, MC_draws = options.mc_draws, probit = options.probit, selection_function = selfunc, injection_pdf = inj_pdf, total_injections = n_total_inj)
         draws      = np.array([mix.density_from_samples(posteriors, make_comp = False) for _ in tqdm(range(options.draws), desc = 'Hierarchical')])
         # Save draws
-        save_density(draws, folder = output_draws, name = 'draws_'+options.hier_name, ext = options.ext)
+        save_density(draws, folder = output_draws, name = 'draws_'+hier_name, ext = options.ext)
     else:
-        draws = load_density(Path(output_draws, 'draws_'+options.hier_name+'.'+options.ext))
+        draws = load_density(Path(output_draws, 'draws_'+hier_name+'.'+options.ext))
     # Plot
     if dim == 1:
-        plot_median_cr(draws, injected = inj_density, selfunc = selfunc, samples = hier_samples, out_folder = output_plots, name = options.hier_name, label = options.symbol, unit = options.unit, hierarchical = True)
+        plot_median_cr(draws, injected = inj_density, samples = hier_samples, out_folder = output_plots, name = options.hier_name, label = options.symbol, unit = options.unit, hierarchical = True)
     else:
-        plot_multidim(draws, samples = hier_samples, out_folder = output_plots, name = options.hier_name, labels = symbols, units = units, hierarchical = True)
+        plot_multidim(draws, samples = hier_samples, out_folder = output_plots, name = hier_name, labels = symbols, units = units, hierarchical = True)
 
 if __name__ == '__main__':
     main()
```

### Comparing `figaro-1.5.5/figaro/_pipelines/par_hierarchical_inference.py` & `figaro-1.6.0/figaro/_pipelines/par_hierarchical_inference.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 from tqdm import tqdm
 
 from figaro.mixture import DPGMM, HDPGMM
 from figaro.transform import transform_to_probit
 from figaro.utils import save_options, load_options, get_priors
 from figaro.plot import plot_median_cr, plot_multidim
-from figaro.load import load_data, load_single_event, save_density, load_density, supported_pars
+from figaro.load import load_data, load_single_event, load_selection_function, save_density, load_density, supported_pars
 
 import ray
 from ray.util import ActorPool
 
 @ray.remote
 class worker:
     def __init__(self, bounds,
@@ -27,29 +27,35 @@
                        scale       = None,
                        events      = None,
                        label       = None,
                        unit        = None,
                        save_se     = True,
                        MC_draws    = None,
                        probit      = True,
+                       selfunc     = None,
+                       inj_pdf     = None,
+                       n_total_inj = None,
                        ):
         self.dim                  = bounds.shape[0]
         self.bounds               = bounds
         self.mixture              = DPGMM(self.bounds, probit = probit)
         self.hierarchical_mixture = HDPGMM(self.bounds,
-                                           MC_draws   = MC_draws,
-                                           probit     = probit,
-                                           prior_pars = get_priors(self.bounds,
-                                                                   samples      = events,
-                                                                   std          = hier_sigma,
-                                                                   scale        = scale,
-                                                                   probit       = probit,
-                                                                   hierarchical = True,
-                                                                   )
-                                            )
+                                           MC_draws           = MC_draws,
+                                           probit             = probit,
+                                           selection_function = selfunc,
+                                           injection_pdf      = inj_pdf,
+                                           total_injections   = n_total_inj,
+                                           prior_pars         = get_priors(self.bounds,
+                                                                           samples      = events,
+                                                                           std          = hier_sigma,
+                                                                           scale        = scale,
+                                                                           probit       = probit,
+                                                                           hierarchical = True,
+                                                                           ),
+                                           )
         self.out_folder_plots = out_folder_plots
         self.out_folder_draws = out_folder_draws
         self.se_sigma         = se_sigma
         self.scale            = scale
         self.save_se          = save_se
         self.label            = label
         self.unit             = unit
@@ -129,16 +135,15 @@
     parser.add_option("--cosmology", type = "string", dest = "cosmology", help = "Cosmological parameters (h, om, ol). Default values from Planck (2021)", default = '0.674,0.315,0.685')
     parser.add_option("-e", "--events", dest = "run_events", action = 'store_false', help = "Skip single-event analysis", default = True)
     parser.add_option("--se_sigma_prior", dest = "se_sigma_prior", type = "string", help = "Expected standard deviation (prior) for single-event inference - single value or n-dim values. If None, it is estimated from samples", default = None)
     parser.add_option("--sigma_prior", dest = "sigma_prior", type = "string", help = "Expected standard deviation (prior) for hierarchical inference - single value or n-dim values. If None, it is estimated from samples", default = None)
     parser.add_option("--fraction", dest = "fraction", type = "float", help = "Fraction of samples standard deviation for sigma prior. Overrided by sigma_prior.", default = None)
     parser.add_option("--n_parallel", dest = "n_parallel", type = "int", help = "Number of parallel threads", default = 2)
     parser.add_option("--mc_draws", dest = "mc_draws", type = "int", help = "Number of draws for assignment MC integral", default = None)
-    parser.add_option("--snr_threshold", dest = "snr_threshold", type = "float", help = "SNR threshold for simulated GW datasets", default = None)
-    parser.add_option("--far_threshold", dest = "far_threshold", type = "float", help = "FAR threshold for simulated GW datasets", default = None)
+    parser.add_option("--far_threshold", dest = "far_threshold", type = "float", help = "FAR threshold for LVK sensitivity estimate injections", default = 1.)
     parser.add_option("--no_probit", dest = "probit", action = 'store_false', help = "Disable probit transformation", default = True)
     parser.add_option("--config", dest = "config", type = "string", help = "Config file. Warning: command line options override config options", default = None)
 
     (options, args) = parser.parse_args()
 
     if options.config is not None:
         options = load_options(options, parser)
@@ -162,14 +167,18 @@
         output_plots.mkdir()
     output_draws = Path(options.output, 'draws')
     if not output_draws.exists():
         output_draws.mkdir()
     # Read hierarchical name
     if options.hier_name is None:
         options.hier_name = options.output.parts[-1]
+    if options.selfunc_file is None:
+        hier_name = 'observed_'+options.hier_name
+    else:
+        hier_name = 'intrinsic_'+options.hier_name
 
     if options.config is None:
         save_options(options, options.output, name = options.hier_name)
 
     # Read bounds
     if options.bounds is not None:
         options.bounds = np.array(np.atleast_2d(eval(options.bounds)), dtype = np.float64)
@@ -197,29 +206,30 @@
         inj_file_name = Path(options.inj_density_file).parts[-1].split('.')[0]
         spec = importlib.util.spec_from_file_location(inj_file_name, options.inj_density_file)
         inj_module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(inj_module)
         inj_density = inj_module.density
     #If provided, load selecton function
     selfunc = None
+    inj_pdf = None
     if options.selfunc_file is not None:
-        selfunc_file_name = Path(options.selfunc_file).parts[-1].split('.')[0]
-        spec = importlib.util.spec_from_file_location(selfunc_file_name, options.selfunc_file)
-        selfunc_module = importlib.util.module_from_spec(spec)
-        spec.loader.exec_module(selfunc_module)
-        selfunc = selfunc_module.selection_function
+        selfunc, inj_pdf, n_total_inj = load_selection_function(options.selfunc_file, par = options.par, far_threshold = options.far_threshold)
+        if not callable(selfunc):
+            # Keeping only the samples within bounds
+            selfunc = selfunc[np.where((np.prod(options.bounds[:,0] < selfunc, axis = 1) & np.prod(selfunc < options.bounds[:,1], axis = 1)))]
+            inj_pdf = inj_pdf[np.where((np.prod(options.bounds[:,0] < selfunc, axis = 1) & np.prod(selfunc < options.bounds[:,1], axis = 1)))]
     # If provided, load true values
     hier_samples = None
     if options.hier_samples is not None:
         options.hier_samples = Path(options.hier_samples).resolve()
         hier_samples, true_name = load_single_event(options.hier_samples, par = options.par, h = options.h, om = options.om, ol = options.ol, waveform = options.wf)
         if np.shape(hier_samples)[-1] == 1:
             hier_samples = hier_samples.flatten()
     # Load samples
-    events, names = load_data(options.input, par = options.par, n_samples = options.n_samples_dsp, h = options.h, om = options.om, ol = options.ol, waveform = options.wf, snr_threshold = options.snr_threshold, far_threshold = options.far_threshold)
+    events, names = load_data(options.input, par = options.par, n_samples = options.n_samples_dsp, h = options.h, om = options.om, ol = options.ol, waveform = options.wf)
     try:
         dim = np.shape(events[0][0])[-1]
     except IndexError:
         dim = 1
     if options.exclude_points:
         print("Ignoring points outside bounds.")
         for i, ev in enumerate(events):
@@ -257,14 +267,17 @@
                                         scale            = options.fraction,
                                         events           = events,
                                         label            = symbols,
                                         unit             = units,
                                         save_se          = options.save_single_event,
                                         MC_draws         = options.mc_draws,
                                         probit           = options.probit,
+                                        selfunc          = selfunc,
+                                        inj_pdf          = inj_pdf,
+                                        n_total_inj      = n_total_inj,
                                         )
                           for _ in range(options.n_parallel)])
         
         if options.run_events:
             # Run each single-event analysis
             posteriors = []
             for s in tqdm(pool.map_unordered(lambda a, v: a.run_event.remote(v), [[ev, name, options.se_draws] for ev, name in zip(events, names)]), total = len(events), desc = 'Events'):
@@ -281,34 +294,33 @@
             pass
         # Run hierarchical analysis
         draws = []
         for s in tqdm(pool.map_unordered(lambda a, v: a.draw_hierarchical.remote(), [_ for _ in range(options.draws)]), total = options.draws, desc = 'Sampling'):
             draws.append(s)
         draws = np.array(draws)
         # Save draws
-        save_density(draws, folder = output_draws, name = 'draws_'+options.hier_name, ext = options.ext)
+        save_density(draws, folder = output_draws, name = 'draws_'+hier_name, ext = options.ext)
     else:
-        draws = load_density(Path(output_draws, 'draws_'+options.hier_name+'.'+options.ext))
+        draws = load_density(Path(output_draws, 'draws_'+hier_name+'.'+options.ext))
     # Plot
     if dim == 1:
         plot_median_cr(draws,
                        injected     = inj_density,
-                       selfunc      = selfunc,
                        samples      = hier_samples,
                        out_folder   = output_plots,
                        name         = options.hier_name,
                        label        = options.symbol,
                        unit         = options.unit,
                        hierarchical = True,
                        )
     else:
         plot_multidim(draws,
                       samples      = hier_samples,
                       out_folder   = output_plots,
-                      name         = options.hier_name,
+                      name         = hier_name,
                       labels       = symbols,
                       units        = units,
                       hierarchical = True,
                       )
 
 if __name__ == '__main__':
     main()
```

### Comparing `figaro-1.5.5/figaro/_pipelines/par_probability_density.py` & `figaro-1.6.0/figaro/_pipelines/par_probability_density.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,19 +103,17 @@
         spec = importlib.util.spec_from_file_location(inj_file_name, options.inj_density_file)
         inj_module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(inj_module)
         inj_density = inj_module.density
     #If provided, load selecton function
     selfunc = None
     if options.selfunc_file is not None:
-        selfunc_file_name = Path(options.selfunc_file).parts[-1].split('.')[0]
-        spec = importlib.util.spec_from_file_location(selfunc_file_name, options.selfunc_file)
-        selfunc_module = importlib.util.module_from_spec(spec)
-        spec.loader.exec_module(selfunc_module)
-        selfunc = selfunc_module.selection_function
+        selfunc, _ = load_selection_function(options.selfunc_file, par = options.par)
+        if not callable(selfunc):
+            raise Exception("Only .py files with callable approximants are allowed for DPGMM reconstruction")
         
     if options.sigma_prior is not None:
         options.sigma_prior = np.array([float(s) for s in options.sigma_prior.split(',')])
     if options.input.is_file():
         files = [options.input]
         output_draws = options.output
         subfolder = False
```

### Comparing `figaro-1.5.5/figaro/_pipelines/probability_density.py` & `figaro-1.6.0/figaro/_pipelines/probability_density.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 from tqdm import tqdm
 from warnings import warn
 
 from figaro.mixture import DPGMM
 from figaro.utils import save_options, load_options, get_priors
 from figaro.plot import plot_median_cr, plot_multidim
-from figaro.load import load_single_event, save_density, load_density, supported_extensions, supported_pars
+from figaro.load import load_single_event, load_selection_function, save_density, load_density, supported_extensions, supported_pars
 
 def main():
 
     parser = optparse.OptionParser(prog = 'figaro-density', description = 'Probability density reconstruction')
     # Input/output
     parser.add_option("-i", "--input", type = "string", dest = "input", help = "File with samples", default = None)
     parser.add_option("-b", "--bounds", type = "string", dest = "bounds", help = "Density bounds. Must be a string formatted as '[[xmin, xmax], [ymin, ymax],...]'. For 1D distributions use '[xmin, xmax]'. Quotation marks are required and scientific notation is accepted", default = None)
@@ -82,19 +82,17 @@
         spec = importlib.util.spec_from_file_location(inj_file_name, options.inj_density_file)
         inj_module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(inj_module)
         inj_density = inj_module.density
     #If provided, load selecton function
     selfunc = None
     if options.selfunc_file is not None:
-        selfunc_file_name = Path(options.selfunc_file).parts[-1].split('.')[0]
-        spec = importlib.util.spec_from_file_location(selfunc_file_name, options.selfunc_file)
-        selfunc_module = importlib.util.module_from_spec(spec)
-        spec.loader.exec_module(selfunc_module)
-        selfunc = selfunc_module.selection_function
+        selfunc, _ = load_selection_function(options.selfunc_file, par = options.par)
+        if not callable(selfunc):
+            raise Exception("Only .py files with callable approximants are allowed for DPGMM reconstruction")
     
     if options.sigma_prior is not None:
         options.sigma_prior = np.array([float(s) for s in options.sigma_prior.split(',')])
     if options.input.is_file():
         files = [options.input]
         output_draws = options.output
         subfolder = False
```

### Comparing `figaro-1.5.5/figaro/cosmology.py` & `figaro-1.6.0/figaro/cosmology.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,7 +58,8 @@
             return 0.
         else:
             def objective(z, self, DL):
                 return DL - self.LuminosityDistance(z)
             return newton(objective,1.0,args=(self, DL))
 
 Planck18 = CosmologicalParameters(0.674, 0.315, 0.685, -1, 0, 0)
+Planck15 = CosmologicalParameters(0.679, 0.3065, 0.6935, -1, 0, 0)
```

### Comparing `figaro-1.5.5/figaro/credible_regions.py` & `figaro-1.6.0/figaro/credible_regions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.5.5/figaro/cumulative.py` & `figaro-1.6.0/figaro/cumulative.py`

 * *Files identical despite different names*

### Comparing `figaro-1.5.5/figaro/decorators.py` & `figaro-1.6.0/figaro/decorators.py`

 * *Files identical despite different names*

### Comparing `figaro-1.5.5/figaro/diagnostic.py` & `figaro-1.6.0/figaro/diagnostic.py`

 * *Files identical despite different names*

### Comparing `figaro-1.5.5/figaro/exceptions.py` & `figaro-1.6.0/figaro/exceptions.py`

 * *Files identical despite different names*

### Comparing `figaro-1.5.5/figaro/load.py` & `figaro-1.6.0/figaro/load.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 import numpy as np
 import h5py
 import warnings
 import json
 import dill
+import copy
+import importlib
 from figaro.exceptions import FIGAROException
 from figaro.mixture import mixture
 from figaro.cosmology import CosmologicalParameters
 from pathlib import Path
 from tqdm import tqdm
 
 supported_extensions = ['h5', 'hdf5', 'txt', 'dat', 'csv']
 supported_waveforms  = ['combined', 'imr', 'seob']
+injected_pars        = ['m1', 'm2', 'z', 's1x', 's1y', 's1z', 's2x', 's2y', 's2z', 'ra', 'dec']
+loadable_inj_pars    = injected_pars + ['q', 'chi_eff', 'chi_p', 's1', 's2']
+mass_parameters      = ['m1', 'm2', 'm1_detect', 'm2_detect', 'mc', 'mt', 'q']
+spin_parameters      = ['s1x', 's1y', 's1z', 's2x', 's2y', 's2z', 's1', 's2', 'chi_eff', 'chi_p']
 
 GW_par = {'m1'                 : 'mass_1_source',
           'm2'                 : 'mass_2_source',
           'm1_detect'          : 'mass_1',
           'm2_detect'          : 'mass_2',
           'mc'                 : 'chirp_mass_source',
           'mc_detect'          : 'chirp_mass',
           'mt'                 : 'total_mass_source',
           'z'                  : 'redshift',
           'q'                  : 'mass_ratio',
           'eta'                : 'symmetric_mass_ratio',
           'chi_eff'            : 'chi_eff',
+          'chi_p'              : 'chi_p',
           'ra'                 : 'ra',
           'dec'                : 'dec',
           'luminosity_distance': 'luminosity_distance',
           'cos_theta_jn'       : 'cos_theta_jn',
           'cos_tilt_1'         : 'cos_tilt_1',
           'cos_tilt_2'         : 'cos_tilt_2',
           's1x'                : 'spin_1x',
@@ -43,14 +50,29 @@
           'tc'                 : 'geocent_time',
           'snr'                : 'network_matched_filter_snr',
           'far'                : 'far',
           'log_prior'          : 'log_prior',
           'log_likelihood'     : 'log_likelihood',
           }
 
+# LVK 03 injections have a slightly different nomenclature (no underscore)
+# See https://zenodo.org/records/7890437
+inj_par = copy.deepcopy(GW_par)
+inj_par['m1']                  = 'mass1_source'
+inj_par['m2']                  = 'mass2_source'
+inj_par['m1_detect']           = 'mass1'
+inj_par['m2_detect']           = 'mass2'
+inj_par['s1x']                 = 'spin1x'
+inj_par['s1y']                 = 'spin1y'
+inj_par['s1z']                 = 'spin1z'
+inj_par['s2x']                 = 'spin2x'
+inj_par['s2y']                 = 'spin2y'
+inj_par['s2z']                 = 'spin2z'
+inj_par['luminosity_distance'] = 'distance'
+
 supported_pars = [p for p in GW_par.keys() if not p in ['snr', 'far']]
 
 def available_gw_pars():
     """
     Print a list of available GW parameters
     """
     print(supported_pars)
@@ -84,15 +106,15 @@
         rdstate = np.random.RandomState()
     event = Path(event).resolve()
     name, ext = str(event).split('/')[-1].split('.')
     if volume:
         par = ['ra', 'dec', 'luminosity_distance']
     if not ext in supported_extensions:
         raise TypeError("File {0}.{1} is not supported".format(name, ext))
-    if ext == 'txt' or ext == 'dat' or ext == 'csv':
+    if not ext in ['h5', 'hdf5']:
         if par is not None:
             warnings.warn("Par names (or volume keyword) are ignored for .txt/.dat/.csv files")
         if n_samples > -1:
             samples = np.atleast_1d(np.loadtxt(event))
             s = int(min([n_samples, len(samples)]))
             out = samples[rdstate.choice(np.arange(len(samples)), size = s, replace = False)]
         else:
@@ -154,18 +176,17 @@
             rdstate = np.random.RandomState(seed = 1)
         else:
             rdstate = np.random.RandomState()
         name, ext = str(event).split('/')[-1].split('.')
         names.append(name)
         if not ext in supported_extensions:
             raise TypeError("File {0}.{1} is not supported".format(name, ext))
-        
-        if ext == 'txt' or ext == 'dat' or ext == 'csv':
+        if not ext in ['h5', 'hdf5']:
             if par is not None:
-                warnings.warn("Par names (or volume keyword) are ignored for .txt/.dat files")
+                warnings.warn("Par names (or volume keyword) are ignored for .txt/.dat/.csv files")
             if n_samples > -1:
                 samples = np.atleast_1d(np.loadtxt(event))
                 s = int(min([n_samples, len(samples)]))
                 samples_subset = samples[rdstate.choice(np.arange(len(samples)), size = s, replace = False)]
                 if len(np.shape(samples_subset)) == 1:
                     samples_subset = np.atleast_2d(samples_subset).T
                 events.append(samples_subset)
@@ -220,15 +241,15 @@
         tuple cosmology:      cosmological parameters (h, om, ol)
         int n_samples:        number of samples for (random) downsampling. Default -1: all samples
         str waveform:         waveform family to be used ('combined', 'imr', 'seob')
         double snr_threhsold: SNR threshold for event filtering. For injection analysis only.
         double far_threshold: FAR threshold for event filtering. For injection analysis only.
     
     Returns:
-        np.ndarray:    samples
+        np.ndarray: samples
     '''
     h, om, ol = cosmology
     omega = CosmologicalParameters(h, om, ol, -1, 0, 0)
     if not waveform in supported_waveforms:
         raise FIGAROException("Unknown waveform: please use 'combined' (default), 'imr' or 'seob'")
     
     if far_threshold is not None and snr_threshold is not None:
@@ -244,15 +265,15 @@
     
     with h5py.File(Path(event), 'r') as f:
         samples     = []
         loaded_pars = []
         flag_filter = False
         try:
             try:
-                # LVK R&P mock data challenge
+                # LVK injections
                 try:
                     data = f['MDC']['posterior_samples']
                 # Playground
                 except:
                     data = f['posterior_samples']
                 MDC_flag = True
             # GWTC-2, GWTC-3
@@ -583,7 +604,140 @@
                     dict_[key] = bool(value)
             draws.append(mixture(**dict_, make_comp = make_comp))
         ll.append(draws)
     if len(ll) == 1:
         return ll[0]
     return ll
 
+def load_selection_function(file, par = None, far_threshold = 1):
+    """
+    Loads the selection function, either from a python module containing a method called 'selection_function' or via injections.
+    If injections, it assumes that the last column of a txt/csv/dat file contains the sampling pdf.
+    
+    Arguments:
+        str or Path file: selection function file
+        list-of-str par:  list with parameter(s) to extract from GW posteriors
+        double threshold: FAR threshold to filter LVK injections
+    
+    Returns:
+        np.ndarray or callable: detected samples or callable with approximant
+        np.ndarray or NoneType: injection pdf (for samples) or None (for approximant)
+    """
+    file = Path(file)
+    ext  = file.parts[-1].split('.')[1]
+    if not ext in supported_extensions + ['py']:
+        raise FIGAROException("Selection function file not supported")
+    if ext == 'py':
+        selfunc_file_name = file.parts[-1].split('.')[0]
+        spec              = importlib.util.spec_from_file_location(selfunc_file_name, file)
+        selfunc_module    = importlib.util.module_from_spec(spec)
+        spec.loader.exec_module(selfunc_module)
+        selfunc           = selfunc_module.selection_function
+        inj_pdf           = None
+        n_total_inj       = None
+    else:
+        if not ext in ['h5','hdf5']:
+            samples     = np.loadtxt(file)
+            det_idx     = samples[:,-1]
+            selfunc     = samples[:,:-2][det_idx == 1]
+            inj_pdf     = samples[:,-2][det_idx == 1]
+            n_total_inj = len(samples)
+        else:
+            selfunc, inj_pdf, n_total_inj = _unpack_injections(file, par, far_threshold)
+    return selfunc, inj_pdf, n_total_inj
+
+def _unpack_injections(file, par, far_threshold = 1.):
+    """
+    Reads data from .h5/.hdf5 injection file (https://zenodo.org/records/7890437).
+    A sample is considered detected if at least one of the searches calls a detection.
+    
+    Arguments:
+        str event:            file to read
+        str par:              parameter to extract
+        double far_threshold: FAR threshold for injection filtering
+    
+    Returns:
+        np.ndarray: samples
+        np.ndarray: injection pdf
+    """
+    # Check that a list of parameters is passed
+    if par is None:
+        raise TypeError("Please provide a list of parameter names you want to load (e.g. ['m1']).")
+    # Check that all the parametes are loadable
+    if not np.all([p in loadable_inj_pars for p in par]):
+        wrong_pars = [p for p in par if not p in loadable_inj_pars]
+        raise FIGAROException("The following parameters are not implemented: "+", ".join(wrong_pars))
+    with h5py.File(file, 'r') as f:
+        data = f['injections']
+        n_total_inj = int(data.attrs['total_generated'])
+        # Detected injections
+        far_cwb    = np.array(data['far_cwb'])
+        far_gstlal = np.array(data['far_gstlal'])
+        far_mbta   = np.array(data['far_mbta'])
+        try:
+            far_pycbc = np.array(data['far_pycbc_bbh'])
+        except:
+            far_pycbc = np.array(data['far_pycbc_hyperbank'])
+        idx = np.where((far_cwb < far_threshold) | (far_gstlal < far_threshold) | (far_mbta < far_threshold) | (far_pycbc < far_threshold))[0]
+        # Load samples
+        samples = np.zeros((len(par), len(idx)))
+        inj_pdf = np.ones(len(idx))
+        # Parameters
+        m1  = np.array(data[inj_par['m1']])[idx]
+        m2  = np.array(data[inj_par['m2']])[idx]
+        q   = m2/m1
+        s1x = np.array(data[inj_par['s1x']])[idx]
+        s1y = np.array(data[inj_par['s1y']])[idx]
+        s1z = np.array(data[inj_par['s1z']])[idx]
+        s2x = np.array(data[inj_par['s2x']])[idx]
+        s2y = np.array(data[inj_par['s2y']])[idx]
+        s2z = np.array(data[inj_par['s2z']])[idx]
+        for i, lab in enumerate(par):
+            # Already available parameters:
+            if lab in injected_pars:
+                if not lab == 'cos_theta_jn':
+                    samples[i] = np.array(data[inj_par[lab]])[idx]
+                else:
+                    samples[i] = np.cos(np.array(data[inj_par[lab]])[idx])
+            else:
+                # Masses
+                if lab == 'q':
+                    samples[i] = q
+                if lab == 'mt':
+                    samples[i] = m1 + m2
+                if lab == 'mc':
+                    samples[i] = m1*m2**(3./5.)/(m1+m2)**(1./5.)
+                # Spins
+                if lab == 's1':
+                    samples[i] = np.sqrt(s1x**2+s1y**2+s1z**2)
+                if lab == 's2':
+                    samples[i] = np.sqrt(s2x**2+s2y**2+s2z**2)
+                if lab == 'chi_eff':
+                    samples[i] = (s1z + q*s2z)/(1+q)
+                if lab == 'chi_p':
+                    samples[i] = np.maximum(np.sqrt(s1x**2+s1y**2), np.sqrt(s2x**2+s2y**2)*q*(4*q+3)/(4+3*q))
+        # Sampling pdf
+        n_mass_pars = len([lab for lab in par if lab in mass_parameters])
+        n_spin_pars = len([lab for lab in par if lab in spin_parameters])
+        # Masses
+        if n_mass_pars == 1:
+            inj_pdf *= np.array(data['mass1_source_sampling_pdf'])[idx]
+        elif n_mass_pars == 2:
+            inj_pdf *= np.array(data['mass1_source_mass2_source_sampling_pdf'])[idx]
+        if 'q' in par:
+            inj_pdf *= m1
+        # Spins
+        if n_spin_pars > 0:
+            inj_pdf *= (np.array(data['spin1x_spin1y_spin1z_sampling_pdf'])[idx]*np.array(data['spin2x_spin2y_spin2z_sampling_pdf'])[idx])**(n_spin_pars/6.)
+        if 's1' in par or 'chi_eff' in par or 'chi_p' in par:
+            inj_pdf /= 2*np.pi*(s1x**2+s1y**2+s1z**2)
+        if 's2' in par or 'chi_eff' in par or 'chi_p' in par:
+            inj_pdf /= 2*np.pi*(s2x**2+s2y**2+s2z**2)
+        # Distance
+        if 'z' in par:
+            inj_pdf *= np.array(data['redshift_sampling_pdf'])[idx]
+        # Sky position
+        if 'ra' in par:
+            inj_pdf *= np.array(data['right_ascension_sampling_pdf'])[idx]
+        if 'dec' in par:
+            inj_pdf *= np.array(data['declination_sampling_pdf'])[idx]
+    return samples.T, inj_pdf, n_total_inj
```

### Comparing `figaro-1.5.5/figaro/marginal.py` & `figaro-1.6.0/figaro/marginal.py`

 * *Files identical despite different names*

### Comparing `figaro-1.5.5/figaro/mixture.py` & `figaro-1.6.0/figaro/mixture.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,27 +258,28 @@
         int dim:       number of dimensions
         prior prior:   instance of the prior class with NIG/NIW prior parameters
         double logL_D: logLikelihood denominator
     
     Returns:
         component_h: instance of component_h class
     """
-    def __init__(self, x, dim, prior, logL_D, mu_MC, sigma_MC):
+    def __init__(self, x, dim, prior, logL_D, mu_MC, sigma_MC, log_alpha_factor):
         self.dim    = dim
         self.N      = 1
         self.logL_D = logL_D
         
         log_norm_D = logsumexp_jit(logL_D)
         
         idx        = np.random.choice(len(mu_MC), p = np.exp(logL_D - log_norm_D))
         self.mu    = np.copy(mu_MC[idx])
         self.sigma = np.copy(sigma_MC[idx])
         if dim == 1:
             self.mu = np.atleast_2d(self.mu).T
             self.sigma = np.atleast_2d(self.sigma).T
+        self.N_true = np.exp(np.log(self.N) - log_alpha_factor[idx])
             
 class density:
     """
     Class to initialise a common set of methods for mixture models. Not to be used.
     """
     def __init__(self):
         pass
@@ -692,16 +693,16 @@
         np.ndarray log_w:  component log weights
         bool make_comp:    make component objects
     
     Returns:
         mixture: instance of mixture class
     """
     def __init__(self, means, covs, w, bounds, dim, n_cl, n_pts, alpha = 1., probit = True, log_w = None, make_comp = True):
-        self.means      = means
-        self.covs       = covs
+        self.means = means
+        self.covs  = covs
         if make_comp:
             self.components = [mn(mean, cov, allow_singular = True) for mean, cov in zip(self.means, self.covs)]
         else:
             self.components = None
         if log_w is None:
             self.w      = w
             self.log_w  = np.log(w)
@@ -1134,44 +1135,61 @@
 
 class HDPGMM(DPGMM):
     """
     Class to infer a distribution given a set of observations (each being a set of samples).
     Child of DPGMM class
     
     Arguments:
-        iterable bounds:     boundaries of the rectangle over which the distribution is defined. It should be in the format [[xmin, xmax],[ymin, ymax],...]
-        iterable prior_pars: IW parameters
-        double alpha0:       initial guess for concentration parameter
-        double MC_draws:     number of MC draws for integral
-        bool probit:         whether to use the probit transformation or not
-        int n_reassignments: number of reassignments. Default is not to reassign.
+        iterable bounds:             boundaries of the rectangle over which the distribution is defined. It should be in the format [[xmin, xmax],[ymin, ymax],...]
+        iterable prior_pars:         IW parameters
+        double alpha0:               initial guess for concentration parameter
+        double MC_draws:             number of MC draws for integral
+        bool probit:                 whether to use the probit transformation or not
+        int n_reassignments:         number of reassignments. Default is not to reassign.
+        callable selection_function: selection function approximant or samples
+        np.ndarray injection_pdf:    pdf of injected samples (for selection function inclusion)
     
     Returns:
         HDPGMM: instance of HDPGMM class
     """
     def __init__(self, bounds,
-                       alpha0          = 1.,
-                       prior_pars      = None,
-                       MC_draws        = None,
-                       probit          = True,
-                       n_reassignments = 0.,
+                       alpha0             = 1.,
+                       prior_pars         = None,
+                       MC_draws           = None,
+                       probit             = True,
+                       n_reassignments    = 0.,
+                       selection_function = None,
+                       injection_pdf      = None,
+                       total_injections   = None,
                        ):
         bounds   = np.atleast_2d(bounds)
         self.dim = len(bounds)
         super().__init__(bounds = bounds, alpha0 = alpha0, probit = probit, n_reassignments = n_reassignments)
         if prior_pars is not None:
             self.exp_sigma, self.a = prior_pars
         else:
             self.exp_sigma, self.a = get_priors(bounds = self.bounds, probit = self.probit, hierarchical = True)
         self.invgamma = invgamma(self.a)
         if MC_draws is None:
             self.MC_draws = int((self.dim+1)*1e3)
         else:
             self.MC_draws = int(MC_draws)
         self.evaluated_logL = {}
+        # Selection function
+        self.selfunc = selection_function
+        if not callable(self.selfunc) and self.selfunc is not None:
+            try:
+                self.log_inj_pdf = np.log(injection_pdf)
+                self.total_inj   = int(total_injections)
+            except TypeError:
+                raise FIGAROException("Please provide injection pdf")
+            self.log_jacobian_inj = np.zeros(len(self.selfunc))
+            if self.probit:
+                self.selfunc = transform_to_probit(self.selfunc, self.bounds)
+                self.log_jacobian_inj = -probit_logJ(self.selfunc, self.bounds, self.probit)
         # MC samples
         self._draw_MC_samples()
         
     def initialise(self):
         """
         Initialise the mixture to initial conditions
         """
@@ -1190,15 +1208,34 @@
         if self.dim == 1:
             self.sigma_MC = self.sigma_MC.flatten()
             self.mu_MC = self.mu_MC.flatten()
         else:
             rhos = invwishart(df = self.dim+2, scale = np.identity(self.dim)).rvs(size = self.MC_draws)
             rhos = np.array([r/outer_jit(np.sqrt(diag_jit(r)), np.sqrt(diag_jit(r))) for r in rhos])
             self.sigma_MC = np.array([r*outer_jit(s,s) for r, s in zip(rhos, np.sqrt(self.sigma_MC))])
-            
+        if self.selfunc is not None:
+            # Approximant
+            if callable(self.selfunc):
+                n_samples = self.MC_draws
+                with np.errstate(divide = 'ignore', invalid = 'ignore'):
+                    if self.probit:
+                        self.log_alpha_factor = np.array([np.log(np.mean(self.selfunc(transform_from_probit(mn(m,s).rvs(self.MC_draws), self.bounds)))) for m, s in zip(self.mu_MC, self.sigma_MC)])
+                    else:
+                        self.log_alpha_factor = np.array([np.log(np.mean(self.selfunc(mn(m,s).rvs(self.MC_draws)))) for m, s in zip(self.mu_MC, self.sigma_MC)])
+            # Injections
+            else:
+                n_samples = self.total_inj
+                self.log_alpha_factor = np.array([logsumexp_jit(mn(m,s).logpdf(self.selfunc) + self.log_jacobian_inj - self.log_inj_pdf) - np.log(self.total_inj) for m, s in zip(self.mu_MC, self.sigma_MC)])
+            # Numerical stability: mu+sigma ignored if p_det too small (not enough predicted points to have a reliable value for alpha)
+            self.log_alpha_factor[self.log_alpha_factor < np.log(5e-3)] = np.inf
+            # Check for NaNs
+            self.log_alpha_factor = np.nan_to_num(self.log_alpha_factor, nan = np.inf, posinf = np.inf, neginf = np.inf)
+        else:
+            self.log_alpha_factor = np.zeros(self.MC_draws)
+        
     def add_new_point(self, ev):
         """
         Update the probability density reconstruction adding a new sample
         
         Arguments:
             iterable ev: set of single-event draws from a DPGMM inference
         """
@@ -1218,17 +1255,17 @@
         Returns:
             dict: p_i for each component
         """
         scores = np.zeros(self.n_cl+1)
         logL_N = np.zeros((self.n_cl+1, self.MC_draws))
         if logL_x is None:
             if self.dim == 1:
-                logL_x = evaluate_mixture_MC_draws_1d(self.mu_MC, self.sigma_MC, x.means, x.covs, x.w)
+                logL_x = evaluate_mixture_MC_draws_1d(self.mu_MC, self.sigma_MC, x.means, x.covs, x.w) - self.log_alpha_factor
             else:
-                logL_x = evaluate_mixture_MC_draws(self.mu_MC, self.sigma_MC, x.means, x.covs, x.w)
+                logL_x = evaluate_mixture_MC_draws(self.mu_MC, self.sigma_MC, x.means, x.covs, x.w) - self.log_alpha_factor
         for i in range(self.n_cl+1):
             if i == 0:
                 ss = None
                 logL_D = np.zeros(self.MC_draws)
                 scores[i] = np.log(self.alpha)
             else:
                 ss        = self.mixture[i-1]
@@ -1258,15 +1295,15 @@
         self.n_pts += 1
         scores, logL_N, logL_x = self._cluster_assignment_distribution(x, logL_x)
         try:
             cid = np.random.choice(np.arange(-1, self.n_cl), p=scores)
         except ValueError:
             cid = -1
         if cid == -1:
-            self.mixture.append(_component_h(x, self.dim, self.prior, logL_N[int(cid)+1], self.mu_MC, self.sigma_MC))
+            self.mixture.append(_component_h(x, self.dim, self.prior, logL_N[int(cid)+1], self.mu_MC, self.sigma_MC, self.log_alpha_factor))
             self.N_list.append(1.)
             self.n_cl += 1
             self.assignations[pt_id] = int(self.n_cl)-1
         else:
             self.mixture[int(cid)] = self._add_datapoint_to_component(self.mixture[int(cid)], logL_N[int(cid)+1])
             self.N_list[int(cid)] += 1
             self.assignations[pt_id] = int(cid)
@@ -1315,14 +1352,15 @@
         ss.mu    = np.copy(self.mu_MC[idx])
         ss.sigma = np.copy(self.sigma_MC[idx])
         if self.dim == 1:
             ss.mu = np.atleast_2d(ss.mu).T
             ss.sigma = np.atleast_2d(ss.sigma).T
         
         ss.N += 1
+        ss.N_true = np.exp(np.log(ss.N) - self.log_alpha_factor[idx])
         return ss
 
     def _remove_datapoint_from_component(self, ss, logL_D):
         """
         Update component parameters after assigning a sample to a component
         
         Arguments:
@@ -1339,14 +1377,15 @@
         ss.mu    = np.copy(self.mu_MC[idx])
         ss.sigma = np.copy(self.sigma_MC[idx])
         if self.dim == 1:
             ss.mu = np.atleast_2d(ss.mu).T
             ss.sigma = np.atleast_2d(ss.sigma).T
         
         ss.N -= 1
+        ss.N_true = np.exp(np.log(ss.N) - self.log_alpha_factor[idx])
         return ss
 
     def build_mixture(self, make_comp = True):
         """
         Instances a mixture class representing the inferred distribution
         
         Arguments:
@@ -1354,15 +1393,16 @@
         
         Returns:
             mixture: the inferred distribution
         """
         if self.n_cl == 0:
             raise FIGAROException("You are trying to build an empty mixture - perhaps you called the initialise() method. If you are using the density_from_samples() method, the inferred mixture is returned by that method as an instance of mixture class.")
         idx = np.where(np.array(self.N_list) > 0)[0]
-        return mixture(np.array([comp.mu for comp in np.array(self.mixture)[idx]]), np.array([comp.sigma for comp in np.array(self.mixture)[idx]]), np.array(self.w)[idx], self.bounds, self.dim, (np.array(self.N_list) > 0).sum(), self.n_pts, self.alpha, probit = self.probit, make_comp = make_comp)
+        w   = dirichlet(np.array([comp.N_true for comp in np.array(self.mixture)[idx]])+self.alpha/self.n_cl).rvs()[0]
+        return mixture(np.array([comp.mu for comp in np.array(self.mixture)[idx]]), np.array([comp.sigma for comp in np.array(self.mixture)[idx]]), w, self.bounds, self.dim, (np.array(self.N_list) > 0).sum(), self.n_pts, self.alpha, probit = self.probit, make_comp = make_comp)
 
     def density_from_samples(self, events, make_comp = True):
         """
         Reconstruct the probability density from a set of samples.
         
         Arguments:
             iterable samples: set of single-event draws from DPGMM
```

### Comparing `figaro-1.5.5/figaro/montecarlo.py` & `figaro-1.6.0/figaro/montecarlo.py`

 * *Files identical despite different names*

### Comparing `figaro-1.5.5/figaro/plot.py` & `figaro-1.6.0/figaro/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         Support placement in figure using the `projection` keyword argument.
         See http://matplotlib.org/devel/add_new_projection.html.
         """
         return cls, {}
         
 projection_registry.register(PPPlot)
 
-def plot_median_cr(draws, injected = None, samples = None, selfunc = None, bounds = None, out_folder = '.', name = 'density', n_pts = 1000, label = None, unit = None, hierarchical = False, show = False, save = True, subfolder = False, true_value = None, true_value_label = '\mathrm{True\ value}', injected_label = '\mathrm{Simulated}', median_label = None, fig = None):
+def plot_median_cr(draws, injected = None, samples = None, selfunc = None, bounds = None, out_folder = '.', name = 'density', n_pts = 1000, label = None, unit = None, hierarchical = False, show = False, save = True, subfolder = False, true_value = None, true_value_label = '\mathrm{True\ value}', injected_label = '\mathrm{Simulated}', median_label = None, fig = None, colors = ['steelblue', 'darkturquoise', 'mediumturquoise']):
     """
     Plot the recovered 1D distribution along with the injected distribution and samples from the true distribution (both if available).
     
     Arguments:
         iterable draws:                  container for mixture instances
         callable or np.ndarray injected: injected distribution (if available)
         np.ndarray samples:              samples from the true distribution (if available)
@@ -119,24 +119,28 @@
         bool show:                       whether to show the plots during the run or not
         bool subfolder:                  whether to save the plots in different subfolders (for multiple events)
         float true_value:                true value to infer
         str true_value_label:            label to assign to the true value marker
         str injected_label:              label to assign to the injected distribution
         str median_label:                label to assign to the reconstruction
         matplotlib.figure.Figure fig:    figure to use for plotting. Must have (dim,dim) axes.
+        list-of-str colors:              list of colors for median, 68% and 90% credible regions
+        
     
     Returns:
         matplotlib.figure.Figure: figure with the plot
     """
     if median_label is None:
         if hierarchical:
             median_label = '\mathrm{(H)DPGMM}'
         else:
             median_label = '\mathrm{DPGMM}'
     
+    color_med, color_68, color_90 = colors
+    
     all_bounds = np.atleast_2d([d.bounds[0] for d in draws])
     x_min = np.max(all_bounds[:,0])
     x_max = np.min(all_bounds[:,1])
     
     probit = np.array([d.probit for d in draws]).any()
     
     if bounds is not None:
@@ -178,41 +182,42 @@
     # Samples (if available)
     if samples is not None:
         ylim = ax.get_ylim()
     else:
         ax.set_yscale('log')
     
     # CR
-    ax.fill_between(x, p[95], p[5], color = 'mediumturquoise', alpha = 0.25)
-    ax.fill_between(x, p[84], p[16], color = 'darkturquoise', alpha = 0.25)
+    ax.fill_between(x, p[95], p[5], color = color_90, alpha = 0.25)
+    ax.fill_between(x, p[84], p[16], color = color_68, alpha = 0.25)
     # Selection function (if available)
     if selfunc is not None:
         if callable(selfunc):
             f_x = selfunc(x)
         else:
             f_x = selfunc
     # Injection (if available)
     if injected is not None:
         if callable(injected):
             p_x = injected(x)
         else:
             p_x = injected
         if injected_label is not None:
             injected_label = '$'+injected_label+'$'
-        ax.plot(x, p_x, lw = 0.5, color = 'red', label = injected_label)
         if selfunc is not None:
             filtered_p_x = p_x*f_x
-            ax.plot(x, filtered_p_x/np.sum(filtered_p_x*dx), lw = 0.5, color = 'k', label = '$\mathrm{Selection\ effects}$')
+            ax.plot(x, filtered_p_x/np.sum(filtered_p_x*dx), lw = 0.5, color = 'red', label = '$'+injected_label+'\ \\mathrm{(observed)}$')
+        else:
+            ax.plot(x, p_x, lw = 0.5, color = 'red', label = injected_label)
         
     # Median
     if true_value is not None:
         if true_value_label is not None:
             true_value_label = '$'+true_value_label+'$'
-        ax.axvline(true_value, ls = '--', color = 'r', dashes = (5,5), lw = 0.5, label = true_value_label)
-    ax.plot(x, p[50], lw = 0.7, color = 'steelblue', label = '${0}$'.format(median_label))
+        ax.axvline(true_value, ls = '--', color = 'firebrick', dashes = (5,5), lw = 0.5, label = true_value_label)
+    ax.plot(x, p[50], lw = 0.7, color = color_med, label = '${0}$'.format(median_label))
     if label is None:
         label = 'x'
     if unit is None or unit == '':
         ax.set_xlabel('${0}$'.format(label))
     else:
         ax.set_xlabel('${0}\ [{1}]$'.format(label, unit))
     ax.set_ylabel('$p({0})$'.format(label))
@@ -244,21 +249,22 @@
                     txt_folder.mkdir()
                 except FileExistsError:
                     pass
         else:
             plot_folder = out_folder
             log_folder  = out_folder
             txt_folder  = out_folder
-        fig.savefig(Path(log_folder, 'log_{0}.pdf'.format(name)), bbox_inches = 'tight')
-        ax.set_yscale('linear')
-        ax.autoscale(True)
-        if samples is not None:
-            ax.set_xlim(xlim)
-        fig.savefig(Path(plot_folder, '{0}.pdf'.format(name)), bbox_inches = 'tight')
-        np.savetxt(Path(txt_folder, 'prob_{0}.txt'.format(name)), np.array([x, p[50], p[5], p[16], p[84], p[95]]).T, header = 'x 50 5 16 84 95')
+        if not (selfunc is not None and hierarchical):
+            fig.savefig(Path(log_folder, 'log_observed_{0}.pdf'.format(name)), bbox_inches = 'tight')
+            ax.set_yscale('linear')
+            ax.autoscale(True)
+            if samples is not None:
+                ax.set_xlim(xlim)
+            fig.savefig(Path(plot_folder, 'observed_{0}.pdf'.format(name)), bbox_inches = 'tight')
+            np.savetxt(Path(txt_folder, 'prob_observed_{0}.txt'.format(name)), np.array([x, p[50], p[5], p[16], p[84], p[95]]).T, header = 'x 50 5 16 84 95')
     if show:
         ax.set_yscale('linear')
         ax.autoscale(True)
         if samples is not None:
             ax.set_xlim(xlim)
         plt.show()
     plt.close()
@@ -288,27 +294,27 @@
         else:
             ax.set_xlabel('${0}\ [{1}]$'.format(label, unit))
         ax.set_ylabel('$p({0})$'.format(label))
         ax.autoscale(True)
         ax.set_ylim(bottom = 1e-5, top = np.max(p[95])*1.1)
         ax.legend(loc = 0)
         if save:
-            fig.savefig(Path(log_folder, 'log_true_{0}.pdf'.format(name)), bbox_inches = 'tight')
+            fig.savefig(Path(log_folder, 'log_intrinsic_{0}.pdf'.format(name)), bbox_inches = 'tight')
             ax.set_yscale('linear')
             ax.autoscale(True)
-            fig.savefig(Path(plot_folder, 'true_{0}.pdf'.format(name)), bbox_inches = 'tight')
-            np.savetxt(Path(txt_folder, 'prob_true_{0}.txt'.format(name)), np.array([x, p[50], p[5], p[16], p[84], p[95]]).T, header = 'x 50 5 16 84 95')
+            fig.savefig(Path(plot_folder, 'intrinsic_{0}.pdf'.format(name)), bbox_inches = 'tight')
+            np.savetxt(Path(txt_folder, 'prob_intrinsic_{0}.txt'.format(name)), np.array([x, p[50], p[5], p[16], p[84], p[95]]).T, header = 'x 50 5 16 84 95')
         if show:
             ax.set_yscale('linear')
             ax.autoscale(True)
             plt.show()
         plt.close()
     return fig
 
-def plot_multidim(draws, samples = None, bounds = None, out_folder = '.', name = 'density', labels = None, units = None, hierarchical = False, show = False, save = True, subfolder = False, n_pts = 200, true_value = None, levels = [0.5, 0.68, 0.9], scatter_points = False, median_label = None, fig = None):
+def plot_multidim(draws, samples = None, bounds = None, out_folder = '.', name = 'density', labels = None, units = None, hierarchical = False, show = False, save = True, subfolder = False, n_pts = 200, true_value = None, levels = [0.5, 0.68, 0.9], scatter_points = False, median_label = None, fig = None, colors = ['steelblue', 'darkturquoise', 'mediumturquoise'], colormap = 'Blues'):
     """
     Plot the recovered multidimensional distribution along with samples from the true distribution (if available) as corner plot.
     
     Arguments:
         iterable draws:                container for mixture instances
         np.ndarray samples:            samples from the true distribution (if available)
         iterable bounds:               bounds for the recovered distribution. If None, bounds from mixture instances are used.
@@ -322,25 +328,30 @@
         bool subfolder:                whether to save in a dedicated subfolder
         int n_pts:                     number of grid points (same for each dimension)
         iterable true_value:           true value to plot
         iterable levels:               credible levels to plot
         bool scatter_points:           scatter samples on 2d plots
         str median_label:              label to assign to the reconstruction
         matplotlib.figure.Figure fig:  figure to use for plotting. Must have (dim,dim) axes.
+        list-of-str colors:            list of colors for median, 68% and 90% credible regions
+        str colormap:                  colormap for contour plots
     
     Returns:
         matplotlib.figure.Figure: figure with the plot
     """
     
     dim = draws[0].dim
     if median_label is None:
         if hierarchical:
             median_label = '\mathrm{(H)DPGMM}'
         else:
             median_label = '\mathrm{DPGMM}'
+    
+    color_med, color_68, color_90 = colors
+
     if labels is None:
         labels = ['$x_{'+'{0}'.format(i+1)+'}$' for i in range(dim)]
     else:
         labels = ['${0}$'.format(l) for l in labels]
     
     if units is not None:
         labels = [l[:-1]+'\ [{0}]$'.format(u) if not u == '' else l for l, u in zip(labels, units)]
@@ -422,20 +433,20 @@
         for perc in percentiles:
             p[perc] = np.percentile(probs, perc, axis = 0)
         norm = p[50].sum()*dx
         for perc in percentiles:
             p[perc] = p[perc]/norm
             
         # CR
-        ax.fill_between(x, p[95], p[5], color = 'mediumturquoise', alpha = 0.25)
-        ax.fill_between(x, p[84], p[16], color = 'darkturquoise', alpha = 0.25)
+        ax.fill_between(x, p[95], p[5], color = color_90, alpha = 0.25)
+        ax.fill_between(x, p[84], p[16], color = color_68, alpha = 0.25)
         if true_value is not None:
             if true_value[column] is not None:
-                ax.axvline(true_value[column], c = 'orangered', lw = 0.5)
-        ax.plot(x, p[50], lw = 0.7, color = 'steelblue', label = '${0}$'.format(median_label))
+                ax.axvline(true_value[column], c = 'firebrick', lw = 0.5)
+        ax.plot(x, p[50], lw = 0.7, color = color_med, label = '${0}$'.format(median_label))
         ax.set_yticks([])
         if column == K - 1:
             if labels is not None:
                 ax.set_xlabel(labels[-1])
         ticks = np.linspace(lim[0], lim[1], 5)
         ax.set_xticks(ticks)
         [l.set_rotation(45) for l in ax.get_xticklabels()]
@@ -486,30 +497,30 @@
             median = median/(median.sum()*np.prod(dgrid))
             median = median.reshape(n_pts, n_pts)
             
             X,Y = np.meshgrid(x,y)
             with np.errstate(divide = 'ignore'):
                 logmedian = np.nan_to_num(np.log(median), nan = -np.inf, neginf = -np.inf)
             _,_,levs = ConfidenceArea(logmedian, x, y, adLevels=levels)
-            ax.contourf(Y, X, np.exp(logmedian), cmap = 'Blues', levels = 100)
+            ax.contourf(Y, X, np.exp(logmedian), cmap = colormap, levels = 100)
             if true_value is not None:
                 if true_value[row] is not None:
-                    ax.axhline(true_value[row], c = 'orangered', lw = 0.5)
+                    ax.axhline(true_value[row], c = 'firebrick', lw = 0.5)
                 if true_value[column] is not None:
-                    ax.axvline(true_value[column], c = 'orangered', lw = 0.5)
+                    ax.axvline(true_value[column], c = 'firebrick', lw = 0.5)
                 if true_value[column] is not None and true_value[row] is not None:
-                    ax.plot(true_value[column], true_value[row], color = 'orangered', marker = 's', ms = 3)
-            c1 = ax.contour(Y, X, logmedian, np.sort(levs), colors='steelblue', linewidths=0.3)
+                    ax.plot(true_value[column], true_value[row], color = 'firebrick', marker = 's', ms = 3)
+            c1 = ax.contour(Y, X, logmedian, np.sort(levs), colors=color_med, linewidths=0.3)
             if plot_settings.tex_flag:
                 ax.clabel(c1, fmt = {l:'{0:.0f}\\%'.format(100*s) for l,s in zip(c1.levels, np.sort(levels)[::-1])}, fontsize = 3)
             else:
                 ax.clabel(c1, fmt = {l:'{0:.0f}\%'.format(100*s) for l,s in zip(c1.levels, np.sort(levels)[::-1])}, fontsize = 3)
             # Samples (if available)
             if samples is not None and scatter_points:
-                ax.scatter(samples[:,column], samples[:,row], marker = '+', c = 'orangered', linewidths = 1)
+                ax.scatter(samples[:,column], samples[:,row], marker = '+', c = 'firebrick', linewidths = 1)
             # Ticks
             xticks = np.linspace(lim[1,0], lim[1,1], 5)
             ax.set_xticks(xticks)
             yticks = np.linspace(lim[0,0], lim[0,1], 5)
             ax.set_yticks(yticks)
             ax.set_xlim(*lim[1])
             ax.set_ylim(*lim[0])
@@ -537,15 +548,15 @@
                     Path(out_folder, 'density').mkdir()
                 except FileExistsError:
                     pass
             fig.savefig(Path(out_folder, 'density', '{0}.pdf'.format(name)), bbox_inches = 'tight')
     plt.close()
     return fig
     
-def plot_1d_dist(x, draws, injected = None, samples = None, out_folder = '.', name = 'density', label = None, unit = None, show = False, save = True, subfolder = False, true_value = None, true_value_label = '\mathrm{True\ value}', injected_label = '\mathrm{Simulated}', median_label = '\mathrm{Median}', logx = False, logy = False):
+def plot_1d_dist(x, draws, injected = None, samples = None, out_folder = '.', name = 'density', label = None, unit = None, show = False, save = True, subfolder = False, true_value = None, true_value_label = '\mathrm{True\ value}', injected_label = '\mathrm{Simulated}', median_label = '\mathrm{Median}', logx = False, logy = False, colors = ['steelblue','darkturquoise','mediumturquoise']):
     """
     Plot a 1D distribution along with samples from the true distribution (if available).
     Differently from plot_median_cr, this method requires the distribution to be already evaluated.
     For FIGARO mixture instances, please use plot_median_cr.
 
     Arguments:
         iterable x:                      values at which realisations are evaluated
@@ -561,53 +572,56 @@
         bool subfolder:                  whether to save the plots in different subfolders (for multiple events)
         float true_value:                true value to infer
         str true_value_label:            label to assign to the true value marker
         str injected_label:              label to assign to the injected distribution
         str median_label:                label to assign to the median distribution
         bool logx:                       x log scale
         bool logy:                       y log scale
+        list-of-str colors:              list of colors for median, 68% and 90% credible regions
     """
     
     if not np.shape(x)[0] == np.shape(draws)[-1]:
         raise ValueError("x and each draw must have the same length")
     
     percentiles = [50, 5, 16, 84, 95]
     p = {}
     for perc in percentiles:
         p[perc] = np.percentile(draws, perc, axis = 0)
     
+    color_med, color_68, color_90 = colors
+    
     fig, ax = plt.subplots()
     
     # Samples (if available)
     if samples is not None:
         ax.hist(samples, bins = int(np.sqrt(len(samples))), histtype = 'step', density = True, label = '$\mathrm{Samples}$')
         xlim = ax.get_xlim()
         ylim = ax.get_ylim()
     
     # CR
-    ax.fill_between(x, p[95], p[5], color = 'mediumturquoise', alpha = 0.25)
-    ax.fill_between(x, p[84], p[16], color = 'darkturquoise', alpha = 0.25)
+    ax.fill_between(x, p[95], p[5], color = color_90, alpha = 0.25)
+    ax.fill_between(x, p[84], p[16], color = color_68, alpha = 0.25)
     # Injection (if available)
     if injected is not None:
         if callable(injected):
             p_x = injected(x)
         else:
             p_x = injected
         if injected_label is not None:
             injected_label = '$'+injected_label+'$'
         ax.plot(x, p_x, lw = 0.5, color = 'red', label = injected_label)
         
     # Median
     if true_value is not None:
         if true_value_label is not None:
             true_value_label = '$'+true_value_label+'$'
-        ax.axvline(true_value, ls = '--', color = 'r', lw = 0.5, dashes = (5,5), label = true_value_label)
+        ax.axvline(true_value, ls = '--', color = 'firebrick', lw = 0.5, dashes = (5,5), label = true_value_label)
     if median_label is not None:
         median_label = '$'+median_label+'$'
-    ax.plot(x, p[50], lw = 0.7, color = 'steelblue', label = median_label)
+    ax.plot(x, p[50], lw = 0.7, color = color_med, label = median_label)
     if label is None:
         label = 'x'
     if unit is None or unit == '':
         ax.set_xlabel('${0}$'.format(label))
     else:
         ax.set_xlabel('${0}\ [{1}]$'.format(label, unit))
     ax.set_ylabel('$p({0})$'.format(label))
@@ -664,18 +678,18 @@
         str name:               name to be given to outputs
         bool save:              whether to save the plot or not
         bool show:              whether to show the plot during the run or not
     """
     fig, ax = plt.subplots()
     ax1 = ax.twinx()
     ax.plot(np.arange(1, len(n_cl)+1), n_cl, ls = '--', marker = '', lw = 0.7, color = 'k')
-    ax1.plot(np.arange(1, len(alpha)+1), alpha, ls = '--', marker = '', lw = 0.7, color = 'r')
+    ax1.plot(np.arange(1, len(alpha)+1), alpha, ls = '--', marker = '', lw = 0.7, color = 'firebrick')
     ax.set_xlabel('$t$')
     ax.set_ylabel('$N_{\mathrm{cl}}(t)$', color = 'k')
-    ax1.set_ylabel('$\alpha(t)$', color = 'r')
+    ax1.set_ylabel('$\alpha(t)$', color = 'firebrick')
     if show:
         plt.show()
     if save:
         fig.savefig(Path(out_folder, '{0}_n_cl_alpha.pdf'.format(name)), bbox_inches = 'tight')
     plt.close()
 
 def pp_plot_cdf(draws, injection, n_points = 1000, out_folder = '.', name = 'event', show = False, save = True):
```

### Comparing `figaro-1.5.5/figaro/plot_settings.py` & `figaro-1.6.0/figaro/plot_settings.py`

 * *Files identical despite different names*

### Comparing `figaro-1.5.5/figaro/transform.py` & `figaro-1.6.0/figaro/transform.py`

 * *Files identical despite different names*

### Comparing `figaro-1.5.5/figaro/utils.py` & `figaro-1.6.0/figaro/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,15 @@
                     samples = np.concatenate((samples, ss))
         if save_samples:
             if names is not None:
                 name = names[i]
             else:
                 name = 'event_{0}'.format(i+1)
             np.savetxt(Path(events_folder, name+'.txt'), samples[1:])
-        mix = mixture(np.atleast_2d(mm), np.atleast_3d(cc), np.ones(len(means))/len(means), bounds, len(bounds), len(means), None, probit = probit, alpha = 1.)
+        mix = mixture(np.atleast_2d(mm), np.atleast_3d(cc), np.ones(len(means))/len(means), bounds, len(bounds), len(means), 0, probit = probit, alpha = 1.)
         if save:
             with open(Path(draws_folder, name+'.pkl'), 'wb') as f:
                 dill.dump(np.array([mix]), f)
         mixtures.append([mix])
     mixtures = np.array(mixtures)
     
     if save:
```

### Comparing `figaro-1.5.5/figaro.egg-info/PKG-INFO` & `figaro-1.6.0/figaro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: figaro
-Version: 1.5.5
+Version: 1.6.0
 Summary: FIGARO: Fast Inference for GW Astronomy, Research & Observations
 Author-email: Stefano Rinaldi <stefano.rinaldi@uni-heidelberg.de>, Walter Del Pozzo <walter.delpozzo@unipi.it>, Daniele Sanfratello <daniele.sanfratello@studenti.unipi.it>
 License: MIT License
         
         Copyright (c) 2022 Stefano Rinaldi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `figaro-1.5.5/figaro.egg-info/SOURCES.txt` & `figaro-1.6.0/figaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `figaro-1.5.5/pyproject.toml` & `figaro-1.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 [tool.setuptools]
 packages = ['figaro', 'figaro._pipelines']
 
 [project]
 name = 'figaro'
 description = 'FIGARO: Fast Inference for GW Astronomy, Research & Observations'
-version = '1.5.5'
+version = '1.6.0'
 requires-python = '< 3.12'
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE"}
 keywords = ['DPGMM', 'figaro', 'hierarchical', 'inference', 'HDPGMM']
 authors = [
   {name = "Stefano Rinaldi", email = "stefano.rinaldi@uni-heidelberg.de"},
   {name = "Walter Del Pozzo", email = "walter.delpozzo@unipi.it"},
```

