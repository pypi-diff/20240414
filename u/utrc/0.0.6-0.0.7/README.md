# Comparing `tmp/utrc-0.0.6.tar.gz` & `tmp/utrc-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utrc-0.0.6.tar", last modified: Sat Apr 13 19:45:50 2024, max compression
+gzip compressed data, was "utrc-0.0.7.tar", last modified: Sun Apr 14 11:24:24 2024, max compression
```

## Comparing `utrc-0.0.6.tar` & `utrc-0.0.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-13 19:45:50.587946 utrc-0.0.6/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2024-02-26 19:42:52.000000 utrc-0.0.6/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2024-02-26 19:42:52.000000 utrc-0.0.6/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     3883 2024-04-13 19:45:50.587704 utrc-0.0.6/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     2720 2024-03-14 20:37:52.000000 utrc-0.0.6/README.md
--rw-r--r--   0 solst      (501) staff       (20)      932 2024-04-06 19:37:05.000000 utrc-0.0.6/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-13 19:45:50.587991 utrc-0.0.6/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2585 2024-02-26 19:42:52.000000 utrc-0.0.6/setup.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-13 19:45:50.585382 utrc-0.0.6/utrc/
--rw-r--r--   0 solst      (501) staff       (20)      980 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    24386 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     3146 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/attr.py
--rw-r--r--   0 solst      (501) staff       (20)     7771 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/atyp.py
--rw-r--r--   0 solst      (501) staff       (20)     3481 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/bend.py
--rw-r--r--   0 solst      (501) staff       (20)    10268 2024-04-04 17:50:33.000000 utrc-0.0.6/utrc/cols.py
--rw-r--r--   0 solst      (501) staff       (20)     1360 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/cons.py
--rw-r--r--   0 solst      (501) staff       (20)     1285 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/data.py
--rw-r--r--   0 solst      (501) staff       (20)     8477 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/diff.py
--rw-r--r--   0 solst      (501) staff       (20)    13575 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/dims.py
--rw-r--r--   0 solst      (501) staff       (20)     7586 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/init.py
--rw-r--r--   0 solst      (501) staff       (20)    33611 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/kwds.py
--rw-r--r--   0 solst      (501) staff       (20)     1226 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/logs.py
--rw-r--r--   0 solst      (501) staff       (20)     6563 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/loss.py
--rw-r--r--   0 solst      (501) staff       (20)     9046 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/misc.py
--rw-r--r--   0 solst      (501) staff       (20)    12556 2024-04-04 19:18:05.000000 utrc-0.0.6/utrc/pand.py
--rw-r--r--   0 solst      (501) staff       (20)     6391 2024-04-06 14:04:05.000000 utrc-0.0.6/utrc/perc.py
--rw-r--r--   0 solst      (501) staff       (20)     2198 2024-04-06 14:04:05.000000 utrc-0.0.6/utrc/seed.py
--rw-r--r--   0 solst      (501) staff       (20)     6822 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/smpl.py
--rw-r--r--   0 solst      (501) staff       (20)     2449 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/strs.py
--rw-r--r--   0 solst      (501) staff       (20)     9168 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/tens.py
--rw-r--r--   0 solst      (501) staff       (20)     1250 2024-04-13 19:45:42.000000 utrc-0.0.6/utrc/util.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-13 19:45:50.586661 utrc-0.0.6/utrc.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     3883 2024-04-13 19:45:50.000000 utrc-0.0.6/utrc.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      541 2024-04-13 19:45:50.000000 utrc-0.0.6/utrc.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-13 19:45:50.000000 utrc-0.0.6/utrc.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-13 19:45:50.000000 utrc-0.0.6/utrc.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-08 15:51:50.000000 utrc-0.0.6/utrc.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)      149 2024-04-13 19:45:50.000000 utrc-0.0.6/utrc.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-13 19:45:50.000000 utrc-0.0.6/utrc.egg-info/top_level.txt
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-14 11:24:24.885276 utrc-0.0.7/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2024-02-26 19:42:52.000000 utrc-0.0.7/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2024-02-26 19:42:52.000000 utrc-0.0.7/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     3883 2024-04-14 11:24:24.885029 utrc-0.0.7/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     2720 2024-03-14 20:37:52.000000 utrc-0.0.7/README.md
+-rw-r--r--   0 solst      (501) staff       (20)      932 2024-04-13 19:46:36.000000 utrc-0.0.7/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-14 11:24:24.885319 utrc-0.0.7/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2585 2024-02-26 19:42:52.000000 utrc-0.0.7/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-14 11:24:24.882751 utrc-0.0.7/utrc/
+-rw-r--r--   0 solst      (501) staff       (20)      980 2024-04-14 11:23:46.000000 utrc-0.0.7/utrc/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    24786 2024-04-14 11:23:46.000000 utrc-0.0.7/utrc/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     3146 2024-04-14 11:23:46.000000 utrc-0.0.7/utrc/attr.py
+-rw-r--r--   0 solst      (501) staff       (20)     7932 2024-04-14 11:23:46.000000 utrc-0.0.7/utrc/atyp.py
+-rw-r--r--   0 solst      (501) staff       (20)     3481 2024-04-14 11:23:46.000000 utrc-0.0.7/utrc/bend.py
+-rw-r--r--   0 solst      (501) staff       (20)    10268 2024-04-04 17:50:33.000000 utrc-0.0.7/utrc/cols.py
+-rw-r--r--   0 solst      (501) staff       (20)     1360 2024-04-14 11:23:46.000000 utrc-0.0.7/utrc/cons.py
+-rw-r--r--   0 solst      (501) staff       (20)     1285 2024-04-14 11:23:46.000000 utrc-0.0.7/utrc/data.py
+-rw-r--r--   0 solst      (501) staff       (20)     8477 2024-04-14 11:23:46.000000 utrc-0.0.7/utrc/diff.py
+-rw-r--r--   0 solst      (501) staff       (20)    13575 2024-04-14 11:23:46.000000 utrc-0.0.7/utrc/dims.py
+-rw-r--r--   0 solst      (501) staff       (20)     7586 2024-04-14 11:23:46.000000 utrc-0.0.7/utrc/init.py
+-rw-r--r--   0 solst      (501) staff       (20)    33611 2024-04-14 11:23:46.000000 utrc-0.0.7/utrc/kwds.py
+-rw-r--r--   0 solst      (501) staff       (20)     1226 2024-04-14 11:23:46.000000 utrc-0.0.7/utrc/logs.py
+-rw-r--r--   0 solst      (501) staff       (20)     6563 2024-04-14 11:23:46.000000 utrc-0.0.7/utrc/loss.py
+-rw-r--r--   0 solst      (501) staff       (20)     9046 2024-04-14 11:23:46.000000 utrc-0.0.7/utrc/misc.py
+-rw-r--r--   0 solst      (501) staff       (20)    12556 2024-04-04 19:18:05.000000 utrc-0.0.7/utrc/pand.py
+-rw-r--r--   0 solst      (501) staff       (20)     6391 2024-04-06 14:04:05.000000 utrc-0.0.7/utrc/perc.py
+-rw-r--r--   0 solst      (501) staff       (20)     2198 2024-04-06 14:04:05.000000 utrc-0.0.7/utrc/seed.py
+-rw-r--r--   0 solst      (501) staff       (20)     6822 2024-04-14 11:23:46.000000 utrc-0.0.7/utrc/smpl.py
+-rw-r--r--   0 solst      (501) staff       (20)     2449 2024-04-14 11:23:46.000000 utrc-0.0.7/utrc/strs.py
+-rw-r--r--   0 solst      (501) staff       (20)     9168 2024-04-14 11:23:46.000000 utrc-0.0.7/utrc/tens.py
+-rw-r--r--   0 solst      (501) staff       (20)     5808 2024-04-14 11:23:46.000000 utrc-0.0.7/utrc/util.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-14 11:24:24.883819 utrc-0.0.7/utrc.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     3883 2024-04-14 11:24:24.000000 utrc-0.0.7/utrc.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      541 2024-04-14 11:24:24.000000 utrc-0.0.7/utrc.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-14 11:24:24.000000 utrc-0.0.7/utrc.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2024-04-14 11:24:24.000000 utrc-0.0.7/utrc.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-08 15:51:50.000000 utrc-0.0.7/utrc.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)      149 2024-04-14 11:24:24.000000 utrc-0.0.7/utrc.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2024-04-14 11:24:24.000000 utrc-0.0.7/utrc.egg-info/top_level.txt
```

### Comparing `utrc-0.0.6/LICENSE` & `utrc-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `utrc-0.0.6/PKG-INFO` & `utrc-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utrc
-Version: 0.0.6
+Version: 0.0.7
 Summary: util torch
 Home-page: https://github.com/dsm-72/utrc
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: utility for pytorch torch util utrc
 Classifier: Development Status :: 4 - Beta
```

