# Comparing `tmp/torchao-nightly-2024.4.8.tar.gz` & `tmp/torchao-nightly-2024.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchao-nightly-2024.4.8.tar", last modified: Mon Apr  8 00:19:23 2024, max compression
+gzip compressed data, was "torchao-nightly-2024.4.9.tar", last modified: Tue Apr  9 00:19:16 2024, max compression
```

## Comparing `torchao-nightly-2024.4.8.tar` & `torchao-nightly-2024.4.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:19:23.257930 torchao-nightly-2024.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-08 00:19:23.257930 torchao-nightly-2024.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6038 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 00:19:23.257930 torchao-nightly-2024.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:19:23.249930 torchao-nightly-2024.4.8/torchao/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/torchao/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:19:23.249930 torchao-nightly-2024.4.8/torchao/dtypes/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/torchao/dtypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/torchao/dtypes/nf4tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/torchao/dtypes/uint4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:19:23.253930 torchao-nightly-2024.4.8/torchao/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/torchao/kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/torchao/kernel/autotuner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/torchao/kernel/intmm.py
--rw-r--r--   0 runner    (1001) docker     (127)    11678 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/torchao/kernel/intmm_triton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:19:23.253930 torchao-nightly-2024.4.8/torchao/quantization/
--rw-r--r--   0 runner    (1001) docker     (127)    52411 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/torchao/quantization/GPTQ.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/torchao/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16941 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/torchao/quantization/autoquant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/torchao/quantization/dynamic_quant.py
--rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/torchao/quantization/quant_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    18695 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/torchao/quantization/quant_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/torchao/quantization/smoothquant.py
--rw-r--r--   0 runner    (1001) docker     (127)    17584 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/torchao/quantization/subclass.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/torchao/quantization/unified.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/torchao/quantization/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/torchao/quantization/weight_only.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:19:23.253930 torchao-nightly-2024.4.8/torchao/sparsity/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/torchao/sparsity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/torchao/sparsity/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-08 00:19:15.000000 torchao-nightly-2024.4.8/torchao/sparsity/wanda.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 00:19:23.257930 torchao-nightly-2024.4.8/torchao_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-08 00:19:23.000000 torchao-nightly-2024.4.8/torchao_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-08 00:19:23.000000 torchao-nightly-2024.4.8/torchao_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 00:19:23.000000 torchao-nightly-2024.4.8/torchao_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-08 00:19:23.000000 torchao-nightly-2024.4.8/torchao_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-08 00:19:23.000000 torchao-nightly-2024.4.8/torchao_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:19:16.070146 torchao-nightly-2024.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-09 00:19:16.070146 torchao-nightly-2024.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6038 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 00:19:16.070146 torchao-nightly-2024.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:19:16.062146 torchao-nightly-2024.4.9/torchao/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/torchao/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:19:16.066146 torchao-nightly-2024.4.9/torchao/dtypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/torchao/dtypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/torchao/dtypes/nf4tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12448 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/torchao/dtypes/uint4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:19:16.066146 torchao-nightly-2024.4.9/torchao/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/torchao/kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/torchao/kernel/autotuner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/torchao/kernel/intmm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11678 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/torchao/kernel/intmm_triton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:19:16.066146 torchao-nightly-2024.4.9/torchao/quantization/
+-rw-r--r--   0 runner    (1001) docker     (127)    52411 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/torchao/quantization/GPTQ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/torchao/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16941 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/torchao/quantization/autoquant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/torchao/quantization/dynamic_quant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/torchao/quantization/quant_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18695 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/torchao/quantization/quant_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9159 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/torchao/quantization/smoothquant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17584 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/torchao/quantization/subclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/torchao/quantization/unified.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/torchao/quantization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/torchao/quantization/weight_only.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:19:16.066146 torchao-nightly-2024.4.9/torchao/sparsity/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/torchao/sparsity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/torchao/sparsity/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-04-09 00:19:05.000000 torchao-nightly-2024.4.9/torchao/sparsity/wanda.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 00:19:16.070146 torchao-nightly-2024.4.9/torchao_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-04-09 00:19:16.000000 torchao-nightly-2024.4.9/torchao_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-09 00:19:16.000000 torchao-nightly-2024.4.9/torchao_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 00:19:16.000000 torchao-nightly-2024.4.9/torchao_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-09 00:19:16.000000 torchao-nightly-2024.4.9/torchao_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-09 00:19:16.000000 torchao-nightly-2024.4.9/torchao_nightly.egg-info/top_level.txt
```

### Comparing `torchao-nightly-2024.4.8/LICENSE` & `torchao-nightly-2024.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.8/PKG-INFO` & `torchao-nightly-2024.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchao-nightly
-Version: 2024.4.8
+Version: 2024.4.9
 Summary: Package for applying ao techniques to GPU models
 Home-page: https://github.com/pytorch-labs/ao
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: sentencepiece
```

### Comparing `torchao-nightly-2024.4.8/README.md` & `torchao-nightly-2024.4.9/README.md`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.8/setup.py` & `torchao-nightly-2024.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.8/torchao/dtypes/nf4tensor.py` & `torchao-nightly-2024.4.9/torchao/dtypes/nf4tensor.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.8/torchao/dtypes/uint4.py` & `torchao-nightly-2024.4.9/torchao/dtypes/uint4.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.8/torchao/kernel/autotuner.py` & `torchao-nightly-2024.4.9/torchao/kernel/autotuner.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.8/torchao/kernel/intmm.py` & `torchao-nightly-2024.4.9/torchao/kernel/intmm.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.8/torchao/kernel/intmm_triton.py` & `torchao-nightly-2024.4.9/torchao/kernel/intmm_triton.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.8/torchao/quantization/GPTQ.py` & `torchao-nightly-2024.4.9/torchao/quantization/GPTQ.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.8/torchao/quantization/__init__.py` & `torchao-nightly-2024.4.9/torchao/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.8/torchao/quantization/autoquant.py` & `torchao-nightly-2024.4.9/torchao/quantization/autoquant.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.8/torchao/quantization/dynamic_quant.py` & `torchao-nightly-2024.4.9/torchao/quantization/dynamic_quant.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.8/torchao/quantization/quant_api.py` & `torchao-nightly-2024.4.9/torchao/quantization/quant_api.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.8/torchao/quantization/quant_primitives.py` & `torchao-nightly-2024.4.9/torchao/quantization/quant_primitives.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.8/torchao/quantization/smoothquant.py` & `torchao-nightly-2024.4.9/torchao/quantization/smoothquant.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.8/torchao/quantization/subclass.py` & `torchao-nightly-2024.4.9/torchao/quantization/subclass.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.8/torchao/quantization/unified.py` & `torchao-nightly-2024.4.9/torchao/quantization/unified.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.8/torchao/quantization/utils.py` & `torchao-nightly-2024.4.9/torchao/quantization/utils.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.8/torchao/quantization/weight_only.py` & `torchao-nightly-2024.4.9/torchao/quantization/weight_only.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.8/torchao/sparsity/utils.py` & `torchao-nightly-2024.4.9/torchao/sparsity/utils.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.8/torchao/sparsity/wanda.py` & `torchao-nightly-2024.4.9/torchao/sparsity/wanda.py`

 * *Files identical despite different names*

### Comparing `torchao-nightly-2024.4.8/torchao_nightly.egg-info/PKG-INFO` & `torchao-nightly-2024.4.9/torchao_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchao-nightly
-Version: 2024.4.8
+Version: 2024.4.9
 Summary: Package for applying ao techniques to GPU models
 Home-page: https://github.com/pytorch-labs/ao
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch
 Requires-Dist: numpy
 Requires-Dist: sentencepiece
```

### Comparing `torchao-nightly-2024.4.8/torchao_nightly.egg-info/SOURCES.txt` & `torchao-nightly-2024.4.9/torchao_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

