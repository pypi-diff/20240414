# Comparing `tmp/bellek-0.77.0.tar.gz` & `tmp/bellek-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bellek-0.77.0.tar", last modified: Sun Apr 14 11:31:29 2024, max compression
+gzip compressed data, was "bellek-0.9.0.tar", last modified: Sat Oct  7 10:06:49 2023, max compression
```

## Comparing `bellek-0.77.0.tar` & `bellek-0.9.0.tar`

### file list

```diff
@@ -1,83 +1,35 @@
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:29.667258 bellek-0.77.0/
--rw-rw-r--   0 bdsaglam   (501) staff       (20)    11337 2022-09-05 16:31:43.000000 bellek-0.77.0/LICENSE
--rw-rw-r--   0 bdsaglam   (501) staff       (20)      111 2022-09-05 16:31:43.000000 bellek-0.77.0/MANIFEST.in
--rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-14 11:31:29.666658 bellek-0.77.0/PKG-INFO
--rw-r--r--   0 bdsaglam   (501) staff       (20)      184 2023-04-09 15:45:53.000000 bellek-0.77.0/README.md
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:29.590425 bellek-0.77.0/bellek/
--rw-r--r--   0 bdsaglam   (501) staff       (20)       23 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    52886 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/_modidx.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:29.602325 bellek-0.77.0/bellek/hf/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/hf/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:29.607655 bellek-0.77.0/bellek/hf/transformers/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/hf/transformers/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    10813 2024-04-14 11:31:24.000000 bellek-0.77.0/bellek/hf/transformers/experiment.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2305 2024-04-14 11:31:24.000000 bellek-0.77.0/bellek/hf/transformers/llama.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2934 2024-04-14 11:31:24.000000 bellek-0.77.0/bellek/hf/transformers/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:29.634181 bellek-0.77.0/bellek/jerx/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/jerx/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1312 2024-04-14 11:31:24.000000 bellek-0.77.0/bellek/jerx/dataset.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3386 2024-04-14 11:31:24.000000 bellek-0.77.0/bellek/jerx/eval.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2582 2024-04-14 11:31:24.000000 bellek-0.77.0/bellek/jerx/prompt.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:29.636069 bellek-0.77.0/bellek/jerx/reward/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/jerx/reward/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2550 2024-04-14 11:31:24.000000 bellek-0.77.0/bellek/jerx/reward/gpt.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      901 2024-04-14 11:31:24.000000 bellek-0.77.0/bellek/jerx/utils.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:29.638605 bellek-0.77.0/bellek/lang/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/lang/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1551 2024-04-14 11:31:24.000000 bellek-0.77.0/bellek/lang/dataset.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2160 2024-04-14 11:31:24.000000 bellek-0.77.0/bellek/lang/qdecomp.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:29.642080 bellek-0.77.0/bellek/langchain/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/langchain/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      915 2024-04-14 11:31:24.000000 bellek-0.77.0/bellek/langchain/cache.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1271 2024-04-14 11:31:24.000000 bellek-0.77.0/bellek/langchain/obs.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:29.645180 bellek-0.77.0/bellek/llama_index/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/llama_index/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:29.646546 bellek-0.77.0/bellek/llama_index/data_structs/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/llama_index/data_structs/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2483 2024-04-14 11:31:24.000000 bellek-0.77.0/bellek/llama_index/data_structs/data_structs.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:29.648072 bellek-0.77.0/bellek/llama_index/graph_stores/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/llama_index/graph_stores/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     9059 2024-04-14 11:31:24.000000 bellek-0.77.0/bellek/llama_index/graph_stores/kuzu.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:29.649099 bellek-0.77.0/bellek/llama_index/indices/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/llama_index/indices/__init__.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:29.650925 bellek-0.77.0/bellek/llama_index/indices/knowledge_graph/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    13058 2024-04-14 11:31:24.000000 bellek-0.77.0/bellek/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    14785 2024-04-14 11:31:24.000000 bellek-0.77.0/bellek/llama_index/indices/knowledge_graph/retrievers.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      855 2024-04-14 11:31:24.000000 bellek-0.77.0/bellek/llama_index/llms.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1420 2024-04-14 11:31:24.000000 bellek-0.77.0/bellek/llama_index/obs.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      779 2024-04-14 11:31:24.000000 bellek-0.77.0/bellek/logging.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:29.660873 bellek-0.77.0/bellek/ml/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/ml/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     2225 2024-04-14 11:31:24.000000 bellek-0.77.0/bellek/ml/clip.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     8515 2024-04-14 11:31:24.000000 bellek-0.77.0/bellek/ml/coop.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)    28983 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/ml/data.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3293 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/ml/evaluation.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3231 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/ml/experiment.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:29.662772 bellek-0.77.0/bellek/ml/lang/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/ml/lang/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1563 2024-03-17 17:22:59.000000 bellek-0.77.0/bellek/ml/lang/dataset.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      711 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/ml/layer.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1718 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/ml/loss.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     9174 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/ml/mcd.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      939 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/ml/vision.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:29.664045 bellek-0.77.0/bellek/musique/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/musique/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     3081 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/musique/eval.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      539 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/testing.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:29.665696 bellek-0.77.0/bellek/text/
--rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/text/__init__.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      399 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/text/utils.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)     4864 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/utils.py
--rw-r--r--   0 bdsaglam   (501) staff       (20)      823 2024-04-14 11:31:25.000000 bellek-0.77.0/bellek/wandb.py
-drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2024-04-14 11:31:29.601561 bellek-0.77.0/bellek.egg-info/
--rw-r--r--   0 bdsaglam   (501) staff       (20)      775 2024-04-14 11:31:29.000000 bellek-0.77.0/bellek.egg-info/PKG-INFO
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1649 2024-04-14 11:31:29.000000 bellek-0.77.0/bellek.egg-info/SOURCES.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2024-04-14 11:31:29.000000 bellek-0.77.0/bellek.egg-info/dependency_links.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)       34 2024-04-14 11:31:29.000000 bellek-0.77.0/bellek.egg-info/entry_points.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2023-01-13 22:27:25.000000 bellek-0.77.0/bellek.egg-info/not-zip-safe
--rw-r--r--   0 bdsaglam   (501) staff       (20)      394 2024-04-14 11:31:29.000000 bellek-0.77.0/bellek.egg-info/requires.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)        7 2024-04-14 11:31:29.000000 bellek-0.77.0/bellek.egg-info/top_level.txt
--rw-r--r--   0 bdsaglam   (501) staff       (20)     1356 2024-04-14 11:31:01.000000 bellek-0.77.0/settings.ini
--rw-r--r--   0 bdsaglam   (501) staff       (20)       38 2024-04-14 11:31:29.667475 bellek-0.77.0/setup.cfg
--rw-rw-r--   0 bdsaglam   (501) staff       (20)     2541 2022-09-05 16:31:43.000000 bellek-0.77.0/setup.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2023-10-07 10:06:49.350399 bellek-0.9.0/
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)    11337 2022-09-05 16:31:43.000000 bellek-0.9.0/LICENSE
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)      111 2022-09-05 16:31:43.000000 bellek-0.9.0/MANIFEST.in
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      943 2023-10-07 10:06:49.349794 bellek-0.9.0/PKG-INFO
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      184 2023-04-09 15:45:53.000000 bellek-0.9.0/README.md
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2023-10-07 10:06:49.334875 bellek-0.9.0/bellek/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       22 2023-10-01 18:46:33.000000 bellek-0.9.0/bellek/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    17651 2023-10-01 18:46:33.000000 bellek-0.9.0/bellek/_modidx.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2023-10-07 10:06:49.347595 bellek-0.9.0/bellek/ml/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2023-10-01 18:46:33.000000 bellek-0.9.0/bellek/ml/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2225 2023-10-01 18:46:33.000000 bellek-0.9.0/bellek/ml/clip.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     8515 2023-10-01 18:46:33.000000 bellek-0.9.0/bellek/ml/coop.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)    28983 2023-10-01 18:46:33.000000 bellek-0.9.0/bellek/ml/data.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     3293 2023-10-01 18:46:33.000000 bellek-0.9.0/bellek/ml/evaluation.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2108 2023-10-01 18:46:33.000000 bellek-0.9.0/bellek/ml/experiment.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2023-10-07 10:06:49.348941 bellek-0.9.0/bellek/ml/kg/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        0 2023-10-01 18:46:33.000000 bellek-0.9.0/bellek/ml/kg/__init__.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1708 2023-10-01 18:46:33.000000 bellek-0.9.0/bellek/ml/kg/cons.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      711 2023-10-01 18:46:33.000000 bellek-0.9.0/bellek/ml/layer.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1718 2023-10-01 18:46:33.000000 bellek-0.9.0/bellek/ml/loss.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     9174 2023-10-01 18:46:33.000000 bellek-0.9.0/bellek/ml/mcd.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      939 2023-10-01 18:46:33.000000 bellek-0.9.0/bellek/ml/vision.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      539 2023-10-01 18:46:33.000000 bellek-0.9.0/bellek/testing.py
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     2838 2023-10-01 18:46:33.000000 bellek-0.9.0/bellek/utils.py
+drwxr-xr-x   0 bdsaglam   (501) staff       (20)        0 2023-10-07 10:06:49.340286 bellek-0.9.0/bellek.egg-info/
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      943 2023-10-07 10:06:49.000000 bellek-0.9.0/bellek.egg-info/PKG-INFO
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      577 2023-10-07 10:06:49.000000 bellek-0.9.0/bellek.egg-info/SOURCES.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2023-10-07 10:06:49.000000 bellek-0.9.0/bellek.egg-info/dependency_links.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       55 2023-10-07 10:06:49.000000 bellek-0.9.0/bellek.egg-info/entry_points.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        1 2023-01-13 22:27:25.000000 bellek-0.9.0/bellek.egg-info/not-zip-safe
+-rw-r--r--   0 bdsaglam   (501) staff       (20)      174 2023-10-07 10:06:49.000000 bellek-0.9.0/bellek.egg-info/requires.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)        7 2023-10-07 10:06:49.000000 bellek-0.9.0/bellek.egg-info/top_level.txt
+-rw-r--r--   0 bdsaglam   (501) staff       (20)     1096 2023-10-01 18:46:27.000000 bellek-0.9.0/settings.ini
+-rw-r--r--   0 bdsaglam   (501) staff       (20)       38 2023-10-07 10:06:49.350606 bellek-0.9.0/setup.cfg
+-rw-rw-r--   0 bdsaglam   (501) staff       (20)     2541 2022-09-05 16:31:43.000000 bellek-0.9.0/setup.py
```

### Comparing `bellek-0.77.0/LICENSE` & `bellek-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bellek-0.77.0/bellek/ml/clip.py` & `bellek-0.9.0/bellek/ml/clip.py`

 * *Files identical despite different names*

### Comparing `bellek-0.77.0/bellek/ml/coop.py` & `bellek-0.9.0/bellek/ml/coop.py`

 * *Files identical despite different names*

### Comparing `bellek-0.77.0/bellek/ml/data.py` & `bellek-0.9.0/bellek/ml/data.py`

 * *Files identical despite different names*

### Comparing `bellek-0.77.0/bellek/ml/evaluation.py` & `bellek-0.9.0/bellek/ml/evaluation.py`

 * *Files identical despite different names*

### Comparing `bellek-0.77.0/bellek/ml/experiment.py` & `bellek-0.9.0/bellek/ml/experiment.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,84 +1,49 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/ml.experiment.ipynb.
 
 # %% auto 0