### Comparing `utrc-0.0.6/README.md` & `utrc-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `utrc-0.0.6/settings.ini` & `utrc-0.0.7/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = utrc
 lib_name = utrc
-version = 0.0.6
+version = 0.0.7
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = utrc
 nbs_path = nbs
 recursive = True
```

### Comparing `utrc-0.0.6/setup.py` & `utrc-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.6/utrc/__init__.py` & `utrc-0.0.7/utrc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00__init__.ipynb.
 
 # %% auto 0
 __all__ = []
 
 # %% ../nbs/00__init__.ipynb 3
 from itertools import chain
```

### Comparing `utrc-0.0.6/utrc/_modidx.py` & `utrc-0.0.7/utrc/_modidx.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,9 +236,13 @@
                            'utrc.tens.pack': ('tens.html#pack', 'utrc/tens.py'),
                            'utrc.tens.pack_padded': ('tens.html#pack_padded', 'utrc/tens.py'),
                            'utrc.tens.pad': ('tens.html#pad', 'utrc/tens.py'),
                            'utrc.tens.sort_sequences': ('tens.html#sort_sequences', 'utrc/tens.py'),
                            'utrc.tens.torchnans': ('tens.html#torchnans', 'utrc/tens.py'),
                            'utrc.tens.unpack': ('tens.html#unpack', 'utrc/tens.py'),
                            'utrc.tens.unpadded_len': ('tens.html#unpadded_len', 'utrc/tens.py')},
