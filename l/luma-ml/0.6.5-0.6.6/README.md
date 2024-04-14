# Comparing `tmp/luma-ml-0.6.5.tar.gz` & `tmp/luma-ml-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luma-ml-0.6.5.tar", last modified: Wed Apr  3 19:59:41 2024, max compression
+gzip compressed data, was "luma-ml-0.6.6.tar", last modified: Sun Apr 14 08:07:54 2024, max compression
```

## Comparing `luma-ml-0.6.5.tar` & `luma-ml-0.6.6.tar`

### file list

```diff
@@ -1,84 +1,86 @@
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.797733 luma-ml-0.6.5/
--rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.6.5/LICENSE
--rw-r--r--   0 chanlee    (501) staff       (20)     5558 2024-04-03 19:59:41.797466 luma-ml-0.6.5/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     5065 2024-04-03 19:59:24.000000 luma-ml-0.6.5/README.md
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.777717 luma-ml-0.6.5/luma/
--rw-r--r--   0 chanlee    (501) staff       (20)     9621 2024-04-03 12:19:39.000000 luma-ml-0.6.5/luma/__import__.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1501 2024-03-17 16:24:24.000000 luma-ml-0.6.5/luma/__init__.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.779895 luma-ml-0.6.5/luma/classifier/
--rw-r--r--   0 chanlee    (501) staff       (20)    12289 2024-04-03 15:07:50.000000 luma-ml-0.6.5/luma/classifier/discriminant.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7650 2024-04-03 15:41:30.000000 luma-ml-0.6.5/luma/classifier/logistic.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5566 2024-04-03 15:52:03.000000 luma-ml-0.6.5/luma/classifier/naive_bayes.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8976 2024-04-03 16:03:41.000000 luma-ml-0.6.5/luma/classifier/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8838 2024-04-03 17:17:16.000000 luma-ml-0.6.5/luma/classifier/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9562 2024-04-03 17:24:32.000000 luma-ml-0.6.5/luma/classifier/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.782068 luma-ml-0.6.5/luma/clustering/
--rw-r--r--   0 chanlee    (501) staff       (20)    17317 2024-04-03 17:28:35.000000 luma-ml-0.6.5/luma/clustering/affinity.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17423 2024-04-03 17:49:28.000000 luma-ml-0.6.5/luma/clustering/density.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7701 2024-04-03 17:55:23.000000 luma-ml-0.6.5/luma/clustering/hierarchy.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17775 2024-04-03 17:56:01.000000 luma-ml-0.6.5/luma/clustering/kmeans.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8022 2024-04-03 17:57:13.000000 luma-ml-0.6.5/luma/clustering/mixture.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11490 2024-04-03 18:01:29.000000 luma-ml-0.6.5/luma/clustering/spectral.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.783030 luma-ml-0.6.5/luma/core/
--rw-r--r--   0 chanlee    (501) staff       (20)     5174 2024-04-03 19:14:20.000000 luma-ml-0.6.5/luma/core/base.py
--rw-r--r--   0 chanlee    (501) staff       (20)      393 2024-03-17 16:24:24.000000 luma-ml-0.6.5/luma/core/main.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10135 2024-04-03 19:09:33.000000 luma-ml-0.6.5/luma/core/super.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.784758 luma-ml-0.6.5/luma/ensemble/
--rw-r--r--   0 chanlee    (501) staff       (20)     9738 2024-04-03 18:04:08.000000 luma-ml-0.6.5/luma/ensemble/bagging.py
--rw-r--r--   0 chanlee    (501) staff       (20)    19296 2024-04-03 18:09:25.000000 luma-ml-0.6.5/luma/ensemble/boost.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9678 2024-04-03 18:09:26.000000 luma-ml-0.6.5/luma/ensemble/forest.py
--rw-r--r--   0 chanlee    (501) staff       (20)    13574 2024-04-03 18:11:50.000000 luma-ml-0.6.5/luma/ensemble/stack.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6500 2024-03-17 16:24:24.000000 luma-ml-0.6.5/luma/ensemble/vote.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.785410 luma-ml-0.6.5/luma/interface/
--rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-04-03 15:51:54.000000 luma-ml-0.6.5/luma/interface/exception.py
--rw-r--r--   0 chanlee    (501) staff       (20)    14307 2024-04-03 17:28:18.000000 luma-ml-0.6.5/luma/interface/util.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.786529 luma-ml-0.6.5/luma/metric/
--rw-r--r--   0 chanlee    (501) staff       (20)     1471 2024-03-17 17:44:55.000000 luma-ml-0.6.5/luma/metric/classification.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5709 2024-03-17 18:40:44.000000 luma-ml-0.6.5/luma/metric/clustering.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1551 2024-03-19 13:36:06.000000 luma-ml-0.6.5/luma/metric/distance.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1646 2024-03-19 16:59:18.000000 luma-ml-0.6.5/luma/metric/regression.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.786822 luma-ml-0.6.5/luma/migrate/
--rw-r--r--   0 chanlee    (501) staff       (20)     3425 2024-04-03 18:12:20.000000 luma-ml-0.6.5/luma/migrate/port.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.788262 luma-ml-0.6.5/luma/model_selection/
--rw-r--r--   0 chanlee    (501) staff       (20)     3357 2024-04-03 18:17:54.000000 luma-ml-0.6.5/luma/model_selection/cv.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7964 2024-04-03 18:17:54.000000 luma-ml-0.6.5/luma/model_selection/fold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11720 2024-04-03 18:17:54.000000 luma-ml-0.6.5/luma/model_selection/search.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3570 2024-04-03 18:17:54.000000 luma-ml-0.6.5/luma/model_selection/split.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.789524 luma-ml-0.6.5/luma/neural/
--rw-r--r--   0 chanlee    (501) staff       (20)     1909 2024-03-29 20:03:35.000000 luma-ml-0.6.5/luma/neural/activation.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10709 2024-04-03 18:19:49.000000 luma-ml-0.6.5/luma/neural/multi_layer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7118 2024-04-03 18:24:38.000000 luma-ml-0.6.5/luma/neural/optimizer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8237 2024-04-03 18:26:58.000000 luma-ml-0.6.5/luma/neural/single.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.789830 luma-ml-0.6.5/luma/pipe/
--rw-r--r--   0 chanlee    (501) staff       (20)     7279 2024-04-03 18:27:03.000000 luma-ml-0.6.5/luma/pipe/pipeline.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.791108 luma-ml-0.6.5/luma/preprocessing/
--rw-r--r--   0 chanlee    (501) staff       (20)     5332 2024-04-03 18:29:25.000000 luma-ml-0.6.5/luma/preprocessing/encoder.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5556 2024-04-03 18:33:19.000000 luma-ml-0.6.5/luma/preprocessing/imputer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3553 2024-04-03 18:34:45.000000 luma-ml-0.6.5/luma/preprocessing/outlier.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2551 2024-04-03 18:34:48.000000 luma-ml-0.6.5/luma/preprocessing/scaler.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.791947 luma-ml-0.6.5/luma/reduction/
--rw-r--r--   0 chanlee    (501) staff       (20)    18473 2024-04-03 18:41:38.000000 luma-ml-0.6.5/luma/reduction/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)    39231 2024-04-03 19:59:39.000000 luma-ml-0.6.5/luma/reduction/manifold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    15454 2024-03-17 16:24:24.000000 luma-ml-0.6.5/luma/reduction/selection.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.794577 luma-ml-0.6.5/luma/regressor/
--rw-r--r--   0 chanlee    (501) staff       (20)    17451 2024-03-29 20:03:41.000000 luma-ml-0.6.5/luma/regressor/general.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11186 2024-04-03 11:16:13.000000 luma-ml-0.6.5/luma/regressor/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6205 2024-03-17 16:24:24.000000 luma-ml-0.6.5/luma/regressor/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2720 2024-03-17 16:24:24.000000 luma-ml-0.6.5/luma/regressor/poly.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10094 2024-03-17 16:24:24.000000 luma-ml-0.6.5/luma/regressor/robust.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6764 2024-04-03 11:16:13.000000 luma-ml-0.6.5/luma/regressor/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6861 2024-03-17 16:24:24.000000 luma-ml-0.6.5/luma/regressor/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.795203 luma-ml-0.6.5/luma/visual/
--rw-r--r--   0 chanlee    (501) staff       (20)     2971 2024-03-17 16:24:24.000000 luma-ml-0.6.5/luma/visual/eda.py
--rw-r--r--   0 chanlee    (501) staff       (20)    29242 2024-03-29 17:27:43.000000 luma-ml-0.6.5/luma/visual/evaluation.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.796358 luma-ml-0.6.5/luma_ml.egg-info/
--rw-r--r--   0 chanlee    (501) staff       (20)     5558 2024-04-03 19:59:41.000000 luma-ml-0.6.5/luma_ml.egg-info/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     1585 2024-04-03 19:59:41.000000 luma-ml-0.6.5/luma_ml.egg-info/SOURCES.txt
--rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-04-03 19:59:41.000000 luma-ml-0.6.5/luma_ml.egg-info/dependency_links.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-04-03 19:59:41.000000 luma-ml-0.6.5/luma_ml.egg-info/requires.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-04-03 19:59:41.000000 luma-ml-0.6.5/luma_ml.egg-info/top_level.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-04-03 19:59:41.797798 luma-ml-0.6.5/setup.cfg
--rw-r--r--   0 chanlee    (501) staff       (20)      795 2024-04-03 19:59:30.000000 luma-ml-0.6.5/setup.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-03 19:59:41.796860 luma-ml-0.6.5/test/
--rw-r--r--   0 chanlee    (501) staff       (20)      105 2024-03-30 12:09:50.000000 luma-ml-0.6.5/test/__local__.py
--rw-r--r--   0 chanlee    (501) staff       (20)      807 2024-04-03 19:42:17.000000 luma-ml-0.6.5/test/_docs.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.809416 luma-ml-0.6.6/
+-rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.6.6/LICENSE
+-rw-r--r--   0 chanlee    (501) staff       (20)     5553 2024-04-14 08:07:54.809083 luma-ml-0.6.6/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     4947 2024-04-14 08:05:18.000000 luma-ml-0.6.6/README.md
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.787294 luma-ml-0.6.6/luma/
+-rw-r--r--   0 chanlee    (501) staff       (20)     9858 2024-04-14 08:03:23.000000 luma-ml-0.6.6/luma/__import__.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1501 2024-03-17 16:24:24.000000 luma-ml-0.6.6/luma/__init__.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.789537 luma-ml-0.6.6/luma/classifier/
+-rw-r--r--   0 chanlee    (501) staff       (20)    12269 2024-04-04 10:30:54.000000 luma-ml-0.6.6/luma/classifier/discriminant.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7627 2024-04-04 10:35:57.000000 luma-ml-0.6.6/luma/classifier/logistic.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5539 2024-04-04 10:36:09.000000 luma-ml-0.6.6/luma/classifier/naive_bayes.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8951 2024-04-04 10:36:38.000000 luma-ml-0.6.6/luma/classifier/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8854 2024-04-04 18:17:19.000000 luma-ml-0.6.6/luma/classifier/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9534 2024-04-04 10:37:54.000000 luma-ml-0.6.6/luma/classifier/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.794968 luma-ml-0.6.6/luma/clustering/
+-rw-r--r--   0 chanlee    (501) staff       (20)    17258 2024-04-04 10:38:24.000000 luma-ml-0.6.6/luma/clustering/affinity.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17399 2024-04-04 10:39:29.000000 luma-ml-0.6.6/luma/clustering/density.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7670 2024-04-04 10:39:48.000000 luma-ml-0.6.6/luma/clustering/hierarchy.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17693 2024-04-04 10:41:26.000000 luma-ml-0.6.6/luma/clustering/kmeans.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8017 2024-04-04 11:10:57.000000 luma-ml-0.6.6/luma/clustering/mixture.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11402 2024-04-04 11:13:10.000000 luma-ml-0.6.6/luma/clustering/spectral.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.795715 luma-ml-0.6.6/luma/core/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5248 2024-04-14 08:02:38.000000 luma-ml-0.6.6/luma/core/base.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      393 2024-04-11 15:05:45.000000 luma-ml-0.6.6/luma/core/main.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10620 2024-04-14 08:01:24.000000 luma-ml-0.6.6/luma/core/super.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.797551 luma-ml-0.6.6/luma/ensemble/
+-rw-r--r--   0 chanlee    (501) staff       (20)     9715 2024-04-04 11:13:31.000000 luma-ml-0.6.6/luma/ensemble/bagging.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    19224 2024-04-04 11:16:30.000000 luma-ml-0.6.6/luma/ensemble/boost.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9631 2024-04-04 11:17:33.000000 luma-ml-0.6.6/luma/ensemble/forest.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    13548 2024-04-04 11:17:49.000000 luma-ml-0.6.6/luma/ensemble/stack.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6479 2024-04-04 11:18:40.000000 luma-ml-0.6.6/luma/ensemble/vote.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.798031 luma-ml-0.6.6/luma/interface/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-04-03 15:51:54.000000 luma-ml-0.6.6/luma/interface/exception.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    14236 2024-04-14 07:13:23.000000 luma-ml-0.6.6/luma/interface/util.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.798731 luma-ml-0.6.6/luma/metric/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1471 2024-03-17 17:44:55.000000 luma-ml-0.6.6/luma/metric/classification.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5709 2024-03-17 18:40:44.000000 luma-ml-0.6.6/luma/metric/clustering.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1551 2024-03-19 13:36:06.000000 luma-ml-0.6.6/luma/metric/distance.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1646 2024-03-19 16:59:18.000000 luma-ml-0.6.6/luma/metric/regression.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.798893 luma-ml-0.6.6/luma/migrate/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3425 2024-04-03 18:12:20.000000 luma-ml-0.6.6/luma/migrate/port.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.800062 luma-ml-0.6.6/luma/model_selection/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3267 2024-04-04 17:34:24.000000 luma-ml-0.6.6/luma/model_selection/cv.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7679 2024-04-04 17:35:02.000000 luma-ml-0.6.6/luma/model_selection/fold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11844 2024-04-11 14:17:07.000000 luma-ml-0.6.6/luma/model_selection/search.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3472 2024-04-12 16:33:14.000000 luma-ml-0.6.6/luma/model_selection/split.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.800773 luma-ml-0.6.6/luma/neural/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1891 2024-04-04 11:21:05.000000 luma-ml-0.6.6/luma/neural/activation.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    16698 2024-04-14 08:07:19.000000 luma-ml-0.6.6/luma/neural/network.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    19581 2024-04-14 08:02:42.000000 luma-ml-0.6.6/luma/neural/optimizer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8208 2024-04-11 14:52:27.000000 luma-ml-0.6.6/luma/neural/single.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.800955 luma-ml-0.6.6/luma/pipe/
+-rw-r--r--   0 chanlee    (501) staff       (20)     7217 2024-04-11 12:45:03.000000 luma-ml-0.6.6/luma/pipe/pipeline.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.801658 luma-ml-0.6.6/luma/preprocessing/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5293 2024-04-10 12:13:12.000000 luma-ml-0.6.6/luma/preprocessing/encoder.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5531 2024-04-10 12:30:21.000000 luma-ml-0.6.6/luma/preprocessing/imputer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3600 2024-04-10 19:13:28.000000 luma-ml-0.6.6/luma/preprocessing/outlier.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2553 2024-04-11 08:17:54.000000 luma-ml-0.6.6/luma/preprocessing/scaler.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.802474 luma-ml-0.6.6/luma/reduction/
+-rw-r--r--   0 chanlee    (501) staff       (20)    18446 2024-04-04 11:25:12.000000 luma-ml-0.6.6/luma/reduction/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    39139 2024-04-04 15:10:56.000000 luma-ml-0.6.6/luma/reduction/manifold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    16170 2024-04-05 18:23:54.000000 luma-ml-0.6.6/luma/reduction/selection.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.804458 luma-ml-0.6.6/luma/regressor/
+-rw-r--r--   0 chanlee    (501) staff       (20)    19091 2024-04-06 10:17:17.000000 luma-ml-0.6.6/luma/regressor/general.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12178 2024-04-07 16:01:11.000000 luma-ml-0.6.6/luma/regressor/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6636 2024-04-07 19:41:56.000000 luma-ml-0.6.6/luma/regressor/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2960 2024-04-07 20:18:45.000000 luma-ml-0.6.6/luma/regressor/poly.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10678 2024-04-08 19:03:59.000000 luma-ml-0.6.6/luma/regressor/robust.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7486 2024-04-10 11:10:31.000000 luma-ml-0.6.6/luma/regressor/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7187 2024-04-10 11:41:01.000000 luma-ml-0.6.6/luma/regressor/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.806152 luma-ml-0.6.6/luma/visual/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3045 2024-04-13 08:30:32.000000 luma-ml-0.6.6/luma/visual/eda.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    24471 2024-04-13 15:18:20.000000 luma-ml-0.6.6/luma/visual/evaluation.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.807349 luma-ml-0.6.6/luma_ml.egg-info/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5553 2024-04-14 08:07:54.000000 luma-ml-0.6.6/luma_ml.egg-info/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     1614 2024-04-14 08:07:54.000000 luma-ml-0.6.6/luma_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-04-14 08:07:54.000000 luma-ml-0.6.6/luma_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-04-14 08:07:54.000000 luma-ml-0.6.6/luma_ml.egg-info/requires.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-04-14 08:07:54.000000 luma-ml-0.6.6/luma_ml.egg-info/top_level.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-04-14 08:07:54.809499 luma-ml-0.6.6/setup.cfg
+-rw-r--r--   0 chanlee    (501) staff       (20)      795 2024-04-14 08:07:32.000000 luma-ml-0.6.6/setup.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-04-14 08:07:54.808463 luma-ml-0.6.6/test/
+-rw-r--r--   0 chanlee    (501) staff       (20)      105 2024-03-30 12:09:50.000000 luma-ml-0.6.6/test/__local__.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2085 2024-04-14 07:50:54.000000 luma-ml-0.6.6/test/_mlp_clf.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2220 2024-04-14 08:01:16.000000 luma-ml-0.6.6/test/_mlp_reg.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1200 2024-04-14 07:04:45.000000 luma-ml-0.6.6/test/_opt.py
```

### Comparing `luma-ml-0.6.5/LICENSE` & `luma-ml-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.5/PKG-INFO` & `luma-ml-0.6.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.6.5
+Version: 0.6.6
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/LUMA
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
 
 <!DOCTYPE html>
 <html>
     <body>
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-4.3k-red">
-        <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/ChanLumerico/luma?color=yellow">
+        <img src="https://img.shields.io/badge/total downloads-4.8k-red">
+        <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
-        <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=purple">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
                     <th>Description</th>
                 </tr>
