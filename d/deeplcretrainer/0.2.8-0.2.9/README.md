# Comparing `tmp/deeplcretrainer-0.2.8.tar.gz` & `tmp/deeplcretrainer-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplcretrainer-0.2.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "deeplcretrainer-0.2.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `deeplcretrainer-0.2.8.tar` & `deeplcretrainer-0.2.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1928 2023-09-18 11:13:17.689519 deeplcretrainer-0.2.8/.gitignore
--rw-r--r--   0        0        0    11558 2023-09-18 11:13:17.689519 deeplcretrainer-0.2.8/LICENSE
--rw-r--r--   0        0        0       17 2023-09-18 11:13:17.690519 deeplcretrainer-0.2.8/README.md
--rw-r--r--   0        0        0       48 2023-11-15 08:41:28.826809 deeplcretrainer-0.2.8/deeplcretrainer/__init__.py
--rw-r--r--   0        0        0    40234 2023-11-15 08:36:32.117753 deeplcretrainer-0.2.8/deeplcretrainer/cnn_functions.py
--rw-r--r--   0        0        0    18047 2023-11-15 08:41:25.624407 deeplcretrainer-0.2.8/deeplcretrainer/deeplcretrainer.py
--rw-r--r--   0        0        0      581 2023-09-18 11:13:17.691519 deeplcretrainer-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      487 1970-01-01 00:00:00.000000 deeplcretrainer-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1928 2023-09-18 11:13:17.689519 deeplcretrainer-0.2.9/.gitignore
+-rw-r--r--   0        0        0    11558 2023-09-18 11:13:17.689519 deeplcretrainer-0.2.9/LICENSE
+-rw-r--r--   0        0        0       17 2023-09-18 11:13:17.690519 deeplcretrainer-0.2.9/README.md
+-rw-r--r--   0        0        0       48 2024-02-16 12:53:27.621941 deeplcretrainer-0.2.9/deeplcretrainer/__init__.py
+-rw-r--r--   0        0        0    36170 2024-02-16 12:52:29.105582 deeplcretrainer-0.2.9/deeplcretrainer/cnn_functions.py
+-rw-r--r--   0        0        0    17625 2024-02-16 12:52:50.008454 deeplcretrainer-0.2.9/deeplcretrainer/deeplcretrainer.py
+-rw-r--r--   0        0        0      761 2024-02-16 12:49:12.931295 deeplcretrainer-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 deeplcretrainer-0.2.9/PKG-INFO
```

### Comparing `deeplcretrainer-0.2.8/.gitignore` & `deeplcretrainer-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `deeplcretrainer-0.2.8/LICENSE` & `deeplcretrainer-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `deeplcretrainer-0.2.8/deeplcretrainer/cnn_functions.py` & `deeplcretrainer-0.2.9/deeplcretrainer/cnn_functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,82 +10,50 @@
     "Prof. Lennart Martens",
     "Prof. Sven Degroeve",
 ]
 __license__ = "Apache License, Version 2.0"
 __maintainer__ = ["Robbin Bouwmeester", "Ralf Gabriels"]
 __email__ = ["Robbin.Bouwmeester@ugent.be", "Ralf.Gabriels@ugent.be"]
 
+import matplotlib
 import numpy as np
 import pandas as pd
 
-import matplotlib
-
 matplotlib.use("Agg")
 
-from matplotlib import pyplot as plt
-import random
-import os
 import math
-
-import time
-
-from joblib import Parallel, delayed
 import multiprocessing
-import itertools
-
-from sklearn.preprocessing import OneHotEncoder
-from sklearn.metrics import roc_auc_score
-from sklearn.metrics import confusion_matrix
+import os
+import random
+import time
 
+import deeplc
+import scipy
 import tensorflow as tf
-from tensorflow.keras.utils import plot_model
+from deeplc.feat_extractor import FeatExtractor
+from psm_utils.io.peptide_record import peprec_to_proforma
+from psm_utils.psm import PSM
+from psm_utils.psm_list import PSMList
+from tensorflow.keras import regularizers
 from tensorflow.keras.layers import (
     Conv1D,
     Dense,
-    MaxPooling1D,
-    AveragePooling1D,
     Flatten,
-    Dropout,
-    GlobalMaxPooling1D,
-    GlobalAveragePooling1D,
+    Input,
+    MaxPooling1D,
+    concatenate,
 )
