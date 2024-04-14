# Comparing `tmp/utrc-0.0.5.tar.gz` & `tmp/utrc-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utrc-0.0.5.tar", last modified: Sat Apr  6 19:36:25 2024, max compression
+gzip compressed data, was "utrc-0.0.6.tar", last modified: Sat Apr 13 19:45:50 2024, max compression
```

## Comparing `utrc-0.0.5.tar` & `utrc-0.0.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 19:36:25.846319 utrc-0.0.5/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2024-02-26 19:42:52.000000 utrc-0.0.5/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2024-02-26 19:42:52.000000 utrc-0.0.5/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     3883 2024-04-06 19:36:25.846086 utrc-0.0.5/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     2720 2024-03-14 20:37:52.000000 utrc-0.0.5/README.md
--rw-r--r--   0 solst      (501) staff       (20)      932 2024-04-06 19:36:12.000000 utrc-0.0.5/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-06 19:36:25.846364 utrc-0.0.5/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2585 2024-02-26 19:42:52.000000 utrc-0.0.5/setup.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 19:36:25.844037 utrc-0.0.5/utrc/
--rw-r--r--   0 solst      (501) staff       (20)      980 2024-04-06 19:36:14.000000 utrc-0.0.5/utrc/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    23626 2024-04-06 19:36:14.000000 utrc-0.0.5/utrc/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     3146 2024-04-06 19:36:14.000000 utrc-0.0.5/utrc/attr.py
--rw-r--r--   0 solst      (501) staff       (20)     7771 2024-04-06 19:36:14.000000 utrc-0.0.5/utrc/atyp.py
--rw-r--r--   0 solst      (501) staff       (20)     3481 2024-04-06 19:36:14.000000 utrc-0.0.5/utrc/bend.py
--rw-r--r--   0 solst      (501) staff       (20)    10268 2024-04-04 17:50:33.000000 utrc-0.0.5/utrc/cols.py
--rw-r--r--   0 solst      (501) staff       (20)     1360 2024-04-06 19:36:14.000000 utrc-0.0.5/utrc/cons.py
--rw-r--r--   0 solst      (501) staff       (20)     1285 2024-04-06 19:36:14.000000 utrc-0.0.5/utrc/data.py
--rw-r--r--   0 solst      (501) staff       (20)     8477 2024-04-06 19:36:14.000000 utrc-0.0.5/utrc/diff.py
--rw-r--r--   0 solst      (501) staff       (20)    13575 2024-04-06 19:36:14.000000 utrc-0.0.5/utrc/dims.py
--rw-r--r--   0 solst      (501) staff       (20)     7586 2024-04-06 19:36:14.000000 utrc-0.0.5/utrc/init.py
--rw-r--r--   0 solst      (501) staff       (20)    32638 2024-04-06 19:36:14.000000 utrc-0.0.5/utrc/kwds.py
--rw-r--r--   0 solst      (501) staff       (20)     1226 2024-04-06 19:36:14.000000 utrc-0.0.5/utrc/logs.py
--rw-r--r--   0 solst      (501) staff       (20)     6563 2024-04-06 19:36:14.000000 utrc-0.0.5/utrc/loss.py
--rw-r--r--   0 solst      (501) staff       (20)     7568 2024-04-06 19:36:14.000000 utrc-0.0.5/utrc/misc.py
--rw-r--r--   0 solst      (501) staff       (20)    12556 2024-04-04 19:18:05.000000 utrc-0.0.5/utrc/pand.py
--rw-r--r--   0 solst      (501) staff       (20)     6391 2024-04-06 14:04:05.000000 utrc-0.0.5/utrc/perc.py
--rw-r--r--   0 solst      (501) staff       (20)     2198 2024-04-06 14:04:05.000000 utrc-0.0.5/utrc/seed.py
--rw-r--r--   0 solst      (501) staff       (20)     6822 2024-04-06 19:36:14.000000 utrc-0.0.5/utrc/smpl.py
--rw-r--r--   0 solst      (501) staff       (20)     2449 2024-04-06 19:36:14.000000 utrc-0.0.5/utrc/strs.py
--rw-r--r--   0 solst      (501) staff       (20)     9168 2024-04-06 19:36:14.000000 utrc-0.0.5/utrc/tens.py
--rw-r--r--   0 solst      (501) staff       (20)     1087 2024-04-06 19:36:14.000000 utrc-0.0.5/utrc/util.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 19:36:25.844979 utrc-0.0.5/utrc.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     3883 2024-04-06 19:36:25.000000 utrc-0.0.5/utrc.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      541 2024-04-06 19:36:25.000000 utrc-0.0.5/utrc.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-06 19:36:25.000000 utrc-0.0.5/utrc.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-06 19:36:25.000000 utrc-0.0.5/utrc.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-08 15:51:50.000000 utrc-0.0.5/utrc.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)      149 2024-04-06 19:36:25.000000 utrc-0.0.5/utrc.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-06 19:36:25.000000 utrc-0.0.5/utrc.egg-info/top_level.txt
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-13 19:45:50.587946 utrc-0.0.6/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2024-02-26 19:42:52.000000 utrc-0.0.6/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2024-02-26 19:42:52.000000 utrc-0.0.6/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     3883 2024-04-13 19:45:50.587704 utrc-0.0.6/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     2720 2024-03-14 20:37:52.000000 utrc-0.0.6/README.md
+-rw-r--r--   0 solst      (501) staff       (20)      932 2024-04-06 19:37:05.000000 utrc-0.0.6/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-13 19:45:50.587991 utrc-0.0.6/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2585 2024-02-26 19:42:52.000000 utrc-0.0.6/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-13 19:45:50.585382 utrc-0.0.6/utrc/
+-rw-r--r--   0 solst      (501) staff       (20)      980 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    24386 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     3146 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/attr.py
+-rw-r--r--   0 solst      (501) staff       (20)     7771 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/atyp.py
+-rw-r--r--   0 solst      (501) staff       (20)     3481 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/bend.py
+-rw-r--r--   0 solst      (501) staff       (20)    10268 2024-04-04 17:50:33.000000 utrc-0.0.6/utrc/cols.py
+-rw-r--r--   0 solst      (501) staff       (20)     1360 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/cons.py
+-rw-r--r--   0 solst      (501) staff       (20)     1285 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/data.py
+-rw-r--r--   0 solst      (501) staff       (20)     8477 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/diff.py
+-rw-r--r--   0 solst      (501) staff       (20)    13575 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/dims.py
+-rw-r--r--   0 solst      (501) staff       (20)     7586 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/init.py
+-rw-r--r--   0 solst      (501) staff       (20)    33611 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/kwds.py
+-rw-r--r--   0 solst      (501) staff       (20)     1226 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/logs.py
+-rw-r--r--   0 solst      (501) staff       (20)     6563 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/loss.py
+-rw-r--r--   0 solst      (501) staff       (20)     9046 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/misc.py
+-rw-r--r--   0 solst      (501) staff       (20)    12556 2024-04-04 19:18:05.000000 utrc-0.0.6/utrc/pand.py
+-rw-r--r--   0 solst      (501) staff       (20)     6391 2024-04-06 14:04:05.000000 utrc-0.0.6/utrc/perc.py
+-rw-r--r--   0 solst      (501) staff       (20)     2198 2024-04-06 14:04:05.000000 utrc-0.0.6/utrc/seed.py
+-rw-r--r--   0 solst      (501) staff       (20)     6822 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/smpl.py
+-rw-r--r--   0 solst      (501) staff       (20)     2449 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/strs.py
+-rw-r--r--   0 solst      (501) staff       (20)     9168 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/tens.py
+-rw-r--r--   0 solst      (501) staff       (20)     1250 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/util.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-13 19:45:50.586661 utrc-0.0.6/utrc.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     3883 2024-04-13 19:45:50.000000 utrc-0.0.6/utrc.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      541 2024-04-13 19:45:50.000000 utrc-0.0.6/utrc.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-13 19:45:50.000000 utrc-0.0.6/utrc.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-13 19:45:50.000000 utrc-0.0.6/utrc.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-08 15:51:50.000000 utrc-0.0.6/utrc.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)      149 2024-04-13 19:45:50.000000 utrc-0.0.6/utrc.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-13 19:45:50.000000 utrc-0.0.6/utrc.egg-info/top_level.txt
```

### Comparing `utrc-0.0.5/LICENSE` & `utrc-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `utrc-0.0.5/PKG-INFO` & `utrc-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utrc
-Version: 0.0.5
+Version: 0.0.6
 Summary: util torch
 Home-page: https://github.com/dsm-72/utrc
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: utility for pytorch torch util utrc
 Classifier: Development Status :: 4 - Beta
```

