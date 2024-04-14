# Comparing `tmp/etrc-0.0.8.tar.gz` & `tmp/etrc-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etrc-0.0.8.tar", last modified: Sun Feb 25 20:18:51 2024, max compression
+gzip compressed data, was "etrc-0.0.9.tar", last modified: Sun Mar 10 17:24:12 2024, max compression
```

## Comparing `etrc-0.0.8.tar` & `etrc-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-02-25 20:18:51.719580 etrc-0.0.8/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2023-12-31 15:21:18.000000 etrc-0.0.8/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2023-12-31 15:21:18.000000 etrc-0.0.8/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     3849 2024-02-25 20:18:51.719375 etrc-0.0.8/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     2602 2024-01-01 19:30:59.000000 etrc-0.0.8/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-02-25 20:18:51.717846 etrc-0.0.8/etrc/
--rw-r--r--   0 solst      (501) staff       (20)      852 2024-02-25 20:18:44.000000 etrc-0.0.8/etrc/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    11313 2024-02-25 20:18:44.000000 etrc-0.0.8/etrc/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)      652 2024-02-25 20:18:44.000000 etrc-0.0.8/etrc/atyp.py
--rw-r--r--   0 solst      (501) staff       (20)      592 2024-02-25 20:18:44.000000 etrc-0.0.8/etrc/cons.py
--rw-r--r--   0 solst      (501) staff       (20)     2562 2024-02-25 20:18:44.000000 etrc-0.0.8/etrc/emod.py
--rw-r--r--   0 solst      (501) staff       (20)    22808 2024-02-25 20:18:44.000000 etrc-0.0.8/etrc/enum.py
--rw-r--r--   0 solst      (501) staff       (20)     4734 2024-01-01 19:27:26.000000 etrc-0.0.8/etrc/kwds.py
--rw-r--r--   0 solst      (501) staff       (20)     3568 2024-02-25 20:18:44.000000 etrc-0.0.8/etrc/meta.py
--rw-r--r--   0 solst      (501) staff       (20)    18602 2024-02-25 20:18:44.000000 etrc-0.0.8/etrc/solv.py
--rw-r--r--   0 solst      (501) staff       (20)     4983 2024-02-25 20:18:44.000000 etrc-0.0.8/etrc/util.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-02-25 20:18:51.718848 etrc-0.0.8/etrc.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     3849 2024-02-25 20:18:51.000000 etrc-0.0.8/etrc.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      385 2024-02-25 20:18:51.000000 etrc-0.0.8/etrc.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-02-25 20:18:51.000000 etrc-0.0.8/etrc.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       30 2024-02-25 20:18:51.000000 etrc-0.0.8/etrc.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-12-31 18:29:47.000000 etrc-0.0.8/etrc.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)      166 2024-02-25 20:18:51.000000 etrc-0.0.8/etrc.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        5 2024-02-25 20:18:51.000000 etrc-0.0.8/etrc.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)     1112 2024-02-25 20:18:42.000000 etrc-0.0.8/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2024-02-25 20:18:51.719618 etrc-0.0.8/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2585 2023-12-31 15:21:18.000000 etrc-0.0.8/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-10 17:24:12.423260 etrc-0.0.9/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2023-12-31 15:21:18.000000 etrc-0.0.9/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2023-12-31 15:21:18.000000 etrc-0.0.9/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     3701 2024-03-10 17:24:12.423055 etrc-0.0.9/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     2602 2024-01-01 19:30:59.000000 etrc-0.0.9/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-10 17:24:12.421196 etrc-0.0.9/etrc/
+-rw-r--r--   0 solst      (501) staff       (20)      852 2024-03-10 17:24:07.000000 etrc-0.0.9/etrc/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    11954 2024-03-10 17:24:07.000000 etrc-0.0.9/etrc/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)      653 2024-03-10 17:24:07.000000 etrc-0.0.9/etrc/atyp.py
+-rw-r--r--   0 solst      (501) staff       (20)      592 2024-03-10 17:24:07.000000 etrc-0.0.9/etrc/cons.py
+-rw-r--r--   0 solst      (501) staff       (20)     2562 2024-03-10 17:24:07.000000 etrc-0.0.9/etrc/emod.py
+-rw-r--r--   0 solst      (501) staff       (20)    25694 2024-03-10 17:24:07.000000 etrc-0.0.9/etrc/enum.py
+-rw-r--r--   0 solst      (501) staff       (20)     4734 2024-01-01 19:27:26.000000 etrc-0.0.9/etrc/kwds.py
+-rw-r--r--   0 solst      (501) staff       (20)     3568 2024-03-10 17:24:07.000000 etrc-0.0.9/etrc/meta.py
+-rw-r--r--   0 solst      (501) staff       (20)    18602 2024-03-10 17:24:07.000000 etrc-0.0.9/etrc/solv.py
+-rw-r--r--   0 solst      (501) staff       (20)     4983 2024-03-10 17:24:07.000000 etrc-0.0.9/etrc/util.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-03-10 17:24:12.422545 etrc-0.0.9/etrc.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     3701 2024-03-10 17:24:12.000000 etrc-0.0.9/etrc.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      385 2024-03-10 17:24:12.000000 etrc-0.0.9/etrc.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-03-10 17:24:12.000000 etrc-0.0.9/etrc.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       30 2024-03-10 17:24:12.000000 etrc-0.0.9/etrc.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-12-31 18:29:47.000000 etrc-0.0.9/etrc.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)      122 2024-03-10 17:24:12.000000 etrc-0.0.9/etrc.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        5 2024-03-10 17:24:12.000000 etrc-0.0.9/etrc.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)     1060 2024-03-10 17:23:57.000000 etrc-0.0.9/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2024-03-10 17:24:12.423301 etrc-0.0.9/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2585 2023-12-31 15:21:18.000000 etrc-0.0.9/setup.py
```

### Comparing `etrc-0.0.8/LICENSE` & `etrc-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `etrc-0.0.8/PKG-INFO` & `etrc-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,35 @@
 Metadata-Version: 2.1
 Name: etrc
-Version: 0.0.8
-Summary: In Vitro Fertilization
+Version: 0.0.9
+Summary: PyTorch Enumerations
 Home-page: https://github.com/dsm-72/etrc
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
-Keywords: python py torch pytorch lightning pl trc enum
+Keywords: python py torch pytorch lightning pl trc enum enums enumeration
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: achn
-Requires-Dist: asto
-Requires-Dist: astr
-Requires-Dist: atup
-Requires-Dist: atyp
-Requires-Dist: calr
-Requires-Dist: chck
-Requires-Dist: dstr
-Requires-Dist: idfunc
-Requires-Dist: itry
-Requires-Dist: jstr
-Requires-Dist: matr
 Requires-Dist: nchr
 Requires-Dist: nlit
-Requires-Dist: pdec
-Requires-Dist: ptyp
-Requires-Dist: regsyn
+Requires-Dist: quac
 Requires-Dist: sigr
+Requires-Dist: dref
+Requires-Dist: chck
+Requires-Dist: astr
+Requires-Dist: dstr
 Requires-Dist: uscr
+Requires-Dist: atup
+Requires-Dist: asto
 Provides-Extra: dev
 Requires-Dist: numpy; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: torch; extra == "dev"
 Requires-Dist: pytorch_lightning; extra == "dev"
 Requires-Dist: torchvision; extra == "dev"
```

