# Comparing `tmp/fringes-1.1.0.tar.gz` & `tmp/fringes-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fringes-1.1.0.tar", max compression
+gzip compressed data, was "fringes-1.1.1.tar", max compression
```

## Comparing `fringes-1.1.0.tar` & `fringes-1.1.1.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     2023 2024-04-04 17:33:01.725323 fringes-1.1.0/fringes/__init__.py
--rw-r--r--   0        0        0    30067 2024-04-04 15:55:32.493493 fringes-1.1.0/fringes/decoder.py
--rw-r--r--   0        0        0   143373 2024-04-05 08:33:10.871524 fringes-1.1.0/fringes/fringes.py
--rw-r--r--   0        0        0     1435 2023-09-15 17:49:38.845283 fringes-1.1.0/fringes/grid.py
--rw-r--r--   0        0        0     1667 2024-04-04 16:58:05.360788 fringes-1.1.0/fringes/main.py
--rw-r--r--   0        0        0      240 2024-04-07 18:18:17.231413 fringes-1.1.0/fringes/readme.txt
--rw-r--r--   0        0        0    15646 2024-04-03 12:08:47.548339 fringes-1.1.0/fringes/util.py
--rw-r--r--   0        0        0    21278 2023-08-24 07:23:04.058802 fringes-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1491 2024-04-05 10:57:46.868229 fringes-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     5850 2024-04-07 18:35:16.174665 fringes-1.1.0/README.md
--rw-r--r--   0        0        0     7046 1970-01-01 00:00:00.000000 fringes-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1827 2024-04-14 11:19:17.015751 fringes-1.1.1/fringes/__init__.py
+-rw-r--r--   0        0        0    30119 2024-04-14 15:34:41.202257 fringes-1.1.1/fringes/decoder.py
+-rw-r--r--   0        0        0   144129 2024-04-14 18:46:23.985206 fringes-1.1.1/fringes/fringes.py
+-rw-r--r--   0        0        0     1493 2024-04-14 10:42:40.003632 fringes-1.1.1/fringes/grid.py
+-rw-r--r--   0        0        0      240 2024-04-14 10:34:27.271830 fringes-1.1.1/fringes/readme.txt
+-rw-r--r--   0        0        0    16839 2024-04-14 18:46:22.304989 fringes-1.1.1/fringes/util.py
+-rw-r--r--   0        0        0    20842 2024-04-14 10:00:48.580328 fringes-1.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     1491 2024-04-14 10:58:26.256769 fringes-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5850 2024-04-14 10:24:04.512646 fringes-1.1.1/README.md
+-rw-r--r--   0        0        0     7046 1970-01-01 00:00:00.000000 fringes-1.1.1/PKG-INFO
```

### Comparing `fringes-1.1.0/fringes/__init__.py` & `fringes-1.1.1/fringes/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,38 +5,33 @@
 import glob
 import webbrowser
 import argparse
 
 from .fringes import Fringes
 from .util import vshape, curvature, height
 
-# logging.getLogger(__name__)
-
-# formatter = logging.Formatter("%(asctime)s %(levelname)-8s %(name)7s: %(message)s")
-# handler = logging.StreamHandler()
-# handler.setFormatter(formatter)
-# logger.addHandler(handler)
+logger = logging.getLogger(__name__)
 
 # use verion string in pyproject.toml as the single source of truth
 try:
     # in order not to confuse an installed version of a package with a local one,
     # first try the local one (not being installed)
     data = toml.load(os.path.join(os.path.dirname(__file__), "..", "pyproject.toml"))
     __version__ = data["project"]["version"]  # Python Packaging User Guide expects version here
 except KeyError:
     __version__ = data["tool"]["poetry"]["version"]  # Poetry expects version here
 except FileNotFoundError:
     __version__ = importlib.metadata.version("fringes")  # installed version
 
-# flist = glob.glob(os.path.join(os.path.dirname(__file__), "__pycache__", "decoder*decode*.nbc"))
-# if not flist or os.path.getmtime(__file__) > max(os.path.getmtime(file) for file in flist):
-#     logging.warning(
-#         "The 'decode()'-function has not been compiled yet. "
-#         "This will take a few minutes (the time depends on your CPU and energy settings)."
-#     )
+flist = glob.glob(os.path.join(os.path.dirname(__file__), "__pycache__", "decoder*decode*.nbc"))
+if not flist or os.path.getmtime(__file__) > max(os.path.getmtime(file) for file in flist):
+    logging.warning(
+        "The 'decode()'-function has not been compiled yet. "
+        "This will take a few minutes (the time depends on your CPU and energy settings)."
+    )
 
 
 def documentation():
     fname = os.path.join(os.path.dirname(__file__), "..", "docs", "_build", "index.html")
     if os.path.isfile(fname):
         webbrowser.open_new_tab(os.path.join(os.path.dirname(__file__), "..", "docs", "_build", "index.html"))
     else:
```

### Comparing `fringes-1.1.0/fringes/decoder.py` & `fringes-1.1.1/fringes/decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -294,16 +294,16 @@
         #     Ka = [x + (y,) for x in Ka for y in pool]
         # Kr = set(Ka) - Kn - Kp  # remaining combinations, i.e. all without neighbouring and also without matching one
         #
         # Kp = np.array(sorted(Kp))
         # Kn = np.array(sorted(Kn))
         # Kr = np.array(sorted(Kr))
 
-        for x in nb.prange(X):  # numba's prange affects only outer prange-loop, so we put largest direction first
-            for y in nb.prange(Y):
+        for y in nb.prange(Y):  # numba's prange affects only outer prange-loop, so we put largest direction first
+            for x in nb.prange(X):  # x at last so that we read out memory efficiently
                 # aa01_crt_tried = 0
                 # aa02_der_tried = 0
                 # aa03_der_tried = 0
                 # aa04_nei_tried = 0
                 # aa05_nei_tried = 0
                 # aa06_exh_tried = 0
                 #
```

### Comparing `fringes-1.1.0/fringes/fringes.py` & `fringes-1.1.1/fringes/fringes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,27 @@
-import os
 import logging
+import os
 import itertools as it
 from collections import namedtuple
 import time
 import json
 
 import numpy as np
 import scipy as sp
 import sympy
 import skimage as ski
 import cv2
 import toml
 import yaml
 
-from .util import vshape, bilateral, _remap
+from .util import vshape, bilateral, _remap, _source
 from . import grid
 from .decoder import decode
 
-# logging.getLogger(__name__)
-# formatter = logging.Formatter("%(asctime)s %(levelname)-8s %(name)7s.%(funcName)-11s: %(message)s")
-# handler = logging.StreamHandler()
-# handler.setFormatter(formatter)
-# logger.addHandler(handler)
-# logging.getLogger(__name__)
+logger = logging.getLogger(__name__)
 
 
 class Fringes:
     """Easy-to-use class to configure, encode and decode customized fringe patterns using phase shifting algorithms."""
 
     # note: the class docstring is continuated at the end of the class
 
@@ -145,23 +140,14 @@
         #  **kwargs,  # bundles all undefined kwargs, else error: __init__() got an unexpected keyword argument
     ) -> None:
         # given values which are in defaults but are not identical to them
         given = {
             k: v for k, v in sorted(locals().items()) if k in self.defaults and not np.array_equal(v, self.defaults[k])
         }
 
-        # logger
-        self.logger = logging.getLogger(self.__class__.__name__)
-        self.logger.setLevel("WARNING")
-        if not self.logger.hasHandlers():
-            formatter = logging.Formatter("%(asctime)s %(levelname)-8s %(name)7s.%(funcName)-11s: %(message)s")
-            handler = logging.StreamHandler()
-            handler.setFormatter(formatter)
-            self.logger.addHandler(handler)
-
         # set default values
         self._UMR = None  # used for caching
         for k, v in self.defaults.items():
             if k not in "HMTlAB":  # these properties are inferred from others
                 setattr(self, f"_{k}", v)  # define private variables from where the properties get their value from
 
         # set given values
@@ -236,39 +222,39 @@
         >>> f.load(fname)
         """
 
         if fname is None:
             fname = os.path.join(os.path.expanduser("~"), ".fringes.yaml")
 
         if not os.path.isfile(fname):
-            logging.error(f"File '{fname}' does not exist.")
+            logger.error(f"File '{fname}' does not exist.")
             return
 
         with open(fname, "r") as f:
             ext = os.path.splitext(fname)[-1]
 
             if ext == ".json":
                 p = json.load(f)
             elif ext == ".yaml":
                 p = yaml.safe_load(f)
             elif ext == ".toml":
                 p = toml.load(f)
             else:
-                logging.error(f"Unknown file type '{ext}'.")
+                logger.error(f"Unknown file type '{ext}'.")
                 return {}
 
         if "fringes" in p:
             params = p["fringes"]
             self.params = params
 
-            logging.info(f"Loaded parameters from '{fname}'.")
+            logger.info(f"Loaded parameters from '{fname}'.")
 
             return params
         else:
-            logging.error(f"No 'fringes' section in file '{fname}'.")
+            logger.error(f"No 'fringes' section in file '{fname}'.")
             return {}
 
     def save(self, fname: str = None) -> None:
         """Save the parameters of the `Fringes` instance to a config file.
 
         Within the file, the parameters are written to the section `fringes`.
 
@@ -291,40 +277,40 @@
         >>> f.save(fname)
         """
 
         if fname is None:
             fname = os.path.join(os.path.expanduser("~"), ".fringes.yaml")
 
         if not os.path.isdir(os.path.dirname(fname)):
-            logging.warning(f"File directory does not exist.")
+            logger.warning(f"File directory does not exist.")
             return
 
         name, ext = os.path.splitext(fname)
         if not ext:
             name, ext = ext, name
 
         if ext not in self._loader.keys():
-            logging.warning(f"File extension is unknown. Must be one of {self._loaders.keys()}")
+            logger.warning(f"File extension is unknown. Must be one of {self._loaders.keys()}")
             return
 
         with open(fname, "w") as f:
             if ext == ".json":
                 json.dump({"fringes": self.params}, f, indent=4)
             elif ext == ".yaml":
                 yaml.dump({"fringes": self.params}, f)
             elif ext == ".toml":
                 toml.dump({"fringes": self.params}, f)
 
-        logging.debug(f"Saved parameters to {fname}.")  # todo: info?
+        logger.debug(f"Saved parameters to {fname}.")  # todo: info?
 
     def reset(self) -> None:
         """Reset parameters of the `Fringes` instance to default values."""
 
         self.params = self.defaults
-        logging.info("Reset parameters to defaults.")
+        logger.info("Reset parameters to defaults.")
 
     def optimize(self, T: int = None, umax: float = None) -> None:  # todo: self.umax
         """Optimize the parameters of the `Fringes` instance.
 
         Parameters
         ----------
          T : int, optional
@@ -361,15 +347,15 @@
                 ...  # todo: check if umax is reached
         else:  # T -> u
             if T is None:
                 T = self.T
 
             self.T = T  # distribute frames optimally (evenly) on shifts
 
-        logging.info("Optimized parameters.")
+        logger.info("Optimized parameters.")
 
     @staticmethod
     def gamma_auto_correct(I: np.ndarray) -> np.ndarray:
         """Automatically estimate and apply the gamma correction factor
         to linearize the display/camera response curve.
 
         Parameters
@@ -435,15 +421,15 @@
 
         T, Y, X, C = vshape(I).shape
         assert T * Y % self.T == 0, "Number of frames of parameters and data don't match."
 
         # I = I.reshape((T * Y, X, C))  # concatenate
         I = I.reshape((-1, self.T, X, C)).swapaxes(0, 1)
 
-        logging.info(f"{1000 * (time.perf_counter() - t0)}ms")
+        logger.info(f"{1000 * (time.perf_counter() - t0)}ms")
 
         return I
 
     def coordinates(self) -> np.ndarray:
         """Generate the coordinate matrices of the coordinate system defined in `grid`.
 
         Returns
