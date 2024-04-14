# Comparing `tmp/xtrain-0.2.0.tar.gz` & `tmp/xtrain-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtrain-0.2.0.tar", max compression
+gzip compressed data, was "xtrain-0.2.1.tar", max compression
```

## Comparing `xtrain-0.2.0.tar` & `xtrain-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2024-04-12 13:52:13.296116 xtrain-0.2.0/LICENSE
--rw-r--r--   0        0        0     1231 2024-04-12 13:52:13.296116 xtrain-0.2.0/README.md
--rw-r--r--   0        0        0      833 2024-04-12 13:52:31.264183 xtrain-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      160 2024-04-12 13:52:13.296116 xtrain-0.2.0/xtrain/__init__.py
--rw-r--r--   0        0        0    10295 2024-04-12 13:52:13.296116 xtrain-0.2.0/xtrain/base_trainer.py
--rw-r--r--   0        0        0     1289 2024-04-12 13:52:13.296116 xtrain-0.2.0/xtrain/loss.py
--rw-r--r--   0        0        0     4564 2024-04-12 13:52:13.296116 xtrain-0.2.0/xtrain/strategy.py
--rw-r--r--   0        0        0     5517 2024-04-12 13:52:13.296116 xtrain-0.2.0/xtrain/utils.py
--rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 xtrain-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-04-14 14:01:13.686413 xtrain-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1231 2024-04-14 14:01:13.686413 xtrain-0.2.1/README.md
+-rw-r--r--   0        0        0      833 2024-04-14 14:01:29.298452 xtrain-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      160 2024-04-14 14:01:13.690413 xtrain-0.2.1/xtrain/__init__.py
+-rw-r--r--   0        0        0    10659 2024-04-14 14:01:13.690413 xtrain-0.2.1/xtrain/base_trainer.py
+-rw-r--r--   0        0        0     1399 2024-04-14 14:01:13.690413 xtrain-0.2.1/xtrain/loss.py
+-rw-r--r--   0        0        0     4564 2024-04-14 14:01:13.690413 xtrain-0.2.1/xtrain/strategy.py
+-rw-r--r--   0        0        0     5517 2024-04-14 14:01:13.690413 xtrain-0.2.1/xtrain/utils.py
+-rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 xtrain-0.2.1/PKG-INFO
```

### Comparing `xtrain-0.2.0/LICENSE` & `xtrain-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xtrain-0.2.0/README.md` & `xtrain-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `xtrain-0.2.0/pyproject.toml` & `xtrain-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xtrain"
-version = "0.2.0"
+version = "0.2.1"
 description = "A Flax trainer"
 authors = ["Ji Yu <jyu@uchc.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 flax = "^0.8"
```

### Comparing `xtrain-0.2.0/xtrain/base_trainer.py` & `xtrain-0.2.1/xtrain/base_trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import dataclasses
 import pickle
 from collections.abc import Iterator
 from functools import lru_cache, partial
 from pathlib import Path
-from typing import Callable, Iterable, Protocol, Sequence, Union
+from typing import Callable, Iterable, Protocol, Sequence, Union, Any, runtime_checkable
 
 import flax.linen as nn
 import jax
 import jax.numpy as jnp
 import numpy as np
 import optax
 from flax import struct
@@ -21,30 +21,33 @@
 from .utils import (
     Peekable,
     _get_name,
     unpack_prediction_and_state,
     unpack_x_y_sample_weight,
 )
 
+@runtime_checkable
 class Metric(Protocol):
-    def update(self, batch: Any, prediction: Any):
+    def update(self, batch: Any, prediction: Any) -> Any:
         ...
 
     def compute(self, *args, **kwargs) -> dict:
         ...
 
+PathLike = Path | str
+MetricLike = Metric | LossFunc
 LOSSES = Union[LossFunc, Sequence[LossFunc]]
-METRICS = Union[Metric, Sequence[Metric]]
+METRICS = Union[MetricLike, Sequence[MetricLike]]
 RNG = jax.Array
+Optimizer = Any
 
 # so that multiple calls return the same obj
 # this avoids JIT when supplying partial func as args
 _cached_partial = lru_cache(partial)
 
