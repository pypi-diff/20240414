# Comparing `tmp/iam_actions-1.2.20240413.tar.gz` & `tmp/iam_actions-1.2.20240414.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240413.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240414.tar", max compression
```

## Comparing `iam_actions-1.2.20240413.tar` & `iam_actions-1.2.20240414.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-04-13 02:07:31.146537 iam_actions-1.2.20240413/LICENSE
--rw-r--r--   0        0        0     2302 2024-04-13 02:07:31.146537 iam_actions-1.2.20240413/README.md
--rw-r--r--   0        0        0      228 2024-04-13 02:07:31.146537 iam_actions-1.2.20240413/iam_actions/__init__.py
--rw-r--r--   0        0        0  4798523 2024-04-13 02:09:50.594507 iam_actions-1.2.20240413/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-04-13 02:07:31.146537 iam_actions-1.2.20240413/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-04-13 02:07:31.146537 iam_actions-1.2.20240413/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-04-13 02:07:31.146537 iam_actions-1.2.20240413/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-04-13 02:07:31.146537 iam_actions-1.2.20240413/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-04-13 02:07:31.146537 iam_actions-1.2.20240413/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-04-13 02:07:31.146537 iam_actions-1.2.20240413/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-04-13 02:07:31.146537 iam_actions-1.2.20240413/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-04-13 02:07:31.146537 iam_actions-1.2.20240413/iam_actions/generate/services.py
--rw-r--r--   0        0        0   623594 2024-04-13 02:09:50.594507 iam_actions-1.2.20240413/iam_actions/policies.json
--rw-r--r--   0        0        0   208021 2024-04-13 02:09:50.594507 iam_actions-1.2.20240413/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   604984 2024-04-13 02:09:50.594507 iam_actions-1.2.20240413/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-04-13 02:09:51.290507 iam_actions-1.2.20240413/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240413/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240413/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-14 03:12:34.225473 iam_actions-1.2.20240414/LICENSE
+-rw-r--r--   0        0        0     2302 2024-04-14 03:12:34.225473 iam_actions-1.2.20240414/README.md
+-rw-r--r--   0        0        0      228 2024-04-14 03:12:34.225473 iam_actions-1.2.20240414/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4798523 2024-04-14 03:14:18.889612 iam_actions-1.2.20240414/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-04-14 03:12:34.225473 iam_actions-1.2.20240414/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-04-14 03:12:34.225473 iam_actions-1.2.20240414/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-04-14 03:12:34.225473 iam_actions-1.2.20240414/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-04-14 03:12:34.225473 iam_actions-1.2.20240414/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-04-14 03:12:34.225473 iam_actions-1.2.20240414/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-04-14 03:12:34.225473 iam_actions-1.2.20240414/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-04-14 03:12:34.225473 iam_actions-1.2.20240414/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-04-14 03:12:34.225473 iam_actions-1.2.20240414/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   623594 2024-04-14 03:14:18.889612 iam_actions-1.2.20240414/iam_actions/policies.json
+-rw-r--r--   0        0        0   208021 2024-04-14 03:14:18.889612 iam_actions-1.2.20240414/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   604984 2024-04-14 03:14:18.889612 iam_actions-1.2.20240414/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-04-14 03:14:19.541612 iam_actions-1.2.20240414/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240414/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240414/PKG-INFO
```

### Comparing `iam_actions-1.2.20240413/LICENSE` & `iam_actions-1.2.20240414/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240413/README.md` & `iam_actions-1.2.20240414/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240413/iam_actions/actions.json` & `iam_actions-1.2.20240414/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Ordering differences only*