-__all__ = ['make_experiment_dir', 'before_experiment', 'after_experiment', 'make_run_experiment_sweep', 'main']
+__all__ = ['make_experiment_dir', 'prepare_config', 'make_run_experiment_sweep', 'main']
 
 # %% ../../nbs/ml.experiment.ipynb 3
-import os
 from pathlib import Path
+import torch
 import wandb
 import json
-from ..utils import NestedDict, flatten_dict
+from ..utils import context_chdir, NestedDict, flatten_dict
 
 # %% ../../nbs/ml.experiment.ipynb 4
 def make_experiment_dir(root=".experiments", name=None):
     if name is None:
         from bellek.utils import generate_time_id
         name = generate_time_id()
     experiment_dir = Path(root) / name
     experiment_dir.mkdir(parents=True, exist_ok=True)
     return experiment_dir
 
 # %% ../../nbs/ml.experiment.ipynb 5
-def before_experiment(wandb_run):
-    config = NestedDict.from_flat_dict(wandb_run.config)
-
-    # W&B variables
-    config.set("wandb.run_id", wandb_run.id)
-    os.environ["WANDB_PROJECT"] = wandb_run.project
-    os.environ["WANDB_LOG_MODEL"] = "end"
-
-    # Set random seed
-    if seed := config.get("seed"):
-        from fastai.torch_core import set_seed
-
-        set_seed(seed)
-
-    pp_config = config.at("metaconfig.preprocessing")
-    
-    # Resolve paths
-    if pp_config.get("resolve_paths"):
-        exclude_resolving_paths = pp_config.get("exclude_resolving_paths", [])
-        for k, v in config.flat().items():
-            if isinstance(k, str) and k.endswith("path") and k not in exclude_resolving_paths:
-                config.set(k, str(Path(v).resolve()))
-
-    # Resolve device
-    if "device" not in config and pp_config.get("resolve_device"):
-        import torch
-
+def prepare_config(config):
+    if "device" not in config:
         config["device"] = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-