-
 @partial(struct.dataclass, frozen=False)
 class TrainIterator(Iterator):
     """The iterator obj returned by Trainer.train(). Iterating this object drives the training. The object supports orbax checkpointing.
 
     Example:
         ```
         import orbax.checkpoint as ocp
@@ -189,15 +192,15 @@
 
         return self.strategy.init_fn(rng, self.model, inputs)
 
     def train(
         self,
         dataset: Iterable,
         strategy: type | None = None,
-        rng_cols: Sequence[str] = [],
+        rng_cols: Sequence[str] = ["dropout"],
         init_vars: dict | None = None,
         frozen: dict | None = None,
         **kwargs,
     ) -> TrainIterator:
         """Create the training iterator
 
         Args:
@@ -223,16 +226,17 @@
 
         seed = (
             self.seed
             if isinstance(self.seed, jnp.ndarray)
             else jax.random.PRNGKey(self.seed)
         )
 
-        rng_cols = rng_cols or []
-
+        rng_cols = rng_cols or ["dropout"]
+        if isinstance(rng_cols, str):
+            rng_cols = [rng_cols]
         seed, key = jax.random.split(seed)
         keys = jax.random.split(key, len(rng_cols))
         rngs = dict(zip(rng_cols, keys))
 
         if init_vars is None:
             seed, key = jax.random.split(seed)
             keys = jax.random.split(seed, len(rng_cols) + 1)
@@ -303,18 +307,21 @@
         Returns:
             An iterator. Stepping through it will drive the updating of each metric
                 obj. The iterator itself return the list of metrics.
         """
         if strategy is None:
             strategy = self.strategy
 
+        if isinstance(metrics, str):
+            metrics = [metrics]
         try:
             iter(metrics)
         except TypeError:
             metrics = [metrics]
+        metrics = [m if isinstance(m, Metric) else LossLog(m) for m in metrics]
 
         apply_fn = _cached_partial(self.model.apply, **kwargs)
 
         predict_fn = strategy.predict
 
         for data in dataset:
             inputs, _, _ = unpack_x_y_sample_weight(data)
```

### Comparing `xtrain-0.2.0/xtrain/loss.py` & `xtrain-0.2.1/xtrain/loss.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 from __future__ import annotations
 
-from typing import Protocol, Sequence, Union
+from typing import Protocol, Sequence, Union, Any
 
 from functools import partial
 
 import jax.numpy as jnp
 from flax import struct
 
 from .utils import _get_name
 
 class LossFunc_(Protocol):
     def __call__(self, batch: Any, prediction: Any) -> float:
         ...
 
 LossFunc = LossFunc_ | str
 
-
 @partial(struct.dataclass, frozen=False)
 class LossLog:
     loss_fn: LossFunc = struct.field(pytree_node=False)
     weight: float = 1.0
     cnt: float = 0.0
     sum: float = 0.0
 
-    # update() is meant to be called in JAX transformation so it cannot
-    # modify its fields. Instead it returns a new copy of self.
+    def __post_init__(self):
+        self.__name__ = _get_name(self.loss_fn)
+
+    # update() is meant to be called in JAX transformation, where objects are immutable
+    # so it returns a copy of self in order for the caller to track changes to the object.
     def update(self, batch, prediction):
         if isinstance(self.loss_fn, str):
             loss = prediction
             for k in self.loss_fn.split("/"):
                 loss = loss[k]
         else:
             loss = self.loss_fn(batch, prediction)
 
         if loss is None:
             return 0.0, self
 
         loss *= self.weight
+        self.cnt += 1
+        self.sum += loss
 
-        return loss, self.replace(cnt=self.cnt + 1, sum=self.sum + loss)
+        return loss, self
 
     def compute(self):
         return self.sum / self.cnt
 
     def reset(self):
         self.cnt = 0.0
         self.sum = 0.0
 
     def __repr__(self) -> str:
-        return _get_name(self.loss_fn) + f": {float(self.sum / self.cnt):.4f}"
+        return self.__name__ + f": {float(self.compute()):.4f}"
```

### Comparing `xtrain-0.2.0/xtrain/strategy.py` & `xtrain-0.2.1/xtrain/strategy.py`

 * *Files identical despite different names*

### Comparing `xtrain-0.2.0/xtrain/utils.py` & `xtrain-0.2.1/xtrain/utils.py`

 * *Files identical despite different names*

### Comparing `xtrain-0.2.0/PKG-INFO` & `xtrain-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtrain
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Flax trainer
 Author: Ji Yu
 Author-email: jyu@uchc.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

