# Comparing `tmp/visionmetrics-0.0.8.tar.gz` & `tmp/visionmetrics-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visionmetrics-0.0.8.tar", last modified: Wed Aug 23 22:06:41 2023, max compression
+gzip compressed data, was "visionmetrics-0.0.9.tar", last modified: Sun Sep  3 03:16:38 2023, max compression
```

## Comparing `visionmetrics-0.0.8.tar` & `visionmetrics-0.0.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 22:06:41.195309 visionmetrics-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-08-23 22:06:41.195309 visionmetrics-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-23 22:06:41.199309 visionmetrics-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 22:06:41.187310 visionmetrics-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/tests/test_caption.py
--rw-r--r--   0 runner    (1001) docker     (123)    13243 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/tests/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/tests/test_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/tests/test_matting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/tests/test_prediction_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     6472 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/tests/test_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/tests/test_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 22:06:41.187310 visionmetrics-0.0.8/visionmetrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 22:06:41.191310 visionmetrics-0.0.8/visionmetrics/caption/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/caption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/caption/bleu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/caption/caption_eval_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/caption/cider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/caption/coco_evalcap_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/caption/meteor.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/caption/rougel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 22:06:41.195309 visionmetrics-0.0.8/visionmetrics/classification/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/classification/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/classification/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/classification/precision_recall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 22:06:41.195309 visionmetrics-0.0.8/visionmetrics/detection/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/detection/mean_ap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 22:06:41.195309 visionmetrics-0.0.8/visionmetrics/matting/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/matting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/matting/boundary_foreground_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/matting/boundary_mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/matting/foreground_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/matting/l1_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/matting/matting_eval_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/matting/mean_iou.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/prediction_filters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 22:06:41.195309 visionmetrics-0.0.8/visionmetrics/regression/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/regression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 22:06:41.195309 visionmetrics-0.0.8/visionmetrics/retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/retrieval/precision_recall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 22:06:41.195309 visionmetrics-0.0.8/visionmetrics/wrappers/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-08-23 22:03:11.000000 visionmetrics-0.0.8/visionmetrics/wrappers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-23 22:06:41.191310 visionmetrics-0.0.8/visionmetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-08-23 22:06:41.000000 visionmetrics-0.0.8/visionmetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-08-23 22:06:41.000000 visionmetrics-0.0.8/visionmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-23 22:06:41.000000 visionmetrics-0.0.8/visionmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-23 22:06:41.000000 visionmetrics-0.0.8/visionmetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-23 22:06:41.000000 visionmetrics-0.0.8/visionmetrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 03:16:38.838262 visionmetrics-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (999)     1141 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)     5267 2023-09-03 03:16:38.838262 visionmetrics-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     4935 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (999)       81 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (999)      738 2023-09-03 03:16:38.838262 visionmetrics-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 03:16:38.834262 visionmetrics-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (999)     2346 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/tests/test_caption.py
+-rw-r--r--   0 runner    (1001) docker     (999)    13243 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/tests/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5633 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/tests/test_detection.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2248 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/tests/test_matting.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1789 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/tests/test_prediction_filters.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6472 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/tests/test_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2561 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/tests/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 03:16:38.834262 visionmetrics-0.0.9/visionmetrics/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 03:16:38.834262 visionmetrics-0.0.9/visionmetrics/caption/
+-rw-r--r--   0 runner    (1001) docker     (999)      192 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/caption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      362 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/caption/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1374 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/caption/caption_eval_base.py
+-rw-r--r--   0 runner    (1001) docker     (999)      320 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/caption/cider.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3707 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/caption/coco_evalcap_utils.py
+-rw-r--r--   0 runner    (1001) docker     (999)      305 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/caption/meteor.py
+-rw-r--r--   0 runner    (1001) docker     (999)      336 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/caption/rougel.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 03:16:38.834262 visionmetrics-0.0.9/visionmetrics/classification/
+-rw-r--r--   0 runner    (1001) docker     (999)     1518 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      186 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/classification/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1323 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/classification/common.py
+-rw-r--r--   0 runner    (1001) docker     (999)      706 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/classification/precision_recall.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 03:16:38.838262 visionmetrics-0.0.9/visionmetrics/detection/
+-rw-r--r--   0 runner    (1001) docker     (999)      154 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3295 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/detection/mean_ap.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 03:16:38.838262 visionmetrics-0.0.9/visionmetrics/matting/
+-rw-r--r--   0 runner    (1001) docker     (999)      303 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/matting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2058 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/matting/boundary_foreground_iou.py
+-rw-r--r--   0 runner    (1001) docker     (999)      694 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/matting/boundary_mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1596 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/matting/foreground_iou.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1043 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/matting/l1_error.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1814 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/matting/matting_eval_base.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1551 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/matting/mean_iou.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2155 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/prediction_filters.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 03:16:38.838262 visionmetrics-0.0.9/visionmetrics/regression/
+-rw-r--r--   0 runner    (1001) docker     (999)      160 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/regression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 03:16:38.838262 visionmetrics-0.0.9/visionmetrics/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (999)      313 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2760 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/retrieval/precision_recall.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 03:16:38.838262 visionmetrics-0.0.9/visionmetrics/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (999)       86 2023-09-03 03:13:43.000000 visionmetrics-0.0.9/visionmetrics/wrappers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-03 03:16:38.834262 visionmetrics-0.0.9/visionmetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)     5267 2023-09-03 03:16:38.000000 visionmetrics-0.0.9/visionmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     1381 2023-09-03 03:16:38.000000 visionmetrics-0.0.9/visionmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-03 03:16:38.000000 visionmetrics-0.0.9/visionmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      155 2023-09-03 03:16:38.000000 visionmetrics-0.0.9/visionmetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)       24 2023-09-03 03:16:38.000000 visionmetrics-0.0.9/visionmetrics.egg-info/top_level.txt
```

### Comparing `visionmetrics-0.0.8/LICENSE` & `visionmetrics-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.8/PKG-INFO` & `visionmetrics-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visionmetrics
-Version: 0.0.8
+Version: 0.0.9
 Summary: Evaluation metric codes for various vision tasks.
 Home-page: https://github.com/microsoft/visionmetrics
 Author: Microsoft
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: caption
```

### Comparing `visionmetrics-0.0.8/README.md` & `visionmetrics-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.8/setup.cfg` & `visionmetrics-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = visionmetrics
-version = 0.0.8
+version = 0.0.9
 description = Evaluation metric codes for various vision tasks.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Microsoft
 license = MIT
 url = https://github.com/microsoft/visionmetrics
