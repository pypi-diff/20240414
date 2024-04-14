# Comparing `tmp/kubescaler-0.0.19.tar.gz` & `tmp/kubescaler-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubescaler-0.0.19.tar", last modified: Tue Mar 26 18:44:56 2024, max compression
+gzip compressed data, was "kubescaler-0.0.2.tar", last modified: Sun Apr 14 21:19:53 2024, max compression
```

## Comparing `kubescaler-0.0.19.tar` & `kubescaler-0.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:44:56.487145 kubescaler-0.0.19/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-26 18:44:09.000000 kubescaler-0.0.19/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-26 18:44:09.000000 kubescaler-0.0.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-26 18:44:09.000000 kubescaler-0.0.19/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-26 18:44:09.000000 kubescaler-0.0.19/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-03-26 18:44:56.487145 kubescaler-0.0.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-03-26 18:44:09.000000 kubescaler-0.0.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:44:56.483145 kubescaler-0.0.19/kubescaler/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-26 18:44:09.000000 kubescaler-0.0.19/kubescaler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-03-26 18:44:09.000000 kubescaler-0.0.19/kubescaler/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-03-26 18:44:09.000000 kubescaler-0.0.19/kubescaler/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-26 18:44:09.000000 kubescaler-0.0.19/kubescaler/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-03-26 18:44:09.000000 kubescaler-0.0.19/kubescaler/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:44:56.483145 kubescaler-0.0.19/kubescaler/scaler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 18:44:09.000000 kubescaler-0.0.19/kubescaler/scaler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:44:56.487145 kubescaler-0.0.19/kubescaler/scaler/aws/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-26 18:44:09.000000 kubescaler-0.0.19/kubescaler/scaler/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-26 18:44:09.000000 kubescaler-0.0.19/kubescaler/scaler/aws/ami.py
--rw-r--r--   0 runner    (1001) docker     (127)    49110 2024-03-26 18:44:09.000000 kubescaler-0.0.19/kubescaler/scaler/aws/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-03-26 18:44:09.000000 kubescaler-0.0.19/kubescaler/scaler/aws/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-03-26 18:44:09.000000 kubescaler-0.0.19/kubescaler/scaler/aws/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    16462 2024-03-26 18:44:09.000000 kubescaler-0.0.19/kubescaler/scaler/google.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:44:56.487145 kubescaler-0.0.19/kubescaler/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-26 18:44:09.000000 kubescaler-0.0.19/kubescaler/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-03-26 18:44:09.000000 kubescaler-0.0.19/kubescaler/utils/fileio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-03-26 18:44:09.000000 kubescaler-0.0.19/kubescaler/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-03-26 18:44:09.000000 kubescaler-0.0.19/kubescaler/utils/terminal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-03-26 18:44:09.000000 kubescaler-0.0.19/kubescaler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 18:44:56.483145 kubescaler-0.0.19/kubescaler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4366 2024-03-26 18:44:56.000000 kubescaler-0.0.19/kubescaler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-26 18:44:56.000000 kubescaler-0.0.19/kubescaler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 18:44:56.000000 kubescaler-0.0.19/kubescaler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 18:44:56.000000 kubescaler-0.0.19/kubescaler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-26 18:44:56.000000 kubescaler-0.0.19/kubescaler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-26 18:44:56.000000 kubescaler-0.0.19/kubescaler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-26 18:44:09.000000 kubescaler-0.0.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-26 18:44:56.487145 kubescaler-0.0.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-03-26 18:44:09.000000 kubescaler-0.0.19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:19:53.330944 kubescaler-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-14 21:19:15.000000 kubescaler-0.0.2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-14 21:19:15.000000 kubescaler-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-14 21:19:15.000000 kubescaler-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-14 21:19:15.000000 kubescaler-0.0.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-14 21:19:53.330944 kubescaler-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-14 21:19:15.000000 kubescaler-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:19:53.326944 kubescaler-0.0.2/kubescaler/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-14 21:19:15.000000 kubescaler-0.0.2/kubescaler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-14 21:19:15.000000 kubescaler-0.0.2/kubescaler/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-14 21:19:15.000000 kubescaler-0.0.2/kubescaler/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-14 21:19:15.000000 kubescaler-0.0.2/kubescaler/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6109 2024-04-14 21:19:15.000000 kubescaler-0.0.2/kubescaler/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:19:53.330944 kubescaler-0.0.2/kubescaler/scaler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 21:19:15.000000 kubescaler-0.0.2/kubescaler/scaler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:19:53.330944 kubescaler-0.0.2/kubescaler/scaler/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-14 21:19:15.000000 kubescaler-0.0.2/kubescaler/scaler/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-14 21:19:15.000000 kubescaler-0.0.2/kubescaler/scaler/aws/ami.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49110 2024-04-14 21:19:15.000000 kubescaler-0.0.2/kubescaler/scaler/aws/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-14 21:19:15.000000 kubescaler-0.0.2/kubescaler/scaler/aws/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-14 21:19:15.000000 kubescaler-0.0.2/kubescaler/scaler/aws/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18258 2024-04-14 21:19:15.000000 kubescaler-0.0.2/kubescaler/scaler/google.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:19:53.330944 kubescaler-0.0.2/kubescaler/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-14 21:19:15.000000 kubescaler-0.0.2/kubescaler/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-04-14 21:19:15.000000 kubescaler-0.0.2/kubescaler/utils/fileio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-14 21:19:15.000000 kubescaler-0.0.2/kubescaler/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-14 21:19:15.000000 kubescaler-0.0.2/kubescaler/utils/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-14 21:19:15.000000 kubescaler-0.0.2/kubescaler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:19:53.326944 kubescaler-0.0.2/kubescaler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-04-14 21:19:53.000000 kubescaler-0.0.2/kubescaler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-14 21:19:53.000000 kubescaler-0.0.2/kubescaler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:19:53.000000 kubescaler-0.0.2/kubescaler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:19:53.000000 kubescaler-0.0.2/kubescaler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-14 21:19:53.000000 kubescaler-0.0.2/kubescaler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-14 21:19:53.000000 kubescaler-0.0.2/kubescaler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-14 21:19:15.000000 kubescaler-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-14 21:19:53.330944 kubescaler-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-14 21:19:15.000000 kubescaler-0.0.2/setup.py
```

### Comparing `kubescaler-0.0.19/LICENSE` & `kubescaler-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.19/NOTICE` & `kubescaler-0.0.2/NOTICE`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.19/PKG-INFO` & `kubescaler-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubescaler
-Version: 0.0.19
+Version: 0.0.2
 Summary: Helper classes for scaling Kubernetes clusters
 Home-page: https://github.com/converged-computing/kubescaler
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: Kubernetes,elasticity,scaling,EKS,GKE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kubescaler Version: 0.0.19 Summary: Helper classes
+Metadata-Version: 2.1 Name: kubescaler Version: 0.0.2 Summary: Helper classes
 for scaling Kubernetes clusters Home-page: https://github.com/converged-
 computing/kubescaler Author: Vanessa Sochat Author-email:
 vsoch@users.noreply.github.com Maintainer: Vanessa Sochat License: LICENSE
 Keywords: Kubernetes,elasticity,scaling,EKS,GKE Classifier: Intended Audience
 :: Science/Research Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Topic :: Software Development Classifier: Topic ::
```