### Comparing `utrc-0.0.5/README.md` & `utrc-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `utrc-0.0.5/settings.ini` & `utrc-0.0.6/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = utrc
 lib_name = utrc
-version = 0.0.5
+version = 0.0.6
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = utrc
 nbs_path = nbs
 recursive = True
```

### Comparing `utrc-0.0.5/setup.py` & `utrc-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.5/utrc/__init__.py` & `utrc-0.0.6/utrc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00__init__.ipynb.
 
 # %% auto 0
 __all__ = []
 
 # %% ../nbs/00__init__.ipynb 3
 from itertools import chain
```

### Comparing `utrc-0.0.5/utrc/_modidx.py` & `utrc-0.0.6/utrc/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,14 +143,17 @@
                            'utrc.kwds.SDEKeywords.__init__': ('kwds.html#sdekeywords.__init__', 'utrc/kwds.py'),
                            'utrc.kwds.SDEProblemKeywords': ('kwds.html#sdeproblemkeywords', 'utrc/kwds.py'),
                            'utrc.kwds.SDEProblemKeywords.__init__': ('kwds.html#sdeproblemkeywords.__init__', 'utrc/kwds.py'),
                            'utrc.kwds.SimpleKeywords': ('kwds.html#simplekeywords', 'utrc/kwds.py'),
                            'utrc.kwds.SimpleKeywords.__init__': ('kwds.html#simplekeywords.__init__', 'utrc/kwds.py'),
                            'utrc.kwds.SubVidInfo': ('kwds.html#subvidinfo', 'utrc/kwds.py'),
                            'utrc.kwds.SubVidInfo.__init__': ('kwds.html#subvidinfo.__init__', 'utrc/kwds.py'),
