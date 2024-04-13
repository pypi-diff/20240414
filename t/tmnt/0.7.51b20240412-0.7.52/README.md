# Comparing `tmp/tmnt-0.7.51b20240412.tar.gz` & `tmp/tmnt-0.7.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmnt-0.7.51b20240412.tar", last modified: Fri Apr 12 23:04:56 2024, max compression
+gzip compressed data, was "tmnt-0.7.52.tar", last modified: Sat Apr 13 16:25:56 2024, max compression
```

## Comparing `tmnt-0.7.51b20240412.tar` & `tmnt-0.7.52.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:04:56.302880 tmnt-0.7.51b20240412/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-12 23:04:46.000000 tmnt-0.7.51b20240412/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-12 23:04:46.000000 tmnt-0.7.51b20240412/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-12 23:04:56.302880 tmnt-0.7.51b20240412/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-12 23:04:46.000000 tmnt-0.7.51b20240412/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 23:04:56.302880 tmnt-0.7.51b20240412/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-12 23:04:46.000000 tmnt-0.7.51b20240412/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:04:56.298880 tmnt-0.7.51b20240412/tmnt/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-12 23:04:46.000000 tmnt-0.7.51b20240412/tmnt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-04-12 23:04:46.000000 tmnt-0.7.51b20240412/tmnt/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    18736 2024-04-12 23:04:46.000000 tmnt-0.7.51b20240412/tmnt/data_loading.py
--rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-04-12 23:04:46.000000 tmnt-0.7.51b20240412/tmnt/distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)    77249 2024-04-12 23:04:46.000000 tmnt-0.7.51b20240412/tmnt/estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-12 23:04:46.000000 tmnt-0.7.51b20240412/tmnt/eval_npmi.py
--rw-r--r--   0 runner    (1001) docker     (127)    17845 2024-04-12 23:04:46.000000 tmnt-0.7.51b20240412/tmnt/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)    35049 2024-04-12 23:04:46.000000 tmnt-0.7.51b20240412/tmnt/modeling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:04:56.302880 tmnt-0.7.51b20240412/tmnt/preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-12 23:04:46.000000 tmnt-0.7.51b20240412/tmnt/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14050 2024-04-12 23:04:46.000000 tmnt-0.7.51b20240412/tmnt/preprocess/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-04-12 23:04:46.000000 tmnt-0.7.51b20240412/tmnt/preprocess/vectorizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:04:56.302880 tmnt-0.7.51b20240412/tmnt/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-12 23:04:46.000000 tmnt-0.7.51b20240412/tmnt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-12 23:04:46.000000 tmnt-0.7.51b20240412/tmnt/utils/csv2json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-12 23:04:46.000000 tmnt-0.7.51b20240412/tmnt/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-12 23:04:46.000000 tmnt-0.7.51b20240412/tmnt/utils/mat_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-12 23:04:46.000000 tmnt-0.7.51b20240412/tmnt/utils/ngram_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-12 23:04:46.000000 tmnt-0.7.51b20240412/tmnt/utils/pubmed_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-12 23:04:46.000000 tmnt-0.7.51b20240412/tmnt/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-12 23:04:46.000000 tmnt-0.7.51b20240412/tmnt/utils/recalibrate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 23:04:56.302880 tmnt-0.7.51b20240412/tmnt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-12 23:04:56.000000 tmnt-0.7.51b20240412/tmnt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-12 23:04:56.000000 tmnt-0.7.51b20240412/tmnt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 23:04:56.000000 tmnt-0.7.51b20240412/tmnt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-12 23:04:56.000000 tmnt-0.7.51b20240412/tmnt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-12 23:04:56.000000 tmnt-0.7.51b20240412/tmnt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:25:56.772062 tmnt-0.7.52/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-13 16:25:42.000000 tmnt-0.7.52/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-13 16:25:42.000000 tmnt-0.7.52/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-13 16:25:56.772062 tmnt-0.7.52/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-13 16:25:42.000000 tmnt-0.7.52/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 16:25:56.772062 tmnt-0.7.52/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-13 16:25:42.000000 tmnt-0.7.52/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:25:56.768062 tmnt-0.7.52/tmnt/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-13 16:25:42.000000 tmnt-0.7.52/tmnt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10054 2024-04-13 16:25:42.000000 tmnt-0.7.52/tmnt/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18736 2024-04-13 16:25:42.000000 tmnt-0.7.52/tmnt/data_loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10866 2024-04-13 16:25:42.000000 tmnt-0.7.52/tmnt/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77217 2024-04-13 16:25:42.000000 tmnt-0.7.52/tmnt/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-04-13 16:25:42.000000 tmnt-0.7.52/tmnt/eval_npmi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17845 2024-04-13 16:25:42.000000 tmnt-0.7.52/tmnt/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34549 2024-04-13 16:25:42.000000 tmnt-0.7.52/tmnt/modeling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:25:56.768062 tmnt-0.7.52/tmnt/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-13 16:25:42.000000 tmnt-0.7.52/tmnt/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14050 2024-04-13 16:25:42.000000 tmnt-0.7.52/tmnt/preprocess/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15796 2024-04-13 16:25:42.000000 tmnt-0.7.52/tmnt/preprocess/vectorizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:25:56.768062 tmnt-0.7.52/tmnt/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-13 16:25:42.000000 tmnt-0.7.52/tmnt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-13 16:25:42.000000 tmnt-0.7.52/tmnt/utils/csv2json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-13 16:25:42.000000 tmnt-0.7.52/tmnt/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-13 16:25:42.000000 tmnt-0.7.52/tmnt/utils/mat_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-13 16:25:42.000000 tmnt-0.7.52/tmnt/utils/ngram_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-13 16:25:42.000000 tmnt-0.7.52/tmnt/utils/pubmed_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-13 16:25:42.000000 tmnt-0.7.52/tmnt/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-13 16:25:42.000000 tmnt-0.7.52/tmnt/utils/recalibrate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 16:25:56.768062 tmnt-0.7.52/tmnt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-13 16:25:56.000000 tmnt-0.7.52/tmnt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-13 16:25:56.000000 tmnt-0.7.52/tmnt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 16:25:56.000000 tmnt-0.7.52/tmnt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-13 16:25:56.000000 tmnt-0.7.52/tmnt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-13 16:25:56.000000 tmnt-0.7.52/tmnt.egg-info/top_level.txt
```

### Comparing `tmnt-0.7.51b20240412/LICENSE` & `tmnt-0.7.52/LICENSE`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.51b20240412/PKG-INFO` & `tmnt-0.7.52/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmnt
-Version: 0.7.51b20240412
+Version: 0.7.52
 Summary: Topic modeling neural toolkit
 Home-page: https://github.com/mitre/tmnt.git
 Author: The MITRE Corporation
 Author-email: wellner@mitre.org
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `tmnt-0.7.51b20240412/setup.py` & `tmnt-0.7.52/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from os import environ
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from pathlib import Path
 
