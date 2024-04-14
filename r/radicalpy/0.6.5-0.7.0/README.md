# Comparing `tmp/radicalpy-0.6.5.tar.gz` & `tmp/radicalpy-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radicalpy-0.6.5.tar", last modified: Thu Aug  3 09:33:38 2023, max compression
+gzip compressed data, was "radicalpy-0.7.0.tar", last modified: Sun Apr 14 12:45:24 2024, max compression
```

## Comparing `radicalpy-0.6.5.tar` & `radicalpy-0.7.0.tar`

### file list

```diff
@@ -1,40 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 09:33:38.497286 radicalpy-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-08-03 09:33:28.000000 radicalpy-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-08-03 09:33:38.497286 radicalpy-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-08-03 09:33:28.000000 radicalpy-0.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1256 2023-08-03 09:33:28.000000 radicalpy-0.6.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 09:33:38.493286 radicalpy-0.6.5/radicalpy/
--rw-r--r--   0 runner    (1001) docker     (122)      311 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7266 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/classical.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 09:33:38.493286 radicalpy-0.6.5/radicalpy/data/
--rw-r--r--   0 runner    (1001) docker     (122)     2498 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/data/constants.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 09:33:38.497286 radicalpy-0.6.5/radicalpy/data/molecules/
--rw-r--r--   0 runner    (1001) docker     (122)      471 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/data/molecules/2_6_aqds.json
--rw-r--r--   0 runner    (1001) docker     (122)      405 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/data/molecules/adenine_cation.json
--rw-r--r--   0 runner    (1001) docker     (122)     6719 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/data/molecules/flavin_anion.json
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/data/molecules/flavin_neutral.json
--rw-r--r--   0 runner    (1001) docker     (122)     3297 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/data/molecules/tryptophan_cation.json
--rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/data/molecules/tyrosine_neutral.json
--rw-r--r--   0 runner    (1001) docker     (122)    27847 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/data/spin_data.json
--rw-r--r--   0 runner    (1001) docker     (122)    16112 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    20384 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/estimations.py
--rw-r--r--   0 runner    (1001) docker     (122)     5054 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/kinetics.py
--rw-r--r--   0 runner    (1001) docker     (122)     6365 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     9706 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/relaxation.py
--rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/shared.py
--rw-r--r--   0 runner    (1001) docker     (122)    37681 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)    11420 2023-08-03 09:33:28.000000 radicalpy-0.6.5/radicalpy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 09:33:38.493286 radicalpy-0.6.5/radicalpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2023-08-03 09:33:38.000000 radicalpy-0.6.5/radicalpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      872 2023-08-03 09:33:38.000000 radicalpy-0.6.5/radicalpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 09:33:38.000000 radicalpy-0.6.5/radicalpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-08-03 09:33:38.000000 radicalpy-0.6.5/radicalpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-08-03 09:33:38.000000 radicalpy-0.6.5/radicalpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       89 2023-08-03 09:33:28.000000 radicalpy-0.6.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-03 09:33:38.497286 radicalpy-0.6.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 09:33:38.497286 radicalpy-0.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     3157 2023-08-03 09:33:28.000000 radicalpy-0.6.5/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     3948 2023-08-03 09:33:28.000000 radicalpy-0.6.5/tests/test_estimations.py
--rw-r--r--   0 runner    (1001) docker     (122)      325 2023-08-03 09:33:28.000000 radicalpy-0.6.5/tests/test_relaxations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1684 2023-08-03 09:33:28.000000 radicalpy-0.6.5/tests/test_shared.py
--rw-r--r--   0 runner    (1001) docker     (122)    19571 2023-08-03 09:33:28.000000 radicalpy-0.6.5/tests/test_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:45:24.296968 radicalpy-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-14 12:45:19.000000 radicalpy-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-14 12:45:24.296968 radicalpy-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-14 12:45:19.000000 radicalpy-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-14 12:45:19.000000 radicalpy-0.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:45:24.296968 radicalpy-0.7.0/radicalpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/classical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20549 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:45:24.296968 radicalpy-0.7.0/radicalpy/data_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/data_files/constants.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:45:24.296968 radicalpy-0.7.0/radicalpy/data_files/molecules/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/data_files/molecules/2_6_aqds.json
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/data_files/molecules/adenine_cation.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/data_files/molecules/fad.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/data_files/molecules/flavin_anion.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/data_files/molecules/flavin_neutral.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3297 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/data_files/molecules/tryptophan_cation.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/data_files/molecules/tyrosine_neutral.json
+-rw-r--r--   0 runner    (1001) docker     (127)    27847 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/data_files/spin_data.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23002 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/estimations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6242 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/kinetics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9475 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9707 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/relaxation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41184 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-04-14 12:45:19.000000 radicalpy-0.7.0/radicalpy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:45:24.296968 radicalpy-0.7.0/radicalpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-14 12:45:24.000000 radicalpy-0.7.0/radicalpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-14 12:45:24.000000 radicalpy-0.7.0/radicalpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 12:45:24.000000 radicalpy-0.7.0/radicalpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-14 12:45:24.000000 radicalpy-0.7.0/radicalpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-14 12:45:24.000000 radicalpy-0.7.0/radicalpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-14 12:45:19.000000 radicalpy-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 12:45:24.296968 radicalpy-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 12:45:24.296968 radicalpy-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-14 12:45:19.000000 radicalpy-0.7.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-14 12:45:19.000000 radicalpy-0.7.0/tests/test_estimations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-14 12:45:19.000000 radicalpy-0.7.0/tests/test_relaxations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-14 12:45:19.000000 radicalpy-0.7.0/tests/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21203 2024-04-14 12:45:19.000000 radicalpy-0.7.0/tests/test_simulation.py
```

### Comparing `radicalpy-0.6.5/LICENSE` & `radicalpy-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.5/README.md` & `radicalpy-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.5/pyproject.toml` & `radicalpy-0.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -27,22 +27,27 @@
 enabled = true
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [tool.setuptools.package-data]
 "*" = ["*.json"]
-
-[tool.black]
-line-length = 88
+["py.typed"]
 
 [tool.pydocstyle]
 convention = "google"
 
+[tool.black]
+line-length = 88
+
 [tool.pylint]
 max-line-length = 88
 disable = ["C0103"]
 
+[tool.isort]
+line_length = 88
+profile = "black"
+
 [tool.mypy]
 plugins = ["numpy.typing.mypy_plugin"]
 disallow_untyped_defs = true
 disallow_untyped_calls = true
```

### Comparing `radicalpy-0.6.5/radicalpy/classical.py` & `radicalpy-0.7.0/radicalpy/classical.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 #!/usr/bin/env python
 
 
+from pathlib import Path
 from typing import Tuple
 
+import dot2tex
 import graphviz
 import numpy as np
 import scipy as sp