+                           'utrc.kwds.TorchDiffEQIntegrationKeywords': ('kwds.html#torchdiffeqintegrationkeywords', 'utrc/kwds.py'),
+                           'utrc.kwds.TorchDiffEQIntegrationKeywords.__init__': ( 'kwds.html#torchdiffeqintegrationkeywords.__init__',
+                                                                                  'utrc/kwds.py'),
                            'utrc.kwds.VidInfo': ('kwds.html#vidinfo', 'utrc/kwds.py'),
                            'utrc.kwds.VidInfo.__init__': ('kwds.html#vidinfo.__init__', 'utrc/kwds.py')},
             'utrc.logs': { 'utrc.logs.TorchMessage': ('logs.html#torchmessage', 'utrc/logs.py'),
                            'utrc.logs.TorchMessage.__init__': ('logs.html#torchmessage.__init__', 'utrc/logs.py')},
             'utrc.loss': { 'utrc.loss.AutoEncoderLoss': ('loss.html#autoencoderloss', 'utrc/loss.py'),
                            'utrc.loss.AutoEncoderLoss.__call__': ('loss.html#autoencoderloss.__call__', 'utrc/loss.py'),
                            'utrc.loss.AutoEncoderLoss.__init__': ('loss.html#autoencoderloss.__init__', 'utrc/loss.py'),
@@ -171,22 +174,25 @@
                            'utrc.loss.MMDLoss.guassian_kernel': ('loss.html#mmdloss.guassian_kernel', 'utrc/loss.py'),
                            'utrc.loss.OptimalTransportLoss': ('loss.html#optimaltransportloss', 'utrc/loss.py'),
                            'utrc.loss.OptimalTransportLoss.__call__': ('loss.html#optimaltransportloss.__call__', 'utrc/loss.py'),
                            'utrc.loss.OptimalTransportLoss.__init__': ('loss.html#optimaltransportloss.__init__', 'utrc/loss.py')},
             'utrc.misc': { 'utrc.misc.calcgrid': ('misc.html#calcgrid', 'utrc/misc.py'),
                            'utrc.misc.drop_column': ('misc.html#drop_column', 'utrc/misc.py'),
                            'utrc.misc.drop_named_index': ('misc.html#drop_named_index', 'utrc/misc.py'),
+                           'utrc.misc.generate_pairs': ('misc.html#generate_pairs', 'utrc/misc.py'),
+                           'utrc.misc.generate_spans': ('misc.html#generate_spans', 'utrc/misc.py'),
                            'utrc.misc.generate_steps': ('misc.html#generate_steps', 'utrc/misc.py'),
                            'utrc.misc.get_categories': ('misc.html#get_categories', 'utrc/misc.py'),
                            'utrc.misc.grididx': ('misc.html#grididx', 'utrc/misc.py'),
                            'utrc.misc.groupget': ('misc.html#groupget', 'utrc/misc.py'),
                            'utrc.misc.grouplens': ('misc.html#grouplens', 'utrc/misc.py'),
                            'utrc.misc.increment_pairs': ('misc.html#increment_pairs', 'utrc/misc.py'),
                            'utrc.misc.pad4grid': ('misc.html#pad4grid', 'utrc/misc.py'),
                            'utrc.misc.pair': ('misc.html#pair', 'utrc/misc.py'),
+                           'utrc.misc.spans': ('misc.html#spans', 'utrc/misc.py'),
                            'utrc.misc.steps': ('misc.html#steps', 'utrc/misc.py'),
                            'utrc.misc.takekeys': ('misc.html#takekeys', 'utrc/misc.py')},
             'utrc.pand': { 'utrc.pand.as_categories': ('pand.html#as_categories', 'utrc/pand.py'),
                            'utrc.pand.column_as_category': ('pand.html#column_as_category', 'utrc/pand.py'),
                            'utrc.pand.drop_column': ('pand.html#drop_column', 'utrc/pand.py'),
                            'utrc.pand.drop_named_index': ('pand.html#drop_named_index', 'utrc/pand.py'),
                            'utrc.pand.extent': ('pand.html#extent', 'utrc/pand.py'),
@@ -230,8 +236,9 @@
                            'utrc.tens.pack': ('tens.html#pack', 'utrc/tens.py'),
                            'utrc.tens.pack_padded': ('tens.html#pack_padded', 'utrc/tens.py'),
                            'utrc.tens.pad': ('tens.html#pad', 'utrc/tens.py'),
                            'utrc.tens.sort_sequences': ('tens.html#sort_sequences', 'utrc/tens.py'),
                            'utrc.tens.torchnans': ('tens.html#torchnans', 'utrc/tens.py'),
                            'utrc.tens.unpack': ('tens.html#unpack', 'utrc/tens.py'),
                            'utrc.tens.unpadded_len': ('tens.html#unpadded_len', 'utrc/tens.py')},
