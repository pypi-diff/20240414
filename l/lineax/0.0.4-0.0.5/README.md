# Comparing `tmp/lineax-0.0.4.tar.gz` & `tmp/lineax-0.0.5.tar.gz`

## Comparing `lineax-0.0.4.tar` & `lineax-0.0.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 lineax-0.0.4/lineax/__init__.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 lineax-0.0.4/lineax/_custom_types.py
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 lineax-0.0.4/lineax/_misc.py
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 lineax-0.0.4/lineax/_norm.py
--rw-r--r--   0        0        0    63854 2020-02-02 00:00:00.000000 lineax-0.0.4/lineax/_operator.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 lineax-0.0.4/lineax/_solution.py
--rw-r--r--   0        0        0    28941 2020-02-02 00:00:00.000000 lineax-0.0.4/lineax/_solve.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 lineax-0.0.4/lineax/_tags.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 lineax-0.0.4/lineax/_solver/__init__.py
--rw-r--r--   0        0        0     8365 2020-02-02 00:00:00.000000 lineax-0.0.4/lineax/_solver/bicgstab.py
--rw-r--r--   0        0        0    13078 2020-02-02 00:00:00.000000 lineax-0.0.4/lineax/_solver/cg.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 lineax-0.0.4/lineax/_solver/cholesky.py
--rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 lineax-0.0.4/lineax/_solver/diagonal.py
--rw-r--r--   0        0        0    18530 2020-02-02 00:00:00.000000 lineax-0.0.4/lineax/_solver/gmres.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 lineax-0.0.4/lineax/_solver/lu.py
--rw-r--r--   0        0        0     4175 2020-02-02 00:00:00.000000 lineax-0.0.4/lineax/_solver/misc.py
--rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 lineax-0.0.4/lineax/_solver/qr.py
--rw-r--r--   0        0        0     3771 2020-02-02 00:00:00.000000 lineax-0.0.4/lineax/_solver/svd.py
--rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 lineax-0.0.4/lineax/_solver/triangular.py
--rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 lineax-0.0.4/lineax/_solver/tridiagonal.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 lineax-0.0.4/lineax/internal/__init__.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 lineax-0.0.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 lineax-0.0.4/LICENSE
--rw-r--r--   0        0        0     3562 2020-02-02 00:00:00.000000 lineax-0.0.4/README.md
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 lineax-0.0.4/pyproject.toml
--rw-r--r--   0        0        0    17694 2020-02-02 00:00:00.000000 lineax-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 lineax-0.0.5/lineax/__init__.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 lineax-0.0.5/lineax/_custom_types.py
+-rw-r--r--   0        0        0     2640 2020-02-02 00:00:00.000000 lineax-0.0.5/lineax/_misc.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 lineax-0.0.5/lineax/_norm.py
+-rw-r--r--   0        0        0    67432 2020-02-02 00:00:00.000000 lineax-0.0.5/lineax/_operator.py
+-rw-r--r--   0        0        0     2772 2020-02-02 00:00:00.000000 lineax-0.0.5/lineax/_solution.py
+-rw-r--r--   0        0        0    29124 2020-02-02 00:00:00.000000 lineax-0.0.5/lineax/_solve.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 lineax-0.0.5/lineax/_tags.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 lineax-0.0.5/lineax/_solver/__init__.py
+-rw-r--r--   0        0        0     8529 2020-02-02 00:00:00.000000 lineax-0.0.5/lineax/_solver/bicgstab.py
+-rw-r--r--   0        0        0    13233 2020-02-02 00:00:00.000000 lineax-0.0.5/lineax/_solver/cg.py
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 lineax-0.0.5/lineax/_solver/cholesky.py
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 lineax-0.0.5/lineax/_solver/diagonal.py
+-rw-r--r--   0        0        0    18843 2020-02-02 00:00:00.000000 lineax-0.0.5/lineax/_solver/gmres.py
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 lineax-0.0.5/lineax/_solver/lu.py
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 lineax-0.0.5/lineax/_solver/misc.py
+-rw-r--r--   0        0        0     4148 2020-02-02 00:00:00.000000 lineax-0.0.5/lineax/_solver/qr.py
+-rw-r--r--   0        0        0     3800 2020-02-02 00:00:00.000000 lineax-0.0.5/lineax/_solver/svd.py
+-rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 lineax-0.0.5/lineax/_solver/triangular.py
+-rw-r--r--   0        0        0     4452 2020-02-02 00:00:00.000000 lineax-0.0.5/lineax/_solver/tridiagonal.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 lineax-0.0.5/lineax/internal/__init__.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 lineax-0.0.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 lineax-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 lineax-0.0.5/README.md
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 lineax-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0    17753 2020-02-02 00:00:00.000000 lineax-0.0.5/PKG-INFO
```

### Comparing `lineax-0.0.4/lineax/__init__.py` & `lineax-0.0.5/lineax/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import importlib.metadata
+
 from . import internal as internal
 from ._operator import (
     AbstractLinearOperator as AbstractLinearOperator,
     AddLinearOperator as AddLinearOperator,
     AuxLinearOperator as AuxLinearOperator,
     ComposedLinearOperator as ComposedLinearOperator,
     conj as conj,
@@ -33,14 +35,15 @@
     is_tridiagonal as is_tridiagonal,
     is_upper_triangular as is_upper_triangular,
     JacobianLinearOperator as JacobianLinearOperator,
     linearise as linearise,
     materialise as materialise,
     MatrixLinearOperator as MatrixLinearOperator,
     MulLinearOperator as MulLinearOperator,
+    NegLinearOperator as NegLinearOperator,
     PyTreeLinearOperator as PyTreeLinearOperator,
     TaggedLinearOperator as TaggedLinearOperator,
     TangentLinearOperator as TangentLinearOperator,
     tridiagonal as tridiagonal,
     TridiagonalLinearOperator as TridiagonalLinearOperator,
 )
 from ._solution import RESULTS as RESULTS, Solution as Solution
@@ -72,8 +75,8 @@
     transpose_tags_rules as transpose_tags_rules,
     tridiagonal_tag as tridiagonal_tag,
     unit_diagonal_tag as unit_diagonal_tag,
     upper_triangular_tag as upper_triangular_tag,
 )
 
 
-__version__ = "0.0.1"
+__version__ = importlib.metadata.version("lineax")
```

### Comparing `lineax-0.0.4/lineax/_custom_types.py` & `lineax-0.0.5/lineax/_custom_types.py`

 * *Files identical despite different names*

### Comparing `lineax-0.0.4/lineax/_norm.py` & `lineax-0.0.5/lineax/_norm.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,20 +17,15 @@
 
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 from equinox.internal import ω
 from jaxtyping import Array, ArrayLike, Inexact, PyTree, Scalar
 
-
-def default_floating_dtype():
-    if jax.config.jax_enable_x64:  # pyright: ignore
-        return jnp.float64
-    else:
-        return jnp.float32
+from ._misc import complex_to_real_dtype, default_floating_dtype
 
 
 def tree_dot(tree1: PyTree[ArrayLike], tree2: PyTree[ArrayLike]) -> Inexact[Array, ""]:
     """Compute the dot product of two pytrees of arrays with the same pytree
     structure."""
     leaves1, treedef1 = jtu.tree_flatten(tree1)
     leaves2, treedef2 = jtu.tree_flatten(tree2)
