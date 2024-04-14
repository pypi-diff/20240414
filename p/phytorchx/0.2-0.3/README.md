# Comparing `tmp/phytorchx-0.2.tar.gz` & `tmp/phytorchx-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phytorchx-0.2.tar", last modified: Wed Aug 16 15:57:48 2023, max compression
+gzip compressed data, was "phytorchx-0.3.tar", last modified: Sun Apr 14 12:03:22 2024, max compression
```

## Comparing `phytorchx-0.2.tar` & `phytorchx-0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 15:57:48.779570 phytorchx-0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 15:57:48.775570 phytorchx-0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 15:57:48.775570 phytorchx-0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-16 15:57:38.000000 phytorchx-0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-16 15:57:38.000000 phytorchx-0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-16 15:57:38.000000 phytorchx-0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-16 15:57:48.779570 phytorchx-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-16 15:57:38.000000 phytorchx-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 15:57:48.779570 phytorchx-0.2/phytorchx/
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-08-16 15:57:38.000000 phytorchx-0.2/phytorchx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-16 15:57:48.000000 phytorchx-0.2/phytorchx/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-16 15:57:38.000000 phytorchx-0.2/phytorchx/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-08-16 15:57:38.000000 phytorchx-0.2/phytorchx/broadcast.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-16 15:57:48.779570 phytorchx-0.2/phytorchx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-08-16 15:57:48.000000 phytorchx-0.2/phytorchx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-08-16 15:57:48.000000 phytorchx-0.2/phytorchx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-16 15:57:48.000000 phytorchx-0.2/phytorchx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-16 15:57:48.000000 phytorchx-0.2/phytorchx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-16 15:57:48.000000 phytorchx-0.2/phytorchx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-16 15:57:38.000000 phytorchx-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-16 15:57:48.779570 phytorchx-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:03:22.530104 phytorchx-0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:03:22.526104 phytorchx-0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:03:22.526104 phytorchx-0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-14 12:03:18.000000 phytorchx-0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-14 12:03:18.000000 phytorchx-0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-14 12:03:18.000000 phytorchx-0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-14 12:03:22.530104 phytorchx-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-14 12:03:18.000000 phytorchx-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:03:22.526104 phytorchx-0.3/phytorchx/
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-04-14 12:03:18.000000 phytorchx-0.3/phytorchx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-14 12:03:22.000000 phytorchx-0.3/phytorchx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-14 12:03:18.000000 phytorchx-0.3/phytorchx/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-14 12:03:18.000000 phytorchx-0.3/phytorchx/broadcast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:03:22.530104 phytorchx-0.3/phytorchx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-14 12:03:22.000000 phytorchx-0.3/phytorchx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-14 12:03:22.000000 phytorchx-0.3/phytorchx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 12:03:22.000000 phytorchx-0.3/phytorchx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-14 12:03:22.000000 phytorchx-0.3/phytorchx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 12:03:22.000000 phytorchx-0.3/phytorchx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-14 12:03:18.000000 phytorchx-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 12:03:22.530104 phytorchx-0.3/setup.cfg
```

### Comparing `phytorchx-0.2/.github/workflows/python-publish.yml` & `phytorchx-0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `phytorchx-0.2/LICENSE.txt` & `phytorchx-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `phytorchx-0.2/PKG-INFO` & `phytorchx-0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: phytorchx
-Version: 0.2
+Version: 0.3
 Summary: Small utiilities package for PyTorch
 Author-email: Kosio Karchev <kosiokarchev@gmail.com>
 License: MIT
 Project-URL: GitHub, https://github.com/kosiokarchev/phytorchx
 Project-URL: Read the Docs, https://phytorchx.readthedocs.org/
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: more-itertools
+Requires-Dist: optree
+Requires-Dist: torch
 
 # φtorch-x
 #### *small utilities package for PyTorch*
```

### Comparing `phytorchx-0.2/phytorchx/__init__.py` & `phytorchx-0.3/phytorchx/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from functools import wraps
 from itertools import starmap
 from operator import mul
-from typing import Iterable
+from typing import Iterable, Optional, Union, TypeVar
 
 import torch
 from more_itertools import last
 from optree import tree_map_
 from torch import Tensor, Size, tensor
 
 from ._version import __version__, version, __version_tuple__, version_tuple