-            'utrc.util': {'utrc.util.extent': ('util.html#extent', 'utrc/util.py')}}}
+            'utrc.util': { 'utrc.util.extent': ('util.html#extent', 'utrc/util.py'),
+                           'utrc.util.integration_steps': ('util.html#integration_steps', 'utrc/util.py')}}}
```

### Comparing `utrc-0.0.5/utrc/attr.py` & `utrc-0.0.6/utrc/attr.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.5/utrc/atyp.py` & `utrc-0.0.6/utrc/atyp.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.5/utrc/bend.py` & `utrc-0.0.6/utrc/bend.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.5/utrc/cols.py` & `utrc-0.0.6/utrc/cols.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.5/utrc/cons.py` & `utrc-0.0.6/utrc/cons.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.5/utrc/data.py` & `utrc-0.0.6/utrc/data.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.5/utrc/diff.py` & `utrc-0.0.6/utrc/diff.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.5/utrc/dims.py` & `utrc-0.0.6/utrc/dims.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.5/utrc/init.py` & `utrc-0.0.6/utrc/init.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.5/utrc/kwds.py` & `utrc-0.0.6/utrc/kwds.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/03_kwds.ipynb.
 
 # %% auto 0
-__all__ = ['NeuralKeywords', 'AugmenterKeywords', 'SimpleKeywords', 'DynamicsForwardKeywords', 'DynamicsKeywords',
-           'NeuralOptimalTransportKeywords', 'DifferentialEquationKeywords', 'ODEKeywords', 'SDEFunctionKeywords',
-           'SDEProblemKeywords', 'SDEKeywords', 'SubVidInfo', 'VidInfo', 'DiffusionKeywords', 'BaseRecurrentKeywords',
-           'LSTMKeywords', 'RNNKeywords', 'RecurrentKeywords', 'RecurrentAutoEncoderKeywords',
+__all__ = ['TorchDiffEQIntegrationKeywords', 'NeuralKeywords', 'AugmenterKeywords', 'SimpleKeywords', 'DynamicsForwardKeywords',
+           'DynamicsKeywords', 'NeuralOptimalTransportKeywords', 'DifferentialEquationKeywords', 'ODEKeywords',
+           'SDEFunctionKeywords', 'SDEProblemKeywords', 'SDEKeywords', 'SubVidInfo', 'VidInfo', 'DiffusionKeywords',
+           'BaseRecurrentKeywords', 'LSTMKeywords', 'RNNKeywords', 'RecurrentKeywords', 'RecurrentAutoEncoderKeywords',
            'RecurrentEncoderKeywords', 'RecurrentDecoderKeywords']
 
 # %% ../nbs/03_kwds.ipynb 6
 from functools import wraps
 
 # %% ../nbs/03_kwds.ipynb 8
 from typing import (
@@ -40,15 +40,40 @@
 )
 
 _TYPE_DICT_KWDS = dict(
     __ignore_values  = _IGNORE_INIT,
     __force_defaults = False
 )
 
-# %% ../nbs/03_kwds.ipynb 19
+# %% ../nbs/03_kwds.ipynb 18
+class TorchDiffEQIntegrationKeywords(TypeDict, **_TYPE_DICT_KWDS):
+    '''Typed dictionary for initalizing a neural network.
+    
+    Attributes
+    ----------
+    device : device | str, optional
+        The device to use for computation.
+    '''
+    rtol: float = 1e-7
+    atol: float = 1e-9
+    method: str | None = None
+    options: dict | None = None
+    event_fn: Callable | None = None
+    adjoint_rtol: float | None = None
+    adjoint_atol: float | None = None
+    adjoint_method: str | None = None
+    adjoint_options: dict | None = None
+    adjoint_params: dict | None = None
+    @overload
+    def __init__(self, device: deviceq) -> 'TorchDiffEQIntegrationKeywords': ...
+    def __init__(self, *args, **kwargs: 'TorchDiffEQIntegrationKeywords') -> 'TorchDiffEQIntegrationKeywords':
+        '''Typed dictionary for initalizing a neural network.'''
+        return super().__init__(self, *(), **kwargs)
+
+# %% ../nbs/03_kwds.ipynb 21
 class NeuralKeywords(TypeDict, **_TYPE_DICT_KWDS):
     '''Typed dictionary for initalizing a neural network.
     
     Attributes
     ----------
     device : device | str, optional
         The device to use for computation.
@@ -57,15 +82,15 @@
     
     @overload
     def __init__(self, device: deviceq) -> 'NeuralKeywords': ...
     def __init__(self, *args, **kwargs: 'NeuralKeywords') -> 'NeuralKeywords':
         '''Typed dictionary for initalizing a neural network.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 22
+# %% ../nbs/03_kwds.ipynb 24
 class AugmenterKeywords(TypeDict, **_TYPE_DICT_KWDS):
     '''Typed dictionary for initalizing an Augmenter.
     
     Attributes
     ----------
     adim : int, optional
         The number of augmenting dimensions.
@@ -78,15 +103,15 @@
     
     @overload
     def __init__(self, adim: intq, afnc: Callable | None) -> 'AugmenterKeywords': ...
     def __init__(self, *args, **kwargs: 'AugmenterKeywords') -> 'AugmenterKeywords':
         '''Typed dictionary for initalizing an Augmenter.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 25
+# %% ../nbs/03_kwds.ipynb 27
 class SimpleKeywords(NeuralKeywords, **_TYPE_DICT_KWDS):
     '''Typed dictionary for initalizing a Simple Neural Network.
     
     Attributes
     ----------
     feats : list[int]
         The number of features per linear layer e.g. [10, 10]
@@ -138,15 +163,15 @@
         outkws: dict,
         device: deviceq
     ) -> 'SimpleKeywords': ...
     def __init__(self, *args, **kwargs: 'SimpleKeywords') -> 'SimpleKeywords':
         '''Typed dictionary for initalizing a Simple Neural Network.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 29
+# %% ../nbs/03_kwds.ipynb 31
 class DynamicsForwardKeywords(TypeDict, **_TYPE_DICT_KWDS):
     '''Typed dictionary for the forward call of a `torchdyn.nn.Module`.
     
     Attributes
     ----------
     x : tensor
     
@@ -192,15 +217,15 @@
         useaug: bool, 
         usedec: bool,
     ) -> 'DynamicsForwardKeywords': ...
     def __init__(self, *args, **kwargs: 'DynamicsForwardKeywords') -> 'DynamicsForwardKeywords':
         '''Typed dictionary for the forward call of a `torchdyn.nn.Module`.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 32
+# %% ../nbs/03_kwds.ipynb 34
 class DynamicsKeywords(AugmenterKeywords, NeuralKeywords, **_TYPE_DICT_KWDS):
     '''Typed dictionary for initalizing a Dynamic Neural Network.
     
     Attributes
     ----------
     diffeq : DynamicsMethod 
         The dynamics method to use e.g. DynamicsMethod.NeuralODE, DynamicsMethod.NeuralSDE
@@ -243,15 +268,15 @@
         tsteps: tensor,
         **kwargs: AugmenterKeywords | NeuralKeywords
     ): ...
     def __init__(self, *args, **kwargs: 'DynamicsForwardKeywords') -> 'DynamicsForwardKeywords':
         '''Typed dictionary for initalizing a Dynamic Neural Network.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 35
+# %% ../nbs/03_kwds.ipynb 37
 class NeuralOptimalTransportKeywords(SimpleKeywords, DynamicsKeywords, AugmenterKeywords, NeuralKeywords, **_TYPE_DICT_KWDS):
     '''Typed dictionary for initalizing an Optimal Transport Neural Network.
     
     Attributes
     ----------
     topk: int
         number of top predictions to consider
@@ -320,15 +345,15 @@
         topk: int,
         **kwargs: DynamicsKeywords | AugmenterKeywords | NeuralKeywords
     ): ...
     def __init__(self, *args, **kwargs: 'NeuralOptimalTransportKeywords') -> 'NeuralOptimalTransportKeywords':
         '''Typed dictionary for initalizing an Optimal Transport Neural Network.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 38
+# %% ../nbs/03_kwds.ipynb 40
 class DifferentialEquationKeywords(TypeDict, **_TYPE_DICT_KWDS):
     '''Typed dictionary for initalizing a Differential Equation.
     
     Attributes
     ----------
     order: Optional[int], default: 1
         order of the differential equation. Defaults to 1.
@@ -365,15 +390,15 @@
         sensitivity: str,
         return_t_eval: bool,
     ): ...
     def __init__(self, *args, **kwargs: 'DifferentialEquationKeywords') -> 'DifferentialEquationKeywords':
         '''Typed dictionary for initalizing a Differential Equation.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 42
+# %% ../nbs/03_kwds.ipynb 44
 class ODEKeywords(DifferentialEquationKeywords, **_TYPE_DICT_KWDS):
     '''Typed dictionary for initalizing an Ordinary Differential Equation.
     
     Attributes
     ----------
     vector_field: Union[Solver, str, nnmodule]
         Defaults to Solver.EulerODE.
@@ -449,15 +474,15 @@
         optimizable_params: Union[Iterable, Generator],
         **kwargs: DifferentialEquationKeywords
     ): ...
     def __init__(self, *args, **kwargs: 'ODEKeywords') -> 'ODEKeywords':
         '''Typed dictionary for initalizing an Ordinary Differential Equation.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 46
+# %% ../nbs/03_kwds.ipynb 48
 class SDEFunctionKeywords(TypeDict, **_TYPE_DICT_KWDS):
     '''Typed dictionary for initalizing a SDE function.
     
     Attributes
     ----------
     drift_func: Callable
         drift function, i.e. f (Callable): callable defining the drift
@@ -488,15 +513,15 @@
         noise_type: SDENoiseType,
         sde_type: Optional[SolverKind],
     ): ...
     def __init__(self, *args, **kwargs: 'SDEFunctionKeywords') -> 'SDEFunctionKeywords':
         '''Typed dictionary for initalizing a SDE function.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 49
+# %% ../nbs/03_kwds.ipynb 51
 class SDEProblemKeywords(TypeDict, **_TYPE_DICT_KWDS):
     '''Typed dictionary for initalizing a SDE Problem function.
     
     Attributes
     ----------
     defunc: sdefunc
         The differnetial equation function e.g. 
@@ -508,15 +533,15 @@
         self, 
         defunc: sdefunc,
     ): ...
     def __init__(self, *args, **kwargs: 'SDEProblemKeywords') -> 'SDEProblemKeywords':
         '''Typed dictionary for initalizing a SDE Problem function.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 52
+# %% ../nbs/03_kwds.ipynb 54
 class SDEKeywords(SDEFunctionKeywords, DifferentialEquationKeywords, **_TYPE_DICT_KWDS):
     '''Typed dictionary for initalizing a Stochastic Differential Equation.
     
     Attributes
     ----------
     t_span: Optional[list[int]]
         Defaults to torch.linspace(0, 1, 2).
@@ -632,15 +657,15 @@
         bm: Optional[brownianintervial],
         **kwargs: SDEFunctionKeywords | DifferentialEquationKeywords
     ): ...
     def __init__(self, *args, **kwargs: 'SDEKeywords') -> 'SDEKeywords':
         '''Typed dictionary for initalizing a Stochastic Differential Equation.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 56
+# %% ../nbs/03_kwds.ipynb 58
 class SubVidInfo(TypeDict, **_TYPE_DICT_KWDS):
     '''Subvideo Information from an AVI file'''
     pos: xypos
     '''The (row, col) position of the subvideo in the grid'''
     bbox: BBox
     '''The bounding box of the subvideo in the grid'''
     subidx: int
@@ -655,15 +680,15 @@
         subidx: int,
         subkey: str
     ): ...
     def __init__(self, *args, **kwargs: 'SubVidInfo') -> 'SubVidInfo':
         '''Typed dictionary containing Subvideo Information from an AVI file.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 59
+# %% ../nbs/03_kwds.ipynb 61
 class VidInfo(TypeDict, **_TYPE_DICT_KWDS):
     '''AVI file information'''
     vidpxs: rect
     '''The frame size (width, height) of the video e.g. (1200, 1200)'''
     subpxs: rect
     '''The standardized subvideo size (sub-width, sub-height) e.g. (400, 400)'''
     values: list[dict[str, SubVidInfo]]
@@ -679,15 +704,15 @@
         values: list[dict[str, SubVidInfo]], 
         source: path
     ): ...
     def __init__(self, *args, **kwargs: 'VidInfo') -> 'VidInfo':
         '''Typed dictionary containing AVI file information.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 63
