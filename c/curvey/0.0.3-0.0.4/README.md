# Comparing `tmp/curvey-0.0.3.tar.gz` & `tmp/curvey-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Apr 13 14:04:30 2024, max compression
+gzip compressed data, last modified: Sun Apr 14 14:10:31 2024, max compression
```

## Comparing `curvey-0.0.3.tar` & `curvey-0.0.4.tar`

### file list

```diff
@@ -1,57 +1,58 @@
--rw-r--r--   0        0        0     1102 2024-04-13 14:04:30.000000 curvey-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      335 2024-04-13 14:04:30.000000 curvey-0.0.3/environment.yml
--rw-r--r--   0        0        0     3197 2024-04-13 14:04:30.000000 curvey-0.0.3/mkdocs.yml
--rw-r--r--   0        0        0       47 2024-04-13 14:04:30.000000 curvey-0.0.3/requirements.txt
--rw-r--r--   0        0        0      588 2024-04-13 14:04:30.000000 curvey-0.0.3/.github/workflows/release.yml
--rw-r--r--   0        0        0      801 2024-04-13 14:04:30.000000 curvey-0.0.3/.github/workflows/test.yml
--rw-r--r--   0        0        0     1615 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/bibliography.md
--rw-r--r--   0        0        0      358 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/index.md
--rw-r--r--   0        0        0       36 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/api/blend.md
--rw-r--r--   0        0        0     3288 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/api/curve.md
--rw-r--r--   0        0        0       38 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/api/curves.md
--rw-r--r--   0        0        0       36 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/api/edges.md
--rw-r--r--   0        0        0       34 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/api/flow.md
--rw-r--r--   0        0        0      578 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/api/index.md
--rw-r--r--   0        0        0       40 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/api/polygon.md
--rw-r--r--   0        0        0       69 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/api/shape_structure_dataset.md
--rw-r--r--   0        0        0       52 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/api/triangulation.md
--rw-r--r--   0        0        0       18 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/api/util.md
--rw-r--r--   0        0        0      308 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/javascripts/katex.js
--rw-r--r--   0        0        0      384 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/javascripts/mathjax.js
--rw-r--r--   0        0        0     9221 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/tutorial/blend.ipynb
--rw-r--r--   0        0        0    10269 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/tutorial/flow.ipynb
--rw-r--r--   0        0        0      794 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/tutorial/index.md
--rw-r--r--   0        0        0    10970 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/tutorial/introduction.ipynb
--rw-r--r--   0        0        0     9638 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/tutorial/polygon.ipynb
--rw-r--r--   0        0        0     3307 2024-04-13 14:04:30.000000 curvey-0.0.3/docs/tutorial/shape_structure_dataset.ipynb
--rw-r--r--   0        0        0      296 2024-04-13 14:04:30.000000 curvey-0.0.3/src/conftest.py
--rw-r--r--   0        0        0      193 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/__init__.py
--rw-r--r--   0        0        0      421 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/_typing.py
--rw-r--r--   0        0        0    11191 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/approx_medial_axis.py
--rw-r--r--   0        0        0    12306 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/blend.py
--rw-r--r--   0        0        0    54874 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/curve.py
--rw-r--r--   0        0        0    20807 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/curves.py
--rw-r--r--   0        0        0    16366 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/edges.py
--rw-r--r--   0        0        0    27476 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/flow.py
--rw-r--r--   0        0        0     7913 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/plot.py
--rw-r--r--   0        0        0    12657 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/polygon.py
--rw-r--r--   0        0        0        0 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/py.typed
--rw-r--r--   0        0        0     5136 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/shape_structure_dataset.py
--rw-r--r--   0        0        0     5651 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/triangulation.py
--rw-r--r--   0        0        0     5818 2024-04-13 14:04:30.000000 curvey-0.0.3/src/curvey/util.py
--rw-r--r--   0        0        0    28332 2024-04-13 14:04:30.000000 curvey-0.0.3/static/ama.png
--rw-r--r--   0        0        0    23917 2024-04-13 14:04:30.000000 curvey-0.0.3/static/curv_interp.png
--rw-r--r--   0        0        0    39468 2024-04-13 14:04:30.000000 curvey-0.0.3/static/curve_plot.png
--rw-r--r--   0        0        0    40234 2024-04-13 14:04:30.000000 curvey-0.0.3/static/willmore_flow.png
--rw-r--r--   0        0        0     1164 2024-04-13 14:04:30.000000 curvey-0.0.3/tests/test_blend.py
--rw-r--r--   0        0        0     6218 2024-04-13 14:04:30.000000 curvey-0.0.3/tests/test_curve.py
--rw-r--r--   0        0        0      968 2024-04-13 14:04:30.000000 curvey-0.0.3/tests/test_curves.py
--rw-r--r--   0        0        0     1211 2024-04-13 14:04:30.000000 curvey-0.0.3/tests/test_edges.py
--rw-r--r--   0        0        0     1092 2024-04-13 14:04:30.000000 curvey-0.0.3/tests/test_flow.py
--rw-r--r--   0        0        0      851 2024-04-13 14:04:30.000000 curvey-0.0.3/tests/test_shape_structure_dataset.py
--rw-r--r--   0        0        0     1352 2024-04-13 14:04:30.000000 curvey-0.0.3/tests/test_triangulation.py
--rw-r--r--   0        0        0       62 2024-04-13 14:04:30.000000 curvey-0.0.3/.gitignore
--rw-r--r--   0        0        0     7651 2024-04-13 14:04:30.000000 curvey-0.0.3/LICENSE
--rw-r--r--   0        0        0     1415 2024-04-13 14:04:30.000000 curvey-0.0.3/README.md
--rw-r--r--   0        0        0     3587 2024-04-13 14:04:30.000000 curvey-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    12447 2024-04-13 14:04:30.000000 curvey-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-04-14 14:10:31.000000 curvey-0.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      335 2024-04-14 14:10:31.000000 curvey-0.0.4/environment.yml
+-rw-r--r--   0        0        0     3197 2024-04-14 14:10:31.000000 curvey-0.0.4/mkdocs.yml
+-rw-r--r--   0        0        0       47 2024-04-14 14:10:31.000000 curvey-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      588 2024-04-14 14:10:31.000000 curvey-0.0.4/.github/workflows/release.yml
+-rw-r--r--   0        0        0      801 2024-04-14 14:10:31.000000 curvey-0.0.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1615 2024-04-14 14:10:31.000000 curvey-0.0.4/docs/bibliography.md
+-rw-r--r--   0        0        0      358 2024-04-14 14:10:31.000000 curvey-0.0.4/docs/index.md
+-rw-r--r--   0        0        0       36 2024-04-14 14:10:31.000000 curvey-0.0.4/docs/api/blend.md
+-rw-r--r--   0        0        0     3288 2024-04-14 14:10:31.000000 curvey-0.0.4/docs/api/curve.md
+-rw-r--r--   0        0        0       38 2024-04-14 14:10:31.000000 curvey-0.0.4/docs/api/curves.md
+-rw-r--r--   0        0        0       36 2024-04-14 14:10:31.000000 curvey-0.0.4/docs/api/edges.md
+-rw-r--r--   0        0        0       34 2024-04-14 14:10:31.000000 curvey-0.0.4/docs/api/flow.md
+-rw-r--r--   0        0        0      578 2024-04-14 14:10:31.000000 curvey-0.0.4/docs/api/index.md
+-rw-r--r--   0        0        0       40 2024-04-14 14:10:31.000000 curvey-0.0.4/docs/api/polygon.md
+-rw-r--r--   0        0        0       69 2024-04-14 14:10:31.000000 curvey-0.0.4/docs/api/shape_structure_dataset.md
+-rw-r--r--   0        0        0       52 2024-04-14 14:10:31.000000 curvey-0.0.4/docs/api/triangulation.md
+-rw-r--r--   0        0        0       18 2024-04-14 14:10:31.000000 curvey-0.0.4/docs/api/util.md
+-rw-r--r--   0        0        0      308 2024-04-14 14:10:31.000000 curvey-0.0.4/docs/javascripts/katex.js
+-rw-r--r--   0        0        0      384 2024-04-14 14:10:31.000000 curvey-0.0.4/docs/javascripts/mathjax.js
+-rw-r--r--   0        0        0     9221 2024-04-14 14:10:31.000000 curvey-0.0.4/docs/tutorial/blend.ipynb
+-rw-r--r--   0        0        0    10269 2024-04-14 14:10:31.000000 curvey-0.0.4/docs/tutorial/flow.ipynb
+-rw-r--r--   0        0        0      794 2024-04-14 14:10:31.000000 curvey-0.0.4/docs/tutorial/index.md
+-rw-r--r--   0        0        0    10970 2024-04-14 14:10:31.000000 curvey-0.0.4/docs/tutorial/introduction.ipynb
+-rw-r--r--   0        0        0     9638 2024-04-14 14:10:31.000000 curvey-0.0.4/docs/tutorial/polygon.ipynb
+-rw-r--r--   0        0        0     3307 2024-04-14 14:10:31.000000 curvey-0.0.4/docs/tutorial/shape_structure_dataset.ipynb
+-rw-r--r--   0        0        0      296 2024-04-14 14:10:31.000000 curvey-0.0.4/src/conftest.py
+-rw-r--r--   0        0        0      193 2024-04-14 14:10:31.000000 curvey-0.0.4/src/curvey/__init__.py
+-rw-r--r--   0        0        0      421 2024-04-14 14:10:31.000000 curvey-0.0.4/src/curvey/_typing.py
+-rw-r--r--   0        0        0    11191 2024-04-14 14:10:31.000000 curvey-0.0.4/src/curvey/approx_medial_axis.py
+-rw-r--r--   0        0        0    12306 2024-04-14 14:10:31.000000 curvey-0.0.4/src/curvey/blend.py
+-rw-r--r--   0        0        0    54874 2024-04-14 14:10:31.000000 curvey-0.0.4/src/curvey/curve.py
+-rw-r--r--   0        0        0    20807 2024-04-14 14:10:31.000000 curvey-0.0.4/src/curvey/curves.py
+-rw-r--r--   0        0        0    16484 2024-04-14 14:10:31.000000 curvey-0.0.4/src/curvey/edges.py
+-rw-r--r--   0        0        0    27476 2024-04-14 14:10:31.000000 curvey-0.0.4/src/curvey/flow.py
+-rw-r--r--   0        0        0     7913 2024-04-14 14:10:31.000000 curvey-0.0.4/src/curvey/plot.py
+-rw-r--r--   0        0        0    12721 2024-04-14 14:10:31.000000 curvey-0.0.4/src/curvey/polygon.py
+-rw-r--r--   0        0        0        0 2024-04-14 14:10:31.000000 curvey-0.0.4/src/curvey/py.typed
+-rw-r--r--   0        0        0     5136 2024-04-14 14:10:31.000000 curvey-0.0.4/src/curvey/shape_structure_dataset.py
+-rw-r--r--   0        0        0     5651 2024-04-14 14:10:31.000000 curvey-0.0.4/src/curvey/triangulation.py
+-rw-r--r--   0        0        0     5818 2024-04-14 14:10:31.000000 curvey-0.0.4/src/curvey/util.py
+-rw-r--r--   0        0        0    28332 2024-04-14 14:10:31.000000 curvey-0.0.4/static/ama.png
+-rw-r--r--   0        0        0    23917 2024-04-14 14:10:31.000000 curvey-0.0.4/static/curv_interp.png
+-rw-r--r--   0        0        0    39468 2024-04-14 14:10:31.000000 curvey-0.0.4/static/curve_plot.png
+-rw-r--r--   0        0        0    40234 2024-04-14 14:10:31.000000 curvey-0.0.4/static/willmore_flow.png
+-rw-r--r--   0        0        0     1164 2024-04-14 14:10:31.000000 curvey-0.0.4/tests/test_blend.py
+-rw-r--r--   0        0        0     6218 2024-04-14 14:10:31.000000 curvey-0.0.4/tests/test_curve.py
+-rw-r--r--   0        0        0      968 2024-04-14 14:10:31.000000 curvey-0.0.4/tests/test_curves.py
+-rw-r--r--   0        0        0     1211 2024-04-14 14:10:31.000000 curvey-0.0.4/tests/test_edges.py
+-rw-r--r--   0        0        0     1092 2024-04-14 14:10:31.000000 curvey-0.0.4/tests/test_flow.py
+-rw-r--r--   0        0        0      403 2024-04-14 14:10:31.000000 curvey-0.0.4/tests/test_medial_axis.py
+-rw-r--r--   0        0        0      851 2024-04-14 14:10:31.000000 curvey-0.0.4/tests/test_shape_structure_dataset.py
+-rw-r--r--   0        0        0     1352 2024-04-14 14:10:31.000000 curvey-0.0.4/tests/test_triangulation.py
+-rw-r--r--   0        0        0       62 2024-04-14 14:10:31.000000 curvey-0.0.4/.gitignore
+-rw-r--r--   0        0        0     7651 2024-04-14 14:10:31.000000 curvey-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1415 2024-04-14 14:10:31.000000 curvey-0.0.4/README.md
+-rw-r--r--   0        0        0     3587 2024-04-14 14:10:31.000000 curvey-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    12447 2024-04-14 14:10:31.000000 curvey-0.0.4/PKG-INFO
```

### Comparing `curvey-0.0.3/.pre-commit-config.yaml` & `curvey-0.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/mkdocs.yml` & `curvey-0.0.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/.github/workflows/release.yml` & `curvey-0.0.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/.github/workflows/test.yml` & `curvey-0.0.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/docs/bibliography.md` & `curvey-0.0.4/docs/bibliography.md`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/docs/api/curve.md` & `curvey-0.0.4/docs/api/curve.md`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/docs/api/index.md` & `curvey-0.0.4/docs/api/index.md`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/docs/tutorial/blend.ipynb` & `curvey-0.0.4/docs/tutorial/blend.ipynb`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/docs/tutorial/flow.ipynb` & `curvey-0.0.4/docs/tutorial/flow.ipynb`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/docs/tutorial/index.md` & `curvey-0.0.4/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/docs/tutorial/introduction.ipynb` & `curvey-0.0.4/docs/tutorial/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/docs/tutorial/polygon.ipynb` & `curvey-0.0.4/docs/tutorial/polygon.ipynb`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/docs/tutorial/shape_structure_dataset.ipynb` & `curvey-0.0.4/docs/tutorial/shape_structure_dataset.ipynb`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/src/curvey/approx_medial_axis.py` & `curvey-0.0.4/src/curvey/approx_medial_axis.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/src/curvey/blend.py` & `curvey-0.0.4/src/curvey/blend.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/src/curvey/curve.py` & `curvey-0.0.4/src/curvey/curve.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/src/curvey/curves.py` & `curvey-0.0.4/src/curvey/curves.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/src/curvey/edges.py` & `curvey-0.0.4/src/curvey/edges.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,15 +369,18 @@
             # Pretty sure triangle expects to be able to write into this array?
             points = self.points.copy()
         else:
             points = concatenate([self.points, interior_points])
 
         constraints = {"vertices": points, "segments": self.edges}
         if holes is not None:
-            constraints["holes"] = holes
+            holes = np.asarray(holes)
+            # triangle doesn't like empty arrays
+            if len(holes):
+                constraints["holes"] = holes
 
         d = triangle.triangulate(constraints, params)
         is_boundary = d["vertex_markers"].astype(bool).squeeze()
 
         out = Triangulation(
             points=d["vertices"],
             faces=d["triangles"],
```

