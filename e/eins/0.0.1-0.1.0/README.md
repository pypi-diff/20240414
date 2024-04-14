# Comparing `tmp/eins-0.0.1.tar.gz` & `tmp/eins-0.1.0.tar.gz`

## Comparing `eins-0.0.1.tar` & `eins-0.1.0.tar`

### file list

```diff
@@ -1,36 +1,49 @@
--rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 eins-0.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 eins-0.0.1/algorithm.md
--rw-r--r--   0        0        0     7355 2020-02-02 00:00:00.000000 eins-0.0.1/benchmarking.ipynb
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 eins-0.0.1/examples.ipynb
--rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 eins-0.0.1/examples.md
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 eins-0.0.1/examples.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 eins-0.0.1/mkdocs.yml
--rw-r--r--   0        0        0    94367 2020-02-02 00:00:00.000000 eins-0.0.1/network.ipynb
--rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 eins-0.0.1/parsing.md
--rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 eins-0.0.1/perf.ipynb
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 eins-0.0.1/.github/workflows/main.yml
--rw-r--r--   0        0        0     4873 2020-02-02 00:00:00.000000 eins-0.0.1/docs/in-depth.md
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 eins-0.0.1/docs/index.md
--rw-r--r--   0        0        0     4222 2020-02-02 00:00:00.000000 eins-0.0.1/docs/tutorial.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 eins-0.0.1/src/eins/__about__.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 eins-0.0.1/src/eins/__init__.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 eins-0.0.1/src/eins/combination.py
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 eins-0.0.1/src/eins/common_types.py
--rw-r--r--   0        0        0     3381 2020-02-02 00:00:00.000000 eins-0.0.1/src/eins/concrete.py
--rw-r--r--   0        0        0     8520 2020-02-02 00:00:00.000000 eins-0.0.1/src/eins/constraint.py
--rw-r--r--   0        0        0    14150 2020-02-02 00:00:00.000000 eins-0.0.1/src/eins/einsop.py
--rw-r--r--   0        0        0     2360 2020-02-02 00:00:00.000000 eins-0.0.1/src/eins/elementwise.py
--rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 eins-0.0.1/src/eins/namespaces.py
--rw-r--r--   0        0        0     4453 2020-02-02 00:00:00.000000 eins-0.0.1/src/eins/parsing.py
--rw-r--r--   0        0        0     7676 2020-02-02 00:00:00.000000 eins-0.0.1/src/eins/reduction.py
--rw-r--r--   0        0        0    17708 2020-02-02 00:00:00.000000 eins-0.0.1/src/eins/symbolic.py
--rw-r--r--   0        0        0     6211 2020-02-02 00:00:00.000000 eins-0.0.1/src/eins/transformation.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 eins-0.0.1/src/eins/utils.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 eins-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 eins-0.0.1/tests/test_basic.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 eins-0.0.1/tests/test_parsing.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 eins-0.0.1/.gitignore
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 eins-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0     4624 2020-02-02 00:00:00.000000 eins-0.0.1/README.md
--rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 eins-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     6097 2020-02-02 00:00:00.000000 eins-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 eins-0.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 eins-0.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 eins-0.1.0/algorithm.md
+-rw-r--r--   0        0        0    12443 2020-02-02 00:00:00.000000 eins-0.1.0/benchmarking.ipynb
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 eins-0.1.0/examples.ipynb
+-rw-r--r--   0        0        0     3660 2020-02-02 00:00:00.000000 eins-0.1.0/examples.md
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 eins-0.1.0/examples.py
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 eins-0.1.0/mkdocs.yml
+-rw-r--r--   0        0        0    16996 2020-02-02 00:00:00.000000 eins-0.1.0/network.ipynb
+-rw-r--r--   0        0        0     7173 2020-02-02 00:00:00.000000 eins-0.1.0/parsing.md
+-rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 eins-0.1.0/perf.ipynb
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 eins-0.1.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 eins-0.1.0/docs/in-depth.md
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 eins-0.1.0/docs/index.md
+-rw-r--r--   0        0        0    16072 2020-02-02 00:00:00.000000 eins-0.1.0/docs/tutorial.md
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 eins-0.1.0/docs/javascripts/katex.js
+-rw-r--r--   0        0        0   201364 2020-02-02 00:00:00.000000 eins-0.1.0/docs/stylesheets/CascadiaCode.woff2
+-rw-r--r--   0        0        0   143760 2020-02-02 00:00:00.000000 eins-0.1.0/docs/stylesheets/CascadiaCodeItalic.woff2
+-rw-r--r--   0        0        0   202128 2020-02-02 00:00:00.000000 eins-0.1.0/docs/stylesheets/InstrumentSans-Italic[wdth,wght].ttf
+-rw-r--r--   0        0        0   194336 2020-02-02 00:00:00.000000 eins-0.1.0/docs/stylesheets/InstrumentSans[wdth,wght].ttf
+-rw-r--r--   0        0        0     1522 2020-02-02 00:00:00.000000 eins-0.1.0/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     4064 2020-02-02 00:00:00.000000 eins-0.1.0/docs/stylesheets/readme.md
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 eins-0.1.0/examples/README.md
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 eins-0.1.0/examples/multi_head_attention.py
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 eins-0.1.0/examples/vit_encoder.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/__about__.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/__init__.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/combination.py
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/common_types.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/concrete.py
+-rw-r--r--   0        0        0     9104 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/constraint.py
+-rw-r--r--   0        0        0    19810 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/einsop.py
+-rw-r--r--   0        0        0     4988 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/elementwise.py
+-rw-r--r--   0        0        0     7537 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/namespaces.py
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/parsing.py
+-rw-r--r--   0        0        0    14784 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/program.py
+-rw-r--r--   0        0        0     8007 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/reduction.py
+-rw-r--r--   0        0        0     5674 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/strategy.py
+-rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/symbolic.py
+-rw-r--r--   0        0        0    10496 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/transformation.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 eins-0.1.0/src/eins/utils.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 eins-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 eins-0.1.0/tests/test_basic.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 eins-0.1.0/tests/test_parsing.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 eins-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 eins-0.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     4300 2020-02-02 00:00:00.000000 eins-0.1.0/README.md
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 eins-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 eins-0.1.0/PKG-INFO
```

### Comparing `eins-0.0.1/CODE_OF_CONDUCT.md` & `eins-0.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `eins-0.0.1/algorithm.md` & `eins-0.1.0/algorithm.md`

 * *Files identical despite different names*

### Comparing `eins-0.0.1/examples.ipynb` & `eins-0.1.0/examples.ipynb`

 * *Files identical despite different names*

### Comparing `eins-0.0.1/examples.md` & `eins-0.1.0/examples.md`

 * *Files identical despite different names*

### Comparing `eins-0.0.1/parsing.md` & `eins-0.1.0/parsing.md`

 * *Files identical despite different names*

### Comparing `eins-0.0.1/perf.ipynb` & `eins-0.1.0/perf.ipynb`

 * *Files identical despite different names*

### Comparing `eins-0.0.1/.github/workflows/main.yml` & `eins-0.1.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `eins-0.0.1/docs/in-depth.md` & `eins-0.1.0/docs/in-depth.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-# Eins In Depth
+# Advanced Eins
 
-If you just want examples of common operations in Eins, consult the [tutorial](tutorial.md). If you're interested in
-maximizing the power of Eins, you're in the right place!
+If you're totally new to Eins or `einops` and want to see what the fuss is about, read the
+[tutorial](tutorial.md). If you're interested in maximizing the power of Eins, you're in the right
+place!
 
 ```py
 from eins import EinsOp
 ```
 
-## Mathematical Functions
+## Beyond Tensor Shapes
 
 Consider an operation `a b, b c -> a c`. This could be matrix multiplication, but it could also be pairwise distances or
 many other things. To control the computation that's being performed beyond the shapes of the inputs and output, Eins
 defines four kinds of functions that specify what's actually happening:
 
 ### Combinations
 Combinations are elementwise functions that combine two arrays into a new array of the same shape. The default,
@@ -46,48 +47,66 @@
 ### Transformations
 Named after the `.transform` method in Pandas, transformations take in a single array and `axis`, like reductions, but
 they don't eliminate the axis. For example, `np.sort(arr, axis=0)` is different than `np.sort(arr, axis=1)`, but both
 return the same shape.
 
 Just like a folded combination becomes a reduction, a *scanned* or *accumulated* combination becomes a transformation.
 Note that the way NumPy and other libraries notate these differs from the idea of a scan. `cumprod`, in Eins, is really
-just an alias for `cummultiply`, because Eins uses the combination rather than the reduction.
+just an alias for `cummultiply`, because Eins uses the combination rather than the reduction. If you have an array with elements `[a, b, c, d]` and an operator like `*`, then Eins computes
+
+```python
+[a, a * b, (a * b) * c, ((a * b) * c) * d]
+```
 
 **Common examples**: `'sort'`, `'l2_normalize'`, `'min_max_normalize'`
 
 ### Composing Functions
 
 Eins uses `combine` and `reduce` arguments that specify how to combine inputs and how to reduce axes. The point of
 elementwise operations and transformations is that they can be composed with combinations and reductions.
 
 Functions are applied right-to-left, matching existing nomenclature and function composition. For example, if
 `'logaddexp'` weren't already a supported combination, you could replicate the functionality as `('log', 'add', 'exp')`.
 This computes the logarithm of the sum of the exponentials of the inputs.
 