-            'utrc.util': { 'utrc.util.extent': ('util.html#extent', 'utrc/util.py'),
-                           'utrc.util.integration_steps': ('util.html#integration_steps', 'utrc/util.py')}}}
+            'utrc.util': { 'utrc.util.batch_zeros': ('util.html#batch_zeros', 'utrc/util.py'),
+                           'utrc.util.extent': ('util.html#extent', 'utrc/util.py'),
+                           'utrc.util.gauss_like': ('util.html#gauss_like', 'utrc/util.py'),
+                           'utrc.util.integration_space': ('util.html#integration_space', 'utrc/util.py'),
+                           'utrc.util.integration_steps': ('util.html#integration_steps', 'utrc/util.py'),
+                           'utrc.util.zero_placeholder': ('util.html#zero_placeholder', 'utrc/util.py')}}}
```

### Comparing `utrc-0.0.6/utrc/attr.py` & `utrc-0.0.7/utrc/attr.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.6/utrc/atyp.py` & `utrc-0.0.7/utrc/atyp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/02_atyp.ipynb.
 
 # %% auto 0
 __all__ = ['T', 'O', 'P', 'Ts', 'VidsInfo', 'XYArray', 'LabelArray', 'DistanceArray', 'RotationMatrix', 'DynamicsInput',
            'DynamicsOutput', 'CellState', 'HiddenState', 'RNNState', 'GRUState', 'LSTMStates', 'RNNStateQ', 'GRUStateQ',
            'LSTMStatesQ', 'RecurrentStates', 'RecurrentStatesQ', 'HiddenStates', 'HiddenStatesQ', 'TorchDynForward',
-           'DynamicsForward', 'KineticsForward', 'LossFunction', 'DiffusionFunction', 'star']
+           'DynamicsForward', 'KineticsForward', 'LossFunction', 'RegulationSpec', 'DiffusionFunction', 'star']
 
 # %% ../nbs/02_atyp.ipynb 6
 #| export
 
 # %% ../nbs/02_atyp.ipynb 8
 from typing import (
     Self, Union, Iterable, 
@@ -20,15 +20,15 @@
 #| export
 
 
 # %% ../nbs/02_atyp.ipynb 12
 from nchr import STAR
 from quac import (
     ints, dim1, dim2, num, bbox, lit, size, tensor, path,
-    neuraldynamics
+    neuraldynamics, nnmodule
 )
 
 # %% ../nbs/02_atyp.ipynb 14
 #| export
 
 
 # %% ../nbs/02_atyp.ipynb 16
@@ -244,15 +244,18 @@
     usedec: bool = True\
 )` -> `y` or `(t, y)`
 ''';
 
 # %% ../nbs/02_atyp.ipynb 33
 LossFunction: TypeAlias = Callable[[tensor, tensor], Union[tensor,  num]]
 
-# %% ../nbs/02_atyp.ipynb 35
+# %% ../nbs/02_atyp.ipynb 34
+RegulationSpec: TypeAlias = LossFunction | list[LossFunction] | tuple[list[LossFunction], list[float]]
+
+# %% ../nbs/02_atyp.ipynb 36
 DiffusionFunction: TypeAlias = Union[
     'Diffusion', 'DiffusionMap', 'DiffusionDistance', 
     'DiffusionAffinity', 'PHATEDistance'
 ]
 
-# %% ../nbs/02_atyp.ipynb 37
+# %% ../nbs/02_atyp.ipynb 38
 #| export
```