-from tensorflow.keras.layers import concatenate
-from tensorflow.keras.layers import Flatten
-from tensorflow.keras.layers import Input
-from tensorflow.keras.layers import BatchNormalization
-from tensorflow.keras.layers import LeakyReLU
-from tensorflow.keras.layers import Masking
-from tensorflow.keras.layers import Bidirectional
-from tensorflow.keras.layers import LSTM
-from tensorflow.keras import regularizers
-from tensorflow.keras.regularizers import l2
-from tensorflow.keras.regularizers import l1
 from tensorflow.keras.models import Model
-from tensorflow.keras.models import Sequential
-from tensorflow.keras.callbacks import ModelCheckpoint
-from tensorflow.keras.models import load_model
-from tensorflow.keras import initializers
-from deeplc.feat_extractor import FeatExtractor
-import deeplc
-
-# import xgboost as xgb
-from tensorflow.keras.layers import BatchNormalization
-from psm_utils.io.peptide_record import peprec_to_proforma
-from psm_utils.psm import PSM
-from psm_utils.psm_list import PSMList
-from psm_utils.io import read_file
-from psm_utils.io import write_file
-import scipy
 
-import tensorflow as tf
-
-from sklearn.metrics import roc_auc_score
-
-from tensorflow.keras.optimizers import Adam
-from multiprocessing import Pool
+try:
+    from matplotlib import pyplot as plt
+except ImportError:
+    _has_matplotlib = False
+else:
+    _has_matplotlib = True
 
 os.environ["CUDA_VISIBLE_DEVICES"] = "0"
 
 
 def read_infile(infile_loc):
     df = pd.read_csv(
         infile_loc,
@@ -1184,88 +1152,7 @@
     plt.scatter(pred_test, y, s=2)
     plt.xlabel("predicted tr")
     plt.ylabel("observed tr")
     plt.title("%s - mae: %s - R: %s" % (plot_title, round(mae, 3), round(corr, 4)))
     plt.plot([0, max(y)], [0, max(y)], c="grey")
     plt.savefig(file_save)
     plt.close()
-
-
-"""
-def write_preds(df,
-               X,
-               X_sum,
-               X_global,
-               X_hc,
-               X2,
-                X_sum2,
-                X_global2,
-                X_hc2,
-               mods,
-               fit_hc=True,
-               correction_factor=1.0,
-               outfile_name="outfile.csv"):
-    df = df.copy()
-
-    preds_test = []
-    for mod in mods:
-        if fit_hc: pred_test = mod.predict([X,X_sum,X_global,X_hc,X2,X_sum2,X_global2,X_hc2]) #*correction_factor #.flatten() #*correction_factor
-        else: pred_test = mod.predict([X,X_sum,X_global]).flatten()
-        preds_test.append(pred_test)
-    #pred_test = [float(sum(pred))/len(pred) for pred in list(zip(*preds_test))]
-
-    df["predictions_one"] = pred_test[:,0]
-    df["predictions_two"] = pred_test[:,1]
-    df["tr"] = df["tr"]
-    df.to_csv(outfile_name)
-
-    return(sum((df["tr"]-df["predictions_one"]).abs())/len(df.index))
-
-def plot_preds(X,
-               X_sum,
-               X_global,
-               X_hc,
-               X2,
-                X_sum2,
-                X_global2,
-                X_hc2,
-               y,
-               mods,
-               fit_hc=True,
-               correction_factor=1.0,
-               file_save="results.png",
-               plot_title="Plot title"):
-    try:
-        preds_test = []
-        for mod in mods:
-            if fit_hc: pred_test = mod.predict([X,X_sum,X_global,X_hc,X2,X_sum2,X_global2,X_hc2])
-            else: pred_test = mod.predict([X,X_sum,X_global,X2,X_sum2,X_global2,X_hc2])
-            preds_test.append(pred_test)
-        #pred_test = [float(sum(pred))/len(pred) for pred in list(zip(*preds_test))]
-    except:
-        if fit_hc: pred_test = mods.predict([X,X_sum,X_global,X_hc,X2,X_sum2,X_global2,X_hc2])
-        else: pred_test = mods.predict([X,X_sum,X_global,X2,X_sum2,X_global2,X_hc2])
-    
-    corr = scipy.stats.pearsonr(y[:,0],pred_test[:,0])[0]
-    mae = sum(abs(np.array(y[:,0])-pred_test[:,0])/len(pred_test[:,0]))
-
-    plt.figure(figsize=(10,8))
-    plt.scatter(y[:,0],pred_test[:,0],s=2)
-    plt.xlabel("predicted tr")
-    plt.ylabel("observed tr")
-    plt.title("%s - mae: %s - R: %s" % (plot_title,round(mae,3),round(corr,4)))
-    plt.plot([0,max(y[:,0])],[0,max(y[:,0])],c="grey")
-    plt.savefig(file_save)
-    plt.close()
-
-    corr = scipy.stats.pearsonr(y[:,1],pred_test[:,1])[0]
-    mae = sum(abs(np.array(y[:,0])-pred_test[:,1])/len(pred_test[:,1]))
-
-    plt.figure(figsize=(10,8))
-    plt.scatter(y[:,1],pred_test[:,1],s=2)
-    plt.xlabel("predicted tr")
-    plt.ylabel("observed tr")
-    plt.title("%s - mae: %s - R: %s" % (plot_title,round(mae,3),round(corr,4)))
-    plt.plot([0,max(y[:,1])],[0,max(y[:,1])],c="grey")
-    plt.savefig(file_save.replace(".png","")+"_std.png")
-    plt.close()
-"""
```

### Comparing `deeplcretrainer-0.2.8/deeplcretrainer/deeplcretrainer.py` & `deeplcretrainer-0.2.9/deeplcretrainer/deeplcretrainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,33 +10,30 @@
     "Prof. Lennart Martens",
     "Prof. Sven Degroeve",
 ]
 __license__ = "Apache License, Version 2.0"
 __maintainer__ = ["Robbin Bouwmeester", "Ralf Gabriels"]
 __email__ = ["Robbin.Bouwmeester@ugent.be", "Ralf.Gabriels@ugent.be"]
 