+from numpy.typing import ArrayLike
 
 from . import utils
 
 
 def get_delta_r(mutual_diffusion: float, delta_T: float) -> float:
     """Mean path between two radicals.
 
@@ -61,76 +64,94 @@
         return (v.value, v.label) if isinstance(v, Rate) else (v, v)
 
     def __rmul__(self, v):
         value, label = self._get_value_label(v)
         return Rate(self.value * value, f"{label} {self.label}")
 
     def __mul__(self, v):
+        # When multiplying with a constant, this puts the constant
+        # before the variable.
         return self.__rmul__(v)
 
     def __radd__(self, v):
         value, label = self._get_value_label(v)
-        return Rate(self.value + value, f"{label} + {self.label}")
+        return Rate(value + self.value, f"{label} + {self.label}")
 
     def __add__(self, v):
         value, label = self._get_value_label(v)
         return Rate(self.value + value, f"{self.label} + {label}")
 
     def __neg__(self):
         return Rate(-self.value, f"-({self.label})")
 
+    def __truediv__(self, v):
+        value, label = self._get_value_label(v)
+        return Rate(self.value / value, f"{self.label} / {label}")
+
+
+class EquationRateResult:
+    def __init__(self, result: np.ndarray, indices: dict):
+        self.result = result
+        self.indices = indices
+
+    def __getitem__(self, keys: list) -> np.ndarray:
+        ks = [keys] if isinstance(keys, str) else keys
+        return np.sum([self.result[:, self.indices[k]] for k in ks], axis=0)
+
 
 class RateEquations:
     """Results for `kinetics_solver`"""
 
-    def __init__(self, rate_equations: dict, time: np.ndarray, initial_states: dict):
+    def __init__(self, rate_equations: dict):
         self.rate_equations = rate_equations
         inner_keys = [list(v.keys()) for v in rate_equations.values()]
         outer_keys = list(rate_equations.keys())
-        all_keys = list(set(sum(inner_keys, outer_keys)))
-        self.indices = {k: i for i, k in enumerate(all_keys)}
-        self._calc_(time, initial_states)
+        if set(outer_keys) != set(sum(inner_keys, [])):
+            print("WARNING:The set of sources and sinks is different!")
+        # all_keys = list(set(sum(inner_keys, outer_keys)))
+        self.indices = {k: i for i, k in enumerate(outer_keys)}
+        self._construct_matrix()
 
     @property
     def all_keys(self) -> list:
         return list(self.indices.keys())
 
     def are_valid_keys(self, keys: dict) -> bool:
         return set(keys).issubset(self.all_keys)
 
-    def check_initial_states(self, initial_states):
+    def check_initial_states(self, initial_states: dict):
         if not self.are_valid_keys(initial_states.keys()):
             raise ValueError("Unknown keys specified in `initial_states`")
         if sum(initial_states.values()) != 1:
-            raise ValueError("Initial state values don't sum up to 1")
+            print("WARNING: Initial state values don't sum up to 1")
 
-    def _calc_(self, time: np.ndarray, initial_states: dict):
-        self.check_initial_states(initial_states)
+    def _construct_matrix(self):
         tmp = [
             (v.value, self.indices[i], self.indices[j])
             for i, d in self.rate_equations.items()
             for j, v in d.items()
         ]
-        dt = time[1] - time[0]
         data, row_ind, col_ind = zip(*tmp)
         N = len(self.all_keys)
-        propagator = sp.sparse.linalg.expm(
-            sp.sparse.csc_matrix((data, (row_ind, col_ind)), (N, N)) * dt
-        )
-        self.result = np.zeros([len(time), len(self.all_keys)], dtype=float)
-        self.result[0] = [initial_states.get(k, 0) for k in self.all_keys]
-        for t in range(1, len(time)):
-            self.result[t] = propagator @ self.result[t - 1]
+        self.matrix = sp.sparse.csc_matrix((data, (row_ind, col_ind)), (N, N))
 
-    def __getitem__(self, keys: list) -> np.ndarray:
-        ks = [keys] if isinstance(keys, str) else keys
-        return np.sum([self.result[:, self.indices[k]] for k in ks], axis=0)
+    def time_evolution(
+        self, time: np.ndarray, initial_states: dict
+    ) -> EquationRateResult:
+        self.check_initial_states(initial_states)
+        dt = time[1] - time[0]
+        propagator = sp.sparse.linalg.expm(self.matrix * dt)
+        result = np.zeros([len(time), len(self.all_keys)], dtype=float)
+        result[0] = [initial_states.get(k, 0) for k in self.all_keys]
+        for t in range(1, len(time)):
+            result[t] = propagator @ result[t - 1]
+        return EquationRateResult(result, self.indices)
 
 
-def reaction_scheme(rate_equations: dict):
+def reaction_scheme(path: str, rate_equations: dict):
     data = [
         (v1, v2, edge.label)
         for v1, rhs_data in rate_equations.items()
         for v2, edge in rhs_data.items()
     ]
     G = graphviz.Digraph("G")
     for v1, v2, edge in data:
@@ -138,29 +159,34 @@
             # TODO: add only if not present already
             # TODO: check position
             # TODO: use sympy (how to check negative)
             G.node(v1, texlbl=f"${v1}$")
             G.node(v2, texlbl=f"${v2}$")
             G.edge(v2, v1, edge, texlbl=f"${edge}$")
 
-    path = Path(f"{__file__[:-3]}_graph.tex")
+    if not path.endswith("tex"):
+        path += ".tex"
     texcode = dot2tex.dot2tex(G.source)
-    path.write_text(texcode)
+    Path(path).write_text(texcode)
 
 
-def _random_theta_phi():
+def random_theta_phi(n: int = 1) -> ArrayLike:
     """Random sampling of theta and phi.
 
+    Args:
+
+            n_samples (int): The number of samples generated.
+
     Returns:
             Theta and phi (radians).
+
     """
-    theta = np.pi * np.random.rand()
-    arg = np.random.uniform(-1, 1)
-    phi = 2 * np.sign(arg) * np.arcsin(np.sqrt(np.abs(arg)))
-    return theta, phi
+    phi = np.random.uniform(0, 2 * np.pi, size=n)
+    theta = np.arccos(np.random.uniform(-1, 1, size=n))
+    return np.array([theta, phi])
 
 
 def randomwalk_3d(
     n_steps: int,
     x_0: float,
     y_0: float,
     z_0: float,
@@ -210,18 +236,18 @@
 
     pos[0] = np.array([x_0, y_0, z_0])
     dist[0] = np.linalg.norm(pos[0])
     if np.linalg.norm(pos[0]) <= r_min:
         raise ValueError("Molecule starting distance is needs to be > r_min.")
 
     for i in range(1, n_steps):
-        theta, phi = _random_theta_phi()
+        theta, phi = random_theta_phi()
         new_pos = pos[i - 1] + delta_r * utils.spherical_to_cartesian(theta, phi)
         d = np.linalg.norm(new_pos)
         while (r_max > 0 and d >= r_max - r_min) or d <= r_min + r_min:
-            theta, phi = _random_theta_phi()
+            theta, phi = random_theta_phi()
             new_pos = pos[i - 1] + delta_r * utils.spherical_to_cartesian(theta, phi)
             d = np.linalg.norm(new_pos)
         angle[i] = theta
         pos[i] = new_pos
         dist[i] = d
     return pos, dist, angle
```

### Comparing `radicalpy-0.6.5/radicalpy/data/constants.json` & `radicalpy-0.7.0/radicalpy/data_files/constants.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.5/radicalpy/data/molecules/flavin_anion.json` & `radicalpy-0.7.0/radicalpy/data_files/molecules/flavin_anion.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.5/radicalpy/data/molecules/flavin_neutral.json` & `radicalpy-0.7.0/radicalpy/data_files/molecules/flavin_neutral.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.5/radicalpy/data/molecules/tryptophan_cation.json` & `radicalpy-0.7.0/radicalpy/data_files/molecules/tryptophan_cation.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.5/radicalpy/data/molecules/tyrosine_neutral.json` & `radicalpy-0.7.0/radicalpy/data_files/molecules/tyrosine_neutral.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.5/radicalpy/data/spin_data.json` & `radicalpy-0.7.0/radicalpy/data_files/spin_data.json`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.5/radicalpy/data.py` & `radicalpy-0.7.0/radicalpy/data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! /usr/bin/env python
 import json
 from functools import singledispatchmethod
-from typing import Optional
+from typing import Iterator, Optional, Tuple
 
 import numpy as np
 from importlib_resources import files
 from importlib_resources.abc import Traversable
 from numpy.typing import NDArray
 
 
@@ -35,15 +35,15 @@
 
     """
     return float(multiplicity - 1) / 2.0
 
 
 def get_data(suffix: str = "") -> Traversable:
     """Get the directory containing data files."""