### Comparing `utrc-0.0.6/utrc/bend.py` & `utrc-0.0.7/utrc/bend.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.6/utrc/cols.py` & `utrc-0.0.7/utrc/cols.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.6/utrc/cons.py` & `utrc-0.0.7/utrc/cons.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.6/utrc/data.py` & `utrc-0.0.7/utrc/data.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.6/utrc/diff.py` & `utrc-0.0.7/utrc/diff.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.6/utrc/dims.py` & `utrc-0.0.7/utrc/dims.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.6/utrc/init.py` & `utrc-0.0.7/utrc/init.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.6/utrc/kwds.py` & `utrc-0.0.7/utrc/kwds.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/03_kwds.ipynb.
 
 # %% auto 0
-__all__ = ['TorchDiffEQIntegrationKeywords', 'NeuralKeywords', 'AugmenterKeywords', 'SimpleKeywords', 'DynamicsForwardKeywords',
-           'DynamicsKeywords', 'NeuralOptimalTransportKeywords', 'DifferentialEquationKeywords', 'ODEKeywords',
-           'SDEFunctionKeywords', 'SDEProblemKeywords', 'SDEKeywords', 'SubVidInfo', 'VidInfo', 'DiffusionKeywords',
-           'BaseRecurrentKeywords', 'LSTMKeywords', 'RNNKeywords', 'RecurrentKeywords', 'RecurrentAutoEncoderKeywords',
-           'RecurrentEncoderKeywords', 'RecurrentDecoderKeywords']
+__all__ = ['NeuralKeywords', 'AugmenterKeywords', 'SimpleKeywords', 'DynamicsForwardKeywords', 'DynamicsKeywords',
+           'NeuralOptimalTransportKeywords', 'DifferentialEquationKeywords', 'ODEKeywords', 'SDEFunctionKeywords',
+           'SDEProblemKeywords', 'SDEKeywords', 'SubVidInfo', 'VidInfo', 'DiffusionKeywords', 'BaseRecurrentKeywords',
+           'LSTMKeywords', 'RNNKeywords', 'RecurrentKeywords', 'RecurrentAutoEncoderKeywords',
+           'RecurrentEncoderKeywords', 'RecurrentDecoderKeywords', 'TorchDiffEQIntegrationKeywords']
 
 # %% ../nbs/03_kwds.ipynb 6
 from functools import wraps
 
 # %% ../nbs/03_kwds.ipynb 8
 from typing import (
     Union, Iterable, TypedDict, 
@@ -40,40 +40,15 @@
 )
 
 _TYPE_DICT_KWDS = dict(
     __ignore_values  = _IGNORE_INIT,
     __force_defaults = False
 )
 