@@ -89,15 +84,17 @@
     # Get zero gradient, rather than NaN gradient, in these cases.
     pred = (out == 0) | jnp.isinf(out)
     denominator = jnp.where(pred, 1, out)
     # We could also switch the dot and the division.
     # This approach is a bit more expensive (more divisions), but should be more
     # numerically stable (`x` and `denominator` should be of the same scale; `tx` is of
     # unknown scale).
-    t_out = tree_dot((x**ω / denominator).ω, tx).real
+    with jax.numpy_dtype_promotion("standard"):
+        div = (x**ω / denominator).ω
+    t_out = tree_dot(div, tx).real
     t_out = jnp.where(pred, 0, t_out)
     return out, t_out
 
 
 def rms_norm(x: PyTree[ArrayLike]) -> Scalar:
     """Compute the RMS (root-mean-squared) norm of a PyTree of arrays.
 
@@ -107,15 +104,15 @@
     """
     leaves = jtu.tree_leaves(x)
     size = sum([jnp.size(xi) for xi in leaves])
     if size == 0:
         if len(leaves) == 0:
             dtype = default_floating_dtype()
         else:
-            dtype = jnp.result_type(*leaves)
+            dtype = complex_to_real_dtype(jnp.result_type(*leaves))
         return jnp.array(0.0, dtype)
     else:
         return two_norm(x) / math.sqrt(size)
 
 
 def max_norm(x: PyTree[ArrayLike]) -> Scalar:
     """Compute the L-infinity norm of a PyTree of arrays.
@@ -125,15 +122,15 @@
     """
     leaves = jtu.tree_leaves(x)
     leaf_maxes = [jnp.max(jnp.abs(xi)) for xi in leaves if jnp.size(xi) > 0]
     if len(leaf_maxes) == 0:
         if len(leaves) == 0:
             dtype = default_floating_dtype()
         else:
-            dtype = jnp.result_type(*leaves)
+            dtype = complex_to_real_dtype(jnp.result_type(*leaves))
         return jnp.array(0.0, dtype)
     else:
         out = ft.reduce(jnp.maximum, leaf_maxes)
         return _zero_grad_at_zero(out)
 
 
 @jax.custom_jvp
```

### Comparing `lineax-0.0.4/lineax/_operator.py` & `lineax-0.0.5/lineax/_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,48 +11,38 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import abc
 import functools as ft
 import math
+import warnings
 from collections.abc import Callable
-from typing import (
-    Any,
-    Iterable,
-    NoReturn,
-    TypeVar,
-    Union,
-)
+from typing import Any, Iterable, Literal, NoReturn, Optional, TypeVar, Union
 
 import equinox as eqx
 import equinox.internal as eqxi
 import jax
 import jax.flatten_util as jfu
 import jax.lax as lax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 import numpy as np
 from equinox.internal import ω
