# Comparing `tmp/geneticalgorithm2-6.9.0.tar.gz` & `tmp/geneticalgorithm2-6.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneticalgorithm2-6.9.0.tar", last modified: Sun Apr 14 06:07:08 2024, max compression
+gzip compressed data, was "geneticalgorithm2-6.9.1.tar", last modified: Sun Apr 14 13:02:47 2024, max compression
```

## Comparing `geneticalgorithm2-6.9.0.tar` & `geneticalgorithm2-6.9.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-04-14 06:07:08.912212 geneticalgorithm2-6.9.0/
--rw-r--r--   0 pasa      (1000) pasa      (1000)     1095 2024-04-13 08:31:16.000000 geneticalgorithm2-6.9.0/LICENSE
--rw-r--r--   0 pasa      (1000) pasa      (1000)    81879 2024-04-14 06:07:08.911212 geneticalgorithm2-6.9.0/PKG-INFO
--rw-r--r--   0 pasa      (1000) pasa      (1000)     2206 2024-04-13 08:31:16.000000 geneticalgorithm2-6.9.0/README.rst
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-04-14 06:07:08.907212 geneticalgorithm2-6.9.0/geneticalgorithm2/
--rw-r--r--   0 pasa      (1000) pasa      (1000)     1077 2024-04-13 16:49:58.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/__init__.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-04-14 06:07:08.909212 geneticalgorithm2-6.9.0/geneticalgorithm2/callbacks/
--rw-r--r--   0 pasa      (1000) pasa      (1000)      171 2024-04-13 16:06:11.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/callbacks/__init__.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)     2087 2024-04-13 17:16:17.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/callbacks/data.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)    13210 2024-04-13 16:05:21.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/callbacks/middle.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)     2705 2024-04-13 14:22:37.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/callbacks/simple.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)     4640 2024-04-13 12:55:10.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/crossovers.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-04-14 06:07:08.910212 geneticalgorithm2-6.9.0/geneticalgorithm2/data_types/
--rw-r--r--   0 pasa      (1000) pasa      (1000)        0 2024-04-13 13:14:05.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/data_types/__init__.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)     4129 2024-04-13 16:34:58.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/data_types/algorithm_params.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)      638 2024-04-13 16:35:09.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/data_types/aliases.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)      227 2024-04-13 13:17:20.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/data_types/base.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)     5570 2024-04-13 13:39:12.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/data_types/generation.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)      656 2024-04-13 13:25:27.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/data_types/result.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)    44998 2024-04-13 16:58:46.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/geneticalgorithm2.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)     2567 2024-04-13 12:52:40.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/mutations.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)     3765 2024-04-13 16:45:38.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/population_initializer.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)     5193 2024-04-13 12:47:59.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/selections.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-04-14 06:07:08.911212 geneticalgorithm2-6.9.0/geneticalgorithm2/utils/
--rw-r--r--   0 pasa      (1000) pasa      (1000)        0 2024-04-13 09:55:36.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/utils/__init__.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)      323 2024-04-13 08:31:16.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/utils/aliases.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)     1448 2024-04-13 09:56:05.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/utils/cache.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)      584 2024-04-13 09:56:05.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/utils/files.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)     1224 2024-04-13 09:56:05.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/utils/funcs.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)     2897 2024-04-13 09:56:06.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/utils/plotting.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-04-14 06:07:08.908212 geneticalgorithm2-6.9.0/geneticalgorithm2.egg-info/
--rw-r--r--   0 pasa      (1000) pasa      (1000)    81879 2024-04-14 06:07:08.000000 geneticalgorithm2-6.9.0/geneticalgorithm2.egg-info/PKG-INFO
--rw-r--r--   0 pasa      (1000) pasa      (1000)     1046 2024-04-14 06:07:08.000000 geneticalgorithm2-6.9.0/geneticalgorithm2.egg-info/SOURCES.txt
--rw-r--r--   0 pasa      (1000) pasa      (1000)        1 2024-04-14 06:07:08.000000 geneticalgorithm2-6.9.0/geneticalgorithm2.egg-info/dependency_links.txt
--rw-r--r--   0 pasa      (1000) pasa      (1000)       83 2024-04-14 06:07:08.000000 geneticalgorithm2-6.9.0/geneticalgorithm2.egg-info/requires.txt
--rw-r--r--   0 pasa      (1000) pasa      (1000)       18 2024-04-14 06:07:08.000000 geneticalgorithm2-6.9.0/geneticalgorithm2.egg-info/top_level.txt
--rw-r--r--   0 pasa      (1000) pasa      (1000)       38 2024-04-14 06:07:08.912212 geneticalgorithm2-6.9.0/setup.cfg
--rw-r--r--   0 pasa      (1000) pasa      (1000)     1453 2024-04-13 08:31:16.000000 geneticalgorithm2-6.9.0/setup.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-04-14 13:02:47.660328 geneticalgorithm2-6.9.1/
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     1095 2024-04-13 08:31:16.000000 geneticalgorithm2-6.9.1/LICENSE
+-rw-r--r--   0 pasa      (1000) pasa      (1000)    66906 2024-04-14 13:02:47.660328 geneticalgorithm2-6.9.1/PKG-INFO
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     2206 2024-04-13 08:31:16.000000 geneticalgorithm2-6.9.1/README.rst
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-04-14 13:02:47.655328 geneticalgorithm2-6.9.1/geneticalgorithm2/
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     1077 2024-04-13 16:49:58.000000 geneticalgorithm2-6.9.1/geneticalgorithm2/__init__.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-04-14 13:02:47.657328 geneticalgorithm2-6.9.1/geneticalgorithm2/callbacks/
+-rw-r--r--   0 pasa      (1000) pasa      (1000)      171 2024-04-13 16:06:11.000000 geneticalgorithm2-6.9.1/geneticalgorithm2/callbacks/__init__.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     2087 2024-04-13 17:16:17.000000 geneticalgorithm2-6.9.1/geneticalgorithm2/callbacks/data.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)    13210 2024-04-13 16:05:21.000000 geneticalgorithm2-6.9.1/geneticalgorithm2/callbacks/middle.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     2705 2024-04-13 14:22:37.000000 geneticalgorithm2-6.9.1/geneticalgorithm2/callbacks/simple.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     4739 2024-04-14 12:26:05.000000 geneticalgorithm2-6.9.1/geneticalgorithm2/crossovers.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-04-14 13:02:47.659328 geneticalgorithm2-6.9.1/geneticalgorithm2/data_types/
+-rw-r--r--   0 pasa      (1000) pasa      (1000)        0 2024-04-13 13:14:05.000000 geneticalgorithm2-6.9.1/geneticalgorithm2/data_types/__init__.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     5600 2024-04-14 12:29:27.000000 geneticalgorithm2-6.9.1/geneticalgorithm2/data_types/algorithm_params.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)      638 2024-04-13 16:35:09.000000 geneticalgorithm2-6.9.1/geneticalgorithm2/data_types/aliases.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)      227 2024-04-13 13:17:20.000000 geneticalgorithm2-6.9.1/geneticalgorithm2/data_types/base.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     5570 2024-04-13 13:39:12.000000 geneticalgorithm2-6.9.1/geneticalgorithm2/data_types/generation.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)      656 2024-04-13 13:25:27.000000 geneticalgorithm2-6.9.1/geneticalgorithm2/data_types/result.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)    47326 2024-04-14 12:46:42.000000 geneticalgorithm2-6.9.1/geneticalgorithm2/geneticalgorithm2.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     2673 2024-04-14 12:27:52.000000 geneticalgorithm2-6.9.1/geneticalgorithm2/mutations.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     3765 2024-04-13 16:45:38.000000 geneticalgorithm2-6.9.1/geneticalgorithm2/population_initializer.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     5294 2024-04-14 12:32:32.000000 geneticalgorithm2-6.9.1/geneticalgorithm2/selections.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-04-14 13:02:47.660328 geneticalgorithm2-6.9.1/geneticalgorithm2/utils/
+-rw-r--r--   0 pasa      (1000) pasa      (1000)        0 2024-04-13 09:55:36.000000 geneticalgorithm2-6.9.1/geneticalgorithm2/utils/__init__.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)      323 2024-04-13 08:31:16.000000 geneticalgorithm2-6.9.1/geneticalgorithm2/utils/aliases.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     1448 2024-04-13 09:56:05.000000 geneticalgorithm2-6.9.1/geneticalgorithm2/utils/cache.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)      584 2024-04-13 09:56:05.000000 geneticalgorithm2-6.9.1/geneticalgorithm2/utils/files.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     1224 2024-04-13 09:56:05.000000 geneticalgorithm2-6.9.1/geneticalgorithm2/utils/funcs.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     2897 2024-04-13 09:56:06.000000 geneticalgorithm2-6.9.1/geneticalgorithm2/utils/plotting.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-04-14 13:02:47.656328 geneticalgorithm2-6.9.1/geneticalgorithm2.egg-info/
+-rw-r--r--   0 pasa      (1000) pasa      (1000)    66906 2024-04-14 13:02:47.000000 geneticalgorithm2-6.9.1/geneticalgorithm2.egg-info/PKG-INFO
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     1046 2024-04-14 13:02:47.000000 geneticalgorithm2-6.9.1/geneticalgorithm2.egg-info/SOURCES.txt
+-rw-r--r--   0 pasa      (1000) pasa      (1000)        1 2024-04-14 13:02:47.000000 geneticalgorithm2-6.9.1/geneticalgorithm2.egg-info/dependency_links.txt
+-rw-r--r--   0 pasa      (1000) pasa      (1000)       83 2024-04-14 13:02:47.000000 geneticalgorithm2-6.9.1/geneticalgorithm2.egg-info/requires.txt
+-rw-r--r--   0 pasa      (1000) pasa      (1000)       18 2024-04-14 13:02:47.000000 geneticalgorithm2-6.9.1/geneticalgorithm2.egg-info/top_level.txt
+-rw-r--r--   0 pasa      (1000) pasa      (1000)       38 2024-04-14 13:02:47.660328 geneticalgorithm2-6.9.1/setup.cfg
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     1453 2024-04-13 08:31:16.000000 geneticalgorithm2-6.9.1/setup.py
```

### Comparing `geneticalgorithm2-6.9.0/LICENSE` & `geneticalgorithm2-6.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geneticalgorithm2-6.9.0/PKG-INFO` & `geneticalgorithm2-6.9.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneticalgorithm2
-Version: 6.9.0
+Version: 6.9.1
 Summary: Supported highly optimized and flexible genetic algorithm package for python
 Home-page: https://github.com/PasaOpasen/geneticalgorithm2
 Author: Demetry Pascal
 Author-email: qtckpuhdsa@gmail.com
 Maintainer: Demetry Pascal
 License: MIT
 Keywords: solve,solver,equation,optimization,problem,genetic,algorithm,GA,easy,fast,genetic-algorithm,combinatorial,mixed,evolutionary