@@ -14,15 +14,26 @@
 
 def get_default_device():
     """Try really hard to return the "default" |PyTorch| device.
 
     This is defined as the device on which a tensor would be allocated by default
     **at the point this function is called**.
     """
-    return torch._C._get_default_device()
+    return (
+        _.device
+        if (_ := getattr(torch, '_GLOBAL_DEVICE_CONTEXT', None)) is not None
+        else torch._C._get_default_device()
+    )
+
+
+_Size = Union[Size, Iterable[int], int]
+
+
+def sizeify(arg: Optional[_Size]) -> Size:
+    return None if arg is None else Size(arg) if isinstance(arg, Iterable) else Size((arg,))
 
 
 @wraps(torch.load, ('__annotations__',), ())
 def load(*args, **kwargs):
     """`torch.load` onto the default device and with the default `~torch.dtype`.
 
     Parameters
@@ -37,15 +48,15 @@
     )
 
 
 def _mid_one_unnormed(a: Tensor, dim: int) -> Tensor:
     return torch.narrow(a, dim, 0, a.shape[dim]-1) + torch.narrow(a, dim, 1, a.shape[dim]-1)
 
 
-def mid_one(a: Tensor, axis: int) -> Tensor:
+def mid_one(a: Tensor, axis: int = -1) -> Tensor:
     r"""Create a new tensor which, along the :arg:`dim`-th dimension, contains the
     average of adjacent elements of the input:
 
     .. math::
        \mathrm{out}[..., i, ...] = (\mathrm{a}[..., i, ...] + \mathrm{a}[..., i+1, ...]) / 2.
 
     Parameters
@@ -59,24 +70,29 @@
     -------
     :
         ``(*a.shape[:axis], a.shape[axis]-1, *a.shape[axis+1:])``
     """
     return _mid_one_unnormed(a, axis) / 2
 
 
-def mid_many(a: Tensor, axes: Iterable[int]) -> Tensor:
+def mid_many(a: Tensor, axes: Iterable[int] = None) -> Tensor:
     r"""Perform `mid_one` along  many (not necessarily dajacent) :arg:`axes` at the same time."""
+    if axes is None:
+        axes = range(a.ndim)
     axes = [ax % a.ndim for ax in axes]
     return last(
         _a for _a in [a] for ax in axes
         for _a in [_mid_one_unnormed(_a, ax)]
     ) / 2**len(axes) if axes else a
 
 
-def ravel_multi_index(indices: Iterable[Tensor], shape: Size) -> Tensor:
+_T = TypeVar('_T', bound=Tensor)
+
+
+def ravel_multi_index(indices: Iterable[_T], shape: Size) -> _T:
     """Transform a multi-dimensional index into a one-dimensional index into the ravelled tensor.
 
     Parameters
     ----------
     indices
         iterable of indices, which will be broadcast against each other.
     shape
```

### Comparing `phytorchx-0.2/phytorchx/broadcast.py` & `phytorchx-0.3/phytorchx/broadcast.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from __future__ import annotations
 
+import torch
 from itertools import chain
-from typing import Iterable
+from typing import Iterable, Union
 
 from more_itertools import split_into, lstrip
 from torch import broadcast_shapes, Size, Tensor, cat, gather, LongTensor
 
 __all__ = (
-    'broadcast_except', 'broadcast_left', 'broadcast_gather', 'broadcast_cat',
+    'broadcast_except', 'broadcast_left',
+    'broadcast_gather', 'broadcast_multigather',
+    'broadcast_cat', 'broadcast_stack',
     'insert_dims', 'pad_dims', 'align_dims',
     'aligned_expand', 'fancy_align'
 )
 
+from . import ravel_multi_index
+
 
 def broadcast_except(*tensors: Tensor, dim=-1) -> list[Tensor]:
     r"""Broadcast the given tensors along all dimensions except :arg:`dim`, which is retained as-is on every input.
 
     For example, ``(1, 3, 2), (4, 5, 1), dim=1 -> (4, 3, 2), (4, 5, 2)``.
 
     Notes
@@ -33,15 +38,15 @@
 
     For example, ``(1, 2, 3, 4), (5, 1, 6), ndim=2 -> (5, 2, 3, 4), (5, 2, 6)``.
     """
     shape = broadcast_shapes(*(t.shape[:ndim] for t in tensors))
     return (t.expand(*shape, *t.shape[ndim:]) for t in tensors)
 
 