-Similarly, if you wanted to compute root-mean-square error along an axis, you could use `reduce=('sqrt', 'mean', 'square')`.
+Similarly, if you wanted to compute root-mean-square error along an axis, you could use
+`reduce=('sqrt', 'mean', 'square')`. This is common enough to get its own name: `'l2_norm'`.
 
 ### Explicit Function Objects
 
 Eins supports a relatively sophisticated "stringly-typed" input format, as you've seen above. This means you rarely need
 any imports beyond `EinsOp`, and plays nicely with any kind of config files or serialization, but it does also make it
 harder to know what functions Eins defines or use your own.
 
 If you prefer, you can instead pass in explicit objects: `Combination`, `Reduction`, `ElementwiseOp`, and
 `Transformation`. These are each base classes that you can implement yourself, but it's easiest to use the associated
-object exported from the base namespace: `Combinations`, `Reductions`, etc. These have methods for creating different
-kinds of functions and class constants for the pre-defined functions you're most likely to use.
+object exported from the base namespace: `Combinations`, `Reductions`, etc. These namespaces provide an autocomplete-friendly way of using these operations.
 
 Explicit objects are the only way to specify compositions with function syntax. If you pass in a callable to `combine`
 or `reduce`, Eins will assume it has the correct signature, but if you pass in `(my_func1, my_func2)` Eins has no way of
 knowing what's what. Instead, you can do:
 
-```py
+```py title="Batched Kurtosis"
 from eins import EinsOp, Reductions as R, ElementwiseOps as E
 from scipy.stats import kurtosis
 # kurtosis has signature (x, axis=0, ...)
 
-# Batched absolute value kurtosis: measures non-normality
-EinsOp(
-  'batch dim -> batch'
-  reduce = (E.abs, R.from_func(kurtosis))
-)
+EinsOp('batch sample_size -> batch', reduce=(E.abs, R.from_func(kurtosis)))
+```
+
+## Standalone Operator Usage
+
+For backend-agnostic code or simply as a wrapper for functionality Eins implements that isn't available in all libraries, there's no reason you can't just use the above functions outside of an EinsOp context:
+
+```python
+from eins import Reductions as R, Transformations as T
+
+# 1.5-norm: somewhere between Manhattan and Euclidean distance
+# akin to torch.nn.functional.normalize, but no direct numpy equivalent
+
+data = np.random.randn(128, 64)
+
+R.PowerNorm(1.5)(data, axis=1)
+
+# Normalize so the 1.5-norm is 1: same shape as input
+T.PowerNormalize(1.5)(data, axis=1)
 ```
```

### Comparing `eins-0.0.1/src/eins/combination.py` & `eins-0.1.0/src/eins/combination.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,17 @@
 
 @dataclass(frozen=True, unsafe_hash=True)
 class ArrayCombination(Combination):
     """Combination operation defined in Array API."""
 
     func_name: str
 
+    def __repr__(self):
+        return repr(self.func_name)
+
     def __str__(self):
         return self.func_name
 
     @classmethod
     def parse(cls, name: str):
         if name in ARRAY_COMBINE_OPS:
             return cls(name)
@@ -49,15 +52,15 @@
             raise ValueError(msg)
 
         arr = arrs[0]
         xp = array_backend(arr)
         if xp is not None and hasattr(xp, self.func_name):
             func = getattr(xp, self.func_name)
         elif hasattr(arr, self.func_name):
-            func = lambda x, y: getattr(x, self.func_name)(y)  # noqa: E731
+            func = lambda x, y: getattr(x, self.func_name)(y)
         else:
             msg = f'Name {self.func_name} not a valid function for array of type {type(arr)}'
             raise ValueError(msg) from None
 
         out = arrs[0]
         for other in arrs[1:]:
             out = func(out, other)
@@ -80,15 +83,15 @@
 
     ops: Sequence[Union[ElementwiseOp, Combination]]
 
     def __call__(self, arr1: Array, arr2: Array) -> Array:
         arrs = (arr1, arr2)
         out = arrs
         combines = 0
-        for op in self.ops:
+        for op in self.ops[::-1]:
             if isinstance(op, Combination):
                 combines += 1
                 if combines > 1:
                     msg = f'{self} has more than one combination operation'
                     raise ValueError(msg)
                 out = [op(*arrs)]
             else:
@@ -104,7 +107,8 @@
     if arr_parse is not None:
         return arr_parse
     else:
         return None
 
 
 ops = {str(op): parse_combination(op) for op in typing.get_args(CombineLiteral)}
+ops = {k: v for k, v in ops.items() if v is not None}
```

### Comparing `eins-0.0.1/src/eins/common_types.py` & `eins-0.1.0/src/eins/common_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,13 @@
 """Type definitions"""
 
 from abc import ABCMeta, abstractmethod
-from typing import Callable, Optional, Protocol, Sequence, Tuple, Union
+from typing import Callable, Optional, Protocol, Sequence, Tuple, TypeVar, Union
 
-
-class Array(Protocol):
-    """Array functionality required for Eins to work."""
-
-    def __getitem__(
-        self,
-        key: Union[int, slice, Tuple[Union[int, slice], ...]],
-    ) -> 'Array': ...
-
-    @property
-    def shape(self) -> Sequence[int]: ...
-
-    @property
-    def ndim(self) -> int: ...
+Array = TypeVar('Array')
 
 
 class Reduction(metaclass=ABCMeta):
     """
     A function with signature f(Array, axis: int) → Array that removes the axis. Common examples:
     sum, product, mean, norm.
     """
```

### Comparing `eins-0.0.1/src/eins/concrete.py` & `eins-0.1.0/src/eins/concrete.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 """Concrete implementations of the shape operations."""
 
-from typing import Sequence
+from typing import Sequence, cast
 
-from array_api_compat import array_namespace
+from array_api_compat import array_namespace, is_jax_array
 
 from eins.common_types import Array
 from eins.constraint import Constraints
 from eins.parsing import Expr
 from eins.symbolic import (
     Combine,
     Concat,
     ExpandTo,
     Reduce,
     Reshape,
     ShapeOp,
     Split,
     Tensor,
+    Tile,
+    Transform,
     Transpose,
 )
 
 
 class ArrayBackend:
     def __init__(self, constr: Constraints):
         self.constr = constr
 
     def do(
         self, x: Sequence[Array], op: ShapeOp, ins: Sequence[Tensor], _outs: Sequence[Tensor]
-    ) -> Sequence[Array]:
+    ) -> Sequence['Array']:
         "Apply the op, which goes from i to o, on x, an actual array."
         if len(x) == 0:
             msg = 'Cannot call operation on empty inputs'
             raise ValueError(msg)
 
         xp = array_namespace(*x)
 
         try:
-            if isinstance(op, Reshape):
+            if op.is_identity_for(ins):
+                # no-op
+                return x
+            elif isinstance(op, Reshape):
                 new_shape = tuple(map(self.constr.value_of, op.new_shape))
                 return [xp.reshape(x[0], shape=new_shape)]
             elif isinstance(op, Transpose):
                 return [xp.permute_dims(x[0], axes=op.perm)]
             elif isinstance(op, Split):
                 split_ax = ins[0].axes[op.axis_num]
                 if not (isinstance(split_ax, Expr) and split_ax.op == '+'):
@@ -48,14 +53,15 @@
 
                 sizes = []
                 for child in split_ax.children:
                     val = self.constr.value_of(child)
                     if val is None:
                         msg = f'Could not compute value of {child} for split operation.'
                         raise ValueError(msg)
+                    sizes.append(val)
 
                 out = []
                 curr = 0
                 for size in sizes:
                     slc = [slice(None) for _ in range(x[0].ndim)]
                     slc[op.axis_num] = slice(curr, curr + size)
                     out.append(x[0][tuple(slc)])
@@ -70,20 +76,52 @@
                     if i < len(ins[0].axes) and out_ax == ins[0].axes[i]:
                         slc.append(slice(None))
                         i += 1
                     else:
                         slc.append(None)
 
                 return [x[0][tuple(slc)]]
