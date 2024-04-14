# Comparing `tmp/alignn-2024.3.4.tar.gz` & `tmp/alignn-2024.4.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alignn-2024.3.4.tar", last modified: Tue Mar 19 05:51:32 2024, max compression
+gzip compressed data, was "alignn-2024.4.10.tar", last modified: Sun Apr 14 14:33:06 2024, max compression
```

## Comparing `alignn-2024.3.4.tar` & `alignn-2024.4.10.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-19 05:51:32.203793 alignn-2024.3.4/
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1878 2024-03-18 20:13:24.000000 alignn-2024.3.4/LICENSE.rst
--rw-r--r--   0 knc6     (54782) 642div   (36677)    30391 2024-03-19 05:51:32.199793 alignn-2024.3.4/PKG-INFO
--rw-r--r--   0 knc6     (54782) 642div   (36677)    29406 2024-03-19 05:33:28.000000 alignn-2024.3.4/README.md
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-19 05:51:32.087793 alignn-2024.3.4/alignn/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       48 2024-03-18 20:13:33.000000 alignn-2024.3.4/alignn/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1871 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/cli.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     6022 2024-03-19 04:22:50.000000 alignn-2024.3.4/alignn/config.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    20309 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/data.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-19 05:51:32.107793 alignn-2024.3.4/alignn/ff/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       31 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/ff/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    50046 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/ff/ff.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    32087 2024-03-19 04:03:26.000000 alignn-2024.3.4/alignn/graphs.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-19 05:51:32.119793 alignn-2024.3.4/alignn/models/
--rw-r--r--   0 knc6     (54782) 642div   (36677)      402 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/models/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    11431 2024-03-18 20:13:33.000000 alignn-2024.3.4/alignn/models/alignn.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    19678 2024-03-19 04:03:51.000000 alignn-2024.3.4/alignn/models/alignn_atomwise.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1234 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/models/utils.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    13787 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/pretrained.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2454 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/profile.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     7857 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/run_alignn_ff.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-19 05:51:32.195793 alignn-2024.3.4/alignn/scripts/
--rw-r--r--   0 knc6     (54782) 642div   (36677)       27 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/__init__.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     4124 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/alignn_evac.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1586 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/all_train_cgcnn.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     3359 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/compare_cfid.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1437 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/cubic_mat_relax.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2188 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/defect.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1442 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/early_stopping_checker.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5445 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/ev_curve.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1593 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/ev_curve_comp.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1340 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/final_model.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)      382 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/graph_viz.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1923 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/make_test_split_cross_pred.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     4270 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/plot_ff_results.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2022 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/plot_phonons_ff.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1192 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/predict.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     2283 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/predict_db.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     4631 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/predict_db_all.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1315 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/train_all_hmof.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1297 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/train_all_hpov.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1725 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/train_all_jv.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1751 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/train_all_jv_class.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1737 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/train_all_jv_dal.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1376 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/train_all_mp.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1413 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/train_all_oqmd.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1242 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/train_all_pdbbind.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1427 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/train_all_qetb.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1336 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/train_all_qm9_jctc.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1411 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/train_all_qmof.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1924 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/train_cgcnn_repo.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1235 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/train_edos_pdos.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     4257 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/scripts/train_megnet.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    34111 2024-03-19 05:32:00.000000 alignn-2024.3.4/alignn/train.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)    13008 2024-03-19 05:00:13.000000 alignn-2024.3.4/alignn/train_alignn.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     5816 2024-03-18 20:13:24.000000 alignn-2024.3.4/alignn/train_props.py
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1178 2024-03-18 20:13:33.000000 alignn-2024.3.4/alignn/utils.py
-drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-03-19 05:51:32.195793 alignn-2024.3.4/alignn.egg-info/
--rw-r--r--   0 knc6     (54782) 642div   (36677)    30391 2024-03-19 05:51:31.000000 alignn-2024.3.4/alignn.egg-info/PKG-INFO
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1572 2024-03-19 05:51:31.000000 alignn-2024.3.4/alignn.egg-info/SOURCES.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)        1 2024-03-19 05:51:31.000000 alignn-2024.3.4/alignn.egg-info/dependency_links.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)      286 2024-03-19 05:51:31.000000 alignn-2024.3.4/alignn.egg-info/requires.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)        7 2024-03-19 05:51:31.000000 alignn-2024.3.4/alignn.egg-info/top_level.txt
--rw-r--r--   0 knc6     (54782) 642div   (36677)      295 2024-03-18 20:13:24.000000 alignn-2024.3.4/pyproject.toml
--rw-r--r--   0 knc6     (54782) 642div   (36677)       38 2024-03-19 05:51:32.203793 alignn-2024.3.4/setup.cfg
--rw-r--r--   0 knc6     (54782) 642div   (36677)     1483 2024-03-19 05:51:23.000000 alignn-2024.3.4/setup.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:33:06.568047 alignn-2024.4.10/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1878 2024-04-14 12:50:42.000000 alignn-2024.4.10/LICENSE.rst
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    30586 2024-04-14 14:33:06.564047 alignn-2024.4.10/PKG-INFO
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    29600 2024-04-14 12:50:42.000000 alignn-2024.4.10/README.md
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:33:06.468047 alignn-2024.4.10/alignn/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       49 2024-04-14 12:52:52.000000 alignn-2024.4.10/alignn/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1871 2024-04-14 12:50:42.000000 alignn-2024.4.10/alignn/cli.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     6022 2024-04-14 12:50:42.000000 alignn-2024.4.10/alignn/config.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    20309 2024-04-14 12:50:42.000000 alignn-2024.4.10/alignn/data.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:33:06.480047 alignn-2024.4.10/alignn/ff/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       31 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/ff/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    50046 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/ff/ff.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    32124 2024-04-14 12:51:53.000000 alignn-2024.4.10/alignn/graphs.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:33:06.492047 alignn-2024.4.10/alignn/models/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      402 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/models/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    11431 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/models/alignn.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    19678 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/models/alignn_atomwise.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1234 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/models/utils.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    14155 2024-04-14 13:06:36.000000 alignn-2024.4.10/alignn/pretrained.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2454 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/profile.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     7857 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/run_alignn_ff.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:33:06.556047 alignn-2024.4.10/alignn/scripts/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       27 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/__init__.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     4124 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/alignn_evac.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1586 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/all_train_cgcnn.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     3359 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/compare_cfid.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1437 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/cubic_mat_relax.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2188 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/defect.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1442 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/early_stopping_checker.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5445 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/ev_curve.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1593 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/ev_curve_comp.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1340 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/final_model.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      382 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/graph_viz.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1923 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/make_test_split_cross_pred.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     4270 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/plot_ff_results.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2022 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/plot_phonons_ff.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1192 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/predict.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     2283 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/predict_db.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     4631 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/predict_db_all.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1315 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/train_all_hmof.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1297 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/train_all_hpov.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1725 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/train_all_jv.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1751 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/train_all_jv_class.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1737 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/train_all_jv_dal.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1376 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/train_all_mp.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1413 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/train_all_oqmd.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1242 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/train_all_pdbbind.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1427 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/train_all_qetb.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1336 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/train_all_qm9_jctc.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1411 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/train_all_qmof.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1924 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/train_cgcnn_repo.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1235 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/train_edos_pdos.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     4257 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/scripts/train_megnet.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    34115 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/train.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    13015 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/train_alignn.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     5816 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/train_props.py
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1178 2024-04-14 12:50:43.000000 alignn-2024.4.10/alignn/utils.py
+drwxr-xr-x   0 knc6     (54782) 642div   (36677)        0 2024-04-14 14:33:06.560047 alignn-2024.4.10/alignn.egg-info/
+-rw-r--r--   0 knc6     (54782) 642div   (36677)    30586 2024-04-14 14:33:06.000000 alignn-2024.4.10/alignn.egg-info/PKG-INFO
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1572 2024-04-14 14:33:06.000000 alignn-2024.4.10/alignn.egg-info/SOURCES.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        1 2024-04-14 14:33:06.000000 alignn-2024.4.10/alignn.egg-info/dependency_links.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      286 2024-04-14 14:33:06.000000 alignn-2024.4.10/alignn.egg-info/requires.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)        7 2024-04-14 14:33:06.000000 alignn-2024.4.10/alignn.egg-info/top_level.txt
+-rw-r--r--   0 knc6     (54782) 642div   (36677)      295 2024-04-14 12:50:43.000000 alignn-2024.4.10/pyproject.toml
+-rw-r--r--   0 knc6     (54782) 642div   (36677)       38 2024-04-14 14:33:06.568047 alignn-2024.4.10/setup.cfg
+-rw-r--r--   0 knc6     (54782) 642div   (36677)     1484 2024-04-14 12:53:05.000000 alignn-2024.4.10/setup.py
```

### Comparing `alignn-2024.3.4/LICENSE.rst` & `alignn-2024.4.10/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/PKG-INFO` & `alignn-2024.4.10/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: alignn
-Version: 2024.3.4
+Version: 2024.4.10
 Summary: alignn
 Home-page: https://github.com/usnistgov/alignn
 Author: Kamal Choudhary, Brian DeCost
 Author-email: kamal.choudhary@nist.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 Requires-Dist: numpy<2.0.0,>=1.19.5
 Requires-Dist: scipy>=1.6.1
 Requires-Dist: jarvis-tools>=2021.07.19