+# %% ../nbs/03_kwds.ipynb 65
 class DiffusionKeywords(TypeDict, **_TYPE_DICT_KWDS):
     '''Typed dictionary for initalizing a Diffusion Operation Method.'''
     knn: int = 5
     tmax: int = 5
     anisotropy: int = 1
     tdiff: int = 1
     topeig: int = 100
@@ -715,15 +740,15 @@
         njobs: int,
         device: deviceq
     ): ...
     def __init__(self, *args, **kwargs: 'DiffusionKeywords') -> 'DiffusionKeywords':
         '''Typed dictionary for initalizing a Diffusion Operation Method.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 67
+# %% ../nbs/03_kwds.ipynb 69
 class BaseRecurrentKeywords(NeuralKeywords, **_TYPE_DICT_KWDS):
     '''Typed dictionary for specifying base keywords for recurrent neural network layers.
 
     Attributes
     ----------
     input_size : int
         The number of expected features in the input.
@@ -785,15 +810,15 @@
         device: deviceq,
         dtype: dtypeq
     ): ...
     def __init__(self, *args, **kwargs: 'BaseRecurrentKeywords') -> 'BaseRecurrentKeywords':
         '''Typed dictionary for specifying base keywords for recurrent neural network layers.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 71
+# %% ../nbs/03_kwds.ipynb 73
 class LSTMKeywords(BaseRecurrentKeywords, **_TYPE_DICT_KWDS):
     '''Typed dictionary for specifying keywords specific to LSTM layers, extending `BaseRecurrentKeywords`.
 
     Attributes
     ----------
     proj_size : int
         The size of the projection layer.
