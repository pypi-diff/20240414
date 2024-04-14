# Comparing `tmp/pykeops-2.2.2.tar.gz` & `tmp/pykeops-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykeops-2.2.2.tar", last modified: Fri Feb  9 16:48:59 2024, max compression
+gzip compressed data, was "pykeops-2.2.3.tar", last modified: Sun Apr 14 08:15:49 2024, max compression
```

## Comparing `pykeops-2.2.2.tar` & `pykeops-2.2.3.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:59.993191 pykeops-2.2.2/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)       37 2022-03-10 16:01:04.000000 pykeops-2.2.2/MANIFEST.in
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2775 2024-02-09 16:48:59.993191 pykeops-2.2.2/PKG-INFO
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1184 2024-01-18 14:06:08.000000 pykeops-2.2.2/licence.txt
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:59.986524 pykeops-2.2.2/pykeops/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2232 2023-02-22 10:18:06.000000 pykeops-2.2.2/pykeops/__init__.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:59.986524 pykeops-2.2.2/pykeops/common/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 pykeops-2.2.2/pykeops/common/__init__.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4548 2023-02-22 10:18:06.000000 pykeops-2.2.2/pykeops/common/get_options.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      106 2022-03-10 16:01:04.000000 pykeops-2.2.2/pykeops/common/gpu_utils.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:59.986524 pykeops-2.2.2/pykeops/common/keops_io/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     7668 2023-12-22 10:13:41.000000 pykeops-2.2.2/pykeops/common/keops_io/LoadKeOps.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     7344 2023-12-22 10:13:41.000000 pykeops-2.2.2/pykeops/common/keops_io/LoadKeOps_cpp.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     3133 2024-02-09 15:59:15.000000 pykeops-2.2.2/pykeops/common/keops_io/LoadKeOps_nvrtc.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      328 2022-03-15 15:17:07.000000 pykeops-2.2.2/pykeops/common/keops_io/__init__.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4476 2024-01-18 14:07:49.000000 pykeops-2.2.2/pykeops/common/keops_io/pykeops_nvrtc.cpp
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)   114903 2024-01-18 16:53:57.000000 pykeops-2.2.2/pykeops/common/lazy_tensor.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     8954 2023-12-22 10:13:41.000000 pykeops-2.2.2/pykeops/common/operations.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     8875 2023-12-22 10:13:41.000000 pykeops-2.2.2/pykeops/common/parse_type.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2727 2023-02-22 10:18:06.000000 pykeops-2.2.2/pykeops/common/utils.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1071 2024-02-07 09:31:44.000000 pykeops-2.2.2/pykeops/config.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        6 2024-02-07 09:49:43.000000 pykeops-2.2.2/pykeops/keops_version
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1184 2024-01-18 14:06:08.000000 pykeops-2.2.2/pykeops/licence.txt
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:59.986524 pykeops-2.2.2/pykeops/numpy/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      674 2023-04-04 07:06:57.000000 pykeops-2.2.2/pykeops/numpy/__init__.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:59.989857 pykeops-2.2.2/pykeops/numpy/cluster/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      476 2022-03-10 16:01:04.000000 pykeops-2.2.2/pykeops/numpy/cluster/__init__.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1528 2022-03-10 16:01:04.000000 pykeops-2.2.2/pykeops/numpy/cluster/grid_cluster.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     6439 2024-01-18 14:06:08.000000 pykeops-2.2.2/pykeops/numpy/cluster/matrix.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     8308 2022-03-10 16:01:04.000000 pykeops-2.2.2/pykeops/numpy/cluster/utils.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:59.989857 pykeops-2.2.2/pykeops/numpy/generic/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 pykeops-2.2.2/pykeops/numpy/generic/__init__.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    10003 2022-03-10 16:01:04.000000 pykeops-2.2.2/pykeops/numpy/generic/generic_ops.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    18353 2024-01-18 16:53:57.000000 pykeops-2.2.2/pykeops/numpy/generic/generic_red.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:59.989857 pykeops-2.2.2/pykeops/numpy/lazytensor/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2810 2022-03-10 16:01:04.000000 pykeops-2.2.2/pykeops/numpy/lazytensor/LazyTensor.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 pykeops-2.2.2/pykeops/numpy/lazytensor/__init__.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    12426 2024-01-18 15:47:38.000000 pykeops-2.2.2/pykeops/numpy/operations.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      700 2022-03-11 15:42:45.000000 pykeops-2.2.2/pykeops/numpy/test_install.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     6563 2023-03-27 09:23:23.000000 pykeops-2.2.2/pykeops/numpy/utils.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      858 2020-01-15 14:47:12.000000 pykeops-2.2.2/pykeops/readme.md
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:59.989857 pykeops-2.2.2/pykeops/test/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 pykeops-2.2.2/pykeops/test/__init__.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1467 2023-12-22 10:13:41.000000 pykeops-2.2.2/pykeops/test/conv2d.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1020 2022-03-11 15:42:45.000000 pykeops-2.2.2/pykeops/test/test_chunks.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1075 2022-03-11 15:42:45.000000 pykeops-2.2.2/pykeops/test/test_chunks_ranges.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1361 2022-03-11 15:42:45.000000 pykeops-2.2.2/pykeops/test/test_complex.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      656 2022-03-11 15:42:45.000000 pykeops-2.2.2/pykeops/test/test_complex_numpy.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      528 2022-03-11 15:42:45.000000 pykeops-2.2.2/pykeops/test/test_contiguous_numpy.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      554 2022-03-11 15:42:45.000000 pykeops-2.2.2/pykeops/test/test_contiguous_torch.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1050 2022-03-11 15:42:45.000000 pykeops-2.2.2/pykeops/test/test_finalchunks.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1075 2022-03-11 15:42:45.000000 pykeops-2.2.2/pykeops/test/test_finalchunks_ranges.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1290 2022-03-11 15:42:45.000000 pykeops-2.2.2/pykeops/test/test_float16.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1238 2022-03-11 15:42:45.000000 pykeops-2.2.2/pykeops/test/test_gpu_cpu.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     3879 2023-02-22 10:18:06.000000 pykeops-2.2.2/pykeops/test/test_kron.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1052 2023-02-22 10:18:06.000000 pykeops-2.2.2/pykeops/test/test_lazytensor_clamp.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1249 2022-03-11 15:42:45.000000 pykeops-2.2.2/pykeops/test/test_lazytensor_gaussian_batch.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1565 2022-03-11 15:42:45.000000 pykeops-2.2.2/pykeops/test/test_lazytensor_gaussian_cpu.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      947 2022-03-11 15:42:45.000000 pykeops-2.2.2/pykeops/test/test_lazytensor_gaussian_fromhost.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1098 2022-03-11 15:42:45.000000 pykeops-2.2.2/pykeops/test/test_lazytensor_gaussian_inplace.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      857 2022-03-11 15:42:45.000000 pykeops-2.2.2/pykeops/test/test_lazytensor_gaussian_numpy_inplace.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1456 2022-03-11 15:42:45.000000 pykeops-2.2.2/pykeops/test/test_lazytensor_grad.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      648 2022-03-11 15:42:45.000000 pykeops-2.2.2/pykeops/test/test_lazytensor_tensordot.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    10838 2023-02-22 10:18:06.000000 pykeops-2.2.2/pykeops/test/test_numpy.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      735 2024-01-25 11:52:46.000000 pykeops-2.2.2/pykeops/test/test_sinc.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    27731 2023-02-22 10:18:06.000000 pykeops-2.2.2/pykeops/test/test_torch.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2546 2024-01-25 12:48:13.000000 pykeops-2.2.2/pykeops/test/test_torch_func.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2296 2024-01-25 12:48:13.000000 pykeops-2.2.2/pykeops/test/test_torch_func_logsumexp.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      492 2024-01-25 11:52:46.000000 pykeops-2.2.2/pykeops/test/test_transpose.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2837 2024-01-25 12:48:13.000000 pykeops-2.2.2/pykeops/test/test_vmap.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:59.993191 pykeops-2.2.2/pykeops/torch/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      929 2023-12-22 10:13:41.000000 pykeops-2.2.2/pykeops/torch/__init__.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:59.993191 pykeops-2.2.2/pykeops/torch/cluster/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      476 2022-03-10 16:01:04.000000 pykeops-2.2.2/pykeops/torch/cluster/__init__.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1821 2023-02-22 10:18:06.000000 pykeops-2.2.2/pykeops/torch/cluster/grid_cluster.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     6985 2024-01-18 15:47:38.000000 pykeops-2.2.2/pykeops/torch/cluster/matrix.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     9220 2023-12-22 10:13:41.000000 pykeops-2.2.2/pykeops/torch/cluster/utils.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:59.993191 pykeops-2.2.2/pykeops/torch/generic/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 pykeops-2.2.2/pykeops/torch/generic/__init__.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     8959 2022-03-10 16:01:04.000000 pykeops-2.2.2/pykeops/torch/generic/generic_ops.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    31602 2024-01-25 11:52:46.000000 pykeops-2.2.2/pykeops/torch/generic/generic_red.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     5643 2023-02-22 10:18:06.000000 pykeops-2.2.2/pykeops/torch/half2_convert.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:59.993191 pykeops-2.2.2/pykeops/torch/lazytensor/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2808 2022-03-10 16:01:04.000000 pykeops-2.2.2/pykeops/torch/lazytensor/LazyTensor.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 pykeops-2.2.2/pykeops/torch/lazytensor/__init__.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    18189 2024-01-18 15:47:38.000000 pykeops-2.2.2/pykeops/torch/operations.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      748 2022-03-11 15:42:45.000000 pykeops-2.2.2/pykeops/torch/test_install.py
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     5366 2024-01-18 15:47:38.000000 pykeops-2.2.2/pykeops/torch/utils.py
-drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-02-09 16:48:59.993191 pykeops-2.2.2/pykeops.egg-info/
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2775 2024-02-09 16:48:59.000000 pykeops-2.2.2/pykeops.egg-info/PKG-INFO
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2555 2024-02-09 16:48:59.000000 pykeops-2.2.2/pykeops.egg-info/SOURCES.txt
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        1 2024-02-09 16:48:59.000000 pykeops-2.2.2/pykeops.egg-info/dependency_links.txt
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      249 2024-02-09 16:48:59.000000 pykeops-2.2.2/pykeops.egg-info/requires.txt
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        8 2024-02-09 16:48:59.000000 pykeops-2.2.2/pykeops.egg-info/top_level.txt
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      858 2020-01-15 14:47:12.000000 pykeops-2.2.2/readme.md
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)       38 2024-02-09 16:48:59.993191 pykeops-2.2.2/setup.cfg
--rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2807 2024-02-09 16:48:46.000000 pykeops-2.2.2/setup.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:49.466236 pykeops-2.2.3/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)       37 2022-03-10 16:01:04.000000 pykeops-2.2.3/MANIFEST.in
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2777 2024-04-14 08:15:49.466236 pykeops-2.2.3/PKG-INFO
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1184 2024-01-18 14:06:08.000000 pykeops-2.2.3/licence.txt
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:49.452902 pykeops-2.2.3/pykeops/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2320 2024-04-14 08:10:33.000000 pykeops-2.2.3/pykeops/__init__.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:49.456236 pykeops-2.2.3/pykeops/common/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 pykeops-2.2.3/pykeops/common/__init__.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4548 2023-02-22 10:18:06.000000 pykeops-2.2.3/pykeops/common/get_options.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      106 2022-03-10 16:01:04.000000 pykeops-2.2.3/pykeops/common/gpu_utils.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:49.456236 pykeops-2.2.3/pykeops/common/keops_io/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     7668 2023-12-22 10:13:41.000000 pykeops-2.2.3/pykeops/common/keops_io/LoadKeOps.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     7344 2023-12-22 10:13:41.000000 pykeops-2.2.3/pykeops/common/keops_io/LoadKeOps_cpp.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     3133 2024-02-09 15:59:15.000000 pykeops-2.2.3/pykeops/common/keops_io/LoadKeOps_nvrtc.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      328 2022-03-15 15:17:07.000000 pykeops-2.2.3/pykeops/common/keops_io/__init__.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     4476 2024-01-18 14:07:49.000000 pykeops-2.2.3/pykeops/common/keops_io/pykeops_nvrtc.cpp
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)   114903 2024-01-18 16:53:57.000000 pykeops-2.2.3/pykeops/common/lazy_tensor.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     8954 2023-12-22 10:13:41.000000 pykeops-2.2.3/pykeops/common/operations.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     8875 2023-12-22 10:13:41.000000 pykeops-2.2.3/pykeops/common/parse_type.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2824 2024-04-14 08:10:33.000000 pykeops-2.2.3/pykeops/common/utils.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1071 2024-02-07 09:31:44.000000 pykeops-2.2.3/pykeops/config.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        6 2024-04-14 08:11:22.000000 pykeops-2.2.3/pykeops/keops_version
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1184 2024-01-18 14:06:08.000000 pykeops-2.2.3/pykeops/licence.txt
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:49.456236 pykeops-2.2.3/pykeops/numpy/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      674 2023-04-04 07:06:57.000000 pykeops-2.2.3/pykeops/numpy/__init__.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:49.459569 pykeops-2.2.3/pykeops/numpy/cluster/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      476 2022-03-10 16:01:04.000000 pykeops-2.2.3/pykeops/numpy/cluster/__init__.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1528 2022-03-10 16:01:04.000000 pykeops-2.2.3/pykeops/numpy/cluster/grid_cluster.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     6439 2024-01-18 14:06:08.000000 pykeops-2.2.3/pykeops/numpy/cluster/matrix.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     8308 2022-03-10 16:01:04.000000 pykeops-2.2.3/pykeops/numpy/cluster/utils.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:49.459569 pykeops-2.2.3/pykeops/numpy/generic/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 pykeops-2.2.3/pykeops/numpy/generic/__init__.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    10003 2022-03-10 16:01:04.000000 pykeops-2.2.3/pykeops/numpy/generic/generic_ops.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    18353 2024-01-18 16:53:57.000000 pykeops-2.2.3/pykeops/numpy/generic/generic_red.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:49.459569 pykeops-2.2.3/pykeops/numpy/lazytensor/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2810 2022-03-10 16:01:04.000000 pykeops-2.2.3/pykeops/numpy/lazytensor/LazyTensor.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 pykeops-2.2.3/pykeops/numpy/lazytensor/__init__.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    12426 2024-01-18 15:47:38.000000 pykeops-2.2.3/pykeops/numpy/operations.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      700 2022-03-11 15:42:45.000000 pykeops-2.2.3/pykeops/numpy/test_install.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     6563 2023-03-27 09:23:23.000000 pykeops-2.2.3/pykeops/numpy/utils.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      858 2020-01-15 14:47:12.000000 pykeops-2.2.3/pykeops/readme.md
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:49.462903 pykeops-2.2.3/pykeops/test/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 pykeops-2.2.3/pykeops/test/__init__.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1467 2023-12-22 10:13:41.000000 pykeops-2.2.3/pykeops/test/conv2d.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1020 2022-03-11 15:42:45.000000 pykeops-2.2.3/pykeops/test/test_chunks.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1075 2022-03-11 15:42:45.000000 pykeops-2.2.3/pykeops/test/test_chunks_ranges.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1361 2022-03-11 15:42:45.000000 pykeops-2.2.3/pykeops/test/test_complex.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      656 2022-03-11 15:42:45.000000 pykeops-2.2.3/pykeops/test/test_complex_numpy.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      528 2022-03-11 15:42:45.000000 pykeops-2.2.3/pykeops/test/test_contiguous_numpy.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      554 2022-03-11 15:42:45.000000 pykeops-2.2.3/pykeops/test/test_contiguous_torch.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1050 2022-03-11 15:42:45.000000 pykeops-2.2.3/pykeops/test/test_finalchunks.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1075 2022-03-11 15:42:45.000000 pykeops-2.2.3/pykeops/test/test_finalchunks_ranges.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1290 2022-03-11 15:42:45.000000 pykeops-2.2.3/pykeops/test/test_float16.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1238 2022-03-11 15:42:45.000000 pykeops-2.2.3/pykeops/test/test_gpu_cpu.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     3879 2023-02-22 10:18:06.000000 pykeops-2.2.3/pykeops/test/test_kron.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1052 2023-02-22 10:18:06.000000 pykeops-2.2.3/pykeops/test/test_lazytensor_clamp.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1249 2022-03-11 15:42:45.000000 pykeops-2.2.3/pykeops/test/test_lazytensor_gaussian_batch.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1565 2022-03-11 15:42:45.000000 pykeops-2.2.3/pykeops/test/test_lazytensor_gaussian_cpu.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      947 2022-03-11 15:42:45.000000 pykeops-2.2.3/pykeops/test/test_lazytensor_gaussian_fromhost.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1098 2022-03-11 15:42:45.000000 pykeops-2.2.3/pykeops/test/test_lazytensor_gaussian_inplace.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      857 2022-03-11 15:42:45.000000 pykeops-2.2.3/pykeops/test/test_lazytensor_gaussian_numpy_inplace.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1456 2022-03-11 15:42:45.000000 pykeops-2.2.3/pykeops/test/test_lazytensor_grad.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      648 2022-03-11 15:42:45.000000 pykeops-2.2.3/pykeops/test/test_lazytensor_tensordot.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    10838 2023-02-22 10:18:06.000000 pykeops-2.2.3/pykeops/test/test_numpy.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      735 2024-01-25 11:52:46.000000 pykeops-2.2.3/pykeops/test/test_sinc.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    27731 2023-02-22 10:18:06.000000 pykeops-2.2.3/pykeops/test/test_torch.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2546 2024-01-25 12:48:13.000000 pykeops-2.2.3/pykeops/test/test_torch_func.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2296 2024-01-25 12:48:13.000000 pykeops-2.2.3/pykeops/test/test_torch_func_logsumexp.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      492 2024-01-25 11:52:46.000000 pykeops-2.2.3/pykeops/test/test_transpose.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2837 2024-01-25 12:48:13.000000 pykeops-2.2.3/pykeops/test/test_vmap.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:49.462903 pykeops-2.2.3/pykeops/torch/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      929 2023-12-22 10:13:41.000000 pykeops-2.2.3/pykeops/torch/__init__.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:49.462903 pykeops-2.2.3/pykeops/torch/cluster/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      476 2022-03-10 16:01:04.000000 pykeops-2.2.3/pykeops/torch/cluster/__init__.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     1821 2023-02-22 10:18:06.000000 pykeops-2.2.3/pykeops/torch/cluster/grid_cluster.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     7048 2024-04-14 08:10:33.000000 pykeops-2.2.3/pykeops/torch/cluster/matrix.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     9220 2023-12-22 10:13:41.000000 pykeops-2.2.3/pykeops/torch/cluster/utils.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:49.462903 pykeops-2.2.3/pykeops/torch/generic/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 pykeops-2.2.3/pykeops/torch/generic/__init__.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     8959 2022-03-10 16:01:04.000000 pykeops-2.2.3/pykeops/torch/generic/generic_ops.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    31602 2024-01-25 11:52:46.000000 pykeops-2.2.3/pykeops/torch/generic/generic_red.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     5643 2023-02-22 10:18:06.000000 pykeops-2.2.3/pykeops/torch/half2_convert.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:49.466236 pykeops-2.2.3/pykeops/torch/lazytensor/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2808 2022-03-10 16:01:04.000000 pykeops-2.2.3/pykeops/torch/lazytensor/LazyTensor.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        0 2022-03-10 16:01:04.000000 pykeops-2.2.3/pykeops/torch/lazytensor/__init__.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)    18189 2024-01-18 15:47:38.000000 pykeops-2.2.3/pykeops/torch/operations.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      748 2022-03-11 15:42:45.000000 pykeops-2.2.3/pykeops/torch/test_install.py
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     5366 2024-01-18 15:47:38.000000 pykeops-2.2.3/pykeops/torch/utils.py
+drwxr-xr-x   0 bcharlier  (1001) bcharlier  (1001)        0 2024-04-14 08:15:49.466236 pykeops-2.2.3/pykeops.egg-info/
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2777 2024-04-14 08:15:49.000000 pykeops-2.2.3/pykeops.egg-info/PKG-INFO
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2555 2024-04-14 08:15:49.000000 pykeops-2.2.3/pykeops.egg-info/SOURCES.txt
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        1 2024-04-14 08:15:49.000000 pykeops-2.2.3/pykeops.egg-info/dependency_links.txt
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      249 2024-04-14 08:15:49.000000 pykeops-2.2.3/pykeops.egg-info/requires.txt
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)        8 2024-04-14 08:15:49.000000 pykeops-2.2.3/pykeops.egg-info/top_level.txt
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)      858 2020-01-15 14:47:12.000000 pykeops-2.2.3/readme.md
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)       38 2024-04-14 08:15:49.466236 pykeops-2.2.3/setup.cfg
+-rw-r--r--   0 bcharlier  (1001) bcharlier  (1001)     2809 2024-04-14 08:15:42.000000 pykeops-2.2.3/setup.py
```

### Comparing `pykeops-2.2.2/PKG-INFO` & `pykeops-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykeops
-Version: 2.2.2
+Version: 2.2.3
 Summary: Python bindings of KeOps: KErnel OPerationS, on CPUs and GPUs, with autodiff and without memory overflows
 Home-page: http://www.kernel-operations.io/
 Author: B. Charlier, J. Feydy, J. Glaunes
 Author-email: benjamin.charlier@umontpellier.fr, jean.feydy@gmail.com, alexis.glaunes@parisdescartes.fr
 Project-URL: Bug Reports, https://github.com/getkeops/keops/issues
 Project-URL: Source, https://github.com/getkeops/keops
 Keywords: kernels gpu autodiff