@@ -467,15 +453,15 @@
 
         if self.D == 1:
             xi = xi[self.axis][None, :, :]  # returns a view
 
         if self.grid in ["polar", "log-polar"]:
             xi *= self.L
 
-        logging.info(f"{1000 * (time.perf_counter() - t0)}ms")
+        logger.info(f"{1000 * (time.perf_counter() - t0)}ms")
 
         return xi
 
     def _orders(self) -> np.ndarray:
         """Generate fringe orders.
 
         Returns
@@ -569,15 +555,15 @@
                             val = val >= 0.5
 
                         I[idx] = val
 
                         idx += 1
                     frame += 1
 
-        logging.debug(f"{1000 * (time.perf_counter() - t0)}ms")
+        logger.debug(f"{1000 * (time.perf_counter() - t0)}ms")
 
         return I.reshape(-1, Y, X, 1)
 
     def _demodulate(
         self, I: np.ndarray, verbose: bool = False, func: str = "ski"
     ) -> (np.ndarray, np.ndarray, np.ndarray, np.ndarray, np.ndarray):
         """Decode base fringe patterns by spatio-temporal demodulation.
@@ -771,15 +757,15 @@
                 self.UMR,
                 self.x0,
                 self.p0,
                 self.Vmin,
                 self.verbose or verbose,
             )
 
-        logging.debug(f"{1000 * (time.perf_counter() - t0)}ms")
+        logger.debug(f"{1000 * (time.perf_counter() - t0)}ms")
 
         return bri, mod, phi, reg, res
 
     def _multiplex(self, I: np.ndarray, rint: bool = True) -> np.ndarray:
         """Multiplex fringe patterns.
 
         Parameters
@@ -829,28 +815,28 @@
         if self.FDM:
             assert not self.WDM
             assert not self.SDM
             assert len(np.unique(self.N)) == 1
             assert I.dtype.kind == "f"
 
             if np.any(self._N < 2 * np.abs(self._f).max() + 1):  # todo: fractional periods
-                logging.warning("Decoding might be disturbed.")
+                logger.warning("Decoding might be disturbed.")
 
             I = I.reshape((self.D * self.K, -1))  # returns a view
             I -= self.A
             I = np.sum(I, axis=0)
             I += self.A
             # I *= 1 / (self.D * self.K)
             I = I.reshape((-1, self.Y, self.X, 1))  # returns a view
             if self.dtype.kind in "uib":
                 if rint:
                     np.rint(I, out=I)
                 I = I.astype(self.dtype, copy=False)  # returns a view
 
-        logging.debug(f"{1000 * (time.perf_counter() - t0)}ms")
+        logger.debug(f"{1000 * (time.perf_counter() - t0)}ms")
 
         return I
 
     def _demultiplex(self, I: np.ndarray) -> np.ndarray:
         """Demultiplex fringe patterns.
 
         Parameters
@@ -923,15 +909,15 @@
 
         if self.FDM:
             assert not self.WDM
             assert not self.SDM  # todo: allow self.SDM?
             assert len(np.unique(self.N)) == 1
             I = np.tile(I, (self.D * self.K, 1, 1, 1))
 
-        logging.debug(f"{1000 * (time.perf_counter() - t0)}ms")
+        logger.debug(f"{1000 * (time.perf_counter() - t0)}ms")
 
         return I
 
     def _colorize(self, I: np.ndarray, frames: np.ndarray) -> np.ndarray:
         """Colorize fringe patterns.
 
         Parameters
@@ -998,15 +984,15 @@
         #                 J[i, ..., c] = I[i, ..., cj]
         #             elif self.dtype.kind in "uib":  # f -> uib
         #                 J[i, ..., c] = np.rint(I[i, ..., cj] * (self.h[h, c] / 255)).astype(self.dtype, copy=False)
         #             else:  # f -> f
         #                 J[i, ..., c] = I[i, ..., cj] * (self.h[h, c] / 255)
         #         i += 1
 
-        logging.debug(f"{1000 * (time.perf_counter() - t0)}ms")
+        logger.debug(f"{1000 * (time.perf_counter() - t0)}ms")
 
         return J
 
     def _decolorize(self, I: np.ndarray) -> np.ndarray:
         """Decolorize fringe patterns by weighted averaging of hues.
 
         Parameters
@@ -1078,15 +1064,15 @@
             #     dtype = I.dtype  # without this, np.sum chooses a dtype which can hold the theoretical maximal sum
             # else:
 
             dtype = float  # without this, np.sum chooses a dtype which can hold the theoretical maximal sum
             I = np.sum(I * w[:, None, None, None, :], axis=0, dtype=dtype)
             # todo: numpy.tensordot ?
 
-        logging.debug(f"{1000 * (time.perf_counter() - t0)}ms")
+        logger.debug(f"{1000 * (time.perf_counter() - t0)}ms")
 
         return I
 
     def encode(
         self,
         xi: list | np.ndarray = None,
         frames: int | tuple = None,
@@ -1230,15 +1216,15 @@
         if self.grid in ["polar", "log-polar"]:
             I *= grid.innercirc(self.Y, self.X)[None, :, :, None]
 
         # colorize (extended averaging)
         if self.H > 1 or np.any(self.h != 255):  # can be used for extended averaging
             I = self._colorize(I, frames)
 
-        logging.info(f"{1000 * (time.perf_counter() - t0)}ms")
+        logger.info(f"{1000 * (time.perf_counter() - t0)}ms")
 
         return (
             self._simulate(I, PSF=0, system_gain=self.gain, dark_current=self.y0 / self.gain, dark_noise=self.dark)
             if simulate
             else I
         )
 
@@ -1361,15 +1347,15 @@
                     phi[..., idx] = np.nan
                     fid[..., idx] = np.nan
                     vis[..., idx] = 0
                     exp[..., idx] = 0
 
         # spatial unwrapping
         if self._ambiguous:
-            logging.warning("Unwrapping is not spatially independent and only yields a relative phase map.")
+            logger.warning("Unwrapping is not spatially independent and only yields a relative phase map.")
             reg = self._unwrap(reg, bri)  # todo: res if verbose
         else:  # coordiante retransformation
             # todo: tests
 
             if self.D == 2:
                 # todo: swapaxes
                 if self.grid == "Cartesian":
@@ -1440,15 +1426,15 @@
             dec = namedtuple(
                 "decoded",
                 "brightness modulation registration residuals uncertainty phase orders visibility exposure",
             )(bri, mod, reg, res, unc, phi, fid, vis, exp)
         else:
             dec = namedtuple("decoded", "brightness modulation registration")(bri, mod, reg)
 
-        logging.info(f"{1000 * (time.perf_counter() - t0)}ms")
+        logger.info(f"{1000 * (time.perf_counter() - t0)}ms")
 
         return dec
 
     def _verbose_(self, I: np.ndarray, A: np.ndarray, B: np.ndarray, xi: np.ndarray, lessbits: bool = False):
         """Compute verbose output.
 
         Parameters
@@ -1589,17 +1575,17 @@
 
         reg = np.empty((self.D, Y, X, C), np.float32)
         if self.verbose:
             res = np.empty((self.D, Y, X, C), np.float32)
 
         for d in range(self.D):
             if self.K == 1:  # todo: self.K[d] == 1
-                logging.info(f"Spatial phase unwrapping in 2D{' for each color indepently' if C > 1 else ''}.")
+                logger.info(f"Spatial phase unwrapping in 2D{' for each color indepently' if C > 1 else ''}.")
             else:
-                logging.info(f"Spatial phase unwrapping in 3D{' for each color indepently' if C > 1 else ''}.")
+                logger.info(f"Spatial phase unwrapping in 3D{' for each color indepently' if C > 1 else ''}.")
                 func = "ski"  # only ski can unwrap in 3D
 
             for c in range(C):
                 if func in "cv2":  # OpenCV algorithm is usually faster, but can be much slower in noisy images
                     # dtype must be np.float32  # todo: test this
                     if False:  # todo: isinstance(B, np.ndarray) and vshape(B).shape == phi.shape:
                         # todo: unwrap with mask
@@ -1628,15 +1614,15 @@
 
             regmin = np.min(reg[d])
             if regmin < 0:
                 reg[d] -= regmin
 
         reg *= self._l[:, 0, None, None, None] / (2 * np.pi)
 
-        logging.debug(f"{1000 * (time.perf_counter() - t0)}ms")
+        logger.debug(f"{1000 * (time.perf_counter() - t0)}ms")
 
         return reg  # todo: res if verbose
 
     # @staticmethod
     # def unwrap(phi: np.ndarray, mask: np.ndarray = None, func: str = "ski") -> np.array:
     #     """Unwrap phase maps spacially.
     #
@@ -1836,24 +1822,34 @@
             # idx = np.rint(xi).astype(int, copy=False)
             # for c in range(C):  # looping through color channels reduces memory consumption
             #     src[idx[1].ravel(), idx[0].ravel(), c] += B[..., c].ravel()  # ravel() returns a view
             # todo: advanced indexing with nan?
             B[~valid] = 0
             src = _remap(src, xi, B)  # todo: if u is array -> also increment region around rint pixel
 
-            # blurring due to uncertainty and PSF
+            # morphology
             u = self.u if self.indexing == "ij" else self.u[::-1]  # todo: D = 1, i.e. shape of sigma equal to axes?
-            sigma = np.sqrt(u**2 + self.PSF**2)
-            src = sp.ndimage.gaussian_filter(src, sigma, mode="nearest", axes=(0, 1))
+            a = 3
+            sigma = np.ceil(dx + a * u).astype(int)
+            # kernel = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, sigma)  # works only if sigma is 2D
+            kernel = cv2.getStructuringElement(cv2.MORPH_ELLIPSE, (sigma[0], sigma[-1]))  # works if sigma is 1D
+            if any(d > 1 for d in kernel.shape):
+                for c in range(C):
+                    src[:, :, c] = sp.ndimage.grey_dilation(src[:, :, c], structure=kernel)
 
-            # blurring due to pixel size
-            dx = 3
-            dx_ = int(dx + 0.5)
-            if dx > 1:
-                src = sp.ndimage.uniform_filter(src, size=dx_, mode="reflect", axes=(0, 1))
+            # # blurring due to uncertainty and PSF
+            # u = self.u if self.indexing == "ij" else self.u[::-1]  # todo: D = 1, i.e. shape of sigma equal to axes?
+            # sigma = np.sqrt(u**2 + self.PSF**2)
+            # src = sp.ndimage.gaussian_filter(src, sigma, mode="nearest", axes=(0, 1))  # todo: uniform?
+            #
+            # # blurring due to pixel size
+            # dx = 3
+            # dx_ = int(dx + 0.5)
+            # if dx > 1:
+            #     src = sp.ndimage.uniform_filter(src, size=dx_, mode="reflect", axes=(0, 1))
         else:
             xi = xi[:, valid].reshape(2, -1, C).swapaxes(0, 1)  # n data points of dimension m
             if B is not None:
                 B = B[valid].reshape(-1, C)  # n data points of dimension m
 
             # todo: use U if given as an array (but how?)
 
@@ -1861,20 +1857,37 @@
                 1 / self.D
             )  # geometric mean averages the semi-axes of the uncertainty ellipses
             sigma = np.sqrt(u**2 + self.PSF**2)
             dr = dx / np.sqrt(np.pi)  # mapping radius of sqare (=dx/2) to radius of circle (dr) with same area
             a = 3  # number of standard deviations
             R = dr + a * sigma
 
+            # # todo: quary_ball
+            # idx = self.coordinates()[:, :, :]
+            # idx = idx.reshape(2, -1).swapaxes(0, 1)  # n data points of dimension m
+            # kdtree_src = sp.spatial.KDTree(idx)
+
             src = np.empty((self.Y, self.X, C), np.float32)
             for c in range(C):
                 kdtree = sp.spatial.KDTree(xi[:, :, c])