-version = '0.7.51'
+version = '0.7.52'
 
 try:
     if not os.getenv('RELEASE'):
         from datetime import date
         today = date.today()
         day = today.strftime("b%Y%m%d")
         version += day
```

### Comparing `tmnt-0.7.51b20240412/tmnt/configuration.py` & `tmnt-0.7.52/tmnt/configuration.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.51b20240412/tmnt/data_loading.py` & `tmnt-0.7.52/tmnt/data_loading.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.51b20240412/tmnt/distribution.py` & `tmnt-0.7.52/tmnt/distribution.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.51b20240412/tmnt/estimator.py` & `tmnt-0.7.52/tmnt/estimator.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import numpy as np
 import scipy.sparse as sp
 import json
 
 from sklearn.metrics import average_precision_score, top_k_accuracy_score, roc_auc_score, ndcg_score, precision_recall_fscore_support
 from tmnt.data_loading import PairedDataLoader, SingletonWrapperLoader, SparseDataLoader, get_llm_model
 from tmnt.modeling import BowVAEModel, CovariateBowVAEModel, SeqBowVED
-from tmnt.modeling import SelfEmbeddingCrossEntropyLoss, GeneralizedSDMLLoss, MultiNegativeCrossEntropyLoss, MetricSeqBowVED, MetricBowVAEModel
+from tmnt.modeling import CrossBatchCosineSimilarityLoss, GeneralizedSDMLLoss, MultiNegativeCrossEntropyLoss, MetricSeqBowVED, MetricBowVAEModel
 from tmnt.eval_npmi import EvaluateNPMI
 from tmnt.distribution import LogisticGaussianDistribution, BaseDistribution, GaussianDistribution, VonMisesDistribution
 
 ## evaluation routines
 from torcheval.metrics import MultilabelAUPRC, MulticlassAUPRC
 
 ## huggingface specifics