@@ -104,23 +108,23 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.6.5</td>
+                    <td>0.6.6</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~15.7K</td>
+                    <td>~16.3K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
-                    <td>Python 3.10 or later</td>
+                    <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
                     <td>NumPy, SciPy, Pandas, Matplotlib, Seaborn</td>
                 </tr>
                 <tr>
                     <td>Documentation</td>
```

#### html2text {}

```diff
@@ -1,19 +1,21 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.6.5 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.6.6 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/LUMA Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.10
-Description-Content-Type: text/markdown License-File: LICENSE
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
+Requires-Dist: seaborn
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-4.3k-red][GitHub last commit][Code Style][GitHub code size in bytes]
+4.8k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -31,12 +33,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.6.5
-Lines of Code  ~15.7K
-Requirement    Python 3.10 or later
+Latest Version 0.6.6
+Lines of Code  ~16.3K
+Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.6.5/README.md` & `luma-ml-0.6.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,18 +4,17 @@
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-4.3k-red">
-        <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/ChanLumerico/luma?color=yellow">
+        <img src="https://img.shields.io/badge/total downloads-4.8k-red">
+        <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
-        <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=purple">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
                     <th>Description</th>
                 </tr>
@@ -90,23 +89,23 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.6.5</td>
+                    <td>0.6.6</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~15.7K</td>
+                    <td>~16.3K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
-                    <td>Python 3.10 or later</td>
+                    <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
                     <td>NumPy, SciPy, Pandas, Matplotlib, Seaborn</td>
                 </tr>
                 <tr>
                     <td>Documentation</td>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-4.3k-red][GitHub last commit][Code Style][GitHub code size in bytes]
+4.8k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -24,12 +24,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.6.5
-Lines of Code  ~15.7K
-Requirement    Python 3.10 or later
+Latest Version 0.6.6
+Lines of Code  ~16.3K
+Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.6.5/luma/__import__.py` & `luma-ml-0.6.6/luma/__import__.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,17 +57,27 @@
 from luma.ensemble.vote import VotingClassifier, VotingRegressor
 from luma.ensemble.bagging import BaggingClassifier, BaggingRegressor
 from luma.ensemble.boost import AdaBoostClassifier, AdaBoostRegressor
 from luma.ensemble.boost import GradientBoostingClassifier, GradientBoostingRegressor
 from luma.ensemble.stack import StackingClassifier, StackingRegressor
 
 from luma.neural.activation import ReLU, LeakyReLU, ELU, Tanh, Sigmoid, Softmax
-from luma.neural.optimizer import SGDOptimizer, MomentumOptimizer, RMSPropOptimizer
+from luma.neural.optimizer import (
+    SGDOptimizer,
+    MomentumOptimizer,
+    RMSPropOptimizer,
+    AdamOptimizer,
+    AdaGradOptimizer,
+    AdaDeltaOptimizer,
+    AdaMaxOptimizer,
+    AdamWOptimizer,
+    NAdamOptimizer,
+)
 from luma.neural.single import PerceptronClassifier, PerceptronRegressor
-from luma.neural.multi_layer import MLPClassifier
+from luma.neural.network import MLPClassifier, MLPRegressor
 
 from luma.metric.classification import Accuracy, Precision, Recall, F1Score, Specificity
 from luma.metric.regression import (
     MeanAbsoluteError,
     MeanSquaredError,
     RootMeanSquaredError,
     MeanAbsolutePercentageError,
@@ -118,26 +128,26 @@
 )
 from luma.regressor.robust import RANSAC, MLESAC
 
 from luma.pipe.pipeline import Pipeline
 
 from luma.visual.eda import (
     CorrelationBar,
-    CorrelationHeatMap,
+    CorrelationHeatmap,
     JointPlot,
     MissingProportion,
 )
 from luma.visual.evaluation import (
     DecisionRegion,
     ClusterPlot,
     ROCCurve,
     PrecisionRecallCurve,
 )
 from luma.visual.evaluation import ConfusionMatrix, ResidualPlot, LearningCurve
-from luma.visual.evaluation import ValidationCurve, ValidationHeatmap, InertiaPlot
+from luma.visual.evaluation import ValidationCurve, InertiaPlot
 
 from luma.migrate.port import ModelPorter
 
 
 if __name__ == "__main__":
 
     # ------------------- [ luma.core ] ------------------------
@@ -198,19 +208,21 @@
     GradientBoostingClassifier, GradientBoostingRegressor
 
     StackingClassifier, StackingRegressor
 
     # ------------------- [ luma.neural ] ----------------------
     PerceptronClassifier, PerceptronRegressor
 
-    MLPClassifier
+    MLPClassifier, MLPRegressor
 
     ReLU, LeakyReLU, ELU, Tanh, Sigmoid, Softmax
 
-    SGDOptimizer, MomentumOptimizer, RMSPropOptimizer
+    SGDOptimizer, MomentumOptimizer, RMSPropOptimizer,
+    AdamOptimizer, AdaGradOptimizer, AdaDeltaOptimizer,
+    AdaMaxOptimizer, AdamWOptimizer, NAdamOptimizer
 
     # ------------------- [ luma.metric ] ----------------------
     Accuracy, Precision, Recall, F1Score, Specificity
 
     MeanAbsoluteError, MeanSquaredError, RootMeanSquaredError,
     MeanAbsolutePercentageError, RSquaredScore,
     AdjustedRSquaredScore
@@ -266,16 +278,16 @@
 
     RANSAC, MLESAC
 
     # -------------------- [ luma.pipe ] -----------------------
     Pipeline
 
     # ------------------- [ luma.visual ] ----------------------
-    CorrelationBar, CorrelationHeatMap, JointPlot,
+    CorrelationBar, CorrelationHeatmap, JointPlot,
     MissingProportion
 
     DecisionRegion, ClusterPlot, ROCCurve, PrecisionRecallCurve,
     ConfusionMatrix, ResidualPlot, LearningCurve,
-    ValidationCurve, ValidationHeatmap, InertiaPlot
+    ValidationCurve, InertiaPlot
 
     # ------------------ [ luma.migrate ] ----------------------
     ModelPorter
```

### Comparing `luma-ml-0.6.5/luma/__init__.py` & `luma-ml-0.6.6/luma/__init__.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.5/luma/classifier/discriminant.py` & `luma-ml-0.6.6/luma/classifier/discriminant.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import numpy as np
+from typing import Self
 from scipy.special import softmax
 from scipy.stats import multivariate_normal
+import numpy as np
 
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.interface.util import Matrix, Scalar, Vector, KernelUtil
 from luma.interface.exception import NotFittedError
 from luma.metric.classification import Accuracy
 
 
@@ -29,15 +30,15 @@
 
     def __init__(self) -> None:
         self.means = (None,)
         self.priors = (None,)
         self.covs = None
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Vector) -> "LDAClassifier":
+    def fit(self, X: Matrix, y: Vector) -> Self:
         m, n = X.shape
         class_labels = np.unique(y)
         n_classes = len(class_labels)
 
         self.means = np.zeros((n_classes, n))
         self.priors = np.zeros(n_classes)
         self.covs = np.zeros((n, n))
@@ -92,15 +93,15 @@
     def __init__(self) -> None:
         self.means = None
         self.covs = None
         self.priors = None
         self.classes = None
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Vector) -> "QDAClassifier":
+    def fit(self, X: Matrix, y: Vector) -> Self:
         m, n = X.shape
         self.classes = np.unique(y)
         n_classes = len(self.classes)
 
         self.means = np.zeros((n_classes, n))
         self.covs = np.zeros((n_classes, n, n))
         self.priors = np.zeros(n_classes)
@@ -183,15 +184,15 @@
         self.priors = None
         self.covs = None
         self._fitted = False
 
         self.set_param_ranges({"alpha": ("0,+1", None), "gamma": ("0<,+inf", None)})
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, y: Vector) -> "RDAClassifier":
+    def fit(self, X: Matrix, y: Vector) -> Self:
         m, n = X.shape
         self.classes = np.unique(y)
         n_classes = len(self.classes)
 
         self.means = np.zeros((n_classes, n))
         self.pooled_cov = np.zeros((n, n))
         self.covs = np.zeros((n_classes, n, n))
@@ -305,15 +306,15 @@
             "gamma": self.gamma,
             "coef": self.coef,
         }
 
         self.set_param_ranges({"deg": ("0,+inf", int), "gamma": ("0<,+inf", None)})
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, y: Vector) -> "KDAClassifier":
+    def fit(self, X: Matrix, y: Vector) -> Self:
         m, _ = X.shape
         self._X = X
         self.classes = np.unique(y)
         self.n_classes = len(self.classes)
 
         self.ku_ = KernelUtil(self.kernel, **self.kernel_params)
         self.class_means = np.zeros((self.n_classes, m))
```

### Comparing `luma-ml-0.6.5/luma/classifier/logistic.py` & `luma-ml-0.6.6/luma/classifier/logistic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal
+from typing import Literal, Self
 import numpy as np
 
 from luma.interface.util import Matrix
 from luma.metric.classification import Accuracy
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.core.super import Estimator, Evaluator, Supervised
 
@@ -53,15 +53,15 @@
             }
         )
         self.check_param_ranges()
 
     def sigmoid(self, z: Matrix) -> Matrix:
         return 1 / (1 + np.exp(-z))
 
-    def fit(self, X: Matrix, y: Matrix) -> "LogisticRegressor":
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         X = np.insert(X, 0, 1, axis=1)
         m, n = X.shape
         self.theta = np.zeros(n)
 
         for i in range(self.max_iter):
             z = np.dot(X, self.theta)
             h = self.sigmoid(z)
@@ -155,15 +155,15 @@
         )
         self.check_param_ranges()
 
     def softmax(self, z: Matrix) -> Matrix:
         exp_z = np.exp(z - np.max(z, axis=1, keepdims=True))
         return exp_z / exp_z.sum(axis=1, keepdims=True)
 
-    def fit(self, X: Matrix, y: Matrix) -> "SoftmaxRegressor":
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         X = np.insert(X, 0, 1, axis=1)
         m, n = X.shape
         num_classes = len(np.unique(y))
         self.theta = np.zeros((n, num_classes))
 
         for i in range(self.max_iter):
             z = np.dot(X, self.theta)
```

### Comparing `luma-ml-0.6.5/luma/classifier/naive_bayes.py` & `luma-ml-0.6.6/luma/classifier/naive_bayes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any
+from typing import Any, Self
 import numpy as np
 
 from luma.interface.util import Matrix, Vector
 from luma.interface.exception import NotFittedError
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.metric.classification import Accuracy
 
@@ -16,15 +16,15 @@
     It's based on Bayes' theorem and makes an assumption
     that the features follow a Gaussian distribution.
     """
 
     def __init__(self) -> None:
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> "GaussianNaiveBayes":
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         self.classes = np.unique(y)
         self.parameters = []
         self.priors = []
         self.X_train = X
         self.y_train = y
 
         shared_cov_matrix = np.zeros((X.shape[1], X.shape[1]))
@@ -95,15 +95,15 @@
     (i.e., they are either present or absent) and that they are
     conditionally independent given the class label.
     """
 
     def __init__(self) -> None:
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> "BernoulliNaiveBayes":
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         self.classes = np.unique(y)
         self.class_probs = np.zeros(len(self.classes))
         self.feature_probs = np.zeros((len(self.classes), X.shape[1]))
 
         for i, c in enumerate(self.classes):
             X_cls = X[y == c]
             self.class_probs[i] = len(X_cls) / len(y)
```

### Comparing `luma-ml-0.6.5/luma/classifier/neighbors.py` & `luma-ml-0.6.6/luma/classifier/neighbors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Self
 from scipy.spatial import distance_matrix
 import numpy as np
 
 from luma.interface.util import Matrix
 from luma.core.super import Estimator, Supervised, Evaluator
 from luma.interface.util import NearestNeighbors
 from luma.interface.exception import NotFittedError
@@ -32,15 +33,15 @@
         self._neighbors = None
         self._y = None
         self._fitted = False
 
         self.set_param_ranges({"n_neighbors": ("0,+inf", int)})
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, y: Matrix) -> "KNNClassifier":
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         self._neighbors = NearestNeighbors(X, self.n_neighbors)
         self._y = y
         self._fitted = True
         return self
 
     def predict(self, X: Matrix) -> Matrix:
         if not self._fitted:
@@ -114,15 +115,15 @@
                 "n_density": ("0<,+int", int),
                 "min_neighbors": ("0<,+int", int),
                 "max_neighbors": ("0<,+int", int),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, y: Matrix) -> "AdaptiveKNNClassifier":
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         self._X = X
         self._y = y
 
         self.dist_matrix = distance_matrix(X, X)
         self.local_density = np.sort(self.dist_matrix, axis=1)
         self.local_density = self.local_density[:, self.n_density]
 
@@ -199,15 +200,15 @@
         self._X = None
         self._y = None
         self._fitted = False
 
         self.set_param_ranges({"n_neighbors": ("0,+inf", int)})
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, y: Matrix) -> "WeightedKNNClassifier":
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         self._X = X
         self._y = y
 
         self._fitted = True
         return self
 
     def predict(self, X: Matrix) -> Matrix:
```

### Comparing `luma-ml-0.6.5/luma/classifier/svm.py` & `luma-ml-0.6.6/luma/classifier/svm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Self
 import numpy as np
 
 from luma.interface.util import Matrix, KernelUtil
 from luma.interface.exception import NotFittedError
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.metric.classification import Accuracy
 
