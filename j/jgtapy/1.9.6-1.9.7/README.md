# Comparing `tmp/jgtapy-1.9.6.tar.gz` & `tmp/jgtapy-1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jgtapy-1.9.6.tar", last modified: Sun Nov 20 08:42:54 2022, max compression
+gzip compressed data, was "dist/jgtapy-1.9.7.tar", last modified: Sun Nov 20 20:11:55 2022, max compression
```

## Comparing `jgtapy-1.9.6.tar` & `jgtapy-1.9.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0     1000     1000        0 2022-11-20 08:42:54.000000 jgtapy-1.9.6/
--rwxrwxrwx   0     1000     1000       45 2022-11-20 04:23:27.000000 jgtapy-1.9.6/AUTHORS
--rwxrwxrwx   0     1000     1000     1066 2022-11-20 04:23:27.000000 jgtapy-1.9.6/LICENSE
--rwxrwxrwx   0     1000     1000      152 2022-11-20 04:23:27.000000 jgtapy-1.9.6/MANIFEST.in
--rwxrwxrwx   0     1000     1000     2651 2022-11-20 08:42:54.000000 jgtapy-1.9.6/PKG-INFO
--rwxrwxrwx   0     1000     1000     1607 2022-11-20 05:33:23.000000 jgtapy-1.9.6/README.rst
-drwxrwxrwx   0     1000     1000        0 2022-11-20 08:42:54.000000 jgtapy-1.9.6/jgtapy/
--rwxrwxrwx   0     1000     1000      162 2022-11-20 05:34:42.000000 jgtapy-1.9.6/jgtapy/__init__.py
--rwxrwxrwx   0     1000     1000   132552 2022-11-20 08:42:32.000000 jgtapy-1.9.6/jgtapy/indicators.py
--rwxrwxrwx   0     1000     1000     1389 2022-11-20 04:23:27.000000 jgtapy-1.9.6/jgtapy/utils.py
-drwxrwxrwx   0     1000     1000        0 2022-11-20 08:42:54.000000 jgtapy-1.9.6/jgtapy.egg-info/
--rwxrwxrwx   0     1000     1000     2651 2022-11-20 08:42:53.000000 jgtapy-1.9.6/jgtapy.egg-info/PKG-INFO
--rwxrwxrwx   0     1000     1000      277 2022-11-20 08:42:53.000000 jgtapy-1.9.6/jgtapy.egg-info/SOURCES.txt
--rwxrwxrwx   0     1000     1000        1 2022-11-20 08:42:53.000000 jgtapy-1.9.6/jgtapy.egg-info/dependency_links.txt
--rwxrwxrwx   0     1000     1000      278 2022-11-20 08:42:53.000000 jgtapy-1.9.6/jgtapy.egg-info/requires.txt
--rwxrwxrwx   0     1000     1000        7 2022-11-20 08:42:53.000000 jgtapy-1.9.6/jgtapy.egg-info/top_level.txt
--rwxrwxrwx   0     1000     1000      549 2022-11-20 08:42:22.000000 jgtapy-1.9.6/pyproject.toml
--rwxrwxrwx   0     1000     1000      103 2022-11-20 08:42:54.000000 jgtapy-1.9.6/setup.cfg
--rwxrwxrwx   0     1000     1000     1780 2022-11-20 08:42:10.000000 jgtapy-1.9.6/setup.py
+drwxrwxrwx   0     1000     1000        0 2022-11-20 20:11:55.000000 jgtapy-1.9.7/
+-rwxrwxrwx   0     1000     1000       45 2022-11-20 20:11:18.000000 jgtapy-1.9.7/AUTHORS
+-rwxrwxrwx   0     1000     1000     1066 2022-11-20 20:11:18.000000 jgtapy-1.9.7/LICENSE
+-rwxrwxrwx   0     1000     1000      152 2022-11-20 20:11:18.000000 jgtapy-1.9.7/MANIFEST.in
+-rwxrwxrwx   0     1000     1000     2651 2022-11-20 20:11:55.000000 jgtapy-1.9.7/PKG-INFO
+-rwxrwxrwx   0     1000     1000     1607 2022-11-20 20:11:18.000000 jgtapy-1.9.7/README.rst
+drwxrwxrwx   0     1000     1000        0 2022-11-20 20:11:55.000000 jgtapy-1.9.7/jgtapy/
+-rwxrwxrwx   0     1000     1000      162 2022-11-20 20:11:18.000000 jgtapy-1.9.7/jgtapy/__init__.py
+-rwxrwxrwx   0     1000     1000   137439 2022-11-20 20:11:18.000000 jgtapy-1.9.7/jgtapy/indicators.py
+-rwxrwxrwx   0     1000     1000     1389 2022-11-20 20:11:18.000000 jgtapy-1.9.7/jgtapy/utils.py
+drwxrwxrwx   0     1000     1000        0 2022-11-20 20:11:55.000000 jgtapy-1.9.7/jgtapy.egg-info/
+-rwxrwxrwx   0     1000     1000     2651 2022-11-20 20:11:55.000000 jgtapy-1.9.7/jgtapy.egg-info/PKG-INFO
+-rwxrwxrwx   0     1000     1000      277 2022-11-20 20:11:55.000000 jgtapy-1.9.7/jgtapy.egg-info/SOURCES.txt
+-rwxrwxrwx   0     1000     1000        1 2022-11-20 20:11:55.000000 jgtapy-1.9.7/jgtapy.egg-info/dependency_links.txt
+-rwxrwxrwx   0     1000     1000      278 2022-11-20 20:11:55.000000 jgtapy-1.9.7/jgtapy.egg-info/requires.txt
+-rwxrwxrwx   0     1000     1000        7 2022-11-20 20:11:55.000000 jgtapy-1.9.7/jgtapy.egg-info/top_level.txt
+-rwxrwxrwx   0     1000     1000      549 2022-11-20 20:11:18.000000 jgtapy-1.9.7/pyproject.toml
+-rwxrwxrwx   0     1000     1000      103 2022-11-20 20:11:55.000000 jgtapy-1.9.7/setup.cfg
+-rwxrwxrwx   0     1000     1000     1780 2022-11-20 20:11:19.000000 jgtapy-1.9.7/setup.py
```

### Comparing `jgtapy-1.9.6/LICENSE` & `jgtapy-1.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jgtapy-1.9.6/PKG-INFO` & `jgtapy-1.9.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jgtapy
-Version: 1.9.6
+Version: 1.9.7
 Summary: Enhanced Tapy
 Home-page: https://github.com/jgwill/jgtapy
 Author: Dmitrii Kurlov/+JG
 Author-email: JGWill <jgi@jgwill.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jgwill/jgtapy
 Project-URL: Bug Tracker, https://github.com/jgwill/jgtapy/issues
