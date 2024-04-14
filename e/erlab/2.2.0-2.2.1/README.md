# Comparing `tmp/erlab-2.2.tar.gz` & `tmp/erlab-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlab-2.2.tar", last modified: Fri Apr 12 18:28:40 2024, max compression
+gzip compressed data, was "erlab-2.2.1.tar", last modified: Sun Apr 14 04:29:20 2024, max compression
```

## Comparing `erlab-2.2.tar` & `erlab-2.2.1.tar`

### file list

```diff
@@ -1,175 +1,176 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.165212 erlab-2.2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.121213 erlab-2.2/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.125213 erlab-2.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      469 2024-04-12 18:28:33.000000 erlab-2.2/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 root         (0) root         (0)      608 2024-04-12 18:28:33.000000 erlab-2.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.125213 erlab-2.2/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-12 18:28:33.000000 erlab-2.2/.github/workflows/pr.yml
--rw-r--r--   0 root         (0) root         (0)     1893 2024-04-12 18:28:33.000000 erlab-2.2/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     2898 2024-04-12 18:28:33.000000 erlab-2.2/.gitignore
--rw-r--r--   0 root         (0) root         (0)      893 2024-04-12 18:28:33.000000 erlab-2.2/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      796 2024-04-12 18:28:33.000000 erlab-2.2/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)   106158 2024-04-12 18:28:36.000000 erlab-2.2/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    35149 2024-04-12 18:28:33.000000 erlab-2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    47782 2024-04-12 18:28:40.161213 erlab-2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1473 2024-04-12 18:28:33.000000 erlab-2.2/PythonInterface.ipf
--rw-r--r--   0 root         (0) root         (0)     4823 2024-04-12 18:28:33.000000 erlab-2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.129212 erlab-2.2/docs/
--rw-r--r--   0 root         (0) root         (0)      638 2024-04-12 18:28:33.000000 erlab-2.2/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)      655 2024-04-12 18:28:33.000000 erlab-2.2/docs/environment.yml
--rw-r--r--   0 root         (0) root         (0)      804 2024-04-12 18:28:33.000000 erlab-2.2/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      451 2024-04-12 18:28:33.000000 erlab-2.2/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.129212 erlab-2.2/docs/source/
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/bibliography.rst
--rw-r--r--   0 root         (0) root         (0)    16040 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/conf.py
--rw-r--r--   0 root         (0) root         (0)    14522 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/contributing.rst
--rw-r--r--   0 root         (0) root         (0)      265 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/erlab.accessors.rst
--rw-r--r--   0 root         (0) root         (0)      101 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/erlab.analysis.rst
--rw-r--r--   0 root         (0) root         (0)      141 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/erlab.characterization.rst
--rw-r--r--   0 root         (0) root         (0)      485 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/erlab.constants.rst
--rw-r--r--   0 root         (0) root         (0)      116 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/erlab.interactive.rst
--rw-r--r--   0 root         (0) root         (0)       81 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/erlab.io.rst
--rw-r--r--   0 root         (0) root         (0)      236 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/erlab.lattice.rst
--rw-r--r--   0 root         (0) root         (0)      242 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/erlab.parallel.rst
--rw-r--r--   0 root         (0) root         (0)      174 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/erlab.plotting.rst
--rw-r--r--   0 root         (0) root         (0)     3806 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/getting-started.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.137213 erlab-2.2/docs/source/images/
--rw-r--r--   0 root         (0) root         (0)   321080 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/images/flowchart_multiple.pdf
--rw-r--r--   0 root         (0) root         (0)   317804 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/images/flowchart_single.pdf
--rw-r--r--   0 root         (0) root         (0)   996803 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/images/imagetool_dark.png
--rw-r--r--   0 root         (0) root         (0)   966547 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/images/imagetool_light.png
--rw-r--r--   0 root         (0) root         (0)   709231 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/images/ktool_1_dark.png
--rw-r--r--   0 root         (0) root         (0)   694078 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/images/ktool_1_light.png
--rw-r--r--   0 root         (0) root         (0)   703343 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/images/ktool_2_dark.png
--rw-r--r--   0 root         (0) root         (0)   686688 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/images/ktool_2_light.png
--rw-r--r--   0 root         (0) root         (0)     3285 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.137213 erlab-2.2/docs/source/pyplots/
--rw-r--r--   0 root         (0) root         (0)     2578 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/pyplots/norms.py
--rw-r--r--   0 root         (0) root         (0)     1344 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/reference.rst
--rw-r--r--   0 root         (0) root         (0)     2729 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/refs.bib
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.141213 erlab-2.2/docs/source/user-guide/
--rw-r--r--   0 root         (0) root         (0)    21971 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/user-guide/curve-fitting.ipynb
--rw-r--r--   0 root         (0) root         (0)     1278 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/user-guide/index.rst
--rw-r--r--   0 root         (0) root         (0)     5063 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/user-guide/indexing.ipynb
--rw-r--r--   0 root         (0) root         (0)    50534 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/user-guide/io.ipynb
--rw-r--r--   0 root         (0) root         (0)   379705 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/user-guide/kconv.ipynb
--rw-r--r--   0 root         (0) root         (0)    16293 2024-04-12 18:28:33.000000 erlab-2.2/docs/source/user-guide/plotting.ipynb
--rw-r--r--   0 root         (0) root         (0)      521 2024-04-12 18:28:33.000000 erlab-2.2/environment.yml
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-12 18:28:33.000000 erlab-2.2/environment_apple.yml
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-12 18:28:33.000000 erlab-2.2/environment_nogit.yml
--rw-r--r--   0 root         (0) root         (0)      603 2024-04-12 18:28:33.000000 erlab-2.2/environment_nogit_mkl.yml
--rw-r--r--   0 root         (0) root         (0)     4373 2024-04-12 18:28:33.000000 erlab-2.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      329 2024-04-12 18:28:33.000000 erlab-2.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 18:28:40.165212 erlab-2.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.121213 erlab-2.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.141213 erlab-2.2/src/erlab/
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-12 18:28:36.000000 erlab-2.2/src/erlab/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35543 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/accessors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.145213 erlab-2.2/src/erlab/analysis/
--rw-r--r--   0 root         (0) root         (0)      757 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5514 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/correlation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.145213 erlab-2.2/src/erlab/analysis/fit/
--rw-r--r--   0 root         (0) root         (0)      168 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/fit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.145213 erlab-2.2/src/erlab/analysis/fit/functions/
--rw-r--r--   0 root         (0) root         (0)      891 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/fit/functions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9760 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/fit/functions/dynamic.py
--rw-r--r--   0 root         (0) root         (0)     7809 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/fit/functions/general.py
--rw-r--r--   0 root         (0) root         (0)     6165 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/fit/minuit.py
--rw-r--r--   0 root         (0) root         (0)    11340 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/fit/models.py
--rw-r--r--   0 root         (0) root         (0)     1168 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/fit/spline.py
--rw-r--r--   0 root         (0) root         (0)    15393 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/gold.py
--rw-r--r--   0 root         (0) root         (0)    17325 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/image.py
--rw-r--r--   0 root         (0) root         (0)     9811 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/interpolate.py
--rw-r--r--   0 root         (0) root         (0)    10629 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.145213 erlab-2.2/src/erlab/analysis/mask/
--rw-r--r--   0 root         (0) root         (0)     5401 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/mask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8440 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/mask/polygon.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/transform.py
--rw-r--r--   0 root         (0) root         (0)     8658 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/analysis/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.145213 erlab-2.2/src/erlab/characterization/
--rw-r--r--   0 root         (0) root         (0)      191 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3093 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/characterization/resistance.py
--rw-r--r--   0 root         (0) root         (0)     1903 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/characterization/xrd.py
--rw-r--r--   0 root         (0) root         (0)     2152 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.149212 erlab-2.2/src/erlab/interactive/
--rw-r--r--   0 root         (0) root         (0)      540 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13953 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/bzplot.py
--rw-r--r--   0 root         (0) root         (0)    21311 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/colors.py
--rw-r--r--   0 root         (0) root         (0)    22774 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/curvefittingtool.py
--rw-r--r--   0 root         (0) root         (0)    11443 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/derivative.py
--rw-r--r--   0 root         (0) root         (0)    16300 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/dtool.ui
--rw-r--r--   0 root         (0) root         (0)     9454 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/exampledata.py
--rw-r--r--   0 root         (0) root         (0)    19072 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/fermiedge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.149212 erlab-2.2/src/erlab/interactive/imagetool/
--rw-r--r--   0 root         (0) root         (0)    19705 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/imagetool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.153213 erlab-2.2/src/erlab/interactive/imagetool/_deprecated/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/imagetool/_deprecated/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51945 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
--rw-r--r--   0 root         (0) root         (0)   114560 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
--rw-r--r--   0 root         (0) root         (0)    27081 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/imagetool/controls.py
--rw-r--r--   0 root         (0) root         (0)    54122 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/imagetool/core.py
--rw-r--r--   0 root         (0) root         (0)    13907 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/imagetool/fastbinning.py
--rw-r--r--   0 root         (0) root         (0)    25270 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/imagetool/slicer.py
--rw-r--r--   0 root         (0) root         (0)    15835 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/kspace.py
--rw-r--r--   0 root         (0) root         (0)    19382 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/ktool.ui
--rw-r--r--   0 root         (0) root         (0)     3341 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/masktool.py
--rw-r--r--   0 root         (0) root         (0)    54143 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/interactive/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.153213 erlab-2.2/src/erlab/io/
--rw-r--r--   0 root         (0) root         (0)     2160 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31737 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/io/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6905 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/io/igor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.153213 erlab-2.2/src/erlab/io/plugins/
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/io/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3672 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/io/plugins/da30.py
--rw-r--r--   0 root         (0) root         (0)     1185 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/io/plugins/kriss.py
--rw-r--r--   0 root         (0) root         (0)     7594 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/io/plugins/merlin.py
--rw-r--r--   0 root         (0) root         (0)     7804 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/io/plugins/ssrl52.py
--rw-r--r--   0 root         (0) root         (0)     6777 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/io/utilities.py
--rw-r--r--   0 root         (0) root         (0)     2515 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/lattice.py
--rw-r--r--   0 root         (0) root         (0)     2242 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/parallel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.157213 erlab-2.2/src/erlab/plotting/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.157213 erlab-2.2/src/erlab/plotting/IgorCT/
--rw-r--r--   0 root         (0) root         (0)     3379 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/IgorCT/Blue-White.txt
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/IgorCT/BlueHot.ibw
--rw-r--r--   0 root         (0) root         (0)     3526 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
--rw-r--r--   0 root         (0) root         (0)     3530 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
--rw-r--r--   0 root         (0) root         (0)     3531 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/IgorCT/ColdWarm.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/IgorCT/PlanetEarth.ibw
--rw-r--r--   0 root         (0) root         (0)     1920 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/IgorCT/ametrine.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/IgorCT/isolum.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/IgorCT/morgenstemning.ibw
--rw-r--r--   0 root         (0) root         (0)     2026 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29010 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/annotations.py
--rw-r--r--   0 root         (0) root         (0)    18284 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/atoms.py
--rw-r--r--   0 root         (0) root         (0)     4295 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/bz.py
--rw-r--r--   0 root         (0) root         (0)    37209 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/colors.py
--rw-r--r--   0 root         (0) root         (0)     2657 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/erplot.py
--rw-r--r--   0 root         (0) root         (0)    31070 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/general.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/plot3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.157213 erlab-2.2/src/erlab/plotting/stylelib/
--rw-r--r--   0 root         (0) root         (0)     6839 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/stylelib/fira.mplstyle
--rw-r--r--   0 root         (0) root         (0)     6826 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/stylelib/firalight.mplstyle
--rw-r--r--   0 root         (0) root         (0)    14358 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/stylelib/khan.mplstyle
--rw-r--r--   0 root         (0) root         (0)     9160 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/stylelib/nature.mplstyle
--rw-r--r--   0 root         (0) root         (0)      630 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/stylelib/poster.mplstyle
--rw-r--r--   0 root         (0) root         (0)     7023 2024-04-12 18:28:33.000000 erlab-2.2/src/erlab/plotting/stylelib/times.mplstyle
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.161213 erlab-2.2/src/erlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)    47782 2024-04-12 18:28:40.000000 erlab-2.2/src/erlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4718 2024-04-12 18:28:40.000000 erlab-2.2/src/erlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 18:28:40.000000 erlab-2.2/src/erlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      536 2024-04-12 18:28:40.000000 erlab-2.2/src/erlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-12 18:28:40.000000 erlab-2.2/src/erlab.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.161213 erlab-2.2/templates/
--rw-r--r--   0 root         (0) root         (0)     1063 2024-04-12 18:28:33.000000 erlab-2.2/templates/.macros.j2
--rw-r--r--   0 root         (0) root         (0)      161 2024-04-12 18:28:33.000000 erlab-2.2/templates/.release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)      423 2024-04-12 18:28:33.000000 erlab-2.2/templates/CHANGELOG.md.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.121213 erlab-2.2/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 18:28:40.161213 erlab-2.2/tests/analysis/
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-12 18:28:33.000000 erlab-2.2/tests/analysis/test_fastbinning.py
--rw-r--r--   0 root         (0) root         (0)     4484 2024-04-12 18:28:33.000000 erlab-2.2/tests/analysis/test_fit_functions_dynamic.py
--rw-r--r--   0 root         (0) root         (0)     4652 2024-04-12 18:28:33.000000 erlab-2.2/tests/analysis/test_fit_functions_general.py
--rw-r--r--   0 root         (0) root         (0)     5228 2024-04-12 18:28:33.000000 erlab-2.2/tests/analysis/test_image.py
--rw-r--r--   0 root         (0) root         (0)      598 2024-04-12 18:28:33.000000 erlab-2.2/tests/analysis/test_interpolate.py
--rw-r--r--   0 root         (0) root         (0)     2423 2024-04-12 18:28:33.000000 erlab-2.2/tests/analysis/test_kspace.py
--rw-r--r--   0 root         (0) root         (0)      718 2024-04-12 18:28:33.000000 erlab-2.2/tests/analysis/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.524856 erlab-2.2.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.480856 erlab-2.2.1/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.488856 erlab-2.2.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      469 2024-04-14 04:29:13.000000 erlab-2.2.1/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 root         (0) root         (0)      608 2024-04-14 04:29:13.000000 erlab-2.2.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.488856 erlab-2.2.1/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-14 04:29:13.000000 erlab-2.2.1/.github/workflows/pr.yml
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-04-14 04:29:13.000000 erlab-2.2.1/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-04-14 04:29:13.000000 erlab-2.2.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      893 2024-04-14 04:29:13.000000 erlab-2.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      796 2024-04-14 04:29:13.000000 erlab-2.2.1/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)   107661 2024-04-14 04:29:16.000000 erlab-2.2.1/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2024-04-14 04:29:13.000000 erlab-2.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    47789 2024-04-14 04:29:20.524856 erlab-2.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-04-14 04:29:13.000000 erlab-2.2.1/PythonInterface.ipf
+-rw-r--r--   0 root         (0) root         (0)     4823 2024-04-14 04:29:13.000000 erlab-2.2.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.488856 erlab-2.2.1/docs/
+-rw-r--r--   0 root         (0) root         (0)      638 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)      682 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      804 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)      469 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.492856 erlab-2.2.1/docs/source/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/bibliography.rst
+-rw-r--r--   0 root         (0) root         (0)    16040 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)    14522 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)      265 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/erlab.accessors.rst
+-rw-r--r--   0 root         (0) root         (0)      101 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/erlab.analysis.rst
+-rw-r--r--   0 root         (0) root         (0)      141 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/erlab.characterization.rst
+-rw-r--r--   0 root         (0) root         (0)      485 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/erlab.constants.rst
+-rw-r--r--   0 root         (0) root         (0)      116 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/erlab.interactive.rst
+-rw-r--r--   0 root         (0) root         (0)       81 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/erlab.io.rst
+-rw-r--r--   0 root         (0) root         (0)      236 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/erlab.lattice.rst
+-rw-r--r--   0 root         (0) root         (0)      242 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/erlab.parallel.rst
+-rw-r--r--   0 root         (0) root         (0)      174 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/erlab.plotting.rst
+-rw-r--r--   0 root         (0) root         (0)     3806 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/getting-started.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.500856 erlab-2.2.1/docs/source/images/
+-rw-r--r--   0 root         (0) root         (0)   321080 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/images/flowchart_multiple.pdf
+-rw-r--r--   0 root         (0) root         (0)   317804 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/images/flowchart_single.pdf
+-rw-r--r--   0 root         (0) root         (0)   996803 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/images/imagetool_dark.png
+-rw-r--r--   0 root         (0) root         (0)   966547 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/images/imagetool_light.png
+-rw-r--r--   0 root         (0) root         (0)   709231 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/images/ktool_1_dark.png
+-rw-r--r--   0 root         (0) root         (0)   694078 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/images/ktool_1_light.png
+-rw-r--r--   0 root         (0) root         (0)   703343 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/images/ktool_2_dark.png
+-rw-r--r--   0 root         (0) root         (0)   686688 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/images/ktool_2_light.png
+-rw-r--r--   0 root         (0) root         (0)     3357 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.500856 erlab-2.2.1/docs/source/pyplots/
+-rw-r--r--   0 root         (0) root         (0)     2578 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/pyplots/norms.py
+-rw-r--r--   0 root         (0) root         (0)     1344 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/reference.rst
+-rw-r--r--   0 root         (0) root         (0)     2729 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/refs.bib
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.500856 erlab-2.2.1/docs/source/user-guide/
+-rw-r--r--   0 root         (0) root         (0)    22039 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/user-guide/curve-fitting.ipynb
+-rw-r--r--   0 root         (0) root         (0)     1278 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/user-guide/index.rst
+-rw-r--r--   0 root         (0) root         (0)     5063 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/user-guide/indexing.ipynb
+-rw-r--r--   0 root         (0) root         (0)    50534 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/user-guide/io.ipynb
+-rw-r--r--   0 root         (0) root         (0)   379705 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/user-guide/kconv.ipynb
+-rw-r--r--   0 root         (0) root         (0)    16293 2024-04-14 04:29:13.000000 erlab-2.2.1/docs/source/user-guide/plotting.ipynb
+-rw-r--r--   0 root         (0) root         (0)      521 2024-04-14 04:29:13.000000 erlab-2.2.1/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-14 04:29:13.000000 erlab-2.2.1/environment_apple.yml
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-14 04:29:13.000000 erlab-2.2.1/environment_nogit.yml
+-rw-r--r--   0 root         (0) root         (0)      603 2024-04-14 04:29:13.000000 erlab-2.2.1/environment_nogit_mkl.yml
+-rw-r--r--   0 root         (0) root         (0)     4381 2024-04-14 04:29:13.000000 erlab-2.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      329 2024-04-14 04:29:13.000000 erlab-2.2.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-14 04:29:20.524856 erlab-2.2.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.480856 erlab-2.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.504856 erlab-2.2.1/src/erlab/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-14 04:29:16.000000 erlab-2.2.1/src/erlab/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35514 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/accessors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.504856 erlab-2.2.1/src/erlab/analysis/
+-rw-r--r--   0 root         (0) root         (0)      757 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5514 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/correlation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.508856 erlab-2.2.1/src/erlab/analysis/fit/
+-rw-r--r--   0 root         (0) root         (0)      168 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/fit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.508856 erlab-2.2.1/src/erlab/analysis/fit/functions/
+-rw-r--r--   0 root         (0) root         (0)      955 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/fit/functions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10583 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/fit/functions/dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     8402 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/fit/functions/general.py
+-rw-r--r--   0 root         (0) root         (0)     6510 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/fit/minuit.py
+-rw-r--r--   0 root         (0) root         (0)    11749 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/fit/models.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/fit/spline.py
+-rw-r--r--   0 root         (0) root         (0)    15393 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/gold.py
+-rw-r--r--   0 root         (0) root         (0)    17325 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/image.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/interpolate.py
+-rw-r--r--   0 root         (0) root         (0)    10629 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.508856 erlab-2.2.1/src/erlab/analysis/mask/
+-rw-r--r--   0 root         (0) root         (0)     5401 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/mask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8440 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/mask/polygon.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/transform.py
+-rw-r--r--   0 root         (0) root         (0)     8658 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/analysis/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.508856 erlab-2.2.1/src/erlab/characterization/
+-rw-r--r--   0 root         (0) root         (0)      191 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/characterization/resistance.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/characterization/xrd.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.512856 erlab-2.2.1/src/erlab/interactive/
+-rw-r--r--   0 root         (0) root         (0)      540 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13953 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/bzplot.py
+-rw-r--r--   0 root         (0) root         (0)    21311 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/colors.py
+-rw-r--r--   0 root         (0) root         (0)    22774 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/curvefittingtool.py
+-rw-r--r--   0 root         (0) root         (0)    11443 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/derivative.py
+-rw-r--r--   0 root         (0) root         (0)    16300 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/dtool.ui
+-rw-r--r--   0 root         (0) root         (0)     9454 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/exampledata.py
+-rw-r--r--   0 root         (0) root         (0)    19072 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/fermiedge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.512856 erlab-2.2.1/src/erlab/interactive/imagetool/
+-rw-r--r--   0 root         (0) root         (0)    19705 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/imagetool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.512856 erlab-2.2.1/src/erlab/interactive/imagetool/_deprecated/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/imagetool/_deprecated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51945 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
+-rw-r--r--   0 root         (0) root         (0)   114560 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
+-rw-r--r--   0 root         (0) root         (0)    27081 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/imagetool/controls.py
+-rw-r--r--   0 root         (0) root         (0)    54122 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/imagetool/core.py
+-rw-r--r--   0 root         (0) root         (0)    13907 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/imagetool/fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)    25270 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/imagetool/slicer.py
+-rw-r--r--   0 root         (0) root         (0)    15835 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/kspace.py
+-rw-r--r--   0 root         (0) root         (0)    19382 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/ktool.ui
+-rw-r--r--   0 root         (0) root         (0)     3341 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/masktool.py
+-rw-r--r--   0 root         (0) root         (0)    54143 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/interactive/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.512856 erlab-2.2.1/src/erlab/io/
+-rw-r--r--   0 root         (0) root         (0)     2160 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31737 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/io/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6905 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/io/igor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.516856 erlab-2.2.1/src/erlab/io/plugins/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/io/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3672 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/io/plugins/da30.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/io/plugins/kriss.py
+-rw-r--r--   0 root         (0) root         (0)     7594 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/io/plugins/merlin.py
+-rw-r--r--   0 root         (0) root         (0)     7804 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/io/plugins/ssrl52.py
+-rw-r--r--   0 root         (0) root         (0)     6777 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/io/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/lattice.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/parallel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.516856 erlab-2.2.1/src/erlab/plotting/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.520856 erlab-2.2.1/src/erlab/plotting/IgorCT/
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/IgorCT/Blue-White.txt
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/IgorCT/BlueHot.ibw
+-rw-r--r--   0 root         (0) root         (0)     3526 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
+-rw-r--r--   0 root         (0) root         (0)     3530 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
+-rw-r--r--   0 root         (0) root         (0)     3531 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/IgorCT/ColdWarm.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/IgorCT/PlanetEarth.ibw
+-rw-r--r--   0 root         (0) root         (0)     1920 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/IgorCT/ametrine.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/IgorCT/isolum.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/IgorCT/morgenstemning.ibw
+-rw-r--r--   0 root         (0) root         (0)     2026 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29010 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/annotations.py
+-rw-r--r--   0 root         (0) root         (0)    18284 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/atoms.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/bz.py
+-rw-r--r--   0 root         (0) root         (0)    37209 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/colors.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/erplot.py
+-rw-r--r--   0 root         (0) root         (0)    31070 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/general.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/plot3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.520856 erlab-2.2.1/src/erlab/plotting/stylelib/
+-rw-r--r--   0 root         (0) root         (0)     6839 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/stylelib/fira.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     6826 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/stylelib/firalight.mplstyle
+-rw-r--r--   0 root         (0) root         (0)    14358 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/stylelib/khan.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     9160 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/stylelib/nature.mplstyle
+-rw-r--r--   0 root         (0) root         (0)      630 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/stylelib/poster.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     7023 2024-04-14 04:29:13.000000 erlab-2.2.1/src/erlab/plotting/stylelib/times.mplstyle
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.524856 erlab-2.2.1/src/erlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    47789 2024-04-14 04:29:20.000000 erlab-2.2.1/src/erlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4752 2024-04-14 04:29:20.000000 erlab-2.2.1/src/erlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-14 04:29:20.000000 erlab-2.2.1/src/erlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      543 2024-04-14 04:29:20.000000 erlab-2.2.1/src/erlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-14 04:29:20.000000 erlab-2.2.1/src/erlab.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.520856 erlab-2.2.1/templates/
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-14 04:29:13.000000 erlab-2.2.1/templates/.macros.j2
+-rw-r--r--   0 root         (0) root         (0)      161 2024-04-14 04:29:13.000000 erlab-2.2.1/templates/.release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)      423 2024-04-14 04:29:13.000000 erlab-2.2.1/templates/CHANGELOG.md.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.484856 erlab-2.2.1/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-14 04:29:20.524856 erlab-2.2.1/tests/analysis/
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-14 04:29:13.000000 erlab-2.2.1/tests/analysis/test_fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)     4484 2024-04-14 04:29:13.000000 erlab-2.2.1/tests/analysis/test_fit_functions_dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     4652 2024-04-14 04:29:13.000000 erlab-2.2.1/tests/analysis/test_fit_functions_general.py
+-rw-r--r--   0 root         (0) root         (0)     6036 2024-04-14 04:29:13.000000 erlab-2.2.1/tests/analysis/test_fit_models.py
+-rw-r--r--   0 root         (0) root         (0)     5228 2024-04-14 04:29:13.000000 erlab-2.2.1/tests/analysis/test_image.py
+-rw-r--r--   0 root         (0) root         (0)      598 2024-04-14 04:29:13.000000 erlab-2.2.1/tests/analysis/test_interpolate.py
+-rw-r--r--   0 root         (0) root         (0)     2423 2024-04-14 04:29:13.000000 erlab-2.2.1/tests/analysis/test_kspace.py
+-rw-r--r--   0 root         (0) root         (0)      718 2024-04-14 04:29:13.000000 erlab-2.2.1/tests/analysis/test_utilities.py
```

### Comparing `erlab-2.2/.github/ISSUE_TEMPLATE/feature_request.md` & `erlab-2.2.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `erlab-2.2/.github/workflows/pr.yml` & `erlab-2.2.1/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.2/.github/workflows/release.yml` & `erlab-2.2.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.2/.gitignore` & `erlab-2.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `erlab-2.2/.pre-commit-config.yaml` & `erlab-2.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `erlab-2.2/.readthedocs.yaml` & `erlab-2.2.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `erlab-2.2/CHANGELOG.md` & `erlab-2.2.1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,44 @@
 # CHANGELOG
 
 
 