### Comparing `etrc-0.0.8/README.md` & `etrc-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `etrc-0.0.8/etrc/__init__.py` & `etrc-0.0.9/etrc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00__init__.ipynb.
 
 # %% auto 0
 __all__ = ['loadmod']
 
 # %% ../nbs/00__init__.ipynb 3
 from itertools import chain
```

### Comparing `etrc-0.0.8/etrc/_modidx.py` & `etrc-0.0.9/etrc/_modidx.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,17 @@
                            'etrc.emod.ModuleEnum.imp': ('emod.html#moduleenum.imp', 'etrc/emod.py'),
                            'etrc.emod.ModuleEnum.init': ('emod.html#moduleenum.init', 'etrc/emod.py'),
                            'etrc.emod.ModuleEnum.make': ('emod.html#moduleenum.make', 'etrc/emod.py'),
                            'etrc.emod.ModuleEnum.module': ('emod.html#moduleenum.module', 'etrc/emod.py'),
                            'etrc.emod.ModuleEnum.safe': ('emod.html#moduleenum.safe', 'etrc/emod.py')},
             'etrc.enum': { 'etrc.enum.CatOrder': ('enum.html#catorder', 'etrc/enum.py'),
                            'etrc.enum.CatOrder._missing_': ('enum.html#catorder._missing_', 'etrc/enum.py'),
+                           'etrc.enum.CatOrder.aug': ('enum.html#catorder.aug', 'etrc/enum.py'),
+                           'etrc.enum.CatOrder.cat': ('enum.html#catorder.cat', 'etrc/enum.py'),
+                           'etrc.enum.CatOrder.safe': ('enum.html#catorder.safe', 'etrc/enum.py'),
                            'etrc.enum.Channels': ('enum.html#channels', 'etrc/enum.py'),
                            'etrc.enum.Channels._missing_': ('enum.html#channels._missing_', 'etrc/enum.py'),
                            'etrc.enum.Channels.cidx': ('enum.html#channels.cidx', 'etrc/enum.py'),
                            'etrc.enum.Channels.flip': ('enum.html#channels.flip', 'etrc/enum.py'),
                            'etrc.enum.Channels.resize': ('enum.html#channels.resize', 'etrc/enum.py'),
                            'etrc.enum.Channels.safe': ('enum.html#channels.safe', 'etrc/enum.py'),
                            'etrc.enum.Channels.to': ('enum.html#channels.to', 'etrc/enum.py'),
@@ -47,15 +50,19 @@
                            'etrc.enum.SliceFormat.safe': ('enum.html#sliceformat.safe', 'etrc/enum.py'),
                            'etrc.enum.SliceFormat.safeflip': ('enum.html#sliceformat.safeflip', 'etrc/enum.py'),
                            'etrc.enum.SliceFormat.to': ('enum.html#sliceformat.to', 'etrc/enum.py'),
                            'etrc.enum.Solver': ('enum.html#solver', 'etrc/enum.py'),
                            'etrc.enum.Solver._missing_': ('enum.html#solver._missing_', 'etrc/enum.py'),
                            'etrc.enum.Stage': ('enum.html#stage', 'etrc/enum.py'),
                            'etrc.enum.Stage._missing_': ('enum.html#stage._missing_', 'etrc/enum.py'),
-                           'etrc.enum.Stage.safe': ('enum.html#stage.safe', 'etrc/enum.py')},
+                           'etrc.enum.Stage.safe': ('enum.html#stage.safe', 'etrc/enum.py'),
+                           'etrc.enum.adjsize': ('enum.html#adjsize', 'etrc/enum.py'),
+                           'etrc.enum.augzeros': ('enum.html#augzeros', 'etrc/enum.py'),
+                           'etrc.enum.iasdim': ('enum.html#iasdim', 'etrc/enum.py'),
+                           'etrc.enum.iindims': ('enum.html#iindims', 'etrc/enum.py')},
             'etrc.kwds': { 'etrc.kwds.diffusion_kwds': ('kwds.html#diffusion_kwds', 'etrc/kwds.py'),
                            'etrc.kwds.recurrent_decoder_kwds': ('kwds.html#recurrent_decoder_kwds', 'etrc/kwds.py'),
                            'etrc.kwds.recurrent_encoder_kwds': ('kwds.html#recurrent_encoder_kwds', 'etrc/kwds.py'),
                            'etrc.kwds.recurrent_kwds': ('kwds.html#recurrent_kwds', 'etrc/kwds.py')},
             'etrc.meta': { 'etrc.meta.ModuleEnumMeta': ('meta.html#moduleenummeta', 'etrc/meta.py'),
                            'etrc.meta.ModuleEnumMeta.__contains__': ('meta.html#moduleenummeta.__contains__', 'etrc/meta.py'),
                            'etrc.meta.ModuleEnumMeta.__copydict__': ('meta.html#moduleenummeta.__copydict__', 'etrc/meta.py'),
```

### Comparing `etrc-0.0.8/etrc/atyp.py` & `etrc-0.0.9/etrc/atyp.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,11 +23,12 @@
 
 
 # %% ../nbs/01_atyp.ipynb 16
 T = TypeVar('T')
 P = ParamSpec('P')
 
 Mixin: TypeAlias = Tuple[Type, Callable[P, Any]]
+
 MetaClass: TypeAlias = Type[Union[T, EnumMeta, ABCMeta]]
 
 # %% ../nbs/01_atyp.ipynb 18
 #| export
```

### Comparing `etrc-0.0.8/etrc/cons.py` & `etrc-0.0.9/etrc/cons.py`

 * *Files identical despite different names*

### Comparing `etrc-0.0.8/etrc/emod.py` & `etrc-0.0.9/etrc/emod.py`

 * *Files identical despite different names*

### Comparing `etrc-0.0.8/etrc/enum.py` & `etrc-0.0.9/etrc/enum.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/10_enum.ipynb.
 
 # %% auto 0
 __all__ = ['DimChars', 'DimType', 'DimName', 'dimchars', 'size2str', 'SDENoiseType', 'SDETypes', 'DynamicsMethod', 'ODETypes',
-           'CatOrder', 'Solver', 'Stage', 'Channels', 'NonLinearity', 'InitMethod', 'RecurrentLayer', 'SliceFormat',
-           'Geodesic', 'Framework']
+           'iindims', 'iasdim', 'adjsize', 'augzeros', 'CatOrder', 'Solver', 'Stage', 'Channels', 'NonLinearity',
+           'InitMethod', 'RecurrentLayer', 'SliceFormat', 'Geodesic', 'Framework']
 
 # %% ../nbs/10_enum.ipynb 6
 from enum import Enum, IntEnum, StrEnum, auto