-                for xs in range(self.X):
-                    for ys in range(self.Y):
-                        i = kdtree.query_ball_point(x=(xs, ys), r=R, p=2)  # , workers=-1)  # list of indices
+
+                # ii = kdtree_src.query_ball_tree(kdtree, r=R, p=2)  # list of list of indices
+                # ii = [i for i in ii if i != []]
+                #
+                # Bc = B[:, c] if B is not None else np.ones((Y, X), np.uint8)[valid[:, :, c]].reshape(-1)  # n data points of dimension m
+                # src[:, :, c] = _source(src[:, :, c], Bc, xi[:, :, c], ii)
+
+                for ys in range(self.Y):  # todo: accelerate with numba
+                    print(ys)
+                    for xs in range(self.X):
+                        i = kdtree.query_ball_point(
+                            x=(xs, ys), r=R, p=2
+                        )  # , workers=-1)  # , workers=-1)  # list of indices
+                        # j = np.ravel_multi_index((ys, xs), src.shape[:-1])
+                        # i = ii[j]
 
                         if not i:  # empty list, i.e. no points found within distance R
                             v = 0
                         else:
                             xr = xi[i, 0, c]  # returns a view
                             yr = xi[i, 1, c]  # returns a view
                             d = np.sqrt((xs - xr) ** 2 + (ys - yr) ** 2)  # distance
@@ -1897,15 +1910,15 @@
 
                         src[ys, xs, c] = v
 
         mx = src.max()
         if mx > 0 and mx != 1:
             src /= mx
 
-        logging.info(f"{1000 * (time.perf_counter() - t0)}ms")
+        logger.info(f"{1000 * (time.perf_counter() - t0)}ms")
 
         return src
 
     def brightfield_inverse(self, src: np.ndarray, t: float = 0.1, k: int = 3) -> np.ndarray:
         """Inverse bright-field
 
         with radiomatric compensation
@@ -2092,15 +2105,15 @@
 
         # clip values
         np.clip(I, 0, self.Imax, out=I)
 
         # quantization noise is added by converting to integer
         I = I.astype(self.dtype, copy=False)
 
-        logging.info(f"{1000 * (time.perf_counter() - t0)}ms")
+        logger.info(f"{1000 * (time.perf_counter() - t0)}ms")
 
         return I
 
     def _trim(self, a: np.ndarray) -> np.ndarray:
         """Change `a`.ndim to 2 and limit `a`.shape."""
 
         if a.ndim == 0:
@@ -2200,15 +2213,15 @@
     def T(self, T: int):
         # attention: params may change even if Tnew == Told
 
         _T = int(min(max(1, T), self._Tmax))
 
         if _T == 1:  # WDM + SDM todo: FTM?
             if self.grid not in self._grids[:2]:
-                logging.error(f"Couldn't set 'T = 1': grid not in {self._grids[:2]}'.")
+                logger.error(f"Couldn't set 'T = 1': grid not in {self._grids[:2]}'.")
                 return
 
             self.H = 1
             self.K = 1
 
             self.FDM = False  # reset FDM before setting N
             self.N = 3  # set N before WDM
@@ -2302,15 +2315,15 @@
 
     @Y.setter
     def Y(self, Y: int):
         _Y = int(min(max(1, Y), self._Ymax, self._Pmax / self.X))
 
         if self._Y != _Y:
             self._Y = _Y
-            logging.debug(f"{self._Y = }")
+            logger.debug(f"{self._Y = }")
             self._UMR = None
 
             if self._X == self._Y == 1:
                 self.D = 1
                 self.axis = 0
             elif self._X == 1:
                 self.D = 1
@@ -2327,15 +2340,15 @@
 
     @X.setter
     def X(self, X: int):
         _X = int(min(max(1, X), self._Xmax, self._Pmax / self.Y))
 
         if self._X != _X:
             self._X = _X
-            logging.debug(f"{self._X = }")
+            logger.debug(f"{self._X = }")
             self._UMR = None
 
             if self._X == self._Y == 1:
                 self.D = 1
                 self.axis = 0
             elif self._X == 1:
                 self.D = 1
@@ -2372,15 +2385,15 @@
 
     @alpha.setter
     def alpha(self, alpha: float):
         _alpha = float(min(max(1, alpha), self._alphamax))
 
         if self._alpha != _alpha:
             self._alpha = _alpha
-            logging.debug(f"{self._alpha = }")
+            logger.debug(f"{self._alpha = }")
             self._UMR = None
 
     @property
     def x0(self) -> float:
         """Coordinate offset."""
         # todo: x0.setter -> update alpha
         #  x0max = np.min(self.l)
@@ -2405,59 +2418,59 @@
         return self._grid
 
     @grid.setter
     def grid(self, grid: str):
         _grid = str(grid)
 
         if (self.SDM or self.uwr == "FTM") and self.grid not in self._grids[:2]:
-            logging.error(f"Couldn't set 'grid': grid not in {self._grids[:2]}'.")
+            logger.error(f"Couldn't set 'grid': grid not in {self._grids[:2]}'.")
             return
 
         if self._grid != _grid and _grid in self._grids:
             self._grid = _grid
-            logging.debug(f"{self._grid = }")
+            logger.debug(f"{self._grid = }")
             self.SDM = self.SDM
 
     @property
     def angle(self) -> float:
         """Angle of the coordinate system's principal axis."""
         return self._angle
 
     @angle.setter
     def angle(self, angle: float):
         _angle = float(np.remainder(angle, 360))  # todo: +- 45
 
         if self._angle != _angle:
             self._angle = _angle
-            logging.debug(f"{self._angle = }")
+            logger.debug(f"{self._angle = }")
 
     @property
     def D(self) -> int:
         """Number of directions."""
         return self._D
 
     @D.setter
     def D(self, D: int):
         _D = int(min(max(1, D), self._Dmax))
 
         if self._D > _D:
             self._D = _D
-            logging.debug(f"{self._D = }")
+            logger.debug(f"{self._D = }")
 
             self.N = self._N[: self.D, :]
             self.v = self._v[: self.D, :]
             self.f = self._f[: self.D, :]
 
             if self._D == self._K == 1:
                 self.FDM = False
 
             self.SDM = False
         elif self._D < _D:
             self._D = _D
-            logging.debug(f"{self._D = }")
+            logger.debug(f"{self._D = }")
 
             self.N = np.append(self._N, np.tile(self._N[-1, :], (_D - self._N.shape[0], 1)), axis=0)
             self.v = np.append(self._v, np.tile(self._v[-1, :], (_D - self._v.shape[0], 1)), axis=0)
             self.f = np.append(self._f, np.tile(self._f[-1, :], (_D - self._f.shape[0], 1)), axis=0)
 
             self.B = self.B
 
@@ -2470,15 +2483,15 @@
 
     @axis.setter
     def axis(self, axis: int):
         _axis = int(min(max(0, axis), 1))
 
         if self._axis != _axis:
             self._axis = _axis
-            logging.debug(f"{self._axis = }")
+            logger.debug(f"{self._axis = }")
             self._UMR = None
 
     @property
     def _M(self) -> np.ndarray:
         """Number of averaged intensity samples."""
         M = np.sum(self.h, axis=0) / 255
         return np.atleast_1d(M[0]) if self._monochrome else M
@@ -2511,15 +2524,15 @@
         return self.h.shape[0]
 
     @H.setter
     def H(self, H: int):
         _H = int(min(max(1, H), self._Hmax))
 
         # if self.WDM:
-        #     logging.error("Couldn't set 'H': WDM is active.")
+        #     logger.error("Couldn't set 'H': WDM is active.")
         #     return
 
         if self.H != _H:
             if self.WDM:
                 self.h = "w" * _H
             elif _H == 1:
                 self.h = "w"
@@ -2582,32 +2595,32 @@
             _h = np.vstack([_h[:3] for h in range(self.H)])
         elif _h.ndim == 2:
             _h = _h[: self._Hmax, :3]
         else:
             _h = _h[: self._Hmax, :3, ..., -1]
 
         if _h.shape[1] == 2:  # C-axis must equal 3
-            logging.error("Couldn't set 'h': Only 2 instead of 3 color channels provided.")
+            logger.error("Couldn't set 'h': Only 2 instead of 3 color channels provided.")
             return
 
         if np.any(np.max(_h, axis=1) == 0):
-            logging.error("Didn't set 'h': Black color is not allowed.")
+            logger.error("Didn't set 'h': Black color is not allowed.")
             return
 
         if self.WDM and not self._monochrome:
-            logging.error("Couldn't set 'h': 'WDM' is active, but not all hues are monochromatic.")
+            logger.error("Couldn't set 'h': 'WDM' is active, but not all hues are monochromatic.")
             return
 
         if not np.array_equal(self._h, _h):
             Hold = self.H
             self._h = _h
-            logging.debug(f"self._h = {str(self._h).replace(chr(10), ',')}")
+            logger.debug(f"self._h = {str(self._h).replace(chr(10), ',')}")
             if Hold != _h.shape[0]:
-                logging.debug(f"self.H = {_h.shape[0]}")  # computed upon call
-            logging.debug(f"{self.M = }")  # computed upon call
+                logger.debug(f"self.H = {_h.shape[0]}")  # computed upon call
+            logger.debug(f"{self.M = }")  # computed upon call
 
     @property
     def TDM(self) -> bool:
         """Temporal division multiplexing."""
         return self.T > 1
 
     @property
@@ -2623,28 +2636,28 @@
     @SDM.setter
     def SDM(self, SDM: bool):
         _SDM = bool(SDM)
 
         if _SDM:
             if self.D != 2:
                 _SDM = False
-                logging.error("Didn't set 'SDM': Pointless as only one dimension exist.")
+                logger.error("Didn't set 'SDM': Pointless as only one dimension exist.")
 
             if self.grid not in self._grids[:2]:
                 _SDM = False
-                logging.error(f"Couldn't set 'SDM': grid not in {self._grids[:2]}'.")
+                logger.error(f"Couldn't set 'SDM': grid not in {self._grids[:2]}'.")
 
             if self.FDM:
                 _SDM = False
-                logging.error("Couldn't set 'SDM': FDM is active.")
+                logger.error("Couldn't set 'SDM': FDM is active.")
 
         if self._SDM != _SDM:
             self._SDM = _SDM
-            logging.debug(f"{self._SDM = }")
-            logging.debug(f"{self.T = }")  # computed upon call
+            logger.debug(f"{self._SDM = }")
+            logger.debug(f"{self.T = }")  # computed upon call
 
             if self.SDM:
                 self.B /= self.D
             else:
                 self.B *= self.D
 
     @property
@@ -2659,28 +2672,28 @@
     @WDM.setter
     def WDM(self, WDM: bool):
         _WDM = bool(WDM)
 
         if _WDM:
             if not np.all(self.N == 3):
                 _WDM = False
-                logging.error("Couldn't set 'WDM': At least one Shift != 3.")
+                logger.error("Couldn't set 'WDM': At least one Shift != 3.")
 
             if not self._monochrome:
                 _WDM = False
-                logging.error("Couldn't set 'WDM': Not all hues are monochromatic.")
+                logger.error("Couldn't set 'WDM': Not all hues are monochromatic.")
 
             if self.FDM:  # todo: remove this, already covered by N
                 _WDM = False
-                logging.error("Couldn't set 'WDM': FDM is active.")
+                logger.error("Couldn't set 'WDM': FDM is active.")
 
         if self._WDM != _WDM:
             self._WDM = _WDM
