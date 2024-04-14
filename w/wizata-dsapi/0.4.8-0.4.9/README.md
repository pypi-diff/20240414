# Comparing `tmp/wizata-dsapi-0.4.8.tar.gz` & `tmp/wizata-dsapi-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-0.4.8.tar", last modified: Tue Feb 27 11:09:00 2024, max compression
+gzip compressed data, was "wizata-dsapi-0.4.9.tar", last modified: Sat Mar  2 10:17:15 2024, max compression
```

## Comparing `wizata-dsapi-0.4.8.tar` & `wizata-dsapi-0.4.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-02-27 11:09:00.254179 wizata-dsapi-0.4.8/
--rw-r--r--   0 wizata.jph   (502) staff       (20)    11356 2023-07-20 17:32:08.000000 wizata-dsapi-0.4.8/LICENSE.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2024-02-27 11:09:00.254061 wizata-dsapi-0.4.8/PKG-INFO
--rw-r--r--   0 wizata.jph   (502) staff       (20)      315 2023-07-20 17:32:08.000000 wizata-dsapi-0.4.8/README.rst
--rw-r--r--   0 wizata.jph   (502) staff       (20)       38 2024-02-27 11:09:00.254225 wizata-dsapi-0.4.8/setup.cfg
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1444 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.8/setup.py
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-02-27 11:09:00.253297 wizata-dsapi-0.4.8/wizata_dsapi/
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1375 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.8/wizata_dsapi/__init__.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1340 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.8/wizata_dsapi/api_dto.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     6270 2024-02-27 11:00:19.000000 wizata-dsapi-0.4.8/wizata_dsapi/api_interface.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     3092 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.8/wizata_dsapi/business_label.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     7101 2024-02-20 13:36:21.000000 wizata-dsapi-0.4.8/wizata_dsapi/context.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     5588 2023-07-20 17:32:08.000000 wizata-dsapi-0.4.8/wizata_dsapi/dataframe_toolkit.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     8370 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.8/wizata_dsapi/datapoint.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2194 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.8/wizata_dsapi/ds_dataframe.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2772 2023-07-20 17:32:08.000000 wizata-dsapi-0.4.8/wizata_dsapi/dsapi_json_encoder.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    19290 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.8/wizata_dsapi/execution.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     4155 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.8/wizata_dsapi/experiment.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)      311 2023-11-24 08:24:01.000000 wizata-dsapi-0.4.8/wizata_dsapi/ilogger.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    10671 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.8/wizata_dsapi/mlmodel.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     1552 2023-07-20 17:32:08.000000 wizata-dsapi-0.4.8/wizata_dsapi/model_toolkit.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)      761 2023-11-24 08:24:01.000000 wizata-dsapi-0.4.8/wizata_dsapi/paged_query_result.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    19316 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.8/wizata_dsapi/pipeline.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     2434 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.8/wizata_dsapi/plot.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    19133 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.8/wizata_dsapi/request.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     8874 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.8/wizata_dsapi/script.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     5080 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.8/wizata_dsapi/solution_component.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    11723 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.8/wizata_dsapi/template.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)     5917 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.8/wizata_dsapi/twin.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    12376 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.8/wizata_dsapi/twinregistration.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)       22 2024-02-27 11:08:33.000000 wizata-dsapi-0.4.8/wizata_dsapi/version.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)      471 2023-07-20 17:32:08.000000 wizata-dsapi-0.4.8/wizata_dsapi/wizard_function.py
--rw-r--r--   0 wizata.jph   (502) staff       (20)    63507 2024-02-27 11:05:15.000000 wizata-dsapi-0.4.8/wizata_dsapi/wizata_dsapi_client.py
-drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-02-27 11:09:00.253912 wizata-dsapi-0.4.8/wizata_dsapi.egg-info/
--rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2024-02-27 11:09:00.000000 wizata-dsapi-0.4.8/wizata_dsapi.egg-info/PKG-INFO
--rw-r--r--   0 wizata.jph   (502) staff       (20)      933 2024-02-27 11:09:00.000000 wizata-dsapi-0.4.8/wizata_dsapi.egg-info/SOURCES.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)        1 2024-02-27 11:09:00.000000 wizata-dsapi-0.4.8/wizata_dsapi.egg-info/dependency_links.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)      585 2024-02-27 11:09:00.000000 wizata-dsapi-0.4.8/wizata_dsapi.egg-info/requires.txt
--rw-r--r--   0 wizata.jph   (502) staff       (20)       13 2024-02-27 11:09:00.000000 wizata-dsapi-0.4.8/wizata_dsapi.egg-info/top_level.txt
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-03-02 10:17:15.210280 wizata-dsapi-0.4.9/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    11356 2023-07-20 17:32:08.000000 wizata-dsapi-0.4.9/LICENSE.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2024-03-02 10:17:15.210150 wizata-dsapi-0.4.9/PKG-INFO
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      315 2023-07-20 17:32:08.000000 wizata-dsapi-0.4.9/README.rst
+-rw-r--r--   0 wizata.jph   (502) staff       (20)       38 2024-03-02 10:17:15.210339 wizata-dsapi-0.4.9/setup.cfg
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1444 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/setup.py
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-03-02 10:17:15.208738 wizata-dsapi-0.4.9/wizata_dsapi/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1375 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/__init__.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1340 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/api_dto.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     6270 2024-02-28 18:32:59.000000 wizata-dsapi-0.4.9/wizata_dsapi/api_interface.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     3092 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/business_label.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     7101 2024-02-20 13:36:21.000000 wizata-dsapi-0.4.9/wizata_dsapi/context.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     5588 2023-07-20 17:32:08.000000 wizata-dsapi-0.4.9/wizata_dsapi/dataframe_toolkit.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     8370 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/datapoint.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2194 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/ds_dataframe.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2772 2023-07-20 17:32:08.000000 wizata-dsapi-0.4.9/wizata_dsapi/dsapi_json_encoder.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    19290 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/execution.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     4155 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/experiment.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      311 2023-11-24 08:24:01.000000 wizata-dsapi-0.4.9/wizata_dsapi/ilogger.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    11814 2024-03-02 10:16:09.000000 wizata-dsapi-0.4.9/wizata_dsapi/mlmodel.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1552 2023-07-20 17:32:08.000000 wizata-dsapi-0.4.9/wizata_dsapi/model_toolkit.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      761 2023-11-24 08:24:01.000000 wizata-dsapi-0.4.9/wizata_dsapi/paged_query_result.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    19316 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/pipeline.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2464 2024-02-28 18:33:10.000000 wizata-dsapi-0.4.9/wizata_dsapi/plot.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    19133 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/request.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     8874 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/script.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     5080 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/solution_component.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    11723 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/template.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     5917 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/twin.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    12376 2024-02-20 15:47:02.000000 wizata-dsapi-0.4.9/wizata_dsapi/twinregistration.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)       22 2024-03-02 10:16:49.000000 wizata-dsapi-0.4.9/wizata_dsapi/version.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      471 2023-07-20 17:32:08.000000 wizata-dsapi-0.4.9/wizata_dsapi/wizard_function.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    63507 2024-02-28 18:32:59.000000 wizata-dsapi-0.4.9/wizata_dsapi/wizata_dsapi_client.py
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2024-03-02 10:17:15.209967 wizata-dsapi-0.4.9/wizata_dsapi.egg-info/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2024-03-02 10:17:15.000000 wizata-dsapi-0.4.9/wizata_dsapi.egg-info/PKG-INFO
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      933 2024-03-02 10:17:15.000000 wizata-dsapi-0.4.9/wizata_dsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)        1 2024-03-02 10:17:15.000000 wizata-dsapi-0.4.9/wizata_dsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      585 2024-03-02 10:17:15.000000 wizata-dsapi-0.4.9/wizata_dsapi.egg-info/requires.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)       13 2024-03-02 10:17:15.000000 wizata-dsapi-0.4.9/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.4.8/LICENSE.txt` & `wizata-dsapi-0.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/setup.py` & `wizata-dsapi-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi/__init__.py` & `wizata-dsapi-0.4.9/wizata_dsapi/__init__.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi/api_dto.py` & `wizata-dsapi-0.4.9/wizata_dsapi/api_dto.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi/api_interface.py` & `wizata-dsapi-0.4.9/wizata_dsapi/api_interface.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi/business_label.py` & `wizata-dsapi-0.4.9/wizata_dsapi/business_label.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi/context.py` & `wizata-dsapi-0.4.9/wizata_dsapi/context.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-0.4.9/wizata_dsapi/dataframe_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi/datapoint.py` & `wizata-dsapi-0.4.9/wizata_dsapi/datapoint.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-0.4.9/wizata_dsapi/ds_dataframe.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi/dsapi_json_encoder.py` & `wizata-dsapi-0.4.9/wizata_dsapi/dsapi_json_encoder.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi/execution.py` & `wizata-dsapi-0.4.9/wizata_dsapi/execution.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi/experiment.py` & `wizata-dsapi-0.4.9/wizata_dsapi/experiment.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi/mlmodel.py` & `wizata-dsapi-0.4.9/wizata_dsapi/mlmodel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,102 +1,145 @@
 import json
 import uuid
 from .api_dto import ApiDto
 from enum import Enum
 
 
