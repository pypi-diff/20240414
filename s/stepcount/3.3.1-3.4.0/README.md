# Comparing `tmp/stepcount-3.3.1.tar.gz` & `tmp/stepcount-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stepcount-3.3.1.tar", last modified: Fri Apr 12 12:25:55 2024, max compression
+gzip compressed data, was "stepcount-3.4.0.tar", last modified: Sun Apr 14 06:26:52 2024, max compression
```

## Comparing `stepcount-3.3.1.tar` & `stepcount-3.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 miko      (1000) miko      (1000)        0 2024-04-12 12:25:55.123067 stepcount-3.3.1/
--rw-r--r--   0 miko      (1000) miko      (1000)     8026 2024-04-12 12:18:04.000000 stepcount-3.3.1/LICENSE.md
--rw-r--r--   0 miko      (1000) miko      (1000)     8200 2024-04-12 12:25:55.123067 stepcount-3.3.1/PKG-INFO
--rw-r--r--   0 miko      (1000) miko      (1000)     6395 2024-04-12 12:18:04.000000 stepcount-3.3.1/README.md
--rw-r--r--   0 miko      (1000) miko      (1000)     6814 2024-04-12 12:18:04.000000 stepcount-3.3.1/pyproject.toml
--rw-r--r--   0 miko      (1000) miko      (1000)       38 2024-04-12 12:25:55.123067 stepcount-3.3.1/setup.cfg
--rw-r--r--   0 miko      (1000) miko      (1000)     2912 2024-04-12 12:18:04.000000 stepcount-3.3.1/setup.py
-drwxr-xr-x   0 miko      (1000) miko      (1000)        0 2024-04-12 12:25:55.113067 stepcount-3.3.1/src/
-drwxr-xr-x   0 miko      (1000) miko      (1000)        0 2024-04-12 12:25:55.123067 stepcount-3.3.1/src/stepcount/
--rw-r--r--   0 miko      (1000) miko      (1000)      580 2024-04-12 12:18:04.000000 stepcount-3.3.1/src/stepcount/__init__.py
--rw-r--r--   0 miko      (1000) miko      (1000)      497 2024-04-12 12:25:55.123067 stepcount-3.3.1/src/stepcount/_version.py
--rw-r--r--   0 miko      (1000) miko      (1000)     5345 2024-04-12 12:18:04.000000 stepcount-3.3.1/src/stepcount/features.py
--rw-r--r--   0 miko      (1000) miko      (1000)     9731 2024-04-12 12:18:04.000000 stepcount-3.3.1/src/stepcount/hmm_utils.py
--rw-r--r--   0 miko      (1000) miko      (1000)    23294 2024-04-12 12:18:04.000000 stepcount-3.3.1/src/stepcount/models.py
--rw-r--r--   0 miko      (1000) miko      (1000)    11941 2024-04-12 12:18:04.000000 stepcount-3.3.1/src/stepcount/sslmodel.py
--rw-r--r--   0 miko      (1000) miko      (1000)    17801 2024-04-12 12:18:04.000000 stepcount-3.3.1/src/stepcount/stepcount.py
-drwxr-xr-x   0 miko      (1000) miko      (1000)        0 2024-04-12 12:25:55.113067 stepcount-3.3.1/src/stepcount/utils/
--rw-r--r--   0 miko      (1000) miko      (1000)      124 2024-04-12 12:18:04.000000 stepcount-3.3.1/src/stepcount/utils/__init__.py
--rw-r--r--   0 miko      (1000) miko      (1000)     1346 2024-04-12 12:18:04.000000 stepcount-3.3.1/src/stepcount/utils/collate_outputs.py
--rw-r--r--   0 miko      (1000) miko      (1000)     2807 2024-04-12 12:18:04.000000 stepcount-3.3.1/src/stepcount/utils/generate_commands.py
-drwxr-xr-x   0 miko      (1000) miko      (1000)        0 2024-04-12 12:25:55.113067 stepcount-3.3.1/src/stepcount.egg-info/
--rw-r--r--   0 miko      (1000) miko      (1000)     8200 2024-04-12 12:25:55.000000 stepcount-3.3.1/src/stepcount.egg-info/PKG-INFO
--rw-r--r--   0 miko      (1000) miko      (1000)      576 2024-04-12 12:25:55.000000 stepcount-3.3.1/src/stepcount.egg-info/SOURCES.txt
--rw-r--r--   0 miko      (1000) miko      (1000)        1 2024-04-12 12:25:55.000000 stepcount-3.3.1/src/stepcount.egg-info/dependency_links.txt
--rw-r--r--   0 miko      (1000) miko      (1000)      189 2024-04-12 12:25:55.000000 stepcount-3.3.1/src/stepcount.egg-info/entry_points.txt
--rw-r--r--   0 miko      (1000) miko      (1000)      385 2024-04-12 12:25:55.000000 stepcount-3.3.1/src/stepcount.egg-info/requires.txt
--rw-r--r--   0 miko      (1000) miko      (1000)       10 2024-04-12 12:25:55.000000 stepcount-3.3.1/src/stepcount.egg-info/top_level.txt
--rw-r--r--   0 miko      (1000) miko      (1000)    83607 2024-04-12 12:18:04.000000 stepcount-3.3.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:26:52.861367 stepcount-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-04-14 06:26:38.000000 stepcount-3.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-04-14 06:26:52.849367 stepcount-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-04-14 06:26:38.000000 stepcount-3.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-14 06:26:38.000000 stepcount-3.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 06:26:52.861367 stepcount-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-14 06:26:38.000000 stepcount-3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:26:52.849367 stepcount-3.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:26:52.861367 stepcount-3.4.0/src/stepcount/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-14 06:26:38.000000 stepcount-3.4.0/src/stepcount/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-14 06:26:52.861367 stepcount-3.4.0/src/stepcount/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-04-14 06:26:38.000000 stepcount-3.4.0/src/stepcount/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9731 2024-04-14 06:26:38.000000 stepcount-3.4.0/src/stepcount/hmm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23562 2024-04-14 06:26:38.000000 stepcount-3.4.0/src/stepcount/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11941 2024-04-14 06:26:38.000000 stepcount-3.4.0/src/stepcount/sslmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22140 2024-04-14 06:26:38.000000 stepcount-3.4.0/src/stepcount/stepcount.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:26:52.849367 stepcount-3.4.0/src/stepcount/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-14 06:26:38.000000 stepcount-3.4.0/src/stepcount/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-14 06:26:38.000000 stepcount-3.4.0/src/stepcount/utils/collate_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-14 06:26:38.000000 stepcount-3.4.0/src/stepcount/utils/generate_commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 06:26:52.849367 stepcount-3.4.0/src/stepcount.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7242 2024-04-14 06:26:52.000000 stepcount-3.4.0/src/stepcount.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-14 06:26:52.000000 stepcount-3.4.0/src/stepcount.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 06:26:52.000000 stepcount-3.4.0/src/stepcount.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-14 06:26:52.000000 stepcount-3.4.0/src/stepcount.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-14 06:26:52.000000 stepcount-3.4.0/src/stepcount.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 06:26:52.000000 stepcount-3.4.0/src/stepcount.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    83607 2024-04-14 06:26:39.000000 stepcount-3.4.0/versioneer.py
```

### Comparing `stepcount-3.3.1/LICENSE.md` & `stepcount-3.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stepcount-3.3.1/PKG-INFO` & `stepcount-3.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,27 @@
 Metadata-Version: 2.1
 Name: stepcount