-# %% ../nbs/03_kwds.ipynb 18
-class TorchDiffEQIntegrationKeywords(TypeDict, **_TYPE_DICT_KWDS):
-    '''Typed dictionary for initalizing a neural network.
-    
-    Attributes
-    ----------
-    device : device | str, optional
-        The device to use for computation.
-    '''
-    rtol: float = 1e-7
-    atol: float = 1e-9
-    method: str | None = None
-    options: dict | None = None
-    event_fn: Callable | None = None
-    adjoint_rtol: float | None = None
-    adjoint_atol: float | None = None
-    adjoint_method: str | None = None
-    adjoint_options: dict | None = None
-    adjoint_params: dict | None = None
-    @overload
-    def __init__(self, device: deviceq) -> 'TorchDiffEQIntegrationKeywords': ...
-    def __init__(self, *args, **kwargs: 'TorchDiffEQIntegrationKeywords') -> 'TorchDiffEQIntegrationKeywords':
-        '''Typed dictionary for initalizing a neural network.'''
-        return super().__init__(self, *(), **kwargs)
-
-# %% ../nbs/03_kwds.ipynb 21
+# %% ../nbs/03_kwds.ipynb 19
 class NeuralKeywords(TypeDict, **_TYPE_DICT_KWDS):
     '''Typed dictionary for initalizing a neural network.
     
     Attributes
     ----------
     device : device | str, optional
         The device to use for computation.
@@ -82,15 +57,15 @@
     
     @overload
     def __init__(self, device: deviceq) -> 'NeuralKeywords': ...
     def __init__(self, *args, **kwargs: 'NeuralKeywords') -> 'NeuralKeywords':
         '''Typed dictionary for initalizing a neural network.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 24
+# %% ../nbs/03_kwds.ipynb 22
 class AugmenterKeywords(TypeDict, **_TYPE_DICT_KWDS):
     '''Typed dictionary for initalizing an Augmenter.
     
     Attributes
     ----------
     adim : int, optional
         The number of augmenting dimensions.
@@ -103,15 +78,15 @@
     
     @overload
     def __init__(self, adim: intq, afnc: Callable | None) -> 'AugmenterKeywords': ...
     def __init__(self, *args, **kwargs: 'AugmenterKeywords') -> 'AugmenterKeywords':
         '''Typed dictionary for initalizing an Augmenter.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 27
+# %% ../nbs/03_kwds.ipynb 25
 class SimpleKeywords(NeuralKeywords, **_TYPE_DICT_KWDS):
     '''Typed dictionary for initalizing a Simple Neural Network.
     
     Attributes
     ----------
     feats : list[int]
         The number of features per linear layer e.g. [10, 10]
@@ -163,15 +138,15 @@
         outkws: dict,
         device: deviceq
     ) -> 'SimpleKeywords': ...
     def __init__(self, *args, **kwargs: 'SimpleKeywords') -> 'SimpleKeywords':
         '''Typed dictionary for initalizing a Simple Neural Network.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 31
+# %% ../nbs/03_kwds.ipynb 29
 class DynamicsForwardKeywords(TypeDict, **_TYPE_DICT_KWDS):
     '''Typed dictionary for the forward call of a `torchdyn.nn.Module`.
     
     Attributes
     ----------
     x : tensor
     
@@ -217,15 +192,15 @@
         useaug: bool, 
         usedec: bool,
     ) -> 'DynamicsForwardKeywords': ...
     def __init__(self, *args, **kwargs: 'DynamicsForwardKeywords') -> 'DynamicsForwardKeywords':
         '''Typed dictionary for the forward call of a `torchdyn.nn.Module`.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 34
+# %% ../nbs/03_kwds.ipynb 32
 class DynamicsKeywords(AugmenterKeywords, NeuralKeywords, **_TYPE_DICT_KWDS):
     '''Typed dictionary for initalizing a Dynamic Neural Network.
     
     Attributes
     ----------
     diffeq : DynamicsMethod 
         The dynamics method to use e.g. DynamicsMethod.NeuralODE, DynamicsMethod.NeuralSDE
@@ -268,15 +243,15 @@
         tsteps: tensor,
         **kwargs: AugmenterKeywords | NeuralKeywords
     ): ...
     def __init__(self, *args, **kwargs: 'DynamicsForwardKeywords') -> 'DynamicsForwardKeywords':
         '''Typed dictionary for initalizing a Dynamic Neural Network.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 37
