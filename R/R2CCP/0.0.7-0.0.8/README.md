# Comparing `tmp/R2CCP-0.0.7-py3-none-any.whl.zip` & `tmp/R2CCP-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 12471 bytes, number of entries: 15
+Zip file size: 12587 bytes, number of entries: 15
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-04 22:41 R2CCP/__init__.py
 -rw-r--r--  2.0 unx     3479 b- defN 24-Jan-04 22:41 R2CCP/argparser.py
 -rw-r--r--  2.0 unx     3766 b- defN 24-Apr-12 03:40 R2CCP/cp.py
 -rw-r--r--  2.0 unx     1428 b- defN 24-Jan-04 22:41 R2CCP/data.py
--rw-r--r--  2.0 unx     7912 b- defN 24-Apr-12 03:40 R2CCP/main.py
+-rw-r--r--  2.0 unx     8018 b- defN 24-Apr-13 23:13 R2CCP/main.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-04 22:41 R2CCP/models/__init__.py
 -rw-r--r--  2.0 unx     1175 b- defN 24-Jan-04 22:41 R2CCP/models/callbacks.py
 -rw-r--r--  2.0 unx     1453 b- defN 24-Jan-04 22:41 R2CCP/models/mlp.py
 -rw-r--r--  2.0 unx     4388 b- defN 24-Jan-04 22:41 R2CCP/models/model.py
 -rw-r--r--  2.0 unx     1396 b- defN 24-Jan-04 22:41 R2CCP/models/transformer.py
--rw-r--r--  2.0 unx     1066 b- defN 24-Apr-12 03:49 R2CCP-0.0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     4890 b- defN 24-Apr-12 03:49 R2CCP-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 03:49 R2CCP-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 24-Apr-12 03:49 R2CCP-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1127 b- defN 24-Apr-12 03:49 R2CCP-0.0.7.dist-info/RECORD
-15 files, 32178 bytes uncompressed, 10635 bytes compressed:  66.9%
+-rw-r--r--  2.0 unx     1066 b- defN 24-Apr-13 23:14 R2CCP-0.0.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5187 b- defN 24-Apr-13 23:14 R2CCP-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-13 23:14 R2CCP-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 24-Apr-13 23:14 R2CCP-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1127 b- defN 24-Apr-13 23:14 R2CCP-0.0.8.dist-info/RECORD
+15 files, 32581 bytes uncompressed, 10751 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: R2CCP/models/model.py
 Comment: 
 
 Filename: R2CCP/models/transformer.py
 Comment: 
 
-Filename: R2CCP-0.0.7.dist-info/LICENSE
+Filename: R2CCP-0.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: R2CCP-0.0.7.dist-info/METADATA
+Filename: R2CCP-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: R2CCP-0.0.7.dist-info/WHEEL
+Filename: R2CCP-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: R2CCP-0.0.7.dist-info/top_level.txt
+Filename: R2CCP-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: R2CCP-0.0.7.dist-info/RECORD
+Filename: R2CCP-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## R2CCP/main.py

```diff
@@ -132,14 +132,17 @@
     
     def get_length(self, X):
         X_train, y_train, X_cal, y_cal = get_train_cal_data(self.train_X, self.train_y, self._args)
         intervals = get_cp_lists(self.scaler_X.transform(X), self._args, self.range_vals, X_cal, y_cal, self.model)
         actual_intervals = self.invert_intervals(intervals)
         return calc_lengths(actual_intervals)
 
+    def set_coverage_level(self, new_alpha):
+        setattr(self._args, "alpha", 1 - new_alpha)
+        
     def predict(self, X):
         if not hasattr(self, 'model'):
             raise Exception('Model not trained yet')
         all_vals = get_predictions(self.scaler_X.transform(X), self.model, self.range_vals)
         
         best_values = self.scaler_y.inverse_transform(np.asarray(all_vals).reshape(-1, 1))
         return best_values
```

## Comparing `R2CCP-0.0.7.dist-info/LICENSE` & `R2CCP-0.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `R2CCP-0.0.7.dist-info/METADATA` & `R2CCP-0.0.8.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: R2CCP
-Version: 0.0.7
+Version: 0.0.8
 Summary: R2CCP Package for Conformal Prediction
 Author: Etash Guha
 Author-email: etashguha@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
