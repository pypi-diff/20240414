# Comparing `tmp/geoshapley-0.0.2.1.tar.gz` & `tmp/geoshapley-0.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geoshapley-0.0.2.1.tar", last modified: Thu Dec  7 21:42:04 2023, max compression
+gzip compressed data, was "geoshapley-0.0.2.2.tar", last modified: Sun Apr 14 13:39:28 2024, max compression
```

## Comparing `geoshapley-0.0.2.1.tar` & `geoshapley-0.0.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ziqili     (502) staff       (20)        0 2023-12-07 21:42:04.392794 geoshapley-0.0.2.1/
--rw-r--r--   0 ziqili     (502) staff       (20)      524 2023-12-07 21:42:04.392675 geoshapley-0.0.2.1/PKG-INFO
--rw-r--r--   0 ziqili     (502) staff       (20)     1770 2023-12-07 21:11:11.000000 geoshapley-0.0.2.1/README.md
-drwxr-xr-x   0 ziqili     (502) staff       (20)        0 2023-12-07 21:42:04.391861 geoshapley-0.0.2.1/geoshapley/
--rw-r--r--   0 ziqili     (502) staff       (20)       43 2023-12-07 21:41:27.000000 geoshapley-0.0.2.1/geoshapley/__init__.py
--rw-r--r--   0 ziqili     (502) staff       (20)    12440 2023-12-05 00:04:32.000000 geoshapley-0.0.2.1/geoshapley/geoshapley.py
-drwxr-xr-x   0 ziqili     (502) staff       (20)        0 2023-12-07 21:42:04.392516 geoshapley-0.0.2.1/geoshapley.egg-info/
--rw-r--r--   0 ziqili     (502) staff       (20)      524 2023-12-07 21:42:04.000000 geoshapley-0.0.2.1/geoshapley.egg-info/PKG-INFO
--rw-r--r--   0 ziqili     (502) staff       (20)      272 2023-12-07 21:42:04.000000 geoshapley-0.0.2.1/geoshapley.egg-info/SOURCES.txt
--rw-r--r--   0 ziqili     (502) staff       (20)       32 2023-12-07 21:42:04.000000 geoshapley-0.0.2.1/geoshapley.egg-info/dependency_links.txt
--rw-r--r--   0 ziqili     (502) staff       (20)       56 2023-12-07 21:42:04.000000 geoshapley-0.0.2.1/geoshapley.egg-info/entry_points.txt
--rw-r--r--   0 ziqili     (502) staff       (20)       31 2023-12-07 21:42:04.000000 geoshapley-0.0.2.1/geoshapley.egg-info/requires.txt
--rw-r--r--   0 ziqili     (502) staff       (20)       11 2023-12-07 21:42:04.000000 geoshapley-0.0.2.1/geoshapley.egg-info/top_level.txt
--rw-r--r--   0 ziqili     (502) staff       (20)       38 2023-12-07 21:42:04.392826 geoshapley-0.0.2.1/setup.cfg
--rw-r--r--   0 ziqili     (502) staff       (20)     1468 2023-12-07 21:41:42.000000 geoshapley-0.0.2.1/setup.py
+drwxr-xr-x   0 ziqili     (502) staff       (20)        0 2024-04-14 13:39:28.322451 geoshapley-0.0.2.2/
+-rw-r--r--   0 ziqili     (502) staff       (20)      524 2024-04-14 13:39:28.322317 geoshapley-0.0.2.2/PKG-INFO
+-rw-r--r--   0 ziqili     (502) staff       (20)     1770 2024-03-27 22:52:44.000000 geoshapley-0.0.2.2/README.md
+drwxr-xr-x   0 ziqili     (502) staff       (20)        0 2024-04-14 13:39:28.321149 geoshapley-0.0.2.2/geoshapley/
+-rw-r--r--   0 ziqili     (502) staff       (20)       43 2023-12-07 21:41:27.000000 geoshapley-0.0.2.2/geoshapley/__init__.py
+-rw-r--r--   0 ziqili     (502) staff       (20)    12985 2024-04-14 13:13:35.000000 geoshapley-0.0.2.2/geoshapley/geoshapley.py
+drwxr-xr-x   0 ziqili     (502) staff       (20)        0 2024-04-14 13:39:28.322126 geoshapley-0.0.2.2/geoshapley.egg-info/
+-rw-r--r--   0 ziqili     (502) staff       (20)      524 2024-04-14 13:39:28.000000 geoshapley-0.0.2.2/geoshapley.egg-info/PKG-INFO
+-rw-r--r--   0 ziqili     (502) staff       (20)      272 2024-04-14 13:39:28.000000 geoshapley-0.0.2.2/geoshapley.egg-info/SOURCES.txt
+-rw-r--r--   0 ziqili     (502) staff       (20)       32 2024-04-14 13:39:28.000000 geoshapley-0.0.2.2/geoshapley.egg-info/dependency_links.txt
+-rw-r--r--   0 ziqili     (502) staff       (20)       56 2024-04-14 13:39:28.000000 geoshapley-0.0.2.2/geoshapley.egg-info/entry_points.txt
+-rw-r--r--   0 ziqili     (502) staff       (20)       31 2024-04-14 13:39:28.000000 geoshapley-0.0.2.2/geoshapley.egg-info/requires.txt
+-rw-r--r--   0 ziqili     (502) staff       (20)       11 2024-04-14 13:39:28.000000 geoshapley-0.0.2.2/geoshapley.egg-info/top_level.txt
+-rw-r--r--   0 ziqili     (502) staff       (20)       38 2024-04-14 13:39:28.322492 geoshapley-0.0.2.2/setup.cfg
+-rw-r--r--   0 ziqili     (502) staff       (20)     1468 2024-04-14 13:38:10.000000 geoshapley-0.0.2.2/setup.py
```

### Comparing `geoshapley-0.0.2.1/PKG-INFO` & `geoshapley-0.0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoshapley
-Version: 0.0.2.1
+Version: 0.0.2.2
 Summary: GeoShapley value for measuring spatial effects
 Home-page: https://github.com/Ziqi-Li/geoshapley
 Author: Ziqi Li
 Author-email: liziqi1992@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `geoshapley-0.0.2.1/README.md` & `geoshapley-0.0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `geoshapley-0.0.2.1/geoshapley/geoshapley.py` & `geoshapley-0.0.2.2/geoshapley/geoshapley.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 class GeoShapleyExplainer:
     def __init__(self, predict_f, background=None, g=2):
         """
         Initialize the GeoShapleyExplainer.
 
         predict_f: The predict function of the model to be explained.
-        background: The background data used for the explanation.
-        g: The number of location features in the data (default is 2). For example, dataframe contains a pair of cooridnates (lat,long) g=2.
+        background: The background data (numpy array) used for the explanation.
+        g: The number of location features in the data (default is 2). For example, feature set contains a pair of cooridnates (lat,long) g=2.
         """
         self.predict_f = predict_f
         self.background = background
         self.g = g
         self.n, self.M = background.shape
         
 