+# %% ../nbs/03_kwds.ipynb 35
 class NeuralOptimalTransportKeywords(SimpleKeywords, DynamicsKeywords, AugmenterKeywords, NeuralKeywords, **_TYPE_DICT_KWDS):
     '''Typed dictionary for initalizing an Optimal Transport Neural Network.
     
     Attributes
     ----------
     topk: int
         number of top predictions to consider
@@ -345,15 +320,15 @@
         topk: int,
         **kwargs: DynamicsKeywords | AugmenterKeywords | NeuralKeywords
     ): ...
     def __init__(self, *args, **kwargs: 'NeuralOptimalTransportKeywords') -> 'NeuralOptimalTransportKeywords':
         '''Typed dictionary for initalizing an Optimal Transport Neural Network.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 40
+# %% ../nbs/03_kwds.ipynb 38
 class DifferentialEquationKeywords(TypeDict, **_TYPE_DICT_KWDS):
     '''Typed dictionary for initalizing a Differential Equation.
     
     Attributes
     ----------
     order: Optional[int], default: 1
         order of the differential equation. Defaults to 1.
@@ -390,15 +365,15 @@
         sensitivity: str,
         return_t_eval: bool,
     ): ...
     def __init__(self, *args, **kwargs: 'DifferentialEquationKeywords') -> 'DifferentialEquationKeywords':
         '''Typed dictionary for initalizing a Differential Equation.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 44
+# %% ../nbs/03_kwds.ipynb 42
 class ODEKeywords(DifferentialEquationKeywords, **_TYPE_DICT_KWDS):
     '''Typed dictionary for initalizing an Ordinary Differential Equation.
     
     Attributes
     ----------
     vector_field: Union[Solver, str, nnmodule]
         Defaults to Solver.EulerODE.
@@ -474,15 +449,15 @@
         optimizable_params: Union[Iterable, Generator],
         **kwargs: DifferentialEquationKeywords
     ): ...
     def __init__(self, *args, **kwargs: 'ODEKeywords') -> 'ODEKeywords':
         '''Typed dictionary for initalizing an Ordinary Differential Equation.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 48
+# %% ../nbs/03_kwds.ipynb 46
 class SDEFunctionKeywords(TypeDict, **_TYPE_DICT_KWDS):
     '''Typed dictionary for initalizing a SDE function.
     
     Attributes
     ----------
     drift_func: Callable
         drift function, i.e. f (Callable): callable defining the drift
@@ -513,15 +488,15 @@
         noise_type: SDENoiseType,
         sde_type: Optional[SolverKind],
     ): ...
     def __init__(self, *args, **kwargs: 'SDEFunctionKeywords') -> 'SDEFunctionKeywords':
         '''Typed dictionary for initalizing a SDE function.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 51
+# %% ../nbs/03_kwds.ipynb 49
 class SDEProblemKeywords(TypeDict, **_TYPE_DICT_KWDS):
     '''Typed dictionary for initalizing a SDE Problem function.
     
     Attributes
     ----------
     defunc: sdefunc
         The differnetial equation function e.g. 
@@ -533,15 +508,15 @@
         self, 
         defunc: sdefunc,
     ): ...
     def __init__(self, *args, **kwargs: 'SDEProblemKeywords') -> 'SDEProblemKeywords':
         '''Typed dictionary for initalizing a SDE Problem function.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 54
+# %% ../nbs/03_kwds.ipynb 52
 class SDEKeywords(SDEFunctionKeywords, DifferentialEquationKeywords, **_TYPE_DICT_KWDS):
     '''Typed dictionary for initalizing a Stochastic Differential Equation.
     
     Attributes
     ----------
     t_span: Optional[list[int]]
         Defaults to torch.linspace(0, 1, 2).
@@ -657,15 +632,15 @@
         bm: Optional[brownianintervial],
         **kwargs: SDEFunctionKeywords | DifferentialEquationKeywords
     ): ...
     def __init__(self, *args, **kwargs: 'SDEKeywords') -> 'SDEKeywords':
         '''Typed dictionary for initalizing a Stochastic Differential Equation.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 58
+# %% ../nbs/03_kwds.ipynb 56
 class SubVidInfo(TypeDict, **_TYPE_DICT_KWDS):
     '''Subvideo Information from an AVI file'''
     pos: xypos
     '''The (row, col) position of the subvideo in the grid'''
     bbox: BBox
     '''The bounding box of the subvideo in the grid'''
     subidx: int