-Version: 3.3.1
+Version: 3.4.0
 Summary: Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset
 Home-page: https://github.com/OxWearables/stepcount
 Download-URL: https://github.com/OxWearables/stepcount
 Author: Shing Chan, Scott Small, Gert Mertes, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE file.
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: actipy>=3.0.5
-Requires-Dist: numpy==1.24.*
-Requires-Dist: scipy==1.10.*
-Requires-Dist: pandas==2.0.*
-Requires-Dist: tqdm==4.64.*
-Requires-Dist: joblib==1.2.*
-Requires-Dist: scikit-learn==1.1.1
-Requires-Dist: imbalanced-learn==0.9.1
-Requires-Dist: hmmlearn==0.3.*
-Requires-Dist: torch==1.13.*
-Requires-Dist: torchvision==0.14.*
-Requires-Dist: transforms3d==0.4.*
 Provides-Extra: dev
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: autopep8; extra == "dev"
-Requires-Dist: ipython; extra == "dev"
-Requires-Dist: ipdb; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-Requires-Dist: tomli; extra == "dev"
-Requires-Dist: jupyter; extra == "dev"
-Requires-Dist: matplotlib; extra == "dev"
 Provides-Extra: docs
-Requires-Dist: sphinx>=4.2; extra == "docs"
-Requires-Dist: sphinx_rtd_theme>=1.0; extra == "docs"
-Requires-Dist: readthedocs-sphinx-search>=0.1; extra == "docs"
-Requires-Dist: sphinxcontrib-programoutput>=0.17; extra == "docs"
-Requires-Dist: docutils<0.18; extra == "docs"
+License-File: LICENSE.md
 
 # stepcount
 
 A Python package to estimate step counts from accelerometer data.
 
 The algorithm is tuned for wrist-worn AX3 data collected at 100 Hz, using data from the open-source [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7), making it compatible with the [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649).