-from tensorflow.compat.v1 import ConfigProto
-from tensorflow.compat.v1 import InteractiveSession
-from tensorflow.keras.callbacks import ModelCheckpoint
-from tensorflow.keras.models import load_model
+import hashlib
+import itertools
+import os
+import tempfile
+
 import h5py
 import pandas as pd
-
-import sys
-from multiprocessing import freeze_support
-from pathlib import Path
-import importlib.resources
-from tensorflow.keras.layers import ReLU
-import importlib
-
-import tempfile
+from psm_utils.io.peptide_record import peprec_to_proforma
+from psm_utils.psm import PSM
+from psm_utils.psm_list import PSMList
+from tensorflow.compat.v1 import ConfigProto, InteractiveSession
+from tensorflow.keras.callbacks import ModelCheckpoint
+from tensorflow.keras.models import load_model
 
 try:
-    from gooey import Gooey, local_resource_path
-    from gooey import GooeyParser
+    from gooey import Gooey, GooeyParser
 except ImportError:
 
     def Gooey(
         program_name="DeepLC re-tR-ainer",
         default_size=(720, 790),
         monospace_display=True,
     ):
@@ -47,37 +44,20 @@
 
 
 try:
     from deeplcretrainer import cnn_functions
 except ImportError:
     import cnn_functions
 
-import itertools
-import hashlib
-
-import sys
-from argparse import HelpFormatter
-import os
-
-from psm_utils.io.peptide_record import peprec_to_proforma
-from psm_utils.psm import PSM
-from psm_utils.psm_list import PSMList
-from psm_utils.io import read_file
-from psm_utils.io import write_file
-
 config = ConfigProto()
 config.gpu_options.allow_growth = True
 session = InteractiveSession(config=config)
 
 import tensorflow as tf
 
-tf.__version__
-
-from . import __version__
-
 
 def parse_arguments(gui=False):
     """Read arguments from the CLI or GUI."""
     parser = GooeyParser(
         prog="DeepLC_retrain",
         description=(
             "Retention time prediction for (modified) peptides using deep " "learning."
```

### Comparing `deeplcretrainer-0.2.8/pyproject.toml` & `deeplcretrainer-0.2.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -5,12 +5,23 @@
 [project]
 name = "deeplcretrainer"
 authors = [{name = "Robbin Bouwmeester", email = "robbin.bouwmeester@ugent.be"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: Apache Software License"]
 dynamic = ["version", "description"]
+dependencies = [
+    "numpy",
+    "pandas",
+    "h5py",
+    "psm_utils",
+    "tensorflow",
+]
+
+[project.optional-dependencies]
+gui = ["gooey>=1.0"]
+plot = ["matplotlib"]
 
 [project.urls]
 Home = "https://github.com/RobbinBouwmeester"
 "Homepage" = "https://github.com/RobbinBouwmeester/DeepLCRetrainer"
 "Bug Tracker" = "https://github.com/RobbinBouwmeester/DeepLCRetrainer/issues"
```