-    # Update W&B config
-    wandb_run.config.update(flatten_dict(config), allow_val_change=True)
-
-    # Save preprocessed config
-    with open("./config.before.json", "w") as f:
-        json.dump(config, f, indent=2)
-
-
-def after_experiment(wandb_run):
-    config = NestedDict.from_flat_dict(wandb_run.config)
-    with open("./config.after.json", "w") as f:
-        json.dump(config, f, indent=2)
+    
+    for k, v in config.flat().items():
+        if isinstance(k, str) and k.endswith("path"):
+            config.set(k, str(Path(v).resolve()))
+    return config
 
 # %% ../../nbs/ml.experiment.ipynb 6
 def make_run_experiment_sweep(run_experiment, config_defaults):
     def func():
         wandb_params = config_defaults["wandb"]
         with wandb.init(config=flatten_dict(config_defaults), **wandb_params) as wandb_run:
-            before_experiment(wandb_run)
             run_experiment(wandb_run)
-            after_experiment(wandb_run)
     return func
 
 def main(run_experiment, args):
     with open(args.cfg) as f:
-        config = NestedDict(json.load(f))
+        config = prepare_config(NestedDict(json.load(f)))
 
     is_sweep = hasattr(args, "sweep_cfg") and args.sweep_cfg
     if is_sweep:
         with open(args.sweep_cfg) as f:
             sweep_config = json.load(f)
     else:
         sweep_config = {}
