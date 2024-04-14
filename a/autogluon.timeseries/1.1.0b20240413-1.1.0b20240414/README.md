# Comparing `tmp/autogluon.timeseries-1.1.0b20240413.tar.gz` & `tmp/autogluon.timeseries-1.1.0b20240414.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-1.1.0b20240413.tar", last modified: Sat Apr 13 09:05:11 2024, max compression
+gzip compressed data, was "autogluon.timeseries-1.1.0b20240414.tar", last modified: Sun Apr 14 10:22:41 2024, max compression
```

## Comparing `autogluon.timeseries-1.1.0b20240413.tar` & `autogluon.timeseries-1.1.0b20240414.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:05:11.664573 autogluon.timeseries-1.1.0b20240413/
--rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-04-13 09:05:11.664573 autogluon.timeseries-1.1.0b20240413/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 09:05:11.664573 autogluon.timeseries-1.1.0b20240413/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:05:11.652573 autogluon.timeseries-1.1.0b20240413/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:05:11.652573 autogluon.timeseries-1.1.0b20240413/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:05:11.656573 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:05:11.656573 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:05:11.656573 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45595 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13828 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:05:11.656573 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/metrics/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)    13399 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/metrics/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/metrics/quantile.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:05:11.656573 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:05:11.660573 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23435 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:05:11.660573 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31303 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/autogluon_tabular/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:05:11.660573 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/chronos/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/chronos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14659 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/chronos/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20784 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/chronos/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/chronos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:05:11.660573 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:05:11.660573 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34017 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:05:11.660573 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19780 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:05:11.660573 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/local/npts.py
--rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/local/statsforecast.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:05:11.660573 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/multi_window/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/multi_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/multi_window/multi_window_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (127)    81219 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:05:11.664573 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59100 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:05:11.664573 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:05:11.664573 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/utils/datetime/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/utils/datetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/utils/datetime/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/utils/datetime/lags.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/utils/datetime/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/utils/datetime/time_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    19492 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-13 09:03:53.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-13 09:05:11.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:05:11.656573 autogluon.timeseries-1.1.0b20240413/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-04-13 09:05:11.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-13 09:05:11.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 09:05:11.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-13 09:05:11.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-13 09:05:11.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-13 09:05:11.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 09:05:11.000000 autogluon.timeseries-1.1.0b20240413/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:41.524768 autogluon.timeseries-1.1.0b20240414/
+-rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-04-14 10:22:41.524768 autogluon.timeseries-1.1.0b20240414/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 10:22:41.524768 autogluon.timeseries-1.1.0b20240414/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:41.512768 autogluon.timeseries-1.1.0b20240414/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:41.512768 autogluon.timeseries-1.1.0b20240414/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:41.516768 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:41.516768 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:41.516768 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45595 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13828 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:41.516768 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/metrics/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13399 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/metrics/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/metrics/quantile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:41.516768 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:41.516768 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23435 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:41.516768 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31303 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/autogluon_tabular/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:41.520768 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/chronos/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/chronos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14659 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/chronos/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20784 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/chronos/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/chronos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:41.520768 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:41.520768 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34017 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:41.520768 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19780 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:41.520768 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11836 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/local/npts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32991 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/local/statsforecast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:41.520768 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11243 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81823 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:41.520768 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59100 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:41.524768 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:41.524768 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/utils/datetime/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/utils/datetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/utils/datetime/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5909 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/utils/datetime/lags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/utils/datetime/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/utils/datetime/time_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19492 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-14 10:21:21.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-14 10:22:41.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 10:22:41.516768 autogluon.timeseries-1.1.0b20240414/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11835 2024-04-14 10:22:41.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-14 10:22:41.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 10:22:41.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 10:22:41.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-14 10:22:41.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 10:22:41.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 10:22:41.000000 autogluon.timeseries-1.1.0b20240414/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-1.1.0b20240413/PKG-INFO` & `autogluon.timeseries-1.1.0b20240414/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 1.1.0b20240413
+Version: 1.1.0b20240414
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-1.1.0b20240413/setup.py` & `autogluon.timeseries-1.1.0b20240414/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     "scipy",  # version range defined in `core/_setup_utils.py`
     "pandas",  # version range defined in `core/_setup_utils.py`
     "torch",  # version range defined in `core/_setup_utils.py`
     "lightning",  # version range defined in `core/_setup_utils.py`
     "pytorch_lightning",  # version range defined in `core/_setup_utils.py`
     "transformers[sentencepiece]",  # version range defined in `core/_setup_utils.py`
     "accelerate",  # version range defined in `core/_setup_utils.py`
-    "statsmodels>=0.13.0,<0.15",
     "gluonts>=0.14.0,<0.14.4",  # 0.14.4 caps pandas<2.2
     "networkx",  # version range defined in `core/_setup_utils.py`
     # TODO: update statsforecast to v1.5.0 - resolve antlr4-python3-runtime dependency clash with multimodal
     "statsforecast>=1.4.0,<1.5",
     "mlforecast>=0.10.0,<0.10.1",
     "utilsforecast>=0.0.10,<0.0.11",
     "tqdm",  # version range defined in `core/_setup_utils.py`