-Requires-Dist: torch<=2.0.0
+Requires-Dist: torch>=2.0.0
 Requires-Dist: mpmath<=1.3.0
 Requires-Dist: dgl>=0.6.0
-Requires-Dist: spglib<=2.0.2
+Requires-Dist: spglib>=2.0.2
 Requires-Dist: scikit-learn>=0.22.2
 Requires-Dist: matplotlib>=3.4.1
 Requires-Dist: tqdm>=4.60.0
 Requires-Dist: pandas>=1.2.3
 Requires-Dist: pydantic>=1.8.1
 Requires-Dist: pydantic-settings
 Requires-Dist: flake8>=3.9.1
@@ -85,21 +85,23 @@
 Now,
 
 ```
 bash Miniconda3-latest-Linux-x86_64.sh (for linux)
 bash Miniconda3-latest-MacOSX-x86_64.sh (for Mac)
 ```
 Download 32/64 bit python 3.10 miniconda exe and install (for windows)
-Now, let's make a conda environment, say "version", choose other name as you like::
+Now, let's make a conda environment, say "my_alignn", choose other name as you like::
 ```
-conda create --name version python=3.10
-source activate version
+conda create --name my_alignn python=3.10
+conda activate my_alignn
+conda install alignn
 ```
+Starting version 2024.3.24, we have developed a conda package for alignn: [https://anaconda.org/conda-forge/alignn](https://anaconda.org/conda-forge/alignn)
 
-#### optional GPU dependencies
+#### optional GPU dependencies notes
 
 If you need CUDA support, it's best to install PyTorch and DGL before installing alignn to ensure that you get a CUDA-enabled version of DGL.
 
 To [install the stable release of PyTorch] on linux with cudatoolkit 11.8 run
 
 ```
 conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia
@@ -116,15 +118,15 @@
 ```
 conda install -c dglteam/label/cu118 dgl==1.0.2.cu118
 ```
 
 
 #### Method 1 (editable in-place install)
 
-You can install a development version of alignn by cloning the repository and installing in place with pip:
+You can laso install a development version of alignn by cloning the repository and installing in place with pip:
 
 ```
 git clone https://github.com/usnistgov/alignn
 cd alignn
 python -m pip install -e .
 ```
```

### Comparing `alignn-2024.3.4/README.md` & `alignn-2024.4.10/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -53,21 +53,23 @@
 Now,
 
 ```
 bash Miniconda3-latest-Linux-x86_64.sh (for linux)
 bash Miniconda3-latest-MacOSX-x86_64.sh (for Mac)
 ```
 Download 32/64 bit python 3.10 miniconda exe and install (for windows)
-Now, let's make a conda environment, say "version", choose other name as you like::
+Now, let's make a conda environment, say "my_alignn", choose other name as you like::
 ```
-conda create --name version python=3.10
-source activate version
+conda create --name my_alignn python=3.10
+conda activate my_alignn
+conda install alignn
 ```
+Starting version 2024.3.24, we have developed a conda package for alignn: [https://anaconda.org/conda-forge/alignn](https://anaconda.org/conda-forge/alignn)
 
-#### optional GPU dependencies
+#### optional GPU dependencies notes
 
 If you need CUDA support, it's best to install PyTorch and DGL before installing alignn to ensure that you get a CUDA-enabled version of DGL.
 
 To [install the stable release of PyTorch] on linux with cudatoolkit 11.8 run
 
 ```
 conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia
@@ -84,15 +86,15 @@
 ```
 conda install -c dglteam/label/cu118 dgl==1.0.2.cu118
 ```
 
 
 #### Method 1 (editable in-place install)
 
-You can install a development version of alignn by cloning the repository and installing in place with pip:
+You can laso install a development version of alignn by cloning the repository and installing in place with pip:
 
 ```
 git clone https://github.com/usnistgov/alignn
 cd alignn
 python -m pip install -e .
 ```
```

### Comparing `alignn-2024.3.4/alignn/cli.py` & `alignn-2024.4.10/alignn/cli.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/config.py` & `alignn-2024.4.10/alignn/config.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/data.py` & `alignn-2024.4.10/alignn/data.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/ff/ff.py` & `alignn-2024.4.10/alignn/ff/ff.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/graphs.py` & `alignn-2024.4.10/alignn/graphs.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,15 +360,16 @@
         neighbor_strategy="k-nearest",
         cutoff=8.0,
         max_neighbors=12,
         atom_features="cgcnn",
         max_attempts=3,
         id: Optional[str] = None,
         compute_line_graph: bool = True,
-        use_canonize: bool = False,
+        use_canonize: bool = True,
+        # use_canonize: bool = False,
         use_lattice_prop: bool = False,
         cutoff_extra=3.5,
     ):
         """Obtain a DGLGraph for Atoms object."""
         # print('id',id)
         if neighbor_strategy == "k-nearest":
             edges = nearest_neighbor_edges(
```

### Comparing `alignn-2024.3.4/alignn/models/alignn.py` & `alignn-2024.4.10/alignn/models/alignn.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/models/alignn_atomwise.py` & `alignn-2024.4.10/alignn/models/alignn_atomwise.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/models/utils.py` & `alignn-2024.4.10/alignn/models/utils.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/pretrained.py` & `alignn-2024.4.10/alignn/pretrained.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 from alignn.models.alignn import ALIGNN, ALIGNNConfig
 from alignn.data import get_torch_dataset
 from torch.utils.data import DataLoader
 import tempfile
 import torch
 import sys
 import json
-
-# from jarvis.db.jsonutils import loadjson
 import argparse
 from jarvis.core.atoms import Atoms
-from jarvis.core.graphs import Graph
+from alignn.graphs import Graph
 from jarvis.db.jsonutils import dumpjson
 import pandas as pd
 
+# from jarvis.core.graphs import Graph
+
 tqdm.pandas()
 
 """
 Name of the model, figshare link, number of outputs,
 extra config params (optional)
 """
 # For ALIGNN-FF pretrained models see, alignn/ff/ff.py
@@ -61,14 +61,26 @@
         "https://figshare.com/ndownloader/files/31458718",
         1,
     ],
     "jv_n-powerfact_alignn": [
         "https://figshare.com/ndownloader/files/31458712",
         1,
     ],
+    "intermat_cbm": [
+        "https://figshare.com/ndownloader/files/45392908",
+        1,
+    ],
+    "intermat_vbm": [
+        "https://figshare.com/ndownloader/files/45392914",
+        1,
+    ],
+    "intermat_phi": [
+        "https://figshare.com/ndownloader/files/45392911",
+        1,
+    ],
     "jv_magmom_oszicar_alignn": [
         "https://figshare.com/ndownloader/files/31458685",
         1,
     ],
     "jv_kpoint_length_unit_alignn": [
         "https://figshare.com/ndownloader/files/31458682",
         1,
@@ -253,14 +265,17 @@
     cfg = []
     for i in names:
         if "checkpoint_" in i and "pt" in i:
             tmp = i
             chks.append(i)
         if "config.json" in i:
             cfg = i
+        if "best_model.pt" in i:
+            tmp = i
+            chks.append(i)
 
     print("Using chk file", tmp, "from ", chks)
     print("Path", os.path.abspath(path))
     print("Config", os.path.abspath(cfg))
     config = json.loads(zipfile.ZipFile(path).read(cfg))
     # print("Loading the zipfile...", zipfile.ZipFile(path).namelist())
     data = zipfile.ZipFile(path).read(tmp)
```

### Comparing `alignn-2024.3.4/alignn/profile.py` & `alignn-2024.4.10/alignn/profile.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/run_alignn_ff.py` & `alignn-2024.4.10/alignn/run_alignn_ff.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/alignn_evac.py` & `alignn-2024.4.10/alignn/scripts/alignn_evac.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/all_train_cgcnn.py` & `alignn-2024.4.10/alignn/scripts/all_train_cgcnn.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/compare_cfid.py` & `alignn-2024.4.10/alignn/scripts/compare_cfid.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/cubic_mat_relax.py` & `alignn-2024.4.10/alignn/scripts/cubic_mat_relax.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/defect.py` & `alignn-2024.4.10/alignn/scripts/defect.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/early_stopping_checker.py` & `alignn-2024.4.10/alignn/scripts/early_stopping_checker.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/ev_curve.py` & `alignn-2024.4.10/alignn/scripts/ev_curve.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/ev_curve_comp.py` & `alignn-2024.4.10/alignn/scripts/ev_curve_comp.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/final_model.py` & `alignn-2024.4.10/alignn/scripts/final_model.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/make_test_split_cross_pred.py` & `alignn-2024.4.10/alignn/scripts/make_test_split_cross_pred.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/plot_ff_results.py` & `alignn-2024.4.10/alignn/scripts/plot_ff_results.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/plot_phonons_ff.py` & `alignn-2024.4.10/alignn/scripts/plot_phonons_ff.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/predict.py` & `alignn-2024.4.10/alignn/scripts/predict.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/predict_db.py` & `alignn-2024.4.10/alignn/scripts/predict_db.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/predict_db_all.py` & `alignn-2024.4.10/alignn/scripts/predict_db_all.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/train_all_hmof.py` & `alignn-2024.4.10/alignn/scripts/train_all_hmof.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/train_all_hpov.py` & `alignn-2024.4.10/alignn/scripts/train_all_hpov.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/train_all_jv.py` & `alignn-2024.4.10/alignn/scripts/train_all_jv.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/train_all_jv_class.py` & `alignn-2024.4.10/alignn/scripts/train_all_jv_class.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/train_all_jv_dal.py` & `alignn-2024.4.10/alignn/scripts/train_all_jv_dal.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/train_all_mp.py` & `alignn-2024.4.10/alignn/scripts/train_all_mp.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/train_all_oqmd.py` & `alignn-2024.4.10/alignn/scripts/train_all_oqmd.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/train_all_pdbbind.py` & `alignn-2024.4.10/alignn/scripts/train_all_pdbbind.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/train_all_qetb.py` & `alignn-2024.4.10/alignn/scripts/train_all_qetb.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/train_all_qm9_jctc.py` & `alignn-2024.4.10/alignn/scripts/train_all_qm9_jctc.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/train_all_qmof.py` & `alignn-2024.4.10/alignn/scripts/train_all_qmof.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/train_cgcnn_repo.py` & `alignn-2024.4.10/alignn/scripts/train_cgcnn_repo.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/train_edos_pdos.py` & `alignn-2024.4.10/alignn/scripts/train_edos_pdos.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/scripts/train_megnet.py` & `alignn-2024.4.10/alignn/scripts/train_megnet.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/train.py` & `alignn-2024.4.10/alignn/train.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,16 +114,16 @@
             print(config)
             config = TrainingConfig(**config)
         except Exception as exp:
             print("Check", exp)
 
     if not os.path.exists(config.output_dir):
         os.makedirs(config.output_dir)
-    checkpoint_dir = os.path.join(config.output_dir)
-    deterministic = False
+    # checkpoint_dir = os.path.join(config.output_dir)
+    # deterministic = False
     classification = False
     print("config:")
     tmp = config.dict()
     f = open(os.path.join(config.output_dir, "config.json"), "w")
     f.write(json.dumps(tmp, indent=4))
     f.close()
     global tmp_output_dir
```

### Comparing `alignn-2024.3.4/alignn/train_alignn.py` & `alignn-2024.4.10/alignn/train_alignn.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,19 +248,19 @@
             info["extra_features"] = i["extra_features"]
         dataset.append(info)
     print("len dataset", len(dataset))
     del dat
     # multioutput = False
     lists_length_equal = True
     line_graph = False
-    alignn_models = {
-        # "alignn",
-        # "alignn_layernorm",
-        "alignn_atomwise",
-    }
+    # alignn_models = {
+    #    # "alignn",
+    #    # "alignn_layernorm",
+    #    "alignn_atomwise",
+    # }
 
     if config.model.alignn_layers > 0:
         line_graph = True
 
     if multioutput:
         print("multioutput", multioutput)
         lists_length_equal = False not in [
```

### Comparing `alignn-2024.3.4/alignn/train_props.py` & `alignn-2024.4.10/alignn/train_props.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn/utils.py` & `alignn-2024.4.10/alignn/utils.py`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/alignn.egg-info/PKG-INFO` & `alignn-2024.4.10/alignn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: alignn
-Version: 2024.3.4
+Version: 2024.4.10
 Summary: alignn
 Home-page: https://github.com/usnistgov/alignn
 Author: Kamal Choudhary, Brian DeCost
 Author-email: kamal.choudhary@nist.gov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 Requires-Dist: numpy<2.0.0,>=1.19.5
 Requires-Dist: scipy>=1.6.1
 Requires-Dist: jarvis-tools>=2021.07.19
-Requires-Dist: torch<=2.0.0
+Requires-Dist: torch>=2.0.0
 Requires-Dist: mpmath<=1.3.0
 Requires-Dist: dgl>=0.6.0
-Requires-Dist: spglib<=2.0.2
+Requires-Dist: spglib>=2.0.2
 Requires-Dist: scikit-learn>=0.22.2
 Requires-Dist: matplotlib>=3.4.1
 Requires-Dist: tqdm>=4.60.0
 Requires-Dist: pandas>=1.2.3
 Requires-Dist: pydantic>=1.8.1
 Requires-Dist: pydantic-settings
 Requires-Dist: flake8>=3.9.1
@@ -85,21 +85,23 @@
 Now,
 
 ```
 bash Miniconda3-latest-Linux-x86_64.sh (for linux)
 bash Miniconda3-latest-MacOSX-x86_64.sh (for Mac)
 ```
 Download 32/64 bit python 3.10 miniconda exe and install (for windows)
-Now, let's make a conda environment, say "version", choose other name as you like::
+Now, let's make a conda environment, say "my_alignn", choose other name as you like::
 ```
-conda create --name version python=3.10
-source activate version
+conda create --name my_alignn python=3.10
+conda activate my_alignn
+conda install alignn
 ```
+Starting version 2024.3.24, we have developed a conda package for alignn: [https://anaconda.org/conda-forge/alignn](https://anaconda.org/conda-forge/alignn)
 
-#### optional GPU dependencies
+#### optional GPU dependencies notes
 
 If you need CUDA support, it's best to install PyTorch and DGL before installing alignn to ensure that you get a CUDA-enabled version of DGL.
 
 To [install the stable release of PyTorch] on linux with cudatoolkit 11.8 run
 
 ```
 conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia
@@ -116,15 +118,15 @@
 ```
 conda install -c dglteam/label/cu118 dgl==1.0.2.cu118
 ```
 
 
 #### Method 1 (editable in-place install)
 
-You can install a development version of alignn by cloning the repository and installing in place with pip:
+You can laso install a development version of alignn by cloning the repository and installing in place with pip:
 
 ```
 git clone https://github.com/usnistgov/alignn
 cd alignn
 python -m pip install -e .
 ```
```

### Comparing `alignn-2024.3.4/alignn.egg-info/SOURCES.txt` & `alignn-2024.4.10/alignn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alignn-2024.3.4/setup.py` & `alignn-2024.4.10/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="alignn",
-    version="2024.3.4",
+    version="2024.4.10",
     author="Kamal Choudhary, Brian DeCost",
     author_email="kamal.choudhary@nist.gov",
     description="alignn",
     install_requires=[
         "numpy>=1.19.5,<2.0.0",
         "scipy>=1.6.1",
         "jarvis-tools>=2021.07.19",
-        "torch<=2.0.0",
+        "torch>=2.0.0",
         "mpmath<=1.3.0",
         "dgl>=0.6.0",
-        "spglib<=2.0.2",
+        "spglib>=2.0.2",
         "scikit-learn>=0.22.2",
         "matplotlib>=3.4.1",
         "tqdm>=4.60.0",
         "pandas>=1.2.3",
         "pydantic>=1.8.1",
         "pydantic-settings",
         "flake8>=3.9.1",
```