-    return files(__package__) / "data" / suffix
+    return files(__package__) / "data_files" / suffix
 
 
 class Isotope:
     """Class representing an isotope.
 
     Args:
         symbol (str): The symbol/identifier of the isotope in the
@@ -196,25 +196,29 @@
     _anisotropic: Optional[NDArray]
     _isotropic: float
 
     def __repr__(self) -> str:  # noqa D105
         available = "not " if self._anisotropic is None else ""
         return f"{self.isotropic:.4} <anisotropic {available}available>"
 
+    # `singledispatchmethod` and `__init__.register` is used to have
+    # one `__init__` function with two implementations BASED ON THE
+    # ARGUMENT TYPE!
     @singledispatchmethod
     def __init__(self, hfc: list[list[float]]):  # noqa D105
         self._anisotropic = np.array(hfc)
         if self._anisotropic.shape != (3, 3):
             lines = [
                 "Anisotropic HFCs should be a float or a 3x3 matrix!",
                 f"Got: {hfc}",
             ]
             raise ValueError("\n".join(lines))
         self._isotropic = self._anisotropic.trace() / 3
 
+    # See the comment above the `singledispatchmethod` decorator.
     @__init__.register
     def _(self, hfc: float):  # noqa D105
         self._anisotropic = None
         self._isotropic = hfc
 
     @property
     def anisotropic(self) -> NDArray:
@@ -302,31 +306,42 @@
         return nucleus
 
     @property
     def gamma_mT(self):
         """Return magnetogyric ratio, :math:`\gamma` (rad/s/mT)."""
         return self.magnetogyric_ratio * 0.001
 
+    @property
+    def spin_quantum_number(self) -> float:
+        """Spin quantum numer of `Isotope`."""
+        return multiplicity_to_spin(self.multiplicity)
+
 
 class Molecule:
     """Representation of a molecule for the simulation.
 
     A molecule is described by a name and a list of nuclei (see
     `Nucleus`).  Using the default constructor is **cumbersome and not
     recommended**.  The preferred way is to use the following
     convenience methods (click on the method name to see its
     documentation):
 
     - `Molecule.fromdb`
     - `Molecule.fromisotopes`
 
     Args:
+
         name (str): The name of the `Molecule`.
+
         nuclei (list[Nucleus]): List of nuclei/atoms which should be
             simulated (see `Nucleus`).
+
+        radical (Nucleus): The radical of the molecule. (Default
+            `Nucleus.fromisotope("E", 0.0)`).
+
         info (dict[str, str]): Dictionary of miscellaneous information
             about the molecule.
 
     Examples:
         The default constructor takes an arbitrary name and a list of
         molecules to construct a molecule.
 
@@ -334,61 +349,73 @@
         >>> gamma_14N = 19337.792
         >>> Molecule("kryptonite", [Nucleus(gamma_1H, 2, Hfc(1.0), "Hydrogen"),
         ...                            Nucleus(gamma_14N, 3, Hfc(-0.5), "Nitrogen")])
         Molecule: kryptonite
         Nuclei:
           Hydrogen(267522186.99999997, 2, 1.0 <anisotropic not available>)
           Nitrogen(19337792.0, 3, -0.5 <anisotropic not available>)
+        Radical: E(-176085963023.0, 2, 0.0 <anisotropic not available>)
 
         Or alternatively:
 
         >>> gammas = [267522.187, 19337.792]
         >>> multis = [2, 3]
         >>> hfcs = [1.0, -0.5]
         >>> names = ["Hydrogen", "Nitrogen"]
         >>> params = zip(gammas, multis, map(Hfc, hfcs), names)
         >>> Molecule("kryptonite", [Nucleus(*param) for param in params])
         Molecule: kryptonite
         Nuclei:
           Hydrogen(267522186.99999997, 2, 1.0 <anisotropic not available>)
           Nitrogen(19337792.0, 3, -0.5 <anisotropic not available>)
+        Radical: E(-176085963023.0, 2, 0.0 <anisotropic not available>)
+
     """
 
     name: str
     nuclei: list[Nucleus]
     info: dict[str, str]
+    radical: Nucleus
     custom: bool
 
     def __repr__(self) -> str:
         """Pretty print the molecule.
 
         Returns:
             str: Representation of a molecule.
         """
         nuclei = "\n".join([f"  {n}" for n in self.nuclei])
         lines = [
             f"Molecule: {self.name}",
             f"Nuclei:\n{nuclei}" if self.nuclei else "No nuclei specified.",
+            f"Radical: {self.radical}",
             # f"\n  Number of particles: {self.num_particles}"
         ]
         if self.info:
             lines.append(f"Info: {self.info}")
         return "\n".join(lines)
 
     def __init__(
-        self, name: str = "", nuclei: list[Nucleus] = [], info: dict[str, str] = {}
+        self,
+        name: str = "",
+        nuclei: list[Nucleus] = [],
+        radical: Nucleus = Nucleus.fromisotope("E", 0.0),
+        info: dict[str, str] = {},
     ):
         """Default constructor."""
         # todo(vatai): check types?
         self.name = name
         self.nuclei = nuclei  # list[gamma, multi, hfc]
         self.info = info
-        self.radical = Nucleus.fromisotope("E", 0.0)
+        self.radical = radical
         self.custom = True
 
+        self.hfc_rng = np.random.default_rng(42)  ##################
+        self.ang_rng = np.random.default_rng(43)  ##################
+
     @classmethod
     def load_molecule_json(cls, molecule: str) -> dict:
         json_path = get_data(f"molecules/{molecule}.json")
         with open(json_path, encoding="utf-8") as f:
             data = json.load(f)
         return data
 
@@ -398,41 +425,90 @@
 
         Returns:
             list[str]: List of available molecules (names).
 
         Examples:
             >>> available = Molecule.available()
             >>> available[:4]
-            ['2_6_aqds', 'adenine_cation', 'flavin_anion', 'flavin_neutral']
+            ['2_6_aqds', 'adenine_cation', 'fad', 'flavin_anion']
         """
         paths = get_data("molecules").glob("*.json")
         return sorted([path.with_suffix("").name for path in paths])
 
     @classmethod
+    def _check_molecule_available(cls, name):
+        if name not in cls.available():
+            lines = [f"Molecule `{name}` not found in database."]
+            lines += ["Available molecules:"]
+            lines += cls.available()
+            raise ValueError("\n".join(lines))
+
+    @classmethod
+    def all_nuclei(cls, name: str):
+        """Construct a molecule from the database with all nuclei.
+
+        Args:
+            name (str): A name of the molecule available in the
+                database (see `Molecule.available()`).
+
+        Examples:
+            >>> Molecule.all_nuclei("flavin_anion")
+            Molecule: flavin_anion
+            Nuclei:
+              14N(19337792.0, 3, 0.5141 <anisotropic available>)
+              14N(19337792.0, 3, -0.001275 <anisotropic available>)
+              14N(19337792.0, 3, -0.03654 <anisotropic available>)
+              1H(267522187.44, 2, 0.05075 <anisotropic available>)
+              1H(267522187.44, 2, -0.1371 <anisotropic available>)
+              1H(267522187.44, 2, -0.1371 <anisotropic available>)
+              1H(267522187.44, 2, -0.1371 <anisotropic available>)
+              1H(267522187.44, 2, -0.4403 <anisotropic available>)
+              1H(267522187.44, 2, 0.4546 <anisotropic available>)
+              1H(267522187.44, 2, 0.4546 <anisotropic available>)
+              1H(267522187.44, 2, 0.4546 <anisotropic available>)
+              1H(267522187.44, 2, 0.009597 <anisotropic available>)
+              1H(267522187.44, 2, 0.4263 <anisotropic available>)
+              1H(267522187.44, 2, 0.4233 <anisotropic available>)
+              1H(267522187.44, 2, -0.02004 <anisotropic available>)
+              14N(19337792.0, 3, 0.1784 <anisotropic available>)
+            Radical: E(-176085963023.0, 2, 0.0 <anisotropic not available>)
+            Info: {'units': 'mT', 'name': 'Flavin radical anion'}
+        """
+        cls._check_molecule_available(name)
+        molecule_json = cls.load_molecule_json(name)
+        info = molecule_json["info"]
+        data = molecule_json["data"]
+        nuclei_list = []
+        for nucleus in data.keys():
+            isotope = data[nucleus]["element"]
+            hfc = data[nucleus]["hfc"]
+            nuclei_list.append(Nucleus.fromisotope(isotope, hfc))
+        molecule = cls(name=name, nuclei=nuclei_list, info=info)
+        molecule.custom = False
+        return molecule
+
+    @classmethod
     def fromdb(cls, name: str, nuclei: list[str] = []):
         """Construct a molecule from the database.
 
         Args:
             name (str): A name of the molecule available in the
                 database (see `Molecule.available()`).
             nuclei (list[str]): A list of nuclei names found in the
                 molecule specified by `name`.
 
         Examples:
             >>> Molecule.fromdb("flavin_anion", nuclei=["N14"])
             Molecule: flavin_anion
             Nuclei:
               14N(19337792.0, 3, -0.001275 <anisotropic available>)
+            Radical: E(-176085963023.0, 2, 0.0 <anisotropic not available>)
             Info: {'units': 'mT', 'name': 'Flavin radical anion'}
         """