```

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/metrics/__init__.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/metrics/abstract.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/metrics/abstract.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/metrics/point.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/metrics/point.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/metrics/quantile.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/metrics/quantile.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/metrics/utils.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/__init__.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/autogluon_tabular/utils.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/autogluon_tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/chronos/model.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/chronos/model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/chronos/pipeline.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/chronos/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/chronos/utils.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/chronos/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/gluonts/torch/models.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/gluonts/torch/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/local/__init__.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/local/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/local/naive.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/local/npts.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/local/npts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/multi_window/multi_window_model.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/multi_window/multi_window_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/models/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/predictor.py`

 * *Files 0% similar despite different names*

```diff
@@ -627,15 +627,19 @@
         val_step_size : int or None, default = None
             Step size between consecutive validation windows. If set to ``None``, defaults to ``prediction_length``
             provided when creating the predictor.
 
             This argument has no effect if ``tuning_data`` is provided.
         refit_every_n_windows: int or None, default = 1
             When performing cross validation, each model will be retrained every ``refit_every_n_windows`` validation
-            windows. If set to ``None``, model will only be fit once for the first validation window.
+            windows, where the number of validation windows is specified by `num_val_windows`. Note that in the
+            default setting where `num_val_windows=1`, this argument has no effect.
+
+            If set to ``None``, models will only be fit once for the first (oldest) validation window. By default,
+            `refit_every_n_windows=1`, i.e., all models will be refit for each validation window.
         refit_full : bool, default = False
             If True, after training is complete, AutoGluon will attempt to re-train all models using all of training
             data (including the data initially reserved for validation). This argument has no effect if ``tuning_data``
             is provided.
         enable_ensemble : bool, default = True
             If True, the ``TimeSeriesPredictor`` will fit a simple weighted ensemble on top of the models specified via
             ``hyperparameters``.
@@ -713,14 +717,20 @@
                     "\tSetting num_val_windows = 0 (disabling backtesting on train_data) because tuning_data is provided."
                 )
                 num_val_windows = 0
 
         if num_val_windows == 0 and tuning_data is None:
             raise ValueError("Please set num_val_windows >= 1 or provide custom tuning_data")
 
+        if num_val_windows <= 1 and refit_every_n_windows > 1:
+            logger.warning(
+                f"\trefit_every_n_windows provided as {refit_every_n_windows} but num_val_windows is set to {num_val_windows}."
+                " Refit_every_n_windows will have no effect."
+            )
+
         if not skip_model_selection:
             train_data = self._filter_useless_train_data(
                 train_data, num_val_windows=num_val_windows, val_step_size=val_step_size
             )
 
         val_splitter = ExpandingWindowSplitter(
             prediction_length=self.prediction_length, num_val_windows=num_val_windows, val_step_size=val_step_size
```

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/utils/datetime/base.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/utils/datetime/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/utils/datetime/lags.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/utils/datetime/lags.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/utils/datetime/seasonality.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/utils/datetime/seasonality.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/utils/datetime/time_features.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/utils/datetime/time_features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/utils/features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/utils/forecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-1.1.0b20240414/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,22 +3,20 @@
 import io
 import logging
 import os
 import re
 import sys
 import warnings
 
-from statsmodels.tools.sm_exceptions import ConvergenceWarning, ValueWarning
-
 __all__ = ["warning_filter", "disable_root_logger", "disable_tqdm"]
 
 
 @contextlib.contextmanager
 def warning_filter(all_warnings: bool = False):
-    categories = [RuntimeWarning, UserWarning, ConvergenceWarning, ValueWarning, FutureWarning]
+    categories = [RuntimeWarning, UserWarning, FutureWarning]
     if all_warnings:
         categories.append(Warning)
     with warnings.catch_warnings():
         env_py_warnings = os.environ.get("PYTHONWARNINGS", "")
         for warning_category in categories:
             warnings.simplefilter("ignore", category=warning_category)
         try:
```

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-1.1.0b20240414/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 1.1.0b20240413
+Version: 1.1.0b20240414
 Summary: Fast and Accurate ML in 3 Lines of Code
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-1.1.0b20240414/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-1.1.0b20240413/src/autogluon.timeseries.egg-info/requires.txt` & `autogluon.timeseries-1.1.0b20240414/src/autogluon.timeseries.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,26 +3,25 @@
 scipy<1.13,>=1.5.4
 pandas<2.3.0,>=2.0.0
 torch<2.2,>=2.1
 lightning<2.2,>=2.1
 pytorch_lightning<2.2,>=2.1
 transformers[sentencepiece]<4.39.0,>=4.38.0
 accelerate<0.22.0,>=0.21.0
-statsmodels<0.15,>=0.13.0
 gluonts<0.14.4,>=0.14.0
 networkx<4,>=3.0
 statsforecast<1.5,>=1.4.0
 mlforecast<0.10.1,>=0.10.0
 utilsforecast<0.0.11,>=0.0.10
 tqdm<5,>=4.38
 orjson~=3.9
 tensorboard<3,>=2.9
-autogluon.core[raytune]==1.1.0b20240413
-autogluon.common==1.1.0b20240413
-autogluon.tabular[catboost,lightgbm,xgboost]==1.1.0b20240413
+autogluon.core[raytune]==1.1.0b20240414
+autogluon.common==1.1.0b20240414
+autogluon.tabular[catboost,lightgbm,xgboost]==1.1.0b20240414
 
 [all]
 optimum[onnxruntime]<1.19,>=1.17
 
 [chronos-onnx]
 optimum[onnxruntime]<1.19,>=1.17
```