```

### Comparing `jgtapy-1.9.6/README.rst` & `jgtapy-1.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `jgtapy-1.9.6/jgtapy/indicators.py` & `jgtapy-1.9.7/jgtapy/indicators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 
 import numpy as np
 
 from .utils import calculate_ao, calculate_sma, calculate_smma, mad
 
-__version__ = "1.9.6"
+__version__ = "1.9.7"
 
 
 class Indicators:
     """
     Add technical indicators data to a pandas data frame
 
     Example:
@@ -2370,7 +2370,111 @@
 
         df_tmp = df_tmp[["value", "signal"]]
         df_tmp = df_tmp.rename(
             columns={"value": column_name_value, "signal": column_name_signal}
         )
 
         self.df = self.df.merge(df_tmp, left_index=True, right_index=True)
+        
+        
+    def pds_add_ohlc_stc_columns(__df,
+                       cleanupOriginalColumn=True,quiet=True):
+        if not 'Open' in __df.columns:
+            __df['Open'] = __df[['BidOpen', 'AskOpen']].mean(axis=1)
+            __df['High'] = __df[['BidHigh', 'AskHigh']].mean(axis=1)
+            __df['Low'] = __df[['BidLow', 'AskLow']].mean(axis=1)
+            __df['Close'] = __df[['BidClose', 'AskClose']].mean(axis=1)
+            #Median
+            __df['Median']= ((__df['High'] + __df['Low']) / 2)
+        if cleanupOriginalColumn:
+            __df=Indicators.__cleanse_original_columns(__df,quiet)
+        return __df
+
+
+    def __cleanse_original_columns(__df,_quiet=True):
+        __df=Indicators.pds_cleanse_original_columns(__df,_quiet)
+        return __df
+
+    def pds_cleanse_original_columns(__df,_quiet=True):
+        __df=Indicators.jgtpd_drop_col_by_name(__df,'AskHigh',1,_quiet)
+        __df=Indicators.jgtpd_drop_col_by_name(__df,'BidHigh',1,_quiet)
+        __df=Indicators.jgtpd_drop_col_by_name(__df,'AskLow',1,_quiet)
+        __df=Indicators.jgtpd_drop_col_by_name(__df,'BidLow',1,_quiet)
+        __df=Indicators.jgtpd_drop_col_by_name(__df,'AskClose',1,_quiet)
+        __df=Indicators.jgtpd_drop_col_by_name(__df,'BidClose',1,_quiet)
+        __df=Indicators.jgtpd_drop_col_by_name(__df,'BidOpen',1,_quiet)
+        __df=Indicators.jgtpd_drop_col_by_name(__df,'AskOpen',1,_quiet)
+        return __df
+
+    def jgtpd_drop_col_by_name(_df,colname,_axis = 1,_quiet=False):
+        """Drop Column in DF by Name
+
+        Args:
+                _df (DataFrame source)
+                ctxcolname (column name from)
+                _axis (  axis)
+                _quiet (quiet output)
+                
+        Returns:
+            Clean DataFrame 
+        """
+        if colname in _df.columns:
+            return _df.drop(_df.loc[:, colname:colname].columns,axis = _axis)
+        else:
+            if not _quiet:
+                print('Col:' + colname + ' was not there')
+            return _df
+
+
+
+    def jgt_create_ids_indicators_as_instance(__df,
+                       enableGatorOscillator=False,
+                       enableMFI=False,
+                       cleanupOriginalColumn=True,
+                       quiet=False):
+        if not quiet:
+            print("Adding indicators...")
+        # if not 'pen' in self.df.columns:
+        #     __df=__.rename(columns={'bidopen': 'BidOpen', 'bidhigh': 'BidHigh','bidclose':'BidClose','bidlow':'BidLow','askopen': 'AskOpen', 'askhigh': 'AskHigh','askclose':'AskClose','asklow':'AskLow','tickqty':'Volume','date':'Date'})
+        __df=Indicators.pds_add_ohlc_stc_columns(__df,cleanupOriginalColumn)
+        i=Indicators(__df)
+        i.accelerator_oscillator( column_name= 'ac')
+        i.alligator(period_jaws=13, period_teeth=8, period_lips=5, shift_jaws=8, shift_teeth=5, shift_lips=3, column_name_jaws='jaw', column_name_teeth='teeth', column_name_lips='lips')
+        i.alligator(period_jaws=89, period_teeth=55, period_lips=34, shift_jaws=55, shift_teeth=34, shift_lips=21, column_name_jaws='bjaw', column_name_teeth='bteeth', column_name_lips='blips')
+        i.awesome_oscillator(column_name='ao')
+        i.fractals(column_name_high='fb', column_name_low='fs')
+        i.fractals3(column_name_high='fb3', column_name_low='fs3')
+        i.fractals5(column_name_high='fb5', column_name_low='fs5')
+        i.fractals8(column_name_high='fb8', column_name_low='fs8')
+        i.fractals13(column_name_high='fb13', column_name_low='fs13')
+        i.fractals21(column_name_high='fb21', column_name_low='fs21')
+        i.fractals34(column_name_high='fb34', column_name_low='fs34')
+        i.fractals55(column_name_high='fb55', column_name_low='fs55')
+        i.fractals89(column_name_high='fb89', column_name_low='fs89')
+        
+        if enableGatorOscillator:
+            i.gator(period_jaws=13, period_teeth=8, period_lips=5, shift_jaws=8, shift_teeth=5, shift_lips=3, column_name_val1='gl', column_name_val2='gh')
+        if enableMFI:
+            i.bw_mfi(column_name='mfi')
+        return i
+    
+    def jgt_create_ids_indicators_as_dataframe(__df,
+                       enableGatorOscillator=False,
+                       enableMFI=False,
+                       cleanupOriginalColumn=True,
+                       dropnavalue=True,
+                       quiet=False):        
+        i=Indicators.jgt_create_ids_indicators_as_instance(__df,
+                       enableGatorOscillator,
+                       enableMFI,                          
+                       cleanupOriginalColumn,                    
+                       quiet)
+        _df=i.df
+        if dropnavalue:
+            _df = _df.dropna()
+        try: 
+            _df=_df.set_index('Date')
+        except TypeError:
+            pass
+        if not quiet:
+            print("done adding indicators :)")
+        return _df
```

### Comparing `jgtapy-1.9.6/jgtapy/utils.py` & `jgtapy-1.9.7/jgtapy/utils.py`

 * *Files identical despite different names*

### Comparing `jgtapy-1.9.6/jgtapy.egg-info/PKG-INFO` & `jgtapy-1.9.7/jgtapy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jgtapy
-Version: 1.9.6
+Version: 1.9.7
 Summary: Enhanced Tapy
 Home-page: https://github.com/jgwill/jgtapy
 Author: Dmitrii Kurlov/+JG
 Author-email: JGWill <jgi@jgwill.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jgwill/jgtapy
 Project-URL: Bug Tracker, https://github.com/jgwill/jgtapy/issues
```

### Comparing `jgtapy-1.9.6/pyproject.toml` & `jgtapy-1.9.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jgtapy"
-version = "1.9.6"
+version = "1.9.7"
 authors = [
   { name="JGWill", email="jgi@jgwill.com" },
 ]
 description = "Enhanced Tapy"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `jgtapy-1.9.6/setup.py` & `jgtapy-1.9.7/setup.py`

 * *Files identical despite different names*