-        if name not in cls.available():
-            lines = [f"Molecule `{name}` not found in database."]
-            lines += ["Available molecules:"]
-            lines += cls.available()
-            raise ValueError("\n".join(lines))
+        cls._check_molecule_available(name)
         molecule_json = cls.load_molecule_json(name)
         info = molecule_json["info"]
         data = molecule_json["data"]
         keys = list(data.keys())
         nuclei_list = []
         for nucleus in nuclei:
             if nucleus not in keys:
@@ -443,15 +519,15 @@
                 )
                 lines = ["Available nuclei:"]
                 lines += [f"{n} (hfc = {h})" for n, h in nuclei_hfcs]
                 raise ValueError("\n".join(lines))
             isotope = data[nucleus]["element"]
             hfc = data[nucleus]["hfc"]
             nuclei_list.append(Nucleus.fromisotope(isotope, hfc))
-        molecule = cls(name, nuclei_list, info)
+        molecule = cls(name=name, nuclei=nuclei_list, info=info)
         molecule.custom = False
         return molecule
 
     @classmethod
     def fromisotopes(cls, isotopes: list[str], hfcs: list, name: str = ""):
         """Construct molecule from isotopes.
 
@@ -465,14 +541,15 @@
             >>> Molecule.fromisotopes(isotopes=["1H", "14N"],
             ...                          hfcs=[1.5, 0.9],
             ...                          name="kryptonite")
             Molecule: kryptonite
             Nuclei:
               1H(267522187.44, 2, 1.5 <anisotropic not available>)
               14N(19337792.0, 3, 0.9 <anisotropic not available>)
+            Radical: E(-176085963023.0, 2, 0.0 <anisotropic not available>)
         """
         isos = []
         for iso in isotopes:
             if iso not in Isotope.available():
                 raise ValueError(
                     f"Isotope {iso} not in database! See `Isotope.available()`"
                 )
@@ -494,7 +571,45 @@
             multiplicities = [Isotope(e).multiplicity for e in elem]
             hfcs = [Hfc(data[n]["hfc"]) for n in nuclei]
 
         # spin quantum number
         spns_np = np.array(list(map(multiplicity_to_spin, multiplicities)))
         hfcs_np = np.array([h.isotropic for h in hfcs])
         return np.sqrt((4 / 3) * sum((hfcs_np**2 * spns_np) * (spns_np + 1)))
+
+    @property  ############ TODO(calc only once)
+    def semiclassical_std(self) -> float:
+        r"""The standard deviation for the semiclassical HFCs.
+
+        Calculate the standard deviation :math:`\sigma` where
+
+        .. math::
+           \sigma = \sqrt{\frac{2}{\tau^2}}
+
+        and
+
+        .. math::
+           \tau_i^{-2} = \frac{1}{6} \sum_k a_k^2 I_k (I_k + 1)
+
+        where :math:`a_k` is the hyperfine coupling and :math:`I_k`
+        the spin quantum number of each nucleus, respectively.
+
+        Examples:
+            >>> m = Molecule.fromdb("flavin_anion", nuclei=["N14"])
+            >>> m.semiclassical_std
+            7.663920853309001e-07
+
+        .. todo::
+           reference
+        """
+        tau = 6 / sum(
+            n.spin_quantum_number * (n.spin_quantum_number + 1) * n.hfc.isotropic**2
+            for n in self.nuclei
+        )
+        return np.sqrt(2) / tau
+
+
+class Triplet(Molecule):
+    def __init__(self):
+        gamma = Isotope("E").gamma_mT
+        triplet = Nucleus(magnetogyric_ratio=gamma, multiplicity=3, hfc=0.0)
+        super().__init__(name="Triplet", nuclei=[], radical=triplet)
```

### Comparing `radicalpy-0.6.5/radicalpy/estimations.py` & `radicalpy-0.7.0/radicalpy/estimations.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 from . import utils
 from .data import Isotope
 from .shared import constants as C
 from .simulation import HilbertSimulation
 from .utils import autocorrelation, mT_to_MHz
 
 
-def Bhalf_theoretical(sim: HilbertSimulation) -> float:
-    """Theoretical B1/2 for radical pairs in solution.
+def Bhalf_theoretical_hyperfine(sim: HilbertSimulation) -> float:
+    """Theoretical B1/2 for radical pairs.
+    Estimated with hyperfine interactions.
 
     Source: `Weller et al. Chem. Phys. Lett. 96, 1, 24-27 (1983)`_.
 
     Args:
             sim: The `sim` object containing the hyperfine coupling
                 constants. It should contain exactly two molecules.
 
@@ -28,14 +29,56 @@
     """
     assert len(sim.molecules) == 2
     sum_hfc2 = sum(m.effective_hyperfine**2 for m in sim.molecules)
     sum_hfc = sum(m.effective_hyperfine for m in sim.molecules)
     return np.sqrt(3) * (sum_hfc2 / sum_hfc)
 
 
+def Bhalf_theoretical_relaxation(kstd: float, krec: float) -> float:
+    """Theoretical B1/2 for radical pairs.
+    Estimated with spin dephasing rate.
+
+    Source: `Golesworthy et al. J. Chem. Phys. 159, 105102 (2023)`_.
+
+    Args:
+            kstd (float): Singlet-triplet dephasing rate (1/s).
+            krec (float): Recombination rate (1/s).
+
+    Returns:
+            float: The B1/2 value (mT).
+
+    .. _Golesworthy et al. J. Chem. Phys. 159, 105102 (2023):
+       https://doi.org/10.1063/5.0166675
+    """
+    return 2.5 + 0.37 * (kstd / krec) ** 0.66
+
+
+def Bhalf_theoretical_relaxation_delay(
+    kstd: float, krec: float, td: float | np.ndarray
+) -> float:
+    """Theoretical B1/2 for radical pairs.
+    Estimated with spin dephasing rate and pump-probe delay time.
+
+    Source: `Golesworthy et al. J. Chem. Phys. 159, 105102 (2023)`_.
+
+    Args:
+            kstd (float): Singlet-triplet dephasing rate (1/s).
+            krec (float): Recombination rate (1/s).
+            td (float or np.ndarray): Pump-probe delay (s).
+
+    Returns:
+            float: The B1/2 value (mT).
+
+    .. _Golesworthy et al. J. Chem. Phys. 159, 105102 (2023):
+       https://doi.org/10.1063/5.0166675
+    """
+    bhalf = Bhalf_theoretical_relaxation(kstd, krec)
+    return (2.5 - bhalf) * np.exp(-(krec * td)) + bhalf
+
+
 def _relaxation_gtensor_term(g: list) -> float:
     return sum((gi - np.mean(g)) ** 2 for gi in g)
 
 
 def T1_relaxation_rate(
     g_tensors: list, B: float | np.ndarray, tau_c: float | np.ndarray
 ) -> float | np.ndarray:
@@ -196,15 +239,15 @@
         multiexponential,
         ts,
         acf,
         bounds=(0, float("inf")),
         p0=np.zeros(num_exp),
     )
     fit = multiexponential(ts, *acf_popt)
-    tau_c = sum(acf_popt * taus) * np.var(mT_to_MHz(trajectory)) / 1e6
+    tau_c = sum(acf_popt * taus)  # * np.var(mT_to_MHz(trajectory)) / 1e6
     return {"fit": fit, "tau_c": tau_c}
 
 
 def diffusion_coefficient(radius: float, temperature: float, eta: float):
     """Diffusion coefficient.
 
     The Stokes-Einstein relation.