### Comparing `kubescaler-0.0.19/README.md` & `kubescaler-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.19/kubescaler/cluster.py` & `kubescaler-0.0.2/kubescaler/cluster.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.19/kubescaler/decorators.py` & `kubescaler-0.0.2/kubescaler/decorators.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.19/kubescaler/defaults.py` & `kubescaler-0.0.2/kubescaler/defaults.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.19/kubescaler/logger.py` & `kubescaler-0.0.2/kubescaler/logger.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.19/kubescaler/scaler/aws/ami.py` & `kubescaler-0.0.2/kubescaler/scaler/aws/ami.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.19/kubescaler/scaler/aws/cluster.py` & `kubescaler-0.0.2/kubescaler/scaler/aws/cluster.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.19/kubescaler/scaler/aws/template.py` & `kubescaler-0.0.2/kubescaler/scaler/aws/template.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.19/kubescaler/scaler/aws/token.py` & `kubescaler-0.0.2/kubescaler/scaler/aws/token.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.19/kubescaler/scaler/google.py` & `kubescaler-0.0.2/kubescaler/scaler/google.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         # Set the zone for a more scoped request
         zone="us-central1-a",
         spot=False,
         max_vcpu=8,
         max_memory=32,
         # Initial labels for the default cluster
         labels=None,