@@ -47,15 +48,15 @@
                 "batch_size": ("0<,+int", int),
                 "learning_rate": ("0<,+inf", None),
                 "max_iter": ("0,+inf", int),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, y: Matrix) -> "SVC":
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         classes = np.unique(y)
         self.models = []
         for cl in classes:
             binary_y = np.where(y == cl, 1, -1)
             self._binary_fit(X, binary_y, cl)
             if self.verbose:
                 print(f"[SVC] Finished OvR fit for class {cl}\n")
@@ -151,24 +152,24 @@
         self.verbose = verbose
         self._kernel_func = None
         self._fitted = False
 
         self.set_param_ranges(
             {
                 "C": ("0,+inf", None),
-                "batch_size": ("0<,+int", int),
+                "batch_size": ("0<,+inf", int),
                 "learning_rate": ("0<,+inf", None),
                 "max_iter": ("0,+inf", int),
                 "deg": ("0,+inf", int),
                 "gamma": ("0,+inf", None),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, y: Matrix) -> "KernelSVC":
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         classes = np.unique(y)
         self.models = []
         self._set_kernel_func()
 
         for cl in classes:
             binary_y = np.where(y == cl, 1, -1)
             self._binary_fit(X, binary_y, cl)
```

### Comparing `luma-ml-0.6.5/luma/classifier/tree.py` & `luma-ml-0.6.6/luma/classifier/tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal, Tuple
+from typing import Literal, Self, Tuple
 import numpy as np
 
 from luma.interface.util import Matrix, Vector
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.interface.util import DecisionTreeNode
 from luma.metric.classification import Accuracy
@@ -66,17 +66,15 @@
                 "min_impurity_decrease": ("0,+inf", None),
                 "max_leaf_nodes": ("0<,+inf", int),
             }
         )
         self.check_param_ranges()
         np.random.seed(random_state)
 
-    def fit(
-        self, X: Matrix, y: Vector, sample_weights: Vector = None
-    ) -> "DecisionTreeClassifier":
+    def fit(self, X: Matrix, y: Vector, sample_weights: Vector = None) -> Self:
         if sample_weights is None:
             sample_weights = np.ones(len(y))
         sample_weights = Vector(sample_weights)
 
         self.classes_ = np.unique(y)
         self.root = self._build_tree(X, y, 0, sample_weights)
         self._fitted = True
```

### Comparing `luma-ml-0.6.5/luma/clustering/affinity.py` & `luma-ml-0.6.6/luma/clustering/affinity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal
+from typing import Literal, Self
 import numpy as np
 
 from luma.interface.util import Matrix, Vector, Scalar, KernelUtil
 from luma.core.super import Estimator, Evaluator, Unsupervised
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.metric.clustering import SilhouetteCoefficient
 
@@ -64,15 +64,15 @@
         self.verbose = verbose
         self._X = None
         self._fitted = False
 
         self.set_param_ranges({"max_iter": ("0<,+inf", int), "damping": ("0,1", None)})
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "AffinityPropagation":
+    def fit(self, X: Matrix) -> Self:
         self._X = X
         m, _ = X.shape
 
         S = self._compute_similarity(X)
         S = self._assign_preference(S)
         S += 1e-12 * np.random.normal(size=(m, m)) * (np.max(S) - np.min(S))
 
@@ -221,15 +221,15 @@
                 "max_iter": ("0<,+inf", int),
                 "damping": ("0,1", None),
                 "lambda_param": ("0,+inf", None),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "AdaptiveAffinityPropagation":
+    def fit(self, X: Matrix) -> Self:
         self._X = X
         m, _ = X.shape
 
         S = self._compute_similarity(X)
         S = self._assign_preference(S)
         S += 1e-12 * np.random.normal(size=(m, m)) * (np.max(S) - np.min(S))
 
@@ -387,15 +387,15 @@
                 "max_iter": ("0<,+inf", int),
                 "damping": ("0,1", None),
                 "gamma": ("0<,+inf", None),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "KernelAffinityPropagation":
+    def fit(self, X: Matrix) -> Self:
         self._X = X
         m, _ = X.shape
 
         kernel_func = KernelUtil(self.kernel, gamma=self.gamma).kernel_func
         X_trans = kernel_func(X)
 
         S = self._compute_similarity(X_trans)
```

### Comparing `luma-ml-0.6.5/luma/clustering/density.py` & `luma-ml-0.6.6/luma/clustering/density.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal, Optional, Tuple, List
+from typing import Literal, Optional, Self, Tuple, List
 from matplotlib import pyplot as plt
 from scipy.spatial.distance import cdist
 import numpy as np
 
 from luma.core.super import Estimator, Evaluator, Unsupervised
 from luma.interface.util import Matrix, Vector, Scalar
 from luma.interface.exception import NotFittedError, NotConvergedError