+            elif isinstance(op, Tile):
+                # Tile isn't in the version of the Array API that the Array API supports,
+                # annoyingly. We try to wrap it as best we can.
+                tiles = []
+                if len(op.new_shape) != len(x[0].shape):
+                    msg = f'Shape {x[0].shape} cannot be tiled to{op.new_shape}: shapes must match.'
+                    raise ValueError(msg)
+
+                for out_ax, in_len in zip(op.new_shape, x[0].shape):
+                    out_len = self.constr.value_of(out_ax)
+                    if out_len % in_len != 0:
+                        msg = f'Cannot tile: {in_len} does not divide {out_len}'
+                        msg += f': {x[0]}, {op.new_shape}'
+                        raise ValueError(msg)
+                    tiles.append(out_len // in_len)
+
+                if hasattr(xp, 'tile'):
+                    return [xp.tile(x[0], tuple(tiles))]
+                elif is_jax_array(x[0]):
+                    # workaround: use jnp.tile
+                    from jax.numpy import tile
+                    from jax.typing import ArrayLike
+
+                    return [tile(cast(ArrayLike, x[0]), tuple(tiles))]
+                else:
+                    msg = (
+                        f'Array of type {type(x[0])!s} does not support tiling. '
+                        'Repeat functionality will not be supported.'
+                    )
+                    raise ValueError(msg)
             elif isinstance(op, Combine):
                 # return [op.method(*xp.broadcast_arrays(*x))]
                 return [op.method(*x)]
             elif isinstance(op, Reduce):
                 # print(ins, _outs, op, id(_outs[0]))
                 return [op.method(x[0], axis=ins[0].axes.index(op.axis))]
+            elif isinstance(op, Transform):
+                return [op.method(x[0], axis=ins[0].axes.index(op.axis))]
             else:
                 msg = 'Op not supported: ' + str(op)
                 raise TypeError(msg)
         except TypeError as err:
             msg = (
                 'An error occurred when applying the operation.\n'
                 f'Operation: {op}\n'
```

### Comparing `eins-0.0.1/src/eins/constraint.py` & `eins-0.1.0/src/eins/constraint.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         if (lhs, rhs) not in self.equations:
             self.equations.append((lhs, rhs))
 
     def process_constraints(self, node: Node):
         if isinstance(node, Expr):
             for i, child in enumerate(node.children):
                 if isinstance(child, Expr) and child.op == '=':
-                    if len(child.children) != 2:  # noqa: PLR2004
+                    if len(child.children) != 2:
                         msg = 'Must have exactly two parts to equality'
                         raise ValueError(msg)
                     lhs, rhs = child.children
                     self.equations.append((lhs, rhs))
                     node.children[i] = lhs
 
     def replace_referents(self, node: Node):
@@ -44,15 +44,17 @@
                     if child == lhs:
                         node.children[i] = rhs
 
     def replace_constants(self, node: Node):
         if isinstance(node, Expr):
             for i, child in enumerate(node.children):
                 if isinstance(child, Constant):
+                    sym = Symbol(str(child.value))
                     node.children[i] = Symbol(str(child.value))
+                    self.equations.append((sym, child))
 
     def disambiguate_axes(self, node: Node, curr_axes: Optional[MutableSequence[str]] = None):
         if curr_axes is None:
             curr_axes = []
         if isinstance(node, Expr):
             if node.op in (',', '->', '@'):
                 for i, child in enumerate(node.children):
@@ -67,14 +69,16 @@
         elif isinstance(node, Symbol):
             num = 1
             orig_value = node.value
             node_value = orig_value
             while node_value in curr_axes:
                 num += 1
                 # use - because it's not allowed in user identifiers
+                # if you ever change this, you need to change the logic in Program that adds
+                # the constraints!
                 node_value = f'{orig_value}-{num}'
 
             curr_axes.append(node_value)
             if num > 1:
                 new_node = Symbol(node_value)
                 self.add_constraint(new_node, node)
                 return new_node
@@ -88,15 +92,21 @@
             elif v in self.free_vars:
                 continue
             else:
                 self.free_vars.append(v)
 
     def fill_in(self, values: Mapping[Symbol, int]):
         for k, v in values.items():
-            self.free_vars.remove(k.value)
+            if k.value in self.free_vars:
+                self.free_vars.remove(k.value)
+            else:
+                old_v = self.known_vars[k.value]
+                if old_v != v:
+                    msg = f'Conflicting values for {k.value}: {old_v} and {v}'
+                    raise ValueError(msg)
             self.known_vars[k.value] = v
 
     def value_of(self, node: Union[Node, str, int]) -> Optional[int]:
         if isinstance(node, str):
             return self.known_vars.get(node)
         elif isinstance(node, int):
             return node
@@ -135,18 +145,20 @@
             '+': lambda x, n: x // n,
             '*': lambda x, n: int(x ** (1 / n)),
         }
         lhs_val = self.value_of(lhs)
         rhs_val = self.value_of(rhs)
         if lhs_val is not None and rhs_val is not None:
             if lhs_val != rhs_val:
+                eqns = '\n'.join(f'{lhs} = {rhs}' for lhs, rhs in self.equations)
                 msg = f"""Incompatible shapes given. The operation requires that {lhs} = {rhs}, but
 the deduced values of {lhs_val} and {rhs_val} are not equal.
 
 Deduced values: {self.known_vars}
+Equations:\n{eqns}
 """
                 raise ValueError(msg)
             return []
         elif lhs_val is not None:
             return self.reduce_eqn(rhs, lhs)
         elif (lhs_val, rhs_val) == (None, None):
             return [(lhs, rhs)]
```

### Comparing `eins-0.0.1/src/eins/einsop.py` & `eins-0.1.0/src/eins/einsop.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,78 @@
 """User-facing API."""
 
 import typing
 from itertools import chain
+from string import ascii_uppercase
 from typing import AnyStr, Callable, Mapping, MutableMapping, Optional, Sequence, Union
 
 from eins.combination import (
-    ARRAY_COMBINE_OPS,
     Combination,
     CombineLiteral,
     CompositeCombination,
     CustomCombination,
     parse_combination,
 )
+from eins.combination import (
+    ops as _combination_ops,
+)
 from eins.common_types import Array
 from eins.concrete import ArrayBackend
 from eins.elementwise import ElementwiseLiteral, ElementwiseOp, parse_elementwise
+from eins.elementwise import ops as _elementwise_ops
 from eins.parsing import Constant, Symbol
+from eins.program import Program, TransformProgram
 from eins.reduction import (
-    ARRAY_REDUCE_OPS,
     CompositeReduction,
     CustomReduction,
     Reduction,
     ReductionLiteral,
     parse_reduction,
 )
-from eins.symbolic import Program, Tensor
-from eins.transformation import Transformation, TransformationLiteral, parse_transformation
+from eins.reduction import (
+    ops as _reduction_ops,
+)
+from eins.strategy import BaseStrategy
+from eins.symbolic import Tensor
+from eins.transformation import (
+    CompositeTransformation,
+    CustomTransformation,
+    Transformation,
+    TransformationLiteral,
+    parse_transformation,
+)
+from eins.transformation import ops as _transformation_ops
 
 ElementwiseKind = Union[ElementwiseLiteral, Callable, ElementwiseOp]
 # use AnyStr to ensure autocomplete works
 # https://stackoverflow.com/questions/77012761/literal-string-union-autocomplete-for-python
 ReductionKind = Union[ReductionLiteral, AnyStr, Callable, Reduction]
 CombinationKind = Union[CombineLiteral, Callable, Combination]
 TransformationKind = Union[TransformationLiteral, Transformation]
 
 GeneralReductionKind = Union[
     ReductionKind, Sequence[Union[ElementwiseKind, TransformationKind, ReductionKind]]
 ]
 ReduceArg = Union[GeneralReductionKind, Mapping[str, GeneralReductionKind]]
-
 CombineArg = Union[CombinationKind, Sequence[Union[ElementwiseKind, CombinationKind]]]
+TransformArg = Union[TransformationKind, Sequence[Union[ElementwiseKind, TransformationKind]]]
 
 
 def _parse_reduce_arg(reduce: GeneralReductionKind) -> Reduction:
     if isinstance(reduce, Reduction):
         return reduce
     elif isinstance(reduce, Callable):
         return CustomReduction(reduce)
     elif isinstance(reduce, str):
         reduce_parse = parse_reduction(reduce)
         if reduce_parse is not None:
             return reduce_parse
 
         msg = f'Cannot parse reduction {reduce}. Valid literals are: ' + ', '.join(
-            ARRAY_REDUCE_OPS + ARRAY_COMBINE_OPS
+            list(_reduction_ops) + list(_combination_ops)
         )
         raise ValueError(msg)
     else:
         ops = []
         for op in reduce:
             if isinstance(op, (ElementwiseOp, Reduction, Transformation)):
                 ops.append(op)
@@ -100,27 +115,70 @@
                 )
             )
             raise ValueError(msg)
 
         return CompositeReduction(tuple(ops))
 
 
+def _parse_transform_arg(transform: TransformArg) -> Transformation:
+    if isinstance(transform, Transformation):
+        return transform
+    elif isinstance(transform, Callable):
+        return CustomTransformation(transform)
+    elif isinstance(transform, str):
+        combo_parse = parse_transformation(transform)
+        if combo_parse is not None:
+            return combo_parse
+
+        msg = f'Cannot parse transformation {transform}. Valid literals: {", ".join(_transformation_ops)}'
+        raise ValueError(msg)
+    else:
+        ops = []
+        for op in transform:
+            if isinstance(op, (ElementwiseOp, Transformation)):
+                ops.append(op)
+                continue
+
+            if isinstance(op, Callable):
+                # callables are ambiguous here
+                msg = f"""
+User-supplied function in transform={transform} is ambiguous: either write a custom lambda combining
+these operations or explicitly create objects using e.g., eins.ElementwiseOps.from_func().
+                      """
+                raise ValueError(msg)
+
+            op_parse = parse_transformation(op)
+            if op_parse is not None:
+                ops.append(op_parse)
+                continue
+
+            op_parse = parse_elementwise(op)
+            if op_parse is not None:
+                ops.append(op_parse)
+                continue
+
+            msg = f'Cannot parse operation {op} in {ops}. Valid literals: ' + (
+                '\n'.join([', '.join(list(_transformation_ops) + list(_elementwise_ops))])
+            )
+            raise ValueError(msg)
+
+        return CompositeTransformation(tuple(ops))
+
+
 def _parse_combine_arg(combine: CombineArg) -> Combination:
     if isinstance(combine, Combination):
         return combine
     elif isinstance(combine, Callable):
         return CustomCombination(combine)
     elif isinstance(combine, str):
         combo_parse = parse_combination(combine)
         if combo_parse is not None:
             return combo_parse
 
-        msg = (
-            f'Cannot parse reduction {combine}. Valid literals are: {", ".join(ARRAY_COMBINE_OPS)}'
-        )
+        msg = f'Cannot parse combination {combine}. Valid literals: {", ".join(_combination_ops)}'
         raise ValueError(msg)
     else:
         ops = []
         for op in combine:
             if isinstance(op, (ElementwiseOp, Combination)):
                 ops.append(op)
                 continue
@@ -139,21 +197,16 @@
                 continue
 
             op_parse = parse_elementwise(op)
             if op_parse is not None:
                 ops.append(op_parse)
                 continue
 