-            logging.debug(f"{self._WDM = }")
-            logging.debug(f"{self.T = }")  # computed upon call
+            logger.debug(f"{self._WDM = }")
+            logger.debug(f"{self.T = }")  # computed upon call
 
     @property
     def FDM(self) -> bool:
         """Frequency division multiplexing.
 
         The directions D and the sets K are multiplexed, resulting in a crossed fringe pattern if D ≡ 2.
         It can only be activated if D ∨ K > 1 i.e. D * K > 1.
@@ -2697,27 +2710,27 @@
     @FDM.setter
     def FDM(self, FDM: bool):
         _FDM = bool(FDM)
 
         if _FDM:
             if self.D == self.K == 1:
                 _FDM = False
-                logging.error("Didn't set 'FDM': Dimensions * Sets = 1, so nothing to multiplex.")
+                logger.error("Didn't set 'FDM': Dimensions * Sets = 1, so nothing to multiplex.")
 
             if self.SDM:
                 _FDM = False
-                logging.error("Couldn't set 'FDM': SDM is active.")
+                logger.error("Couldn't set 'FDM': SDM is active.")
 
             if self.WDM:  # todo: remove, already covered by N
                 _FDM = False
-                logging.error("Couldn't set 'FDM': WDM is active.")
+                logger.error("Couldn't set 'FDM': WDM is active.")
 
         if self._FDM != _FDM:
             self._FDM = _FDM
-            logging.debug(f"{self._FDM = }")
+            logger.debug(f"{self._FDM = }")
             # self.K = self._K
             self.N = self._N
             self.v = self._v
             if self.FDM:
                 self.f = self._f
             else:
                 self.f = np.ones((self.D, self.K))
@@ -2735,15 +2748,15 @@
 
     @static.setter
     def static(self, static: bool):
         _static = bool(static)
 
         if self._static != _static:
             self._static = _static
-            logging.debug(f"{self._static = }")
+            logger.debug(f"{self._static = }")
             self.v = self._v
             self.f = self._f
 
     @property
     def K(self) -> int:
         """Number of sets (number of fringe patterns with different spatial frequencies)."""
         return self._K
@@ -2756,25 +2769,25 @@
         # c = np.array([a, b])
 
         Kmax = (self._Nmax - 1) / 2 / self.D if self.FDM else self._Kmax  # todo: check if necessary
         _K = int(min(max(1, K), Kmax))
 
         if self._K > _K:  # remove elements
             self._K = _K
-            logging.debug(f"{self._K = }")
+            logger.debug(f"{self._K = }")
 
             self.N = self._N[:, : self.K]
             self.v = self._v[:, : self.K]
             self.f = self._f[:, : self.K]
 
             if self._D == self._K == 1:
                 self.FDM = False
         elif self._K < _K:  # add elements
             self._K = _K
-            logging.debug(f"{self._K = }")
+            logger.debug(f"{self._K = }")
 
             self.N = np.append(
                 self._N, np.tile(self._N[0, 0], (self.D, _K - self._N.shape[1])), axis=1
             )  # don't append N from defaults, this might be in conflict with WDM!
             v = self.L ** (1 / np.arange(self._v.shape[1] + 1, _K + 1))
             self.v = np.append(self._v, np.tile(v, (self.D, 1)), axis=1)
             self.f = np.append(
@@ -2821,27 +2834,27 @@
         elif np.any(_N <= 2):
             for d in range(self.D):
                 if not any(_N[d] >= 3):
                     i = np.argmax(_N[d])  # np.argmin(_N[d])
                     _N[d, i] = 3
 
         if self.WDM and not np.all(_N == 3):
-            logging.error("Couldn't set 'N': At least one Shift != 3.")
+            logger.error("Couldn't set 'N': At least one Shift != 3.")
             return
 
         if self.FDM and not np.all(_N == _N[0, 0]):
             # _N = np.tile(self._Nmin, _N.shape)
             _N = np.tile(_N[0, 0], _N.shape)
 
         if not np.array_equal(self._N, _N):
             self._N = _N
-            logging.debug(f"self._N = {str(self._N).replace(chr(10), ',')}")
+            logger.debug(f"self._N = {str(self._N).replace(chr(10), ',')}")
             self._UMR = None
             self.D, self.K = self._N.shape
-            logging.debug(f"{self.T = }")
+            logger.debug(f"{self.T = }")
 
     @property
     def lmin(self) -> float:
         """Minimum resolvable wavelength.
         [lmin] = px."""
 
         # don't use self._fmax, else circular loop
@@ -2853,16 +2866,16 @@
 
     @lmin.setter
     def lmin(self, lmin: float):
         _lmin = float(max(self._lminmin, lmin))
 
         if self._lmin != _lmin:
             self._lmin = _lmin
-            logging.debug(f"{self._lmin = }")
-            logging.debug(f"{self.vmax = }")  # computed upon call
+            logger.debug(f"{self._lmin = }")
+            logger.debug(f"{self.vmax = }")  # computed upon call
             self.l = self.l  # l triggers v
 
     @property
     def lopt(self) -> float:
         """Optimal wavelength for minimal decoding uncertainty.
         [lopt] = px."""
         return self.L / self.vopt
@@ -3089,25 +3102,25 @@
                 ):  # todo: allow coprimes?!
                     n = min(10, self.vmax // 2)
                     ith = self.D * self.K
                     pmax = sympy.ntheory.generate.nextprime(n, ith + 1)
                     p = np.array(list(sympy.ntheory.generate.primerange(n, pmax + 1)))[:ith]  # primes
                     p = [p[-i // 2] if i % 2 else p[i // 2] for i in range(len(p))]  # resort primes
                     _v = np.sort(np.array(p, float).reshape((self.D, self.K)), axis=1)  # resort primes
-                    logging.warning(
+                    logger.warning(
                         f"Periods were not coprime. " f"Changing values to {str(_v.round(3)).replace(chr(10), ',')}."
                     )
             # else:
             #     vmax = (self._Nmax - 1) / 2 > _v
             #     _v = np.minimum(_v, vmax)
 
         if not np.array_equal(self._v, _v):
             self._v = _v
-            logging.debug(f"self.v = {str(self._v.round(3)).replace(chr(10), ',')}")
-            logging.debug(f"self.l = {str(self._l.round(3)).replace(chr(10), ',')}")
+            logger.debug(f"self.v = {str(self._v.round(3)).replace(chr(10), ',')}")
+            logger.debug(f"self.l = {str(self._l.round(3)).replace(chr(10), ',')}")
             self._UMR = None
             self.D, self.K = self._v.shape
             self.f = self._f
 
     @property
     def _fmax(self):
         """Maximum temporal frequency (maximum number of periods to shift over)."""
@@ -3146,15 +3159,15 @@
                     or not np.all(i % 1 == 0 for i in _f)
                     or len(np.unique(np.abs(_f))) < _f.size
                 ):  # assure _f are int and absolute values of _f differ
                     _f = np.arange(1, self.D * self.K + 1, dtype=float).reshape((self.D, self.K))
 
         if 0 not in _f and not np.array_equal(self._f, _f):
             self._f = _f
-            logging.debug(f"self._f = {str((self._f * (-1 if self.reverse else 1)).round(3)).replace(chr(10), ',')}")
+            logger.debug(f"self._f = {str((self._f * (-1 if self.reverse else 1)).round(3)).replace(chr(10), ',')}")
             self.D, self.K = self._f.shape
             self.N = self._N  # todo: remove if fractional periods is implemented, log warning
 
     @property
     def p0(self) -> float:
         """Phase offset within interval (-2pi, +2pi).
 
@@ -3164,28 +3177,28 @@
 
     @p0.setter
     def p0(self, p0: float):
         _p0 = float(np.abs(p0) % (2 * np.pi) * np.sign(p0))
 
         if self._p0 != _p0:
             self._p0 = _p0
-            logging.debug(f"self._p0 = {self._p0 / np.pi} PI")
+            logger.debug(f"self._p0 = {self._p0 / np.pi} PI")
 
     @property
     def Bv(self) -> np.ndarray:
         """Modulation at spatial frequencies `v`.
 
         The modulation values are determined from a measurement."""
         return self._Bv
 
     @Bv.setter
     def Bv(self, B: np.ndarray):
         if B is None:
             self._Bv = None
-            logging.debug(f"self.Bv = {self._Bv}")
+            logger.debug(f"self.Bv = {self._Bv}")
             return
 
         _B = np.array(np.maximum(0, B), float)
 
         _B.shape = T, Y, X, C = vshape(_B).shape
 
         assert T == self.D * self.K
@@ -3202,15 +3215,15 @@
         _B /= Bmax
         _B[np.isnan(_B)] = 0
 
         _Bv = np.vstack(_B, self._v)
 
         if not np.array_equal(self._Bv, _Bv):
             self._Bv = _B
-            logging.debug(f"self.Bv = {str(self.Bv.round(3)).replace(chr(10), ',')}")
+            logger.debug(f"self.Bv = {str(self.Bv.round(3)).replace(chr(10), ',')}")
 
     @property
     def _monochrome(self) -> bool:
         """True if all hues are monochromatic, i.e. the RGB values are identical for each hue."""
         return all(len(set(h)) == 1 for h in self.h)
 
     @property
@@ -3229,30 +3242,30 @@
 
     @indexing.setter
     def indexing(self, indexing):
         _indexing = str(indexing)
 
         if self._indexing != _indexing and _indexing in self._indexings:
             self._indexing = _indexing
-            logging.debug(f"{self._indexing = }")
+            logger.debug(f"{self._indexing = }")
             self._UMR = None
 
     @property
     def reverse(self) -> bool:
         """Flag for shifting fringes in reverse direction."""
         return self._reverse
 
     @reverse.setter
     def reverse(self, reverse: bool):
         _reverse = bool(reverse)
 
         if self._reverse != _reverse:
             self._reverse = _reverse
-            logging.debug(f"{self._reverse = }")
-            logging.debug(f"self._f = {str((self._f * (-1 if self.reverse else 1)).round(3)).replace(chr(10), ',')}")
+            logger.debug(f"{self._reverse = }")
+            logger.debug(f"self._f = {str((self._f * (-1 if self.reverse else 1)).round(3)).replace(chr(10), ',')}")
 
     @property
     def verbose(self) -> bool:
         """Flag for additionally returning intermediate and verbose results:\n
         - phase maps\n
         - residuals\n
         - fringe orders\n
@@ -3263,15 +3276,15 @@
 
     @verbose.setter
     def verbose(self, verbose: bool):
         _verbose = bool(verbose)
 
         if self._verbose != _verbose:
             self._verbose = _verbose
-            logging.debug(f"{self._verbose = }")
+            logger.debug(f"{self._verbose = }")
 
     @property
     def mode(self) -> str:
         """Mode for remapping.
 
         The following values can be set:\n
         - 'fast'\n
@@ -3281,15 +3294,15 @@
 
     @mode.setter
     def mode(self, mode: str):
         _mode = str(mode)
 
         if self._mode != _mode and _mode in self._modes:
             self._mode = _mode
-            logging.debug(f"{self._mode = }")
+            logger.debug(f"{self._mode = }")
 
     @property
     def uwr(self) -> str:
         """Phase unwrapping method."""
 
         if self.K == 1 and np.all(self._N == 1) and self.grid in self._grids[:2]:
             # todo: v >> 1, i.e. l ~ 8
@@ -3310,15 +3323,15 @@
 
     @gamma.setter
     def gamma(self, gamma: float):
         _gamma = float(min(max(0, gamma), self._gammamax))
 
         if self._gamma != _gamma and _gamma != 0:
             self._gamma = _gamma
-            logging.debug(f"{self._gamma = }")
+            logger.debug(f"{self._gamma = }")
 
     @property
     def shape(self) -> tuple[int]:
         """Shape of fringe pattern sequence in video shape (frames, height, with, color channels)."""
         return self.T, self.Y, self.X, self.C
 
     @property
@@ -3350,17 +3363,17 @@
 
     @dtype.setter
     def dtype(self, dtype: np.dtype | str):
         _dtype = np.dtype(dtype)
 
         if self._dtype != _dtype and str(_dtype) in self._dtypes:
             self._dtype = _dtype
-            logging.debug(f"{self._dtype = }")
-            logging.debug(f"self.A = {self.A}")
-            logging.debug(f"self.B = {self.B}")
+            logger.debug(f"{self._dtype = }")
+            logger.debug(f"self.A = {self.A}")
+            logger.debug(f"self.B = {self.B}")
 
     @property
     def Imax(self) -> int:
         """Maximum gray value."""
         return np.iinfo(self.dtype).max if self.dtype.kind in "ui" else 1
 
     @property