@@ -483,18 +526,22 @@
     return 10 ** (
         13
         - 0.6 * (separation - 3.6)
         - 3.1 * ((driving_force + reorganisation_energy) ** 2 / reorganisation_energy)
     )
 
 
-def k_excitation(
-    power: float, wavelength: float, volume: float, pathlength: float, epsilon: float
+def k_excitation_extinction_coefficient(
+    power: float,
+    wavelength: float,
+    volume: float,
+    pathlength: float,
+    epsilon: float,
 ) -> float:
-    """Groundstate excitation rate.
+    """Groundstate excitation rate using extinction coefficient.
 
     Args:
             power (float): The excitation laser power (W).
             wavelength (float): The excitation wavelength (m).
             volume (float): The excitation beam volume (m^3).
             pathlength (float): The path length of the sample cell
                 (m).
@@ -505,14 +552,46 @@
             float: The excitation rate (1/s).
     """
     nu = C.c / wavelength  # Frequency of excitation beam (1/s)
     I0 = power / (C.h * nu * C.N_A * volume)  # Initial intensity (I0)
     return I0 * np.log(10) * epsilon * pathlength
 
 
+def k_excitation_photon_flux(
+    power: float,
+    wavelength: float,
+    beam_radius: float,
+    pathlength: float,
+    absorbance: float,
+    concentration: float,
+) -> float:
+    """Groundstate excitation rate using photon flux.
+
+    Args:
+            power (float): The excitation laser power (W).
+            wavelength (float): The excitation wavelength (m).
+            beam_radius (float): Radius of the beam spot (m).
+            pathlength (float): The path length of the sample cell
+                (m).
+            absorbance (float): Absorbance of the sample (OD).
+            concentration (float): Concentration of the sample (mol/m^3).
+
+    Returns:
+            float: The excitation rate (1/s).
+    """
+    photon_energy = (C.h * C.c) / wavelength  # energy of one photon (J)
+    beam_spot_area = np.pi * beam_radius**2  # beam spot area (m^2)
+    number_density = concentration * C.N_A  # number density of the sample (m^-3)
+    absorbance_cross_section = absorbance / (
+        number_density * pathlength
+    )  # absorbance cross section (m^2)
+    photon_flux = power / (beam_spot_area * photon_energy)  # photon flux (m^2 / s)
+    return photon_flux * absorbance_cross_section
+
+
 def k_recombination(MFE: float, k_escape: float) -> float:
     """Singlet recombination rate.
 
     Source: `Maeda et al. Mol. Phys., 117:19, 2709-2718 (2019)`_.
 
     Args:
             MFE (float): The magnetic field effect (0.00-1.00).
@@ -564,16 +643,15 @@
 
     .. _Atkins et al. Mol. Phys., 27, 6 (1974):
        https://doi.org/10.1080/00268977400101361
     """
     B0 = utils.mT_to_MHz(B0)
     nu_0 = (C.g_e * (C.mu_B * 1e-3) * B0) / C.h
     jnu0tc = (2 / 15) * (
-        (4 * tau_c) / (1 + 4 * nu_0**2 * tau_c**2)
-        + (tau_c) / (1 + nu_0**2 * tau_c**2)
+        (4 * tau_c) / (1 + 4 * nu_0**2 * tau_c**2) + (tau_c) / (1 + nu_0**2 * tau_c**2)
     )
     return (D**2 + 3 * E**2) * jnu0tc
 
 
 def rotational_correlation_time_for_molecule(
     radius: float, temp: float, eta: float = 0.89e-3
 ) -> float:
```

### Comparing `radicalpy-0.6.5/radicalpy/kinetics.py` & `radicalpy-0.7.0/radicalpy/kinetics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from math import prod
+"""Kinetics classes."""
 
 import numpy as np
 
 from .simulation import (
     HilbertIncoherentProcessBase,
     LiouvilleIncoherentProcessBase,
     LiouvilleSimulation,
@@ -21,18 +21,14 @@
 class LiouvilleKineticsBase(LiouvilleIncoherentProcessBase):
     """Base class for kinetics superoperators (Liouville space)."""
 
     def _name(self):
         name = super()._name()
         return f"Kinetics: {name}"
 
-    @staticmethod
-    def _convert(Q: np.ndarray) -> np.ndarray:
-        return np.kron(Q, np.eye(len(Q))) + np.kron(np.eye(len(Q)), Q)
-
 
 class Exponential(HilbertKineticsBase):
     """Exponential model kinetics operator.
 
     Source: `Kaptein et al. Chem. Phys. Lett. 4, 4, 195-197 (1969)`_.
 
     >>> Exponential(rate_constant=1e6)
@@ -75,23 +71,31 @@
     .. _Haberkorn, Mol. Phys. 32:5, 1491-1493 (1976):
        http://dx.doi.org/10.1080/00268977600102851
     """
 
     def __init__(self, rate_constant: float, target: State):
         super().__init__(rate_constant)
         self.target = target
-        if target not in {State.SINGLET, State.TRIPLET}:
+        if target not in {
+            State.SINGLET,
+            State.TP_SINGLET,
+            State.TRIPLET,
+            State.TRIPLET_MINUS,
+            State.TRIPLET_PLUS,
+            State.TRIPLET_PLUS_MINUS,
+            State.TRIPLET_ZERO,
+        }:
             raise ValueError(
                 "Haberkorn kinetics supports only SINGLET and TRIPLET targets"
             )
 
     def init(self, sim: LiouvilleSimulation):
         """See `radicalpy.simulation.HilbertIncoherentProcessBase.init`."""
         Q = sim.projection_operator(self.target)
-        self.subH = 0.5 * self.rate * self._convert(Q)
+        self.subH = 0.5 * self.rate * sim._convert(Q)
 
     def __repr__(self):
         lines = [
             super().__repr__(),
             f"Target: {self.target.value}",
         ]
         return "\n".join(lines)
@@ -108,16 +112,15 @@
 
     .. _Haberkorn, Mol. Phys. 32:5, 1491-1493 (1976):
        http://dx.doi.org/10.1080/00268977600102851
     """
 
     def init(self, sim: LiouvilleSimulation):
         """See `radicalpy.simulation.HilbertIncoherentProcessBase.init`."""
-        size = prod(p.multiplicity for p in sim.particles) ** 2
-        self.subH = self.rate * np.eye(size)
+        self.subH = self.rate * np.eye(sim.hamiltonian_size)
 
 
 class JonesHore(LiouvilleKineticsBase):
     """Jones-Hore kinetics superoperator for two-site models.
 
     Source: `Jones et al. Chem. Phys. Lett. 507, 269-273 (2011)`_.
 
@@ -139,16 +142,16 @@
         self.triplet_rate = triplet_rate
 
     def init(self, sim: LiouvilleSimulation):
         """See `radicalpy.simulation.HilbertIncoherentProcessBase.init`."""
         QS = sim.projection_operator(State.SINGLET)
         QT = sim.projection_operator(State.TRIPLET)
         self.subH = (
-            0.5 * self.singlet_rate * self._convert(QS)
-            + 0.5 * self.triplet_rate * self._convert(QT)
+            0.5 * self.singlet_rate * sim._convert(QS)
+            + 0.5 * self.triplet_rate * sim._convert(QT)
             + (0.5 * (self.singlet_rate + self.triplet_rate))
             * (np.kron(QS, QT) + np.kron(QT, QS))
         )
 
     def __repr__(self):
         lines = [
             self._name(),
```

### Comparing `radicalpy-0.6.5/radicalpy/relaxation.py` & `radicalpy-0.7.0/radicalpy/relaxation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Relaxation superoperators.
 
 .. todo:: Add module docstring.
 """
+
 import numpy as np
 
 from .simulation import LiouvilleIncoherentProcessBase, LiouvilleSimulation, State
 from .utils import spectral_density
 
 
 class LiouvilleRelaxationBase(LiouvilleIncoherentProcessBase):
```

### Comparing `radicalpy-0.6.5/radicalpy/shared.py` & `radicalpy-0.7.0/radicalpy/shared.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,9 +30,9 @@
             SimpleNamespace: A namespace containing all constants.
         """
         with open(json_file, encoding="utf-8") as f:
             data = json.load(f)
         return SimpleNamespace(**{k: Constant(v) for k, v in data.items()})
 
 
-DATA_DIR = Path(__file__).parent / "data"
+DATA_DIR = Path(__file__).parent / "data_files"
 constants = Constant.fromjson(DATA_DIR / "constants.json")
```

### Comparing `radicalpy-0.6.5/radicalpy/simulation.py` & `radicalpy-0.7.0/radicalpy/simulation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 #!/usr/bin/env python
 
 import enum
 import itertools
 from math import prod
-from typing import Optional
+from typing import Iterator, Optional
 
 import numpy as np
 import scipy as sp
+from numpy.typing import NDArray
 from tqdm import tqdm
 
 from . import utils
 from .data import Molecule
 
 
 class State(enum.Enum):
     EQUILIBRIUM = "Eq"
     SINGLET = "S"
     TRIPLET = "T"
     TRIPLET_ZERO = "T_0"
     TRIPLET_PLUS = "T_+"
     TRIPLET_PLUS_MINUS = "T_\\pm"
     TRIPLET_MINUS = "T_-"
+    TP_SINGLET = "TP_S"
 
 
 class Basis(enum.Enum):
     ZEEMAN = "Zeeman"
     ST = "ST"
 
 
@@ -100,14 +102,18 @@
     def nuclei(self):
         return sum([[n for n in m.nuclei] for m in self.molecules], [])
 
     @property
     def particles(self):
         return self.radicals + self.nuclei
 
+    @property
+    def hamiltonian_size(self):
+        return np.prod([p.multiplicity for p in self.particles])
+
     def __repr__(self) -> str:
         return "\n".join(
             [
                 # "Simulation summary:",
                 f"Number of electrons: {len(self.radicals)}",
                 f"Number of nuclei: {len(self.nuclei)}",
                 f"Number of particles: {len(self.particles)}",
@@ -202,18 +208,18 @@
                 axis `axis`.
 
         """
         assert 0 <= idx and idx < len(self.particles)
         assert axis in "xyzpmu"
 
         sigma = self.pauli(self.particles[idx].multiplicity)[axis]
-        eye_before = np.eye(prod(p.multiplicity for p in self.particles[:idx]))
-        eye_after = np.eye(prod(p.multiplicity for p in self.particles[idx + 1 :]))
-
-        spinop = np.kron(np.kron(eye_before, sigma), eye_after)
+        before_size = prod(p.multiplicity for p in self.particles[:idx])
+        after_size = prod(p.multiplicity for p in self.particles[idx + 1 :])
+        spinop = np.kron(np.eye(before_size), sigma)
+        spinop = np.kron(spinop, np.eye(after_size))
         if self.basis == Basis.ST:
             return self.ST_basis(spinop)
         else:
             return spinop
 
     def product_operator(self, idx1: int, idx2: int, h: float = 1.0) -> np.ndarray:
         """Construct the (1D) product operator.
@@ -301,17 +307,30 @@
             State.TRIPLET: (3 / 4) * eye + SASB,
             State.TRIPLET_PLUS: (2 * SAz**2 + SAz) * (2 * SBz**2 + SBz),
             State.TRIPLET_MINUS: (2 * SAz**2 - SAz) * (2 * SBz**2 - SBz),
             State.TRIPLET_ZERO: (1 / 4) * eye + SAx @ SBx + SAy @ SBy - SAz @ SBz,
             State.TRIPLET_PLUS_MINUS: (2 * SAz**2 + SAz) * (2 * SBz**2 + SBz)
             + (2 * SAz**2 - SAz) * (2 * SBz**2 - SBz),
             State.EQUILIBRIUM: 1.05459e-34 / (1.38e-23 * 298),
+            State.TP_SINGLET: self.tp_singlet_projop(SAx, SAy, SAz, SBx, SBy, SBz),
         }
+
         return result[state]
 
+    def tp_singlet_projop(self, SAx, SAy, SAz, SBx, SBy, SBz):
+        # For radical triplet pair (RTP)
+        SAsquared = SAx @ SAx + SAy @ SAy + SAz @ SAz
+        SBsquared = SBx @ SBx + SBy @ SBy + SBz @ SBz
+        Ssquared = SAsquared + SBsquared + 2 * (SAx @ SBx + SAy @ SBy + SAz @ SBz)  #
+        return (
+            (1 / 12)
+            * (Ssquared - (6 * np.eye(len(SAx))))
+            @ (Ssquared - (2 * np.eye(len(SAx))))
+        )
+
     def zeeman_hamiltonian(
         self, B0: float, theta: Optional[float] = None, phi: Optional[float] = None
     ) -> np.ndarray:
         """Construct the Zeeman Hamiltonian (1D or 3D).
 
         Construct the Zeeman Hamiltonian based on the external
         magnetic field `B0`.  If the angles `theta` and `phi` are also
@@ -451,40 +470,44 @@
             (
                 self.particles[ei].gamma_mT
                 * prodop(ei, len(self.radicals) + ni, hfcs[ni])
                 for ni, ei in enumerate(self.coupling)
             )
         )
 