@@ -27,47 +27,51 @@
         """
         Calculate GeoShapley value for a single sample and a reference point in the background data
 
         x: current sample
         reference: a reference point in the background data
         """
 
-    
+        #M = 4, g = 2, k = 2
+
+        k = self.M - self.g
         M = self.M
-        Z = np.zeros((2**(M-1),M-1+M-2+1))
+
+        Z = np.zeros((2**(k+1),2*k+2))
 
         #intercept
         Z[:,-1] = 1
     
-        weights = np.zeros(2**(M-1))
+        weights = np.zeros(2**(k+1))
     
-        V = np.zeros((2**(M-1),M))
+        V = np.zeros((2**(k+1),M))
     
-        for i in range(2**(M-1)):
+        for i in range(2**(k+1)):
             V[i,:] = reference
 
         #Mark 1 for each combination
-        for i,s in enumerate(self._powerset(range(M-1))):
+        for i,s in enumerate(self._powerset(range(k+1))):
         
             s = list(s)
             Z[i,s] = 1
             V[i,s] = x[s]
         
-            if (M-2) in s: #If location is in
-                V[i, (M-1)] = x[(M-1)]
+            if k in s: #If location is in
+                V[i, (k+1):] = x[(k+1):]
             
-                if (len(s) > 1):
+                if (len(s) > 1): #mark interaction
                     for j in s:
-                      if j < (M-2):
-                          Z[i, M-1+j] = 1
+                      if j < k:
+                          Z[i, k+1+j] = 1
         
-            weights[i] = self._shapley_kernel(M-1, len(s))
-    
-        y = self.predict_f(V).reshape(-1)
+            weights[i] = self._shapley_kernel(k+1, len(s))
+            #print("s:", s)
+            #print("Z:", Z[i,:])
 