@@ -52,15 +52,15 @@
             raise UnsupportedParameterError(self.metric)
 
         self.set_param_ranges(
             {"epsilon": ("0<,+inf", None), "min_points": ("0<,+inf", int)}
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "DBSCAN":
+    def fit(self, X: Matrix) -> Self:
         self._X = X
         clusters = [0] * X.shape[0]
         curPt = 0
 
         for i in range(X.shape[0]):
             if clusters[i]:
                 continue
@@ -155,15 +155,15 @@
                 "epsilon": ("0<,+inf", None),
                 "min_points": ("0<,+inf", int),
                 "threshold": ("0,+inf", None),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "OPTICS":
+    def fit(self, X: Matrix) -> Self:
         self._X = X
         m, _ = X.shape
 
         self.processed = np.full(m, False, dtype=bool)
         self.reachability = np.full(m, np.inf)
         self.ordered_points = []
 
@@ -317,15 +317,15 @@
         self._fitted = False
 
         self.set_param_ranges(
             {"max_climb": ("0<,+inf", int), "min_density": ("0,+inf", None)}
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "DENCLUE":
+    def fit(self, X: Matrix) -> Self:
         self._m, self._n = X.shape
 
         attractors: Vector = np.zeros((self._m, self._n))
         rad: Vector = np.zeros((self._m, 1))
         density: Vector = np.zeros((self._m, 1))
 
         if self.h == "auto":
@@ -473,15 +473,15 @@
         self._fitted = False
 
         self.set_param_ranges(
             {"bandwidth": ("0<,+inf", None), "max_iter": ("0<,+inf", int)}
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "MeanShiftClustering":
+    def fit(self, X: Matrix) -> Self:
         self._X = X
         m, _ = X.shape
 
         centers = np.copy(X)
         for iter in range(self.max_iter):
             new_centers = []
             for i in range(m):
```

### Comparing `luma-ml-0.6.5/luma/clustering/hierarchy.py` & `luma-ml-0.6.6/luma/clustering/hierarchy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal, Optional, Tuple
+from typing import Literal, Optional, Self, Tuple
 from scipy.spatial.distance import pdist, squareform
 from scipy.cluster.hierarchy import linkage, dendrogram
 import matplotlib.pyplot as plt
 import numpy as np
 
 from luma.interface.util import Matrix
 from luma.core.super import Estimator, Evaluator, Unsupervised
@@ -53,15 +53,15 @@
         self.linkage = linkage
         self._X = None
         self._fitted = False
 
         self.set_param_ranges({"n_clusters": ("0<,+inf", int)})
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "AgglomerativeClustering":
+    def fit(self, X: Matrix) -> Self:
         self._X = X
         n_samples = X.shape[0]
         dist_matrix = squareform(pdist(X, metric="euclidean"))
         clusters = {i: [i] for i in range(n_samples)}
 
         while len(clusters) > self.n_clusters:
             closest_pair, _ = self._find_closest_clusters(dist_matrix, clusters)
@@ -187,15 +187,15 @@
         self.clusters = []
         self._X = None
         self._fitted = False
 
         self.set_param_ranges({"n_clusters": ("0<,+inf", int)})
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "DivisiveClustering":
+    def fit(self, X: Matrix) -> Self:
         initial_cluster = [0] * X.shape[0]
         self._X = X
         self.clusters.append(initial_cluster)
         self._recursive_split(X)
 
         self._fitted = True
         return self
```

### Comparing `luma-ml-0.6.5/luma/clustering/kmeans.py` & `luma-ml-0.6.6/luma/clustering/kmeans.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Self
 import numpy as np
 
 from luma.interface.util import Matrix, Vector
 from luma.interface.exception import NotFittedError
 from luma.core.super import Estimator, Evaluator, Unsupervised
 from luma.metric.clustering import SilhouetteCoefficient
 
@@ -41,15 +42,15 @@
         self._fitted = False
 
         self.set_param_ranges(
             {"n_clusters": ("0<,+inf", int), "max_iter": ("0<,+inf", int)}
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "KMeansClustering":
+    def fit(self, X: Matrix) -> Self:
         init_indices = np.random.choice(X.shape[0], self.n_clusters, replace=False)
         self.centroids = X[init_indices]
         self._X = X
 
         for i in range(self.max_iter):
             distances = np.linalg.norm(X[:, np.newaxis] - self.centroids, axis=2)
             labels = np.argmin(distances, axis=1)
@@ -127,15 +128,15 @@
             ]
             distances = Matrix(distances)
 
             probs = distances / distances.sum()
             next_centroid = np.random.choice(X.shape[0], p=probs)
             self.centroids.append(X[next_centroid])
 
-    def fit(self, X: Matrix) -> "KMeansClusteringPlus":
+    def fit(self, X: Matrix) -> Self:
         self._X = X
         self._initialize_centroids(X)
 
         for _ in range(self.max_iter):
             distances = np.linalg.norm(X[:, np.newaxis] - self.centroids, axis=2)
             labels = np.argmin(distances, axis=1)
 
@@ -193,15 +194,15 @@
         self._fitted = False
 
         self.set_param_ranges(
             {"n_clusters": ("0<,+inf", int), "max_iter": ("0<,+inf", int)}
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "KMediansClustering":
+    def fit(self, X: Matrix) -> Self:
         self._X = X
         self.medians = X[np.random.choice(X.shape[0], self.n_clusters, replace=False)]
 
         for i in range(self.max_iter):
             distances = np.abs(X[:, np.newaxis] - self.medians)
             labels = np.argmin(distances.sum(axis=2), axis=1)
 
@@ -275,15 +276,15 @@
         self._fitted = False
 
         self.set_param_ranges(
             {"n_clusters": ("0<,+inf", int), "max_iter": ("0<,+inf", int)}
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "KMedoidsClustering":
+    def fit(self, X: Matrix) -> Self:
         self._X = X
         m, _ = X.shape
         np.random.seed(self.random_state)
         initial_indices = np.random.choice(m, self.n_clusters, replace=False)
         self.medoids = X[initial_indices]
 
         for i in range(self.max_iter):
@@ -364,15 +365,15 @@
                 "n_clusters": ("0<,+inf", int),
                 "max_iter": ("0<,+inf", int),
                 "batch_size": ("0<,+inf", int),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "MiniBatchKMeansClustering":
+    def fit(self, X: Matrix) -> Self:
         m, _ = X.shape
         self._X = X
 
         rand_idx = np.random.choice(m, self.n_clusters, replace=False)
         self.centroids = X[rand_idx]
 
         for _ in range(self.max_iter):
@@ -448,15 +449,15 @@
                 "n_clusters": ("0<,+inf", int),
                 "max_iter": ("0<,+inf", int),
                 "m": ("0,+inf", None),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "FuzzyCMeansClustering":
+    def fit(self, X: Matrix) -> Self:
         self._X = X
         m, _ = X.shape
 
         np.random.seed(self.random_state)
         self.centers = X[np.random.choice(m, self.n_clusters, replace=False)]
         self.membership = np.zeros((m, self.n_clusters))
```

### Comparing `luma-ml-0.6.5/luma/clustering/mixture.py` & `luma-ml-0.6.6/luma/clustering/mixture.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Self
 import numpy as np
 
 from luma.core.super import Estimator, Evaluator, Unsupervised
 from luma.interface.util import Matrix, Vector
 from luma.metric.clustering import SilhouetteCoefficient
 from luma.interface.exception import NotFittedError
 
@@ -47,15 +48,15 @@
             {
                 "n_clusters": ("0<,+inf", int),
                 "max_iter": ("0<,+inf", int),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "GaussianMixture":
+    def fit(self, X: Matrix) -> Self:
         self._X = X
         self._initialize_params(X)
         for i in range(self.max_iter):
             R = self._E_step(X)
             means_old = self.means.copy()
 
             self._M_step(X, R)
@@ -161,15 +162,15 @@
             {
                 "n_clusters": ("0<,+inf", int),
                 "max_iter": ("0<,+inf", int),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "MultinomialMixture":
+    def fit(self, X: Matrix) -> Self:
         self.X_ = X
         self._initialize_parameters(X)
         logL = None
 
         for i in range(self.max_iter):
             resp = self._E_step(X)
             self._M_step(X, resp)
```

### Comparing `luma-ml-0.6.5/luma/clustering/spectral.py` & `luma-ml-0.6.6/luma/clustering/spectral.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal, Optional
+from typing import Literal, Optional, Self
 from scipy.spatial.distance import pdist, squareform
 from scipy.linalg import eigh
 import matplotlib.pyplot as plt
 import numpy as np
 
 from luma.clustering.kmeans import KMeansClusteringPlus
 from luma.clustering.hierarchy import AgglomerativeClustering, DivisiveClustering
@@ -51,15 +51,15 @@
         self._fitted = False
 
         self.set_param_ranges(
             {"n_clusters": ("0<,+inf", int), "gamma": ("0<,+inf", None)}
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "SpectralClustering":
+    def fit(self, X: Matrix) -> Self:
         self._X = X
         W = self._similarity_matrix(X)
         L = self._laplacian(W)
 
         _, eigenvecs = eigh(L)
         V = eigenvecs[:, : self.n_clusters]
         kmeans = KMeansClusteringPlus(n_clusters=self.n_clusters)
@@ -122,15 +122,15 @@
         self._fitted = False
 
         self.set_param_ranges(
             {"n_clusters": ("0<,+inf", int), "gamma": ("0<,+inf", None)}
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "NormalizedSpectralClustering":
+    def fit(self, X: Matrix) -> Self:
         self._X = X
         W = self._similarity_matrix(X)
         L_norm = self._normalize_laplacian(W)
 
         _, eigvecs = eigh(L_norm)
         V = eigvecs[:, : self.n_clusters]
         kmeans = KMeansClusteringPlus(n_clusters=self.n_clusters)
@@ -209,15 +209,15 @@
         self._fitted = False
 
         self.set_param_ranges(
             {"n_clusters": ("0<,+inf", int), "gamma": ("0<,+inf", None)}
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "HierarchicalSpectralClustering":
+    def fit(self, X: Matrix) -> Self:
         self._X = X
         W = self._similarity_matrix(X)
         L = self._laplacian(W)
 
         _, eigenvecs = eigh(L)
         V = eigenvecs[:, : self.n_clusters]
 
@@ -290,15 +290,15 @@
         self._fitted = False
 
         self.set_param_ranges(
             {"max_clusters": ("0<,+inf", int), "gamma": ("0<,+inf", None)}
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "AdaptiveSpectralClustering":
+    def fit(self, X: Matrix) -> Self:
         self._X = X
         W = self._similarity_matrix(X)
         L = self._laplacian(W)
 
         eigvals, eigvecs = eigh(L)
         self.n_clusters = self._optimal_clusters(eigvals)
```

### Comparing `luma-ml-0.6.5/luma/core/base.py` & `luma-ml-0.6.6/luma/core/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,20 +52,22 @@
 
     def __dealloc__(self) -> None:
         return super().__dealloc__()
 
     def fit(self, **kwargs) -> Any:
         kwargs
 
-    def set_params(self, **kwargs) -> None:
+    def set_params(self, ignore_missing: bool = False, **kwargs) -> None:
         for key, val in kwargs.items():
             if hasattr(self, key):
                 setattr(self, key, val)
             else:
-                print(f"'{type(self).__name__}' has no attribute '{key}'")
+                if not ignore_missing:
+                    print(f"'{type(self).__name__}' has no attribute '{key}'")
+
         self.check_param_ranges()
 
     def set_param_ranges(self, range_dict: Dict[str, tuple]) -> None:
         self._param_range_dict = {
             name_: ParamRange(range_, type_)
             for name_, (range_, type_) in range_dict.items()
         }
```

### Comparing `luma-ml-0.6.5/luma/core/super.py` & `luma-ml-0.6.6/luma/core/super.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from typing import Any, Dict
-from abc import ABCMeta, abstractmethod, abstractstaticmethod
+from typing import Any, Dict, Self
+from abc import ABCMeta, abstractmethod
 
 from luma.core.base import *
 
 
 __all__ = (
     "Estimator",
     "Transformer",
@@ -27,15 +27,15 @@
     relationships within the data to make accurate predictions on new, unseen data.
 
     Methods
     -------
     For training:
     ```py
         @abstractmethod
-        def fit(self, *args) -> Estimator
+        def fit(self, *args) -> Self
     ```
 
     For prediction:
     ```py
         @abstractmethod
         def predict(self, *args) -> Vector
     ```
@@ -82,24 +82,24 @@
           integrating `TimeSeries` models with `Meta` estimators,
           special consideration is needed to ensure compatibility and
           effective integration.
 
         """
 
     @abstractmethod
-    def fit(self, *args) -> "Estimator": ...
+    def fit(self, *args) -> Self: ...
 
     @abstractmethod
     def predict(self, *args) -> Any: ...
 
     @abstractmethod
     def score(self, *args) -> float: ...
 
-    def set_params(self, **kwargs) -> None:
-        return super().set_params(**kwargs)
+    def set_params(self, ignore_missing: bool = False, **kwargs) -> None:
+        return super().set_params(ignore_missing=ignore_missing, **kwargs)
 
     def set_param_ranges(self, range_dict: Dict[str, tuple]) -> None:
         return super().set_param_ranges(range_dict)
 
     def check_param_ranges(self) -> None:
         return super().check_param_ranges()
 
@@ -116,15 +116,15 @@
     or noise.
 
     Methods
     -------
     For fitting:
     ```py
         @abstractmethod
-        def fit(self, *args) -> Transformer
+        def fit(self, *args) -> Self
     ```
 
     For transformation:
     ```py
         @abstractmethod
         def transform(self, *args) -> Matrix
     ```
@@ -195,24 +195,24 @@
 
             ```py
             def transform(self, X: Matrix, y: Vector) -> Tuple[Matrix, Matrix | Vector]
             ```
         """
 
     @abstractmethod
-    def fit(self, *args) -> "Transformer": ...
+    def fit(self, *args) -> Self: ...
 
     @abstractmethod
     def transform(self, *args) -> Any: ...
 
     @abstractmethod
     def fit_transform(self, *args) -> Any: ...
 
-    def set_params(self, **kwargs) -> None:
-        return super().set_params(**kwargs)
+    def set_params(self, ignore_missing: bool = False, **kwargs) -> None:
+        return super().set_params(ignore_missing=ignore_missing, **kwargs)
 
     def set_param_ranges(self, range_dict: Dict[str, tuple]) -> None:
         return super().set_param_ranges(range_dict)
 
     def check_param_ranges(self) -> None:
         return super().check_param_ranges()
 
@@ -232,17 +232,33 @@
     Get the best(optimized) estimator or transformer:
     ```py
         @property
         def best_model(self) -> Estimator | Transformer
 
     """
 
+    class Neural:
+        """
+        An inner class of `Optimizer` dedicated to neural optimizing techniques.
+
+        Methods
+        -------
+        For updating weights:
+        ```py
+        @abstractmethod
+        def update(self, **kwargs) -> tuple
+        ```
+        """
+
+        @abstractmethod
+        def update(self, **kwargs) -> tuple: ...
+
     @property
     def best_model(self) -> Estimator | Transformer: ...
-    
+
     def fit(self, **kwargs) -> Any:
         return super().fit(**kwargs)
 
     def set_params(self, **kwargs) -> None:
         return super().set_params(**kwargs)
 
     def set_param_ranges(self, range_dict: Dict[str, tuple]) -> None:
@@ -259,20 +275,22 @@
     how well a model is performing on a particular task,
     such as classification or regression.
 
     Methods
     -------
     For scoring:
     ```py
-        @abstractstaticmethod
+        @staticmethod
+        @abstractmethod
         def score(*args) -> float
     ```
     """
 
-    @abstractstaticmethod
+    @staticmethod
+    @abstractmethod
     def score(*args) -> float: ...
 
 
 class Visualizer(VisualBase, metaclass=ABCMeta):
     """
     A visualizer is a tool that helps visualize and understand various aspects
     of machine learning models, datasets, and the results the analysis.
@@ -333,14 +351,16 @@
     or "difference" there is between two points, objects, or distributions. Different
     types of distances serve various purposes, and they are used in different contexts.
 
     Methods
     -------
     For computing the distance:
     ```py
-        @abstractstaticmethod
+        @staticmethod
+        @abstractmethod
         def compute(*args) -> float
     ```
     """
 
-    @abstractstaticmethod
+    @staticmethod
+    @abstractmethod
     def compute(*args) -> float: ...
```

### Comparing `luma-ml-0.6.5/luma/ensemble/bagging.py` & `luma-ml-0.6.6/luma/ensemble/bagging.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict
+from typing import Any, Dict, Self
 import numpy as np
 
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.interface.util import Matrix, Vector, Clone
 from luma.interface.exception import NotFittedError
 from luma.classifier.tree import DecisionTreeClassifier
 from luma.regressor.tree import DecisionTreeRegressor
@@ -72,15 +72,15 @@
         self.verbose = verbose
         self._base_estimator_params = kwargs
         self._fitted = False
 
         self.set_param_ranges({"n_estimators": ("0<,+inf", int)})
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, y: Vector) -> "BaggingClassifier":
+    def fit(self, X: Matrix, y: Vector) -> Self:
         np.random.seed(self.random_state)
         self.base_estimator.set_params(**self._base_estimator_params)
         self.estimators_ = []
 
         m, n = X.shape
         if self.max_samples <= 1.0:
             max_samples = int(m * self.max_samples)
@@ -198,15 +198,15 @@
         self.verbose = verbose
         self._base_estimator_params = kwargs
         self._fitted = False
 
         self.set_param_ranges({"n_estimators": ("0<,+inf", int)})
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, y: Vector) -> "BaggingRegressor":
+    def fit(self, X: Matrix, y: Vector) -> Self:
         np.random.seed(self.random_state)
         self.base_estimator.set_params(**self._base_estimator_params)
         self.estimators_ = []
 
         m, n = X.shape
         if self.max_samples <= 1.0:
             max_samples = int(m * self.max_samples)
```

### Comparing `luma-ml-0.6.5/luma/ensemble/boost.py` & `luma-ml-0.6.6/luma/ensemble/boost.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List, Literal, Tuple
+from typing import Any, Dict, List, Literal, Self, Tuple
 from scipy.special import softmax
 import numpy as np
 
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.interface.util import Matrix, Vector, Clone
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.classifier.tree import DecisionTreeClassifier
@@ -70,15 +70,15 @@
         self._fitted = False
 
         self.set_param_ranges(
             {"n_estimators": ("0<,+inf", int), "learning_rate": ("0<,+inf", None)}
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, y: Matrix) -> "AdaBoostClassifier":
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         self.classes_ = np.unique(y)
 
         m, _ = X.shape
         n_classes = len(self.classes_)
         sample_weights = np.ones(m)
 
         lb = LabelBinarizer().fit(self.classes_)
@@ -198,15 +198,15 @@
         self._fitted = False
 
         self.set_param_ranges(
             {"n_estimators": ("0<,+inf", int), "learning_rate": ("0<,+inf", None)}
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, y: Vector) -> "AdaBoostRegressor":
+    def fit(self, X: Matrix, y: Vector) -> Self:
         m, _ = X.shape
         sample_weights = np.ones(m)
 
         for i in range(self.n_estimators):
             est = Clone(self.base_estimator).get
             if hasattr(est, "max_depth"):
                 est.max_depth = 3
@@ -340,15 +340,15 @@
                 "n_estimators": ("0<,+inf", int),
                 "learning_rate": ("0<,+inf", None),
                 "subsample": ("0,1", None),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, y: Vector) -> "GradientBoostingClassifier":
+    def fit(self, X: Matrix, y: Vector) -> Self:
         self._initialize(y)
         m, _ = X.shape
         Fm = np.zeros((m, self.n_classes_)) + self.initial_preds_
 
         for cl in range(self.n_classes_):
             y_c = (y == self.classes_[cl]).astype(float)
             for i in range(self.n_estimators):
@@ -466,15 +466,15 @@
                 "learning_rate": ("0<,+inf", None),
                 "subsample": ("0,1", None),
                 "delta": ("0,1", None),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, y: Vector) -> "GradientBoostingRegressor":
+    def fit(self, X: Matrix, y: Vector) -> Self:
         self.init_pred_ = self._initial_prediction(y)
         self.estimators_ = []
         m, _ = X.shape
         Fm = np.mean(y)
 
         for i in range(self.n_estimators):
             residuals = self._loss_derivative(y, Fm)
```

### Comparing `luma-ml-0.6.5/luma/ensemble/forest.py` & `luma-ml-0.6.6/luma/ensemble/forest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal
+from typing import Literal, Self
 from scipy.stats import mode
 import numpy as np
 
 from luma.interface.util import Matrix, Vector
 from luma.classifier.tree import DecisionTreeClassifier
 from luma.regressor.tree import DecisionTreeRegressor
 from luma.core.super import Estimator, Evaluator, Supervised
@@ -74,17 +74,15 @@
                 "min_samples_split": ("0<,+inf", int),
                 "max_samples_leaf": ("0<,+inf", int),
                 "min_impurity_decrease": ("0,+inf", None),
             }
         )
         self.check_param_ranges()
 
-    def fit(
-        self, X: Matrix, y: Matrix, sample_weights: Vector = None
-    ) -> "RandomForestClassifier":
+    def fit(self, X: Matrix, y: Matrix, sample_weights: Vector = None) -> Self:
         m, n = X.shape
         if self.n_features == "auto":
             self.n_features = int(n**0.5)
         else:
             if isinstance(self.n_features, str):
                 raise UnsupportedParameterError(self.n_features)
 
@@ -193,15 +191,15 @@
                 "min_samples_split": ("0<,+inf", int),
                 "max_samples_leaf": ("0<,+inf", int),
                 "min_variance_decrease": ("0,+inf", None),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, y: Matrix) -> "RandomForestRegressor":
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         m, n = X.shape
         if self.n_features == "auto":
             self.n_features = int(n**0.5)
         else:
             if isinstance(self.n_features, str):
                 raise UnsupportedParameterError(self.n_features)
```

### Comparing `luma-ml-0.6.5/luma/ensemble/stack.py` & `luma-ml-0.6.6/luma/ensemble/stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, List, Dict, Literal
+from typing import Any, List, Dict, Literal, Self
 import numpy as np
 
 from luma.core.super import Estimator, Transformer, Evaluator, Supervised
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.interface.util import Matrix, Vector
 from luma.classifier.logistic import SoftmaxRegressor
 from luma.regressor.linear import LinearRegressor
@@ -100,15 +100,15 @@
 
         if self.method not in ("label", "prob"):
             raise UnsupportedParameterError(self.method)
 
         self.set_param_ranges({"cv": ("0,+inf", int)})
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, y: Vector) -> "StackingClassifier":
+    def fit(self, X: Matrix, y: Vector) -> Self:
         m, _ = X.shape
         self.n_classes = len(np.unique(y))
 
         fold = self.fold_type(
             X, y, n_folds=self.cv, shuffle=self.shuffle, random_state=self.random_state
         )
 
@@ -309,15 +309,15 @@
         self._final_estimator_params = kwargs
         self._base_estimators: List[Estimator] = []
         self._fitted = False
 
         self.set_param_ranges({"cv": ("0,+inf", int)})
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, y: Vector) -> "StackingClassifier":
+    def fit(self, X: Matrix, y: Vector) -> Self:
         m, _ = X.shape
         self.n_classes = len(np.unique(y))
 
         fold = self.fold_type(
             X, y, n_folds=self.cv, shuffle=self.shuffle, random_state=self.random_state
         )
```

### Comparing `luma-ml-0.6.5/luma/ensemble/vote.py` & `luma-ml-0.6.6/luma/ensemble/vote.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Literal
+from typing import List, Literal, Self
 import numpy as np
 
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.interface.util import Matrix, Vector, Scalar, Clone
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.metric.classification import Accuracy
 from luma.metric.regression import MeanSquaredError
@@ -51,15 +51,15 @@
     ) -> None:
         self.estimators = estimators
         self.voting = voting
         self.weights = weights
         self.verbose = verbose
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Vector) -> "VotingClassifier":
+    def fit(self, X: Matrix, y: Vector) -> Self:
         if self.voting not in ("label", "prob"):
             raise UnsupportedParameterError(self.voting)
 
         if self.weights and len(self.weights) != len(self.estimators):
             raise ValueError(f"Size mismatch between 'weights' and 'estimators'!")
 
         self.le = LabelEncoder()
@@ -146,15 +146,15 @@
         verbose: bool = False,
     ) -> None:
         self.estimators = estimators
         self.weights = weights
         self.verbose = verbose
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Vector) -> "VotingRegressor":
+    def fit(self, X: Matrix, y: Vector) -> Self:
         if self.weights and len(self.weights) != len(self.estimators):
             raise ValueError(f"Size mismatch between 'weights' and 'estimators'!")
 
         self.estimators_ = []
         for est in self.estimators:
             fitted_est = Clone(est).get
             if hasattr(fitted_est, "verbose"):