@@ -828,15 +853,15 @@
         proj_size: int,
         **kwargs: BaseRecurrentKeywords
     ): ...
     def __init__(self, *args, **kwargs: 'LSTMKeywords') -> 'LSTMKeywords':
         '''Typed dictionary for specifying keywords specific to LSTM layers, extending `BaseRecurrentKeywords`.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 74
+# %% ../nbs/03_kwds.ipynb 76
 class RNNKeywords(BaseRecurrentKeywords, **_TYPE_DICT_KWDS):    
     '''Typed dictionary for specifying keywords specific to RNN layers, extending `BaseRecurrentKeywords`.
 
     Attributes
     ----------
     nonlinearity : NonLinearity
         The non-linearity to use ('relu' or 'tanh').
@@ -871,15 +896,15 @@
         nonlinearity: NonLinearity,
         **kwargs: BaseRecurrentKeywords
     ): ...
     def __init__(self, *args, **kwargs: 'RNNKeywords') -> 'RNNKeywords':
         '''Typed dictionary for specifying keywords specific to RNN layers, extending `BaseRecurrentKeywords`.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 77
+# %% ../nbs/03_kwds.ipynb 79
 class RecurrentKeywords(LSTMKeywords, RNNKeywords, **_TYPE_DICT_KWDS): 
     '''Typed dictionary for specifying keywords for recurrent neural network layers, combining `LSTMKeywords` and `RNNKeywords`.
 
     Examples
     --------
     >>> recurrent_keywords = RecurrentKeywords(
     ...     input_size=64, hidden_size=128, nlays=2, proj_size=64, nonlinearity=NonLinearity.Tanh, 
@@ -920,15 +945,15 @@
     def __init__(
         self, *args, **kwargs: LSTMKeywords | RNNKeywords
     ): ...
     def __init__(self, *args, **kwargs: 'RecurrentKeywords') -> 'RecurrentKeywords':
         '''Typed dictionary for specifying keywords for recurrent neural network layers, combining `LSTMKeywords` and `RNNKeywords`.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 80
+# %% ../nbs/03_kwds.ipynb 82
 class RecurrentAutoEncoderKeywords(RecurrentKeywords, **_TYPE_DICT_KWDS):
     '''Typed dictionary for specifying keywords for recurrent autoencoder models, extending `RecurrentKeywords`.
 
     Attributes
     ----------
     output_size : int
         The size of the output layer.
@@ -1006,30 +1031,30 @@
         '''Typed dictionary for specifying keywords specific to RNN layers, extending `BaseRecurrentKeywords`.'''
         result, params = dict(), kwargs.copy()
         kind = params.pop(KIND, RecurrentLayer.LSTM)
         if RecurrentLayer(kind) != RecurrentLayer.RNN:  params.pop(NONLINEARITY, None)
         if RecurrentLayer(kind) != RecurrentLayer.LSTM: params.pop(PROJ_SIZE, None)
         return super().__init__(self, *args, **{**result, **params})
 
-# %% ../nbs/03_kwds.ipynb 83
+# %% ../nbs/03_kwds.ipynb 85
 class RecurrentEncoderKeywords(RecurrentAutoEncoderKeywords, **_TYPE_DICT_KWDS):
     def __init__(self, *args, **kwargs: 'RecurrentEncoderKeywords'):
         super().__init__(self, *args, **kwargs)
         input_size  = self.pop(INPUT_SIZE,  None)
         hidden_size = self.pop(HIDDEN_SIZE, None)
         output_size = self.pop(OUTPUT_SIZE, None)
         self.setdefault(INPUT_SIZE,  input_size or hidden_size)
         self.setdefault(HIDDEN_SIZE, output_size or hidden_size)
         
 
-# %% ../nbs/03_kwds.ipynb 86
+# %% ../nbs/03_kwds.ipynb 88
 class RecurrentDecoderKeywords(RecurrentAutoEncoderKeywords, **_TYPE_DICT_KWDS):
     def __init__(self, *args, **kwargs: 'RecurrentDecoderKeywords'):
         super().__init__(self, *args, **kwargs)
         input_size  = self.pop(INPUT_SIZE,  None)
         hidden_size = self.pop(HIDDEN_SIZE, None)
         output_size = self.pop(OUTPUT_SIZE, None)
         self.setdefault(HIDDEN_SIZE, input_size  or hidden_size)
         self.setdefault(OUTPUT_SIZE, output_size or hidden_size)
 
-# %% ../nbs/03_kwds.ipynb 89
+# %% ../nbs/03_kwds.ipynb 91
 #| export
```

### Comparing `utrc-0.0.5/utrc/logs.py` & `utrc-0.0.6/utrc/logs.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.5/utrc/loss.py` & `utrc-0.0.6/utrc/loss.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.5/utrc/misc.py` & `utrc-0.0.6/utrc/misc.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/10_misc.ipynb.
 
 # %% auto 0
 __all__ = ['drop_named_index', 'drop_column', 'groupget', 'grouplens', 'get_categories', 'pair', 'steps', 'increment_pairs',
-           'generate_steps', 'calcgrid', 'grididx', 'pad4grid', 'takekeys']
+           'generate_pairs', 'generate_steps', 'generate_spans', 'spans', 'calcgrid', 'grididx', 'pad4grid', 'takekeys']
 
 # %% ../nbs/10_misc.ipynb 6
 import math
 from functools import wraps, singledispatch