+from functools import partial
 
 # %% ../nbs/10_enum.ipynb 8
-from types import  ModuleType
-from typing import (Type, Callable)
+from types import  ModuleType, FunctionType
+from typing import (Type, Self, Callable, Optional)
 
 # %% ../nbs/10_enum.ipynb 10
 try: import numpy as np
 except ImportError: ...
 
 try: import torchvision.transforms.functional as F
 except ImportError: ...
 
-# %% ../nbs/10_enum.ipynb 12
-from atyp import Tensor, ImgSizeQ, Slcs, DeviceQ
-from chck import isnone, notnone, isslice
+try: import torch
+except ImportError: ...
 
+# %% ../nbs/10_enum.ipynb 12
 from nchr import U1
-from nlit import NUMPY, DEVICE
+from nlit import NUMPY, DEVICE, SHAPE
 
-from asto import asdev, asten, asarr
-from itry import imod
+from quac import tensor, imagesizeq, slicespecs, deviceq
+from quac.eggs import tv_functional, pt
 
+from chck import isnone, notnone, isslice
+
+from asto import asdev, asten, asarr
 from dstr import (
     DimChars as _DimChars, DimType as _DimType, DimName as _DimName, 
     dimchars as _dimchars, size2str as _size2str
 )
 
 # %% ../nbs/10_enum.ipynb 14
 from .cons import _SUFFIX
