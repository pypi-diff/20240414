# Comparing `tmp/ecomplexity-0.5.2.tar.gz` & `tmp/ecomplexity-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ecomplexity-0.5.2.tar", last modified: Fri Oct 23 03:32:40 2020, max compression
+gzip compressed data, was "ecomplexity-0.5.3.tar", last modified: Sun Apr 14 10:24:39 2024, max compression
```

## Comparing `ecomplexity-0.5.2.tar` & `ecomplexity-0.5.3.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 shg309   (458091743) 937845540        0 2020-10-23 03:32:40.000000 ecomplexity-0.5.2/
--rw-r--r--   0 shg309   (458091743) 937845540     4642 2020-10-23 03:32:40.000000 ecomplexity-0.5.2/PKG-INFO
-drwxr-xr-x   0 shg309   (458091743) 937845540        0 2020-10-23 03:32:40.000000 ecomplexity-0.5.2/ecomplexity/
--rw-r--r--   0 shg309   (458091743) 937845540     1270 2020-10-22 23:04:30.000000 ecomplexity-0.5.2/ecomplexity/calc_proximity.py
--rw-r--r--   0 shg309   (458091743) 937845540     6593 2020-10-22 23:04:30.000000 ecomplexity-0.5.2/ecomplexity/ComplexityData.py
--rw-r--r--   0 shg309   (458091743) 937845540     8400 2020-10-23 03:27:03.000000 ecomplexity-0.5.2/ecomplexity/ecomplexity.py
--rw-r--r--   0 shg309   (458091743) 937845540      114 2020-10-22 23:04:30.000000 ecomplexity-0.5.2/ecomplexity/__init__.py
--rw-r--r--   0 shg309   (458091743) 937845540      840 2020-10-22 23:04:30.000000 ecomplexity-0.5.2/ecomplexity/density.py
--rw-r--r--   0 shg309   (458091743) 937845540      770 2020-10-22 23:04:30.000000 ecomplexity-0.5.2/ecomplexity/coicog.py
--rw-r--r--   0 shg309   (458091743) 937845540     4082 2020-10-22 23:04:30.000000 ecomplexity-0.5.2/ecomplexity/proximity.py
-drwxr-xr-x   0 shg309   (458091743) 937845540        0 2020-10-23 03:32:40.000000 ecomplexity-0.5.2/ecomplexity.egg-info/
--rw-r--r--   0 shg309   (458091743) 937845540     4642 2020-10-23 03:32:40.000000 ecomplexity-0.5.2/ecomplexity.egg-info/PKG-INFO
--rw-r--r--   0 shg309   (458091743) 937845540        1 2019-04-03 02:09:50.000000 ecomplexity-0.5.2/ecomplexity.egg-info/not-zip-safe
--rw-r--r--   0 shg309   (458091743) 937845540      419 2020-10-23 03:32:40.000000 ecomplexity-0.5.2/ecomplexity.egg-info/SOURCES.txt
--rw-r--r--   0 shg309   (458091743) 937845540       27 2020-10-23 03:32:40.000000 ecomplexity-0.5.2/ecomplexity.egg-info/requires.txt
--rw-r--r--   0 shg309   (458091743) 937845540       12 2020-10-23 03:32:40.000000 ecomplexity-0.5.2/ecomplexity.egg-info/top_level.txt
--rw-r--r--   0 shg309   (458091743) 937845540        1 2020-10-23 03:32:40.000000 ecomplexity-0.5.2/ecomplexity.egg-info/dependency_links.txt
--rw-r--r--   0 shg309   (458091743) 937845540       18 2018-11-14 18:42:11.000000 ecomplexity-0.5.2/MANIFEST.in
--rw-r--r--   0 shg309   (458091743) 937845540     3515 2020-10-23 00:03:05.000000 ecomplexity-0.5.2/README.md
--rw-r--r--   0 shg309   (458091743) 937845540      857 2020-10-23 03:30:44.000000 ecomplexity-0.5.2/setup.py
--rw-r--r--   0 shg309   (458091743) 937845540       38 2020-10-23 03:32:40.000000 ecomplexity-0.5.2/setup.cfg
+drwxr-xr-x   0 shg309     (502) staff       (20)        0 2024-04-14 10:24:39.603449 ecomplexity-0.5.3/
+-rw-r--r--   0 shg309     (502) staff       (20)     1647 2024-04-14 10:04:33.000000 ecomplexity-0.5.3/.gitignore
+-rw-r--r--   0 shg309     (502) staff       (20)     1125 2018-10-24 19:24:11.000000 ecomplexity-0.5.3/LICENSE
+-rw-r--r--   0 shg309     (502) staff       (20)       18 2018-11-14 18:42:11.000000 ecomplexity-0.5.3/MANIFEST.in
+-rw-r--r--   0 shg309     (502) staff       (20)     5090 2024-04-14 10:24:39.603188 ecomplexity-0.5.3/PKG-INFO
+-rw-r--r--   0 shg309     (502) staff       (20)     4449 2024-04-14 10:11:14.000000 ecomplexity-0.5.3/README.md
+drwxr-xr-x   0 shg309     (502) staff       (20)        0 2024-04-14 10:24:39.600780 ecomplexity-0.5.3/ecomplexity/
+-rw-r--r--   0 shg309     (502) staff       (20)     6512 2023-04-26 14:41:38.000000 ecomplexity-0.5.3/ecomplexity/ComplexityData.py
+-rw-r--r--   0 shg309     (502) staff       (20)      114 2020-10-22 23:04:30.000000 ecomplexity-0.5.3/ecomplexity/__init__.py
+-rw-r--r--   0 shg309     (502) staff       (20)     2135 2023-04-17 17:13:48.000000 ecomplexity-0.5.3/ecomplexity/calc_density.py
+-rw-r--r--   0 shg309     (502) staff       (20)     1270 2020-10-22 23:04:30.000000 ecomplexity-0.5.3/ecomplexity/calc_proximity.py
+-rw-r--r--   0 shg309     (502) staff       (20)      770 2020-10-22 23:04:30.000000 ecomplexity-0.5.3/ecomplexity/coicog.py
+-rw-r--r--   0 shg309     (502) staff       (20)    14391 2024-04-13 23:43:37.000000 ecomplexity-0.5.3/ecomplexity/ecomplexity.py
+-rw-r--r--   0 shg309     (502) staff       (20)     6572 2024-04-13 23:39:13.000000 ecomplexity-0.5.3/ecomplexity/log_supermodularity.py
+-rw-r--r--   0 shg309     (502) staff       (20)     4103 2023-04-26 14:47:38.000000 ecomplexity-0.5.3/ecomplexity/proximity.py
+drwxr-xr-x   0 shg309     (502) staff       (20)        0 2024-04-14 10:24:39.602742 ecomplexity-0.5.3/ecomplexity.egg-info/
+-rw-r--r--   0 shg309     (502) staff       (20)     5090 2024-04-14 10:24:39.000000 ecomplexity-0.5.3/ecomplexity.egg-info/PKG-INFO
+-rw-r--r--   0 shg309     (502) staff       (20)      495 2024-04-14 10:24:39.000000 ecomplexity-0.5.3/ecomplexity.egg-info/SOURCES.txt
+-rw-r--r--   0 shg309     (502) staff       (20)        1 2024-04-14 10:24:39.000000 ecomplexity-0.5.3/ecomplexity.egg-info/dependency_links.txt
+-rw-r--r--   0 shg309     (502) staff       (20)        1 2019-04-03 02:09:50.000000 ecomplexity-0.5.3/ecomplexity.egg-info/not-zip-safe
+-rw-r--r--   0 shg309     (502) staff       (20)       46 2024-04-14 10:24:39.000000 ecomplexity-0.5.3/ecomplexity.egg-info/requires.txt
+-rw-r--r--   0 shg309     (502) staff       (20)       12 2024-04-14 10:24:39.000000 ecomplexity-0.5.3/ecomplexity.egg-info/top_level.txt
+-rw-r--r--   0 shg309     (502) staff       (20)       47 2023-01-26 17:51:59.000000 ecomplexity-0.5.3/requirements.txt
+-rw-r--r--   0 shg309     (502) staff       (20)       38 2024-04-14 10:24:39.603505 ecomplexity-0.5.3/setup.cfg
+-rw-r--r--   0 shg309     (502) staff       (20)      964 2024-04-14 10:24:33.000000 ecomplexity-0.5.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ecomplexity-0.5.2/PKG-INFO` & `ecomplexity-0.5.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,107 @@
 Metadata-Version: 2.1
 Name: ecomplexity