+        y = self.predict_f(V).reshape(-1)
 
         #Solve WLS
         ZTw = np.dot(Z.T, np.diag(weights))
     
         phi = np.linalg.solve(np.dot(ZTw, Z), np.dot(ZTw, y))
     
         return phi
@@ -76,21 +80,23 @@
     def _kernel_geoshap_all(self, x):
         """
         Calculate GeoShapley value for a single sample and averaged over the background data
 
         x: current sample
         """
     
-        n,M = self.background.shape
+        k = self.M - self.g
+        n = self.n
     
         # feature primary +
         # 2*geo_interaction to other features +
         # interaction + 
         # intercept
-        phi = np.zeros(M + (M-2))
+
+        phi = np.zeros(k + k + 1 + 1)
         
         for i in range(n):
             reference = self.background[i,:]
             phi = phi + self._kernel_geoshap_single(x, reference)
     
         phi = phi/n
         base_value = phi[-1]
@@ -100,35 +106,36 @@
 
 
 
     def explain(self, X_geo, n_jobs=-1):
         """
         Explain the data.
 
-        X_geo: data to be explained
+        X_geo: pandas dataframe to be explained
         n_jobs: number of jobs for parallel computation (default is -1, using all available processors)
 
         return: A GeoShapleyResults object containing the results of the explanation.
         """
         
         self.X_geo = X_geo
-        n,k = X_geo.shape
+        n,M = X_geo.shape
+        k = M - self.g
 
-        geoshaps_total = np.zeros((n,(k-1+k-2)))
+        geoshaps_total = np.zeros((n,(2*k + 1)))
     
         # Parallel computation
         results = Parallel(n_jobs=n_jobs)(delayed(self._kernel_geoshap_all)(X_geo.values[i, :]) for i in tqdm(range(n)))
 
         # Extract results
         geoshaps_total = np.array([result[1] for result in results])
         base_value = results[0][0]  # Assuming base_value is same for all
 
-        primary = geoshaps_total[:,:(k-2)]
-        geo = geoshaps_total[:,(k-2)]
-        geo_intera = geoshaps_total[:,(k-1):]
+        primary = geoshaps_total[:,:k]
+        geo = geoshaps_total[:,k]
+        geo_intera = geoshaps_total[:,(k+1):]
     
     
         return GeoShapleyResults(self, base_value, primary, geo, geo_intera)
 
 
     def _powerset(self, iterable):
         """
@@ -173,53 +180,56 @@
         self.predict_f = explainer.predict_f
         self.X_geo = explainer.X_geo
         self.g = explainer.g
         self.M = explainer.M
         self.background = explainer.background
 
 
-    def get_svc(self, col, coef_type = "gwr", include_primary=False):
+    def get_svc(self, col, coef_type = "gwr", include_primary=False, coords=None):
         """
-        Calculate the spatial coefficient for each feature
+        Calculate the spatial (location-spefific) coefficient for each feature
 
         col: specify the column index to be calculated
         coef_type: 
-            "raw": raw coefficient based on the ratio of interaction effect and mean removed feature value
-            "gwr": coefficient based on GWR smoothing
-
-        include_primary: whether to include the primary effect in the SVC
-
+            "raw": raw coefficient based on the ratio of interaction effect and mean removed feature value. 
+                   May result in extreme values.
+            "gwr": coefficient based on GWR smoothing. Requires mgwr package.
+        
+        include_primary: whether to include the primary effect in the spatial coefficient
+        coords: a numpy array of the coordinates of the data. If not provided, the last two columns of the data will be used as coordinates.
+        
         """
     
         n,k = self.primary.shape
     
         params = np.zeros((n, k))
-        params[:,:] = self.geo_intera 
+        params[:,:] = self.geo_intera
 
         if include_primary:
             params[:,:] = params[:,:] + self.primary
 
         for j in col:
             if coef_type == "raw":
                 params[:,j] = params[:,j] / (self.X_geo.values - self.X_geo.values.mean(axis=0))[:,j]
 
             if coef_type == "gwr":
                 try:
                     import mgwr
                 except ImportError:
                     print("Please install mgwr package (e.g., pip install mgwr)")
                 
-                coords = list(zip(self.X_geo.values[:,-2], self.X_geo.values[:,-1]))
+                if coords is None: #Assuming the last two columns are the coordinates
+                    coords = np.array(list(zip(self.X_geo.values[:,-2], self.X_geo.values[:,-1])))
+
                 y = params[:,j].reshape(-1,1)
                 X = (self.X_geo.values - self.X_geo.values.mean(axis=0))[:,j].reshape(-1,1)
                 gwr_selector = mgwr.sel_bw.Sel_BW(coords, y, X,constant=False)
-                gwr_bw = gwr_selector.search()
+                gwr_bw = gwr_selector.search(bw_min=20)
                 gwr_model = mgwr.gwr.GWR(coords, y, X, gwr_bw,constant=False).fit()
                 params[:,j] = gwr_model.params[:,0]
-                #print(gwr_model.R2)
     
         return params[:,col]
     
 
     def geoshap_to_shap(self):
         """
         Convert GeoShapley values to Shapley values.