@@ -173,14 +177,50 @@
     RungeKutta4 = RungeKutta4
     Tsitouras45 = Tsitouras45
     @classmethod
     def _missing_(cls, val: str):  
         return missing(cls, val, cls.Euler)
 
 # %% ../nbs/10_enum.ipynb 26
+def iindims(i: int, dims: tuple) -> int:
+    '''Ensure that the index `i` is within the bounds of the `dims`.'''
+    return abs(i) < len(dims)
+
+def iasdim(i: int, dims: tuple) -> int:
+    '''Ensure that the index `i` is within the bounds of the `dims` or return -1.'''
+    return i if iindims(i, dims) else -1
+
+# %% ../nbs/10_enum.ipynb 27
+def adjsize(x: tensor, idx: int = 1, dim: int = 1, add: bool = False) -> tuple:
+    '''Return the size of the tensor `x` if adjusted at index `idx` to `dim`.'''
+    dims = list(getattr(x, SHAPE, ()))
+    idx = iasdim(idx, dims)
+    dims =  dims + [None]
+    
+    if add: 
+        # NOTE: dim will never overwrite a dimension if add is True
+        dims = dims[:idx] + [dim,] + dims[idx:]
+        
+    else: 
+        # NOTE: dim might overwrite a dimension if add is False
+        dims[idx] = dim
+    
+    if dims[-1] is None: 
+        dims.pop()
+        
+    return tuple(dims)
+
+# %% ../nbs/10_enum.ipynb 28
+def augzeros(x: tensor, idx: int = 1, dim: int = 1, add: bool = False) -> tensor:
+    try: import torch
+    except: ...
+    dims = adjsize(x, idx, dim, add)
+    return torch.zeros(dims)
+
+# %% ../nbs/10_enum.ipynb 29
 class CatOrder(IntEnum):
     '''Integer enumeration to specify concatenation order.
 
     Attributes
     ----------
     first : 1
         Indicates first order.
@@ -205,16 +245,56 @@
     last  = -1
     
     @classmethod
     def _missing_(cls, n: int) -> 'CatOrder':
         if str(n) in {'first', '1'}: n = 1
         if str(n) in {'last', '-1'}: n = -1
         return cls.first if isinstance(n, int) and n > 0 else cls.last
+    
+    @classmethod
+    def safe(cls, stage: 'CatOrder') -> 'CatOrder':
+        '''Take a key and return the corresponding enum member if it exists, 
+        otherwise return the default member'''
+        try: return cls(stage)
+        except ValueError: return cls.last
+    
+    @classmethod
+    def cat(
+        cls: Type[Self], 
+        x: tensor, 
+        y: tensor, 
+        idx: int = 1,
+        order: Type[Self] = 'last', 
+    ) -> tensor | NotImplementedError:
+        '''Concatenate two tensors along a specified dimension.'''
+        # trc: ModuleType = imod('torch')
+        trc: ModuleType = pt.duck
+        ord = cls.safe(order)
+        match CatOrder(ord):
+            case CatOrder.first: return trc.cat([y.to(x), x], idx)
+            case CatOrder.last:  return trc.cat([x, y.to(x)], idx)
+            case _: raise NotImplementedError(f'CatOrder {order} not implemented.')
+    
+    @classmethod
+    def aug(
+        cls: Type[Self], 
+        x: tensor, 
+        fnc: Optional[Callable[[tensor], tensor]] = None, 
+        dim: int = 1,
+        idx: int = 1,
+        order: Type[Self] = 'last', 
+    ) -> tensor | NotImplementedError:
+        '''Augment a tensor at index `idx` by `dim` dimensions
+        with a augment function `fnc` with the concatenated in `order`.'''
+        ord = cls.safe(order)
+        idx = iasdim(idx)
+        fnc = fnc or partial(augzeros, idx=idx, dim=dim)
+        return cls.cat(x, fnc(x), idx, ord)
 
-# %% ../nbs/10_enum.ipynb 29
+# %% ../nbs/10_enum.ipynb 32
 class Solver(Enum):
     '''Enumeration for solver types, including both ODE and SDE solvers.
 
     Methods
     -------
     _missing_(val: str)
         Returns a default solver for missing entries.
