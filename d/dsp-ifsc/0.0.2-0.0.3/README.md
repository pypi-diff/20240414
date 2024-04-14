# Comparing `tmp/dsp_ifsc-0.0.2.tar.gz` & `tmp/dsp_ifsc-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsp_ifsc-0.0.2.tar", max compression
+gzip compressed data, was "dsp_ifsc-0.0.3.tar", max compression
```

## Comparing `dsp_ifsc-0.0.2.tar` & `dsp_ifsc-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,4 @@
--rw-r--r--   0        0        0     1074 2024-03-11 13:26:20.040237 dsp_ifsc-0.0.2/LICENSE
--rw-r--r--   0        0        0      113 2024-04-08 11:55:51.403524 dsp_ifsc-0.0.2/README.md
--rw-r--r--   0        0        0      985 2024-04-14 20:15:49.660447 dsp_ifsc-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-14 19:56:23.845986 dsp_ifsc-0.0.2/src/__init__.py
--rw-r--r--   0        0        0     2282 2024-04-14 19:58:51.072369 dsp_ifsc-0.0.2/src/sequence.py
--rw-r--r--   0        0        0     6700 2024-04-14 20:04:31.269400 dsp_ifsc-0.0.2/src/signal.py
--rw-r--r--   0        0        0     1028 1970-01-01 00:00:00.000000 dsp_ifsc-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-03-11 13:26:20.040237 dsp_ifsc-0.0.3/LICENSE
+-rw-r--r--   0        0        0      113 2024-04-08 11:55:51.403524 dsp_ifsc-0.0.3/README.md
+-rw-r--r--   0        0        0      990 2024-04-14 20:35:35.153798 dsp_ifsc-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1028 1970-01-01 00:00:00.000000 dsp_ifsc-0.0.3/PKG-INFO
```

### Comparing `dsp_ifsc-0.0.2/LICENSE` & `dsp_ifsc-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dsp_ifsc-0.0.2/pyproject.toml` & `dsp_ifsc-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [project.urls]
 Homepage = "https://github.com/JoaoMario109/ifsc-dsp-2024"
 Issues = "https://github.com/JoaoMario109/ifsc-dsp-2024/issues"
 
 [tool.poetry]
 name = "dsp-ifsc"
-version = "0.0.2"
+version = "0.0.3"
 description = "A small package with some utilities for DSP grade at IFSC - Campus Florianópolis"
 authors = [
     "João Mário Lago <joao.mcil2003@aluno.ifsc.edu.br>",
     "Alejo Perdomo Milar <alejo.pm@aluno.ifsc.edu.br>"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 readme = "README.md"
 repository = "https://github.com/JoaoMario109/ifsc-dsp-2024"
 license = "MIT"
-packages = [{include = "src"}]
+packages = [{include = "dsp_ifsc"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 numpy = "*"
 
 [tool.poetry.urls]
 Homepage = "https://github.com/JoaoMario109/ifsc-dsp-2024"
```

### Comparing `dsp_ifsc-0.0.2/PKG-INFO` & `dsp_ifsc-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsp-ifsc
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small package with some utilities for DSP grade at IFSC - Campus Florianópolis
 Home-page: https://github.com/JoaoMario109/ifsc-dsp-2024
 License: MIT
 Author: João Mário Lago
 Author-email: joao.mcil2003@aluno.ifsc.edu.br
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

