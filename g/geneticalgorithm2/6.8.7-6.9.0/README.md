# Comparing `tmp/geneticalgorithm2-6.8.7.tar.gz` & `tmp/geneticalgorithm2-6.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneticalgorithm2-6.8.7.tar", last modified: Wed Mar 13 18:56:19 2024, max compression
+gzip compressed data, was "geneticalgorithm2-6.9.0.tar", last modified: Sun Apr 14 06:07:08 2024, max compression
```

## Comparing `geneticalgorithm2-6.8.7.tar` & `geneticalgorithm2-6.9.0.tar`

### file list

```diff
@@ -1,26 +1,38 @@
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-03-13 18:56:19.555411 geneticalgorithm2-6.8.7/
--rw-rw-r--   0 pasa      (1000) pasa      (1000)     1095 2022-03-30 10:00:05.000000 geneticalgorithm2-6.8.7/LICENSE
--rw-r--r--   0 pasa      (1000) pasa      (1000)    81583 2024-03-13 18:56:19.554411 geneticalgorithm2-6.8.7/PKG-INFO
--rw-rw-r--   0 pasa      (1000) pasa      (1000)     2206 2022-03-30 10:00:05.000000 geneticalgorithm2-6.8.7/README.rst
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-03-13 18:56:19.553411 geneticalgorithm2-6.8.7/geneticalgorithm2/
--rw-r--r--   0 pasa      (1000) pasa      (1000)     1529 2022-04-12 19:42:34.000000 geneticalgorithm2-6.8.7/geneticalgorithm2/__init__.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)      323 2024-03-13 18:55:00.000000 geneticalgorithm2-6.8.7/geneticalgorithm2/aliases.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)     1425 2023-11-29 12:26:48.000000 geneticalgorithm2-6.8.7/geneticalgorithm2/cache.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)    14511 2024-03-13 18:55:00.000000 geneticalgorithm2-6.8.7/geneticalgorithm2/callbacks.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)    11174 2024-03-13 18:55:00.000000 geneticalgorithm2-6.8.7/geneticalgorithm2/classes.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)     4550 2023-11-29 12:26:48.000000 geneticalgorithm2-6.8.7/geneticalgorithm2/crossovers.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)      561 2024-03-13 18:55:00.000000 geneticalgorithm2-6.8.7/geneticalgorithm2/files.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)    46755 2024-03-13 18:55:00.000000 geneticalgorithm2-6.8.7/geneticalgorithm2/geneticalgorithm2.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)     3339 2023-11-29 12:26:48.000000 geneticalgorithm2-6.8.7/geneticalgorithm2/initializer.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)     2428 2023-11-29 12:26:48.000000 geneticalgorithm2-6.8.7/geneticalgorithm2/mutations.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)     2884 2024-03-13 18:55:00.000000 geneticalgorithm2-6.8.7/geneticalgorithm2/plotting_tools.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)     5252 2023-11-29 12:26:48.000000 geneticalgorithm2-6.8.7/geneticalgorithm2/selections.py
--rw-r--r--   0 pasa      (1000) pasa      (1000)     1227 2024-03-13 18:55:00.000000 geneticalgorithm2-6.8.7/geneticalgorithm2/utils.py
-drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-03-13 18:56:19.554411 geneticalgorithm2-6.8.7/geneticalgorithm2.egg-info/
--rw-rw-r--   0 pasa      (1000) pasa      (1000)    81583 2024-03-13 18:56:19.000000 geneticalgorithm2-6.8.7/geneticalgorithm2.egg-info/PKG-INFO
--rw-rw-r--   0 pasa      (1000) pasa      (1000)      634 2024-03-13 18:56:19.000000 geneticalgorithm2-6.8.7/geneticalgorithm2.egg-info/SOURCES.txt
--rw-rw-r--   0 pasa      (1000) pasa      (1000)        1 2024-03-13 18:56:19.000000 geneticalgorithm2-6.8.7/geneticalgorithm2.egg-info/dependency_links.txt
--rw-rw-r--   0 pasa      (1000) pasa      (1000)       83 2024-03-13 18:56:19.000000 geneticalgorithm2-6.8.7/geneticalgorithm2.egg-info/requires.txt
--rw-rw-r--   0 pasa      (1000) pasa      (1000)       18 2024-03-13 18:56:19.000000 geneticalgorithm2-6.8.7/geneticalgorithm2.egg-info/top_level.txt
--rw-r--r--   0 pasa      (1000) pasa      (1000)       38 2024-03-13 18:56:19.555411 geneticalgorithm2-6.8.7/setup.cfg
--rw-r--r--   0 pasa      (1000) pasa      (1000)     1453 2023-11-29 13:19:45.000000 geneticalgorithm2-6.8.7/setup.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-04-14 06:07:08.912212 geneticalgorithm2-6.9.0/
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     1095 2024-04-13 08:31:16.000000 geneticalgorithm2-6.9.0/LICENSE
+-rw-r--r--   0 pasa      (1000) pasa      (1000)    81879 2024-04-14 06:07:08.911212 geneticalgorithm2-6.9.0/PKG-INFO
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     2206 2024-04-13 08:31:16.000000 geneticalgorithm2-6.9.0/README.rst
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-04-14 06:07:08.907212 geneticalgorithm2-6.9.0/geneticalgorithm2/
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     1077 2024-04-13 16:49:58.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/__init__.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-04-14 06:07:08.909212 geneticalgorithm2-6.9.0/geneticalgorithm2/callbacks/
+-rw-r--r--   0 pasa      (1000) pasa      (1000)      171 2024-04-13 16:06:11.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/callbacks/__init__.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     2087 2024-04-13 17:16:17.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/callbacks/data.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)    13210 2024-04-13 16:05:21.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/callbacks/middle.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     2705 2024-04-13 14:22:37.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/callbacks/simple.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     4640 2024-04-13 12:55:10.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/crossovers.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-04-14 06:07:08.910212 geneticalgorithm2-6.9.0/geneticalgorithm2/data_types/
+-rw-r--r--   0 pasa      (1000) pasa      (1000)        0 2024-04-13 13:14:05.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/data_types/__init__.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     4129 2024-04-13 16:34:58.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/data_types/algorithm_params.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)      638 2024-04-13 16:35:09.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/data_types/aliases.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)      227 2024-04-13 13:17:20.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/data_types/base.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     5570 2024-04-13 13:39:12.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/data_types/generation.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)      656 2024-04-13 13:25:27.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/data_types/result.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)    44998 2024-04-13 16:58:46.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/geneticalgorithm2.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     2567 2024-04-13 12:52:40.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/mutations.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     3765 2024-04-13 16:45:38.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/population_initializer.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     5193 2024-04-13 12:47:59.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/selections.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-04-14 06:07:08.911212 geneticalgorithm2-6.9.0/geneticalgorithm2/utils/
+-rw-r--r--   0 pasa      (1000) pasa      (1000)        0 2024-04-13 09:55:36.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/utils/__init__.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)      323 2024-04-13 08:31:16.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/utils/aliases.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     1448 2024-04-13 09:56:05.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/utils/cache.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)      584 2024-04-13 09:56:05.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/utils/files.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     1224 2024-04-13 09:56:05.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/utils/funcs.py
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     2897 2024-04-13 09:56:06.000000 geneticalgorithm2-6.9.0/geneticalgorithm2/utils/plotting.py
+drwxr-xr-x   0 pasa      (1000) pasa      (1000)        0 2024-04-14 06:07:08.908212 geneticalgorithm2-6.9.0/geneticalgorithm2.egg-info/
+-rw-r--r--   0 pasa      (1000) pasa      (1000)    81879 2024-04-14 06:07:08.000000 geneticalgorithm2-6.9.0/geneticalgorithm2.egg-info/PKG-INFO
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     1046 2024-04-14 06:07:08.000000 geneticalgorithm2-6.9.0/geneticalgorithm2.egg-info/SOURCES.txt
+-rw-r--r--   0 pasa      (1000) pasa      (1000)        1 2024-04-14 06:07:08.000000 geneticalgorithm2-6.9.0/geneticalgorithm2.egg-info/dependency_links.txt
+-rw-r--r--   0 pasa      (1000) pasa      (1000)       83 2024-04-14 06:07:08.000000 geneticalgorithm2-6.9.0/geneticalgorithm2.egg-info/requires.txt
+-rw-r--r--   0 pasa      (1000) pasa      (1000)       18 2024-04-14 06:07:08.000000 geneticalgorithm2-6.9.0/geneticalgorithm2.egg-info/top_level.txt
+-rw-r--r--   0 pasa      (1000) pasa      (1000)       38 2024-04-14 06:07:08.912212 geneticalgorithm2-6.9.0/setup.cfg
+-rw-r--r--   0 pasa      (1000) pasa      (1000)     1453 2024-04-13 08:31:16.000000 geneticalgorithm2-6.9.0/setup.py
```

### Comparing `geneticalgorithm2-6.8.7/LICENSE` & `geneticalgorithm2-6.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geneticalgorithm2-6.8.7/PKG-INFO` & `geneticalgorithm2-6.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneticalgorithm2
-Version: 6.8.7
+Version: 6.9.0
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
+  - [6.9.0 reborn](#690-reborn)
   - [6.8.7 minor update](#687-minor-update)
   - [6.8.6 minor update](#686-minor-update)
   - [6.8.5 minor update](#685-minor-update)
   - [6.8.4 minor update](#684-minor-update)
   - [6.8.3 types update](#683-types-update)
   - [6.8.2 patch](#682-patch)
   - [6.8.1 patch](#681-patch)
@@ -169,14 +170,24 @@
 - `function_timeout` and `function` will be moved to `run()` method
 - new stop criteria callbacks (min std, max functions evaluations)
 - `vartype` will support strings like `iiiiibbf`
 
 ## **TODO firstly**
 - Remove old style mensions from README
 
+
+## 6.9.0 reborn
+
+- recreate the repository without excess heavy files materials 
+- host the [code documentation](https://pasaopasen.github.io/geneticalgorithm2/)
+- rename `geneticalgorithm2` class to `GeneticAlgorithm2`
+- substantial package architecture refactor
+- add more docstrings
+- reduce documentation duplicates 
+
 ## 6.8.7 minor update
 
 - some code refactor
 - fixes:
   - ensure the directory of generation file exists on save
 
 ## 6.8.6 minor update
@@ -297,15 +308,15 @@
 ## 6.3.0 minor update (refactoring)
 
 - type hints for entire part of functions
 - new valid forms for function parameters (now u don't need to use numpy arrays everywhere)
 - `AlgorithmParams` class for base GA algorithm parameters (instead of dictionary)
 - `Generation` class for saving/loading/returning generation (instead of dictionary)
 
-All that classes are collected [in file](geneticalgorithm2/classes.py). To maintain backward compatibility, `AlgorithmParams` and `Generation` classes have dictionary-like interface for getting fields: u can use `object.field` or `object['field']` notations.
+All that classes are collected [in file](geneticalgorithm2/data_types/classes.py). To maintain backward compatibility, `AlgorithmParams` and `Generation` classes have dictionary-like interface for getting fields: u can use `object.field` or `object['field']` notations.
 
 
 # Working process
 
 ## Main algorithm structure
 
 ```
@@ -340,29 +351,29 @@
 
 Firstly, u should **import needed packages**. All available (but not always necessary) imports are:
 
 ```python
 import numpy as np
 
 # the only one required import
-from geneticalgorithm2 import geneticalgorithm2 as ga # for creating and running optimization model
+from geneticalgorithm2 import GeneticAlgorithm2 as ga  # for creating and running optimization model
 
-from geneticalgorithm2 import Generation, AlgorithmParams # classes for comfortable parameters setting and getting
+from geneticalgorithm2 import Generation, AlgorithmParams  # classes for comfortable parameters setting and getting
 
-from geneticalgorithm2 import Crossover, Mutations, Selection # classes for specific mutation and crossover behavior
+from geneticalgorithm2 import Crossover, Mutations, Selection  # classes for specific mutation and crossover behavior
 
-from geneticalgorithm2 import Population_initializer # for creating better start population
+from geneticalgorithm2 import get_population_initializer  # for creating better start population
 
-from geneticalgorithm2 import np_lru_cache # for cache function (if u want)
+from geneticalgorithm2 import np_lru_cache  # for cache function (if u want)
 
-from geneticalgorithm2 import plot_pop_scores # for plotting population scores, if u want
+from geneticalgorithm2 import plot_pop_scores  # for plotting population scores, if u want
 
-from geneticalgorithm2 import Callbacks # simple callbacks (will be deprecated)
+from geneticalgorithm2 import Callbacks  # simple callbacks (will be deprecated)
 
-from geneticalgorithm2 import Actions, ActionConditions, MiddleCallbacks # middle callbacks
+from geneticalgorithm2 import Actions, ActionConditions, MiddleCallbacks  # middle callbacks
 ```
 
 Next step: **define minimized function** like
 
 ```python
 def function(X: np.ndarray) -> float: # X as 1d-numpy array
     return np.sum(X**2) + X.mean() + X.min() + X[0]*X[2] # some float result
@@ -579,40 +590,41 @@
 params = model.param
 ```
 
 An example of setting a new set of parameters for genetic algorithm and running `geneticalgorithm2` for our first simple example again:
 
 ```python
 import numpy as np
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
+
 
 def f(X):
     return np.sum(X)
-    
-    
-varbound=[(0,10)]*3
+
+
+varbound = [(0, 10)] * 3
 
 algorithm_param = {'max_num_iteration': 3000,
-                   'population_size':100,
+                   'population_size': 100,
                    'mutation_probability': 0.1,
                    'mutation_discrete_probability': None,
                    'elit_ratio': 0.01,
                    'parents_portion': 0.3,
-                   'crossover_type':'uniform',
+                   'crossover_type': 'uniform',
                    'mutation_type': 'uniform_by_center',
                    'mutation_discrete_type': 'uniform_discrete',
                    'selection_type': 'roulette',
-                   'max_iteration_without_improv':None}
+                   'max_iteration_without_improv': None}
 
-model=ga(function=f,
-            dimension=3,
-            variable_type='real',
-            variable_boundaries=varbound,
-            algorithm_parameters=algorithm_param
-        )
+model = ga(function=f,
+           dimension=3,
+           variable_type='real',
+           variable_boundaries=varbound,
+           algorithm_parameters=algorithm_param
+           )
 
 model.run()
 ```
 **Important**. U may use the small dictionary with only important parameters; other parameters will be default. It means the dictionary
 ```js
 algorithm_param = {'max_num_iteration': 150,
                    'population_size':1000}
@@ -804,21 +816,22 @@
 This is a trivial problem and we already know that the answer is `X = (0,0,0)` where `f(X) = 0`.  
 
 We just use this simple example to see how to implement geneticalgorithm2. First we import geneticalgorithm2 and [numpy](https://numpy.org). Next, we define 
 function `f` which we want to minimize and the boundaries of the decision variables. Then simply geneticalgorithm2 is called to solve the defined optimization problem as follows:
 
 ```python
 import numpy as np
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
+
 
 def f(X):
     return np.sum(X)
-    
-    
-varbound = [[0,10]]*3
+
+
+varbound = [[0, 10]] * 3
 
 model = ga(function=f, dimension=3, variable_type='real', variable_boundaries=varbound)
 
 model.run()
 ```
 
     
@@ -849,21 +862,22 @@
 
 Considering the problem given in the simple example above.
 Now assume all variables are integers. So `x1, x2, x3` can be any integers in `[0, 10]`.
 In this case the code is as the following:
 
 ```python
 import numpy as np
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
+
 
 def f(X):
     return np.sum(X)
-    
-    
-varbound = [[0,10]]*3
+
+
+varbound = [[0, 10]] * 3
 
 model = ga(function=f, dimension=3, variable_type='int', variable_boundaries=varbound)
 
 model.run()
 ```
 So, as it is seen the only difference is that for `variable_type` we use string `'int'`. 
 
@@ -871,19 +885,21 @@
 
 Considering the problem given in the simple example above.
 Now assume all variables are boolean instead of real or integer. So `X` can be either zero or one. Also instead of three let's have 30 variables.
 In this case the code is as the following:
 
 ```python
 import numpy as np
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
+
 
 def f(X):
     return np.sum(X)
 
+
 model = ga(function=f, dimension=30, variable_type='bool')
 
 model.run()
 ```
 
 Note for variable_type we use string `'bool'` when all variables are boolean.  
 Note that when variable_type equal `'bool'` there is no need for `variable_boundaries` to be defined.
@@ -893,43 +909,47 @@
 Considering the problem given in the the simple example above where we want to minimize `f(X) = x1 + x2 + x3`. 
 Now assume `x1` is a real (continuous) variable in `[0.5,1.5]`, `x2` is an integer variable in `[1,100]`, and `x3` is a boolean variable that can be either zero or one.
 We already know that the answer is `X = (0.5,1,0)` where `f(X) = 1.5`
 We implement geneticalgorithm2 as the following:
 
 ```python
 import numpy as np
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
+
 
 def f(X):
     return np.sum(X)
-    
-varbound = [[0.5,1.5],[1,100],[0,1]]
+
+
+varbound = [[0.5, 1.5], [1, 100], [0, 1]]
 vartype = ('real', 'int', 'int')
 model = ga(function=f, dimension=3, variable_type=vartype, variable_boundaries=varbound)
 
 model.run()
 ```
 
 ## Optimization problems with constraints
 In all above examples, the optimization problem was unconstrained. Now consider that we want to minimize `f(X) = x1+x2+x3` where `X` is a set of real variables in `[0, 10]`. Also we have an extra constraint so that sum of `x1` and `x2` is equal or greater than 2. The minimum of `f(X)` is 2.
 In such a case, a trick is to define penalty function. Hence we use the code below:
 
 ```python
 import numpy as np
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
+
 
 def f(X):
-    pen=0
-    if X[0]+X[1]<2:
-        pen=500+1000*(2-X[0]-X[1])
-    return np.sum(X)+pen
-    
-varbound=[[0,10]]*3
+    pen = 0
+    if X[0] + X[1] < 2:
+        pen = 500 + 1000 * (2 - X[0] - X[1])
+    return np.sum(X) + pen
+
 
-model=ga(function=f,dimension=3,variable_type='real',variable_boundaries=varbound)
+varbound = [[0, 10]] * 3
+
+model = ga(function=f, dimension=3, variable_type='real', variable_boundaries=varbound)
 
 model.run()
 
 ```
 As seen above we add a penalty to the objective function whenever the constraint is not met.  
 
 Some hints about how to define a penalty function:  
@@ -945,72 +965,73 @@
 
     From set like X = {x1, x2, x3, ..., xn} u should select only k objects which get the best function value
 
 U can do it using this code:
 
 ```python
 import numpy as np
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
 
+subset_size = 20  # how many objects we can choose
 
-subset_size = 20 # how many objects we can choose
+objects_count = 100  # how many objects are in set
 
-objects_count = 100 # how many objects are in set
+my_set = np.random.random(objects_count) * 10 - 5  # set values
 
-my_set = np.random.random(objects_count)*10 - 5 # set values
 
 # minimized function
 def f(X):
-    return abs(np.mean(my_set[X==1]) - np.median(my_set[X==1]))
+    return abs(np.mean(my_set[X == 1]) - np.median(my_set[X == 1]))
+
 
 # initialize start generation and params
 
-N = 1000 # size of population
+N = 1000  # size of population
 start_generation = np.zeros((N, objects_count))
-indexes = np.arange(0, objects_count, dtype = np.int8) # indexes of variables
+indexes = np.arange(0, objects_count, dtype=np.int8)  # indexes of variables
 
 for i in range(N):
-    inds = np.random.choice(indexes, subset_size, replace = False)
-    start_generation[i, inds] = 1 
+    inds = np.random.choice(indexes, subset_size, replace=False)
+    start_generation[i, inds] = 1
 
 
 def my_crossover(parent_a, parent_b):
     a_indexes = set(indexes[parent_a == 1])
     b_indexes = set(indexes[parent_b == 1])
-    
-    intersect = a_indexes.intersection(b_indexes) # elements in both parents
-    a_only = a_indexes - intersect # elements only in 'a' parent
+
+    intersect = a_indexes.intersection(b_indexes)  # elements in both parents
+    a_only = a_indexes - intersect  # elements only in 'a' parent
     b_only = b_indexes - intersect
-    
-    child_inds = np.array(list(a_only) + list(b_only), dtype = np.int8)
-    np.random.shuffle(child_inds) # mix
-    
+
+    child_inds = np.array(list(a_only) + list(b_only), dtype=np.int8)
+    np.random.shuffle(child_inds)  # mix
+
     children = np.zeros((2, parent_a.size))
     if intersect:
         children[:, np.array(list(intersect))] = 1
-    children[0, child_inds[:int(child_inds.size/2)]] = 1
-    children[1, child_inds[int(child_inds.size/2):]] = 1
-    
-    return children[0,:], children[1,:]
-    
+    children[0, child_inds[:int(child_inds.size / 2)]] = 1
+    children[1, child_inds[int(child_inds.size / 2):]] = 1
+
+    return children[0, :], children[1, :]
 
-model = ga(function=f, 
-           dimension=objects_count, 
+
+model = ga(function=f,
+           dimension=objects_count,
            variable_type='bool',
            algorithm_parameters={
-                       'max_num_iteration': 500,
-                       'mutation_probability': 0, # no mutation, just crossover
-                       'elit_ratio': 0.05,
-                       'parents_portion': 0.3,
-                       'crossover_type': my_crossover,
-                       'max_iteration_without_improv': 20
-               }
+               'max_num_iteration': 500,
+               'mutation_probability': 0,  # no mutation, just crossover
+               'elit_ratio': 0.05,
+               'parents_portion': 0.3,
+               'crossover_type': my_crossover,
+               'max_iteration_without_improv': 20
+           }
            )
 
-model.run(no_plot = False, start_generation=(start_generation, None))
+model.run(no_plot=False, start_generation=(start_generation, None))
 ```
 
 # U should know these features
 
 ## Available crossovers
 
 For two example parents (*one with ones* and *one with zeros*) next crossovers will give same children ([examples](tests/crossovers_examples.py)): 
@@ -1119,52 +1140,50 @@
 
 ```python
 import numpy as np
 import matplotlib.pyplot as plt
 
 from DiscreteHillClimbing import Hill_Climbing_descent
 
-from geneticalgorithm2 import geneticalgorithm2 as ga
-from geneticalgorithm2 import Population_initializer
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
+from geneticalgorithm2 import get_population_initializer
 
 
 def f(arr):
-    arr2 = arr/25
-    return -np.sum(arr2*np.sin(np.sqrt(np.abs(arr2))))**5 + np.sum(np.abs(arr2))**2
+    arr2 = arr / 25
+    return -np.sum(arr2 * np.sin(np.sqrt(np.abs(arr2)))) ** 5 + np.sum(np.abs(arr2)) ** 2
 
-iterations = 100    
-    
-varbound = [[-100, 100]]*15
 
-available_values = [np.arange(-100, 101)]*15
+iterations = 100
 
+varbound = [[-100, 100]] * 15
 
-my_local_optimizer = lambda arr, score: Hill_Climbing_descent(function = f, available_predictors_values=available_values, max_function_evals=50, start_solution=arr )
+available_values = [np.arange(-100, 101)] * 15
 
+my_local_optimizer = lambda arr, score: Hill_Climbing_descent(function=f, available_predictors_values=available_values,
+                                                              max_function_evals=50, start_solution=arr)
 
-model = ga(function=f, dimension=varbound.shape[0], 
-           variable_type='int', 
-           variable_boundaries = varbound,
+model = ga(function=f, dimension=varbound.shape[0],
+           variable_type='int',
+           variable_boundaries=varbound,
            algorithm_parameters={
                'max_num_iteration': iterations,
                'population_size': 400
-               })
-
+           })
 
 for time in ('before_select', 'after_select', 'never'):
-    model.run(no_plot = True,
-                  population_initializer = Population_initializer(
-                      select_best_of = 3,
-                      local_optimization_step = time,
-                      local_optimizer = my_local_optimizer
-                      )
-                  )
-
-    plt.plot(model.report, label = f"local optimization time = '{time}'")
+    model.run(no_plot=True,
+              population_initializer=get_population_initializer(
+                  select_best_of=3,
+                  local_optimization_step=time,
+                  local_optimizer=my_local_optimizer
+              )
+              )
 
+    plt.plot(model.report, label=f"local optimization time = '{time}'")
 
 plt.xlabel('Generation')
 plt.ylabel('Minimized function (40 simulations average)')
 plt.title('Selection best N object before running GA')
 plt.legend()
 ```
 
@@ -1215,47 +1234,49 @@
 Basically the model checks best population score (minimal score of generation) each generation and saves it to `report` field. Actually this sequence of numbers u see in big part of plots. This behavior is needed for several parts and u cannot disable it. But if u want to report some other metric without using [callbacks](#middle-callbacks), there is highly simple and fast way.
 
 After creating `model` but before running `run()` u need to append ur logic to `model.checked_reports` field. Take a look at example:
 
 ```python
 import numpy as np
 
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
 from geneticalgorithm2 import plot_several_lines
 
+
 def f(X):
-    return 50*np.sum(X) - np.sum(np.sqrt(X) * np.sin(X))
+    return 50 * np.sum(X) - np.sum(np.sqrt(X) * np.sin(X))
+
 
 dim = 25
-varbound = [[0 ,10]]*dim
+varbound = [[0, 10]] * dim
 
 model = ga(function=f, dimension=dim,
            variable_type='real', variable_boundaries=varbound,
            algorithm_parameters={
                'max_num_iteration': 600
            }
-)
+           )
 
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
-model.run(no_plot = False)
+model.run(no_plot=False)
 
 # now u have not only model.report but model.report_25 and so on
 
-#plot reports
+# plot reports
 names = [name for name, _ in model.checked_reports[::-1]]
 plot_several_lines(
     lines=[getattr(model, name) for name in names],
     colors=('green', 'black', 'red', 'blue'),
     labels=['median value', '25% quantile', 'mean of population', 'best pop score'],
     linewidths=(1, 1.5, 1, 2),
     title="Several custom reports with base reports",
@@ -1303,15 +1324,15 @@
 It's very simple to create your own `action` and `condition` functions. But there are several popular functions contained in `Actions` and `ActionConditions` classes:
 * `actions`:
   * `Stop()` -- just stop optimization process
   * `ReduceMutationProb(reduce_coef = 0.9)` -- reduce mutation probability
   * `ChangeRandomCrossover(available_crossovers: Sequence[Callable[[np.ndarray, np.ndarray], Tuple[np.ndarray, np.ndarray]]])` -- change another (random) crossover from list of crossovers
   * `ChangeRandomSelection(available_selections: Sequence[Callable[[np.ndarray, int], np.ndarray]])`
   * `ChangeRandomMutation(available_mutations: Sequence[Callable[[float, float, float], float]])`
-  * `RemoveDuplicates(oppositor = None, creator = None, converter = None)`; see [doc](geneticalgorithm2/callbacks.py)
+  * `RemoveDuplicates(oppositor = None, creator = None, converter = None)`; see [doc](geneticalgorithm2/callbacks/middle.py)
   * `CopyBest(by_indexes)` -- copies best population object values (from dimensions in `by_indexes`) to all population
   * `PlotPopulationScores(title_pattern = lambda data: f"Generation {data['current_generation']}", save_as_name_pattern = None)` -- plot population scores; needs 2 functions like `data`->string for title and file name (to save)
 * `conditions`:
   * `ActionConditions.EachGen(generation_step = 10)` -- do action each `generation_step` generations
   * `ActionConditions.Always()` do action each generations, equals to `ActionConditions.EachGen(1)`
   * `ActionConditions.AfterStagnation(stagnation_generations = 50)` -- do action after `stagnation_generations` stagnation generations
   * `ActionConditions.Several(list_of_conditions)` -- do action if all conditions in list are true
@@ -1665,48 +1686,50 @@
 ## How to plot population scores?
 
 There are 2 ways to plot of scores of population:
 * use `plot_pop_scores(scores, title = 'Population scores', save_as = None)` function from `geneticalgorithm2` environment
 * use `plot_generation_scores(self, title = 'Last generation scores', save_as = None)` method of `ga` object for plotting scores of last generation (yes, it's wrapper of previous function)
 
 Let's check example:
+
 ```python
 import numpy as np
 
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
+
+from geneticalgorithm2 import plot_pop_scores  # for plotting scores without ga object
 
-from geneticalgorithm2 import plot_pop_scores # for plotting scores without ga object
 
 def f(X):
-    return 50*np.sum(X) - np.sum(np.sqrt(X)*np.sin(X))
-    
+    return 50 * np.sum(X) - np.sum(np.sqrt(X) * np.sin(X))
+
+
 dim = 25
-varbound = [[0,10]]*dim
+varbound = [[0, 10]] * dim
 
 # create start population
 start_pop = np.random.uniform(0, 10, (50, dim))
 # eval scores of start population
 start_scores = np.array([f(start_pop[i]) for i in range(start_pop.shape[0])])
 
 # plot start scores using plot_pop_scores function
-plot_pop_scores(start_scores, title = 'Population scores before beginning of searching', save_as= 'plot_scores_start.png')
-
+plot_pop_scores(start_scores, title='Population scores before beginning of searching', save_as='plot_scores_start.png')
 
 model = ga(function=f, dimension=dim, variable_type='real', variable_boundaries=varbound)
 # run optimization process
-model.run(no_plot = True,
+model.run(no_plot=True,
           start_generation={
               'variables': start_pop,
               'scores': start_scores
-              })
+          })
 # plot and save optimization process plot
-model.plot_results(save_as = 'plot_scores_process.png')
+model.plot_results(save_as='plot_scores_process.png')
 
 # plot scores of last population
-model.plot_generation_scores(title = 'Population scores after ending of searching', save_as= 'plot_scores_end.png')
+model.plot_generation_scores(title='Population scores after ending of searching', save_as='plot_scores_end.png')
 ```
 ![](tests/output/plot_scores_start.png)
 ![](tests/output/plot_scores_process.png)
 ![](tests/output/plot_scores_end.png)
 
 
 
@@ -1743,156 +1766,153 @@
 
 By using `set_function` u can determine your own behavior for parallelism or u can use `geneticalgorithm2.set_function_multiprocess(f, n_jobs = -1)` for using just parallelism (recommended for heavy functions and big populations, not recommended for fast functions and small populations).
 
 For example:
 
 ```python
 import numpy as np
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
+
 
 def f(X):
     import math
     a = X[0]
     b = X[1]
     c = X[2]
     s = 0
     for i in range(10000):
-        s += math.sin(a*i) + math.sin(b*i) + math.cos(c*i)
+        s += math.sin(a * i) + math.sin(b * i) + math.cos(c * i)
 
     return s
- 
+
 
 algorithm_param = {'max_num_iteration': 50,
-                   'population_size':100,
-                   'mutation_probability':0.1,
+                   'population_size': 100,
+                   'mutation_probability': 0.1,
                    'elit_ratio': 0.01,
                    'parents_portion': 0.3,
-                   'crossover_type':'uniform',
+                   'crossover_type': 'uniform',
                    'mutation_type': 'uniform_by_center',
                    'selection_type': 'roulette',
-                   'max_iteration_without_improv':None}   
-    
-varbound = np.array([[-10,10]]*3)
+                   'max_iteration_without_improv': None}
 
-model = ga(function=f, dimension=3, 
-    variable_type='real',           
-    variable_boundaries=varbound, 
-    algorithm_parameters = algorithm_param)
+varbound = np.array([[-10, 10]] * 3)
+
+model = ga(function=f, dimension=3,
+           variable_type='real',
+           variable_boundaries=varbound,
+           algorithm_parameters=algorithm_param)
 
 ########
 
-%time model.run()
+%time
+model.run()
 # Wall time: 1min 52s
 
-%time model.run(set_function= ga.set_function_multiprocess(f, n_jobs = 6))
+%time
+model.run(set_function=ga.set_function_multiprocess(f, n_jobs=6))
 # Wall time: 31.7 s
 ```
 
 ## How to initialize start population? How to continue optimization with new run?
 
 For this there is `start_generation` parameter in `run()` method. It's the dictionary with structure like returned `model.output_dict['last_generation']`. Let's see example how can u to use it:
 
 ```python
 import numpy as np
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
+
 
 def f(X):
     return np.sum(X)
-    
+
+
 dim = 6
-    
-varbound = [(0,10)]*dim
 
+varbound = [(0, 10)] * dim
 
 algorithm_param = {'max_num_iteration': 500,
-                   'population_size':100,
-                   'mutation_probability':0.1,
+                   'population_size': 100,
+                   'mutation_probability': 0.1,
                    'elit_ratio': 0.01,
                    'parents_portion': 0.3,
-                   'crossover_type':'uniform',
-                   'max_iteration_without_improv':None}
+                   'crossover_type': 'uniform',
+                   'max_iteration_without_improv': None}
 
-model = ga(function=f, 
-           dimension=dim, 
-           variable_type='real', 
+model = ga(function=f,
+           dimension=dim,
+           variable_type='real',
            variable_boundaries=varbound,
-           algorithm_parameters = algorithm_param)
+           algorithm_parameters=algorithm_param)
 
 # start generation
 # as u see u can use any values been valid for ur function
-samples = np.random.uniform(0, 50, (300, dim)) # 300 is the new size of your generation
-
-
+samples = np.random.uniform(0, 50, (300, dim))  # 300 is the new size of your generation
 
-model.run(no_plot = False, start_generation={'variables':samples, 'scores': None}) 
+model.run(no_plot=False, start_generation={'variables': samples, 'scores': None})
 # it's not necessary to evaluate scores before
 # but u can do it if u have evaluated scores and don't wanna repeat calculations
 
 
-
 # from version 6.3.0 it's recommended to use this form
 from geneticalgorithm2 import Generation
-model.run(no_plot = False, start_generation=Generation(variables = samples, scores = None))
 
+model.run(no_plot=False, start_generation=Generation(variables=samples, scores=None))
 
 # from version 6.4.0 u also can use these forms
-model.run(no_plot = False, start_generation= samples)
-model.run(no_plot = False, start_generation= (samples, None))
-
+model.run(no_plot=False, start_generation=samples)
+model.run(no_plot=False, start_generation=(samples, None))
 
 # if u have scores array, u can put it too
 scores = np.array([f(sample) for sample in samples])
-model.run(no_plot = False, start_generation= (samples, scores))
-
+model.run(no_plot=False, start_generation=(samples, scores))
 
 ##
 ## after first run
 ## best value = 0.10426190111045064
 ##
 
 # okay, let's continue optimization using saved last generation
-model.run(no_plot = True, start_generation=model.output_dict['last_generation']) 
+model.run(no_plot=True, start_generation=model.output_dict['last_generation'])
 
 ##
 ## after second run
 ## best value = 0.06128462776296528
 ##
 
 ```
 
 Also u can save and load populations using likely code:
 
 ```python
 import numpy as np
 
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
 
 from OptimizationTestFunctions import Eggholder
 
+dim = 2 * 15
 
-dim = 2*15
-
-f =  Eggholder(dim)
+f = Eggholder(dim)
 
 xmin, xmax, ymin, ymax = f.bounds
-        
-varbound = np.array([[xmin, xmax], [ymin, ymax]]*15)
-    
+
+varbound = np.array([[xmin, xmax], [ymin, ymax]] * 15)
+
 model = ga(function=f,
-               dimension = dim,
-               variable_type='real',
-               variable_boundaries=varbound,
-               algorithm_parameters = {
-                       'max_num_iteration': 300,
-                       'population_size': 100
-                       })
+           dimension=dim,
+           variable_type='real',
+           variable_boundaries=varbound,
+           algorithm_parameters={
+               'max_num_iteration': 300,
+               'population_size': 100
+           })
 
 # first run and save last generation to file
 filename = "eggholder_lastgen.npz"
-model.run(save_last_generation_as = filename)
-
+model.run(save_last_generation_as=filename)
 
 # load start generation from file and run again (continue optimization)
 model.run(start_generation=filename)
 ```
```

### Comparing `geneticalgorithm2-6.8.7/README.rst` & `geneticalgorithm2-6.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `geneticalgorithm2-6.8.7/geneticalgorithm2/cache.py` & `geneticalgorithm2-6.9.0/geneticalgorithm2/utils/cache.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 
 from functools import lru_cache, wraps
 
 #from fastcache import clru_cache
 
-from .aliases import array1D
+from geneticalgorithm2.utils.aliases import array1D
 
 
 def np_lru_cache(*args, **kwargs):
     """
     LRU cache implementation for functions whose FIRST parameter is a numpy array
         forked from: https://gist.github.com/Susensio/61f4fee01150caaac1e10fc5f005eb75
     """
```

### Comparing `geneticalgorithm2-6.8.7/geneticalgorithm2/callbacks.py` & `geneticalgorithm2-6.9.0/geneticalgorithm2/callbacks/middle.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,256 +1,186 @@
 
-from typing import List, Optional, Callable, Tuple, Sequence
+from typing import Optional, Callable, Tuple, Sequence
 
-import os
 import random
 
 import numpy as np
 
 from OppOpPopInit import OppositionOperators, SampleInitializers
+from OppOpPopInit.oppositor import OppositorFunc
+from OppOpPopInit.initialiser import CreatorFunc
 
-from .aliases import TypeAlias, array1D, array2D, PathLike
-from .files import mkdir_of_file, mkdir
+from ..utils.aliases import array1D, array2D
+from ..utils.funcs import union_to_matrix, fast_max
 
-from .classes import MiddleCallbackData, Generation
-
-from .utils import union_to_matrix, fast_max
-
-from .crossovers import CrossoverFunc
-from .selections import SelectionFunc
-from .mutations import MutationFunc
-
-
-CallbackFunc: TypeAlias = Callable[[int, List[float], array2D, array1D], None]
-MiddleCallbackActionFunc: TypeAlias = Callable[[MiddleCallbackData], MiddleCallbackData]
-MiddleCallbackConditionFunc: TypeAlias = Callable[[MiddleCallbackData], bool]
-MiddleCallbackFunc: TypeAlias = Callable[[MiddleCallbackData], Tuple[MiddleCallbackData, bool]]
-
-
-class Callbacks:
-    
-    @staticmethod
-    def NoneCallback():
-        return lambda generation_number, report_list, last_population, last_scores: None
-
-    @staticmethod
-    def SavePopulation(folder: PathLike, save_gen_step: int = 50, file_prefix: str = 'population') -> CallbackFunc:
-        
-        mkdir(folder)
-
-        def func(generation_number: int, report_list: List[float], last_population: array2D, last_scores: array1D):
-    
-            if generation_number % save_gen_step != 0:
-                return
-
-            Generation(last_population, last_scores).save(
-                os.path.join(
-                    folder,
-                    f"{file_prefix}_{generation_number}.npz"
-                )
-            )
-        
-        return func
-    
-    @staticmethod
-    def PlotOptimizationProcess(
-        folder: PathLike,
-        save_gen_step: int = 50,
-        show: bool = False,
-        main_color: str = 'green',
-        file_prefix: str = 'report'
-    ) -> CallbackFunc:
-        import matplotlib.pyplot as plt
-        from matplotlib.ticker import MaxNLocator
-        
-        mkdir(folder)
-
-        def func(generation_number: int, report_list: List[float], last_population: array2D, last_scores: array1D):
-
-            if generation_number % save_gen_step != 0:
-                return
-
-            # if len(report_list) == 0:
-            #     sys.stdout.write("No results to plot!\n")
-            #     return
-            
-            ax = plt.axes()
-            ax.xaxis.set_major_locator(MaxNLocator(integer=True))
-            
-            plt.plot(
-                np.arange(1, 1 + len(report_list)),
-                report_list,
-                color=main_color,
-                label='best of generation',
-                linewidth=2
-            )
-            
-            plt.xlabel('Generation')
-            plt.ylabel('Minimized function')
-            plt.title('GA optimization process')
-            plt.legend()
-            
-            plt.savefig(os.path.join(folder, f"{file_prefix}_{generation_number}.png"), dpi=200)
-
-            if show:
-                plt.show()
-            else:
-                plt.close()
-        
-        return func
+from ..data_types.generation import Generation
+from .data import MiddleCallbackData, MiddleCallbackActionFunc, \
+    MiddleCallbackConditionFunc, MiddleCallbackFunc
+
+from ..crossovers import CrossoverFunc
+from ..selections import SelectionFunc
+from ..mutations import MutationFunc
 
 
 class Actions:
+    """Static class of built-in middle callback actions"""
 
     @staticmethod
     def Stop(reason_name: str = 'stopped by Stop callback') -> MiddleCallbackActionFunc:
+        """stops optimization"""
         
         def func(data: MiddleCallbackData):
             data.reason_to_stop = reason_name
             return data
         return func
 
     @staticmethod
     def ReduceMutationProb(reduce_coef: float = 0.9) -> MiddleCallbackActionFunc:
-        
+        """reduces mutation prob by the coefficient"""
+
         def func(data: MiddleCallbackData):
             data.mutation_prob *= reduce_coef
             return data
         
         return func
 
-
     #def DualStrategyStep():
     #    pass
 
     #def SetFunction():
     #    pass
 
-
     @staticmethod
     def ChangeRandomCrossover(
         available_crossovers: Sequence[CrossoverFunc]
     ) -> MiddleCallbackActionFunc:
+        """randomly changes crossover"""
 
         def func(data: MiddleCallbackData):
             data.crossover = random.choice(available_crossovers)
             return data
 
         return func
     
     @staticmethod
     def ChangeRandomSelection(available_selections: Sequence[SelectionFunc]) -> MiddleCallbackActionFunc:
+        """randomly changes selection function"""
 
         def func(data: MiddleCallbackData):
             data.selection = random.choice(available_selections)
             return data
 
         return func
 
     @staticmethod
     def ChangeRandomMutation(available_mutations: Sequence[MutationFunc]) -> MiddleCallbackActionFunc:
+        """randomly changes mutation function"""
 
         def func(data):
             data.mutation = random.choice(available_mutations)
             return data
 
         return func
-    
 
     @staticmethod
     def RemoveDuplicates(
-        oppositor: Optional[Callable[[array1D], array1D]] = None,
-        creator: Optional[Callable[[], array1D]] = None,
+        oppositor: Optional[OppositorFunc] = None,
+        creator: Optional[CreatorFunc] = None,
         converter: Optional[Callable[[array1D], array1D]] = None
     ) -> MiddleCallbackActionFunc:
         """
         Removes duplicates from population
 
-        Parameters
-        ----------
-        oppositor : oppositor from OppOpPopInit, optional
-            oppositor for applying after duplicates removing. By default -- using just random initializer from creator.
-                The default is None.
-        creator : the function creates population samples, optional
-            the function creates population samples if oppositor is None. The default is None.
-        converter : func, optional
-            function converts population samples in new format to compare (if needed). The default is None.
+        Args:
+            oppositor: oppositor from OppOpPopInit, optional
+                oppositor for applying after duplicates removing.
+                None (default) means to just use the random initializer from creator.
+            creator: the function creates population samples, optional
+                the function creates population samples if oppositor is None. The default is None.
+            converter: function converts (preprocesses) population samples in new format to compare (if needed)
+                before duplicates will be searched
 
         """
 
-        if creator is None and oppositor is None:
-            raise Exception("No functions to fill population! creator or oppositors must be not None")
-
+        assert creator is not None or oppositor is not None, (
+            "No functions to fill population! creator or oppositors must be not None"
+        )
+
+        #
+        # create the function searches for duplicates
+        #
         if converter is None:
             def without_dup(pop: array2D, scores: array1D) -> Tuple[array2D, int]:
                 """returns population without dups"""
                 _, index_of_dups = np.unique(pop, axis=0, return_index=True)
                 return union_to_matrix(pop[index_of_dups], scores[index_of_dups]), pop.shape[0] - index_of_dups.size
         else:
-             def without_dup(pop: array2D, scores: array1D) -> Tuple[array2D, int]:
+            def without_dup(pop: array2D, scores: array1D) -> Tuple[array2D, int]:
                 """returns population without dups"""
                 _, index_of_dups = np.unique(
-                    np.array([converter(pop[i]) for i in range(pop.shape[0])]), axis=0, return_index=True
+                    np.array([converter(r) for r in pop]),
+                    axis=0, return_index=True
                 )
                 return union_to_matrix(pop[index_of_dups], scores[index_of_dups]), pop.shape[0] - index_of_dups.size
 
-
+        #
+        # create the function will create new samples instead of removed duplicates
+        #
         if oppositor is None:
             def remover(pop: array2D, scores: array1D, set_function: Callable[[array2D], array1D]) -> array2D:
 
                 pp, count_to_create = without_dup(pop, scores)  # pop without dups
                 pp2 = np.empty((count_to_create, pp.shape[1])) 
                 pp2[:, :-1] = SampleInitializers.CreateSamples(creator, count_to_create)  # new pop elements
                 pp2[:, -1] = set_function(pp2[:, :-1])  # new elements values
 
                 new_pop = np.vstack((pp, pp2))
 
-                return new_pop[np.argsort(new_pop[:, -1])]  # new pop
+                return new_pop[new_pop[:, -1].argsort()]  # new pop
 
         else:  # using oppositors
             def remover(pop: array2D, scores: array1D, set_function: Callable[[array2D], array1D]) -> array2D:
 
                 pp, count_to_create = without_dup(pop, scores)  # pop without dups
 
                 if count_to_create > pp.shape[0]:
                     raise Exception("Too many duplicates, cannot oppose")
                 
                 if count_to_create == 0:
-                    return pp[np.argsort(pp[:, -1])]
+                    return pp[pp[:, -1].argsort()]
                 
                 pp2 = np.empty((count_to_create, pp.shape[1])) 
                 # oppose count_to_create worse elements
                 pp2[:, :-1] = OppositionOperators.Reflect(pp[-count_to_create:, :-1], oppositor)  # new pop elements
                 pp2[:, -1] = set_function(pp2[:, :-1])  # new elements values
                     
                 new_pop = np.vstack((pp, pp2))
                     
-                return new_pop[np.argsort(new_pop[:, -1])]  # new pop
+                return new_pop[new_pop[:, -1].argsort()]  # new pop
 
         def func(data: MiddleCallbackData):
             new_pop = remover(
                 data.last_generation.variables,
                 data.last_generation.scores,
                 data.set_function
             )
 
             data.last_generation = Generation.from_pop_matrix(new_pop)
 
             return data
-
         
         return func
     
     @staticmethod
     def CopyBest(by_indexes: Sequence[int]) -> MiddleCallbackActionFunc:
         """
         Copies best population object values (from dimensions in by_indexes) to all population
         """
 
-        if type(by_indexes) != np.ndarray:
+        if not isinstance(by_indexes, np.ndarray):
             by_indexes = np.array(by_indexes)
 
         def func(data: MiddleCallbackData):
 
             pop = data.last_generation.variables
             scores = data.last_generation.scores
 
@@ -266,15 +196,15 @@
         title_pattern: Callable[[MiddleCallbackData], str] = lambda data: f"Generation {data.current_generation}",
         save_as_name_pattern: Optional[Callable[[MiddleCallbackData], str]] = None
     ) -> MiddleCallbackActionFunc:
         """
         plots population scores
         needs 2 functions like data->str for title and file name
         """
-        from .plotting_tools import plot_pop_scores
+        from ..utils.plotting import plot_pop_scores
 
         use_save_as = (lambda data: None) if save_as_name_pattern is None else save_as_name_pattern
 
         def local_plot_callback(data: MiddleCallbackData):
 
             plot_pop_scores(
                 data.last_generation.scores,
@@ -284,15 +214,16 @@
 
             return data
 
         return local_plot_callback
 
 
 class ActionConditions:
-    
+    """Static class of built-in middle callback actions"""
+
     @staticmethod
     def EachGen(generation_step: int = 10) -> MiddleCallbackConditionFunc:
 
         if generation_step < 1 or type(generation_step) is not int:
             raise Exception(f"Invalid generation step {generation_step}! Should be int and >=1")
         
         if generation_step == 1:
@@ -313,36 +244,57 @@
     @staticmethod
     def AfterStagnation(stagnation_generations: int = 50) -> MiddleCallbackConditionFunc:
 
         def func(data: MiddleCallbackData):
             return data.current_stagnation % stagnation_generations == 0 and data.current_stagnation > 0
         return func
 
-
     @staticmethod
-    def Several(conditions: Sequence[MiddleCallbackConditionFunc]) -> MiddleCallbackConditionFunc:
+    def All(conditions: Sequence[MiddleCallbackConditionFunc]) -> MiddleCallbackConditionFunc:
         """
         returns function which checks all conditions from conditions
         """
 
         def func(data: MiddleCallbackData):
             return all(cond(data) for cond in conditions)
         
         return func
 
+    @staticmethod
+    def Any(conditions: Sequence[MiddleCallbackConditionFunc]) -> MiddleCallbackConditionFunc:
+        """
+        returns function which checks for any conditions from conditions
+        """
+
+        def func(data: MiddleCallbackData):
+            return any(cond(data) for cond in conditions)
+
+        return func
+
 
 class MiddleCallbacks:
+    """Static class for middle callbacks creation"""
 
     @staticmethod
     def UniversalCallback(
         action: MiddleCallbackActionFunc,
         condition: MiddleCallbackConditionFunc,
         set_data_after_callback: bool = True
     ) -> MiddleCallbackFunc:
-        
+        """
+        universal function which constructs middle callback from action and condition
+        Args:
+            action:
+            condition:
+            set_data_after_callback: whether to signal internal data update if action update the data
+
+        Returns:
+
+        """
+
         def func(data: MiddleCallbackData):
 
             cond = condition(data)
             if cond:
                 data = action(data)
 
             return data, (cond if set_data_after_callback else False)
@@ -385,24 +337,22 @@
 
     #def ReduceMutationStagnation(reduce = 0.5, stagnation_gens = 50):
     #    pass 
 
     @staticmethod
     def GeneDiversityStats(step_generations_for_plotting: int = 10) -> MiddleCallbackFunc:
 
-        if step_generations_for_plotting < 1:
-            raise Exception(f"Wrong step = {step_generations_for_plotting}, should be int and > 0!!")
+        assert step_generations_for_plotting > 0, step_generations_for_plotting
 
         import matplotlib.pyplot as plt
 
         div = []
         count = []
         most = []
 
-
         def func(data: MiddleCallbackData):
 
             nonlocal div, count, most
 
             dt = data.last_generation.variables
 
             uniq, counts = np.unique(dt, return_counts=True, axis=0)
```

### Comparing `geneticalgorithm2-6.8.7/geneticalgorithm2/crossovers.py` & `geneticalgorithm2-6.9.0/geneticalgorithm2/crossovers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 
 from typing import Callable, Tuple, Dict
 
 import random
 import numpy as np
 
-from .aliases import TypeAlias, array1D
+from .utils.aliases import TypeAlias, array1D
 
 CrossoverFunc: TypeAlias = Callable[[array1D, array1D], Tuple[array1D, array1D]]
+"""
+Function (parent1, parent2) -> (child1, child2)
+"""
 
 
 def get_copies(x: array1D, y: array1D) -> Tuple[array1D, array1D]:
     return x.copy(), y.copy()
 
 
 class Crossover:
+    """Crossover functions static class"""
 
     @staticmethod
     def crossovers_dict() -> Dict[str, CrossoverFunc]:
         return {
-            'one_point': Crossover.one_point(),
-            'two_point': Crossover.two_point(),
-            'uniform': Crossover.uniform(),
-            'segment': Crossover.segment(),
-            'shuffle': Crossover.shuffle(),
+            n: getattr(Crossover, n)()
+            for n in (
+                'one_point',
+                'two_point',
+                'uniform',
+                'segment',
+                'shuffle',
+            )
         }
     
     @staticmethod
     def one_point() -> CrossoverFunc:
         
         def func(x: array1D, y: array1D):
             ofs1, ofs2 = get_copies(x, y)
@@ -88,15 +95,15 @@
     @staticmethod
     def shuffle() -> CrossoverFunc:
         
         def func(x: array1D, y: array1D):
             
             ofs1, ofs2 = get_copies(x, y)
             
-            index = np.random.choice(np.arange(0, x.size), x.size, replace = False)
+            index = np.random.choice(np.arange(0, x.size), x.size, replace=False)
             
             ran = np.random.randint(0, x.size)
             
             for i in range(ran):
                 ind = index[i]
                 ofs1[ind] = y[ind]
                 ofs2[ind] = x[ind]
```

### Comparing `geneticalgorithm2-6.8.7/geneticalgorithm2/geneticalgorithm2.py` & `geneticalgorithm2-6.9.0/geneticalgorithm2/geneticalgorithm2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,159 +1,146 @@
-"""
-Copyright 2021 Demetry Pascal (forked from Ryan (Mohammad) Solgi)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of 
-this software and associated documentation files (the "Software"), to deal in 
-the Software without restriction, including without limitation the rights to use, 
-copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the 
-Software, and to permit persons to whom the Software is furnished to do so, 
-subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, 
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL 
-THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, 
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE 
-SOFTWARE.
-"""
-
 
-from typing import Callable, List, Tuple, Optional, Dict, Any, Union, Sequence, Set, Literal
+from typing import Callable, List, Tuple, Optional, Dict, Any, Union, Sequence, Literal, Iterable
 from typing_extensions import TypeAlias
 
 import collections
 import warnings
 import operator
 
-
 import sys
 import time
 import random
 import math
 
 import numpy as np
 
+from OppOpPopInit.initialiser import CreatorFunc
+from OppOpPopInit.oppositor import OppositorFunc
+
 #region INTERNAL IMPORTS
 
-from .aliases import array1D, array2D
+from .utils.aliases import array1D, array2D
 
-from .classes import AlgorithmParams, Generation, MiddleCallbackData, GAResult, GenerationConvertible
+from .data_types.aliases import FunctionToMinimize, SetFunctionToMinimize
+from .data_types.algorithm_params import AlgorithmParams
+from .data_types.generation import GenerationConvertible, Generation
+from .data_types.result import GAResult
 
-from .initializer import Population_initializer
-from .plotting_tools import plot_pop_scores, plot_several_lines
+from .population_initializer import get_population_initializer, PopulationModifier
+from .utils.plotting import plot_pop_scores, plot_several_lines
 
-from .utils import can_be_prob, is_numpy, is_current_gen_number, fast_min, random_indexes_pair
+from .utils.funcs import can_be_prob, is_numpy, is_current_gen_number, fast_min, random_indexes_pair
 
-from .callbacks import MiddleCallbackFunc, CallbackFunc
+from .callbacks.data import MiddleCallbackData
+from .callbacks import MiddleCallbackFunc, SimpleCallbackFunc
 
 #endregion
 
 #region ALIASES
 
 VARIABLE_TYPE: TypeAlias = Literal['int', 'real', 'bool']
+"""
+the variable type for a given or all dimension, determines the values discretion:
+    real: double numbers
+    int: integer number only
+    bool: in the fact is integer with bounds [0, 1]
+"""
 
 #endregion
 
 
-class geneticalgorithm2:
-    
+class GeneticAlgorithm2:
     """
-    Genetic Algorithm (Elitist version) for Python
-    
-    An implementation of elitist genetic algorithm for solving problems with
-    continuous, integers, or mixed variables.
-    
-    repo path https://github.com/PasaOpasen/geneticalgorithm2
+    Genetic algorithm optimization process
     """
     
     default_params = AlgorithmParams()
     PROGRESS_BAR_LEN = 20
+    """max count of symbols in the progress bar"""
 
     @property
     def output_dict(self):
         warnings.warn(
-            "'output_dict' is deprecated and will be removed at version 7 \n use 'result' instead"
+            "'output_dict' is deprecated and will be removed at version 7 \n"
+            "use 'result' instead"
         )
         return self.result
 
     @property
     def needs_mutation(self) -> bool:
+        """whether the mutation is required"""
         return self.prob_mut > 0 or self.prob_mut_discrete > 0
 
     #region INIT
 
     def __init__(
         self,
-        function: Callable[[array1D], float],
+        function: FunctionToMinimize,
 
         dimension: int,
         variable_type: Union[VARIABLE_TYPE, Sequence[VARIABLE_TYPE]] = 'bool',
         variable_boundaries: Optional[Union[array2D, Sequence[Tuple[float, float]]]] = None,
 
         variable_type_mixed=None,
 
         function_timeout: Optional[float] = None,
         algorithm_parameters: Union[AlgorithmParams, Dict[str, Any]] = default_params
     ):
         """
+        initializes the GA object and performs main checks
+
         Args:
-            function <Callable[[np.ndarray], float]> - the given objective function to be minimized
-            #NOTE: This implementation minimizes the given objective function.
-            (For maximization multiply function by a negative sign: the absolute
-            value of the output would be the actual objective function)
-
-            dimension <integer> - the number of decision variables
-
-            variable_type <string> - 'bool' if all variables are Boolean;
-            'int' if all variables are integer; and 'real' if all variables are
-            real value or continuous. For mixed types use sequence of string of type for each variable
-
-            variable_boundaries <Optional[Union[np.ndarray, Sequence[Tuple[float, float]]]]> - Default None; leave it
-            None if variable_type is 'bool'; otherwise provide an array of tuples
-            of length two as boundaries for each variable;
-            the length of the array must be equal dimension. For example,
-            np.array([0,100],[0,200]) determines lower boundary 0 and upper boundary 100 for first
-            and upper boundary 200 for second variable where dimension is 2.
+            function: the given objective function to be minimized
+            dimension: the number of decision variables, the population samples dimention
+
+            variable_type: string means the variable type for all variables,
+                for mixed types use sequence of strings of type for each variable
+
+            variable_boundaries: leave it None if variable_type is 'bool';
+                otherwise provide a sequence of tuples of length two as boundaries for each variable;
+                the length of the array must be equal dimension.
+                For example, ([0,100], [0,200]) determines
+                    lower boundary 0 and upper boundary 100 for first
+                    and upper boundary 200 for second variable
+                    and dimension must be 2.
 
             variable_type_mixed -- deprecated
 
-            function_timeout <float> - if the given function does not provide
-            output before function_timeout (unit is seconds) the algorithm raise error.
-            For example, when there is an infinite loop in the given function. `None` means disabling
-
-            algorithm_parameters <Union[AlgorithmParams, Dict[str, Any]]>:
-                @ max_num_iteration <int> - stoping criteria of the genetic algorithm (GA)
-                @ population_size <int>
-                @ mutation_probability <float in [0,1]>
-                @ elit_ratio <float in [0,1]>
-                @ crossover_probability <float in [0,1]>
-                @ parents_portion <float in [0,1]>
-                @ crossover_type <string/function> - Default is 'uniform'; 'one_point' or 'two_point' (not only) are other options
-                @ mutation_type <string/function> - Default is 'uniform_by_x'; see GitHub to check other options
-                @ mutation_discrete_type <string/function> - mutation type for discrete variables
-                @ selection_type <string/function> - Default is 'roulette'; see GitHub to check other options
-                @ max_iteration_without_improv <int> - maximum number of successive iterations without improvement. If None it is ineffective
+            function_timeout: if the given function does not provide
+                output before function_timeout (unit is seconds) the algorithm raises error.
+                For example, when there is an infinite loop in the given function.
+                `None` means disabling
+
+            algorithm_parameters: AlgorithmParams object or usual dictionary with algorithm parameter;
+                it is not mandatory to provide all possible parameters
+
+        Notes:
+            - This implementation minimizes the given objective function.
+            For maximization u can multiply the function by -1 (for instance): the absolute
+                value of the output would be the actual objective function
+
+            - If u want to use set_function only and maybe u dont have usual function,
+                just set the function to something like lambda x: 0 but set function_timeout=None too
 
         for more details and examples of implementation please visit:
             https://github.com/PasaOpasen/geneticalgorithm2
   
         """
 
         # all default fields
 
-        self.param: AlgorithmParams = None
         # self.crossover: Callable[[np.ndarray, np.ndarray], Tuple[np.ndarray, np.ndarray]] = None
         # self.real_mutation: Callable[[float, float, float], float] = None
         # self.discrete_mutation: Callable[[int, int, int], int] = None
         # self.selection: Callable[[np.ndarray, int], np.ndarray] = None
 
+        self.revolution_oppositor = None
+        self.dup_oppositor = None
+        self.creator = None
+        self.init_oppositors = None
         self.f: Callable[[array1D], float] = None
         self.funtimeout: float = None
         self.set_function: Callable[[np.ndarray], np.ndarray] = None
 
         # self.dim: int = None
         self.var_bounds: List[Tuple[Union[int, float], Union[int, float]]] = None
         # self.indexes_int: np.ndarray = None
@@ -167,17 +154,17 @@
         # input algorithm's parameters
 
         assert isinstance(algorithm_parameters, (dict, AlgorithmParams)), (
             "algorithm_parameters must be dict or AlgorithmParams object"
         )
         if not isinstance(algorithm_parameters, AlgorithmParams):
             algorithm_parameters = AlgorithmParams.from_dict(algorithm_parameters)
-
-        algorithm_parameters.check_if_valid()
+        algorithm_parameters.validate()
         self.param = algorithm_parameters
+
         self.crossover, self.real_mutation, self.discrete_mutation, self.selection = algorithm_parameters.get_CMS_funcs()
 
         # dimension and area bounds
         self.dim = int(dimension)
         assert self.dim > 0, f"dimension count must be int and >0, gotten {dimension}"
 
         if variable_type_mixed is not None:
@@ -221,15 +208,16 @@
 
         #############################################################
         
         self.population_size = int(self.param.population_size)
         self._set_parents_count(self.param.parents_portion)
         self._set_elit_count(self.population_size, self.param.elit_ratio)
         assert self.parents_count >= self.elit_count, (
-            f"\n number of parents ({self.parents_count}) must be greater than number of elits ({self.elit_count})"
+            f"\n number of parents ({self.parents_count}) "
+            f"must be greater than number of elits ({self.elit_count})"
         )
 
         self._set_max_iterations()
 
         self._set_report()
 
         # specify this function to speed up or change default behaviour
@@ -378,17 +366,17 @@
 
     #region RUN METHODS
 
     def _progress(self, count: int, total: int, status: str = ''):
 
         part = count / total
 
-        filled_len = round(geneticalgorithm2.PROGRESS_BAR_LEN * part)
+        filled_len = round(GeneticAlgorithm2.PROGRESS_BAR_LEN * part)
         percents = round(100.0 * part, 1)
-        bar = '|' * filled_len + '_' * (geneticalgorithm2.PROGRESS_BAR_LEN - filled_len)
+        bar = '|' * filled_len + '_' * (GeneticAlgorithm2.PROGRESS_BAR_LEN - filled_len)
 
         self.progress_stream.write('\r%s %s%s %s' % (bar, percents, '%', status))
         self.progress_stream.flush()
 
     def __str__(self):
         return f"Genetic algorithm object with parameters {self.param}"
 
@@ -417,59 +405,59 @@
         tp = type(obj)
         assert (
             tp in (int, float) or np.issubdtype(tp, np.floating) or np.issubdtype(tp, np.integer)
         ), f"Minimized function should return a number, but got '{obj}' object with type {tp}"
 
         return obj, eval_time
 
-    def _set_mutation_indexes(self, mutation_indexes: Optional[Sequence[int]]):
+    def _set_mutation_indexes(self, mutation_indexes: Optional[Iterable[int]]):
 
         if mutation_indexes is None:
             self.indexes_float_mut = self.indexes_float
             self.indexes_int_mut = self.indexes_int
         else:
             tmp_indexes = set(mutation_indexes)
-            self.indexes_int_mut = np.array(list(set(self.indexes_int).intersection(tmp_indexes)))
-            self.indexes_float_mut = np.array(list(set(self.indexes_float).intersection(tmp_indexes)))
+            self.indexes_int_mut = np.array(list(tmp_indexes.intersection(self.indexes_int)))
+            self.indexes_float_mut = np.array(list(tmp_indexes.intersection(self.indexes_float)))
 
             if self.indexes_float_mut.size == 0 and self.indexes_int_mut.size == 0:
                 warnings.warn(f"No mutation dimensions!!! Check ur mutation indexes!!")
 
     #@profile
     def run(
         self,
         no_plot: bool = False,
         disable_printing: bool = False,
         progress_bar_stream: Optional[str] = 'stdout',
 
         # deprecated
         disable_progress_bar: bool = False,
 
-        set_function: Optional[Callable[[array2D], array1D]] = None,
+        set_function: SetFunctionToMinimize = None,
         apply_function_to_parents: bool = False,
         start_generation: GenerationConvertible = Generation(),
         studEA: bool = False,
-        mutation_indexes: Optional[Union[Sequence[int], Set[int]]] = None,
+        mutation_indexes: Optional[Iterable[int]] = None,
 
-        init_creator: Optional[Callable[[], array1D]] = None,
-        init_oppositors: Optional[Sequence[Callable[[array1D], array1D]]] = None,
+        init_creator: Optional[CreatorFunc] = None,
+        init_oppositors: Optional[Sequence[OppositorFunc]] = None,
 
-        duplicates_oppositor: Optional[Callable[[array1D], array1D]] = None,
+        duplicates_oppositor: Optional[OppositorFunc] = None,
         remove_duplicates_generation_step: Optional[int] = None,
 
-        revolution_oppositor: Optional[Callable[[array1D], array1D]] = None,
+        revolution_oppositor: Optional[OppositorFunc] = None,
         revolution_after_stagnation_step: Optional[int] = None,
         revolution_part: float = 0.3,
 
         population_initializer: Tuple[
-            int, Callable[[array2D, array1D], Tuple[array2D, array1D]]
-        ] = Population_initializer(select_best_of=1, local_optimization_step='never', local_optimizer=None),
+            int, PopulationModifier
+        ] = get_population_initializer(select_best_of=1, local_optimization_step='never', local_optimizer=None),
 
         stop_when_reached: Optional[float] = None,
-        callbacks: Optional[Sequence[CallbackFunc]] = None,
+        callbacks: Optional[Sequence[SimpleCallbackFunc]] = None,
         middle_callbacks: Optional[Sequence[MiddleCallbackFunc]] = None,  #+
         time_limit_secs: Optional[float] = None,
         save_last_generation_as: Optional[str] = None,
         seed: Optional[int] = None
     ):
         """
         runs optimization process
@@ -477,50 +465,48 @@
         Args:
             no_plot: do not plot results using matplotlib by default
 
             disable_printing: do not print log info of optimization process
 
             progress_bar_stream: 'stdout', 'stderr' or None to disable progress bar
 
-            disable_progress_bar:
+            disable_progress_bar: deprecated
 
-            set_function : 2D-array -> 1D-array function,
-                which applyes to matrix of population (size (samples, dimention))
-                    to estimate their values
+            set_function: set function to be used instead of usual function
 
-            apply_function_to_parents: apply function to parents from previous generation (if it's needed)
+            apply_function_to_parents: whether to apply function to parents from previous generation (if it's needed)
 
-            start_generation: Generation object or a dictionary with structure
-                {'variables':2D-array of samples, 'scores': function values on samples}
-                or path to .npz file (str) with saved generation; if 'scores' value is None the scores will be compute
+            start_generation: initial generation object of any `GenerationConvertible` type
 
             studEA: using stud EA strategy (crossover with best object always)
 
             mutation_indexes: indexes of dimensions where mutation can be performed (all dimensions by default)
 
             init_creator: the function creates population samples.
                 By default -- random uniform for real variables and random uniform for int
             init_oppositors: the list of oppositors creates oppositions for base population. No by default
+
             duplicates_oppositor: oppositor for applying after duplicates removing.
                 By default -- using just random initializer from creator
             remove_duplicates_generation_step: step for removing duplicates (have a sense with discrete tasks).
                 No by default
+
             revolution_oppositor: oppositor for revolution time. No by default
             revolution_after_stagnation_step: create revolution after this generations of stagnation. No by default
             revolution_part: float, the part of generation to being oppose. By default is 0.3
 
             population_initializer: object for actions at population initialization step
                 to create better start population. See doc
 
             stop_when_reached: stop searching after reaching this value (it can be potential minimum or something else)
 
             callbacks: sequence of callback functions with structure:
                 (generation_number, report_list, last_population, last_scores) -> do some action
 
-            middle_callbacks: sequence of functions made MiddleCallbacks class
+            middle_callbacks: sequence of functions made `MiddleCallback` class
 
             time_limit_secs: limit time of working (in seconds)
 
             save_last_generation_as: path to .npz file for saving last_generation as numpy dictionary like
                 {'population': 2D-array, 'scores': 1D-array}, None if doesn't need to save in file
 
             seed: random seed (None if doesn't matter)
@@ -580,19 +566,15 @@
         )
 
         t: int = 0
         count_stagnation: int = 0
         pop: array2D = None
         scores: array1D = None
 
-        #
-        #
-        # callbacks part
-        #
-        #
+        #region CALLBACKS
 
         def get_data():
             """
             returns all important data about model
             """
             return MiddleCallbackData(
                 last_generation=Generation(pop, scores),
@@ -669,26 +651,26 @@
                 for cb in middle_callbacks:
                     data, has_sense = cb(data)
                     if has_sense:
                         flag = True
                 if flag:
                     set_data(data)  # update global date if there was real callback step
 
-        ############################################################
+        #endregion
 
         start_time = time.time()
         time_is_done = (
             (lambda: False)
             if time_limit_secs is None
             else (lambda: int(time.time() - start_time) >= time_limit_secs)
         )
 
-        ############################################################# 
-        # Initial Population
-        self.set_function = set_function or geneticalgorithm2.default_set_function(self.f)
+        self.set_function = set_function or GeneticAlgorithm2.default_set_function(self.f)
+
+        #region Initial population, duplicates filter, revolutionary
 
         pop_coef, initializer_func = population_initializer
         
         # population creator by random or with oppositions
         if init_creator is None:
 
             from OppOpPopInit import SampleInitializers
@@ -828,14 +810,16 @@
                 if SHOW_PROGRESS:
                     show_progress(t, self.max_iterations,
                                   f"GA is running...{t} gen from {self.max_iterations}. Revolution!")
 
                 args = args[:scores.size]
                 return combined[args], combined_scores[args]
 
+        #enregion
+
         #
         #
         #  START ALGORITHM LOGIC
         #
         #
 
         # Report
```

### Comparing `geneticalgorithm2-6.8.7/geneticalgorithm2/initializer.py` & `geneticalgorithm2-6.9.0/geneticalgorithm2/population_initializer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,101 @@
 
 from typing import Callable, Optional, Tuple, Literal
 
 import numpy as np
 
-from .aliases import TypeAlias, array1D, array2D
+from .utils.aliases import TypeAlias, array1D, array2D
 
 
-LOCAL_OPT_STEPS: TypeAlias = Literal['before_select', 'after_select', 'never']
+PopulationModifier: TypeAlias = Callable[[array2D, array1D], Tuple[array2D, array1D]]
+"""
+function (population matrix, population scores) -> (new matrix, new scores)
+which will perform the bests selection and local optimization and other population transformations
+"""
+
+LOCAL_OPTIMIZATION_STEP_CASE: TypeAlias = Literal['before_select', 'after_select', 'never']
+"""
+When the local optimization (candidates enhancing) must be performed:
+    * 'never' -- don't do local optimization
+    * 'before_select' -- before selection best N objects 
+        (example: do local optimization for 5N objects and select N best results)
+    * 'after_select' -- do local optimization on best selected N objects
+"""
 
 
-def Population_initializer(
+def get_population_initializer(
     select_best_of: int = 4,
-    local_optimization_step: LOCAL_OPT_STEPS = 'never',
+    local_optimization_step: LOCAL_OPTIMIZATION_STEP_CASE = 'never',
     local_optimizer: Optional[
         Callable[
             [array1D, float],
             Tuple[array1D, float]
         ]
     ] = None
-) -> Tuple[int, Callable[[array2D, array1D], Tuple[array2D, array1D]]]:
+) -> Tuple[int, PopulationModifier]:
     """
-    select_best_of (int) -- select 1/select_best_of best part of start population. For example, for select_best_of = 4 and population_size = N will be selected N best objects from 5N generated objects (if start_generation = None dictionary). If start_generation is not None dictionary, it will be selected best size(start_generation)/N  objects
-
-    local_optimization_step (str) -- when should we do local optimization? Available values:
-    
-    * 'never' -- don't do local optimization
-    * 'before_select' -- before selection best N objects (example: do local optimization for 5N objects and select N best results)
-    * 'after_select' -- do local optimization on best selected N objects
+    Args:
+        select_best_of: determines population size to select 1/select_best_of best part of start population.
+            For example, for select_best_of = 4 and population_size = N there will be selected N best objects
+                from 5N generated objects (if start_generation=None dictionary).
+            If start_generation is not None dictionary, there will be selected best (start_generation) / N objects
+        local_optimization_step: when to perform local optimization
+        local_optimizer: the local optimization function (object array, its score) -> (modified array, its score)
 
-    local_optimizer (function) -- local optimization function like:
-        def loc_opt(object_as_array, current_score):
-            # some code
-            return better_object_as_array, better_score
+    Returns:
+        select_best_of, population modifier
     """
     
-    assert (select_best_of > 0 and type(select_best_of) == int), "select_best_of argument should be integer and more than 0"
-
-    assert (local_optimization_step in LOCAL_OPT_STEPS.__args__), f"local_optimization_step should be in {LOCAL_OPT_STEPS.__args__}, but got {local_optimization_step}"
-
-    if local_optimizer is None and local_optimization_step in LOCAL_OPT_STEPS.__args__[:2]:
-        raise Exception(f"for local_optimization_step from {LOCAL_OPT_STEPS.__args__[:2]} local_optimizer function mustn't be None")
+    assert select_best_of > 0 and isinstance(select_best_of, int), (select_best_of, type(select_best_of))
 
+    assert local_optimization_step in LOCAL_OPTIMIZATION_STEP_CASE.__args__, (
+        local_optimization_step, LOCAL_OPTIMIZATION_STEP_CASE.__args__
+    )
+
+    if local_optimizer is None and local_optimization_step in LOCAL_OPTIMIZATION_STEP_CASE.__args__[:2]:
+        raise Exception(
+            f"for local_optimization_step from {LOCAL_OPTIMIZATION_STEP_CASE.__args__[:2]} "
+            f"local_optimizer function mustn't be None"
+        )
 
-    def Select_best(population: array2D, scores: array1D) -> Tuple[array2D, array1D]:
+    def select_best(population: array2D, scores: array1D) -> Tuple[array2D, array1D]:
         args = np.argsort(scores)
         args = args[:round(args.size/select_best_of)]
         return population[args], scores[args]
 
-    def Local_opt(population: array2D, scores: array1D):
+    def local_opt(population: array2D, scores: array1D):
         _pop, _score = zip(
             *[
                 local_optimizer(population[i], scores[i]) for i in range(scores.size)
             ]
         )
         return np.array(_pop), np.array(_score)
 
-
     #def Create_population(func, start_generation, expected_size, #variable_boundaries):
     #    
     #    if not (start_generation['variables'] is None):
     #        pop = start_generation['variables']
     #        scores = start_generation['scores']
     #        if scores is None:
     #            scores = np.array([func(pop[i, :]) for i in range(pop.shape[0])])
     #        return pop, scores
 
-
-    def Result(population: array2D, scores: array1D):
+    def process_population(population: array2D, scores: array1D):
         if local_optimization_step == 'before_select':
-            pop, s = Local_opt(population, scores)
-            return Select_best(pop, s)
+            pop, s = local_opt(population, scores)
+            return select_best(pop, s)
 
         if local_optimization_step == 'after_select':
-            pop, s = Select_best(population, scores)
-            return Local_opt(pop, s)
+            pop, s = select_best(population, scores)
+            return local_opt(pop, s)
 
         #if local_optimization_step == 'never':
-        return Select_best(population, scores)
-    
+        return select_best(population, scores)
 
-    return select_best_of, Result
+    return select_best_of, process_population
```

### Comparing `geneticalgorithm2-6.8.7/geneticalgorithm2/mutations.py` & `geneticalgorithm2-6.9.0/geneticalgorithm2/mutations.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,49 @@
 
 from typing import Callable, Dict, Union
 
 import random
 import numpy as np
 
 
-from .utils import fast_min, fast_max
+from .utils.aliases import TypeAlias
+from .utils.funcs import fast_min, fast_max
 
-from .aliases import TypeAlias
 
 MutationFloatFunc: TypeAlias = Callable[[float, float, float], float]
 MutationIntFunc: TypeAlias = Callable[[int, int, int], int]
 MutationFunc: TypeAlias = Union[MutationIntFunc, MutationFloatFunc]
+"""
+Function (x, left, right) -> value
+
+Which mutates x to value according to bounds (left, right)
+"""
 
 
 class Mutations:
+    """Mutations functions static class"""
 
     @staticmethod
     def mutations_dict() -> Dict[str, MutationFloatFunc]:
         return {
-            'uniform_by_x': Mutations.uniform_by_x(),
-            'uniform_by_center': Mutations.uniform_by_center(),
-            'gauss_by_center': Mutations.gauss_by_center(),
-            'gauss_by_x': Mutations.gauss_by_x(),
+            n: getattr(Mutations, n)()
+            for n in (
+                'uniform_by_x',
+                'uniform_by_center',
+                'gauss_by_center',
+                'gauss_by_x',
+            )
         }
 
     @staticmethod
     def mutations_discrete_dict() -> Dict[str, MutationIntFunc]:
         return {
             'uniform_discrete': Mutations.uniform_discrete()
         }
 
-
     @staticmethod
     def uniform_by_x() -> MutationFloatFunc:
         
         def func(x: float, left: float, right: float):
             alp: float = fast_min(x - left, right - x)
             return random.uniform(x - alp, x + alp)
         return func
```

### Comparing `geneticalgorithm2-6.8.7/geneticalgorithm2/plotting_tools.py` & `geneticalgorithm2-6.9.0/geneticalgorithm2/utils/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from typing import Optional, Sequence
 
 import numpy as np
 
-from .aliases import PathLike
+from geneticalgorithm2.utils.aliases import PathLike
 from .files import mkdir_of_file
 
 
 def plot_several_lines(
     lines: Sequence[Sequence[float]],
     colors: Sequence[str],
     labels: Optional[Sequence[str]] = None,
@@ -47,14 +47,15 @@
     plt.legend()
 
     if save_as is not None:
         plt.savefig(save_as, dpi=dpi)
 
     plt.show()
 
+
 def plot_pop_scores(scores: Sequence[float], title: str = 'Population scores', save_as: Optional[str] = None):
     """
     plots scores (numeric values) as sorted bars
     """
     # import matplotlib
     # matplotlib.use('Agg')
     import matplotlib.pyplot as plt
@@ -72,16 +73,14 @@
         for rect in rects[-1:]:
             height = round(rect.get_height(), 2)
             ax.annotate('{}'.format(height),
                         xy=(rect.get_x() + rect.get_width() / 2, height),
                         xytext=(0, 3),  # 3 points vertical offset
                         textcoords="offset points",
                         ha='center', va='bottom', fontsize=14, fontweight='bold')
-    
-
 
     cols = np.zeros(len(sc))
     cols[-1] = 1
 
     x_coord = np.arange(len(sc))
     my_norm = Normalize(vmin=0, vmax=1)
     
@@ -92,15 +91,14 @@
     #ax.set_xticks(x_coord)
     ax.set_title(title, fontsize=16, fontweight='bold')
     ax.set_xlabel('Population objects')
     ax.set_ylabel('Cost values')
     #ax.set_ylim([0, max(subdict.values())*1.2])
     #fig.suptitle(title, fontsize=15, fontweight='bold')
 
-    
     fig.tight_layout()
     
     if save_as is not None:
         mkdir_of_file(save_as)
         plt.savefig(save_as, dpi=200)
     
     plt.show()
```

### Comparing `geneticalgorithm2-6.8.7/geneticalgorithm2/selections.py` & `geneticalgorithm2-6.9.0/geneticalgorithm2/selections.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,87 +1,99 @@
 
 from typing import Callable, Dict, List
 
 import math
 import random
 import numpy as np
 
-from .aliases import array1D, TypeAlias
+from .utils.aliases import array1D, TypeAlias
 
 SelectionFunc: TypeAlias = Callable[[array1D, int], array1D]
+"""
+Function (scores, count to select) -> indexes of selected
+"""
 
 
+#region UTILS
+
+def inverse_scores(scores: array1D) -> array1D:
+    """
+    inverses scores (min val goes to max)
+    """
+    minobj = scores[0]
+    normobj = scores - minobj if minobj < 0 else scores
+
+    return (np.amax(normobj) + 1) - normobj
+
+
+def roulette(scores: array1D, parents_count: int) -> array1D:
+    """simplest roulette selector for which the highest score means more preferred"""
+
+    sum_normobj = np.sum(scores)
+    prob = scores / sum_normobj
+    cumprob = np.cumsum(prob)
+
+    parents_indexes = np.array(
+        [
+            index if index < cumprob.size else np.random.randint(0, index - 1)
+            for index in (
+                np.searchsorted(cumprob, np.random.random())
+                for _ in range(parents_count)
+            )
+        ]
+    )
+
+    return parents_indexes
+
+
+#endregion
+
 class Selection:
+    """
+    Selections functions static class
+    """
 
     @staticmethod
     def selections_dict() -> Dict[str, SelectionFunc]:
         return {
-            'fully_random': Selection.fully_random(),
-            'roulette': Selection.roulette(),
-            'stochastic': Selection.stochastic(),
-            'sigma_scaling': Selection.sigma_scaling(),
-            'ranking': Selection.ranking(),
-            'linear_ranking': Selection.linear_ranking(),
-            'tournament': Selection.tournament(),
+            n: getattr(Selection, n)()
+            for n in (
+                'fully_random',
+                'roulette',
+                'stochastic',
+                'sigma_scaling',
+                'ranking',
+                'linear_ranking',
+                'tournament',
+            )
         }
 
     @staticmethod
-    def __inverse_scores(scores: array1D) -> array1D:
-        """
-        inverse scores (min val goes to max)
-        """
-        minobj = scores[0]
-        normobj = scores - minobj if minobj < 0 else scores
-                
-        return (np.amax(normobj) + 1) - normobj
-
-    @staticmethod
     def fully_random() -> SelectionFunc:
+        """returns the selector of fully random parents (for tests purposes)"""
         
         def func(scores: array1D, parents_count: int):
             indexes = np.arange(parents_count)
-            return np.random.choice(indexes, parents_count, replace = False)
+            return np.random.choice(indexes, parents_count, replace=False)
         
         return func
 
     @staticmethod
-    def __roulette(scores: array1D, parents_count: int) -> array1D:
-        
-        sum_normobj = np.sum(scores)
-        prob = scores/sum_normobj
-        cumprob = np.cumsum(prob)            
-            
-        parents_indexes = np.empty(parents_count)
-            
-        # it can be vectorized
-        for k in range(parents_count):
-            index = np.searchsorted(cumprob, np.random.random())
-            if index < cumprob.size:
-                parents_indexes[k] = index
-            else:
-                parents_indexes[k] = np.random.randint(0, index - 1)
-            
-        return parents_indexes
-
-    @staticmethod
     def roulette() -> SelectionFunc:
         
         def func(scores: array1D, parents_count: int):
-
-            normobj = Selection.__inverse_scores(scores)
-
-            return Selection.__roulette(normobj, parents_count)
+            return roulette(inverse_scores(scores), parents_count)
         
         return func
 
     @staticmethod
     def stochastic() -> SelectionFunc:
         
         def func(scores: np.ndarray, parents_count: int):
-            f = Selection.__inverse_scores(scores)
+            f = inverse_scores(scores)
             
             fN: float = 1.0 / parents_count
             k: int = 0
             acc: float = 0.0
             parents: List[int] = []
             r: float = random.random() * fN
             
@@ -101,15 +113,15 @@
         
         return func
 
     @staticmethod
     def sigma_scaling(epsilon: float = 0.01, is_noisy: bool = False) -> SelectionFunc:
         
         def func(scores: array1D, parents_count):
-            f = Selection.__inverse_scores(scores)
+            f = inverse_scores(scores)
             
             sigma = np.std(f, ddof = 1) if is_noisy else np.std(f)
             average = np.mean(f)
             
             if sigma == 0:
                 f = 1
             else:
@@ -119,39 +131,42 @@
         
         return func
 
     @staticmethod
     def ranking() -> SelectionFunc:
         
         def func(scores: array1D, parents_count: int):
-            return Selection.__roulette(1 + np.arange(parents_count)[::-1], parents_count)
+            return roulette(1 + np.arange(parents_count)[::-1], parents_count)
         
         return func
 
     @staticmethod
     def linear_ranking(selection_pressure: float = 1.5) -> SelectionFunc:
         
-        assert (selection_pressure > 1 and selection_pressure < 2), f"selection_pressure should be in (1, 2), but got {selection_pressure}"
+        assert 1 <= selection_pressure <= 2, f"selection_pressure should be in (1, 2), but got {selection_pressure}"
         
         def func(scores: array1D, parents_count: int):
             tmp = parents_count * (parents_count-1)
             alpha = (2 * parents_count - selection_pressure * (parents_count + 1)) / tmp
             beta = 2 * (selection_pressure - 1) / tmp
-            
-            
+
             a = -2 * alpha - beta
             b = (2 * alpha + beta) ** 2
             c = 8 * beta
             d = 2 * beta
             
             indexes = np.arange(parents_count)
             
-            return np.array([indexes[-round((a + math.sqrt(b + c*random.random()))/d)] for _ in range(parents_count)])
-            
-        
+            return np.array(
+                [
+                    indexes[-round((a + math.sqrt(b + c * random.random())) / d)]
+                    for _ in range(parents_count)
+                ]
+            )
+
         return func
 
     @staticmethod
     def tournament(tau: int = 2) -> SelectionFunc:
 
         # NOTE
         # this code really does tournament selection
@@ -159,19 +174,18 @@
         
         def func(scores: array1D, parents_count: int):
             
             indexes = np.arange(parents_count)
             
             return np.array(
                 [
-                    np.min(np.random.choice(indexes, tau, replace = False)) 
+                    np.min(np.random.choice(indexes, tau, replace=False))
                     for _ in range(parents_count)
                 ]
             )
-            
         
         return func
```

### Comparing `geneticalgorithm2-6.8.7/geneticalgorithm2/utils.py` & `geneticalgorithm2-6.9.0/geneticalgorithm2/utils/funcs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 
 from typing import Optional, Any, Tuple
 
-from pathlib import Path
-
 import random
 import numpy as np
 
-from .aliases import array1D, array2D
+from geneticalgorithm2.utils.aliases import array1D, array2D
 
 
 def fast_min(a, b):
     '''
     1.5 times faster than row min(a, b)
     '''
     return a if a < b else b
```

### Comparing `geneticalgorithm2-6.8.7/geneticalgorithm2.egg-info/PKG-INFO` & `geneticalgorithm2-6.9.0/geneticalgorithm2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneticalgorithm2
-Version: 6.8.7
+Version: 6.9.0
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
+  - [6.9.0 reborn](#690-reborn)
   - [6.8.7 minor update](#687-minor-update)
   - [6.8.6 minor update](#686-minor-update)
   - [6.8.5 minor update](#685-minor-update)
   - [6.8.4 minor update](#684-minor-update)
   - [6.8.3 types update](#683-types-update)
   - [6.8.2 patch](#682-patch)
   - [6.8.1 patch](#681-patch)
@@ -169,14 +170,24 @@
 - `function_timeout` and `function` will be moved to `run()` method
 - new stop criteria callbacks (min std, max functions evaluations)
 - `vartype` will support strings like `iiiiibbf`
 
 ## **TODO firstly**
 - Remove old style mensions from README
 
+
+## 6.9.0 reborn
+
+- recreate the repository without excess heavy files materials 
+- host the [code documentation](https://pasaopasen.github.io/geneticalgorithm2/)
+- rename `geneticalgorithm2` class to `GeneticAlgorithm2`
+- substantial package architecture refactor
+- add more docstrings
+- reduce documentation duplicates 
+
 ## 6.8.7 minor update
 
 - some code refactor
 - fixes:
   - ensure the directory of generation file exists on save
 
 ## 6.8.6 minor update
@@ -297,15 +308,15 @@
 ## 6.3.0 minor update (refactoring)
 
 - type hints for entire part of functions
 - new valid forms for function parameters (now u don't need to use numpy arrays everywhere)
 - `AlgorithmParams` class for base GA algorithm parameters (instead of dictionary)
 - `Generation` class for saving/loading/returning generation (instead of dictionary)
 
-All that classes are collected [in file](geneticalgorithm2/classes.py). To maintain backward compatibility, `AlgorithmParams` and `Generation` classes have dictionary-like interface for getting fields: u can use `object.field` or `object['field']` notations.
+All that classes are collected [in file](geneticalgorithm2/data_types/classes.py). To maintain backward compatibility, `AlgorithmParams` and `Generation` classes have dictionary-like interface for getting fields: u can use `object.field` or `object['field']` notations.
 
 
 # Working process
 
 ## Main algorithm structure
 
 ```
@@ -340,29 +351,29 @@
 
 Firstly, u should **import needed packages**. All available (but not always necessary) imports are:
 
 ```python
 import numpy as np
 
 # the only one required import
-from geneticalgorithm2 import geneticalgorithm2 as ga # for creating and running optimization model
+from geneticalgorithm2 import GeneticAlgorithm2 as ga  # for creating and running optimization model
 
-from geneticalgorithm2 import Generation, AlgorithmParams # classes for comfortable parameters setting and getting
+from geneticalgorithm2 import Generation, AlgorithmParams  # classes for comfortable parameters setting and getting
 
-from geneticalgorithm2 import Crossover, Mutations, Selection # classes for specific mutation and crossover behavior
+from geneticalgorithm2 import Crossover, Mutations, Selection  # classes for specific mutation and crossover behavior
 
-from geneticalgorithm2 import Population_initializer # for creating better start population
+from geneticalgorithm2 import get_population_initializer  # for creating better start population
 
-from geneticalgorithm2 import np_lru_cache # for cache function (if u want)
+from geneticalgorithm2 import np_lru_cache  # for cache function (if u want)
 
-from geneticalgorithm2 import plot_pop_scores # for plotting population scores, if u want
+from geneticalgorithm2 import plot_pop_scores  # for plotting population scores, if u want
 
-from geneticalgorithm2 import Callbacks # simple callbacks (will be deprecated)
+from geneticalgorithm2 import Callbacks  # simple callbacks (will be deprecated)
 
-from geneticalgorithm2 import Actions, ActionConditions, MiddleCallbacks # middle callbacks
+from geneticalgorithm2 import Actions, ActionConditions, MiddleCallbacks  # middle callbacks
 ```
 
 Next step: **define minimized function** like
 
 ```python
 def function(X: np.ndarray) -> float: # X as 1d-numpy array
     return np.sum(X**2) + X.mean() + X.min() + X[0]*X[2] # some float result
@@ -579,40 +590,41 @@
 params = model.param
 ```
 
 An example of setting a new set of parameters for genetic algorithm and running `geneticalgorithm2` for our first simple example again:
 
 ```python
 import numpy as np
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
+
 
 def f(X):
     return np.sum(X)
-    
-    
-varbound=[(0,10)]*3
+
+
+varbound = [(0, 10)] * 3
 
 algorithm_param = {'max_num_iteration': 3000,
-                   'population_size':100,
+                   'population_size': 100,
                    'mutation_probability': 0.1,
                    'mutation_discrete_probability': None,
                    'elit_ratio': 0.01,
                    'parents_portion': 0.3,
-                   'crossover_type':'uniform',
+                   'crossover_type': 'uniform',
                    'mutation_type': 'uniform_by_center',
                    'mutation_discrete_type': 'uniform_discrete',
                    'selection_type': 'roulette',
-                   'max_iteration_without_improv':None}
+                   'max_iteration_without_improv': None}
 
-model=ga(function=f,
-            dimension=3,
-            variable_type='real',
-            variable_boundaries=varbound,
-            algorithm_parameters=algorithm_param
-        )
+model = ga(function=f,
+           dimension=3,
+           variable_type='real',
+           variable_boundaries=varbound,
+           algorithm_parameters=algorithm_param
+           )
 
 model.run()
 ```
 **Important**. U may use the small dictionary with only important parameters; other parameters will be default. It means the dictionary
 ```js
 algorithm_param = {'max_num_iteration': 150,
                    'population_size':1000}
@@ -804,21 +816,22 @@
 This is a trivial problem and we already know that the answer is `X = (0,0,0)` where `f(X) = 0`.  
 
 We just use this simple example to see how to implement geneticalgorithm2. First we import geneticalgorithm2 and [numpy](https://numpy.org). Next, we define 
 function `f` which we want to minimize and the boundaries of the decision variables. Then simply geneticalgorithm2 is called to solve the defined optimization problem as follows:
 
 ```python
 import numpy as np
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
+
 
 def f(X):
     return np.sum(X)
-    
-    
-varbound = [[0,10]]*3
+
+
+varbound = [[0, 10]] * 3
 
 model = ga(function=f, dimension=3, variable_type='real', variable_boundaries=varbound)
 
 model.run()
 ```
 
     
@@ -849,21 +862,22 @@
 
 Considering the problem given in the simple example above.
 Now assume all variables are integers. So `x1, x2, x3` can be any integers in `[0, 10]`.
 In this case the code is as the following:
 
 ```python
 import numpy as np
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
+
 
 def f(X):
     return np.sum(X)
-    
-    
-varbound = [[0,10]]*3
+
+
+varbound = [[0, 10]] * 3
 
 model = ga(function=f, dimension=3, variable_type='int', variable_boundaries=varbound)
 
 model.run()
 ```
 So, as it is seen the only difference is that for `variable_type` we use string `'int'`. 
 
@@ -871,19 +885,21 @@
 
 Considering the problem given in the simple example above.
 Now assume all variables are boolean instead of real or integer. So `X` can be either zero or one. Also instead of three let's have 30 variables.
 In this case the code is as the following:
 
 ```python
 import numpy as np
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
+
 
 def f(X):
     return np.sum(X)
 
+
 model = ga(function=f, dimension=30, variable_type='bool')
 
 model.run()
 ```
 
 Note for variable_type we use string `'bool'` when all variables are boolean.  
 Note that when variable_type equal `'bool'` there is no need for `variable_boundaries` to be defined.
@@ -893,43 +909,47 @@
 Considering the problem given in the the simple example above where we want to minimize `f(X) = x1 + x2 + x3`. 
 Now assume `x1` is a real (continuous) variable in `[0.5,1.5]`, `x2` is an integer variable in `[1,100]`, and `x3` is a boolean variable that can be either zero or one.
 We already know that the answer is `X = (0.5,1,0)` where `f(X) = 1.5`
 We implement geneticalgorithm2 as the following:
 
 ```python
 import numpy as np
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
+
 
 def f(X):
     return np.sum(X)
-    
-varbound = [[0.5,1.5],[1,100],[0,1]]
+
+
+varbound = [[0.5, 1.5], [1, 100], [0, 1]]
 vartype = ('real', 'int', 'int')
 model = ga(function=f, dimension=3, variable_type=vartype, variable_boundaries=varbound)
 
 model.run()
 ```
 
 ## Optimization problems with constraints
 In all above examples, the optimization problem was unconstrained. Now consider that we want to minimize `f(X) = x1+x2+x3` where `X` is a set of real variables in `[0, 10]`. Also we have an extra constraint so that sum of `x1` and `x2` is equal or greater than 2. The minimum of `f(X)` is 2.
 In such a case, a trick is to define penalty function. Hence we use the code below:
 
 ```python
 import numpy as np
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
+
 
 def f(X):
-    pen=0
-    if X[0]+X[1]<2:
-        pen=500+1000*(2-X[0]-X[1])
-    return np.sum(X)+pen
-    
-varbound=[[0,10]]*3
+    pen = 0
+    if X[0] + X[1] < 2:
+        pen = 500 + 1000 * (2 - X[0] - X[1])
+    return np.sum(X) + pen
+
 
-model=ga(function=f,dimension=3,variable_type='real',variable_boundaries=varbound)
+varbound = [[0, 10]] * 3
+
+model = ga(function=f, dimension=3, variable_type='real', variable_boundaries=varbound)
 
 model.run()
 
 ```
 As seen above we add a penalty to the objective function whenever the constraint is not met.  
 
 Some hints about how to define a penalty function:  
@@ -945,72 +965,73 @@
 
     From set like X = {x1, x2, x3, ..., xn} u should select only k objects which get the best function value
 
 U can do it using this code:
 
 ```python
 import numpy as np
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
 
+subset_size = 20  # how many objects we can choose
 
-subset_size = 20 # how many objects we can choose
+objects_count = 100  # how many objects are in set
 
-objects_count = 100 # how many objects are in set
+my_set = np.random.random(objects_count) * 10 - 5  # set values
 
-my_set = np.random.random(objects_count)*10 - 5 # set values
 
 # minimized function
 def f(X):
-    return abs(np.mean(my_set[X==1]) - np.median(my_set[X==1]))
+    return abs(np.mean(my_set[X == 1]) - np.median(my_set[X == 1]))
+
 
 # initialize start generation and params
 
-N = 1000 # size of population
+N = 1000  # size of population
 start_generation = np.zeros((N, objects_count))
-indexes = np.arange(0, objects_count, dtype = np.int8) # indexes of variables
+indexes = np.arange(0, objects_count, dtype=np.int8)  # indexes of variables
 
 for i in range(N):
-    inds = np.random.choice(indexes, subset_size, replace = False)
-    start_generation[i, inds] = 1 
+    inds = np.random.choice(indexes, subset_size, replace=False)
+    start_generation[i, inds] = 1
 
 
 def my_crossover(parent_a, parent_b):
     a_indexes = set(indexes[parent_a == 1])
     b_indexes = set(indexes[parent_b == 1])
-    
-    intersect = a_indexes.intersection(b_indexes) # elements in both parents
-    a_only = a_indexes - intersect # elements only in 'a' parent
+
+    intersect = a_indexes.intersection(b_indexes)  # elements in both parents
+    a_only = a_indexes - intersect  # elements only in 'a' parent
     b_only = b_indexes - intersect
-    
-    child_inds = np.array(list(a_only) + list(b_only), dtype = np.int8)
-    np.random.shuffle(child_inds) # mix
-    
+
+    child_inds = np.array(list(a_only) + list(b_only), dtype=np.int8)
+    np.random.shuffle(child_inds)  # mix
+
     children = np.zeros((2, parent_a.size))
     if intersect:
         children[:, np.array(list(intersect))] = 1
-    children[0, child_inds[:int(child_inds.size/2)]] = 1
-    children[1, child_inds[int(child_inds.size/2):]] = 1
-    
-    return children[0,:], children[1,:]
-    
+    children[0, child_inds[:int(child_inds.size / 2)]] = 1
+    children[1, child_inds[int(child_inds.size / 2):]] = 1
+
+    return children[0, :], children[1, :]
 
-model = ga(function=f, 
-           dimension=objects_count, 
+
+model = ga(function=f,
+           dimension=objects_count,
            variable_type='bool',
            algorithm_parameters={
-                       'max_num_iteration': 500,
-                       'mutation_probability': 0, # no mutation, just crossover
-                       'elit_ratio': 0.05,
-                       'parents_portion': 0.3,
-                       'crossover_type': my_crossover,
-                       'max_iteration_without_improv': 20
-               }
+               'max_num_iteration': 500,
+               'mutation_probability': 0,  # no mutation, just crossover
+               'elit_ratio': 0.05,
+               'parents_portion': 0.3,
+               'crossover_type': my_crossover,
+               'max_iteration_without_improv': 20
+           }
            )
 
-model.run(no_plot = False, start_generation=(start_generation, None))
+model.run(no_plot=False, start_generation=(start_generation, None))
 ```
 
 # U should know these features
 
 ## Available crossovers
 
 For two example parents (*one with ones* and *one with zeros*) next crossovers will give same children ([examples](tests/crossovers_examples.py)): 
@@ -1119,52 +1140,50 @@
 
 ```python
 import numpy as np
 import matplotlib.pyplot as plt
 
 from DiscreteHillClimbing import Hill_Climbing_descent
 
-from geneticalgorithm2 import geneticalgorithm2 as ga
-from geneticalgorithm2 import Population_initializer
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
+from geneticalgorithm2 import get_population_initializer
 
 
 def f(arr):
-    arr2 = arr/25
-    return -np.sum(arr2*np.sin(np.sqrt(np.abs(arr2))))**5 + np.sum(np.abs(arr2))**2
+    arr2 = arr / 25
+    return -np.sum(arr2 * np.sin(np.sqrt(np.abs(arr2)))) ** 5 + np.sum(np.abs(arr2)) ** 2
 
-iterations = 100    
-    
-varbound = [[-100, 100]]*15
 
-available_values = [np.arange(-100, 101)]*15
+iterations = 100
 
+varbound = [[-100, 100]] * 15
 
-my_local_optimizer = lambda arr, score: Hill_Climbing_descent(function = f, available_predictors_values=available_values, max_function_evals=50, start_solution=arr )
+available_values = [np.arange(-100, 101)] * 15
 
+my_local_optimizer = lambda arr, score: Hill_Climbing_descent(function=f, available_predictors_values=available_values,
+                                                              max_function_evals=50, start_solution=arr)
 
-model = ga(function=f, dimension=varbound.shape[0], 
-           variable_type='int', 
-           variable_boundaries = varbound,
+model = ga(function=f, dimension=varbound.shape[0],
+           variable_type='int',
+           variable_boundaries=varbound,
            algorithm_parameters={
                'max_num_iteration': iterations,
                'population_size': 400
-               })
-
+           })
 
 for time in ('before_select', 'after_select', 'never'):
-    model.run(no_plot = True,
-                  population_initializer = Population_initializer(
-                      select_best_of = 3,
-                      local_optimization_step = time,
-                      local_optimizer = my_local_optimizer
-                      )
-                  )
-
-    plt.plot(model.report, label = f"local optimization time = '{time}'")
+    model.run(no_plot=True,
+              population_initializer=get_population_initializer(
+                  select_best_of=3,
+                  local_optimization_step=time,
+                  local_optimizer=my_local_optimizer
+              )
+              )
 
+    plt.plot(model.report, label=f"local optimization time = '{time}'")
 
 plt.xlabel('Generation')
 plt.ylabel('Minimized function (40 simulations average)')
 plt.title('Selection best N object before running GA')
 plt.legend()
 ```
 
@@ -1215,47 +1234,49 @@
 Basically the model checks best population score (minimal score of generation) each generation and saves it to `report` field. Actually this sequence of numbers u see in big part of plots. This behavior is needed for several parts and u cannot disable it. But if u want to report some other metric without using [callbacks](#middle-callbacks), there is highly simple and fast way.
 
 After creating `model` but before running `run()` u need to append ur logic to `model.checked_reports` field. Take a look at example:
 
 ```python
 import numpy as np
 
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
 from geneticalgorithm2 import plot_several_lines
 
+
 def f(X):
-    return 50*np.sum(X) - np.sum(np.sqrt(X) * np.sin(X))
+    return 50 * np.sum(X) - np.sum(np.sqrt(X) * np.sin(X))
+
 
 dim = 25
-varbound = [[0 ,10]]*dim
+varbound = [[0, 10]] * dim
 
 model = ga(function=f, dimension=dim,
            variable_type='real', variable_boundaries=varbound,
            algorithm_parameters={
                'max_num_iteration': 600
            }
-)
+           )
 
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
-model.run(no_plot = False)
+model.run(no_plot=False)
 
 # now u have not only model.report but model.report_25 and so on
 
-#plot reports
+# plot reports
 names = [name for name, _ in model.checked_reports[::-1]]
 plot_several_lines(
     lines=[getattr(model, name) for name in names],
     colors=('green', 'black', 'red', 'blue'),
     labels=['median value', '25% quantile', 'mean of population', 'best pop score'],
     linewidths=(1, 1.5, 1, 2),
     title="Several custom reports with base reports",
@@ -1303,15 +1324,15 @@
 It's very simple to create your own `action` and `condition` functions. But there are several popular functions contained in `Actions` and `ActionConditions` classes:
 * `actions`:
   * `Stop()` -- just stop optimization process
   * `ReduceMutationProb(reduce_coef = 0.9)` -- reduce mutation probability
   * `ChangeRandomCrossover(available_crossovers: Sequence[Callable[[np.ndarray, np.ndarray], Tuple[np.ndarray, np.ndarray]]])` -- change another (random) crossover from list of crossovers
   * `ChangeRandomSelection(available_selections: Sequence[Callable[[np.ndarray, int], np.ndarray]])`
   * `ChangeRandomMutation(available_mutations: Sequence[Callable[[float, float, float], float]])`
-  * `RemoveDuplicates(oppositor = None, creator = None, converter = None)`; see [doc](geneticalgorithm2/callbacks.py)
+  * `RemoveDuplicates(oppositor = None, creator = None, converter = None)`; see [doc](geneticalgorithm2/callbacks/middle.py)
   * `CopyBest(by_indexes)` -- copies best population object values (from dimensions in `by_indexes`) to all population
   * `PlotPopulationScores(title_pattern = lambda data: f"Generation {data['current_generation']}", save_as_name_pattern = None)` -- plot population scores; needs 2 functions like `data`->string for title and file name (to save)
 * `conditions`:
   * `ActionConditions.EachGen(generation_step = 10)` -- do action each `generation_step` generations
   * `ActionConditions.Always()` do action each generations, equals to `ActionConditions.EachGen(1)`
   * `ActionConditions.AfterStagnation(stagnation_generations = 50)` -- do action after `stagnation_generations` stagnation generations
   * `ActionConditions.Several(list_of_conditions)` -- do action if all conditions in list are true
@@ -1665,48 +1686,50 @@
 ## How to plot population scores?
 
 There are 2 ways to plot of scores of population:
 * use `plot_pop_scores(scores, title = 'Population scores', save_as = None)` function from `geneticalgorithm2` environment
 * use `plot_generation_scores(self, title = 'Last generation scores', save_as = None)` method of `ga` object for plotting scores of last generation (yes, it's wrapper of previous function)
 
 Let's check example:
+
 ```python
 import numpy as np
 
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
+
+from geneticalgorithm2 import plot_pop_scores  # for plotting scores without ga object
 
-from geneticalgorithm2 import plot_pop_scores # for plotting scores without ga object
 
 def f(X):
-    return 50*np.sum(X) - np.sum(np.sqrt(X)*np.sin(X))
-    
+    return 50 * np.sum(X) - np.sum(np.sqrt(X) * np.sin(X))
+
+
 dim = 25
-varbound = [[0,10]]*dim
+varbound = [[0, 10]] * dim
 
 # create start population
 start_pop = np.random.uniform(0, 10, (50, dim))
 # eval scores of start population
 start_scores = np.array([f(start_pop[i]) for i in range(start_pop.shape[0])])
 
 # plot start scores using plot_pop_scores function
-plot_pop_scores(start_scores, title = 'Population scores before beginning of searching', save_as= 'plot_scores_start.png')
-
+plot_pop_scores(start_scores, title='Population scores before beginning of searching', save_as='plot_scores_start.png')
 
 model = ga(function=f, dimension=dim, variable_type='real', variable_boundaries=varbound)
 # run optimization process
-model.run(no_plot = True,
+model.run(no_plot=True,
           start_generation={
               'variables': start_pop,
               'scores': start_scores
-              })
+          })
 # plot and save optimization process plot
-model.plot_results(save_as = 'plot_scores_process.png')
+model.plot_results(save_as='plot_scores_process.png')
 
 # plot scores of last population
-model.plot_generation_scores(title = 'Population scores after ending of searching', save_as= 'plot_scores_end.png')
+model.plot_generation_scores(title='Population scores after ending of searching', save_as='plot_scores_end.png')
 ```
 ![](tests/output/plot_scores_start.png)
 ![](tests/output/plot_scores_process.png)
 ![](tests/output/plot_scores_end.png)
 
 
 
@@ -1743,156 +1766,153 @@
 
 By using `set_function` u can determine your own behavior for parallelism or u can use `geneticalgorithm2.set_function_multiprocess(f, n_jobs = -1)` for using just parallelism (recommended for heavy functions and big populations, not recommended for fast functions and small populations).
 
 For example:
 
 ```python
 import numpy as np
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
+
 
 def f(X):
     import math
     a = X[0]
     b = X[1]
     c = X[2]
     s = 0
     for i in range(10000):
-        s += math.sin(a*i) + math.sin(b*i) + math.cos(c*i)
+        s += math.sin(a * i) + math.sin(b * i) + math.cos(c * i)
 
     return s
- 
+
 
 algorithm_param = {'max_num_iteration': 50,
-                   'population_size':100,
-                   'mutation_probability':0.1,
+                   'population_size': 100,
+                   'mutation_probability': 0.1,
                    'elit_ratio': 0.01,
                    'parents_portion': 0.3,
-                   'crossover_type':'uniform',
+                   'crossover_type': 'uniform',
                    'mutation_type': 'uniform_by_center',
                    'selection_type': 'roulette',
-                   'max_iteration_without_improv':None}   
-    
-varbound = np.array([[-10,10]]*3)
+                   'max_iteration_without_improv': None}
 
-model = ga(function=f, dimension=3, 
-    variable_type='real',           
-    variable_boundaries=varbound, 
-    algorithm_parameters = algorithm_param)
+varbound = np.array([[-10, 10]] * 3)
+
+model = ga(function=f, dimension=3,
+           variable_type='real',
+           variable_boundaries=varbound,
+           algorithm_parameters=algorithm_param)
 
 ########
 
-%time model.run()
+%time
+model.run()
 # Wall time: 1min 52s
 
-%time model.run(set_function= ga.set_function_multiprocess(f, n_jobs = 6))
+%time
+model.run(set_function=ga.set_function_multiprocess(f, n_jobs=6))
 # Wall time: 31.7 s
 ```
 
 ## How to initialize start population? How to continue optimization with new run?
 
 For this there is `start_generation` parameter in `run()` method. It's the dictionary with structure like returned `model.output_dict['last_generation']`. Let's see example how can u to use it:
 
 ```python
 import numpy as np
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
+
 
 def f(X):
     return np.sum(X)
-    
+
+
 dim = 6
-    
-varbound = [(0,10)]*dim
 
+varbound = [(0, 10)] * dim
 
 algorithm_param = {'max_num_iteration': 500,
-                   'population_size':100,
-                   'mutation_probability':0.1,
+                   'population_size': 100,
+                   'mutation_probability': 0.1,
                    'elit_ratio': 0.01,
                    'parents_portion': 0.3,
-                   'crossover_type':'uniform',
-                   'max_iteration_without_improv':None}
+                   'crossover_type': 'uniform',
+                   'max_iteration_without_improv': None}
 
-model = ga(function=f, 
-           dimension=dim, 
-           variable_type='real', 
+model = ga(function=f,
+           dimension=dim,
+           variable_type='real',
            variable_boundaries=varbound,
-           algorithm_parameters = algorithm_param)
+           algorithm_parameters=algorithm_param)
 
 # start generation
 # as u see u can use any values been valid for ur function
-samples = np.random.uniform(0, 50, (300, dim)) # 300 is the new size of your generation
-
-
+samples = np.random.uniform(0, 50, (300, dim))  # 300 is the new size of your generation
 
-model.run(no_plot = False, start_generation={'variables':samples, 'scores': None}) 
+model.run(no_plot=False, start_generation={'variables': samples, 'scores': None})
 # it's not necessary to evaluate scores before
 # but u can do it if u have evaluated scores and don't wanna repeat calculations
 
 
-
 # from version 6.3.0 it's recommended to use this form
 from geneticalgorithm2 import Generation
-model.run(no_plot = False, start_generation=Generation(variables = samples, scores = None))
 
+model.run(no_plot=False, start_generation=Generation(variables=samples, scores=None))
 
 # from version 6.4.0 u also can use these forms
-model.run(no_plot = False, start_generation= samples)
-model.run(no_plot = False, start_generation= (samples, None))
-
+model.run(no_plot=False, start_generation=samples)
+model.run(no_plot=False, start_generation=(samples, None))
 
 # if u have scores array, u can put it too
 scores = np.array([f(sample) for sample in samples])
-model.run(no_plot = False, start_generation= (samples, scores))
-
+model.run(no_plot=False, start_generation=(samples, scores))
 
 ##
 ## after first run
 ## best value = 0.10426190111045064
 ##
 
 # okay, let's continue optimization using saved last generation
-model.run(no_plot = True, start_generation=model.output_dict['last_generation']) 
+model.run(no_plot=True, start_generation=model.output_dict['last_generation'])
 
 ##
 ## after second run
 ## best value = 0.06128462776296528
 ##
 
 ```
 
 Also u can save and load populations using likely code:
 
 ```python
 import numpy as np
 
-from geneticalgorithm2 import geneticalgorithm2 as ga
+from geneticalgorithm2 import GeneticAlgorithm2 as ga
 
 from OptimizationTestFunctions import Eggholder
 
+dim = 2 * 15
 
-dim = 2*15
-
-f =  Eggholder(dim)
+f = Eggholder(dim)
 
 xmin, xmax, ymin, ymax = f.bounds
-        
-varbound = np.array([[xmin, xmax], [ymin, ymax]]*15)
-    
+
+varbound = np.array([[xmin, xmax], [ymin, ymax]] * 15)
+
 model = ga(function=f,
-               dimension = dim,
-               variable_type='real',
-               variable_boundaries=varbound,
-               algorithm_parameters = {
-                       'max_num_iteration': 300,
-                       'population_size': 100
-                       })
+           dimension=dim,
+           variable_type='real',
+           variable_boundaries=varbound,
+           algorithm_parameters={
+               'max_num_iteration': 300,
+               'population_size': 100
+           })
 
 # first run and save last generation to file
 filename = "eggholder_lastgen.npz"
-model.run(save_last_generation_as = filename)
-
+model.run(save_last_generation_as=filename)
 
 # load start generation from file and run again (continue optimization)
 model.run(start_generation=filename)
 ```
```

### Comparing `geneticalgorithm2-6.8.7/setup.py` & `geneticalgorithm2-6.9.0/setup.py`

 * *Files identical despite different names*

