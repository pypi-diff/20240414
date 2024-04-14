# Comparing `tmp/mesmerize-core-0.3.0.tar.gz` & `tmp/mesmerize_core-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mesmerize-core-0.3.0.tar", last modified: Tue Oct 31 07:56:26 2023, max compression
+gzip compressed data, was "mesmerize_core-0.4.0.tar", last modified: Sun Apr 14 00:18:49 2024, max compression
```

## Comparing `mesmerize-core-0.3.0.tar` & `mesmerize_core-0.4.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 07:56:26.427307 mesmerize-core-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2023-10-31 07:56:26.427307 mesmerize-core-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9439 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 07:56:26.423307 mesmerize-core-0.3.0/mesmerize_core/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/mesmerize_core/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      514 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/mesmerize_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 07:56:26.423307 mesmerize-core-0.3.0/mesmerize_core/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/mesmerize_core/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5399 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/mesmerize_core/algorithms/cnmf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4769 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/mesmerize_core/algorithms/cnmfe.py
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/mesmerize_core/algorithms/mcorr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 07:56:26.423307 mesmerize-core-0.3.0/mesmerize_core/arrays/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/mesmerize_core/arrays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/mesmerize_core/arrays/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7747 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/mesmerize_core/arrays/_cnmf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/mesmerize_core/arrays/_tiff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4058 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/mesmerize_core/arrays/_video.py
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/mesmerize_core/batch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 07:56:26.427307 mesmerize-core-0.3.0/mesmerize_core/caiman_extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/mesmerize_core/caiman_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/mesmerize_core/caiman_extensions/_batch_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1882 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/mesmerize_core/caiman_extensions/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8188 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/mesmerize_core/caiman_extensions/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    25770 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/mesmerize_core/caiman_extensions/cnmf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20536 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/mesmerize_core/caiman_extensions/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4371 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/mesmerize_core/caiman_extensions/mcorr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/mesmerize_core/movie_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5602 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/mesmerize_core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 07:56:26.423307 mesmerize-core-0.3.0/mesmerize_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2023-10-31 07:56:26.000000 mesmerize-core-0.3.0/mesmerize_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2023-10-31 07:56:26.000000 mesmerize-core-0.3.0/mesmerize_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-31 07:56:26.000000 mesmerize-core-0.3.0/mesmerize_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-10-31 07:56:26.000000 mesmerize-core-0.3.0/mesmerize_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-31 07:56:26.000000 mesmerize-core-0.3.0/mesmerize_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-31 07:56:26.427307 mesmerize-core-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 07:56:26.427307 mesmerize-core-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/tests/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    46638 2023-10-31 07:56:10.000000 mesmerize-core-0.3.0/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:18:49.919316 mesmerize_core-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9422 2024-04-14 00:18:49.919316 mesmerize_core-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8352 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:18:49.915315 mesmerize_core-0.4.0/mesmerize_core/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/mesmerize_core/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/mesmerize_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:18:49.915315 mesmerize_core-0.4.0/mesmerize_core/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/mesmerize_core/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5399 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/mesmerize_core/algorithms/cnmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4769 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/mesmerize_core/algorithms/cnmfe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/mesmerize_core/algorithms/mcorr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:18:49.915315 mesmerize_core-0.4.0/mesmerize_core/arrays/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/mesmerize_core/arrays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/mesmerize_core/arrays/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7747 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/mesmerize_core/arrays/_cnmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/mesmerize_core/arrays/_tiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/mesmerize_core/arrays/_video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/mesmerize_core/batch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:18:49.919316 mesmerize_core-0.4.0/mesmerize_core/caiman_extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/mesmerize_core/caiman_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/mesmerize_core/caiman_extensions/_batch_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1882 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/mesmerize_core/caiman_extensions/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8188 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/mesmerize_core/caiman_extensions/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25789 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/mesmerize_core/caiman_extensions/cnmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20536 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/mesmerize_core/caiman_extensions/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/mesmerize_core/caiman_extensions/mcorr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/mesmerize_core/movie_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/mesmerize_core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:18:49.919316 mesmerize_core-0.4.0/mesmerize_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9422 2024-04-14 00:18:49.000000 mesmerize_core-0.4.0/mesmerize_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-14 00:18:49.000000 mesmerize_core-0.4.0/mesmerize_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 00:18:49.000000 mesmerize_core-0.4.0/mesmerize_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-14 00:18:49.000000 mesmerize_core-0.4.0/mesmerize_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-14 00:18:49.000000 mesmerize_core-0.4.0/mesmerize_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 00:18:49.919316 mesmerize_core-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:18:49.919316 mesmerize_core-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/tests/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46638 2024-04-14 00:18:42.000000 mesmerize_core-0.4.0/tests/test_core.py
```

### Comparing `mesmerize-core-0.3.0/LICENSE` & `mesmerize_core-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.3.0/PKG-INFO` & `mesmerize_core-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mesmerize-core
-Version: 0.3.0
+Version: 0.4.0
 Summary: High level pandas-based API for batch analysis of Calcium Imaging data using CaImAn
 Home-page: https://github.com/nel-lab/mesmerize-core
 Author: Kushal Kolar, Caitlin Lewis, Arjun Putcha
 Author-email: 
 License: Apache-Software-License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -31,16 +31,14 @@
 [![Linux pip](https://github.com/nel-lab/mesmerize-core/actions/workflows/linux-pip.yml/badge.svg)](https://github.com/nel-lab/mesmerize-core/actions/workflows/linux-pip.yml)
 [![Linux Conda](https://github.com/nel-lab/mesmerize-core/actions/workflows/linux-conda.yml/badge.svg)](https://github.com/nel-lab/mesmerize-core/actions/workflows/linux-conda.yml)
 [![MacOS Conda](https://github.com/nel-lab/mesmerize-core/actions/workflows/macos-conda.yml/badge.svg)](https://github.com/nel-lab/mesmerize-core/actions/workflows/macos-conda.yml)
 [![Windows Conda](https://github.com/nel-lab/mesmerize-core/actions/workflows/windows-conda.yml/badge.svg)](https://github.com/nel-lab/mesmerize-core/actions/workflows/windows-conda.yml)
 [![Documentation Status](https://readthedocs.org/projects/mesmerize-core/badge/?version=latest)](https://mesmerize-core.readthedocs.io/en/latest/?badge=latest)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/mesmerize-core.svg)](https://anaconda.org/conda-forge/mesmerize-core)
 
-[![Gitter](https://badges.gitter.im/mesmerize_discussion/mesmerize-viz.svg)](https://gitter.im/mesmerize_discussion/mesmerize-viz?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
-
 ### Mesmerize core backend
 [**Installation**](https://github.com/nel-lab/mesmerize-core#installation) | [**Examples**](https://github.com/nel-lab/mesmerize-core#examples)
 
 A batch management system for calcium imaging analysis using the CaImAn library. 
 It contains `pandas.DataFrame` and `pandas.Series` extensions that interface with CaImAn for running the various algorithms and organizing input & output data.
 
 This **replaces** the [Mesmerize legacy desktop application](https://github.com/kushalkolar/MESmerize).\
@@ -49,73 +47,55 @@
 # Documentation
 
 We recommend starting out with the demo notebook ```notebooks/mcorr_cnmf.ipynb```
 
 Documentation is available at: https://mesmerize-core.readthedocs.io/ \
 User guide: https://mesmerize-core.readthedocs.io/en/latest/user_guide.html
 
-Please use the GitHub issue tracker for any issues. For smaller questions or discussion use gitter.
+## Getting Help
 
-gitter: https://gitter.im/mesmerize_discussion/mesmerize-viz
+Please use the GitHub issue tracker for any issues, and discussions for discussions. We no longer use gitter. If you are in the Slack, we usually only respond on slack around workshops. GitHub is for long term support.
 
-Video tutorial/virtual workshop from September 2022: https://www.youtube.com/watch?v=0AGiAaslJdk
+Video tutorial/virtual workshop from September 2022 (quite outdated, if you have question post on github): https://www.youtube.com/watch?v=0AGiAaslJdk
 
 # Overview
 
 ![batch_management](https://user-images.githubusercontent.com/9403332/179145962-82317da6-0340-44e4-83ba-7dace0300f55.png)
 
 # Visualization
 
-For visualization we strongly recommend [`fastplotlib`](https://github.com/kushalkolar/fastplotlib), a very new but very fast plotting library. Here are some examples of `fastplotlib` visualizations using `mesmerize-core` outputs. You can create these interactive plots within jupyter notebooks, therefore they will also work on cloud computing intrastructure!
-
-### View raw and motion corrected movie side by side:
-
-![mcorr](https://user-images.githubusercontent.com/9403332/210932452-5ed344dd-9a82-41ee-adc5-a9476e1f03a5.gif)
-
-### Contours from CNMF, good components shown here in cyan and bad components in magenta:
+Install [mesmerize-viz](https://github.com/kushalkolar/mesmerize-viz) for visualization. Mesmerize-viz gives you ready-to-use viuslizations for motion correction and CNMF - including component exploration, interactive component evaluation using metrics, and manual addition or removal of components. 
 
-![cnmf](https://user-images.githubusercontent.com/9403332/210932670-d797d301-839c-48d9-b11f-3330e076e0e4.gif)
-
-### Input movie, constructed movie `(A * C)`, residuals `(Y - A * C - b * f)`, and reconstructed background `(b * f)`:
-
-![cnmf-rcm](https://user-images.githubusercontent.com/9403332/210932903-b994359b-62d4-49fd-aa6b-cd4855ba873e.gif)
+```
+pip install mesmerize-viz
+```
 
-### Interactive Component evaluation after CNMF:
+:exclamation: **Harware requirements** The large CNMF visualizations with contours etc. usually require either a dedicated GPU or integrated GPU with access to at least 1GB of VRAM. 
 
-https://user-images.githubusercontent.com/9403332/191207883-2393664d-b5e1-49a5-84d1-8ed7eadcf7a0.mp4
+You may need to install drivers depending on your system, see the `fastplotlib` repo for more information: https://github.com/kushalkolar/fastplotlib#graphics-drivers
 
-As mentioned, fastplotlib is meant to be a fast plotting library which can handle **millions** of points. You can create highly complex and interactive plots to combine outputs from the CaImAn algorithms with other experimentally relevant analysis, such as behavioral data.
+If you use `fastplotlib` directly you can create highly complex and interactive plots to combine outputs from the CaImAn algorithms with other experimentally relevant analysis, such as behavioral data.
 
 ![epic](https://user-images.githubusercontent.com/9403332/210304473-f36f2aaf-319e-435b-bcc8-0e8d3e1ef282.gif)
 
 # Examples
 
 **See the `notebooks` directory for detailed examples.**
 
-Note that [`fastplotlib`](https://github.com/kushalkolar/fastplotlib) is required for the visualizations.
-
 # Installation
 
 ## For users
 
 The instructions below will install `mesmerize-core`.
 
-For visualization install `fastplotlib` into the same environment as `mesmerize-core`:
-
-```bash
-pip install "fastplotlib[notebook]"
-```
-
-You may need to install Vulkan drivers depending on your system, see the `fastplotlib` repo for more information: https://github.com/kushalkolar/fastplotlib#graphics-drivers
-
 ### Conda
 
-`mesmerize-core` is availabe as a conda package which also gives you CaImAn! These instructions will give you a working `mesmerize-core` along with `caiman` in the same environment.
+`mesmerize-core` is available as a conda package which also gives you CaImAn. These instructions will give you a working `mesmerize-core` along with `caiman` in the same environment.
 
-**Important note: Sometimes conda or mamba will get stuck at a step, such as creating an environment or installing a package. I found that pressing `Enter` on your keyboard can sometimes help it continue when it pauses.**
+**Important note: Sometimes conda or mamba will get stuck at a step, such as creating an environment or installing a package. Pressing `Enter` on your keyboard can sometimes help it continue when it pauses.**
 
 1. Install `mamba` into your base environment. Skip this step if you have `mamba`. This step may take 10 minutes and display several messages like "Solving environment: failed with..." but it should eventually install `mamba`.
 
 ```bash
 conda install -c conda-forge mamba
 
 # if conda is behaving slow, this command can sometimes help
@@ -156,21 +136,21 @@
 
 ```bash
 # run in ipython
 import mesmerize_core
 mesmerize_core.__version__
 ```
 
-6. Install `fastplotlib` for visualization into the same environment (run this in the anaconda prompt, not ipython). You may also need to install Vulkan drivers depending on your system, see the `fastplotlib` repo for more information: https://github.com/kushalkolar/fastplotlib#graphics-drivers
+6. Install `mesmerize-viz` for visualization into the same environment (run this in the anaconda prompt, not ipython). You may also need to install graphics drivers depending on your system, see the `fastplotlib` repo for more information: https://github.com/kushalkolar/fastplotlib#graphics-drivers
 
 ```bash
-pip install "fastplotlib[notebook]"
+pip install mesmerize-viz
 ```
 
-**Optional: install `simplejpeg` for much faster notebook visualization, you will need C compilers and [libjpeg-turbo](https://libjpeg-turbo.org/) for this to work:**
+**Strongly recommended: install `simplejpeg` for much faster notebook visualization, you will need C compilers and [libjpeg-turbo](https://libjpeg-turbo.org/) for this to work:**
 
 ```bash
 pip install simplejpeg
 ```
 
 ### python virtual environments
 
@@ -193,16 +173,19 @@
 pip install -r requirements.txt
 pip install .
 caimanmanager install
 
 # install mesmerize-core
 pip install mesmerize-core
 
-# install fastplotlib
-pip install "fastplotlib[notebook]"
+# install mesmerize-viz
+pip install mesmerize-viz
+
+# install simplejpeg
+pip install simplejpeg
 
 # you should now be able to import mesmerize_core
 # start ipython
 ipython
 
 # run in ipython
 import mesmerize_core
@@ -214,18 +197,15 @@
 ### conda
 
 ```bash
 # install mamba in your base environment
 conda install -c conda-forge mamba
 conda clean -a
 
-# on linux and mac you can use python=3.10
-conda create --name mesmerize-core python=3.10
-# on windows you MUST use python=3.9
-conda create --name mesmerize-core python=3.9
+conda create --name mesmerize-core
 
 # activate environment
 conda activate mesmerize-core
 conda clean -a
 
 # clone this repo
 git clone https://github.com/nel-lab/mesmerize-core.git
```

### Comparing `mesmerize-core-0.3.0/README.md` & `mesmerize_core-0.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 [![Linux pip](https://github.com/nel-lab/mesmerize-core/actions/workflows/linux-pip.yml/badge.svg)](https://github.com/nel-lab/mesmerize-core/actions/workflows/linux-pip.yml)
 [![Linux Conda](https://github.com/nel-lab/mesmerize-core/actions/workflows/linux-conda.yml/badge.svg)](https://github.com/nel-lab/mesmerize-core/actions/workflows/linux-conda.yml)
 [![MacOS Conda](https://github.com/nel-lab/mesmerize-core/actions/workflows/macos-conda.yml/badge.svg)](https://github.com/nel-lab/mesmerize-core/actions/workflows/macos-conda.yml)
 [![Windows Conda](https://github.com/nel-lab/mesmerize-core/actions/workflows/windows-conda.yml/badge.svg)](https://github.com/nel-lab/mesmerize-core/actions/workflows/windows-conda.yml)
 [![Documentation Status](https://readthedocs.org/projects/mesmerize-core/badge/?version=latest)](https://mesmerize-core.readthedocs.io/en/latest/?badge=latest)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/mesmerize-core.svg)](https://anaconda.org/conda-forge/mesmerize-core)
 
-[![Gitter](https://badges.gitter.im/mesmerize_discussion/mesmerize-viz.svg)](https://gitter.im/mesmerize_discussion/mesmerize-viz?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
-
 ### Mesmerize core backend
 [**Installation**](https://github.com/nel-lab/mesmerize-core#installation) | [**Examples**](https://github.com/nel-lab/mesmerize-core#examples)
 
 A batch management system for calcium imaging analysis using the CaImAn library. 
 It contains `pandas.DataFrame` and `pandas.Series` extensions that interface with CaImAn for running the various algorithms and organizing input & output data.
 
 This **replaces** the [Mesmerize legacy desktop application](https://github.com/kushalkolar/MESmerize).\
@@ -21,73 +19,55 @@
 # Documentation
 
 We recommend starting out with the demo notebook ```notebooks/mcorr_cnmf.ipynb```
 
 Documentation is available at: https://mesmerize-core.readthedocs.io/ \
 User guide: https://mesmerize-core.readthedocs.io/en/latest/user_guide.html
 
-Please use the GitHub issue tracker for any issues. For smaller questions or discussion use gitter.
+## Getting Help
 
-gitter: https://gitter.im/mesmerize_discussion/mesmerize-viz
+Please use the GitHub issue tracker for any issues, and discussions for discussions. We no longer use gitter. If you are in the Slack, we usually only respond on slack around workshops. GitHub is for long term support.
 
-Video tutorial/virtual workshop from September 2022: https://www.youtube.com/watch?v=0AGiAaslJdk
+Video tutorial/virtual workshop from September 2022 (quite outdated, if you have question post on github): https://www.youtube.com/watch?v=0AGiAaslJdk
 
 # Overview
 
 ![batch_management](https://user-images.githubusercontent.com/9403332/179145962-82317da6-0340-44e4-83ba-7dace0300f55.png)
 
 # Visualization
 
-For visualization we strongly recommend [`fastplotlib`](https://github.com/kushalkolar/fastplotlib), a very new but very fast plotting library. Here are some examples of `fastplotlib` visualizations using `mesmerize-core` outputs. You can create these interactive plots within jupyter notebooks, therefore they will also work on cloud computing intrastructure!
-
-### View raw and motion corrected movie side by side:
-
-![mcorr](https://user-images.githubusercontent.com/9403332/210932452-5ed344dd-9a82-41ee-adc5-a9476e1f03a5.gif)
-
-### Contours from CNMF, good components shown here in cyan and bad components in magenta:
+Install [mesmerize-viz](https://github.com/kushalkolar/mesmerize-viz) for visualization. Mesmerize-viz gives you ready-to-use viuslizations for motion correction and CNMF - including component exploration, interactive component evaluation using metrics, and manual addition or removal of components. 
 
-![cnmf](https://user-images.githubusercontent.com/9403332/210932670-d797d301-839c-48d9-b11f-3330e076e0e4.gif)
-
-### Input movie, constructed movie `(A * C)`, residuals `(Y - A * C - b * f)`, and reconstructed background `(b * f)`:
-
-![cnmf-rcm](https://user-images.githubusercontent.com/9403332/210932903-b994359b-62d4-49fd-aa6b-cd4855ba873e.gif)
+```
+pip install mesmerize-viz
+```
 
-### Interactive Component evaluation after CNMF:
+:exclamation: **Harware requirements** The large CNMF visualizations with contours etc. usually require either a dedicated GPU or integrated GPU with access to at least 1GB of VRAM. 
 
-https://user-images.githubusercontent.com/9403332/191207883-2393664d-b5e1-49a5-84d1-8ed7eadcf7a0.mp4
+You may need to install drivers depending on your system, see the `fastplotlib` repo for more information: https://github.com/kushalkolar/fastplotlib#graphics-drivers
 
-As mentioned, fastplotlib is meant to be a fast plotting library which can handle **millions** of points. You can create highly complex and interactive plots to combine outputs from the CaImAn algorithms with other experimentally relevant analysis, such as behavioral data.
+If you use `fastplotlib` directly you can create highly complex and interactive plots to combine outputs from the CaImAn algorithms with other experimentally relevant analysis, such as behavioral data.
 
 ![epic](https://user-images.githubusercontent.com/9403332/210304473-f36f2aaf-319e-435b-bcc8-0e8d3e1ef282.gif)
 
 # Examples
 
 **See the `notebooks` directory for detailed examples.**
 
-Note that [`fastplotlib`](https://github.com/kushalkolar/fastplotlib) is required for the visualizations.
-
 # Installation
 
 ## For users
 
 The instructions below will install `mesmerize-core`.
 
-For visualization install `fastplotlib` into the same environment as `mesmerize-core`:
-
-```bash
-pip install "fastplotlib[notebook]"
-```
-
-You may need to install Vulkan drivers depending on your system, see the `fastplotlib` repo for more information: https://github.com/kushalkolar/fastplotlib#graphics-drivers
-
 ### Conda
 
-`mesmerize-core` is availabe as a conda package which also gives you CaImAn! These instructions will give you a working `mesmerize-core` along with `caiman` in the same environment.
+`mesmerize-core` is available as a conda package which also gives you CaImAn. These instructions will give you a working `mesmerize-core` along with `caiman` in the same environment.
 
-**Important note: Sometimes conda or mamba will get stuck at a step, such as creating an environment or installing a package. I found that pressing `Enter` on your keyboard can sometimes help it continue when it pauses.**
+**Important note: Sometimes conda or mamba will get stuck at a step, such as creating an environment or installing a package. Pressing `Enter` on your keyboard can sometimes help it continue when it pauses.**
 
 1. Install `mamba` into your base environment. Skip this step if you have `mamba`. This step may take 10 minutes and display several messages like "Solving environment: failed with..." but it should eventually install `mamba`.
 
 ```bash
 conda install -c conda-forge mamba
 
 # if conda is behaving slow, this command can sometimes help
@@ -128,21 +108,21 @@
 
 ```bash
 # run in ipython
 import mesmerize_core
 mesmerize_core.__version__
 ```
 
-6. Install `fastplotlib` for visualization into the same environment (run this in the anaconda prompt, not ipython). You may also need to install Vulkan drivers depending on your system, see the `fastplotlib` repo for more information: https://github.com/kushalkolar/fastplotlib#graphics-drivers
+6. Install `mesmerize-viz` for visualization into the same environment (run this in the anaconda prompt, not ipython). You may also need to install graphics drivers depending on your system, see the `fastplotlib` repo for more information: https://github.com/kushalkolar/fastplotlib#graphics-drivers
 
 ```bash
-pip install "fastplotlib[notebook]"
+pip install mesmerize-viz
 ```
 
-**Optional: install `simplejpeg` for much faster notebook visualization, you will need C compilers and [libjpeg-turbo](https://libjpeg-turbo.org/) for this to work:**
+**Strongly recommended: install `simplejpeg` for much faster notebook visualization, you will need C compilers and [libjpeg-turbo](https://libjpeg-turbo.org/) for this to work:**
 
 ```bash
 pip install simplejpeg
 ```
 
 ### python virtual environments
 
@@ -165,16 +145,19 @@
 pip install -r requirements.txt
 pip install .
 caimanmanager install
 
 # install mesmerize-core
 pip install mesmerize-core
 
-# install fastplotlib
-pip install "fastplotlib[notebook]"
+# install mesmerize-viz
+pip install mesmerize-viz
+
+# install simplejpeg
+pip install simplejpeg
 
 # you should now be able to import mesmerize_core
 # start ipython
 ipython
 
 # run in ipython
 import mesmerize_core
@@ -186,18 +169,15 @@
 ### conda
 
 ```bash
 # install mamba in your base environment
 conda install -c conda-forge mamba
 conda clean -a
 
-# on linux and mac you can use python=3.10
-conda create --name mesmerize-core python=3.10
-# on windows you MUST use python=3.9
-conda create --name mesmerize-core python=3.9
+conda create --name mesmerize-core
 
 # activate environment
 conda activate mesmerize-core
 conda clean -a
 
 # clone this repo
 git clone https://github.com/nel-lab/mesmerize-core.git
```

### Comparing `mesmerize-core-0.3.0/mesmerize_core/__init__.py` & `mesmerize_core-0.4.0/mesmerize_core/__init__.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.3.0/mesmerize_core/algorithms/cnmf.py` & `mesmerize_core-0.4.0/mesmerize_core/algorithms/cnmf.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.3.0/mesmerize_core/algorithms/cnmfe.py` & `mesmerize_core-0.4.0/mesmerize_core/algorithms/cnmfe.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.3.0/mesmerize_core/algorithms/mcorr.py` & `mesmerize_core-0.4.0/mesmerize_core/algorithms/mcorr.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.3.0/mesmerize_core/arrays/_base.py` & `mesmerize_core-0.4.0/mesmerize_core/arrays/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
     @property
     def nbytes(self) -> int:
         """
         int
             number of bytes for the array if it were fully computed
         """
-        return np.prod(self.shape + (np.dtype(self.dtype).itemsize,))
+        return np.prod(self.shape + (np.dtype(self.dtype).itemsize,), dtype=np.int64)
 
     @property
     def nbytes_gb(self) -> float:
         """
         float
             number of gigabytes for the array if it were fully computed
         """
```

### Comparing `mesmerize-core-0.3.0/mesmerize_core/arrays/_cnmf.py` & `mesmerize_core-0.4.0/mesmerize_core/arrays/_cnmf.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.3.0/mesmerize_core/arrays/_tiff.py` & `mesmerize_core-0.4.0/mesmerize_core/arrays/_tiff.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.3.0/mesmerize_core/arrays/_video.py` & `mesmerize_core-0.4.0/mesmerize_core/arrays/_video.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.3.0/mesmerize_core/batch_utils.py` & `mesmerize_core-0.4.0/mesmerize_core/batch_utils.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.3.0/mesmerize_core/caiman_extensions/_utils.py` & `mesmerize_core-0.4.0/mesmerize_core/caiman_extensions/_utils.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.3.0/mesmerize_core/caiman_extensions/cache.py` & `mesmerize_core-0.4.0/mesmerize_core/caiman_extensions/cache.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.3.0/mesmerize_core/caiman_extensions/cnmf.py` & `mesmerize_core-0.4.0/mesmerize_core/caiman_extensions/cnmf.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,15 +377,15 @@
         f = cnmf_obj.estimates.f
 
         temporal = C
 
         if add_background:
             temporal += f
         elif add_residuals:
-            temporal += cnmf_obj.estimates.YrA
+            temporal += cnmf_obj.estimates.YrA[component_indices]
 
         return temporal
 
     @validate("cnmf")
     @_component_indices_parser
     @cnmf_cache.use_cache
     def get_rcm(
```

### Comparing `mesmerize-core-0.3.0/mesmerize_core/caiman_extensions/common.py` & `mesmerize_core-0.4.0/mesmerize_core/caiman_extensions/common.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.3.0/mesmerize_core/caiman_extensions/mcorr.py` & `mesmerize_core-0.4.0/mesmerize_core/caiman_extensions/mcorr.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.3.0/mesmerize_core/movie_readers.py` & `mesmerize_core-0.4.0/mesmerize_core/movie_readers.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.3.0/mesmerize_core/utils.py` & `mesmerize_core-0.4.0/mesmerize_core/utils.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.3.0/mesmerize_core.egg-info/PKG-INFO` & `mesmerize_core-0.4.0/mesmerize_core.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mesmerize-core
-Version: 0.3.0
+Version: 0.4.0
 Summary: High level pandas-based API for batch analysis of Calcium Imaging data using CaImAn
 Home-page: https://github.com/nel-lab/mesmerize-core
 Author: Kushal Kolar, Caitlin Lewis, Arjun Putcha
 Author-email: 
 License: Apache-Software-License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -31,16 +31,14 @@
 [![Linux pip](https://github.com/nel-lab/mesmerize-core/actions/workflows/linux-pip.yml/badge.svg)](https://github.com/nel-lab/mesmerize-core/actions/workflows/linux-pip.yml)
 [![Linux Conda](https://github.com/nel-lab/mesmerize-core/actions/workflows/linux-conda.yml/badge.svg)](https://github.com/nel-lab/mesmerize-core/actions/workflows/linux-conda.yml)
 [![MacOS Conda](https://github.com/nel-lab/mesmerize-core/actions/workflows/macos-conda.yml/badge.svg)](https://github.com/nel-lab/mesmerize-core/actions/workflows/macos-conda.yml)
 [![Windows Conda](https://github.com/nel-lab/mesmerize-core/actions/workflows/windows-conda.yml/badge.svg)](https://github.com/nel-lab/mesmerize-core/actions/workflows/windows-conda.yml)
 [![Documentation Status](https://readthedocs.org/projects/mesmerize-core/badge/?version=latest)](https://mesmerize-core.readthedocs.io/en/latest/?badge=latest)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/mesmerize-core.svg)](https://anaconda.org/conda-forge/mesmerize-core)
 
-[![Gitter](https://badges.gitter.im/mesmerize_discussion/mesmerize-viz.svg)](https://gitter.im/mesmerize_discussion/mesmerize-viz?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
-
 ### Mesmerize core backend
 [**Installation**](https://github.com/nel-lab/mesmerize-core#installation) | [**Examples**](https://github.com/nel-lab/mesmerize-core#examples)
 
 A batch management system for calcium imaging analysis using the CaImAn library. 
 It contains `pandas.DataFrame` and `pandas.Series` extensions that interface with CaImAn for running the various algorithms and organizing input & output data.
 
 This **replaces** the [Mesmerize legacy desktop application](https://github.com/kushalkolar/MESmerize).\
@@ -49,73 +47,55 @@
 # Documentation
 
 We recommend starting out with the demo notebook ```notebooks/mcorr_cnmf.ipynb```
 
 Documentation is available at: https://mesmerize-core.readthedocs.io/ \
 User guide: https://mesmerize-core.readthedocs.io/en/latest/user_guide.html
 
-Please use the GitHub issue tracker for any issues. For smaller questions or discussion use gitter.
+## Getting Help
 
-gitter: https://gitter.im/mesmerize_discussion/mesmerize-viz
+Please use the GitHub issue tracker for any issues, and discussions for discussions. We no longer use gitter. If you are in the Slack, we usually only respond on slack around workshops. GitHub is for long term support.
 
-Video tutorial/virtual workshop from September 2022: https://www.youtube.com/watch?v=0AGiAaslJdk
+Video tutorial/virtual workshop from September 2022 (quite outdated, if you have question post on github): https://www.youtube.com/watch?v=0AGiAaslJdk
 
 # Overview
 
 ![batch_management](https://user-images.githubusercontent.com/9403332/179145962-82317da6-0340-44e4-83ba-7dace0300f55.png)
 
 # Visualization
 
-For visualization we strongly recommend [`fastplotlib`](https://github.com/kushalkolar/fastplotlib), a very new but very fast plotting library. Here are some examples of `fastplotlib` visualizations using `mesmerize-core` outputs. You can create these interactive plots within jupyter notebooks, therefore they will also work on cloud computing intrastructure!
-
-### View raw and motion corrected movie side by side:
-
-![mcorr](https://user-images.githubusercontent.com/9403332/210932452-5ed344dd-9a82-41ee-adc5-a9476e1f03a5.gif)
-
-### Contours from CNMF, good components shown here in cyan and bad components in magenta:
+Install [mesmerize-viz](https://github.com/kushalkolar/mesmerize-viz) for visualization. Mesmerize-viz gives you ready-to-use viuslizations for motion correction and CNMF - including component exploration, interactive component evaluation using metrics, and manual addition or removal of components. 
 
-![cnmf](https://user-images.githubusercontent.com/9403332/210932670-d797d301-839c-48d9-b11f-3330e076e0e4.gif)
-
-### Input movie, constructed movie `(A * C)`, residuals `(Y - A * C - b * f)`, and reconstructed background `(b * f)`:
-
-![cnmf-rcm](https://user-images.githubusercontent.com/9403332/210932903-b994359b-62d4-49fd-aa6b-cd4855ba873e.gif)
+```
+pip install mesmerize-viz
+```
 
-### Interactive Component evaluation after CNMF:
+:exclamation: **Harware requirements** The large CNMF visualizations with contours etc. usually require either a dedicated GPU or integrated GPU with access to at least 1GB of VRAM. 
 
-https://user-images.githubusercontent.com/9403332/191207883-2393664d-b5e1-49a5-84d1-8ed7eadcf7a0.mp4
+You may need to install drivers depending on your system, see the `fastplotlib` repo for more information: https://github.com/kushalkolar/fastplotlib#graphics-drivers
 
-As mentioned, fastplotlib is meant to be a fast plotting library which can handle **millions** of points. You can create highly complex and interactive plots to combine outputs from the CaImAn algorithms with other experimentally relevant analysis, such as behavioral data.
+If you use `fastplotlib` directly you can create highly complex and interactive plots to combine outputs from the CaImAn algorithms with other experimentally relevant analysis, such as behavioral data.
 
 ![epic](https://user-images.githubusercontent.com/9403332/210304473-f36f2aaf-319e-435b-bcc8-0e8d3e1ef282.gif)
 
 # Examples
 
 **See the `notebooks` directory for detailed examples.**
 
-Note that [`fastplotlib`](https://github.com/kushalkolar/fastplotlib) is required for the visualizations.
-
 # Installation
 
 ## For users
 
 The instructions below will install `mesmerize-core`.
 
-For visualization install `fastplotlib` into the same environment as `mesmerize-core`:
-
-```bash
-pip install "fastplotlib[notebook]"
-```
-
-You may need to install Vulkan drivers depending on your system, see the `fastplotlib` repo for more information: https://github.com/kushalkolar/fastplotlib#graphics-drivers
-
 ### Conda
 
-`mesmerize-core` is availabe as a conda package which also gives you CaImAn! These instructions will give you a working `mesmerize-core` along with `caiman` in the same environment.
+`mesmerize-core` is available as a conda package which also gives you CaImAn. These instructions will give you a working `mesmerize-core` along with `caiman` in the same environment.
 
-**Important note: Sometimes conda or mamba will get stuck at a step, such as creating an environment or installing a package. I found that pressing `Enter` on your keyboard can sometimes help it continue when it pauses.**
+**Important note: Sometimes conda or mamba will get stuck at a step, such as creating an environment or installing a package. Pressing `Enter` on your keyboard can sometimes help it continue when it pauses.**
 
 1. Install `mamba` into your base environment. Skip this step if you have `mamba`. This step may take 10 minutes and display several messages like "Solving environment: failed with..." but it should eventually install `mamba`.
 
 ```bash
 conda install -c conda-forge mamba
 
 # if conda is behaving slow, this command can sometimes help
@@ -156,21 +136,21 @@
 
 ```bash
 # run in ipython
 import mesmerize_core
 mesmerize_core.__version__
 ```
 
-6. Install `fastplotlib` for visualization into the same environment (run this in the anaconda prompt, not ipython). You may also need to install Vulkan drivers depending on your system, see the `fastplotlib` repo for more information: https://github.com/kushalkolar/fastplotlib#graphics-drivers
+6. Install `mesmerize-viz` for visualization into the same environment (run this in the anaconda prompt, not ipython). You may also need to install graphics drivers depending on your system, see the `fastplotlib` repo for more information: https://github.com/kushalkolar/fastplotlib#graphics-drivers
 
 ```bash
-pip install "fastplotlib[notebook]"
+pip install mesmerize-viz
 ```
 
-**Optional: install `simplejpeg` for much faster notebook visualization, you will need C compilers and [libjpeg-turbo](https://libjpeg-turbo.org/) for this to work:**
+**Strongly recommended: install `simplejpeg` for much faster notebook visualization, you will need C compilers and [libjpeg-turbo](https://libjpeg-turbo.org/) for this to work:**
 
 ```bash
 pip install simplejpeg
 ```
 
 ### python virtual environments
 
@@ -193,16 +173,19 @@
 pip install -r requirements.txt
 pip install .
 caimanmanager install
 
 # install mesmerize-core
 pip install mesmerize-core
 
-# install fastplotlib
-pip install "fastplotlib[notebook]"
+# install mesmerize-viz
+pip install mesmerize-viz
+
+# install simplejpeg
+pip install simplejpeg
 
 # you should now be able to import mesmerize_core
 # start ipython
 ipython
 
 # run in ipython
 import mesmerize_core
@@ -214,18 +197,15 @@
 ### conda
 
 ```bash
 # install mamba in your base environment
 conda install -c conda-forge mamba
 conda clean -a
 
-# on linux and mac you can use python=3.10
-conda create --name mesmerize-core python=3.10
-# on windows you MUST use python=3.9
-conda create --name mesmerize-core python=3.9
+conda create --name mesmerize-core
 
 # activate environment
 conda activate mesmerize-core
 conda clean -a
 
 # clone this repo
 git clone https://github.com/nel-lab/mesmerize-core.git
```

### Comparing `mesmerize-core-0.3.0/mesmerize_core.egg-info/SOURCES.txt` & `mesmerize_core-0.4.0/mesmerize_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.3.0/setup.py` & `mesmerize_core-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.3.0/tests/params.py` & `mesmerize_core-0.4.0/tests/params.py`

 * *Files identical despite different names*

### Comparing `mesmerize-core-0.3.0/tests/test_core.py` & `mesmerize_core-0.4.0/tests/test_core.py`

 * *Files identical despite different names*