-from itertools import takewhile, count
+from itertools import takewhile, count, zip_longest
 
 # %% ../nbs/10_misc.ipynb 8
 from numbers import Number
 from typing import Generator, Iterator, Iterable, overload
 
 # %% ../nbs/10_misc.ipynb 11
 #| export
@@ -132,28 +132,45 @@
     '''Alias for `pair`.'''
     return pair(*args, **kwargs)
 
 @wraps(pair, assigned=WRAPS_ASSIGN_ANNDOCS)
 def increment_pairs(*args, **kwargs):
     return pair(*args, **kwargs)
 
+@wraps(pair, assigned=WRAPS_ASSIGN_ANNDOCS)
+def generate_pairs(*args, **kwargs):
+    return pair(*args, **kwargs)
+
 # %% ../nbs/10_misc.ipynb 28
-def generate_steps(incr, step, stop):
+@overload
+def generate_steps(stop: int, *, include_stop: bool = True): ...
+@overload
+def generate_steps(step: int , stop: int, *, include_stop: bool = True): ...
+@overload
+def generate_steps(incr: int, step: int, stop: int, *, include_stop: bool = True): ...
+@overload
+def generate_steps(init: int, incr: int, step: int, stop: int, *, include_stop: bool = True): ...
+def generate_steps(*args, include_stop: bool = True):
     '''
     Generate a list of tuples representing step intervals from 0 up to stop,
     incrementing by incr and ensuring each step interval does not exceed step.
     
     Parameters
     ----------
+    init : int, default: 0
+        The initial value to start at.
     incr : int
         The increment between each start of the step intervals.
     step : int
         The maximum allowed difference between the start and end of each interval.
     stop : int
         The stopping point for the generation of intervals.
+        
+    include_stop : bool, default: True
+        Whether or not to include the stop value in the incrementations
     
     Returns
     -------
     list of tuples
         A list of tuples, where each tuple contains the start and end of each step interval.
         
     Examples
@@ -173,23 +190,46 @@
     ... good_inc = all(e == incr for e in firstdiff)
 
     ... # each tuple increments by +incr, has a (a, b) diff of <= step and ends at stop
     ... all_valid = good_inc and good_step and good_end
     ... vals, all_valid
 
     '''