### Comparing `curvey-0.0.3/src/curvey/flow.py` & `curvey-0.0.4/src/curvey/flow.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/src/curvey/plot.py` & `curvey-0.0.4/src/curvey/plot.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/src/curvey/polygon.py` & `curvey-0.0.4/src/curvey/polygon.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Protocol, cast
 
 import numpy as np
 import shapely
 from matplotlib.axes import Axes
 from matplotlib.patches import PathPatch
 from matplotlib.path import Path
-from numpy import argmax, array, ndarray, pi, stack
+from numpy import argmax, array, ndarray, pi, stack, zeros
 from typing_extensions import Self
 
 from .approx_medial_axis import ApproxMedialAxisBuilder
 from .curve import Curve
 from .edges import Edges
 from .plot import _get_ax
 from .triangulation import Triangulation
@@ -211,15 +211,18 @@
 
     @cached_property
     def hole_points(self) -> ndarray:
         """A `(len(self.interiors), 2)` array of points inside interior holes
 
         This is probably only useful for triangulation.
         """
-        return stack(list(self._iter_hole_points()), axis=0)
+        if pts := list(self._iter_hole_points()):
+            return stack(pts, axis=0)
+
+        return zeros((0, 2))
 
     @cached_property
     def boundary(self) -> Edges:
         """Boundary edges as an edge soup"""
         return Edges.concatenate(*(c.to_edges() for c in self.boundaries()))
 
     def triangulate(
```

### Comparing `curvey-0.0.3/src/curvey/shape_structure_dataset.py` & `curvey-0.0.4/src/curvey/shape_structure_dataset.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/src/curvey/triangulation.py` & `curvey-0.0.4/src/curvey/triangulation.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/src/curvey/util.py` & `curvey-0.0.4/src/curvey/util.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/static/ama.png` & `curvey-0.0.4/static/ama.png`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/static/curv_interp.png` & `curvey-0.0.4/static/curv_interp.png`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/static/curve_plot.png` & `curvey-0.0.4/static/curve_plot.png`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/static/willmore_flow.png` & `curvey-0.0.4/static/willmore_flow.png`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/tests/test_blend.py` & `curvey-0.0.4/tests/test_blend.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/tests/test_curve.py` & `curvey-0.0.4/tests/test_curve.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/tests/test_curves.py` & `curvey-0.0.4/tests/test_curves.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/tests/test_edges.py` & `curvey-0.0.4/tests/test_edges.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/tests/test_flow.py` & `curvey-0.0.4/tests/test_flow.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/tests/test_shape_structure_dataset.py` & `curvey-0.0.4/tests/test_shape_structure_dataset.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/tests/test_triangulation.py` & `curvey-0.0.4/tests/test_triangulation.py`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/LICENSE` & `curvey-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/README.md` & `curvey-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `curvey-0.0.3/pyproject.toml` & `curvey-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "curvey"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     {name = "Darik Gamble", email = "darik.gamble@gmail.com"},
 ]
 maintainers = [
     {name = "Darik Gamble", email = "darik.gamble@gmail.com"}
 ]
 description = "Pythonic geometric processing of discrete planar closed curves"
```

### Comparing `curvey-0.0.3/PKG-INFO` & `curvey-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: curvey
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pythonic geometric processing of discrete planar closed curves
 Project-URL: Homepage, https://github.com/darikg/curvey/
 Project-URL: Documentation, https://darikg.github.io/curvey/
 Project-URL: Source Code, https://github.com/darikg/curvey/
 Author-email: Darik Gamble <darik.gamble@gmail.com>
 Maintainer-email: Darik Gamble <darik.gamble@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
```