@@ -243,15 +323,15 @@
     Tsitouras45 = Tsitouras45
     ImplicitEuler = ImplicitEuler
     AsynchronousLeapfrog = AsynchronousLeapfrog
     @classmethod
     def _missing_(cls, val: str):  
         return missing(cls, val, cls.EulerODE)
 
-# %% ../nbs/10_enum.ipynb 32
+# %% ../nbs/10_enum.ipynb 35
 class Stage(StrEnum):
     '''Enumeration for specifying the stage in a processing or evaluation pipeline.
 
     Attributes
     ----------
     fit : auto
         Indicates the fitting or training stage.
@@ -292,15 +372,15 @@
     @classmethod
     def safe(cls, stage: 'Stage') -> 'Stage':
         '''Take a key and return the corresponding enum member if it exists, 
         otherwise return the default member'''
         try: return cls(stage)
         except ValueError: return cls.predict
 
-# %% ../nbs/10_enum.ipynb 35
+# %% ../nbs/10_enum.ipynb 38
 class Channels(StrEnum):
     '''
     Enumeration for different channel configurations in tensors, particularly for image data.
 
     Methods
     -------
     flip(t: Tensor) -> Tensor
@@ -315,20 +395,20 @@
     resize(t: Tensor, resize: ImgSizeQ, output_channels: 'Channels') -> Tensor
         Resizes the tensor and optionally changes its channel configuration.
     '''
     THWC = auto() # 0, 1, 2, 3
     TCHW = auto() # 0, 3, 1, 2
     
     @classmethod
-    def flip(cls, t: Tensor) -> Tensor:
+    def flip(cls, t: tensor) -> tensor:
         '''Flips the tensor between THWC and TCHW channel configurations.'''
         return t.transpose(1, 3)
     
     @classmethod
-    def cidx(cls, t: Tensor) -> int:
+    def cidx(cls, t: tensor) -> int:
         '''Returns the index of the channel dimension'''
         idx = -1
         for i in range(len(t.shape)):
             if t.shape[i] != 3: continue
             idx = i
         
         idx = idx if idx >= 0 else np.argmin(t.shape)
@@ -355,15 +435,15 @@
         Channels
             The validated channel configuration, defaults to THWC if input is invalid.
         '''
         try: return cls(c)
         except ValueError: return cls.THWC
         
     @classmethod