@@ -247,15 +257,15 @@
 
         try:
             import shap
         except ImportError:
             print("Please install shap package (e.g., pip install shap)")
         
 
-        names = self.X_geo.iloc[:,:-2].copy()
+        names = self.X_geo.iloc[:,:-self.g].copy()
         names["GEO"] = 0
     
         if include_interaction:
             total = np.hstack((self.primary, self.geo.reshape(-1,1), self.geo_intera))
             names[[name + " x GEO" for name in self.X_geo.columns[:-self.g]]] = self.X_geo.iloc[:,:-self.g].copy()
         else:
             total = self.geoshap_to_shap()
@@ -338,27 +348,27 @@
         The table is ranked based on the mean absolute value of the GeoShapley values.
 
         include_interaction: whether to include the interaction effect in the summary statistics
 
         """
         cols = ["min","25%","50%","75%","max"]
         summary_table = pd.DataFrame(np.percentile(self.primary, [0,25,50,75,100],axis=0).T,columns=cols)
-        summary_table.index = self.X_geo.columns[:-2]
+        summary_table.index = self.X_geo.columns[:-self.g]
         summary_table["mean"] = np.mean(self.primary,axis=0)
         summary_table["std"] = np.std(self.primary,axis=0)
         summary_table["abs. mean"] = np.mean(np.abs(self.primary),axis=0)
 
         summary_table.loc['GEO'] = np.append(np.percentile(self.geo, [0,25,50,75,100],axis=0).T, 
                                      [np.mean(self.geo), np.std(self.geo),
                                       np.mean(np.abs(self.geo))])
         
 
         if include_interaction:
             intera_summary_table = pd.DataFrame(np.percentile(self.geo_intera, [0,25,50,75,100],axis=0).T,columns=cols)
-            intera_summary_table.index = self.X_geo.columns[:-2] + " x GEO"
+            intera_summary_table.index = self.X_geo.columns[:-self.g] + " x GEO"
             intera_summary_table["mean"] = np.mean(self.geo_intera,axis=0)
             intera_summary_table["std"] = np.std(self.geo_intera,axis=0)
             intera_summary_table["abs. mean"] = np.mean(np.abs(self.geo_intera),axis=0) 
 
             summary_table = pd.concat([summary_table, intera_summary_table], ignore_index=False)
         
         summary_table.sort_values(by=['abs. mean'],ascending=False,inplace=True)
```

### Comparing `geoshapley-0.0.2.1/geoshapley.egg-info/PKG-INFO` & `geoshapley-0.0.2.2/geoshapley.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geoshapley
-Version: 0.0.2.1
+Version: 0.0.2.2
 Summary: GeoShapley value for measuring spatial effects
 Home-page: https://github.com/Ziqi-Li/geoshapley
 Author: Ziqi Li
 Author-email: liziqi1992@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `geoshapley-0.0.2.1/setup.py` & `geoshapley-0.0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     not x.startswith('#')) and (not x.startswith('-'))]
 dependency_links = [x.strip().replace('git+', '') for x in all_reqs \
                     if 'git+' not in x]
 
 
 setup(
     name="geoshapley",
-    version='0.0.2.1',
+    version='0.0.2.2',
     description="GeoShapley value for measuring spatial effects",
     long_description="GeoShapley: A game theory based approach to measuring spatial effects from machine learning models",
     author="Ziqi Li",
     author_email="liziqi1992@gmail.com",
     url="https://github.com/Ziqi-Li/geoshapley",
     license="MIT",
     entry_points={'console_scripts': ['geoshapley=geoshapley.__main__:main',],},
```