+        scaling_profile=0,
         **kwargs,
     ):
         """
         A simple class to control creating a cluster
         """
         super().__init__(**kwargs)
 
@@ -52,14 +53,15 @@
         print("⭐️ Creating global cluster manager client...")
         self.client = container_v1.ClusterManagerClient()
         self.project = project
         self.machine_type = self.machine_type or "c2-standard-8"
         self.tags = self.tags or ["kubescaler-cluster"]
         self.default_pool = default_pool_name
         self.configuration = None
+        self.scaling_profile = scaling_profile
         self.labels = labels
         self.zone = zone
         self.max_vcpu = max_vcpu
         self.max_memory = max_memory
         self.spot = False
 
     @timed
@@ -303,46 +305,62 @@
         """
         node_pool = name or self.default_pool
         name = f"{self.cluster_name}/nodePools/{node_pool}"
         request = container_v1.DeleteNodePoolRequest(name=name)
         self.client.delete_node_pool(request=request)
         return self.wait_for_status(2)
 
-    def get_cluster(self, node_pools=None):
+    def get_cluster(self, node_pools=None, scaling_profile=None):
         """
         Get the cluster proto with our defaults
         """
+        if scaling_profile is None:
+            scaling_profile = self.scaling_profile
+        if scaling_profile not in [0, 1, 2]:
+            raise ValueError("Scaling profile must be one of 0,1,2")
+
+        # autoprovisioning node defaults. Note that upgrade settings
+        # default to a surge strategy, max surge 1 and nodes unavailable 2
+        # I tried setting auto_upgrade and auto_repair to False but that
+        # must be the default, they don't show up
+
         # Design our initial cluster!
         # Autoscaling - try optimizing
         # PROFILE_UNSPECIFIED = 0
         # OPTIMIZE_UTILIZATION = 1
         # BALANCED = 2
-        autoscaling_profile = container_v1.ClusterAutoscaling.AutoscalingProfile(1)
+        autoscaling_profile = container_v1.ClusterAutoscaling.AutoscalingProfile(
+            scaling_profile
+        )
 
-        # These are required, you get an error without them.
+        # These are only intended if you want GKE to make new node pools for you
+        # I highly do not recommend this, I've never had this result in desired
+        # behavior.
         # https://cloud.google.com/compute/docs/compute-optimized-machines
-        resource_limits = [
-            container_v1.ResourceLimit(
-                resource_type="cpu",
-                minimum=0,
-                maximum=self.max_vcpu * self.node_count,
-            ),
-            container_v1.ResourceLimit(
-                resource_type="memory",
-                minimum=0,
-                maximum=self.max_memory * self.node_count,
-            ),
-        ]
+        # resource_limits = [
+        #    container_v1.ResourceLimit(
+        #        resource_type="cpu",
+        #        minimum=0,
+        #        maximum=self.max_vcpu * self.node_count,
+        #    ),
+        #    container_v1.ResourceLimit(
+        #        resource_type="memory",
+        #        minimum=0,
+        #        maximum=self.max_memory * self.node_count,
+        #    ),
+        # ]
 
-        # Note that I removed resource_limits, no limits!
+        # When autoprovisioning is enabled the cluster explodes into much
+        # larger sizes than you want.
         cluster_autoscaling = container_v1.ClusterAutoscaling(
-            enable_node_autoprovisioning=True,
-            autoprovisioning_locations=[self.zone],
+            enable_node_autoprovisioning=False,
             autoscaling_profile=autoscaling_profile,
-            resource_limits=resource_limits,
+            # These two fields are only for node autoprovisioning
+            # autoprovisioning_locations=[self.location],
+            # resource_limits=resource_limits,
         )
 
         # vertical_pod_autoscaling (google.cloud.container_v1.types.VerticalPodAutoscaling):
         #  Cluster-level Vertical Pod Autoscaling
         #  configuration.
         cluster = container_v1.Cluster(
             name=self.name,
@@ -362,14 +380,38 @@
             cluster.node_config = node_config
 
         print("\n🥣️ cluster spec")
         print(cluster)
         return cluster
 
     @timed
+    def update_cluster(self, size, max_nodes, min_nodes):
+        """
+        Update a cluster. Currently we support the max and min size
+        """
+        autoscaling = container_v1.NodePoolAutoscaling(
+            enabled=True,
+            total_max_node_count=max_nodes,
+            total_min_node_count=min_nodes,
+        )
+        request = container_v1.SetNodePoolAutoscalingRequest(
+            autoscaling=autoscaling,
+            name=f"projects/{self.project}/locations/{self.location}/clusters/{self.name}/nodePools/{self.default_pool}",
+        )
+        print("\n🥣️ cluster node pool update request")
+        print(request)
+
+        response = self.client.set_node_pool_autoscaling(request=request)
+        print(response)
+
+        # Status 2 is running (1 is provisioning)
+        print(f"⏱️   Waiting for {self.cluster_name} to be ready...")
+        return self.wait_for_status(2)
+
+    @timed
     def create_cluster(self):
         """
         Create a cluster, with hard coded variables for now.
 
         Since we can't create an empty cluster, and the API doesn't allow you
         to create one from scratch setting a min/max count, what we are going
         to do is create the NodePool (with our preferences) first, and then