@@ -3380,15 +3393,15 @@
 
     @A.setter
     def A(self, A: float):
         _A = float(min(max(self._Amin, A), self._Amax))
 
         if self.A != _A:
             self.beta = _A / self.Imax
-            logging.debug(f"{self.A = }")
+            logger.debug(f"{self.A = }")
 
     @property
     def _Bmax(self):
         """Maximum amplitude."""
         return min(self.A, self.Imax - self.A) * self._Vmax
 
     @property
@@ -3398,15 +3411,15 @@
 
     @B.setter
     def B(self, B: float):
         _B = float(min(max(0, B), self._Bmax))
 
         if self.B != _B:  # and _B != 0:
             self.V = _B / self.A
-            logging.debug(f"{self.B = }")
+            logger.debug(f"{self.B = }")
 
     @property
     def _betamax(self):
         """Maximum relative bias (exposure)."""
         return 1 / (1 + self.V)
 
     @property
@@ -3416,15 +3429,15 @@
 
     @beta.setter
     def beta(self, beta) -> float:
         _beta = float(min(max(0, beta), self._betamax))
 
         if self._beta != _beta:
             self._beta = _beta
-            logging.debug(f"{self.beta = }")
+            logger.debug(f"{self.beta = }")
 
     @property
     def _Vmax(self):
         """Maximum visibility."""
         if self.FDM:
             return 1 / (self.D * self.K)
         elif self.SDM:
@@ -3439,42 +3452,42 @@
 
     @V.setter
     def V(self, V: float):
         _V = float(min(max(0, V), self._Vmax))
 
         if self._V != _V:
             self._V = _V
-            logging.debug(f"{self.V = }")
+            logger.debug(f"{self.V = }")
 
     @property
     def Vmin(self) -> float:
         """Minimum visibility for measurement to be valid."""
         return self._Vmin
 
     @Vmin.setter
     def Vmin(self, Vmin: float):
         _Vmin = float(min(max(0, Vmin), 1))
 
         if self._Vmin != _Vmin:
             self._Vmin = _Vmin
-            logging.debug(f"{self._Vmin = }")
+            logger.debug(f"{self._Vmin = }")
 
     @property
     def umax(self) -> float:
         """Standard deviation of maximum uncertainty for measurement to be valid.
         [umax] = px."""
         return self._umax
 
     @umax.setter
     def umax(self, umax: float):
         _umax = float(min(max(0, umax), self.L))  # todo: L / 2 due to circular distribution  # todo: R.max() / 2
 
         if self._umax != _umax:
             self._umax = _umax
-            logging.debug(f"{self._umax = }")
+            logger.debug(f"{self._umax = }")
 
     # @property
     # def r(self) -> int:
     #     """Number of quantization bits."""
     #     return 1 if self.dtype.kind in "b" else np.iinfo(
     #         self.dtype).bits if self.dtype.kind in "ui" else 10 ** np.finfo(self.dtype).precision
 
@@ -3507,15 +3520,15 @@
 
         # _dark = max(_dark, 0.49)  # todo: temporal noise is dominated by quantization noise ->
 
         _dark = max(0, _dark - self.quant)  # correct for quantization noise contained in dark noise measurement
 
         if self._dark != _dark:
             self._dark = _dark
-            logging.debug(f"{self._dark = }")
+            logger.debug(f"{self._dark = }")
 
     @property
     def shot(self) -> float:
         """Shot noise of digital camera (standard deviation).
         [shot] = DN."""
         A = self.A * self.MTF(0)  # todo: Paper from (!) includes B
         return np.sqrt(self.gain * max(0, A - self.y0)) if self.gain != 0 else 0  # average intensity is bias
@@ -3528,43 +3541,43 @@
 
     @gain.setter
     def gain(self, gain: float):
         _gain = min(max(0, gain), 1)
 
         if self._gain != _gain:
             self._gain = _gain
-            logging.debug(f"{self._gain = }")
+            logger.debug(f"{self._gain = }")
 
     @property
     def PSF(self) -> float:  # todo: magnification?
         """Standard deviation of Point Spread Function for defocus.
         [PSF] = px."""
         return self._PSF
 
     @PSF.setter
     def PSF(self, PSF):
         _PSF = float(max(0, PSF))
 
         if self._PSF != _PSF:
             self._PSF = _PSF
-            logging.debug(f"{self._PSF = }")
+            logger.debug(f"{self._PSF = }")
 
     @property
     def y0(self) -> float:
         """Dark signal.
         [y0] = DN"""
         return self._y0
 
     @y0.setter
     def y0(self, y0: int | float):
         _y0 = float(min(max(0, y0), self.Imax))
 
         if self._y0 != _y0:
             self._y0 = _y0
-            logging.debug(f"{self._y0 = }")
+            logger.debug(f"{self._y0 = }")
 
     @property
     def UMR(self) -> np.ndarray:
         """Unambiguous measurement range.
         [UMR] = px
 
         The coding is only unique within the interval [0, UMR); after that it repeats itself.
@@ -3627,29 +3640,27 @@
                 # estimate whether elements are rational or irrational
                 if Dl < precision or Dv < precision:  # rational numbers without integers
                     # extend lcm/gcd to rational numbers
 
                     if Dl <= Dv:
                         ls = l * 10**Dl  # wavelengths scaled
                         UMR[d] = np.lcm.reduce(ls.astype(int, copy=False)) / 10**Dl
-                        logging.debug("Extended lcm to rational numbers.")
+                        logger.debug("Extended lcm to rational numbers.")
                     else:
                         vs = v * 10**Dv  # spatial frequencies scaled
                         UMR[d] = self.L / (np.gcd.reduce(vs.astype(int, copy=False)) / 10**Dv)
-                        logging.debug("Extended gcd to rational numbers.")
+                        logger.debug("Extended gcd to rational numbers.")
                 else:  # irrational numbers or rational numbers with more digits than "precision"
                     UMR[d] = np.prod(l)
 
         self._UMR = UMR
-        logging.debug(f"self.UMR = {str(self._UMR)}")
+        logger.debug(f"self.UMR = {str(self._UMR)}")
 
         if self._ambiguous:
-            logging.warning(
-                "UMR < R. Unwrapping will not be spatially independent and only yield a relative phase map."
-            )
+            logger.warning("UMR < R. Unwrapping will not be spatially independent and only yield a relative phase map.")
 
         return self._UMR
 
     @property
     def eta(self) -> float:
         """Coding efficiency."""
         eta = self.R / self.UMR
@@ -3754,15 +3765,15 @@
                         break
                 else:
                     if not np.array_equal(v, params[k]):
                         break
         else:  # else clause executes only after the loop completes normally, i.e. did not encounter a break
             return
 
-        logging.warning(f"'{k}' got overwritten by interdependencies. Choose a consistent parameter set.")
+        logger.warning(f"'{k}' got overwritten by interdependencies. Choose a consistent parameter set.")
         self.params = params_old
 
     types: dict = dict(sorted(__init__.__annotations__.items()))
     """Types of 'params' values."""
 
     defaults: dict = dict(sorted(__init__.__kwdefaults__.items()))
     """Default values for `params`."""
@@ -3792,12 +3803,12 @@
     #     # because for the latter, names in class scope are not accessible
     #     if __k not in defaults and not __k.startswith("_") and isinstance(__v, property):
     #         __doc__ += f"\n{__k} : {type(__v)}"
     # __doc__ += "\ntypes : dict"
     # __doc__ += "\ndefaults : dict"
     # __doc__ += "\nglossary : dict"
     # __doc__ += f"\nlogger : Logger, default = logger.getLogger({__qualname__})"  # todo
-    # __doc__ += "\n    https://docs.python.org/3/library/logging.html#logger-objects"
+    # __doc__ += "\n    https://docs.python.org/3/library/logger.html#logger-objects"
     # __doc__ += "\n\nMethods\n-------"
     # __doc__ += f"\nencode\n    {encode.__doc__.splitlines()[0]}"
     # __doc__ += f"\ndecode\n    {decode.__doc__.splitlines()[0]}"
     del __k, __v
```

### Comparing `fringes-1.1.0/fringes/grid.py` & `fringes-1.1.1/fringes/grid.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+import logging
+
 import numpy as np
 
 # todo: import numba as nb
 
+logger = logging.getLogger(__name__)
+
 
 def img(Y: int = 720, X: int = 720, a: float = 0):
     yy, xx = np.indices((Y, X))
     return rot(xx, yy, a)
 
 
 def cart(Y: int = 720, X: int = 720, a: float = 0):
```

### Comparing `fringes-1.1.0/fringes/util.py` & `fringes-1.1.1/fringes/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+import logging
 import time
 import typing as tp
 import itertools as it
-import logging
 
 import numpy as np
 import numba as nb
 import scipy as sp
 
 # import sympy.ntheory.generate
 import skimage as ski
 import cv2
 
+logger = logging.getLogger(__name__)
+
 
 def vshape(data: np.ndarray) -> np.ndarray:
     """Standardizes the input data shape.
 
     Transforms video data into the standardized shape (T, Y, X, C), where
     T is number of frames, Y is height, X is width, and C is number of color channels.
 
@@ -385,14 +387,52 @@
 
                                 if not np.isnan(mod[yc, xc, c]):
                                     m = mod[yc, xc, c]
                                     src[ys, xs, c] += m
     return src
 
 
+@nb.jit(cache=True, nopython=True, nogil=True, parallel=True, fastmath=True)
+def _source(
+    src: np.ndarray,
+    B: np.ndarray,
+    xi: np.ndarray,
+    ii: list,
+) -> np.ndarray:
+    """Helper function for `source()`."""
+    Y, X = src.shape
+
+    for ys in range(Y):
+        for xs in range(X):
+            # j = np.ravel_multi_index((ys, xs), src.shape)  # not supported by numba
+            j = ys * X + xs
+            i = ii[j]
+
+            xr = xi[i, 0]  # returns a view
+            yr = xi[i, 1]  # returns a view
+            d = np.sqrt((xs - xr) ** 2 + (ys - yr) ** 2)  # distance
+
+            # inverse distance weighting using modified Shepard's method:
+            # https://en.wikipedia.org/wiki/Inverse_distance_weighting
+            w = 1 / (d**2)  # todo: use PSF as weights
+            w[d == 0] = 1
+            # w[d > R] = 0
+            w /= np.sum(w)  # todo: sum / avg / max of vals within R
+
+            if B is not None:
+                # v = np.sum(B[i] * w)
+                v = np.dot(B[i], w)
+            else:
+                v = np.sum(w)
+
+            src[ys, xs] = v
+
+    return src
+
+
 # # @nb.jit(cache=True, nopython=True, nogil=True, parallel=True, fastmath=True)  # todo
 # def filter(combos, K, L, lmin):
 #     kroot = L ** (1 / K)
 #     if lmin <= kroot:
 #         lcombos = np.array([l for l in combos if np.any(l > kroot) and np.lcm.reduce(l) >= L])
 #     else:
 #         lcombos = np.array([l for l in combos if np.lcm.reduce(l) >= L])