-    def to(cls, t: Tensor, c: 'Channels' = 'THWC', cidx: int = None) -> Tensor:
+    def to(cls, t: tensor, c: 'Channels' = 'THWC', cidx: int = None) -> tensor:
         '''
         Converts a tensor to the specified channel configuration.
 
         Parameters
         ----------
         t : Tensor
             The input tensor to convert.
@@ -382,15 +462,15 @@
         if c == cls.THWC and cidx == 1: return cls.flip(t)
         if c == cls.THWC and cidx == 3: return t
         if c == cls.TCHW and cidx == 1: return t
         if c == cls.TCHW and cidx == 3: return cls.flip(t)
         return t
     
     @classmethod
-    def resize(cls, t: Tensor, resize: ImgSizeQ = None, output_channels: 'Channels' = 'THWC') -> Tensor:
+    def resize(cls, t: tensor, resize: imagesizeq = None, output_channels: 'Channels' = 'THWC') -> tensor:
         '''
         Resizes a tensor and changes its channel configuration if needed.
 
         Parameters
         ----------
         t : Tensor
             The input tensor to resize.
@@ -401,21 +481,22 @@
 
         Returns
         -------
         Tensor
             The resized tensor, potentially with a different channel configuration.
         '''
         if isnone(resize): return t 
-        F: ModuleType = imod('torchvision.transforms.functional')
+        # F: ModuleType = imod('torchvision.transforms.functional')
+        F: ModuleType = tv_functional.duck
         t = Channels.to(t, Channels.TCHW)
         t = F.resize(t, resize)
         t = Channels.to(t, output_channels)
         return t
 
-# %% ../nbs/10_enum.ipynb 37
+# %% ../nbs/10_enum.ipynb 40
 class NonLinearity(str, ModuleEnum, module = 'torch.nn', default='Tanh'):
     '''
     Enumeration of non-linear activation functions and other related layers in PyTorch.
 
     Methods
     -------
     get(*args, **kwargs) -> Layer
@@ -449,15 +530,15 @@
     Softmax = auto()
     Softmax2d = auto()
     LogSoftmax = auto()
     AdaptiveLogSoftmaxWithLoss = auto()
     
     Identity = auto()
 
-# %% ../nbs/10_enum.ipynb 39
+# %% ../nbs/10_enum.ipynb 42
 class InitMethod(str, ModuleEnum, module = 'torch.nn.init', default = 'xavier_normal'):
     '''
     Enumeration for different initialization methods for neural network layers in PyTorch.
 
     Methods
     -------
     get(*args, **kwargs) -> Layer
@@ -480,36 +561,36 @@
         '''Import the class or function corresponding to the enum member, 
         or the default member of the enum class'''
         mth = cls.safe(key)
         mod = cls.module()
         suffix = kwargs.pop(_SUFFIX, U1)
         return getattr(mod, f'{mth}{suffix}')
 
-# %% ../nbs/10_enum.ipynb 41
+# %% ../nbs/10_enum.ipynb 44
 class RecurrentLayer(str, ModuleEnum, module = 'torch.nn', default='LSTM'):
     '''
     Enumeration for different types of recurrent layers in PyTorch.
 
     Methods
     -------
     get(*args, **kwargs) -> Layer
         Retrieves the corresponding recurrent layer from PyTorch.
     '''
     GRU = auto()
     RNN = auto()
     LSTM = auto()
 
-# %% ../nbs/10_enum.ipynb 43
+# %% ../nbs/10_enum.ipynb 46
 DimChars = _DimChars
 DimType  = _DimType
 DimName  = _DimName
 dimchars = _dimchars
 size2str = _size2str
 
-# %% ../nbs/10_enum.ipynb 45
+# %% ../nbs/10_enum.ipynb 48
 class SliceFormat(StrEnum):
     '''
     Enumeration for representing different formats of slices used in tensor operations.
 
     This class provides methods to handle two common slice formats:
     - 'coord': where slices are represented as coordinates (e.g., (x0, y0, z0, ...), (x1, y1, z1, ...))
     - 'slice': where slices are represented as Python slice objects (e.g., (x0, x1), (y0, y1), (z0, z1), ...)
@@ -552,15 +633,15 @@
 
     coord = auto()
     '''(x0, y0, z0, ...), (x1, y1, z1, ...), (x2, y2, z2, ...), ...'''
     slice = auto()
     '''(x0, x1, ), (y0, y1, ), (z0, z1, ), ...'''
     
     @classmethod
-    def flip(cls, *slcs: Slcs) -> Slcs:
+    def flip(cls, *slcs: slicespecs) -> slicespecs:
         '''
         Flips the format of the given slices between 'coord' and 'slice'.
 
         Parameters
         ----------
         slcs : Slcs
             The slices to flip. Can be in 'coord' or 'slice' format.
@@ -597,15 +678,15 @@
         >>> SliceFormat.safe('unknown_format')
         SliceFormat.slice
         '''
         try: return cls(c)
         except ValueError: return cls.slice
 
     @classmethod