@@ -680,15 +655,15 @@
         subidx: int,
         subkey: str
     ): ...
     def __init__(self, *args, **kwargs: 'SubVidInfo') -> 'SubVidInfo':
         '''Typed dictionary containing Subvideo Information from an AVI file.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 61
+# %% ../nbs/03_kwds.ipynb 59
 class VidInfo(TypeDict, **_TYPE_DICT_KWDS):
     '''AVI file information'''
     vidpxs: rect
     '''The frame size (width, height) of the video e.g. (1200, 1200)'''
     subpxs: rect
     '''The standardized subvideo size (sub-width, sub-height) e.g. (400, 400)'''
     values: list[dict[str, SubVidInfo]]
@@ -704,15 +679,15 @@
         values: list[dict[str, SubVidInfo]], 
         source: path
     ): ...
     def __init__(self, *args, **kwargs: 'VidInfo') -> 'VidInfo':
         '''Typed dictionary containing AVI file information.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 65
+# %% ../nbs/03_kwds.ipynb 63
 class DiffusionKeywords(TypeDict, **_TYPE_DICT_KWDS):
     '''Typed dictionary for initalizing a Diffusion Operation Method.'''
     knn: int = 5
     tmax: int = 5
     anisotropy: int = 1
     tdiff: int = 1
     topeig: int = 100
@@ -740,15 +715,15 @@
         njobs: int,
         device: deviceq
     ): ...
     def __init__(self, *args, **kwargs: 'DiffusionKeywords') -> 'DiffusionKeywords':
         '''Typed dictionary for initalizing a Diffusion Operation Method.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 69
+# %% ../nbs/03_kwds.ipynb 67
 class BaseRecurrentKeywords(NeuralKeywords, **_TYPE_DICT_KWDS):
     '''Typed dictionary for specifying base keywords for recurrent neural network layers.
 
     Attributes
     ----------
     input_size : int
         The number of expected features in the input.
@@ -810,15 +785,15 @@
         device: deviceq,
         dtype: dtypeq
     ): ...
     def __init__(self, *args, **kwargs: 'BaseRecurrentKeywords') -> 'BaseRecurrentKeywords':
         '''Typed dictionary for specifying base keywords for recurrent neural network layers.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 73
+# %% ../nbs/03_kwds.ipynb 71
 class LSTMKeywords(BaseRecurrentKeywords, **_TYPE_DICT_KWDS):
     '''Typed dictionary for specifying keywords specific to LSTM layers, extending `BaseRecurrentKeywords`.
 
     Attributes
     ----------
     proj_size : int
         The size of the projection layer.
@@ -853,15 +828,15 @@
         proj_size: int,
         **kwargs: BaseRecurrentKeywords
     ): ...
     def __init__(self, *args, **kwargs: 'LSTMKeywords') -> 'LSTMKeywords':
         '''Typed dictionary for specifying keywords specific to LSTM layers, extending `BaseRecurrentKeywords`.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 76
+# %% ../nbs/03_kwds.ipynb 74
 class RNNKeywords(BaseRecurrentKeywords, **_TYPE_DICT_KWDS):    
     '''Typed dictionary for specifying keywords specific to RNN layers, extending `BaseRecurrentKeywords`.
 
     Attributes
     ----------
     nonlinearity : NonLinearity
         The non-linearity to use ('relu' or 'tanh').