@@ -12,19 +12,19 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pybind11
-Requires-Dist: keopscore==2.2.2
+Requires-Dist: keopscore==2.2.3
 Provides-Extra: full
 Requires-Dist: sphinx; extra == "full"
 Requires-Dist: sphinx-gallery; extra == "full"
 Requires-Dist: recommonmark; extra == "full"
 Requires-Dist: sphinxcontrib-httpdomain; extra == "full"
 Requires-Dist: sphinx_rtd_theme; extra == "full"
 Requires-Dist: sphinx-prompt; extra == "full"
```

### Comparing `pykeops-2.2.2/licence.txt` & `pykeops-2.2.3/licence.txt`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/__init__.py` & `pykeops-2.2.3/pykeops/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import os
 
+##############################################################
+# Verbosity level (we must do this before importing keopscore)
+verbose = True
+if os.getenv("PYKEOPS_VERBOSE") == "0":
+    verbose = False
+    os.environ["KEOPS_VERBOSE"] = "0"
+
 import keopscore
 import keopscore.config
 import keopscore.config.config
 from keopscore.config.config import get_build_folder as keops_get_build_folder
 
 from . import config as pykeopsconfig
 
-###########################################################
-# Verbosity level
-verbose = True
-if os.getenv("PYKEOPS_VERBOSE") == "0":
-    verbose = False
-    os.environ["KEOPS_VERBOSE"] = "0"
+from keopscore import show_cuda_status
 
 
 def set_verbose(val):
     global verbose
     verbose = val
     keopscore.verbose = val
```