+    init, incr, step, stop = 0, 1, 1, 1 
+    match len(args):
+        case 0:
+            init, incr, step, stop = 0, 1, 1, 1 
+        case 1: 
+            stop = args
+        case 2: 
+            step, stop = args
+        case 3: 
+            incr, step, stop = args
+        case 4: 
+            init, incr, step, stop = args
+        case _:
+            init, incr, step, stop, *_ = args
+    
     # Use takewhile to generate values up to the stop condition
-    vals_gen = takewhile(lambda x: x < stop, count(0, incr))
+    vals_gen = takewhile(lambda x: x + init < stop, count(0, incr))
     
     # Generate the list of tuples with the specified conditions
-    vals = [(i, min(i + step, stop)) for i in vals_gen]
-    
+    vals = [((i + init), min((i + init) + step, (stop if include_stop else stop - 1))) for i in vals_gen]
     return vals
 
-# %% ../nbs/10_misc.ipynb 32
+# %% ../nbs/10_misc.ipynb 30
+@wraps(generate_steps, assigned=WRAPS_ASSIGN_ANNDOCS)
+def generate_spans(*args, **kwargs):
+    return generate_steps(*args, **kwargs)
+
+@wraps(generate_steps, assigned=WRAPS_ASSIGN_ANNDOCS)
+def spans(*args, **kwargs):
+    return generate_steps(*args, **kwargs)
+
+# %% ../nbs/10_misc.ipynb 33
 def calcgrid(n: int) -> rect:
     '''
     Find the closest rectangle layout that accommodates n elements.
 
     Parameters
     ----------
     n : int
@@ -201,15 +241,15 @@
         A tuple representing the dimensions (rows, cols) of the grid.
     '''
     x = math.isqrt(n)
     while n % x != 0: x -= 1
     y = n // x
     return x, y
 
-# %% ../nbs/10_misc.ipynb 34
+# %% ../nbs/10_misc.ipynb 35
 def grididx(pos: xypos, grid: rect) -> int:
     '''
     Calculate the linear index of an element in a `grid` given its `(row, col)` position (`pos`).
 
     Parameters
     ----------
     pos : XYPos
@@ -222,15 +262,15 @@
     int
         The linear index of the element in the grid.
     '''
     nrows, ncols = grid
     cur_r, cur_c = pos
     return cur_r * ncols + cur_c
 
-# %% ../nbs/10_misc.ipynb 36
+# %% ../nbs/10_misc.ipynb 37
 @overload
 def pad4grid(arr: list, rows: int, cols: int) -> list: ...
 @overload
 def pad4grid(arr: list, n: int) -> list: ...
 def pad4grid(arr: list, *args) -> list:
     '''
     Pad the list of objects to the closest grid layout that accommodates a specified number of elements.
@@ -246,15 +286,15 @@
     -------
     list
         The padded list.
     '''
     rows, cols = args[0], (1 if len(args) <= 1 else args[1])
     return list(fillnone(arr, rows * cols))
 
-# %% ../nbs/10_misc.ipynb 38
+# %% ../nbs/10_misc.ipynb 39
 def takekeys(d: dict, keys: list | dict) -> dict:
     keys = keys or []
     if isdict(keys): keys = keys.keys()
     return {k: d.get(k, None) for k in keys if k in d}
 
-# %% ../nbs/10_misc.ipynb 40
+# %% ../nbs/10_misc.ipynb 41
 #| export
```

### Comparing `utrc-0.0.5/utrc/pand.py` & `utrc-0.0.6/utrc/pand.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.5/utrc/perc.py` & `utrc-0.0.6/utrc/perc.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.5/utrc/seed.py` & `utrc-0.0.6/utrc/seed.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.5/utrc/smpl.py` & `utrc-0.0.6/utrc/smpl.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.5/utrc/strs.py` & `utrc-0.0.6/utrc/strs.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.5/utrc/tens.py` & `utrc-0.0.6/utrc/tens.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.5/utrc.egg-info/PKG-INFO` & `utrc-0.0.6/utrc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utrc
-Version: 0.0.5
+Version: 0.0.6
 Summary: util torch
 Home-page: https://github.com/dsm-72/utrc
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: utility for pytorch torch util utrc
 Classifier: Development Status :: 4 - Beta
```

### Comparing `utrc-0.0.5/utrc.egg-info/SOURCES.txt` & `utrc-0.0.6/utrc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