@@ -30,14 +30,15 @@
 **geneticalgorithm2** (from [DPEA](https://github.com/PasaOpasen/PasaOpasen.github.io/blob/master/EA_packages.md)) **is the supported advanced optimized fork of non-supported package** [geneticalgorithm](https://github.com/rmsolgi/geneticalgorithm) of *Ryan (Mohammad) Solgi*
 
 - [About](#about)
 - [Installation](#installation)
 - [Updates information](#updates-information)
   - [**Future**](#future)
   - [**TODO firstly**](#todo-firstly)
+  - [6.9.1 refactor](#691-refactor)
   - [6.9.0 reborn](#690-reborn)
   - [6.8.7 minor update](#687-minor-update)
   - [6.8.6 minor update](#686-minor-update)
   - [6.8.5 minor update](#685-minor-update)
   - [6.8.4 minor update](#684-minor-update)
   - [6.8.3 types update](#683-types-update)
   - [6.8.2 patch](#682-patch)
@@ -57,33 +58,39 @@
   - [6.5.1 patch](#651-patch)
   - [6.5.0 minor update (refactoring)](#650-minor-update-refactoring)
   - [6.4.1 patch (bug fix)](#641-patch-bug-fix)
   - [6.4.0 minor update (refactoring)](#640-minor-update-refactoring)
   - [6.3.0 minor update (refactoring)](#630-minor-update-refactoring)
 - [Working process](#working-process)
   - [Main algorithm structure](#main-algorithm-structure)
+  - [Optimization process components](#optimization-process-components)
+    - [Function to minimize](#function-to-minimize)
+    - [Optimization space](#optimization-space)
+    - [Algorithm parameters](#algorithm-parameters)
+    - [Samples constructors](#samples-constructors)
+    - [Callbacks](#callbacks)
   - [How to run](#how-to-run)
   - [Constructor parameters](#constructor-parameters)
   - [Genetic algorithm's parameters](#genetic-algorithms-parameters)
     - [AlgorithmParams object](#algorithmparams-object)
     - [Parameters of algorithm](#parameters-of-algorithm)
-      - [**Count parameters**](#count-parameters)
       - [**Crossover**](#crossover)
       - [**Mutation**](#mutation)
       - [**Selection**](#selection)
-  - [Methods and Properties of model:](#methods-and-properties-of-model)
+  - [Methods and Properties of model](#methods-and-properties-of-model)
 - [Examples for beginner](#examples-for-beginner)
   - [A minimal example](#a-minimal-example)
   - [The simple example with integer variables](#the-simple-example-with-integer-variables)
   - [The simple example with Boolean variables](#the-simple-example-with-boolean-variables)
   - [The simple example with mixed variables](#the-simple-example-with-mixed-variables)
   - [Optimization problems with constraints](#optimization-problems-with-constraints)
   - [Middle example: select fixed count of objects from set](#middle-example-select-fixed-count-of-objects-from-set)
 - [U should know these features](#u-should-know-these-features)
   - [Available crossovers](#available-crossovers)
+  - [Available selections](#available-selections)
   - [Function timeout](#function-timeout)
   - [Standard GA vs. Elitist GA](#standard-ga-vs-elitist-ga)
   - [Standard crossover vs. stud EA crossover](#standard-crossover-vs-stud-ea-crossover)
   - [Creating better start population](#creating-better-start-population)
     - [Select best N of kN](#select-best-n-of-kn)
     - [Do local optimization](#do-local-optimization)
     - [Optimization with oppositions](#optimization-with-oppositions)
@@ -125,14 +132,15 @@
   - [Using GA with image reconstruction by polygons](#using-ga-with-image-reconstruction-by-polygons)
 - [Popular questions](#popular-questions)
   - [How to disable autoplot?](#how-to-disable-autoplot)
   - [How to plot population scores?](#how-to-plot-population-scores)
   - [How to specify evaluated function for all population?](#how-to-specify-evaluated-function-for-all-population)
   - [What about parallelism?](#what-about-parallelism)
   - [How to initialize start population? How to continue optimization with new run?](#how-to-initialize-start-population-how-to-continue-optimization-with-new-run)
+
 # About
 
 [**geneticalgorithm2**](https://pasaopasen.github.io/geneticalgorithm2/) is very flexible and highly optimized Python library for implementing classic
 [genetic-algorithm](https://towardsdatascience.com/introduction-to-optimization-with-genetic-algorithm-2f5001d9964b) (GA).
 
 Features of this package:
 
@@ -147,46 +155,49 @@
 * support of mixed types of variables
 * **support of classic, elitist and studEA genetic algorithm combinations**
 * **support of revolutions and duplicates utilization**
 * **reach support of customization**
     
 # Installation
 
-Install this package with standard dependencies to use the entire functional.
+Install this package with standard light dependencies to use the base functional.
 ```
 pip install geneticalgorithm2
 ```
 
-Install this package with full dependencies to use all provided functional.
+Install this package with full dependencies to use all provided functional including plotting and built-in parallelism tools.
 
 ```
 pip install geneticalgorithm2[full]
 ```
 
 # Updates information
 
 ## **Future**
 
 - duplicates removing and revolutions will be moved to `MiddleCallbacks` and removed as alone `run()` parameters
-- `function_timeout` and `function` will be moved to `run()` method
 - new stop criteria callbacks (min std, max functions evaluations)
 - `vartype` will support strings like `iiiiibbf`
 
 ## **TODO firstly**
-- Remove old style mensions from README
+- Remove old style mentions from README
+
+## 6.9.1 refactor
 
+- Finally move `function_timeout` and `function` to `run()` method and deprecate its usage in init()
+- `function` is not mandatory to be non-empty 
+- reduce documentation duplicates
 
 ## 6.9.0 reborn
 
 - recreate the repository without excess heavy files materials 
 - host the [code documentation](https://pasaopasen.github.io/geneticalgorithm2/)
 - rename `geneticalgorithm2` class to `GeneticAlgorithm2`
 - substantial package architecture refactor
 - add more docstrings
-- reduce documentation duplicates 
 
 ## 6.8.7 minor update
 
 - some code refactor
 - fixes:
   - ensure the directory of generation file exists on save
 
@@ -220,15 +231,15 @@
 
 - printing progress bar to `'stderr'` or `'stdout'` or `None` (disable) by choice (`progress_bar_stream` argument of `run()`), deprecated `disable_progress_bar`
 - little speed up
 - new `geneticalgorithm2.vectorized_set_function` set function, which can be faster for big populations 
 
 ## 6.8.0 minor update
 
-- remove `crossover_probability` model parameter because of it has no sense to exist (and 1.0 value is better than others, take a look at [results](/tests/output/sense_of_crossover_prob__no_sense.png)). This parameter came from `geneticalgorithm` old package and did`t change before.
+- remove `crossover_probability` model parameter because of it has no sense to exist (and 1.0 value is better than others, take a look at [results](/examples/output/sense_of_crossover_prob__no_sense.png)). This parameter came from `geneticalgorithm` old package and did`t change before.
 
 ## 6.7.7 refactor
 
 - change some behavior about parents selection
 
 ## 6.7.6 bug fix
 
@@ -298,15 +309,15 @@
     * `None`
     * `str` path to saved generation
     * dictionary with structure `{'variables': variables/None, 'scores': scores/None}`
     * `Generation` object: `Generation(variables = variables, scores = scores)`
     * `np.ndarray` with shape `(samples, dim)` for only population or `(samples, dim+1)` for concatenated population and score (scores is the last matrix column)
     * `tuple(np.ndarray/None, np.ndarray/None)` for variables and scores
   
-  here `variables` is 2D numpy array with shape `(samples, dim)`, `scores` is 1D numpy array with scores (function values) for each sample; [here](tests/output/start_gen.py) and [here](#how-to-initialize-start-population-how-to-continue-optimization-with-new-run) u can see examples of using these valid forms 
+  here `variables` is 2D numpy array with shape `(samples, dim)`, `scores` is 1D numpy array with scores (function values) for each sample; [here](examples/output/start_gen.py) and [here](#how-to-initialize-start-population-how-to-continue-optimization-with-new-run) u can see examples of using these valid forms 
 
 
 ## 6.3.0 minor update (refactoring)
 
 - type hints for entire part of functions
 - new valid forms for function parameters (now u don't need to use numpy arrays everywhere)
 - `AlgorithmParams` class for base GA algorithm parameters (instead of dictionary)
@@ -343,17 +354,60 @@
     remove duplicates, make revolutions, sort population by scores
     use callbacks, use middle callbacks
 
 Post-process: plotting results, saving
 
 ```
 
+## Optimization process components
+
+### Function to minimize
+
+The goal of the optimization process is to find the *minimum* of the given `function (1D array) -> float` where the function argument is a vector of some values in different dimensions. 
+
+If u want to find the *maximum*, use this idea:
+```python
+opt_func = lambda arr: -func(arr)
+
+#
+# ... find global min of opt_func
+#
+
+opt_minimum=opt_func(best value)
+maximum = -opt_minimum
+```
+
+Also it is possible and highly recommended to create and use a *vectorized* version of this function called `set_function (2D array) -> (1D array)` which transforms several samples matrix to samples scores vector by one call. Using this way u can speed up calculations or set up more complex tasks optimization
+
+### Optimization space
+
+The function rates 1D arrays (vectors) where each component (dimension) means something u program it to mean. Each dimension has its `bound` (`[min; max]` cut) and `variable type` (real/discrete).
+
+**Advice**. Genetic algorithms work much faster and efficient for discrete tasks. If high precision is not required u can split any real dimension to many discrete values (for instance, `[1.1, 1.2, 1.25, 1.44]`) and try to optimize indexes of the given array which are converted to real values inside `function` itself.
+
+### Algorithm parameters
+
+There are a number of hyperparameters u can probe to optimize including population size and selection/crossover/mutation types.
+
+### Samples constructors
+
+There are several ways to create new testing samples from zero when u start with empty population or when u need new samples after [duplicates removing](#duplicates-removing) and [revolutions](#revolutions). 
+
+
+### Callbacks
+
+Now the package supports 2 different types of highly customized callbacks:
+* [simple callbacks](#callbacks)
+* [middle callbacks](#middle-callbacks)
+
 ## How to run
 
-Firstly, u should **import needed packages**. All available (but not always necessary) imports are:
+Firstly, u should **import needed packages**. 
+
+All available (but not always necessary) imports are:
 
 ```python
 import numpy as np
 
 # the only one required import
 from geneticalgorithm2 import GeneticAlgorithm2 as ga  # for creating and running optimization model
 
@@ -368,116 +422,89 @@
 from geneticalgorithm2 import plot_pop_scores  # for plotting population scores, if u want
 
 from geneticalgorithm2 import Callbacks  # simple callbacks (will be deprecated)
 
 from geneticalgorithm2 import Actions, ActionConditions, MiddleCallbacks  # middle callbacks
 ```
 
-Next step: **define minimized function** like
+Next step: **define the function to minimize**:
 
 ```python
 def function(X: np.ndarray) -> float: # X as 1d-numpy array
     return np.sum(X**2) + X.mean() + X.min() + X[0]*X[2] # some float result
 ```
 
-If u want to find *maximum*, use this idea:
-
-```python
-f_tmp = lambda arr: -target(arr)
-
-#
-# ... find global min
-#
-
-target_result = -global_min
-```
-
-Okay, also u should **create the bounds for each variable** (if exist) like here:
+Also u should **create the bounds for each variable** (if exist) such as:
 
 ```python
 var_bound = np.array([[0,10]]*3) # 2D numpy array with shape (dim, 2)
 
 # also u can use Sequence of Tuples (from version 6.3.0)
 var_bound = [
     (0, 10),
     (0, 10),
     (0, 10)
 ]
-
 ```
-U don't need to use variable boundaries only if variable type of each variable is boolean. This case will be converted to discret variables with bounds `(0, 1)`.
 
-After that **create a `geneticalgorithm2` (was imported early as ga) object**:
+**Important**. U don't need to use variable boundaries only if variable type of each variable is boolean. This case will be automatically converted to discrete variables with bounds `(0, 1)`.
+
+After that u **create a `GeneticAlgorithm2` (was imported early as ga) object**:
 
 ```python
-# style before 6.3.0 version (but still works)
-model = ga(
-    function, 
+model = ga( 
     dimension = 3, 
     variable_type='real', 
     variable_boundaries = var_bound,
-    function_timeout = 10,
     algorithm_parameters={
         'max_num_iteration': None,
         'population_size':100,
         'mutation_probability': 0.1,
         'mutation_discrete_probability': None,
         'elit_ratio': 0.01,
         'parents_portion': 0.3,
         'crossover_type':'uniform',
         'mutation_type': 'uniform_by_center',
         'mutation_discrete_type': 'uniform_discrete',
         'selection_type': 'roulette',
         'max_iteration_without_improv':None
     }
 )
+```
 
-# from version 6.3.0 it is equal to
+**Note**: it is not mandatory to write all possible `algorithm_parameters`, here it is done only to show u defaults. Also u can use `AlgorithmParams` (with typehints and docstrings) class instead of dicts:
 
-model = ga(
-    function, 
-    dimension = 3, 
-    variable_type='real', 
-    variable_boundaries = var_bound,
-    function_timeout = 10,
-    algorithm_parameters=AlgorithmParams(
-        max_num_iteration = None,
-        population_size = 100,
-        mutation_probability = 0.1,
-        mutation_discrete_probability = None,
-        elit_ratio = 0.01,
-        parents_portion = 0.3,
-        crossover_type = 'uniform',
-        mutation_type = 'uniform_by_center',
-        mutation_discrete_type = 'uniform_discrete',
-        selection_type = 'roulette',
-        max_iteration_without_improv = None
-    )
+```python
+algorithm_parameters=AlgorithmParams(
+    max_num_iteration=None,
+    population_size=100,
+    mutation_probability=0.1,
+    mutation_discrete_probability=None,
+    elit_ratio=0.01,
+    parents_portion=0.3,
+    crossover_type='uniform',
+    mutation_type='uniform_by_center',
+    mutation_discrete_type='uniform_discrete',
+    selection_type='roulette',
+    max_iteration_without_improv=None
 )
-
-# or (with defaults)           
-model = ga(
-    function, dimension = 3, 
-    variable_type='real', 
-    variable_boundaries = var_bound,
-    function_timeout = 10,
-    algorithm_parameters=AlgorithmParams()
-)           
-
 ```
 
 **Run the search method**:
 
 ```python
 # all of this parameters are default
 result = model.run(
     no_plot = False, 
     progress_bar_stream = 'stdout',
     disable_printing = False,
 
+    function=function,
+    function_timeout=None,
+
     set_function = None, 
     apply_function_to_parents = False, 
     start_generation = None,
     studEA = False,
     mutation_indexes = None,
 
     init_creator = None,
@@ -494,359 +521,89 @@
     callbacks = [],
     middle_callbacks = [],
     time_limit_secs = None, 
     save_last_generation_as = None,
     seed = None
 )
 
-# best solution
+# best candidate
 print(result.variable)
 
 # best score
 print(result.score)
 
 # last generation
 print(result.last_generation)
 
 ```
 
 ## Constructor parameters
 
-* **function** (`Callable[[np.ndarray], float]`) - the given objective function to be minimized  
-NOTE: This implementation minimizes the given objective function. (For maximization multiply function by a negative sign: the absolute value of the output would be the actual objective function)
-        
-* **dimension** (`int`) - the number of decision variables
-        
-* **variable_type** (`Union[str, Sequence[str]]`) - 'bool' if all variables are Boolean; 'int' if all variables are integer; and 'real' if all variables are real value or continuous. For mixed types use sequence of string of type for each variable
-        
-* **variable_boundaries** (`Optional[Union[np.ndarray, Sequence[Tuple[float, float]]]]`) - Default None; leave it None if variable_type is 'bool'; otherwise provide an sequence of tuples of length two as boundaries for each variable; the length of the array must be equal dimension. 
-For example, `np.array([[0,100],[0,200]])` or `[(0, 100), (0, 200)]` determines lower boundary 0 and upper boundary 100 for first and upper boundary 200 for second variable where dimension is 2.
-        
-* **function_timeout** (`float`) - if the given function does not provide 
-output before function_timeout (unit is seconds) the algorithm raise error.
-For example, when there is an infinite loop in the given function. `None` means disabling
-        
-* **algorithm_parameters** (`Union[AlgorithmParams, Dict[str, Any]]`). Dictionary or AlgorithmParams object with fields:  
-    * @ **max_num_iteration** (`int/None`) - stopping criteria of the genetic algorithm (GA)  
-    * @ **population_size** (`int > 0`)   
-    * @ **mutation_probability** (`float in [0,1]`)
-    * @ **mutation_discrete_probability** (`float in [0,1]` or `None`)
-    * @ **elit_ration** (`float in [0,1]`) - part of elit objects in population; if > 0, there always will be 1 elit object at least  
-    * @ **parents_portion** (`float in [0,1]`) - part of parents from previous population to save in next population (including `elit_ration`)  
-    * @ **crossover_type** (`Union[str, Callable[[np.ndarray, np.ndarray], Tuple[np.ndarray, np.ndarray]]]`) - Default is `uniform`.
-    * @ **mutation_type** (`Union[str, Callable[[float, float, float], float]]`) - Default is `uniform_by_center`
-    * @ **mutation_discrete_type** (`Union[str, Callable[[int, int, int], int]]`) - Default is `uniform_discrete`
-    * @ **selection_type** (`Union[str, Callable[[np.ndarray, int], np.ndarray]]`) - Default is `roulette`
-    * @ **max_iteration_without_improv** (`int/None`) - maximum number of successive iterations without improvement. If `None` it is ineffective
+Have a look at https://pasaopasen.github.io/geneticalgorithm2/geneticalgorithm2/geneticalgorithm2.html#GeneticAlgorithm2.__init__
 
 ## Genetic algorithm's parameters
 
 ### AlgorithmParams object
 
-The parameters of GA is defined as a dictionary or `AlgorithmParams` object:
-
-```python
-
-algorithm_param = AlgorithmParams(
-                max_num_iteration = None,
-                population_size = 100,
-                mutation_probability = 0.1,
-                mutation_discrete_probability = None,
-                elit_ratio = 0.01,
-                parents_portion = 0.3,
-                crossover_type = 'uniform',
-                mutation_type = 'uniform_by_center',
-                mutation_discrete_type = 'uniform_discrete',
-                selection_type = 'roulette',
-                max_iteration_without_improv = None
-            )
-
-
-# old style with dictionary
-# sometimes it's easier to use this style
-# especially if u need to set only few params
-algorithm_param = {
-                   'max_num_iteration': None,
-                   'population_size':100,
-                   'mutation_probability': 0.1,
-                   'mutation_discrete_probability': None,
-                   'elit_ratio': 0.01,
-                   'parents_portion': 0.3,
-                   'crossover_type':'uniform',
-                   'mutation_type': 'uniform_by_center',
-                   'mutation_discrete_type': 'uniform_discrete',
-                   'selection_type': 'roulette',
-                   'max_iteration_without_improv':None
-                   }
-
-```
+The parameters of GA is defined as a dictionary or `AlgorithmParams` object: https://pasaopasen.github.io/geneticalgorithm2/geneticalgorithm2/data_types/algorithm_params.html
 
-To get actual default params use code:
+To get the global default params use code:
 ```python
 params = ga.default_params
 ```
 
-To get actual parameters of existing model use code:
+To get actual parameters of an existing model use code:
 ```python
 params = model.param
 ```
 
-An example of setting a new set of parameters for genetic algorithm and running `geneticalgorithm2` for our first simple example again:
-
-```python
-import numpy as np
-from geneticalgorithm2 import GeneticAlgorithm2 as ga
-
-
-def f(X):
-    return np.sum(X)
-
-
-varbound = [(0, 10)] * 3
-
-algorithm_param = {'max_num_iteration': 3000,
-                   'population_size': 100,
-                   'mutation_probability': 0.1,
-                   'mutation_discrete_probability': None,
-                   'elit_ratio': 0.01,
-                   'parents_portion': 0.3,
-                   'crossover_type': 'uniform',
-                   'mutation_type': 'uniform_by_center',
-                   'mutation_discrete_type': 'uniform_discrete',
-                   'selection_type': 'roulette',
-                   'max_iteration_without_improv': None}
-
-model = ga(function=f,
-           dimension=3,
-           variable_type='real',
-           variable_boundaries=varbound,
-           algorithm_parameters=algorithm_param
-           )
-
-model.run()
-```
-**Important**. U may use the small dictionary with only important parameters; other parameters will be default. It means the dictionary
-```js
-algorithm_param = {'max_num_iteration': 150,
-                   'population_size':1000}
-```
-is equal to:
-```js
-algorithm_param = {'max_num_iteration': 150,
-                   'population_size':1000,
-                   'mutation_probability': 0.1,
-                   'mutation_discrete_probability': None,
-                   'elit_ratio': 0.01,
-                   'parents_portion': 0.3,
-                   'crossover_type':'uniform',
-                   'mutation_type': 'uniform_by_center',
-                   'mutation_discrete_type': 'uniform_discrete',
-                   'selection_type': 'roulette',
-                   'max_iteration_without_improv':None}
-```
-
-But it is better to use `AlgorithmParams` object instead of dictionaries.
-
 ### Parameters of algorithm
 
-#### **Count parameters**
-
-* **max_num_iteration**: The termination criterion of GA. 
-If this parameter's value is `None` the algorithm sets maximum number of iterations automatically as a function of the dimension, boundaries, and population size. The user may enter any number of iterations that they want. It is highly recommended that the user themselves determines the **max_num_iterations** and not to use `None`. Notice that **max_num_iteration** has been changed to 3000 (it was already `None`). 
-
-* **population_size**: determines the number of trial solutions in each iteration.
-
-* **elit_ration**: determines the number of elites in the population. The default value is 0.01 (i.e. 1 percent). For example when population size is 100 and **elit_ratio** is 0.01 then there is one elite unit in the population. If this parameter is set to be zero then `geneticalgorithm2` implements a standard genetic algorithm instead of elitist GA. [See example](#standard-ga-vs-elitist-ga) of difference
-
-* **parents_portion**: the portion of population filled by the members of the previous generation (aka parents); default is 0.3 (i.e. 30 percent of population)
-
-* **max_iteration_without_improv**: if the algorithms does not improve the objective function over the number of successive iterations determined by this parameter, then GA stops and report the best found solution before the `max_num_iterations` to be met. The default value is `None`. 
-
 #### **Crossover**
 
-* **crossover_type**: there are several options including `'one_point'`, `'two_point'`, `'uniform'`, `'segment'`, `'shuffle'` crossover functions; default is `'uniform'` crossover. U also can use crossover as functions from `Crossover` class:
-    * `Crossover.one_point()`
-    * `Crossover.two_point()`
-    * `Crossover.uniform()`
-    * `Crossover.uniform_window(window = 7)`
-    * `Crossover.shuffle()`
-    * `Crossover.segment()`
-    * `Crossover.mixed(alpha = 0.5)` -- only for real variables
-    * `Crossover.arithmetic()` -- only for real variables
-    
-    Have a look at [crossovers' logic](#available-crossovers)
-
-    If u want, write your own crossover function using simple syntax:
-    ```python
-    def my_crossover(parent_a: np.ndarray, parent_b: np.ndarray):
-        # some code
-        return child_1, child_2
-    ```
+https://pasaopasen.github.io/geneticalgorithm2/geneticalgorithm2/crossovers.html
 
 #### **Mutation**
 
-* **mutation_probability**: determines the chance of each gene in each individual solution to be replaced by a random value. Works for continuous variables or for all variables if **mutation_discrete_probability** is `None`
-
-* **mutation_discrete_probability**: works like **mutation_probability** but for discrete variables. If `None`, will be changed to **mutation_probability** value; so just don't specify this parameter if u don't need special mutation behavior for discrete variables
-
-* **mutation_type**: there are several options (only for real variables) including `'uniform_by_x'`, `'uniform_by_center'`, `'gauss_by_x'`, `'gauss_by_center'`; default is `'uniform_by_center'`. U also can use mutation as functions from `Mutations` class:
-    * `Mutations.gauss_by_center(sd = 0.2)`
-    * `Mutations.gauss_by_x(sd = 0.1)`
-    * `Mutations.uniform_by_center()`
-    * `Mutations.uniform_by_x()`
-
-    (If u want) write your mutation function using syntax:
-    ```python
-    def my_mutation(current_value: float, left_border: float, right_border: float) -> float:
-        # some code
-        return new_value 
-    ```
-
-* **mutation_discrete_type**: now there is only one option for discrete variables mutation: `uniform_discrete` (`Mutations.uniform_discrete()`) which works like `uniform_by_center` real mutation but with integer numbers. Anyway, this option was included at version 6.7.0 to support custom discrete mutations if u need it. For using custom mutation just set this parameter to function like
-  ```python
-    def my_mutation(current_value: int, left_border: int, right_border: int) -> int:
-        # some code
-        return new_value 
-  ```
+https://pasaopasen.github.io/geneticalgorithm2/geneticalgorithm2/mutations.html
 
 #### **Selection**
 
-* **selection_type**: there are several options (only for real) including `'fully_random'` (just for fun), `'roulette'`, `'stochastic'`, `'sigma_scaling'`, `'ranking'`, `'linear_ranking'`, `'tournament'`; default is `roulette`. U also can use selection as functions from `Selection` class:
-    * `Selection.fully_random()`
-    * `Selection.roulette()`
-    * `Selection.stochastic()`
-    * `Selection.sigma_scaling(epsilon = 0.05)`
-    * `Selection.ranking()`
-    * `Selection.linear_ranking(selection_pressure = 1.5)`
-    * `Selection.tournament(tau = 2)`
-
-    If u want, write your selection function using syntax:
-    ```python
-    def my_mutation(sorted_scores: np.ndarray, parents_count: int):
-        # some code
-        return array_of_parents_indexes 
-    ```
-![](tests/output/selections.png)
-
-## Methods and Properties of model:
-
-The main method if **run()**. It has parameters:
-
-* **no_plot** (`bool`) - do not plot results using matplotlib by default
-
-* **progress_bar_stream** (`Optional[str]`) - `'stdout'` to print progress bar to `stdout`, `'stderr'` for `stderr`, `None` to disable progress bar (also it can be faster by 10-20 seconds)
-
-* **disable_printing** (`bool`) - don't print any text (except progress bar)
-
-* **set_function** (`Optional[Callable[[np.ndarray], np.ndarray]]`): 2D-array -> 1D-array function, which applies to matrix of population (size (samples, dimension)) to estimate their values ("scores" in some sense)
-        
-* **apply_function_to_parents** (`bool`) - apply function to parents from previous generation (if it's needed), it can be needed at working with games agents, but for other tasks will just waste time
-
-* **start_generation** (`Union[str, Dict[str, np.ndarray], Generation, np.ndarray, Tuple[Optional[np.ndarray], Optional[np.ndarray]]]`) -- one of cases ([take a look](#how-to-initialize-start-population-how-to-continue-optimization-with-new-run)):
-  *  `Generation` object
-  *  dictionary with structure `{'variables':2D-array of samples, 'scores': function values on samples}` (if `'scores'` value is `None` the scores will be compute)
-  *  path to `.npz` file (`str`) with saved generation  
-  *  `np.ndarray` (with shape `(samples, dim)` or `(samples, dim+1)`) 
-  *  tuple of `np.ndarray`s / `None`. 
-
-* **studEA** (`bool`) - using stud EA strategy (crossover with best object always). Default is false. [Take a look](#standard-crossover-vs-stud-ea-crossover)
-* **mutation_indexes** (`Optional[Union[Sequence[int], Set[int]]]`) - indexes of dimensions where mutation can be performed (all dimensions by default). [Example](tests/mut_indexes.py)
-
-* **init_creator**: (`Optional[Callable[[], np.ndarray]]`), the function creates population samples. By default -- random uniform for real variables and random uniform for int. [Example](#optimization-with-oppositions)
-* **init_oppositors**: (`Optional[Sequence[Callable[[np.ndarray], np.ndarray]]]`) -- the list of oppositors creates oppositions for base population. No by default. [Example](#optimization-with-oppositions)
-* **duplicates_oppositor**: `Optional[Callable[[np.ndarray], np.ndarray]]`, oppositor for applying after duplicates removing. By default -- using just random initializer from creator. [Example](#duplicates-removing)
-* **remove_duplicates_generation_step**: `None/int`, step for removing duplicates (have a sense with discrete tasks). No by default. [Example](#duplicates-removing)
-* **revolution_oppositor** = `Optional[Callable[[np.ndarray], np.ndarray]]`, oppositor for revolution time. No by default. [Example](#revolutions)
-* **revolution_after_stagnation_step** = `None/int`, create revolution after this generations of stagnation. No by default. [Example](#revolutions)
-* **revolution_part** (`float`): the part of generation to being oppose. By default is 0.3. [Example](#revolutions)
-
-* **population_initializer** (`Tuple[int, Callable[[np.ndarray, np.ndarray], Tuple[np.ndarray, np.ndarray]]]`) -- object for actions at population initialization step to create better start population. [Take a look](#creating-better-start-population)
-
-* **stop_when_reached** (`Optional[float]`) -- stop searching after reaching this value (it can be potential minimum or something else)
-
-* **callbacks** (`Optional[Sequence[Callable[[int, List[float],  np.ndarray, np.ndarray], None]]]`) - list of callback functions with structure:
-  ```python 
-  def callback(generation_number, report_list, last_population_as_2D_array, last_population_scores_as_1D_array):
-      #
-      # do some action
-      #
-  ```
-    See [example of using callbacks](tests/callbacks.py). There are several callbacks in `Callbacks` class, such as:
-    * `Callbacks.SavePopulation(folder, save_gen_step = 50, file_prefix = 'population')`
-    * `Callbacks.PlotOptimizationProcess(folder, save_gen_step = 50, show = False, main_color = 'green', file_prefix = 'report')`
-
-* **middle_callbacks** (`Sequence`) - list of functions made `MiddleCallbacks` class (large opportunity, please, have a look at [this](#middle-callbacks)) 
-
-
-* **time_limit_secs** (`Optional[float]`) - limit time of working (in seconds). If `None`, there is no time limit (limit only for count of generation and so on). See [little example of using](tests/time_limit.py). Also there is simple conversion function for conversion some time in seconds:
-  ```python
-  from truefalsepython import time_to_seconds
-
-  total_seconds = time_to_seconds(
-      days = 2, # 2 days
-      hours = 13, # plus 13 hours
-      minutes = 7, # plus 7 minutes
-      seconds = 44 # plus 44 seconds
-  )
-  ```
-
-* **save_last_generation_as** (`Optional[str]`) - path to `.npz` file for saving last_generation as numpy dictionary like `{'population': 2D-array, 'scores': 1D-array}`, `None` if doesn't need to save in file; [take a look](#how-to-initialize-start-population-how-to-continue-optimization-with-new-run)
-
-* **seed** (`Optional[int]`) - random seed (None is doesn't matter)
-
-It would be more logical to use params like `studEA` as an algorithm param, but `run()`-way can be more comfortable for real using.
-
-    
-**output**:  
-  
-* `result`: is a wrap on last generation with fields:
-  * `last_generation` -- `Generation` object of last generation
-  * `variable` -- best unit of last generation
-  * `score` -- metric of the best unit
-  
-* `report`: is a record of the progress of the algorithm over iterations. Also u can specify to report not only best values. [Go to](#report-checker)
-
+https://pasaopasen.github.io/geneticalgorithm2/geneticalgorithm2/selections.html
 
+## Methods and Properties of model
 
+Have a look at https://pasaopasen.github.io/geneticalgorithm2/geneticalgorithm2/geneticalgorithm2.html#GeneticAlgorithm2.run
 
 # Examples for beginner
 
 ## A minimal example 
-Assume we want to find a set of `X = (x1,x2,x3)` that minimizes function `f(X) = x1 + x2 + x3` where `X` can be any real number in `[0, 10]`.
 
-This is a trivial problem and we already know that the answer is `X = (0,0,0)` where `f(X) = 0`.  
+Assume we want to find a set of `X = (x1, x2, x3)` that minimizes function `f(X) = x1 + x2 + x3` where `X` can be any real number in `[0, 10]`.
+
+This is a trivial problem and we already know that the answer is `X = (0, 0, 0)` where `f(X) = 0`.  
 
-We just use this simple example to see how to implement geneticalgorithm2. First we import geneticalgorithm2 and [numpy](https://numpy.org). Next, we define 
-function `f` which we want to minimize and the boundaries of the decision variables. Then simply geneticalgorithm2 is called to solve the defined optimization problem as follows:
+We just use this simple example to show how to implement it with `geneticalgorithm2`. First we import `geneticalgorithm2` and [numpy](https://numpy.org). Next, we define 
+function `f` which we want to minimize and the boundaries of the decision variables. Then simply `geneticalgorithm2` is called to solve the defined optimization problem as follows:
 
 ```python
 import numpy as np
 from geneticalgorithm2 import GeneticAlgorithm2 as ga
 
 
 def f(X):
     return np.sum(X)
 
 
 varbound = [[0, 10]] * 3
 
-model = ga(function=f, dimension=3, variable_type='real', variable_boundaries=varbound)
+model = ga(dimension=3, variable_type='real', variable_boundaries=varbound)
 
-model.run()
+model.run(function=f)
 ```
-
-    
-**geneticalgorithm2 has some arguments**:   
-1. Obviously the first argument is the function `f` we already defined.  
-2. Our problem has three variables so we set dimension equal `3`.   
-3. Variables are real (continuous) so we use string `'real'` to notify the type of 
-variables (geneticalgorithm2 accepts other types including boolean, integers and 
-mixed; see other examples).  
-1. Finally, we input `varbound` which includes the boundaries of the variables. 
-Note that the length of variable_boundaries must be equal to dimension.
   
 If you run the code, you should see a progress bar that shows the progress of the 
 genetic algorithm (GA) and then the solution, objective function value and the convergence curve as follows:
 
 ![](https://github.com/PasaOpasen/geneticalgorithm2/blob/master/genetic_algorithm_convergence.gif)
 
 Also we can access to the best answer of the defined optimization problem found by GA as a dictionary and a report of the progress of the genetic algorithm. 
@@ -868,20 +625,19 @@
 import numpy as np
 from geneticalgorithm2 import GeneticAlgorithm2 as ga
 
 
 def f(X):
     return np.sum(X)
 
-
 varbound = [[0, 10]] * 3
 
-model = ga(function=f, dimension=3, variable_type='int', variable_boundaries=varbound)
+model = ga(dimension=3, variable_type='int', variable_boundaries=varbound)
 
-model.run()
+model.run(function=f)
 ```
 So, as it is seen the only difference is that for `variable_type` we use string `'int'`. 
 
 ## The simple example with Boolean variables
 
 Considering the problem given in the simple example above.
 Now assume all variables are boolean instead of real or integer. So `X` can be either zero or one. Also instead of three let's have 30 variables.
@@ -891,48 +647,47 @@
 import numpy as np
 from geneticalgorithm2 import GeneticAlgorithm2 as ga
 
 
 def f(X):
     return np.sum(X)
 
+model = ga(dimension=30, variable_type='bool')
 
-model = ga(function=f, dimension=30, variable_type='bool')
-
-model.run()
+model.run(function=f)
 ```
-
 Note for variable_type we use string `'bool'` when all variables are boolean.  
 Note that when variable_type equal `'bool'` there is no need for `variable_boundaries` to be defined.
 
 ## The simple example with mixed variables
 
 Considering the problem given in the the simple example above where we want to minimize `f(X) = x1 + x2 + x3`. 
-Now assume `x1` is a real (continuous) variable in `[0.5,1.5]`, `x2` is an integer variable in `[1,100]`, and `x3` is a boolean variable that can be either zero or one.
-We already know that the answer is `X = (0.5,1,0)` where `f(X) = 1.5`
+Now assume `x1` is a real (continuous) variable in `[0.5; 1.5]`, `x2` is an integer variable in `[1;100]`, and `x3` is a boolean variable that can be either zero or one.
+We already know that the answer is `X = (0.5, 1, 0)` where `f(X) = 1.5`.
 We implement geneticalgorithm2 as the following:
 
 ```python
 import numpy as np
 from geneticalgorithm2 import GeneticAlgorithm2 as ga
 
 
 def f(X):
     return np.sum(X)
 
 
 varbound = [[0.5, 1.5], [1, 100], [0, 1]]
 vartype = ('real', 'int', 'int')
-model = ga(function=f, dimension=3, variable_type=vartype, variable_boundaries=varbound)
+model = ga(dimension=3, variable_type=vartype, variable_boundaries=varbound)
 
-model.run()
+model.run(function=f)
 ```
 
 ## Optimization problems with constraints
-In all above examples, the optimization problem was unconstrained. Now consider that we want to minimize `f(X) = x1+x2+x3` where `X` is a set of real variables in `[0, 10]`. Also we have an extra constraint so that sum of `x1` and `x2` is equal or greater than 2. The minimum of `f(X)` is 2.
+
+In all above examples, the optimization problem was unconstrained. Now consider that we want to minimize `f(X) = x1+x2+x3` where `X` is a set of real variables in `[0; 10]`. Also we have an extra constraint so that sum of `x1` and `x2` is equal or greater than 2. The minimum of `f(X)` is 2.
 In such a case, a trick is to define penalty function. Hence we use the code below:
 
 ```python
 import numpy as np
 from geneticalgorithm2 import GeneticAlgorithm2 as ga
 
 
@@ -941,34 +696,34 @@
     if X[0] + X[1] < 2:
         pen = 500 + 1000 * (2 - X[0] - X[1])
     return np.sum(X) + pen
 
 
 varbound = [[0, 10]] * 3
 
-model = ga(function=f, dimension=3, variable_type='real', variable_boundaries=varbound)
+model = ga(dimension=3, variable_type='real', variable_boundaries=varbound)
 
-model.run()
+model.run(function=f)
 
 ```
 As seen above we add a penalty to the objective function whenever the constraint is not met.  
 
 Some hints about how to define a penalty function:  
 
 1. Usually you may use a constant greater than the maximum possible value of the objective function if the maximum is known or if we have a guess of that. Here the highest possible value of our function is 300 (i.e. if all variables were 10, `f(X)=300`). So I chose a constant of 500. So, if a trial solution is not in the feasible region even though its objective function may be small, the penalized objective function (fitness function) is worse than any feasible solution.
 2. Use a coefficient big enough and multiply that by the amount of violation. This helps the algorithm learn how to approach feasible domain.
 3. How to define penalty function usually influences the convergence rate of an evolutionary algorithm. In my [book on metaheuristics and evolutionary algorithms](https://www.wiley.com/en-us/Meta+heuristic+and+Evolutionary+Algorithms+for+Engineering+Optimization-p-9781119386995) you can learn more about that. 
 4. Finally after you solved the problem test the solution to see if boundaries are met. If the solution does not meet constraints, it shows that a bigger penalty is required. However, in problems where optimum is exactly on the boundary of the feasible region (or very close to the constraints) which is common in some kinds of problems, a very strict and big penalty may prevent the genetic algorithm to approach the optimal region. In such a case designing an appropriate penalty function might be more challenging. Actually what we have to do is to design a penalty function that let the algorithm searches unfeasible domain while finally converge to a feasible solution. Hence you may need more sophisticated penalty functions. But in most cases the above formulation work fairly well.
 
 ## Middle example: select fixed count of objects from set
 
 For some task u need to think a lot and create good specific crossover or mutation functions. For example, take a look at this problem:
-
+```
     From set like X = {x1, x2, x3, ..., xn} u should select only k objects which get the best function value
-
+```
 U can do it using this code:
 
 ```python
 import numpy as np
 from geneticalgorithm2 import GeneticAlgorithm2 as ga
 
 subset_size = 20  # how many objects we can choose
@@ -1010,35 +765,39 @@
         children[:, np.array(list(intersect))] = 1
     children[0, child_inds[:int(child_inds.size / 2)]] = 1
     children[1, child_inds[int(child_inds.size / 2):]] = 1
 
     return children[0, :], children[1, :]
 
 
-model = ga(function=f,
-           dimension=objects_count,
-           variable_type='bool',
-           algorithm_parameters={
-               'max_num_iteration': 500,
-               'mutation_probability': 0,  # no mutation, just crossover
-               'elit_ratio': 0.05,
-               'parents_portion': 0.3,
-               'crossover_type': my_crossover,
-               'max_iteration_without_improv': 20
-           }
-           )
+model = ga(
+    dimension=objects_count,
+    variable_type='bool',
+    algorithm_parameters={
+        'max_num_iteration': 500,
+        'mutation_probability': 0,  # no mutation, just crossover
+        'elit_ratio': 0.05,
+        'parents_portion': 0.3,
+        'crossover_type': my_crossover,
+        'max_iteration_without_improv': 20
+    }
+)
 
-model.run(no_plot=False, start_generation=(start_generation, None))
+model.run(
+    function=f,
+    no_plot=False, 
+    start_generation=(start_generation, None)
+)
 ```
 
 # U should know these features
 
 ## Available crossovers
 
-For two example parents (*one with ones* and *one with zeros*) next crossovers will give same children ([examples](tests/crossovers_examples.py)): 
+For two example parents (*one with ones* and *one with zeros*) next crossovers will give same children ([examples](examples/crossovers_examples.py)): 
 
 * **one_point**:
 
 |0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 1 | 1 | 1 | 1 | 1 | 1 | 1|
 |:---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---:|
 |1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 0 | 0 | 0 | 0 | 0 | 0 | 0|
 
@@ -1080,61 +839,47 @@
 
 * **mixed**:
 
 |0.63 | 0.84 | 1.1 | 0.73 | 0.67 | -0.19 | 0.3 | 0.72 | -0.18 | 0.61 | 0.84 | 1.14 | 1.36 | -0.37 | -0.19|
 |:---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---:|
 |0.51 | 0.58 | 0.43 | 0.42 | 0.55 | 0.49 | 0.57 | 0.48 | 0.46 | 0.56 | 0.56 | 0.54 | 0.44 | 0.51 | 0.4|
 
+## Available selections
+
+![](examples/output/selections.png)
+
 
 ## Function timeout
 
-**geneticalgorithm2** is designed such that if the given function does not provide
-any output before timeout (the default value is 10 seconds), the algorithm
-would be terminated and raise the appropriate error. 
-
-In such a case make sure the given function
-works correctly (i.e. there is no infinite loop in the given function). Also if the given function takes more than 10 seconds to complete the work
-make sure to increase function_timeout in arguments.
+**geneticalgorithm2** inherited several features from `geneticalgorithm` package sush as that if the given function does not provide any output before timeout, the algorithm would be terminated and raise the appropriate error. 
+
+In such a case make sure the given function works correctly (i.e. there is no infinite loop in the given function). Also if the given function takes more than 10 seconds to complete the work
+make sure to increase `function_timeout` in arguments.
 
 ## Standard GA vs. Elitist GA
 
 The convergence curve of an elitist genetic algorithm is always non-increasing. So, the best ever found solution is equal to the best solution of the last iteration. However, the convergence curve of a standard genetic algorithm is different. If `elit_ratio` is zero geneticalgorithm2 implements a standard GA. The output of geneticalgorithm2 for standard GA is the best ever found solution not the solution of the last iteration. The difference between the convergence curve of standard GA and elitist GA is shown below:
 
-![](tests/output/standard_vs_elitist.png)
+![](examples/output/standard_vs_elitist.png)
 
 ## Standard crossover vs. stud EA crossover
 
 [Stud EA](https://link.springer.com/chapter/10.1007%2FBFb0056910) is the idea of using crossover always with best object. So one of two parents is always the best object of population. It can help us in a lot of tasks!
 
-![](tests/output/studEA.png)
+![](examples/output/studEA.png)
 
 ## Creating better start population
 
-There is `Population_initializer(select_best_of = 4, local_optimization_step = 'never', local_optimizer = None)` object for creating better start population. It has next arguments:
-
-* `select_best_of` (`int`) -- select `1/select_best_of` best part of start population. For example, for `select_best_of = 4` and `population_size = N` will be selected N best objects from 5N generated objects (if `start_generation = None`). If `start_generation` is not None, it will be selected best `size(start_generation)/N`  objects
-
-* `local_optimization_step` (`str`) -- when should we do local optimization? Available values:
-    
-    * `'never'` -- don't do local optimization
-    * `'before_select'` -- before selection best N objects (example: do local optimization for 5N objects and select N best results)
-    * `'after_select'` -- do local optimization on best selected N objects
-
-* `local_optimizer` (function) -- local optimization function like:
-    ```python
-    def loc_opt(object_as_array, current_score):
-        # some code
-        return better_object_as_array, better_score
-    ```
+There is `get_population_initializer(select_best_of = 4, local_optimization_step = 'never', local_optimizer = None)` function for creating start population creators. Take a look at [its docs](https://pasaopasen.github.io/geneticalgorithm2/geneticalgorithm2/population_initializer.html)
 
 ### Select best N of kN
 
 This little option can help u especially with multimodal tasks. 
 
-![](tests/output/init_best_of.png)
+![](examples/output/init_best_of.png)
 
 ### Do local optimization
 
 We can apply some local optimization on start generation before starting GA search. It can be some gradient descent or hill climbing and so on. Also we can apply it before selection best objects (on entire population) or after (on best part of population) and so forth.
 
 In next example I'm using my [DiscreteHillClimbing](https://github.com/PasaOpasen/DiscreteHillClimbing) algorithm for local optimization my discrete task:
 
@@ -1155,71 +900,77 @@
 
 iterations = 100
 
 varbound = [[-100, 100]] * 15
 
 available_values = [np.arange(-100, 101)] * 15
 
-my_local_optimizer = lambda arr, score: Hill_Climbing_descent(function=f, available_predictors_values=available_values,
-                                                              max_function_evals=50, start_solution=arr)
+my_local_optimizer = lambda arr, score: Hill_Climbing_descent(
+    function=f, available_predictors_values=available_values,
+    max_function_evals=50, start_solution=arr
+)
 
-model = ga(function=f, dimension=varbound.shape[0],
-           variable_type='int',
-           variable_boundaries=varbound,
-           algorithm_parameters={
-               'max_num_iteration': iterations,
-               'population_size': 400
-           })
+model = ga(
+    dimension=varbound.shape[0],
+    variable_type='int',
+    variable_boundaries=varbound,
+    algorithm_parameters={
+        'max_num_iteration': iterations,
+        'population_size': 400
+    }
+)
 
 for time in ('before_select', 'after_select', 'never'):
-    model.run(no_plot=True,
-              population_initializer=get_population_initializer(
-                  select_best_of=3,
-                  local_optimization_step=time,
-                  local_optimizer=my_local_optimizer
-              )
-              )
+    model.run(
+        function=f
+        no_plot=True,
+        population_initializer=get_population_initializer(
+            select_best_of=3,
+            local_optimization_step=time,
+            local_optimizer=my_local_optimizer
+        )
+    )
 
     plt.plot(model.report, label=f"local optimization time = '{time}'")
 
 plt.xlabel('Generation')
 plt.ylabel('Minimized function (40 simulations average)')
 plt.title('Selection best N object before running GA')
 plt.legend()
 ```
 
-![](tests/output/init_local_opt.png)
+![](examples/output/init_local_opt.png)
 
 ### Optimization with oppositions
 
-Also u can create start population with [oppositions](https://github.com/PasaOpasen/opp-op-pop-init). See [example of code](tests/best_of_N_with_opp.py)
+Also u can create start population with [oppositions](https://github.com/PasaOpasen/opp-op-pop-init). See [example of code](examples/best_of_N_with_opp.py)
 
-![](tests/output/init_best_of_opp.png)
+![](examples/output/init_best_of_opp.png)
 
 ## Revolutions
 
-U can create [revolutions in your population](https://github.com/PasaOpasen/opp-op-pop-init) after some stagnation steps. It really can help u for some tasks. See [example](tests/revolution.py)
+U can create [revolutions in your population](https://github.com/PasaOpasen/opp-op-pop-init) after some stagnation steps. It really can help u for some tasks. See [example](examples/revolution.py)
 
-![](tests/output/revolution.png)
+![](examples/output/revolution.png)
 
 
 ## Duplicates removing
 
-If u remove duplicates each `k` generations, u can speed up the optimization process ([example](tests/remove_dups.py))
+If u remove duplicates each `k` generations, u can speed up the optimization process ([example](examples/remove_dups.py))
 
-![](tests/output/remove_dups.png)
+![](examples/output/remove_dups.png)
 
 ## Cache
 
 It can be useful for run-speed to use cache with *some discrete tasks*. For this u can import `np_lru_cache` decorator and use it like here:
 
 ```python
 import np_lru_cache
 
-@np_lru_cache(maxsize = some_size)
+@np_lru_cache(maxsize=some_size)
 def minimized_func(arr):
     # code
     return result
 
 #
 # run
 #    algorithm
@@ -1245,34 +996,39 @@
 def f(X):
     return 50 * np.sum(X) - np.sum(np.sqrt(X) * np.sin(X))
 
 
 dim = 25
 varbound = [[0, 10]] * dim
 
-model = ga(function=f, dimension=dim,
-           variable_type='real', variable_boundaries=varbound,
-           algorithm_parameters={
-               'max_num_iteration': 600
-           }
-           )
+model = ga(
+    dimension=dim,
+    variable_type='real', 
+    variable_boundaries=varbound,
+    algorithm_parameters={
+        'max_num_iteration': 600
+    }
+)
 
 # here model exists and has checked_reports field
 # now u can append any functions to report
 
 model.checked_reports.extend(
     [
         ('report_average', np.mean),
         ('report_25', lambda arr: np.quantile(arr, 0.25)),
         ('report_50', np.median)
     ]
 )
 
 # run optimization process
-model.run(no_plot=False)
+model.run(
+    function=f,
+    no_plot=False
+)
 
 # now u have not only model.report but model.report_25 and so on
 
 # plot reports
 names = [name for name, _ in model.checked_reports[::-1]]
 plot_several_lines(
     lines=[getattr(model, name) for name in names],
@@ -1280,15 +1036,15 @@
     labels=['median value', '25% quantile', 'mean of population', 'best pop score'],
     linewidths=(1, 1.5, 1, 2),
     title="Several custom reports with base reports",
     save_as='./output/report.png'
 )
 ```
 
-![](tests/output/report.png)
+![](examples/output/report.png)
 
 As u see, u should append tuple `(name of report, func to evaluate report)` to `model.checked_report`. It's highly recommended to start this name with `report_` (e. g. `report_my_median`). And the function u use will get 1D-numpy *sorted* array of population scores.
 
 
 ## Middle callbacks
 
 There is an amazing way to control optimization process using `MiddleCallbacks` class. Just learn next logic:
@@ -1339,19 +1095,19 @@
 
 To combine `action` and `condition` to callback, just use `MiddleCallbacks.UniversalCallback(action, condition)` methods.
 
 
 There are also next high-level useful callbacks:
 
 * `MiddleCallbacks.ReduceMutationGen(reduce_coef = 0.9, min_mutation = 0.005, reduce_each_generation = 50, reload_each_generation = 500)`
-* `MiddleCallbacks.GeneDiversityStats(step_generations_for_plotting:int = 10)` -- plots some duplicates statistics each gen ([example](/tests/plot_diversities.py))
+* `MiddleCallbacks.GeneDiversityStats(step_generations_for_plotting:int = 10)` -- plots some duplicates statistics each gen ([example](/examples/plot_diversities.py))
 ![](diversity.gif)
 
 
-See [code example](tests/small_middle_callbacks.py)
+See [code example](examples/small_middle_callbacks.py)
 
 ## How to compare efficiency of several versions of GA optimization
 
 To compare efficiency of several versions of GA optimization (such as several values of several hyperparameters or including/excepting some actions like oppositions) u should make some count of simulations and compare results using some statistical test. I have realized this logic [here](https://github.com/PasaOpasen/ab-testing-results-difference) 
 
 ## Hints on how to adjust genetic algorithm's parameters (from `geneticalgorithm` package)
 
@@ -1557,91 +1313,91 @@
 
 # Examples pretty collection
 
 ## Optimization test functions
 
 Here there is the implementation of `geneticalgorithm2` for some benchmark problems. Test functions are got from my [`OptimizationTestFunctions`](https://github.com/PasaOpasen/OptimizationTestFunctions) package. 
 
-The code for optimizations process is same for each function and is contained [in file](tests/optimization_test_functions.py).
+The code for optimizations process is same for each function and is contained [in file](examples/optimization_test_functions.py).
 
 ### [Sphere](https://github.com/PasaOpasen/OptimizationTestFunctions#sphere)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Sphere.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Sphere.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Sphere.png)
 
 ### [Ackley](https://github.com/PasaOpasen/OptimizationTestFunctions#ackley)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Ackley.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Ackley.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Ackley.png)
 
 ### [AckleyTest](https://github.com/PasaOpasen/OptimizationTestFunctions#ackleytest)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20AckleyTest.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20AckleyTest.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20AckleyTest.png)
 
 ### [Rosenbrock](https://github.com/PasaOpasen/OptimizationTestFunctions#rosenbrock)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Rosenbrock.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Rosenbrock.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Rosenbrock.png)
 
 ### [Fletcher](https://github.com/PasaOpasen/OptimizationTestFunctions#fletcher)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Fletcher.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Fletcher.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Fletcher.png)
 
 ### [Griewank](https://github.com/PasaOpasen/OptimizationTestFunctions#griewank)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Griewank.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Griewank.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Griewank.png)
 
 ### [Penalty2](https://github.com/PasaOpasen/OptimizationTestFunctions#penalty2)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Penalty2.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Penalty2.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Penalty2.png)
 
 ### [Quartic](https://github.com/PasaOpasen/OptimizationTestFunctions#quartic)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Quartic.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Quartic.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Quartic.png)
 
 ### [Rastrigin](https://github.com/PasaOpasen/OptimizationTestFunctions#rastrigin)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Rastrigin.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Rastrigin.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Rastrigin.png)
 
 ### [SchwefelDouble](https://github.com/PasaOpasen/OptimizationTestFunctions#schwefeldouble)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20SchwefelDouble.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20SchwefelDouble.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20SchwefelDouble.png)
 
 ### [SchwefelMax](https://github.com/PasaOpasen/OptimizationTestFunctions#schwefelmax)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20SchwefelMax.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20SchwefelMax.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20SchwefelMax.png)
 
 ### [SchwefelAbs](https://github.com/PasaOpasen/OptimizationTestFunctions#schwefelabs)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20SchwefelAbs.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20SchwefelAbs.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20SchwefelAbs.png)
 
 ### [SchwefelSin](https://github.com/PasaOpasen/OptimizationTestFunctions#schwefelsin)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20SchwefelSin.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20SchwefelSin.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20SchwefelSin.png)
 
 ### [Stairs](https://github.com/PasaOpasen/OptimizationTestFunctions#stairs)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Stairs.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Stairs.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Stairs.png)
 
 ### [Abs](https://github.com/PasaOpasen/OptimizationTestFunctions#abs)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Abs.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Abs.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Abs.png)
 
 ### [Michalewicz](https://github.com/PasaOpasen/OptimizationTestFunctions#michalewicz)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Michalewicz.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Michalewicz.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Michalewicz.png)
 
 ### [Scheffer](https://github.com/PasaOpasen/OptimizationTestFunctions#scheffer)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Scheffer.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Scheffer.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Scheffer.png)
 
 ### [Eggholder](https://github.com/PasaOpasen/OptimizationTestFunctions#eggholder)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Eggholder.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Eggholder.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Eggholder.png)
 
 ### [Weierstrass](https://github.com/PasaOpasen/OptimizationTestFunctions#weierstrass)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Weierstrass.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Weierstrass.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Weierstrass.png)
 
 
 
 ## Using GA in reinforcement learning
 
 See [example of using GA optimization with keras neural networks](https://www.kaggle.com/demetrypascal/opengym-tasks-using-keras-and-geneticalgorithm2) for solving OpenGym tasks.
 
@@ -1723,17 +1479,17 @@
           })
 # plot and save optimization process plot
 model.plot_results(save_as='plot_scores_process.png')
 
 # plot scores of last population
 model.plot_generation_scores(title='Population scores after ending of searching', save_as='plot_scores_end.png')
 ```
-![](tests/output/plot_scores_start.png)
-![](tests/output/plot_scores_process.png)
-![](tests/output/plot_scores_end.png)
+![](examples/output/plot_scores_start.png)
+![](examples/output/plot_scores_process.png)
+![](examples/output/plot_scores_end.png)
 
 
 
 ## How to specify evaluated function for all population?
 
 U can do it using `set_function` parameter into `run()` method.
```

### Comparing `geneticalgorithm2-6.9.0/README.rst` & `geneticalgorithm2-6.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `geneticalgorithm2-6.9.0/geneticalgorithm2/__init__.py` & `geneticalgorithm2-6.9.1/geneticalgorithm2/__init__.py`

 * *Files identical despite different names*

### Comparing `geneticalgorithm2-6.9.0/geneticalgorithm2/callbacks/data.py` & `geneticalgorithm2-6.9.1/geneticalgorithm2/callbacks/data.py`

 * *Files identical despite different names*

### Comparing `geneticalgorithm2-6.9.0/geneticalgorithm2/callbacks/middle.py` & `geneticalgorithm2-6.9.1/geneticalgorithm2/callbacks/middle.py`

 * *Files identical despite different names*

### Comparing `geneticalgorithm2-6.9.0/geneticalgorithm2/callbacks/simple.py` & `geneticalgorithm2-6.9.1/geneticalgorithm2/callbacks/simple.py`

 * *Files identical despite different names*

### Comparing `geneticalgorithm2-6.9.0/geneticalgorithm2/crossovers.py` & `geneticalgorithm2-6.9.1/geneticalgorithm2/crossovers.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 
 
 def get_copies(x: array1D, y: array1D) -> Tuple[array1D, array1D]:
     return x.copy(), y.copy()
 
 
 class Crossover:
-    """Crossover functions static class"""
+    """
+    Crossover functions static class
+    
+    Crossover creates 2 children from 2 parents someway, usually mixing the parents
+    """
 
     @staticmethod
     def crossovers_dict() -> Dict[str, CrossoverFunc]:
         return {
             n: getattr(Crossover, n)()
             for n in (
                 'one_point',
```

### Comparing `geneticalgorithm2-6.9.0/geneticalgorithm2/data_types/algorithm_params.py` & `geneticalgorithm2-6.9.1/geneticalgorithm2/data_types/algorithm_params.py`

 * *Files 26% similar despite different names*

```diff
@@ -30,28 +30,66 @@
 
 
 @dataclass
 class AlgorithmParams(DictLikeGetSet):
     """Base optimization parameters container"""
 
     max_num_iteration: Optional[int] = None
-    """max iterations count of the algorithm"""
+    """
+    max iterations count of the algorithm
+    
+    If this parameter's value is `None` the algorithm sets maximum number of iterations automatically 
+        as a function of the dimension, boundaries, and population size. 
+    The user may enter any number of iterations that they want. 
+    It is highly recommended that the user themselves determines 
+        the `max_num_iterations` and not to use `None`
+    """
+    
     max_iteration_without_improv: Optional[int] = None
-    """max iteration without progress"""
+    """
+    max iteration without progress
+    
+    if the algorithms does not improve 
+        the objective function over the number of successive iterations 
+            determined by this parameter, 
+            then GA stops and report the best found solution 
+            before the `max_num_iterations` to be met
+    """
 
     population_size: int = 100
+    """
+    determines the number of trial solutions in each iteration
+    """
 
     mutation_probability: float = 0.1
     mutation_discrete_probability: Optional[float] = None
+    """
+    works like `mutation_probability` but for discrete variables. 
+    
+    If `None`, will be assigned to `mutation_probability` value; 
+        so just don't specify this parameter 
+        if u don't need special mutation behavior for discrete variables
+    """
 
     #  deprecated
     crossover_probability: Optional[float] = None
 
     elit_ratio: float = 0.04
+    """
+    determines the number of elites in the population. 
+    
+    For example, when population size is 100 and `elit_ratio` is 0.01 
+        then there is 4 elite units in the population. 
+    If this parameter is set to be zero then `GeneticAlgorithm2` implements 
+        a standard genetic algorithm instead of elitist GA
+    """
     parents_portion: float = 0.3
+    """
+    the portion of population filled by the members of the previous generation (aka parents)
+    """
 
     crossover_type: Union[str, CrossoverFunc] = 'uniform'
     mutation_type: Union[str, MutationFloatFunc] = 'uniform_by_center'
     """mutation type for real variable"""
     mutation_discrete_type: Union[str, MutationIntFunc] = 'uniform_discrete'
     """mutation type for discrete variables"""
     selection_type: Union[str, SelectionFunc] = 'roulette'
```

### Comparing `geneticalgorithm2-6.9.0/geneticalgorithm2/data_types/aliases.py` & `geneticalgorithm2-6.9.1/geneticalgorithm2/data_types/aliases.py`

 * *Files identical despite different names*

### Comparing `geneticalgorithm2-6.9.0/geneticalgorithm2/data_types/generation.py` & `geneticalgorithm2-6.9.1/geneticalgorithm2/data_types/generation.py`

 * *Files identical despite different names*

### Comparing `geneticalgorithm2-6.9.0/geneticalgorithm2/data_types/result.py` & `geneticalgorithm2-6.9.1/geneticalgorithm2/data_types/result.py`

 * *Files identical despite different names*

### Comparing `geneticalgorithm2-6.9.0/geneticalgorithm2/geneticalgorithm2.py` & `geneticalgorithm2-6.9.1/geneticalgorithm2/geneticalgorithm2.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,31 +70,31 @@
         """whether the mutation is required"""
         return self.prob_mut > 0 or self.prob_mut_discrete > 0
 
     #region INIT
 
     def __init__(
         self,
-        function: FunctionToMinimize,
+        function: FunctionToMinimize = None,
 
-        dimension: int,
+        dimension: int = 0,
         variable_type: Union[VARIABLE_TYPE, Sequence[VARIABLE_TYPE]] = 'bool',
         variable_boundaries: Optional[Union[array2D, Sequence[Tuple[float, float]]]] = None,
 
         variable_type_mixed=None,
 
         function_timeout: Optional[float] = None,
         algorithm_parameters: Union[AlgorithmParams, Dict[str, Any]] = default_params
     ):
         """
         initializes the GA object and performs main checks
 
         Args:
-            function: the given objective function to be minimized
-            dimension: the number of decision variables, the population samples dimention
+            function: the given objective function to be minimized -- deprecated and moved to run() method
+            dimension: the number of decision variables, the population samples dimension
 
             variable_type: string means the variable type for all variables,
                 for mixed types use sequence of strings of type for each variable
 
             variable_boundaries: leave it None if variable_type is 'bool';
                 otherwise provide a sequence of tuples of length two as boundaries for each variable;
                 the length of the array must be equal dimension.
@@ -104,45 +104,47 @@
                     and dimension must be 2.
 
             variable_type_mixed -- deprecated
 
             function_timeout: if the given function does not provide
                 output before function_timeout (unit is seconds) the algorithm raises error.
                 For example, when there is an infinite loop in the given function.
-                `None` means disabling
+                `None` means disabling -- deprecated and moved to run()
 
             algorithm_parameters: AlgorithmParams object or usual dictionary with algorithm parameter;
                 it is not mandatory to provide all possible parameters
 
         Notes:
             - This implementation minimizes the given objective function.
             For maximization u can multiply the function by -1 (for instance): the absolute
                 value of the output would be the actual objective function
 
-            - If u want to use set_function only and maybe u dont have usual function,
-                just set the function to something like lambda x: 0 but set function_timeout=None too
-
         for more details and examples of implementation please visit:
             https://github.com/PasaOpasen/geneticalgorithm2
   
         """
 
         # all default fields
 
         # self.crossover: Callable[[np.ndarray, np.ndarray], Tuple[np.ndarray, np.ndarray]] = None
         # self.real_mutation: Callable[[float, float, float], float] = None
         # self.discrete_mutation: Callable[[int, int, int], int] = None
         # self.selection: Callable[[np.ndarray, int], np.ndarray] = None
 
+        self.result = None
+        self.best_function = None
+
         self.revolution_oppositor = None
         self.dup_oppositor = None
         self.creator = None
         self.init_oppositors = None
+
         self.f: Callable[[array1D], float] = None
         self.funtimeout: float = None
+
         self.set_function: Callable[[np.ndarray], np.ndarray] = None
 
         # self.dim: int = None
         self.var_bounds: List[Tuple[Union[int, float], Union[int, float]]] = None
         # self.indexes_int: np.ndarray = None
         # self.indexes_float: np.ndarray = None
 
@@ -187,28 +189,26 @@
             warnings.warn(
                 f"crossover_probability is deprecated and will be removed in version 7. "
                 f"Reason: it's old and has no sense"
             )
 
         #############################################################
         # input function
-        assert (callable(function)), "function must be callable!"
-        self.f = function
-
-        if function_timeout is not None and function_timeout > 0:
-            try:
-                from func_timeout import func_timeout, FunctionTimedOut
-            except ModuleNotFoundError:
-                raise ModuleNotFoundError(
-                    "function_timeout > 0 needs additional package func_timeout\n"
-                    "run `python -m pip install func_timeout`\n"
-                    "or disable this parameter: function_timeout=None"
-                )
-
-        self.funtimeout = None if function_timeout is None else float(function_timeout)
+        if function:
+            warnings.warn(
+                f"function is deprecated in init constructor and will be removed in version 7. "
+                f"Move this argument to run() method"
+            )
+            self._check_function(function)
+        if function_timeout:
+            warnings.warn(
+                f"function_timeout is deprecated in init constructor and will be removed in version 7. "
+                f"Move this argument to run() method"
+            )
+            self._check_function_timeout(function_timeout)
 
         #############################################################
         
         self.population_size = int(self.param.population_size)
         self._set_parents_count(self.param.parents_portion)
         self._set_elit_count(self.population_size, self.param.elit_ratio)
         assert self.parents_count >= self.elit_count, (
@@ -321,14 +321,32 @@
 
         max_it = self.param.max_iteration_without_improv
         if max_it is None:
             self.max_stagnations = self.max_iterations + 1
         else:
             self.max_stagnations = math.ceil(max_it)
 
+    def _check_function(self, function: Callable[[array1D], float]):
+        assert callable(function), "function must be callable!"
+        self.f = function
+
+    def _check_function_timeout(self, function_timeout: Optional[float]):
+
+        if function_timeout is not None and function_timeout > 0:
+            try:
+                from func_timeout import func_timeout, FunctionTimedOut
+            except ModuleNotFoundError:
+                raise ModuleNotFoundError(
+                    "function_timeout > 0 needs additional package func_timeout\n"
+                    "run `python -m pip install func_timeout`\n"
+                    "or disable this parameter: function_timeout=None"
+                )
+
+        self.funtimeout = None if function_timeout is None else float(function_timeout)
+
     #endregion
 
     #region REPORT
 
     def _set_report(self):
         """
         creates default report checker
@@ -428,14 +446,17 @@
         no_plot: bool = False,
         disable_printing: bool = False,
         progress_bar_stream: Optional[str] = 'stdout',
 
         # deprecated
         disable_progress_bar: bool = False,
 
+        function: FunctionToMinimize = None,
+        function_timeout: Optional[float] = None,
+
         set_function: SetFunctionToMinimize = None,
         apply_function_to_parents: bool = False,
         start_generation: GenerationConvertible = Generation(),
         studEA: bool = False,
         mutation_indexes: Optional[Iterable[int]] = None,
 
         init_creator: Optional[CreatorFunc] = None,
@@ -454,30 +475,40 @@
 
         stop_when_reached: Optional[float] = None,
         callbacks: Optional[Sequence[SimpleCallbackFunc]] = None,
         middle_callbacks: Optional[Sequence[MiddleCallbackFunc]] = None,  #+
         time_limit_secs: Optional[float] = None,
         save_last_generation_as: Optional[str] = None,
         seed: Optional[int] = None
-    ):
+    ) -> GAResult:
         """
         runs optimization process
 
         Args:
             no_plot: do not plot results using matplotlib by default
 
-            disable_printing: do not print log info of optimization process
+            disable_printing: do not print log info of optimization process (except progress bar)
 
-            progress_bar_stream: 'stdout', 'stderr' or None to disable progress bar
+            progress_bar_stream: 'stdout', 'stderr' or None to disable progress bar;
+                disabling progress bar can speed up the optimization process in many cases
 
             disable_progress_bar: deprecated
 
-            set_function: set function to be used instead of usual function
+            function: the given objective function (sample -> its score) to be minimized;
+
+            function_timeout: if the given function does not provide
+                output before function_timeout (unit is seconds) the algorithm raises error.
+                For example, when there is an infinite loop in the given function.
+                `None` means disabling
+
+            set_function: set function (all samples -> score per sample) to be used instead of usual function
+                (usually for optimization purposes)
 
-            apply_function_to_parents: whether to apply function to parents from previous generation (if it's needed)
+            apply_function_to_parents: whether to apply function to parents from previous generation (if it's needed), 
+                it can be needed at working with games agents, but for other tasks will just waste time
 
             start_generation: initial generation object of any `GenerationConvertible` type
 
             studEA: using stud EA strategy (crossover with best object always)
 
             mutation_indexes: indexes of dimensions where mutation can be performed (all dimensions by default)
 
@@ -493,27 +524,40 @@
             revolution_oppositor: oppositor for revolution time. No by default
             revolution_after_stagnation_step: create revolution after this generations of stagnation. No by default
             revolution_part: float, the part of generation to being oppose. By default is 0.3
 
             population_initializer: object for actions at population initialization step
                 to create better start population. See doc
 
-            stop_when_reached: stop searching after reaching this value (it can be potential minimum or something else)
+            stop_when_reached: stop searching after reaching this value 
+                (it can be potential minimum or something else)
 
             callbacks: sequence of callback functions with structure:
                 (generation_number, report_list, last_population, last_scores) -> do some action
 
-            middle_callbacks: sequence of functions made `MiddleCallback` class
+            middle_callbacks: sequence of functions made by `MiddleCallback` class
 
-            time_limit_secs: limit time of working (in seconds)
+            time_limit_secs: limit time of working (in seconds);
+                `None` means no time limit (limit will be only for count of generation and so on)
 
-            save_last_generation_as: path to .npz file for saving last_generation as numpy dictionary like
-                {'population': 2D-array, 'scores': 1D-array}, None if doesn't need to save in file
+            save_last_generation_as: path to .npz file 
+                for saving last_generation as numpy dictionary like
+                {'population': 2D-array, 'scores': 1D-array}; 
+                None disables this option
 
             seed: random seed (None if doesn't matter)
+
+        Returns:
+            `GAResult` object;
+            also fills the self.report and self.result with many report information
+
+        Notes:
+            - if `function_timeout` is enabled then `function` must be set
+            - it would be more logical to use params like `studEA` as an algorithm parameter, 
+                but `run()`-way can be more convenient for real using
         """
 
         if disable_progress_bar:
             warnings.warn(
                 f"disable_progress_bar is deprecated and will be removed in version 7, "
                 f"use probress_bar_stream=None to disable progress bar"
             )
@@ -640,15 +684,15 @@
                     cb(generation_number, report_list, last_population, last_scores)
 
         if not middle_callbacks:
             total_middle_callback = lambda: None
         else:
             def total_middle_callback():
                 """
-                applies callbacks and sets new data if there is a sence
+                applies callbacks and sets new data if there is a sense
                 """
                 data = get_data()
                 flag = False
                 for cb in middle_callbacks:
                     data, has_sense = cb(data)
                     if has_sense:
                         flag = True
@@ -660,14 +704,24 @@
         start_time = time.time()
         time_is_done = (
             (lambda: False)
             if time_limit_secs is None
             else (lambda: int(time.time() - start_time) >= time_limit_secs)
         )
 
+        # combine with deprecated parts
+        function = function or self.f
+        function_timeout = function_timeout or self.funtimeout
+
+        assert function or set_function, 'no function to minimize'
+        if function:
+            self._check_function(function)
+        if function_timeout:
+            self._check_function_timeout(function_timeout)
+
         self.set_function = set_function or GeneticAlgorithm2.default_set_function(self.f)
 
         #region Initial population, duplicates filter, revolutionary
 
         pop_coef, initializer_func = population_initializer
         
         # population creator by random or with oppositions
```

### Comparing `geneticalgorithm2-6.9.0/geneticalgorithm2/mutations.py` & `geneticalgorithm2-6.9.1/geneticalgorithm2/mutations.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,19 @@
 Function (x, left, right) -> value
 
 Which mutates x to value according to bounds (left, right)
 """
 
 
 class Mutations:
-    """Mutations functions static class"""
+    """
+    Mutations functions static class
+    
+    Mutation changes the sample randomly providing the evolution component to optimization
+    """
 
     @staticmethod
     def mutations_dict() -> Dict[str, MutationFloatFunc]:
         return {
             n: getattr(Mutations, n)()
             for n in (
                 'uniform_by_x',
```

### Comparing `geneticalgorithm2-6.9.0/geneticalgorithm2/population_initializer.py` & `geneticalgorithm2-6.9.1/geneticalgorithm2/population_initializer.py`

 * *Files identical despite different names*

### Comparing `geneticalgorithm2-6.9.0/geneticalgorithm2/selections.py` & `geneticalgorithm2-6.9.1/geneticalgorithm2/selections.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 """
 
 
 #region UTILS
 
 def inverse_scores(scores: array1D) -> array1D:
     """
-    inverses scores (min val goes to max)
+    inverses scores (min values become to max)
     """
     minobj = scores[0]
     normobj = scores - minobj if minobj < 0 else scores
 
     return (np.amax(normobj) + 1) - normobj
 
 
@@ -46,14 +46,16 @@
 
 
 #endregion
 
 class Selection:
     """
     Selections functions static class
+    
+    Selection function selects the population subset according to scores and its own rules
     """
 
     @staticmethod
     def selections_dict() -> Dict[str, SelectionFunc]:
         return {
             n: getattr(Selection, n)()
             for n in (
```

### Comparing `geneticalgorithm2-6.9.0/geneticalgorithm2/utils/cache.py` & `geneticalgorithm2-6.9.1/geneticalgorithm2/utils/cache.py`

 * *Files identical despite different names*

### Comparing `geneticalgorithm2-6.9.0/geneticalgorithm2/utils/files.py` & `geneticalgorithm2-6.9.1/geneticalgorithm2/utils/files.py`

 * *Files identical despite different names*

### Comparing `geneticalgorithm2-6.9.0/geneticalgorithm2/utils/funcs.py` & `geneticalgorithm2-6.9.1/geneticalgorithm2/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `geneticalgorithm2-6.9.0/geneticalgorithm2/utils/plotting.py` & `geneticalgorithm2-6.9.1/geneticalgorithm2/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `geneticalgorithm2-6.9.0/geneticalgorithm2.egg-info/PKG-INFO` & `geneticalgorithm2-6.9.1/geneticalgorithm2.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneticalgorithm2
-Version: 6.9.0
+Version: 6.9.1
 Summary: Supported highly optimized and flexible genetic algorithm package for python
 Home-page: https://github.com/PasaOpasen/geneticalgorithm2
 Author: Demetry Pascal
 Author-email: qtckpuhdsa@gmail.com
 Maintainer: Demetry Pascal
 License: MIT
 Keywords: solve,solver,equation,optimization,problem,genetic,algorithm,GA,easy,fast,genetic-algorithm,combinatorial,mixed,evolutionary
@@ -30,14 +30,15 @@
 **geneticalgorithm2** (from [DPEA](https://github.com/PasaOpasen/PasaOpasen.github.io/blob/master/EA_packages.md)) **is the supported advanced optimized fork of non-supported package** [geneticalgorithm](https://github.com/rmsolgi/geneticalgorithm) of *Ryan (Mohammad) Solgi*
 
 - [About](#about)
 - [Installation](#installation)
 - [Updates information](#updates-information)
   - [**Future**](#future)
   - [**TODO firstly**](#todo-firstly)
+  - [6.9.1 refactor](#691-refactor)
   - [6.9.0 reborn](#690-reborn)
   - [6.8.7 minor update](#687-minor-update)
   - [6.8.6 minor update](#686-minor-update)
   - [6.8.5 minor update](#685-minor-update)
   - [6.8.4 minor update](#684-minor-update)
   - [6.8.3 types update](#683-types-update)
   - [6.8.2 patch](#682-patch)
@@ -57,33 +58,39 @@
   - [6.5.1 patch](#651-patch)
   - [6.5.0 minor update (refactoring)](#650-minor-update-refactoring)
   - [6.4.1 patch (bug fix)](#641-patch-bug-fix)
   - [6.4.0 minor update (refactoring)](#640-minor-update-refactoring)
   - [6.3.0 minor update (refactoring)](#630-minor-update-refactoring)
 - [Working process](#working-process)
   - [Main algorithm structure](#main-algorithm-structure)
+  - [Optimization process components](#optimization-process-components)
+    - [Function to minimize](#function-to-minimize)
+    - [Optimization space](#optimization-space)
+    - [Algorithm parameters](#algorithm-parameters)
+    - [Samples constructors](#samples-constructors)
+    - [Callbacks](#callbacks)
   - [How to run](#how-to-run)
   - [Constructor parameters](#constructor-parameters)
   - [Genetic algorithm's parameters](#genetic-algorithms-parameters)
     - [AlgorithmParams object](#algorithmparams-object)
     - [Parameters of algorithm](#parameters-of-algorithm)
-      - [**Count parameters**](#count-parameters)
       - [**Crossover**](#crossover)
       - [**Mutation**](#mutation)
       - [**Selection**](#selection)
-  - [Methods and Properties of model:](#methods-and-properties-of-model)
+  - [Methods and Properties of model](#methods-and-properties-of-model)
 - [Examples for beginner](#examples-for-beginner)
   - [A minimal example](#a-minimal-example)
   - [The simple example with integer variables](#the-simple-example-with-integer-variables)
   - [The simple example with Boolean variables](#the-simple-example-with-boolean-variables)
   - [The simple example with mixed variables](#the-simple-example-with-mixed-variables)
   - [Optimization problems with constraints](#optimization-problems-with-constraints)
   - [Middle example: select fixed count of objects from set](#middle-example-select-fixed-count-of-objects-from-set)
 - [U should know these features](#u-should-know-these-features)
   - [Available crossovers](#available-crossovers)
+  - [Available selections](#available-selections)
   - [Function timeout](#function-timeout)
   - [Standard GA vs. Elitist GA](#standard-ga-vs-elitist-ga)
   - [Standard crossover vs. stud EA crossover](#standard-crossover-vs-stud-ea-crossover)
   - [Creating better start population](#creating-better-start-population)
     - [Select best N of kN](#select-best-n-of-kn)
     - [Do local optimization](#do-local-optimization)
     - [Optimization with oppositions](#optimization-with-oppositions)
@@ -125,14 +132,15 @@
   - [Using GA with image reconstruction by polygons](#using-ga-with-image-reconstruction-by-polygons)
 - [Popular questions](#popular-questions)
   - [How to disable autoplot?](#how-to-disable-autoplot)
   - [How to plot population scores?](#how-to-plot-population-scores)
   - [How to specify evaluated function for all population?](#how-to-specify-evaluated-function-for-all-population)
   - [What about parallelism?](#what-about-parallelism)
   - [How to initialize start population? How to continue optimization with new run?](#how-to-initialize-start-population-how-to-continue-optimization-with-new-run)
+
 # About
 
 [**geneticalgorithm2**](https://pasaopasen.github.io/geneticalgorithm2/) is very flexible and highly optimized Python library for implementing classic
 [genetic-algorithm](https://towardsdatascience.com/introduction-to-optimization-with-genetic-algorithm-2f5001d9964b) (GA).
 
 Features of this package:
 
@@ -147,46 +155,49 @@
 * support of mixed types of variables
 * **support of classic, elitist and studEA genetic algorithm combinations**
 * **support of revolutions and duplicates utilization**
 * **reach support of customization**
     
 # Installation
 
-Install this package with standard dependencies to use the entire functional.
+Install this package with standard light dependencies to use the base functional.
 ```
 pip install geneticalgorithm2
 ```
 
-Install this package with full dependencies to use all provided functional.
+Install this package with full dependencies to use all provided functional including plotting and built-in parallelism tools.
 
 ```
 pip install geneticalgorithm2[full]
 ```
 
 # Updates information
 
 ## **Future**
 
 - duplicates removing and revolutions will be moved to `MiddleCallbacks` and removed as alone `run()` parameters
-- `function_timeout` and `function` will be moved to `run()` method
 - new stop criteria callbacks (min std, max functions evaluations)
 - `vartype` will support strings like `iiiiibbf`
 
 ## **TODO firstly**
-- Remove old style mensions from README
+- Remove old style mentions from README
+
+## 6.9.1 refactor
 
+- Finally move `function_timeout` and `function` to `run()` method and deprecate its usage in init()
+- `function` is not mandatory to be non-empty 
+- reduce documentation duplicates
 
 ## 6.9.0 reborn
 
 - recreate the repository without excess heavy files materials 
 - host the [code documentation](https://pasaopasen.github.io/geneticalgorithm2/)
 - rename `geneticalgorithm2` class to `GeneticAlgorithm2`
 - substantial package architecture refactor
 - add more docstrings
-- reduce documentation duplicates 
 
 ## 6.8.7 minor update
 
 - some code refactor
 - fixes:
   - ensure the directory of generation file exists on save
 
@@ -220,15 +231,15 @@
 
 - printing progress bar to `'stderr'` or `'stdout'` or `None` (disable) by choice (`progress_bar_stream` argument of `run()`), deprecated `disable_progress_bar`
 - little speed up
 - new `geneticalgorithm2.vectorized_set_function` set function, which can be faster for big populations 
 
 ## 6.8.0 minor update
 
-- remove `crossover_probability` model parameter because of it has no sense to exist (and 1.0 value is better than others, take a look at [results](/tests/output/sense_of_crossover_prob__no_sense.png)). This parameter came from `geneticalgorithm` old package and did`t change before.
+- remove `crossover_probability` model parameter because of it has no sense to exist (and 1.0 value is better than others, take a look at [results](/examples/output/sense_of_crossover_prob__no_sense.png)). This parameter came from `geneticalgorithm` old package and did`t change before.
 
 ## 6.7.7 refactor
 
 - change some behavior about parents selection
 
 ## 6.7.6 bug fix
 
@@ -298,15 +309,15 @@
     * `None`
     * `str` path to saved generation
     * dictionary with structure `{'variables': variables/None, 'scores': scores/None}`
     * `Generation` object: `Generation(variables = variables, scores = scores)`
     * `np.ndarray` with shape `(samples, dim)` for only population or `(samples, dim+1)` for concatenated population and score (scores is the last matrix column)
     * `tuple(np.ndarray/None, np.ndarray/None)` for variables and scores
   
-  here `variables` is 2D numpy array with shape `(samples, dim)`, `scores` is 1D numpy array with scores (function values) for each sample; [here](tests/output/start_gen.py) and [here](#how-to-initialize-start-population-how-to-continue-optimization-with-new-run) u can see examples of using these valid forms 
+  here `variables` is 2D numpy array with shape `(samples, dim)`, `scores` is 1D numpy array with scores (function values) for each sample; [here](examples/output/start_gen.py) and [here](#how-to-initialize-start-population-how-to-continue-optimization-with-new-run) u can see examples of using these valid forms 
 
 
 ## 6.3.0 minor update (refactoring)
 
 - type hints for entire part of functions
 - new valid forms for function parameters (now u don't need to use numpy arrays everywhere)
 - `AlgorithmParams` class for base GA algorithm parameters (instead of dictionary)
@@ -343,17 +354,60 @@
     remove duplicates, make revolutions, sort population by scores
     use callbacks, use middle callbacks
 
 Post-process: plotting results, saving
 
 ```
 
+## Optimization process components
+
+### Function to minimize
+
+The goal of the optimization process is to find the *minimum* of the given `function (1D array) -> float` where the function argument is a vector of some values in different dimensions. 
+
+If u want to find the *maximum*, use this idea:
+```python
+opt_func = lambda arr: -func(arr)
+
+#
+# ... find global min of opt_func
+#
+
+opt_minimum=opt_func(best value)
+maximum = -opt_minimum
+```
+
+Also it is possible and highly recommended to create and use a *vectorized* version of this function called `set_function (2D array) -> (1D array)` which transforms several samples matrix to samples scores vector by one call. Using this way u can speed up calculations or set up more complex tasks optimization
+
+### Optimization space
+
+The function rates 1D arrays (vectors) where each component (dimension) means something u program it to mean. Each dimension has its `bound` (`[min; max]` cut) and `variable type` (real/discrete).
+
+**Advice**. Genetic algorithms work much faster and efficient for discrete tasks. If high precision is not required u can split any real dimension to many discrete values (for instance, `[1.1, 1.2, 1.25, 1.44]`) and try to optimize indexes of the given array which are converted to real values inside `function` itself.
+
+### Algorithm parameters
+
+There are a number of hyperparameters u can probe to optimize including population size and selection/crossover/mutation types.
+
+### Samples constructors
+
+There are several ways to create new testing samples from zero when u start with empty population or when u need new samples after [duplicates removing](#duplicates-removing) and [revolutions](#revolutions). 
+
+
+### Callbacks
+
+Now the package supports 2 different types of highly customized callbacks:
+* [simple callbacks](#callbacks)
+* [middle callbacks](#middle-callbacks)
+
 ## How to run
 
-Firstly, u should **import needed packages**. All available (but not always necessary) imports are:
+Firstly, u should **import needed packages**. 
+
+All available (but not always necessary) imports are:
 
 ```python
 import numpy as np
 
 # the only one required import
 from geneticalgorithm2 import GeneticAlgorithm2 as ga  # for creating and running optimization model
 
@@ -368,116 +422,89 @@
 from geneticalgorithm2 import plot_pop_scores  # for plotting population scores, if u want
 
 from geneticalgorithm2 import Callbacks  # simple callbacks (will be deprecated)
 
 from geneticalgorithm2 import Actions, ActionConditions, MiddleCallbacks  # middle callbacks
 ```
 
-Next step: **define minimized function** like
+Next step: **define the function to minimize**:
 
 ```python
 def function(X: np.ndarray) -> float: # X as 1d-numpy array
     return np.sum(X**2) + X.mean() + X.min() + X[0]*X[2] # some float result
 ```
 
-If u want to find *maximum*, use this idea:
-
-```python
-f_tmp = lambda arr: -target(arr)
-
-#
-# ... find global min
-#
-
-target_result = -global_min
-```
-
-Okay, also u should **create the bounds for each variable** (if exist) like here:
+Also u should **create the bounds for each variable** (if exist) such as:
 
 ```python
 var_bound = np.array([[0,10]]*3) # 2D numpy array with shape (dim, 2)
 
 # also u can use Sequence of Tuples (from version 6.3.0)
 var_bound = [
     (0, 10),
     (0, 10),
     (0, 10)
 ]
-
 ```
-U don't need to use variable boundaries only if variable type of each variable is boolean. This case will be converted to discret variables with bounds `(0, 1)`.
 
-After that **create a `geneticalgorithm2` (was imported early as ga) object**:
+**Important**. U don't need to use variable boundaries only if variable type of each variable is boolean. This case will be automatically converted to discrete variables with bounds `(0, 1)`.
+
+After that u **create a `GeneticAlgorithm2` (was imported early as ga) object**:
 
 ```python
-# style before 6.3.0 version (but still works)
-model = ga(
-    function, 
+model = ga( 
     dimension = 3, 
     variable_type='real', 
     variable_boundaries = var_bound,
-    function_timeout = 10,
     algorithm_parameters={
         'max_num_iteration': None,
         'population_size':100,
         'mutation_probability': 0.1,
         'mutation_discrete_probability': None,
         'elit_ratio': 0.01,
         'parents_portion': 0.3,
         'crossover_type':'uniform',
         'mutation_type': 'uniform_by_center',
         'mutation_discrete_type': 'uniform_discrete',
         'selection_type': 'roulette',
         'max_iteration_without_improv':None
     }
 )
+```
 
-# from version 6.3.0 it is equal to
+**Note**: it is not mandatory to write all possible `algorithm_parameters`, here it is done only to show u defaults. Also u can use `AlgorithmParams` (with typehints and docstrings) class instead of dicts:
 
-model = ga(
-    function, 
-    dimension = 3, 
-    variable_type='real', 
-    variable_boundaries = var_bound,
-    function_timeout = 10,
-    algorithm_parameters=AlgorithmParams(
-        max_num_iteration = None,
-        population_size = 100,
-        mutation_probability = 0.1,
-        mutation_discrete_probability = None,
-        elit_ratio = 0.01,
-        parents_portion = 0.3,
-        crossover_type = 'uniform',
-        mutation_type = 'uniform_by_center',
-        mutation_discrete_type = 'uniform_discrete',
-        selection_type = 'roulette',
-        max_iteration_without_improv = None
-    )
+```python
+algorithm_parameters=AlgorithmParams(
+    max_num_iteration=None,
+    population_size=100,
+    mutation_probability=0.1,
+    mutation_discrete_probability=None,
+    elit_ratio=0.01,
+    parents_portion=0.3,
+    crossover_type='uniform',
+    mutation_type='uniform_by_center',
+    mutation_discrete_type='uniform_discrete',
+    selection_type='roulette',
+    max_iteration_without_improv=None
 )
-
-# or (with defaults)           
-model = ga(
-    function, dimension = 3, 
-    variable_type='real', 
-    variable_boundaries = var_bound,
-    function_timeout = 10,
-    algorithm_parameters=AlgorithmParams()
-)           
-
 ```
 
 **Run the search method**:
 
 ```python
 # all of this parameters are default
 result = model.run(
     no_plot = False, 
     progress_bar_stream = 'stdout',
     disable_printing = False,
 
+    function=function,
+    function_timeout=None,
+
     set_function = None, 
     apply_function_to_parents = False, 
     start_generation = None,
     studEA = False,
     mutation_indexes = None,
 
     init_creator = None,
@@ -494,359 +521,89 @@
     callbacks = [],
     middle_callbacks = [],
     time_limit_secs = None, 
     save_last_generation_as = None,
     seed = None
 )
 
-# best solution
+# best candidate
 print(result.variable)
 
 # best score
 print(result.score)
 
 # last generation
 print(result.last_generation)
 
 ```
 
 ## Constructor parameters
 
-* **function** (`Callable[[np.ndarray], float]`) - the given objective function to be minimized  
-NOTE: This implementation minimizes the given objective function. (For maximization multiply function by a negative sign: the absolute value of the output would be the actual objective function)
-        
-* **dimension** (`int`) - the number of decision variables
-        
-* **variable_type** (`Union[str, Sequence[str]]`) - 'bool' if all variables are Boolean; 'int' if all variables are integer; and 'real' if all variables are real value or continuous. For mixed types use sequence of string of type for each variable
-        
-* **variable_boundaries** (`Optional[Union[np.ndarray, Sequence[Tuple[float, float]]]]`) - Default None; leave it None if variable_type is 'bool'; otherwise provide an sequence of tuples of length two as boundaries for each variable; the length of the array must be equal dimension. 
-For example, `np.array([[0,100],[0,200]])` or `[(0, 100), (0, 200)]` determines lower boundary 0 and upper boundary 100 for first and upper boundary 200 for second variable where dimension is 2.
-        
-* **function_timeout** (`float`) - if the given function does not provide 
-output before function_timeout (unit is seconds) the algorithm raise error.
-For example, when there is an infinite loop in the given function. `None` means disabling
-        
-* **algorithm_parameters** (`Union[AlgorithmParams, Dict[str, Any]]`). Dictionary or AlgorithmParams object with fields:  
-    * @ **max_num_iteration** (`int/None`) - stopping criteria of the genetic algorithm (GA)  
-    * @ **population_size** (`int > 0`)   
-    * @ **mutation_probability** (`float in [0,1]`)
-    * @ **mutation_discrete_probability** (`float in [0,1]` or `None`)
-    * @ **elit_ration** (`float in [0,1]`) - part of elit objects in population; if > 0, there always will be 1 elit object at least  
-    * @ **parents_portion** (`float in [0,1]`) - part of parents from previous population to save in next population (including `elit_ration`)  
-    * @ **crossover_type** (`Union[str, Callable[[np.ndarray, np.ndarray], Tuple[np.ndarray, np.ndarray]]]`) - Default is `uniform`.
-    * @ **mutation_type** (`Union[str, Callable[[float, float, float], float]]`) - Default is `uniform_by_center`
-    * @ **mutation_discrete_type** (`Union[str, Callable[[int, int, int], int]]`) - Default is `uniform_discrete`
-    * @ **selection_type** (`Union[str, Callable[[np.ndarray, int], np.ndarray]]`) - Default is `roulette`
-    * @ **max_iteration_without_improv** (`int/None`) - maximum number of successive iterations without improvement. If `None` it is ineffective
+Have a look at https://pasaopasen.github.io/geneticalgorithm2/geneticalgorithm2/geneticalgorithm2.html#GeneticAlgorithm2.__init__
 
 ## Genetic algorithm's parameters
 
 ### AlgorithmParams object
 
-The parameters of GA is defined as a dictionary or `AlgorithmParams` object:
-
-```python
-
-algorithm_param = AlgorithmParams(
-                max_num_iteration = None,
-                population_size = 100,
-                mutation_probability = 0.1,
-                mutation_discrete_probability = None,
-                elit_ratio = 0.01,
-                parents_portion = 0.3,
-                crossover_type = 'uniform',
-                mutation_type = 'uniform_by_center',
-                mutation_discrete_type = 'uniform_discrete',
-                selection_type = 'roulette',
-                max_iteration_without_improv = None
-            )
-
-
-# old style with dictionary
-# sometimes it's easier to use this style
-# especially if u need to set only few params
-algorithm_param = {
-                   'max_num_iteration': None,
-                   'population_size':100,
-                   'mutation_probability': 0.1,
-                   'mutation_discrete_probability': None,
-                   'elit_ratio': 0.01,
-                   'parents_portion': 0.3,
-                   'crossover_type':'uniform',
-                   'mutation_type': 'uniform_by_center',
-                   'mutation_discrete_type': 'uniform_discrete',
-                   'selection_type': 'roulette',
-                   'max_iteration_without_improv':None
-                   }
-
-```
+The parameters of GA is defined as a dictionary or `AlgorithmParams` object: https://pasaopasen.github.io/geneticalgorithm2/geneticalgorithm2/data_types/algorithm_params.html
 
-To get actual default params use code:
+To get the global default params use code:
 ```python
 params = ga.default_params
 ```
 
-To get actual parameters of existing model use code:
+To get actual parameters of an existing model use code:
 ```python
 params = model.param
 ```
 
-An example of setting a new set of parameters for genetic algorithm and running `geneticalgorithm2` for our first simple example again:
-
-```python
-import numpy as np
-from geneticalgorithm2 import GeneticAlgorithm2 as ga
-
-
-def f(X):
-    return np.sum(X)
-
-
-varbound = [(0, 10)] * 3
-
-algorithm_param = {'max_num_iteration': 3000,
-                   'population_size': 100,
-                   'mutation_probability': 0.1,
-                   'mutation_discrete_probability': None,
-                   'elit_ratio': 0.01,
-                   'parents_portion': 0.3,
-                   'crossover_type': 'uniform',
-                   'mutation_type': 'uniform_by_center',
-                   'mutation_discrete_type': 'uniform_discrete',
-                   'selection_type': 'roulette',
-                   'max_iteration_without_improv': None}
-
-model = ga(function=f,
-           dimension=3,
-           variable_type='real',
-           variable_boundaries=varbound,
-           algorithm_parameters=algorithm_param
-           )
-
-model.run()
-```
-**Important**. U may use the small dictionary with only important parameters; other parameters will be default. It means the dictionary
-```js
-algorithm_param = {'max_num_iteration': 150,
-                   'population_size':1000}
-```
-is equal to:
-```js
-algorithm_param = {'max_num_iteration': 150,
-                   'population_size':1000,
-                   'mutation_probability': 0.1,
-                   'mutation_discrete_probability': None,
-                   'elit_ratio': 0.01,
-                   'parents_portion': 0.3,
-                   'crossover_type':'uniform',
-                   'mutation_type': 'uniform_by_center',
-                   'mutation_discrete_type': 'uniform_discrete',
-                   'selection_type': 'roulette',
-                   'max_iteration_without_improv':None}
-```
-
-But it is better to use `AlgorithmParams` object instead of dictionaries.
-
 ### Parameters of algorithm
 
-#### **Count parameters**
-
-* **max_num_iteration**: The termination criterion of GA. 
-If this parameter's value is `None` the algorithm sets maximum number of iterations automatically as a function of the dimension, boundaries, and population size. The user may enter any number of iterations that they want. It is highly recommended that the user themselves determines the **max_num_iterations** and not to use `None`. Notice that **max_num_iteration** has been changed to 3000 (it was already `None`). 
-
-* **population_size**: determines the number of trial solutions in each iteration.
-
-* **elit_ration**: determines the number of elites in the population. The default value is 0.01 (i.e. 1 percent). For example when population size is 100 and **elit_ratio** is 0.01 then there is one elite unit in the population. If this parameter is set to be zero then `geneticalgorithm2` implements a standard genetic algorithm instead of elitist GA. [See example](#standard-ga-vs-elitist-ga) of difference
-
-* **parents_portion**: the portion of population filled by the members of the previous generation (aka parents); default is 0.3 (i.e. 30 percent of population)
-
-* **max_iteration_without_improv**: if the algorithms does not improve the objective function over the number of successive iterations determined by this parameter, then GA stops and report the best found solution before the `max_num_iterations` to be met. The default value is `None`. 
-
 #### **Crossover**
 
-* **crossover_type**: there are several options including `'one_point'`, `'two_point'`, `'uniform'`, `'segment'`, `'shuffle'` crossover functions; default is `'uniform'` crossover. U also can use crossover as functions from `Crossover` class:
-    * `Crossover.one_point()`
-    * `Crossover.two_point()`
-    * `Crossover.uniform()`
-    * `Crossover.uniform_window(window = 7)`
-    * `Crossover.shuffle()`
-    * `Crossover.segment()`
-    * `Crossover.mixed(alpha = 0.5)` -- only for real variables
-    * `Crossover.arithmetic()` -- only for real variables
-    
-    Have a look at [crossovers' logic](#available-crossovers)
-
-    If u want, write your own crossover function using simple syntax:
-    ```python
-    def my_crossover(parent_a: np.ndarray, parent_b: np.ndarray):
-        # some code
-        return child_1, child_2
-    ```
+https://pasaopasen.github.io/geneticalgorithm2/geneticalgorithm2/crossovers.html
 
 #### **Mutation**
 
-* **mutation_probability**: determines the chance of each gene in each individual solution to be replaced by a random value. Works for continuous variables or for all variables if **mutation_discrete_probability** is `None`
-
-* **mutation_discrete_probability**: works like **mutation_probability** but for discrete variables. If `None`, will be changed to **mutation_probability** value; so just don't specify this parameter if u don't need special mutation behavior for discrete variables
-
-* **mutation_type**: there are several options (only for real variables) including `'uniform_by_x'`, `'uniform_by_center'`, `'gauss_by_x'`, `'gauss_by_center'`; default is `'uniform_by_center'`. U also can use mutation as functions from `Mutations` class:
-    * `Mutations.gauss_by_center(sd = 0.2)`
-    * `Mutations.gauss_by_x(sd = 0.1)`
-    * `Mutations.uniform_by_center()`
-    * `Mutations.uniform_by_x()`
-
-    (If u want) write your mutation function using syntax:
-    ```python
-    def my_mutation(current_value: float, left_border: float, right_border: float) -> float:
-        # some code
-        return new_value 
-    ```
-
-* **mutation_discrete_type**: now there is only one option for discrete variables mutation: `uniform_discrete` (`Mutations.uniform_discrete()`) which works like `uniform_by_center` real mutation but with integer numbers. Anyway, this option was included at version 6.7.0 to support custom discrete mutations if u need it. For using custom mutation just set this parameter to function like
-  ```python
-    def my_mutation(current_value: int, left_border: int, right_border: int) -> int:
-        # some code
-        return new_value 
-  ```
+https://pasaopasen.github.io/geneticalgorithm2/geneticalgorithm2/mutations.html
 
 #### **Selection**
 
-* **selection_type**: there are several options (only for real) including `'fully_random'` (just for fun), `'roulette'`, `'stochastic'`, `'sigma_scaling'`, `'ranking'`, `'linear_ranking'`, `'tournament'`; default is `roulette`. U also can use selection as functions from `Selection` class:
-    * `Selection.fully_random()`
-    * `Selection.roulette()`
-    * `Selection.stochastic()`
-    * `Selection.sigma_scaling(epsilon = 0.05)`
-    * `Selection.ranking()`
-    * `Selection.linear_ranking(selection_pressure = 1.5)`
-    * `Selection.tournament(tau = 2)`
-
-    If u want, write your selection function using syntax:
-    ```python
-    def my_mutation(sorted_scores: np.ndarray, parents_count: int):
-        # some code
-        return array_of_parents_indexes 
-    ```
-![](tests/output/selections.png)
-
-## Methods and Properties of model:
-
-The main method if **run()**. It has parameters:
-
-* **no_plot** (`bool`) - do not plot results using matplotlib by default
-
-* **progress_bar_stream** (`Optional[str]`) - `'stdout'` to print progress bar to `stdout`, `'stderr'` for `stderr`, `None` to disable progress bar (also it can be faster by 10-20 seconds)
-
-* **disable_printing** (`bool`) - don't print any text (except progress bar)
-
-* **set_function** (`Optional[Callable[[np.ndarray], np.ndarray]]`): 2D-array -> 1D-array function, which applies to matrix of population (size (samples, dimension)) to estimate their values ("scores" in some sense)
-        
-* **apply_function_to_parents** (`bool`) - apply function to parents from previous generation (if it's needed), it can be needed at working with games agents, but for other tasks will just waste time
-
-* **start_generation** (`Union[str, Dict[str, np.ndarray], Generation, np.ndarray, Tuple[Optional[np.ndarray], Optional[np.ndarray]]]`) -- one of cases ([take a look](#how-to-initialize-start-population-how-to-continue-optimization-with-new-run)):
-  *  `Generation` object
-  *  dictionary with structure `{'variables':2D-array of samples, 'scores': function values on samples}` (if `'scores'` value is `None` the scores will be compute)
-  *  path to `.npz` file (`str`) with saved generation  
-  *  `np.ndarray` (with shape `(samples, dim)` or `(samples, dim+1)`) 
-  *  tuple of `np.ndarray`s / `None`. 
-
-* **studEA** (`bool`) - using stud EA strategy (crossover with best object always). Default is false. [Take a look](#standard-crossover-vs-stud-ea-crossover)
-* **mutation_indexes** (`Optional[Union[Sequence[int], Set[int]]]`) - indexes of dimensions where mutation can be performed (all dimensions by default). [Example](tests/mut_indexes.py)
-
-* **init_creator**: (`Optional[Callable[[], np.ndarray]]`), the function creates population samples. By default -- random uniform for real variables and random uniform for int. [Example](#optimization-with-oppositions)
-* **init_oppositors**: (`Optional[Sequence[Callable[[np.ndarray], np.ndarray]]]`) -- the list of oppositors creates oppositions for base population. No by default. [Example](#optimization-with-oppositions)
-* **duplicates_oppositor**: `Optional[Callable[[np.ndarray], np.ndarray]]`, oppositor for applying after duplicates removing. By default -- using just random initializer from creator. [Example](#duplicates-removing)
-* **remove_duplicates_generation_step**: `None/int`, step for removing duplicates (have a sense with discrete tasks). No by default. [Example](#duplicates-removing)
-* **revolution_oppositor** = `Optional[Callable[[np.ndarray], np.ndarray]]`, oppositor for revolution time. No by default. [Example](#revolutions)
-* **revolution_after_stagnation_step** = `None/int`, create revolution after this generations of stagnation. No by default. [Example](#revolutions)
-* **revolution_part** (`float`): the part of generation to being oppose. By default is 0.3. [Example](#revolutions)
-
-* **population_initializer** (`Tuple[int, Callable[[np.ndarray, np.ndarray], Tuple[np.ndarray, np.ndarray]]]`) -- object for actions at population initialization step to create better start population. [Take a look](#creating-better-start-population)
-
-* **stop_when_reached** (`Optional[float]`) -- stop searching after reaching this value (it can be potential minimum or something else)
-
-* **callbacks** (`Optional[Sequence[Callable[[int, List[float],  np.ndarray, np.ndarray], None]]]`) - list of callback functions with structure:
-  ```python 
-  def callback(generation_number, report_list, last_population_as_2D_array, last_population_scores_as_1D_array):
-      #
-      # do some action
-      #
-  ```
-    See [example of using callbacks](tests/callbacks.py). There are several callbacks in `Callbacks` class, such as:
-    * `Callbacks.SavePopulation(folder, save_gen_step = 50, file_prefix = 'population')`
-    * `Callbacks.PlotOptimizationProcess(folder, save_gen_step = 50, show = False, main_color = 'green', file_prefix = 'report')`
-
-* **middle_callbacks** (`Sequence`) - list of functions made `MiddleCallbacks` class (large opportunity, please, have a look at [this](#middle-callbacks)) 
-
-
-* **time_limit_secs** (`Optional[float]`) - limit time of working (in seconds). If `None`, there is no time limit (limit only for count of generation and so on). See [little example of using](tests/time_limit.py). Also there is simple conversion function for conversion some time in seconds:
-  ```python
-  from truefalsepython import time_to_seconds
-
-  total_seconds = time_to_seconds(
-      days = 2, # 2 days
-      hours = 13, # plus 13 hours
-      minutes = 7, # plus 7 minutes
-      seconds = 44 # plus 44 seconds
-  )
-  ```
-
-* **save_last_generation_as** (`Optional[str]`) - path to `.npz` file for saving last_generation as numpy dictionary like `{'population': 2D-array, 'scores': 1D-array}`, `None` if doesn't need to save in file; [take a look](#how-to-initialize-start-population-how-to-continue-optimization-with-new-run)
-
-* **seed** (`Optional[int]`) - random seed (None is doesn't matter)
-
-It would be more logical to use params like `studEA` as an algorithm param, but `run()`-way can be more comfortable for real using.
-
-    
-**output**:  
-  
-* `result`: is a wrap on last generation with fields:
-  * `last_generation` -- `Generation` object of last generation
-  * `variable` -- best unit of last generation
-  * `score` -- metric of the best unit
-  
-* `report`: is a record of the progress of the algorithm over iterations. Also u can specify to report not only best values. [Go to](#report-checker)
-
+https://pasaopasen.github.io/geneticalgorithm2/geneticalgorithm2/selections.html
 
+## Methods and Properties of model
 
+Have a look at https://pasaopasen.github.io/geneticalgorithm2/geneticalgorithm2/geneticalgorithm2.html#GeneticAlgorithm2.run
 
 # Examples for beginner
 
 ## A minimal example 
-Assume we want to find a set of `X = (x1,x2,x3)` that minimizes function `f(X) = x1 + x2 + x3` where `X` can be any real number in `[0, 10]`.
 
-This is a trivial problem and we already know that the answer is `X = (0,0,0)` where `f(X) = 0`.  
+Assume we want to find a set of `X = (x1, x2, x3)` that minimizes function `f(X) = x1 + x2 + x3` where `X` can be any real number in `[0, 10]`.
+
+This is a trivial problem and we already know that the answer is `X = (0, 0, 0)` where `f(X) = 0`.  
 
-We just use this simple example to see how to implement geneticalgorithm2. First we import geneticalgorithm2 and [numpy](https://numpy.org). Next, we define 
-function `f` which we want to minimize and the boundaries of the decision variables. Then simply geneticalgorithm2 is called to solve the defined optimization problem as follows:
+We just use this simple example to show how to implement it with `geneticalgorithm2`. First we import `geneticalgorithm2` and [numpy](https://numpy.org). Next, we define 
+function `f` which we want to minimize and the boundaries of the decision variables. Then simply `geneticalgorithm2` is called to solve the defined optimization problem as follows:
 
 ```python
 import numpy as np
 from geneticalgorithm2 import GeneticAlgorithm2 as ga
 
 
 def f(X):
     return np.sum(X)
 
 
 varbound = [[0, 10]] * 3
 
-model = ga(function=f, dimension=3, variable_type='real', variable_boundaries=varbound)
+model = ga(dimension=3, variable_type='real', variable_boundaries=varbound)
 
-model.run()
+model.run(function=f)
 ```
-
-    
-**geneticalgorithm2 has some arguments**:   
-1. Obviously the first argument is the function `f` we already defined.  
-2. Our problem has three variables so we set dimension equal `3`.   
-3. Variables are real (continuous) so we use string `'real'` to notify the type of 
-variables (geneticalgorithm2 accepts other types including boolean, integers and 
-mixed; see other examples).  
-1. Finally, we input `varbound` which includes the boundaries of the variables. 
-Note that the length of variable_boundaries must be equal to dimension.
   
 If you run the code, you should see a progress bar that shows the progress of the 
 genetic algorithm (GA) and then the solution, objective function value and the convergence curve as follows:
 
 ![](https://github.com/PasaOpasen/geneticalgorithm2/blob/master/genetic_algorithm_convergence.gif)
 
 Also we can access to the best answer of the defined optimization problem found by GA as a dictionary and a report of the progress of the genetic algorithm. 
@@ -868,20 +625,19 @@
 import numpy as np
 from geneticalgorithm2 import GeneticAlgorithm2 as ga
 
 
 def f(X):
     return np.sum(X)
 
-
 varbound = [[0, 10]] * 3
 
-model = ga(function=f, dimension=3, variable_type='int', variable_boundaries=varbound)
+model = ga(dimension=3, variable_type='int', variable_boundaries=varbound)
 
-model.run()
+model.run(function=f)
 ```
 So, as it is seen the only difference is that for `variable_type` we use string `'int'`. 
 
 ## The simple example with Boolean variables
 
 Considering the problem given in the simple example above.
 Now assume all variables are boolean instead of real or integer. So `X` can be either zero or one. Also instead of three let's have 30 variables.
@@ -891,48 +647,47 @@
 import numpy as np
 from geneticalgorithm2 import GeneticAlgorithm2 as ga
 
 
 def f(X):
     return np.sum(X)
 
+model = ga(dimension=30, variable_type='bool')
 
-model = ga(function=f, dimension=30, variable_type='bool')
-
-model.run()
+model.run(function=f)
 ```
-
 Note for variable_type we use string `'bool'` when all variables are boolean.  
 Note that when variable_type equal `'bool'` there is no need for `variable_boundaries` to be defined.
 
 ## The simple example with mixed variables
 
 Considering the problem given in the the simple example above where we want to minimize `f(X) = x1 + x2 + x3`. 
-Now assume `x1` is a real (continuous) variable in `[0.5,1.5]`, `x2` is an integer variable in `[1,100]`, and `x3` is a boolean variable that can be either zero or one.
-We already know that the answer is `X = (0.5,1,0)` where `f(X) = 1.5`
+Now assume `x1` is a real (continuous) variable in `[0.5; 1.5]`, `x2` is an integer variable in `[1;100]`, and `x3` is a boolean variable that can be either zero or one.
+We already know that the answer is `X = (0.5, 1, 0)` where `f(X) = 1.5`.
 We implement geneticalgorithm2 as the following:
 
 ```python
 import numpy as np
 from geneticalgorithm2 import GeneticAlgorithm2 as ga
 
 
 def f(X):
     return np.sum(X)
 
 
 varbound = [[0.5, 1.5], [1, 100], [0, 1]]
 vartype = ('real', 'int', 'int')
-model = ga(function=f, dimension=3, variable_type=vartype, variable_boundaries=varbound)
+model = ga(dimension=3, variable_type=vartype, variable_boundaries=varbound)
 
-model.run()
+model.run(function=f)
 ```
 
 ## Optimization problems with constraints
-In all above examples, the optimization problem was unconstrained. Now consider that we want to minimize `f(X) = x1+x2+x3` where `X` is a set of real variables in `[0, 10]`. Also we have an extra constraint so that sum of `x1` and `x2` is equal or greater than 2. The minimum of `f(X)` is 2.
+
+In all above examples, the optimization problem was unconstrained. Now consider that we want to minimize `f(X) = x1+x2+x3` where `X` is a set of real variables in `[0; 10]`. Also we have an extra constraint so that sum of `x1` and `x2` is equal or greater than 2. The minimum of `f(X)` is 2.
 In such a case, a trick is to define penalty function. Hence we use the code below:
 
 ```python
 import numpy as np
 from geneticalgorithm2 import GeneticAlgorithm2 as ga
 
 
@@ -941,34 +696,34 @@
     if X[0] + X[1] < 2:
         pen = 500 + 1000 * (2 - X[0] - X[1])
     return np.sum(X) + pen
 
 
 varbound = [[0, 10]] * 3
 
-model = ga(function=f, dimension=3, variable_type='real', variable_boundaries=varbound)
+model = ga(dimension=3, variable_type='real', variable_boundaries=varbound)
 
-model.run()
+model.run(function=f)
 
 ```
 As seen above we add a penalty to the objective function whenever the constraint is not met.  
 
 Some hints about how to define a penalty function:  
 
 1. Usually you may use a constant greater than the maximum possible value of the objective function if the maximum is known or if we have a guess of that. Here the highest possible value of our function is 300 (i.e. if all variables were 10, `f(X)=300`). So I chose a constant of 500. So, if a trial solution is not in the feasible region even though its objective function may be small, the penalized objective function (fitness function) is worse than any feasible solution.
 2. Use a coefficient big enough and multiply that by the amount of violation. This helps the algorithm learn how to approach feasible domain.
 3. How to define penalty function usually influences the convergence rate of an evolutionary algorithm. In my [book on metaheuristics and evolutionary algorithms](https://www.wiley.com/en-us/Meta+heuristic+and+Evolutionary+Algorithms+for+Engineering+Optimization-p-9781119386995) you can learn more about that. 
 4. Finally after you solved the problem test the solution to see if boundaries are met. If the solution does not meet constraints, it shows that a bigger penalty is required. However, in problems where optimum is exactly on the boundary of the feasible region (or very close to the constraints) which is common in some kinds of problems, a very strict and big penalty may prevent the genetic algorithm to approach the optimal region. In such a case designing an appropriate penalty function might be more challenging. Actually what we have to do is to design a penalty function that let the algorithm searches unfeasible domain while finally converge to a feasible solution. Hence you may need more sophisticated penalty functions. But in most cases the above formulation work fairly well.
 
 ## Middle example: select fixed count of objects from set
 
 For some task u need to think a lot and create good specific crossover or mutation functions. For example, take a look at this problem:
-
+```
     From set like X = {x1, x2, x3, ..., xn} u should select only k objects which get the best function value
-
+```
 U can do it using this code:
 
 ```python
 import numpy as np
 from geneticalgorithm2 import GeneticAlgorithm2 as ga
 
 subset_size = 20  # how many objects we can choose
@@ -1010,35 +765,39 @@
         children[:, np.array(list(intersect))] = 1
     children[0, child_inds[:int(child_inds.size / 2)]] = 1
     children[1, child_inds[int(child_inds.size / 2):]] = 1
 
     return children[0, :], children[1, :]
 
 
-model = ga(function=f,
-           dimension=objects_count,
-           variable_type='bool',
-           algorithm_parameters={
-               'max_num_iteration': 500,
-               'mutation_probability': 0,  # no mutation, just crossover
-               'elit_ratio': 0.05,
-               'parents_portion': 0.3,
-               'crossover_type': my_crossover,
-               'max_iteration_without_improv': 20
-           }
-           )
+model = ga(
+    dimension=objects_count,
+    variable_type='bool',
+    algorithm_parameters={
+        'max_num_iteration': 500,
+        'mutation_probability': 0,  # no mutation, just crossover
+        'elit_ratio': 0.05,
+        'parents_portion': 0.3,
+        'crossover_type': my_crossover,
+        'max_iteration_without_improv': 20
+    }
+)
 
-model.run(no_plot=False, start_generation=(start_generation, None))
+model.run(
+    function=f,
+    no_plot=False, 
+    start_generation=(start_generation, None)
+)
 ```
 
 # U should know these features
 
 ## Available crossovers
 
-For two example parents (*one with ones* and *one with zeros*) next crossovers will give same children ([examples](tests/crossovers_examples.py)): 
+For two example parents (*one with ones* and *one with zeros*) next crossovers will give same children ([examples](examples/crossovers_examples.py)): 
 
 * **one_point**:
 
 |0 | 0 | 0 | 0 | 0 | 0 | 0 | 0 | 1 | 1 | 1 | 1 | 1 | 1 | 1|
 |:---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---:|
 |1 | 1 | 1 | 1 | 1 | 1 | 1 | 1 | 0 | 0 | 0 | 0 | 0 | 0 | 0|
 
@@ -1080,61 +839,47 @@
 
 * **mixed**:
 
 |0.63 | 0.84 | 1.1 | 0.73 | 0.67 | -0.19 | 0.3 | 0.72 | -0.18 | 0.61 | 0.84 | 1.14 | 1.36 | -0.37 | -0.19|
 |:---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---:|
 |0.51 | 0.58 | 0.43 | 0.42 | 0.55 | 0.49 | 0.57 | 0.48 | 0.46 | 0.56 | 0.56 | 0.54 | 0.44 | 0.51 | 0.4|
 
+## Available selections
+
+![](examples/output/selections.png)
+
 
 ## Function timeout
 
-**geneticalgorithm2** is designed such that if the given function does not provide
-any output before timeout (the default value is 10 seconds), the algorithm
-would be terminated and raise the appropriate error. 
-
-In such a case make sure the given function
-works correctly (i.e. there is no infinite loop in the given function). Also if the given function takes more than 10 seconds to complete the work
-make sure to increase function_timeout in arguments.
+**geneticalgorithm2** inherited several features from `geneticalgorithm` package sush as that if the given function does not provide any output before timeout, the algorithm would be terminated and raise the appropriate error. 
+
+In such a case make sure the given function works correctly (i.e. there is no infinite loop in the given function). Also if the given function takes more than 10 seconds to complete the work
+make sure to increase `function_timeout` in arguments.
 
 ## Standard GA vs. Elitist GA
 
 The convergence curve of an elitist genetic algorithm is always non-increasing. So, the best ever found solution is equal to the best solution of the last iteration. However, the convergence curve of a standard genetic algorithm is different. If `elit_ratio` is zero geneticalgorithm2 implements a standard GA. The output of geneticalgorithm2 for standard GA is the best ever found solution not the solution of the last iteration. The difference between the convergence curve of standard GA and elitist GA is shown below:
 
-![](tests/output/standard_vs_elitist.png)
+![](examples/output/standard_vs_elitist.png)
 
 ## Standard crossover vs. stud EA crossover
 
 [Stud EA](https://link.springer.com/chapter/10.1007%2FBFb0056910) is the idea of using crossover always with best object. So one of two parents is always the best object of population. It can help us in a lot of tasks!
 
-![](tests/output/studEA.png)
+![](examples/output/studEA.png)
 
 ## Creating better start population
 
-There is `Population_initializer(select_best_of = 4, local_optimization_step = 'never', local_optimizer = None)` object for creating better start population. It has next arguments:
-
-* `select_best_of` (`int`) -- select `1/select_best_of` best part of start population. For example, for `select_best_of = 4` and `population_size = N` will be selected N best objects from 5N generated objects (if `start_generation = None`). If `start_generation` is not None, it will be selected best `size(start_generation)/N`  objects
-
-* `local_optimization_step` (`str`) -- when should we do local optimization? Available values:
-    
-    * `'never'` -- don't do local optimization
-    * `'before_select'` -- before selection best N objects (example: do local optimization for 5N objects and select N best results)
-    * `'after_select'` -- do local optimization on best selected N objects
-
-* `local_optimizer` (function) -- local optimization function like:
-    ```python
-    def loc_opt(object_as_array, current_score):
-        # some code
-        return better_object_as_array, better_score
-    ```
+There is `get_population_initializer(select_best_of = 4, local_optimization_step = 'never', local_optimizer = None)` function for creating start population creators. Take a look at [its docs](https://pasaopasen.github.io/geneticalgorithm2/geneticalgorithm2/population_initializer.html)
 
 ### Select best N of kN
 
 This little option can help u especially with multimodal tasks. 
 
-![](tests/output/init_best_of.png)
+![](examples/output/init_best_of.png)
 
 ### Do local optimization
 
 We can apply some local optimization on start generation before starting GA search. It can be some gradient descent or hill climbing and so on. Also we can apply it before selection best objects (on entire population) or after (on best part of population) and so forth.
 
 In next example I'm using my [DiscreteHillClimbing](https://github.com/PasaOpasen/DiscreteHillClimbing) algorithm for local optimization my discrete task:
 
@@ -1155,71 +900,77 @@
 
 iterations = 100
 
 varbound = [[-100, 100]] * 15
 
 available_values = [np.arange(-100, 101)] * 15
 
-my_local_optimizer = lambda arr, score: Hill_Climbing_descent(function=f, available_predictors_values=available_values,
-                                                              max_function_evals=50, start_solution=arr)
+my_local_optimizer = lambda arr, score: Hill_Climbing_descent(
+    function=f, available_predictors_values=available_values,
+    max_function_evals=50, start_solution=arr
+)
 
-model = ga(function=f, dimension=varbound.shape[0],
-           variable_type='int',
-           variable_boundaries=varbound,
-           algorithm_parameters={
-               'max_num_iteration': iterations,
-               'population_size': 400
-           })
+model = ga(
+    dimension=varbound.shape[0],
+    variable_type='int',
+    variable_boundaries=varbound,
+    algorithm_parameters={
+        'max_num_iteration': iterations,
+        'population_size': 400
+    }
+)
 
 for time in ('before_select', 'after_select', 'never'):
-    model.run(no_plot=True,
-              population_initializer=get_population_initializer(
-                  select_best_of=3,
-                  local_optimization_step=time,
-                  local_optimizer=my_local_optimizer
-              )
-              )
+    model.run(
+        function=f
+        no_plot=True,
+        population_initializer=get_population_initializer(
+            select_best_of=3,
+            local_optimization_step=time,
+            local_optimizer=my_local_optimizer
+        )
+    )
 
     plt.plot(model.report, label=f"local optimization time = '{time}'")
 
 plt.xlabel('Generation')
 plt.ylabel('Minimized function (40 simulations average)')
 plt.title('Selection best N object before running GA')
 plt.legend()
 ```
 
-![](tests/output/init_local_opt.png)
+![](examples/output/init_local_opt.png)
 
 ### Optimization with oppositions
 
-Also u can create start population with [oppositions](https://github.com/PasaOpasen/opp-op-pop-init). See [example of code](tests/best_of_N_with_opp.py)
+Also u can create start population with [oppositions](https://github.com/PasaOpasen/opp-op-pop-init). See [example of code](examples/best_of_N_with_opp.py)
 
-![](tests/output/init_best_of_opp.png)
+![](examples/output/init_best_of_opp.png)
 
 ## Revolutions
 
-U can create [revolutions in your population](https://github.com/PasaOpasen/opp-op-pop-init) after some stagnation steps. It really can help u for some tasks. See [example](tests/revolution.py)
+U can create [revolutions in your population](https://github.com/PasaOpasen/opp-op-pop-init) after some stagnation steps. It really can help u for some tasks. See [example](examples/revolution.py)
 
-![](tests/output/revolution.png)
+![](examples/output/revolution.png)
 
 
 ## Duplicates removing
 
-If u remove duplicates each `k` generations, u can speed up the optimization process ([example](tests/remove_dups.py))
+If u remove duplicates each `k` generations, u can speed up the optimization process ([example](examples/remove_dups.py))
 
-![](tests/output/remove_dups.png)
+![](examples/output/remove_dups.png)
 
 ## Cache
 
 It can be useful for run-speed to use cache with *some discrete tasks*. For this u can import `np_lru_cache` decorator and use it like here:
 
 ```python
 import np_lru_cache
 
-@np_lru_cache(maxsize = some_size)
+@np_lru_cache(maxsize=some_size)
 def minimized_func(arr):
     # code
     return result
 
 #
 # run
 #    algorithm
@@ -1245,34 +996,39 @@
 def f(X):
     return 50 * np.sum(X) - np.sum(np.sqrt(X) * np.sin(X))
 
 
 dim = 25
 varbound = [[0, 10]] * dim
 
-model = ga(function=f, dimension=dim,
-           variable_type='real', variable_boundaries=varbound,
-           algorithm_parameters={
-               'max_num_iteration': 600
-           }
-           )
+model = ga(
+    dimension=dim,
+    variable_type='real', 
+    variable_boundaries=varbound,
+    algorithm_parameters={
+        'max_num_iteration': 600
+    }
+)
 
 # here model exists and has checked_reports field
 # now u can append any functions to report
 
 model.checked_reports.extend(
     [
         ('report_average', np.mean),
         ('report_25', lambda arr: np.quantile(arr, 0.25)),
         ('report_50', np.median)
     ]
 )
 
 # run optimization process
-model.run(no_plot=False)
+model.run(
+    function=f,
+    no_plot=False
+)
 
 # now u have not only model.report but model.report_25 and so on
 
 # plot reports
 names = [name for name, _ in model.checked_reports[::-1]]
 plot_several_lines(
     lines=[getattr(model, name) for name in names],
@@ -1280,15 +1036,15 @@
     labels=['median value', '25% quantile', 'mean of population', 'best pop score'],
     linewidths=(1, 1.5, 1, 2),
     title="Several custom reports with base reports",
     save_as='./output/report.png'
 )
 ```
 
-![](tests/output/report.png)
+![](examples/output/report.png)
 
 As u see, u should append tuple `(name of report, func to evaluate report)` to `model.checked_report`. It's highly recommended to start this name with `report_` (e. g. `report_my_median`). And the function u use will get 1D-numpy *sorted* array of population scores.
 
 
 ## Middle callbacks
 
 There is an amazing way to control optimization process using `MiddleCallbacks` class. Just learn next logic:
@@ -1339,19 +1095,19 @@
 
 To combine `action` and `condition` to callback, just use `MiddleCallbacks.UniversalCallback(action, condition)` methods.
 
 
 There are also next high-level useful callbacks:
 
 * `MiddleCallbacks.ReduceMutationGen(reduce_coef = 0.9, min_mutation = 0.005, reduce_each_generation = 50, reload_each_generation = 500)`
-* `MiddleCallbacks.GeneDiversityStats(step_generations_for_plotting:int = 10)` -- plots some duplicates statistics each gen ([example](/tests/plot_diversities.py))
+* `MiddleCallbacks.GeneDiversityStats(step_generations_for_plotting:int = 10)` -- plots some duplicates statistics each gen ([example](/examples/plot_diversities.py))
 ![](diversity.gif)
 
 
-See [code example](tests/small_middle_callbacks.py)
+See [code example](examples/small_middle_callbacks.py)
 
 ## How to compare efficiency of several versions of GA optimization
 
 To compare efficiency of several versions of GA optimization (such as several values of several hyperparameters or including/excepting some actions like oppositions) u should make some count of simulations and compare results using some statistical test. I have realized this logic [here](https://github.com/PasaOpasen/ab-testing-results-difference) 
 
 ## Hints on how to adjust genetic algorithm's parameters (from `geneticalgorithm` package)
 
@@ -1557,91 +1313,91 @@
 
 # Examples pretty collection
 
 ## Optimization test functions
 
 Here there is the implementation of `geneticalgorithm2` for some benchmark problems. Test functions are got from my [`OptimizationTestFunctions`](https://github.com/PasaOpasen/OptimizationTestFunctions) package. 
 
-The code for optimizations process is same for each function and is contained [in file](tests/optimization_test_functions.py).
+The code for optimizations process is same for each function and is contained [in file](examples/optimization_test_functions.py).
 
 ### [Sphere](https://github.com/PasaOpasen/OptimizationTestFunctions#sphere)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Sphere.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Sphere.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Sphere.png)
 
 ### [Ackley](https://github.com/PasaOpasen/OptimizationTestFunctions#ackley)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Ackley.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Ackley.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Ackley.png)
 
 ### [AckleyTest](https://github.com/PasaOpasen/OptimizationTestFunctions#ackleytest)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20AckleyTest.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20AckleyTest.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20AckleyTest.png)
 
 ### [Rosenbrock](https://github.com/PasaOpasen/OptimizationTestFunctions#rosenbrock)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Rosenbrock.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Rosenbrock.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Rosenbrock.png)
 
 ### [Fletcher](https://github.com/PasaOpasen/OptimizationTestFunctions#fletcher)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Fletcher.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Fletcher.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Fletcher.png)
 
 ### [Griewank](https://github.com/PasaOpasen/OptimizationTestFunctions#griewank)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Griewank.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Griewank.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Griewank.png)
 
 ### [Penalty2](https://github.com/PasaOpasen/OptimizationTestFunctions#penalty2)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Penalty2.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Penalty2.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Penalty2.png)
 
 ### [Quartic](https://github.com/PasaOpasen/OptimizationTestFunctions#quartic)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Quartic.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Quartic.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Quartic.png)
 
 ### [Rastrigin](https://github.com/PasaOpasen/OptimizationTestFunctions#rastrigin)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Rastrigin.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Rastrigin.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Rastrigin.png)
 
 ### [SchwefelDouble](https://github.com/PasaOpasen/OptimizationTestFunctions#schwefeldouble)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20SchwefelDouble.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20SchwefelDouble.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20SchwefelDouble.png)
 
 ### [SchwefelMax](https://github.com/PasaOpasen/OptimizationTestFunctions#schwefelmax)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20SchwefelMax.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20SchwefelMax.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20SchwefelMax.png)
 
 ### [SchwefelAbs](https://github.com/PasaOpasen/OptimizationTestFunctions#schwefelabs)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20SchwefelAbs.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20SchwefelAbs.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20SchwefelAbs.png)
 
 ### [SchwefelSin](https://github.com/PasaOpasen/OptimizationTestFunctions#schwefelsin)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20SchwefelSin.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20SchwefelSin.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20SchwefelSin.png)
 
 ### [Stairs](https://github.com/PasaOpasen/OptimizationTestFunctions#stairs)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Stairs.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Stairs.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Stairs.png)
 
 ### [Abs](https://github.com/PasaOpasen/OptimizationTestFunctions#abs)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Abs.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Abs.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Abs.png)
 
 ### [Michalewicz](https://github.com/PasaOpasen/OptimizationTestFunctions#michalewicz)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Michalewicz.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Michalewicz.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Michalewicz.png)
 
 ### [Scheffer](https://github.com/PasaOpasen/OptimizationTestFunctions#scheffer)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Scheffer.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Scheffer.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Scheffer.png)
 
 ### [Eggholder](https://github.com/PasaOpasen/OptimizationTestFunctions#eggholder)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Eggholder.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Eggholder.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Eggholder.png)
 
 ### [Weierstrass](https://github.com/PasaOpasen/OptimizationTestFunctions#weierstrass)
 ![](https://github.com/PasaOpasen/OptimizationTestFunctions/blob/main/tests/heatmap%20for%20Weierstrass.png)
-![](tests/output/opt_test_funcs/Optimization%20process%20for%20Weierstrass.png)
+![](examples/output/opt_test_funcs/Optimization%20process%20for%20Weierstrass.png)
 
 
 
 ## Using GA in reinforcement learning
 
 See [example of using GA optimization with keras neural networks](https://www.kaggle.com/demetrypascal/opengym-tasks-using-keras-and-geneticalgorithm2) for solving OpenGym tasks.
 
@@ -1723,17 +1479,17 @@
           })
 # plot and save optimization process plot
 model.plot_results(save_as='plot_scores_process.png')
 
 # plot scores of last population
 model.plot_generation_scores(title='Population scores after ending of searching', save_as='plot_scores_end.png')
 ```
-![](tests/output/plot_scores_start.png)
-![](tests/output/plot_scores_process.png)
-![](tests/output/plot_scores_end.png)
+![](examples/output/plot_scores_start.png)
+![](examples/output/plot_scores_process.png)
+![](examples/output/plot_scores_end.png)
 
 
 
 ## How to specify evaluated function for all population?
 
 U can do it using `set_function` parameter into `run()` method.
```

### Comparing `geneticalgorithm2-6.9.0/geneticalgorithm2.egg-info/SOURCES.txt` & `geneticalgorithm2-6.9.1/geneticalgorithm2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geneticalgorithm2-6.9.0/setup.py` & `geneticalgorithm2-6.9.1/setup.py`

 * *Files identical despite different names*

