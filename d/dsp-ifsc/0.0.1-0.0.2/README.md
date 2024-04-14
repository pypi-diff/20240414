# Comparing `tmp/dsp_ifsc-0.0.1.tar.gz` & `tmp/dsp_ifsc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_ifsc-0.0.1.tar", max compression
+gzip compressed data, was "dsp_ifsc-0.0.2.tar", max compression
```

## Comparing `dsp_ifsc-0.0.1.tar` & `dsp_ifsc-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2024-03-11 13:26:20.040237 dsp_ifsc-0.0.1/LICENSE
--rw-r--r--   0        0        0      113 2024-03-11 14:15:29.553736 dsp_ifsc-0.0.1/README.md
--rw-r--r--   0        0        0      985 2024-03-11 13:50:12.624180 dsp_ifsc-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-11 13:30:38.984864 dsp_ifsc-0.0.1/src/__init__.py
--rw-r--r--   0        0        0     2278 2024-03-11 13:19:02.479601 dsp_ifsc-0.0.1/src/sequence.py
--rw-r--r--   0        0        0     3432 2024-03-11 13:18:46.582379 dsp_ifsc-0.0.1/src/signal.py
--rw-r--r--   0        0        0     1028 1970-01-01 00:00:00.000000 dsp_ifsc-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-03-11 13:26:20.040237 dsp_ifsc-0.0.2/LICENSE
+-rw-r--r--   0        0        0      113 2024-04-08 11:55:51.403524 dsp_ifsc-0.0.2/README.md
+-rw-r--r--   0        0        0      985 2024-04-14 20:15:49.660447 dsp_ifsc-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-14 19:56:23.845986 dsp_ifsc-0.0.2/src/__init__.py
+-rw-r--r--   0        0        0     2282 2024-04-14 19:58:51.072369 dsp_ifsc-0.0.2/src/sequence.py
+-rw-r--r--   0        0        0     6700 2024-04-14 20:04:31.269400 dsp_ifsc-0.0.2/src/signal.py
+-rw-r--r--   0        0        0     1028 1970-01-01 00:00:00.000000 dsp_ifsc-0.0.2/PKG-INFO
```

### Comparing `dsp_ifsc-0.0.1/LICENSE` & `dsp_ifsc-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_ifsc-0.0.1/pyproject.toml` & `dsp_ifsc-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project.urls]
 Homepage = "https://github.com/JoaoMario109/ifsc-dsp-2024"
 Issues = "https://github.com/JoaoMario109/ifsc-dsp-2024/issues"
 
 [tool.poetry]
 name = "dsp-ifsc"
-version = "0.0.1"
+version = "0.0.2"
 description = "A small package with some utilities for DSP grade at IFSC - Campus Florianópolis"
 authors = [
     "João Mário Lago <joao.mcil2003@aluno.ifsc.edu.br>",
     "Alejo Perdomo Milar <alejo.pm@aluno.ifsc.edu.br>"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `dsp_ifsc-0.0.1/src/sequence.py` & `dsp_ifsc-0.0.2/src/sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy
 from typing import Tuple
 
+
 def impulse(position: int, n_start: int, n_end: int) -> Tuple[numpy.ndarray, numpy.ndarray]:
     """
     Generates x(n) = delta(n - n0); n_start <= n <= n_end
     Args:
         position: The position of the impulse.
         n_start: The start of the sequence.
         n_end: The end of the sequence.
@@ -15,14 +16,15 @@
     """
 
     n = numpy.arange(n_start, n_end + 1)
     x = (n == position).astype(int)
 
     return x, n
 
+
 def step(position: int, n_start: int, n_end: int) -> Tuple[numpy.ndarray, numpy.ndarray]:
     """
     Generates x(n) = u(n - n0); n_start <= n <= n_end
     Args:
         position: The position of the step.
         n_start: The start of the sequence.
         n_end: The end of the sequence.
@@ -33,14 +35,15 @@
     """
 
     n = numpy.arange(n_start, n_end + 1)
     x = ((n - position) >= 0).astype(int)
 
     return x, n
 
+
 def ramp(slope: float, position: int, n_start: int, n_end: int) -> Tuple[numpy.ndarray, numpy.ndarray]:
     """
     Generates x(n) = (n - n0) * a; n_start <= n <= n_end
     Args:
         slope: The slope of the ramp.
         position: The position of the ramp.
         n_start: The start of the sequence.
@@ -52,14 +55,15 @@
     """
 
     n = numpy.arange(n_start, n_end + 1)
     x = (n - position) * slope
 
     return x, n
 
+
 def exponential(amplitude: float, decay: float, position: int, n_start: int, n_end: int) -> Tuple[numpy.ndarray, numpy.ndarray]:
     """
     Generates x(n) = a * exp(-b * (n - n0)); n_start <= n <= n_end
     Args:
         amplitude: The amplitude of the exponential.
         decay: The decay of the exponential.
         position: The position of the exponential.
```

### Comparing `dsp_ifsc-0.0.1/PKG-INFO` & `dsp_ifsc-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsp-ifsc
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small package with some utilities for DSP grade at IFSC - Campus Florianópolis
 Home-page: https://github.com/JoaoMario109/ifsc-dsp-2024
 License: MIT
 Author: João Mário Lago
 Author-email: joao.mcil2003@aluno.ifsc.edu.br
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

