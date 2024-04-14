# Comparing `tmp/slcl1butils-2024.2.23.post2.tar.gz` & `tmp/slcl1butils-2024.4.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slcl1butils-2024.2.23.post2.tar", last modified: Fri Feb 23 11:12:47 2024, max compression
+gzip compressed data, was "slcl1butils-2024.4.14.tar", last modified: Sun Apr 14 11:48:36 2024, max compression
```

## Comparing `slcl1butils-2024.2.23.post2.tar` & `slcl1butils-2024.4.14.tar`

### file list

```diff
@@ -1,94 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:47.456390 slcl1butils-2024.2.23.post2/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:47.444390 slcl1butils-2024.2.23.post2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:47.444390 slcl1butils-2024.2.23.post2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-02-23 11:12:47.456390 slcl1butils-2024.2.23.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:47.440390 slcl1butils-2024.2.23.post2/ci/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:47.444390 slcl1butils-2024.2.23.post2/ci/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/ci/requirements/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/ci/requirements/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:47.444390 slcl1butils-2024.2.23.post2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:47.440390 slcl1butils-2024.2.23.post2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:47.448390 slcl1butils-2024.2.23.post2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/docs/_static/css/slcl1butils.css
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/docs/atbd.rst
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/docs/basic_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:47.448390 slcl1butils-2024.2.23.post2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/docs/examples/display_a_IW_L1B_xspectra.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/docs/examples/intro.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (127)    59687 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/docs/oceanspectrumSAR.png
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)    10438 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/get_polygons_from_l1b.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/requirements_doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-23 11:12:47.456390 slcl1butils-2024.2.23.post2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:47.448390 slcl1butils-2024.2.23.post2/slcl1butils/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:47.448390 slcl1butils-2024.2.23.post2/slcl1butils/coloc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/coloc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/coloc/coloc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/coloc/coloc_IW_WW3spectra.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/coloc/coloc_WV_WW3spectra.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:47.452390 slcl1butils-2024.2.23.post2/slcl1butils/compute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/compute/compute_from_l1b.py
--rw-r--r--   0 runner    (1001) docker     (127)     5933 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/compute/stack_iw_l1b.py
--rw-r--r--   0 runner    (1001) docker     (127)    22624 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/compute/stack_wv_l1c_monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/conversion_polar_cartesian.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/get_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11055 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/get_polygons_from_l1b.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:47.452390 slcl1butils-2024.2.23.post2/slcl1butils/legacy_ocean/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/legacy_ocean/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:47.452390 slcl1butils-2024.2.23.post2/slcl1butils/legacy_ocean/ocean/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:47.452390 slcl1butils-2024.2.23.post2/slcl1butils/legacy_ocean/ocean/spectrum_private/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/legacy_ocean/ocean/spectrum_private/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11700 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/legacy_ocean/ocean/spectrum_private/spectra_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    26633 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/legacy_ocean/ocean/xPolarSpectrum.py
--rw-r--r--   0 runner    (1001) docker     (127)    21633 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/legacy_ocean/ocean/xspectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:47.452390 slcl1butils-2024.2.23.post2/slcl1butils/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py
--rw-r--r--   0 runner    (1001) docker     (127)    20821 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/plotting/display_one_spectra.py
--rw-r--r--   0 runner    (1001) docker     (127)    12819 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/plotting/display_xspectra_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/plotting/quadmeshgeoviewsL1B.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/raster_readers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:47.452390 slcl1butils-2024.2.23.post2/slcl1butils/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      925 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs
--rw-r--r--   0 runner    (1001) docker     (127)    13789 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6115 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE_prun.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      590 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs
--rw-r--r--   0 runner    (1001) docker     (127)    13914 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2982 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE_prun.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/spectrum_clockwise_to_trigo.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/spectrum_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/symmetrize_l1b_spectra.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:47.452390 slcl1butils-2024.2.23.post2/slcl1butils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/tests/test_resampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     6886 2024-02-23 11:12:34.000000 slcl1butils-2024.2.23.post2/slcl1butils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 11:12:47.456390 slcl1butils-2024.2.23.post2/slcl1butils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-02-23 11:12:47.000000 slcl1butils-2024.2.23.post2/slcl1butils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-02-23 11:12:47.000000 slcl1butils-2024.2.23.post2/slcl1butils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 11:12:47.000000 slcl1butils-2024.2.23.post2/slcl1butils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-23 11:12:47.000000 slcl1butils-2024.2.23.post2/slcl1butils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-23 11:12:47.000000 slcl1butils-2024.2.23.post2/slcl1butils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-23 11:12:47.000000 slcl1butils-2024.2.23.post2/slcl1butils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:36.486579 slcl1butils-2024.4.14/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:36.478579 slcl1butils-2024.4.14/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:36.478579 slcl1butils-2024.4.14/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-14 11:48:36.486579 slcl1butils-2024.4.14/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:36.474579 slcl1butils-2024.4.14/ci/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:36.478579 slcl1butils-2024.4.14/ci/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/ci/requirements/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/ci/requirements/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:36.478579 slcl1butils-2024.4.14/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:36.474579 slcl1butils-2024.4.14/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:36.478579 slcl1butils-2024.4.14/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/docs/_static/css/slcl1butils.css
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/docs/atbd.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/docs/basic_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:36.478579 slcl1butils-2024.4.14/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/docs/examples/display_a_IW_L1B_xspectra.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/docs/examples/intro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    59687 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/docs/oceanspectrumSAR.png
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    10438 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/get_polygons_from_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/requirements_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 11:48:36.486579 slcl1butils-2024.4.14/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:36.482579 slcl1butils-2024.4.14/slcl1butils/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:36.482579 slcl1butils-2024.4.14/slcl1butils/coloc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/coloc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7168 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/coloc/coloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/coloc/coloc_IW_WW3spectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/coloc/coloc_WV_WW3spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:36.482579 slcl1butils-2024.4.14/slcl1butils/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/compute/compute_from_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/compute/homogeneous_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7387 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/compute/stack_iw_l1b.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22624 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/compute/stack_wv_l1c_monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/conversion_polar_cartesian.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/get_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11055 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/get_polygons_from_l1b.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:36.482579 slcl1butils-2024.4.14/slcl1butils/legacy_ocean/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/legacy_ocean/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:36.482579 slcl1butils-2024.4.14/slcl1butils/legacy_ocean/ocean/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:36.486579 slcl1butils-2024.4.14/slcl1butils/legacy_ocean/ocean/spectrum_private/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/legacy_ocean/ocean/spectrum_private/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11700 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/legacy_ocean/ocean/spectrum_private/spectra_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26633 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/legacy_ocean/ocean/xPolarSpectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21633 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/legacy_ocean/ocean/xspectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:36.486579 slcl1butils-2024.4.14/slcl1butils/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20821 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/plotting/display_one_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12819 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/plotting/display_xspectra_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7277 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/plotting/quadmeshgeoviewsL1B.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/raster_readers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:36.486579 slcl1butils-2024.4.14/slcl1butils/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      925 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs
+-rw-r--r--   0 runner    (1001) docker     (127)    16408 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6115 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE_prun.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      590 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs
+-rw-r--r--   0 runner    (1001) docker     (127)    13914 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2982 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE_prun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/spectrum_clockwise_to_trigo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/spectrum_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/symmetrize_l1b_spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:36.486579 slcl1butils-2024.4.14/slcl1butils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/tests/test_output_filename_l1c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/tests/test_output_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/tests/test_resampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7610 2024-04-14 11:48:22.000000 slcl1butils-2024.4.14/slcl1butils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 11:48:36.486579 slcl1butils-2024.4.14/slcl1butils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-14 11:48:36.000000 slcl1butils-2024.4.14/slcl1butils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-14 11:48:36.000000 slcl1butils-2024.4.14/slcl1butils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 11:48:36.000000 slcl1butils-2024.4.14/slcl1butils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-14 11:48:36.000000 slcl1butils-2024.4.14/slcl1butils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-14 11:48:36.000000 slcl1butils-2024.4.14/slcl1butils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-14 11:48:36.000000 slcl1butils-2024.4.14/slcl1butils.egg-info/top_level.txt
```

### Comparing `slcl1butils-2024.2.23.post2/.github/workflows/publish.yml` & `slcl1butils-2024.4.14/.github/workflows/publish.yml`

 * *Files 9% similar despite different names*

```diff
@@ -47,8 +47,8 @@
       - name: Download build artifacts
         uses: actions/download-artifact@v4
         with:
           name: packages
           path: dist/
 
       - name: Publish to PyPI