-class ModelKeyType(Enum):
-    DIRECT = "direct"
-    TEMPLATE = "template"
-    VARIABLE = "variable"
+def get_bool(obj, name: str):
+    if isinstance(obj[name], str) and obj[name].lower() == "false":
+        return False
+    else:
+        return bool(obj[name])
 
 
 class MLModelConfig(ApiDto):
     """
     a model config defines execution properties for a specific model.
     usually to define how a pipeline should train and predict your model.
 
     :ivar train_script: name of function referencing the script to train the model.
     :ivar train_test_split_pct: percentage repartition to split the data for training and scoring.
     :ivar target_feat: target feature name if existing.
     :ivar features: filter list of datapoint columns if necessary.
     :ivar train_test_split_type: name of function referencing the script to train the model.
     :ivar model_key: key of the model to store (or use story property if dynamic).
-    :ivar model_key_type: ModelKeyType by default at DIRECT. Use TEMPLATE or VARIABLE to get key from another source.
     :ivar output_property: name of dataframe column where to store results (or template property).
     """
 
     def __init__(self,
                  train_script=None,
                  train_test_split_pct: float = 1.0,
+                 train_test_split_type: str = "ignore",
+                 function: str = "predict",
                  target_feat: str = None,
+                 output_property: str = "result",
                  features: list = None,
-                 train_test_split_type: str = "ignore",
                  model_key: str = None,
-                 model_key_type: ModelKeyType = ModelKeyType.DIRECT,
-                 output_property: str = "result",
-                 function: str = "predict"):
+                 by_twin: bool = False,
+                 by_property: bool = True,
+                 property_name: str = None,
+                 source: str = "wizata"
+                 ):
+
+        # training
         self.train_script = train_script
         self.train_test_split_pct = train_test_split_pct
         self.train_test_split_type = train_test_split_type