```

### Comparing `luma-ml-0.6.5/luma/interface/exception.py` & `luma-ml-0.6.6/luma/interface/exception.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.5/luma/interface/util.py` & `luma-ml-0.6.6/luma/interface/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -454,19 +454,17 @@
     Notes
     -----
     - When setting a custom range for `param_range`, it must follow the form of
         "lower_bound,upper_bound". (i.e. `-inf,20`, `-5,5`)
     - For open intervals, add '<' inside the range. (i.e. `0<,+inf`, `0<,<10`)
     """
 
-    Ranges = Literal["-inf,+inf", "-inf,0", "-1,0", "-1,1", "0,1", "0,+inf"]
+    type RangeStr = AnyStr
 
-    def __init__(
-        self, param_range: Ranges | AnyStr, param_type: Type[Scalar] = None
-    ) -> None:
+    def __init__(self, param_range: RangeStr, param_type: Type[Scalar] = None) -> None:
         self.param_range = param_range
 
         if param_type is None:
             self.param_type = int | float
         else:
             if not ParamRange.validate_type(param_type):
                 raise UnsupportedParameterError(param_type)
```

### Comparing `luma-ml-0.6.5/luma/metric/classification.py` & `luma-ml-0.6.6/luma/metric/classification.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.5/luma/metric/clustering.py` & `luma-ml-0.6.6/luma/metric/clustering.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.5/luma/metric/distance.py` & `luma-ml-0.6.6/luma/metric/distance.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.5/luma/metric/regression.py` & `luma-ml-0.6.6/luma/metric/regression.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.5/luma/migrate/port.py` & `luma-ml-0.6.6/luma/migrate/port.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.6.5/luma/model_selection/cv.py` & `luma-ml-0.6.6/luma/model_selection/cv.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,17 +58,14 @@
         self.fold_type = fold_type
         self.shuffle = shuffle
         self.random_state = random_state
         self.verbose = verbose
         self.train_scores_ = []
         self.test_scores_ = []
 
-        self.set_param_ranges({"cv": ("0,+inf", int)})
-        self.check_param_ranges()
-
     def _fit(self, X: Matrix, y: Vector) -> None:
         fold = self.fold_type(
             X, y, n_folds=self.cv, shuffle=self.shuffle, random_state=self.random_state
         )
 
         for i, (train_indices, test_indices) in enumerate(fold.split):
             X_train, y_train = X[train_indices], y[train_indices]
```

### Comparing `luma-ml-0.6.5/luma/model_selection/fold.py` & `luma-ml-0.6.6/luma/model_selection/fold.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,17 +65,14 @@
     ) -> None:
         self.X = X
         self.y = y
         self.shuffle = shuffle
         self.random_state = random_state
         self.n_folds = n_folds
 
-        self.set_param_ranges({"n_folds": ("0,+inf", int)})
-        self.check_param_ranges()
-
     @property
     def split(self) -> Generator[Tuple[Vector, Vector], None, None]:
         np.random.seed(self.random_state)
         m, _ = self.X.shape
         fold_size = m // self.n_folds
 
         indices = np.arange(m)
@@ -144,17 +141,14 @@
     ) -> None:
         self.X = X
         self.y = y
         self.n_folds = n_folds
         self.shuffle = shuffle
         self.random_state = random_state
 
-        self.set_param_ranges({"n_folds": ("0,+inf", int)})
-        self.check_param_ranges()
-
     @property
     def split(self) -> Generator[Tuple[Vector, Vector], None, None]:
         np.random.seed(self.random_state)
 
         indices_per_class = defaultdict(list)
         for idx, class_ in enumerate(self.y):
             indices_per_class[class_].append(idx)
@@ -238,17 +232,14 @@
         self.X = X
         self.y = y
         self.groups = groups
         self.n_folds = n_folds
         self.shuffle = shuffle
         self.random_state = random_state
 
-        self.set_param_ranges({"n_folds": ("0,+inf", int)})
-        self.check_param_ranges()
-
     @property
     def split(self) -> Generator[Tuple[Vector, Vector], None, None]:
         np.random.seed(self.random_state)
         _, groups_indices = np.unique(self.groups, return_inverse=True)
 
         group_counts = Counter(groups_indices)
         group_indices = defaultdict(list)
```

### Comparing `luma-ml-0.6.5/luma/model_selection/search.py` & `luma-ml-0.6.6/luma/model_selection/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,16 @@
                     k: f"{v:.4f}" if isinstance(v, float) else v
                     for k, v in params.items()
                 }
                 print(
                     f"[GridSearchCV] candidate {i}/{max_iter} {params_f}",
                     f"- score:{mean_score:.3f}",
                 )
+            if np.isnan(mean_score):
+                continue
 
             if self.maximize:
                 if best_score is None or mean_score > best_score:
                     best_score = mean_score
                     best_params = params
             else:
                 if best_score is None or mean_score < best_score:
@@ -298,14 +300,16 @@
                     k: f"{v:.4f}" if isinstance(v, float) else v
                     for k, v in params.items()
                 }
                 print(
                     f"[RandomSearchCV] candidate {i + 1}/{self.max_iter}",
                     f"{params_f} - score: {mean_score:.3f}",
                 )
+            if np.isnan(mean_score):
+                continue
 
             if self.maximize:
                 if best_score is None or mean_score > best_score:
                     best_score = mean_score
                     best_params = params
             else:
                 if best_score is None or mean_score < best_score:
```

### Comparing `luma-ml-0.6.5/luma/model_selection/split.py` & `luma-ml-0.6.6/luma/model_selection/split.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,17 +43,14 @@
         self.X = X
         self.y = y
         self.test_size = test_size
         self.shuffle = shuffle
         self.stratify = stratify
         self.random_state = random_state
 
-        self.set_param_ranges({"test_size": ("0<,+inf", int)})
-        self.check_param_ranges()
-
     @property
     def get(self) -> Tuple[Matrix, Matrix, Vector, Vector]:
         if self.X.shape[0] != self.y.shape[0]:
             raise ValueError("Sample size mismatch between 'X' and 'y'!")
 
         if self.stratify:
             return self._stratified_split()
```

### Comparing `luma-ml-0.6.5/luma/neural/activation.py` & `luma-ml-0.6.6/luma/neural/activation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 import numpy as np
 
 
 __all__ = ("ReLU", "LeakyReLU", "ELU", "Tanh", "Sigmoid", "Softmax")
 
 
-class _Matrix:
-    pass
-
-
-Matrix = _Matrix
+type Matrix = np.ndarray
 
 
 class ReLU:
     def func(self, X: Matrix) -> Matrix:
         return np.maximum(0, X)
 
     def derivative(self, X: Matrix) -> Matrix:
```

### Comparing `luma-ml-0.6.5/luma/neural/single.py` & `luma-ml-0.6.6/luma/neural/single.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal
+from typing import Literal, Self
 import numpy as np
 
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.interface.util import Matrix, Vector
 from luma.preprocessing.encoder import LabelBinarizer
 from luma.metric.classification import Accuracy
@@ -60,15 +60,15 @@
                 "max_iter": ("0<,+inf", int),
                 "alpha": ("0,+inf", None),
                 "l1_ratio": ("0,1", None),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, y: Vector) -> "PerceptronClassifier":
+    def fit(self, X: Matrix, y: Vector) -> Self:
         m, n = X.shape
         np.random.seed(self.random_state)
         n_classes = len(np.unique(y))
 
         X = self._add_bias(X)
         y_binary = LabelBinarizer().fit_transform(y)
         self.weights_ = np.random.uniform(-0.01, 0.01, (n_classes, n + 1))
@@ -173,15 +173,15 @@
                 "max_iter": ("0<,+inf", int),
                 "alpha": ("0,+inf", None),
                 "l1_ratio": ("0,1", None),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, y: Vector) -> "PerceptronRegressor":
+    def fit(self, X: Matrix, y: Vector) -> Self:
         m, n = X.shape
         np.random.seed(self.random_state)
 
         X = self._add_bias(X)
         self.weights_ = np.random.uniform(-0.01, 0.01, n + 1)
 
         for i in range(self.max_iter):
```

### Comparing `luma-ml-0.6.5/luma/pipe/pipeline.py` & `luma-ml-0.6.6/luma/pipe/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from typing import Dict, Literal, Tuple, List, TypeVar, Any
+from typing import Dict, Literal, Self, Tuple, List, Any
 
 from luma.core.super import Estimator, Transformer, Evaluator
 from luma.core.super import Supervised
 from luma.interface.util import Matrix
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.metric.classification import Accuracy
 from luma.metric.regression import MeanSquaredError
 
-MT = TypeVar("MT", bound=Estimator | Transformer)
+type Model = Estimator | Transformer
 
 
 __all__ = "Pipeline"
 
 
-class Pipeline(Estimator, Estimator.Meta):
+class Pipeline(Estimator, Estimator.Meta, Transformer):
     """
     A pipeline is a sequence of steps to process data and build a model.
     It includes data collection and preprocessing, model selection and training,
     evaluation, and deployment. This systematic approach ensures efficiency
     and accuracy in model development. Pipelines are often automated for
     scalability and reproducibility in real-world applications.
 
@@ -76,25 +76,24 @@
     -----
     * To use `Pipeline` with visual methods of `luma.visual`, make sure to
     transform data using `pipe.transform()` if the pipeline sequence contains
     transformers
 
     * More than one estimator might cause procedural failure
     * Not all the models are compatible with `Pipeline`
-    * Type `MT` is a generic type for `Estimator` and `Transformer`
 
     """
 
     def __init__(
         self,
-        models: List[Tuple[str, MT]] | List[MT],
+        models: List[Tuple[str, Model]] | List[Model],
         param_dict: Dict[str, Any] = dict(),
         verbose: bool = False,
     ) -> None:
-        self.models: Dict[MT] = dict()
+        self.models: Dict[Model] = dict()
         self.param_dict = param_dict
         self.verbose = verbose
         self._X: Matrix
         self._y: Matrix
         self._fitted = False
 
         for model in models:
@@ -102,15 +101,15 @@
                 _name, _model = model
                 self.models[_name] = _model
             else:
                 self.models[type(model).__name__] = model
 
         self.set_params(param_dict)
 
-    def fit(self, X: Matrix, y: Matrix) -> "Pipeline":
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         self._X, self._y = self.fit_transform(X, y)
         model = self.estimator
         if hasattr(model, "verbose"):
             model.verbose = self.verbose
 
         data = [self._X]
         if isinstance(model, Supervised):
@@ -213,16 +212,16 @@
             if isinstance(model, Estimator):
                 return model
 
     @property
     def transformed_data(self) -> Tuple[Matrix, Matrix]:
         return self._X, self._y
 
-    def __getitem__(self, index: int) -> MT:
+    def __getitem__(self, index: int) -> Model:
         for i, model in enumerate(self.models.values()):
             if index == i:
                 return model
         else:
             raise IndexError("Model index out of bounds!")
 
-    def __setitem__(self, label: str, model: MT):
+    def __setitem__(self, label: str, model: Model):
         self.models[label] = model
```

### Comparing `luma-ml-0.6.5/luma/preprocessing/encoder.py` & `luma-ml-0.6.6/luma/preprocessing/encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal
+from typing import Literal, Self
 import numpy as np
 
 from luma.core.super import Transformer
 from luma.interface.util import Matrix, Vector
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 
 
@@ -11,15 +11,15 @@
 
 class OneHotEncoder(Transformer, Transformer.Feature):
     def __init__(self, features: list = None):
         self.categories = None
         self.features = features
         self._fitted = False
 
-    def fit(self, X: Matrix) -> "OneHotEncoder":
+    def fit(self, X: Matrix) -> Self:
         if self.features is None:
             self.features = range(X.shape[1])
 
         self.categories = [np.unique(X[:, col]) for col in self.features]
         self._fitted = True
         return self
 
@@ -54,15 +54,15 @@
 
 
 class LabelEncoder(Transformer, Transformer.Target):
     def __init__(self):
         self.classes = None
         self._fitted = False
 
-    def fit(self, y: Matrix) -> "LabelEncoder":
+    def fit(self, y: Matrix) -> Self:
         self.classes = np.unique(y)
         self._fitted = True
         return self
 
     def transform(self, y: Matrix) -> Matrix[int]:
         if not self._fitted:
             raise NotFittedError(self)
@@ -92,15 +92,15 @@
 
 class OrdinalEncoder(Transformer, Transformer.Feature):
     def __init__(self, strategy: Literal["occur", "alpha"] = "occur"):
         self.categories = None
         self.strategy = strategy
         self._fitted = False
 
-    def fit(self, X: Matrix) -> "OrdinalEncoder":
+    def fit(self, X: Matrix) -> Self:
         if self.strategy == "occur":
             self.categories = [np.unique(col, return_index=True)[0] for col in X.T]
         elif self.strategy == "alpha":
             self.categories = [np.sort(np.unique(col)) for col in X.T]
         else:
             raise UnsupportedParameterError(self.strategy)
 
@@ -131,15 +131,15 @@
 
 class LabelBinarizer(Transformer, Transformer.Target):
     def __init__(self, negative_target: bool = False) -> None:
         self.negative_target = negative_target
         self.classes_ = None
         self._fitted = False
 
-    def fit(self, y: Vector) -> "LabelBinarizer":
+    def fit(self, y: Vector) -> Self:
         self.classes_ = np.unique(y)
         self._fitted = True
         return self
 
     def transform(self, y: Vector) -> Vector:
         if not self._fitted:
             raise NotFittedError(self)
```

### Comparing `luma-ml-0.6.5/luma/preprocessing/imputer.py` & `luma-ml-0.6.6/luma/preprocessing/imputer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal
+from typing import Literal, Self
 from scipy.spatial.distance import cdist
 from scipy.stats import mode
 import numpy as np
 import pandas as pd
 
 from luma.interface.util import Matrix
 from luma.core.super import Transformer
@@ -14,15 +14,15 @@
 
 class SimpleImputer(Transformer, Transformer.Feature):
     def __init__(self, strategy: Literal["mean", "median", "mode"] = "mean"):
         self.strategy = strategy
         self.statistics = None
         self._fitted = False
 
-    def fit(self, X: Matrix) -> "SimpleImputer":
+    def fit(self, X: Matrix) -> Self:
         if self.strategy == "mean":
             self.statistics = np.nanmean(X, axis=0)
         elif self.strategy == "median":
             self.statistics = np.nanmedian(X, axis=0)
         elif self.strategy == "mode":
             self.statistics = []
 
@@ -79,15 +79,15 @@
         self.n_neighbors = n_neighbors
         self.distances = None
         self._fitted = False
 
         self.set_param_ranges({"n_neighbors": ("0<,+inf", int)})
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "KNNImputer":
+    def fit(self, X: Matrix) -> Self:
         if np.isnan(X).any():
             self.distances = self._compute_distances(X)
 
         self._fitted = True
         return self
 
     def transform(self, X: Matrix) -> Matrix:
@@ -128,15 +128,15 @@
 
 class HotDeckImputer(Transformer, Transformer.Feature):
     def __init__(self):
         self._X = None
         self._similar_rows = None
         self._fitted = False
 
-    def fit(self, X: Matrix) -> "HotDeckImputer":
+    def fit(self, X: Matrix) -> Self:
         self._X = X
         self._similar_rows = [self._find_similar_row(row) for row in self._X]
 
         self._fitted = True
         return self
 
     def _find_similar_row(self, row: Matrix) -> Matrix:
```

### Comparing `luma-ml-0.6.5/luma/preprocessing/outlier.py` & `luma-ml-0.6.6/luma/preprocessing/outlier.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,32 @@
-from typing import Tuple
+from typing import Self, Tuple
 from scipy.spatial.distance import cdist
 import numpy as np
 
-from luma.core.super import Transformer, Supervised
+from luma.core.super import Transformer
 from luma.interface.util import Matrix, Vector
 from luma.interface.exception import NotFittedError
 
 
 __all__ = "LocalOutlierFactor"
 
 
-class LocalOutlierFactor(Transformer, Transformer.Both, Supervised):
+class LocalOutlierFactor(Transformer, Transformer.Both):
     """
     The Local Outlier Factor (LOF) algorithm identifies outliers by comparing
     the local density of a data point with the densities of its neighbors.
     Points with significantly lower density than their neighbors are considered
     outliers. LOF scores greater than 1 indicate potential outliers. It is
     effective in datasets with varying densities and does not require a prior
     assumption about the data distribution.
 
     Parameters
     ----------
     `n_neighbors` : Number of neighbors to estimate the local densities
+    `threshold` : Cutoff value deciding whether a point is considered an outlier
 
     Examples
     --------
     >>> lof = LocalOutlierFactor()
     >>> lof.fit(X)
 
     Getting LOF Scores
@@ -44,15 +45,15 @@
         self._fitted = False
 
         self.set_param_ranges(
             {"n_neighbors": ("0<,+inf", int), "threshold": ("0,+inf", None)}
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, _=None) -> "LocalOutlierFactor":
+    def fit(self, X: Matrix, _=None) -> Self:
         n_samples = len(X)
         self.lrd_ = np.zeros(n_samples)
         self.neighbors_ = []
 
         for i in range(n_samples):
             distances = cdist([X[i]], X)[0]
             neighbors_idx = np.argsort(distances)[1 : self.n_neighbors + 1]
```

### Comparing `luma-ml-0.6.5/luma/preprocessing/scaler.py` & `luma-ml-0.6.6/luma/preprocessing/scaler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Self
 import numpy as np
 
 from luma.interface.util import Matrix
 from luma.core.super import Transformer
 from luma.interface.exception import NotFittedError
 
 