```diff
@@ -4442,217 +4442,217 @@
             "resources": [
                 "application",
                 "configurationprofile"
             ]
         }
     },
     "appfabric": {
-        "UpdateIngestionDestination": {
+        "UpdateAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "UpdateIngestionDestination",
+            "action": "UpdateAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ConnectAppAuthorization": {
+        "CreateAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "ConnectAppAuthorization",
+            "action": "CreateAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIngestionDestination": {
+        "UpdateIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "GetIngestionDestination",
+            "action": "UpdateIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAppBundle": {
+        "CreateAppBundle": {
             "access_level": "Undocumented",
-            "action": "GetAppBundle",
+            "action": "CreateAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIngestions": {
+        "StopIngestion": {
             "access_level": "Undocumented",
-            "action": "ListIngestions",
+            "action": "StopIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartUserAccessTasks": {
+        "StartIngestion": {
             "access_level": "Undocumented",
-            "action": "StartUserAccessTasks",
+            "action": "StartIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppAuthorizations": {
+        "CreateIngestion": {
             "access_level": "Undocumented",
-            "action": "ListAppAuthorizations",
+            "action": "CreateIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIngestionDestinations": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListIngestionDestinations",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartIngestion": {
+        "ListIngestionDestinations": {
             "access_level": "Undocumented",
-            "action": "StartIngestion",
+            "action": "ListIngestionDestinations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIngestionDestination": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteIngestionDestination",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteIngestion": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppBundle": {
+        "DeleteAppBundle": {
             "access_level": "Undocumented",
-            "action": "CreateAppBundle",
+            "action": "DeleteAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIngestionDestination": {
+        "DeleteIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "CreateIngestionDestination",
+            "action": "DeleteIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppBundle": {
+        "GetIngestion": {
             "access_level": "Undocumented",
-            "action": "DeleteAppBundle",
+            "action": "GetIngestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAppAuthorization": {
+        "GetIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "UpdateAppAuthorization",
+            "action": "GetIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListAppAuthorizations": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListAppAuthorizations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppAuthorization": {
+        "BatchGetUserAccessTasks": {
             "access_level": "Undocumented",
-            "action": "CreateAppAuthorization",
+            "action": "BatchGetUserAccessTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIngestion": {
+        "StartUserAccessTasks": {
             "access_level": "Undocumented",
-            "action": "CreateIngestion",
+            "action": "StartUserAccessTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppBundles": {
+        "GetAppBundle": {
             "access_level": "Undocumented",
-            "action": "ListAppBundles",
+            "action": "GetAppBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetUserAccessTasks": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "BatchGetUserAccessTasks",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppAuthorization": {
+        "CreateIngestionDestination": {
             "access_level": "Undocumented",
-            "action": "DeleteAppAuthorization",
+            "action": "CreateIngestionDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopIngestion": {
+        "ConnectAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "StopIngestion",
+            "action": "ConnectAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIngestion": {
+        "DeleteAppAuthorization": {
             "access_level": "Undocumented",
-            "action": "DeleteIngestion",
+            "action": "DeleteAppAuthorization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAppAuthorization": {
+        "ListIngestions": {
             "access_level": "Undocumented",
-            "action": "GetAppAuthorization",
+            "action": "ListIngestions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIngestion": {
+        "ListAppBundles": {
             "access_level": "Undocumented",
-            "action": "GetIngestion",
+            "action": "ListAppBundles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "appflow": {
@@ -5170,121 +5170,121 @@
             "condition_keys": [],
             "description": "Grants permission to update an existing Application Cost Profiler Report configuration",
             "orphan": false,
             "resources": []
         }
     },
     "application-transformation": {
-        "StartDeployment": {
+        "StartPortingRecommendationAssessment": {
             "access_level": "Undocumented",
-            "action": "StartDeployment",
+            "action": "StartPortingRecommendationAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPortingCompatibilityAssessment": {
+        "StartContainerization": {
             "access_level": "Undocumented",
-            "action": "GetPortingCompatibilityAssessment",
+            "action": "StartContainerization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroupingAssessment": {
+        "GetPortingRecommendationAssessment": {
             "access_level": "Undocumented",
-            "action": "GetGroupingAssessment",
+            "action": "GetPortingRecommendationAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContainerization": {
+        "PutMetricData": {
             "access_level": "Undocumented",
-            "action": "GetContainerization",
+            "action": "PutMetricData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutMetricData": {
+        "PutLogData": {
             "access_level": "Undocumented",
-            "action": "PutMetricData",
+            "action": "PutLogData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetRuntimeAssessment": {
             "access_level": "Undocumented",
             "action": "GetRuntimeAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartPortingCompatibilityAssessment": {
+        "StartDeployment": {
             "access_level": "Undocumented",
-            "action": "StartPortingCompatibilityAssessment",
+            "action": "StartDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartPortingRecommendationAssessment": {
+        "StartRuntimeAssessment": {
             "access_level": "Undocumented",
-            "action": "StartPortingRecommendationAssessment",
+            "action": "StartRuntimeAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPortingRecommendationAssessment": {
+        "StartGroupingAssessment": {
             "access_level": "Undocumented",
-            "action": "GetPortingRecommendationAssessment",
+            "action": "StartGroupingAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutLogData": {
+        "GetPortingCompatibilityAssessment": {
             "access_level": "Undocumented",
-            "action": "PutLogData",
+            "action": "GetPortingCompatibilityAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetDeployment": {
             "access_level": "Undocumented",
             "action": "GetDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartRuntimeAssessment": {
+        "GetContainerization": {
             "access_level": "Undocumented",
-            "action": "StartRuntimeAssessment",
+            "action": "GetContainerization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartContainerization": {
+        "GetGroupingAssessment": {
             "access_level": "Undocumented",
-            "action": "StartContainerization",
+            "action": "GetGroupingAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartGroupingAssessment": {
+        "StartPortingCompatibilityAssessment": {
             "access_level": "Undocumented",
-            "action": "StartGroupingAssessment",
+            "action": "StartPortingCompatibilityAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "applicationinsights": {
@@ -11937,225 +11937,225 @@
             "condition_keys": [],
             "description": "Validates Server Migration Connector Id that was registered with AWS Connector Service.",
             "orphan": false,
             "resources": []
         }
     },
     "b2bi": {
-        "CreatePartnership": {
+        "DeletePartnership": {
             "access_level": "Undocumented",
-            "action": "CreatePartnership",
+            "action": "DeletePartnership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTransformerJob": {
+        "TestMapping": {
             "access_level": "Undocumented",
-            "action": "GetTransformerJob",
+            "action": "TestMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePartnership": {
+        "GetTransformer": {
             "access_level": "Undocumented",
-            "action": "UpdatePartnership",
+            "action": "GetTransformer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPartnerships": {
+        "UpdateProfile": {
             "access_level": "Undocumented",
-            "action": "ListPartnerships",
+            "action": "UpdateProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCapability": {
+        "ListProfiles": {
             "access_level": "Undocumented",
-            "action": "GetCapability",
+            "action": "ListProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProfiles": {
+        "CreateTransformer": {
             "access_level": "Undocumented",
-            "action": "ListProfiles",
+            "action": "CreateTransformer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCapability": {
+        "ListPartnerships": {
             "access_level": "Undocumented",
-            "action": "CreateCapability",
+            "action": "ListPartnerships",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartTransformerJob": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "StartTransformerJob",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProfile": {
+        "UpdateTransformer": {
             "access_level": "Undocumented",
-            "action": "DeleteProfile",
+            "action": "UpdateTransformer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCapabilities": {
+        "CreateCapability": {
             "access_level": "Undocumented",
-            "action": "ListCapabilities",
+            "action": "CreateCapability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProfile": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateProfile",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePartnership": {
+        "StartTransformerJob": {
             "access_level": "Undocumented",
-            "action": "DeletePartnership",
+            "action": "StartTransformerJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCapability": {
+        "GetPartnership": {
             "access_level": "Undocumented",
-            "action": "DeleteCapability",
+            "action": "GetPartnership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTransformers": {
+        "UpdatePartnership": {
             "access_level": "Undocumented",
-            "action": "ListTransformers",
+            "action": "UpdatePartnership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPartnership": {
+        "GetTransformerJob": {
             "access_level": "Undocumented",
-            "action": "GetPartnership",
+            "action": "GetTransformerJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListTransformers": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListTransformers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTransformer": {
+        "GetCapability": {
             "access_level": "Undocumented",
-            "action": "DeleteTransformer",
+            "action": "GetCapability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreatePartnership": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreatePartnership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteTransformer": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteTransformer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTransformer": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetTransformer",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProfile": {
+        "UpdateCapability": {
             "access_level": "Undocumented",
-            "action": "GetProfile",
+            "action": "UpdateCapability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCapability": {
+        "TestParsing": {
             "access_level": "Undocumented",
-            "action": "UpdateCapability",
+            "action": "TestParsing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTransformer": {
+        "ListCapabilities": {
             "access_level": "Undocumented",
-            "action": "CreateTransformer",
+            "action": "ListCapabilities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TestParsing": {
+        "DeleteProfile": {
             "access_level": "Undocumented",
-            "action": "TestParsing",
+            "action": "DeleteProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTransformer": {
+        "GetProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateTransformer",
+            "action": "GetProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProfile": {
+        "CreateProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateProfile",
+            "action": "CreateProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TestMapping": {
+        "DeleteCapability": {
             "access_level": "Undocumented",
-            "action": "TestMapping",
+            "action": "DeleteCapability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "backup": {
@@ -13789,97 +13789,97 @@
             "orphan": false,
             "resources": [
                 "scheduling-policy"
             ]
         }
     },
     "bcm-data-exports": {
-        "GetExecution": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetExecution",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExport": {
+        "CreateExport": {
             "access_level": "Undocumented",
-            "action": "GetExport",
+            "action": "CreateExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExecutions": {
+        "DeleteExport": {
             "access_level": "Undocumented",
-            "action": "ListExecutions",
+            "action": "DeleteExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExports": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListExports",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetExport": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTables": {
+        "UpdateExport": {
             "access_level": "Undocumented",
-            "action": "ListTables",
+            "action": "UpdateExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListTables": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListTables",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateExport": {
+        "GetExecution": {
             "access_level": "Undocumented",
-            "action": "UpdateExport",
+            "action": "GetExecution",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteExport": {
+        "ListExports": {
             "access_level": "Undocumented",
-            "action": "DeleteExport",
+            "action": "ListExports",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateExport": {
+        "ListExecutions": {
             "access_level": "Undocumented",
-            "action": "CreateExport",
+            "action": "ListExecutions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetTable": {
             "access_level": "Undocumented",
@@ -13887,787 +13887,787 @@
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "bedrock": {
-        "GetDataSource": {
+        "GetModelCustomizationJob": {
             "access_level": "Undocumented",
-            "action": "GetDataSource",
+            "action": "GetModelCustomizationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateThirdPartyKnowledgeBase": {
+        "UpdateAgentKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "AssociateThirdPartyKnowledgeBase",
+            "action": "UpdateAgentKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIngestionJob": {
+        "DeleteProvisionedModelThroughput": {
             "access_level": "Undocumented",
-            "action": "GetIngestionJob",
+            "action": "DeleteProvisionedModelThroughput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InvokeAgent": {
+        "GetGuardrail": {
             "access_level": "Undocumented",
-            "action": "InvokeAgent",
+            "action": "GetGuardrail",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGuardrail": {
+        "CreateModelInvocationJob": {
             "access_level": "Undocumented",
-            "action": "UpdateGuardrail",
+            "action": "CreateModelInvocationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSource": {
+        "GetUseCaseForModelAccess": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSource",
+            "action": "GetUseCaseForModelAccess",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFoundationModelAvailability": {
+        "DeleteCustomModel": {
             "access_level": "Undocumented",
-            "action": "GetFoundationModelAvailability",
+            "action": "DeleteCustomModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateModelInvocationJob": {
+        "StopModelCustomizationJob": {
             "access_level": "Undocumented",
-            "action": "CreateModelInvocationJob",
+            "action": "StopModelCustomizationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAgent": {
+        "ListAgents": {
             "access_level": "Undocumented",
-            "action": "UpdateAgent",
+            "action": "ListAgents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgents": {
+        "ListAgentAliases": {
             "access_level": "Undocumented",
-            "action": "ListAgents",
+            "action": "ListAgentAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "RetrieveAndGenerate": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "RetrieveAndGenerate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateModelEvaluationJob": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateModelEvaluationJob",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProvisionedModelThroughput": {
+        "CreateFoundationModelAgreement": {
             "access_level": "Undocumented",
-            "action": "GetProvisionedModelThroughput",
+            "action": "CreateFoundationModelAgreement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InvokeModelWithResponseStream": {
+        "GetCustomModel": {
             "access_level": "Undocumented",
-            "action": "InvokeModelWithResponseStream",
+            "action": "GetCustomModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PrepareAgent": {
+        "ListAgentVersions": {
             "access_level": "Undocumented",
-            "action": "PrepareAgent",
+            "action": "ListAgentVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetModelInvocationLoggingConfiguration": {
+        "GetProvisionedModelThroughput": {
             "access_level": "Undocumented",
-            "action": "GetModelInvocationLoggingConfiguration",
+            "action": "GetProvisionedModelThroughput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCustomModels": {
+        "DeleteModelInvocationLoggingConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListCustomModels",
+            "action": "DeleteModelInvocationLoggingConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCustomModel": {
+        "GetFoundationModelAvailability": {
             "access_level": "Undocumented",
-            "action": "DeleteCustomModel",
+            "action": "GetFoundationModelAvailability",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RetrieveAndGenerate": {
+        "GetAgentAlias": {
             "access_level": "Undocumented",
-            "action": "RetrieveAndGenerate",
+            "action": "GetAgentAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgentActionGroups": {
+        "PutModelInvocationLoggingConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListAgentActionGroups",
+            "action": "PutModelInvocationLoggingConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAgentActionGroup": {
+        "ListDataSources": {
             "access_level": "Undocumented",
-            "action": "GetAgentActionGroup",
+            "action": "ListDataSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InvokeModel": {
+        "DeleteGuardrail": {
             "access_level": "Undocumented",
-            "action": "InvokeModel",
+            "action": "DeleteGuardrail",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProvisionedModelThroughput": {
+        "UpdateAgent": {
             "access_level": "Undocumented",
-            "action": "UpdateProvisionedModelThroughput",
+            "action": "UpdateAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAgentAlias": {
+        "DeleteAgentVersion": {
             "access_level": "Undocumented",
-            "action": "DeleteAgentAlias",
+            "action": "DeleteAgentVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAgentActionGroup": {
+        "DeleteAgent": {
             "access_level": "Undocumented",
-            "action": "CreateAgentActionGroup",
+            "action": "DeleteAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateKnowledgeBase": {
+        "UpdateDataSource": {
             "access_level": "Undocumented",
-            "action": "CreateKnowledgeBase",
+            "action": "UpdateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListModelCustomizationJobs": {
+        "InvokeModel": {
             "access_level": "Undocumented",
-            "action": "ListModelCustomizationJobs",
+            "action": "InvokeModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgentVersions": {
+        "ListModelCustomizationJobs": {
             "access_level": "Undocumented",
-            "action": "ListAgentVersions",
+            "action": "ListModelCustomizationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAgentActionGroup": {
+        "ListFoundationModels": {
             "access_level": "Undocumented",
-            "action": "UpdateAgentActionGroup",
+            "action": "ListFoundationModels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAgentKnowledgeBase": {
+        "UpdateGuardrail": {
             "access_level": "Undocumented",
-            "action": "UpdateAgentKnowledgeBase",
+            "action": "UpdateGuardrail",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFoundationModelAgreement": {
+        "StartIngestionJob": {
             "access_level": "Undocumented",
-            "action": "CreateFoundationModelAgreement",
+            "action": "StartIngestionJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetectGeneratedContent": {
+        "Retrieve": {
             "access_level": "Undocumented",
-            "action": "DetectGeneratedContent",
+            "action": "Retrieve",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateAgentKnowledgeBase": {
+        "ListKnowledgeBases": {
             "access_level": "Undocumented",
-            "action": "AssociateAgentKnowledgeBase",
+            "action": "ListKnowledgeBases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFoundationModelAgreement": {
+        "ListIngestionJobs": {
             "access_level": "Undocumented",
-            "action": "DeleteFoundationModelAgreement",
+            "action": "ListIngestionJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAgentVersion": {
+        "CreateAgentActionGroup": {
             "access_level": "Undocumented",
-            "action": "GetAgentVersion",
+            "action": "CreateAgentActionGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUseCaseForModelAccess": {
+        "GetDataSource": {
             "access_level": "Undocumented",
-            "action": "GetUseCaseForModelAccess",
+            "action": "GetDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGuardrail": {
+        "ListProvisionedModelThroughputs": {
             "access_level": "Undocumented",
-            "action": "DeleteGuardrail",
+            "action": "ListProvisionedModelThroughputs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGuardrailVersion": {
+        "DeleteAgentAlias": {
             "access_level": "Undocumented",
-            "action": "CreateGuardrailVersion",
+            "action": "DeleteAgentAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateModelCustomizationJob": {
+        "InvokeModelWithResponseStream": {
             "access_level": "Undocumented",
-            "action": "CreateModelCustomizationJob",
+            "action": "InvokeModelWithResponseStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteKnowledgeBase": {
+        "ListModelEvaluationJobs": {
             "access_level": "Undocumented",
-            "action": "DeleteKnowledgeBase",
+            "action": "ListModelEvaluationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCustomModel": {
+        "AssociateThirdPartyKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "GetCustomModel",
+            "action": "AssociateThirdPartyKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopModelCustomizationJob": {
+        "CreateGuardrail": {
             "access_level": "Undocumented",
-            "action": "StopModelCustomizationJob",
+            "action": "CreateGuardrail",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteModelInvocationLoggingConfiguration": {
+        "ListAgentKnowledgeBases": {
             "access_level": "Undocumented",
-            "action": "DeleteModelInvocationLoggingConfiguration",
+            "action": "ListAgentKnowledgeBases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetModelInvocationJob": {
+        "CreateDataSource": {
             "access_level": "Undocumented",
-            "action": "GetModelInvocationJob",
+            "action": "CreateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataSource": {
+        "GetAgentActionGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteDataSource",
+            "action": "GetAgentActionGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAgentVersion": {
+        "PutFoundationModelEntitlement": {
             "access_level": "Undocumented",
-            "action": "DeleteAgentVersion",
+            "action": "PutFoundationModelEntitlement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListKnowledgeBases": {
+        "DeleteKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "ListKnowledgeBases",
+            "action": "DeleteKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAgent": {
+        "GetAgent": {
             "access_level": "Undocumented",
-            "action": "DeleteAgent",
+            "action": "GetAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetModelEvaluationJob": {
+        "CreateAgent": {
             "access_level": "Undocumented",
-            "action": "GetModelEvaluationJob",
+            "action": "CreateAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateAgentAlias": {
             "access_level": "Undocumented",
             "action": "UpdateAgentAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopModelInvocationJob": {
+        "CreateKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "StopModelInvocationJob",
+            "action": "CreateKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUseCaseForModelAccess": {
+        "GetIngestionJob": {
             "access_level": "Undocumented",
-            "action": "PutUseCaseForModelAccess",
+            "action": "GetIngestionJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartIngestionJob": {
+        "CreateGuardrailVersion": {
             "access_level": "Undocumented",
-            "action": "StartIngestionJob",
+            "action": "CreateGuardrailVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSources": {
+        "DeleteAgentActionGroup": {
             "access_level": "Undocumented",
-            "action": "ListDataSources",
+            "action": "DeleteAgentActionGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAgentAlias": {
+        "DeleteDataSource": {
             "access_level": "Undocumented",
-            "action": "GetAgentAlias",
+            "action": "DeleteDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListFoundationModelAgreementOffers": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListFoundationModelAgreementOffers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetKnowledgeBase": {
+        "GetFoundationModel": {
             "access_level": "Undocumented",
-            "action": "GetKnowledgeBase",
+            "action": "GetFoundationModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAgent": {
+        "DetectGeneratedContent": {
             "access_level": "Undocumented",
-            "action": "GetAgent",
+            "action": "DetectGeneratedContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAgentActionGroup": {
+        "UpdateProvisionedModelThroughput": {
             "access_level": "Undocumented",
-            "action": "DeleteAgentActionGroup",
+            "action": "UpdateProvisionedModelThroughput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProvisionedModelThroughput": {
+        "GetAgentVersion": {
             "access_level": "Undocumented",
-            "action": "DeleteProvisionedModelThroughput",
+            "action": "GetAgentVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateKnowledgeBase": {
+        "AssociateAgentKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "UpdateKnowledgeBase",
+            "action": "AssociateAgentKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFoundationModel": {
+        "ListAgentActionGroups": {
             "access_level": "Undocumented",
-            "action": "GetFoundationModel",
+            "action": "ListAgentActionGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAgentKnowledgeBase": {
+        "StopModelInvocationJob": {
             "access_level": "Undocumented",
-            "action": "GetAgentKnowledgeBase",
+            "action": "StopModelInvocationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProvisionedModelThroughputs": {
+        "PrepareAgent": {
             "access_level": "Undocumented",
-            "action": "ListProvisionedModelThroughputs",
+            "action": "PrepareAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgentAliases": {
+        "PutUseCaseForModelAccess": {
             "access_level": "Undocumented",
-            "action": "ListAgentAliases",
+            "action": "PutUseCaseForModelAccess",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGuardrails": {
+        "GetModelEvaluationJob": {
             "access_level": "Undocumented",
-            "action": "ListGuardrails",
+            "action": "GetModelEvaluationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetModelCustomizationJob": {
+        "CreateProvisionedModelThroughput": {
             "access_level": "Undocumented",
-            "action": "GetModelCustomizationJob",
+            "action": "CreateProvisionedModelThroughput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutFoundationModelEntitlement": {
+        "GetModelInvocationJob": {
             "access_level": "Undocumented",
-            "action": "PutFoundationModelEntitlement",
+            "action": "GetModelInvocationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAgentAlias": {
+        "ListGuardrails": {
             "access_level": "Undocumented",
-            "action": "CreateAgentAlias",
+            "action": "ListGuardrails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutModelInvocationLoggingConfiguration": {
+        "UpdateKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "PutModelInvocationLoggingConfiguration",
+            "action": "UpdateKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFoundationModelAgreementOffers": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListFoundationModelAgreementOffers",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIngestionJobs": {
+        "CreateModelEvaluationJob": {
             "access_level": "Undocumented",
-            "action": "ListIngestionJobs",
+            "action": "CreateModelEvaluationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListModelInvocationJobs": {
+        "GetAgentKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "ListModelInvocationJobs",
+            "action": "GetAgentKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "CreateModelCustomizationJob": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreateModelCustomizationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFoundationModels": {
+        "GetKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "ListFoundationModels",
+            "action": "GetKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListModelEvaluationJobs": {
+        "UpdateAgentActionGroup": {
             "access_level": "Undocumented",
-            "action": "ListModelEvaluationJobs",
+            "action": "UpdateAgentActionGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGuardrail": {
+        "DisassociateAgentKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "GetGuardrail",
+            "action": "DisassociateAgentKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateAgentKnowledgeBase": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DisassociateAgentKnowledgeBase",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAgentKnowledgeBases": {
+        "DeleteFoundationModelAgreement": {
             "access_level": "Undocumented",
-            "action": "ListAgentKnowledgeBases",
+            "action": "DeleteFoundationModelAgreement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Retrieve": {
+        "InvokeAgent": {
             "access_level": "Undocumented",
-            "action": "Retrieve",
+            "action": "InvokeAgent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAgent": {
+        "GetModelInvocationLoggingConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateAgent",
+            "action": "GetModelInvocationLoggingConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDataSource": {
+        "CreateAgentAlias": {
             "access_level": "Undocumented",
-            "action": "CreateDataSource",
+            "action": "CreateAgentAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProvisionedModelThroughput": {
+        "ListCustomModels": {
             "access_level": "Undocumented",
-            "action": "CreateProvisionedModelThroughput",
+            "action": "ListCustomModels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGuardrail": {
+        "ListModelInvocationJobs": {
             "access_level": "Undocumented",
-            "action": "CreateGuardrail",
+            "action": "ListModelInvocationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "billing": {
-        "GetBillingData": {
+        "GetBillingPreferences": {
             "access_level": "Undocumented",
-            "action": "GetBillingData",
+            "action": "GetBillingPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContractInformation": {
+        "GetCredits": {
             "access_level": "Undocumented",
-            "action": "GetContractInformation",
+            "action": "GetCredits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBillingNotifications": {
+        "PutContractInformation": {
             "access_level": "Undocumented",
-            "action": "GetBillingNotifications",
+            "action": "PutContractInformation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListBillingViews": {
+        "GetBillingData": {
             "access_level": "Undocumented",
-            "action": "ListBillingViews",
+            "action": "GetBillingData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RedeemCredits": {
+        "GetSellerOfRecord": {
             "access_level": "Undocumented",
-            "action": "RedeemCredits",
+            "action": "GetSellerOfRecord",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBillingDetails": {
+        "UpdateIAMAccessPreference": {
             "access_level": "Undocumented",
-            "action": "GetBillingDetails",
+            "action": "UpdateIAMAccessPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateBillingPreferences": {
+        "GetBillingDetails": {
             "access_level": "Undocumented",
-            "action": "UpdateBillingPreferences",
+            "action": "GetBillingDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBillingPreferences": {
+        "RedeemCredits": {
             "access_level": "Undocumented",
-            "action": "GetBillingPreferences",
+            "action": "RedeemCredits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIAMAccessPreference": {
+        "ListBillingViews": {
             "access_level": "Undocumented",
-            "action": "UpdateIAMAccessPreference",
+            "action": "ListBillingViews",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCredits": {
+        "UpdateBillingPreferences": {
             "access_level": "Undocumented",
-            "action": "GetCredits",
+            "action": "UpdateBillingPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetIAMAccessPreference": {
             "access_level": "Undocumented",
             "action": "GetIAMAccessPreference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSellerOfRecord": {
+        "GetBillingNotifications": {
             "access_level": "Undocumented",
-            "action": "GetSellerOfRecord",
+            "action": "GetBillingNotifications",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutContractInformation": {
+        "GetContractInformation": {
             "access_level": "Undocumented",
-            "action": "PutContractInformation",
+            "action": "GetContractInformation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "billingconductor": {
@@ -19752,715 +19752,715 @@
             "condition_keys": [],
             "description": "Grants permission to validate an address to be used for 911 calls made with Amazon Chime Voice Connectors",
             "orphan": false,
             "resources": []
         }
     },
     "cleanrooms": {
-        "DeleteMembership": {
+        "GetMembership": {
             "access_level": "Undocumented",
-            "action": "DeleteMembership",
+            "action": "GetMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProtectedQueries": {
+        "UpdateCollaboration": {
             "access_level": "Undocumented",
-            "action": "ListProtectedQueries",
+            "action": "UpdateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchema": {
+        "ListPrivacyBudgetTemplates": {
             "access_level": "Undocumented",
-            "action": "GetSchema",
+            "action": "ListPrivacyBudgetTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetSchema": {
+        "ListCollaborations": {
             "access_level": "Undocumented",
-            "action": "BatchGetSchema",
+            "action": "ListCollaborations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredAudienceModelAssociations": {
+        "CreateAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredAudienceModelAssociations",
+            "action": "CreateAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCollaboration": {
+        "ListCollaborationAnalysisTemplates": {
             "access_level": "Undocumented",
-            "action": "UpdateCollaboration",
+            "action": "ListCollaborationAnalysisTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMembership": {
+        "GetCollaborationAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "GetMembership",
+            "action": "GetCollaborationAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTable": {
+        "UpdatePrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTable",
+            "action": "UpdatePrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborationAnalysisTemplates": {
+        "GetSchemaAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "ListCollaborationAnalysisTemplates",
+            "action": "GetSchemaAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTableAssociation": {
+        "DeleteCollaboration": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTableAssociation",
+            "action": "DeleteCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchemaAnalysisRule": {
+        "ListCollaborationPrivacyBudgetTemplates": {
             "access_level": "Undocumented",
-            "action": "GetSchemaAnalysisRule",
+            "action": "ListCollaborationPrivacyBudgetTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredTables": {
+        "ListProtectedQueries": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredTables",
+            "action": "ListProtectedQueries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAnalysisTemplate": {
+        "UpdateConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "CreateAnalysisTemplate",
+            "action": "UpdateConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePrivacyBudgetTemplate": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdatePrivacyBudgetTemplate",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredAudienceModelAssociation": {
+        "GetCollaboration": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredAudienceModelAssociation",
+            "action": "GetCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMemberships": {
+        "UpdateConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "ListMemberships",
+            "action": "UpdateConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMembers": {
+        "DeletePrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "ListMembers",
+            "action": "DeletePrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTableAssociation": {
+        "GetProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTableAssociation",
+            "action": "GetProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTableAssociation": {
+        "CreateConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTableAssociation",
+            "action": "CreateConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSchemas": {
+        "DeleteMember": {
             "access_level": "Undocumented",
-            "action": "ListSchemas",
+            "action": "DeleteMember",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetSchemaAnalysisRule": {
+        "ListCollaborationPrivacyBudgets": {
             "access_level": "Undocumented",
-            "action": "BatchGetSchemaAnalysisRule",
+            "action": "ListCollaborationPrivacyBudgets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListConfiguredTables": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListConfiguredTables",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UpdateAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UpdateAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProtectedQuery": {
+        "ListConfiguredTableAssociations": {
             "access_level": "Undocumented",
-            "action": "GetProtectedQuery",
+            "action": "ListConfiguredTableAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMembership": {
+        "DeleteConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "UpdateMembership",
+            "action": "DeleteConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborations": {
+        "GetCollaborationPrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "ListCollaborations",
+            "action": "GetCollaborationPrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAnalysisTemplate": {
+        "BatchGetSchema": {
             "access_level": "Undocumented",
-            "action": "DeleteAnalysisTemplate",
+            "action": "BatchGetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborationPrivacyBudgets": {
+        "UpdateConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "ListCollaborationPrivacyBudgets",
+            "action": "UpdateConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredTableAnalysisRule": {
+        "DeleteMembership": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredTableAnalysisRule",
+            "action": "DeleteMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetCollaborationAnalysisTemplate": {
+        "CreateConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "BatchGetCollaborationAnalysisTemplate",
+            "action": "CreateConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAnalysisTemplate": {
+        "GetCollaborationConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "GetAnalysisTemplate",
+            "action": "GetCollaborationConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAnalysisTemplates": {
+        "ListConfiguredAudienceModelAssociations": {
             "access_level": "Undocumented",
-            "action": "ListAnalysisTemplates",
+            "action": "ListConfiguredAudienceModelAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPrivacyBudgetTemplate": {
+        "ListSchemas": {
             "access_level": "Undocumented",
-            "action": "GetPrivacyBudgetTemplate",
+            "action": "ListSchemas",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProtectedQuery": {
+        "UpdateMembership": {
             "access_level": "Undocumented",
-            "action": "UpdateProtectedQuery",
+            "action": "UpdateMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePrivacyBudgetTemplate": {
+        "DeleteConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "CreatePrivacyBudgetTemplate",
+            "action": "DeleteConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborationPrivacyBudgetTemplates": {
+        "ListAnalysisTemplates": {
             "access_level": "Undocumented",
-            "action": "ListCollaborationPrivacyBudgetTemplates",
+            "action": "ListAnalysisTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredAudienceModelAssociation": {
+        "ListPrivacyBudgets": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredAudienceModelAssociation",
+            "action": "ListPrivacyBudgets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCollaboration": {
+        "CreatePrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateCollaboration",
+            "action": "CreatePrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredTableAssociations": {
+        "UpdateConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredTableAssociations",
+            "action": "UpdateConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTableAssociation": {
+        "BatchGetSchemaAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTableAssociation",
+            "action": "BatchGetSchemaAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredAudienceModelAssociation": {
+        "CreateConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredAudienceModelAssociation",
+            "action": "CreateConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCollaborationConfiguredAudienceModelAssociations": {
+        "StartProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "ListCollaborationConfiguredAudienceModelAssociations",
+            "action": "StartProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrivacyBudgetTemplates": {
+        "UpdateProtectedQuery": {
             "access_level": "Undocumented",
-            "action": "ListPrivacyBudgetTemplates",
+            "action": "UpdateProtectedQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTable": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTable",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCollaboration": {
+        "GetPrivacyBudgetTemplate": {
             "access_level": "Undocumented",
-            "action": "DeleteCollaboration",
+            "action": "GetPrivacyBudgetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTable": {
+        "CreateCollaboration": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTable",
+            "action": "CreateCollaboration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartProtectedQuery": {
+        "DeleteAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "StartProtectedQuery",
+            "action": "DeleteAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredAudienceModelAssociation": {
+        "GetSchema": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredAudienceModelAssociation",
+            "action": "GetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredTableAnalysisRule": {
+        "GetConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredTableAnalysisRule",
+            "action": "GetConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePrivacyBudgetTemplate": {
+        "DeleteConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "DeletePrivacyBudgetTemplate",
+            "action": "DeleteConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTableAnalysisRule": {
+        "BatchGetCollaborationAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTableAnalysisRule",
+            "action": "BatchGetCollaborationAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaborationPrivacyBudgetTemplate": {
+        "GetConfiguredTableAssociation": {
             "access_level": "Undocumented",
-            "action": "GetCollaborationPrivacyBudgetTemplate",
+            "action": "GetConfiguredTableAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaborationAnalysisTemplate": {
+        "DeleteConfiguredTableAnalysisRule": {
             "access_level": "Undocumented",
-            "action": "GetCollaborationAnalysisTemplate",
+            "action": "DeleteConfiguredTableAnalysisRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PreviewPrivacyImpact": {
+        "GetConfiguredAudienceModelAssociation": {
             "access_level": "Undocumented",
-            "action": "PreviewPrivacyImpact",
+            "action": "GetConfiguredAudienceModelAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListMemberships": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListMemberships",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMembership": {
+        "CreateConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "CreateMembership",
+            "action": "CreateConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAnalysisTemplate": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UpdateAnalysisTemplate",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredTable": {
+        "GetConfiguredTable": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredTable",
+            "action": "GetConfiguredTable",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaborationConfiguredAudienceModelAssociation": {
+        "PreviewPrivacyImpact": {
             "access_level": "Undocumented",
-            "action": "GetCollaborationConfiguredAudienceModelAssociation",
+            "action": "PreviewPrivacyImpact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMember": {
+        "ListMembers": {
             "access_level": "Undocumented",
-            "action": "DeleteMember",
+            "action": "ListMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrivacyBudgets": {
+        "GetAnalysisTemplate": {
             "access_level": "Undocumented",
-            "action": "ListPrivacyBudgets",
+            "action": "GetAnalysisTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredTableAnalysisRule": {
+        "ListCollaborationConfiguredAudienceModelAssociations": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredTableAnalysisRule",
+            "action": "ListCollaborationConfiguredAudienceModelAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCollaboration": {
+        "CreateMembership": {
             "access_level": "Undocumented",
-            "action": "GetCollaboration",
+            "action": "CreateMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cleanrooms-ml": {
-        "ListTrainingDatasets": {
+        "ListConfiguredAudienceModels": {
             "access_level": "Undocumented",
-            "action": "ListTrainingDatasets",
+            "action": "ListConfiguredAudienceModels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredAudienceModelPolicy": {
+        "UnTagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredAudienceModelPolicy",
+            "action": "UnTagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteAudienceGenerationJob": {
             "access_level": "Undocumented",
             "action": "DeleteAudienceGenerationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAudienceExportJob": {
+        "GetAudienceModel": {
             "access_level": "Undocumented",
-            "action": "StartAudienceExportJob",
+            "action": "GetAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAudienceModel": {
+        "ListAudienceGenerationJobs": {
             "access_level": "Undocumented",
-            "action": "CreateAudienceModel",
+            "action": "ListAudienceGenerationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAudienceExportJobs": {
+        "CreateConfiguredAudienceModel": {
             "access_level": "Undocumented",
-            "action": "ListAudienceExportJobs",
+            "action": "CreateConfiguredAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTrainingDataset": {
+        "ListAudienceExportJobs": {
             "access_level": "Undocumented",
-            "action": "DeleteTrainingDataset",
+            "action": "ListAudienceExportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConfiguredAudienceModels": {
+        "DeleteConfiguredAudienceModel": {
             "access_level": "Undocumented",
-            "action": "ListConfiguredAudienceModels",
+            "action": "DeleteConfiguredAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTrainingDataset": {
+        "GetConfiguredAudienceModelPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateTrainingDataset",
+            "action": "GetConfiguredAudienceModelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAudienceGenerationJobs": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListAudienceGenerationJobs",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAudienceModel": {
+        "GetAudienceGenerationJob": {
             "access_level": "Undocumented",
-            "action": "GetAudienceModel",
+            "action": "GetAudienceGenerationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTrainingDataset": {
+        "GetConfiguredAudienceModel": {
             "access_level": "Undocumented",
-            "action": "GetTrainingDataset",
+            "action": "GetConfiguredAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConfiguredAudienceModel": {
+        "CreateTrainingDataset": {
             "access_level": "Undocumented",
-            "action": "UpdateConfiguredAudienceModel",
+            "action": "CreateTrainingDataset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAudienceGenerationJob": {
+        "ListTrainingDatasets": {
             "access_level": "Undocumented",
-            "action": "StartAudienceGenerationJob",
+            "action": "ListTrainingDatasets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "StartAudienceGenerationJob": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "StartAudienceGenerationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateAudienceModel": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredAudienceModel": {
+        "StartAudienceExportJob": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredAudienceModel",
+            "action": "StartAudienceExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "PutConfiguredAudienceModelPolicy": {
             "access_level": "Undocumented",
             "action": "PutConfiguredAudienceModelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAudienceGenerationJob": {
+        "UpdateConfiguredAudienceModel": {
             "access_level": "Undocumented",
-            "action": "GetAudienceGenerationJob",
+            "action": "UpdateConfiguredAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConfiguredAudienceModel": {
+        "DeleteTrainingDataset": {
             "access_level": "Undocumented",
-            "action": "CreateConfiguredAudienceModel",
+            "action": "DeleteTrainingDataset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UnTagResource": {
+        "ListAudienceModels": {
             "access_level": "Undocumented",
-            "action": "UnTagResource",
+            "action": "ListAudienceModels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAudienceModel": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteAudienceModel",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetConfiguredAudienceModelPolicy": {
+        "DeleteAudienceModel": {
             "access_level": "Undocumented",
-            "action": "GetConfiguredAudienceModelPolicy",
+            "action": "DeleteAudienceModel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAudienceModels": {
+        "GetTrainingDataset": {
             "access_level": "Undocumented",
-            "action": "ListAudienceModels",
+            "action": "GetTrainingDataset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConfiguredAudienceModel": {
+        "DeleteConfiguredAudienceModelPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteConfiguredAudienceModel",
+            "action": "DeleteConfiguredAudienceModelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cloud9": {
@@ -23447,57 +23447,57 @@
             "orphan": false,
             "resources": [
                 "streaming-distribution"
             ]
         }
     },
     "cloudfront-keyvaluestore": {
-        "PutKey": {
+        "GetKey": {
             "access_level": "Undocumented",
-            "action": "PutKey",
+            "action": "GetKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateKeys": {
+        "DescribeKeyValueStore": {
             "access_level": "Undocumented",
-            "action": "UpdateKeys",
+            "action": "DescribeKeyValueStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteKey": {
+        "UpdateKeys": {
             "access_level": "Undocumented",
-            "action": "DeleteKey",
+            "action": "UpdateKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetKey": {
+        "ListKeys": {
             "access_level": "Undocumented",
-            "action": "GetKey",
+            "action": "ListKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListKeys": {
+        "DeleteKey": {
             "access_level": "Undocumented",
-            "action": "ListKeys",
+            "action": "DeleteKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeKeyValueStore": {
+        "PutKey": {
             "access_level": "Undocumented",
-            "action": "DescribeKeyValueStore",
+            "action": "PutKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cloudhsm": {
@@ -27649,309 +27649,309 @@
             "orphan": false,
             "resources": [
                 "repository"
             ]
         }
     },
     "codeconnections": {
-        "GetSyncBlockerSummary": {
-            "access_level": "Undocumented",
-            "action": "GetSyncBlockerSummary",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "StartOAuthHandshake": {
+        "PassConnection": {
             "access_level": "Undocumented",
-            "action": "StartOAuthHandshake",
+            "action": "PassConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateSyncConfiguration": {
             "access_level": "Undocumented",
             "action": "CreateSyncConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterAppCode": {
+        "GetInstallationUrl": {
             "access_level": "Undocumented",
-            "action": "RegisterAppCode",
+            "action": "GetInstallationUrl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRepositorySyncDefinitions": {
+        "DeleteHost": {
             "access_level": "Undocumented",
-            "action": "ListRepositorySyncDefinitions",
+            "action": "DeleteHost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSyncConfiguration": {
+        "GetSyncBlockerSummary": {
             "access_level": "Undocumented",
-            "action": "DeleteSyncConfiguration",
+            "action": "GetSyncBlockerSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRepositorySyncStatus": {
+        "StartAppRegistrationHandshake": {
             "access_level": "Undocumented",
-            "action": "GetRepositorySyncStatus",
+            "action": "StartAppRegistrationHandshake",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetHost": {
+        "GetResourceSyncStatus": {
             "access_level": "Undocumented",
-            "action": "GetHost",
+            "action": "GetResourceSyncStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteHost": {
+        "UpdateHost": {
             "access_level": "Undocumented",
-            "action": "DeleteHost",
+            "action": "UpdateHost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRepositoryLinks": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListRepositoryLinks",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSyncConfigurations": {
+        "CreateHost": {
             "access_level": "Undocumented",
-            "action": "ListSyncConfigurations",
+            "action": "CreateHost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetRepositorySyncStatus": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetRepositorySyncStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListRepositoryLinks": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListRepositoryLinks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListConnections": {
             "access_level": "Undocumented",
             "action": "ListConnections",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSyncConfiguration": {
+        "DeleteRepositoryLink": {
             "access_level": "Undocumented",
-            "action": "GetSyncConfiguration",
+            "action": "DeleteRepositoryLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAppRegistrationHandshake": {
+        "UpdateConnectionInstallation": {
             "access_level": "Undocumented",
-            "action": "StartAppRegistrationHandshake",
+            "action": "UpdateConnectionInstallation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateConnectionInstallation": {
+        "DeleteConnection": {
             "access_level": "Undocumented",
-            "action": "UpdateConnectionInstallation",
+            "action": "DeleteConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConnection": {
+        "ListRepositorySyncDefinitions": {
             "access_level": "Undocumented",
-            "action": "DeleteConnection",
+            "action": "ListRepositorySyncDefinitions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateSyncBlocker": {
             "access_level": "Undocumented",
             "action": "UpdateSyncBlocker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSyncConfiguration": {
+        "GetHost": {
             "access_level": "Undocumented",
-            "action": "UpdateSyncConfiguration",
+            "action": "GetHost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceSyncStatus": {
+        "UseConnection": {
             "access_level": "Undocumented",
-            "action": "GetResourceSyncStatus",
+            "action": "UseConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRepositoryLink": {
+        "CreateRepositoryLink": {
             "access_level": "Undocumented",
-            "action": "UpdateRepositoryLink",
+            "action": "CreateRepositoryLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListHosts": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListHosts",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UseConnection": {
+        "ListInstallationTargets": {
             "access_level": "Undocumented",
-            "action": "UseConnection",
+            "action": "ListInstallationTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PassConnection": {
+        "PassRepository": {
             "access_level": "Undocumented",
-            "action": "PassConnection",
+            "action": "PassRepository",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRepositoryLink": {
+        "GetSyncConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateRepositoryLink",
+            "action": "GetSyncConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PassRepository": {
+        "RegisterAppCode": {
             "access_level": "Undocumented",
-            "action": "PassRepository",
+            "action": "RegisterAppCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRepositoryLink": {
+        "UpdateSyncConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteRepositoryLink",
+            "action": "UpdateSyncConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListHosts": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListHosts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRepositoryLink": {
+        "StartOAuthHandshake": {
             "access_level": "Undocumented",
-            "action": "GetRepositoryLink",
+            "action": "StartOAuthHandshake",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstallationTargets": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListInstallationTargets",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInstallationUrl": {
+        "UpdateRepositoryLink": {
             "access_level": "Undocumented",
-            "action": "GetInstallationUrl",
+            "action": "UpdateRepositoryLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateHost": {
+        "GetIndividualAccessToken": {
             "access_level": "Undocumented",
-            "action": "UpdateHost",
+            "action": "GetIndividualAccessToken",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIndividualAccessToken": {
+        "DeleteSyncConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetIndividualAccessToken",
+            "action": "DeleteSyncConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateHost": {
+        "ListSyncConfigurations": {
             "access_level": "Undocumented",
-            "action": "CreateHost",
+            "action": "ListSyncConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConnection": {
+        "GetRepositoryLink": {
             "access_level": "Undocumented",
-            "action": "CreateConnection",
+            "action": "GetRepositoryLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetConnection": {
             "access_level": "Undocumented",
             "action": "GetConnection",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
+        },
+        "CreateConnection": {
+            "access_level": "Undocumented",
+            "action": "CreateConnection",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         }
     },
     "codedeploy": {
         "AddTagsToOnPremisesInstances": {
             "access_level": "Tagging",
             "action": "AddTagsToOnPremisesInstances",
             "condition_keys": [],
@@ -28879,129 +28879,129 @@
             "orphan": false,
             "resources": [
                 "association"
             ]
         }
     },
     "codeguru-security": {
-        "GetAccountConfiguration": {
+        "CreateUploadUrl": {
             "access_level": "Undocumented",
-            "action": "GetAccountConfiguration",
+            "action": "CreateUploadUrl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteScansByCategory": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteScansByCategory",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetricsSummary": {
+        "ListScans": {
             "access_level": "Undocumented",
-            "action": "GetMetricsSummary",
+            "action": "ListScans",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetScan": {
+        "GetMetricsSummary": {
             "access_level": "Undocumented",
-            "action": "GetScan",
+            "action": "GetMetricsSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFindingsMetrics": {
+        "GetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListFindingsMetrics",
+            "action": "GetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateScan": {
+        "GetFindings": {
             "access_level": "Undocumented",
-            "action": "CreateScan",
+            "action": "GetFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFindings": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetFindings",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "BatchGetFindings": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "BatchGetFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListFindingsMetrics": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListFindingsMetrics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFindings": {
+        "UpdateAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListFindings",
+            "action": "UpdateAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListScans": {
+        "CreateScan": {
             "access_level": "Undocumented",
-            "action": "ListScans",
+            "action": "CreateScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountConfiguration": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountConfiguration",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteScansByCategory": {
+        "GetScan": {
             "access_level": "Undocumented",
-            "action": "DeleteScansByCategory",
+            "action": "GetScan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUploadUrl": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateUploadUrl",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetFindings": {
+        "ListFindings": {
             "access_level": "Undocumented",
-            "action": "BatchGetFindings",
+            "action": "ListFindings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "codepipeline": {
@@ -37497,43 +37497,43 @@
             "orphan": false,
             "resources": [
                 "campaign"
             ]
         }
     },
     "consoleapp": {
-        "ListDeviceIdentities": {
+        "GetDeviceIdentity": {
             "access_level": "Undocumented",
-            "action": "ListDeviceIdentities",
+            "action": "GetDeviceIdentity",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceIdentity": {
+        "ListDeviceIdentities": {
             "access_level": "Undocumented",
-            "action": "GetDeviceIdentity",
+            "action": "ListDeviceIdentities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "consolidatedbilling": {
-        "GetAccountBillingRole": {
+        "ListLinkedAccounts": {
             "access_level": "Undocumented",
-            "action": "GetAccountBillingRole",
+            "action": "ListLinkedAccounts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListLinkedAccounts": {
+        "GetAccountBillingRole": {
             "access_level": "Undocumented",
-            "action": "ListLinkedAccounts",
+            "action": "GetAccountBillingRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "controlcatalog": {
@@ -37541,25 +37541,25 @@
             "access_level": "Undocumented",
             "action": "ListDomains",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListObjectives": {
+        "ListCommonControls": {
             "access_level": "Undocumented",
-            "action": "ListObjectives",
+            "action": "ListCommonControls",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListCommonControls": {
+        "ListObjectives": {
             "access_level": "Undocumented",
-            "action": "ListCommonControls",
+            "action": "ListObjectives",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "controltower": {
@@ -38109,65 +38109,65 @@
             "orphan": false,
             "resources": [
                 "LandingZone"
             ]
         }
     },
     "cost-optimization-hub": {
-        "UpdateEnrollmentStatus": {
+        "GetRecommendation": {
             "access_level": "Undocumented",
-            "action": "UpdateEnrollmentStatus",
+            "action": "GetRecommendation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRecommendations": {
+        "UpdateEnrollmentStatus": {
             "access_level": "Undocumented",
-            "action": "ListRecommendations",
+            "action": "UpdateEnrollmentStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRecommendationSummaries": {
+        "ListRecommendations": {
             "access_level": "Undocumented",
-            "action": "ListRecommendationSummaries",
+            "action": "ListRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRecommendation": {
+        "GetPreferences": {
             "access_level": "Undocumented",
-            "action": "GetRecommendation",
+            "action": "GetPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnrollmentStatuses": {
+        "ListRecommendationSummaries": {
             "access_level": "Undocumented",
-            "action": "ListEnrollmentStatuses",
+            "action": "ListRecommendationSummaries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPreferences": {
+        "UpdatePreferences": {
             "access_level": "Undocumented",
-            "action": "GetPreferences",
+            "action": "UpdatePreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePreferences": {
+        "ListEnrollmentStatuses": {
             "access_level": "Undocumented",
-            "action": "UpdatePreferences",
+            "action": "ListEnrollmentStatuses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "cur": {
@@ -38302,25 +38302,25 @@
             "access_level": "Undocumented",
             "action": "GetCustomerVerificationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCustomerVerificationEligibility": {
+        "CreateCustomerVerificationDetails": {
             "access_level": "Undocumented",
-            "action": "GetCustomerVerificationEligibility",
+            "action": "CreateCustomerVerificationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateCustomerVerificationDetails": {
+        "GetCustomerVerificationEligibility": {
             "access_level": "Undocumented",
-            "action": "CreateCustomerVerificationDetails",
+            "action": "GetCustomerVerificationEligibility",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "databrew": {
@@ -40004,1065 +40004,1065 @@
             "orphan": false,
             "resources": [
                 "taskexecution"
             ]
         }
     },
     "datazone": {
-        "DeleteGlossary": {
+        "ListEnvironmentBlueprints": {
             "access_level": "Undocumented",
-            "action": "DeleteGlossary",
+            "action": "ListEnvironmentBlueprints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSource": {
+        "ListSubscriptionRequests": {
             "access_level": "Undocumented",
-            "action": "GetDataSource",
+            "action": "ListSubscriptionRequests",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutEnvironmentBlueprintConfiguration": {
+        "StopMetadataGenerationRun": {
             "access_level": "Undocumented",
-            "action": "PutEnvironmentBlueprintConfiguration",
+            "action": "StopMetadataGenerationRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopMetadataGenerationRun": {
+        "DeleteGlossary": {
             "access_level": "Undocumented",
-            "action": "StopMetadataGenerationRun",
+            "action": "DeleteGlossary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyGrants": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListPolicyGrants",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMetadataGenerationRuns": {
+        "RevokeSubscription": {
             "access_level": "Undocumented",
-            "action": "ListMetadataGenerationRuns",
+            "action": "RevokeSubscription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSubscriptionRequest": {
+        "ListEnvironmentBlueprintConfigurations": {
             "access_level": "Undocumented",
-            "action": "CreateSubscriptionRequest",
+            "action": "ListEnvironmentBlueprintConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAssetType": {
+        "RemovePolicyGrant": {
             "access_level": "Undocumented",
-            "action": "DeleteAssetType",
+            "action": "RemovePolicyGrant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAssetType": {
+        "ListWarehouseMetadata": {
             "access_level": "Undocumented",
-            "action": "GetAssetType",
+            "action": "ListWarehouseMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSource": {
+        "GetDomainSharingPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSource",
+            "action": "GetDomainSharingPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGlossary": {
+        "GetDataSourceRun": {
             "access_level": "Undocumented",
-            "action": "UpdateGlossary",
+            "action": "GetDataSourceRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSubscriptions": {
+        "StartMetadataGenerationRun": {
             "access_level": "Undocumented",
-            "action": "ListSubscriptions",
+            "action": "StartMetadataGenerationRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchTypes": {
+        "UpdateDataSource": {
             "access_level": "Undocumented",
-            "action": "SearchTypes",
+            "action": "UpdateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGlossaryTerm": {
+        "DeleteDomain": {
             "access_level": "Undocumented",
-            "action": "GetGlossaryTerm",
+            "action": "DeleteDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAsset": {
+        "SearchUserProfiles": {
             "access_level": "Undocumented",
-            "action": "CreateAsset",
+            "action": "SearchUserProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGlossaryTerm": {
+        "ValidatePassRole": {
             "access_level": "Undocumented",
-            "action": "UpdateGlossaryTerm",
+            "action": "ValidatePassRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSubscriptionGrants": {
+        "UpdateDomain": {
             "access_level": "Undocumented",
-            "action": "ListSubscriptionGrants",
+            "action": "UpdateDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartMetadataGenerationRun": {
+        "CreateSubscriptionTarget": {
             "access_level": "Undocumented",
-            "action": "StartMetadataGenerationRun",
+            "action": "CreateSubscriptionTarget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RefreshToken": {
+        "DeleteGlossaryTerm": {
             "access_level": "Undocumented",
-            "action": "RefreshToken",
+            "action": "DeleteGlossaryTerm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironmentDeploymentStatus": {
+        "DeleteSubscriptionTarget": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironmentDeploymentStatus",
+            "action": "DeleteSubscriptionTarget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironmentConfiguration": {
+        "ListSubscriptions": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironmentConfiguration",
+            "action": "ListSubscriptions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDomains": {
+        "GetDomain": {
             "access_level": "Undocumented",
-            "action": "ListDomains",
+            "action": "GetDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFormType": {
+        "CreateDomain": {
             "access_level": "Undocumented",
-            "action": "CreateFormType",
+            "action": "CreateDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Search": {
+        "GetGlossary": {
             "access_level": "Undocumented",
-            "action": "Search",
+            "action": "GetGlossary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateListingChangeSet": {
+        "ListNotifications": {
             "access_level": "Undocumented",
-            "action": "CreateListingChangeSet",
+            "action": "ListNotifications",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSourceRunActivities": {
+        "DeleteSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "ListDataSourceRunActivities",
+            "action": "DeleteSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemovePolicyGrant": {
+        "RejectSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "RemovePolicyGrant",
+            "action": "RejectSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAsset": {
+        "UpdateDataSourceRunActivities": {
             "access_level": "Undocumented",
-            "action": "DeleteAsset",
+            "action": "UpdateDataSourceRunActivities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGlossaryTerm": {
+        "GetSubscriptionEligibility": {
             "access_level": "Undocumented",
-            "action": "DeleteGlossaryTerm",
+            "action": "GetSubscriptionEligibility",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironmentProfile": {
+        "DeleteProject": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironmentProfile",
+            "action": "DeleteProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSubscriptionGrantStatus": {
+        "UpdateGlossary": {
             "access_level": "Undocumented",
-            "action": "UpdateSubscriptionGrantStatus",
+            "action": "UpdateGlossary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFormType": {
+        "CreateDataSource": {
             "access_level": "Undocumented",
-            "action": "DeleteFormType",
+            "action": "CreateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentBlueprint": {
+        "GetSubscriptionGrant": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentBlueprint",
+            "action": "GetSubscriptionGrant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSubscriptionGrant": {
+        "AddPolicyGrant": {
             "access_level": "Undocumented",
-            "action": "CreateSubscriptionGrant",
+            "action": "AddPolicyGrant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RejectPredictions": {
+        "ListDomains": {
             "access_level": "Undocumented",
-            "action": "RejectPredictions",
+            "action": "ListDomains",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscription": {
+        "CreateProjectMembership": {
             "access_level": "Undocumented",
-            "action": "GetSubscription",
+            "action": "CreateProjectMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SsoLogin": {
+        "GetFormType": {
             "access_level": "Undocumented",
-            "action": "SsoLogin",
+            "action": "GetFormType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSourceRun": {
+        "UpdateSubscriptionTarget": {
             "access_level": "Undocumented",
-            "action": "GetDataSourceRun",
+            "action": "UpdateSubscriptionTarget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAssetType": {
+        "ListSubscriptionGrants": {
             "access_level": "Undocumented",
-            "action": "CreateAssetType",
+            "action": "ListSubscriptionGrants",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PostTimeSeriesDataPoints": {
+        "GetSubscription": {
             "access_level": "Undocumented",
-            "action": "PostTimeSeriesDataPoints",
+            "action": "GetSubscription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscriptionRequestDetails": {
+        "SearchGroupProfiles": {
             "access_level": "Undocumented",
-            "action": "GetSubscriptionRequestDetails",
+            "action": "SearchGroupProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroupProfile": {
+        "GetIamPortalLoginUrl": {
             "access_level": "Undocumented",
-            "action": "GetGroupProfile",
+            "action": "GetIamPortalLoginUrl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchListings": {
+        "CancelSubscription": {
             "access_level": "Undocumented",
-            "action": "SearchListings",
+            "action": "CancelSubscription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentActionLink": {
+        "GetAssetType": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentActionLink",
+            "action": "GetAssetType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironment": {
+        "DeleteAsset": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironment",
+            "action": "DeleteAsset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGroupProfile": {
+        "SsoLogout": {
             "access_level": "Undocumented",
-            "action": "UpdateGroupProfile",
+            "action": "SsoLogout",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateProject": {
+        "UpdateEnvironmentProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateProject",
+            "action": "UpdateEnvironmentProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetadataGenerationRun": {
+        "UpdateEnvironment": {
             "access_level": "Undocumented",
-            "action": "GetMetadataGenerationRun",
+            "action": "UpdateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataSource": {
+        "UpdateGlossaryTerm": {
             "access_level": "Undocumented",
-            "action": "DeleteDataSource",
+            "action": "UpdateGlossaryTerm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateUserProfile": {
+        "CreateEnvironment": {
             "access_level": "Undocumented",
-            "action": "UpdateUserProfile",
+            "action": "CreateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFormType": {
+        "ListTimeSeriesDataPoints": {
             "access_level": "Undocumented",
-            "action": "GetFormType",
+            "action": "ListTimeSeriesDataPoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDomainSharingPolicy": {
+        "DeleteAssetType": {
             "access_level": "Undocumented",
-            "action": "DeleteDomainSharingPolicy",
+            "action": "DeleteAssetType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSubscriptionGrant": {
+        "RefreshToken": {
             "access_level": "Undocumented",
-            "action": "DeleteSubscriptionGrant",
+            "action": "RefreshToken",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSubscriptionTargets": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListSubscriptionTargets",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateGlossary": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateGlossary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDomain": {
+        "ListAccountEnvironments": {
             "access_level": "Undocumented",
-            "action": "DeleteDomain",
+            "action": "ListAccountEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscriptionEligibility": {
+        "ListSubscriptionTargets": {
             "access_level": "Undocumented",
-            "action": "GetSubscriptionEligibility",
+            "action": "ListSubscriptionTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTimeSeriesDataPoints": {
+        "DeleteTimeSeriesDataPoints": {
             "access_level": "Undocumented",
-            "action": "ListTimeSeriesDataPoints",
+            "action": "DeleteTimeSeriesDataPoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetListing": {
+        "GetGlossaryTerm": {
             "access_level": "Undocumented",
-            "action": "GetListing",
+            "action": "GetGlossaryTerm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironmentProfiles": {
+        "CreateAssetType": {
             "access_level": "Undocumented",
-            "action": "ListEnvironmentProfiles",
+            "action": "CreateAssetType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ProvisionDomain": {
+        "UpdateSubscriptionGrantStatus": {
             "access_level": "Undocumented",
-            "action": "ProvisionDomain",
+            "action": "UpdateSubscriptionGrantStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptSubscriptionRequest": {
+        "CreateSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "AcceptSubscriptionRequest",
+            "action": "CreateSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProject": {
+        "CreateGlossaryTerm": {
             "access_level": "Undocumented",
-            "action": "DeleteProject",
+            "action": "CreateGlossaryTerm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironmentBlueprintConfigurations": {
+        "PutDomainSharingPolicy": {
             "access_level": "Undocumented",
-            "action": "ListEnvironmentBlueprintConfigurations",
+            "action": "PutDomainSharingPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironmentBlueprint": {
+        "AcceptPredictions": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironmentBlueprint",
+            "action": "AcceptPredictions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSubscriptionRequest": {
+        "CreateAssetRevision": {
             "access_level": "Undocumented",
-            "action": "DeleteSubscriptionRequest",
+            "action": "CreateAssetRevision",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscriptionGrant": {
+        "ListMetadataGenerationRuns": {
             "access_level": "Undocumented",
-            "action": "GetSubscriptionGrant",
+            "action": "ListMetadataGenerationRuns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartDataSourceRun": {
+        "PostTimeSeriesDataPoints": {
             "access_level": "Undocumented",
-            "action": "StartDataSourceRun",
+            "action": "PostTimeSeriesDataPoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteProjectMembership": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteProjectMembership",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssetRevisions": {
+        "SearchTypes": {
             "access_level": "Undocumented",
-            "action": "ListAssetRevisions",
+            "action": "SearchTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironmentBlueprint": {
+        "UpdateUserProfile": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironmentBlueprint",
+            "action": "UpdateUserProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProjects": {
+        "CreateGroupProfile": {
             "access_level": "Undocumented",
-            "action": "ListProjects",
+            "action": "CreateGroupProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelMetadataGenerationRun": {
+        "ListDataSources": {
             "access_level": "Undocumented",
-            "action": "CancelMetadataGenerationRun",
+            "action": "ListDataSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUserProfile": {
+        "GetEnvironmentCredentials": {
             "access_level": "Undocumented",
-            "action": "GetUserProfile",
+            "action": "GetEnvironmentCredentials",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironment": {
+        "CreateEnvironmentBlueprint": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironment",
+            "action": "CreateEnvironmentBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentProfile": {
+        "CreateAsset": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentProfile",
+            "action": "CreateAsset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDataSource": {
+        "ListEnvironments": {
             "access_level": "Undocumented",
-            "action": "CreateDataSource",
+            "action": "ListEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidatePassRole": {
+        "PutEnvironmentBlueprintConfiguration": {
             "access_level": "Undocumented",
-            "action": "ValidatePassRole",
+            "action": "PutEnvironmentBlueprintConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentCredentials": {
+        "GetTimeSeriesDataPoint": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentCredentials",
+            "action": "GetTimeSeriesDataPoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironmentBlueprintConfiguration": {
+        "CancelMetadataGenerationRun": {
             "access_level": "Undocumented",
-            "action": "GetEnvironmentBlueprintConfiguration",
+            "action": "CancelMetadataGenerationRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProject": {
+        "ListProjectMemberships": {
             "access_level": "Undocumented",
-            "action": "GetProject",
+            "action": "ListProjectMemberships",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteEnvironmentProfile": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteEnvironmentProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDomain": {
+        "GetSubscriptionTarget": {
             "access_level": "Undocumented",
-            "action": "GetDomain",
+            "action": "GetSubscriptionTarget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSubscriptionRequests": {
+        "GetDataSource": {
             "access_level": "Undocumented",
-            "action": "ListSubscriptionRequests",
+            "action": "GetDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchUserProfiles": {
+        "CreateSubscriptionGrant": {
             "access_level": "Undocumented",
-            "action": "SearchUserProfiles",
+            "action": "CreateSubscriptionGrant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListGroupsForUser": {
             "access_level": "Undocumented",
             "action": "ListGroupsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUserProfile": {
+        "GetUserProfile": {
             "access_level": "Undocumented",
-            "action": "CreateUserProfile",
+            "action": "GetUserProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGlossary": {
+        "UpdateProject": {
             "access_level": "Undocumented",
-            "action": "GetGlossary",
+            "action": "UpdateProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProjectMembership": {
+        "ListAssetRevisions": {
             "access_level": "Undocumented",
-            "action": "DeleteProjectMembership",
+            "action": "ListAssetRevisions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSubscriptionTarget": {
+        "DeleteListing": {
             "access_level": "Undocumented",
-            "action": "GetSubscriptionTarget",
+            "action": "DeleteListing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGroupProfile": {
+        "ListEnvironmentBlueprintConfigurationSummaries": {
             "access_level": "Undocumented",
-            "action": "CreateGroupProfile",
+            "action": "ListEnvironmentBlueprintConfigurationSummaries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTimeSeriesDataPoint": {
+        "ListDataSourceRuns": {
             "access_level": "Undocumented",
-            "action": "GetTimeSeriesDataPoint",
+            "action": "ListDataSourceRuns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIamPortalLoginUrl": {
+        "UpdateEnvironmentBlueprint": {
             "access_level": "Undocumented",
-            "action": "GetIamPortalLoginUrl",
+            "action": "UpdateEnvironmentBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWarehouseMetadata": {
+        "ListPolicyGrants": {
             "access_level": "Undocumented",
-            "action": "ListWarehouseMetadata",
+            "action": "ListPolicyGrants",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironmentProfile": {
+        "SearchListings": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironmentProfile",
+            "action": "SearchListings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironment": {
+        "UpdateSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "GetEnvironment",
+            "action": "UpdateSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProject": {
+        "DeleteEnvironment": {
             "access_level": "Undocumented",
-            "action": "CreateProject",
+            "action": "DeleteEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RevokeSubscription": {
+        "ListEnvironmentProfiles": {
             "access_level": "Undocumented",
-            "action": "RevokeSubscription",
+            "action": "ListEnvironmentProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SsoLogout": {
+        "Search": {
             "access_level": "Undocumented",
-            "action": "SsoLogout",
+            "action": "Search",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddPolicyGrant": {
+        "GetSubscriptionRequestDetails": {
             "access_level": "Undocumented",
-            "action": "AddPolicyGrant",
+            "action": "GetSubscriptionRequestDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutDomainSharingPolicy": {
+        "UpdateGroupProfile": {
             "access_level": "Undocumented",
-            "action": "PutDomainSharingPolicy",
+            "action": "UpdateGroupProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSourceRunActivities": {
+        "GetAsset": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSourceRunActivities",
+            "action": "GetAsset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAsset": {
+        "GetProject": {
             "access_level": "Undocumented",
-            "action": "GetAsset",
+            "action": "GetProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGlossaryTerm": {
+        "GetEnvironmentBlueprint": {
             "access_level": "Undocumented",
-            "action": "CreateGlossaryTerm",
+            "action": "GetEnvironmentBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotifications": {
+        "GetEnvironmentProfile": {
             "access_level": "Undocumented",
-            "action": "ListNotifications",
+            "action": "GetEnvironmentProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccountEnvironments": {
+        "GetMetadataGenerationRun": {
             "access_level": "Undocumented",
-            "action": "ListAccountEnvironments",
+            "action": "GetMetadataGenerationRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProjectMemberships": {
+        "DeleteDataSource": {
             "access_level": "Undocumented",
-            "action": "ListProjectMemberships",
+            "action": "DeleteDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptPredictions": {
+        "UpdateEnvironmentConfiguration": {
             "access_level": "Undocumented",
-            "action": "AcceptPredictions",
+            "action": "UpdateEnvironmentConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDomainSharingPolicy": {
+        "AcceptSubscriptionRequest": {
             "access_level": "Undocumented",
-            "action": "GetDomainSharingPolicy",
+            "action": "AcceptSubscriptionRequest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSubscriptionTarget": {
+        "CreateListingChangeSet": {
             "access_level": "Undocumented",
-            "action": "UpdateSubscriptionTarget",
+            "action": "CreateListingChangeSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSourceRuns": {
+        "StartDataSourceRun": {
             "access_level": "Undocumented",
-            "action": "ListDataSourceRuns",
+            "action": "StartDataSourceRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSources": {
+        "DeleteSubscriptionGrant": {
             "access_level": "Undocumented",
-            "action": "ListDataSources",
+            "action": "DeleteSubscriptionGrant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSubscriptionRequest": {
+        "DeleteFormType": {
             "access_level": "Undocumented",
-            "action": "UpdateSubscriptionRequest",
+            "action": "DeleteFormType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDomain": {
+        "ListProjects": {
             "access_level": "Undocumented",
-            "action": "UpdateDomain",
+            "action": "ListProjects",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteListing": {
+        "GetEnvironmentActionLink": {
             "access_level": "Undocumented",
-            "action": "DeleteListing",
+            "action": "GetEnvironmentActionLink",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironmentBlueprint": {
+        "GetEnvironment": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironmentBlueprint",
+            "action": "GetEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironmentBlueprintConfiguration": {
+        "GetListing": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironmentBlueprintConfiguration",
+            "action": "GetListing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironments": {
+        "SsoLogin": {
             "access_level": "Undocumented",
-            "action": "ListEnvironments",
+            "action": "SsoLogin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironmentBlueprintConfigurationSummaries": {
+        "ListDataSourceRunActivities": {
             "access_level": "Undocumented",
-            "action": "ListEnvironmentBlueprintConfigurationSummaries",
+            "action": "ListDataSourceRunActivities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSubscriptionTarget": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteSubscriptionTarget",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGlossary": {
+        "GetGroupProfile": {
             "access_level": "Undocumented",
-            "action": "CreateGlossary",
+            "action": "GetGroupProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchGroupProfiles": {
+        "ProvisionDomain": {
             "access_level": "Undocumented",
-            "action": "SearchGroupProfiles",
+            "action": "ProvisionDomain",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironmentProfile": {
+        "UpdateEnvironmentDeploymentStatus": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironmentProfile",
+            "action": "UpdateEnvironmentDeploymentStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironment": {
+        "DeleteEnvironmentBlueprint": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironment",
+            "action": "DeleteEnvironmentBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RejectSubscriptionRequest": {
+        "GetEnvironmentBlueprintConfiguration": {
             "access_level": "Undocumented",
-            "action": "RejectSubscriptionRequest",
+            "action": "GetEnvironmentBlueprintConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDomain": {
+        "DeleteEnvironmentBlueprintConfiguration": {
             "access_level": "Undocumented",
-            "action": "CreateDomain",
+            "action": "DeleteEnvironmentBlueprintConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTimeSeriesDataPoints": {
+        "CreateEnvironmentProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteTimeSeriesDataPoints",
+            "action": "CreateEnvironmentProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelSubscription": {
+        "CreateProject": {
             "access_level": "Undocumented",
-            "action": "CancelSubscription",
+            "action": "CreateProject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProjectMembership": {
+        "CreateUserProfile": {
             "access_level": "Undocumented",
-            "action": "CreateProjectMembership",
+            "action": "CreateUserProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironmentBlueprints": {
+        "RejectPredictions": {
             "access_level": "Undocumented",
-            "action": "ListEnvironmentBlueprints",
+            "action": "RejectPredictions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAssetRevision": {
+        "DeleteDomainSharingPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateAssetRevision",
+            "action": "DeleteDomainSharingPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSubscriptionTarget": {
+        "CreateFormType": {
             "access_level": "Undocumented",
-            "action": "CreateSubscriptionTarget",
+            "action": "CreateFormType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "dax": {
@@ -41456,833 +41456,833 @@
             "condition_keys": [],
             "description": "Grants permission to update query tab",
             "orphan": false,
             "resources": []
         }
     },
     "deadline": {
-        "GetSession": {
+        "PutMeteredProduct": {
             "access_level": "Undocumented",
-            "action": "GetSession",
+            "action": "PutMeteredProduct",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateStorageProfile": {
+        "GetSessionAction": {
             "access_level": "Undocumented",
-            "action": "UpdateStorageProfile",
+            "action": "GetSessionAction",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSessionsStatisticsAggregation": {
+        "UpdateFleet": {
             "access_level": "Undocumented",
-            "action": "GetSessionsStatisticsAggregation",
+            "action": "UpdateFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateQueueEnvironment": {
+        "GetStorageProfile": {
             "access_level": "Undocumented",
-            "action": "CreateQueueEnvironment",
+            "action": "GetStorageProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMonitor": {
+        "ListStorageProfilesForQueue": {
             "access_level": "Undocumented",
-            "action": "UpdateMonitor",
+            "action": "ListStorageProfilesForQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateStep": {
+        "DeleteMeteredProduct": {
             "access_level": "Undocumented",
-            "action": "UpdateStep",
+            "action": "DeleteMeteredProduct",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateQueue": {
+        "CreateJob": {
             "access_level": "Undocumented",
-            "action": "UpdateQueue",
+            "action": "CreateJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTasks": {
+        "AssumeFleetRoleForRead": {
             "access_level": "Undocumented",
-            "action": "ListTasks",
+            "action": "AssumeFleetRoleForRead",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFleet": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateFleet",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueueFleetAssociations": {
+        "AssumeFleetRoleForWorker": {
             "access_level": "Undocumented",
-            "action": "ListQueueFleetAssociations",
+            "action": "AssumeFleetRoleForWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTask": {
+        "CreateFarm": {
             "access_level": "Undocumented",
-            "action": "GetTask",
+            "action": "CreateFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueues": {
+        "ListJobMembers": {
             "access_level": "Undocumented",
-            "action": "ListQueues",
+            "action": "ListJobMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateJob": {
+        "CreateBudget": {
             "access_level": "Undocumented",
-            "action": "CreateJob",
+            "action": "CreateBudget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteLicenseEndpoint": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteLicenseEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchTasks": {
+        "DeleteQueue": {
             "access_level": "Undocumented",
-            "action": "SearchTasks",
+            "action": "DeleteQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutMeteredProduct": {
+        "UpdateStep": {
             "access_level": "Undocumented",
-            "action": "PutMeteredProduct",
+            "action": "UpdateStep",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFleetMembers": {
+        "SearchSteps": {
             "access_level": "Undocumented",
-            "action": "ListFleetMembers",
+            "action": "SearchSteps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStorageProfiles": {
+        "CreateQueueEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListStorageProfiles",
+            "action": "CreateQueueEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWorker": {
+        "AssociateMemberToFarm": {
             "access_level": "Undocumented",
-            "action": "UpdateWorker",
+            "action": "AssociateMemberToFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueueEnvironment": {
+        "DeleteFleet": {
             "access_level": "Undocumented",
-            "action": "DeleteQueueEnvironment",
+            "action": "DeleteFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStepDependencies": {
+        "AssumeQueueRoleForRead": {
             "access_level": "Undocumented",
-            "action": "ListStepDependencies",
+            "action": "AssumeQueueRoleForRead",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetStorageProfile": {
+        "BatchGetJobEntity": {
             "access_level": "Undocumented",
-            "action": "GetStorageProfile",
+            "action": "BatchGetJobEntity",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkers": {
+        "DisassociateMemberFromFarm": {
             "access_level": "Undocumented",
-            "action": "ListWorkers",
+            "action": "DisassociateMemberFromFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueue": {
+        "CopyJobTemplate": {
             "access_level": "Undocumented",
-            "action": "DeleteQueue",
+            "action": "CopyJobTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMonitor": {
+        "DeleteFarm": {
             "access_level": "Undocumented",
-            "action": "CreateMonitor",
+            "action": "DeleteFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBudget": {
+        "AssociateMemberToQueue": {
             "access_level": "Undocumented",
-            "action": "GetBudget",
+            "action": "AssociateMemberToQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetStorageProfileForQueue": {
+        "DeleteBudget": {
             "access_level": "Undocumented",
-            "action": "GetStorageProfileForQueue",
+            "action": "DeleteBudget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMeteredProduct": {
+        "DisassociateMemberFromFleet": {
             "access_level": "Undocumented",
-            "action": "DeleteMeteredProduct",
+            "action": "DisassociateMemberFromFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQueue": {
+        "CreateLicenseEndpoint": {
             "access_level": "Undocumented",
-            "action": "GetQueue",
+            "action": "CreateLicenseEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFleets": {
+        "ListFleetMembers": {
             "access_level": "Undocumented",
-            "action": "ListFleets",
+            "action": "ListFleetMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetJobEntity": {
+        "StartSessionsStatisticsAggregation": {
             "access_level": "Undocumented",
-            "action": "BatchGetJobEntity",
+            "action": "StartSessionsStatisticsAggregation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFarms": {
+        "GetQueue": {
             "access_level": "Undocumented",
-            "action": "ListFarms",
+            "action": "GetQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQueueEnvironment": {
+        "ListFarms": {
             "access_level": "Undocumented",
-            "action": "GetQueueEnvironment",
+            "action": "ListFarms",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWorker": {
+        "UpdateQueue": {
             "access_level": "Undocumented",
-            "action": "CreateWorker",
+            "action": "UpdateQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSessions": {
+        "GetApplicationVersion": {
             "access_level": "Undocumented",
-            "action": "ListSessions",
+            "action": "GetApplicationVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeFleetRoleForRead": {
+        "GetTask": {
             "access_level": "Undocumented",
-            "action": "AssumeFleetRoleForRead",
+            "action": "GetTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateQueueFleetAssociation": {
+        "ListQueueMembers": {
             "access_level": "Undocumented",
-            "action": "CreateQueueFleetAssociation",
+            "action": "ListQueueMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetStep": {
+        "DeleteStorageProfile": {
             "access_level": "Undocumented",
-            "action": "GetStep",
+            "action": "DeleteStorageProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListLicenseEndpoints": {
+        "UpdateSession": {
             "access_level": "Undocumented",
-            "action": "ListLicenseEndpoints",
+            "action": "UpdateSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListJobs": {
+        "UpdateMonitor": {
             "access_level": "Undocumented",
-            "action": "ListJobs",
+            "action": "UpdateMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSessionsForWorker": {
+        "SearchWorkers": {
             "access_level": "Undocumented",
-            "action": "ListSessionsForWorker",
+            "action": "SearchWorkers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchJobs": {
+        "ListAvailableMeteredProducts": {
             "access_level": "Undocumented",
-            "action": "SearchJobs",
+            "action": "ListAvailableMeteredProducts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSteps": {
+        "DisassociateMemberFromJob": {
             "access_level": "Undocumented",
-            "action": "ListSteps",
+            "action": "DisassociateMemberFromJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorker": {
+        "GetLicenseEndpoint": {
             "access_level": "Undocumented",
-            "action": "GetWorker",
+            "action": "GetLicenseEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQueueFleetAssociation": {
+        "ListWorkers": {
             "access_level": "Undocumented",
-            "action": "GetQueueFleetAssociation",
+            "action": "ListWorkers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFarm": {
+        "UpdateJob": {
             "access_level": "Undocumented",
-            "action": "DeleteFarm",
+            "action": "UpdateJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFarmMembers": {
+        "ListMonitors": {
             "access_level": "Undocumented",
-            "action": "ListFarmMembers",
+            "action": "ListMonitors",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateQueueFleetAssociation": {
+        "GetSession": {
             "access_level": "Undocumented",
-            "action": "UpdateQueueFleetAssociation",
+            "action": "GetSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLicenseEndpoint": {
+        "GetStep": {
             "access_level": "Undocumented",
-            "action": "GetLicenseEndpoint",
+            "action": "GetStep",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteLicenseEndpoint": {
+        "CreateFleet": {
             "access_level": "Undocumented",
-            "action": "DeleteLicenseEndpoint",
+            "action": "CreateFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchWorkers": {
+        "GetQueueFleetAssociation": {
             "access_level": "Undocumented",
-            "action": "SearchWorkers",
+            "action": "GetQueueFleetAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteStorageProfile": {
+        "SearchJobs": {
             "access_level": "Undocumented",
-            "action": "DeleteStorageProfile",
+            "action": "SearchJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMeteredProducts": {
+        "DeleteQueueEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListMeteredProducts",
+            "action": "DeleteQueueEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateFleet": {
+        "CreateStorageProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateFleet",
+            "action": "CreateStorageProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateLicenseEndpoint": {
+        "DisassociateMemberFromQueue": {
             "access_level": "Undocumented",
-            "action": "CreateLicenseEndpoint",
+            "action": "DisassociateMemberFromQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMemberToFarm": {
+        "ListBudgets": {
             "access_level": "Undocumented",
-            "action": "AssociateMemberToFarm",
+            "action": "ListBudgets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMonitors": {
+        "GetJob": {
             "access_level": "Undocumented",
-            "action": "ListMonitors",
+            "action": "GetJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CopyJobTemplate": {
+        "ListSessions": {
             "access_level": "Undocumented",
-            "action": "CopyJobTemplate",
+            "action": "ListSessions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStepConsumers": {
+        "ListSessionActions": {
             "access_level": "Undocumented",
-            "action": "ListStepConsumers",
+            "action": "ListSessionActions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateQueue": {
+        "ListJobs": {
             "access_level": "Undocumented",
-            "action": "CreateQueue",
+            "action": "ListJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeQueueRoleForRead": {
+        "UpdateTask": {
             "access_level": "Undocumented",
-            "action": "AssumeQueueRoleForRead",
+            "action": "UpdateTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeFleetRoleForWorker": {
+        "ListQueueEnvironments": {
             "access_level": "Undocumented",
-            "action": "AssumeFleetRoleForWorker",
+            "action": "ListQueueEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListBudgets": {
+        "ListQueues": {
             "access_level": "Undocumented",
-            "action": "ListBudgets",
+            "action": "ListQueues",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMemberToJob": {
+        "ListTasks": {
             "access_level": "Undocumented",
-            "action": "AssociateMemberToJob",
+            "action": "ListTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetApplicationVersion": {
+        "UpdateWorkerSchedule": {
             "access_level": "Undocumented",
-            "action": "GetApplicationVersion",
+            "action": "UpdateWorkerSchedule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFarm": {
+        "ListStepConsumers": {
             "access_level": "Undocumented",
-            "action": "CreateFarm",
+            "action": "ListStepConsumers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteBudget": {
+        "CreateWorker": {
             "access_level": "Undocumented",
-            "action": "DeleteBudget",
+            "action": "CreateWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteWorker": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListJobMembers": {
+        "SearchTasks": {
             "access_level": "Undocumented",
-            "action": "ListJobMembers",
+            "action": "SearchTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMemberFromJob": {
+        "UpdateQueueFleetAssociation": {
             "access_level": "Undocumented",
-            "action": "DisassociateMemberFromJob",
+            "action": "UpdateQueueFleetAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMonitor": {
+        "AssociateMemberToFleet": {
             "access_level": "Undocumented",
-            "action": "GetMonitor",
+            "action": "AssociateMemberToFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMemberFromFarm": {
+        "GetQueueEnvironment": {
             "access_level": "Undocumented",
-            "action": "DisassociateMemberFromFarm",
+            "action": "GetQueueEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateJob": {
+        "UpdateStorageProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateJob",
+            "action": "UpdateStorageProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetJob": {
+        "ListQueueFleetAssociations": {
             "access_level": "Undocumented",
-            "action": "GetJob",
+            "action": "ListQueueFleetAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFleet": {
+        "GetFleet": {
             "access_level": "Undocumented",
-            "action": "DeleteFleet",
+            "action": "GetFleet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateBudget": {
+        "UpdateFarm": {
             "access_level": "Undocumented",
-            "action": "UpdateBudget",
+            "action": "UpdateFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSession": {
+        "AssumeQueueRoleForUser": {
             "access_level": "Undocumented",
-            "action": "UpdateSession",
+            "action": "AssumeQueueRoleForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeQueueRoleForUser": {
+        "GetMonitor": {
             "access_level": "Undocumented",
-            "action": "AssumeQueueRoleForUser",
+            "action": "GetMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWorkerSchedule": {
+        "CreateQueue": {
             "access_level": "Undocumented",
-            "action": "UpdateWorkerSchedule",
+            "action": "CreateQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFarm": {
+        "ListFleets": {
             "access_level": "Undocumented",
-            "action": "GetFarm",
+            "action": "ListFleets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateStorageProfile": {
+        "ListSteps": {
             "access_level": "Undocumented",
-            "action": "CreateStorageProfile",
+            "action": "ListSteps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSessionAction": {
+        "ListMeteredProducts": {
             "access_level": "Undocumented",
-            "action": "GetSessionAction",
+            "action": "ListMeteredProducts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMemberFromQueue": {
+        "DeleteMonitor": {
             "access_level": "Undocumented",
-            "action": "DisassociateMemberFromQueue",
+            "action": "DeleteMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueueEnvironments": {
+        "GetWorker": {
             "access_level": "Undocumented",
-            "action": "ListQueueEnvironments",
+            "action": "GetWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueueFleetAssociation": {
+        "ListStepDependencies": {
             "access_level": "Undocumented",
-            "action": "DeleteQueueFleetAssociation",
+            "action": "ListStepDependencies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartSessionsStatisticsAggregation": {
+        "AssumeQueueRoleForWorker": {
             "access_level": "Undocumented",
-            "action": "StartSessionsStatisticsAggregation",
+            "action": "AssumeQueueRoleForWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStorageProfilesForQueue": {
+        "DeleteQueueFleetAssociation": {
             "access_level": "Undocumented",
-            "action": "ListStorageProfilesForQueue",
+            "action": "DeleteQueueFleetAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFleet": {
+        "GetBudget": {
             "access_level": "Undocumented",
-            "action": "GetFleet",
+            "action": "GetBudget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateBudget": {
+        "GetSessionsStatisticsAggregation": {
             "access_level": "Undocumented",
-            "action": "CreateBudget",
+            "action": "GetSessionsStatisticsAggregation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateQueueEnvironment": {
+        "UpdateBudget": {
             "access_level": "Undocumented",
-            "action": "UpdateQueueEnvironment",
+            "action": "UpdateBudget",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssumeQueueRoleForWorker": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "AssumeQueueRoleForWorker",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSessionActions": {
+        "ListLicenseEndpoints": {
             "access_level": "Undocumented",
-            "action": "ListSessionActions",
+            "action": "ListLicenseEndpoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "UpdateQueueEnvironment": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "UpdateQueueEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAvailableMeteredProducts": {
+        "ListFarmMembers": {
             "access_level": "Undocumented",
-            "action": "ListAvailableMeteredProducts",
+            "action": "ListFarmMembers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWorker": {
+        "UpdateWorker": {
             "access_level": "Undocumented",
-            "action": "DeleteWorker",
+            "action": "UpdateWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTask": {
+        "ListStorageProfiles": {
             "access_level": "Undocumented",
-            "action": "UpdateTask",
+            "action": "ListStorageProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMonitor": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteMonitor",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMemberToFleet": {
+        "GetStorageProfileForQueue": {
             "access_level": "Undocumented",
-            "action": "AssociateMemberToFleet",
+            "action": "GetStorageProfileForQueue",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchSteps": {
+        "AssociateMemberToJob": {
             "access_level": "Undocumented",
-            "action": "SearchSteps",
+            "action": "AssociateMemberToJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueueMembers": {
+        "CreateMonitor": {
             "access_level": "Undocumented",
-            "action": "ListQueueMembers",
+            "action": "CreateMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMemberToQueue": {
+        "GetFarm": {
             "access_level": "Undocumented",
-            "action": "AssociateMemberToQueue",
+            "action": "GetFarm",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMemberFromFleet": {
+        "ListSessionsForWorker": {
             "access_level": "Undocumented",
-            "action": "DisassociateMemberFromFleet",
+            "action": "ListSessionsForWorker",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateFarm": {
+        "CreateQueueFleetAssociation": {
             "access_level": "Undocumented",
-            "action": "UpdateFarm",
+            "action": "CreateQueueFleetAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "deepcomposer": {
@@ -64775,305 +64775,305 @@
             ],
             "description": "Grants permission to replace the current set of policies for the specified load balancer port with the specified set of policies",
             "orphan": false,
             "resources": [
                 "loadbalancer"
             ]
         },
-        "DescribeTrustStores": {
+        "CreateTargetGroup": {
             "access_level": "Undocumented",
-            "action": "DescribeTrustStores",
+            "action": "CreateTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateListener": {
+        "DescribeTargetGroups": {
             "access_level": "Undocumented",
-            "action": "CreateListener",
+            "action": "DescribeTargetGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTrustStoreRevocationContent": {
+        "RegisterTargets": {
             "access_level": "Undocumented",
-            "action": "GetTrustStoreRevocationContent",
+            "action": "RegisterTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyRule": {
+        "ModifyTrustStore": {
             "access_level": "Undocumented",
-            "action": "ModifyRule",
+            "action": "ModifyTrustStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeRules": {
+        "SetRulePriorities": {
             "access_level": "Undocumented",
-            "action": "DescribeRules",
+            "action": "SetRulePriorities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteListener": {
+        "DescribeSSLPolicies": {
             "access_level": "Undocumented",
-            "action": "DeleteListener",
+            "action": "DescribeSSLPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetWebAcl": {
+        "RemoveTrustStoreRevocations": {
             "access_level": "Undocumented",
-            "action": "SetWebAcl",
+            "action": "RemoveTrustStoreRevocations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTrustStore": {
+        "SetWebAcl": {
             "access_level": "Undocumented",
-            "action": "DeleteTrustStore",
+            "action": "SetWebAcl",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTrustStore": {
+        "DeleteTargetGroup": {
             "access_level": "Undocumented",
-            "action": "CreateTrustStore",
+            "action": "DeleteTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetGroupAttributes": {
+        "DeleteListener": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetGroupAttributes",
+            "action": "DeleteListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTrustStoreRevocations": {
+        "DescribeTrustStores": {
             "access_level": "Undocumented",
-            "action": "DescribeTrustStoreRevocations",
+            "action": "DescribeTrustStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeListeners": {
+        "DeleteTrustStore": {
             "access_level": "Undocumented",
-            "action": "DescribeListeners",
+            "action": "DeleteTrustStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTrustStoreAssociations": {
+        "DescribeListeners": {
             "access_level": "Undocumented",
-            "action": "DescribeTrustStoreAssociations",
+            "action": "DescribeListeners",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ModifyTargetGroup": {
             "access_level": "Undocumented",
             "action": "ModifyTargetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddListenerCertificates": {
+        "DeleteRule": {
             "access_level": "Undocumented",
-            "action": "AddListenerCertificates",
+            "action": "DeleteRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "SetSubnets": {
             "access_level": "Undocumented",
             "action": "SetSubnets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetHealth": {
+        "CreateTrustStore": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetHealth",
+            "action": "CreateTrustStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterTargets": {
+        "DescribeTrustStoreAssociations": {
             "access_level": "Undocumented",
-            "action": "DeregisterTargets",
+            "action": "DescribeTrustStoreAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeTargetGroups": {
+        "SetSecurityGroups": {
             "access_level": "Undocumented",
-            "action": "DescribeTargetGroups",
+            "action": "SetSecurityGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetRulePriorities": {
+        "RemoveListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "SetRulePriorities",
+            "action": "RemoveListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetIpAddressType": {
+        "DescribeListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "SetIpAddressType",
+            "action": "DescribeListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRule": {
+        "DeregisterTargets": {
             "access_level": "Undocumented",
-            "action": "DeleteRule",
+            "action": "DeregisterTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeListenerCertificates": {
+        "ModifyRule": {
             "access_level": "Undocumented",
-            "action": "DescribeListenerCertificates",
+            "action": "ModifyRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTargetGroup": {
+        "DescribeAccountLimits": {
             "access_level": "Undocumented",
-            "action": "DeleteTargetGroup",
+            "action": "DescribeAccountLimits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveTrustStoreRevocations": {
+        "DescribeRules": {
             "access_level": "Undocumented",
-            "action": "RemoveTrustStoreRevocations",
+            "action": "DescribeRules",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterTargets": {
+        "ModifyListener": {
             "access_level": "Undocumented",
-            "action": "RegisterTargets",
+            "action": "ModifyListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeSSLPolicies": {
+        "DescribeTrustStoreRevocations": {
             "access_level": "Undocumented",
-            "action": "DescribeSSLPolicies",
+            "action": "DescribeTrustStoreRevocations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddTrustStoreRevocations": {
+        "AddListenerCertificates": {
             "access_level": "Undocumented",
-            "action": "AddTrustStoreRevocations",
+            "action": "AddListenerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyTargetGroupAttributes": {
+        "GetTrustStoreCaCertificatesBundle": {
             "access_level": "Undocumented",
-            "action": "ModifyTargetGroupAttributes",
+            "action": "GetTrustStoreCaCertificatesBundle",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRule": {
+        "DescribeTargetHealth": {
             "access_level": "Undocumented",
-            "action": "CreateRule",
+            "action": "DescribeTargetHealth",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyListener": {
+        "AddTrustStoreRevocations": {
             "access_level": "Undocumented",
-            "action": "ModifyListener",
+            "action": "AddTrustStoreRevocations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ModifyTrustStore": {
+        "GetTrustStoreRevocationContent": {
             "access_level": "Undocumented",
-            "action": "ModifyTrustStore",
+            "action": "GetTrustStoreRevocationContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAccountLimits": {
+        "SetIpAddressType": {
             "access_level": "Undocumented",
-            "action": "DescribeAccountLimits",
+            "action": "SetIpAddressType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTrustStoreCaCertificatesBundle": {
+        "DescribeTargetGroupAttributes": {
             "access_level": "Undocumented",
-            "action": "GetTrustStoreCaCertificatesBundle",
+            "action": "DescribeTargetGroupAttributes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTargetGroup": {
+        "CreateRule": {
             "access_level": "Undocumented",
-            "action": "CreateTargetGroup",
+            "action": "CreateRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSecurityGroups": {
+        "CreateListener": {
             "access_level": "Undocumented",
-            "action": "SetSecurityGroups",
+            "action": "CreateListener",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveListenerCertificates": {
+        "ModifyTargetGroupAttributes": {
             "access_level": "Undocumented",
-            "action": "RemoveListenerCertificates",
+            "action": "ModifyTargetGroupAttributes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "elasticmapreduce": {
@@ -66745,305 +66745,305 @@
             "orphan": false,
             "resources": [
                 "application"
             ]
         }
     },
     "entityresolution": {
-        "ListIdMappingJobs": {
+        "GetIdMappingWorkflow": {
             "access_level": "Undocumented",
-            "action": "ListIdMappingJobs",
+            "action": "GetIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UseIdNamespace": {
+        "CreateIdNamespace": {
             "access_level": "Undocumented",
-            "action": "UseIdNamespace",
+            "action": "CreateIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIdNamespace": {
+        "StartIdMappingJob": {
             "access_level": "Undocumented",
-            "action": "UpdateIdNamespace",
+            "action": "StartIdMappingJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIdMappingWorkflow": {
+        "GetPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteIdMappingWorkflow",
+            "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMatchingWorkflow": {
+        "GetProviderService": {
             "access_level": "Undocumented",
-            "action": "CreateMatchingWorkflow",
+            "action": "GetProviderService",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMatchingWorkflow": {
+        "GetSchemaMapping": {
             "access_level": "Undocumented",
-            "action": "GetMatchingWorkflow",
+            "action": "GetSchemaMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UpdateSchemaMapping": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UpdateSchemaMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UseIdNamespace": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UseIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMatchingJobs": {
+        "GetIdNamespace": {
             "access_level": "Undocumented",
-            "action": "ListMatchingJobs",
+            "action": "GetIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMatchingWorkflow": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteMatchingWorkflow",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyStatement": {
+        "ListMatchingJobs": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyStatement",
+            "action": "ListMatchingJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIdMappingWorkflows": {
+        "DeleteSchemaMapping": {
             "access_level": "Undocumented",
-            "action": "ListIdMappingWorkflows",
+            "action": "DeleteSchemaMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutPolicy": {
+        "DeletePolicyStatement": {
             "access_level": "Undocumented",
-            "action": "PutPolicy",
+            "action": "DeletePolicyStatement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProviderServices": {
+        "GetMatchingWorkflow": {
             "access_level": "Undocumented",
-            "action": "ListProviderServices",
+            "action": "GetMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchemaMapping": {
+        "PutPolicy": {
             "access_level": "Undocumented",
-            "action": "GetSchemaMapping",
+            "action": "PutPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartMatchingJob": {
+        "ListProviderServices": {
             "access_level": "Undocumented",
-            "action": "StartMatchingJob",
+            "action": "ListProviderServices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdNamespace": {
+        "GetMatchId": {
             "access_level": "Undocumented",
-            "action": "GetIdNamespace",
+            "action": "GetMatchId",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMatchingWorkflows": {
+        "DeleteMatchingWorkflow": {
             "access_level": "Undocumented",
-            "action": "ListMatchingWorkflows",
+            "action": "DeleteMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicy": {
+        "CreateMatchingWorkflow": {
             "access_level": "Undocumented",
-            "action": "GetPolicy",
+            "action": "CreateMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSchemaMapping": {
+        "ListMatchingWorkflows": {
             "access_level": "Undocumented",
-            "action": "CreateSchemaMapping",
+            "action": "ListMatchingWorkflows",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSchemaMappings": {
+        "DeleteIdMappingWorkflow": {
             "access_level": "Undocumented",
-            "action": "ListSchemaMappings",
+            "action": "DeleteIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIdMappingWorkflow": {
+        "GetMatchingJob": {
             "access_level": "Undocumented",
-            "action": "CreateIdMappingWorkflow",
+            "action": "GetMatchingJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMatchId": {
+        "ListIdNamespaces": {
             "access_level": "Undocumented",
-            "action": "GetMatchId",
+            "action": "ListIdNamespaces",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSchemaMapping": {
+        "AddPolicyStatement": {
             "access_level": "Undocumented",
-            "action": "UpdateSchemaMapping",
+            "action": "AddPolicyStatement",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddPolicyStatement": {
+        "CreateIdMappingWorkflow": {
             "access_level": "Undocumented",
-            "action": "AddPolicyStatement",
+            "action": "CreateIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMatchingWorkflow": {
+        "GetIdMappingJob": {
             "access_level": "Undocumented",
-            "action": "UpdateMatchingWorkflow",
+            "action": "GetIdMappingJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListIdMappingWorkflows": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListIdMappingWorkflows",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIdNamespace": {
+        "UpdateIdMappingWorkflow": {
             "access_level": "Undocumented",
-            "action": "DeleteIdNamespace",
+            "action": "UpdateIdMappingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdMappingJob": {
+        "ListIdMappingJobs": {
             "access_level": "Undocumented",
-            "action": "GetIdMappingJob",
+            "action": "ListIdMappingJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIdNamespaces": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListIdNamespaces",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartIdMappingJob": {
+        "UpdateMatchingWorkflow": {
             "access_level": "Undocumented",
-            "action": "StartIdMappingJob",
+            "action": "UpdateMatchingWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIdMappingWorkflow": {
+        "UpdateIdNamespace": {
             "access_level": "Undocumented",
-            "action": "UpdateIdMappingWorkflow",
+            "action": "UpdateIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSchemaMapping": {
+        "StartMatchingJob": {
             "access_level": "Undocumented",
-            "action": "DeleteSchemaMapping",
+            "action": "StartMatchingJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetProviderService": {
+        "CreateSchemaMapping": {
             "access_level": "Undocumented",
-            "action": "GetProviderService",
+            "action": "CreateSchemaMapping",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMatchingJob": {
+        "ListSchemaMappings": {
             "access_level": "Undocumented",
-            "action": "GetMatchingJob",
+            "action": "ListSchemaMappings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIdNamespace": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "CreateIdNamespace",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdMappingWorkflow": {
+        "DeleteIdNamespace": {
             "access_level": "Undocumented",
-            "action": "GetIdMappingWorkflow",
+            "action": "DeleteIdNamespace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "es": {
@@ -69761,225 +69761,225 @@
             "orphan": false,
             "resources": [
                 "deliverystream"
             ]
         }
     },
     "fis": {
-        "ListExperiments": {
+        "CreateTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListExperiments",
+            "action": "CreateTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTargetResourceTypes": {
+        "InjectApiInternalError": {
             "access_level": "Undocumented",
-            "action": "ListTargetResourceTypes",
+            "action": "InjectApiInternalError",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InjectApiInternalError": {
+        "InjectApiUnavailableError": {
             "access_level": "Undocumented",
-            "action": "InjectApiInternalError",
+            "action": "InjectApiUnavailableError",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExperiment": {
+        "GetTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetExperiment",
+            "action": "GetTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartExperiment": {
+        "GetExperimentTemplate": {
             "access_level": "Undocumented",
-            "action": "StartExperiment",
+            "action": "GetExperimentTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTargetAccountConfigurations": {
+        "GetExperiment": {
             "access_level": "Undocumented",
-            "action": "ListTargetAccountConfigurations",
+            "action": "GetExperiment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExperimentTargetAccountConfiguration": {
+        "InjectApiThrottleError": {
             "access_level": "Undocumented",
-            "action": "GetExperimentTargetAccountConfiguration",
+            "action": "InjectApiThrottleError",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateExperimentTemplate": {
+        "ListTargetAccountConfigurations": {
             "access_level": "Undocumented",
-            "action": "CreateExperimentTemplate",
+            "action": "ListTargetAccountConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExperimentTargetAccountConfigurations": {
+        "ListExperimentResolvedTargets": {
             "access_level": "Undocumented",
-            "action": "ListExperimentTargetAccountConfigurations",
+            "action": "ListExperimentResolvedTargets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExperimentResolvedTargets": {
+        "DeleteTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListExperimentResolvedTargets",
+            "action": "DeleteTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteExperimentTemplate": {
+        "GetAction": {
             "access_level": "Undocumented",
-            "action": "DeleteExperimentTemplate",
+            "action": "GetAction",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExperimentTemplates": {
+        "StopExperiment": {
             "access_level": "Undocumented",
-            "action": "ListExperimentTemplates",
+            "action": "StopExperiment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTargetAccountConfiguration": {
+        "DeleteExperimentTemplate": {
             "access_level": "Undocumented",
-            "action": "DeleteTargetAccountConfiguration",
+            "action": "DeleteExperimentTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTargetAccountConfiguration": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetTargetAccountConfiguration",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UpdateTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UpdateTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAction": {
+        "ListExperimentTargetAccountConfigurations": {
             "access_level": "Undocumented",
-            "action": "GetAction",
+            "action": "ListExperimentTargetAccountConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetTargetResourceType": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetTargetResourceType",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTargetAccountConfiguration": {
+        "ListActions": {
             "access_level": "Undocumented",
-            "action": "UpdateTargetAccountConfiguration",
+            "action": "ListActions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InjectApiThrottleError": {
+        "GetExperimentTargetAccountConfiguration": {
             "access_level": "Undocumented",
-            "action": "InjectApiThrottleError",
+            "action": "GetExperimentTargetAccountConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExperimentTemplate": {
+        "StartExperiment": {
             "access_level": "Undocumented",
-            "action": "GetExperimentTemplate",
+            "action": "StartExperiment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateExperimentTemplate": {
             "access_level": "Undocumented",
             "action": "UpdateExperimentTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InjectApiUnavailableError": {
+        "ListTargetResourceTypes": {
             "access_level": "Undocumented",
-            "action": "InjectApiUnavailableError",
+            "action": "ListTargetResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopExperiment": {
+        "ListExperimentTemplates": {
             "access_level": "Undocumented",
-            "action": "StopExperiment",
+            "action": "ListExperimentTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListActions": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListActions",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTargetResourceType": {
+        "ListExperiments": {
             "access_level": "Undocumented",
-            "action": "GetTargetResourceType",
+            "action": "ListExperiments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTargetAccountConfiguration": {
+        "CreateExperimentTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateTargetAccountConfiguration",
+            "action": "CreateExperimentTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "fms": {
@@ -80394,169 +80394,169 @@
             "condition_keys": [],
             "description": "Grants permission to enable the Organizational View feature",
             "orphan": false,
             "resources": []
         }
     },
     "healthlake": {
-        "ReadResource": {
+        "ListFHIRDatastores": {
             "access_level": "Undocumented",
-            "action": "ReadResource",
+            "action": "ListFHIRDatastores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeFHIRImportJob": {
+        "StartFHIRExportJob": {
             "access_level": "Undocumented",
-            "action": "DescribeFHIRImportJob",
+            "action": "StartFHIRExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeFHIRDatastore": {
+        "CreateFHIRDatastore": {
             "access_level": "Undocumented",
-            "action": "DescribeFHIRDatastore",
+            "action": "CreateFHIRDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFHIRExportJobs": {
+        "DescribeFHIRExportJob": {
             "access_level": "Undocumented",
-            "action": "ListFHIRExportJobs",
+            "action": "DescribeFHIRExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFHIRDatastore": {
+        "ReadResource": {
             "access_level": "Undocumented",
-            "action": "CreateFHIRDatastore",
+            "action": "ReadResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFHIRDatastore": {
+        "SearchWithGet": {
             "access_level": "Undocumented",
-            "action": "DeleteFHIRDatastore",
+            "action": "SearchWithGet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeFHIRExportJob": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DescribeFHIRExportJob",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartFHIRImportJob": {
+        "ListFHIRImportJobs": {
             "access_level": "Undocumented",
-            "action": "StartFHIRImportJob",
+            "action": "ListFHIRImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFHIRImportJobs": {
+        "DescribeFHIRImportJob": {
             "access_level": "Undocumented",
-            "action": "ListFHIRImportJobs",
+            "action": "DescribeFHIRImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchWithGet": {
+        "UpdateResource": {
             "access_level": "Undocumented",
-            "action": "SearchWithGet",
+            "action": "UpdateResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetCapabilities": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetCapabilities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartFHIRExportJob": {
+        "DescribeFHIRDatastore": {
             "access_level": "Undocumented",
-            "action": "StartFHIRExportJob",
+            "action": "DescribeFHIRDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchWithPost": {
+        "DeleteFHIRDatastore": {
             "access_level": "Undocumented",
-            "action": "SearchWithPost",
+            "action": "DeleteFHIRDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFHIRDatastores": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ListFHIRDatastores",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "SearchWithPost": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "SearchWithPost",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "StartFHIRImportJob": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "StartFHIRImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCapabilities": {
+        "ListFHIRExportJobs": {
             "access_level": "Undocumented",
-            "action": "GetCapabilities",
+            "action": "ListFHIRExportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResource": {
+        "CreateResource": {
             "access_level": "Undocumented",
-            "action": "DeleteResource",
+            "action": "CreateResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResource": {
+        "DeleteResource": {
             "access_level": "Undocumented",
-            "action": "UpdateResource",
+            "action": "DeleteResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "honeycode": {
@@ -80822,1377 +80822,1377 @@
             "condition_keys": [],
             "description": "Grants permission to update an Amazon Honeycode team for your AWS Account",
             "orphan": false,
             "resources": []
         }
     },
     "iam": {
-        "ListCloudFrontPublicKeys": {
+        "CreateAccountAlias": {
             "access_level": "Undocumented",
-            "action": "ListCloudFrontPublicKeys",
+            "action": "CreateAccountAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPoliciesGrantingServiceAccess": {
+        "SetDefaultPolicyVersion": {
             "access_level": "Undocumented",
-            "action": "ListPoliciesGrantingServiceAccess",
+            "action": "SetDefaultPolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLastAccessedDetails": {
+        "PutRolePolicy": {
             "access_level": "Undocumented",
-            "action": "GetServiceLastAccessedDetails",
+            "action": "PutRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateInstanceProfile": {
+        "GetAccountName": {
             "access_level": "Undocumented",
-            "action": "CreateInstanceProfile",
+            "action": "GetAccountName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGroup": {
+        "CreateVirtualMFADevice": {
             "access_level": "Undocumented",
-            "action": "CreateGroup",
+            "action": "CreateVirtualMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOpenIDConnectProvider": {
+        "CreatePolicy": {
             "access_level": "Undocumented",
-            "action": "GetOpenIDConnectProvider",
+            "action": "CreatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSSHPublicKeys": {
+        "UpdateCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "ListSSHPublicKeys",
+            "action": "UpdateCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLinkedRoleDeletionStatus": {
+        "DeleteSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "GetServiceLinkedRoleDeletionStatus",
+            "action": "DeleteSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOpenIDConnectProviderTags": {
+        "UpdateRoleDescription": {
             "access_level": "Undocumented",
-            "action": "ListOpenIDConnectProviderTags",
+            "action": "UpdateRoleDescription",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSigningCertificates": {
+        "DeleteRolePolicy": {
             "access_level": "Undocumented",
-            "action": "ListSigningCertificates",
+            "action": "DeleteRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyVersion": {
+        "GetContextKeysForCustomPolicy": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyVersion",
+            "action": "GetContextKeysForCustomPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddUserToGroup": {
+        "GetServiceLinkedRoleDeletionStatus": {
             "access_level": "Undocumented",
-            "action": "AddUserToGroup",
+            "action": "GetServiceLinkedRoleDeletionStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagInstanceProfile": {
+        "ListServiceSpecificCredentials": {
             "access_level": "Undocumented",
-            "action": "UntagInstanceProfile",
+            "action": "ListServiceSpecificCredentials",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceLinkedRole": {
+        "GetAccountSummary": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceLinkedRole",
+            "action": "GetAccountSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagInstanceProfile": {
+        "UpdateLoginProfile": {
             "access_level": "Undocumented",
-            "action": "TagInstanceProfile",
+            "action": "UpdateLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountAuthorizationDetails": {
+        "ListAccountAliases": {
             "access_level": "Undocumented",
-            "action": "GetAccountAuthorizationDetails",
+            "action": "ListAccountAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountEmailAddress": {
+        "ListMFADevices": {
             "access_level": "Undocumented",
-            "action": "GetAccountEmailAddress",
+            "action": "ListMFADevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccessKey": {
+        "GetCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "DeleteAccessKey",
+            "action": "GetCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUserPolicy": {
+        "DeleteServiceLinkedRole": {
             "access_level": "Undocumented",
-            "action": "PutUserPolicy",
+            "action": "DeleteServiceLinkedRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateUser": {
+        "UntagPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateUser",
+            "action": "UntagPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagRole": {
+        "UpdateRole": {
             "access_level": "Undocumented",
-            "action": "UntagRole",
+            "action": "UpdateRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUser": {
+        "GenerateCredentialReport": {
             "access_level": "Undocumented",
-            "action": "GetUser",
+            "action": "GenerateCredentialReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteLoginProfile": {
+        "ListPolicyVersions": {
             "access_level": "Undocumented",
-            "action": "DeleteLoginProfile",
+            "action": "ListPolicyVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSTSRegionalEndpointStatus": {
+        "ChangePassword": {
             "access_level": "Undocumented",
-            "action": "SetSTSRegionalEndpointStatus",
+            "action": "ChangePassword",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateOpenIDConnectProviderThumbprint": {
+        "GetCredentialReport": {
             "access_level": "Undocumented",
-            "action": "UpdateOpenIDConnectProviderThumbprint",
+            "action": "GetCredentialReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagRole": {
+        "CreateGroup": {
             "access_level": "Undocumented",
-            "action": "TagRole",
+            "action": "CreateGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSAMLProvider": {
+        "ListCloudFrontPublicKeys": {
             "access_level": "Undocumented",
-            "action": "GetSAMLProvider",
+            "action": "ListCloudFrontPublicKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicy": {
+        "GetUserPolicy": {
             "access_level": "Undocumented",
-            "action": "GetPolicy",
+            "action": "GetUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfilesForRole": {
+        "AttachGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfilesForRole",
+            "action": "AttachGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccessKey": {
+        "ListGroupPolicies": {
             "access_level": "Undocumented",
-            "action": "CreateAccessKey",
+            "action": "ListGroupPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfiles": {
+        "TagSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfiles",
+            "action": "TagSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddRoleToInstanceProfile": {
+        "CreateInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "AddRoleToInstanceProfile",
+            "action": "CreateInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateServiceSpecificCredential": {
+        "UpdateSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "UpdateServiceSpecificCredential",
+            "action": "UpdateSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServerCertificateTags": {
+        "ListUserPolicies": {
             "access_level": "Undocumented",
-            "action": "ListServerCertificateTags",
+            "action": "ListUserPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateServiceLastAccessedDetails": {
+        "GetServiceLastAccessedDetailsWithEntities": {
             "access_level": "Undocumented",
-            "action": "GenerateServiceLastAccessedDetails",
+            "action": "GetServiceLastAccessedDetailsWithEntities",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOpenIDConnectProvider": {
+        "SimulateCustomPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteOpenIDConnectProvider",
+            "action": "SimulateCustomPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagServerCertificate": {
+        "GetGroup": {
             "access_level": "Undocumented",
-            "action": "TagServerCertificate",
+            "action": "GetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSAMLProviders": {
+        "GenerateServiceLastAccessedDetails": {
             "access_level": "Undocumented",
-            "action": "ListSAMLProviders",
+            "action": "GenerateServiceLastAccessedDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetSecurityTokenServicePreferences": {
+        "ListInstanceProfileTags": {
             "access_level": "Undocumented",
-            "action": "SetSecurityTokenServicePreferences",
+            "action": "ListInstanceProfileTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagPolicy": {
+        "UntagOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "TagPolicy",
+            "action": "UntagOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateCredentialReport": {
+        "GetServerCertificate": {
             "access_level": "Undocumented",
-            "action": "GenerateCredentialReport",
+            "action": "GetServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMFADeviceTags": {
+        "DetachRolePolicy": {
             "access_level": "Undocumented",
-            "action": "ListMFADeviceTags",
+            "action": "DetachRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SimulateCustomPolicy": {
+        "UntagUser": {
             "access_level": "Undocumented",
-            "action": "SimulateCustomPolicy",
+            "action": "UntagUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceLinkedRole": {
+        "TagUser": {
             "access_level": "Undocumented",
-            "action": "CreateServiceLinkedRole",
+            "action": "TagUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRolePolicy": {
+        "UpdateSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "GetRolePolicy",
+            "action": "UpdateSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagOpenIDConnectProvider": {
+        "UploadServerCertificate": {
             "access_level": "Undocumented",
-            "action": "TagOpenIDConnectProvider",
+            "action": "UploadServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SimulatePrincipalPolicy": {
+        "GetRole": {
             "access_level": "Undocumented",
-            "action": "SimulatePrincipalPolicy",
+            "action": "GetRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContextKeysForCustomPolicy": {
+        "CreateAccessKey": {
             "access_level": "Undocumented",
-            "action": "GetContextKeysForCustomPolicy",
+            "action": "CreateAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSAMLProviderTags": {
+        "UpdateAssumeRolePolicy": {
             "access_level": "Undocumented",
-            "action": "ListSAMLProviderTags",
+            "action": "UpdateAssumeRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResyncMFADevice": {
+        "ListAttachedRolePolicies": {
             "access_level": "Undocumented",
-            "action": "ResyncMFADevice",
+            "action": "ListAttachedRolePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSAMLProvider": {
+        "ListSSHPublicKeys": {
             "access_level": "Undocumented",
-            "action": "UpdateSAMLProvider",
+            "action": "ListSSHPublicKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetDefaultPolicyVersion": {
+        "ListSTSRegionalEndpointsStatus": {
             "access_level": "Undocumented",
-            "action": "SetDefaultPolicyVersion",
+            "action": "ListSTSRegionalEndpointsStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceLastAccessedDetailsWithEntities": {
+        "DeleteGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "GetServiceLastAccessedDetailsWithEntities",
+            "action": "DeleteGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachRolePolicy": {
+        "CreateSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "AttachRolePolicy",
+            "action": "CreateSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagOpenIDConnectProvider": {
+        "GetAccountEmailAddress": {
             "access_level": "Undocumented",
-            "action": "UntagOpenIDConnectProvider",
+            "action": "GetAccountEmailAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccessKeyLastUsed": {
+        "UntagRole": {
             "access_level": "Undocumented",
-            "action": "GetAccessKeyLastUsed",
+            "action": "UntagRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachGroupPolicy": {
+        "PutUserPermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "AttachGroupPolicy",
+            "action": "PutUserPermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteCloudFrontPublicKey": {
+        "AddRoleToInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteCloudFrontPublicKey",
+            "action": "AddRoleToInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateOrganizationsAccessReport": {
+        "GetRolePolicy": {
             "access_level": "Undocumented",
-            "action": "GenerateOrganizationsAccessReport",
+            "action": "GetRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedGroupPolicies": {
+        "UpdateGroup": {
             "access_level": "Undocumented",
-            "action": "ListAttachedGroupPolicies",
+            "action": "UpdateGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateLoginProfile": {
+        "ListGroups": {
             "access_level": "Undocumented",
-            "action": "UpdateLoginProfile",
+            "action": "ListGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSigningCertificate": {
+        "GetContextKeysForPrincipalPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteSigningCertificate",
+            "action": "GetContextKeysForPrincipalPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupPolicies": {
+        "UpdateServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "ListGroupPolicies",
+            "action": "UpdateServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveUserFromGroup": {
+        "GetServiceLastAccessedDetails": {
             "access_level": "Undocumented",
-            "action": "RemoveUserFromGroup",
+            "action": "GetServiceLastAccessedDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateCloudFrontPublicKey": {
+        "UpdateAccountEmailAddress": {
             "access_level": "Undocumented",
-            "action": "UpdateCloudFrontPublicKey",
+            "action": "UpdateAccountEmailAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceSpecificCredential": {
+        "GetOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceSpecificCredential",
+            "action": "GetOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroup": {
+        "GetInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "GetGroup",
+            "action": "GetInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMFADevices": {
+        "UntagServerCertificate": {
             "access_level": "Undocumented",
-            "action": "ListMFADevices",
+            "action": "UntagServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInstanceProfile": {
+        "DeleteRolePermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "GetInstanceProfile",
+            "action": "DeleteRolePermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEntitiesForPolicy": {
+        "UpdateAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "ListEntitiesForPolicy",
+            "action": "UpdateAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadSigningCertificate": {
+        "PassRole": {
             "access_level": "Undocumented",
-            "action": "UploadSigningCertificate",
+            "action": "PassRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteInstanceProfile": {
+        "PutGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteInstanceProfile",
+            "action": "PutGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroups": {
+        "ListSAMLProviders": {
             "access_level": "Undocumented",
-            "action": "ListGroups",
+            "action": "ListSAMLProviders",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUserPolicy": {
+        "DeleteAccessKey": {
             "access_level": "Undocumented",
-            "action": "DeleteUserPolicy",
+            "action": "DeleteAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddClientIDToOpenIDConnectProvider": {
+        "DetachGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "AddClientIDToOpenIDConnectProvider",
+            "action": "DetachGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSSHPublicKey": {
+        "UpdateOpenIDConnectProviderThumbprint": {
             "access_level": "Undocumented",
-            "action": "GetSSHPublicKey",
+            "action": "UpdateOpenIDConnectProviderThumbprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRole": {
+        "GetUser": {
             "access_level": "Undocumented",
-            "action": "UpdateRole",
+            "action": "GetUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateServerCertificate": {
+        "DeleteUserPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateServerCertificate",
+            "action": "DeleteUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSTSRegionalEndpointsStatus": {
+        "ListPolicyTags": {
             "access_level": "Undocumented",
-            "action": "ListSTSRegionalEndpointsStatus",
+            "action": "ListPolicyTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PassRole": {
+        "DeleteInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "PassRole",
+            "action": "DeleteInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveClientIDFromOpenIDConnectProvider": {
+        "AddUserToGroup": {
             "access_level": "Undocumented",
-            "action": "RemoveClientIDFromOpenIDConnectProvider",
+            "action": "AddUserToGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRolePolicy": {
+        "DeleteAccountAlias": {
             "access_level": "Undocumented",
-            "action": "PutRolePolicy",
+            "action": "DeleteAccountAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachRolePolicy": {
+        "ListMFADeviceTags": {
             "access_level": "Undocumented",
-            "action": "DetachRolePolicy",
+            "action": "ListMFADeviceTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountPasswordPolicy": {
+        "ListVirtualMFADevices": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountPasswordPolicy",
+            "action": "ListVirtualMFADevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAssumeRolePolicy": {
+        "PutUserPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateAssumeRolePolicy",
+            "action": "PutUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableMFADevice": {
+        "DeleteServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "EnableMFADevice",
+            "action": "DeleteServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountSummary": {
+        "DetachUserPolicy": {
             "access_level": "Undocumented",
-            "action": "GetAccountSummary",
+            "action": "DetachUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContextKeysForPrincipalPolicy": {
+        "DeleteUser": {
             "access_level": "Undocumented",
-            "action": "GetContextKeysForPrincipalPolicy",
+            "action": "DeleteUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccountPasswordPolicy": {
+        "DeleteCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "DeleteAccountPasswordPolicy",
+            "action": "DeleteCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountEmailAddress": {
+        "PutRolePermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountEmailAddress",
+            "action": "PutRolePermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateVirtualMFADevice": {
+        "GetAccessKeyLastUsed": {
             "access_level": "Undocumented",
-            "action": "CreateVirtualMFADevice",
+            "action": "GetAccessKeyLastUsed",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCredentialReport": {
+        "ResetServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "GetCredentialReport",
+            "action": "ResetServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUser": {
+        "CreateLoginProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteUser",
+            "action": "CreateLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAccountAlias": {
+        "UploadSigningCertificate": {
             "access_level": "Undocumented",
-            "action": "DeleteAccountAlias",
+            "action": "UploadSigningCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyVersion": {
+        "GetAccountAuthorizationDetails": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyVersion",
+            "action": "GetAccountAuthorizationDetails",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLoginProfile": {
+        "GetPolicy": {
             "access_level": "Undocumented",
-            "action": "GetLoginProfile",
+            "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRolePermissionsBoundary": {
+        "UpdateServerCertificate": {
             "access_level": "Undocumented",
-            "action": "PutRolePermissionsBoundary",
+            "action": "UpdateServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagSAMLProvider": {
+        "GetOrganizationsAccessReport": {
             "access_level": "Undocumented",
-            "action": "UntagSAMLProvider",
+            "action": "GetOrganizationsAccessReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServerCertificate": {
+        "CreateServiceSpecificCredential": {
             "access_level": "Undocumented",
-            "action": "DeleteServerCertificate",
+            "action": "CreateServiceSpecificCredential",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroupPolicy": {
+        "UpdateUser": {
             "access_level": "Undocumented",
-            "action": "DeleteGroupPolicy",
+            "action": "UpdateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSAMLProvider": {
+        "ListPolicies": {
             "access_level": "Undocumented",
-            "action": "DeleteSAMLProvider",
+            "action": "ListPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagPolicy": {
+        "DeletePolicyVersion": {
             "access_level": "Undocumented",
-            "action": "UntagPolicy",
+            "action": "DeletePolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRole": {
+        "ListServerCertificateTags": {
             "access_level": "Undocumented",
-            "action": "GetRole",
+            "action": "ListServerCertificateTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUsers": {
+        "ListOpenIDConnectProviders": {
             "access_level": "Undocumented",
-            "action": "ListUsers",
+            "action": "ListOpenIDConnectProviders",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccessKey": {
+        "CreateOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "UpdateAccessKey",
+            "action": "CreateOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAccountAlias": {
+        "DeleteServerCertificate": {
             "access_level": "Undocumented",
-            "action": "CreateAccountAlias",
+            "action": "DeleteServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutGroupPolicy": {
+        "AttachUserPolicy": {
             "access_level": "Undocumented",
-            "action": "PutGroupPolicy",
+            "action": "AttachUserPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroupsForUser": {
+        "CreatePolicyVersion": {
             "access_level": "Undocumented",
-            "action": "ListGroupsForUser",
+            "action": "CreatePolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountPasswordPolicy": {
+        "DeletePolicy": {
             "access_level": "Undocumented",
-            "action": "GetAccountPasswordPolicy",
+            "action": "DeletePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSSHPublicKey": {
+        "ListSigningCertificates": {
             "access_level": "Undocumented",
-            "action": "DeleteSSHPublicKey",
+            "action": "ListSigningCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServerCertificate": {
+        "UntagMFADevice": {
             "access_level": "Undocumented",
-            "action": "GetServerCertificate",
+            "action": "UntagMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRoleTags": {
+        "EnableMFADevice": {
             "access_level": "Undocumented",
-            "action": "ListRoleTags",
+            "action": "EnableMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadCloudFrontPublicKey": {
+        "ListAttachedGroupPolicies": {
             "access_level": "Undocumented",
-            "action": "UploadCloudFrontPublicKey",
+            "action": "ListAttachedGroupPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyTags": {
+        "ListUserTags": {
             "access_level": "Undocumented",
-            "action": "ListPolicyTags",
+            "action": "ListUserTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroup": {
+        "CreateRole": {
             "access_level": "Undocumented",
-            "action": "DeleteGroup",
+            "action": "CreateRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetCloudFrontPublicKey": {
+        "ListUsers": {
             "access_level": "Undocumented",
-            "action": "GetCloudFrontPublicKey",
+            "action": "ListUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagUser": {
+        "TagPolicy": {
             "access_level": "Undocumented",
-            "action": "TagUser",
+            "action": "TagPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagUser": {
+        "TagInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "UntagUser",
+            "action": "TagInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOpenIDConnectProviders": {
+        "ListAttachedUserPolicies": {
             "access_level": "Undocumented",
-            "action": "ListOpenIDConnectProviders",
+            "action": "ListAttachedUserPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListVirtualMFADevices": {
+        "GetMFADevice": {
             "access_level": "Undocumented",
-            "action": "ListVirtualMFADevices",
+            "action": "GetMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadSSHPublicKey": {
+        "SimulatePrincipalPolicy": {
             "access_level": "Undocumented",
-            "action": "UploadSSHPublicKey",
+            "action": "SimulatePrincipalPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServerCertificates": {
+        "ListInstanceProfilesForRole": {
             "access_level": "Undocumented",
-            "action": "ListServerCertificates",
+            "action": "ListInstanceProfilesForRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSigningCertificate": {
+        "UntagInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateSigningCertificate",
+            "action": "UntagInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRolePolicy": {
+        "ListGroupsForUser": {
             "access_level": "Undocumented",
-            "action": "DeleteRolePolicy",
+            "action": "ListGroupsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyVersions": {
+        "UpdateAccountName": {
             "access_level": "Undocumented",
-            "action": "ListPolicyVersions",
+            "action": "UpdateAccountName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicy": {
+        "TagServerCertificate": {
             "access_level": "Undocumented",
-            "action": "CreatePolicy",
+            "action": "TagServerCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeactivateMFADevice": {
+        "GetLoginProfile": {
             "access_level": "Undocumented",
-            "action": "DeactivateMFADevice",
+            "action": "GetLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAccountName": {
+        "RemoveUserFromGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateAccountName",
+            "action": "RemoveUserFromGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ChangePassword": {
+        "RemoveClientIDFromOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "ChangePassword",
+            "action": "RemoveClientIDFromOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstanceProfileTags": {
+        "ListInstanceProfiles": {
             "access_level": "Undocumented",
-            "action": "ListInstanceProfileTags",
+            "action": "ListInstanceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUserPermissionsBoundary": {
+        "GetSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "DeleteUserPermissionsBoundary",
+            "action": "GetSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUser": {
+        "AddClientIDToOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "CreateUser",
+            "action": "AddClientIDToOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRolePermissionsBoundary": {
+        "GetPolicyVersion": {
             "access_level": "Undocumented",
-            "action": "DeleteRolePermissionsBoundary",
+            "action": "GetPolicyVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagServerCertificate": {
+        "SetSTSRegionalEndpointStatus": {
             "access_level": "Undocumented",
-            "action": "UntagServerCertificate",
+            "action": "SetSTSRegionalEndpointStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadServerCertificate": {
+        "UpdateSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "UploadServerCertificate",
+            "action": "UpdateSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserPolicies": {
+        "ListEntitiesForPolicy": {
             "access_level": "Undocumented",
-            "action": "ListUserPolicies",
+            "action": "ListEntitiesForPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetServiceSpecificCredential": {
+        "DeactivateMFADevice": {
             "access_level": "Undocumented",
-            "action": "ResetServiceSpecificCredential",
+            "action": "DeactivateMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUserPolicy": {
+        "TagMFADevice": {
             "access_level": "Undocumented",
-            "action": "GetUserPolicy",
+            "action": "TagMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagSAMLProvider": {
+        "DeleteSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "TagSAMLProvider",
+            "action": "DeleteSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicy": {
+        "SetSecurityTokenServicePreferences": {
             "access_level": "Undocumented",
-            "action": "DeletePolicy",
+            "action": "SetSecurityTokenServicePreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicies": {
+        "UploadSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "ListPolicies",
+            "action": "UploadSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSAMLProvider": {
+        "ListSAMLProviderTags": {
             "access_level": "Undocumented",
-            "action": "CreateSAMLProvider",
+            "action": "ListSAMLProviderTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateLoginProfile": {
+        "RemoveRoleFromInstanceProfile": {
             "access_level": "Undocumented",
-            "action": "CreateLoginProfile",
+            "action": "RemoveRoleFromInstanceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AttachUserPolicy": {
+        "DeleteSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "AttachUserPolicy",
+            "action": "DeleteSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRole": {
+        "DeleteGroup": {
             "access_level": "Undocumented",
-            "action": "CreateRole",
+            "action": "DeleteGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroupPolicy": {
+        "AttachRolePolicy": {
             "access_level": "Undocumented",
-            "action": "GetGroupPolicy",
+            "action": "AttachRolePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagMFADevice": {
+        "TagOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "UntagMFADevice",
+            "action": "TagOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMFADevice": {
+        "TagRole": {
             "access_level": "Undocumented",
-            "action": "GetMFADevice",
+            "action": "TagRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRoles": {
+        "GetGroupPolicy": {
             "access_level": "Undocumented",
-            "action": "ListRoles",
+            "action": "GetGroupPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicyVersion": {
+        "ListRoleTags": {
             "access_level": "Undocumented",
-            "action": "GetPolicyVersion",
+            "action": "ListRoleTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveRoleFromInstanceProfile": {
+        "DeleteUserPermissionsBoundary": {
             "access_level": "Undocumented",
-            "action": "RemoveRoleFromInstanceProfile",
+            "action": "DeleteUserPermissionsBoundary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAccountName": {
+        "ListOpenIDConnectProviderTags": {
             "access_level": "Undocumented",
-            "action": "GetAccountName",
+            "action": "ListOpenIDConnectProviderTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteVirtualMFADevice": {
+        "DeleteLoginProfile": {
             "access_level": "Undocumented",
-            "action": "DeleteVirtualMFADevice",
+            "action": "DeleteLoginProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRoleDescription": {
+        "ListRolePolicies": {
             "access_level": "Undocumented",
-            "action": "UpdateRoleDescription",
+            "action": "ListRolePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedUserPolicies": {
+        "ListServerCertificates": {
             "access_level": "Undocumented",
-            "action": "ListAttachedUserPolicies",
+            "action": "ListServerCertificates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteRole": {
             "access_level": "Undocumented",
             "action": "DeleteRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachGroupPolicy": {
+        "UploadCloudFrontPublicKey": {
             "access_level": "Undocumented",
-            "action": "DetachGroupPolicy",
+            "action": "UploadCloudFrontPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAttachedRolePolicies": {
+        "DeleteVirtualMFADevice": {
             "access_level": "Undocumented",
-            "action": "ListAttachedRolePolicies",
+            "action": "DeleteVirtualMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServiceSpecificCredentials": {
+        "CreateUser": {
             "access_level": "Undocumented",
-            "action": "ListServiceSpecificCredentials",
+            "action": "CreateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagMFADevice": {
+        "ListAccessKeys": {
             "access_level": "Undocumented",
-            "action": "TagMFADevice",
+            "action": "ListAccessKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSSHPublicKey": {
+        "CreateServiceLinkedRole": {
             "access_level": "Undocumented",
-            "action": "UpdateSSHPublicKey",
+            "action": "CreateServiceLinkedRole",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateOpenIDConnectProvider": {
+        "ResyncMFADevice": {
             "access_level": "Undocumented",
-            "action": "CreateOpenIDConnectProvider",
+            "action": "ResyncMFADevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceSpecificCredential": {
+        "GetAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateServiceSpecificCredential",
+            "action": "GetAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutUserPermissionsBoundary": {
+        "ListPoliciesGrantingServiceAccess": {
             "access_level": "Undocumented",
-            "action": "PutUserPermissionsBoundary",
+            "action": "ListPoliciesGrantingServiceAccess",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccessKeys": {
+        "DeleteAccountPasswordPolicy": {
             "access_level": "Undocumented",
-            "action": "ListAccessKeys",
+            "action": "DeleteAccountPasswordPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOrganizationsAccessReport": {
+        "GetSSHPublicKey": {
             "access_level": "Undocumented",
-            "action": "GetOrganizationsAccessReport",
+            "action": "GetSSHPublicKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserTags": {
+        "UntagSAMLProvider": {
             "access_level": "Undocumented",
-            "action": "ListUserTags",
+            "action": "UntagSAMLProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGroup": {
+        "UpdateAccessKey": {
             "access_level": "Undocumented",
-            "action": "UpdateGroup",
+            "action": "UpdateAccessKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DetachUserPolicy": {
+        "DeleteOpenIDConnectProvider": {
             "access_level": "Undocumented",
-            "action": "DetachUserPolicy",
+            "action": "DeleteOpenIDConnectProvider",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAccountAliases": {
+        "ListRoles": {
             "access_level": "Undocumented",
-            "action": "ListAccountAliases",
+            "action": "ListRoles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRolePolicies": {
+        "GenerateOrganizationsAccessReport": {
             "access_level": "Undocumented",
-            "action": "ListRolePolicies",
+            "action": "GenerateOrganizationsAccessReport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "identity-sync": {
@@ -84415,22 +84415,14 @@
             "orphan": false,
             "resources": [
                 "Monitor"
             ]
         }
     },
     "invoicing": {
-        "ListInvoiceSummaries": {
-            "access_level": "Undocumented",
-            "action": "ListInvoiceSummaries",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
         "GetInvoiceEmailDeliveryPreferences": {
             "access_level": "Undocumented",
             "action": "GetInvoiceEmailDeliveryPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -84446,14 +84438,22 @@
         "PutInvoiceEmailDeliveryPreferences": {
             "access_level": "Undocumented",
             "action": "PutInvoiceEmailDeliveryPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
+        },
+        "ListInvoiceSummaries": {
+            "access_level": "Undocumented",
+            "action": "ListInvoiceSummaries",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         }
     },
     "iot": {
         "AcceptCertificateTransfer": {
             "access_level": "Write",
             "action": "AcceptCertificateTransfer",
             "condition_keys": [],
@@ -90614,913 +90614,913 @@
             "orphan": false,
             "resources": [
                 "workspace"
             ]
         }
     },
     "iotwireless": {
-        "DeleteWirelessGatewayTask": {
+        "DeleteNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGatewayTask",
+            "action": "DeleteNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayTaskDefinition": {
+        "CreateNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayTaskDefinition",
+            "action": "CreateNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDestination": {
+        "UpdateLogLevelsByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "CreateDestination",
+            "action": "UpdateLogLevelsByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEventConfigurationByResourceTypes": {
+        "ListPositionConfigurations": {
             "access_level": "Undocumented",
-            "action": "GetEventConfigurationByResourceTypes",
+            "action": "ListPositionConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDestination": {
+        "GetWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "GetDestination",
+            "action": "GetWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceProfile": {
+        "ListWirelessDeviceImportTasks": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceProfile",
+            "action": "ListWirelessDeviceImportTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePosition": {
+        "DeleteWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "UpdatePosition",
+            "action": "DeleteWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMulticastGroup": {
+        "DisassociateWirelessDeviceFromThing": {
             "access_level": "Undocumented",
-            "action": "GetMulticastGroup",
+            "action": "DisassociateWirelessDeviceFromThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourceEventConfiguration": {
+        "UpdateMetricConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdateResourceEventConfiguration",
+            "action": "UpdateMetricConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithThing": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithThing",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithFuotaTask": {
+        "ListWirelessDevices": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithFuotaTask",
+            "action": "ListWirelessDevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartFuotaTask": {
+        "DeleteMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "StartFuotaTask",
+            "action": "DeleteMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMulticastGroups": {
+        "DisassociateWirelessDeviceFromMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "ListMulticastGroups",
+            "action": "DisassociateWirelessDeviceFromMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessDeviceWithMulticastGroup": {
+        "GetResourcePosition": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessDeviceWithMulticastGroup",
+            "action": "GetResourcePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPosition": {
+        "CreateWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "GetPosition",
+            "action": "CreateWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessDeviceImportTasks": {
+        "GetWirelessGatewayCertificate": {
             "access_level": "Undocumented",
-            "action": "ListWirelessDeviceImportTasks",
+            "action": "GetWirelessGatewayCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceLogLevel": {
+        "DeleteWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "GetResourceLogLevel",
+            "action": "DeleteWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromFuotaTask": {
+        "CreateServiceProfile": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromFuotaTask",
+            "action": "CreateServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessDeviceImportTask": {
+        "CreateDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessDeviceImportTask",
+            "action": "CreateDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNetworkAnalyzerConfiguration": {
+        "UpdateResourcePosition": {
             "access_level": "Undocumented",
-            "action": "GetNetworkAnalyzerConfiguration",
+            "action": "UpdateResourcePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceEndpoint": {
+        "GetMetricConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetServiceEndpoint",
+            "action": "GetMetricConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayFirmwareInformation": {
+        "DeleteQueuedMessages": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayFirmwareInformation",
+            "action": "DeleteQueuedMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromThing": {
+        "GetServiceProfile": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromThing",
+            "action": "GetServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateAwsAccountWithPartnerAccount": {
+        "TestWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "AssociateAwsAccountWithPartnerAccount",
+            "action": "TestWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLogLevelsByResourceTypes": {
+        "AssociateWirelessGatewayWithThing": {
             "access_level": "Undocumented",
-            "action": "GetLogLevelsByResourceTypes",
+            "action": "AssociateWirelessGatewayWithThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDeviceImportTask": {
+        "AssociateWirelessDeviceWithFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDeviceImportTask",
+            "action": "AssociateWirelessDeviceWithFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDeviceProfile": {
+        "GetLogLevelsByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "DeleteDeviceProfile",
+            "action": "GetLogLevelsByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TestWirelessDevice": {
+        "GetMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "TestWirelessDevice",
+            "action": "GetMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartBulkDisassociateWirelessDeviceFromMulticastGroup": {
+        "PutPositionConfiguration": {
             "access_level": "Undocumented",
-            "action": "StartBulkDisassociateWirelessDeviceFromMulticastGroup",
+            "action": "PutPositionConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateNetworkAnalyzerConfiguration": {
+        "DisassociateWirelessGatewayFromCertificate": {
             "access_level": "Undocumented",
-            "action": "CreateNetworkAnalyzerConfiguration",
+            "action": "DisassociateWirelessGatewayFromCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayStatistics": {
+        "UpdateWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayStatistics",
+            "action": "UpdateWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessDeviceImportTask": {
+        "CreateDestination": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessDeviceImportTask",
+            "action": "CreateDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEventConfigurationByResourceTypes": {
+        "GetPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "UpdateEventConfigurationByResourceTypes",
+            "action": "GetPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPositionConfiguration": {
+        "StartNetworkAnalyzerStream": {
             "access_level": "Undocumented",
-            "action": "GetPositionConfiguration",
+            "action": "StartNetworkAnalyzerStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPartnerAccounts": {
+        "GetResourceEventConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListPartnerAccounts",
+            "action": "GetResourceEventConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDestinations": {
+        "DeleteWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "ListDestinations",
+            "action": "DeleteWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDevicesForWirelessDeviceImportTask": {
+        "DisassociateMulticastGroupFromFuotaTask": {
             "access_level": "Undocumented",
-            "action": "ListDevicesForWirelessDeviceImportTask",
+            "action": "DisassociateMulticastGroupFromFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetResourceLogLevel": {
+        "GetWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "ResetResourceLogLevel",
+            "action": "GetWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutPositionConfiguration": {
+        "AssociateMulticastGroupWithFuotaTask": {
             "access_level": "Undocumented",
-            "action": "PutPositionConfiguration",
+            "action": "AssociateMulticastGroupWithFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateLogLevelsByResourceTypes": {
+        "DisassociateWirelessGatewayFromThing": {
             "access_level": "Undocumented",
-            "action": "UpdateLogLevelsByResourceTypes",
+            "action": "DisassociateWirelessGatewayFromThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayCertificate": {
+        "UpdateFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayCertificate",
+            "action": "UpdateFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEventConfigurations": {
+        "GetWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "ListEventConfigurations",
+            "action": "GetWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServiceProfile": {
+        "GetWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "CreateServiceProfile",
+            "action": "GetWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPositionConfigurations": {
+        "GetNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListPositionConfigurations",
+            "action": "GetNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceProfiles": {
+        "ListServiceProfiles": {
             "access_level": "Undocumented",
-            "action": "ListDeviceProfiles",
+            "action": "ListServiceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessGatewayTaskDefinitions": {
+        "ListEventConfigurations": {
             "access_level": "Undocumented",
-            "action": "ListWirelessGatewayTaskDefinitions",
+            "action": "ListEventConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMulticastGroupsByFuotaTask": {
+        "AssociateWirelessDeviceWithThing": {
             "access_level": "Undocumented",
-            "action": "ListMulticastGroupsByFuotaTask",
+            "action": "AssociateWirelessDeviceWithThing",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDeviceStatistics": {
+        "CreateWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDeviceStatistics",
+            "action": "CreateWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartMulticastGroupSession": {
+        "DeregisterWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "StartMulticastGroupSession",
+            "action": "DeregisterWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartSingleWirelessDeviceImportTask": {
+        "GetWirelessGatewayFirmwareInformation": {
             "access_level": "Undocumented",
-            "action": "StartSingleWirelessDeviceImportTask",
+            "action": "GetWirelessGatewayFirmwareInformation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMulticastGroup": {
+        "StartBulkAssociateWirelessDeviceWithMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateMulticastGroup",
+            "action": "StartBulkAssociateWirelessDeviceWithMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessGatewayFromCertificate": {
+        "GetFuotaTask": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessGatewayFromCertificate",
+            "action": "GetFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNetworkAnalyzerConfigurations": {
+        "UpdateEventConfigurationByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "ListNetworkAnalyzerConfigurations",
+            "action": "UpdateEventConfigurationByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourcePosition": {
+        "DisassociateWirelessDeviceFromFuotaTask": {
             "access_level": "Undocumented",
-            "action": "UpdateResourcePosition",
+            "action": "DisassociateWirelessDeviceFromFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessDevice": {
+        "GetPositionConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetWirelessDevice",
+            "action": "GetPositionConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServiceProfile": {
+        "ListDeviceProfiles": {
             "access_level": "Undocumented",
-            "action": "DeleteServiceProfile",
+            "action": "ListDeviceProfiles",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFuotaTasks": {
+        "DeleteWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "ListFuotaTasks",
+            "action": "DeleteWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessDevice": {
+        "DisassociateAwsAccountFromPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessDevice",
+            "action": "DisassociateAwsAccountFromPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueuedMessages": {
+        "DeleteServiceProfile": {
             "access_level": "Undocumented",
-            "action": "ListQueuedMessages",
+            "action": "DeleteServiceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartNetworkAnalyzerStream": {
+        "GetMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "StartNetworkAnalyzerStream",
+            "action": "GetMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPositionEstimate": {
+        "ListNetworkAnalyzerConfigurations": {
             "access_level": "Undocumented",
-            "action": "GetPositionEstimate",
+            "action": "ListNetworkAnalyzerConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGatewayTaskDefinition": {
+        "CreateFuotaTask": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGatewayTaskDefinition",
+            "action": "CreateFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServiceProfile": {
+        "DeleteFuotaTask": {
             "access_level": "Undocumented",
-            "action": "GetServiceProfile",
+            "action": "DeleteFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePartnerAccount": {
+        "ListWirelessGatewayTaskDefinitions": {
             "access_level": "Undocumented",
-            "action": "UpdatePartnerAccount",
+            "action": "ListWirelessGatewayTaskDefinitions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetFuotaTask": {
+        "GetWirelessDeviceStatistics": {
             "access_level": "Undocumented",
-            "action": "GetFuotaTask",
+            "action": "GetWirelessDeviceStatistics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelMulticastGroupSession": {
+        "DeleteWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "CancelMulticastGroupSession",
+            "action": "DeleteWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendDataToWirelessDevice": {
+        "GetWirelessGatewayStatistics": {
             "access_level": "Undocumented",
-            "action": "SendDataToWirelessDevice",
+            "action": "GetWirelessGatewayStatistics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteFuotaTask": {
+        "UpdateResourceEventConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteFuotaTask",
+            "action": "UpdateResourceEventConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteNetworkAnalyzerConfiguration": {
+        "AssociateAwsAccountWithPartnerAccount": {
             "access_level": "Undocumented",
-            "action": "DeleteNetworkAnalyzerConfiguration",
+            "action": "AssociateAwsAccountWithPartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGatewayTask": {
+        "UpdateNetworkAnalyzerConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGatewayTask",
+            "action": "UpdateNetworkAnalyzerConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessGateways": {
+        "SendDataToWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "ListWirelessGateways",
+            "action": "SendDataToWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGatewayTaskDefinition": {
+        "GetPosition": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGatewayTaskDefinition",
+            "action": "GetPosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMetricConfiguration": {
+        "ListDevicesForWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "UpdateMetricConfiguration",
+            "action": "ListDevicesForWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetAllResourceLogLevels": {
+        "ListMulticastGroupsByFuotaTask": {
             "access_level": "Undocumented",
-            "action": "ResetAllResourceLogLevels",
+            "action": "ListMulticastGroupsByFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendDataToMulticastGroup": {
+        "GetResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "SendDataToMulticastGroup",
+            "action": "GetResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessGatewayWithCertificate": {
+        "UpdateDestination": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessGatewayWithCertificate",
+            "action": "UpdateDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListFuotaTasks": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListFuotaTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessDevice": {
+        "StartWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessDevice",
+            "action": "StartWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetricConfiguration": {
+        "CreateMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetMetricConfiguration",
+            "action": "CreateMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMetrics": {
+        "SendDataToMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetMetrics",
+            "action": "SendDataToMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWirelessGateway": {
+        "CreateWirelessGatewayTaskDefinition": {
             "access_level": "Undocumented",
-            "action": "GetWirelessGateway",
+            "action": "CreateWirelessGatewayTaskDefinition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessGateway": {
+        "ResetAllResourceLogLevels": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessGateway",
+            "action": "ResetAllResourceLogLevels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWirelessGateway": {
+        "ListMulticastGroups": {
             "access_level": "Undocumented",
-            "action": "UpdateWirelessGateway",
+            "action": "ListMulticastGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteDestination": {
             "access_level": "Undocumented",
             "action": "DeleteDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQueuedMessages": {
+        "CreateWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "DeleteQueuedMessages",
+            "action": "CreateWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateFuotaTask": {
+        "DeleteDeviceProfile": {
             "access_level": "Undocumented",
-            "action": "CreateFuotaTask",
+            "action": "DeleteDeviceProfile",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceProfile": {
+        "StartSingleWirelessDeviceImportTask": {
             "access_level": "Undocumented",
-            "action": "GetDeviceProfile",
+            "action": "StartSingleWirelessDeviceImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGatewayTask": {
+        "UpdateWirelessGateway": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGatewayTask",
+            "action": "UpdateWirelessGateway",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessDeviceFromMulticastGroup": {
+        "ListQueuedMessages": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessDeviceFromMulticastGroup",
+            "action": "ListQueuedMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMulticastGroupSession": {
+        "ListWirelessGateways": {
             "access_level": "Undocumented",
-            "action": "GetMulticastGroupSession",
+            "action": "ListWirelessGateways",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateMulticastGroupFromFuotaTask": {
+        "UpdatePartnerAccount": {
             "access_level": "Undocumented",
-            "action": "DisassociateMulticastGroupFromFuotaTask",
+            "action": "UpdatePartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDestination": {
+        "PutResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "UpdateDestination",
+            "action": "PutResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceEventConfiguration": {
+        "StartBulkDisassociateWirelessDeviceFromMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetResourceEventConfiguration",
+            "action": "StartBulkDisassociateWirelessDeviceFromMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateAwsAccountFromPartnerAccount": {
+        "GetMetrics": {
             "access_level": "Undocumented",
-            "action": "DisassociateAwsAccountFromPartnerAccount",
+            "action": "GetMetrics",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateNetworkAnalyzerConfiguration": {
+        "GetServiceEndpoint": {
             "access_level": "Undocumented",
-            "action": "UpdateNetworkAnalyzerConfiguration",
+            "action": "GetServiceEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListServiceProfiles": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListServiceProfiles",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteMulticastGroup": {
+        "GetEventConfigurationByResourceTypes": {
             "access_level": "Undocumented",
-            "action": "DeleteMulticastGroup",
+            "action": "GetEventConfigurationByResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWirelessDevices": {
+        "AssociateWirelessGatewayWithCertificate": {
             "access_level": "Undocumented",
-            "action": "ListWirelessDevices",
+            "action": "AssociateWirelessGatewayWithCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListDestinations": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListDestinations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterWirelessDevice": {
+        "GetPositionEstimate": {
             "access_level": "Undocumented",
-            "action": "DeregisterWirelessDevice",
+            "action": "GetPositionEstimate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMulticastGroup": {
+        "GetWirelessGatewayTask": {
             "access_level": "Undocumented",
-            "action": "CreateMulticastGroup",
+            "action": "GetWirelessGatewayTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartBulkAssociateWirelessDeviceWithMulticastGroup": {
+        "StartFuotaTask": {
             "access_level": "Undocumented",
-            "action": "StartBulkAssociateWirelessDeviceWithMulticastGroup",
+            "action": "StartFuotaTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWirelessDevice": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteWirelessDevice",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePosition": {
+        "UpdateMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "GetResourcePosition",
+            "action": "UpdateMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateWirelessGatewayFromThing": {
+        "GetDestination": {
             "access_level": "Undocumented",
-            "action": "DisassociateWirelessGatewayFromThing",
+            "action": "GetDestination",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPartnerAccount": {
+        "StartMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "GetPartnerAccount",
+            "action": "StartMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartWirelessDeviceImportTask": {
+        "AssociateWirelessDeviceWithMulticastGroup": {
             "access_level": "Undocumented",
-            "action": "StartWirelessDeviceImportTask",
+            "action": "AssociateWirelessDeviceWithMulticastGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateMulticastGroupWithFuotaTask": {
+        "UpdatePosition": {
             "access_level": "Undocumented",
-            "action": "AssociateMulticastGroupWithFuotaTask",
+            "action": "UpdatePosition",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutResourceLogLevel": {
+        "ListPartnerAccounts": {
             "access_level": "Undocumented",
-            "action": "PutResourceLogLevel",
+            "action": "ListPartnerAccounts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWirelessGateway": {
+        "ResetResourceLogLevel": {
             "access_level": "Undocumented",
-            "action": "CreateWirelessGateway",
+            "action": "ResetResourceLogLevel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateFuotaTask": {
+        "CancelMulticastGroupSession": {
             "access_level": "Undocumented",
-            "action": "UpdateFuotaTask",
+            "action": "CancelMulticastGroupSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateWirelessGatewayWithThing": {
+        "UpdateWirelessDevice": {
             "access_level": "Undocumented",
-            "action": "AssociateWirelessGatewayWithThing",
+            "action": "UpdateWirelessDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "iq": {
@@ -94687,38 +94687,46 @@
             "resources": [
                 "index",
                 "thesaurus"
             ]
         }
     },
     "kendra-ranking": {
-        "UntagResource": {
+        "Rescore": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "Rescore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Rescore": {
+        "DeleteRescoreExecutionPlan": {
             "access_level": "Undocumented",
-            "action": "Rescore",
+            "action": "DeleteRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateRescoreExecutionPlan": {
             "access_level": "Undocumented",
             "action": "UpdateRescoreExecutionPlan",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
+        "CreateRescoreExecutionPlan": {
+            "access_level": "Undocumented",
+            "action": "CreateRescoreExecutionPlan",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListTagsForResource": {
             "access_level": "Undocumented",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
@@ -94727,17 +94735,17 @@
             "access_level": "Undocumented",
             "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRescoreExecutionPlan": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateRescoreExecutionPlan",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeRescoreExecutionPlan": {
             "access_level": "Undocumented",
@@ -94750,276 +94758,268 @@
         "ListRescoreExecutionPlans": {
             "access_level": "Undocumented",
             "action": "ListRescoreExecutionPlans",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
-        },
-        "DeleteRescoreExecutionPlan": {
+        }
+    },
+    "kinesis": {
+        "RegisterStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "DeleteRescoreExecutionPlan",
+            "action": "RegisterStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
-        }
-    },
-    "kinesis": {
-        "SubscribeToShard": {
+        },
+        "SplitShard": {
             "access_level": "Undocumented",
-            "action": "SubscribeToShard",
+            "action": "SplitShard",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStreams": {
+        "GetRecords": {
             "access_level": "Undocumented",
-            "action": "ListStreams",
+            "action": "GetRecords",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DisableEnhancedMonitoring": {
             "access_level": "Undocumented",
             "action": "DisableEnhancedMonitoring",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteStream": {
+        "MergeShards": {
             "access_level": "Undocumented",
-            "action": "DeleteStream",
+            "action": "MergeShards",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStream": {
+        "PutResourcePolicy": {
             "access_level": "Undocumented",
-            "action": "DescribeStream",
+            "action": "PutResourcePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListStreamConsumers": {
+        "UpdateStreamMode": {
             "access_level": "Undocumented",
-            "action": "ListStreamConsumers",
+            "action": "UpdateStreamMode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeLimits": {
             "access_level": "Undocumented",
             "action": "DescribeLimits",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterStreamConsumer": {
+        "DeleteStream": {
             "access_level": "Undocumented",
-            "action": "DeregisterStreamConsumer",
+            "action": "DeleteStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetShardIterator": {
+        "DescribeStreamSummary": {
             "access_level": "Undocumented",
-            "action": "GetShardIterator",
+            "action": "DescribeStreamSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IncreaseStreamRetentionPeriod": {
+        "DecreaseStreamRetentionPeriod": {
             "access_level": "Undocumented",
-            "action": "IncreaseStreamRetentionPeriod",
+            "action": "DecreaseStreamRetentionPeriod",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableEnhancedMonitoring": {
+        "ListTagsForStream": {
             "access_level": "Undocumented",
-            "action": "EnableEnhancedMonitoring",
+            "action": "ListTagsForStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRecord": {
+        "UpdateShardCount": {
             "access_level": "Undocumented",
-            "action": "PutRecord",
+            "action": "UpdateShardCount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterStreamConsumer": {
+        "GetShardIterator": {
             "access_level": "Undocumented",
-            "action": "RegisterStreamConsumer",
+            "action": "GetShardIterator",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "MergeShards": {
+        "IncreaseStreamRetentionPeriod": {
             "access_level": "Undocumented",
-            "action": "MergeShards",
+            "action": "IncreaseStreamRetentionPeriod",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateShardCount": {
+        "ListShards": {
             "access_level": "Undocumented",
-            "action": "UpdateShardCount",
+            "action": "ListShards",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRecords": {
+        "AddTagsToStream": {
             "access_level": "Undocumented",
-            "action": "GetRecords",
+            "action": "AddTagsToStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutResourcePolicy": {
+        "DescribeStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "PutResourcePolicy",
+            "action": "DescribeStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveTagsFromStream": {
+        "SubscribeToShard": {
             "access_level": "Undocumented",
-            "action": "RemoveTagsFromStream",
+            "action": "SubscribeToShard",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddTagsToStream": {
+        "ListStreams": {
             "access_level": "Undocumented",
-            "action": "AddTagsToStream",
+            "action": "ListStreams",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateStreamMode": {
+        "StopStreamEncryption": {
             "access_level": "Undocumented",
-            "action": "UpdateStreamMode",
+            "action": "StopStreamEncryption",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePolicy": {
+        "StartStreamEncryption": {
             "access_level": "Undocumented",
-            "action": "GetResourcePolicy",
+            "action": "StartStreamEncryption",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SplitShard": {
+        "DescribeStream": {
             "access_level": "Undocumented",
-            "action": "SplitShard",
+            "action": "DescribeStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopStreamEncryption": {
+        "PutRecords": {
             "access_level": "Undocumented",
-            "action": "StopStreamEncryption",
+            "action": "PutRecords",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DecreaseStreamRetentionPeriod": {
+        "CreateStream": {
             "access_level": "Undocumented",
-            "action": "DecreaseStreamRetentionPeriod",
+            "action": "CreateStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForStream": {
+        "GetResourcePolicy": {
             "access_level": "Undocumented",
-            "action": "ListTagsForStream",
+            "action": "GetResourcePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListShards": {
+        "PutRecord": {
             "access_level": "Undocumented",
-            "action": "ListShards",
+            "action": "PutRecord",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStreamConsumer": {
+        "DeregisterStreamConsumer": {
             "access_level": "Undocumented",
-            "action": "DescribeStreamConsumer",
+            "action": "DeregisterStreamConsumer",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutRecords": {
+        "RemoveTagsFromStream": {
             "access_level": "Undocumented",
-            "action": "PutRecords",
+            "action": "RemoveTagsFromStream",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteResourcePolicy": {
             "access_level": "Undocumented",
             "action": "DeleteResourcePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateStream": {
-            "access_level": "Undocumented",
-            "action": "CreateStream",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "StartStreamEncryption": {
+        "ListStreamConsumers": {
             "access_level": "Undocumented",
-            "action": "StartStreamEncryption",
+            "action": "ListStreamConsumers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeStreamSummary": {
+        "EnableEnhancedMonitoring": {
             "access_level": "Undocumented",
-            "action": "DescribeStreamSummary",
+            "action": "EnableEnhancedMonitoring",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "kinesisanalytics": {
@@ -97678,273 +97678,273 @@
             "orphan": false,
             "resources": [
                 "function"
             ]
         }
     },
     "launchwizard": {
-        "DeleteApp": {
+        "ListWorkloadDeploymentOptions": {
             "access_level": "Undocumented",
-            "action": "DeleteApp",
+            "action": "ListWorkloadDeploymentOptions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetInfrastructureSuggestion": {
+        "GetIpAddress": {
             "access_level": "Undocumented",
-            "action": "GetInfrastructureSuggestion",
+            "action": "GetIpAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAllowedResources": {
+        "ListDeployments": {
             "access_level": "Undocumented",
-            "action": "ListAllowedResources",
+            "action": "ListDeployments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIpAddress": {
+        "ListWorkloadDeploymentPatterns": {
             "access_level": "Undocumented",
-            "action": "GetIpAddress",
+            "action": "ListWorkloadDeploymentPatterns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateDeployment": {
             "access_level": "Undocumented",
             "action": "CreateDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSettingsSet": {
+        "ListDeploymentEvents": {
             "access_level": "Undocumented",
-            "action": "PutSettingsSet",
+            "action": "ListDeploymentEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListProvisionedApps": {
+        "UpdateSettingsSet": {
             "access_level": "Undocumented",
-            "action": "ListProvisionedApps",
+            "action": "UpdateSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSettingsSet": {
+        "DescribeProvisionedApp": {
             "access_level": "Undocumented",
-            "action": "CreateSettingsSet",
+            "action": "DescribeProvisionedApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkloadAssets": {
+        "GetInfrastructureSuggestion": {
             "access_level": "Undocumented",
-            "action": "GetWorkloadAssets",
+            "action": "GetInfrastructureSuggestion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkloadAsset": {
+        "DescribeProvisioningEvents": {
             "access_level": "Undocumented",
-            "action": "GetWorkloadAsset",
+            "action": "DescribeProvisioningEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeployments": {
+        "DescribeAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "ListDeployments",
+            "action": "DescribeAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeProvisioningEvents": {
+        "ListWorkloads": {
             "access_level": "Undocumented",
-            "action": "DescribeProvisioningEvents",
+            "action": "ListWorkloads",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceCostEstimate": {
+        "ListSettingsSets": {
             "access_level": "Undocumented",
-            "action": "GetResourceCostEstimate",
+            "action": "ListSettingsSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeploymentEvents": {
+        "ListProvisionedApps": {
             "access_level": "Undocumented",
-            "action": "ListDeploymentEvents",
+            "action": "ListProvisionedApps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSettingsSet": {
+        "GetDeployment": {
             "access_level": "Undocumented",
-            "action": "UpdateSettingsSet",
+            "action": "GetDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkload": {
+        "GetSettingsSet": {
             "access_level": "Undocumented",
-            "action": "GetWorkload",
+            "action": "GetSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeSettingsSet": {
+        "CreateSettingsSet": {
             "access_level": "Undocumented",
-            "action": "DescribeSettingsSet",
+            "action": "CreateSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAdditionalNodes": {
+        "DeleteApp": {
             "access_level": "Undocumented",
-            "action": "ListAdditionalNodes",
+            "action": "DeleteApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSettingsSets": {
+        "DeleteDeployment": {
             "access_level": "Undocumented",
-            "action": "ListSettingsSets",
+            "action": "DeleteDeployment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDeployment": {
+        "GetResourceCostEstimate": {
             "access_level": "Undocumented",
-            "action": "DeleteDeployment",
+            "action": "GetResourceCostEstimate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartProvisioning": {
+        "GetWorkloadAssets": {
             "access_level": "Undocumented",
-            "action": "StartProvisioning",
+            "action": "GetWorkloadAssets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSettingsSet": {
+        "DeleteSettingsSet": {
             "access_level": "Undocumented",
-            "action": "GetSettingsSet",
+            "action": "DeleteSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceRecommendation": {
+        "DeleteAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "GetResourceRecommendation",
+            "action": "DeleteAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloadDeploymentOptions": {
+        "GetWorkload": {
             "access_level": "Undocumented",
-            "action": "ListWorkloadDeploymentOptions",
+            "action": "GetWorkload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloadDeploymentPatterns": {
+        "PutSettingsSet": {
             "access_level": "Undocumented",
-            "action": "ListWorkloadDeploymentPatterns",
+            "action": "PutSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAdditionalNode": {
+        "GetResourceRecommendation": {
             "access_level": "Undocumented",
-            "action": "DeleteAdditionalNode",
+            "action": "GetResourceRecommendation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSettingsSet": {
+        "StartProvisioning": {
             "access_level": "Undocumented",
-            "action": "DeleteSettingsSet",
+            "action": "StartProvisioning",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAdditionalNode": {
+        "ListAllowedResources": {
             "access_level": "Undocumented",
-            "action": "DescribeAdditionalNode",
+            "action": "ListAllowedResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkloads": {
+        "GetWorkloadAsset": {
             "access_level": "Undocumented",
-            "action": "ListWorkloads",
+            "action": "GetWorkloadAsset",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceCostEstimates": {
+        "CreateAdditionalNode": {
             "access_level": "Undocumented",
-            "action": "ListResourceCostEstimates",
+            "action": "CreateAdditionalNode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeployment": {
+        "ListResourceCostEstimates": {
             "access_level": "Undocumented",
-            "action": "GetDeployment",
+            "action": "ListResourceCostEstimates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeProvisionedApp": {
+        "DescribeSettingsSet": {
             "access_level": "Undocumented",
-            "action": "DescribeProvisionedApp",
+            "action": "DescribeSettingsSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAdditionalNode": {
+        "ListAdditionalNodes": {
             "access_level": "Undocumented",
-            "action": "CreateAdditionalNode",
+            "action": "ListAdditionalNodes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "lex": {
@@ -105159,99 +105159,99 @@
             "orphan": false,
             "resources": [
                 "proposal"
             ]
         }
     },
     "managedblockchain-query": {
-        "ListTransactions": {
+        "ListFilteredTransactionEvents": {
             "access_level": "Undocumented",
-            "action": "ListTransactions",
+            "action": "ListFilteredTransactionEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTransactionEvents": {
+        "ListTokenBalances": {
             "access_level": "Undocumented",
-            "action": "ListTransactionEvents",
+            "action": "ListTokenBalances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssetContracts": {
+        "GetTransaction": {
             "access_level": "Undocumented",
-            "action": "ListAssetContracts",
+            "action": "GetTransaction",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTransaction": {
+        "BatchGetTokenBalance": {
             "access_level": "Undocumented",
-            "action": "GetTransaction",
+            "action": "BatchGetTokenBalance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchGetTokenBalance": {
+        "GetAssetContract": {
             "access_level": "Undocumented",
-            "action": "BatchGetTokenBalance",
+            "action": "GetAssetContract",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListFilteredTransactionEvents": {
+        "ListAssetContracts": {
             "access_level": "Undocumented",
-            "action": "ListFilteredTransactionEvents",
+            "action": "ListAssetContracts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTokenBalances": {
+        "ListTransactionEvents": {
             "access_level": "Undocumented",
-            "action": "ListTokenBalances",
+            "action": "ListTransactionEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetTokenBalance": {
             "access_level": "Undocumented",
             "action": "GetTokenBalance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAssetContract": {
+        "ListTransactions": {
             "access_level": "Undocumented",
-            "action": "GetAssetContract",
+            "action": "ListTransactions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "mapcredits": {
-        "ListQuarterSpend": {
+        "ListAssociatedPrograms": {
             "access_level": "Undocumented",
-            "action": "ListQuarterSpend",
+            "action": "ListAssociatedPrograms",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssociatedPrograms": {
+        "ListQuarterSpend": {
             "access_level": "Undocumented",
-            "action": "ListAssociatedPrograms",
+            "action": "ListQuarterSpend",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListQuarterCredits": {
             "access_level": "Undocumented",
@@ -107703,225 +107703,225 @@
             "orphan": false,
             "resources": [
                 "packaging-groups"
             ]
         }
     },
     "mediapackagev2": {
-        "CreateChannelGroup": {
+        "UpdateChannel": {
             "access_level": "Undocumented",
-            "action": "CreateChannelGroup",
+            "action": "UpdateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetHeadObject": {
+        "DeleteChannelGroup": {
             "access_level": "Undocumented",
-            "action": "GetHeadObject",
+            "action": "DeleteChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannelGroups": {
+        "ListOriginEndpoints": {
             "access_level": "Undocumented",
-            "action": "ListChannelGroups",
+            "action": "ListOriginEndpoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannelGroup": {
+        "GetChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "GetChannelGroup",
+            "action": "GetChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannels": {
+        "DeleteChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "ListChannels",
+            "action": "DeleteChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateChannel": {
+        "GetHeadObject": {
             "access_level": "Undocumented",
-            "action": "CreateChannel",
+            "action": "GetHeadObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOriginEndpoint": {
+        "GetChannel": {
             "access_level": "Undocumented",
-            "action": "GetOriginEndpoint",
+            "action": "GetChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannel": {
+        "DeleteChannel": {
             "access_level": "Undocumented",
-            "action": "GetChannel",
+            "action": "DeleteChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetObject": {
+        "GetOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "GetObject",
+            "action": "GetOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutOriginEndpointPolicy": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "PutOriginEndpointPolicy",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutChannelPolicy": {
+        "CreateOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "PutChannelPolicy",
+            "action": "CreateOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateChannelGroup": {
+        "PutObject": {
             "access_level": "Undocumented",
-            "action": "UpdateChannelGroup",
+            "action": "PutObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateOriginEndpoint": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateOriginEndpoint",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetOriginEndpointPolicy": {
+        "CreateChannel": {
             "access_level": "Undocumented",
-            "action": "GetOriginEndpointPolicy",
+            "action": "CreateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateChannel": {
+        "PutOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateChannel",
+            "action": "PutOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "CreateChannelGroup": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreateChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannelGroup": {
+        "ListChannelGroups": {
             "access_level": "Undocumented",
-            "action": "DeleteChannelGroup",
+            "action": "ListChannelGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChannelPolicy": {
+        "UpdateChannelGroup": {
             "access_level": "Undocumented",
-            "action": "GetChannelPolicy",
+            "action": "UpdateChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListOriginEndpoints": {
+        "GetOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "ListOriginEndpoints",
+            "action": "GetOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListChannels": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListChannels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOriginEndpoint": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteOriginEndpoint",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteOriginEndpointPolicy": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteOriginEndpointPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteOriginEndpointPolicy": {
+        "UpdateOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "DeleteOriginEndpointPolicy",
+            "action": "UpdateOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutObject": {
+        "DeleteOriginEndpoint": {
             "access_level": "Undocumented",
-            "action": "PutObject",
+            "action": "DeleteOriginEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateOriginEndpoint": {
+        "GetObject": {
             "access_level": "Undocumented",
-            "action": "CreateOriginEndpoint",
+            "action": "GetObject",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannel": {
+        "GetChannelGroup": {
             "access_level": "Undocumented",
-            "action": "DeleteChannel",
+            "action": "GetChannelGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChannelPolicy": {
+        "PutChannelPolicy": {
             "access_level": "Undocumented",
-            "action": "DeleteChannelPolicy",
+            "action": "PutChannelPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "mediastore": {
@@ -108639,153 +108639,153 @@
             "orphan": false,
             "resources": [
                 "vodSource"
             ]
         }
     },
     "medical-imaging": {
-        "StartDICOMImportJob": {
+        "GetDatastore": {
             "access_level": "Undocumented",
-            "action": "StartDICOMImportJob",
+            "action": "GetDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListImageSetVersions": {
+        "DeleteImageSet": {
             "access_level": "Undocumented",
-            "action": "ListImageSetVersions",
+            "action": "DeleteImageSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetImageSetMetadata": {
+        "CopyImageSet": {
             "access_level": "Undocumented",
-            "action": "GetImageSetMetadata",
+            "action": "CopyImageSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDICOMImportJobs": {
+        "GetImageSetMetadata": {
             "access_level": "Undocumented",
-            "action": "ListDICOMImportJobs",
+            "action": "GetImageSetMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDatastore": {
+        "GetDICOMImportJob": {
             "access_level": "Undocumented",
-            "action": "GetDatastore",
+            "action": "GetDICOMImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteImageSet": {
+        "GetImageFrame": {
             "access_level": "Undocumented",
-            "action": "DeleteImageSet",
+            "action": "GetImageFrame",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchImageSets": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "SearchImageSets",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetImageSet": {
+        "UpdateImageSetMetadata": {
             "access_level": "Undocumented",
-            "action": "GetImageSet",
+            "action": "UpdateImageSetMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDatastore": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteDatastore",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CopyImageSet": {
+        "ListDICOMImportJobs": {
             "access_level": "Undocumented",
-            "action": "CopyImageSet",
+            "action": "ListDICOMImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateImageSetMetadata": {
+        "StartDICOMImportJob": {
             "access_level": "Undocumented",
-            "action": "UpdateImageSetMetadata",
+            "action": "StartDICOMImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDatastores": {
+        "ListImageSetVersions": {
             "access_level": "Undocumented",
-            "action": "ListDatastores",
+            "action": "ListImageSetVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreateDatastore": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreateDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "SearchImageSets": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "SearchImageSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDICOMImportJob": {
+        "DeleteDatastore": {
             "access_level": "Undocumented",
-            "action": "GetDICOMImportJob",
+            "action": "DeleteDatastore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetImageFrame": {
+        "ListDatastores": {
             "access_level": "Undocumented",
-            "action": "GetImageFrame",
+            "action": "ListDatastores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDatastore": {
+        "GetImageSet": {
             "access_level": "Undocumented",
-            "action": "CreateDatastore",
+            "action": "GetImageSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "memorydb": {
@@ -113201,265 +113201,265 @@
             "orphan": false,
             "resources": [
                 "database"
             ]
         }
     },
     "neptune-graph": {
-        "GetGraph": {
+        "GetGraphSnapshot": {
             "access_level": "Undocumented",
-            "action": "GetGraph",
+            "action": "GetGraphSnapshot",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelImportTask": {
+        "GetPrivateGraphEndpoint": {
             "access_level": "Undocumented",
-            "action": "CancelImportTask",
+            "action": "GetPrivateGraphEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQueries": {
+        "CreateGraphSnapshot": {
             "access_level": "Undocumented",
-            "action": "ListQueries",
+            "action": "CreateGraphSnapshot",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResetGraph": {
+        "ListGraphSnapshots": {
             "access_level": "Undocumented",
-            "action": "ResetGraph",
+            "action": "ListGraphSnapshots",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataViaQuery": {
+        "GetGraphSummary": {
             "access_level": "Undocumented",
-            "action": "DeleteDataViaQuery",
+            "action": "GetGraphSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGraphSnapshot": {
+        "CreateGraphUsingImportTask": {
             "access_level": "Undocumented",
-            "action": "GetGraphSnapshot",
+            "action": "CreateGraphUsingImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RestoreGraphFromSnapshot": {
+        "CancelImportTask": {
             "access_level": "Undocumented",
-            "action": "RestoreGraphFromSnapshot",
+            "action": "CancelImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGraphSummary": {
+        "GetStatisticsStatus": {
             "access_level": "Undocumented",
-            "action": "GetGraphSummary",
+            "action": "GetStatisticsStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGraphSnapshot": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteGraphSnapshot",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteDataViaQuery": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteDataViaQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteGraphSnapshot": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteGraphSnapshot",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelQuery": {
+        "ListQueries": {
             "access_level": "Undocumented",
-            "action": "CancelQuery",
+            "action": "ListQueries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGraph": {
+        "StartImportTask": {
             "access_level": "Undocumented",
-            "action": "DeleteGraph",
+            "action": "StartImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePrivateGraphEndpoint": {
+        "ListGraphs": {
             "access_level": "Undocumented",
-            "action": "CreatePrivateGraphEndpoint",
+            "action": "ListGraphs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePrivateGraphEndpoint": {
+        "ResetGraph": {
             "access_level": "Undocumented",
-            "action": "DeletePrivateGraphEndpoint",
+            "action": "ResetGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPrivateGraphEndpoint": {
+        "CreateGraph": {
             "access_level": "Undocumented",
-            "action": "GetPrivateGraphEndpoint",
+            "action": "CreateGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartImportTask": {
+        "ListPrivateGraphEndpoints": {
             "access_level": "Undocumented",
-            "action": "StartImportTask",
+            "action": "ListPrivateGraphEndpoints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEngineStatus": {
+        "GetImportTask": {
             "access_level": "Undocumented",
-            "action": "GetEngineStatus",
+            "action": "GetImportTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "WriteDataViaQuery": {
+        "CreatePrivateGraphEndpoint": {
             "access_level": "Undocumented",
-            "action": "WriteDataViaQuery",
+            "action": "CreatePrivateGraphEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetStatisticsStatus": {
+        "GetQueryStatus": {
             "access_level": "Undocumented",
-            "action": "GetStatisticsStatus",
+            "action": "GetQueryStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGraph": {
+        "CancelQuery": {
             "access_level": "Undocumented",
-            "action": "CreateGraph",
+            "action": "CancelQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGraphSnapshots": {
+        "GetEngineStatus": {
             "access_level": "Undocumented",
-            "action": "ListGraphSnapshots",
+            "action": "GetEngineStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGraphUsingImportTask": {
+        "DeleteGraph": {
             "access_level": "Undocumented",
-            "action": "CreateGraphUsingImportTask",
+            "action": "DeleteGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReadDataViaQuery": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ReadDataViaQuery",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListImportTasks": {
+        "ReadDataViaQuery": {
             "access_level": "Undocumented",
-            "action": "ListImportTasks",
+            "action": "ReadDataViaQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "RestoreGraphFromSnapshot": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "RestoreGraphFromSnapshot",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateGraphSnapshot": {
+        "WriteDataViaQuery": {
             "access_level": "Undocumented",
-            "action": "CreateGraphSnapshot",
+            "action": "WriteDataViaQuery",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateGraph": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UpdateGraph",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetImportTask": {
+        "GetGraph": {
             "access_level": "Undocumented",
-            "action": "GetImportTask",
+            "action": "GetGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGraphs": {
+        "ListImportTasks": {
             "access_level": "Undocumented",
-            "action": "ListGraphs",
+            "action": "ListImportTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQueryStatus": {
+        "UpdateGraph": {
             "access_level": "Undocumented",
-            "action": "GetQueryStatus",
+            "action": "UpdateGraph",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrivateGraphEndpoints": {
+        "DeletePrivateGraphEndpoint": {
             "access_level": "Undocumented",
-            "action": "ListPrivateGraphEndpoints",
+            "action": "DeletePrivateGraphEndpoint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "network-firewall": {
@@ -114826,163 +114826,163 @@
             "orphan": false,
             "resources": [
                 "attachment"
             ]
         }
     },
     "networkmanager-chat": {
-        "NotifyConversationIsActive": {
+        "ListConversationMessages": {
             "access_level": "Undocumented",
-            "action": "NotifyConversationIsActive",
+            "action": "ListConversationMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendConversationMessage": {
+        "CancelMessageResponse": {
             "access_level": "Undocumented",
-            "action": "SendConversationMessage",
+            "action": "CancelMessageResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelMessageResponse": {
+        "CreateConversation": {
             "access_level": "Undocumented",
-            "action": "CancelMessageResponse",
+            "action": "CreateConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteConversation": {
             "access_level": "Undocumented",
             "action": "DeleteConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConversation": {
+        "ListConversations": {
             "access_level": "Undocumented",
-            "action": "CreateConversation",
+            "action": "ListConversations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConversations": {
+        "NotifyConversationIsActive": {
             "access_level": "Undocumented",
-            "action": "ListConversations",
+            "action": "NotifyConversationIsActive",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConversationMessages": {
+        "SendConversationMessage": {
             "access_level": "Undocumented",
-            "action": "ListConversationMessages",
+            "action": "SendConversationMessage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "networkmonitor": {
-        "CreateMonitor": {
-            "access_level": "Undocumented",
-            "action": "CreateMonitor",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
-            "orphan": false,
-            "resources": []
-        },
-        "UntagResource": {
+        "ListMonitors": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListMonitors",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UpdateProbe": {
             "access_level": "Undocumented",
             "action": "UpdateProbe",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UpdateMonitor": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UpdateMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CreateProbe": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CreateProbe",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteMonitor": {
             "access_level": "Undocumented",
             "action": "DeleteMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateMonitor": {
+        "DeleteProbe": {
             "access_level": "Undocumented",
-            "action": "UpdateMonitor",
+            "action": "DeleteProbe",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetMonitor": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetMonitor",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteProbe": {
+        "CreateMonitor": {
             "access_level": "Undocumented",
-            "action": "DeleteProbe",
+            "action": "CreateMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateProbe": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateProbe",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetProbe": {
             "access_level": "Undocumented",
             "action": "GetProbe",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMonitors": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListMonitors",
+            "action": "UntagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetMonitor": {
+            "access_level": "Undocumented",
+            "action": "GetMonitor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "nimble": {
@@ -115550,145 +115550,145 @@
             "orphan": false,
             "resources": [
                 "studio-component"
             ]
         }
     },
     "notifications": {
-        "RegisterNotificationHub": {
+        "ListEventRules": {
             "access_level": "Undocumented",
-            "action": "RegisterNotificationHub",
+            "action": "ListEventRules",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateNotificationConfiguration": {
+        "AssociateChannel": {
             "access_level": "Undocumented",
-            "action": "UpdateNotificationConfiguration",
+            "action": "AssociateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteNotificationConfiguration": {
+        "DisassociateChannel": {
             "access_level": "Undocumented",
-            "action": "DeleteNotificationConfiguration",
+            "action": "DisassociateChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListChannels": {
+        "RegisterNotificationHub": {
             "access_level": "Undocumented",
-            "action": "ListChannels",
+            "action": "RegisterNotificationHub",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListNotificationHubs": {
             "access_level": "Undocumented",
             "action": "ListNotificationHubs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterNotificationHub": {
+        "DeleteEventRule": {
             "access_level": "Undocumented",
-            "action": "DeregisterNotificationHub",
+            "action": "DeleteEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetNotificationConfiguration": {
+        "GetEventRule": {
             "access_level": "Undocumented",
-            "action": "GetNotificationConfiguration",
+            "action": "GetEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationEvents": {
+        "CreateNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListNotificationEvents",
+            "action": "CreateNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateNotificationConfiguration": {
+        "ListNotificationEvents": {
             "access_level": "Undocumented",
-            "action": "CreateNotificationConfiguration",
+            "action": "ListNotificationEvents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEventRule": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteEventRule",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListNotificationConfigurations": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListNotificationConfigurations",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEventRule": {
+        "GetNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdateEventRule",
+            "action": "GetNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeregisterNotificationHub": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeregisterNotificationHub",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateChannel": {
+        "ListChannels": {
             "access_level": "Undocumented",
-            "action": "DisassociateChannel",
+            "action": "ListChannels",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEventRules": {
+        "ListNotificationConfigurations": {
             "access_level": "Undocumented",
-            "action": "ListEventRules",
+            "action": "ListNotificationConfigurations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTagsForResource": {
             "access_level": "Undocumented",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetNotificationEvent": {
             "access_level": "Undocumented",
@@ -115702,59 +115702,59 @@
             "access_level": "Undocumented",
             "action": "CreateEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEventRule": {
+        "UpdateEventRule": {
             "access_level": "Undocumented",
-            "action": "GetEventRule",
+            "action": "UpdateEventRule",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateChannel": {
+        "UpdateNotificationConfiguration": {
             "access_level": "Undocumented",
-            "action": "AssociateChannel",
+            "action": "UpdateNotificationConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "notifications-contacts": {
-        "UntagResource": {
+        "ListEmailContacts": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListEmailContacts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEmailContacts": {
+        "GetEmailContact": {
             "access_level": "Undocumented",
-            "action": "ListEmailContacts",
+            "action": "GetEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateEmailContact": {
             "access_level": "Undocumented",
             "action": "CreateEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEmailContact": {
+        "SendActivationCode": {
             "access_level": "Undocumented",
-            "action": "GetEmailContact",
+            "action": "SendActivationCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTagsForResource": {
             "access_level": "Undocumented",
@@ -115784,17 +115784,17 @@
             "access_level": "Undocumented",
             "action": "DeleteEmailContact",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SendActivationCode": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "SendActivationCode",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "oam": {
@@ -115972,883 +115972,883 @@
             "orphan": false,
             "resources": [
                 "Link"
             ]
         }
     },
     "omics": {
-        "ListReferences": {
+        "UpdateRunGroup": {
             "access_level": "Undocumented",
-            "action": "ListReferences",
+            "action": "UpdateRunGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateReferenceStore": {
+        "ListReferenceStores": {
             "access_level": "Undocumented",
-            "action": "CreateReferenceStore",
+            "action": "ListReferenceStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelAnnotationImportJob": {
+        "ListWorkflows": {
             "access_level": "Undocumented",
-            "action": "CancelAnnotationImportJob",
+            "action": "ListWorkflows",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSetActivationJob": {
+        "ListVariantStores": {
             "access_level": "Undocumented",
-            "action": "GetReadSetActivationJob",
+            "action": "ListVariantStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteReferenceStore": {
+        "ListRunGroups": {
             "access_level": "Undocumented",
-            "action": "DeleteReferenceStore",
+            "action": "ListRunGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptShare": {
+        "GetAnnotationStoreVersion": {
             "access_level": "Undocumented",
-            "action": "AcceptShare",
+            "action": "GetAnnotationStoreVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRun": {
+        "GetReadSetMetadata": {
             "access_level": "Undocumented",
-            "action": "DeleteRun",
+            "action": "GetReadSetMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSequenceStores": {
+        "CreateAnnotationStore": {
             "access_level": "Undocumented",
-            "action": "ListSequenceStores",
+            "action": "CreateAnnotationStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartVariantImportJob": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "StartVariantImportJob",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListVariantImportJobs": {
+        "CreateVariantStore": {
             "access_level": "Undocumented",
-            "action": "ListVariantImportJobs",
+            "action": "CreateVariantStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteReference": {
+        "GetReadSet": {
             "access_level": "Undocumented",
-            "action": "DeleteReference",
+            "action": "GetReadSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetReference": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetReference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelVariantImportJob": {
+        "GetAnnotationStore": {
             "access_level": "Undocumented",
-            "action": "CancelVariantImportJob",
+            "action": "GetAnnotationStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListWorkflows": {
+        "GetRunTask": {
             "access_level": "Undocumented",
-            "action": "ListWorkflows",
+            "action": "GetRunTask",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateShare": {
+        "GetReferenceMetadata": {
             "access_level": "Undocumented",
-            "action": "CreateShare",
+            "action": "GetReferenceMetadata",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateMultipartReadSetUpload": {
+        "DeleteReferenceStore": {
             "access_level": "Undocumented",
-            "action": "CreateMultipartReadSetUpload",
+            "action": "DeleteReferenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReference": {
+        "ListReadSetImportJobs": {
             "access_level": "Undocumented",
-            "action": "GetReference",
+            "action": "ListReadSetImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSetMetadata": {
+        "ListReadSets": {
             "access_level": "Undocumented",
-            "action": "GetReadSetMetadata",
+            "action": "ListReadSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetVariantStore": {
+        "ListAnnotationStores": {
             "access_level": "Undocumented",
-            "action": "GetVariantStore",
+            "action": "ListAnnotationStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateVariantStore": {
+        "ListAnnotationStoreVersions": {
             "access_level": "Undocumented",
-            "action": "CreateVariantStore",
+            "action": "ListAnnotationStoreVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAnnotationStore": {
+        "DeleteRunGroup": {
             "access_level": "Undocumented",
-            "action": "GetAnnotationStore",
+            "action": "DeleteRunGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteShare": {
+        "DeleteVariantStore": {
             "access_level": "Undocumented",
-            "action": "DeleteShare",
+            "action": "DeleteVariantStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRunGroup": {
+        "CreateMultipartReadSetUpload": {
             "access_level": "Undocumented",
-            "action": "CreateRunGroup",
+            "action": "CreateMultipartReadSetUpload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAnnotationStoreVersion": {
+        "StartReadSetActivationJob": {
             "access_level": "Undocumented",
-            "action": "UpdateAnnotationStoreVersion",
+            "action": "StartReadSetActivationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartReadSetActivationJob": {
+        "ListMultipartReadSetUploads": {
             "access_level": "Undocumented",
-            "action": "StartReadSetActivationJob",
+            "action": "ListMultipartReadSetUploads",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSequenceStore": {
+        "GetReadSetActivationJob": {
             "access_level": "Undocumented",
-            "action": "CreateSequenceStore",
+            "action": "GetReadSetActivationJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSetActivationJobs": {
+        "StartReadSetImportJob": {
             "access_level": "Undocumented",
-            "action": "ListReadSetActivationJobs",
+            "action": "StartReadSetImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAnnotationStores": {
+        "UpdateWorkflow": {
             "access_level": "Undocumented",
-            "action": "ListAnnotationStores",
+            "action": "UpdateWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetVariantImportJob": {
+        "GetRun": {
             "access_level": "Undocumented",
-            "action": "GetVariantImportJob",
+            "action": "GetRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSetImportJob": {
+        "AcceptShare": {
             "access_level": "Undocumented",
-            "action": "GetReadSetImportJob",
+            "action": "AcceptShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAnnotationStoreVersion": {
+        "CompleteMultipartReadSetUpload": {
             "access_level": "Undocumented",
-            "action": "CreateAnnotationStoreVersion",
+            "action": "CompleteMultipartReadSetUpload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReferenceImportJobs": {
+        "DeleteAnnotationStoreVersions": {
             "access_level": "Undocumented",
-            "action": "ListReferenceImportJobs",
+            "action": "DeleteAnnotationStoreVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchDeleteReadSet": {
+        "GetReadSetExportJob": {
             "access_level": "Undocumented",
-            "action": "BatchDeleteReadSet",
+            "action": "GetReadSetExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRunGroups": {
+        "GetReadSetImportJob": {
             "access_level": "Undocumented",
-            "action": "ListRunGroups",
+            "action": "GetReadSetImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CompleteMultipartReadSetUpload": {
+        "UpdateAnnotationStoreVersion": {
             "access_level": "Undocumented",
-            "action": "CompleteMultipartReadSetUpload",
+            "action": "UpdateAnnotationStoreVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetShare": {
+        "GetReferenceStore": {
             "access_level": "Undocumented",
-            "action": "GetShare",
+            "action": "GetReferenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSet": {
+        "GetSequenceStore": {
             "access_level": "Undocumented",
-            "action": "GetReadSet",
+            "action": "GetSequenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSequenceStore": {
+        "CreateSequenceStore": {
             "access_level": "Undocumented",
-            "action": "GetSequenceStore",
+            "action": "CreateSequenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWorkflow": {
+        "GetVariantImportJob": {
             "access_level": "Undocumented",
-            "action": "GetWorkflow",
+            "action": "GetVariantImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAnnotationStore": {
+        "CreateShare": {
             "access_level": "Undocumented",
-            "action": "CreateAnnotationStore",
+            "action": "CreateShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReadSetExportJob": {
+        "ListShares": {
             "access_level": "Undocumented",
-            "action": "GetReadSetExportJob",
+            "action": "ListShares",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWorkflow": {
+        "DeleteRun": {
             "access_level": "Undocumented",
-            "action": "DeleteWorkflow",
+            "action": "DeleteRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRunGroup": {
+        "ListRuns": {
             "access_level": "Undocumented",
-            "action": "UpdateRunGroup",
+            "action": "ListRuns",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAnnotationStoreVersions": {
+        "ListReferences": {
             "access_level": "Undocumented",
-            "action": "DeleteAnnotationStoreVersions",
+            "action": "ListReferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartReadSetImportJob": {
+        "ListReferenceImportJobs": {
             "access_level": "Undocumented",
-            "action": "StartReadSetImportJob",
+            "action": "ListReferenceImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateVariantStore": {
+        "ListRunTasks": {
             "access_level": "Undocumented",
-            "action": "UpdateVariantStore",
+            "action": "ListRunTasks",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSetImportJobs": {
+        "ListVariantImportJobs": {
             "access_level": "Undocumented",
-            "action": "ListReadSetImportJobs",
+            "action": "ListVariantImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRunTask": {
+        "GetRunGroup": {
             "access_level": "Undocumented",
-            "action": "GetRunTask",
+            "action": "GetRunGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReferenceStores": {
+        "ListReadSetActivationJobs": {
             "access_level": "Undocumented",
-            "action": "ListReferenceStores",
+            "action": "ListReadSetActivationJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "CancelAnnotationImportJob": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "CancelAnnotationImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRunGroup": {
+        "DeleteReference": {
             "access_level": "Undocumented",
-            "action": "DeleteRunGroup",
+            "action": "DeleteReference",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReferenceMetadata": {
+        "GetAnnotationImportJob": {
             "access_level": "Undocumented",
-            "action": "GetReferenceMetadata",
+            "action": "GetAnnotationImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReferenceStore": {
+        "DeleteShare": {
             "access_level": "Undocumented",
-            "action": "GetReferenceStore",
+            "action": "DeleteShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSetUploadParts": {
+        "AbortMultipartReadSetUpload": {
             "access_level": "Undocumented",
-            "action": "ListReadSetUploadParts",
+            "action": "AbortMultipartReadSetUpload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAnnotationStoreVersion": {
+        "ListReadSetUploadParts": {
             "access_level": "Undocumented",
-            "action": "GetAnnotationStoreVersion",
+            "action": "ListReadSetUploadParts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAnnotationImportJob": {
+        "BatchDeleteReadSet": {
             "access_level": "Undocumented",
-            "action": "StartAnnotationImportJob",
+            "action": "BatchDeleteReadSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWorkflow": {
+        "GetWorkflow": {
             "access_level": "Undocumented",
-            "action": "UpdateWorkflow",
+            "action": "GetWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRunTasks": {
+        "UpdateAnnotationStore": {
             "access_level": "Undocumented",
-            "action": "ListRunTasks",
+            "action": "UpdateAnnotationStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CancelRun": {
             "access_level": "Undocumented",
             "action": "CancelRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAnnotationImportJob": {
+        "GetShare": {
             "access_level": "Undocumented",
-            "action": "GetAnnotationImportJob",
+            "action": "GetShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAnnotationStore": {
+        "CreateRunGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateAnnotationStore",
+            "action": "CreateRunGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartReadSetExportJob": {
+        "GetReferenceImportJob": {
             "access_level": "Undocumented",
-            "action": "StartReadSetExportJob",
+            "action": "GetReferenceImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSequenceStore": {
+        "UpdateVariantStore": {
             "access_level": "Undocumented",
-            "action": "DeleteSequenceStore",
+            "action": "UpdateVariantStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "StartReferenceImportJob": {
             "access_level": "Undocumented",
             "action": "StartReferenceImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListVariantStores": {
+        "StartReadSetExportJob": {
             "access_level": "Undocumented",
-            "action": "ListVariantStores",
+            "action": "StartReadSetExportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWorkflow": {
+        "DeleteAnnotationStore": {
             "access_level": "Undocumented",
-            "action": "CreateWorkflow",
+            "action": "DeleteAnnotationStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRuns": {
+        "CreateReferenceStore": {
             "access_level": "Undocumented",
-            "action": "ListRuns",
+            "action": "CreateReferenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteVariantStore": {
+        "StartRun": {
             "access_level": "Undocumented",
-            "action": "DeleteVariantStore",
+            "action": "StartRun",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSets": {
+        "CreateWorkflow": {
             "access_level": "Undocumented",
-            "action": "ListReadSets",
+            "action": "CreateWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListShares": {
+        "ListAnnotationImportJobs": {
             "access_level": "Undocumented",
-            "action": "ListShares",
+            "action": "ListAnnotationImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AbortMultipartReadSetUpload": {
+        "ListReadSetExportJobs": {
             "access_level": "Undocumented",
-            "action": "AbortMultipartReadSetUpload",
+            "action": "ListReadSetExportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRunGroup": {
+        "DeleteSequenceStore": {
             "access_level": "Undocumented",
-            "action": "GetRunGroup",
+            "action": "DeleteSequenceStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "StartVariantImportJob": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "StartVariantImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UploadReadSetPart": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "UploadReadSetPart",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAnnotationStore": {
+        "CancelVariantImportJob": {
             "access_level": "Undocumented",
-            "action": "DeleteAnnotationStore",
+            "action": "CancelVariantImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListReadSetExportJobs": {
+        "CreateAnnotationStoreVersion": {
             "access_level": "Undocumented",
-            "action": "ListReadSetExportJobs",
+            "action": "CreateAnnotationStoreVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMultipartReadSetUploads": {
+        "UploadReadSetPart": {
             "access_level": "Undocumented",
-            "action": "ListMultipartReadSetUploads",
+            "action": "UploadReadSetPart",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAnnotationImportJobs": {
+        "DeleteWorkflow": {
             "access_level": "Undocumented",
-            "action": "ListAnnotationImportJobs",
+            "action": "DeleteWorkflow",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartRun": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "StartRun",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetReferenceImportJob": {
+        "StartAnnotationImportJob": {
             "access_level": "Undocumented",
-            "action": "GetReferenceImportJob",
+            "action": "StartAnnotationImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRun": {
+        "ListSequenceStores": {
             "access_level": "Undocumented",
-            "action": "GetRun",
+            "action": "ListSequenceStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAnnotationStoreVersions": {
+        "GetVariantStore": {
             "access_level": "Undocumented",
-            "action": "ListAnnotationStoreVersions",
+            "action": "GetVariantStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "one": {
-        "GetSite": {
+        "ListDeviceConfigurationTemplates": {
             "access_level": "Undocumented",
-            "action": "GetSite",
+            "action": "ListDeviceConfigurationTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSite": {
+        "CreateDeviceInstanceConfiguration": {
             "access_level": "Undocumented",
-            "action": "DeleteSite",
+            "action": "CreateDeviceInstanceConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSiteAddress": {
+        "DeleteSite": {
             "access_level": "Undocumented",
-            "action": "GetSiteAddress",
+            "action": "DeleteSite",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDeviceConfigurationTemplate": {
+        "GetSiteAddress": {
             "access_level": "Undocumented",
-            "action": "DeleteDeviceConfigurationTemplate",
+            "action": "GetSiteAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceInstances": {
+        "CreateDeviceConfigurationTemplate": {
             "access_level": "Undocumented",
-            "action": "ListDeviceInstances",
+            "action": "CreateDeviceConfigurationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUser": {
+        "CreateSite": {
             "access_level": "Undocumented",
-            "action": "DeleteUser",
+            "action": "CreateSite",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDeviceInstance": {
+        "RebootDevice": {
             "access_level": "Undocumented",
-            "action": "UpdateDeviceInstance",
+            "action": "RebootDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAssociatedDevice": {
+        "UpdateSite": {
             "access_level": "Undocumented",
-            "action": "DeleteAssociatedDevice",
+            "action": "UpdateSite",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceInstance": {
+        "GetDeviceConfigurationTemplate": {
             "access_level": "Undocumented",
-            "action": "GetDeviceInstance",
+            "action": "GetDeviceConfigurationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceConfigurationTemplate": {
+        "DeleteDeviceConfigurationTemplate": {
             "access_level": "Undocumented",
-            "action": "GetDeviceConfigurationTemplate",
+            "action": "DeleteDeviceConfigurationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSite": {
+        "ListUsers": {
             "access_level": "Undocumented",
-            "action": "UpdateSite",
+            "action": "ListUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDeviceInstance": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteDeviceInstance",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceInstance": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceInstance",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSiteAddress": {
+        "DeleteAssociatedDevice": {
             "access_level": "Undocumented",
-            "action": "UpdateSiteAddress",
+            "action": "DeleteAssociatedDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteDeviceInstance": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteDeviceInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateDeviceActivationQrCode": {
             "access_level": "Undocumented",
             "action": "CreateDeviceActivationQrCode",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSite": {
+        "DeleteUser": {
             "access_level": "Undocumented",
-            "action": "CreateSite",
+            "action": "DeleteUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetDeviceInstanceConfiguration": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetDeviceInstanceConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDeviceInstanceConfiguration": {
+        "ListDeviceInstances": {
             "access_level": "Undocumented",
-            "action": "GetDeviceInstanceConfiguration",
+            "action": "ListDeviceInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUsers": {
+        "UpdateSiteAddress": {
             "access_level": "Undocumented",
-            "action": "ListUsers",
+            "action": "UpdateSiteAddress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetSite": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetSite",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDeviceConfigurationTemplate": {
+        "CreateDeviceInstance": {
             "access_level": "Undocumented",
-            "action": "UpdateDeviceConfigurationTemplate",
+            "action": "CreateDeviceInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RebootDevice": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "RebootDevice",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSites": {
+        "UpdateDeviceInstance": {
             "access_level": "Undocumented",
-            "action": "ListSites",
+            "action": "UpdateDeviceInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceInstanceConfiguration": {
+        "UpdateDeviceConfigurationTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceInstanceConfiguration",
+            "action": "UpdateDeviceConfigurationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDeviceConfigurationTemplate": {
+        "GetDeviceInstance": {
             "access_level": "Undocumented",
-            "action": "CreateDeviceConfigurationTemplate",
+            "action": "GetDeviceInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceConfigurationTemplates": {
+        "ListSites": {
             "access_level": "Undocumented",
-            "action": "ListDeviceConfigurationTemplates",
+            "action": "ListSites",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "opsworks": {
@@ -118321,129 +118321,129 @@
             "orphan": false,
             "resources": [
                 "policy"
             ]
         }
     },
     "osis": {
-        "ListPipelineBlueprints": {
+        "GetPipeline": {
             "access_level": "Undocumented",
-            "action": "ListPipelineBlueprints",
+            "action": "GetPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipelineChangeProgress": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetPipelineChangeProgress",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "CreatePipeline": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "CreatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidatePipeline": {
+        "GetPipelineBlueprint": {
             "access_level": "Undocumented",
-            "action": "ValidatePipeline",
+            "action": "GetPipelineBlueprint",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListPipelineBlueprints": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListPipelineBlueprints",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeletePipeline": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeletePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipelineBlueprint": {
+        "GetPipelineChangeProgress": {
             "access_level": "Undocumented",
-            "action": "GetPipelineBlueprint",
+            "action": "GetPipelineChangeProgress",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPipelines": {
+        "StopPipeline": {
             "access_level": "Undocumented",
-            "action": "ListPipelines",
+            "action": "StopPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePipeline": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "CreatePipeline",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopPipeline": {
+        "ListPipelines": {
             "access_level": "Undocumented",
-            "action": "StopPipeline",
+            "action": "ListPipelines",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePipeline": {
+        "UpdatePipeline": {
             "access_level": "Undocumented",
-            "action": "DeletePipeline",
+            "action": "UpdatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartPipeline": {
+        "ValidatePipeline": {
             "access_level": "Undocumented",
-            "action": "StartPipeline",
+            "action": "ValidatePipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePipeline": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdatePipeline",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "Ingest": {
             "access_level": "Undocumented",
             "action": "Ingest",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPipeline": {
+        "StartPipeline": {
             "access_level": "Undocumented",
-            "action": "GetPipeline",
+            "action": "StartPipeline",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "outposts": {
@@ -119058,543 +119058,543 @@
             "orphan": false,
             "resources": [
                 "device"
             ]
         }
     },
     "partnercentral-account-management": {
-        "DisassociatePartnerUser": {
+        "AssociatePartnerAccount": {
             "access_level": "Undocumented",
-            "action": "DisassociatePartnerUser",
+            "action": "AssociatePartnerAccount",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociatePartnerAccount": {
+        "AssociatePartnerUser": {
             "access_level": "Undocumented",
-            "action": "AssociatePartnerAccount",
+            "action": "AssociatePartnerUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociatePartnerUser": {
+        "DisassociatePartnerUser": {
             "access_level": "Undocumented",
-            "action": "AssociatePartnerUser",
+            "action": "DisassociatePartnerUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "payment-cryptography": {
-        "TranslatePinData": {
+        "VerifyCardValidationData": {
             "access_level": "Undocumented",
-            "action": "TranslatePinData",
+            "action": "VerifyCardValidationData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetKey": {
+        "GeneratePinData": {
             "access_level": "Undocumented",
-            "action": "GetKey",
+            "action": "GeneratePinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAlias": {
+        "CreateKey": {
             "access_level": "Undocumented",
-            "action": "CreateAlias",
+            "action": "CreateKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GeneratePinData": {
+        "DeleteKey": {
             "access_level": "Undocumented",
-            "action": "GeneratePinData",
+            "action": "DeleteKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAlias": {
+        "GetPublicKeyCertificate": {
             "access_level": "Undocumented",
-            "action": "GetAlias",
+            "action": "GetPublicKeyCertificate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetParametersForExport": {
+        "StopKeyUsage": {
             "access_level": "Undocumented",
-            "action": "GetParametersForExport",
+            "action": "StopKeyUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateKey": {
+        "GenerateMac": {
             "access_level": "Undocumented",
-            "action": "CreateKey",
+            "action": "GenerateMac",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetParametersForImport": {
+        "VerifyMac": {
             "access_level": "Undocumented",
-            "action": "GetParametersForImport",
+            "action": "VerifyMac",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListAliases": {
             "access_level": "Undocumented",
             "action": "ListAliases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopKeyUsage": {
+        "UpdateAlias": {
             "access_level": "Undocumented",
-            "action": "StopKeyUsage",
+            "action": "UpdateAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EncryptData": {
+        "VerifyPinData": {
             "access_level": "Undocumented",
-            "action": "EncryptData",
+            "action": "VerifyPinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateCardValidationData": {
+        "ExportKey": {
             "access_level": "Undocumented",
-            "action": "GenerateCardValidationData",
+            "action": "ExportKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ImportKey": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ImportKey",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartKeyUsage": {
+        "ImportKey": {
             "access_level": "Undocumented",
-            "action": "StartKeyUsage",
+            "action": "ImportKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ExportKey": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ExportKey",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "VerifyAuthRequestCryptogram": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "VerifyAuthRequestCryptogram",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DecryptData": {
+        "DeleteAlias": {
             "access_level": "Undocumented",
-            "action": "DecryptData",
+            "action": "DeleteAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyMac": {
+        "GetKey": {
             "access_level": "Undocumented",
-            "action": "VerifyMac",
+            "action": "GetKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAlias": {
+        "ListKeys": {
             "access_level": "Undocumented",
-            "action": "DeleteAlias",
+            "action": "ListKeys",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyAuthRequestCryptogram": {
+        "TranslatePinData": {
             "access_level": "Undocumented",
-            "action": "VerifyAuthRequestCryptogram",
+            "action": "TranslatePinData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreateAlias": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreateAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ReEncryptData": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ReEncryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAlias": {
+        "RestoreKey": {
             "access_level": "Undocumented",
-            "action": "UpdateAlias",
+            "action": "RestoreKey",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReEncryptData": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "ReEncryptData",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyCardValidationData": {
+        "GenerateCardValidationData": {
             "access_level": "Undocumented",
-            "action": "VerifyCardValidationData",
+            "action": "GenerateCardValidationData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPublicKeyCertificate": {
+        "GetAlias": {
             "access_level": "Undocumented",
-            "action": "GetPublicKeyCertificate",
+            "action": "GetAlias",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "VerifyPinData": {
+        "EncryptData": {
             "access_level": "Undocumented",
-            "action": "VerifyPinData",
+            "action": "EncryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GenerateMac": {
+        "StartKeyUsage": {
             "access_level": "Undocumented",
-            "action": "GenerateMac",
+            "action": "StartKeyUsage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteKey": {
+        "DecryptData": {
             "access_level": "Undocumented",
-            "action": "DeleteKey",
+            "action": "DecryptData",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListKeys": {
+        "GetParametersForExport": {
             "access_level": "Undocumented",
-            "action": "ListKeys",
+            "action": "GetParametersForExport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RestoreKey": {
+        "GetParametersForImport": {
             "access_level": "Undocumented",
-            "action": "RestoreKey",
+            "action": "GetParametersForImport",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "payments": {
-        "UpdatePaymentPreferences": {
+        "MakePayment": {
             "access_level": "Undocumented",
-            "action": "UpdatePaymentPreferences",
+            "action": "MakePayment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePaymentInstrument": {
+        "GetPaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "CreatePaymentInstrument",
+            "action": "GetPaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeletePaymentInstrument": {
             "access_level": "Undocumented",
             "action": "DeletePaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "MakePayment": {
+        "ListPaymentPreferences": {
             "access_level": "Undocumented",
-            "action": "MakePayment",
+            "action": "ListPaymentPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetPaymentStatus": {
             "access_level": "Undocumented",
             "action": "GetPaymentStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPaymentInstrument": {
+        "CreatePaymentInstrument": {
             "access_level": "Undocumented",
-            "action": "GetPaymentInstrument",
+            "action": "CreatePaymentInstrument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPaymentPreferences": {
+        "UpdatePaymentPreferences": {
             "access_level": "Undocumented",
-            "action": "ListPaymentPreferences",
+            "action": "UpdatePaymentPreferences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "pca-connector-ad": {
-        "ListConnectors": {
+        "ListDirectoryRegistrations": {
             "access_level": "Undocumented",
-            "action": "ListConnectors",
+            "action": "ListDirectoryRegistrations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetServicePrincipalName": {
+        "DeleteConnector": {
             "access_level": "Undocumented",
-            "action": "GetServicePrincipalName",
+            "action": "DeleteConnector",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTemplate": {
+        "CreateTemplate": {
             "access_level": "Undocumented",
-            "action": "GetTemplate",
+            "action": "CreateTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateConnector": {
+        "CreateServicePrincipalName": {
             "access_level": "Undocumented",
-            "action": "CreateConnector",
+            "action": "CreateServicePrincipalName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTemplate": {
+        "GetServicePrincipalName": {
             "access_level": "Undocumented",
-            "action": "UpdateTemplate",
+            "action": "GetServicePrincipalName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTemplate": {
+        "GetTemplateGroupAccessControlEntry": {
             "access_level": "Undocumented",
-            "action": "DeleteTemplate",
+            "action": "GetTemplateGroupAccessControlEntry",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteTemplateGroupAccessControlEntry": {
+        "DeleteDirectoryRegistration": {
             "access_level": "Undocumented",
-            "action": "DeleteTemplateGroupAccessControlEntry",
+            "action": "DeleteDirectoryRegistration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetConnector": {
             "access_level": "Undocumented",
             "action": "GetConnector",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTemplate": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "CreateTemplate",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTemplateGroupAccessControlEntries": {
+        "ListTemplates": {
             "access_level": "Undocumented",
-            "action": "ListTemplateGroupAccessControlEntries",
+            "action": "ListTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDirectoryRegistration": {
+        "CreateDirectoryRegistration": {
             "access_level": "Undocumented",
-            "action": "DeleteDirectoryRegistration",
+            "action": "CreateDirectoryRegistration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDirectoryRegistration": {
+        "UpdateTemplateGroupAccessControlEntry": {
             "access_level": "Undocumented",
-            "action": "CreateDirectoryRegistration",
+            "action": "UpdateTemplateGroupAccessControlEntry",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateTemplateGroupAccessControlEntry": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateTemplateGroupAccessControlEntry",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTemplateGroupAccessControlEntry": {
+        "ListTemplateGroupAccessControlEntries": {
             "access_level": "Undocumented",
-            "action": "GetTemplateGroupAccessControlEntry",
+            "action": "ListTemplateGroupAccessControlEntries",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteServicePrincipalName": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteServicePrincipalName",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConnector": {
+        "UpdateTemplate": {
             "access_level": "Undocumented",
-            "action": "DeleteConnector",
+            "action": "UpdateTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteServicePrincipalName": {
+        "DeleteTemplateGroupAccessControlEntry": {
             "access_level": "Undocumented",
-            "action": "DeleteServicePrincipalName",
+            "action": "DeleteTemplateGroupAccessControlEntry",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTemplates": {
+        "ListConnectors": {
             "access_level": "Undocumented",
-            "action": "ListTemplates",
+            "action": "ListConnectors",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetDirectoryRegistration": {
             "access_level": "Undocumented",
             "action": "GetDirectoryRegistration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetTemplate": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateTemplateGroupAccessControlEntry": {
+        "DeleteTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateTemplateGroupAccessControlEntry",
+            "action": "DeleteTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListServicePrincipalNames": {
             "access_level": "Undocumented",
             "action": "ListServicePrincipalNames",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDirectoryRegistrations": {
+        "CreateTemplateGroupAccessControlEntry": {
             "access_level": "Undocumented",
-            "action": "ListDirectoryRegistrations",
+            "action": "CreateTemplateGroupAccessControlEntry",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateServicePrincipalName": {
+        "CreateConnector": {
             "access_level": "Undocumented",
-            "action": "CreateServicePrincipalName",
+            "action": "CreateConnector",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "personalize": {
@@ -122923,475 +122923,475 @@
             "orphan": false,
             "resources": [
                 "purchase-order"
             ]
         }
     },
     "q": {
-        "SendMessage": {
+        "GetTroubleshootingResults": {
             "access_level": "Undocumented",
-            "action": "SendMessage",
+            "action": "GetTroubleshootingResults",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "StartTroubleshootingResolutionExplanation": {
             "access_level": "Undocumented",
             "action": "StartTroubleshootingResolutionExplanation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetTroubleshootingResults": {
+        "StartConversation": {
             "access_level": "Undocumented",
-            "action": "GetTroubleshootingResults",
+            "action": "StartConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetConversation": {
             "access_level": "Undocumented",
             "action": "GetConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartTroubleshootingAnalysis": {
+        "SendMessage": {
             "access_level": "Undocumented",
-            "action": "StartTroubleshootingAnalysis",
+            "action": "SendMessage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConversations": {
+        "StartTroubleshootingAnalysis": {
             "access_level": "Undocumented",
-            "action": "ListConversations",
+            "action": "StartTroubleshootingAnalysis",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartConversation": {
+        "ListConversations": {
             "access_level": "Undocumented",
-            "action": "StartConversation",
+            "action": "ListConversations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "qbusiness": {
-        "PutFeedback": {
+        "UpdateRetriever": {
             "access_level": "Undocumented",
-            "action": "PutFeedback",
+            "action": "UpdateRetriever",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDataSource": {
+        "DeleteIndex": {
             "access_level": "Undocumented",
-            "action": "GetDataSource",
+            "action": "DeleteIndex",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteConversation": {
+        "RemoveUserLicenses": {
             "access_level": "Undocumented",
-            "action": "DeleteConversation",
+            "action": "RemoveUserLicenses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutGroup": {
+        "CreateRetriever": {
             "access_level": "Undocumented",
-            "action": "PutGroup",
+            "action": "CreateRetriever",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListMessages": {
+        "DeleteWebExperience": {
             "access_level": "Undocumented",
-            "action": "ListMessages",
+            "action": "DeleteWebExperience",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteChatControlsConfiguration": {
+        "DeleteConversation": {
             "access_level": "Undocumented",
-            "action": "DeleteChatControlsConfiguration",
+            "action": "DeleteConversation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateUser": {
+        "GetLicense": {
             "access_level": "Undocumented",
-            "action": "CreateUser",
+            "action": "GetLicense",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteUser": {
+        "CreatePlugin": {
             "access_level": "Undocumented",
-            "action": "DeleteUser",
+            "action": "CreatePlugin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIndices": {
+        "AddUserLicenses": {
             "access_level": "Undocumented",
-            "action": "ListIndices",
+            "action": "AddUserLicenses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StopDataSourceSyncJob": {
+        "UpdatePlugin": {
             "access_level": "Undocumented",
-            "action": "StopDataSourceSyncJob",
+            "action": "UpdatePlugin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateWebExperience": {
+        "CreateDataSource": {
             "access_level": "Undocumented",
-            "action": "UpdateWebExperience",
+            "action": "CreateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDataSource": {
+        "PutFeedback": {
             "access_level": "Undocumented",
-            "action": "DeleteDataSource",
+            "action": "PutFeedback",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDataSource": {
+        "ListGroups": {
             "access_level": "Undocumented",
-            "action": "UpdateDataSource",
+            "action": "ListGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ChatSync": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ChatSync",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetGroup": {
+        "UpdateUser": {
             "access_level": "Undocumented",
-            "action": "GetGroup",
+            "action": "UpdateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetWebExperience": {
+        "DeleteApplication": {
             "access_level": "Undocumented",
-            "action": "GetWebExperience",
+            "action": "DeleteApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSources": {
+        "CreateLicense": {
             "access_level": "Undocumented",
-            "action": "ListDataSources",
+            "action": "CreateLicense",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateUser": {
+        "ListConversations": {
             "access_level": "Undocumented",
-            "action": "UpdateUser",
+            "action": "ListConversations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePlugin": {
+        "ListMessages": {
             "access_level": "Undocumented",
-            "action": "DeletePlugin",
+            "action": "ListMessages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetLicense": {
+        "BatchPutDocument": {
             "access_level": "Undocumented",
-            "action": "GetLicense",
+            "action": "BatchPutDocument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRetriever": {
+        "DeletePlugin": {
             "access_level": "Undocumented",
-            "action": "GetRetriever",
+            "action": "DeletePlugin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListPlugins": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListPlugins",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePlugin": {
+        "DeleteDataSource": {
             "access_level": "Undocumented",
-            "action": "CreatePlugin",
+            "action": "DeleteDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListUserLicenses": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListUserLicenses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveUserLicenses": {
+        "StartDataSourceSyncJob": {
             "access_level": "Undocumented",
-            "action": "RemoveUserLicenses",
+            "action": "StartDataSourceSyncJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetUser": {
+        "UpdateChatControlsConfiguration": {
             "access_level": "Undocumented",
-            "action": "GetUser",
+            "action": "UpdateChatControlsConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPlugins": {
+        "ListApplications": {
             "access_level": "Undocumented",
-            "action": "ListPlugins",
+            "action": "ListApplications",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateApplication": {
+        "UpdateWebExperience": {
             "access_level": "Undocumented",
-            "action": "UpdateApplication",
+            "action": "UpdateWebExperience",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIndex": {
+        "ListDataSources": {
             "access_level": "Undocumented",
-            "action": "CreateIndex",
+            "action": "ListDataSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDataSourceSyncJobs": {
+        "DeleteGroup": {
             "access_level": "Undocumented",
-            "action": "ListDataSourceSyncJobs",
+            "action": "DeleteGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRetrievers": {
+        "UpdateApplication": {
             "access_level": "Undocumented",
-            "action": "ListRetrievers",
+            "action": "UpdateApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchDeleteDocument": {
+        "GetPlugin": {
             "access_level": "Undocumented",
-            "action": "BatchDeleteDocument",
+            "action": "GetPlugin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateApplication": {
+        "ListRetrievers": {
             "access_level": "Undocumented",
-            "action": "CreateApplication",
+            "action": "ListRetrievers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateChatControlsConfiguration": {
+        "GetWebExperience": {
             "access_level": "Undocumented",
-            "action": "UpdateChatControlsConfiguration",
+            "action": "GetWebExperience",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPlugin": {
+        "ListIndices": {
             "access_level": "Undocumented",
-            "action": "GetPlugin",
+            "action": "ListIndices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateRetriever": {
+        "GetApplication": {
             "access_level": "Undocumented",
-            "action": "UpdateRetriever",
+            "action": "GetApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetChatControlsConfiguration": {
+        "GetIndex": {
             "access_level": "Undocumented",
-            "action": "GetChatControlsConfiguration",
+            "action": "GetIndex",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListGroups": {
+        "GetUser": {
             "access_level": "Undocumented",
-            "action": "ListGroups",
+            "action": "GetUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateLicense": {
+        "UpdateDataSource": {
             "access_level": "Undocumented",
-            "action": "CreateLicense",
+            "action": "UpdateDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteGroup": {
+        "CreateWebExperience": {
             "access_level": "Undocumented",
-            "action": "DeleteGroup",
+            "action": "CreateWebExperience",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUserLicenses": {
+        "BatchDeleteDocument": {
             "access_level": "Undocumented",
-            "action": "ListUserLicenses",
+            "action": "BatchDeleteDocument",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIndex": {
+        "GetGroup": {
             "access_level": "Undocumented",
-            "action": "UpdateIndex",
+            "action": "GetGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListApplications": {
+        "PutGroup": {
             "access_level": "Undocumented",
-            "action": "ListApplications",
+            "action": "PutGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRetriever": {
+        "ChatSync": {
             "access_level": "Undocumented",
-            "action": "CreateRetriever",
+            "action": "ChatSync",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartDataSourceSyncJob": {
+        "DeleteChatControlsConfiguration": {
             "access_level": "Undocumented",
-            "action": "StartDataSourceSyncJob",
+            "action": "DeleteChatControlsConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIndex": {
+        "CreateApplication": {
             "access_level": "Undocumented",
-            "action": "GetIndex",
+            "action": "CreateApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "UntagResource": {
             "access_level": "Undocumented",
             "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchPutDocument": {
+        "CreateUser": {
             "access_level": "Undocumented",
-            "action": "BatchPutDocument",
+            "action": "CreateUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIndex": {
+        "DeleteUser": {
             "access_level": "Undocumented",
-            "action": "DeleteIndex",
+            "action": "DeleteUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteRetriever": {
             "access_level": "Undocumented",
             "action": "DeleteRetriever",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteWebExperience": {
+        "ListDataSourceSyncJobs": {
             "access_level": "Undocumented",
-            "action": "DeleteWebExperience",
+            "action": "ListDataSourceSyncJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListDocuments": {
             "access_level": "Undocumented",
@@ -123405,73 +123405,73 @@
             "access_level": "Undocumented",
             "action": "ListWebExperiences",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "Chat": {
+        "StopDataSourceSyncJob": {
             "access_level": "Undocumented",
-            "action": "Chat",
+            "action": "StopDataSourceSyncJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteApplication": {
+        "GetDataSource": {
             "access_level": "Undocumented",
-            "action": "DeleteApplication",
+            "action": "GetDataSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddUserLicenses": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "AddUserLicenses",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateWebExperience": {
+        "UpdateIndex": {
             "access_level": "Undocumented",
-            "action": "CreateWebExperience",
+            "action": "UpdateIndex",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListConversations": {
+        "Chat": {
             "access_level": "Undocumented",
-            "action": "ListConversations",
+            "action": "Chat",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetApplication": {
+        "CreateIndex": {
             "access_level": "Undocumented",
-            "action": "GetApplication",
+            "action": "CreateIndex",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDataSource": {
+        "GetRetriever": {
             "access_level": "Undocumented",
-            "action": "CreateDataSource",
+            "action": "GetRetriever",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePlugin": {
+        "GetChatControlsConfiguration": {
             "access_level": "Undocumented",
-            "action": "UpdatePlugin",
+            "action": "GetChatControlsConfiguration",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "qldb": {
@@ -125920,281 +125920,281 @@
             "orphan": false,
             "resources": [
                 "vpcconnection"
             ]
         }
     },
     "ram": {
-        "CreatePermissionVersion": {
+        "CreatePermission": {
             "access_level": "Undocumented",
-            "action": "CreatePermissionVersion",
+            "action": "CreatePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissionAssociations": {
+        "CreateResourceShare": {
             "access_level": "Undocumented",
-            "action": "ListPermissionAssociations",
+            "action": "CreateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResourceShare": {
+        "PromoteResourceShareCreatedFromPolicy": {
             "access_level": "Undocumented",
-            "action": "UpdateResourceShare",
+            "action": "PromoteResourceShareCreatedFromPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissions": {
+        "CreatePermissionVersion": {
             "access_level": "Undocumented",
-            "action": "ListPermissions",
+            "action": "CreatePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPermission": {
+        "DeleteResourceShare": {
             "access_level": "Undocumented",
-            "action": "GetPermission",
+            "action": "DeleteResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShareInvitations": {
+        "ListResourceTypes": {
             "access_level": "Undocumented",
-            "action": "GetResourceShareInvitations",
+            "action": "ListResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceSharePermissions": {
+        "ListPermissions": {
             "access_level": "Undocumented",
-            "action": "ListResourceSharePermissions",
+            "action": "ListPermissions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourcePolicies": {
+        "ListPendingInvitationResources": {
             "access_level": "Undocumented",
-            "action": "GetResourcePolicies",
+            "action": "ListPendingInvitationResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePermissionVersion": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "DeletePermissionVersion",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetResourcePolicies": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetResourcePolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPrincipals": {
+        "UpdateResourceShare": {
             "access_level": "Undocumented",
-            "action": "ListPrincipals",
+            "action": "UpdateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateResourceShare": {
+        "ListPermissionAssociations": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceShare",
+            "action": "ListPermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePermission": {
+        "AssociateResourceShare": {
             "access_level": "Undocumented",
-            "action": "DeletePermission",
+            "action": "AssociateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ReplacePermissionAssociations": {
+        "AssociateResourceSharePermission": {
             "access_level": "Undocumented",
-            "action": "ReplacePermissionAssociations",
+            "action": "AssociateResourceSharePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RejectResourceShareInvitation": {
+        "ListPermissionVersions": {
             "access_level": "Undocumented",
-            "action": "RejectResourceShareInvitation",
+            "action": "ListPermissionVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AcceptResourceShareInvitation": {
+        "GetResourceShareAssociations": {
             "access_level": "Undocumented",
-            "action": "AcceptResourceShareInvitation",
+            "action": "GetResourceShareAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResources": {
+        "EnableSharingWithAwsOrganization": {
             "access_level": "Undocumented",
-            "action": "ListResources",
+            "action": "EnableSharingWithAwsOrganization",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResourceShare": {
+        "GetResourceShares": {
             "access_level": "Undocumented",
-            "action": "DeleteResourceShare",
+            "action": "GetResourceShares",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceTypes": {
+        "SetDefaultPermissionVersion": {
             "access_level": "Undocumented",
-            "action": "ListResourceTypes",
+            "action": "SetDefaultPermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateResourceShare": {
+        "ReplacePermissionAssociations": {
             "access_level": "Undocumented",
-            "action": "CreateResourceShare",
+            "action": "ReplacePermissionAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListReplacePermissionAssociationsWork": {
             "access_level": "Undocumented",
             "action": "ListReplacePermissionAssociationsWork",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PromotePermissionCreatedFromPolicy": {
+        "DisassociateResourceShare": {
             "access_level": "Undocumented",
-            "action": "PromotePermissionCreatedFromPolicy",
+            "action": "DisassociateResourceShare",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShareAssociations": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetResourceShareAssociations",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeletePermissionVersion": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeletePermissionVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPermissionVersions": {
+        "ListPrincipals": {
             "access_level": "Undocumented",
-            "action": "ListPermissionVersions",
+            "action": "ListPrincipals",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetResourceShares": {
+        "PromotePermissionCreatedFromPolicy": {
             "access_level": "Undocumented",
-            "action": "GetResourceShares",
+            "action": "PromotePermissionCreatedFromPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePermission": {
+        "DisassociateResourceSharePermission": {
             "access_level": "Undocumented",
-            "action": "CreatePermission",
+            "action": "DisassociateResourceSharePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPendingInvitationResources": {
+        "DeletePermission": {
             "access_level": "Undocumented",
-            "action": "ListPendingInvitationResources",
+            "action": "DeletePermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SetDefaultPermissionVersion": {
+        "ListResourceSharePermissions": {
             "access_level": "Undocumented",
-            "action": "SetDefaultPermissionVersion",
+            "action": "ListResourceSharePermissions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "EnableSharingWithAwsOrganization": {
+        "GetPermission": {
             "access_level": "Undocumented",
-            "action": "EnableSharingWithAwsOrganization",
+            "action": "GetPermission",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PromoteResourceShareCreatedFromPolicy": {
+        "RejectResourceShareInvitation": {
             "access_level": "Undocumented",
-            "action": "PromoteResourceShareCreatedFromPolicy",
+            "action": "RejectResourceShareInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateResourceShare": {
+        "ListResources": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceShare",
+            "action": "ListResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AssociateResourceSharePermission": {
+        "AcceptResourceShareInvitation": {
             "access_level": "Undocumented",
-            "action": "AssociateResourceSharePermission",
+            "action": "AcceptResourceShareInvitation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DisassociateResourceSharePermission": {
+        "GetResourceShareInvitations": {
             "access_level": "Undocumented",
-            "action": "DisassociateResourceSharePermission",
+            "action": "GetResourceShareInvitations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "rbin": {
@@ -131576,557 +131576,557 @@
             "orphan": false,
             "resources": [
                 "streamprocessor"
             ]
         }
     },
     "repostspace": {
-        "SendInvites": {
+        "ListSpaces": {
             "access_level": "Undocumented",
-            "action": "SendInvites",
+            "action": "ListSpaces",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeregisterAdmin": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeregisterAdmin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSpace": {
+        "UpdateSpace": {
             "access_level": "Undocumented",
-            "action": "GetSpace",
+            "action": "UpdateSpace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSpace": {
+        "RegisterAdmin": {
             "access_level": "Undocumented",
-            "action": "DeleteSpace",
+            "action": "RegisterAdmin",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSpaces": {
+        "CreateSpace": {
             "access_level": "Undocumented",
-            "action": "ListSpaces",
+            "action": "CreateSpace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetSpace": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetSpace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterAdmin": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeregisterAdmin",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DeleteSpace": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DeleteSpace",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSpace": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateSpace",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSpace": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateSpace",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RegisterAdmin": {
+        "SendInvites": {
             "access_level": "Undocumented",
-            "action": "RegisterAdmin",
+            "action": "SendInvites",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "resiliencehub": {
-        "DeleteApp": {
+        "ListAppVersionAppComponents": {
             "access_level": "Undocumented",
-            "action": "DeleteApp",
+            "action": "ListAppVersionAppComponents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppVersions": {
+        "ListAlarmRecommendations": {
             "access_level": "Undocumented",
-            "action": "ListAppVersions",
+            "action": "ListAlarmRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartAppAssessment": {
+        "DescribeAppVersionResourcesResolutionStatus": {
             "access_level": "Undocumented",
-            "action": "StartAppAssessment",
+            "action": "DescribeAppVersionResourcesResolutionStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppVersionResources": {
+        "CreateApp": {
             "access_level": "Undocumented",
-            "action": "ListAppVersionResources",
+            "action": "CreateApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DescribeApp": {
             "access_level": "Undocumented",
             "action": "DescribeApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppVersionResource": {
+        "ListTestRecommendations": {
             "access_level": "Undocumented",
-            "action": "CreateAppVersionResource",
+            "action": "ListTestRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutDraftAppVersionTemplate": {
+        "ResolveAppVersionResources": {
             "access_level": "Undocumented",
-            "action": "PutDraftAppVersionTemplate",
+            "action": "ResolveAppVersionResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeDraftAppVersionResourcesImportStatus": {
+        "ImportResourcesToDraftAppVersion": {
             "access_level": "Undocumented",
-            "action": "DescribeDraftAppVersionResourcesImportStatus",
+            "action": "ImportResourcesToDraftAppVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersionResourcesResolutionStatus": {
+        "StartAppAssessment": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersionResourcesResolutionStatus",
+            "action": "StartAppAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTestRecommendations": {
+        "CreateAppVersionAppComponent": {
             "access_level": "Undocumented",
-            "action": "ListTestRecommendations",
+            "action": "CreateAppVersionAppComponent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "BatchUpdateRecommendationStatus": {
+        "AddDraftAppVersionResourceMappings": {
             "access_level": "Undocumented",
-            "action": "BatchUpdateRecommendationStatus",
+            "action": "AddDraftAppVersionResourceMappings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAlarmRecommendations": {
+        "CreateAppVersionResource": {
             "access_level": "Undocumented",
-            "action": "ListAlarmRecommendations",
+            "action": "CreateAppVersionResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppAssessmentComplianceDrifts": {
+        "DescribeResiliencyPolicy": {
             "access_level": "Undocumented",
-            "action": "ListAppAssessmentComplianceDrifts",
+            "action": "DescribeResiliencyPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSuggestedResiliencyPolicies": {
+        "ListUnsupportedAppVersionResources": {
             "access_level": "Undocumented",
-            "action": "ListSuggestedResiliencyPolicies",
+            "action": "ListUnsupportedAppVersionResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAppVersionResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateAppVersionResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAppVersionAppComponent": {
+        "CreateRecommendationTemplate": {
             "access_level": "Undocumented",
-            "action": "UpdateAppVersionAppComponent",
+            "action": "CreateRecommendationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppAssessments": {
+        "ListResiliencyPolicies": {
             "access_level": "Undocumented",
-            "action": "ListAppAssessments",
+            "action": "ListResiliencyPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ImportResourcesToDraftAppVersion": {
+        "DeleteAppAssessment": {
             "access_level": "Undocumented",
-            "action": "ImportResourcesToDraftAppVersion",
+            "action": "DeleteAppAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResiliencyPolicies": {
+        "ListAppComponentCompliances": {
             "access_level": "Undocumented",
-            "action": "ListResiliencyPolicies",
+            "action": "ListAppComponentCompliances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppVersionAppComponents": {
+        "DeleteRecommendationTemplate": {
             "access_level": "Undocumented",
-            "action": "ListAppVersionAppComponents",
+            "action": "DeleteRecommendationTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "ListAppVersionResources": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "ListAppVersionResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "DescribeAppVersionResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "DescribeAppVersionResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAppVersionAppComponent": {
+        "UpdateApp": {
             "access_level": "Undocumented",
-            "action": "CreateAppVersionAppComponent",
+            "action": "UpdateApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteRecommendationTemplate": {
+        "DeleteAppVersionAppComponent": {
             "access_level": "Undocumented",
-            "action": "DeleteRecommendationTemplate",
+            "action": "DeleteAppVersionAppComponent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersionResource": {
+        "DescribeDraftAppVersionResourcesImportStatus": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersionResource",
+            "action": "DescribeDraftAppVersionResourcesImportStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateRecommendationTemplate": {
+        "RemoveDraftAppVersionResourceMappings": {
             "access_level": "Undocumented",
-            "action": "CreateRecommendationTemplate",
+            "action": "RemoveDraftAppVersionResourceMappings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListRecommendationTemplates": {
+        "UpdateAppVersionAppComponent": {
             "access_level": "Undocumented",
-            "action": "ListRecommendationTemplates",
+            "action": "UpdateAppVersionAppComponent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ResolveAppVersionResources": {
+        "PublishAppVersion": {
             "access_level": "Undocumented",
-            "action": "ResolveAppVersionResources",
+            "action": "PublishAppVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppComponentRecommendations": {
+        "DescribeAppVersionAppComponent": {
             "access_level": "Undocumented",
-            "action": "ListAppComponentRecommendations",
+            "action": "DescribeAppVersionAppComponent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateAppVersion": {
+        "ListRecommendationTemplates": {
             "access_level": "Undocumented",
-            "action": "UpdateAppVersion",
+            "action": "ListRecommendationTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppInputSource": {
+        "ListSopRecommendations": {
             "access_level": "Undocumented",
-            "action": "DeleteAppInputSource",
+            "action": "ListSopRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppAssessment": {
+        "UpdateAppVersionResource": {
             "access_level": "Undocumented",
-            "action": "DescribeAppAssessment",
+            "action": "UpdateAppVersionResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveDraftAppVersionResourceMappings": {
+        "ListAppAssessmentComplianceDrifts": {
             "access_level": "Undocumented",
-            "action": "RemoveDraftAppVersionResourceMappings",
+            "action": "ListAppAssessmentComplianceDrifts",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersion": {
+        "ListSuggestedResiliencyPolicies": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersion",
+            "action": "ListSuggestedResiliencyPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersionTemplate": {
+        "UpdateResiliencyPolicy": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersionTemplate",
+            "action": "UpdateResiliencyPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeAppVersionAppComponent": {
+        "DeleteApp": {
             "access_level": "Undocumented",
-            "action": "DescribeAppVersionAppComponent",
+            "action": "DeleteApp",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeResiliencyPolicy": {
+        "ListAppAssessments": {
             "access_level": "Undocumented",
-            "action": "DescribeResiliencyPolicy",
+            "action": "ListAppAssessments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSopRecommendations": {
+        "ListAppVersionResourceMappings": {
             "access_level": "Undocumented",
-            "action": "ListSopRecommendations",
+            "action": "ListAppVersionResourceMappings",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppInputSources": {
+        "DescribeAppVersionTemplate": {
             "access_level": "Undocumented",
-            "action": "ListAppInputSources",
+            "action": "DescribeAppVersionTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppVersionResourceMappings": {
+        "DeleteResiliencyPolicy": {
             "access_level": "Undocumented",
-            "action": "ListAppVersionResourceMappings",
+            "action": "DeleteResiliencyPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteResiliencyPolicy": {
+        "UpdateAppVersion": {
             "access_level": "Undocumented",
-            "action": "DeleteResiliencyPolicy",
+            "action": "UpdateAppVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppAssessment": {
+        "DeleteAppVersionResource": {
             "access_level": "Undocumented",
-            "action": "DeleteAppAssessment",
+            "action": "DeleteAppVersionResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppVersionResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteAppVersionResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateApp": {
+        "PutDraftAppVersionTemplate": {
             "access_level": "Undocumented",
-            "action": "UpdateApp",
+            "action": "PutDraftAppVersionTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAppComponentCompliances": {
+        "ListAppComponentRecommendations": {
             "access_level": "Undocumented",
-            "action": "ListAppComponentCompliances",
+            "action": "ListAppComponentRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListUnsupportedAppVersionResources": {
+        "CreateResiliencyPolicy": {
             "access_level": "Undocumented",
-            "action": "ListUnsupportedAppVersionResources",
+            "action": "CreateResiliencyPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateApp": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "CreateApp",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DescribeAppVersion": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DescribeAppVersion",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAppVersionAppComponent": {
+        "BatchUpdateRecommendationStatus": {
             "access_level": "Undocumented",
-            "action": "DeleteAppVersionAppComponent",
+            "action": "BatchUpdateRecommendationStatus",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateResiliencyPolicy": {
+        "ListAppInputSources": {
             "access_level": "Undocumented",
-            "action": "CreateResiliencyPolicy",
+            "action": "ListAppInputSources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListApps": {
+        "DescribeAppAssessment": {
             "access_level": "Undocumented",
-            "action": "ListApps",
+            "action": "DescribeAppAssessment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateResiliencyPolicy": {
+        "DeleteAppInputSource": {
             "access_level": "Undocumented",
-            "action": "UpdateResiliencyPolicy",
+            "action": "DeleteAppInputSource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PublishAppVersion": {
+        "ListAppVersions": {
             "access_level": "Undocumented",
-            "action": "PublishAppVersion",
+            "action": "ListAppVersions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "AddDraftAppVersionResourceMappings": {
+        "ListApps": {
             "access_level": "Undocumented",
-            "action": "AddDraftAppVersionResourceMappings",
+            "action": "ListApps",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "resource-explorer": {
-        "ListResources": {
+        "ListTags": {
             "access_level": "Undocumented",
-            "action": "ListResources",
+            "action": "ListTags",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTags": {
+        "ListResourceTypes": {
             "access_level": "Undocumented",
-            "action": "ListTags",
+            "action": "ListResourceTypes",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListResourceTypes": {
+        "ListResources": {
             "access_level": "Undocumented",
-            "action": "ListResourceTypes",
+            "action": "ListResources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "resource-explorer-2": {
@@ -140081,65 +140081,65 @@
             "orphan": false,
             "resources": [
                 "object"
             ]
         }
     },
     "s3express": {
-        "GetBucketPolicy": {
+        "PutBucketPolicy": {
             "access_level": "Undocumented",
-            "action": "GetBucketPolicy",
+            "action": "PutBucketPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteBucketPolicy": {
+        "ListAllMyDirectoryBuckets": {
             "access_level": "Undocumented",
-            "action": "DeleteBucketPolicy",
+            "action": "ListAllMyDirectoryBuckets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSession": {
+        "DeleteBucketPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateSession",
+            "action": "DeleteBucketPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAllMyDirectoryBuckets": {
+        "CreateSession": {
             "access_level": "Undocumented",
-            "action": "ListAllMyDirectoryBuckets",
+            "action": "CreateSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteBucket": {
+        "CreateBucket": {
             "access_level": "Undocumented",
-            "action": "DeleteBucket",
+            "action": "CreateBucket",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutBucketPolicy": {
+        "DeleteBucket": {
             "access_level": "Undocumented",
-            "action": "PutBucketPolicy",
+            "action": "DeleteBucket",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateBucket": {
+        "GetBucketPolicy": {
             "access_level": "Undocumented",
-            "action": "CreateBucket",
+            "action": "GetBucketPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "sagemaker": {
@@ -144920,137 +144920,137 @@
             "orphan": false,
             "resources": [
                 "schema"
             ]
         }
     },
     "scn": {
-        "AssignAdminPermissionsToUser": {
+        "RemoveAdminPermissionsForUser": {
             "access_level": "Undocumented",
-            "action": "AssignAdminPermissionsToUser",
+            "action": "RemoveAdminPermissionsForUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateInstance": {
+        "GetBillOfMaterialsImportJob": {
             "access_level": "Undocumented",
-            "action": "UpdateInstance",
+            "action": "GetBillOfMaterialsImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateBillOfMaterialsImportJob": {
+        "UpdateInstance": {
             "access_level": "Undocumented",
-            "action": "CreateBillOfMaterialsImportJob",
+            "action": "UpdateInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetBillOfMaterialsImportJob": {
+        "DescribeInstance": {
             "access_level": "Undocumented",
-            "action": "GetBillOfMaterialsImportJob",
+            "action": "DescribeInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListInstances": {
+        "DeleteInstance": {
             "access_level": "Undocumented",
-            "action": "ListInstances",
+            "action": "DeleteInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DescribeInstance": {
+        "DeleteSSOApplication": {
             "access_level": "Undocumented",
-            "action": "DescribeInstance",
+            "action": "DeleteSSOApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveAdminPermissionsForUser": {
+        "CreateSSOApplication": {
             "access_level": "Undocumented",
-            "action": "RemoveAdminPermissionsForUser",
+            "action": "CreateSSOApplication",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateInstance": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "CreateInstance",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "SendDataIntegrationEvent": {
             "access_level": "Undocumented",
             "action": "SendDataIntegrationEvent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAdminUsers": {
+        "ListInstances": {
             "access_level": "Undocumented",
-            "action": "ListAdminUsers",
+            "action": "ListInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CreateBillOfMaterialsImportJob": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CreateBillOfMaterialsImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListAdminUsers": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListAdminUsers",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSSOApplication": {
+        "CreateInstance": {
             "access_level": "Undocumented",
-            "action": "DeleteSSOApplication",
+            "action": "CreateInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSSOApplication": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "CreateSSOApplication",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteInstance": {
+        "AssignAdminPermissionsToUser": {
             "access_level": "Undocumented",
-            "action": "DeleteInstance",
+            "action": "AssignAdminPermissionsToUser",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "sdb": {
@@ -156065,25 +156065,25 @@
             "access_level": "Undocumented",
             "action": "OpenDataChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "OpenControlChannel": {
+        "CreateDataChannel": {
             "access_level": "Undocumented",
-            "action": "OpenControlChannel",
+            "action": "CreateDataChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDataChannel": {
+        "OpenControlChannel": {
             "access_level": "Undocumented",
-            "action": "CreateDataChannel",
+            "action": "OpenControlChannel",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateControlChannel": {
             "access_level": "Undocumented",
@@ -160907,145 +160907,145 @@
             "orphan": false,
             "resources": [
                 "adapter"
             ]
         }
     },
     "thinclient": {
-        "UpdateDevice": {
+        "ListEnvironments": {
             "access_level": "Undocumented",
-            "action": "UpdateDevice",
+            "action": "ListEnvironments",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDevices": {
+        "DeleteEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListDevices",
+            "action": "DeleteEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListEnvironments": {
+        "GetEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListEnvironments",
+            "action": "GetEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSoftwareSets": {
+        "UpdateEnvironment": {
             "access_level": "Undocumented",
-            "action": "ListSoftwareSets",
+            "action": "UpdateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteEnvironment": {
+        "CreateEnvironment": {
             "access_level": "Undocumented",
-            "action": "DeleteEnvironment",
+            "action": "CreateEnvironment",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateEnvironment": {
+        "ListDevices": {
             "access_level": "Undocumented",
-            "action": "CreateEnvironment",
+            "action": "ListDevices",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetEnvironment": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "GetEnvironment",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListDeviceSessions": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListDeviceSessions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "UpdateSoftwareSet": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "UpdateSoftwareSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeregisterDevice": {
+        "DeleteDevice": {
             "access_level": "Undocumented",
-            "action": "DeregisterDevice",
+            "action": "DeleteDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDeviceSessions": {
+        "GetDevice": {
             "access_level": "Undocumented",
-            "action": "ListDeviceSessions",
+            "action": "GetDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateEnvironment": {
+        "DeregisterDevice": {
             "access_level": "Undocumented",
-            "action": "UpdateEnvironment",
+            "action": "DeregisterDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDevice": {
+        "ListSoftwareSets": {
             "access_level": "Undocumented",
-            "action": "GetDevice",
+            "action": "ListSoftwareSets",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDevice": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "DeleteDevice",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSoftwareSet": {
+        "GetSoftwareSet": {
             "access_level": "Undocumented",
-            "action": "UpdateSoftwareSet",
+            "action": "GetSoftwareSet",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSoftwareSet": {
+        "UpdateDevice": {
             "access_level": "Undocumented",
-            "action": "GetSoftwareSet",
+            "action": "UpdateDevice",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "timestream": {
@@ -161395,89 +161395,89 @@
             "orphan": false,
             "resources": [
                 "table"
             ]
         }
     },
     "timestream-influxdb": {
-        "UntagResource": {
+        "UpdateDbInstance": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "UpdateDbInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListDbParameterGroups": {
+        "DeleteDbInstance": {
             "access_level": "Undocumented",
-            "action": "ListDbParameterGroups",
+            "action": "DeleteDbInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListDbInstances": {
             "access_level": "Undocumented",
             "action": "ListDbInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDbInstance": {
+        "CreateDbParameterGroup": {
             "access_level": "Undocumented",
-            "action": "GetDbInstance",
+            "action": "CreateDbParameterGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "ListTagsForResource": {
             "access_level": "Undocumented",
             "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteDbInstance": {
+        "GetDbInstance": {
             "access_level": "Undocumented",
-            "action": "DeleteDbInstance",
+            "action": "GetDbInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "ListDbParameterGroups": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "ListDbParameterGroups",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateDbParameterGroup": {
+        "GetDbParameterGroup": {
             "access_level": "Undocumented",
-            "action": "CreateDbParameterGroup",
+            "action": "GetDbParameterGroup",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateDbInstance": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "UpdateDbInstance",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetDbParameterGroup": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetDbParameterGroup",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "CreateDbInstance": {
             "access_level": "Undocumented",
@@ -161527,273 +161527,273 @@
             "condition_keys": [],
             "description": "Grants permission to list accounts that might be useful in a new query",
             "orphan": false,
             "resources": []
         }
     },
     "tnb": {
-        "UpdateSolFunctionPackage": {
+        "CreateSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "UpdateSolFunctionPackage",
+            "action": "CreateSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolFunctionPackages": {
+        "DeleteSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "ListSolFunctionPackages",
+            "action": "DeleteSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackageContent": {
+        "PutSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackageContent",
+            "action": "PutSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TerminateSolNetworkInstance": {
+        "UpdateSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "TerminateSolNetworkInstance",
+            "action": "UpdateSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "CancelSolNetworkOperation": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "CancelSolNetworkOperation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolNetworkPackage": {
+        "GetSolNetworkPackageDescriptor": {
             "access_level": "Undocumented",
-            "action": "CreateSolNetworkPackage",
+            "action": "GetSolNetworkPackageDescriptor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetSolFunctionPackageDescriptor": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetSolFunctionPackageDescriptor",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolFunctionPackage": {
+        "GetSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "CreateSolFunctionPackage",
+            "action": "GetSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolFunctionPackage": {
+        "CreateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "DeleteSolFunctionPackage",
+            "action": "CreateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidateSolNetworkPackageContent": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ValidateSolNetworkPackageContent",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ValidateSolFunctionPackageContent": {
+        "ValidateSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "ValidateSolFunctionPackageContent",
+            "action": "ValidateSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackageDescriptor": {
+        "GetSolFunctionInstance": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackageDescriptor",
+            "action": "GetSolFunctionInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkInstance": {
+        "GetSolNetworkOperation": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkInstance",
+            "action": "GetSolNetworkOperation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSolNetworkInstance": {
+        "ListSolFunctionPackages": {
             "access_level": "Undocumented",
-            "action": "CreateSolNetworkInstance",
+            "action": "ListSolFunctionPackages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkOperation": {
+        "PutSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkOperation",
+            "action": "PutSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkOperations": {
+        "GetSolNetworkPackageContent": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkOperations",
+            "action": "GetSolNetworkPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolNetworkInstance": {
+        "GetSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "UpdateSolNetworkInstance",
+            "action": "GetSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSolNetworkPackage": {
+        "ValidateSolFunctionPackageContent": {
             "access_level": "Undocumented",
-            "action": "UpdateSolNetworkPackage",
+            "action": "ValidateSolFunctionPackageContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSolFunctionPackageContent": {
+        "TerminateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "PutSolFunctionPackageContent",
+            "action": "TerminateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSolNetworkPackageContent": {
+        "InstantiateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "PutSolNetworkPackageContent",
+            "action": "InstantiateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "DeleteSolNetworkPackage": {
             "access_level": "Undocumented",
             "action": "DeleteSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CancelSolNetworkOperation": {
+        "ListSolNetworkInstances": {
             "access_level": "Undocumented",
-            "action": "CancelSolNetworkOperation",
+            "action": "ListSolNetworkInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteSolNetworkInstance": {
+        "ListSolNetworkPackages": {
             "access_level": "Undocumented",
-            "action": "DeleteSolNetworkInstance",
+            "action": "ListSolNetworkPackages",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "DeleteSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "DeleteSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackage": {
+        "ListSolFunctionInstances": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackage",
+            "action": "ListSolFunctionInstances",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetSolFunctionPackage": {
             "access_level": "Undocumented",
             "action": "GetSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolFunctionInstances": {
+        "UpdateSolNetworkPackage": {
             "access_level": "Undocumented",
-            "action": "ListSolFunctionInstances",
+            "action": "UpdateSolNetworkPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkInstances": {
+        "ListSolNetworkOperations": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkInstances",
+            "action": "ListSolNetworkOperations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListSolNetworkPackages": {
+        "UpdateSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "ListSolNetworkPackages",
+            "action": "UpdateSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolNetworkPackageContent": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "GetSolNetworkPackageContent",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionPackageDescriptor": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionPackageDescriptor",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "InstantiateSolNetworkInstance": {
+        "GetSolNetworkInstance": {
             "access_level": "Undocumented",
-            "action": "InstantiateSolNetworkInstance",
+            "action": "GetSolNetworkInstance",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSolFunctionInstance": {
+        "CreateSolFunctionPackage": {
             "access_level": "Undocumented",
-            "action": "GetSolFunctionInstance",
+            "action": "CreateSolFunctionPackage",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "transcribe": {
@@ -163493,81 +163493,81 @@
             "condition_keys": [],
             "description": "Grants permission to update the risk status in AWS Trusted Advisor Priority",
             "orphan": false,
             "resources": []
         }
     },
     "ts": {
-        "GetExecution": {
+        "StartExecution": {
             "access_level": "Undocumented",
-            "action": "GetExecution",
+            "action": "StartExecution",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListExecutions": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListExecutions",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetExecutionOutput": {
+        "ListTools": {
             "access_level": "Undocumented",
-            "action": "GetExecutionOutput",
+            "action": "ListTools",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetTool": {
             "access_level": "Undocumented",
             "action": "GetTool",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "GetExecutionOutput": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "GetExecutionOutput",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetExecution": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetExecution",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartExecution": {
+        "ListExecutions": {
             "access_level": "Undocumented",
-            "action": "StartExecution",
+            "action": "ListExecutions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTools": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "ListTools",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "vendor-insights": {
@@ -163853,201 +163853,201 @@
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "verifiedpermissions": {
-        "GetPolicyStore": {
+        "GetIdentitySource": {
             "access_level": "Undocumented",
-            "action": "GetPolicyStore",
+            "action": "GetIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListIdentitySources": {
+        "UpdatePolicy": {
             "access_level": "Undocumented",
-            "action": "ListIdentitySources",
+            "action": "UpdatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyTemplates": {
+        "DeletePolicy": {
             "access_level": "Undocumented",
-            "action": "ListPolicyTemplates",
+            "action": "DeletePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSchema": {
+        "UpdateIdentitySource": {
             "access_level": "Undocumented",
-            "action": "GetSchema",
+            "action": "UpdateIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateIdentitySource": {
+        "CreatePolicyStore": {
             "access_level": "Undocumented",
-            "action": "UpdateIdentitySource",
+            "action": "CreatePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetPolicy": {
+        "DeletePolicyStore": {
             "access_level": "Undocumented",
-            "action": "GetPolicy",
+            "action": "DeletePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetIdentitySource": {
+        "UpdatePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "GetIdentitySource",
+            "action": "UpdatePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IsAuthorizedWithToken": {
+        "CreatePolicy": {
             "access_level": "Undocumented",
-            "action": "IsAuthorizedWithToken",
+            "action": "CreatePolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "IsAuthorized": {
+        "CreateIdentitySource": {
             "access_level": "Undocumented",
-            "action": "IsAuthorized",
+            "action": "CreateIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "PutSchema": {
+        "IsAuthorizedWithToken": {
             "access_level": "Undocumented",
-            "action": "PutSchema",
+            "action": "IsAuthorizedWithToken",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePolicy": {
+        "DeleteIdentitySource": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicy",
+            "action": "DeleteIdentitySource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyTemplate": {
+        "GetPolicy": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyTemplate",
+            "action": "GetPolicy",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicyStores": {
+        "PutSchema": {
             "access_level": "Undocumented",
-            "action": "ListPolicyStores",
+            "action": "PutSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyTemplate": {
+        "UpdatePolicyStore": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyTemplate",
+            "action": "UpdatePolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
         "GetPolicyTemplate": {
             "access_level": "Undocumented",
             "action": "GetPolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicy": {
+        "GetSchema": {
             "access_level": "Undocumented",
-            "action": "DeletePolicy",
+            "action": "GetSchema",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePolicyStore": {
+        "IsAuthorized": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicyStore",
+            "action": "IsAuthorized",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListPolicies": {
+        "CreatePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "ListPolicies",
+            "action": "CreatePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeletePolicyStore": {
+        "ListPolicies": {
             "access_level": "Undocumented",
-            "action": "DeletePolicyStore",
+            "action": "ListPolicies",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteIdentitySource": {
+        "ListPolicyTemplates": {
             "access_level": "Undocumented",
-            "action": "DeleteIdentitySource",
+            "action": "ListPolicyTemplates",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateIdentitySource": {
+        "DeletePolicyTemplate": {
             "access_level": "Undocumented",
-            "action": "CreateIdentitySource",
+            "action": "DeletePolicyTemplate",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicy": {
+        "ListPolicyStores": {
             "access_level": "Undocumented",
-            "action": "CreatePolicy",
+            "action": "ListPolicyStores",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdatePolicyTemplate": {
+        "ListIdentitySources": {
             "access_level": "Undocumented",
-            "action": "UpdatePolicyTemplate",
+            "action": "ListIdentitySources",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreatePolicyStore": {
+        "GetPolicyStore": {
             "access_level": "Undocumented",
-            "action": "CreatePolicyStore",
+            "action": "GetPolicyStore",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "voiceid": {
@@ -167978,353 +167978,353 @@
             "orphan": false,
             "resources": [
                 "network"
             ]
         }
     },
     "wisdom": {
-        "PutFeedback": {
+        "GetSession": {
             "access_level": "Undocumented",
-            "action": "PutFeedback",
+            "action": "GetSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchContent": {
+        "GetQuickResponse": {
             "access_level": "Undocumented",
-            "action": "SearchContent",
+            "action": "GetQuickResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetSession": {
+        "GetContentSummary": {
             "access_level": "Undocumented",
-            "action": "GetSession",
+            "action": "GetContentSummary",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchSessions": {
+        "DeleteQuickResponse": {
             "access_level": "Undocumented",
-            "action": "SearchSessions",
+            "action": "DeleteQuickResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAssistant": {
+        "GetContent": {
             "access_level": "Undocumented",
-            "action": "GetAssistant",
+            "action": "GetContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteKnowledgeBase": {
+        "StartContentUpload": {
             "access_level": "Undocumented",
-            "action": "DeleteKnowledgeBase",
+            "action": "StartContentUpload",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetImportJob": {
+        "ListContents": {
             "access_level": "Undocumented",
-            "action": "GetImportJob",
+            "action": "ListContents",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetRecommendations": {
+        "CreateAssistant": {
             "access_level": "Undocumented",
-            "action": "GetRecommendations",
+            "action": "CreateAssistant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "QueryAssistant": {
+        "PutFeedback": {
             "access_level": "Undocumented",
-            "action": "QueryAssistant",
+            "action": "PutFeedback",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssistants": {
+        "CreateQuickResponse": {
             "access_level": "Undocumented",
-            "action": "ListAssistants",
+            "action": "CreateQuickResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListKnowledgeBases": {
+        "TagResource": {
             "access_level": "Undocumented",
-            "action": "ListKnowledgeBases",
+            "action": "TagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartContentUpload": {
+        "GetRecommendations": {
             "access_level": "Undocumented",
-            "action": "StartContentUpload",
+            "action": "GetRecommendations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAssistant": {
+        "DeleteKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "DeleteAssistant",
+            "action": "DeleteKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateSession": {
+        "CreateKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "CreateSession",
+            "action": "CreateKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "RemoveKnowledgeBaseTemplateUri": {
+        "CreateSession": {
             "access_level": "Undocumented",
-            "action": "RemoveKnowledgeBaseTemplateUri",
+            "action": "CreateSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListTagsForResource": {
+        "DeleteImportJob": {
             "access_level": "Undocumented",
-            "action": "ListTagsForResource",
+            "action": "DeleteImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "TagResource": {
+        "GetAssistantAssociation": {
             "access_level": "Undocumented",
-            "action": "TagResource",
+            "action": "GetAssistantAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetKnowledgeBase": {
+        "SearchQuickResponses": {
             "access_level": "Undocumented",
-            "action": "GetKnowledgeBase",
+            "action": "SearchQuickResponses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContent": {
+        "ListAssistantAssociations": {
             "access_level": "Undocumented",
-            "action": "GetContent",
+            "action": "ListAssistantAssociations",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteQuickResponse": {
+        "ListAssistants": {
             "access_level": "Undocumented",
-            "action": "DeleteQuickResponse",
+            "action": "ListAssistants",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteContent": {
+        "GetAssistant": {
             "access_level": "Undocumented",
-            "action": "DeleteContent",
+            "action": "GetAssistant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAssistant": {
+        "SearchContent": {
             "access_level": "Undocumented",
-            "action": "CreateAssistant",
+            "action": "SearchContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteAssistantAssociation": {
+        "GetImportJob": {
             "access_level": "Undocumented",
-            "action": "DeleteAssistantAssociation",
+            "action": "GetImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetQuickResponse": {
+        "SearchSessions": {
             "access_level": "Undocumented",
-            "action": "GetQuickResponse",
+            "action": "SearchSessions",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateSession": {
+        "DeleteContent": {
             "access_level": "Undocumented",
-            "action": "UpdateSession",
+            "action": "DeleteContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateQuickResponse": {
+        "UpdateKnowledgeBaseTemplateUri": {
             "access_level": "Undocumented",
-            "action": "UpdateQuickResponse",
+            "action": "UpdateKnowledgeBaseTemplateUri",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListQuickResponses": {
+        "UpdateContent": {
             "access_level": "Undocumented",
-            "action": "ListQuickResponses",
+            "action": "UpdateContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetAssistantAssociation": {
+        "DeleteAssistantAssociation": {
             "access_level": "Undocumented",
-            "action": "GetAssistantAssociation",
+            "action": "DeleteAssistantAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateKnowledgeBaseTemplateUri": {
+        "NotifyRecommendationsReceived": {
             "access_level": "Undocumented",
-            "action": "UpdateKnowledgeBaseTemplateUri",
+            "action": "NotifyRecommendationsReceived",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateAssistantAssociation": {
+        "ListQuickResponses": {
             "access_level": "Undocumented",
-            "action": "CreateAssistantAssociation",
+            "action": "ListQuickResponses",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateKnowledgeBase": {
+        "ListKnowledgeBases": {
             "access_level": "Undocumented",
-            "action": "CreateKnowledgeBase",
+            "action": "ListKnowledgeBases",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "DeleteImportJob": {
+        "UntagResource": {
             "access_level": "Undocumented",
-            "action": "DeleteImportJob",
+            "action": "UntagResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListContents": {
+        "QueryAssistant": {
             "access_level": "Undocumented",
-            "action": "ListContents",
+            "action": "QueryAssistant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListAssistantAssociations": {
+        "CreateAssistantAssociation": {
             "access_level": "Undocumented",
-            "action": "ListAssistantAssociations",
+            "action": "CreateAssistantAssociation",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "NotifyRecommendationsReceived": {
+        "UpdateQuickResponse": {
             "access_level": "Undocumented",
-            "action": "NotifyRecommendationsReceived",
+            "action": "UpdateQuickResponse",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "ListImportJobs": {
+        "UpdateSession": {
             "access_level": "Undocumented",
-            "action": "ListImportJobs",
+            "action": "UpdateSession",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UntagResource": {
+        "GetKnowledgeBase": {
             "access_level": "Undocumented",
-            "action": "UntagResource",
+            "action": "GetKnowledgeBase",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateContent": {
+        "ListImportJobs": {
             "access_level": "Undocumented",
-            "action": "CreateContent",
+            "action": "ListImportJobs",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "UpdateContent": {
+        "ListTagsForResource": {
             "access_level": "Undocumented",
-            "action": "UpdateContent",
+            "action": "ListTagsForResource",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "StartImportJob": {
+        "DeleteAssistant": {
             "access_level": "Undocumented",
-            "action": "StartImportJob",
+            "action": "DeleteAssistant",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "CreateQuickResponse": {
+        "RemoveKnowledgeBaseTemplateUri": {
             "access_level": "Undocumented",
-            "action": "CreateQuickResponse",
+            "action": "RemoveKnowledgeBaseTemplateUri",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "SearchQuickResponses": {
+        "CreateContent": {
             "access_level": "Undocumented",
-            "action": "SearchQuickResponses",
+            "action": "CreateContent",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         },
-        "GetContentSummary": {
+        "StartImportJob": {
             "access_level": "Undocumented",
-            "action": "GetContentSummary",
+            "action": "StartImportJob",
             "condition_keys": [],
             "description": "Not Documented by AWS",
             "orphan": false,
             "resources": []
         }
     },
     "workdocs": {
```

### Comparing `iam_actions-1.2.20240413/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240414/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240413/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240414/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240413/iam_actions/generate/generate.py` & `iam_actions-1.2.20240414/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240413/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240414/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240413/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240414/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240413/iam_actions/generate/services.py` & `iam_actions-1.2.20240414/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240413/iam_actions/policies.json` & `iam_actions-1.2.20240414/iam_actions/policies.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240413/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240414/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240413/iam_actions/services.json` & `iam_actions-1.2.20240414/iam_actions/services.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240413/pyproject.toml` & `iam_actions-1.2.20240414/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240413"
+version = "1.2.20240414"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240413/setup.py` & `iam_actions-1.2.20240414/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240413',
+    'version': '1.2.20240414',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240413/PKG-INFO` & `iam_actions-1.2.20240414/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240413
+Version: 1.2.20240414
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