### Comparing `pykeops-2.2.2/pykeops/common/get_options.py` & `pykeops-2.2.3/pykeops/common/get_options.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/common/keops_io/LoadKeOps.py` & `pykeops-2.2.3/pykeops/common/keops_io/LoadKeOps.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/common/keops_io/LoadKeOps_cpp.py` & `pykeops-2.2.3/pykeops/common/keops_io/LoadKeOps_cpp.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/common/keops_io/LoadKeOps_nvrtc.py` & `pykeops-2.2.3/pykeops/common/keops_io/LoadKeOps_nvrtc.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/common/keops_io/pykeops_nvrtc.cpp` & `pykeops-2.2.3/pykeops/common/keops_io/pykeops_nvrtc.cpp`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/common/lazy_tensor.py` & `pykeops-2.2.3/pykeops/common/lazy_tensor.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/common/operations.py` & `pykeops-2.2.3/pykeops/common/operations.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/common/parse_type.py` & `pykeops-2.2.3/pykeops/common/parse_type.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/common/utils.py` & `pykeops-2.2.3/pykeops/common/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,14 +91,19 @@
             raise ValueError(
                 "Incompatible batch dimensions: {} and {}.".format(dims_1, dims_2)
             )
 
     return max_tuple(padded_dims_1, padded_dims_2)
 
 