```

### Comparing `stepcount-3.3.1/README.md` & `stepcount-3.4.0/README.md`

 * *Files identical despite different names*

### Comparing `stepcount-3.3.1/pyproject.toml` & `stepcount-3.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stepcount-3.3.1/setup.py` & `stepcount-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.3.1/src/stepcount/__init__.py` & `stepcount-3.4.0/src/stepcount/__init__.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.3.1/src/stepcount/features.py` & `stepcount-3.4.0/src/stepcount/features.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.3.1/src/stepcount/hmm_utils.py` & `stepcount-3.4.0/src/stepcount/hmm_utils.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.3.1/src/stepcount/models.py` & `stepcount-3.4.0/src/stepcount/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import warnings
 from copy import deepcopy
 from collections import defaultdict, Counter
 import torch
 import numpy as np
 import pandas as pd
 from scipy.signal import find_peaks
 from scipy.optimize import minimize
@@ -347,19 +348,26 @@
             Ypp = Yp
 
         self.hmms.fit(Ypp, Y, groups=groups)
 
         return self
 
     def predict(self, X, groups=None):
-        X_feats = batch_extract_features(X, self.sample_rate, n_jobs=self.n_jobs, verbose=self.verbose)
-        whr_ok = ~(np.isnan(X_feats).any(1))
+
+        if len(X) == 0:
+            warnings.warn("No data to predict")
+            return np.array([], dtype='int')
+
         W = np.zeros(len(X), dtype='int')  # nan defaults to non-walk
-        W[whr_ok] = (self.clf.predict_proba(X_feats[whr_ok])[:, 1] > self.thresh).astype('int')
+        X_feats = batch_extract_features(X, self.sample_rate, n_jobs=self.n_jobs, verbose=self.verbose)
+        ok = ~(np.isnan(X_feats).any(1))
+        if ok.any():
+            W[ok] = (self.clf.predict_proba(X_feats[ok])[:, 1] > self.thresh).astype('int')
         W = self.hmms.predict(W, groups=groups)