-    def guess(cls, *slcs: Slcs) -> Slcs:
+    def guess(cls, *slcs: slicespecs) -> slicespecs:
         '''
         Guesses the slice format based on the given slices.
 
         Parameters
         ----------
         slcs : Slcs
             The slices to evaluate.
@@ -620,15 +701,15 @@
         >>> SliceFormat.guess((0, 10), (0, 10))
         SliceFormat.slice
         '''
         if any(isslice(slc) for slc in slcs): return cls.slice
         if any([len(slc) > 3 for slc in slcs]): return cls.coord
         return cls.slice
 
-    def safeflip(self, *slcs: Slcs, fmt: 'SliceFormat') -> Slcs:
+    def safeflip(self, *slcs: slicespecs, fmt: 'SliceFormat') -> slicespecs:
         '''
         Safely flips the slice format to the specified format.
 
         Parameters
         ----------
         slcs : Slcs
             The slices to flip.
@@ -646,15 +727,15 @@
         (0, 0), (10, 10)
         '''
         fmt = self.safe(fmt)
         if self == fmt: return slcs
         else: return self.flip(*slcs)
 
     @classmethod
-    def to(cls, *slcs: Slcs, fmt: 'SliceFormat', cur: 'SliceFormat' = None) -> Slcs:
+    def to(cls, *slcs: slicespecs, fmt: 'SliceFormat', cur: 'SliceFormat' = None) -> slicespecs:
         '''
         Converts the given slices to the specified format.
 
         Parameters
         ----------
         slcs : Slcs
             The slices to convert.
@@ -674,15 +755,15 @@
         (0, 0), (10, 10)
         '''
         fmt = cls.safe(fmt)
         if isnone(cur): cur = cls.guess(*slcs)
         if cur == fmt: return slcs
         return cls.flip(*slcs)
 
-# %% ../nbs/10_enum.ipynb 49
+# %% ../nbs/10_enum.ipynb 52
 class Geodesic(str, ModuleEnum, module = 'ptrc.diff', default='diffusion'):
     '''Enumeration for specifying geodesic computation methods in differential geometry contexts.
 
     Attributes
     ----------
     diffusion : auto
         Uses diffusion process for geodesic computation.
@@ -726,15 +807,15 @@
             case cls.distance:  fnc = getattr(mod, 'DiffusionDistance', None)
             case cls.diff_map:  fnc = getattr(mod, 'DiffusionMap', None)
             case cls.affinity:  fnc = getattr(mod, 'DiffusionAffinity', None)
             case cls.phate:     fnc = getattr(mod, 'PHATEDistance', None)
             case _: fnc = getattr(mod, 'PHATEDistance', None)
         return fnc
 
-# %% ../nbs/10_enum.ipynb 51
+# %% ../nbs/10_enum.ipynb 54
 class Framework(StrEnum):
     '''Enumeration for specifying the tensor operation framework.
 
     Attributes
     ----------
     numpy : auto
         Indicates the use of NumPy for tensor operations.
@@ -769,15 +850,15 @@
     
     @classmethod
     def safe(cls, framework: 'Framework') -> 'Framework':
         try: return cls(framework)
         except ValueError: return cls.numpy
     
     @classmethod
-    def swap(cls, X, framework: 'Framework' = NUMPY, device: DeviceQ = None):
+    def swap(cls, X, framework: 'Framework' = NUMPY, device: deviceq = None):
         framework = cls.safe(framework)
         device = asdev(getattr(X, DEVICE, device))
         match framework:
             case cls.numpy:
                 return asarr(X)
             
             case cls.torch:
@@ -785,9 +866,9 @@
                 if notnone(device): 
                     X = X.to(device)
                 return X
             
             case _: ...
         return X
 
-# %% ../nbs/10_enum.ipynb 53
+# %% ../nbs/10_enum.ipynb 56
 #| export
```

### Comparing `etrc-0.0.8/etrc/kwds.py` & `etrc-0.0.9/etrc/kwds.py`

 * *Files identical despite different names*

### Comparing `etrc-0.0.8/etrc/meta.py` & `etrc-0.0.9/etrc/meta.py`

 * *Files identical despite different names*

### Comparing `etrc-0.0.8/etrc/solv.py` & `etrc-0.0.9/etrc/solv.py`

 * *Files identical despite different names*

### Comparing `etrc-0.0.8/etrc/util.py` & `etrc-0.0.9/etrc/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 from typing import (Type)
 
 # %% ../nbs/02_util.ipynb 10
 #| export
 
 
 # %% ../nbs/02_util.ipynb 12