+def pyKeOps_Print(message, **kwargs):
+    if pykeops.verbose:
+        print(message, **kwargs)
+
+
 def pyKeOps_Message(message, use_tag=True, **kwargs):
     if pykeops.verbose:
         tag = "[pyKeOps] " if use_tag else ""
         message = tag + message
         print(message, **kwargs)
```

### Comparing `pykeops-2.2.2/pykeops/config.py` & `pykeops-2.2.3/pykeops/config.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/licence.txt` & `pykeops-2.2.3/pykeops/licence.txt`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/numpy/__init__.py` & `pykeops-2.2.3/pykeops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/numpy/cluster/grid_cluster.py` & `pykeops-2.2.3/pykeops/numpy/cluster/grid_cluster.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/numpy/cluster/matrix.py` & `pykeops-2.2.3/pykeops/numpy/cluster/matrix.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/numpy/cluster/utils.py` & `pykeops-2.2.3/pykeops/numpy/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/numpy/generic/generic_ops.py` & `pykeops-2.2.3/pykeops/numpy/generic/generic_ops.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/numpy/generic/generic_red.py` & `pykeops-2.2.3/pykeops/numpy/generic/generic_red.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/numpy/lazytensor/LazyTensor.py` & `pykeops-2.2.3/pykeops/numpy/lazytensor/LazyTensor.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/numpy/operations.py` & `pykeops-2.2.3/pykeops/numpy/operations.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/numpy/test_install.py` & `pykeops-2.2.3/pykeops/numpy/test_install.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/numpy/utils.py` & `pykeops-2.2.3/pykeops/numpy/utils.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/readme.md` & `pykeops-2.2.3/pykeops/readme.md`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/conv2d.py` & `pykeops-2.2.3/pykeops/test/conv2d.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_chunks.py` & `pykeops-2.2.3/pykeops/test/test_chunks.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_chunks_ranges.py` & `pykeops-2.2.3/pykeops/test/test_chunks_ranges.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_complex.py` & `pykeops-2.2.3/pykeops/test/test_complex.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_complex_numpy.py` & `pykeops-2.2.3/pykeops/test/test_complex_numpy.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_contiguous_numpy.py` & `pykeops-2.2.3/pykeops/test/test_contiguous_numpy.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_contiguous_torch.py` & `pykeops-2.2.3/pykeops/test/test_contiguous_torch.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_finalchunks.py` & `pykeops-2.2.3/pykeops/test/test_finalchunks.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_finalchunks_ranges.py` & `pykeops-2.2.3/pykeops/test/test_finalchunks_ranges.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_float16.py` & `pykeops-2.2.3/pykeops/test/test_float16.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_gpu_cpu.py` & `pykeops-2.2.3/pykeops/test/test_gpu_cpu.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_kron.py` & `pykeops-2.2.3/pykeops/test/test_kron.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_lazytensor_clamp.py` & `pykeops-2.2.3/pykeops/test/test_lazytensor_clamp.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_lazytensor_gaussian_batch.py` & `pykeops-2.2.3/pykeops/test/test_lazytensor_gaussian_batch.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_lazytensor_gaussian_cpu.py` & `pykeops-2.2.3/pykeops/test/test_lazytensor_gaussian_cpu.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_lazytensor_gaussian_fromhost.py` & `pykeops-2.2.3/pykeops/test/test_lazytensor_gaussian_fromhost.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_lazytensor_gaussian_inplace.py` & `pykeops-2.2.3/pykeops/test/test_lazytensor_gaussian_inplace.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_lazytensor_gaussian_numpy_inplace.py` & `pykeops-2.2.3/pykeops/test/test_lazytensor_gaussian_numpy_inplace.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_lazytensor_grad.py` & `pykeops-2.2.3/pykeops/test/test_lazytensor_grad.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_lazytensor_tensordot.py` & `pykeops-2.2.3/pykeops/test/test_lazytensor_tensordot.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_numpy.py` & `pykeops-2.2.3/pykeops/test/test_numpy.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_sinc.py` & `pykeops-2.2.3/pykeops/test/test_sinc.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_torch.py` & `pykeops-2.2.3/pykeops/test/test_torch.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_torch_func.py` & `pykeops-2.2.3/pykeops/test/test_torch_func.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_torch_func_logsumexp.py` & `pykeops-2.2.3/pykeops/test/test_torch_func_logsumexp.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/test/test_vmap.py` & `pykeops-2.2.3/pykeops/test/test_vmap.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/torch/__init__.py` & `pykeops-2.2.3/pykeops/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/torch/cluster/grid_cluster.py` & `pykeops-2.2.3/pykeops/torch/cluster/grid_cluster.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/torch/cluster/matrix.py` & `pykeops-2.2.3/pykeops/torch/cluster/matrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pykeops.common.utils import pyKeOps_Print
 import torch
 
 
 def from_matrix(ranges_i, ranges_j, keep):
     r"""Turns a boolean matrix into a KeOps-friendly **ranges** argument.
 
     This routine is a helper for the **block-sparse** reduction mode of KeOps,
@@ -131,10 +132,10 @@
 
 if __name__ == "__main__":
     r_i = torch.IntTensor([[2, 5], [7, 12]])
     r_j = torch.IntTensor([[1, 4], [4, 9], [20, 30]])
     x, y = torch.Tensor([0.0, 1.0]), torch.Tensor([0.0, 0.7, 2.0])
     dist = (x[:, None] - y[None, :]) ** 2
     keep = dist <= 0.8
-    print(keep)
+    pyKeOps_Print(keep)
     for item in from_matrix(r_i, r_j, keep):
-        print(item)
+        pyKeOps_Print(item)
```

### Comparing `pykeops-2.2.2/pykeops/torch/cluster/utils.py` & `pykeops-2.2.3/pykeops/torch/cluster/utils.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/torch/generic/generic_ops.py` & `pykeops-2.2.3/pykeops/torch/generic/generic_ops.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/torch/generic/generic_red.py` & `pykeops-2.2.3/pykeops/torch/generic/generic_red.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/torch/half2_convert.py` & `pykeops-2.2.3/pykeops/torch/half2_convert.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/torch/lazytensor/LazyTensor.py` & `pykeops-2.2.3/pykeops/torch/lazytensor/LazyTensor.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/torch/operations.py` & `pykeops-2.2.3/pykeops/torch/operations.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/torch/test_install.py` & `pykeops-2.2.3/pykeops/torch/test_install.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops/torch/utils.py` & `pykeops-2.2.3/pykeops/torch/utils.py`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/pykeops.egg-info/PKG-INFO` & `pykeops-2.2.3/pykeops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykeops
-Version: 2.2.2
+Version: 2.2.3
 Summary: Python bindings of KeOps: KErnel OPerationS, on CPUs and GPUs, with autodiff and without memory overflows
 Home-page: http://www.kernel-operations.io/
 Author: B. Charlier, J. Feydy, J. Glaunes
 Author-email: benjamin.charlier@umontpellier.fr, jean.feydy@gmail.com, alexis.glaunes@parisdescartes.fr
 Project-URL: Bug Reports, https://github.com/getkeops/keops/issues
 Project-URL: Source, https://github.com/getkeops/keops
 Keywords: kernels gpu autodiff
@@ -12,19 +12,19 @@
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: pybind11
-Requires-Dist: keopscore==2.2.2
+Requires-Dist: keopscore==2.2.3
 Provides-Extra: full
 Requires-Dist: sphinx; extra == "full"
 Requires-Dist: sphinx-gallery; extra == "full"
 Requires-Dist: recommonmark; extra == "full"
 Requires-Dist: sphinxcontrib-httpdomain; extra == "full"
 Requires-Dist: sphinx_rtd_theme; extra == "full"
 Requires-Dist: sphinx-prompt; extra == "full"
```

### Comparing `pykeops-2.2.2/pykeops.egg-info/SOURCES.txt` & `pykeops-2.2.3/pykeops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/readme.md` & `pykeops-2.2.3/readme.md`

 * *Files identical despite different names*

### Comparing `pykeops-2.2.2/setup.py` & `pykeops-2.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     url="http://www.kernel-operations.io/",
     project_urls={
         "Bug Reports": "https://github.com/getkeops/keops/issues",
         "Source": "https://github.com/getkeops/keops",
     },
     author="B. Charlier, J. Feydy, J. Glaunes",
     author_email="benjamin.charlier@umontpellier.fr, jean.feydy@gmail.com, alexis.glaunes@parisdescartes.fr",
-    python_requires=">=3",
+    python_requires=">=3.8",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Scientific/Engineering",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
```