+        self.function = function
+
+        # features management
         self.target_feat = target_feat
         self.features = features
-        self.model_key_type = model_key_type
-        self.model_key = model_key
         self.output_property = output_property
-        self.function = function
+
+        # key and identification
+        self.model_key = model_key
+        self.by_twin = by_twin
+        self.by_property = by_property
+        self.property_name = property_name
+
+        # source
+        self.source = source
 
     def from_json(self, obj):
+
+        # blocking old configs
+        if "store_property" in obj.keys():
+            raise ValueError("deprecated and unsupported configuration 'store_property'")
+        if "model_key_type" in obj.keys():
+            raise ValueError("deprecated and unsupported configuration 'model_key_type'")
+
+        # training info
         if "train_script" in obj.keys() and obj["train_script"] is not None:
             self.train_script = obj["train_script"]
         if "train_test_split_pct" in obj.keys() and obj["train_test_split_pct"] is not None:
             self.train_test_split_pct = float(obj["train_test_split_pct"])
         if "train_test_split_type" in obj.keys() and obj["train_test_split_type"] is not None:
             self.train_test_split_type = obj["train_test_split_type"]
+        if "function" in obj.keys() and obj["function"] is not None:
+            self.function = obj["function"]
+
+        # features info
         if "target_feat" in obj.keys() and obj["target_feat"] is not None:
             self.target_feat = obj["target_feat"]
         if "features" in obj.keys() and obj["features"] is not None:
             self.features = obj["features"]
+        if "output_property" in obj.keys() and obj["output_property"] is not None:
+            self.output_property = obj["output_property"]
 