@@ -1569,19 +1569,19 @@
             v_res['accuracy'] = metric_val[0]
         return v_res, metric_nm, metric_val
 
 
 class SeqBowMetricEstimator(SeqBowEstimator):
 
     def __init__(self, *args, sdml_smoothing_factor=0.3, metric_loss_temp=0.1, use_teacher_forcing=False, 
-                 teacher_forcing_right=True,
+                 teacher_forcing_mode='rand',
                  use_sdml=False, non_scoring_index=-1, **kwargs):
         super(SeqBowMetricEstimator, self).__init__(*args, **kwargs)
         if use_teacher_forcing:
-            self.loss_function = SelfEmbeddingCrossEntropyLoss(teacher_right=teacher_forcing_right, metric_loss_temp=metric_loss_temp)
+            self.loss_function = CrossBatchCosineSimilarityLoss(teacher_mode = teacher_forcing_mode)
         else:
             self.loss_function = \
                 GeneralizedSDMLLoss(smoothing_parameter=sdml_smoothing_factor, x2_downweight_idx=non_scoring_index) if use_sdml \
                 else MultiNegativeCrossEntropyLoss(smoothing_parameter=sdml_smoothing_factor, metric_loss_temp=metric_loss_temp)
         self.non_scoring_index = non_scoring_index ## if >=0 this will avoid considering this label index in evaluation
```

### Comparing `tmnt-0.7.51b20240412/tmnt/eval_npmi.py` & `tmnt-0.7.52/tmnt/eval_npmi.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.51b20240412/tmnt/inference.py` & `tmnt-0.7.52/tmnt/inference.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.51b20240412/tmnt/modeling.py` & `tmnt-0.7.52/tmnt/modeling.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import logging
 
 from tmnt.distribution import LogisticGaussianDistribution
 from tmnt.distribution import BaseDistribution
 from torch import nn
 from torch.nn.modules.loss import _Loss
 import torch