-def broadcast_gather(input: Tensor, dim, index: LongTensor, index_ndim: int = 1, *, sparse_grad=False) -> Tensor:
+def broadcast_gather(input: Tensor, dim, index: Union[LongTensor, Tensor], index_ndim: int = 1, *, sparse_grad=False) -> Tensor:
     r"""Like `torch.gather` but more batched.
 
     .. code-block:: text
 
         input.shape: (batch_shape..., N, event_shape...)
         index.shape: (batch_shape..., index_shape...)
         out.shape:   (batch_shape..., index_shape..., event_shape...)
@@ -53,30 +58,49 @@
     index
         its *rightmost* :arg:`index_ndim` dimensions are considered the desired "extracted shape" and expanded in the
         place of the index dimension of :arg:`input` (:arg:`dim`).
 
     Returns
     -------
     """
-    index_shape = index.shape[-index_ndim:]
-    index = index.flatten(-index_ndim)
+    _index_dim = index.ndim-index_ndim
+    index_shape = index.shape[_index_dim:]
+    index = index.unsqueeze(-1).flatten(_index_dim)
     batch_shape = broadcast_shapes(input.shape[:dim], index.shape[:-1])
     input = input.expand(*batch_shape, *input.shape[dim:])
     index = index.expand(*batch_shape, index.shape[-1])
     return gather(input, dim, index.reshape(
-        *index.shape, *(input.ndim - index.ndim)*(1,)).expand(
+        *index.shape, *(input.ndim - index.ndim)*(1,)
+    ).expand(
         *index.shape, *input.shape[index.ndim:]
-    ) if input.ndim > index.ndim else index, sparse_grad=sparse_grad).reshape(*index.shape[:-1], *index_shape, *input.shape[dim % input.ndim + 1:])
+    ) if input.ndim > index.ndim else index, sparse_grad=sparse_grad).reshape((
+        *index.shape[:-1], *index_shape, *input.shape[dim % input.ndim + 1:]))
+
+
+def broadcast_multigather(input: Tensor, *indices: LongTensor, index_ndim=0, event_ndim=0):
+    event_pos = input.ndim - event_ndim
+    idx_start = event_pos-len(indices)
+    return broadcast_gather(
+        input.flatten(idx_start, event_pos-1),
+        idx_start-input.ndim,
+        ravel_multi_index(indices, input.shape[idx_start:event_pos]),
+        index_ndim=index_ndim
+    )
 
 
 def broadcast_cat(ts: Iterable[Tensor], dim=-1):
     r"""`torch.concatenate` but first broadcast the rest of the dimensions."""
     return cat(broadcast_except(*ts, dim=dim), dim)
 
 
+def broadcast_stack(ts: Iterable[Tensor], dim=0):
+    r"""`torch.stack` but first broadcast the tensors."""
+    return torch.stack(torch.broadcast_tensors(*ts), dim=dim)
+
+
 def insert_dims(t: Tensor, loc: int, shape: Size):
     r"""Inject phony :arg:`shape` into :arg:`t` at the given :arg:`loc`\ ation.
 
     Equivalent to
 
     - `unsqueezing <torch.Tensor.unsqueeze>` :arg:`loc`,
     - `expanding <torch.Tensor.expand>` so that ``t.shape[loc] == shape.numel()``,
```

### Comparing `phytorchx-0.2/phytorchx.egg-info/PKG-INFO` & `phytorchx-0.3/phytorchx.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: phytorchx
-Version: 0.2
+Version: 0.3
 Summary: Small utiilities package for PyTorch
 Author-email: Kosio Karchev <kosiokarchev@gmail.com>
 License: MIT
 Project-URL: GitHub, https://github.com/kosiokarchev/phytorchx
 Project-URL: Read the Docs, https://phytorchx.readthedocs.org/
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: more-itertools
+Requires-Dist: optree
+Requires-Dist: torch
 
 # φtorch-x
 #### *small utilities package for PyTorch*
```

### Comparing `phytorchx-0.2/pyproject.toml` & `phytorchx-0.3/pyproject.toml`

 * *Files identical despite different names*