-        if "store_property" in obj.keys() and obj["store_property"] is not None:
-            self.model_key = obj["store_property"]
-            self.model_key_type = ModelKeyType.TEMPLATE
-        elif "model_key" in obj.keys() and obj["model_key"] is not None:
-            self.model_key = obj["model_key"]
-            if "model_key_type" in obj.keys():
-                self.model_key_type = ModelKeyType(obj["model_key_type"])
+        # source
+        if "source" in obj.keys() and obj["source"] is not None:
+            self.source = obj["source"]
+            if self.source not in ["wizata", "mlflow"]:
+                raise ValueError("source must be wizata or mlflow")
 
-        if self.model_key is None:
+        # key and target
+        if "model_key" not in obj.keys() or obj["model_key"] is None:
             raise KeyError('model_key must be declared in the config.')
-
-        if "output_property" in obj.keys() and obj["output_property"] is not None:
-            self.output_property = obj["output_property"]
-        if "function" in obj.keys() and obj["function"] is not None:
-            self.function = obj["function"]
+        self.model_key = obj["model_key"]
+        if "by_twin" in obj.keys():
+            self.by_twin = get_bool(obj, name="by_twin")
+        if "by_property" in obj.keys():
+            self.by_property = get_bool(obj, name="by_property")
+        if "property_name" in obj.keys() and obj["property_name"] is not None:
+            self.property_name = obj["property_name"]
 
     def to_json(self, target: str = None):
-        obj = {}
+        obj = {
+            "source": self.source
+        }
+
+        # training info
         if self.train_script is not None:
             obj["train_script"] = str(self.train_script)
         if self.train_test_split_pct is not None:
             obj["train_test_split_pct"] = float(self.train_test_split_pct)
         if self.train_test_split_type is not None:
             obj["train_test_split_type"] = str(self.train_test_split_type)
-        if self.target_feat is not None:
-            obj["target_feat"] = str(self.target_feat)
         if self.features is not None:
             obj["features"] = self.features
-        if self.model_key_type is not None:
-            obj["model_key_type"] = str(self.model_key_type.value)
-        if self.model_key is not None:
-            obj["model_key"] = self.model_key
+
+        # features info
+        if self.target_feat is not None:
+            obj["target_feat"] = str(self.target_feat)
         if self.output_property is not None:
             obj["output_property"] = self.output_property
         if self.function is not None:
             obj["function"] = self.function
+
+        # key and target
+        if self.model_key is not None:
+            obj["model_key"] = self.model_key
+        if self.by_twin is not None:
+            obj["by_twin"] = str(self.by_twin)
+        if self.by_property is not None:
+            obj["by_property"] = str(self.by_property)
+        if self.property_name is not None:
+            obj["property_name"] = self.property_name
+
         return obj
 
 
 class MLModel(ApiDto):
     """
     A trained Machine Learning Model stored to be executed on demand.
     Can contain also a scaler, both object are stored as pickled file.
```

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-0.4.9/wizata_dsapi/model_toolkit.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi/paged_query_result.py` & `wizata-dsapi-0.4.9/wizata_dsapi/paged_query_result.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi/pipeline.py` & `wizata-dsapi-0.4.9/wizata_dsapi/pipeline.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi/plot.py` & `wizata-dsapi-0.4.9/wizata_dsapi/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 
     def __init__(self, plot_id=None, name=None, generated_by_id=None, figure=None):
         if plot_id is None:
             self.plot_id = uuid.uuid4()
         else:
             self.plot_id = plot_id
         self.name = name
-        self.generatedById = generated_by_id
+        self.generatedById = generated_by_id # Execution
+        # Step Id
         self.figure = figure
 
     def api_id(self) -> str:
         """
         Id of the plot (plot_id)
 
         :return: string formatted UUID of the plot.
```

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi/request.py` & `wizata-dsapi-0.4.9/wizata_dsapi/request.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi/script.py` & `wizata-dsapi-0.4.9/wizata_dsapi/script.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi/solution_component.py` & `wizata-dsapi-0.4.9/wizata_dsapi/solution_component.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi/template.py` & `wizata-dsapi-0.4.9/wizata_dsapi/template.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi/twin.py` & `wizata-dsapi-0.4.9/wizata_dsapi/twin.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi/twinregistration.py` & `wizata-dsapi-0.4.9/wizata_dsapi/twinregistration.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi/wizata_dsapi_client.py` & `wizata-dsapi-0.4.9/wizata_dsapi/wizata_dsapi_client.py`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-0.4.9/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wizata-dsapi-0.4.8/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-0.4.9/wizata_dsapi.egg-info/requires.txt`

 * *Files identical despite different names*