+from torch import Tensor
 from torch.distributions.categorical import Categorical
 
 from typing import List, Tuple, Dict, Optional, Union, NoReturn
 
 class BaseVAE(nn.Module):
 
     def __init__(self, vocab_size=2000, latent_distribution=LogisticGaussianDistribution(100, 20),
@@ -771,45 +772,43 @@
         return self.cross_entropy_loss(distances, labels.to(distances.device))
 
 
     def forward(self, x1, l1, x2, l2):
         return self._loss(x1, l1, x2, l2)    
 
 
-class SelfEmbeddingCrossEntropyLoss(_Loss):
+class CrossBatchCosineSimilarityLoss(_Loss):
     """
     Inputs:
         - **x1**: Minibatch of data points with shape (batch_size, vector_dim)
         - **x2**: Minibatch of data points with shape (batch_size, vector_dim)
           Each item in x1 is a positive sample for the items with the same label in x2
-          That is, x1[0] and x2[0] form a positive pair iff label(x1[0]) = label(x2[0])
-          All data points in different rows should be decorrelated
 
     Outputs:
         - **loss**: loss tensor with shape (batch_size,).
     """
 
-    def __init__(self, teacher_right=True, metric_loss_temp=0.5, batch_axis=0, **kwargs):
-        super(SelfEmbeddingCrossEntropyLoss, self).__init__(batch_axis, **kwargs)
-        self.cross_entropy_loss = nn.CrossEntropyLoss()
-        self.metric_loss_temp = metric_loss_temp
-        self.teacher_right = teacher_right
+    def __init__(self, teacher_mode='rand', batch_axis=0, **kwargs):
+        super(CrossBatchCosineSimilarityLoss, self).__init__(batch_axis, **kwargs)
+        self.loss_fn = nn.MSELoss() 
+        self.teacher_mode = teacher_mode
+        
+    def cosine_sim(self, a: Tensor, b: Tensor) -> Tensor:
+        a_norm = torch.nn.functional.normalize(a, p=2, dim=1)
+        b_norm = torch.nn.functional.normalize(b, p=2, dim=1)
+        return torch.mm(a_norm, b_norm.transpose(0, 1))
 
     def _loss(self, x1: torch.Tensor, l1: torch.Tensor, x2: torch.Tensor, l2: torch.Tensor):
-        """
-        the function computes the kl divergence between the negative distances
-        and the smoothed label matrix.
-        """
-        batch_size = l1.size()[0]
-        x1_norm = torch.nn.functional.normalize(x1, p=2, dim=1)
-        x2_norm = torch.nn.functional.normalize(x2, p=2, dim=1)
-        cross_side_distances = torch.mm(x1_norm, x2_norm.transpose(0,1)) / self.metric_loss_temp
-        single_side_distances = torch.mm(x2_norm, x2_norm.transpose(0,1)) / self.metric_loss_temp if self.teacher_right \
-            else torch.mm(x1_norm, x1_norm.transpose(0,1)) / self.metric_loss_temp
-        # need to normalize these
-        single_side_distances = single_side_distances / single_side_distances.sum(axis=1,keepdim=True).expand(batch_size, batch_size)
-        # multiply by the batch size to obtain the sum loss (kl_loss averages instead of sum)
-        return self.cross_entropy_loss(cross_side_distances, single_side_distances.to(single_side_distances.device))
-
+        scores = self.cosine_sim(x1,x2) 
+        if self.teacher_mode == 'right':
+            labels = self.cosine_sim(x2,x2).detach()
+        elif self.teacher_mode == 'left':
+            labels = self.cosine_sim(x1,x1).detach()
+        else:
+            if np.random.randint(2):
+                labels = self.cosine_sim(x2,x2).detach() 
+            else:
+                labels = self.cosine_sim(x1,x1).detach()
+        return self.loss_fn(scores, labels)
 
     def forward(self, x1, l1, x2, l2):
         return self._loss(x1, l1, x2, l2)
```

### Comparing `tmnt-0.7.51b20240412/tmnt/preprocess/tokenizer.py` & `tmnt-0.7.52/tmnt/preprocess/tokenizer.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.51b20240412/tmnt/preprocess/vectorizer.py` & `tmnt-0.7.52/tmnt/preprocess/vectorizer.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.51b20240412/tmnt/utils/csv2json.py` & `tmnt-0.7.52/tmnt/utils/csv2json.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.51b20240412/tmnt/utils/log_utils.py` & `tmnt-0.7.52/tmnt/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.51b20240412/tmnt/utils/mat_utils.py` & `tmnt-0.7.52/tmnt/utils/mat_utils.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.51b20240412/tmnt/utils/ngram_helpers.py` & `tmnt-0.7.52/tmnt/utils/ngram_helpers.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.51b20240412/tmnt/utils/pubmed_utils.py` & `tmnt-0.7.52/tmnt/utils/pubmed_utils.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.51b20240412/tmnt/utils/recalibrate.py` & `tmnt-0.7.52/tmnt/utils/recalibrate.py`

 * *Files identical despite different names*

### Comparing `tmnt-0.7.51b20240412/tmnt.egg-info/PKG-INFO` & `tmnt-0.7.52/tmnt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmnt
-Version: 0.7.51b20240412
+Version: 0.7.52
 Summary: Topic modeling neural toolkit
 Home-page: https://github.com/mitre/tmnt.git
 Author: The MITRE Corporation
 Author-email: wellner@mitre.org
 License: Apache
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `tmnt-0.7.51b20240412/tmnt.egg-info/SOURCES.txt` & `tmnt-0.7.52/tmnt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