-Version: 0.5.2
+Version: 0.5.3
 Summary: Package to calculate economic complexity and associated variables
 Home-page: https://github.com/cid-harvard/py-ecomplexity
 Author: Shreyas Gadgin Matha
 Author-email: shreyas.gm61@gmail.com
 License: MIT
-Description: # Economic Complexity and Product Complexity
-        ## by the Growth Lab at Harvard's Center for International Development
-        This package is part of Harvard Growth Lab’s portfolio of software packages, digital products and interactive data visualizations. To browse our entire portfolio, please visit growthlab.app. To learn more about our research, please visit [Harvard Growth Lab’s home page](https://growthlab.cid.harvard.edu/).
-        
-        # About
-        Python package to calculate economic complexity indices.
-        
-        STATA implementation of the economic complexity index available at: <https://github.com/cid-harvard/ecomplexity>
-        
-        Explore complexity and associated data using Harvard CID's Atlas tool: <http://atlas.cid.harvard.edu>
-        
-        ## Tutorial
-        
-        **Installation**:
-        At terminal: `pip install ecomplexity`
-        
-        **Usage**:
-        
-        ```python
-        from ecomplexity import ecomplexity
-        from ecomplexity import proximity
-        
-        # Import trade data from CID Atlas
-        data_url = "https://intl-atlas-downloads.s3.amazonaws.com/country_hsproduct2digit_year.csv.zip"
-        data = pd.read_csv(data_url, compression="zip", low_memory=False)
-        data = data[['year','location_code','hs_product_code','export_value']]
-        
-        # Calculate complexity
-        trade_cols = {'time':'year', 'loc':'location_code', 'prod':'hs_product_code', 'val':'export_value'}
-        cdata = ecomplexity(data, trade_cols)
-        
-        # Calculate proximity matrix
-        prox_df = proximity(data, trade_cols)
-        ```
-        
-        **Arguments**:
-        
-        ```text
-        data: pandas dataframe containing production / trade data.
-            Including variables indicating time, location, product and value
-        cols_input: dict of column names for time, location, product and value.
-            Example: {'time':'year', 'loc':'origin', 'prod':'hs92', 'val':'export_val'}
-        presence_test: str for test used for presence of industry in location.
-            One of "rca" (default), "rpop", "both", or "manual".
-            Determines which values are used for M_cp calculations.
-            If "manual", M_cp is taken as given from the "value" column in data
-        val_errors_flag: {'coerce','ignore','raise'}. Passed to pd.to_numeric
-            *default* coerce.
-        rca_mcp_threshold: numeric indicating RCA threshold beyond which mcp is 1.
-            *default* 1.
-        rpop_mcp_threshold: numeric indicating RPOP threshold beyond which mcp is 1.
-            *default* 1. Only used if presence_test is not "rca".
-        pop: pandas df, with time, location and corresponding population, in that order.
-            Not required if presence_test is "rca" (default).
-        continuous: Used to calculate product proximities, indicates whether
-            to consider correlation of every product pair (True) or product
-            co-occurrence (False). *default* False.
-        asymmetric: Used to calculate product proximities, indicates whether
-            to generate asymmetric proximity matrix (True) or symmetric (False).
-            *default* False.
-        ```
-        
-        ### TODO
-        
-        - There are very minor differences in the values of density, COI and COG between STATA and Python due to the way matrix computations are handled by the two. These should be aligned in the future.
-        - knn options for density: in the future, allow knn parameter for density calculation
-        
-        ### References
-        
-        - Hausmann, R., Hidalgo, C. A., Bustos, S., Coscia, M., Simoes, A., & Yıldırım, M. (2013). The Atlas of Economic Complexity: Mapping Paths to Prosperity (Part 1). Retrieved from <https://growthlab.cid.harvard.edu/files/growthlab/files/atlas_2013_part1.pdf>
-        - Hidalgo, C. A., Klinger, B., Barabasi, A.-L., & Hausmann, R. (2007). The Product Space Conditions the Development of Nations. Science, 317(5837), 482–487. <http://doi.org/10.1126/science.1144581>
-        
 Keywords: pandas python networks economics complexity
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pandas>0.23.0
+Requires-Dist: numpy>1.22.0
+Requires-Dist: scikit-learn>1.0.0
+
+# Economic Complexity and Product Complexity
+
+By the Growth Lab at Harvard's Center for International Development
+
+This package is part of Harvard Growth Lab’s portfolio of software packages, digital products and interactive data visualizations. To browse our entire portfolio, please visit [growthlab.app](growthlab.app). To learn more about our research, please visit [Harvard Growth Lab’s home page](https://growthlab.cid.harvard.edu/).
+
+# About
+Python package to calculate economic complexity indices.
+
+STATA implementation of the economic complexity index available at: <https://github.com/cid-harvard/ecomplexity>
+
+Explore complexity and associated data using Harvard CID's Atlas tool: <http://atlas.cid.harvard.edu>
+
+## Tutorial
+
+**Installation**:
+For the latest stable version: `pip install ecomplexity`
+
+Latest version of the package under development (untested and possibly with bugs), install directly from GitHub:
+`pip install git+https://github.com/cid-harvard/py-ecomplexity@develop`
+
+**Usage**:
+
+```python
+from ecomplexity import ecomplexity
+from ecomplexity import proximity
+
+# Import trade data from CID Atlas
+data_url = "https://intl-atlas-downloads.s3.amazonaws.com/country_hsproduct2digit_year.csv.zip"
+data = pd.read_csv(data_url, compression="zip", low_memory=False)
+data = data[['year','location_code','hs_product_code','export_value']]
+
+# Calculate complexity
+trade_cols = {'time':'year', 'loc':'location_code', 'prod':'hs_product_code', 'val':'export_value'}
+cdata = ecomplexity(data, trade_cols)
+
+# Calculate proximity matrix
+prox_df = proximity(data, trade_cols)
+```
+
+**Arguments**:
+
+```text
+data: pandas dataframe containing production / trade data.
+    Including variables indicating time, location, product and value
+cols_input: dict of column names for time, location, product and value.
+    Example: {'time':'year', 'loc':'origin', 'prod':'hs92', 'val':'export_val'}
+presence_test: str for test used for presence of industry in location.
+    One of "rca" (default), "rpop", or "manual".
+    Determines which values are used for M_cp calculations.
+    If "manual", M_cp is taken as given from the "value" column in data
+val_errors_flag: {'coerce','ignore','raise'}. Passed to pd.to_numeric
+    *default* coerce.
+rca_mcp_threshold: numeric indicating RCA threshold beyond which mcp is 1.
+    *default* 1.
+rpop_mcp_threshold: numeric indicating RPOP threshold beyond which mcp is 1.
+    *default* 1. Only used if presence_test is not "rca".
+pop: pandas df, with time, location and corresponding population, in that order.
+    Not required if presence_test is "rca", which is the default.
+continuous: Used to calculate product proximities, indicates whether
+    to consider correlation of every product pair (True) or product
+    co-occurrence (False). *default* False.
+asymmetric: Used to calculate product proximities, indicates whether
+    to generate asymmetric proximity matrix (True) or symmetric (False).
+    *default* False.
+proximity_edgelist: pandas df with cols 'prod1', 'prod2', 'proximity'.
+    If None (default), proximity values are calculated from data.
+knn: Number of nearest neighbors from proximity matrix to use to calculate
+    density. Will use entire proximity matrix if None.
+    *default* None.
+check_logsupermodularity: If True (default), check log-supermodularity.
+    If int, use roughly that many samples to check log-supermodularity.
+report_logsupermodularity: If True, print warning if log-supermodularity.
+    If False (default), don't.
+verbose: Print year being processed
+```
+
+## FAQ
+
+- Why are ECI and PCI are both normalized using ECI's mean and std. dev?
+    + This normalization preserves the property that ECI = (mean of PCI of products for which MCP=1)
+- What is log-supermodularity?
+    + Refer `ecomplexity/log_supermodularity.py` for a brief explanation. More at Schetter, U. (2019). A Structural Ranking of Economic Complexity (SSRN Scholarly Paper 3485842). https://doi.org/10.2139/ssrn.3485842.
+
+### References
+
+- Hausmann, R., Hidalgo, C. A., Bustos, S., Coscia, M., Simoes, A., & Yıldırım, M. (2013). The Atlas of Economic Complexity: Mapping Paths to Prosperity (Part 1). Retrieved from <https://growthlab.cid.harvard.edu/files/growthlab/files/atlas_2013_part1.pdf>
+- Hidalgo, C. A., Klinger, B., Barabasi, A.-L., & Hausmann, R. (2007). The Product Space Conditions the Development of Nations. Science, 317(5837), 482–487. <http://doi.org/10.1126/science.1144581>
```

### Comparing `ecomplexity-0.5.2/ecomplexity/calc_proximity.py` & `ecomplexity-0.5.3/ecomplexity/calc_proximity.py`

 * *Files identical despite different names*

### Comparing `ecomplexity-0.5.2/ecomplexity/ComplexityData.py` & `ecomplexity-0.5.3/ecomplexity/ComplexityData.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,33 +53,38 @@
         if dups.sum() > 0:
             warnings.warn("Duplicate values exist, keeping the first occurrence")
             self.data = self.data[~self.data.index.duplicated()]
 
     def create_full_df(self, t):
         """Rectangularize, but remove rows with diversity or ubiquity zero
 
-        Rows with zero diversity / ubiquity lead to dividebyzero errors and
-        incorrect values during normzalization
+        Rows with zero diversity / ubiquity lead to ZeroDivision errors and
+        incorrect values during normalization
         """
         self.t = t
         self.data_t = self.data.loc[t].copy()
-        diversity_check = (
+        # Check for zero diversity and ubiquity
+        val_diversity_check = (
             self.data_t.reset_index().groupby(["loc"])["val"].sum().reset_index()
         )
-        ubiquity_check = (
+        val_ubiquity_check = (
             self.data_t.reset_index().groupby(["prod"])["val"].sum().reset_index()
         )
-        diversity_check = diversity_check[diversity_check.val != 0]
-        ubiquity_check = ubiquity_check[ubiquity_check.val != 0]
+        val_diversity_check = val_diversity_check[val_diversity_check.val != 0]
+        val_ubiquity_check = val_ubiquity_check[val_ubiquity_check.val != 0]
+        # Remove locations and products with zero diversity and ubiquity respectively
         self.data_t = self.data_t.reset_index()
-        self.data_t = self.data_t.merge(diversity_check[["loc"]], on="loc", how="right")
         self.data_t = self.data_t.merge(
-            ubiquity_check[["prod"]], on="prod", how="right"
+            val_diversity_check[["loc"]], on="loc", how="right"
+        )
+        self.data_t = self.data_t.merge(
+            val_ubiquity_check[["prod"]], on="prod", how="right"
         )
         self.data_t.set_index(["loc", "prod"], inplace=True)
+        # Create full dataframe with all combinations of locations and products
         data_index = pd.MultiIndex.from_product(
             self.data_t.index.levels, names=self.data_t.index.names
         )
         self.data_t = self.data_t.reindex(data_index, fill_value=0)
 
     def calculate_rca(self):
         """Calculate RCA"""
@@ -144,23 +149,15 @@
         elif presence_test == "both":
             self.calculate_rpop(pop, t)
             self.mcp_t = convert_to_binary(
                 self.rca_t, rca_mcp_threshold_input
             ) + convert_to_binary(self.rpop_t, rpop_mcp_threshold_input)
 
     def calculate_manual_mcp(self):
-        """If pre-computed MCP supplied, check validity and reshape"""
-        # Test to see if indeed MCP
-        if np.any(~np.isin(self.data_t.values, [0, 1])):
-            error_val = self.data_t.values[~np.isin(self.data_t.values, [0, 1])].flat[0]
-            raise ValueError(
-                "Manually supplied MCP column contains values other than 0 or 1 - Val: {}".format(
-                    error_val
-                )
-            )
-
+        """If pre-computed MCP supplied, reshape"""
         # Convert data into numpy array
         loc_n_vals = len(self.data_t.index.levels[0])
         prod_n_vals = len(self.data_t.index.levels[1])
         data_np = self.data_t.values.reshape((loc_n_vals, prod_n_vals))
-
+        
+        self.rca_t = data_np
         self.mcp_t = data_np
```

### Comparing `ecomplexity-0.5.2/ecomplexity/coicog.py` & `ecomplexity-0.5.3/ecomplexity/coicog.py`

 * *Files identical despite different names*

### Comparing `ecomplexity-0.5.2/ecomplexity/proximity.py` & `ecomplexity-0.5.3/ecomplexity/proximity.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,50 @@
 import pandas as pd
 import numpy as np
 from ecomplexity.calc_proximity import calc_discrete_proximity
 from ecomplexity.calc_proximity import calc_continuous_proximity
 from ecomplexity.ComplexityData import ComplexityData
 
-def proximity(data, cols_input, presence_test="rca", val_errors_flag='coerce',
-              rca_mcp_threshold=1, rpop_mcp_threshold=1, pop=None,
-              continuous=False, asymmetric=False):
+
+def proximity(
+    data,
+    cols_input,
+    presence_test="rca",
+    val_errors_flag="coerce",
+    rca_mcp_threshold=1,
+    rpop_mcp_threshold=1,
+    pop=None,
+    continuous=False,
+    asymmetric=False,
+):
     """Wrapper function to calculate product proximity matrices
 
-    Args:
-        data: pandas df with cols 'time','loc','prod','val'
-        cols_input: dict of column names for time, location, product and value.
-            Example: {'time':'year', 'loc':'origin', 'prod':'hs92', 'val':'export_val'}
-        presence_test: str for test used for presence of industry in location.
-            One of "rca" (default), "rpop", "both", or "manual".
-            Determines which values are
- used for M_cp calculations.
-            If "manual", M_cp is taken as given from the "value" column in data
-        val_errors_flag: {'coerce','ignore','raise'}. Passed to pd.to_numeric
-            *default* coerce.
-        rca_mcp_threshold: numeric indicating RCA threshold beyond which mcp is 1.
-            *default* 1.
-        rpop_mcp_threshold: numeric indicating RPOP threshold beyond which mcp is 1.
-            *default* 1. Only used if presence_test is not "rca".
-        pop: pandas df, with time, location and corresponding population, in that order.
-            Not required if presence_test is "rca" (default).
-        continuous: Whether to consider correlation of every product pair (True)
-            or product co-occurrence (False). *default* False.
-        asymmetric: Whether to generate asymmetric proximity matrix (True) or
-            symmetric (False). *default* False.
+        Args:
+            data: pandas df with cols 'time','loc','prod','val'
+            cols_input: dict of column names for time, location, product and value.
+                Example: {'time':'year', 'loc':'origin', 'prod':'hs92', 'val':'export_val'}
+            presence_test: str for test used for presence of industry in location.
+                One of "rca" (default), "rpop", "both", or "manual".
+                Determines which values are used for M_cp calculations.
+                If "manual", M_cp is taken as given from the "value" column in data
+            val_errors_flag: {'coerce','ignore','raise'}. Passed to pd.to_numeric
+                *default* coerce.
+            rca_mcp_threshold: numeric indicating RCA threshold beyond which mcp is 1.
+                *default* 1.
+            rpop_mcp_threshold: numeric indicating RPOP threshold beyond which mcp is 1.
+                *default* 1. Only used if presence_test is not "rca".
+            pop: pandas df, with time, location and corresponding population, in that order.
+                Not required if presence_test is "rca" (default).
+            continuous: Whether to consider correlation of every product pair (True)
+                or product co-occurrence (False). *default* False.
+            asymmetric: Whether to generate asymmetric proximity matrix (True) or
+                symmetric (False). *default* False.
 
-    Returns:
-        pandas df with proximity values for every product pair
+        Returns:
+            pandas df with proximity values for every product pair
     """
 
     cdata = ComplexityData(data, cols_input, val_errors_flag)
 
     output_list = []
 
     # Iterate over time stamps
@@ -44,48 +52,56 @@
         print(t)
         # Rectangularize df
         cdata.create_full_df(t)
 
         # Check if Mcp is pre-computed
         if presence_test != "manual":
             cdata.calculate_rca()
-            cdata.calculate_mcp(rca_mcp_threshold, rpop_mcp_threshold,
-                                presence_test, pop, t)
+            cdata.calculate_mcp(
+                rca_mcp_threshold, rpop_mcp_threshold, presence_test, pop, t
+            )
         else:
             cdata.calculate_manual_mcp()
 
         # Calculate diversity and ubiquity
         cdata.diversity_t = np.nansum(cdata.mcp_t, axis=1)
         cdata.ubiquity_t = np.nansum(cdata.mcp_t, axis=0)
 
         # Calculate proximity
-        if continuous==False:
-            prox_mat = calc_discrete_proximity(cdata.mcp_t, cdata.ubiquity_t,
-                                               asymmetric)
-        elif continuous==True and presence_test=="rpop":
+        if continuous == False:
+            prox_mat = calc_discrete_proximity(
+                cdata.mcp_t, cdata.ubiquity_t, asymmetric
+            )
+        elif continuous == True and presence_test == "rpop":
             prox_mat = calc_continuous_proximity(cdata.rpop_t, cdata.ubiquity_t)
-        elif continuous==True and presence_test!="rpop":
+        elif continuous == True and presence_test != "rpop":
             prox_mat = calc_continuous_proximity(cdata.rca_t, cdata.ubiquity_t)
 
         # Reshape as df
-        output_index = pd.MultiIndex.from_product([cdata.data_t.index.levels[1],
-                                                   cdata.data_t.index.levels[1]],
-                                                  names=['prod1','prod2'])
-        output = pd.DataFrame(data={'proximity':prox_mat.ravel()},
-                              index=output_index)
-        output['time'] = t
+        output_index = pd.MultiIndex.from_product(
+            [cdata.data_t.index.levels[1], cdata.data_t.index.levels[1]],
+            names=["prod1", "prod2"],
+        )
+        output = pd.DataFrame(data={"proximity": prox_mat.ravel()}, index=output_index)
+        output["time"] = t
         output_list.append(output)
 
     output = pd.concat(output_list)
 
-    # Remove entries for product's proximity with itself
+    # Format
     output = output.reset_index()
-    output.columns = ['prod1','prod2','proximity','time']
-    output = output[['time','prod1','prod2','proximity']]
-    output = output[output.prod1!=output.prod2]
+    output.columns = ["prod1", "prod2", "proximity", "time"]
+    output = output[["time", "prod1", "prod2", "proximity"]]
+    
+    # # Remove entries for product's proximity with itself
+    # output = output[output.prod1 != output.prod2]
 
     # Rename based on original product column name
-    output = output.rename(columns={'prod1':cdata.cols_input['prod']+'_1',
-                                    'prod2':cdata.cols_input['prod']+'_2',
-                                    'time':cdata.cols_input['time']})
+    output = output.rename(
+        columns={
+            "prod1": cdata.cols_input["prod"] + "_1",
+            "prod2": cdata.cols_input["prod"] + "_2",
+            "time": cdata.cols_input["time"],
+        }
+    )
 
-    return(output)
+    return output
```

### Comparing `ecomplexity-0.5.2/ecomplexity.egg-info/PKG-INFO` & `ecomplexity-0.5.3/ecomplexity.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,87 +1,107 @@
 Metadata-Version: 2.1
 Name: ecomplexity
-Version: 0.5.2
+Version: 0.5.3
 Summary: Package to calculate economic complexity and associated variables
 Home-page: https://github.com/cid-harvard/py-ecomplexity
 Author: Shreyas Gadgin Matha
 Author-email: shreyas.gm61@gmail.com
 License: MIT
-Description: # Economic Complexity and Product Complexity
-        ## by the Growth Lab at Harvard's Center for International Development
-        This package is part of Harvard Growth Lab’s portfolio of software packages, digital products and interactive data visualizations. To browse our entire portfolio, please visit growthlab.app. To learn more about our research, please visit [Harvard Growth Lab’s home page](https://growthlab.cid.harvard.edu/).
-        
-        # About
-        Python package to calculate economic complexity indices.
-        
-        STATA implementation of the economic complexity index available at: <https://github.com/cid-harvard/ecomplexity>
-        
-        Explore complexity and associated data using Harvard CID's Atlas tool: <http://atlas.cid.harvard.edu>
-        
-        ## Tutorial
-        
-        **Installation**:
-        At terminal: `pip install ecomplexity`
-        
-        **Usage**:
-        
-        ```python
-        from ecomplexity import ecomplexity
-        from ecomplexity import proximity
-        
-        # Import trade data from CID Atlas
-        data_url = "https://intl-atlas-downloads.s3.amazonaws.com/country_hsproduct2digit_year.csv.zip"
-        data = pd.read_csv(data_url, compression="zip", low_memory=False)
-        data = data[['year','location_code','hs_product_code','export_value']]
-        
-        # Calculate complexity
-        trade_cols = {'time':'year', 'loc':'location_code', 'prod':'hs_product_code', 'val':'export_value'}
-        cdata = ecomplexity(data, trade_cols)
-        
-        # Calculate proximity matrix
-        prox_df = proximity(data, trade_cols)
-        ```
-        
-        **Arguments**:
-        
-        ```text
-        data: pandas dataframe containing production / trade data.
-            Including variables indicating time, location, product and value
-        cols_input: dict of column names for time, location, product and value.
-            Example: {'time':'year', 'loc':'origin', 'prod':'hs92', 'val':'export_val'}
-        presence_test: str for test used for presence of industry in location.
-            One of "rca" (default), "rpop", "both", or "manual".
-            Determines which values are used for M_cp calculations.
-            If "manual", M_cp is taken as given from the "value" column in data
-        val_errors_flag: {'coerce','ignore','raise'}. Passed to pd.to_numeric
-            *default* coerce.
-        rca_mcp_threshold: numeric indicating RCA threshold beyond which mcp is 1.
-            *default* 1.
-        rpop_mcp_threshold: numeric indicating RPOP threshold beyond which mcp is 1.
-            *default* 1. Only used if presence_test is not "rca".
-        pop: pandas df, with time, location and corresponding population, in that order.
-            Not required if presence_test is "rca" (default).
-        continuous: Used to calculate product proximities, indicates whether
-            to consider correlation of every product pair (True) or product
-            co-occurrence (False). *default* False.
-        asymmetric: Used to calculate product proximities, indicates whether
-            to generate asymmetric proximity matrix (True) or symmetric (False).
-            *default* False.
-        ```
-        
-        ### TODO
-        
-        - There are very minor differences in the values of density, COI and COG between STATA and Python due to the way matrix computations are handled by the two. These should be aligned in the future.
-        - knn options for density: in the future, allow knn parameter for density calculation
-        
-        ### References
-        
-        - Hausmann, R., Hidalgo, C. A., Bustos, S., Coscia, M., Simoes, A., & Yıldırım, M. (2013). The Atlas of Economic Complexity: Mapping Paths to Prosperity (Part 1). Retrieved from <https://growthlab.cid.harvard.edu/files/growthlab/files/atlas_2013_part1.pdf>
-        - Hidalgo, C. A., Klinger, B., Barabasi, A.-L., & Hausmann, R. (2007). The Product Space Conditions the Development of Nations. Science, 317(5837), 482–487. <http://doi.org/10.1126/science.1144581>
-        
 Keywords: pandas python networks economics complexity
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pandas>0.23.0
+Requires-Dist: numpy>1.22.0
+Requires-Dist: scikit-learn>1.0.0
+
+# Economic Complexity and Product Complexity
+
+By the Growth Lab at Harvard's Center for International Development
+
+This package is part of Harvard Growth Lab’s portfolio of software packages, digital products and interactive data visualizations. To browse our entire portfolio, please visit [growthlab.app](growthlab.app). To learn more about our research, please visit [Harvard Growth Lab’s home page](https://growthlab.cid.harvard.edu/).
+
+# About
+Python package to calculate economic complexity indices.
+
+STATA implementation of the economic complexity index available at: <https://github.com/cid-harvard/ecomplexity>
+
+Explore complexity and associated data using Harvard CID's Atlas tool: <http://atlas.cid.harvard.edu>
+
+## Tutorial
+
+**Installation**:
+For the latest stable version: `pip install ecomplexity`
+
+Latest version of the package under development (untested and possibly with bugs), install directly from GitHub:
+`pip install git+https://github.com/cid-harvard/py-ecomplexity@develop`
+
+**Usage**:
+
+```python
+from ecomplexity import ecomplexity
+from ecomplexity import proximity
+
+# Import trade data from CID Atlas
+data_url = "https://intl-atlas-downloads.s3.amazonaws.com/country_hsproduct2digit_year.csv.zip"
+data = pd.read_csv(data_url, compression="zip", low_memory=False)
+data = data[['year','location_code','hs_product_code','export_value']]
+
+# Calculate complexity
+trade_cols = {'time':'year', 'loc':'location_code', 'prod':'hs_product_code', 'val':'export_value'}
+cdata = ecomplexity(data, trade_cols)
+
+# Calculate proximity matrix
+prox_df = proximity(data, trade_cols)
+```
+
+**Arguments**:
+
+```text
+data: pandas dataframe containing production / trade data.
+    Including variables indicating time, location, product and value
+cols_input: dict of column names for time, location, product and value.
+    Example: {'time':'year', 'loc':'origin', 'prod':'hs92', 'val':'export_val'}
+presence_test: str for test used for presence of industry in location.
+    One of "rca" (default), "rpop", or "manual".
+    Determines which values are used for M_cp calculations.
+    If "manual", M_cp is taken as given from the "value" column in data
+val_errors_flag: {'coerce','ignore','raise'}. Passed to pd.to_numeric
+    *default* coerce.
+rca_mcp_threshold: numeric indicating RCA threshold beyond which mcp is 1.
+    *default* 1.
+rpop_mcp_threshold: numeric indicating RPOP threshold beyond which mcp is 1.
+    *default* 1. Only used if presence_test is not "rca".
+pop: pandas df, with time, location and corresponding population, in that order.
+    Not required if presence_test is "rca", which is the default.
+continuous: Used to calculate product proximities, indicates whether
+    to consider correlation of every product pair (True) or product
+    co-occurrence (False). *default* False.
+asymmetric: Used to calculate product proximities, indicates whether
+    to generate asymmetric proximity matrix (True) or symmetric (False).
+    *default* False.
+proximity_edgelist: pandas df with cols 'prod1', 'prod2', 'proximity'.
+    If None (default), proximity values are calculated from data.
+knn: Number of nearest neighbors from proximity matrix to use to calculate
+    density. Will use entire proximity matrix if None.
+    *default* None.
+check_logsupermodularity: If True (default), check log-supermodularity.
+    If int, use roughly that many samples to check log-supermodularity.
+report_logsupermodularity: If True, print warning if log-supermodularity.
+    If False (default), don't.
+verbose: Print year being processed
+```
+
+## FAQ
+
+- Why are ECI and PCI are both normalized using ECI's mean and std. dev?
+    + This normalization preserves the property that ECI = (mean of PCI of products for which MCP=1)
+- What is log-supermodularity?
+    + Refer `ecomplexity/log_supermodularity.py` for a brief explanation. More at Schetter, U. (2019). A Structural Ranking of Economic Complexity (SSRN Scholarly Paper 3485842). https://doi.org/10.2139/ssrn.3485842.
+
+### References
+
+- Hausmann, R., Hidalgo, C. A., Bustos, S., Coscia, M., Simoes, A., & Yıldırım, M. (2013). The Atlas of Economic Complexity: Mapping Paths to Prosperity (Part 1). Retrieved from <https://growthlab.cid.harvard.edu/files/growthlab/files/atlas_2013_part1.pdf>
+- Hidalgo, C. A., Klinger, B., Barabasi, A.-L., & Hausmann, R. (2007). The Product Space Conditions the Development of Nations. Science, 317(5837), 482–487. <http://doi.org/10.1126/science.1144581>
```

### Comparing `ecomplexity-0.5.2/setup.py` & `ecomplexity-0.5.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from setuptools import setup, find_packages
 
 
 def readme():
-    with open("README.md") as f:
+    with open("README.md", encoding="utf-8") as f:
         return f.read()
 
-
-setup(
-    name="ecomplexity",
-    version="0.5.2",
-    description="Package to calculate economic complexity and associated variables",
-    long_description=readme(),
-    long_description_content_type="text/markdown",
-    url="https://github.com/cid-harvard/py-ecomplexity",
-    author="Shreyas Gadgin Matha",
-    author_email="shreyas.gm61@gmail.com",
-    license="MIT",
-    packages=find_packages(),
-    keywords="pandas python networks economics complexity",
-    python_requires=">=3",
-    install_requires=["pandas >0.23.0", "numpy >1.15.0"],
-    zip_safe=False,
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-)
+setup(name='ecomplexity',
+      version='0.5.3',
+      description='Package to calculate economic complexity and associated variables',
+      long_description=readme(),
+      long_description_content_type='text/markdown',
+      url='https://github.com/cid-harvard/py-ecomplexity',
+      author='Shreyas Gadgin Matha',
+      author_email='shreyas.gm61@gmail.com',
+      license='MIT',
+      packages=find_packages(),
+      keywords="pandas python networks economics complexity",
+      python_requires='>=3',
+      install_requires=[
+          'pandas >0.23.0',
+          'numpy >1.22.0',
+          'scikit-learn >1.0.0'
+      ],
+      zip_safe=False,
+      classifiers=[
+          "Programming Language :: Python :: 3",
+          "License :: OSI Approved :: MIT License",
+          "Operating System :: OS Independent",
+      ])
```

