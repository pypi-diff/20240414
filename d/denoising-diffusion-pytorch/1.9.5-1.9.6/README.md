# Comparing `tmp/denoising-diffusion-pytorch-1.9.5.tar.gz` & `tmp/denoising-diffusion-pytorch-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denoising-diffusion-pytorch-1.9.5.tar", last modified: Mon Jan  1 13:56:46 2024, max compression
+gzip compressed data, was "denoising-diffusion-pytorch-1.9.6.tar", last modified: Mon Jan 22 15:11:57 2024, max compression
```

## Comparing `denoising-diffusion-pytorch-1.9.5.tar` & `denoising-diffusion-pytorch-1.9.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 13:56:46.756956 denoising-diffusion-pytorch-1.9.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-01-01 13:56:38.000000 denoising-diffusion-pytorch-1.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-01-01 13:56:46.756956 denoising-diffusion-pytorch-1.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11068 2024-01-01 13:56:38.000000 denoising-diffusion-pytorch-1.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 13:56:46.756956 denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-01-01 13:56:38.000000 denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-01-01 13:56:38.000000 denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (127)    28142 2024-01-01 13:56:38.000000 denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/classifier_free_guidance.py
--rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-01-01 13:56:38.000000 denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    38320 2024-01-01 13:56:38.000000 denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)    30229 2024-01-01 13:56:38.000000 denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-01-01 13:56:38.000000 denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/elucidated_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-01-01 13:56:38.000000 denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/fid_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    35848 2024-01-01 13:56:38.000000 denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/guided_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-01-01 13:56:38.000000 denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    21236 2024-01-01 13:56:38.000000 denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/simple_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-01-01 13:56:38.000000 denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-01 13:56:38.000000 denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-01-01 13:56:38.000000 denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-01 13:56:46.756956 denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-01-01 13:56:46.000000 denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-01-01 13:56:46.000000 denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-01 13:56:46.000000 denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-01 13:56:46.000000 denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-01 13:56:46.000000 denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-01 13:56:46.756956 denoising-diffusion-pytorch-1.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-01-01 13:56:38.000000 denoising-diffusion-pytorch-1.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:11:57.731436 denoising-diffusion-pytorch-1.9.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-01-22 15:11:57.731436 denoising-diffusion-pytorch-1.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11068 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:11:57.727436 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28142 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/classifier_free_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38313 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30229 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9203 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/elucidated_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/fid_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35848 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/guided_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5714 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/learned_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21236 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/simple_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5780 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3390 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:11:57.731436 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-01-22 15:11:57.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-01-22 15:11:57.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 15:11:57.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-22 15:11:57.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-22 15:11:57.000000 denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 15:11:57.731436 denoising-diffusion-pytorch-1.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-01-22 15:11:49.000000 denoising-diffusion-pytorch-1.9.6/setup.py
```

### Comparing `denoising-diffusion-pytorch-1.9.5/LICENSE` & `denoising-diffusion-pytorch-1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.9.5/PKG-INFO` & `denoising-diffusion-pytorch-1.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.9.5
+Version: 1.9.6
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.9.5/README.md` & `denoising-diffusion-pytorch-1.9.6/README.md`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/__init__.py` & `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/attend.py` & `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/classifier_free_guidance.py` & `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/classifier_free_guidance.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py` & `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -781,15 +781,15 @@
 
         # if doing self-conditioning, 50% of the time, predict x_start from current set of times
         # and condition with unet with that
         # this technique will slow down training by 25%, but seems to lower FID significantly
 
         x_self_cond = None
         if self.self_condition and random() < 0.5:
-            with torch.inference_mode():
+            with torch.no_grad():
                 x_self_cond = self.model_predictions(x, t).pred_x_start
                 x_self_cond.detach_()
 
         # predict and take gradient step
 
         model_out = self.model(x, t, x_self_cond)
```

### Comparing `denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py` & `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/denoising_diffusion_pytorch_1d.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/elucidated_diffusion.py` & `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/elucidated_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/fid_evaluation.py` & `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/fid_evaluation.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/guided_diffusion.py` & `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/guided_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/learned_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/learned_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/simple_diffusion.py` & `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/simple_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/v_param_continuous_time_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py` & `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch/weighted_objective_gaussian_diffusion.py`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch.egg-info/PKG-INFO` & `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: denoising-diffusion-pytorch
-Version: 1.9.5
+Version: 1.9.6
 Summary: Denoising Diffusion Probabilistic Models - Pytorch
 Home-page: https://github.com/lucidrains/denoising-diffusion-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,generative models
 Classifier: Development Status :: 4 - Beta
```

### Comparing `denoising-diffusion-pytorch-1.9.5/denoising_diffusion_pytorch.egg-info/SOURCES.txt` & `denoising-diffusion-pytorch-1.9.6/denoising_diffusion_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `denoising-diffusion-pytorch-1.9.5/setup.py` & `denoising-diffusion-pytorch-1.9.6/setup.py`

 * *Files identical despite different names*