@@ -378,16 +420,16 @@
         node_config = self.get_node_config(
             self.machine_type, spot=self.spot, labels=self.labels
         )
 
         # If you don't set this, your cluster will grow as it pleases.
         autoscaling = container_v1.NodePoolAutoscaling(
             enabled=True,
-            min_node_count=self.min_nodes,
-            max_node_count=self.max_nodes,
+            total_max_node_count=self.max_nodes,
+            total_min_node_count=self.min_nodes,
         )
         node_pool = container_v1.types.NodePool(
             name=self.default_pool,
             config=node_config,
             initial_node_count=self.node_count,
             autoscaling=autoscaling,
             # not specifying network_config uses cluster defaults
```

### Comparing `kubescaler-0.0.19/kubescaler/utils/fileio.py` & `kubescaler-0.0.2/kubescaler/utils/fileio.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.19/kubescaler/utils/misc.py` & `kubescaler-0.0.2/kubescaler/utils/misc.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.19/kubescaler/utils/terminal.py` & `kubescaler-0.0.2/kubescaler/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.19/kubescaler/version.py` & `kubescaler-0.0.2/kubescaler/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2023-2024 Lawrence Livermore National Security, LLC and other
 # HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (MIT)
 
-__version__ = "0.0.19"
+__version__ = "0.0.2"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "kubescaler"
 PACKAGE_URL = "https://github.com/converged-computing/kubescaler"
 KEYWORDS = "Kubernetes, elasticity, scaling, EKS, GKE"
 DESCRIPTION = "Helper classes for scaling Kubernetes clusters"
 LICENSE = "LICENSE"
```

### Comparing `kubescaler-0.0.19/kubescaler.egg-info/PKG-INFO` & `kubescaler-0.0.2/kubescaler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubescaler
-Version: 0.0.19
+Version: 0.0.2
 Summary: Helper classes for scaling Kubernetes clusters
 Home-page: https://github.com/converged-computing/kubescaler
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: Kubernetes,elasticity,scaling,EKS,GKE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kubescaler Version: 0.0.19 Summary: Helper classes
+Metadata-Version: 2.1 Name: kubescaler Version: 0.0.2 Summary: Helper classes
 for scaling Kubernetes clusters Home-page: https://github.com/converged-
 computing/kubescaler Author: Vanessa Sochat Author-email:
 vsoch@users.noreply.github.com Maintainer: Vanessa Sochat License: LICENSE
 Keywords: Kubernetes,elasticity,scaling,EKS,GKE Classifier: Intended Audience
 :: Science/Research Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python Classifier: Topic :: Software Development Classifier: Topic ::
```

### Comparing `kubescaler-0.0.19/kubescaler.egg-info/SOURCES.txt` & `kubescaler-0.0.2/kubescaler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kubescaler-0.0.19/setup.py` & `kubescaler-0.0.2/setup.py`

 * *Files identical despite different names*