+## v2.2.1 (2024-04-14)
+
+### Chore
+
+* (**deps**) pin lmfit&lt;1.3.0 ([`915fc60`](https://github.com/kmnhan/erlabpy/commit/915fc60e8e7e8a2dfc9a56bbc1afd1c737bcc3d5))
+
+### Documentation
+
+* rephrase some docstrings ([`e67597c`](https://github.com/kmnhan/erlabpy/commit/e67597c90e009748d1bd39c43c03a8cc1b439840))
+
+* add link to changelog ([`fbb6d32`](https://github.com/kmnhan/erlabpy/commit/fbb6d3254ae254278dec74b2ce9965e20a4dc88d))
+
+* add ipywidgets as requirement ([`41024eb`](https://github.com/kmnhan/erlabpy/commit/41024ebbef02609d9a2fc70c4630fec06aa96012))
+
+* temporarily pin lmfit&lt;1.3.0 to build docs ([`6b86ac2`](https://github.com/kmnhan/erlabpy/commit/6b86ac2f89c2a822753f3fbe106eb5dfaa2cb22c))
+
+### Fix
+
+* (**fit**) add sigma and amplitude expressions to MultiPeakModel parameters ([`3f6ba5e`](https://github.com/kmnhan/erlabpy/commit/3f6ba5e84922129296183e02255506df73da0276))
+
+* (**fit.minuit**) properly handle parameters constrained with expressions ([`d03f012`](https://github.com/kmnhan/erlabpy/commit/d03f012b4fde92f445a24657dca1fb5b3600fa45))
+
+### Refactor
+
+* set informative model name for MultiPeakModel ([`d14ee9d`](https://github.com/kmnhan/erlabpy/commit/d14ee9d6ac7962207700de50039a5b7a858fea6a))
+
+* add gaussian and lorentzian for consistency ([`07c0dfb`](https://github.com/kmnhan/erlabpy/commit/07c0dfb9ecfb882e4f5f0ccfe942c1a835b613b2))
+
+### Test
+
+* add tests for fit models ([`3f9125c`](https://github.com/kmnhan/erlabpy/commit/3f9125ce19a4a30dd31b9d039d6614a8cae19966))
+
+
 ## v2.2.0 (2024-04-12)
 
 ### Documentation
 
 * improve fitting documentation ([`9e0a106`](https://github.com/kmnhan/erlabpy/commit/9e0a10611a32ac75798e68f864cff55b5661330f))
 
 * add curve fitting guide ([`ff9743c`](https://github.com/kmnhan/erlabpy/commit/ff9743c2203eb773af6bdb8d88426907f4300924))
```

### Comparing `erlab-2.2/LICENSE` & `erlab-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `erlab-2.2/PKG-INFO` & `erlab-2.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.2.0
+Version: 2.2.1
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -694,15 +694,15 @@
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: h5netcdf>=1.2.0
 Requires-Dist: igor2>=0.5.6
 Requires-Dist: iminuit>=2.25.2
 Requires-Dist: joblib>=1.3.2
-Requires-Dist: lmfit>=1.2.0
+Requires-Dist: lmfit<1.3.0,>=1.2.0
 Requires-Dist: matplotlib>=3.8.0
 Requires-Dist: numba-progress>=1.0.0
 Requires-Dist: numba>=0.59.0
 Requires-Dist: numbagg>=0.8.1
 Requires-Dist: numpy>=1.26.0
 Requires-Dist: pyperclip>=1.8.2
 Requires-Dist: pyqtgraph>=0.13.1
```

### Comparing `erlab-2.2/PythonInterface.ipf` & `erlab-2.2.1/PythonInterface.ipf`

 * *Files identical despite different names*

### Comparing `erlab-2.2/README.md` & `erlab-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `erlab-2.2/docs/Makefile` & `erlab-2.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `erlab-2.2/docs/environment.yml` & `erlab-2.2.1/docs/environment.yml`

 * *Files 24% similar despite different names*

```diff
@@ -28,12 +28,14 @@
   - sphinx-copybutton
   - sphinxcontrib-bibtex
   - pybtex
   - nbsphinx
   - furo
   - sphinx-design
   - pyperclip
+  - ipywidgets
+  - ipython
   - pip:
     - pyqt6>=6.2.2
     - csaps
     - -e git+https://github.com/kmnhan/erlabpy.git#egg=erlab
     - sphinx-qt-documentation
```

### Comparing `erlab-2.2/docs/make.bat` & `erlab-2.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `erlab-2.2/docs/source/conf.py` & `erlab-2.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/docs/source/contributing.rst` & `erlab-2.2.1/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.2/docs/source/getting-started.rst` & `erlab-2.2.1/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.2/docs/source/images/flowchart_multiple.pdf` & `erlab-2.2.1/docs/source/images/flowchart_multiple.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.2/docs/source/images/flowchart_single.pdf` & `erlab-2.2.1/docs/source/images/flowchart_single.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.2/docs/source/images/imagetool_dark.png` & `erlab-2.2.1/docs/source/images/imagetool_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.2/docs/source/images/imagetool_light.png` & `erlab-2.2.1/docs/source/images/imagetool_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.2/docs/source/images/ktool_1_dark.png` & `erlab-2.2.1/docs/source/images/ktool_1_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.2/docs/source/images/ktool_1_light.png` & `erlab-2.2.1/docs/source/images/ktool_1_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.2/docs/source/images/ktool_2_dark.png` & `erlab-2.2.1/docs/source/images/ktool_2_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.2/docs/source/images/ktool_2_light.png` & `erlab-2.2.1/docs/source/images/ktool_2_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.2/docs/source/index.rst` & `erlab-2.2.1/docs/source/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -92,7 +92,8 @@
    :caption: Contents
 
    getting-started
    user-guide/index
    reference
    contributing
    bibliography
+   Changelog <https://github.com/kmnhan/erlabpy/blob/main/CHANGELOG.md>
```

### Comparing `erlab-2.2/docs/source/pyplots/norms.py` & `erlab-2.2.1/docs/source/pyplots/norms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/docs/source/reference.rst` & `erlab-2.2.1/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.2/docs/source/refs.bib` & `erlab-2.2.1/docs/source/refs.bib`

 * *Files identical despite different names*

### Comparing `erlab-2.2/docs/source/user-guide/curve-fitting.ipynb` & `erlab-2.2.1/docs/source/user-guide/curve-fitting.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996307319223986%*

 * *Differences: {"'cells'": '{25: {\'source\': {insert: [(3, \'plt.plot(x, comps["1Peak_p0"], "--", '*

 * *            'label="Peak")\\n\'), (4, \'plt.plot(x, comps["1Peak_bkg"], "--", '*

 * *            'label="Background")\\n\')], delete: [4, 3]}}, 35: {\'source\': {insert: [(5, \'    - '*

 * *            'Requires `ipywidgets <https://github.com/jupyter-widgets/ipywidgets>`_ to be '*

 * *            "installed.\\n'), (6, '    - If you are viewing this documentation online, changing "*

 * *            "the sliders won’t change the plot. run the  […]*

```diff
@@ -353,16 +353,16 @@
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "comps = result.eval_components()\n",
                 "plt.errorbar(x, y, yerr, fmt=\"o\", zorder=-1, alpha=0.3)\n",
                 "plt.plot(x, result.eval(), label=\"Best fit\")\n",
-                "plt.plot(x, comps[\"MultiPeakFunction_p0\"], \"--\", label=\"Peak\")\n",
-                "plt.plot(x, comps[\"MultiPeakFunction_bkg\"], \"--\", label=\"Background\")\n",
+                "plt.plot(x, comps[\"1Peak_p0\"], \"--\", label=\"Peak\")\n",
+                "plt.plot(x, comps[\"1Peak_bkg\"], \"--\", label=\"Background\")\n",
                 "plt.legend()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -515,16 +515,16 @@
             },
             "source": [
                 "You can also use the `interactive fitting interface\n",
                 "<https://scikit-hep.org/iminuit/notebooks/interactive.html>`_ provided by iminuit.\n",
                 "\n",
                 ".. note::\n",
                 "\n",
-                "    If you are viewing this documentation online, changing the sliders won\u2019t change the\n",
-                "    plot. run the code locally to try it out.\n"
+                "    - Requires `ipywidgets <https://github.com/jupyter-widgets/ipywidgets>`_ to be installed.\n",
+                "    - If you are viewing this documentation online, changing the sliders won\u2019t change the plot. run the code locally to try it out.\n"
             ]
         },
         {
             "cell_type": "raw",
             "metadata": {
                 "vscode": {
                     "languageId": "raw"
```

### Comparing `erlab-2.2/docs/source/user-guide/index.rst` & `erlab-2.2.1/docs/source/user-guide/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.2/docs/source/user-guide/indexing.ipynb` & `erlab-2.2.1/docs/source/user-guide/indexing.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.2/docs/source/user-guide/io.ipynb` & `erlab-2.2.1/docs/source/user-guide/io.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.2/docs/source/user-guide/kconv.ipynb` & `erlab-2.2.1/docs/source/user-guide/kconv.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.2/docs/source/user-guide/plotting.ipynb` & `erlab-2.2.1/docs/source/user-guide/plotting.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.2/environment.yml` & `erlab-2.2.1/environment.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.2/environment_apple.yml` & `erlab-2.2.1/environment_apple.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.2/environment_nogit.yml` & `erlab-2.2.1/environment_nogit.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.2/environment_nogit_mkl.yml` & `erlab-2.2.1/environment_nogit_mkl.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.2/pyproject.toml` & `erlab-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ]
 dynamic = ["version"]
 dependencies = [
     "h5netcdf>=1.2.0",
     "igor2>=0.5.6",
     "iminuit>=2.25.2",
     "joblib>=1.3.2",
-    "lmfit>=1.2.0",
+    "lmfit>=1.2.0, <1.3.0",
     "matplotlib>=3.8.0",
     "numba-progress>=1.0.0",
     "numba>=0.59.0",
     "numbagg>=0.8.1",
     "numpy>=1.26.0",
     "pyperclip>=1.8.2",
     "pyqtgraph>=0.13.1",
```

### Comparing `erlab-2.2/src/erlab/accessors.py` & `erlab-2.2.1/src/erlab/accessors.py`

 * *Files 2% similar despite different names*

```diff
@@ -400,16 +400,16 @@
         self._obj.attrs["inner_potential"] = float(value)
 
     @property
     def work_function(self) -> float:
         """Work function of the sample in eV.
 
         The work function is stored in the ``sample_workfunction`` attribute of the
-        data. If the work function is not set, a warning is issued and a default value
-        of 4.5 eV is assumed.
+        data. If not found, a warning is issued and a default value of 4.5 eV is
+        assumed.
 
         Note
         ----
         This property provides a setter method that takes a float value and sets the
         data attribute accordingly.
 
         Example
@@ -430,20 +430,21 @@
 
     @work_function.setter
     def work_function(self, value: float):
         self._obj.attrs["sample_workfunction"] = float(value)
 
     @property
     def angle_resolution(self) -> float:
-        """Angular resolution of the data in degrees.
+        """Retrieve the angular resolution of the data in degrees.
 
-        The angular resolution is stored in the ``angle_resolution`` attribute of the
-        data. If it is not set, a default value of 0.1° is silently used. It is used in
-        `best_kp_resolution` when automatically estimating momentum steps through
-        `estimate_resolution`.
+        Checks for the ``angle_resolution`` attribute of the data. If not found, a
+        default value of 0.1° is silently assumed.
+
+        This property is used in `best_kp_resolution` upon estimating momentum step
+        sizes through `estimate_resolution`.
         """
 
         try:
             return float(self._obj.attrs["angle_resolution"])
         except KeyError:
             # warnings.warn(
             #     "Angle resolution not found in data attributes, assuming 0.1 degrees"
```

### Comparing `erlab-2.2/src/erlab/analysis/__init__.py` & `erlab-2.2.1/src/erlab/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/analysis/correlation.py` & `erlab-2.2.1/src/erlab/analysis/correlation.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/analysis/fit/functions/__init__.py` & `erlab-2.2.1/src/erlab/analysis/fit/functions/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,15 +22,17 @@
     "do_convolve",
     "do_convolve_y",
     "dynes",
     "fermi_dirac",
     "fermi_dirac_linbkg",
     "fermi_dirac_linbkg_broad",
     "gaussian_wh",
+    "gaussian",
     "lorentzian_wh",
+    "lorentzian",
     "step_broad",
     "step_linbkg_broad",
 ]
 
 from erlab.analysis.fit.functions.dynamic import (
     FermiEdge2dFunction,
     MultiPeakFunction,
@@ -42,11 +44,13 @@
     do_convolve,
     do_convolve_y,
     dynes,
     fermi_dirac,
     fermi_dirac_linbkg,
     fermi_dirac_linbkg_broad,
     gaussian_wh,
+    gaussian,
     lorentzian_wh,
+    lorentzian,
     step_broad,
     step_linbkg_broad,
 )
```

### Comparing `erlab-2.2/src/erlab/analysis/fit/functions/dynamic.py` & `erlab-2.2.1/src/erlab/analysis/fit/functions/dynamic.py`

 * *Files 4% similar despite different names*

```diff
@@ -232,17 +232,38 @@
             kws += [("resolution", 0.02)]
 
         for i, func in enumerate(self.peak_funcs):
             for arg, val in self.peak_all_args[func]["kwargs"].items():
                 kws.append((f"p{i}_{arg}", val))
         return kws
 
+    def sigma_expr(self, index: int, prefix: str) -> str | None:
+        if self._peak_funcs[index] == gaussian_wh:
+            return f"{prefix}p{index}_width / (2 * sqrt(2 * log(2)))"
+        elif self._peak_funcs[index] == lorentzian_wh:
+            return f"{prefix}p{index}_width / 2"
+        else:
+            return None
+
+    def amplitude_expr(self, index: int, prefix: str) -> str | None:
+        if self._peak_funcs[index] == gaussian_wh:
+            return f"{prefix}p{index}_height * {prefix}p{index}_sigma / sqrt(2 * pi)"
+        elif self._peak_funcs[index] == lorentzian_wh:
+            return f"{prefix}p{index}_height * {prefix}p{index}_sigma * pi"
+        else:
+            return None
+
     def eval_peak(self, index: int, x: npt.NDArray[np.float64], **params: dict):
         return self.peak_funcs[index](
-            x, **{k[3:]: v for k, v in params.items() if k.startswith(f"p{index}")}
+            x,
+            **{
+                k[3:]: v
+                for k, v in params.items()
+                if k.startswith(f"p{index}") and not k.endswith(("sigma", "amplitude"))
+            },
         )
 
     def eval_bkg(self, x: npt.NDArray[np.float64], **params: dict):
         return params["lin_bkg"] * x + params["const_bkg"]
 
     def pre_call(
         self, x: npt.NDArray[np.float64], **params: dict
```

### Comparing `erlab-2.2/src/erlab/analysis/fit/functions/general.py` & `erlab-2.2.1/src/erlab/analysis/fit/functions/general.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,17 @@
     "do_convolve",
     "do_convolve_y",
     "dynes",
     "fermi_dirac",
     "fermi_dirac_linbkg",
     "fermi_dirac_linbkg_broad",
     "gaussian_wh",
+    "gaussian",
     "lorentzian_wh",
+    "lorentzian",
     "step_broad",
     "step_linbkg_broad",
 ]
 
 from collections.abc import Callable
 
 import numba
@@ -25,14 +27,15 @@
 import numpy.typing as npt
 import scipy.special
 
 from erlab.constants import kb_eV
 
 #: From :mod:`lmfit.lineshapes`, equal to `numpy.finfo(numpy.float64).resolution`
 TINY: float = 1.0e-15
+S2PI = np.sqrt(2 * np.pi)
 
 
 @numba.njit(cache=True)
 def _gen_kernel(
     x: npt.NDArray[np.float64], resolution: float, pad: int = 5
 ) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.float64]]:
     r"""Generate a Gaussian kernel for convolution.
@@ -61,15 +64,15 @@
 
     extended = np.linspace(x[0] - x_pad, x[-1] + x_pad, 2 * n_pad + len(x))
     gauss = (
         delta_x
         * np.exp(
             -(np.linspace(-x_pad, x_pad, 2 * n_pad + 1) ** 2) / max(TINY, 2 * sigma**2)
         )
-        / max(TINY, np.sqrt(2 * np.pi) * sigma)
+        / max(TINY, S2PI * sigma)
     )
     return extended, gauss
 
 
 def do_convolve(
     x: npt.NDArray[np.float64],
     func: Callable,
@@ -133,28 +136,46 @@
     """
     return height * np.exp(
         -16 * np.log(2) * (1.0 * x - center) ** 2 / max(TINY, width**2)
     )
 
 
 @numba.njit(cache=True)
+def gaussian(
+    x: npt.NDArray[np.float64], center: float, sigma: float, amplitude: float
+) -> npt.NDArray[np.float64]:
+    return (amplitude / (max(TINY, S2PI * sigma))) * np.exp(
+        -((1.0 * x - center) ** 2) / max(TINY, (2 * sigma**2))
+    )
+
+
+@numba.njit(cache=True)
 def lorentzian_wh(
     x: npt.NDArray[np.float64], center: float, width: float, height: float
 ) -> npt.NDArray[np.float64]:
     r"""Lorentzian parametrized with FWHM and peak height.
 
     Note
     ----
     :math:`\sigma=w/2`
 
     """
     return height / (1 + 4 * ((1.0 * x - center) / max(TINY, width)) ** 2)
 
 
 @numba.njit(cache=True)
+def lorentzian(
+    x: npt.NDArray[np.float64], center: float, sigma: float, amplitude: float
+) -> npt.NDArray[np.float64]:
+    return (amplitude / (1 + ((1.0 * x - center) / max(TINY, sigma)) ** 2)) / max(
+        TINY, (np.pi * sigma)
+    )
+
+
+@numba.njit(cache=True)
 def fermi_dirac(
     x: npt.NDArray[np.float64], center: float, temp: float
 ) -> npt.NDArray[np.float64]:
     """Fermi-dirac edge in terms of temperature."""
     return 1 / (1 + np.exp((1.0 * x - center) / max(TINY, temp * kb_eV)))
```

### Comparing `erlab-2.2/src/erlab/analysis/fit/minuit.py` & `erlab-2.2.1/src/erlab/analysis/fit/minuit.py`

 * *Files 15% similar despite different names*

```diff
@@ -140,21 +140,31 @@
 
         except NotImplementedError:
             params = model.make_params(**kwargs)
 
         # Convert data to numpy array (must be after guessing parameters)
         data = np.asarray(data)
 
-        fixedparams = []
+        param_names: list[str] = []
+        fixed_params: list[str] = []
         values: dict[str, float] = {}
         limits: dict[str, tuple[float, float]] = {}
 
         for k, par in params.items():
+            if par.expr is not None:
+                if par.vary:
+                    raise ValueError(
+                        "Parameters constrained with expressions are not supported by Minuit."
+                    )
+                else:
+                    continue
+
+            param_names.append(k)
             if not par.vary:
-                fixedparams.append(k)
+                fixed_params.append(k)
 
             val = float(par.value)
             if not np.isfinite(val):
                 val = 0.0
 
             values[k] = val
             limits[k] = (float(par.min), float(par.max))
@@ -167,18 +177,18 @@
 
         else:
 
             def _temp_func(x, *fargs):
                 return model.func(*x, **dict(zip(model._param_root_names, fargs)))
 
         c = LeastSq(x, data, yerr, _temp_func)
-        m = cls(c, name=model.param_names, **values)
+        m = cls(c, name=param_names, **values)
 
-        for n in model.param_names:
-            m.fixed[n] = n in fixedparams
+        for n in param_names:
+            m.fixed[n] = n in fixed_params
             m.limits[n] = limits[n]
 
         if return_cost:
             return c, m
         return m
 
     def _repr_html_(self):
```

### Comparing `erlab-2.2/src/erlab/analysis/fit/models.py` & `erlab-2.2.1/src/erlab/analysis/fit/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -228,24 +228,31 @@
         self,
         npeaks: int = 1,
         peak_shapes: list[str] | str | None = None,
         fd: bool = True,
         convolve: bool = True,
         **kwargs,
     ):
+        kwargs.setdefault("name", f"{npeaks}Peak")
         super().__init__(
             MultiPeakFunction(
                 npeaks, peak_shapes=peak_shapes, fd=fd, convolve=convolve
             ),
             **kwargs,
         )
 
         for i in range(self.func.npeaks):
             self.set_param_hint(f"p{i}_width", min=0.0)
             self.set_param_hint(f"p{i}_height", min=0.0)
+            sigma_expr = self.func.sigma_expr(i, self.prefix)
+            if sigma_expr is not None:
+                self.set_param_hint(f"p{i}_sigma", expr=sigma_expr)
+            amplitude_expr = self.func.amplitude_expr(i, self.prefix)
+            if amplitude_expr is not None:
+                self.set_param_hint(f"p{i}_amplitude", expr=amplitude_expr)
 
         if self.func.fd:
             self.set_param_hint("temp", min=0.0)
 
         if self.func.convolve:
             self.set_param_hint("resolution", min=0.0)
```

### Comparing `erlab-2.2/src/erlab/analysis/fit/spline.py` & `erlab-2.2.1/src/erlab/analysis/fit/spline.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/analysis/gold.py` & `erlab-2.2.1/src/erlab/analysis/gold.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/analysis/image.py` & `erlab-2.2.1/src/erlab/analysis/image.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/analysis/interpolate.py` & `erlab-2.2.1/src/erlab/analysis/interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/analysis/kspace.py` & `erlab-2.2.1/src/erlab/analysis/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/analysis/mask/__init__.py` & `erlab-2.2.1/src/erlab/analysis/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/analysis/mask/polygon.py` & `erlab-2.2.1/src/erlab/analysis/mask/polygon.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/analysis/transform.py` & `erlab-2.2.1/src/erlab/analysis/transform.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/analysis/utilities.py` & `erlab-2.2.1/src/erlab/analysis/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/characterization/resistance.py` & `erlab-2.2.1/src/erlab/characterization/resistance.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/characterization/xrd.py` & `erlab-2.2.1/src/erlab/characterization/xrd.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/constants.py` & `erlab-2.2.1/src/erlab/constants.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/interactive/__init__.py` & `erlab-2.2.1/src/erlab/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/interactive/bzplot.py` & `erlab-2.2.1/src/erlab/interactive/bzplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/interactive/colors.py` & `erlab-2.2.1/src/erlab/interactive/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/interactive/curvefittingtool.py` & `erlab-2.2.1/src/erlab/interactive/curvefittingtool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/interactive/derivative.py` & `erlab-2.2.1/src/erlab/interactive/derivative.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/interactive/dtool.ui` & `erlab-2.2.1/src/erlab/interactive/dtool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/interactive/exampledata.py` & `erlab-2.2.1/src/erlab/interactive/exampledata.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/interactive/fermiedge.py` & `erlab-2.2.1/src/erlab/interactive/fermiedge.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/interactive/imagetool/__init__.py` & `erlab-2.2.1/src/erlab/interactive/imagetool/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py` & `erlab-2.2.1/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py` & `erlab-2.2.1/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/interactive/imagetool/controls.py` & `erlab-2.2.1/src/erlab/interactive/imagetool/controls.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/interactive/imagetool/core.py` & `erlab-2.2.1/src/erlab/interactive/imagetool/core.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/interactive/imagetool/fastbinning.py` & `erlab-2.2.1/src/erlab/interactive/imagetool/fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/interactive/imagetool/slicer.py` & `erlab-2.2.1/src/erlab/interactive/imagetool/slicer.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/interactive/kspace.py` & `erlab-2.2.1/src/erlab/interactive/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/interactive/ktool.ui` & `erlab-2.2.1/src/erlab/interactive/ktool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/interactive/masktool.py` & `erlab-2.2.1/src/erlab/interactive/masktool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/interactive/utilities.py` & `erlab-2.2.1/src/erlab/interactive/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/io/__init__.py` & `erlab-2.2.1/src/erlab/io/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/io/dataloader.py` & `erlab-2.2.1/src/erlab/io/dataloader.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/io/igor.py` & `erlab-2.2.1/src/erlab/io/igor.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/io/plugins/__init__.py` & `erlab-2.2.1/src/erlab/io/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/io/plugins/da30.py` & `erlab-2.2.1/src/erlab/io/plugins/da30.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/io/plugins/kriss.py` & `erlab-2.2.1/src/erlab/io/plugins/kriss.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/io/plugins/merlin.py` & `erlab-2.2.1/src/erlab/io/plugins/merlin.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/io/plugins/ssrl52.py` & `erlab-2.2.1/src/erlab/io/plugins/ssrl52.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/io/utilities.py` & `erlab-2.2.1/src/erlab/io/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/lattice.py` & `erlab-2.2.1/src/erlab/lattice.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/parallel.py` & `erlab-2.2.1/src/erlab/parallel.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/IgorCT/Blue-White.txt` & `erlab-2.2.1/src/erlab/plotting/IgorCT/Blue-White.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/IgorCT/BlueHot.ibw` & `erlab-2.2.1/src/erlab/plotting/IgorCT/BlueHot.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/IgorCT/CTBlueWhite.ibw` & `erlab-2.2.1/src/erlab/plotting/IgorCT/CTBlueWhite.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw` & `erlab-2.2.1/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/IgorCT/CTRedTemperature.ibw` & `erlab-2.2.1/src/erlab/plotting/IgorCT/CTRedTemperature.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/IgorCT/ColdWarm.ibw` & `erlab-2.2.1/src/erlab/plotting/IgorCT/ColdWarm.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/IgorCT/PlanetEarth.ibw` & `erlab-2.2.1/src/erlab/plotting/IgorCT/PlanetEarth.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/IgorCT/ametrine.ibw` & `erlab-2.2.1/src/erlab/plotting/IgorCT/ametrine.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/IgorCT/isolum.ibw` & `erlab-2.2.1/src/erlab/plotting/IgorCT/isolum.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/IgorCT/morgenstemning.ibw` & `erlab-2.2.1/src/erlab/plotting/IgorCT/morgenstemning.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/__init__.py` & `erlab-2.2.1/src/erlab/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/annotations.py` & `erlab-2.2.1/src/erlab/plotting/annotations.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/atoms.py` & `erlab-2.2.1/src/erlab/plotting/atoms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/bz.py` & `erlab-2.2.1/src/erlab/plotting/bz.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/colors.py` & `erlab-2.2.1/src/erlab/plotting/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/erplot.py` & `erlab-2.2.1/src/erlab/plotting/erplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/general.py` & `erlab-2.2.1/src/erlab/plotting/general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/plot3d.py` & `erlab-2.2.1/src/erlab/plotting/plot3d.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/stylelib/fira.mplstyle` & `erlab-2.2.1/src/erlab/plotting/stylelib/fira.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/stylelib/firalight.mplstyle` & `erlab-2.2.1/src/erlab/plotting/stylelib/firalight.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/stylelib/khan.mplstyle` & `erlab-2.2.1/src/erlab/plotting/stylelib/khan.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/stylelib/nature.mplstyle` & `erlab-2.2.1/src/erlab/plotting/stylelib/nature.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/stylelib/poster.mplstyle` & `erlab-2.2.1/src/erlab/plotting/stylelib/poster.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab/plotting/stylelib/times.mplstyle` & `erlab-2.2.1/src/erlab/plotting/stylelib/times.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.2/src/erlab.egg-info/PKG-INFO` & `erlab-2.2.1/src/erlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.2.0
+Version: 2.2.1
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -694,15 +694,15 @@
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: h5netcdf>=1.2.0
 Requires-Dist: igor2>=0.5.6
 Requires-Dist: iminuit>=2.25.2
 Requires-Dist: joblib>=1.3.2
-Requires-Dist: lmfit>=1.2.0
+Requires-Dist: lmfit<1.3.0,>=1.2.0
 Requires-Dist: matplotlib>=3.8.0
 Requires-Dist: numba-progress>=1.0.0
 Requires-Dist: numba>=0.59.0
 Requires-Dist: numbagg>=0.8.1
 Requires-Dist: numpy>=1.26.0
 Requires-Dist: pyperclip>=1.8.2
 Requires-Dist: pyqtgraph>=0.13.1
```

### Comparing `erlab-2.2/src/erlab.egg-info/SOURCES.txt` & `erlab-2.2.1/src/erlab.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -135,11 +135,12 @@
 src/erlab/plotting/stylelib/times.mplstyle
 templates/.macros.j2
 templates/.release_notes.md.j2
 templates/CHANGELOG.md.j2
 tests/analysis/test_fastbinning.py
 tests/analysis/test_fit_functions_dynamic.py
 tests/analysis/test_fit_functions_general.py
+tests/analysis/test_fit_models.py
 tests/analysis/test_image.py
 tests/analysis/test_interpolate.py
 tests/analysis/test_kspace.py
 tests/analysis/test_utilities.py
```

### Comparing `erlab-2.2/src/erlab.egg-info/requires.txt` & `erlab-2.2.1/src/erlab.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 h5netcdf>=1.2.0
 igor2>=0.5.6
 iminuit>=2.25.2
 joblib>=1.3.2
-lmfit>=1.2.0
+lmfit<1.3.0,>=1.2.0
 matplotlib>=3.8.0
 numba-progress>=1.0.0
 numba>=0.59.0
 numbagg>=0.8.1
 numpy>=1.26.0
 pyperclip>=1.8.2
 pyqtgraph>=0.13.1
```

### Comparing `erlab-2.2/templates/.macros.j2` & `erlab-2.2.1/templates/.macros.j2`

 * *Files identical despite different names*

### Comparing `erlab-2.2/tests/analysis/test_fastbinning.py` & `erlab-2.2.1/tests/analysis/test_fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/tests/analysis/test_fit_functions_dynamic.py` & `erlab-2.2.1/tests/analysis/test_fit_functions_dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/tests/analysis/test_fit_functions_general.py` & `erlab-2.2.1/tests/analysis/test_fit_functions_general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/tests/analysis/test_image.py` & `erlab-2.2.1/tests/analysis/test_image.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/tests/analysis/test_interpolate.py` & `erlab-2.2.1/tests/analysis/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/tests/analysis/test_kspace.py` & `erlab-2.2.1/tests/analysis/test_kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.2/tests/analysis/test_utilities.py` & `erlab-2.2.1/tests/analysis/test_utilities.py`

 * *Files identical despite different names*