```

### Comparing `visionmetrics-0.0.8/tests/test_caption.py` & `visionmetrics-0.0.9/tests/test_caption.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.8/tests/test_classification.py` & `visionmetrics-0.0.9/tests/test_classification.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.8/tests/test_detection.py` & `visionmetrics-0.0.9/tests/test_detection.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.8/tests/test_matting.py` & `visionmetrics-0.0.9/tests/test_matting.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.8/tests/test_prediction_filters.py` & `visionmetrics-0.0.9/tests/test_prediction_filters.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.8/tests/test_retrieval.py` & `visionmetrics-0.0.9/tests/test_retrieval.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.8/tests/test_wrappers.py` & `visionmetrics-0.0.9/tests/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.8/visionmetrics/caption/caption_eval_base.py` & `visionmetrics-0.0.9/visionmetrics/caption/caption_eval_base.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.8/visionmetrics/caption/coco_evalcap_utils.py` & `visionmetrics-0.0.9/visionmetrics/caption/coco_evalcap_utils.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.8/visionmetrics/classification/__init__.py` & `visionmetrics-0.0.9/visionmetrics/classification/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Import metrics directly from torchmetrics
-from torchmetrics.classification import (BinaryAUROC, MulticlassAUROC,
+from torchmetrics.classification import (BinaryAccuracy, BinaryAUROC,
+                                         BinaryAveragePrecision,
+                                         BinaryConfusionMatrix, BinaryF1Score,
+                                         BinaryPrecision, BinaryRecall,
+                                         MulticlassAUROC,
                                          MulticlassAveragePrecision,
                                          MulticlassCalibrationError,
                                          MulticlassConfusionMatrix,
                                          MulticlassExactMatch,
                                          MultilabelAccuracy, MultilabelAUROC,
                                          MultilabelAveragePrecision,
                                          MultilabelConfusionMatrix,
```

### Comparing `visionmetrics-0.0.8/visionmetrics/classification/common.py` & `visionmetrics-0.0.9/visionmetrics/classification/common.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.8/visionmetrics/classification/precision_recall.py` & `visionmetrics-0.0.9/visionmetrics/classification/precision_recall.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.8/visionmetrics/detection/mean_ap.py` & `visionmetrics-0.0.9/visionmetrics/detection/mean_ap.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.8/visionmetrics/matting/boundary_foreground_iou.py` & `visionmetrics-0.0.9/visionmetrics/matting/boundary_foreground_iou.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.8/visionmetrics/matting/boundary_mean_iou.py` & `visionmetrics-0.0.9/visionmetrics/matting/boundary_mean_iou.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.8/visionmetrics/matting/foreground_iou.py` & `visionmetrics-0.0.9/visionmetrics/matting/foreground_iou.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.8/visionmetrics/matting/l1_error.py` & `visionmetrics-0.0.9/visionmetrics/matting/l1_error.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.8/visionmetrics/matting/matting_eval_base.py` & `visionmetrics-0.0.9/visionmetrics/matting/matting_eval_base.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.8/visionmetrics/matting/mean_iou.py` & `visionmetrics-0.0.9/visionmetrics/matting/mean_iou.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.8/visionmetrics/prediction_filters.py` & `visionmetrics-0.0.9/visionmetrics/prediction_filters.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.8/visionmetrics/retrieval/precision_recall.py` & `visionmetrics-0.0.9/visionmetrics/retrieval/precision_recall.py`

 * *Files identical despite different names*

### Comparing `visionmetrics-0.0.8/visionmetrics.egg-info/PKG-INFO` & `visionmetrics-0.0.9/visionmetrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visionmetrics
-Version: 0.0.8
+Version: 0.0.9
 Summary: Evaluation metric codes for various vision tasks.
 Home-page: https://github.com/microsoft/visionmetrics
 Author: Microsoft
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: caption
```

### Comparing `visionmetrics-0.0.8/visionmetrics.egg-info/SOURCES.txt` & `visionmetrics-0.0.9/visionmetrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

