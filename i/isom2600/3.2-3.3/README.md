# Comparing `tmp/isom2600-3.2.tar.gz` & `tmp/isom2600-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\isom2600-3.2.tar", last modified: Sun Apr 14 00:13:50 2024, max compression
+gzip compressed data, was "dist\isom2600-3.3.tar", last modified: Sun Apr 14 00:24:02 2024, max compression
```

## Comparing `isom2600-3.2.tar` & `isom2600-3.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 00:13:50.000000 isom2600-3.2/
--rw-rw-rw-   0        0        0      204 2024-04-14 00:13:50.000000 isom2600-3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-14 00:13:50.000000 isom2600-3.2/isom2600/
--rw-rw-rw-   0        0        0       44 2024-03-15 15:35:38.000000 isom2600-3.2/isom2600/__init__.py
--rw-rw-rw-   0        0        0     2335 2024-04-08 04:26:45.000000 isom2600-3.2/isom2600/data.py
--rw-rw-rw-   0        0        0     9046 2024-04-14 00:12:43.000000 isom2600-3.2/isom2600/regression.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:13:50.000000 isom2600-3.2/isom2600.egg-info/
--rw-rw-rw-   0        0        0      204 2024-04-14 00:13:50.000000 isom2600-3.2/isom2600.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-14 00:13:50.000000 isom2600-3.2/isom2600.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 00:13:50.000000 isom2600-3.2/isom2600.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-14 00:13:50.000000 isom2600-3.2/isom2600.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 00:13:50.000000 isom2600-3.2/setup.cfg
--rw-rw-rw-   0        0        0      146 2024-04-14 00:13:47.000000 isom2600-3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 00:24:02.000000 isom2600-3.3/
+-rw-rw-rw-   0        0        0      204 2024-04-14 00:24:02.000000 isom2600-3.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-14 00:24:02.000000 isom2600-3.3/isom2600/
+-rw-rw-rw-   0        0        0       44 2024-03-15 15:35:38.000000 isom2600-3.3/isom2600/__init__.py
+-rw-rw-rw-   0        0        0     2335 2024-04-08 04:26:45.000000 isom2600-3.3/isom2600/data.py
+-rw-rw-rw-   0        0        0     9024 2024-04-14 00:23:40.000000 isom2600-3.3/isom2600/regression.py
+drwxrwxrwx   0        0        0        0 2024-04-14 00:24:02.000000 isom2600-3.3/isom2600.egg-info/
+-rw-rw-rw-   0        0        0      204 2024-04-14 00:24:02.000000 isom2600-3.3/isom2600.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-14 00:24:02.000000 isom2600-3.3/isom2600.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 00:24:02.000000 isom2600-3.3/isom2600.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-14 00:24:02.000000 isom2600-3.3/isom2600.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 00:24:02.000000 isom2600-3.3/setup.cfg
+-rw-rw-rw-   0        0        0      146 2024-04-14 00:23:53.000000 isom2600-3.3/setup.py
```

### Comparing `isom2600-3.2/isom2600/data.py` & `isom2600-3.3/isom2600/data.py`

 * *Files identical despite different names*

### Comparing `isom2600-3.2/isom2600/regression.py` & `isom2600-3.3/isom2600/regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,16 +201,16 @@
 
 def getvif(X):
     X = sm.add_constant(X)
     vif = pd.DataFrame()
     vif["VIF"] = [variance_inflation_factor(X.values, i) for i in range(X.shape[1])]
     vif["Predictors"] = X.columns
     return(vif.drop(index = 0).round(2))
-def four_in_one(X,Y,model):
-    fitted_y = model.predict(sm.add_constant(X))
+def residual_plot(model):
+    fitted_y = model.fittedvalues
     studentized_residuals = model.get_influence().resid_studentized_internal
     plt.figure(figsize=(10,10))
     ax1 = plt.subplot(221)
     stats.probplot(studentized_residuals, dist="norm", plot=plt)
     ax1.set_title('Normal Q-Q')
     ax1.set_xlabel('Normal Quantiles')
     ax1.set_ylabel('Studentized Residuals');
@@ -218,15 +218,15 @@
     ax2 = plt.subplot(222)
     ax2.hist(studentized_residuals)
     ax2.set_xlabel('Studentized Residuals')
     ax2.set_ylabel('Count')
     ax2.set_title('Histogram')
 
     ax3 = plt.subplot(223)
-    t = range(dataframe.shape[0])
+    t = range(len(fitted_y))
     ax3.scatter(t, studentized_residuals)
     ax3.set_xlabel('Observation order')
     ax3.set_ylabel('Residuals')
     ax3.set_title('Time series plot of studentized residuals')
 
     ax4 = plt.subplot(224)
     ax4 = sns.residplot(x=fitted_y, y=studentized_residuals,
```