+
         return W
 
 
 class WalkDetectorSSL:
     def __init__(
             self,
             device='cpu',
@@ -442,14 +450,19 @@
         # move model to cpu to get a device-less state dict (prevents device conflicts when loading on cpu/gpu later)
         model.to('cpu')
         self.state_dict = model.state_dict()
 
         return self
 
     def predict(self, X, groups=None):
+
+        if len(X) == 0:
+            warnings.warn("No data to predict")
+            return np.array([], dtype='int')
+
         sslmodel.verbose = self.verbose
 
         dataset = sslmodel.NormalDataset(X, name='prediction')
         dataloader = DataLoader(
             dataset,
             batch_size=512,
             shuffle=False,
```

### Comparing `stepcount-3.3.1/src/stepcount/sslmodel.py` & `stepcount-3.4.0/src/stepcount/sslmodel.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.3.1/src/stepcount/stepcount.py` & `stepcount-3.4.0/src/stepcount/stepcount.py`

 * *Files 20% similar despite different names*

```diff
@@ -77,225 +77,315 @@
     model.wd.device = args.pytorch_device
 
     if verbose:
         print("Running step counter...")
     Y, W, T_steps = model.predict_from_frame(data)
 
     # Save step counts
-    Y.to_csv(f"{outdir}/{basename}-Steps.csv")
+    Y.to_csv(f"{outdir}/{basename}-Steps.csv.gz")
     # Save timestamps of each step
-    T_steps.to_csv(f"{outdir}/{basename}-StepTimes.csv", index=False)
+    T_steps.to_csv(f"{outdir}/{basename}-StepTimes.csv.gz", index=False)
 
-    # Summary
-    summary = summarize(Y, model.steptol)
-    summary['hourly'].to_csv(f"{outdir}/{basename}-HourlySteps.csv")
-    summary['daily_stats'].to_csv(f"{outdir}/{basename}-DailySteps.csv")
+    # ENMO summary
+    enmo_summary = summarize_enmo(data)
+    info['ENMO(mg)'] = enmo_summary['avg']
+    enmo_summary['minutely'].to_csv(f"{outdir}/{basename}-MinutelyENMO.csv.gz")
+    enmo_summary['hourly'].to_csv(f"{outdir}/{basename}-HourlyENMO.csv.gz")
+    enmo_summary['daily'].to_csv(f"{outdir}/{basename}-DailyENMO.csv.gz")
+
+    # ENMO summary, adjusted
+    enmo_summary_adj = summarize_enmo(data, adjust_estimates=True)
+    info['ENMOAdjusted(mg)'] = enmo_summary_adj['avg']
+    enmo_summary_adj['minutely'].to_csv(f"{outdir}/{basename}-MinutelyENMOAdjusted.csv.gz")
+    enmo_summary_adj['hourly'].to_csv(f"{outdir}/{basename}-HourlyENMOAdjusted.csv.gz")
+    enmo_summary_adj['daily'].to_csv(f"{outdir}/{basename}-DailyENMOAdjusted.csv.gz")
+
+    # Steps summary
+    summary = summarize_steps(Y, model.steptol)
+    summary['minutely'].to_csv(f"{outdir}/{basename}-MinutelySteps.csv.gz")
+    summary['hourly'].to_csv(f"{outdir}/{basename}-HourlySteps.csv.gz")
+    summary['daily'].to_csv(f"{outdir}/{basename}-DailySteps.csv.gz")
     info['TotalSteps'] = summary['total']
     info['StepsDayAvg'] = summary['daily_avg']
     info['StepsDayMed'] = summary['daily_med']
     info['StepsDayMin'] = summary['daily_min']
     info['StepsDayMax'] = summary['daily_max']
     info['TotalWalking(mins)'] = summary['total_walk']
     info['WalkingDayAvg(mins)'] = summary['daily_walk_avg']
     info['WalkingDayMed(mins)'] = summary['daily_walk_med']
     info['WalkingDayMin(mins)'] = summary['daily_walk_min']
     info['WalkingDayMax(mins)'] = summary['daily_walk_max']
     info['CadencePeak1(steps/min)'] = summary['cadence_peak1']
     info['CadencePeak30(steps/min)'] = summary['cadence_peak30']
-    info['StepsQ1DayAvgAt'] = summary['daily_QAt_avg']['StepsQ1At']
-    info['StepsQ2DayAvgAt'] = summary['daily_QAt_avg']['StepsQ2At']
-    info['StepsQ3DayAvgAt'] = summary['daily_QAt_avg']['StepsQ3At']
-    info['StepsQ1DayMedAt'] = summary['daily_QAt_med']['StepsQ1At']
-    info['StepsQ2DayMedAt'] = summary['daily_QAt_med']['StepsQ2At']
-    info['StepsQ3DayMedAt'] = summary['daily_QAt_med']['StepsQ3At']
-
-    # Impute missing periods & recalculate summary
-    summary_adj = summarize(Y, model.steptol, adjust_estimates=True)
-    summary_adj['hourly'].to_csv(f"{outdir}/{basename}-HourlyStepsAdjusted.csv")
-    summary_adj['daily_stats'].to_csv(f"{outdir}/{basename}-DailyStepsAdjusted.csv")
+    info['Cadence95th(steps/min)'] = summary['cadence_p95']
+    info['Steps5thDayAvgAt'] = summary['daily_ptile_at_avg']['p05_at']
+    info['Steps25thDayAvgAt'] = summary['daily_ptile_at_avg']['p25_at']
+    info['Steps50thDayAvgAt'] = summary['daily_ptile_at_avg']['p50_at']
+    info['Steps75thDayAvgAt'] = summary['daily_ptile_at_avg']['p75_at']
+    info['Steps95thDayAvgAt'] = summary['daily_ptile_at_avg']['p95_at']
+    info['Steps5thDayMedAt'] = summary['daily_ptile_at_med']['p05_at']
+    info['Steps25thDayMedAt'] = summary['daily_ptile_at_med']['p25_at']
+    info['Steps50thDayMedAt'] = summary['daily_ptile_at_med']['p50_at']
+    info['Steps75thDayMedAt'] = summary['daily_ptile_at_med']['p75_at']
+    info['Steps95thDayMedAt'] = summary['daily_ptile_at_med']['p95_at']
+
+    # Steps summary, adjusted
+    summary_adj = summarize_steps(Y, model.steptol, adjust_estimates=True)
+    summary_adj['minutely'].to_csv(f"{outdir}/{basename}-MinutelyStepsAdjusted.csv.gz")
+    summary_adj['hourly'].to_csv(f"{outdir}/{basename}-HourlyStepsAdjusted.csv.gz")
+    summary_adj['daily'].to_csv(f"{outdir}/{basename}-DailyStepsAdjusted.csv.gz")
     info['TotalStepsAdjusted'] = summary_adj['total']
     info['StepsDayAvgAdjusted'] = summary_adj['daily_avg']
     info['StepsDayMedAdjusted'] = summary_adj['daily_med']
     info['StepsDayMinAdjusted'] = summary_adj['daily_min']
     info['StepsDayMaxAdjusted'] = summary_adj['daily_max']
     info['TotalWalkingAdjusted(mins)'] = summary_adj['total_walk']
     info['WalkingDayAvgAdjusted(mins)'] = summary_adj['daily_walk_avg']
     info['WalkingDayMedAdjusted(mins)'] = summary_adj['daily_walk_med']
     info['WalkingDayMinAdjusted(mins)'] = summary_adj['daily_walk_min']
     info['WalkingDayMaxAdjusted(mins)'] = summary_adj['daily_walk_max']
     info['CadencePeak1Adjusted(steps/min)'] = summary_adj['cadence_peak1']
     info['CadencePeak30Adjusted(steps/min)'] = summary_adj['cadence_peak30']
-    info['StepsQ1DayAvgAdjustedAt'] = summary_adj['daily_QAt_avg']['StepsQ1At']
-    info['StepsQ2DayAvgAdjustedAt'] = summary_adj['daily_QAt_avg']['StepsQ2At']
-    info['StepsQ3DayAvgAdjustedAt'] = summary_adj['daily_QAt_avg']['StepsQ3At']
-    info['StepsQ1DayMedAdjustedAt'] = summary_adj['daily_QAt_med']['StepsQ1At']
-    info['StepsQ2DayMedAdjustedAt'] = summary_adj['daily_QAt_med']['StepsQ2At']
-    info['StepsQ3DayMedAdjustedAt'] = summary_adj['daily_QAt_med']['StepsQ3At']
+    info['Cadence95thAdjusted(steps/min)'] = summary_adj['cadence_p95']
+    info['Steps5thDayAvgAdjustedAt'] = summary_adj['daily_ptile_at_avg']['p05_at']
+    info['Steps25thDayAvgAdjustedAt'] = summary_adj['daily_ptile_at_avg']['p25_at']
+    info['Steps50thDayAvgAdjustedAt'] = summary_adj['daily_ptile_at_avg']['p50_at']
+    info['Steps75thDayAvgAdjustedAt'] = summary_adj['daily_ptile_at_avg']['p75_at']
+    info['Steps95thDayAvgAdjustedAt'] = summary_adj['daily_ptile_at_avg']['p95_at']
+    info['Steps5thDayMedAdjustedAt'] = summary_adj['daily_ptile_at_med']['p05_at']
+    info['Steps25thDayMedAdjustedAt'] = summary_adj['daily_ptile_at_med']['p25_at']
+    info['Steps50thDayMedAdjustedAt'] = summary_adj['daily_ptile_at_med']['p50_at']
+    info['Steps75thDayMedAdjustedAt'] = summary_adj['daily_ptile_at_med']['p75_at']
+    info['Steps95thDayMedAdjustedAt'] = summary_adj['daily_ptile_at_med']['p95_at']
 
     # Save info
     with open(f"{outdir}/{basename}-Info.json", 'w') as f:
         json.dump(info, f, indent=4, cls=NpEncoder)
 
     # Print
     print("\nSummary\n-------")
     print(json.dumps(info, indent=4, cls=NpEncoder))
     print("\nEstimated Daily Stats\n---------------------")
-    print(summary['daily_stats'])
+    print(summary['daily'])
     print("\nEstimated Daily Stats (Adjusted)\n---------------------")
-    print(summary_adj['daily_stats'])
+    print(summary_adj['daily'])
 
     after = time.time()
     print(f"Done! ({round(after - before,2)}s)")
 
 
-def summarize(Y, steptol=3, adjust_estimates=False):
+def summarize_enmo(data: pd.DataFrame, adjust_estimates=False):
+    """ Summarize ENMO data """
+
+    # Truncated ENMO: Euclidean norm minus one and clipped at zero
+    v = np.sqrt(data['x'] ** 2 + data['y'] ** 2 + data['z'] ** 2)
+    v = np.clip(v - 1, a_min=0, a_max=None)
+    v *= 1000  # convert to mg
+
+    if adjust_estimates:
+        v = impute_missing(v)
+        skipna = False
+    else:
+        # crude summary ignores missing data
+        skipna = True
+
+    def _mean(x):
+        if not skipna and x.isna().any():
+            return np.nan
+        return x.mean()
+
+    # steps
+    hourly = v.resample('H').agg(_mean).rename('ENMO(mg)')  # ENMO, hourly
+    daily = v.resample('D').agg(_mean).rename('ENMO(mg)')  # ENMO, daily
+    minutely = v.resample('T').agg(_mean).rename('ENMO(mg)')  # ENMO, minutely
+
+    # steps, daily stats
+    if not adjust_estimates:
+        avg = daily.mean()
+    else:
+        day_of_week = daily.groupby(daily.index.weekday).mean()
+        avg = day_of_week.mean()
+
+    return {
+        'avg': avg,
+        'hourly': hourly,
+        'daily': daily,
+        'minutely': minutely,
+    }
+
+
+def summarize_steps(Y, steptol=3, adjust_estimates=False):
+    """ Summarize step count data """
 
     if adjust_estimates:
         Y = impute_missing(Y)
         skipna = False
     else:
         # crude summary ignores missing data
         skipna = True
 
     def _sum(x):
-        x = x.to_numpy()
-        if skipna:
-            return np.nansum(x)
-        return np.sum(x)
+        if not skipna and x.isna().any():
+            return np.nan
+        return x.sum()
 
     def _max(x, n=1):
-        if skipna:
-            return x.nlargest(n, keep='all').mean()
-        elif x.isna().any():
+        if not skipna and x.isna().any():
+            return np.nan
+        return x.nlargest(n, keep='all').mean()
+
+    def _p95(x, steptol):
+        if not skipna and x.isna().any():
+            return np.nan
+        return x[x >= steptol].quantile(.95)
+
+    def _percentile_at(x, ps=(5, 25, 50, 75, 95)):
+        percentiles = {f'p{p:02}_at': np.nan for p in ps}
+        if not skipna and x.isna().any():
+            return percentiles
+        z = x.cumsum() / x.sum()
+        for p in ps:
+            try:
+                p_at = z[z >= p / 100].index[0]
+                p_at = p_at - p_at.floor('D')
+                percentiles[f'p{p:02}_at'] = p_at
+            except IndexError:
+                pass
+        return percentiles
+
+    def _tdelta_to_str(tdelta):
+        if pd.isna(tdelta):
             return np.nan
+        hours, rem = divmod(tdelta.seconds, 3600)
+        minutes, seconds = divmod(rem, 60)
+        return f"{hours:02}:{minutes:02}:{seconds:02}"
 
     # there's a bug with .resample().sum(skipna)
     # https://github.com/pandas-dev/pandas/issues/29382
 
     # steps
     total = np.round(Y.agg(_sum))  # total steps
-    hourly = Y.resample('H').agg(_sum).round().rename('Steps')  # steps, hourly
-    daily = Y.resample('D').agg(_sum).round().rename('Steps')  # steps, daily
-    minutely = Y.resample('T').agg(_sum).round().rename('Steps')  # steps, minutely
+    hourly = Y.resample('H').agg(_sum).rename('Steps')  # steps, hourly
+    daily = Y.resample('D').agg(_sum).rename('Steps')  # steps, daily
+    minutely = Y.resample('T').agg(_sum).rename('Steps')  # steps, minutely
 
     # steps, daily stats
     if not adjust_estimates:
         daily_avg = np.round(daily.mean())
-        daily_med = np.round(daily.median())
+        with warnings.catch_warnings():
+            warnings.filterwarnings('ignore', message='Mean of empty slice')
+            daily_med = np.round(daily.median())
         daily_min = np.round(daily.min())
         daily_max = np.round(daily.max())
     else:
-        weekdaily = daily.groupby(daily.index.weekday).mean()
-        daily_avg = np.round(weekdaily.mean())
-        daily_med = np.round(weekdaily.median())
-        daily_min = np.round(weekdaily.min())
-        daily_max = np.round(weekdaily.max())
+        day_of_week = daily.groupby(daily.index.weekday).mean()
+        daily_avg = np.round(day_of_week.mean())
+        with warnings.catch_warnings():
+            warnings.filterwarnings('ignore', message='Mean of empty slice')
+            daily_med = np.round(day_of_week.median())
+        daily_min = np.round(day_of_week.min())
+        daily_max = np.round(day_of_week.max())
 
     # walking
     dt = pd.Timedelta(infer_freq(Y.index)).seconds
     W = Y.mask(~Y.isna(), Y >= steptol)
     total_walk = np.round(W.agg(_sum) * dt / 60)
-    daily_walk = (W.resample('D').agg(_sum) * dt / 60).round().rename('Walk(mins)')
+    daily_walk = (W.resample('D').agg(_sum) * dt / 60).rename('Walk(mins)')
 
     # walking, daily stats
     if not adjust_estimates:
         daily_walk_avg = np.round(daily_walk.mean())
-        daily_walk_med = np.round(daily_walk.median())
+        with warnings.catch_warnings():
+            warnings.filterwarnings('ignore', message='Mean of empty slice')
+            daily_walk_med = np.round(daily_walk.median())
         daily_walk_min = np.round(daily_walk.min())
         daily_walk_max = np.round(daily_walk.max())
     else:
-        weekdaily_walk = daily_walk.groupby(daily_walk.index.weekday).mean()
-        daily_walk_avg = np.round(weekdaily_walk.mean())
-        daily_walk_med = np.round(weekdaily_walk.median())
-        daily_walk_min = np.round(weekdaily_walk.min())
-        daily_walk_max = np.round(weekdaily_walk.max())
+        day_of_week_walk = daily_walk.groupby(daily_walk.index.weekday).mean()
+        daily_walk_avg = np.round(day_of_week_walk.mean())
+        with warnings.catch_warnings():
+            warnings.filterwarnings('ignore', message='Mean of empty slice')
+            daily_walk_med = np.round(day_of_week_walk.median())
+        daily_walk_min = np.round(day_of_week_walk.min())
+        daily_walk_max = np.round(day_of_week_walk.max())
 
     # cadence https://jamanetwork.com/journals/jama/fullarticle/2763292
-    daily_cadence_peak1 = minutely.resample('D').agg(_max, n=1)
-    daily_cadence_peak30 = minutely.resample('D').agg(_max, n=30)
+    daily_cadence_peak1 = minutely.resample('D').agg(_max, n=1).rename('CadencePeak1')
+    daily_cadence_peak30 = minutely.resample('D').agg(_max, n=30).rename('CadencePeak30')
+    daily_cadence_p95 = minutely.resample('D').agg(_p95, steptol=steptol * 60 / dt).rename('Cadence95th')  # scale steptol to steps/min
     if not adjust_estimates:
         cadence_peak1 = np.round(daily_cadence_peak1.mean())
         cadence_peak30 = np.round(daily_cadence_peak30.mean())
+        cadence_p95 = np.round(daily_cadence_p95.mean())
     else:
-        weekdaily_cadence_peak1 = daily_cadence_peak1.groupby(daily_cadence_peak1.index.weekday).mean()
-        weekdaily_cadence_peak30 = daily_cadence_peak30.groupby(daily_cadence_peak30.index.weekday).mean()
-        cadence_peak1 = np.round(weekdaily_cadence_peak1.mean())
-        cadence_peak30 = np.round(weekdaily_cadence_peak30.mean())
-
-    # distributional features - quantiles
-    def _QAt(x):
-        na_return = {'StepsQ1At': np.nan, 'StepsQ2At': np.nan, 'StepsQ3At': np.nan}
-        if adjust_estimates and x.isna().any():
-            return na_return
-        z = x.cumsum() / x.sum()
-        try:
-            q1_at = z[z >= 0.25].index[0]
-            q1_at = q1_at - q1_at.floor('D')
-            q2_at = z[z >= 0.5].index[0]
-            q2_at = q2_at - q2_at.floor('D')
-            q3_at = z[z >= 0.75].index[0]
-            q3_at = q3_at - q3_at.floor('D')
-            return {'StepsQ1At': q1_at, 'StepsQ2At': q2_at, 'StepsQ3At': q3_at}
-        except IndexError:
-            return na_return
-
-    def _QAt_to_str(tdelta):
-        if pd.isna(tdelta):
-            return np.nan
-        hours, rem = divmod(tdelta.seconds, 3600)
-        minutes, seconds = divmod(rem, 60)
-        return f"{hours:02}:{minutes:02}:{seconds:02}"
-
-    daily_QAt = Y.groupby(pd.Grouper(freq='D')).apply(_QAt).unstack(1)
-    daily_QAt_avg = daily_QAt.mean()
-    daily_QAt_med = daily_QAt.median()
+        day_of_week_cadence_peak1 = daily_cadence_peak1.groupby(daily_cadence_peak1.index.weekday).mean()
+        day_of_week_cadence_peak30 = daily_cadence_peak30.groupby(daily_cadence_peak30.index.weekday).mean()
+        day_of_week_cadence_p95 = daily_cadence_p95.groupby(daily_cadence_p95.index.weekday).mean()
+        cadence_peak1 = np.round(day_of_week_cadence_peak1.mean())
+        cadence_peak30 = np.round(day_of_week_cadence_peak30.mean())
+        cadence_p95 = np.round(day_of_week_cadence_p95.mean())
+
+    daily_ptile_at = Y.groupby(pd.Grouper(freq='D')).apply(_percentile_at).unstack(1)
+    daily_ptile_at_avg = daily_ptile_at.mean()
+    daily_ptile_at_med = daily_ptile_at.median()
 
     # daily stats
-    daily_stats = pd.concat([
-        daily_walk,
-        daily,
-        daily_QAt.applymap(_QAt_to_str),
+    daily = pd.concat([
+        pd.to_numeric(daily_walk.round(), downcast='integer'),
+        pd.to_numeric(daily.round(), downcast='integer'),
+        pd.to_numeric(daily_cadence_peak1.round(), downcast='integer'),
+        pd.to_numeric(daily_cadence_peak30.round(), downcast='integer'),
+        pd.to_numeric(daily_cadence_p95.round(), downcast='integer'),
+        daily_ptile_at.rename(columns={
+            'p05_at': 'Steps5thAt',
+            'p25_at': 'Steps25thAt',
+            'p50_at': 'Steps50thAt',
+            'p75_at': 'Steps75thAt',
+            'p95_at': 'Steps95thAt'
+        }).applymap(_tdelta_to_str),
     ], axis=1)
 
     # convert units
     total = nanint(total)
-    hourly = pd.to_numeric(hourly, downcast='integer')
-    daily = pd.to_numeric(daily, downcast='integer')
+    minutely = pd.to_numeric(minutely.round(), downcast='integer')
+    hourly = pd.to_numeric(hourly.round(), downcast='integer')
     daily_avg = nanint(daily_avg)
     daily_med = nanint(daily_med)
     daily_min = nanint(daily_min)
     daily_max = nanint(daily_max)
     total_walk = nanint(total_walk)
-    daily_walk = pd.to_numeric(daily_walk, downcast='integer')
     daily_walk_avg = nanint(daily_walk_avg)
     daily_walk_med = nanint(daily_walk_med)
     daily_walk_min = nanint(daily_walk_min)
     daily_walk_max = nanint(daily_walk_max)
     cadence_peak1 = nanint(cadence_peak1)
     cadence_peak30 = nanint(cadence_peak30)
-    daily_QAt_avg = daily_QAt_avg.map(_QAt_to_str)
-    daily_QAt_med = daily_QAt_med.map(_QAt_to_str)
+    cadence_p95 = nanint(cadence_p95)
+    daily_ptile_at_avg = daily_ptile_at_avg.map(_tdelta_to_str)
+    daily_ptile_at_med = daily_ptile_at_med.map(_tdelta_to_str)
 
     return {
         'total': total,
+        'minutely': minutely,
         'hourly': hourly,
-        'daily_stats': daily_stats,
+        'daily': daily,
         'daily_avg': daily_avg,
         'daily_med': daily_med,
         'daily_min': daily_min,
         'daily_max': daily_max,
         'total_walk': total_walk,
         'daily_walk_avg': daily_walk_avg,
         'daily_walk_med': daily_walk_med,
         'daily_walk_min': daily_walk_min,
         'daily_walk_max': daily_walk_max,
         'cadence_peak1': cadence_peak1,
         'cadence_peak30': cadence_peak30,
-        'daily_QAt_avg': daily_QAt_avg,
-        'daily_QAt_med': daily_QAt_med,
+        'cadence_p95': cadence_p95,
+        'daily_ptile_at_avg': daily_ptile_at_avg,
+        'daily_ptile_at_med': daily_ptile_at_med,
     }
 
 
 def impute_missing(data: pd.DataFrame, extrapolate=True):
 
     if extrapolate:  # extrapolate beyond start/end times to have full 24h
         freq = infer_freq(data.index)
```

### Comparing `stepcount-3.3.1/src/stepcount/utils/collate_outputs.py` & `stepcount-3.4.0/src/stepcount/utils/collate_outputs.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.3.1/src/stepcount/utils/generate_commands.py` & `stepcount-3.4.0/src/stepcount/utils/generate_commands.py`

 * *Files identical despite different names*

### Comparing `stepcount-3.3.1/src/stepcount.egg-info/PKG-INFO` & `stepcount-3.4.0/src/stepcount.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,27 @@
 Metadata-Version: 2.1
 Name: stepcount
-Version: 3.3.1
+Version: 3.4.0
 Summary: Step counter for wrist-worn accelerometers compatible with the UK Biobank Accelerometer Dataset
 Home-page: https://github.com/OxWearables/stepcount
 Download-URL: https://github.com/OxWearables/stepcount
 Author: Shing Chan, Scott Small, Gert Mertes, Aiden Doherty
 Maintainer: Shing Chan
 Maintainer-email: shing.chan@ndph.ox.ac.uk
 License: See LICENSE file.
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.8, <3.11
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: actipy>=3.0.5
-Requires-Dist: numpy==1.24.*
-Requires-Dist: scipy==1.10.*
-Requires-Dist: pandas==2.0.*
-Requires-Dist: tqdm==4.64.*
-Requires-Dist: joblib==1.2.*
-Requires-Dist: scikit-learn==1.1.1
-Requires-Dist: imbalanced-learn==0.9.1
-Requires-Dist: hmmlearn==0.3.*
-Requires-Dist: torch==1.13.*
-Requires-Dist: torchvision==0.14.*
-Requires-Dist: transforms3d==0.4.*
 Provides-Extra: dev
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: autopep8; extra == "dev"
-Requires-Dist: ipython; extra == "dev"
-Requires-Dist: ipdb; extra == "dev"
-Requires-Dist: twine; extra == "dev"
-Requires-Dist: tomli; extra == "dev"
-Requires-Dist: jupyter; extra == "dev"
-Requires-Dist: matplotlib; extra == "dev"
 Provides-Extra: docs
-Requires-Dist: sphinx>=4.2; extra == "docs"
-Requires-Dist: sphinx_rtd_theme>=1.0; extra == "docs"
-Requires-Dist: readthedocs-sphinx-search>=0.1; extra == "docs"
-Requires-Dist: sphinxcontrib-programoutput>=0.17; extra == "docs"
-Requires-Dist: docutils<0.18; extra == "docs"
+License-File: LICENSE.md
 
 # stepcount
 
 A Python package to estimate step counts from accelerometer data.
 
 The algorithm is tuned for wrist-worn AX3 data collected at 100 Hz, using data from the open-source [OxWalk Dataset](https://ora.ox.ac.uk/objects/uuid:19d3cb34-e2b3-4177-91b6-1bad0e0163e7), making it compatible with the [UK Biobank Accelerometer Dataset](https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0169649).
```

### Comparing `stepcount-3.3.1/src/stepcount.egg-info/SOURCES.txt` & `stepcount-3.4.0/src/stepcount.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stepcount-3.3.1/versioneer.py` & `stepcount-3.4.0/versioneer.py`

 * *Files identical despite different names*