@@ -15,15 +16,15 @@
     """
 
     def __init__(self) -> None:
         self.mean = None
         self.std = None
         self._fitted = False
 
-    def fit(self, X: Matrix) -> "StandardScaler":
+    def fit(self, X: Matrix) -> Self:
         self.mean = np.mean(X, axis=0)
         self.std = np.std(X, axis=0, ddof=1)
         self._fitted = True
         return self
 
     def transform(self, X: Matrix) -> Matrix:
         if not self._fitted:
@@ -56,15 +57,15 @@
 
     def __init__(self, feature_range: tuple = (0, 1)) -> None:
         self.feature_range = feature_range
         self.min = None
         self.max = None
         self._fitted = False
 
-    def fit(self, X: Matrix) -> "MinMaxScaler":
+    def fit(self, X: Matrix) -> Self:
         self.min = np.min(X, axis=0)
         self.max = np.max(X, axis=0)
         self._fitted = True
         return self
 
     def transform(self, X: Matrix) -> Matrix:
         if not self._fitted:
```

### Comparing `luma-ml-0.6.5/luma/reduction/linear.py` & `luma-ml-0.6.6/luma/reduction/linear.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple
+from typing import Self, Tuple
 from scipy.linalg import svd, eigh
 import numpy as np
 
 from luma.interface.util import Matrix, Vector, KernelUtil
 from luma.core.super import Transformer, Unsupervised, Supervised
 from luma.interface.exception import (
     NotFittedError,
@@ -29,15 +29,15 @@
     def __init__(self, n_components: int = None) -> None:
         self.n_components = n_components
         self._fitted = False
 
         self.set_param_ranges({"n_components": ("0<,+inf", int)})
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "PCA":
+    def fit(self, X: Matrix) -> Self:
         self.mean = np.mean(X, axis=0)
         X_centered = X - self.mean
         covariance_matrix = np.cov(X_centered, rowvar=False)
         eigenvalues, eigenvectors = np.linalg.eigh(covariance_matrix)
 
         sorted_indices = np.argsort(eigenvalues)[::-1]
         eigenvalues = eigenvalues[sorted_indices]
@@ -104,15 +104,15 @@
                 "n_components": ("0<,+inf", int),
                 "deg": ("0,+inf", int),
                 "gamma": ("0<,+inf", None),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "KernelPCA":
+    def fit(self, X: Matrix) -> Self:
         self.X = X
         self._select_kernel_function()
         N = X.shape[0]
         self.K = self._compute_kernel_matrix(X, X)
 
         one_n = np.ones((N, N)) / N
         self.K_centered = self.K - one_n.dot(self.K) - self.K.dot(one_n)
@@ -203,15 +203,15 @@
     def __init__(self, n_components: int = None) -> None:
         self.n_components = n_components
         self._fitted = False
 
         self.set_param_ranges({"n_components": ("0<,+inf", int)})
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, y: Matrix) -> "LDA":
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         self.classes = np.unique(y)
         self.class_means = [np.mean(X[y == c], axis=0) for c in self.classes]
 
         within_class_scatter = np.zeros((X.shape[1], X.shape[1]))
         for c in self.classes:
             X_c = X[y == c]
             mean_diff = X_c - self.class_means[c]
@@ -268,15 +268,15 @@
     def __init__(self, n_components: int = None) -> None:
         self.n_components = n_components
         self._fitted = False
 
         self.set_param_ranges({"n_components": ("0<,+inf", int)})
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "TruncatedSVD":
+    def fit(self, X: Matrix) -> Self:
         mean = np.mean(X, axis=0)
         X_centered = X - mean
         U, S, VT = np.linalg.svd(X_centered, full_matrices=False)
 
         self.U = U[:, : self.n_components]
         self.S = np.diag(S[: self.n_components])
         self.VT = VT[: self.n_components, :]
@@ -328,15 +328,15 @@
         self._fitted = False
 
         self.set_param_ranges(
             {"n_components": ("0<,+inf", int), "max_iter": ("0<,+inf", int)}
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "FactorAnalysis":
+    def fit(self, X: Matrix) -> Self:
         m, n = X.shape
         self.mean = X.mean(axis=0)
         X -= self.mean
 
         logL_const = n * np.log(2 * np.pi) * self.n_components
         variance = X.var(axis=0)
         psi = np.ones(n)
@@ -449,15 +449,15 @@
                 "n_components": ("0<,+inf", int),
                 "deg": ("0,+inf", int),
                 "gamma": ("0<,+inf", None),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, y: Vector) -> "KDA":
+    def fit(self, X: Matrix, y: Vector) -> Self:
         m, _ = X.shape
         self.X_ = X
         self.classes = np.unique(y)
         self.ku_ = KernelUtil(self.kernel, **self.kernel_params)
 
         K = self.ku_.kernel_func(X)
         M = np.mean(K, axis=0)
@@ -519,15 +519,15 @@
         self.n_components = n_components
         self.correlations_ = None
         self._fitted = False
 
         self.set_param_ranges({"n_components": ("0<,+inf", int)})
         self.check_param_ranges()
 
-    def fit(self, X: Matrix, Y: Matrix) -> "CCA":
+    def fit(self, X: Matrix, Y: Matrix) -> Self:
         _, n = X.shape
         X -= X.mean(axis=0)
         Y -= Y.mean(axis=0)
 
         Cxx = np.cov(X.T)
         Cyy = np.cov(Y.T)
         Cxy = np.cov(X.T, Y.T)[:n, n:]
```

### Comparing `luma-ml-0.6.5/luma/reduction/manifold.py` & `luma-ml-0.6.6/luma/reduction/manifold.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Callable, Literal
+from typing import Any, Callable, Literal, Self
 
 from scipy.spatial.distance import pdist, cdist, squareform
 from scipy.sparse.csgraph import shortest_path
 from scipy.spatial import KDTree
 from scipy.linalg import eigh, svd
 import numpy as np
 
@@ -67,15 +67,15 @@
                 "max_iter": ("0<,+inf", int),
                 "learning_rate": ("0<,+inf", int),
                 "perplexity": ("0<,+inf", int),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "TSNE":
+    def fit(self, X: Matrix) -> Self:
         size = X.shape[0]
         P = self._P_joint_probabilities(X)
         y = np.random.normal(0.0, 1e-4, (size, self.n_components))
         Y = [y, y]
 
         for i in range(1, self.max_iter + 1):
             Q = self._Q_joint_probabilities(Y[-1])
@@ -200,15 +200,15 @@
     def __init__(self, n_components: int = None) -> None:
         self.n_components = n_components
         self._fitted = False
 
         self.set_param_ranges({"n_components": ("0<,+inf", int)})
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "MDS":
+    def fit(self, X: Matrix) -> Self:
         D = self._compute_dissimilarity(X)
         n = D.shape[0]
         H = np.eye(n) - np.ones((n, n)) / n
         B = -0.5 * H.dot(D).dot(H)
 
         eigvals, eigvecs = np.linalg.eigh(B)
         sorted_indices = np.argsort(eigvals)[::-1]
@@ -279,15 +279,15 @@
         self._fitted = False
 
         self.set_param_ranges(
             {"n_components": ("0<,+inf", int), "p": ("0<,+inf", None)}
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "MetricMDS":
+    def fit(self, X: Matrix) -> Self:
         D = self._compute_dissimilarity(X)
         n = D.shape[0]
         H = np.eye(n) - np.ones((n, n)) / n
         B = -0.5 * H.dot(D).dot(H)
 
         eigvals, eigvecs = np.linalg.eigh(B)
         sorted_indices = np.argsort(eigvals)[::-1]
@@ -376,15 +376,15 @@
         self._fitted = False
 
         self.set_param_ranges(
             {"n_components": ("0<,+inf", int), "n_landmarks": ("0<,+inf", int)}
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "LandmarkMDS":
+    def fit(self, X: Matrix) -> Self:
         self.landmarks = self._initialize_landmarks(X)
         D = self._compute_dissimilarity(self.landmarks)
         n = D.shape[0]
         H = np.eye(n) - np.ones((n, n)) / n
         B = -0.5 * H.dot(D).dot(H)
 
         eigvals, eigvecs = np.linalg.eigh(B)
@@ -475,15 +475,15 @@
         self._fitted = False
 
         self.set_param_ranges(
             {"n_components": ("0<,+inf", int), "n_neighbors": ("0<,+inf", int)}
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "LLE":
+    def fit(self, X: Matrix) -> Self:
         m, _ = X.shape
         distances = np.zeros((m, m))
         for i in range(m):
             for j in range(m):
                 distances[i, j] = np.linalg.norm(X[i] - X[j])
 
         W = np.zeros((m, m))
@@ -552,15 +552,15 @@
                 "n_components": ("0<,+inf", int),
                 "n_neighbors": ("0<,+inf", int),
                 "regularization": ("0,+inf", None),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "ModifiedLLE":
+    def fit(self, X: Matrix) -> Self:
         m, _ = X.shape
         distances = np.zeros((m, m))
         for i in range(m):
             for j in range(m):
                 distances[i, j] = np.linalg.norm(X[i] - X[j])
 
         W = np.zeros((m, m))
@@ -627,15 +627,15 @@
                 "n_components": ("0<,+inf", int),
                 "n_neighbors": ("0<,+inf", int),
                 "regularization": ("0,+inf", None),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "HessianLLE":
+    def fit(self, X: Matrix) -> Self:
         m, _ = X.shape
         dp = self.n_components * (self.n_components + 1) // 2
 
         if self.n_neighbors <= self.n_components + dp:
             self.n_neighbors = self.n_components * (self.n_components + 3)
             self.n_neighbors /= 2
             print(
@@ -746,15 +746,15 @@
                 "n_components": ("0<,+inf", int),
                 "max_iter": ("0<,+inf", int),
                 "max_halves": ("0<,+inf", int),
             }
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "SammonMapping":
+    def fit(self, X: Matrix) -> Self:
         m, _ = X.shape
         X_dist = cdist(X, X)
         scale = 0.5 / X_dist.sum()
 
         Y = np.random.normal(0, 1, (m, self.n_components))
         if self.initialize == "pca":
             Y = PCA(n_components=self.n_components).fit_transform(X)
@@ -867,15 +867,15 @@
         self._fitted = False
 
         self.set_param_ranges(
             {"n_components": ("0<,+inf", int), "sigma": ("0<,+inf", None)}
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "LaplacianEigenmap":
+    def fit(self, X: Matrix) -> Self:
         pairwise = cdist(X, X)
         weights = np.exp(-pairwise / (2 * self.sigma**2))
         np.fill_diagonal(weights, 0)
 
         laplacian = self._compute_laplacian(weights)
         normalized_laplacian = self._normalize_laplacian(weights, laplacian)
 
@@ -940,15 +940,15 @@
         self._fitted = False
 
         self.set_param_ranges(
             {"n_components": ("0<,+inf", int), "epsilon": ("0<,+inf", None)}
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "Isomap":
+    def fit(self, X: Matrix) -> Self:
         self.adj = self._make_adjacency(X)
         if np.isinf(self.adj).any():
             print(f"[Isomap] Too narrow bin size with epsilon of {self.epsilon}!")
             return
 
         m, _ = self.adj.shape
         H = np.eye(m) - (1 / m) * np.ones((m, m))
@@ -1010,21 +1010,21 @@
         epsilon: float = 5.0,
         algorithm: Literal["dijkstra", "floyd"] = "dijkstra",
     ) -> None:
         self.n_components = n_components
         self.epsilon = epsilon
         self.algorithm = algorithm
         self._fitted = False
-        
+
         self.set_param_ranges(
             {"n_components": ("0<,+inf", int), "epsilon": ("0<,+inf", None)}
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "ConformalIsomap":
+    def fit(self, X: Matrix) -> Self:
         self.adj = self._make_adjacency(X)
         if np.isinf(self.adj).any():
             print(f"[C-Isomap] Too narrow bin size with epsilon of {self.epsilon}!")
             return
 
         m, _ = self.adj.shape
         H = np.eye(m) - (1 / m) * np.ones((m, m))
@@ -1085,21 +1085,21 @@
 
     """
 
     def __init__(self, n_components: int = None, n_neighbors: int = 10) -> None:
         self.n_components = n_components
         self.n_neighbors = n_neighbors
         self._fitted = False
-        
+
         self.set_param_ranges(
             {"n_components": ("0<,+inf", int), "n_neighbors": ("0<,+inf", int)}
         )
         self.check_param_ranges()
 
-    def fit(self, X: Matrix) -> "LTSA":
+    def fit(self, X: Matrix) -> Self:
         m, n = X.shape
         self.neighbors, self.neighbor_indices = self._compute_neighborhood(X)
         M = np.zeros((m, m))
         use_svd = self.n_neighbors > n
 
         for i in range(m):
             Xi = self.neighbors[i]
```

### Comparing `luma-ml-0.6.5/luma/reduction/selection.py` & `luma-ml-0.6.6/luma/reduction/selection.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,14 +73,23 @@
         self.shuffle = shuffle
         self.stratify = stratify
         self.fold_type = fold_type
         self.random_state = random_state
         self.verbose = verbose
         self._fitted = False
 
+        self.set_param_ranges(
+            {
+                "n_features": ("0<,+inf", None),
+                "test_size": ("0,1", float),
+                "cv": ("0<,+inf", int),
+            }
+        )
+        self.check_param_ranges()
+
     def fit(self, X: Matrix, y: Vector) -> "SBS":
         _, n = X.shape
         self.estimator = Clone(self.estimator).get
 
         if 0 < self.n_features < 1:
             self.n_features = np.ceil(n * self.n_features).astype(int)
         elif self.n_features <= 0 or self.n_features > n:
@@ -237,14 +246,23 @@
         self.shuffle = shuffle
         self.stratify = stratify
         self.fold_type = fold_type
         self.random_state = random_state
         self.verbose = verbose
         self._fitted = False
 
+        self.set_param_ranges(
+            {
+                "n_features": ("0<,+inf", None),
+                "test_size": ("0,1", float),
+                "cv": ("0<,+inf", int),
+            }
+        )
+        self.check_param_ranges()
+
     def fit(self, X: Matrix, y: Vector) -> "SFS":
         _, n = X.shape
         self.estimator = Clone(self.estimator).get
 
         if isinstance(self.n_features, float) and 0 < self.n_features < 1:
             self.n_features = np.ceil(n * self.n_features).astype(int)
         elif self.n_features <= 0 or self.n_features > n:
@@ -390,14 +408,23 @@
         self.cv = cv
         self.shuffle = shuffle
         self.fold_type = fold_type
         self.random_state = random_state
         self.verbose = verbose
         self._fitted = False
 
+        self.set_param_ranges(
+            {
+                "n_features": ("0<,+inf", None),
+                "step_size": ("0<,+inf", int),
+                "cv": ("0<,+inf", int),
+            }
+        )
+        self.check_param_ranges()
+
     def fit(self, X: Matrix, y: Vector) -> "RFE":
         _, n = X.shape
         self.estimator = Clone(self.estimator).get
 
         if 0 < self.n_features < 1:
             self.n_features = np.floor(n * self.n_features).astype(int)
         elif self.n_features <= 0 or self.n_features > n:
```

### Comparing `luma-ml-0.6.5/luma/regressor/general.py` & `luma-ml-0.6.6/luma/regressor/general.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal
+from typing import Literal, Self
 from scipy.special import psi
 import numpy as np
 
 from luma.interface.util import Matrix
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.metric.regression import MeanSquaredError
@@ -48,18 +48,28 @@
         self.max_iter = max_iter
         self.regularization = regularization
         self.l1_ratio = l1_ratio
         self.alpha = alpha
         self.verbose = verbose
         self._fitted = False
 
+        self.set_param_ranges(
+            {
+                "learning_rate": ("0<,+inf", None),
+                "max_iter": ("0<,+inf", int),
+                "l1_ratio": ("0,1", None),
+                "alpha": ("0<,+inf", None),
+            }
+        )
+        self.check_param_ranges()
+
     def link_funciton(self, X: Matrix) -> Matrix:
         return np.exp(np.dot(X, self.weights))
 
-    def fit(self, X: Matrix, y: Matrix) -> "PoissonRegressor":
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         X = np.column_stack((np.ones(X.shape[0]), X))
         m, n = X.shape
         self.weights = np.zeros(n)
 
         for i in range(self.max_iter):
             predictions = self.link_funciton(X)
             gradient = np.dot(X.T, y - predictions) * self.learning_rate
@@ -139,18 +149,29 @@
         self.alpha = alpha
         self.l1_ratio = l1_ratio
         self.phi = phi
         self.regularization = regularization
         self.verbose = verbose
         self._fitted = False
 