```

### Comparing `fringes-1.1.0/LICENSE.txt` & `fringes-1.1.1/LICENSE.txt`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,437 +1,437 @@
-Attribution-NonCommercial-ShareAlike 4.0 International
-
-=======================================================================
-
-Creative Commons Corporation ("Creative Commons") is not a law firm and
-does not provide legal services or legal advice. Distribution of
-Creative Commons public licenses does not create a lawyer-client or
-other relationship. Creative Commons makes its licenses and related
-information available on an "as-is" basis. Creative Commons gives no
-warranties regarding its licenses, any material licensed under their
-terms and conditions, or any related information. Creative Commons
-disclaims all liability for damages resulting from their use to the
-fullest extent possible.
-
-Using Creative Commons Public Licenses
-
-Creative Commons public licenses provide a standard set of terms and
-conditions that creators and other rights holders may use to share
-original works of authorship and other material subject to copyright
-and certain other rights specified in the public license below. The
-following considerations are for informational purposes only, are not
-exhaustive, and do not form part of our licenses.
-
-     Considerations for licensors: Our public licenses are
-     intended for use by those authorized to give the public
-     permission to use material in ways otherwise restricted by
-     copyright and certain other rights. Our licenses are
-     irrevocable. Licensors should read and understand the terms
-     and conditions of the license they choose before applying it.
-     Licensors should also secure all rights necessary before
-     applying our licenses so that the public can reuse the
-     material as expected. Licensors should clearly mark any
-     material not subject to the license. This includes other CC-
-     licensed material, or material used under an exception or
-     limitation to copyright. More considerations for licensors:
-	wiki.creativecommons.org/Considerations_for_licensors
-
-     Considerations for the public: By using one of our public
-     licenses, a licensor grants the public permission to use the
-     licensed material under specified terms and conditions. If
-     the licensor's permission is not necessary for any reason--for
-     example, because of any applicable exception or limitation to
-     copyright--then that use is not regulated by the license. Our
-     licenses grant only permissions under copyright and certain
-     other rights that a licensor has authority to grant. Use of
-     the licensed material may still be restricted for other
-     reasons, including because others have copyright or other
-     rights in the material. A licensor may make special requests,
-     such as asking that all changes be marked or described.
-     Although not required by our licenses, you are encouraged to
-     respect those requests where reasonable. More_considerations
-     for the public:
-	wiki.creativecommons.org/Considerations_for_licensees
-
-=======================================================================
-
-Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International
-Public License
-
-By exercising the Licensed Rights (defined below), You accept and agree
-to be bound by the terms and conditions of this Creative Commons
-Attribution-NonCommercial-ShareAlike 4.0 International Public License
-("Public License"). To the extent this Public License may be
-interpreted as a contract, You are granted the Licensed Rights in
-consideration of Your acceptance of these terms and conditions, and the
-Licensor grants You such rights in consideration of benefits the
-Licensor receives from making the Licensed Material available under
-these terms and conditions.
-
-
-Section 1 -- Definitions.
-
-  a. Adapted Material means material subject to Copyright and Similar
-     Rights that is derived from or based upon the Licensed Material
-     and in which the Licensed Material is translated, altered,
-     arranged, transformed, or otherwise modified in a manner requiring
-     permission under the Copyright and Similar Rights held by the
-     Licensor. For purposes of this Public License, where the Licensed
-     Material is a musical work, performance, or sound recording,
-     Adapted Material is always produced where the Licensed Material is
-     synched in timed relation with a moving image.
-
-  b. Adapter's License means the license You apply to Your Copyright
-     and Similar Rights in Your contributions to Adapted Material in
-     accordance with the terms and conditions of this Public License.
-
-  c. BY-NC-SA Compatible License means a license listed at
-     creativecommons.org/compatiblelicenses, approved by Creative
-     Commons as essentially the equivalent of this Public License.
-
-  d. Copyright and Similar Rights means copyright and/or similar rights
-     closely related to copyright including, without limitation,
-     performance, broadcast, sound recording, and Sui Generis Database
-     Rights, without regard to how the rights are labeled or
-     categorized. For purposes of this Public License, the rights
-     specified in Section 2(b)(1)-(2) are not Copyright and Similar
-     Rights.
-
-  e. Effective Technological Measures means those measures that, in the
-     absence of proper authority, may not be circumvented under laws
-     fulfilling obligations under Article 11 of the WIPO Copyright
-     Treaty adopted on December 20, 1996, and/or similar international
-     agreements.
-
-  f. Exceptions and Limitations means fair use, fair dealing, and/or
-     any other exception or limitation to Copyright and Similar Rights
-     that applies to Your use of the Licensed Material.
-
-  g. License Elements means the license attributes listed in the name
-     of a Creative Commons Public License. The License Elements of this
-     Public License are Attribution, NonCommercial, and ShareAlike.
-
-  h. Licensed Material means the artistic or literary work, database,
-     or other material to which the Licensor applied this Public
-     License.
-
-  i. Licensed Rights means the rights granted to You subject to the
-     terms and conditions of this Public License, which are limited to
-     all Copyright and Similar Rights that apply to Your use of the
-     Licensed Material and that the Licensor has authority to license.
-
-  j. Licensor means the individual(s) or entity(ies) granting rights
-     under this Public License.
-
-  k. NonCommercial means not primarily intended for or directed towards
-     commercial advantage or monetary compensation. For purposes of
-     this Public License, the exchange of the Licensed Material for
-     other material subject to Copyright and Similar Rights by digital
-     file-sharing or similar means is NonCommercial provided there is
-     no payment of monetary compensation in connection with the
-     exchange.
-
-  l. Share means to provide material to the public by any means or
-     process that requires permission under the Licensed Rights, such
-     as reproduction, public display, public performance, distribution,
-     dissemination, communication, or importation, and to make material
-     available to the public including in ways that members of the
-     public may access the material from a place and at a time
-     individually chosen by them.
-
-  m. Sui Generis Database Rights means rights other than copyright
-     resulting from Directive 96/9/EC of the European Parliament and of
-     the Council of 11 March 1996 on the legal protection of databases,
-     as amended and/or succeeded, as well as other essentially
-     equivalent rights anywhere in the world.
-
-  n. You means the individual or entity exercising the Licensed Rights
-     under this Public License. Your has a corresponding meaning.
-
-
-Section 2 -- Scope.
-
-  a. License grant.
-
-       1. Subject to the terms and conditions of this Public License,
-          the Licensor hereby grants You a worldwide, royalty-free,
-          non-sublicensable, non-exclusive, irrevocable license to
-          exercise the Licensed Rights in the Licensed Material to:
-
-            a. reproduce and Share the Licensed Material, in whole or
-               in part, for NonCommercial purposes only; and
-
-            b. produce, reproduce, and Share Adapted Material for
-               NonCommercial purposes only.
-
-       2. Exceptions and Limitations. For the avoidance of doubt, where
-          Exceptions and Limitations apply to Your use, this Public
-          License does not apply, and You do not need to comply with
-          its terms and conditions.
-
-       3. Term. The term of this Public License is specified in Section
-          6(a).
-
-       4. Media and formats; technical modifications allowed. The
-          Licensor authorizes You to exercise the Licensed Rights in
-          all media and formats whether now known or hereafter created,
-          and to make technical modifications necessary to do so. The
-          Licensor waives and/or agrees not to assert any right or
-          authority to forbid You from making technical modifications
-          necessary to exercise the Licensed Rights, including
-          technical modifications necessary to circumvent Effective
-          Technological Measures. For purposes of this Public License,
-          simply making modifications authorized by this Section 2(a)
-          (4) never produces Adapted Material.
-
-       5. Downstream recipients.
-
-            a. Offer from the Licensor -- Licensed Material. Every
-               recipient of the Licensed Material automatically
-               receives an offer from the Licensor to exercise the
-               Licensed Rights under the terms and conditions of this
-               Public License.
-
-            b. Additional offer from the Licensor -- Adapted Material.
-               Every recipient of Adapted Material from You
-               automatically receives an offer from the Licensor to
-               exercise the Licensed Rights in the Adapted Material
-               under the conditions of the Adapter's License You apply.
-
-            c. No downstream restrictions. You may not offer or impose
-               any additional or different terms or conditions on, or
-               apply any Effective Technological Measures to, the
-               Licensed Material if doing so restricts exercise of the
-               Licensed Rights by any recipient of the Licensed
-               Material.
-
-       6. No endorsement. Nothing in this Public License constitutes or
-          may be construed as permission to assert or imply that You
-          are, or that Your use of the Licensed Material is, connected
-          with, or sponsored, endorsed, or granted official status by,
-          the Licensor or others designated to receive attribution as
-          provided in Section 3(a)(1)(A)(i).
-
-  b. Other rights.
-
-       1. Moral rights, such as the right of integrity, are not
-          licensed under this Public License, nor are publicity,
-          privacy, and/or other similar personality rights; however, to
-          the extent possible, the Licensor waives and/or agrees not to
-          assert any such rights held by the Licensor to the limited
-          extent necessary to allow You to exercise the Licensed
-          Rights, but not otherwise.
-
-       2. Patent and trademark rights are not licensed under this
-          Public License.
-
-       3. To the extent possible, the Licensor waives any right to
-          collect royalties from You for the exercise of the Licensed
-          Rights, whether directly or through a collecting society
-          under any voluntary or waivable statutory or compulsory
-          licensing scheme. In all other cases the Licensor expressly
-          reserves any right to collect such royalties, including when
-          the Licensed Material is used other than for NonCommercial
-          purposes.
-
-
-Section 3 -- License Conditions.
-
-Your exercise of the Licensed Rights is expressly made subject to the
-following conditions.
-
-  a. Attribution.
-
-       1. If You Share the Licensed Material (including in modified
-          form), You must:
-
-            a. retain the following if it is supplied by the Licensor
-               with the Licensed Material:
-
-                 i. identification of the creator(s) of the Licensed
-                    Material and any others designated to receive
-                    attribution, in any reasonable manner requested by
-                    the Licensor (including by pseudonym if
-                    designated);
-
-                ii. a copyright notice;
-
-               iii. a notice that refers to this Public License;
-
-                iv. a notice that refers to the disclaimer of
-                    warranties;
-
-                 v. a URI or hyperlink to the Licensed Material to the
-                    extent reasonably practicable;
-
-            b. indicate if You modified the Licensed Material and
-               retain an indication of any previous modifications; and
-
-            c. indicate the Licensed Material is licensed under this
-               Public License, and include the text of, or the URI or
-               hyperlink to, this Public License.
-
-       2. You may satisfy the conditions in Section 3(a)(1) in any
-          reasonable manner based on the medium, means, and context in
-          which You Share the Licensed Material. For example, it may be
-          reasonable to satisfy the conditions by providing a URI or
-          hyperlink to a resource that includes the required
-          information.
-       3. If requested by the Licensor, You must remove any of the
-          information required by Section 3(a)(1)(A) to the extent
-          reasonably practicable.
-
-  b. ShareAlike.
-
-     In addition to the conditions in Section 3(a), if You Share
-     Adapted Material You produce, the following conditions also apply.
-
-       1. The Adapter's License You apply must be a Creative Commons
-          license with the same License Elements, this version or
-          later, or a BY-NC-SA Compatible License.
-
-       2. You must include the text of, or the URI or hyperlink to, the
-          Adapter's License You apply. You may satisfy this condition
-          in any reasonable manner based on the medium, means, and
-          context in which You Share Adapted Material.
-
-       3. You may not offer or impose any additional or different terms
-          or conditions on, or apply any Effective Technological
-          Measures to, Adapted Material that restrict exercise of the
-          rights granted under the Adapter's License You apply.
-
-
-Section 4 -- Sui Generis Database Rights.
-
-Where the Licensed Rights include Sui Generis Database Rights that
-apply to Your use of the Licensed Material:
-
-  a. for the avoidance of doubt, Section 2(a)(1) grants You the right
-     to extract, reuse, reproduce, and Share all or a substantial
-     portion of the contents of the database for NonCommercial purposes
-     only;
-
-  b. if You include all or a substantial portion of the database
-     contents in a database in which You have Sui Generis Database
-     Rights, then the database in which You have Sui Generis Database
-     Rights (but not its individual contents) is Adapted Material,
-     including for purposes of Section 3(b); and
-
-  c. You must comply with the conditions in Section 3(a) if You Share
-     all or a substantial portion of the contents of the database.
-
-For the avoidance of doubt, this Section 4 supplements and does not
-replace Your obligations under this Public License where the Licensed
-Rights include other Copyright and Similar Rights.
-
-
-Section 5 -- Disclaimer of Warranties and Limitation of Liability.
-
-  a. UNLESS OTHERWISE SEPARATELY UNDERTAKEN BY THE LICENSOR, TO THE
-     EXTENT POSSIBLE, THE LICENSOR OFFERS THE LICENSED MATERIAL AS-IS
-     AND AS-AVAILABLE, AND MAKES NO REPRESENTATIONS OR WARRANTIES OF
-     ANY KIND CONCERNING THE LICENSED MATERIAL, WHETHER EXPRESS,
-     IMPLIED, STATUTORY, OR OTHER. THIS INCLUDES, WITHOUT LIMITATION,
-     WARRANTIES OF TITLE, MERCHANTABILITY, FITNESS FOR A PARTICULAR
-     PURPOSE, NON-INFRINGEMENT, ABSENCE OF LATENT OR OTHER DEFECTS,
-     ACCURACY, OR THE PRESENCE OR ABSENCE OF ERRORS, WHETHER OR NOT
-     KNOWN OR DISCOVERABLE. WHERE DISCLAIMERS OF WARRANTIES ARE NOT
-     ALLOWED IN FULL OR IN PART, THIS DISCLAIMER MAY NOT APPLY TO YOU.
-
-  b. TO THE EXTENT POSSIBLE, IN NO EVENT WILL THE LICENSOR BE LIABLE
-     TO YOU ON ANY LEGAL THEORY (INCLUDING, WITHOUT LIMITATION,
-     NEGLIGENCE) OR OTHERWISE FOR ANY DIRECT, SPECIAL, INDIRECT,
-     INCIDENTAL, CONSEQUENTIAL, PUNITIVE, EXEMPLARY, OR OTHER LOSSES,
-     COSTS, EXPENSES, OR DAMAGES ARISING OUT OF THIS PUBLIC LICENSE OR
-     USE OF THE LICENSED MATERIAL, EVEN IF THE LICENSOR HAS BEEN
-     ADVISED OF THE POSSIBILITY OF SUCH LOSSES, COSTS, EXPENSES, OR
-     DAMAGES. WHERE A LIMITATION OF LIABILITY IS NOT ALLOWED IN FULL OR
-     IN PART, THIS LIMITATION MAY NOT APPLY TO YOU.
-
-  c. The disclaimer of warranties and limitation of liability provided
-     above shall be interpreted in a manner that, to the extent
-     possible, most closely approximates an absolute disclaimer and
-     waiver of all liability.
-
-
-Section 6 -- Term and Termination.
-
-  a. This Public License applies for the term of the Copyright and
-     Similar Rights licensed here. However, if You fail to comply with
-     this Public License, then Your rights under this Public License
-     terminate automatically.
-
-  b. Where Your right to use the Licensed Material has terminated under
-     Section 6(a), it reinstates:
-
-       1. automatically as of the date the violation is cured, provided
-          it is cured within 30 days of Your discovery of the
-          violation; or
-
-       2. upon express reinstatement by the Licensor.
-
-     For the avoidance of doubt, this Section 6(b) does not affect any
-     right the Licensor may have to seek remedies for Your violations
-     of this Public License.
-
-  c. For the avoidance of doubt, the Licensor may also offer the
-     Licensed Material under separate terms or conditions or stop
-     distributing the Licensed Material at any time; however, doing so
-     will not terminate this Public License.
-
-  d. Sections 1, 5, 6, 7, and 8 survive termination of this Public
-     License.
-
-
-Section 7 -- Other Terms and Conditions.
-
-  a. The Licensor shall not be bound by any additional or different
-     terms or conditions communicated by You unless expressly agreed.
-
-  b. Any arrangements, understandings, or agreements regarding the
-     Licensed Material not stated herein are separate from and
-     independent of the terms and conditions of this Public License.
-
-
-Section 8 -- Interpretation.
-
-  a. For the avoidance of doubt, this Public License does not, and
-     shall not be interpreted to, reduce, limit, restrict, or impose
-     conditions on any use of the Licensed Material that could lawfully
-     be made without permission under this Public License.
-
-  b. To the extent possible, if any provision of this Public License is
-     deemed unenforceable, it shall be automatically reformed to the
-     minimum extent necessary to make it enforceable. If the provision
-     cannot be reformed, it shall be severed from this Public License
-     without affecting the enforceability of the remaining terms and
-     conditions.
-
-  c. No term or condition of this Public License will be waived and no
-     failure to comply consented to unless expressly agreed to by the
-     Licensor.
-
-  d. Nothing in this Public License constitutes or may be interpreted
-     as a limitation upon, or waiver of, any privileges and immunities
-     that apply to the Licensor or You, including from the legal
-     processes of any jurisdiction or authority.
-
-=======================================================================
-
-Creative Commons is not a party to its public
-licenses. Notwithstanding, Creative Commons may elect to apply one of
-its public licenses to material it publishes and in those instances
-will be considered the “Licensor.” The text of the Creative Commons
-public licenses is dedicated to the public domain under the CC0 Public
-Domain Dedication. Except for the limited purpose of indicating that
-material is shared under a Creative Commons public license or as
-otherwise permitted by the Creative Commons policies published at
-creativecommons.org/policies, Creative Commons does not authorize the
-use of the trademark "Creative Commons" or any other trademark or logo
-of Creative Commons without its prior written consent including,
-without limitation, in connection with any unauthorized modifications
-to any of its public licenses or any other arrangements,
-understandings, or agreements concerning use of licensed material. For
-the avoidance of doubt, this paragraph does not form part of the
-public licenses.
-
+Attribution-NonCommercial-ShareAlike 4.0 International
+
+=======================================================================
+
+Creative Commons Corporation ("Creative Commons") is not a law firm and
+does not provide legal services or legal advice. Distribution of
+Creative Commons public licenses does not create a lawyer-client or
+other relationship. Creative Commons makes its licenses and related
+information available on an "as-is" basis. Creative Commons gives no
+warranties regarding its licenses, any material licensed under their
+terms and conditions, or any related information. Creative Commons
+disclaims all liability for damages resulting from their use to the
+fullest extent possible.
+
+Using Creative Commons Public Licenses
+
+Creative Commons public licenses provide a standard set of terms and
+conditions that creators and other rights holders may use to share
+original works of authorship and other material subject to copyright
+and certain other rights specified in the public license below. The
+following considerations are for informational purposes only, are not
+exhaustive, and do not form part of our licenses.
+
+     Considerations for licensors: Our public licenses are
+     intended for use by those authorized to give the public
+     permission to use material in ways otherwise restricted by
+     copyright and certain other rights. Our licenses are
+     irrevocable. Licensors should read and understand the terms
+     and conditions of the license they choose before applying it.
+     Licensors should also secure all rights necessary before
+     applying our licenses so that the public can reuse the
+     material as expected. Licensors should clearly mark any
+     material not subject to the license. This includes other CC-
+     licensed material, or material used under an exception or
+     limitation to copyright. More considerations for licensors:
+	wiki.creativecommons.org/Considerations_for_licensors
+
+     Considerations for the public: By using one of our public
+     licenses, a licensor grants the public permission to use the
+     licensed material under specified terms and conditions. If
+     the licensor's permission is not necessary for any reason--for
+     example, because of any applicable exception or limitation to
+     copyright--then that use is not regulated by the license. Our
+     licenses grant only permissions under copyright and certain
+     other rights that a licensor has authority to grant. Use of
+     the licensed material may still be restricted for other
+     reasons, including because others have copyright or other
+     rights in the material. A licensor may make special requests,
+     such as asking that all changes be marked or described.
+     Although not required by our licenses, you are encouraged to
+     respect those requests where reasonable. More_considerations
+     for the public:
+	wiki.creativecommons.org/Considerations_for_licensees
+
+=======================================================================
+
+Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International
+Public License
+
+By exercising the Licensed Rights (defined below), You accept and agree
+to be bound by the terms and conditions of this Creative Commons
+Attribution-NonCommercial-ShareAlike 4.0 International Public License
+("Public License"). To the extent this Public License may be
+interpreted as a contract, You are granted the Licensed Rights in
+consideration of Your acceptance of these terms and conditions, and the
+Licensor grants You such rights in consideration of benefits the
+Licensor receives from making the Licensed Material available under
+these terms and conditions.
+
+
+Section 1 -- Definitions.
+
+  a. Adapted Material means material subject to Copyright and Similar
+     Rights that is derived from or based upon the Licensed Material
+     and in which the Licensed Material is translated, altered,
+     arranged, transformed, or otherwise modified in a manner requiring
+     permission under the Copyright and Similar Rights held by the
+     Licensor. For purposes of this Public License, where the Licensed
+     Material is a musical work, performance, or sound recording,
+     Adapted Material is always produced where the Licensed Material is
+     synched in timed relation with a moving image.
+
+  b. Adapter's License means the license You apply to Your Copyright
+     and Similar Rights in Your contributions to Adapted Material in
+     accordance with the terms and conditions of this Public License.
+
+  c. BY-NC-SA Compatible License means a license listed at
+     creativecommons.org/compatiblelicenses, approved by Creative
+     Commons as essentially the equivalent of this Public License.
+
+  d. Copyright and Similar Rights means copyright and/or similar rights
+     closely related to copyright including, without limitation,
+     performance, broadcast, sound recording, and Sui Generis Database
+     Rights, without regard to how the rights are labeled or
+     categorized. For purposes of this Public License, the rights
+     specified in Section 2(b)(1)-(2) are not Copyright and Similar
+     Rights.
+
+  e. Effective Technological Measures means those measures that, in the
+     absence of proper authority, may not be circumvented under laws
+     fulfilling obligations under Article 11 of the WIPO Copyright
+     Treaty adopted on December 20, 1996, and/or similar international
+     agreements.
+
+  f. Exceptions and Limitations means fair use, fair dealing, and/or
+     any other exception or limitation to Copyright and Similar Rights
+     that applies to Your use of the Licensed Material.
+
+  g. License Elements means the license attributes listed in the name
+     of a Creative Commons Public License. The License Elements of this
+     Public License are Attribution, NonCommercial, and ShareAlike.
+
+  h. Licensed Material means the artistic or literary work, database,
+     or other material to which the Licensor applied this Public
+     License.
+
+  i. Licensed Rights means the rights granted to You subject to the
+     terms and conditions of this Public License, which are limited to
+     all Copyright and Similar Rights that apply to Your use of the
+     Licensed Material and that the Licensor has authority to license.
+
+  j. Licensor means the individual(s) or entity(ies) granting rights
+     under this Public License.
+
+  k. NonCommercial means not primarily intended for or directed towards
+     commercial advantage or monetary compensation. For purposes of
+     this Public License, the exchange of the Licensed Material for
+     other material subject to Copyright and Similar Rights by digital
+     file-sharing or similar means is NonCommercial provided there is
+     no payment of monetary compensation in connection with the
+     exchange.
+
+  l. Share means to provide material to the public by any means or
+     process that requires permission under the Licensed Rights, such
+     as reproduction, public display, public performance, distribution,
+     dissemination, communication, or importation, and to make material
+     available to the public including in ways that members of the
+     public may access the material from a place and at a time
+     individually chosen by them.
+
+  m. Sui Generis Database Rights means rights other than copyright
+     resulting from Directive 96/9/EC of the European Parliament and of
+     the Council of 11 March 1996 on the legal protection of databases,
+     as amended and/or succeeded, as well as other essentially
+     equivalent rights anywhere in the world.
+
+  n. You means the individual or entity exercising the Licensed Rights
+     under this Public License. Your has a corresponding meaning.
+
+
+Section 2 -- Scope.
+
+  a. License grant.
+
+       1. Subject to the terms and conditions of this Public License,
+          the Licensor hereby grants You a worldwide, royalty-free,
+          non-sublicensable, non-exclusive, irrevocable license to
+          exercise the Licensed Rights in the Licensed Material to:
+
+            a. reproduce and Share the Licensed Material, in whole or
+               in part, for NonCommercial purposes only; and
+
+            b. produce, reproduce, and Share Adapted Material for
+               NonCommercial purposes only.
+
+       2. Exceptions and Limitations. For the avoidance of doubt, where
+          Exceptions and Limitations apply to Your use, this Public
+          License does not apply, and You do not need to comply with
+          its terms and conditions.
+
+       3. Term. The term of this Public License is specified in Section
+          6(a).
+
+       4. Media and formats; technical modifications allowed. The
+          Licensor authorizes You to exercise the Licensed Rights in
+          all media and formats whether now known or hereafter created,
+          and to make technical modifications necessary to do so. The
+          Licensor waives and/or agrees not to assert any right or
+          authority to forbid You from making technical modifications
+          necessary to exercise the Licensed Rights, including
+          technical modifications necessary to circumvent Effective
+          Technological Measures. For purposes of this Public License,
+          simply making modifications authorized by this Section 2(a)
+          (4) never produces Adapted Material.
+
+       5. Downstream recipients.
+
+            a. Offer from the Licensor -- Licensed Material. Every
+               recipient of the Licensed Material automatically
+               receives an offer from the Licensor to exercise the
+               Licensed Rights under the terms and conditions of this
+               Public License.
+
+            b. Additional offer from the Licensor -- Adapted Material.
+               Every recipient of Adapted Material from You
+               automatically receives an offer from the Licensor to
+               exercise the Licensed Rights in the Adapted Material
+               under the conditions of the Adapter's License You apply.
+
+            c. No downstream restrictions. You may not offer or impose
+               any additional or different terms or conditions on, or
+               apply any Effective Technological Measures to, the
+               Licensed Material if doing so restricts exercise of the
+               Licensed Rights by any recipient of the Licensed
+               Material.
+
+       6. No endorsement. Nothing in this Public License constitutes or
+          may be construed as permission to assert or imply that You
+          are, or that Your use of the Licensed Material is, connected
+          with, or sponsored, endorsed, or granted official status by,
+          the Licensor or others designated to receive attribution as
+          provided in Section 3(a)(1)(A)(i).
+
+  b. Other rights.
+
+       1. Moral rights, such as the right of integrity, are not
+          licensed under this Public License, nor are publicity,
+          privacy, and/or other similar personality rights; however, to
+          the extent possible, the Licensor waives and/or agrees not to
+          assert any such rights held by the Licensor to the limited
+          extent necessary to allow You to exercise the Licensed
+          Rights, but not otherwise.
+
+       2. Patent and trademark rights are not licensed under this
+          Public License.
+
+       3. To the extent possible, the Licensor waives any right to
+          collect royalties from You for the exercise of the Licensed
+          Rights, whether directly or through a collecting society
+          under any voluntary or waivable statutory or compulsory
+          licensing scheme. In all other cases the Licensor expressly
+          reserves any right to collect such royalties, including when
+          the Licensed Material is used other than for NonCommercial
+          purposes.
+
+
+Section 3 -- License Conditions.
+
+Your exercise of the Licensed Rights is expressly made subject to the
+following conditions.
+
+  a. Attribution.
+
+       1. If You Share the Licensed Material (including in modified
+          form), You must:
+
+            a. retain the following if it is supplied by the Licensor
+               with the Licensed Material:
+
+                 i. identification of the creator(s) of the Licensed
+                    Material and any others designated to receive
+                    attribution, in any reasonable manner requested by
+                    the Licensor (including by pseudonym if
+                    designated);
+
+                ii. a copyright notice;
+
+               iii. a notice that refers to this Public License;
+
+                iv. a notice that refers to the disclaimer of
+                    warranties;
+
+                 v. a URI or hyperlink to the Licensed Material to the
+                    extent reasonably practicable;
+
+            b. indicate if You modified the Licensed Material and
+               retain an indication of any previous modifications; and
+
+            c. indicate the Licensed Material is licensed under this
+               Public License, and include the text of, or the URI or
+               hyperlink to, this Public License.
+
+       2. You may satisfy the conditions in Section 3(a)(1) in any
+          reasonable manner based on the medium, means, and context in
+          which You Share the Licensed Material. For example, it may be
+          reasonable to satisfy the conditions by providing a URI or
+          hyperlink to a resource that includes the required
+          information.
+       3. If requested by the Licensor, You must remove any of the
+          information required by Section 3(a)(1)(A) to the extent
+          reasonably practicable.
+
+  b. ShareAlike.
+
+     In addition to the conditions in Section 3(a), if You Share
+     Adapted Material You produce, the following conditions also apply.
+
+       1. The Adapter's License You apply must be a Creative Commons
+          license with the same License Elements, this version or
+          later, or a BY-NC-SA Compatible License.
+
+       2. You must include the text of, or the URI or hyperlink to, the
+          Adapter's License You apply. You may satisfy this condition
+          in any reasonable manner based on the medium, means, and
+          context in which You Share Adapted Material.
+
+       3. You may not offer or impose any additional or different terms
+          or conditions on, or apply any Effective Technological
+          Measures to, Adapted Material that restrict exercise of the
+          rights granted under the Adapter's License You apply.
+
+
+Section 4 -- Sui Generis Database Rights.
+
+Where the Licensed Rights include Sui Generis Database Rights that
+apply to Your use of the Licensed Material:
+
+  a. for the avoidance of doubt, Section 2(a)(1) grants You the right
+     to extract, reuse, reproduce, and Share all or a substantial
+     portion of the contents of the database for NonCommercial purposes
+     only;
+
+  b. if You include all or a substantial portion of the database
+     contents in a database in which You have Sui Generis Database
+     Rights, then the database in which You have Sui Generis Database
+     Rights (but not its individual contents) is Adapted Material,
+     including for purposes of Section 3(b); and
+
+  c. You must comply with the conditions in Section 3(a) if You Share
+     all or a substantial portion of the contents of the database.
+
+For the avoidance of doubt, this Section 4 supplements and does not
+replace Your obligations under this Public License where the Licensed
+Rights include other Copyright and Similar Rights.
+
+
+Section 5 -- Disclaimer of Warranties and Limitation of Liability.
+
+  a. UNLESS OTHERWISE SEPARATELY UNDERTAKEN BY THE LICENSOR, TO THE
+     EXTENT POSSIBLE, THE LICENSOR OFFERS THE LICENSED MATERIAL AS-IS
+     AND AS-AVAILABLE, AND MAKES NO REPRESENTATIONS OR WARRANTIES OF
+     ANY KIND CONCERNING THE LICENSED MATERIAL, WHETHER EXPRESS,
+     IMPLIED, STATUTORY, OR OTHER. THIS INCLUDES, WITHOUT LIMITATION,
+     WARRANTIES OF TITLE, MERCHANTABILITY, FITNESS FOR A PARTICULAR
+     PURPOSE, NON-INFRINGEMENT, ABSENCE OF LATENT OR OTHER DEFECTS,
+     ACCURACY, OR THE PRESENCE OR ABSENCE OF ERRORS, WHETHER OR NOT
+     KNOWN OR DISCOVERABLE. WHERE DISCLAIMERS OF WARRANTIES ARE NOT
+     ALLOWED IN FULL OR IN PART, THIS DISCLAIMER MAY NOT APPLY TO YOU.
+
+  b. TO THE EXTENT POSSIBLE, IN NO EVENT WILL THE LICENSOR BE LIABLE
+     TO YOU ON ANY LEGAL THEORY (INCLUDING, WITHOUT LIMITATION,
+     NEGLIGENCE) OR OTHERWISE FOR ANY DIRECT, SPECIAL, INDIRECT,
+     INCIDENTAL, CONSEQUENTIAL, PUNITIVE, EXEMPLARY, OR OTHER LOSSES,
+     COSTS, EXPENSES, OR DAMAGES ARISING OUT OF THIS PUBLIC LICENSE OR
+     USE OF THE LICENSED MATERIAL, EVEN IF THE LICENSOR HAS BEEN
+     ADVISED OF THE POSSIBILITY OF SUCH LOSSES, COSTS, EXPENSES, OR
+     DAMAGES. WHERE A LIMITATION OF LIABILITY IS NOT ALLOWED IN FULL OR
+     IN PART, THIS LIMITATION MAY NOT APPLY TO YOU.
+
+  c. The disclaimer of warranties and limitation of liability provided
+     above shall be interpreted in a manner that, to the extent
+     possible, most closely approximates an absolute disclaimer and
+     waiver of all liability.
+
+
+Section 6 -- Term and Termination.
+
+  a. This Public License applies for the term of the Copyright and
+     Similar Rights licensed here. However, if You fail to comply with
+     this Public License, then Your rights under this Public License
+     terminate automatically.
+
+  b. Where Your right to use the Licensed Material has terminated under
+     Section 6(a), it reinstates:
+
+       1. automatically as of the date the violation is cured, provided
+          it is cured within 30 days of Your discovery of the
+          violation; or
+
+       2. upon express reinstatement by the Licensor.
+
+     For the avoidance of doubt, this Section 6(b) does not affect any
+     right the Licensor may have to seek remedies for Your violations
+     of this Public License.
+
+  c. For the avoidance of doubt, the Licensor may also offer the
+     Licensed Material under separate terms or conditions or stop
+     distributing the Licensed Material at any time; however, doing so
+     will not terminate this Public License.
+
+  d. Sections 1, 5, 6, 7, and 8 survive termination of this Public
+     License.
+
+
+Section 7 -- Other Terms and Conditions.
+
+  a. The Licensor shall not be bound by any additional or different
+     terms or conditions communicated by You unless expressly agreed.
+
+  b. Any arrangements, understandings, or agreements regarding the
+     Licensed Material not stated herein are separate from and
+     independent of the terms and conditions of this Public License.
+
+
+Section 8 -- Interpretation.
+
+  a. For the avoidance of doubt, this Public License does not, and
+     shall not be interpreted to, reduce, limit, restrict, or impose
+     conditions on any use of the Licensed Material that could lawfully
+     be made without permission under this Public License.
+
+  b. To the extent possible, if any provision of this Public License is
+     deemed unenforceable, it shall be automatically reformed to the
+     minimum extent necessary to make it enforceable. If the provision
+     cannot be reformed, it shall be severed from this Public License
+     without affecting the enforceability of the remaining terms and
+     conditions.
+
+  c. No term or condition of this Public License will be waived and no
+     failure to comply consented to unless expressly agreed to by the
+     Licensor.
+
+  d. Nothing in this Public License constitutes or may be interpreted
+     as a limitation upon, or waiver of, any privileges and immunities
+     that apply to the Licensor or You, including from the legal
+     processes of any jurisdiction or authority.
+
+=======================================================================
+
+Creative Commons is not a party to its public
+licenses. Notwithstanding, Creative Commons may elect to apply one of
+its public licenses to material it publishes and in those instances
+will be considered the “Licensor.” The text of the Creative Commons
+public licenses is dedicated to the public domain under the CC0 Public
+Domain Dedication. Except for the limited purpose of indicating that
+material is shared under a Creative Commons public license or as
+otherwise permitted by the Creative Commons policies published at
+creativecommons.org/policies, Creative Commons does not authorize the
+use of the trademark "Creative Commons" or any other trademark or logo
+of Creative Commons without its prior written consent including,
+without limitation, in connection with any unauthorized modifications
+to any of its public licenses or any other arrangements,
+understandings, or agreements concerning use of licensed material. For
+the avoidance of doubt, this paragraph does not form part of the
+public licenses.
+
 Creative Commons may be contacted at creativecommons.org.
```

### Comparing `fringes-1.1.0/pyproject.toml` & `fringes-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Fringes"
-version = "1.1.0"
+version = "1.1.1"
 description = "Phase shifting algorithms for encoding and decoding sinusoidal fringe patterns."
 license = "CC-BY-NC-SA-4.0"
 authors = ["Christian Kludt"]
 readme = "README.md"
 repository = "https://github.com/comimag/fringes"
 documentation = "https://fringes.readthedocs.io"
 keywords = [
```

### Comparing `fringes-1.1.0/README.md` & `fringes-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fringes-1.1.0/PKG-INFO` & `fringes-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fringes
-Version: 1.1.0
+Version: 1.1.1
 Summary: Phase shifting algorithms for encoding and decoding sinusoidal fringe patterns.
 Home-page: https://github.com/comimag/fringes
 License: CC-BY-NC-SA-4.0
 Keywords: phase shifting,phase unwrapping,fringe analysis,fringe projection,deflectometry,computational imaging
 Author: Christian Kludt
 Requires-Python: >=3.9,<3.13
 Classifier: Intended Audience :: Education
```

