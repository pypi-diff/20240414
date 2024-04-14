# Comparing `tmp/isom2600-3.3.tar.gz` & `tmp/isom2600-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\isom2600-3.3.tar", last modified: Sun Apr 14 00:24:02 2024, max compression
+gzip compressed data, was "dist\isom2600-3.4.tar", last modified: Sun Apr 14 00:29:39 2024, max compression
```

## Comparing `isom2600-3.3.tar` & `isom2600-3.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-14 00:24:02.000000 isom2600-3.3/
--rw-rw-rw-   0        0        0      204 2024-04-14 00:24:02.000000 isom2600-3.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-14 00:24:02.000000 isom2600-3.3/isom2600/
--rw-rw-rw-   0        0        0       44 2024-03-15 15:35:38.000000 isom2600-3.3/isom2600/__init__.py
--rw-rw-rw-   0        0        0     2335 2024-04-08 04:26:45.000000 isom2600-3.3/isom2600/data.py
--rw-rw-rw-   0        0        0     9024 2024-04-14 00:23:40.000000 isom2600-3.3/isom2600/regression.py
-drwxrwxrwx   0        0        0        0 2024-04-14 00:24:02.000000 isom2600-3.3/isom2600.egg-info/
--rw-rw-rw-   0        0        0      204 2024-04-14 00:24:02.000000 isom2600-3.3/isom2600.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-14 00:24:02.000000 isom2600-3.3/isom2600.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-14 00:24:02.000000 isom2600-3.3/isom2600.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-14 00:24:02.000000 isom2600-3.3/isom2600.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-14 00:24:02.000000 isom2600-3.3/setup.cfg
--rw-rw-rw-   0        0        0      146 2024-04-14 00:23:53.000000 isom2600-3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-14 00:29:39.000000 isom2600-3.4/
+-rw-rw-rw-   0        0        0      204 2024-04-14 00:29:39.000000 isom2600-3.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-14 00:29:39.000000 isom2600-3.4/isom2600/
+-rw-rw-rw-   0        0        0       44 2024-03-15 15:35:38.000000 isom2600-3.4/isom2600/__init__.py
+-rw-rw-rw-   0        0        0     2335 2024-04-08 04:26:45.000000 isom2600-3.4/isom2600/data.py
+-rw-rw-rw-   0        0        0     9001 2024-04-14 00:29:30.000000 isom2600-3.4/isom2600/regression.py
+drwxrwxrwx   0        0        0        0 2024-04-14 00:29:39.000000 isom2600-3.4/isom2600.egg-info/
+-rw-rw-rw-   0        0        0      204 2024-04-14 00:29:39.000000 isom2600-3.4/isom2600.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-14 00:29:39.000000 isom2600-3.4/isom2600.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-14 00:29:39.000000 isom2600-3.4/isom2600.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-14 00:29:39.000000 isom2600-3.4/isom2600.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-14 00:29:39.000000 isom2600-3.4/setup.cfg
+-rw-rw-rw-   0        0        0      146 2024-04-14 00:29:34.000000 isom2600-3.4/setup.py
```

### Comparing `isom2600-3.3/isom2600/data.py` & `isom2600-3.4/isom2600/data.py`

 * *Files identical despite different names*

### Comparing `isom2600-3.3/isom2600/regression.py` & `isom2600-3.4/isom2600/regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,17 +222,17 @@
     ax2.set_title('Histogram')
 
     ax3 = plt.subplot(223)
     t = range(len(fitted_y))
     ax3.scatter(t, studentized_residuals)
     ax3.set_xlabel('Observation order')
     ax3.set_ylabel('Residuals')
-    ax3.set_title('Time series plot of studentized residuals')
+    ax3.set_title('Time series plot of residuals')
 
     ax4 = plt.subplot(224)
     ax4 = sns.residplot(x=fitted_y, y=studentized_residuals,
                               lowess=True,
                               scatter_kws={'alpha': 0.5},
                               line_kws={'color': 'red', 'lw': 1, 'alpha': 0.8})
-    ax4.set_title('Internally Studentized Residuals vs Fitted values')
+    ax4.set_title('Studentized Residuals vs Fitted values')
     ax4.set_xlabel('Fitted values')
     ax4.set_ylabel('Studentized Residuals');
```