+        self.set_param_ranges(
+            {
+                "learning_rate": ("0<,+inf", None),
+                "max_iter": ("0<,+inf", int),
+                "alpha": ("0,+inf", None),
+                "l1_ratio": ("0,1", None),
+                "phi": ("0,+inf", None),
+            }
+        )
+        self.check_param_ranges()
+
     def link_function(self, X: Matrix) -> Matrix:
         return np.log(1 + np.exp(np.dot(X, self.weights)))
 
-    def fit(self, X: Matrix, y: Matrix) -> "NegativeBinomialRegressor":
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         X = np.column_stack((np.ones(X.shape[0]), X))
         m, n = X.shape
         self.weights = np.zeros(n)
 
         for i in range(self.max_iter):
             mu = self.link_function(X)
             gradient = (y - mu) / (self.phi * (1 + mu / self.phi))
@@ -235,15 +256,27 @@
         self.max_iter = max_iter
         self.reg_strength = reg_strength
         self.l1_ratio = l1_ratio
         self.regularization = regularization
         self.verbose = verbose
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> "GammaRegressor":
+        self.set_param_ranges(
+            {
+                "learning_rate": ("0<,+inf", None),
+                "max_iter": ("0<,+inf", int),
+                "reg_strength": ("0,+inf", None),
+                "l1_ratio": ("0,1", None),
+                "alpha": ("-inf,inf", None),
+                "beta": ("-inf,inf", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         X = np.column_stack((np.ones(X.shape[0]), X))
         m, n = X.shape
         self.alpha = np.ones(n) * self.alpha
         self.beta = np.ones(n) * self.beta
 
         for i in range(self.max_iter):
             gradient = (self.alpha - 1) / self.alpha - psi(self.alpha)
@@ -334,15 +367,27 @@
         self.max_iter = max_iter
         self.reg_strength = reg_strength
         self.l1_ratio = l1_ratio
         self.regularization = regularization
         self.verbose = verbose
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> "BetaRegressor":
+        self.set_param_ranges(
+            {
+                "learning_rate": ("0<,+inf", None),
+                "max_iter": ("0<,+inf", int),
+                "reg_strength": ("0,+inf", None),
+                "l1_ratio": ("0,1", None),
+                "alpha": ("-inf,inf", None),
+                "beta": ("-inf,inf", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         X = np.column_stack((np.ones(X.shape[0]), X))
         m, n = X.shape
         self.alpha = np.ones(n) * self.alpha
         self.beta = np.ones(n) * self.beta
 
         for i in range(self.max_iter):
             gradient_alpha = psi(self.alpha) - psi(self.alpha + self.beta)
@@ -429,15 +474,26 @@
         self.phi = phi
         self.l1_ratio = l1_ratio
         self.alpha = alpha
         self.regularization = regularization
         self.verbose = verbose
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> "InverseGaussianRegressor":
+        self.set_param_ranges(
+            {
+                "learning_rate": ("0<,+inf", None),
+                "max_iter": ("0<,+inf", int),
+                "phi": ("0<,+inf", None),
+                "l1_ratio": ("0,1", None),
+                "alpha": ("0,+inf", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         X = np.column_stack((np.ones(X.shape[0]), X))
         m, n = X.shape
         self.weights = np.ones(n)
 
         for i in range(self.max_iter):
             error = y - np.dot(X, self.weights)
```

### Comparing `luma-ml-0.6.5/luma/regressor/linear.py` & `luma-ml-0.6.6/luma/regressor/linear.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Self
 import numpy as np
 
 from luma.interface.util import Matrix, Vector, KernelUtil
 from luma.interface.exception import NotFittedError
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.metric.regression import MeanSquaredError
 
@@ -30,15 +31,18 @@
 
     """
 
     def __init__(self, alpha: float = 1.0) -> None:
         self.alpha = alpha
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> "RidgeRegressor":
+        self.set_param_ranges({"alpha": ("0,+inf", None)})
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         X = np.column_stack((np.ones(X.shape[0]), X))
         identity_matrix = np.identity(X.shape[1])
         self.coef_ = np.linalg.inv(X.T.dot(X) + self.alpha * identity_matrix)
         self.coef_ = self.coef_.dot(X.T).dot(y)
         self._fitted = True
         return self
 
@@ -81,18 +85,27 @@
     ) -> None:
         self.alpha = alpha
         self.max_iter = max_iter
         self.learning_rate = learning_rate
         self.verbose = verbose
         self._fitted = False
 
+        self.set_param_ranges(
+            {
+                "alpha": ("0,+inf", None),
+                "max_iter": ("0<,+inf", int),
+                "learning_rate": ("0<,+inf", None),
+            }
+        )
+        self.check_param_ranges()
+
     def _soft_threshold(self, x: Matrix, threshold: float) -> Matrix:
         return np.sign(x) * np.maximum(0, np.abs(x) - threshold)
 
-    def fit(self, X: Matrix, y: Matrix) -> "LassoRegressor":
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         X = np.column_stack((np.ones(X.shape[0]), X))
         self.coef_ = np.zeros(X.shape[1])
 
         for i in range(self.max_iter):
             coefficients_prev = self.coef_.copy()
             y_pred = X.dot(self.coef_)
             gradient = -(X.T.dot(y - y_pred)) * self.learning_rate
@@ -149,18 +162,28 @@
         self.l1_ratio = l1_ratio
         self.max_iter = max_iter
         self.learning_rate = learning_rate
         self.verbose = verbose
         self.coef_ = None
         self._fitted = False
 
+        self.set_param_ranges(
+            {
+                "alpha": ("0,+inf", None),
+                "l1_ratio": ("0,1", None),
+                "max_iter": ("0<,+inf", int),
+                "learning_rate": ("0<,+inf", None),
+            }
+        )
+        self.check_param_ranges()
+
     def _soft_threshold(self, x: Matrix, alpha: float) -> Matrix:
         return np.sign(x) * np.maximum(np.abs(x) - alpha, 0)
 
-    def fit(self, X: Matrix, y: Matrix) -> "ElasticNetRegressor":
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         N, p = X.shape
         self.coef_ = np.zeros(p)
 
         for i in range(self.max_iter):
             y_pred = X.dot(self.coef_)
             gradient = -(1 / N) * X.T.dot(y - y_pred)
             lefthand = self.coef_ - self.learning_rate * gradient
@@ -199,15 +222,15 @@
     simplicity and efficiency in modeling linear relationships.
     """
 
     def __init__(self):
         self.coef_ = None
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> "LinearRegressor":
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         X = np.hstack([np.ones((X.shape[0], 1)), X])
         X_T = np.transpose(X)
         self.coef_ = np.linalg.inv(X_T.dot(X)).dot(X_T).dot(y)
 
         self._fitted = True
         return self
 
@@ -263,15 +286,25 @@
         self.kernel_params = {
             "alpha": self.alpha,
             "gamma": self.gamma,
             "deg": self.deg,
             "coef": self.coef,
         }
 
-    def fit(self, X: Matrix, y: Vector) -> "KernelRidgeRegressor":
+        self.set_param_ranges(
+            {
+                "alpha": ("0,+inf", None),
+                "deg": ("0<,+inf", int),
+                "gamma": ("0<,+inf", None),
+                "coef": ("-inf,+inf", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Vector) -> Self:
         m, _ = X.shape
         self._X = X
         self.ku_ = KernelUtil(self.kernel, **self.kernel_params)
 
         K = self.ku_.kernel_func(X)
         self.alpha_mat = np.eye(m) * self.alpha
         self.dual_coef = np.linalg.inv(K + self.alpha_mat).dot(y)
@@ -309,15 +342,20 @@
     """
 
     def __init__(self, alpha_init: float = None, lambda_init: float = None) -> None:
         self.alpha_init = alpha_init
         self.lambda_init = lambda_init
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Vector) -> "BayesianRidgeRegressor":
+        self.set_param_ranges(
+            {"alpha_init": ("0<,+inf", None), "lambda_init": ("0<,+inf", None)}
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Vector) -> Self:
         if self.alpha_init is None:
             self.alpha_init = 1 / np.var(y)
         if self.lambda_init is None:
             self.lambda_init = 1.0
 
         m, n = X.shape
         X = np.column_stack((np.ones(m), X))
```

### Comparing `luma-ml-0.6.5/luma/regressor/neighbors.py` & `luma-ml-0.6.6/luma/regressor/neighbors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Self
 from scipy.spatial import distance_matrix
 import numpy as np
 
 from luma.interface.util import Matrix
 from luma.core.super import Estimator, Supervised, Evaluator
 from luma.interface.util import NearestNeighbors
 from luma.interface.exception import NotFittedError
@@ -30,15 +31,18 @@
 
     def __init__(self, n_neighbors: int = 5):
         self.n_neighbors = n_neighbors
         self._neighbors = None
         self._y = None
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> "KNNRegressor":
+        self.set_param_ranges({"n_neighbors": ("0<,+inf", int)})
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         self._neighbors = NearestNeighbors(X, self.n_neighbors)
         self._y = y
         self._fitted = True
         return self
 
     def predict(self, X: Matrix) -> Matrix:
         if not self._fitted:
@@ -84,15 +88,24 @@
         self.n_density = n_density
         self.min_neighbors = min_neighbors
         self.max_neighbors = max_neighbors
         self._X = None
         self._y = None
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> "AdaptiveKNNRegressor":
+        self.set_param_ranges(
+            {
+                "n_density": ("0<,+inf", int),
+                "min_neighbors": ("0<,+inf", int),
+                "max_neighbors": ("0<,+inf", int),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         self._X = X
         self._y = y
         self.dist_matrix = distance_matrix(X, X)
         self.local_density = np.sort(self.dist_matrix, axis=1)
         self.local_density = self.local_density[:, self.n_density]
 
         self._fitted = True
@@ -143,15 +156,18 @@
 
     def __init__(self, n_neighbors: int = 5):
         self.n_neighbors = n_neighbors
         self._X = None
         self._y = None
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> "WeightedKNNRegressor":
+        self.set_param_ranges({"n_neighbors": ("0<,+inf", int)})
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         self._X = X
         self._y = y
 
         self._fitted = True
         return self
 
     def predict(self, X: Matrix) -> Matrix:
```

### Comparing `luma-ml-0.6.5/luma/regressor/poly.py` & `luma-ml-0.6.6/luma/regressor/poly.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Literal
+from typing import Literal, Self
 import numpy as np
 
 from luma.interface.util import Matrix
 from luma.interface.exception import NotFittedError
 from luma.core.super import Estimator, Evaluator
 from luma.metric.regression import MeanSquaredError
 
@@ -34,25 +34,36 @@
     ) -> None:
         self.deg = deg
         self.alpha = alpha
         self.l1_ratio = l1_ratio
         self.regularization = regularization
         self._fitted = False
 
-    def _generate_polynomial_features(self, X):
+        self.set_param_ranges(
+            {
+                "deg": ("0<,+inf", int),
+                "alpha": ("0,+inf", None),
+                "l1_ratio": ("0,1", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def _generate_polynomial_features(self, X: Matrix) -> Matrix:
         X_poly = X.copy()
         for d in range(2, self.deg + 1):
             X_poly = np.hstack((X_poly, X**d))
         return X_poly
 
-    def fit(self, X: Matrix, y: Matrix) -> "PolynomialRegressor":
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         X_poly = self._generate_polynomial_features(X)
         reg_matrix = self._regularization_matrix(X_poly.shape[1])
+
         augmented_matrix = np.vstack([X_poly, np.sqrt(self.alpha) * reg_matrix])
         augmented_target = np.hstack([y, np.zeros(X_poly.shape[1])])
+
         self.coef_ = np.linalg.lstsq(augmented_matrix, augmented_target, rcond=None)[0]
         self._fitted = True
         return self
 
     def _regularization_matrix(self, n: int) -> Matrix:
         if self.regularization == "l2":
             return self.alpha * np.eye(n)
```

### Comparing `luma-ml-0.6.5/luma/regressor/robust.py` & `luma-ml-0.6.6/luma/regressor/robust.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple
+from typing import Self, Tuple
 import numpy as np
 
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.interface.util import Matrix, Vector
 from luma.interface.exception import NotFittedError
 from luma.metric.regression import MeanSquaredError
 from luma.regressor.linear import LinearRegressor
@@ -56,15 +56,25 @@
         self.min_inliers = min_inliers
         self.threshold = threshold
         self.random_state = random_state
         self.verbose = verbose
         self.inliers_ = None
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Vector) -> "RANSAC":
+        self.set_param_ranges(
+            {
+                "min_points": ("0,+inf", int),
+                "max_iter": ("0<,+inf", int),
+                "min_inliers": ("0,+inf", None),
+                "threshold": ("0,+inf", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Vector) -> Self:
         m, _ = X.shape
         best_err = np.inf
         best_indices = None
 
         np.random.seed(self.random_state)
         Xy = np.hstack((X, y.reshape(-1, 1)))
 
@@ -189,15 +199,25 @@
         self.min_inliers = min_inliers
         self.threshold = threshold
         self.random_state = random_state
         self.verbose = verbose
         self.inliers_ = None
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Vector) -> "MLESAC":
+        self.set_param_ranges(
+            {
+                "min_points": ("0,+inf", int),
+                "max_iter": ("0<,+inf", int),
+                "min_inliers": ("0,+inf", None),
+                "threshold": ("0,+inf", None),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Vector) -> Self:
         m, _ = X.shape
         best_likelihood = -np.inf
         best_indices = None
 
         np.random.seed(self.random_state)
         Xy = np.hstack((X, y.reshape(-1, 1)))
```

### Comparing `luma-ml-0.6.5/luma/regressor/svm.py` & `luma-ml-0.6.6/luma/regressor/svm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Self
 import numpy as np
 
 from luma.interface.util import Matrix, KernelUtil
 from luma.interface.exception import NotFittedError, UnsupportedParameterError
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.metric.regression import MeanSquaredError
 
@@ -39,15 +40,26 @@
         self.epsilon = epsilon
         self.batch_size = batch_size
         self.learning_rate = learning_rate
         self.max_iter = max_iter
         self.verbose = verbose
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> "SVR":
+        self.set_param_ranges(
+            {
+                "C": ("0,+inf", None),
+                "epsilon": ("0,+inf", None),
+                "batch_size": ("0<,+inf", int),
+                "learning_rate": ("0<,+inf", None),
+                "max_iter": ("0<,+inf", int),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         m, n = X.shape
         id = np.arange(m)
         np.random.shuffle(id)
 
         self.bias = 0.0
         self.weight = np.zeros(n)
 
@@ -126,15 +138,27 @@
         self.learning_rate = learning_rate
         self.max_iter = max_iter
         self.kernel = kernel
         self.verbose = verbose
         self._kernel_func = None
         self._fitted = False
 
-    def fit(self, X: Matrix, y: Matrix) -> "KernelSVR":
+        self.set_param_ranges(
+            {
+                "C": ("0<,+inf", None),
+                "deg": ("0<,+inf", int),
+                "gamma": ("0<,+inf", None),
+                "coef": ("-inf,+inf", None),
+                "learning_rate": ("0<,+inf", None),
+                "max_iter": ("0<,+inf", int),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Matrix) -> Self:
         m, _ = X.shape
         self._set_kernel_func()
         self.alpha = np.random.random(m)
         self.bias = 0
 
         y_mul_kernel = np.outer(y, y) * self._kernel_func(X, X)
         for i in range(self.max_iter):
```

### Comparing `luma-ml-0.6.5/luma/regressor/tree.py` & `luma-ml-0.6.6/luma/regressor/tree.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple
+from typing import Self, Tuple
 import numpy as np
 
 from luma.interface.util import Matrix, Vector
 from luma.interface.exception import NotFittedError
 from luma.core.super import Estimator, Evaluator, Supervised
 from luma.interface.util import DecisionTreeNode
 from luma.metric.regression import MeanSquaredError
@@ -20,15 +20,14 @@
     on feature values. At each node of the tree, it chooses the split
     that minimizes the variance (or another specified criterion) of the
     target variable within the regions created by the split.
 
     Parameters
     ----------
     `max_depth` : Maximum depth of the tree
-    `criterion` : Function used to measure the quality of a split
     `min_samples_split` : Minimum samples required to split a node
     `min_samples_leaf` : Minimum samples required to be at a leaf node
     `max_features` : Number of features to consider
     `min_variance_decrease` : Minimum decrement of variance for a split
     `max_leaf_nodes` : Maximum amount of leaf nodes
     `random_state` : The randomness seed of the estimator
 
@@ -50,17 +49,27 @@
         self.max_features = max_features
         self.min_variance_decrease = min_variance_decrease
         self.max_leaf_nodes = max_leaf_nodes
         self.random_state = random_state
         self.root = None
         self._fitted = False
 
-    def fit(
-        self, X: Matrix, y: Vector, sample_weights: Vector = None
-    ) -> "DecisionTreeRegressor":
+        self.set_param_ranges(
+            {
+                "max_depth": ("0<,+inf", int),
+                "min_samples_split": ("0,+inf", int),
+                "min_samples_leaf": ("0<,+inf", int),
+                "max_features": ("0<,+inf", int),
+                "min_variance_decrese": ("0,+inf", None),
+                "max_leaf_nodes": ("0<,+inf", int),
+            }
+        )
+        self.check_param_ranges()
+
+    def fit(self, X: Matrix, y: Vector, sample_weights: Vector = None) -> Self:
         if sample_weights is None:
             sample_weights = np.ones(len(y))
         sample_weights = Vector(sample_weights)
         np.random.seed(self.random_state)
 
         self.root = self._build_tree(X, y, 0, sample_weights)
         self._fitted = True
```

### Comparing `luma-ml-0.6.5/luma/visual/eda.py` & `luma-ml-0.6.6/luma/visual/eda.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import matplotlib.pyplot as plt
 import seaborn as sns
 import pandas as pd
 
 from luma.core.super import Visualizer
 
 
-__all__ = ("CorrelationHeatMap", "CorrelationBar", "JointPlot", "MissingProportion")
+__all__ = ("CorrelationHeatmap", "CorrelationBar", "JointPlot", "MissingProportion")
 
 
-class CorrelationHeatMap(Visualizer):
+class CorrelationHeatmap(Visualizer):
     def __init__(self, data: pd.DataFrame) -> None:
         self.data = data
         self.corr = data.corr()
 
     def plot(
         self,
         ax: Optional[plt.Axes] = None,
@@ -22,14 +22,15 @@
         colorBar: bool = True,
         show: bool = False,
     ) -> plt.Axes:
         if ax is None:
             n_features = self.data.shape[1]
             size = n_features / 2 if n_features < 20 else 10
             _, ax = plt.subplots(figsize=(size + 1, size))
+            show = True
 
         sns.heatmap(
             self.corr, ax=ax, cmap=colorMap, annot=annotate, cbar=colorBar, fmt="0.2f"
         )
 
         ax.set_title("Correlation Heat Map")
         ax.figure.tight_layout()
@@ -43,14 +44,16 @@
     def __init__(self, data: pd.DataFrame, target: str) -> None:
         self.data = data
         self.target = target
 
     def plot(self, ax: Optional[plt.Axes] = None, show: bool = False) -> plt.Axes:
         if ax is None:
             _, ax = plt.subplots()
+            show = True
+
         corr_bar = [
             abs(self.data[col].corr(self.data[self.target])) for col in self.data
         ]
         sns.barplot(x=self.data.columns, y=corr_bar, hue=self.data.columns, ax=ax)
 
         ax.set_xticklabels(ax.get_xticklabels(), rotation=45)
         ax.set_title(f"Correlations with {self.target}")
@@ -83,14 +86,16 @@
     def nan_proportions(self) -> pd.DataFrame:
         nan_props = self.data.isna().mean()
         return nan_props
 
     def plot(self, ax: Optional[plt.Axes] = None, show: bool = False) -> plt.Axes:
         if ax is None:
             _, ax = plt.subplots()
+            show = True
+
         nan_props = self.nan_proportions()
         sns.barplot(x=nan_props.index, y=nan_props.values, hue=self.data.columns, ax=ax)
 
         ax.set_xticklabels(ax.get_xticklabels(), rotation=45)
         ax.set_xlabel("Columns")
         ax.set_ylabel("Proportion")
         ax.set_title("Missing Value Proportions")
```

### Comparing `luma-ml-0.6.5/luma/visual/evaluation.py` & `luma-ml-0.6.6/luma/visual/evaluation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from itertools import product
-from typing import Any, Dict, List, Literal, Optional, Tuple
+from typing import List, Literal, Optional, Tuple
 from matplotlib.colors import ListedColormap
 import matplotlib.pyplot as plt
 import numpy as np
 
 from luma.interface.util import Matrix, Vector
 from luma.core.super import Evaluator, Visualizer, Estimator
 from luma.model_selection.split import TrainTestSplit
@@ -18,15 +17,14 @@
     "ClusterPlot",
     "ROCCurve",
     "PrecisionRecallCurve",
     "ConfusionMatrix",
     "ResidualPlot",
     "LearningCurve",
     "ValidationCurve",
-    "ValidationHeatmap",
     "InertiaPlot",
 )
 
 
 class DecisionRegion(Visualizer):
     def __init__(
         self,
@@ -55,14 +53,15 @@
             self.y = self.estimator.labels
 
     def plot(
         self,
         ax: Optional[plt.Axes] = None,
         size: float = 250,
         scale: float = 10.0,
+        grid: bool = True,
         show: bool = False,
     ) -> plt.Axes:
         x1_min, x1_max = self.X[:, 0].min(), self.X[:, 0].max()
         x2_min, x2_max = self.X[:, 1].min(), self.X[:, 1].max()
         delta_1, delta_2 = (x1_max - x1_min) / size, (x2_max - x2_min) / size
 
         x1_min, x1_max = x1_min - delta_1 * scale, x1_max + delta_1 * scale
@@ -93,16 +92,18 @@
             alpha=0.8,
             edgecolors="black",
         )
 
         ax.set_xlabel(self.xlabel)
         ax.set_ylabel(self.ylabel)
         ax.set_title(self.title)
-        ax.figure.tight_layout()
+        if grid:
+            ax.grid(alpha=0.2)
 
+        ax.figure.tight_layout()
         if show:
             plt.show()
         return ax
 
 
 class ClusterPlot(Visualizer):
     def __init__(
@@ -615,15 +616,15 @@
         param_range: Vector,
         cv: int = 5,
         shuffle: bool = True,
         fold_type: FoldType = KFold,
         metric: Evaluator = Accuracy,
         random_state: int = None,
         verbose: bool = False,
-    ):
+    ) -> None:
         self.estimator = estimator
         self.X = X
         self.y = y
         self.param_name = param_name
         self.param_range = param_range
         self.cv = cv
         self.shuffle = shuffle
@@ -717,164 +718,14 @@
         ax.figure.tight_layout()
 
         if show:
             plt.show()
         return ax
 
 
-class ValidationHeatmap(Visualizer):
-    """
-    A validation heatmap in machine learning is a graphical representation that
-    illustrates the performance of a model on a validation dataset for different
-    combinations of two hyperparameters. Each cell in the heatmap corresponds to a
-    specific combination of the hyperparameters' values, and the color intensity
-    represents the performance metric score. This visualization is useful for
-    identifying the interaction between two hyperparameters and selecting the best
-    combination for model tuning.
-
-    Parameters
-    ----------
-    `estimator` : An estimator to evaluate
-    `X` : Feature data for training
-    `y` : Target data for training
-    `param_dict` : Dictionary with two hyperparameters and their respective ranges
-    `cv` : Number of times for cross-validation
-    `shuffle` : Whether to shuffle the dataset
-    `fold_type` : Fold type (Default `KFold`)
-    `metric` : Evaluation metric for scoring
-    `random_state` : Seed for random sampling upon splitting samples
-
-    """
-
-    def __init__(
-        self,
-        estimator: Estimator,
-        X: Matrix,
-        y: Vector,
-        param_dict: Dict[str, Any],
-        cv: int = 5,
-        shuffle: bool = True,
-        fold_type: FoldType = KFold,
-        metric: Evaluator = Accuracy,
-        random_state: int = None,
-        verbose: bool = False,
-    ) -> None:
-        self.estimator = estimator
-        self.X = X
-        self.y = y
-        self.param_dict = param_dict
-        self.cv = cv
-        self.shuffle = shuffle
-        self.fold_type = fold_type
-        self.metric = metric
-        self.random_state = random_state
-        self.verbose = verbose
-
-        self.names_ = list(self.param_dict.keys())
-
-        self.sizes_ = (
-            len(self.param_dict[self.names_[0]]),
-            len(self.param_dict[self.names_[1]]),
-        )
-
-        self.values_ = (
-            self.param_dict[self.names_[0]],
-            self.param_dict[self.names_[1]],
-        )
-
-        self.scores = np.zeros(self.sizes_)
-
-    def _evaluate(self) -> None:
-        param_combs = list(product(*self.param_dict.values()))
-        max_iter = len(param_combs)
-
-        if self.verbose:
-            print(
-                f"Fitting {self.cv} folds for {max_iter} candidates,",
-                f"totalling {self.cv * max_iter} fits.\n",
-            )
-
-        for idx, params in enumerate(param_combs):
-            param_values = dict(zip(self.names_, params))
-            self.estimator.set_params(**param_values)
-
-            cv_model = CrossValidator(
-                estimator=self.estimator,
-                metric=self.metric,
-                cv=self.cv,
-                shuffle=self.shuffle,
-                fold_type=self.fold_type,
-                random_state=self.random_state,
-                verbose=False,
-            )
-
-            _, score = cv_model.score(self.X, self.y)
-            i, j = idx // self.sizes_[1], idx % self.sizes_[1]
-            self.scores[i, j] = score
-
-            if self.verbose:
-                print(
-                    f"[ValidationHeatmap] candidate {idx + 1}/{max_iter}",
-                    f"{param_values} - score: {score:.3f}",
-                )
-
-    def plot(
-        self,
-        ax: Optional[plt.Axes] = None,
-        cmap: ListedColormap = "RdYlGn",
-        log_xticks: bool = True,
-        log_yticks: bool = True,
-        annotate: bool = True,
-        show: bool = False,
-    ) -> plt.Axes:
-        if ax is None:
-            _, ax = plt.subplots()
-            show = True
-
-        cax = ax.imshow(self.scores, cmap=cmap)
-        ax.figure.colorbar(cax)
-
-        self._evaluate()
-        if annotate:
-            for i in range(self.sizes_[0]):
-                for j in range(self.sizes_[1]):
-                    score = self.scores[i, j]
-                    ax.text(
-                        j,
-                        i,
-                        f"{score:.2f}",
-                        ha="center",
-                        va="center",
-                        color="white",
-                        alpha=0.7,
-                    )
-
-        ax.set_xticks(range(self.sizes_[0]), np.round(self.values_[0], 2))
-        ax.set_yticks(range(self.sizes_[1]), np.round(self.values_[1], 2))
-
-        if log_xticks:
-            ax.set_xticklabels(
-                [r"$10^{" + f"{np.log10(n):.1f}" + r"}$" for n in self.values_[0]]
-            )
-        if log_yticks:
-            ax.set_yticklabels(
-                [r"$10^{" + f"{np.log10(n):.1f}" + r"}$" for n in self.values_[1]]
-            )
-
-        ax.set_xlabel(self.names_[1])
-        ax.set_ylabel(self.names_[0])
-
-        ax.set_title("Validation Heatmap")
-        ax.figure.tight_layout()
-
-        if show:
-            plt.show()
-        return ax
-
-
 class InertiaPlot(Visualizer):
     """
     An inertia plot in clustering visualizes the inertia against the number of
     clusters, helping to determine the optimal number of clusters by identifying
     the "elbow" point where the rate of decrease in inertia sharply changes.
     It reflects how well clusters are compact and separated, with lower inertia
     indicating better clustering. The plot aids in applying the elbow method for
```

### Comparing `luma-ml-0.6.5/luma_ml.egg-info/PKG-INFO` & `luma-ml-0.6.6/luma_ml.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.6.5
+Version: 0.6.6
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/LUMA
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: scipy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
 
 <!DOCTYPE html>
 <html>
     <body>
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
         <h1 class="main-title">LUMA</h1>
         <p class="subtitle">A Comprehensive Python Module for Machine Learning and Data Science</p>
         <img alt="pypi-version" src="https://img.shields.io/pypi/v/luma-ml?logo=python&logoColor=white&color=blue">
         <img alt="pypi-downloads" src="https://img.shields.io/pypi/dm/luma-ml">
-        <img src="https://img.shields.io/badge/total downloads-4.3k-red">
-        <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/ChanLumerico/luma?color=yellow">
+        <img src="https://img.shields.io/badge/total downloads-4.8k-red">
+        <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=yellow">
         <img alt="Code Style" src="https://img.shields.io/badge/code%20style-black-000000.svg">
-        <img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/ChanLumerico/luma?color=purple">
         <div class="module">
             <h3 class="module-header">Submodules</h3>
             <table>
                 <tr>
                     <th>Name</th>
                     <th>Description</th>
                 </tr>
@@ -104,23 +108,23 @@
         </div>
         <h2></h2>
         <div class="others">
             <h3 class="others-header">Others</h3>
             <table>
                 <tr>
                     <td>Latest Version</td>
-                    <td>0.6.5</td>
+                    <td>0.6.6</td>
                 </tr>
                 <tr>
                     <td>Lines of Code</td>
-                    <td>~15.7K</td>
+                    <td>~16.3K</td>
                 </tr>
                 <tr>
                     <td>Requirement</td>
-                    <td>Python 3.10 or later</td>
+                    <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
                     <td>NumPy, SciPy, Pandas, Matplotlib, Seaborn</td>
                 </tr>
                 <tr>
                     <td>Documentation</td>
```

#### html2text {}

```diff
@@ -1,19 +1,21 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.6.5 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.6.6 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/LUMA Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.10
-Description-Content-Type: text/markdown License-File: LICENSE
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
+Requires-Dist: seaborn
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
-4.3k-red][GitHub last commit][Code Style][GitHub code size in bytes]
+4.8k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
 luma.classifier      Toolkit for classification models including various
                      algorithms.
 luma.clustering      Focuses on unsupervised learning and clustering
                      algorithms.
 luma.core            Foundational backbone providing essential data structures
@@ -31,12 +33,12 @@
 luma.reduction       Dimensionality reduction techniques for high-dimensional
                      datasets.
 luma.regressor       Comprehensive range of regression algorithms.
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
-Latest Version 0.6.5
-Lines of Code  ~15.7K
-Requirement    Python 3.10 or later
+Latest Version 0.6.6
+Lines of Code  ~16.3K
+Requirement    Python 3.12 or later
 Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.6.5/luma_ml.egg-info/SOURCES.txt` & `luma-ml-0.6.6/luma_ml.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 luma/metric/regression.py
 luma/migrate/port.py
 luma/model_selection/cv.py
 luma/model_selection/fold.py
 luma/model_selection/search.py
 luma/model_selection/split.py
 luma/neural/activation.py
-luma/neural/multi_layer.py
+luma/neural/network.py
 luma/neural/optimizer.py
 luma/neural/single.py
 luma/pipe/pipeline.py
 luma/preprocessing/encoder.py
 luma/preprocessing/imputer.py
 luma/preprocessing/outlier.py
 luma/preprocessing/scaler.py
@@ -57,8 +57,10 @@
 luma/visual/evaluation.py
 luma_ml.egg-info/PKG-INFO
 luma_ml.egg-info/SOURCES.txt
 luma_ml.egg-info/dependency_links.txt
 luma_ml.egg-info/requires.txt
 luma_ml.egg-info/top_level.txt
 test/__local__.py
-test/_docs.py
+test/_mlp_clf.py
+test/_mlp_reg.py
+test/_opt.py
```

### Comparing `luma-ml-0.6.5/setup.py` & `luma-ml-0.6.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="luma-ml",
-    version="0.6.5",
+    version="0.6.6",
     author="ChanLumerico",
     author_email="greensox284@gmail.com",
     description="A Comprehensive Python Module for Machine Learning and Data Science",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ChanLumerico/LUMA",
     packages=setuptools.find_namespace_packages(),
```