-    def exchange_hamiltonian(self, J: float) -> np.ndarray:
+    def exchange_hamiltonian(self, J: float, prod_coeff: float = 2) -> np.ndarray:
         """Construct the exchange Hamiltonian.
 
         Construct the exchange (J-coupling) Hamiltonian based on the
         coupling constant J between two electrons.
 
         The J-coupling constant can be obtained using:
 
         - `radicalpy.estimations.exchange_interaction_in_protein`
         - `radicalpy.estimations.exchange_interaction_in_solution`
 
         Args:
 
             J (float): Exchange coupling constant.
 
+            prod_coeff (float): Coefficient of the product operator
+                (default, radical-pair convention uses 2.0,
+                spintronics convention uses 1.0).
+
         Returns:
             np.ndarray:
 
                 The exchange (J-coupling) Hamiltonian corresponding to
                 the system described by the `HilbertSimulation` object
                 and the coupling constant `J`.
 
         """
         Jcoupling = J * self.radicals[0].gamma_mT
         SASB = self.product_operator(0, 1)
-        return Jcoupling * (2 * SASB + 0.5 * np.eye(SASB.shape[0]))
+        return Jcoupling * (prod_coeff * SASB + 0.5 * np.eye(SASB.shape[0]))
 
     def dipolar_hamiltonian(self, D: float | np.ndarray) -> np.ndarray:
         """Construct the Dipolar Hamiltonian.
 
         Construct the Dipolar Hamiltonian based on dipolar coupling
         constant or dipolar interaction tensor `D` between two
         electrons.  Depending on the `type` of `D`, the 1D or the 3D
@@ -567,14 +590,28 @@
             (
                 -self.radicals[0].gamma_mT
                 * self.product_operator_3d(ei, ne + ni, dipolar_tensor)
                 for ni, ei in enumerate(self.coupling)
             )
         )
 
+    def zero_field_splitting_hamiltonian(self, D, E) -> np.ndarray:
+        """Construct the Zero Field Splitting (ZFS) Hamiltonian."""
+        Dmod = D * -self.radicals[0].gamma_mT
+        Emod = E * -self.radicals[0].gamma_mT
+        result = complex(0.0)
+        for idx, p in enumerate(self.particles):
+            Sx = self.spin_operator(idx, "x")
+            Sy = self.spin_operator(idx, "y")
+            Sz = self.spin_operator(idx, "z")
+            Ssquared = Sx @ Sx + Sy @ Sy + Sz @ Sz
+            result += Dmod * (Sz @ Sz - (1 / 3) * Ssquared)
+            result += Emod * ((Sx @ Sx) - (Sy @ Sy))
+        return result
+
     def total_hamiltonian(
         self,
         B0: float,
         J: float,
         D: float | np.ndarray,
         theta: Optional[float] = None,
         phi: Optional[float] = None,
@@ -666,21 +703,23 @@
             rhos[t] = self.propagate(propagator, rhos[t - 1])
         return rhos
 
     def product_probability(self, obs: State, rhos: np.ndarray) -> np.ndarray:
         """Calculate the probability of the observable from the densities."""
         if obs == State.EQUILIBRIUM:
             raise ValueError("Observable state should not be EQUILIBRIUM")
-        obs = self.observable_projection_operator(obs)
-        return np.real(np.trace(obs @ rhos, axis1=-2, axis2=-1))
+        Q = self.observable_projection_operator(obs)
+        return np.real(np.trace(Q @ rhos, axis1=-2, axis2=-1))
 
     @staticmethod
     def product_yield(product_probability, time, k):
         """Calculate the product yield and the product yield sum."""
-        product_yield = k * sp.integrate.cumtrapz(product_probability, time, initial=0)
+        product_yield = k * sp.integrate.cumulative_trapezoid(
+            product_probability, time, initial=0
+        )
         product_yield_sum = k * np.trapz(product_probability, dx=time[1])
         return product_yield, product_yield_sum
 
     def apply_liouville_hamiltonian_modifiers(self, H, modifiers):
         for K in modifiers:  # skip in hilbert
             K.init(self)
             K.adjust_hamiltonian(H)
@@ -934,14 +973,18 @@
             product_yield_sums=product_yield_sums,
         )
 
     @staticmethod
     def convert(H: np.ndarray) -> np.ndarray:
         return H
 
+    @staticmethod
+    def _convert(Q: np.ndarray) -> np.ndarray:
+        return Q
+
     def initial_density_matrix(self, state: State, H: np.ndarray) -> np.ndarray:
         """Create an initial desity matrix.
 
         Create an initial density matrix for time evolution of the
         spin Hamiltonian density matrix.
 
         Args:
@@ -1039,15 +1082,25 @@
 
 
 class LiouvilleSimulation(HilbertSimulation):
     @staticmethod
     def convert(H: np.ndarray) -> np.ndarray:
         """Convert the Hamiltonian from Hilbert to Liouville space."""
         eye = np.eye(len(H))
-        return 1j * (np.kron(H, eye) - np.kron(eye, H.T))
+        tmp = np.kron(H, eye) - np.kron(eye, H.T)
+        return 1j * tmp
+
+    @staticmethod
+    def _convert(Q: np.ndarray) -> np.ndarray:
+        eye = np.eye(len(Q))
+        return np.kron(Q, eye) + np.kron(eye, Q)
+
+    @property
+    def hamiltonian_size(self):
+        return super().hamiltonian_size ** 2
 
     @staticmethod
     def _square_liouville_rhos(rhos):
         shape = rhos.shape
         dim = int(np.sqrt(shape[-2]))
         return rhos.reshape(*shape[:-2], dim, dim)
 
@@ -1148,7 +1201,54 @@
         """
         return propagator @ rho
 
 
 class LiouvilleIncoherentProcessBase(HilbertIncoherentProcessBase):
     def adjust_hamiltonian(self, H: np.ndarray):
         H -= self.subH
+
+
+# class SemiclassicalSimulation(LiouvilleSimulation):
+#    def semiclassical_gen(
+#        self,
+#        num_samples: int,
+#        #B: float,
+#    ) -> Iterator[NDArray[np.float_]]:
+#        num_particles = len(self.radicals)
+#        spinops = [
+#            [self.spin_operator(ri, ax) for ax in "xyz"] for ri in range(num_particles)
+#        ]
+#        for i in range(num_samples):
+#            result = complex(0)
+#            for ri, m in enumerate(self.molecules):
+#                std = m.semiclassical_std
+#                Is = np.random.normal(0, std, size=1)
+#                gamma = m.radical.gamma_mT
+#                for ax in range(3):
+#                    spinop = spinops[ri][ax]
+#                    result += gamma * spinop * Is
+#                #result += gamma * B * spinop
+#            yield result
+
+
+class SemiclassicalSimulation(LiouvilleSimulation):
+    def semiclassical_HHs(
+        self,
+        num_samples: int,
+    ) -> np.ndarray:
+        assert len(self.radicals) == 2
+        assert self.radicals[0].multiplicity == 2
+        assert self.radicals[1].multiplicity == 2
+
+        spinops = np.array([self.spin_operator(0, ax) for ax in "xyz"])
+        cov = np.diag([m.semiclassical_std for m in self.molecules])
+        samples = np.random.multivariate_normal(
+            mean=[0, 0],
+            cov=cov,
+            size=(num_samples, 3),
+        )
+        result = np.einsum("nam,axy->nxy", samples, spinops) * 2
+        return result * self.radicals[0].gamma_mT
+
+    @property
+    def nuclei(self):
+        return []
```

### Comparing `radicalpy-0.6.5/tests/test_data.py` & `radicalpy-0.7.0/tests/test_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #! /usr/bin/env python
 
 import doctest
 import unittest
 
 import numpy as np
 import numpy.testing
+
 from radicalpy import data
 
 
 def load_tests(loader, tests, ignore):
     tests.addTests(doctest.DocTestSuite(data))
     return tests
 
@@ -86,10 +87,10 @@
         self.assertRaises(ValueError, data.Hfc, 42)
 
 
 class MoleculeTestCase(unittest.TestCase):
     """Test case for the `Molecule` class."""
 
     def test_number_of_molecules(self):
-        previous_number = 6
+        previous_number = 7
         current_number = len(data.Molecule.available())
         self.assertEqual(current_number, previous_number)
```

### Comparing `radicalpy-0.6.5/tests/test_estimations.py` & `radicalpy-0.7.0/tests/test_estimations.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,36 @@
 
 import unittest
 
 import radicalpy as rp
 
 
 class EstimationsTests(unittest.TestCase):
-    def test_Bhalf_theoretical(self):
+    def test_Bhalf_theoretical_hyperfine(self):
         flavin = rp.simulation.Molecule.fromdb("flavin_anion")
         trp = rp.simulation.Molecule.fromdb("tryptophan_cation")
         sim = rp.simulation.HilbertSimulation([flavin, trp])
-        Bhalf_theoretical = rp.estimations.Bhalf_theoretical(sim)
+        Bhalf_theoretical = rp.estimations.Bhalf_theoretical_hyperfine(sim)
         self.assertAlmostEqual(Bhalf_theoretical, 2.9692816566569937, places=2)
 
+    def test_Bhalf_theoretical_relaxation(self):
+        gold = 6.581867450174098
+        kstd = 3.8e7
+        krec = 1e6
+        bhalf = rp.estimations.Bhalf_theoretical_relaxation(kstd, krec)
+        self.assertAlmostEqual(gold, bhalf)
+
+    def test_Bhalf_theoretical_relaxation_delay(self):
+        gold = 7.386542039837055
+        kstd = 1e8
+        krec = 1e6
+        td = 1e-6
+        bhalf = rp.estimations.Bhalf_theoretical_relaxation_delay(kstd, krec, td)
+        self.assertAlmostEqual(gold, bhalf)
+
     def test_T1_relaxation_rate(self):
         gold = 557760.0907618533
         g = [2.00429, 2.00389, 2.00216]
         B = 0.05
         tau_c = 1.3006195732809966e-07
         t1 = rp.estimations.T1_relaxation_rate(g, B, tau_c)
         self.assertAlmostEqual(gold, t1)
@@ -66,22 +81,22 @@
 
     def test_k_electron_transfer(self):
         gold = 15135612.484362071
         R = 13.3
         k_et = rp.estimations.k_electron_transfer(R)
         self.assertAlmostEqual(gold, k_et)
 
-    def test_k_excitation(self):
+    def test_k_excitation_extinction_coefficient(self):
         gold = 52749.44112741747
         P = 290e-6
         wl = 450e-9
         V = 0.54e-15
         l = 900e-9
         epsilon = 12600
-        kI = rp.estimations.k_excitation(P, wl, V, l, epsilon)
+        kI = rp.estimations.k_excitation_extinction_coefficient(P, wl, V, l, epsilon)
         self.assertAlmostEqual(gold, kI)
 
     def test_k_recombination(self):
         gold = 14161120.442179158
         MFE = 0.35
         k_escape = 5.3e6
         k_rec = rp.estimations.k_recombination(MFE, k_escape)
```

### Comparing `radicalpy-0.6.5/tests/test_shared.py` & `radicalpy-0.7.0/tests/test_shared.py`

 * *Files identical despite different names*

### Comparing `radicalpy-0.6.5/tests/test_simulation.py` & `radicalpy-0.7.0/tests/test_simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,23 @@
 import doctest
 import os
 import time
 import unittest
 
 import matplotlib.pyplot as plt
 import numpy as np
+
 import radicalpy as rp
 from radicalpy import estimations, kinetics, relaxation
 from radicalpy.simulation import Basis
 
+# quick test:
+# comment the next line out, and run in repo root:
+# set PYTHONPATH=.
+# python tests/test_simulation.py TripletTests.test_time_evolution
 from . import radpy
 
 # np.seterr(divide="raise", invalid="raise")
 
 RUN_SLOW_TESTS = "INSIDE_EMACS" not in os.environ  # or True
 MEASURE_TIME = False
 
@@ -293,14 +298,16 @@
         approx = estimations.dipolar_interaction_isotropic(1)
         gold = approx
         self.assertEqual(gold, approx)
 
     def test_initial_density_matrix(self):
         H = self.sim.total_hamiltonian(PARAMS["B"][0], PARAMS["J"], PARAMS["D"])
         for state in rp.simulation.State:
+            if state == rp.simulation.State.TP_SINGLET:
+                continue
             rho0 = self.sim.initial_density_matrix(state, H)
             rpstate = state2radpy(state)
             rho0_true = radpy.Hilbert_initial(rpstate, len(self.sim.particles), H)
             np.testing.assert_almost_equal(rho0, rho0_true)
 
     def test_unitary_propagator(self):
         dt = np.random.uniform(1e-6)
@@ -310,17 +317,21 @@
         np.testing.assert_almost_equal(unitary_true, unitary)
 
     def test_time_evolution(self):
         k = np.random.uniform()
         H = self.sim.total_hamiltonian(PARAMS["B"][0], PARAMS["J"], PARAMS["D"])
         Kexp = kinetics.Exponential(k)
         for init_state in rp.simulation.State:
+            if init_state == rp.simulation.State.TP_SINGLET:
+                continue
             for obs_state in rp.simulation.State:
                 if obs_state == rp.simulation.State.EQUILIBRIUM:
                     continue
+                if obs_state == rp.simulation.State.TP_SINGLET:
+                    continue
                 evol_true = radpy.TimeEvolution(
                     len(self.sim.particles),
                     state2radpy(init_state),
                     state2radpy(obs_state),
                     self.t_max,
                     self.dt,
                     k,
@@ -406,15 +417,14 @@
                 plt.suptitle(suptitle)
                 plt.plot(rslt["time"], rslt[key][Bi])
                 plt.plot(strs["time"], strs[key][Bi])
         # np.testing.assert_almost_equal(rslt[key], strs[key])
         plt.show()
 
     def test_hyperfine_3d(self):
-
         results = self.sim.MARY(
             rp.simulation.State.SINGLET,
             rp.simulation.State.TRIPLET,
             self.time,
             PARAMS["B"],
             PARAMS["D"],
             PARAMS["J"],
@@ -493,14 +503,16 @@
         self.dt = 0.01
         self.t_max = 1.0
         self.time = np.arange(0, self.t_max, self.dt)
 
     def test_initial_density_matrix(self):
         H = self.sim.total_hamiltonian(PARAMS["B"][0], PARAMS["J"], PARAMS["D"])
         for state in rp.simulation.State:
+            if state == rp.simulation.State.TP_SINGLET:
+                continue
             rho0 = self.sim.initial_density_matrix(state, H)
             rpstate = state2radpy(state)
             rho0_true = radpy.Liouville_initial(rpstate, len(self.sim.particles), H)
             np.testing.assert_almost_equal(rho0, rho0_true)
 
     def test_unitary_propagator(self):
         dt = np.random.uniform(0, 1e-6)
@@ -566,7 +578,42 @@
         )
 
         # idx = 0
         # plt.plot(results["time"], results["time_evolutions"][idx])
         # plt.title(f"B={results['B'][idx]}")
         # plt.show()
         # print("DONE")
+
+
+class TripletTests(unittest.TestCase):
+    def setUp(self):
+        dummy_hfc = rp.data.Hfc(0.0)
+        gamma = -176085963.0230
+        radical = rp.data.Nucleus(gamma, 3, dummy_hfc)
+        z1 = rp.data.Molecule("Z", [], radical=radical)
+        z2 = rp.data.Molecule(name="Z", nuclei=[], radical=radical)
+        basis = rp.simulation.Basis.ZEEMAN
+        self.sim = rp.simulation.HilbertSimulation([z1, z2], basis=basis)
+        self.dt = 0.01
+        self.t_max = 1.0
+        self.time = np.arange(0, self.t_max, self.dt)
+
+    def test_time_evolution(self):
+        init_state = rp.simulation.State.TRIPLET
+        H = self.sim.total_hamiltonian(B0=0, J=0, D=100)
+        rhos = self.sim.time_evolution(init_state, self.time, H)
+        obs = rp.simulation.State.SINGLET
+        k = 0
+        prod_prob = self.sim.product_probability(obs, rhos)
+        result, _ = self.sim.product_yield(prod_prob, self.time, k)
+
+        # fig, axs = plt.subplots(2)
+        # plt.sca(axs[0])
+        # plt.plot(self.time, result)
+
+        # plt.sca(axs[1])
+        # plt.spy(H)
+        # plt.show()
+
+
+if __name__ == "__main__":
+    unittest.main()
```