-from atyp import Layer, BoolQ
 from nchr import NIL
 from nlit import NAME, VALUE, _DEFAULT_
+from quac import layer, boolq
 from chck import isnone, notnone
 
 # %% ../nbs/02_util.ipynb 14
 from .cons import TORCH_NN
 from .atyp import T
 
 # %% ../nbs/02_util.ipynb 16
@@ -120,17 +120,17 @@
         try: return enm(default)
         except: return default
     return default
 
 # %% ../nbs/02_util.ipynb 18
 def get_torch_module(
     obj, *args, __module: ModuleType = TORCH_NN, 
-    __enumkey: BoolQ = None, __enumval: BoolQ = None, __suffix: str = NIL,
+    __enumkey: boolq = None, __enumval: boolq = None, __suffix: str = NIL,
     **kwargs
-) -> Layer:
+) -> layer:
     '''
     Fetch a torch module based on an enumeration value or its name.
 
     Parameters
     ----------
     obj : Enum
         An enumeration instance or class.
```

### Comparing `etrc-0.0.8/etrc.egg-info/PKG-INFO` & `etrc-0.0.9/etrc.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,35 @@
 Metadata-Version: 2.1
 Name: etrc
-Version: 0.0.8
-Summary: In Vitro Fertilization
+Version: 0.0.9
+Summary: PyTorch Enumerations
 Home-page: https://github.com/dsm-72/etrc
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
-Keywords: python py torch pytorch lightning pl trc enum
+Keywords: python py torch pytorch lightning pl trc enum enums enumeration
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: achn
-Requires-Dist: asto
-Requires-Dist: astr
-Requires-Dist: atup
-Requires-Dist: atyp
-Requires-Dist: calr
-Requires-Dist: chck
-Requires-Dist: dstr
-Requires-Dist: idfunc
-Requires-Dist: itry
-Requires-Dist: jstr
-Requires-Dist: matr
 Requires-Dist: nchr
 Requires-Dist: nlit
-Requires-Dist: pdec
-Requires-Dist: ptyp
-Requires-Dist: regsyn
+Requires-Dist: quac
 Requires-Dist: sigr
+Requires-Dist: dref
+Requires-Dist: chck
+Requires-Dist: astr
+Requires-Dist: dstr
 Requires-Dist: uscr
+Requires-Dist: atup
+Requires-Dist: asto
 Provides-Extra: dev
 Requires-Dist: numpy; extra == "dev"
 Requires-Dist: pandas; extra == "dev"
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: torch; extra == "dev"
 Requires-Dist: pytorch_lightning; extra == "dev"
 Requires-Dist: torchvision; extra == "dev"
```

### Comparing `etrc-0.0.8/settings.ini` & `etrc-0.0.9/settings.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = etrc
 lib_name = etrc
-version = 0.0.8
+version = 0.0.9
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = etrc
 nbs_path = nbs
 recursive = True
@@ -17,23 +17,23 @@
 doc_baseurl = /etrc
 git_url = https://github.com/dsm-72/etrc
 title = etrc
 audience = Developers
 author = dsm-72
 author_email = sumner.magruder@yale.edu
 copyright = 2023 onwards, dsm-72
-description = In Vitro Fertilization
-keywords = python py torch pytorch lightning pl trc enum
+description = PyTorch Enumerations
+keywords = python py torch pytorch lightning pl trc enum enums enumeration 
 language = English
 status = 3
 user = dsm-72
 conda_user = dsm-72
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
-; requirements = nchr nlit astr uscr pdec itry matr ptyp typs ptyp atyp nchr nlit chck asto itry regsyn idfunc calr achn atup jstr dstr sigr
-requirements = achn asto astr atup atyp calr chck dstr idfunc itry jstr matr nchr nlit pdec ptyp regsyn sigr uscr
+; requirements = achn asto astr atup atyp calr chck dstr idfunc itry jstr matr nchr nlit pdec ptyp regsyn sigr uscr
+requirements = nchr nlit quac sigr dref chck astr dstr uscr atup asto
 dev_requirements = numpy pandas matplotlib torch pytorch_lightning torchvision
```

### Comparing `etrc-0.0.8/setup.py` & `etrc-0.0.9/setup.py`

 * *Files identical despite different names*