```

### Comparing `bellek-0.77.0/bellek/ml/layer.py` & `bellek-0.9.0/bellek/ml/layer.py`

 * *Files identical despite different names*

### Comparing `bellek-0.77.0/bellek/ml/loss.py` & `bellek-0.9.0/bellek/ml/loss.py`

 * *Files identical despite different names*

### Comparing `bellek-0.77.0/bellek/ml/mcd.py` & `bellek-0.9.0/bellek/ml/mcd.py`

 * *Files identical despite different names*

### Comparing `bellek-0.77.0/bellek/ml/vision.py` & `bellek-0.9.0/bellek/ml/vision.py`

 * *Files identical despite different names*

### Comparing `bellek-0.77.0/bellek/testing.py` & `bellek-0.9.0/bellek/testing.py`

 * *Files identical despite different names*

### Comparing `bellek-0.77.0/settings.ini` & `bellek-0.9.0/settings.ini`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [DEFAULT]
 repo = bellek
 lib_name = bellek
-version = 0.77.0
-min_python = 3.10
+version = 0.9.0
+min_python = 3.7
 license = apache2
 doc_path = _docs
 lib_path = bellek
 nbs_path = nbs
 recursive = True
 tst_flags = notest
 put_version_in_init = True
@@ -22,44 +22,33 @@
 copyright = 2022 onwards, Barış Deniz Sağlam
 description = My digital memory
 keywords = notebook
 language = English
 status = 3
 user = bdsaglam
 requirements = 
-    numpy>=1.26.2
-    pandas>=2.1.4
-    datasets>=2.15.0 
-    evaluate>=0.4.1
-    fastcore>=1.5.29
+    numpy 
+    pandas 
     fastai>=2.7.11 
     fastmtl>=1.2.0 
-    langchain~=0.1.7
-    langchain-openai~=0.0.2.post1
-    llama-index~=0.9.22
-    litellm~=1.16.12
-    sentence_transformers>=2.2.2
-    transformers>=4.39.3
-    text-generation~=0.6.1
-    arize-phoenix>=2.1.0
     python-dotenv 
-    wandb 
-    # clip@git+https://github.com/openai/CLIP.git
+    datasets 
+    transformers 
+    openai 
+    langchain 
+    sentence_transformers 
 dev_requirements = 
     nbdev 
     jupyter 
     twine 
     pre-commit 
     isort 
     black 
-    dvc
-    dvc-s3
-    huggingface_hub
-    typer
-    rich
+    wandb 
+    # clip@git+https://github.com/openai/CLIP.git
 black_formatting = False
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
```

### Comparing `bellek-0.77.0/setup.py` & `bellek-0.9.0/setup.py`

 * *Files identical despite different names*