-            msg = f'Cannot parse operation {op} in {ops}. Valid literals are: ' + (
-                '\n'.join(
-                    [
-                        ', '.join(typing.get_args(ops))
-                        for ops in (CombineLiteral, ElementwiseLiteral)
-                    ]
-                )
+            msg = f'Cannot parse operation {op} in {ops}. Valid literals: ' + (
+                '\n'.join([', '.join(list(_combination_ops) + list(_elementwise_ops))])
             )
             raise ValueError(msg)
 
         return CompositeCombination(tuple(ops))
 
 
 class EinsOp:
@@ -162,86 +215,154 @@
     def __init__(
         self,
         op: str,
         /,
         *,
         reduce: ReduceArg = 'sum',
         combine: CombineArg = 'multiply',
+        transform: Optional[Mapping[str, TransformArg]] = None,
         symbol_values: Optional[Mapping[str, int]] = None,
     ):
         """
         A tensor operation that takes in tensors of the given shapes and outputs a tensor of the
         given shape. Has a generic, powerful shape description language that supports the majority
         of tensor operations.
 
         Parameters
         ----------
-        op:
-            The description of the operation. For example, `'a b, b c -> a c'` performs matrix
-            multiplication, and `'batch (size size) channels -> batch size size channels'` unpacks a
-            batch of square images.
+        op: str or sequence of strs
+            The description of the operation.
+
+            If a list of strings is passed in, the last string is assumed to be the output, and the
+            others are assumed to be inputs.
+
+            For example, `'a b, b c -> a c'` performs matrix multiplication. There is a lot of
+            supported syntax: consult the tutorial for more information.
 
-        reduce: function f(Array, axis: int) → Array, Reduction, str, or mapping from axes to
-        previous
+        reduce: function, Reduction, str, sequence of ops, or mapping from axes to previous
             Describes how axes that appear in the input but not the output are eliminated: use
-            [eins.Reductions] to get an autocomplete-friendly list of options. The default is
-            `'sum'`, like in `einsum`. Common alternatives are `'mean'`, `'std'`, `'max'`, and
-            `'min'`. This can also be a combine operation, which is reduced in the functional
-            programming sense. For example, `'add'` would perform the same reduction as `'sum'` but
-            in a less efficient loop. You can also pass in a function: it should be callable as
-            `func(arr, axis=0)` and return an array with that axis eliminated. `eins` makes no
-            guarantees about the order reductions are performed.
+            [eins.Reductions] to get an autocomplete-friendly list of options.
+
+            The default is `'sum'`, like in `einsum`. Common alternatives are `'mean'`, `'std'`,
+            `'max'`, and `'min'`. This can also be a combine operation, which is reduced in the
+            functional programming sense. For example, `'add'` would perform the same reduction as
+            `'sum'` but in a less efficient loop. You can also pass in a function: it should be
+            callable as `func(arr, axis=0)` and return an array with that axis eliminated. `eins`
+            makes no guarantees about the order reductions are performed.
 
             For even more flexibility, this can be any of the previous inputs "sandwiched" by
             elementwise operations. For example, `('log', 'sum', 'exp')` would be equivalent to
             `logsumexp`. Note that passing in custom callables here is not allowed, because `eins`
             doesn't know whether a user-supplied function is an elementwise operation or not. Use a
             lambda instead.
 
             The final option is to pass in a mapping from axes to any of the previous reduction
             operation specifications. `eins` makes no guarantees about the order reductions are
             performed unless explicitly indicated, so be careful. `'a b c -> a', reduce={'b': 'max',
             'c': 'min'}` has two meanings, depending on which happens first. Instead, you can pass
             `'a b c -> a b -> a'`, which forces a specific order.
 
-        combine:
+        combine: function, Combination, str, sequence of ops, or mapping from axes to previous
             Describes how the elements of different input tensors are combined: use
-            [eins.Combinations] to get an autocomplete-friendly list of options. The default is
-            `'multiply'`, which is what `einsum` does. This can be a list of elementwise operations
-            and a single combination operation, like reduce: `('log', 'add', 'exp')` would be a less
-            efficient equivalent operation to `'logaddexp'`.
+            [eins.Combinations] to get an autocomplete-friendly list of options.
+
+            The default is `'multiply'`, which is what `einsum` does. This can be a list of
+            elementwise operations and a single combination operation, like reduce: `('log', 'add',
+            'exp')` would be a less efficient equivalent operation to `'logaddexp'`.
 
             A custom callable should be callable as `func(arr1, arr2)` and return an array of the
             same shape as the two inputs. `eins` makes no guarantees about the order combinations
             are performed, so this function should be commutative and associative.
 
+        transform: mapping from axes to: function, Transformation, str, or sequence of previous
+
         symbol_values: mapping from symbols to integers or None
             An alternative to using = to specify axis values.
         """
-        if '->' not in op:
-            msg = f'Einsop "{op}" has no "->", which is required'
+        if transform is None:
+            transform = {}
+
+        if '->' not in op and len(transform) == 0:
+            msg = f'Einsop "{op}" has no "->", which is required unless transform is given.'
             raise ValueError(msg)
+        elif '->' in op and len(transform) > 0:
+            msg = f'Einsop "{op}" has "->", which is not allowed with transform.'
+            raise ValueError(msg)
+
+        self.is_transform = len(transform) > 0
 
-        self.op_str = op
+        if isinstance(op, str):
+            self.op_str = op
+        elif len(op) == 0:
+            msg = 'EinsOp must have at least one operation.'
+            raise ValueError(msg)
+        elif len(op) == 1:
+            self.op_str = op[0]
+        else:
+            *inputs, output = op[-1]
+            self.op_str = ', '.join(inputs) + ' -> ' + output
 
-        if isinstance(reduce, Mapping):
-            self.reduce = {k: _parse_reduce_arg(v) for k, v in reduce.items()}
+        if self.is_transform:
+            self.transform = {k: _parse_transform_arg(v) for k, v in transform.items()}
+            self.program = TransformProgram.parse(self.op_str, transform=self.transform)
         else:
-            self.reduce = _parse_reduce_arg(reduce)
+            if isinstance(reduce, Mapping):
+                self.reduce = {k: _parse_reduce_arg(v) for k, v in reduce.items()}
+            else:
+                self.reduce = _parse_reduce_arg(reduce)
 
-        self.combine = _parse_combine_arg(combine)
+            self.combine = _parse_combine_arg(combine)
 
-        self.program = Program.parse(self.op_str, combine=self.combine, reduce=self.reduce)
+            self.program = Program.parse(self.op_str, combine=self.combine, reduce=self.reduce)
 
         self.symbol_values = symbol_values or {}
         for k, v in self.symbol_values.items():
             self.program.constr.add_constraint(Symbol(k), Constant(v))
 
     def __repr__(self) -> str:
-        return f'EinsOp({self.op_str}, reduce={self.reduce}, combine={self.combine})'
+        if self.is_transform:
+            return f'EinsOp({self.op_str}, transform={self.transform})'
+        else:
+            return f'EinsOp({self.op_str}, reduce={self.reduce}, combine={self.combine})'
+
+    def __str__(self) -> str:
+        names = {}
+
+        def get_name(tens_id, names=names):
+            if tens_id in names:
+                return names[tens_id]
+            else:
+                name_symbols = ascii_uppercase
+                if len(names) < len(name_symbols):
+                    suffix = ''
+                else:
+                    suffix = str(len(names) // len(name_symbols) - 1)
+
+                name_sym_base = name_symbols[len(names) % len(name_symbols)]
+                name_sym = f'{name_sym_base}{suffix}'
+                names[tens_id] = name_sym
+                return name_sym
+
+        out = [repr(self)]
+        if hasattr(self, 'instructions') and self.instructions:
+            # has graph
+            out.append('Execution Graph:\n')
+            for op, sources, sinks in self.instructions:
+                source_str = ', '.join(
+                    [get_name(i) + '{' + str(self.abstract.get(i, 'NA')) + '}' for i in sources]
+                )
+
+                sink_str = ', '.join(
+                    [get_name(i) + '{' + str(self.abstract.get(i, 'NA')) + '}' for i in sinks]
+                )
+                out.append(f'{op!s:>60}\t{source_str:>40} → {sink_str:<25}')
+
+        out.append('Constraints:')
+        out.append(str(self.program.constr))
+        return '\n'.join(out)
 
     def __call__(self, *tensors: Array) -> Array:
         """
         Apply the operation to the given tensors, returning the output tensor.
 
         Parameters
         ----------
@@ -268,69 +389,93 @@
 
         self.program.constr.solve()
         if self.program.constr.free_vars:
             # print(prog.constr)
             msg = f'Could not solve: free variables {self.program.constr.free_vars} remain'
             raise ValueError(msg)
 
-        backend = ArrayBackend(self.program.constr)
+        self.strat = BaseStrategy(self.program)
+
+        self.program.make_path(self.strat)
+
+        self.backend = ArrayBackend(self.program.constr)
+        self.instructions = []
 
-        abstract: MutableMapping[int, Tensor] = {}
-        concrete: MutableMapping[int, Array] = {}
+        self.abstract: MutableMapping[int, Tensor] = {}
+        self.concrete: MutableMapping[int, Array] = {}
 
-        def fill_from(src: Tensor, arr: Array):
+        def fill_from(src: Tensor, arr: Array, instructions=self.instructions):
             """Fills forward from the known tensor. Returns the answer, if found."""
-            concrete[id(src)] = arr
-            abstract[id(src)] = src
+            self.concrete[id(src)] = arr
+            self.abstract[id(src)] = src
+
+            # print(src, src.children)
 
             if len(src.children) == 0:
                 # we're done
-                return arr
+                return [arr]
+
+            leaves = []
 
             for op, children in src.children:
                 if len(children) == 1:
                     # could be a many-to-one op
                     child = children[0]
-                    concrete_parents = [concrete.get(id(parent)) for parent in child.parents]
+                    concrete_parents = [self.concrete.get(id(parent)) for parent in child.parents]
                     if all(p is not None for p in concrete_parents):
                         # we can fill in this operation
-                        result = backend.do(concrete_parents, op, child.parents, [child])[0]  # type: ignore
+                        result = self.backend.do(concrete_parents, op, child.parents, [child])[0]
+                        instructions.append((op, list(map(id, child.parents)), [id(child)]))
+                        # type: ignore
                         res = fill_from(child, result)
-                        if res is not None:
-                            return res
+                        leaves.extend(res)
+
                 else:
                     # no many-to-many ops: we can fill in all of these
-                    child_results = backend.do([arr], op, [src], children)
+                    child_results = self.backend.do([arr], op, [src], children)
+                    instructions.append((op, [id(src)], list(map(id, children))))
                     for child, result in zip(children, child_results):
                         res = fill_from(child, result)
-                        if res is not None:
-                            return res
+                        leaves.extend(res)
 
-            return None
+            return leaves
 
         try:
+            leaves = []
             for src, arr in zip(self.program.sources, tensors):
                 ans = fill_from(src, arr)
-                if ans is not None:
-                    return ans
+                leaves.extend(ans)
+
+            self.out_shape = [
+                self.program.constr.value_of(ax) for ax in self.program.orig_sink.axes
+            ]
+            potential_returns = [l for l in leaves if list(l.shape) == self.out_shape]
+            if potential_returns:
+                ans = potential_returns[-1]
+                self.abstract[id(ans)] = self.program.orig_sink
+                # the concrete arrays are large: we don't want to store them indefinitely
+                self.concrete.clear()
+                return ans
         except ValueError as err:
             msg = f"""
 Error occurred during computation.
-Program:\n{self.program}
+{self}
 """
             raise ValueError(msg) from err
 
-        msg = f'Could not solve tensor graph: {self.program}'
+        msg = f'Could not solve tensor graph: \n{self}'
         raise ValueError(msg)
 
 
 def einsop(
     *tensors_and_pattern: Union[Array, str],
     reduce: ReduceArg = 'sum',
     combine: CombineArg = 'multiply',
+    transform: Optional[Mapping[str, TransformArg]] = None,
+    **kwargs,
 ) -> Array:
     """
     A functional version of [EinsOp] that does not allow for inspection or caching.
 
     This exists mainly as a bridge between that interface and the familiar one used by einops. Use
     [EinsOp] instead, unless you really want a roughly compatible einops-like function.
 
@@ -358,9 +503,9 @@
 Two strings passed in: {pattern} and {t}. Perhaps you mean reduce= or combine=?"""
                 raise ValueError(msg)
             else:
                 pattern = t
         else:
             tensors.append(t)
 
-    op = EinsOp(pattern, reduce=reduce, combine=combine)
+    op = EinsOp(pattern, reduce=reduce, combine=combine, transform=transform, symbol_values=kwargs)
     return op(*tensors)
```

### Comparing `eins-0.0.1/src/eins/parsing.py` & `eins-0.1.0/src/eins/parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 from dataclasses import dataclass
-from typing import Callable, MutableSequence, Sequence, Union
+from typing import Callable, MutableSequence, Union
 
 import pyparsing as pp
 
 lparen = '('
 rparen = ')'
 parens = re.compile(r'\{[^{}]*\}')
 index = re.compile(r'([^[ ,]+)\[([^\]]*)\]')
```

### Comparing `eins-0.0.1/src/eins/reduction.py` & `eins-0.1.0/src/eins/reduction.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 
 @dataclass(frozen=True, unsafe_hash=True)
 class ArrayReduction(Reduction):
     """One of the methods in the Array API. Falls back to a method of the object."""
 
     func_name: str
 
+    def __repr__(self):
+        return repr(self.func_name)
+
     def __str__(self):
         return self.func_name
 
     @classmethod
     def parse(cls, name: str):
         if name in ARRAY_REDUCE_OPS:
             return cls(name)
@@ -193,14 +196,17 @@
             if isinstance(op, Reduction):
                 reductions += 1
                 if reductions > 1:
                     msg = f'{self} has more than one reduction operation'
                     raise ValueError(msg)
                 out = op(out, axis=axis)
             elif isinstance(op, Transformation):
+                if reductions == 1:
+                    msg = f'{self} is invalid. Cannot transform after reducing.'
+                    msg += '\nPerhaps you meant the reverse? Sequences are applied right-to-left.'
                 out = op(out, axis=axis)
             else:
                 out = op(out)
 
         if reductions == 0:
             msg = f'{self} must have one reduction operation'
             raise ValueError(msg)
@@ -230,7 +236,8 @@
 
 ReductionLiteral = Union[ArrayReductionLiteral, NormLiteral, RangeLiteral]
 
 ops = {
     str(op): parse_reduction(op)
     for op in chain.from_iterable(map(typing.get_args, typing.get_args(ReductionLiteral)))
 }
+ops = {k: v for k, v in ops.items() if v is not None}
```

### Comparing `eins-0.0.1/src/eins/symbolic.py` & `eins-0.1.0/src/eins/program.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,188 +1,30 @@
-"""Symbolic representation of tensor operations and manipulations."""
-
-import functools as ft
+# Ruff *really* does not like magic numbers!
 import pprint
-from abc import ABCMeta, abstractmethod
 from collections import defaultdict
 from copy import deepcopy
-from dataclasses import dataclass
 from itertools import chain
-from typing import Mapping, MutableSequence, Sequence, Union, cast
+from typing import Mapping, MutableSequence, Sequence, Tuple, Union, cast
 
-from eins.combination import ArrayCombination, Combination
+from eins.combination import ArrayCombination
+from eins.common_types import Combination, Reduction, Transformation
 from eins.constraint import Constraints, postprocess_ast
 from eins.parsing import Constant, Expr, Node, Symbol, make_expr, unpack_shorthands
 from eins.parsing import expr as expr_parser
-from eins.reduction import ArrayReduction, Reduction
-
-
-class Tensor:
-    """Node in a tensor network."""
-
-    def __init__(self, expr: Node):
-        self.parents = []
-        self.children = []
-        self.idx_axis = None
-        self.axes: MutableSequence[Node] = []
-        if isinstance(expr, (Constant, Symbol)):
-            self.axes.append(expr)
-            return
-
-        if expr.op == ' ':
-            self.axes = expr.children
-        elif expr.op == '@':
-            self.axes = Tensor(expr.children[0]).axes
-            self.idx_axis = expr.children[1]
-        else:
-            self.axes.append(expr)
-
-    def deepcopy(self) -> 'Tensor':
-        t = Tensor(Expr(' ', deepcopy(self.axes)))
-        t.idx_axis = self.idx_axis
-        return t
-
-    def axes_list(self) -> 'list[str]':
-        if any(not isinstance(ax, Symbol) for ax in self.axes):
-            msg = f'All axes must be symbols, but got {pprint.pformat(self.axes)}'
-            raise ValueError(msg)
-        return [ax.value for ax in self.axes if isinstance(ax, Symbol)]
-
-    def add_child_op(self, children: 'Sequence[Tensor]', op: 'ShapeOp'):
-        for child in children:
-            child.parents.append(self)
-        self.children.append((op, children))
-
-    def is_same_shape(self, other: 'Tensor') -> bool:
-        return self.axes == other.axes and self.idx_axis == other.idx_axis
-
-    def __repr__(self):
-        idx_expr = '' if self.idx_axis is None else f' @ {self.idx_axis}'
-        ax_expr = ' '.join(map(str, self.axes))
-        return ax_expr + idx_expr
-
-
-class ShapeOp(metaclass=ABCMeta):
-    @abstractmethod
-    def apply(self, tensors: Sequence[Tensor]) -> Sequence[Tensor]:
-        raise NotImplementedError
-
-    def __call__(self, tensors: Union[Tensor, Sequence[Tensor]]) -> Sequence[Tensor]:
-        if isinstance(tensors, Tensor):
-            tensors = [tensors]
-
-        if self.is_identity_for(tensors):
-            return tensors
-
-        children = self.apply(tensors)
-
-        for t in tensors:
-            t.add_child_op(children, self)
-        return children
-
-    def is_identity_for(self, _tensors: Sequence[Tensor]) -> bool:
-        return False
-
-
-@dataclass(unsafe_hash=True)
-class Reshape(ShapeOp):
-    new_shape: Sequence[Node]
-
-    def apply(self, tensors: Sequence[Tensor]) -> Sequence[Tensor]:  # noqa: ARG002
-        return [Tensor(Expr(' ', list(self.new_shape)))]
-
-
-@dataclass(unsafe_hash=True)
-class Transpose(ShapeOp):
-    perm: Sequence[int]
-
-    def apply(self, tensors: Sequence[Tensor]) -> Sequence[Tensor]:
-        return [Tensor(Expr(' ', [tensors[0].axes[i] for i in self.perm]))]
-
-    def is_identity_for(self, _tensors: Sequence[Tensor]) -> bool:
-        return tuple(self.perm) == tuple(range(len(self.perm)))
-
-
-@dataclass(unsafe_hash=True)
-class Split(ShapeOp):
-    axis_num: int
-
-    def apply(self, tensors: Sequence[Tensor]) -> Sequence[Tensor]:
-        children = []
-        split_ax = tensors[0].axes[self.axis_num]
-        if not isinstance(split_ax, Expr) or split_ax.op != '+':
-            msg = f'Tried to split on {split_ax} in {tensors}, which is not a sum.'
-            raise ValueError(msg)
-
-        for addend in split_ax.children:
-            child = tensors[0].deepcopy()
-            child.axes[self.axis_num] = addend
-            children.append(child)
-        return children
-
-
-@dataclass(unsafe_hash=True)
-class Concat(ShapeOp):
-    axis_num: int
-
-    def apply(self, tensors: Sequence[Tensor]) -> Sequence[Tensor]:
-        add_axes = [tensor.axes[self.axis_num] for tensor in tensors]
-        concatenated = tensors[0].deepcopy()
-        concatenated.axes[self.axis_num] = Expr('+', add_axes)
-        return [concatenated]
-
-
-@dataclass(unsafe_hash=True)
-class OneHot(ShapeOp):
-    idx_axis: Node
-
-    def apply(self, tensors: Sequence[Tensor]) -> Sequence[Tensor]:
-        child = tensors[0].deepcopy()
-        if child.idx_axis is None:
-            msg = f'Cannot one-hot on {child} because it does not have an index axis'
-            raise ValueError(msg)
-        child.axes.append(child.idx_axis)
-        child.idx_axis = None
-        return [child]
-
-
-@dataclass(unsafe_hash=True)
-class ExpandTo(ShapeOp):
-    """Adds new axes with 1 to broadcast with the current shape. Output should be
-    a supersequence of the current shape."""
-
-    new_shape: Sequence[Node]
-
-    def apply(self, tensors: Sequence[Tensor]) -> Sequence[Tensor]:  # noqa: ARG002
-        return [Tensor(Expr(' ', list(self.new_shape)))]
-
-
-@dataclass(unsafe_hash=True)
-class Combine(ShapeOp):
-    method: Combination
-
-    def apply(self, tensors: Sequence[Tensor]) -> Sequence[Tensor]:
-        return [tensors[0].deepcopy()]
-
-    def is_identity_for(self, tensors: Sequence[Tensor]) -> bool:
-        return len(tensors) == 1
-
+from eins.reduction import ArrayReduction
+from eins.symbolic import (
+    Concat,
+    OneHot,
+    Reshape,
+    ShapeOp,
+    Split,
+    Tensor,
+    Transform,
+)
 
-@dataclass(unsafe_hash=True)
-class Reduce(ShapeOp):
-    method: Reduction
-    axis: Node
-
-    def apply(self, tensors: Sequence[Tensor]) -> Sequence[Tensor]:
-        out = tensors[0].deepcopy()
-        out.axes = [ax for ax in out.axes if ax != self.axis]
-        return [out]
-
-
-# Ruff *really* does not like magic numbers!
 EXP_ARITY = 2
 
 
 def expanded_shape(node: Node) -> Sequence[Node]:
     if isinstance(node, (Constant, Symbol)):
         return [node]
     elif node.op == '*':
@@ -258,51 +100,32 @@
         return Reshape(root.axes)([reverse_graph(children[0])])[0]
     elif isinstance(op, Split):
         return Concat(op.axis_num)([reverse_graph(child) for child in children])[0]
     else:
         raise ValueError
 
 
-def optimal_supersequence(axes: Sequence[Sequence[str]]):
-    """
-    Computes an ordering for the superset of the given axes that minimizes the number of
-    transpositions.
-
-    At least from preliminary testing, the exact permutation in a transposition has a small impact
-    on its cost relative to whether one is performed at all. As such, the goal is to minimize the
-    *number* of arrays that need to be transposed and the number of elements per transposed array,
-    not the transpositions themselves.
-
-    Examples:
-
-    optimal_supersequence([['a', 'b', 'd'], ['a', 'c', 'd']]) == ['a', 'b', 'c', 'd']
-    optimal_supersequence(['abcd', 'cba', 'dcb') == ['d', 'c', 'b', 'a']
-    """
-    pass
-
-
 DEFAULT_COMBINE = ArrayCombination('multiply')
 DEFAULT_REDUCE = ArrayReduction('sum')
 # *rolls eyes*
 MAX_ARROW_OPERANDS = 2
 
 
 class Program:
     def __init__(
         self,
         expr: Expr,
         constr: Constraints,
         combine: Combination = DEFAULT_COMBINE,
         reduce: Union[Reduction, Mapping[str, Reduction]] = DEFAULT_REDUCE,
-        reduce_early: bool = True,  # noqa: FBT001, FBT002
     ):
-        self.reduce_early = reduce_early
         self.graph = {}
+        self.expr = expr
         if expr.op != '->':
-            msg = f'Expected -> as operator, but got {expr.op}'
+            msg = 'Eins expressions must have -> unless they are a transformation.'
             raise ValueError(msg)
 
         if len(expr.op) != MAX_ARROW_OPERANDS:
             msg = f'For now, Eins only supports one -> per expression, but got {len(expr.op)}'
             raise ValueError(msg)
 
         lhs, rhs = expr.children
@@ -315,71 +138,128 @@
 
         if lhs.op == ',':
             self.sources = [Tensor(c) for c in lhs.children]
         else:
             self.sources = [Tensor(lhs)]
 
         self.current = []
-        for source in self.sources:
-            self.current.extend(normalize_until_done(source))
+        self.source_curr_map = {}
+        for i, source in enumerate(self.sources):
+            currents = normalize_until_done(source)
+            self.current.extend(currents)
+            self.source_curr_map[i] = currents
 
         self.orig_sink = Tensor(rhs)
         self.sinks = list(normalize_until_done(self.orig_sink))
         self.constr = constr
 
         for t in self.current + self.sinks:
             self.constr.add_variables(t.axes_list())
 
         self.combine = combine
 
         if isinstance(reduce, Reduction):
             self.reduce = defaultdict(lambda: reduce)
         else:
             self.reduce = dict(reduce)
+            # we may have already renamed axes, but the user is passing in the old names
+            # e.g., a b b, c b b -> a, reduce={'b': 'mean', 'c': 'sum'}
+            # b now is b-1 and b-2
+            for lhs, rhs in self.constr.equations:
+                if isinstance(rhs, Symbol) and isinstance(lhs, Symbol):
+                    if rhs.value in self.reduce:
+                        self.reduce[lhs.value] = self.reduce[rhs.value]
+                    elif lhs.value in self.reduce:
+                        self.reduce[rhs.value] = self.reduce[lhs.value]
+
         if not isinstance(reduce, Reduction):
             for k, v in reduce.items():
                 self.reduce[k] = v
 
+    def make_path(self, strat):
         self.outputs = []
-        if len(self.sinks) > 1:
-            # multiple tensors in output this is the one time the rules are relaxed about using all
-            # inputs tensors that only have an axis in a different split aren't used e.g., a b, a c
-            # -> a b+c just does a b -> a b, a c -> a c
-            axes_sets = [set(sink.axes_list()) for sink in self.sinks]
-
-            all_splits = set()
-            diffs = []
-            for i, ax_set in enumerate(axes_sets):
-                others = set()
-                for j, ax_set2 in enumerate(axes_sets):
-                    if i == j:
-                        continue
-                    others |= ax_set2
-                diff = ax_set - others
-                diffs.append(diff)
-                all_splits |= diff
-
-            per_sink_inputs = []
-            for diff in diffs:
-                per_sink_input = []
-                for curr in self.current:
-                    # TODO needs to be more robust for multiple splits? it can't be on the "wrong
-                    # side" of a single split a c, a d, b c, b d -> a+b c+d
-                    curr_ax = set(curr.axes_list())
-                    if curr_ax.isdisjoint(all_splits - diff):
-                        per_sink_input.append(curr)
-                per_sink_inputs.append(per_sink_input)
-
-            # print(per_sink_inputs) print(self.sinks)
-            for sink_input, sink in zip(per_sink_inputs, self.sinks):
-                self.outputs.append(self.connect(sink_input, sink))
+        # Normally, every input is used for every output. The exception is when there are splits in
+        # the input. For example, a b+c -> a b doesn't use a c. The rule is that a tensor with a
+        # split input is unused for an output only if it was split from a sum, of which at least one
+        # axis is in the output, but the specific split we're dealing with isn't.
+
+        # a c, b c -> a+b c: all used
+        # a+b c -> a c: only a c used, not b c, because a in {a, c} but b not in {a c}
+        # a+b c, a+b d -> a c+d: a c used for a c, a d used for a d
+
+        # TODO very challenging case: a+b c, a+b d, e a -> e c+d
+
+        # only necessary if we split at some point, so either multiple outputs or multiple inputs
+        # from a single source
+        if len(self.sinks) > 1 or len(self.current) != len(self.sources):
+            sink_axes = [set(sink.axes_list()) for sink in self.sinks]
+            common_sink_axes = set.intersection(*sink_axes)
+            split_sink_axes = [ax - common_sink_axes for ax in sink_axes]
+            missing_sink_axes = [common_sink_axes - ax for ax in sink_axes]
+
+            for sink_i, (axs, split, missing) in enumerate(
+                zip(sink_axes, split_sink_axes, missing_sink_axes)
+            ):
+                sink_inputs = []
+                for source_i, currs in self.source_curr_map.items():
+                    curr_axes = [set(curr.axes_list()) for curr in currs]
+                    common_curr_axes = set.union(*curr_axes) - set.intersection(*curr_axes)
+                    split_curr_axes = [ax & common_curr_axes for ax in curr_axes]
+                    missing_curr_axes = [common_curr_axes - ax for ax in curr_axes]
+                    for curr, curr_axs, curr_split, curr_missing in zip(
+                        currs, curr_axes, split_curr_axes, missing_curr_axes
+                    ):
+                        # print(currs, curr_axes, curr_split, curr_missing, axs)
+                        add_to_input = False
+                        if curr_split <= axs and curr_missing.isdisjoint(axs):
+                            # split axes line up with output
+                            add_to_input = True
+                        elif curr_missing <= axs and curr_split.isdisjoint(axs):
+                            # other axes line up with output, skip
+                            add_to_input = False
+                        else:
+                            # e.g., a+b, c a, d b, d e -> c e
+
+                            # Neither a nor b appear in output. Probably not solvable in general,
+                            # but we can at least try a basic heuristic: if the split axis appears
+                            # in another input, include it
+                            other_axes = []
+                            for source_j, other_currs in self.source_curr_map.items():
+                                if source_i != source_j:
+                                    other_axes.extend(
+                                        [set(curr.axes_list()) for curr in other_currs]
+                                    )
+                            other_axes = set.union(*other_axes)
+                            # print(other_axes)
+                            if curr_missing.isdisjoint(other_axes) and curr_split <= other_axes:
+                                add_to_input = True
+                            elif curr_missing <= other_axes and curr_split.isdisjoint(other_axes):
+                                add_to_input = False
+                            else:
+                                msg = (
+                                    f'Unclear split: {axs}, {split}, {missing} '
+                                    f'{curr_axs}, {curr_split}, {curr_missing}'
+                                )
+                                raise ValueError(msg)
+
+                        if add_to_input:
+                            sink_inputs.append(curr)
+
+                # print(sink_inputs, self.sinks[sink_i])
+                self.outputs.append(strat.connect(sink_inputs, self.sinks[sink_i]))
 
         else:
-            self.outputs.append(self.connect(self.current, self.sinks[0]))
+            self.outputs.append(strat.connect(self.current, self.sinks[0]))
 
+        self.link_outs_to_sink()
+
+    def link_outs_to_sink(self):
+        """
+        Connects the outputs (from the sources) to the sink.
+        """
         reverse_graph(self.orig_sink)
 
         for out, sink in zip(self.outputs, self.sinks):
             if not out.is_same_shape(sink):
                 msg = f'Output {out} is not the same shape as sink {sink}'
                 raise ValueError(msg)
 
@@ -398,99 +278,23 @@
         if key in self.graph:
             return self.graph[key]
         else:
             res = op(tensors)
             self.graph[key] = res
             return res
 
-    def combine_mismatched(self, combine: Combine, tensors: Sequence[Tensor]) -> Tensor:
-        """Combines tensors together, broadcasting and transposing as needed. Assumes tensors are in
-        normal form."""
-        # We want to find an order of axes that can avoid transpositions. For example, the best way
-        # to broadcast a b c and a d c is a b d c, not a b c d or a d c b.
-        out = tensors[0]
-        for t in tensors[1:]:
-            new_axes = out.axes_list() + [ax for ax in t.axes_list() if ax not in out.axes_list()]
-            axs = t.axes_list()
-            perm = tuple(sorted(range(len(axs)), key=lambda x: new_axes.index(axs[x])))
-            transposed_t = Transpose(perm)(t)[0]
-            new_ax_op = ExpandTo(tuple(map(Symbol, new_axes)))
-            expanded_t = self.apply_op(new_ax_op, transposed_t)[0]
-            expanded_out = self.apply_op(new_ax_op, out)[0]
-            out = self.apply_op(combine, (expanded_out, expanded_t))[0]
-        return out
-
     @classmethod
     def parse(cls, op: str, **kwargs):
         expr = make_expr(expr_parser.parse_string(unpack_shorthands(op)).as_list())
         if not isinstance(expr, Expr):
             msg = f'Expected expression, but got {expr}'
             raise ValueError(msg)
         constraints = postprocess_ast(expr)
         return cls(expr, constraints, **kwargs)
 
-    def connect(self, start: Sequence[Tensor], goal: Tensor):
-        goal_axes = goal.axes_list()
-        start_axes = start[0].axes_list()
-        for other in start[1:]:
-            for ax in other.axes_list():
-                if ax not in start_axes:
-                    start_axes.append(ax)
-
-        reduce_axes = set(start_axes) - set(goal_axes)
-
-        transposed = []
-        for s in start:
-            axs = s.axes_list()
-            perm = tuple(sorted(range(len(axs)), key=lambda x: start_axes.index(axs[x])))
-            transposed.extend(self.apply_op(Transpose(perm), s))
-
-        if self.reduce_early:
-            exp_axes = [set(exp.axes_list()) for exp in transposed]
-            combined = transposed[0]
-            for i, exp in enumerate(transposed):
-                if i == 0:
-                    continue
-                else:
-                    combined = self.combine_mismatched(Combine(self.combine), (combined, exp))
-
-                in_rest = set()
-                for remaining_axes in exp_axes[i + 1 :]:
-                    in_rest |= remaining_axes
-
-                # axes in the input, to reduce, that aren't in future tensors
-                to_reduce = (reduce_axes - in_rest) & set(combined.axes_list())
-                for r_ax in to_reduce:
-                    combined = self.apply_op(Reduce(self.reduce[r_ax], Symbol(r_ax)), combined)[0]
-            reduced = combined
-        else:
-            expanded = []
-            for t in transposed:
-                expanded.extend(self.apply_op(ExpandTo(tuple(map(Symbol, start_axes))), t))
-            combined = self.apply_op(Combine(self.combine), tuple(expanded))[0]
-
-            reduced = combined
-            for ax in reduce_axes:
-                reduced = self.apply_op(Reduce(self.reduce[ax], Symbol(ax)), reduced)[0]
-
-        r_axs = reduced.axes_list()
-        if set(r_axs) != set(goal_axes):
-            msg = f'{r_axs} != {goal_axes}'
-            raise ValueError(msg)
-
-        perm = tuple(sorted(range(len(r_axs)), key=lambda x: goal_axes.index(r_axs[x])))
-
-        out = self.apply_op(Transpose(perm), reduced)[0]
-
-        if out.axes_list() != goal_axes:
-            msg = f'{out.axes_list()} != {goal_axes}'
-            raise ValueError(msg)
-
-        return out
-
     def __repr__(self):
         strings = []
         for i, inp in enumerate(self.sources):
             strings.append(f'Input {i+1}:\n{pprint.pformat(inp)}')
         strings.append('-' * 50)
         for i, inp in enumerate(self.current):
             strings.append(f'Current {i+1}:\n{pprint.pformat(inp)}')
@@ -501,12 +305,79 @@
         strings.append(f'Final Output:\n{pprint.pformat(self.orig_sink)}')
         strings.append('-' * 50)
         strings.append('Equations:')
         strings.append(str(self.constr))
         return '\n'.join(strings)
 
 
-# env = Program.parse('b ((n p) (n p)) c d=c, b p*p*d*c h, h[g+i k] -> b (n^2 g+i) k') env =
-# Program.parse('a b, b c -> a+c b') print(env)
+class TransformProgram(Program):
+    """
+    Program that applies transformations to the input tensor without modifying the shape.
+    """
+
+    def __init__(self, expr: Node, constr: Constraints, transform: Mapping[str, Transformation]):
+        if not isinstance(expr, Expr):
+            expr = Expr(' ', cast(MutableSequence[Node], [expr]))
+
+        if expr.op in (',', '->'):
+            msg = 'Eins transformations only take in a single input tensor.'
+            raise ValueError(msg)
+
+        self.constr = constr
+        self.graph = {}
+        self.expr = expr
 
+        self.sources = [Tensor(expr)]
+        self.current = list(normalize_until_done(self.sources[0]))
+
+        for t in self.current:
+            self.constr.add_variables(t.axes_list())
+
+        self.transform = transform
+
+        self.orig_sink = Tensor(expr)
+        self.sinks = list(normalize_until_done(self.orig_sink))
+
+        for lhs, rhs in self.constr.equations:
+            if isinstance(rhs, Symbol) and isinstance(lhs, Symbol):
+                if lhs.value in self.transform or rhs.value in self.transform:
+                    val = lhs.value if lhs.value in self.transform else rhs.value
+                    msg = (
+                        f"It's not clear which {val} axis you want to apply the transformation to."
+                        " Specify by giving the duplicates different names, e.g., 'a b=a' instead"
+                        " of 'a a'."
+                    )
+                    raise ValueError(msg)
+
+    def make_path(self, strat=None):  # noqa: ARG002
+        self.transform_map = {}
+        used_axes = set()
+
+        for i, curr in enumerate(self.current):
+            for ax in curr.axes_list():
+                if ax in self.transform:
+                    if ax in used_axes:
+                        msg = (
+                            f'Axis {ax} appears on both sides of a split axis. '
+                            'It is ambiguous whether transformation should happen'
+                            ' before or after the split.'
+                        )
+                        raise ValueError(msg)
+
+                    if curr in self.transform_map:
+                        msg = (
+                            f'Multiple transforms could be applied to tensor {curr}.'
+                            ' Split the operation into multiple to ensure consistent order.'
+                        )
+
+                    self.transform_map[i] = Transform(self.transform[ax], Symbol(ax))
+                    used_axes.add(ax)
+
+        self.outputs = []
+        for i, curr in enumerate(self.current):
+            if i in self.transform_map:
+                out = self.apply_op(self.transform_map[i], curr)[0]
+            else:
+                out = curr
+            self.outputs.append(out)
 
-# ops to reverse graph from sink to targets just get it fing done
+        self.link_outs_to_sink()
```

### Comparing `eins-0.0.1/tests/test_basic.py` & `eins-0.1.0/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `eins-0.0.1/LICENSE.txt` & `eins-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eins-0.0.1/pyproject.toml` & `eins-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   'artificial intelligence',
   'deep learning',
   'einops',
   'machine learning',
   'neural networks',
   'scientific computing',
   'tensor manipulation',
-
+  'array manipulation',
 ]
 authors = [
   { name = "Nicholas Miklaucic", email = "nicholas.miklaucic@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: MIT License",
@@ -53,14 +53,16 @@
 dependencies = [
   "coverage[toml]>=6.5",
   "pytest",
   "numpy",
   "jax",
   "jaxlib",
   "torch",
+  "flax",
+  "jaxtyping",
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = ["- coverage combine", "coverage report"]
 cov = ["test-cov", "cov-report"]
 
@@ -124,14 +126,18 @@
   "C901",
   "PLR0911",
   "PLR0912",
   "PLR0913",
   "PLR0915",
   # 2 is not a magic number, this is ridiculous
   "PLR2004",
+  # Jaxtyping uses annotations ruff doesn't understand
+  "F722",
+  # named lambdas are fine
+  "E731",
 ]
 unfixable = [
   # Don't touch unused imports
   "F401",
 ]
 fix = true
```

### Comparing `eins-0.0.1/PKG-INFO` & `eins-0.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.3
 Name: eins
-Version: 0.0.1
+Version: 0.1.0
 Summary: One tensor operation is all you need
 Project-URL: Documentation, https://github.com/nicholas-miklaucic/eins#readme
 Project-URL: Issues, https://github.com/nicholas-miklaucic/eins/issues
 Project-URL: Source, https://github.com/nicholas-miklaucic/eins
 Author-email: Nicholas Miklaucic <nicholas.miklaucic@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
-Keywords: artificial intelligence,deep learning,einops,machine learning,neural networks,scientific computing,tensor manipulation
+Keywords: array manipulation,artificial intelligence,deep learning,einops,machine learning,neural networks,scientific computing,tensor manipulation
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -26,98 +26,111 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: array-api-compat
 Requires-Dist: pyparsing
 Description-Content-Type: text/markdown
 
 # eins
+
 ## One tensor operation is all you need
 
 [![PyPI - Version](https://img.shields.io/pypi/v/eins.svg)](https://pypi.org/project/eins)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/eins.svg)](https://pypi.org/project/eins)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](code_of_conduct.md)
+[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)
 
-What if most of your machine learning model code could be replaced by a single operation? `eins` gives you a powerful language to describe tensor manipulation, making it a one-stop shop for all of your AI needs.
+What if most of your machine learning model code could be replaced by a single operation? Eins gives
+you a powerful language to describe array manipulation, making it a one-stop shop for all of your AI
+needs.
+
+For a sample of what Eins does, let's do [the patch embedding from a vision
+transformer](https://nn.labml.ai/transformers/vit/index.html#PatchEmbeddings). That means breaking
+up an image into patches and then linearly embedding each patch.
 
-As an example, here's [the patch embedding from a vision transformer](https://nn.labml.ai/transformers/vit/index.html#PatchEmbeddings):
 ```python
-linear = EinsOp('b (n_p patch) (n_p patch) c, (patch patch c) emb -> b (n_p n_p) emb')
+from eins import EinsOp
+patchify = EinsOp('''b (n_p patch) (n_p patch) c, (patch patch c) emb -> b (n_p n_p) emb''')
 
 kernel = randn(5 * 5 * 3, 12)
 images = randn(4, 55, 55, 3)
 patches = linear(images, kernel)
 print(patches.shape)  # (4, 121, 12)
 ```
 
-This takes in a batch of square images: `b` images in a batch, `c` channels, and height and width both divisible into `n_p` patches of size `patch`. It combines those images with an embedding layer that takes each of the `patch * patch * c` values in a patch and produces a vector of length `emb`.
+You input the shapes and Eins will figure out what to do.
+
+If you've used [`einops`](https://github.com/arogozhnikov/einops), then think of Eins as `einops`
+with a more ambitious goal—being the only operation you should need for your next deep learning
+project.
+
+Interested? Check out the [tutorial](https://nicholas-miklaucic.github.io/eins/tutorial/), which
+walks you through the highlights of Eins with examples of how Eins can make the array operations you
+know and love more readable, portable, and robust.
 
-If you've used the wonderful [`einops`](https://github.com/arogozhnikov/einops), then think of `eins` as `einops` with a more ambitious goal—being the only operation you should need for your next deep learning project.
+To learn more, consult the [documentation](https://nicholas-miklaucic.github.io/eins/) or
+the [examples](examples/README.md).
 
 ## Installation
 
 ```console
 pip install eins
 ```
 
-Then, just use `eins` with any library that implements the [Array API](https://data-apis.org/array-api/latest/index.html#), including NumPy, Torch, JAX, CuPy, and Dask.
-
-One of the design goals of `eins` is to be painless to use in almost any Python project. If `pip install eins` is not the only thing you need to do to use Eins in your project, feel free to [file an issue](https://github.com/nicholas-miklaucic/eins/issues/new).
+Eins works with anything that implements the [Array
+API](https://data-apis.org/array-api/latest/index.html), and Eins explicitly promises to support
+NumPy, PyTorch, and JAX—including full differentiability. You will need one of those libraries to
+actually use Eins operations.
+
+## Features
+
+- 🧩 A solver that can handle duplicate axes, named constants, and constraints
+- 🚀 Compilation and optimization for high performance without sacrificing readability
+- Split, concatenate, stack, flatten, transpose, normalize, reduce, broadcast, and more
+- Works across frameworks
+- A composable set of unified array operations for portable softmax, power normalization, and more
 
 ## Roadmap
 
-`eins` is still in heavy development. Here's a sense of where we're headed.
+Eins is still in heavy development. Here's a sense of where we're headed.
 
-### Short-Term (days)
+### Near-Term (weeks)
 
-- [x] Better error reporting
+- [ ] Updating indexing syntax to match `eindex`
+- [ ] Unit array to indicate zero-dimensional tensors
 - [ ] `...` for batching over dynamic numbers of batch axes
 - [ ] Specifying intermediate results to control the order of reduction
-- [ ] Support `-` and `/` as natural pairs to `+` and `*`
-- [ ] Implementing `repeat`
-- [x] Adding support for reductions that aren't in Array API (e.g., p-norm)
-- [x] Adding support for "transformations" that are elementwise but use an axis (standardize)
-- [x] Flip order of inputs (logsumexp is log + sum + exp)
-- [ ] Unit array to indicate zero-dimensional tensors
-- [ ] Updating indexing syntax to match `eindex`
-- [/] Much more thorough documentation and tests for existing functionality
-- [ ] Better visualization of the program graph
-- [ ] `@local` syntax
-
-### Near-Term (weeks)
-- [ ] Easy performance gains
-- [ ] Much better error reporting
-- [ ] Completing full support for tensor indexing
-- [ ] Warnings or errors for ambiguous expressions
+- [ ] Support `-` and `/`
+- [ ] Better error reporting
 - [ ] Ways of visualizing and inspecting the computation graph
+- [ ] Typo checking in errors about axes
+- [ ] Multiple outputs, either through arrows or commas
 
 ### Long-Term (months)
-- [ ] Layers for popular ML frameworks?
-- [ ] Automatically optimizing the execution of a specific EinsOp for a specific computer and input size
-- [ ] Static typing support that shows the array shapes
+
+- [ ] Layers for popular ML frameworks
+- [ ] Automatically optimizing the execution of a specific EinsOp for a specific
+      computer and input size
+- [ ] Completing full support for tensor indexing
+- [ ] Static typing support
 - [ ] Tabulating the model FLOPs/memory usage as a function of named axes
-- [ ] Functionality akin to `pack` and `unpack`?
+- [ ] Functionality akin to `pack` and `unpack`
 
 ## Acknowledgements
 
-The excellent [`einops`](https://github.com/arogozhnikov/einops) library inspired this project and its syntax. After working on my own extension to handle indexing, I realized that [`eindex`](https://github.com/arogozhnikov/eindex) already had a more coherent vision for what indexing can look like, and so much of that syntax in this library borrows from that one.
+The excellent [`einops`](https://github.com/arogozhnikov/einops) library
+inspired this project and its syntax. After working on my own extension to
+handle indexing, I realized that
+[`eindex`](https://github.com/arogozhnikov/eindex) already had a more coherent
+vision for what indexing can look like, and so much of that syntax in this
+library borrows from that one.
 
 ## Contributing
 
-Any contributions to `eins` are welcomed and appreciated! If you're interested in making serious changes or extensions to the syntax of operations, consider reaching out first to make sure we're on the same page. For any code changes, do make sure you're using the project Ruff settings.
+Any contributions to Eins are welcomed and appreciated! If you're interested
+in making serious changes or extensions to the syntax of operations, consider
+reaching out first to make sure we're on the same page. For any code changes, do
+make sure you're using the project Ruff settings.
 
 ## License
 
-`eins` is distributed under the terms of the [MIT](https://spdx.org/licenses/MIT.html) license.
-
-
-To do:
-
-- Passing in constants: this needs to be desugared to named values, I think?
-- When we duplicate n to n-2, also copy n's reduction
-- Test with JIT and PyTorch
-- Get a basic perf comparison
-- Docs website, maybe rewrite a few big models
-- Example with non-Latin characters
-- `pyproject.toml` fun stuff
-- Get ops from `nn` libraries or logit or something
-- Intermediate chaining syntax
-- Constants file with op characters and similar
+Eins is distributed under the terms of the
+[MIT](https://spdx.org/licenses/MIT.html) license.
```