@@ -30,14 +30,21 @@
 Requires-Dist: mpmath
 
 # Overview
 This is a library for generating prediction sets for machine learning regression tasks. 
 We do this by first converting regression to a classification problem (divide the output space into 50 bins) and then using CP techniques for
 classification to obtain a conformal set.
 
+## Installation
+
+You can install by using pip.
+```
+pip install R2CCP
+```
+
 ## Get Started
 Our example file (example.py) provides a simple demonstration of how to use our R2CCP class for conformal prediction. At a high level, the basic steps are instantiating the model class, fitting against data, and analyzing the results. 
 ```
 # Import the model
 from R2CCP.main import R2CCP
 
 # Instiantiate the model
@@ -53,14 +60,19 @@
 print(f"Coverage: {np.mean(coverage)}, Length: {np.mean(length)}")
 
 # If you don't have labels, you can just use get_length
 length = model.get_length(X_test)
 
 # Get model predictions
 predictions = model.predict(X_test)
+
+# You can also change the desired coverage level
+model.set_coverage_level(.8)
+new_coverage, new_length = model.get_coverage_length(X_test, Y_test)
+print(f"New Coverage: {np.mean(coverage)}, New Length: {np.mean(length)}")
 ```
 
 Here, we give a small example on a regression problem. We first generate a synthetic dataset of features of labels. We then generate the conformal intervals from this dataset.
 
 ```
 from R2CCP.main import R2CCP
 import numpy as np
```

## Comparing `R2CCP-0.0.7.dist-info/RECORD` & `R2CCP-0.0.8.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 R2CCP/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 R2CCP/argparser.py,sha256=COH3i2xm6DF1fgrIj5nSYwCe1xaeh17osPRTCcamnEQ,3479
 R2CCP/cp.py,sha256=QgXUNETpZzlxS7RU6uStA4lPcAzOCzhus-ylcc7EeIE,3766
 R2CCP/data.py,sha256=6cV94WjWrCGkPZR3EejHtludlRiAHMVdytwMcRuQnvI,1428
-R2CCP/main.py,sha256=stG2bmaUodvpNDf08H_tsG9vAfVOg9YeapHM5FYJEpY,7912
+R2CCP/main.py,sha256=ES2szjyUA_wcUMM6JgSBLJfzz9fev_xyMlYhznk4_6Y,8018
 R2CCP/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 R2CCP/models/callbacks.py,sha256=gS8krj4v7Kqw2lR7n_UpgRns9kJecOegtelR6PRkelo,1175
 R2CCP/models/mlp.py,sha256=Zc8IT-ZI_jNbV3DX7DRVKqkMVN9xFVghPmq2jtuzi8Q,1453
 R2CCP/models/model.py,sha256=229uzve4lMvRf4oU8lergvNH_7-pfOsDwSWP37-bvPg,4388
 R2CCP/models/transformer.py,sha256=IbGDC6HVojGzful3Ny_R8ILu_Ajuu79jZwkXphZFNTg,1396
-R2CCP-0.0.7.dist-info/LICENSE,sha256=MuaEqpmBuZSU_yIcLOuGcqDBSp0hDpLws9HMfSXS3KE,1066
-R2CCP-0.0.7.dist-info/METADATA,sha256=74bMTyda9E9lVHWJwecVilIxZqgjo6oZgjdLH4S6TMk,4890
-R2CCP-0.0.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-R2CCP-0.0.7.dist-info/top_level.txt,sha256=rd-xnbTsoZleFkGR217O5tQXT3pw8mUDF_zXextPGPM,6
-R2CCP-0.0.7.dist-info/RECORD,,
+R2CCP-0.0.8.dist-info/LICENSE,sha256=MuaEqpmBuZSU_yIcLOuGcqDBSp0hDpLws9HMfSXS3KE,1066
+R2CCP-0.0.8.dist-info/METADATA,sha256=oSV8HRYeI-8a2NPCewMylRRHSYUmrEc3kTb5sLnAEoo,5187
+R2CCP-0.0.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+R2CCP-0.0.8.dist-info/top_level.txt,sha256=rd-xnbTsoZleFkGR217O5tQXT3pw8mUDF_zXextPGPM,6
+R2CCP-0.0.8.dist-info/RECORD,,
```