-        uses: pypa/gh-action-pypi-publish@2f6f737ca5f74c637829c0f5c3acd0e29ea5e8bf
+        uses: pypa/gh-action-pypi-publish@81e9d935c883d0b210363ab89cf05f3894778450
```

### Comparing `slcl1butils-2024.2.23.post2/.gitignore` & `slcl1butils-2024.4.14/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -123,7 +123,8 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+localconfig.yaml
```

### Comparing `slcl1butils-2024.2.23.post2/.pre-commit-config.yaml` & `slcl1butils-2024.4.14/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/LICENSE` & `slcl1butils-2024.4.14/LICENSE`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/PKG-INFO` & `slcl1butils-2024.4.14/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slcl1butils
-Version: 2024.2.23.post2
+Version: 2024.4.14
 Summary: Python library to exploit SAR IFREMER L1B products
 Author: Alexis Mouche
 License: GPL-3.0
 Keywords: SAR,wave,reseach,cross-spectra
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `slcl1butils-2024.2.23.post2/README.md` & `slcl1butils-2024.4.14/README.md`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/ci/requirements/environment.yaml` & `slcl1butils-2024.4.14/ci/requirements/environment.yaml`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/docs/Makefile` & `slcl1butils-2024.4.14/docs/Makefile`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/docs/basic_api.rst` & `slcl1butils-2024.4.14/docs/basic_api.rst`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/docs/conf.py` & `slcl1butils-2024.4.14/docs/conf.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/docs/examples/display_a_IW_L1B_xspectra.ipynb` & `slcl1butils-2024.4.14/docs/examples/display_a_IW_L1B_xspectra.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb` & `slcl1butils-2024.4.14/docs/examples/do_L1C_SAFE_from_L1B_SAFE_example.ipynb`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9794642857142857%*

 * *Differences: {"'cells'": '{6: {\'source\': {insert: [(8, "    ret = '*

 * *            'do_L1C_SAFE_from_L1B_SAFE(full_safe_file,version=version,outputdir=conf[\'iw_outputdir\'],\\n"), '*

 * *            "(9, '                                    "*

 * *            "ancillary_list=ancillary_datasets,dev=True)\\n')], delete: [8]}}, insert: [(5, "*

 * *            "OrderedDict([('cell_type', 'code'), ('execution_count', None), ('metadata', "*

 * *            'OrderedDict()), (\'outputs\', []), (\'source\', ["ancillary_datasets = '*

 * *            'con […]*

```diff
@@ -59,28 +59,39 @@
             "source": [
                 "conf['iw_outputdir']"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "ancillary_datasets = conf['auxilliary_dataset']\n",
+                "ancillary_datasets.pop('ww3hindcast_spectra',None)"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
             "metadata": {
                 "tags": []
             },
             "outputs": [],
             "source": [
                 "full_safe_files = [one_safe_l1b]\n",
                 "version = '0.1'\n",
                 "for full_safe_file in full_safe_files:\n",
                 "    \n",
                 "    print('')\n",
                 "    print('===')\n",
                 "    print(os.path.basename(full_safe_file))\n",
                 "    print('===')\n",
-                "    ret = do_L1C_SAFE_from_L1B_SAFE(full_safe_file,version=version,outputdir=conf['iw_outputdir'],dev=True)\n",
+                "    ret = do_L1C_SAFE_from_L1B_SAFE(full_safe_file,version=version,outputdir=conf['iw_outputdir'],\n",
+                "                                    ancillary_list=ancillary_datasets,dev=True)\n",
                 "            "
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
@@ -93,13 +104,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.8"
+            "version": "3.11.0"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `slcl1butils-2024.2.23.post2/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb` & `slcl1butils-2024.4.14/docs/examples/plotting_L1B_geometry_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb` & `slcl1butils-2024.4.14/docs/examples/plotting_L1B_variables_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/docs/index.rst` & `slcl1butils-2024.4.14/docs/index.rst`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/docs/installing.rst` & `slcl1butils-2024.4.14/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/docs/oceanspectrumSAR.png` & `slcl1butils-2024.4.14/docs/oceanspectrumSAR.png`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/get_polygons_from_l1b.py` & `slcl1butils-2024.4.14/get_polygons_from_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/pyproject.toml` & `slcl1butils-2024.4.14/pyproject.toml`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/coloc/coloc.py` & `slcl1butils-2024.4.14/slcl1butils/coloc/coloc.py`

 * *Files 4% similar despite different names*

```diff
@@ -147,18 +147,20 @@
             sar_date = datetime.strptime(str.split(l1b_ds.attrs['start_date'], '.')[0], '%Y-%m-%d %H:%M:%S')
             closest_date, filename = resource_strftime(ancillary['resource'], step=ancillary['step'], date=sar_date)
             if (len(glob(filename)) != 1):
                 continue
             # Getting the raster from anxillary data
             if (ancillary['name'] == 'ecmwf_0100_1h'):
                 raster_ds = ecmwf_0100_1h(filename)
-            if (ancillary['name'] == 'ww3_global_yearly_3h'):
+            elif (ancillary['name'] == 'ww3_global_yearly_3h'):
                 raster_ds = ww3_global_yearly_3h(filename, closest_date)
-            if (ancillary['name']) == 'ww3hindcast_field':
+            elif (ancillary['name']) == 'ww3hindcast_field':
                 raster_ds == ww3_IWL1Btrack_hindcasts_30min(filename,closest_date)
+            else:
+                raise ValueError('%s not a correct dataset name'%ancillary['name'])
 
             # Get the polygons of the swath data
             polygons = get_swath_tiles_polygons_from_l1bgroup(l1b_ds, swath_only=True)
             # Crop the raster to the swath bounding box limit
             raster_bb_ds = raster_cropping_in_polygon_bounding_box(polygons['swath'][0], raster_ds)
 
             # Loop on the grid in the product
```

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/coloc/coloc_IW_WW3spectra.py` & `slcl1butils-2024.4.14/slcl1butils/coloc/coloc_IW_WW3spectra.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,16 @@
     start_date_dt = datetime.datetime.strptime(
         dsar.attrs["start_date"], "%Y-%m-%d %H:%M:%S.%f"
     )
     pathww3sp = get_ww3HINDCAST_TRCKspectra_path_from_date(sar_date=start_date_dt)
     gridsar = {
         d: k
         for d, k in dsar.sizes.items()
-        if d in ["burst", "tile_sample", "tile_line"]
+        #if d in ["burst", "tile_sample", "tile_line"]
+        if d in [ "tile_sample", "tile_line"]
     }
     if (xspeckind == "intra" and "xspectra_2tau_Re" in dsar) or (xspeckind == "inter" and "xspectra_Re" in dsar): # in a future version of L1B xspectra variable could be always present (even on land) but filled by NaN
         # symmetrize and combine Re+1j*Im for all the xspectra SAR
         if xspeckind == "intra":
             xsSAR = dsar["xspectra_2tau_Re"] + 1j * dsar["xspectra_2tau_Im"]
         elif xspeckind == "inter":
             xsSAR = dsar["xspectra_Re"] + 1j * dsar["xspectra_Im"]
@@ -108,19 +109,19 @@
                         dsww3raw["efth"].isel(time=indiceww3spectra).rename("ww3EFTHraw")
                     )
                     rawspww3.attrs["description"] = "raw EFTH(f,dir) spectra"
                     ds_ww3_cartesian = ds_ww3_cartesian.swap_dims(
                         {"kx": "k_rg", "ky": "k_az"}
                     ).T
                     rawspww3 = rawspww3.assign_coords(i)
-                    rawspww3 = rawspww3.expand_dims(["burst", "tile_line", "tile_sample"])
+                    rawspww3 = rawspww3.expand_dims(["tile_line", "tile_sample"])
+                    #rawspww3 = rawspww3.expand_dims(["burst", "tile_line", "tile_sample"])
                     ds_ww3_cartesian = ds_ww3_cartesian.assign_coords(i)
-                    ds_ww3_cartesian = ds_ww3_cartesian.expand_dims(
-                        ["burst", "tile_line", "tile_sample"]
-                    )
+                    ds_ww3_cartesian = ds_ww3_cartesian.expand_dims(["tile_line", "tile_sample"])
+                    #ds_ww3_cartesian = ds_ww3_cartesian.expand_dims(["burst", "tile_line", "tile_sample"])
                     list_ww3_cart_sp.append(ds_ww3_cartesian)
                     list_ww3_efth_sp.append(rawspww3)
                 ds_ww3_cartesian_merged = xr.merge(list_ww3_cart_sp)
                 ds_ww3_efth_merged = xr.merge(list_ww3_efth_sp)
                 dsar = xr.merge([dsar, ds_ww3_cartesian_merged, ds_ww3_efth_merged])
                 flag_ww3spectra_added = True
         if xspeckind == "intra":
```

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/coloc/coloc_WV_WW3spectra.py` & `slcl1butils-2024.4.14/slcl1butils/coloc/coloc_WV_WW3spectra.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/compute/compute_from_l1b.py` & `slcl1butils-2024.4.14/slcl1butils/compute/compute_from_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/compute/stack_iw_l1b.py` & `slcl1butils-2024.4.14/slcl1butils/compute/stack_iw_l1b.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,80 +1,119 @@
 import xarray as xr
 import logging
 import numpy as np
 import os
 from tqdm import tqdm
 
+
 def get_a_valid_krg_vector(ds):
-    notfound=True
-    bb=0
-    ts=0
+    """
+    method to get a single k-range vector to be used on each stacked spectra
+
+    Args:
+        ds: xr.Dataset one of the group from L1B IW product
+
+    Returns:
+
+    """
+    notfound = True
+    bb = 0
+    ts = 0
+    tl = 0
     while notfound:
-        k_rg = ds['k_rg'].isel(burst=bb, tile_sample=0)
+        if "burst" in ds["k_rg"].coords:
+            k_rg = ds["k_rg"].isel(burst=bb, tile_sample=ts)
+        else:
+            k_rg = ds["k_rg"].isel(tile_sample=ts, tile_line=tl)
         if np.isfinite(k_rg).all():
-            notfound=False
+            notfound = False
         bb += 1
         ts += 1
+        tl += 1
     return k_rg
 
+
 def get_index_wavenumbers(ds):
-    #print(2 * np.pi / 0.16, 'm')
+    """
+    method to get index for azimuth and range k vectors in order to crop the spectra and get ride of the part that are different from one tile to another
+
+    Args:
+        ds:
+
+    Returns:
+
+    """
+    # print(2 * np.pi / 0.16, 'm')
     k_rg = get_a_valid_krg_vector(ds)
-    indkrg = np.where(abs(k_rg- 0.16) == np.amin(abs(k_rg - 0.16)))[0][0]
+    indkrg = np.where(abs(k_rg - 0.16) == np.amin(abs(k_rg - 0.16)))[0][0]
     # if True:
     #     import matplotlib.pyplot as plt
     #     plt.figure()
     #     plt.plot(k_rg,'.-')
     #     plt.axvline(x=indkrg)
     #     plt.show()
-    #print('indkrg', indkrg)
-    #print(ds['k_rg'].isel(freq_sample=indkrg).values)
+    # print('indkrg', indkrg)
+    # print(ds['k_rg'].isel(freq_sample=indkrg).values)
 
     val_k_az = 0.14
-    indkaz_up = np.where(abs(ds['k_az'] - val_k_az) == np.amin(abs(ds['k_az'] - val_k_az)))[0][0]
-    #print('indkaz_up', indkaz_up)
-    indkaz_bo = np.where(abs(ds['k_az'] + val_k_az) == np.amin(abs(ds['k_az'] + val_k_az)))[0][0]
-    #print('indkaz_bo', indkaz_bo)
-    #print(ds['k_az'].isel(freq_line=indkaz_bo).values)
-    return indkaz_bo,indkaz_up,indkrg
+    indkaz_up = np.where(
+        abs(ds["k_az"] - val_k_az) == np.amin(abs(ds["k_az"] - val_k_az))
+    )[0][0]
+    # print('indkaz_up', indkaz_up)
+    indkaz_bo = np.where(
+        abs(ds["k_az"] + val_k_az) == np.amin(abs(ds["k_az"] + val_k_az))
+    )[0][0]
+    # print('indkaz_bo', indkaz_bo)
+    # print(ds['k_az'].isel(freq_line=indkaz_bo).values)
+    return indkaz_bo, indkaz_up, indkrg
 
 
-def get_reference_wavenumbers(ds,indkaz_bo,indkaz_up,indkrg):
+def get_reference_wavenumbers(ds, indkaz_bo, indkaz_up, indkrg):
     """
 
     Parameters
     ----------
     ds xr.Dataset
     indkaz_bo int
     indkaz_up int
 
     Returns
     -------
 
     """
 
-    #k_rg = ds['k_rg'].isel(burst=0,tile_sample=0)
+    # k_rg = ds['k_rg'].isel(burst=0,tile_sample=0)
     k_rg = get_a_valid_krg_vector(ds)
-    #k_rg_ref = k_rg[k_rg < 0.16]
-    k_rg_ref = k_rg.isel(freq_sample=slice(0,indkrg))
-
-    #k_rg_ref = k_rg_ref.swap_dims({'freq_sample':'k_rg'})
-    k_rg_ref = k_rg_ref.assign_coords({'freq_sample':np.arange(len(k_rg_ref))})
-    k_rg_ref = xr.DataArray(k_rg_ref.values,coords={'freq_sample':np.arange(len(k_rg_ref))},dims=['freq_sample'])
-    logging.info('k_rg_ref %s',k_rg_ref)
-    k_az = ds['k_az']
+    # k_rg_ref = k_rg[k_rg < 0.16]
+    k_rg_ref = k_rg.isel(freq_sample=slice(0, indkrg))
+    logging.debug("k_rg_ref: %s", k_rg_ref)
+    # k_rg_ref = k_rg_ref.swap_dims({'freq_sample':'k_rg'})
+    k_rg_ref = k_rg_ref.assign_coords({"freq_sample": np.arange(len(k_rg_ref))})
+    k_rg_ref = xr.DataArray(
+        k_rg_ref.values,
+        coords={"freq_sample": np.arange(len(k_rg_ref))},
+        dims=["freq_sample"],
+    )
+    logging.debug("k_rg_ref %s", k_rg_ref)
+    k_az = ds["k_az"]
     k_az_ref = k_az.isel(freq_line=slice(indkaz_bo, indkaz_up))
 
-    #k_az_ref = k_az_ref.swap_dims({'freq_line': 'k_az'})
-    k_az_ref = k_az_ref.assign_coords({'freq_line': np.arange(len(k_az_ref))})
-    k_az_ref = xr.DataArray(k_az_ref.values, coords={'freq_line': np.arange(len(k_az_ref))}, dims=['freq_line'])
-    return k_rg_ref,k_az_ref
+    # k_az_ref = k_az_ref.swap_dims({'freq_line': 'k_az'})
+    k_az_ref = k_az_ref.assign_coords({"freq_line": np.arange(len(k_az_ref))})
+    k_az_ref = xr.DataArray(
+        k_az_ref.values,
+        coords={"freq_line": np.arange(len(k_az_ref))},
+        dims=["freq_line"],
+    )
+    return k_rg_ref, k_az_ref
 
 
-def preprrocess(filee,indkrg,indkaz_bo,indkaz_up,k_rg_ref,k_az_ref,typee,tiffnumber):
+def preprrocess(
+    filee, indkrg, indkaz_bo, indkaz_up, k_rg_ref, k_az_ref, typee, tiffnumber
+):
     """
 
     Parameters
     ----------
     filee str full path
     indkrg int
     indkaz_bo int
@@ -84,75 +123,121 @@
     typee str intra or inter
 
     Returns
     -------
     dsu xr.Dataset
 
     """
-    dsu = xr.open_dataset(filee,group=typee+'burst',engine='netcdf4',cache=False)
-    #dsu['subswath'] = xr.DataArray(int(os.path.basename(filee).split('-')[1].replace('iw','')))
-    tmpsubswath = xr.DataArray(int(os.path.basename(filee).split('-')[1].replace('iw','')))
-    dsu = dsu.assign_coords({'subswath':tmpsubswath})
+    dsu = xr.open_dataset(filee, group=typee + "burst", engine="h5netcdf", cache=False)
+    # dsu['subswath'] = xr.DataArray(int(os.path.basename(filee).split('-')[1].replace('iw','')))
+    if os.path.basename(filee).split("-")[0] == "l1b":
+        tmpsubswath = xr.DataArray(
+            int(os.path.basename(filee).split("-")[2].replace("iw", ""))
+        )
+    else:
+        tmpsubswath = xr.DataArray(
+            int(os.path.basename(filee).split("-")[1].replace("iw", ""))
+        )
+    dsu = dsu.assign_coords({"subswath": tmpsubswath})
     dsu = dsu.isel(freq_sample=slice(0, indkrg), freq_line=slice(indkaz_bo, indkaz_up))
-    dsu = dsu.assign_coords({'k_rg': k_rg_ref.values, 'k_az': k_az_ref.values})
-    dsu = dsu.assign_coords({'tiff':tiffnumber})
-    if 'xspectra_0tau_Re' in dsu:
+    dsu = dsu.assign_coords({"k_rg": k_rg_ref.values, "k_az": k_az_ref.values})
+    dsu = dsu.assign_coords({"tiff": tiffnumber})
+    if "xspectra_0tau_Re" in dsu:
         for tautau in range(3):
-            dsu['xspectra_%stau' % tautau] = dsu['xspectra_%stau_Re' % tautau] + 1j * dsu['xspectra_%stau_Im' % tautau]
-            dsu = dsu.drop(['xspectra_%stau_Re' % tautau, 'xspectra_%stau_Im' % tautau])
-    dsu = dsu.drop(['xspectra_0tau','xspectra_1tau','var_xspectra_0tau','var_xspectra_1tau','var_xspectra_2tau'])
-    dsu['xspectra_2tau'] = dsu['xspectra_2tau'].mean(dim=['2tau'])
+            dsu["xspectra_%stau" % tautau] = (
+                dsu["xspectra_%stau_Re" % tautau]
+                + 1j * dsu["xspectra_%stau_Im" % tautau]
+            )
+            dsu = dsu.drop(["xspectra_%stau_Re" % tautau, "xspectra_%stau_Im" % tautau])
+    dsu = dsu.drop(
+        [
+            "xspectra_0tau",
+            "xspectra_1tau",
+            "var_xspectra_0tau",
+            "var_xspectra_1tau",
+            "var_xspectra_2tau",
+        ]
+    )
+    dsu["xspectra_2tau"] = dsu["xspectra_2tau"].mean(dim=["2tau"])
     return dsu
 
-def read_data_L1B(all_l1B, typee='intra',sens='Ascending'):
+
+def read_data_L1B(all_l1B, typee="intra", sens="Ascending"):
     """
 
     Parameters
     ----------
     all_l1B list of str
     typee str intra or inter [optional]
     sens str : Ascending or Descending
 
     Returns
     -------
 
     """
     tmp = []
-    dsfirst = xr.open_dataset(all_l1B[0],group=typee+'burst',engine='netcdf4',cache=False)
-    indkaz_bo,indkaz_up,indkrg = get_index_wavenumbers(dsfirst)
-    k_rg_ref,k_az_ref = get_reference_wavenumbers(dsfirst, indkaz_bo, indkaz_up,indkrg=indkrg)
+    dsfirst = xr.open_dataset(
+        all_l1B[0], group=typee + "burst", engine="h5netcdf", cache=False
+    )
+    indkaz_bo, indkaz_up, indkrg = get_index_wavenumbers(dsfirst)
+    k_rg_ref, k_az_ref = get_reference_wavenumbers(
+        dsfirst, indkaz_bo, indkaz_up, indkrg=indkrg
+    )
     dsfirst.close()
-    print('start loop')
+    logging.info("start loop")
     # xx = partial(preprrocess,indkrg=indkrg,indkaz_bo=indkaz_bo,indkaz_up=indkaz_up,k_rg_ref=k_rg_ref,k_az_ref=k_az_ref,typee=typee)
     consolidated_list = []
     pbar = tqdm(range(len(all_l1B)))
     for ffi in pbar:
-        pbar.set_description('')
-        #for ffi,ff in enumerate(all_l1B):
+        pbar.set_description("")
+        # for ffi,ff in enumerate(all_l1B):
         ff = all_l1B[ffi]
-        tmpds = xr.open_dataset(ff,group=typee+'burst',engine='netcdf4')
-        if 'freq_line' in tmpds.dims and tmpds.orbit_pass==sens and 'xspectra_2tau_Re' in tmpds:
-            tmpds = preprrocess(ff, indkrg, indkaz_bo, indkaz_up, k_rg_ref, k_az_ref, typee, tiffnumber=ffi)
+        tmpds = xr.open_dataset(ff, group=typee + "burst", engine="h5netcdf")
+        if (
+            "freq_line" in tmpds.dims
+            and tmpds.orbit_pass == sens
+            and "xspectra_2tau_Re" in tmpds
+        ):
+            tmpds = preprrocess(
+                ff,
+                indkrg,
+                indkaz_bo,
+                indkaz_up,
+                k_rg_ref,
+                k_az_ref,
+                typee,
+                tiffnumber=ffi,
+            )
             consolidated_list.append(ff)
             tmp.append(tmpds)
         else:
-            logging.debug('%s seems empty or not in right orbit direction',ff)
+            logging.debug("%s seems empty or not in right orbit direction", ff)
 
     # print('nb nc file to read',len(consolidated_list))
-    #ds = xr.concat(tmp,dim='tiff')
+    # ds = xr.concat(tmp,dim='tiff')
     feinte_combine_by_coords = True
     if feinte_combine_by_coords:
         # feinte FN (on remplace des index de coords par des vrais coords) pcq xr.align ne gere pas bien cela
         tmp2 = [
-            x.assign_coords({'tile_sample': range(x.sizes['tile_sample']), 'tile_line': range(x.sizes['tile_line'])}) for x
-            in tmp]  # coords assignement is for alignment below
+            x.assign_coords(
+                {
+                    "tile_sample": range(x.sizes["tile_sample"]),
+                    "tile_line": range(x.sizes["tile_line"]),
+                }
+            )
+            for x in tmp
+        ]  # coords assignement is for alignment below
         dims_not_align = set()
         for x in tmp2:
             dims_not_align = dims_not_align.union(set(x.dims))
-        dims_not_align = dims_not_align - set(['tile_sample', 'tile_line'])
-        tmp3 = xr.align(*tmp2, exclude=dims_not_align,
-                            join='outer')  # tile sample/line are aligned (thanks to their coordinate value) to avoid bug in combine_by_coords below
+        dims_not_align = dims_not_align - set(["tile_sample", "tile_line"])
+        tmp3 = xr.align(
+            *tmp2, exclude=dims_not_align, join="outer"
+        )  # tile sample/line are aligned (thanks to their coordinate value) to avoid bug in combine_by_coords below
         # end feinte Fred
-        ds = xr.combine_by_coords([tt.expand_dims('tiff').expand_dims('subswath') for tt in tmp3],combine_attrs='drop_conflicts')
+        ds = xr.combine_by_coords(
+            [tt.expand_dims("tiff").expand_dims("subswath") for tt in tmp3],
+            combine_attrs="drop_conflicts",
+        )
     else:
-        ds = xr.concat(tmp,dim='dummydim')
-    return ds
+        ds = xr.concat(tmp, dim="dummydim")
+    return ds
```

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/compute/stack_wv_l1c_monthly.py` & `slcl1butils-2024.4.14/slcl1butils/compute/stack_wv_l1c_monthly.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/conversion_polar_cartesian.py` & `slcl1butils-2024.4.14/slcl1butils/conversion_polar_cartesian.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/get_config.py` & `slcl1butils-2024.4.14/slcl1butils/get_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
     Returns:
         conf: dict
     """
     local_config_pontential_path = os.path.join(os.path.dirname(slcl1butils.__file__), 'localconfig.yaml')
 
     if os.path.exists(local_config_pontential_path):
+        logging.debug('local config used')
         config_path = local_config_pontential_path
     else:
+        logging.debug('default config used')
         config_path = os.path.join(os.path.dirname(slcl1butils.__file__), 'config.yaml')
     logging.debug('config path: %s',config_path)
     stream = open(config_path, 'r')
     conf = load(stream, Loader=Loader)
     return conf
```

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/get_polygons_from_l1b.py` & `slcl1butils-2024.4.14/slcl1butils/get_polygons_from_l1b.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/legacy_ocean/ocean/spectrum_private/spectra_functions.py` & `slcl1butils-2024.4.14/slcl1butils/legacy_ocean/ocean/spectrum_private/spectra_functions.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/legacy_ocean/ocean/xPolarSpectrum.py` & `slcl1butils-2024.4.14/slcl1butils/legacy_ocean/ocean/xPolarSpectrum.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/legacy_ocean/ocean/xspectrum.py` & `slcl1butils-2024.4.14/slcl1butils/legacy_ocean/ocean/xspectrum.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py` & `slcl1butils-2024.4.14/slcl1butils/plotting/add_azimuth_cutoff_lines_on_polar_spec_fig.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/plotting/display_one_spectra.py` & `slcl1butils-2024.4.14/slcl1butils/plotting/display_one_spectra.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/plotting/display_xspectra_grid.py` & `slcl1butils-2024.4.14/slcl1butils/plotting/display_xspectra_grid.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb` & `slcl1butils-2024.4.14/slcl1butils/plotting/plotting_L1B_geometry_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb` & `slcl1butils-2024.4.14/slcl1butils/plotting/plotting_L1B_variables_with_holoview_example.ipynb`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/plotting/quadmeshgeoviewsL1B.py` & `slcl1butils-2024.4.14/slcl1butils/plotting/quadmeshgeoviewsL1B.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,17 +43,32 @@
             clipping_colors=clipping,
             tools=["hover"],
             clim=clim,
         )
     else:
         if lst_vars:
             clim = lst_vars[variable][1]
-            fig = qmeshes.opts(width=1200, height=900, colorbar=True, cmap=cmap,clipping_colors=clipping,tools=['hover'],clim=clim) #
+            fig = qmeshes.opts(
+                width=1200,
+                height=900,
+                colorbar=True,
+                cmap=cmap,
+                clipping_colors=clipping,
+                tools=["hover"],
+                clim=clim,
+            )  #
         else:
-            fig = qmeshes.opts(width=1200, height=900, colorbar=True, cmap=cmap,clipping_colors=clipping,tools=['hover']) #
+            fig = qmeshes.opts(
+                width=1200,
+                height=900,
+                colorbar=True,
+                cmap=cmap,
+                clipping_colors=clipping,
+                tools=["hover"],
+            )  #
 
     return fig
 
 
 def open_of_use(ff, bursttype):
     """
 
@@ -81,37 +96,46 @@
         kwargs (dict): optional keyword arguments : k_gp (int) phi_hf (int) lambda_range_max_macs(int) are valid entries
     Returns:
 
     """
     ds = open_of_use(ff, bursttype)
     # ds.load()
     # ds = datatree.open_datatree(ff)[bursttype].to_dataset() # it doesnt change anything to segmentation fault...
+    if "burst" in ds[variable].coords:
+        stackable_coords = ["burst", "tile_line"]
+    else:
+        stackable_coords = ["tile_line"]
     if variable in ["cwave_params"]:
         sub = (
             ds[variable]
             .isel(
                 {"2tau": 0, "k_gp": kwargs.get("k_gp"), "phi_hf": kwargs.get("phi_hf")}
             )
-            .stack({"y": ["burst", "tile_line"]})
+            .stack({"y": stackable_coords})
         )
     elif variable in ["macs_Im", "macs_Re"]:
+
         sub = (
             ds[variable]
             .isel({"lambda_range_max_macs": kwargs.get("lambda_range_max_macs")})
-            .stack({"y": ["burst", "tile_line"]})
+            .stack({"y": stackable_coords})
         )
     else:
-        sub = ds[variable].stack({"y": ["burst", "tile_line"]})
+        if "burst" in ds[variable].coords:
+            sub = ds[variable].stack({"y": ["burst", "tile_line"]})
+        else:
+            sub = ds[variable].stack({"y": ["tile_line"]})
     if np.isnan(sub).any():
         logging.debug(
             "there are %s NaN in the variable stacked : %s",
             np.isnan(sub.data).sum(),
             variable,
         )
     sub = sub.rename({"tile_sample": "x"})
+    sub = sub.drop_vars(['y', 'tile_line'])
     sub = sub.assign_coords({"y": np.arange(sub.y.size)})
     sub = sub.assign_coords({"x": np.arange(sub.x.size)})
     if (sub == 0).any() and variable == "sigma0":
         pdb.set_trace()
     else:
         pass
         # print('debug not zeros found -> continue')
```

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py` & `slcl1butils-2024.4.14/slcl1butils/plotting/spectra_plot_circles_wavenumbers.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/raster_readers.py` & `slcl1butils-2024.4.14/slcl1butils/raster_readers.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs` & `slcl1butils-2024.4.14/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py` & `slcl1butils-2024.4.14/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 import slcl1butils
 from slcl1butils.raster_readers import ecmwf_0100_1h
 from slcl1butils.raster_readers import ww3_global_yearly_3h
 from slcl1butils.raster_readers import resource_strftime
 from slcl1butils.raster_readers import ww3_IWL1Btrack_hindcasts_30min
 from slcl1butils.utils import get_l1c_filepath
+from slcl1butils.compute.homogeneous_output import add_missing_variables
 from datetime import datetime, timedelta
 from glob import glob
 import numpy as np
 import xarray as xr
-import zarr
 from datatree import DataTree
 import time
 import logging
 import sys, os
 from slcl1butils.get_polygons_from_l1b import get_swath_tiles_polygons_from_l1bgroup
 from slcl1butils.coloc.coloc import (
     raster_cropping_in_polygon_bounding_box,
@@ -36,62 +36,65 @@
 conf = get_conf()
 
 
 def do_L1C_SAFE_from_L1B_SAFE(
     full_safe_file,
     version,
     outputdir,
+    ancillary_list,
     colocat=True,
     time_separation="2tau",
     overwrite=False,
     output_format="nc",
     dev=False,
 ):
     """
 
     Args:
         full_safe_file: str (e.g. /path/to/l1b-ifremer-dataset/..SAFE)
         version: str version of the product to generate
         outputdir: str where to store l1c netcdf files
+        ancillary_list: dict of dict with names of the dataset (defined in conf.yaml or localconfig.yaml) to be colocated
         colocat: bool
         time_separation: str (e.g. '2tau')
         overwrite: bool True -> overwrite existing l1c if it exists
         dev: bool True -> early stop after one l1b nc file processing to dev/test
 
     Returns:
 
     """
     l1c_full_path = None
     # Ancillary data to be colocated
-    ancillary_ecmwf = {}
-    ancillary_ecmwf["resource"] = conf["ecmwf0.1_pattern"]
-    ancillary_ecmwf["step"] = 1
-    ancillary_ecmwf["name"] = "ecmwf_0100_1h"
+    # ancillary_ecmwf = {}
+    # ancillary_ecmwf["resource"] = conf["ecmwf0.1_pattern"]
+    # ancillary_ecmwf["step"] = 1
+    # ancillary_ecmwf["name"] = "ecmwf_0100_1h"
 
     # ancillary_ww3 = {}
     # ancillary_ww3["resource"] = conf["ww3_pattern"]
     # ancillary_ww3["step"] = 3
     # ancillary_ww3["name"] = "ww3_global_yearly_3h"
 
-    ancillary_ww3hindcast_field = {}
-    ancillary_ww3hindcast_field["resource"] = conf["ww3hindcast_field_pattern"]
-    ancillary_ww3hindcast_field["step"] = 3
-    ancillary_ww3hindcast_field["name"] = "ww3hindcast_field"
+    # ancillary_ww3hindcast_field = {}
+    # ancillary_ww3hindcast_field["resource"] = conf["ww3hindcast_field_pattern"]
+    # ancillary_ww3hindcast_field["step"] = 3
+    # ancillary_ww3hindcast_field["name"] = "ww3hindcast_field"
 
     # ancillary_list = [ancillary_ecmwf]#,ancillary_ww3]
-    ancillary_list = [ancillary_ecmwf, ancillary_ww3hindcast_field]
+    # ancillary_list = [ancillary_ecmwf, ancillary_ww3hindcast_field]
     logging.info("ancillary data: %s", ancillary_list)
 
     #
     safe_file = os.path.basename(full_safe_file)
     run_directory = os.path.dirname(full_safe_file) + "/"
 
     # Processing Parameters:
 
-    files = glob(os.path.join(run_directory, safe_file, "*_L1B_*nc"))
+    #files = glob(os.path.join(run_directory, safe_file, "*_L1B_*nc"))
+    files = glob(os.path.join(run_directory, safe_file, "l1b*nc"))
     logging.info("Number of files: %s", len(files))
     if len(files) == 0:
         return None
 
     # Loop on L1B netCDF files (per slice)
     if dev:
         logging.info("dev mode -> only one L1B file to treat")
@@ -111,62 +114,82 @@
         else:
             ds_intra, ds_inter, flag_ancillaries_added = enrich_onesubswath_l1b(
                 l1b_fullpath,
                 ancillary_list=ancillary_list,
                 colocat=colocat,
                 time_separation=time_separation,
             )
+            ds_intra, ds_inter = add_missing_variables(ds_intra, ds_inter)
             for anc in flag_ancillaries_added:
                 if flag_ancillaries_added[anc]:
                     cpt[anc + " ancillary_field_added"] += 1
                 else:
                     cpt[anc + " missing"] += 1
-            if (
-                "xspectra_Re" in ds_inter
-                or "xsSAR" in ds_inter
-                or "xspectra" in ds_inter
-            ):
-                ds_intra = netcdf_compliant(ds_intra)
-                ds_inter = netcdf_compliant(ds_inter)
-                if output_format == "nc":
-                    save_l1c_to_netcdf(
+            # if (
+            #     "xspectra_Re" in ds_inter
+            #     or "xsSAR" in ds_inter
+            #     or "xspectra" in ds_inter
+            # ):
+            #     pass # nothing to do
+            # else:
+            #     logging.debug(
+            #         "there is no xspectra in this subswath -> creation of empty xspectra variables"
+            #     )
+            #     cpt["L1B_without_spectra"] += 1
+            #     freq_sample = 453
+            #     freq_line = 50
+            #     # list of variables that would currently miss {'bt_thresh', 'azimuth_cutoff_error', 'nesz_filt',
+            #     'macs_Im', 'bright_targets_histogram', 'lambda_range_max_macs', 'normalized_variance_filt', 'macs_Re',
+            #     'cwave_params', 'tau', 'k_rg', 'azimuth_cutoff', 'sigma0_filt', 'phi_hf', 'doppler_centroid', 'k_az',
+            #     'k_gp'}
+            #     #k_rg(burst, tile_sample, freq_sample)
+            #     #k_az(freq_line)
+            #     empty_xsp = np.nan*np.ones((ds_intra.burst.size,
+            #                                                         ds_intra.tile_line.size,
+            #                                                         ds_intra.tile_sample.size,
+            #                                                         freq_line,freq_sample,1))
+            #     ds_intra['xspectra_2tau_Re'] = xr.DataArray(empty_xsp,dims=['burst', 'tile_line',
+            #                                                         'tile_sample', 'freq_line', 'freq_sample', '2tau'])
+            #     ds_intra['xspectra_2tau_Im'] = ds_intra['xspectra_2tau_Re']
+            #
+            #      # xspectra_2tau_Re(burst, tile_line, tile_sample, freq_line, freq_sample, \2tau)
+            ds_intra = netcdf_compliant(ds_intra)
+            ds_inter = netcdf_compliant(ds_inter)
+            if output_format == "nc":
+                save_l1c_to_netcdf(
                         l1c_full_path, ds_intra, ds_inter, version=version
                     )
-                elif output_format == "zarr":
-                    save_l1c_to_zarr(l1c_full_path, ds_intra, ds_inter, version=version)
-                cpt["saved_in_nc"] += 1
-            else:
-                logging.debug(
-                    "there is no xspectra in this subswath -> the L1C will not be saved"
-                )
-                cpt["L1B_without_spectra"] += 1
+                cpt['saved_in_nc'] += 1
+            elif output_format == "zarr":
+                save_l1c_to_zarr(l1c_full_path, ds_intra, ds_inter, version=version)
+                cpt["saved_in_zarr"] += 1
     logging.info("cpt: %s", cpt)
     return l1c_full_path
 
 
 def enrich_onesubswath_l1b(
     l1b_fullpath, ancillary_list=None, colocat=True, time_separation="2tau"
 ):
     """
 
     Args:
         l1b_fullpath: str one single sub-swath
-        ancillary_list: list
+        ancillary_list: dict
         colocat: cool
         time_separation: str
 
     Returns:
         ds_intra: xarray.Dataset
         ds_inter: xarray.Dataset
         ancillary_fields_added: bool
     """
 
     logging.debug("File in: %s", l1b_fullpath)
     if ancillary_list is None:
-        ancillary_list = []
+        ancillary_list = {}
     # ====================
     # X-SPEC
     # ====================
     #
     # Intraburst at 2tau x-spectra
     burst_type = "intra"
 
@@ -180,33 +203,33 @@
         l1b_fullpath, burst_type=burst_type, time_separation=time_separation
     )
     # ====================
     # COLOC
     # ====================
     flag_ancillaries = {}
     if colocat:
-        for ancillary in ancillary_list:
-            logging.debug("ancillary: %s", ancillary)
+        for ancillary_name in ancillary_list:
+            logging.debug("ancillary: %s", ancillary_name)
             ds_intra, ds_inter, ancillary_fields_added = append_ancillary_field(
-                ancillary, ds_intra, ds_inter
+                ancillary_list[ancillary_name], ds_intra, ds_inter
             )
-            flag_ancillaries[ancillary["name"]] = ancillary_fields_added
-
-    (
-        ds_intra,
-        flag_ww3spectra_added,
-        flag_ww3spectra_found,
-    ) = resampleWW3spectra_on_TOPS_SAR_cartesian_grid(dsar=ds_intra, xspeckind="intra")
-    flag_ancillaries["ww3spectra_intra"] = flag_ww3spectra_added
-    (
-        ds_inter,
-        flag_ww3spectra_added,
-        flag_ww3spectra_found,
-    ) = resampleWW3spectra_on_TOPS_SAR_cartesian_grid(dsar=ds_inter, xspeckind="inter")
-    flag_ancillaries["ww3spectra_inter"] = flag_ww3spectra_added
+            flag_ancillaries[ancillary_name] = ancillary_fields_added
+    if 'ww3hindcast_spectra' in ancillary_list:
+        (
+            ds_intra,
+            flag_ww3spectra_added,
+            flag_ww3spectra_found,
+        ) = resampleWW3spectra_on_TOPS_SAR_cartesian_grid(dsar=ds_intra, xspeckind="intra")
+        flag_ancillaries["ww3spectra_intra"] = flag_ww3spectra_added
+        (
+            ds_inter,
+            flag_ww3spectra_added,
+            flag_ww3spectra_found,
+        ) = resampleWW3spectra_on_TOPS_SAR_cartesian_grid(dsar=ds_inter, xspeckind="inter")
+        flag_ancillaries["ww3spectra_inter"] = flag_ww3spectra_added
     return ds_intra, ds_inter, flag_ancillaries
 
 
 def append_ancillary_field(ancillary, ds_intra, ds_inter):
     """
 
     Args:
@@ -226,28 +249,31 @@
     # ===========================================
     ## Check if the ancillary data can be found
     ancillary_fields_added = False
     sar_date = datetime.strptime(
         str.split(ds_intra.attrs["start_date"], ".")[0], "%Y-%m-%d %H:%M:%S"
     )
     closest_date, filename = resource_strftime(
-        ancillary["resource"], step=ancillary["step"], date=sar_date
+        ancillary["pattern"], step=int(ancillary["step"]), date=sar_date
     )
     if len(glob(filename)) != 1:
         logging.debug("no ancillary files matching %s", filename)
         return ds_intra, ds_inter, ancillary_fields_added
     else:
         ancillary_fields_added = True
     # Getting the raster from anxillary data
     if ancillary["name"] == "ecmwf_0100_1h":
         raster_ds = ecmwf_0100_1h(filename)
     elif ancillary["name"] == "ww3_global_yearly_3h":
         raster_ds = ww3_global_yearly_3h(filename, closest_date)
     elif ancillary["name"] == "ww3hindcast_field":
         raster_ds = ww3_IWL1Btrack_hindcasts_30min(glob(filename)[0], closest_date)
+    elif ancillary["name"] == "ww3hindcast_spectra":
+        pass #nothing to do here, there is a specific method called later in the code.
+        return ds_intra, ds_inter, ancillary_fields_added
     else:
         raise ValueError("%s ancillary name not handled" % ancillary["name"])
     # Get the polygons of the swath data
     polygons, coordinates, variables = get_swath_tiles_polygons_from_l1bgroup(
         ds_intra, swath_only=True
     )
     # Crop the raster to the swath bounding box limit
@@ -362,14 +388,20 @@
     parser.add_argument(
         "--version",
         help="set the output product version (e.g. 0.3) default version will be read from config.yaml",
         required=False,
         default=conf["l1c_iw_version"],
     )
     parser.add_argument(
+        "--ww3spectra",
+        action="store_true",
+        default=False,
+        help="add WW3 spectra to L1C [default is False]",
+    )
+    parser.add_argument(
         "--dev",
         action="store_true",
         default=False,
         help="dev mode stops the computation early",
     )
     args = parser.parse_args()
     fmt = "%(asctime)s %(levelname)s %(filename)s(%(lineno)d) %(message)s"
@@ -380,25 +412,31 @@
     else:
         logging.basicConfig(
             level=logging.INFO, format=fmt, datefmt="%d/%m/%Y %H:%M:%S", force=True
         )
     t0 = time.time()
     logging.info("product version to produce: %s", args.version)
     logging.info("outputdir will be: %s", args.outputdir)
+    ancillary_list = {'ecmwf_0100_1h':conf['auxilliary_dataset']['ecmwf_0100_1h'],
+                      'ww3hindcast_field':conf['auxilliary_dataset']['ww3hindcast_field']
+                      }
+    if args.ww3spectra:
+        ancillary_list['ww3hindcast_spectra'] = conf['auxilliary_dataset']['ww3hindcast_spectra']
     final_L1C_path = do_L1C_SAFE_from_L1B_SAFE(
         args.l1bsafe,
         version=args.version,
         outputdir=args.outputdir,
+        ancillary_list=ancillary_list,
         colocat=True,
         time_separation="2tau",
         overwrite=args.overwrite,
         dev=args.dev,
         output_format="nc",
     )
-    logging.info("last tiff available for this SAFE: %s", final_L1C_path)
+    logging.info("last measurement generated for this SAFE: %s", final_L1C_path)
     logging.info("successful SAFE processing")
     logging.info("peak memory usage: %s ", get_memory_usage())
     logging.info("done in %1.3f min", (time.time() - t0) / 60.0)
 
 
 if __name__ == "__main__":
     root = logging.getLogger()
```

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE_prun.py` & `slcl1butils-2024.4.14/slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE_prun.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs` & `slcl1butils-2024.4.14/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py` & `slcl1butils-2024.4.14/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE_prun.py` & `slcl1butils-2024.4.14/slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE_prun.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/spectrum_clockwise_to_trigo.py` & `slcl1butils-2024.4.14/slcl1butils/spectrum_clockwise_to_trigo.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/spectrum_rotation.py` & `slcl1butils-2024.4.14/slcl1butils/spectrum_rotation.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/symmetrize_l1b_spectra.py` & `slcl1butils-2024.4.14/slcl1butils/symmetrize_l1b_spectra.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/tests/test_resampling.py` & `slcl1butils-2024.4.14/slcl1butils/tests/test_resampling.py`

 * *Files identical despite different names*

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils/utils.py` & `slcl1butils-2024.4.14/slcl1butils/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -200,16 +200,31 @@
     ):  # classical ESA SLC naming #:TODO once xsarslc will be updated this case could be removed
         basesafe = basesafe.replace(".SAFE", "_" + version.upper() + ".SAFE")
     else:  # there is already a product ID in the L1B SAFE name
         lastpart = basesafe.split("_")[-1]
         basesafe = basesafe.replace(lastpart, version.upper() + ".SAFE")
     l1c_full_path = l1c_full_path.replace(basesafe0, basesafe)
 
-    lastpiece = l1c_full_path.split("_")[-1]
+    #suffix measurement
+    measu_base = os.path.basename(l1c_full_path)
+    if 's1' in measu_base[0:2]:
+        measu_base = 'l1c-'+measu_base
+    elif 'l1b' in measu_base[0:3]:
+        measu_base = measu_base.replace('l1b','l1c')
+    measu_base = measu_base.replace('slc','xsp') #security old products
+    measu_base = measu_base.replace('L1C_xspec_IFR_','') # security
+    l1c_full_path = l1c_full_path.replace(os.path.basename(l1c_full_path),measu_base)
+
+    # lastpiece = l1c_full_path.split("_")[-1]
+    if '_' in os.path.basename(l1c_full_path):
+        lastpiece = '_'+l1c_full_path.split("_")[-1]
+    elif '-' in os.path.basename(l1c_full_path):
+        # lastpiece = l1c_full_path[-6:]
+        lastpiece = '-'+l1c_full_path.split("-")[-1]
     if format == "nc":
-        l1c_full_path = l1c_full_path.replace(lastpiece, version + ".nc")
+        l1c_full_path = l1c_full_path.replace(lastpiece, '-'+version.lower() + ".nc")
     elif format == "zarr":
-        l1c_full_path = l1c_full_path.replace(lastpiece, version + ".zarr")
+        l1c_full_path = l1c_full_path.replace(lastpiece, version.lower() + ".zarr")
     logging.debug("File out: %s ", l1c_full_path)
     if not os.path.exists(os.path.dirname(l1c_full_path)) and makedir:
         os.makedirs(os.path.dirname(l1c_full_path), 0o0775)
     return l1c_full_path
```

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils.egg-info/PKG-INFO` & `slcl1butils-2024.4.14/slcl1butils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slcl1butils
-Version: 2024.2.23.post2
+Version: 2024.4.14
 Summary: Python library to exploit SAR IFREMER L1B products
 Author: Alexis Mouche
 License: GPL-3.0
 Keywords: SAR,wave,reseach,cross-spectra
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `slcl1butils-2024.2.23.post2/slcl1butils.egg-info/SOURCES.txt` & `slcl1butils-2024.4.14/slcl1butils.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 slcl1butils.egg-info/top_level.txt
 slcl1butils/coloc/__init__.py
 slcl1butils/coloc/coloc.py
 slcl1butils/coloc/coloc_IW_WW3spectra.py
 slcl1butils/coloc/coloc_WV_WW3spectra.py
 slcl1butils/compute/__init__.py
 slcl1butils/compute/compute_from_l1b.py
+slcl1butils/compute/homogeneous_output.py
 slcl1butils/compute/stack_iw_l1b.py
 slcl1butils/compute/stack_wv_l1c_monthly.py
 slcl1butils/legacy_ocean/__init__.py
 slcl1butils/legacy_ocean/ocean/xPolarSpectrum.py
 slcl1butils/legacy_ocean/ocean/xspectrum.py
 slcl1butils/legacy_ocean/ocean/spectrum_private/__init__.py
 slcl1butils/legacy_ocean/ocean/spectrum_private/spectra_functions.py
@@ -66,8 +67,10 @@
 slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.pbs
 slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE.py
 slcl1butils/scripts/do_IW_L1C_SAFE_from_L1B_SAFE_prun.py
 slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.pbs
 slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE.py
 slcl1butils/scripts/do_WV_L1C_SAFE_from_L1B_SAFE_prun.py
 slcl1butils/tests/__init__.py
+slcl1butils/tests/test_output_filename_l1c.py
+slcl1butils/tests/test_output_path.py
 slcl1butils/tests/test_resampling.py
```