@@ -896,15 +871,15 @@
         nonlinearity: NonLinearity,
         **kwargs: BaseRecurrentKeywords
     ): ...
     def __init__(self, *args, **kwargs: 'RNNKeywords') -> 'RNNKeywords':
         '''Typed dictionary for specifying keywords specific to RNN layers, extending `BaseRecurrentKeywords`.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 79
+# %% ../nbs/03_kwds.ipynb 77
 class RecurrentKeywords(LSTMKeywords, RNNKeywords, **_TYPE_DICT_KWDS): 
     '''Typed dictionary for specifying keywords for recurrent neural network layers, combining `LSTMKeywords` and `RNNKeywords`.
 
     Examples
     --------
     >>> recurrent_keywords = RecurrentKeywords(
     ...     input_size=64, hidden_size=128, nlays=2, proj_size=64, nonlinearity=NonLinearity.Tanh, 
@@ -945,15 +920,15 @@
     def __init__(
         self, *args, **kwargs: LSTMKeywords | RNNKeywords
     ): ...
     def __init__(self, *args, **kwargs: 'RecurrentKeywords') -> 'RecurrentKeywords':
         '''Typed dictionary for specifying keywords for recurrent neural network layers, combining `LSTMKeywords` and `RNNKeywords`.'''
         return super().__init__(self, *(), **kwargs)
 
-# %% ../nbs/03_kwds.ipynb 82
+# %% ../nbs/03_kwds.ipynb 80
 class RecurrentAutoEncoderKeywords(RecurrentKeywords, **_TYPE_DICT_KWDS):
     '''Typed dictionary for specifying keywords for recurrent autoencoder models, extending `RecurrentKeywords`.
 
     Attributes
     ----------
     output_size : int
         The size of the output layer.
@@ -1031,30 +1006,55 @@
         '''Typed dictionary for specifying keywords specific to RNN layers, extending `BaseRecurrentKeywords`.'''
         result, params = dict(), kwargs.copy()
         kind = params.pop(KIND, RecurrentLayer.LSTM)
         if RecurrentLayer(kind) != RecurrentLayer.RNN:  params.pop(NONLINEARITY, None)
         if RecurrentLayer(kind) != RecurrentLayer.LSTM: params.pop(PROJ_SIZE, None)
         return super().__init__(self, *args, **{**result, **params})
 
-# %% ../nbs/03_kwds.ipynb 85
+# %% ../nbs/03_kwds.ipynb 83
 class RecurrentEncoderKeywords(RecurrentAutoEncoderKeywords, **_TYPE_DICT_KWDS):
     def __init__(self, *args, **kwargs: 'RecurrentEncoderKeywords'):
         super().__init__(self, *args, **kwargs)
         input_size  = self.pop(INPUT_SIZE,  None)
         hidden_size = self.pop(HIDDEN_SIZE, None)
         output_size = self.pop(OUTPUT_SIZE, None)
         self.setdefault(INPUT_SIZE,  input_size or hidden_size)
         self.setdefault(HIDDEN_SIZE, output_size or hidden_size)
         
 
-# %% ../nbs/03_kwds.ipynb 88
+# %% ../nbs/03_kwds.ipynb 86
 class RecurrentDecoderKeywords(RecurrentAutoEncoderKeywords, **_TYPE_DICT_KWDS):
     def __init__(self, *args, **kwargs: 'RecurrentDecoderKeywords'):
         super().__init__(self, *args, **kwargs)
         input_size  = self.pop(INPUT_SIZE,  None)
         hidden_size = self.pop(HIDDEN_SIZE, None)
         output_size = self.pop(OUTPUT_SIZE, None)
         self.setdefault(HIDDEN_SIZE, input_size  or hidden_size)
         self.setdefault(OUTPUT_SIZE, output_size or hidden_size)
 
+# %% ../nbs/03_kwds.ipynb 89
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
 # %% ../nbs/03_kwds.ipynb 91
 #| export
```

### Comparing `utrc-0.0.6/utrc/logs.py` & `utrc-0.0.7/utrc/logs.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.6/utrc/loss.py` & `utrc-0.0.7/utrc/loss.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.6/utrc/misc.py` & `utrc-0.0.7/utrc/misc.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.6/utrc/pand.py` & `utrc-0.0.7/utrc/pand.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.6/utrc/perc.py` & `utrc-0.0.7/utrc/perc.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.6/utrc/seed.py` & `utrc-0.0.7/utrc/seed.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.6/utrc/smpl.py` & `utrc-0.0.7/utrc/smpl.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.6/utrc/strs.py` & `utrc-0.0.7/utrc/strs.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.6/utrc/tens.py` & `utrc-0.0.7/utrc/tens.py`

 * *Files identical despite different names*

### Comparing `utrc-0.0.6/utrc.egg-info/PKG-INFO` & `utrc-0.0.7/utrc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utrc
-Version: 0.0.6
+Version: 0.0.7
 Summary: util torch
 Home-page: https://github.com/dsm-72/utrc
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: utility for pytorch torch util utrc
 Classifier: Development Status :: 4 - Beta
```

### Comparing `utrc-0.0.6/utrc.egg-info/SOURCES.txt` & `utrc-0.0.7/utrc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