-from jaxtyping import (  # pyright: ignore
+from jaxtyping import (
     Array,
     ArrayLike,
     Inexact,
-    PyTree,
+    PyTree,  # pyright: ignore
     Scalar,
     Shaped,
 )
 
 from ._custom_types import sentinel
-from ._misc import (
-    inexact_asarray,
-    jacobian,
-    NoneAux,
-)
-from ._norm import default_floating_dtype
+from ._misc import default_floating_dtype, inexact_asarray, jacobian, NoneAux
 from ._tags import (
     diagonal_tag,
     lower_triangular_tag,
     negative_semidefinite_tag,
     positive_semidefinite_tag,
     symmetric_tag,
     transpose_tags,
@@ -67,15 +57,15 @@
         iter_x = iter(x)  # pyright: ignore
     except TypeError:
         return frozenset([x])
     else:
         return frozenset(iter_x)
 
 
-class AbstractLinearOperator(eqx.Module):
+class AbstractLinearOperator(eqx.Module, strict=True):
     """Abstract base class for all linear operators.
 
     Linear operators can act between PyTrees. Each `AbstractLinearOperator` is thought
     of as a linear function `X -> Y`, where each element of `X` is as PyTree of
     floating-point JAX arrays, and each element of `Y` is a PyTree of floating-point
     JAX arrays.
 
@@ -224,18 +214,18 @@
     def __truediv__(self, other) -> "AbstractLinearOperator":
         other = jnp.asarray(other)
         if other.shape != ():
             raise ValueError("Can only divide AbstractLinearOperators by scalars.")
         return DivLinearOperator(self, other)
 
     def __neg__(self) -> "AbstractLinearOperator":
-        return self * (-1)
+        return NegLinearOperator(self)
 
 
-class MatrixLinearOperator(AbstractLinearOperator):
+class MatrixLinearOperator(AbstractLinearOperator, strict=True):
     """Wraps a 2-dimensional JAX array into a linear operator.
 
     If the matrix has shape `(a, b)` then matrix-vector multiplication (`self.mv`) is
     defined in the usual way: as performing a matrix-vector that accepts a vector of
     shape `(a,)` and returns a vector of shape `(b,)`.
     """
 
@@ -327,15 +317,15 @@
 class _Leaf:  # not a pytree
     def __init__(self, value):
         self.value = value
 
 
 # The `{input,output}_structure`s have to be static because otherwise abstract
 # evaluation rules will promote them to ShapedArrays.
-class PyTreeLinearOperator(AbstractLinearOperator):
+class PyTreeLinearOperator(AbstractLinearOperator, strict=True):
     """Represents a PyTree of floating-point JAX arrays as a linear operator.
 
     This is basically a generalisation of [`lineax.MatrixLinearOperator`][], from
     taking just a single array to take a PyTree-of-arrays. (And likewise from returning
     a single array to returning a PyTree-of-arrays.)
 
     Specifically, suppose we want this to be a linear operator `X -> Y`, for which
@@ -425,15 +415,16 @@
         # return has struture [tree(out), leaf(out)]
         def matmul(_, matrix):
             return _tree_matmul(matrix, vector)
 
         return jtu.tree_map(matmul, self.out_structure(), self.pytree)
 
     def as_matrix(self):
-        dtype = jnp.result_type(*jtu.tree_leaves(self.pytree))
+        with jax.numpy_dtype_promotion("standard"):
+            dtype = jnp.result_type(*jtu.tree_leaves(self.pytree))
 
         def concat_in(struct, subpytree):
             leaves = jtu.tree_leaves(subpytree)
             assert all(leaf.shape[: struct.ndim] == struct.shape for leaf in leaves)
             leaves = [
                 leaf.astype(dtype).reshape(
                     struct.size, math.prod(leaf.shape[struct.ndim :])
@@ -497,15 +488,15 @@
     fn: Callable
 
     def __call__(self, x):
         (f,) = self.fn(x)
         return f
 
 
-class JacobianLinearOperator(AbstractLinearOperator):
+class JacobianLinearOperator(AbstractLinearOperator, strict=True):
     """Given a function `fn: X -> Y`, and a point `x in X`, then this defines the
     linear operator (also a function `X -> Y`) given by the Jacobian `(d(fn)/dx)(x)`.
 
     For example if the inputs and outputs are just arrays, then this is equivalent to
     `MatrixLinearOperator(jax.jacfwd(fn)(x))`.
 
     The Jacobian is not materialised; matrix-vector products, which are in fact
@@ -522,55 +513,73 @@
 
     fn: Callable[
         [PyTree[Inexact[Array, "..."]], PyTree[Any]], PyTree[Inexact[Array, "..."]]
     ]
     x: PyTree[Inexact[Array, "..."]]
     args: PyTree[Any]
     tags: frozenset[object] = eqx.field(static=True)
+    jac: Optional[Literal["fwd", "bwd"]]
 
+    @eqxi.doc_remove_args("closure_convert", "_has_aux")
     def __init__(
         self,
         fn: Callable,
         x: PyTree[ArrayLike],
         args: PyTree[Any] = None,
         tags: Union[object, Iterable[object]] = (),
-        _has_aux: bool = False,
+        closure_convert: bool = True,
+        _has_aux: bool = False,  # TODO(kidger): remove, no longer used
+        jac: Optional[Literal["fwd", "bwd"]] = None,
     ):
         """**Arguments:**
 
         - `fn`: A function `(x, args) -> y`. The Jacobian `d(fn)/dx` is used as the
             linear operator, and `args` are just any other arguments that should not be
             differentiated.
         - `x`: The point to evaluate `d(fn)/dx` at: `(d(fn)/dx)(x, args)`.
         - `args`: As `x`; this is the point to evaluate `d(fn)/dx` at:
             `(d(fn)/dx)(x, args)`.
         - `tags`: any tags indicating whether this operator has any particular
             properties, like symmetry or positive-definite-ness. Note that these
             properties are unchecked and you may get incorrect values elsewhere if these
             tags are wrong.
+        - `jac`: allows to use specific jacobian computation method. If `jac=fwd`
+           forces `jax.jacfwd` to be used, similarly `jac=bwd` mandates the use of
+           `jax.jacrev`. Otherwise, if not specified it will be chosen
+           by default according to input and output shape.
         """
         if not _has_aux:
             fn = NoneAux(fn)
         # Flush out any closed-over values, so that we can safely pass `self`
         # across API boundaries. (In particular, across `linear_solve_p`.)
         # We don't use `jax.closure_convert` as that only flushes autodiffable
         # (=floating-point) constants. It probably doesn't matter, but if `fn` is a
         # PyTree capturing non-floating-point constants, we should probably continue
         # to respect that, and keep any non-floating-point constants as part of the
         # PyTree structure.
         x = jtu.tree_map(inexact_asarray, x)
-        fn = eqx.filter_closure_convert(fn, x, args)
+        if closure_convert:
+            fn = eqx.filter_closure_convert(fn, x, args)
         self.fn = fn
         self.x = x
         self.args = args
         self.tags = _frozenset(tags)
+        self.jac = jac
 
     def mv(self, vector):
         fn = _NoAuxOut(_NoAuxIn(self.fn, self.args))
-        _, out = jax.jvp(fn, (self.x,), (vector,))
+        if self.jac == "fwd" or self.jac is None:
+            _, out = jax.jvp(fn, (self.x,), (vector,))
+        elif self.jac == "bwd":
+            jac = jax.jacrev(fn)(self.x)
+            out = PyTreeLinearOperator(jac, output_structure=self.out_structure()).mv(
+                vector
+            )
+        else:
+            raise ValueError("`jac` should be either `'fwd'`, `'bwd'`, or `None`.")
         return out
 
     def as_matrix(self):
         return materialise(self).as_matrix()
 
     def transpose(self):
         if symmetric_tag in self.tags:
@@ -588,31 +597,33 @@
 
     def out_structure(self):
         fn = _NoAuxOut(_NoAuxIn(self.fn, self.args))
         return eqxi.cached_filter_eval_shape(fn, self.x)
 
 
 # `input_structure` must be static as with `JacobianLinearOperator`
-class FunctionLinearOperator(AbstractLinearOperator):
+class FunctionLinearOperator(AbstractLinearOperator, strict=True):
     """Wraps a *linear* function `fn: X -> Y` into a linear operator. (So that
     `self.mv(x)` is defined by `self.mv(x) == fn(x)`.)
 
     See also [`lineax.materialise`][], which materialises the whole linear operator
     in memory. (Similar to `.as_matrix()`.)
     """
 
     fn: Callable[[PyTree[Inexact[Array, "..."]]], PyTree[Inexact[Array, "..."]]]
     input_structure: _FlatPyTree[jax.ShapeDtypeStruct] = eqx.field(static=True)
     tags: frozenset[object] = eqx.field(static=True)
 
+    @eqxi.doc_remove_args("closure_convert")
     def __init__(
         self,
         fn: Callable[[PyTree[Inexact[Array, "..."]]], PyTree[Inexact[Array, "..."]]],
         input_structure: PyTree[jax.ShapeDtypeStruct],
         tags: Union[object, Iterable[object]] = (),
+        closure_convert: bool = True,
     ):
         """**Arguments:**
 
         - `fn`: a linear function. Should accept a PyTree of floating-point JAX arrays,
             and return a PyTree of floating-point JAX arrays.
         - `input_structure`: A PyTree of `jax.ShapeDtypeStruct`s specifying the
             structure of the input to the function. (When later calling `self.mv(x)`
@@ -620,16 +631,17 @@
             `jax.eval_shape(lambda: x)`.)
         - `tags`: any tags indicating whether this operator has any particular
             properties, like symmetry or positive-definite-ness. Note that these
             properties are unchecked and you may get incorrect values elsewhere if these
             tags are wrong.
         """
         # See matching comment in JacobianLinearOperator.
-        fn = eqx.filter_closure_convert(fn, input_structure)
         input_structure = _inexact_structure(input_structure)
+        if closure_convert:
+            fn = eqx.filter_closure_convert(fn, input_structure)
         self.fn = fn
         self.input_structure = jtu.tree_flatten(input_structure)
         self.tags = _frozenset(tags)
 
     def mv(self, vector):
         return self.fn(vector)
 
@@ -655,15 +667,15 @@
         return jtu.tree_unflatten(treedef, leaves)
 
     def out_structure(self):
         return eqxi.cached_filter_eval_shape(self.fn, self.in_structure())
 
 
 # `structure` must be static as with `JacobianLinearOperator`
-class IdentityLinearOperator(AbstractLinearOperator):
+class IdentityLinearOperator(AbstractLinearOperator, strict=True):
     """Represents the identity transformation `X -> X`, where each `x in X` is some
     PyTree of floating-point JAX arrays.
     """
 
     input_structure: _FlatPyTree[jax.ShapeDtypeStruct] = eqx.field(static=True)
     output_structure: _FlatPyTree[jax.ShapeDtypeStruct] = eqx.field(static=True)
 
@@ -695,28 +707,33 @@
             raise ValueError("Vector and operator structures do not match")
         elif self.input_structure == self.output_structure:
             return vector  # fast-path for common special case
         else:
             # TODO(kidger): this could be done slightly more efficiently, by iterating
             #     leaf-by-leaf.
             leaves = jtu.tree_leaves(vector)
-            dtype = jnp.result_type(*leaves)
+            with jax.numpy_dtype_promotion("standard"):
+                dtype = jnp.result_type(*leaves)
             vector = jnp.concatenate([x.astype(dtype).reshape(-1) for x in leaves])
             out_size = self.out_size()
             if vector.size < out_size:
                 vector = jnp.concatenate(
                     [vector, jnp.zeros(out_size - vector.size, vector.dtype)]
                 )
             else:
                 vector = vector[:out_size]
             leaves, treedef = jtu.tree_flatten(self.out_structure())
             sizes = np.cumsum([math.prod(x.shape) for x in leaves[:-1]])
             split = jnp.split(vector, sizes)
             assert len(split) == len(leaves)
-            shaped = [x.reshape(y.shape).astype(y.dtype) for x, y in zip(split, leaves)]
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore")  # ignore complex-to-real cast warning
+                shaped = [
+                    x.reshape(y.shape).astype(y.dtype) for x, y in zip(split, leaves)
+                ]
             return jtu.tree_unflatten(treedef, shaped)
 
     def as_matrix(self):
         return jnp.eye(self.out_size(), self.in_size())
 
     def transpose(self):
         return IdentityLinearOperator(self.out_structure(), self.in_structure())
@@ -730,15 +747,15 @@
         return jtu.tree_unflatten(treedef, leaves)
 
     @property
     def tags(self):
         return frozenset()
 
 
-class DiagonalLinearOperator(AbstractLinearOperator):
+class DiagonalLinearOperator(AbstractLinearOperator, strict=True):
     """As [`lineax.MatrixLinearOperator`][], but for specifically a diagonal matrix.
 
     Only the diagonal of the matrix is stored (for memory efficiency). Matrix-vector
     products are computed by doing a pointwise `diagonal * vector`, rather than a full
     `matrix @ vector` (for speed).
     """
 
@@ -766,15 +783,15 @@
         return jax.ShapeDtypeStruct(shape=(size,), dtype=self.diagonal.dtype)
 
     def out_structure(self):
         (size,) = jnp.shape(self.diagonal)
         return jax.ShapeDtypeStruct(shape=(size,), dtype=self.diagonal.dtype)
 
 
-class TridiagonalLinearOperator(AbstractLinearOperator):
+class TridiagonalLinearOperator(AbstractLinearOperator, strict=True):
     """As [`lineax.MatrixLinearOperator`][], but for specifically a tridiagonal
     matrix.
     """
 
     diagonal: Inexact[Array, " size"]
     lower_diagonal: Inexact[Array, " size-1"]
     upper_diagonal: Inexact[Array, " size-1"]
@@ -830,15 +847,15 @@
         return jax.ShapeDtypeStruct(shape=(size,), dtype=self.diagonal.dtype)
 
     def out_structure(self):
         (size,) = jnp.shape(self.diagonal)
         return jax.ShapeDtypeStruct(shape=(size,), dtype=self.diagonal.dtype)
 
 
-class TaggedLinearOperator(AbstractLinearOperator):
+class TaggedLinearOperator(AbstractLinearOperator, strict=True):
     """Wraps another linear operator and specifies that it has certain tags, e.g.
     representing symmetry.
 
     !!! Example
 
         ```python
         # Some other operator.
@@ -894,15 +911,15 @@
 #
 
 
 def _is_none(x):
     return x is None
 
 
-class TangentLinearOperator(AbstractLinearOperator):
+class TangentLinearOperator(AbstractLinearOperator, strict=True):
     """Internal to lineax. Used to represent the tangent (jvp) computation with
     respect to the linear operator in a linear solve.
     """
 
     primal: AbstractLinearOperator
     tangent: AbstractLinearOperator
 
@@ -929,15 +946,15 @@
     def in_structure(self):
         return self.primal.in_structure()
 
     def out_structure(self):
         return self.primal.out_structure()
 
 
-class AddLinearOperator(AbstractLinearOperator):
+class AddLinearOperator(AbstractLinearOperator, strict=True):
     """A linear operator formed by adding two other linear operators together.
 
     !!! Example
 
         ```python
         x = MatrixLinearOperator(...)
         y = MatrixLinearOperator(...)
@@ -968,15 +985,15 @@
     def in_structure(self):
         return self.operator1.in_structure()
 
     def out_structure(self):
         return self.operator1.out_structure()
 
 
-class MulLinearOperator(AbstractLinearOperator):
+class MulLinearOperator(AbstractLinearOperator, strict=True):
     """A linear operator formed by multiplying a linear operator by a scalar.
 
     !!! Example
 
         ```python
         x = MatrixLinearOperator(...)
         y = 0.5
@@ -999,15 +1016,46 @@
     def in_structure(self):
         return self.operator.in_structure()
 
     def out_structure(self):
         return self.operator.out_structure()
 
 
-class DivLinearOperator(AbstractLinearOperator):
+# Not just `MulLinearOperator(..., -1)` for compatibility with
+# `jax_numpy_dtype_promotion=strict`.
+class NegLinearOperator(AbstractLinearOperator, strict=True):
+    """A linear operator formed by computing the negative of a linear operator.
+
+    !!! Example
+
+        ```python
+        x = MatrixLinearOperator(...)
+        assert isinstance(-x, NegLinearOperator)
+        ```
+    """
+
+    operator: AbstractLinearOperator
+
+    def mv(self, vector):
+        return (-(self.operator.mv(vector) ** ω)).ω
+
+    def as_matrix(self):
+        return -self.operator.as_matrix()
+
+    def transpose(self):
+        return -self.operator.transpose()
+
+    def in_structure(self):
+        return self.operator.in_structure()
+
+    def out_structure(self):
+        return self.operator.out_structure()
+
+
+class DivLinearOperator(AbstractLinearOperator, strict=True):
     """A linear operator formed by dividing a linear operator by a scalar.
 
     !!! Example
 
         ```python
         x = MatrixLinearOperator(...)
         y = 0.5
@@ -1015,30 +1063,31 @@
         ```
     """
 
     operator: AbstractLinearOperator
     scalar: Scalar
 
     def mv(self, vector):
-        return (self.operator.mv(vector) ** ω / self.scalar).ω
+        with jax.numpy_dtype_promotion("standard"):
+            return (self.operator.mv(vector) ** ω / self.scalar).ω
 
     def as_matrix(self):
         return self.operator.as_matrix() / self.scalar
 
     def transpose(self):
         return self.operator.transpose() / self.scalar
 
     def in_structure(self):
         return self.operator.in_structure()
 
     def out_structure(self):
         return self.operator.out_structure()
 
 
-class ComposedLinearOperator(AbstractLinearOperator):
+class ComposedLinearOperator(AbstractLinearOperator, strict=True):
     """A linear operator formed by composing (matrix-multiplying) two other linear
     operators together.
 
     !!! Example
 
         ```python
         x = MatrixLinearOperator(matrix1)
@@ -1059,28 +1108,28 @@
     def mv(self, vector):
         return self.operator1.mv(self.operator2.mv(vector))
 
     def as_matrix(self):
         return jnp.matmul(
             self.operator1.as_matrix(),
             self.operator2.as_matrix(),
-            precision=lax.Precision.HIGHEST,
+            precision=lax.Precision.HIGHEST,  # pyright: ignore
         )
 
     def transpose(self):
         return self.operator2.transpose() @ self.operator1.transpose()
 
     def in_structure(self):
         return self.operator2.in_structure()
 
     def out_structure(self):
         return self.operator1.out_structure()
 
 
-class AuxLinearOperator(AbstractLinearOperator):
+class AuxLinearOperator(AbstractLinearOperator, strict=True):
     """Internal to lineax. Used to represent a linear operator with additional
     metadata attached.
     """
 
     operator: AbstractLinearOperator
     aux: PyTree[Array]
 
@@ -1243,14 +1292,15 @@
     fn = _NoAuxIn(operator.fn, operator.args)
     jac, aux = jacobian(
         fn,
         operator.in_size(),
         operator.out_size(),
         holomorphic=any(jnp.iscomplexobj(xi) for xi in jtu.tree_leaves(operator.x)),
         has_aux=True,
+        jac=operator.jac,
     )(operator.x)
     out = PyTreeLinearOperator(jac, operator.out_structure(), operator.tags)
     return AuxLinearOperator(out, aux)
 
 
 @materialise.register(FunctionLinearOperator)
 def _(operator):
@@ -1739,14 +1789,18 @@
     def _(operator, transform=transform):
         return transform(operator.operator1) + transform(operator.operator2)
 
     @transform.register(MulLinearOperator)
     def _(operator, transform=transform):
         return transform(operator.operator) * operator.scalar
 
+    @transform.register(NegLinearOperator)  # pyright: ignore
+    def _(operator, transform=transform):
+        return -transform(operator.operator)
+
     @transform.register(DivLinearOperator)
     def _(operator, transform=transform):
         return transform(operator.operator) / operator.scalar
 
     @transform.register(AuxLinearOperator)  # pyright: ignore
     def _(operator, transform=transform):
         return transform(operator.operator)
@@ -1795,14 +1849,20 @@
 
 @tridiagonal.register(MulLinearOperator)
 def _(operator):
     (diag, lower, upper) = tridiagonal(operator.operator)
     return (diag * operator.scalar, lower * operator.scalar, upper * operator.scalar)
 
 
+@tridiagonal.register(NegLinearOperator)
+def _(operator):
+    (diag, lower, upper) = tridiagonal(operator.operator)
+    return (-diag, -lower, -upper)
+
+
 @tridiagonal.register(DivLinearOperator)
 def _(operator):
     (diag, lower, upper) = tridiagonal(operator.operator)
     return (diag / operator.scalar, lower / operator.scalar, upper / operator.scalar)
 
 
 @tridiagonal.register(AuxLinearOperator)
@@ -1837,25 +1897,48 @@
 
 for check in (
     is_symmetric,
     is_diagonal,
     has_unit_diagonal,
     is_lower_triangular,
     is_upper_triangular,
-    is_positive_semidefinite,
-    is_negative_semidefinite,
     is_tridiagonal,
 ):
 
     @check.register(TangentLinearOperator)
     def _(operator, check=check):
         return check(operator.primal)
 
     @check.register(MulLinearOperator)
+    @check.register(NegLinearOperator)
+    @check.register(DivLinearOperator)
+    @check.register(AuxLinearOperator)
+    def _(operator, check=check):
+        return check(operator.operator)
+
+
+for check in (is_positive_semidefinite, is_negative_semidefinite):
+
+    @check.register(TangentLinearOperator)
+    def _(operator):
+        # Should be unreachable: TangentLinearOperator is used for a narrow set of
+        # operations only (mv; transpose) inside the JVP rule linear_solve_p.
+        raise NotImplementedError(
+            "Please open a GitHub issue: https://github.com/google/lineax"
+        )
+
+    @check.register(MulLinearOperator)
     @check.register(DivLinearOperator)
+    def _(operator):
+        return False  # play it safe, no way to tell.
+
+    @check.register(NegLinearOperator)
+    def _(operator, check=check):
+        return not check(operator.operator)
+
     @check.register(AuxLinearOperator)
     def _(operator, check=check):
         return check(operator.operator)
 
 
 for check, tag in (
     (is_symmetric, symmetric_tag),
@@ -1998,14 +2081,19 @@
 
 
 @conj.register(MulLinearOperator)
 def _(operator):
     return conj(operator.operator) * operator.scalar.conj()
 
 
+@conj.register(NegLinearOperator)
+def _(operator):
+    return -conj(operator.operator)
+
+
 @conj.register(DivLinearOperator)
 def _(operator):
     return conj(operator.operator) / operator.scalar.conj()
 
 
 @conj.register(ComposedLinearOperator)
 def _(operator):
```

### Comparing `lineax-0.0.4/lineax/_solution.py` & `lineax-0.0.5/lineax/_solution.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     )
     stagnation = (
         "A stagnation in an iterative linear solve has occurred. Try increasing "
         "`stagnation_iters` or `restart`."
     )
 
 
-class Solution(eqx.Module):
+class Solution(eqx.Module, strict=True):
     """The solution to a linear solve.
 
     **Attributes:**
 
     - `value`: The solution to the solve.
     - `result`: An integer representing whether the solve was successful or not. This
         can be converted into a human-readable error message via
```

### Comparing `lineax-0.0.4/lineax/_solve.py` & `lineax-0.0.5/lineax/_solve.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,14 +263,19 @@
 @eqxi.filter_primitive_transpose(materialise_zeros=True)  # pyright: ignore
 def _linear_solve_transpose(inputs, cts_out):
     cts_solution, _, _ = cts_out
     operator, state, vector, options, solver, _ = inputs
     jtu.tree_map(
         _assert_defined, (operator, state, options, solver), is_leaf=_is_undefined
     )
+    cts_solution = jtu.tree_map(
+        ft.partial(eqxi.materialise_zeros, allow_struct=True),
+        operator.in_structure(),
+        cts_solution,
+    )
     operator_transpose = operator.transpose()
     state_transpose, options_transpose = solver.transpose(state, options)
     cts_vector, _, _ = eqxi.filter_primitive_bind(
         linear_solve_p,
         operator_transpose,
         state_transpose,
         cts_solution,
@@ -308,15 +313,15 @@
 # linear_solve
 #
 
 
 _SolverState = TypeVar("_SolverState")
 
 
-class AbstractLinearSolver(eqx.Module, Generic[_SolverState]):
+class AbstractLinearSolver(eqx.Module, Generic[_SolverState], strict=True):
     """Abstract base class for all linear solvers."""
 
     @abc.abstractmethod
     def init(
         self, operator: AbstractLinearOperator, options: dict[str, Any]
     ) -> _SolverState:
         """Do any initial computation on just the `operator`.
@@ -516,15 +521,15 @@
     }
     return _lookup_dict[token]
 
 
 _AutoLinearSolverState: TypeAlias = tuple[Any, Any]
 
 
-class AutoLinearSolver(AbstractLinearSolver[_AutoLinearSolverState]):
+class AutoLinearSolver(AbstractLinearSolver[_AutoLinearSolverState], strict=True):
     """Automatically determines a good linear solver based on the structure of the
     operator.
 
     - If `well_posed=True`:
         - If the operator is diagonal, then use [`lineax.Diagonal`][].
         - If the operator is tridiagonal, then use [`lineax.Tridiagonal`][].
         - If the operator is triangular, then use [`lineax.Triangular`][].
```

### Comparing `lineax-0.0.4/lineax/_tags.py` & `lineax-0.0.5/lineax/_tags.py`

 * *Files identical despite different names*

### Comparing `lineax-0.0.4/lineax/_solver/__init__.py` & `lineax-0.0.5/lineax/_solver/__init__.py`

 * *Files identical despite different names*

### Comparing `lineax-0.0.4/lineax/_solver/bicgstab.py` & `lineax-0.0.5/lineax/_solver/bicgstab.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from .._solve import AbstractLinearSolver
 from .misc import preconditioner_and_y0
 
 
 _BiCGStabState: TypeAlias = AbstractLinearOperator
 
 
-class BiCGStab(AbstractLinearSolver[_BiCGStabState]):
+class BiCGStab(AbstractLinearSolver[_BiCGStabState], strict=True):
     """Biconjugate gradient stabilised method for linear systems.
 
     The operator should be square.
 
     Equivalent to `jax.scipy.sparse.linalg.bicgstab`.
 
     This supports the following `options` (as passed to
@@ -97,14 +97,15 @@
             b_scale = (self.atol + self.rtol * ω(vector).call(jnp.abs)).ω
 
         # This implementation is the same a jax.scipy.sparse.linalg.bicgstab
         # but with AbstractLinearOperator.
         # We use the notation found on the wikipedia except with y instead of x:
         # https://en.wikipedia.org/wiki/
         # Biconjugate_gradient_stabilized_method#Preconditioned_BiCGSTAB
+        # preconditioner in this case is K2^(-1) (i.e., right preconditioning)
 
         r0 = (vector**ω - operator.mv(y0) ** ω).ω
 
         def breakdown_occurred(omega, alpha, rho):
             # Empirically, the tolerance checks for breakdown are very tight.
             # These specific tolerances are heuristic.
             if jax.config.jax_enable_x64:  # pyright: ignore
@@ -113,41 +114,42 @@
                 return (omega < 1e-16) | (alpha < 1e-16) | (rho < 1e-16)
 
         def not_converged(r, diff, y):
             # The primary tolerance check.
             # Given Ay=b, then we have to be doing better than `scale` in both
             # the `y` and the `b` spaces.
             if has_scale:
-                y_scale = (self.atol + self.rtol * ω(y).call(jnp.abs)).ω
-                norm1 = self.norm((r**ω / b_scale**ω).ω)  # pyright: ignore
-                norm2 = self.norm((diff**ω / y_scale**ω).ω)
+                with jax.numpy_dtype_promotion("standard"):
+                    y_scale = (self.atol + self.rtol * ω(y).call(jnp.abs)).ω
+                    norm1 = self.norm((r**ω / b_scale**ω).ω)  # pyright: ignore
+                    norm2 = self.norm((diff**ω / y_scale**ω).ω)
                 return (norm1 > 1) | (norm2 > 1)
             else:
                 return True
 
         def cond_fun(carry):
             y, r, alpha, omega, rho, _, _, diff, step = carry
             out = jnp.invert(breakdown_occurred(omega, alpha, rho))
             out = out & not_converged(r, diff, y)
             out = out & (step < max_steps)
             return out
 
         def body_fun(carry):
             y, r, alpha, omega, rho, p, v, diff, step = carry
 
-            rho_new = tree_dot(r0, r)
+            rho_new = tree_dot(r, r0)
             beta = (rho_new / rho) * (alpha / omega)
             p_new = (r**ω + beta * (p**ω - omega * v**ω)).ω
 
             # TODO(raderj): reduce this to a single operator.mv call
             # by using the scan trick.
             x = preconditioner.mv(p_new)
             v_new = operator.mv(x)
 
-            alpha_new = rho_new / tree_dot(r0, v_new)
+            alpha_new = rho_new / tree_dot(v_new, r0)
             s = (r**ω - alpha_new * v_new**ω).ω
 
             z = preconditioner.mv(s)
             t = operator.mv(z)
 
             omega_new = tree_dot(t, s) / tree_dot(t, t)
```

### Comparing `lineax-0.0.4/lineax/_solver/cg.py` & `lineax-0.0.5/lineax/_solver/cg.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 from collections.abc import Callable
 from typing import Any, ClassVar, Optional
 from typing_extensions import TYPE_CHECKING, TypeAlias
 
 import equinox.internal as eqxi
+import jax
 import jax.lax as lax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 from equinox.internal import ω
 from jaxtyping import Array, PyTree, Scalar
 
 
@@ -46,15 +47,15 @@
 _CGState: TypeAlias = tuple[AbstractLinearOperator, bool]
 
 
 # TODO(kidger): this is pretty slow to compile.
 # - CG evaluates `operator.mv` three times.
 # - Normal CG evaluates `operator.mv` seven (!) times.
 # Possibly this can be cheapened a bit somehow?
-class _CG(AbstractLinearSolver[_CGState]):
+class _AbstractCG(AbstractLinearSolver[_CGState], strict=True):
     rtol: float
     atol: float
     norm: Callable[[PyTree], Scalar] = max_norm
     stabilise_every: Optional[int] = 10
     max_steps: Optional[int] = None
 
     _normal: AbstractClassVar[bool]
@@ -153,17 +154,18 @@
             b_scale = (self.atol + self.rtol * ω(vector).call(jnp.abs)).ω
 
         def not_converged(r, diff, y):
             # The primary tolerance check.
             # Given Ay=b, then we have to be doing better than `scale` in both
             # the `y` and the `b` spaces.
             if has_scale:
-                y_scale = (self.atol + self.rtol * ω(y).call(jnp.abs)).ω
-                norm1 = self.norm((r**ω / b_scale**ω).ω)  # pyright: ignore
-                norm2 = self.norm((diff**ω / y_scale**ω).ω)
+                with jax.numpy_dtype_promotion("standard"):
+                    y_scale = (self.atol + self.rtol * ω(y).call(jnp.abs)).ω
+                    norm1 = self.norm((r**ω / b_scale**ω).ω)  # pyright: ignore
+                    norm2 = self.norm((diff**ω / y_scale**ω).ω)
                 return (norm1 > 1) | (norm2 > 1)
             else:
                 return True
 
         def cond_fun(value):
             diff, y, r, _, gamma, step = value
             out = gamma > 0
@@ -173,15 +175,15 @@
 
         def body_fun(value):
             _, y, r, p, gamma, step = value
             mat_p = mv(p)
             inner_prod = tree_dot(p, mat_p)
             alpha = gamma / inner_prod
             alpha = tree_where(
-                jnp.abs(inner_prod) > 100 * rcond * gamma, alpha, jnp.nan
+                jnp.abs(inner_prod) > 100 * rcond * jnp.abs(gamma), alpha, jnp.nan
             )
             diff = (alpha * p**ω).ω
             y = (y**ω + diff**ω).ω
             step = step + 1
 
             # E.g. see B.2 of
             # https://www.cs.cmu.edu/~quake-papers/painless-conjugate-gradient.pdf
@@ -242,15 +244,15 @@
         del options
         psd_op, is_nsd = state
         conj_state = conj(psd_op), is_nsd
         conj_options = {}
         return conj_state, conj_options
 
 
-class CG(_CG):
+class CG(_AbstractCG, strict=True):
     """Conjugate gradient solver for linear systems.
 
     The operator should be positive or negative definite.
 
     Equivalent to `scipy.sparse.linalg.cg`.
 
     This supports the following `options` (as passed to
@@ -272,15 +274,15 @@
     def allow_dependent_columns(self, operator):
         return False
 
     def allow_dependent_rows(self, operator):
         return False
 
 
-class NormalCG(_CG):
+class NormalCG(_AbstractCG, strict=True):
     """Conjugate gradient applied to the normal equations:
 
     `A^T A = A^T b`
 
     of a system of linear equations. Note that this squares the condition
     number, so it is not recommended. This is a fast but potentially inaccurate
     method, especially in 32 bit floating point precision.
```

### Comparing `lineax-0.0.4/lineax/_solver/cholesky.py` & `lineax-0.0.5/lineax/_solver/cholesky.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from .._solution import RESULTS
 from .._solve import AbstractLinearSolver
 
 
 _CholeskyState: TypeAlias = tuple[Array, bool]
 
 
-class Cholesky(AbstractLinearSolver[_CholeskyState]):
+class Cholesky(AbstractLinearSolver[_CholeskyState], strict=True):
     """Cholesky solver for linear systems. This is generally the preferred solver for
     positive or negative definite systems.
 
     Equivalent to `scipy.linalg.solve(..., assume_a="pos")`.
 
     The operator must be square, nonsingular, and either positive or negative definite.
     """
```

### Comparing `lineax-0.0.4/lineax/_solver/diagonal.py` & `lineax-0.0.5/lineax/_solver/diagonal.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from .._solution import RESULTS
 from .._solve import AbstractLinearSolver
 
 
 _DiagonalState: TypeAlias = Optional[Array]
 
 
-class Diagonal(AbstractLinearSolver[_DiagonalState]):
+class Diagonal(AbstractLinearSolver[_DiagonalState], strict=True):
     """Diagonal solver for linear systems.
 
     Requires that the operator be diagonal. Then $Ax = b$, with $A = diag[a]$, is
     solved simply by doing an elementwise division $x = b / a$.
 
     This solver can handle singular operators (i.e. diagonal entries with value 0).
     """
```

### Comparing `lineax-0.0.4/lineax/_solver/gmres.py` & `lineax-0.0.5/lineax/_solver/gmres.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 
 import functools as ft
 from collections.abc import Callable
 from typing import Any, cast, Optional
 from typing_extensions import TypeAlias
 
 import equinox.internal as eqxi
+import jax
 import jax.lax as lax
 import jax.numpy as jnp
 import jax.tree_util as jtu
 from equinox.internal import ω
-from jaxtyping import Array, ArrayLike, Bool, Float, PyTree
+from jaxtyping import Array, ArrayLike, Bool, Float, Inexact, PyTree
 
 from .._norm import max_norm, two_norm
 from .._operator import (
     AbstractLinearOperator,
     conj,
     MatrixLinearOperator,
 )
@@ -35,15 +36,15 @@
 from .misc import preconditioner_and_y0
 from .qr import QR
 
 
 _GMRESState: TypeAlias = AbstractLinearOperator
 
 
-class GMRES(AbstractLinearSolver[_GMRESState]):
+class GMRES(AbstractLinearSolver[_GMRESState], strict=True):
     """GMRES solver for linear systems.
 
     The operator should be square.
 
     Similar to `jax.scipy.sparse.linalg.gmres`.
 
     This supports the following `options` (as passed to
@@ -128,17 +129,18 @@
         restart = min(self.restart, size)
 
         def not_converged(r, diff, y):
             # The primary tolerance check.
             # Given Ay=b, then we have to be doing better than `scale` in both
             # the `y` and the `b` spaces.
             if has_scale:
-                y_scale = (self.atol + self.rtol * ω(y).call(jnp.abs)).ω
-                norm1 = self.norm((r**ω / b_scale**ω).ω)  # pyright: ignore
-                norm2 = self.norm((diff**ω / y_scale**ω).ω)
+                with jax.numpy_dtype_promotion("standard"):
+                    y_scale = (self.atol + self.rtol * ω(y).call(jnp.abs)).ω
+                    norm1 = self.norm((r**ω / b_scale**ω).ω)  # pyright: ignore
+                    norm2 = self.norm((diff**ω / y_scale**ω).ω)
                 return (norm1 > 1) | (norm2 > 1)
             else:
                 return True
 
         def cond_fun(carry):
             y, r, _, deferred_breakdown, diff, _, step, stagnation_counter = carry
             # NOTE: we defer ending due to breakdown by one loop! This is nonstandard,
@@ -287,15 +289,18 @@
                 return basis, coeff_mat
 
             init_carry = (basis_init, coeff_mat_init, initial_breakdown, 0)
             basis, coeff_mat, breakdown, steps = eqxi.while_loop(
                 cond_fun, body_fun, init_carry, kind="lax", buffers=buffers
             )
             beta_vec = jnp.concatenate(
-                (r_norm[None], jnp.zeros_like(coeff_mat, shape=(restart,)))
+                (
+                    r_norm[None].astype(coeff_mat),
+                    jnp.zeros_like(coeff_mat, shape=(restart,)),
+                )
             )
             coeff_op_transpose = MatrixLinearOperator(coeff_mat.T)
             # TODO(raderj): move to a Hessenberg-specific solver
             z = linear_solve(coeff_op_transpose, beta_vec, QR(), throw=False).value
             diff = jtu.tree_map(
                 lambda mat: jnp.tensordot(
                     mat[..., :-1], z, axes=1, precision=lax.Precision.HIGHEST
@@ -364,15 +369,15 @@
             basis_step_new, eps=eps
         )
         basis_new = jtu.tree_map(
             lambda y, mat: mat.at[..., step + 1].set(y),
             basis_step_normalised,
             basis,
         )
-        proj_new = proj.at[step + 1].set(step_norm_new)
+        proj_new = proj.at[step + 1].set(step_norm_new.astype(proj))
         #
         # NOTE: two somewhat complicated things are going on here:
         #
         # The `coeff_mat` in_place update has a batch tracer, so we need to be
         # careful and wrap it in a buffer, hence the use of eqxi.while_loop
         # instead of lax.while_loop throughout.
         #
@@ -391,21 +396,24 @@
         coeff_mat_new = coeff_mat.at[step, :].set(
             proj_new, pred=jnp.invert(initial_breakdown)
         )
         return basis_new, coeff_mat_new, breakdown
 
     def _normalise(
         self, x: PyTree[Array], eps: Optional[Float[ArrayLike, ""]]
-    ) -> tuple[PyTree[Array], Float[Array, ""], Bool[ArrayLike, ""]]:
+    ) -> tuple[PyTree[Array], Inexact[Array, ""], Bool[ArrayLike, ""]]:
         norm = two_norm(x)
         if eps is None:
             eps = jnp.finfo(norm.dtype).eps
+        else:
+            eps = jnp.astype(eps, norm.dtype)
         breakdown = norm < eps
         safe_norm = jnp.where(breakdown, jnp.inf, norm)
-        x_normalised = (x**ω / safe_norm).ω
+        with jax.numpy_dtype_promotion("standard"):
+            x_normalised = (x**ω / safe_norm).ω
         return x_normalised, norm, breakdown
 
     def transpose(self, state: _GMRESState, options: dict[str, Any]):
         del options
         operator = state
         transpose_options = {}
         return operator.transpose(), transpose_options
```

### Comparing `lineax-0.0.4/lineax/_solver/lu.py` & `lineax-0.0.5/lineax/_solver/lu.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     unravel_solution,
 )
 
 
 _LUState: TypeAlias = tuple[tuple[Array, Array], PackedStructures, bool]
 
 
-class LU(AbstractLinearSolver[_LUState]):
+class LU(AbstractLinearSolver[_LUState], strict=True):
     """LU solver for linear systems.
 
     This solver can only handle square nonsingular operators.
     """
 
     def init(self, operator: AbstractLinearOperator, options: dict[str, Any]):
         del options
```

### Comparing `lineax-0.0.4/lineax/_solver/misc.py` & `lineax-0.0.5/lineax/_solver/misc.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import math
+import warnings
 from typing import Any, NewType
 
 import equinox as eqx
 import equinox.internal as eqxi
 import jax
 import jax.numpy as jnp
 import jax.tree_util as jtu
@@ -93,15 +94,17 @@
 ) -> PyTree[Array]:
     leaves, treedef = packed_structures.value
     _, in_structure = jtu.tree_unflatten(treedef, leaves)
     leaves, treedef = jtu.tree_flatten(in_structure)
     sizes = np.cumsum([math.prod(x.shape) for x in leaves[:-1]])
     split = jnp.split(solution, sizes)
     assert len(split) == len(leaves)
-    shaped = [x.reshape(y.shape).astype(y.dtype) for x, y in zip(split, leaves)]
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore")  # ignore complex-to-real cast warning
+        shaped = [x.reshape(y.shape).astype(y.dtype) for x, y in zip(split, leaves)]
     return jtu.tree_unflatten(treedef, shaped)
 
 
 def transpose_packed_structures(
     packed_structures: PackedStructures,
 ) -> PackedStructures:
     leaves, treedef = packed_structures.value
```

### Comparing `lineax-0.0.4/lineax/_solver/qr.py` & `lineax-0.0.5/lineax/_solver/qr.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     unravel_solution,
 )
 
 
 _QRState: TypeAlias = tuple[tuple[Array, Array], bool, PackedStructures]
 
 
-class QR(AbstractLinearSolver):
+class QR(AbstractLinearSolver, strict=True):
     """QR solver for linear systems.
 
     This solver can handle non-square operators.
 
     This is usually the preferred solver when dealing with non-square operators.
 
     !!! info
```

### Comparing `lineax-0.0.4/lineax/_solver/svd.py` & `lineax-0.0.5/lineax/_solver/svd.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     unravel_solution,
 )
 
 
 _SVDState: TypeAlias = tuple[tuple[Array, Array, Array], PackedStructures]
 
 
-class SVD(AbstractLinearSolver[_SVDState]):
+class SVD(AbstractLinearSolver[_SVDState], strict=True):
     """SVD solver for linear systems.
 
     This solver can handle any operator, even nonsquare or singular ones. In these
     cases it will return the pseudoinverse solution to the linear system.
 
     Equivalent to `scipy.linalg.lstsq`.
     """
@@ -68,15 +68,15 @@
         rcond = jnp.array(rcond, dtype=s.dtype)
         if s.size > 0:
             rcond = rcond * s[0]
         # Not >=, or this fails with a matrix of all-zeros.
         mask = s > rcond
         rank = mask.sum()
         safe_s = jnp.where(mask, s, 1)
-        s_inv = jnp.where(mask, jnp.array(1.0) / safe_s, 0)
+        s_inv = jnp.where(mask, jnp.array(1.0) / safe_s, 0).astype(u.dtype)
         uTb = jnp.matmul(u.conj().T, vector, precision=lax.Precision.HIGHEST)
         solution = jnp.matmul(vt.conj().T, s_inv * uTb, precision=lax.Precision.HIGHEST)
         solution = unravel_solution(solution, packed_structures)
         return solution, RESULTS.successful, {"rank": rank}
 
     def transpose(self, state: _SVDState, options: dict[str, Any]):
         del options
```

### Comparing `lineax-0.0.4/lineax/_solver/triangular.py` & `lineax-0.0.5/lineax/_solver/triangular.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     unravel_solution,
 )
 
 
 _TriangularState: TypeAlias = tuple[Array, bool, bool, PackedStructures, bool]
 
 
-class Triangular(AbstractLinearSolver[_TriangularState]):
+class Triangular(AbstractLinearSolver[_TriangularState], strict=True):
     """Triangular solver for linear systems.
 
     The operator should either be lower triangular or upper triangular.
     """
 
     def init(self, operator: AbstractLinearOperator, options: dict[str, Any]):
         del options
```

### Comparing `lineax-0.0.4/lineax/_solver/tridiagonal.py` & `lineax-0.0.5/lineax/_solver/tridiagonal.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     unravel_solution,
 )
 
 
 _TridiagonalState: TypeAlias = tuple[tuple[Array, Array, Array], PackedStructures]
 
 
-class Tridiagonal(AbstractLinearSolver[_TridiagonalState]):
+class Tridiagonal(AbstractLinearSolver[_TridiagonalState], strict=True):
     """Tridiagonal solver for linear systems, using the Thomas algorithm."""
 
     def init(self, operator: AbstractLinearOperator, options: dict[str, Any]):
         del options
         if operator.in_size() != operator.out_size():
             raise ValueError(
                 "`Tridiagonal` may only be used for linear solves with square matrices"
```

### Comparing `lineax-0.0.4/lineax/internal/__init__.py` & `lineax-0.0.5/lineax/internal/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,16 +8,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .._norm import (
+
+from .._misc import (
+    complex_to_real_dtype as complex_to_real_dtype,
     default_floating_dtype as default_floating_dtype,
+)
+from .._norm import (
     max_norm as max_norm,
     rms_norm as rms_norm,
     sum_squares as sum_squares,
     tree_dot as tree_dot,
     two_norm as two_norm,
 )
 from .._solve import linear_solve_p as linear_solve_p
```

### Comparing `lineax-0.0.4/LICENSE` & `lineax-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lineax-0.0.4/README.md` & `lineax-0.0.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 - PyTree-valued matrices and vectors;
 - General linear operators for Jacobians, transposes, etc.;
 - Efficient linear least squares (e.g. QR solvers);
 - Numerically stable gradients through linear least squares;
 - Support for structured (e.g. symmetric) matrices;
 - Improved compilation times;
 - Improved runtime of some algorithms;
-- All the benefits of working with JAX: autodiff, autoparallelism, GPU/TPU support etc.
+- Support for both real-valued and complex-valued inputs;
+- All the benefits of working with JAX: autodiff, autoparallelism, GPU/TPU support, etc.
 
 ## Installation
 
 ```bash
 pip install lineax
 ```
```

### Comparing `lineax-0.0.4/pyproject.toml` & `lineax-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "lineax"
-version = "0.0.4"
+version = "0.0.5"
 description = "Linear solvers in JAX and Equinox."
 readme = "README.md"
 requires-python ="~=3.9"
 license = {file = "LICENSE"}
 authors = [
   {name = "Jason Rader", email = "raderjason@outlook.com"},
   {name = "Patrick Kidger", email = "contact@kidger.site"},
@@ -20,15 +20,15 @@
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Mathematics",
 ]
 urls = {repository = "https://github.com/google/lineax" }
-dependencies = ["jax>=0.4.13", "jaxtyping>=0.2.20", "equinox>=0.11.0", "typing_extensions>=4.5.0"]
+dependencies = ["jax>=0.4.26", "jaxtyping>=0.2.20", "equinox>=0.11.3", "typing_extensions>=4.5.0"]
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 include = ["lineax/*"]
```

### Comparing `lineax-0.0.4/PKG-INFO` & `lineax-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: lineax
-Version: 0.0.4
+Version: 0.0.5
 Summary: Linear solvers in JAX and Equinox.
 Project-URL: repository, https://github.com/google/lineax
 Author-email: Jason Rader <raderjason@outlook.com>, Patrick Kidger <contact@kidger.site>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -215,16 +215,16 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: ~=3.9
-Requires-Dist: equinox>=0.11.0
-Requires-Dist: jax>=0.4.13
+Requires-Dist: equinox>=0.11.3
+Requires-Dist: jax>=0.4.26
 Requires-Dist: jaxtyping>=0.2.20
 Requires-Dist: typing-extensions>=4.5.0
 Description-Content-Type: text/markdown
 
 <h1 align='center'>Lineax</h1>
 
 Lineax is a [JAX](https://github.com/google/jax) library for linear solves and linear least squares. That is, Lineax provides routines that solve for $x$ in $Ax = b$. (Even when $A$ may be ill-posed or rectangular.)
@@ -233,15 +233,16 @@
 - PyTree-valued matrices and vectors;
 - General linear operators for Jacobians, transposes, etc.;
 - Efficient linear least squares (e.g. QR solvers);
 - Numerically stable gradients through linear least squares;
 - Support for structured (e.g. symmetric) matrices;
 - Improved compilation times;
 - Improved runtime of some algorithms;
-- All the benefits of working with JAX: autodiff, autoparallelism, GPU/TPU support etc.
+- Support for both real-valued and complex-valued inputs;
+- All the benefits of working with JAX: autodiff, autoparallelism, GPU/TPU support, etc.
 
 ## Installation
 
 ```bash
 pip install lineax
 ```
```

