# Comparing `tmp/image_registration-0.2.8.tar.gz` & `tmp/image_registration-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image_registration-0.2.8.tar", last modified: Tue Nov 14 18:45:33 2023, max compression
+gzip compressed data, was "image_registration-0.2.9.tar", last modified: Sun Apr 14 15:18:53 2024, max compression
```

## Comparing `image_registration-0.2.8.tar` & `image_registration-0.2.9.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:45:33.362923 image_registration-0.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:45:33.342923 image_registration-0.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:45:33.346924 image_registration-0.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2023-11-14 18:45:22.000000 image_registration-0.2.8/.github/workflows/ci_cron_weekly.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2023-11-14 18:45:22.000000 image_registration-0.2.8/.github/workflows/ci_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2023-11-14 18:45:22.000000 image_registration-0.2.8/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-11-14 18:45:22.000000 image_registration-0.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      305 2023-11-14 18:45:22.000000 image_registration-0.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3727 2023-11-14 18:45:22.000000 image_registration-0.2.8/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      455 2023-11-14 18:45:22.000000 image_registration-0.2.8/CHANGES
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2023-11-14 18:45:22.000000 image_registration-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      155 2023-11-14 18:45:22.000000 image_registration-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2023-11-14 18:45:33.362923 image_registration-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2023-11-14 18:45:22.000000 image_registration-0.2.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-11-14 18:45:22.000000 image_registration-0.2.8/REQUIREMENTS
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:45:33.354924 image_registration-0.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)   446999 2023-11-14 18:45:22.000000 image_registration-0.2.8/docs/CrossCorrelationSimulation.pdf
--rw-r--r--   0 runner    (1001) docker     (127)  2093536 2023-11-14 18:45:22.000000 image_registration-0.2.8/docs/Fourier Scaling = Zooming = Similarity.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   665023 2023-11-14 18:45:22.000000 image_registration-0.2.8/docs/Image Registration Debugging.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2023-11-14 18:45:22.000000 image_registration-0.2.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       77 2023-11-14 18:45:22.000000 image_registration-0.2.8/docs/REQUIREMENTS
--rw-r--r--   0 runner    (1001) docker     (127)    63148 2023-11-14 18:45:22.000000 image_registration-0.2.8/docs/SpectralXCorr.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:45:33.342923 image_registration-0.2.8/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:45:33.354924 image_registration-0.2.8/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2023-11-14 18:45:22.000000 image_registration-0.2.8/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      251 2023-11-14 18:45:22.000000 image_registration-0.2.8/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-11-14 18:45:22.000000 image_registration-0.2.8/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6679 2023-11-14 18:45:22.000000 image_registration-0.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2023-11-14 18:45:22.000000 image_registration-0.2.8/docs/fourier_tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)    45043 2023-11-14 18:45:22.000000 image_registration-0.2.8/docs/image.png
--rw-r--r--   0 runner    (1001) docker     (127)      472 2023-11-14 18:45:22.000000 image_registration-0.2.8/docs/image_registration.FITS_tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2023-11-14 18:45:22.000000 image_registration-0.2.8/docs/image_registration.fft_tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)      767 2023-11-14 18:45:22.000000 image_registration-0.2.8/docs/image_registration.rst
--rw-r--r--   0 runner    (1001) docker     (127)    52277 2023-11-14 18:45:22.000000 image_registration-0.2.8/docs/image_shifted_corrupted.png
--rw-r--r--   0 runner    (1001) docker     (127)     6515 2023-11-14 18:45:22.000000 image_registration-0.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      392 2023-11-14 18:45:22.000000 image_registration-0.2.8/docs/spectral_xcorr.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:45:33.354924 image_registration-0.2.8/docs/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (127)     5864 2023-11-14 18:45:22.000000 image_registration-0.2.8/docs/sphinxext/edit_on_github.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2023-11-14 18:45:22.000000 image_registration-0.2.8/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:45:33.354924 image_registration-0.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)   158024 2023-11-14 18:45:22.000000 image_registration-0.2.8/examples/Cross Correlation.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6057 2023-11-14 18:45:22.000000 image_registration-0.2.8/examples/benchmarks_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2023-11-14 18:45:22.000000 image_registration-0.2.8/examples/benchmarks_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2023-11-14 18:45:22.000000 image_registration-0.2.8/examples/demo_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)    12155 2023-11-14 18:45:22.000000 image_registration-0.2.8/ez_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:45:33.354924 image_registration-0.2.8/image_registration/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:45:33.358924 image_registration-0.2.8/image_registration/FITS_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/FITS_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/FITS_tools/fits_overlap.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/FITS_tools/hcongrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/FITS_tools/load_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     6703 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/FITS_tools/match_images.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/_astropy_init.py
--rw-r--r--   0 runner    (1001) docker     (127)    25022 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/chi2_shifts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10225 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/cross_correlation_shifts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:45:33.358924 image_registration-0.2.8/image_registration/fft_tools/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/fft_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13881 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/fft_tools/convolve_nd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/fft_tools/correlate2d.py
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/fft_tools/downsample.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/fft_tools/fast_ffts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6303 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/fft_tools/scale.py
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/fft_tools/shift.py
--rw-r--r--   0 runner    (1001) docker     (127)     8034 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/fft_tools/smooth_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:45:33.362923 image_registration-0.2.8/image_registration/fft_tools/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/fft_tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/fft_tools/tests/measure_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/fft_tools/tests/test_downsample.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/fft_tools/tests/test_shift.py
--rw-r--r--   0 runner    (1001) docker     (127)    13842 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/fft_tools/tests/test_upsample.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/fft_tools/tests/test_upsample_1d.py
--rw-r--r--   0 runner    (1001) docker     (127)     5352 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/fft_tools/tests/test_zoomnd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8559 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/fft_tools/upsample.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/fft_tools/zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     8555 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/iterative_zoom.py
--rw-r--r--   0 runner    (1001) docker     (127)    14087 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/register_images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:45:33.362923 image_registration-0.2.8/image_registration/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/tests/coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)     6748 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/tests/debug_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8564 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/tests/measure_expected_offsets.py
--rw-r--r--   0 runner    (1001) docker     (127)    24331 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/tests/registration_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/tests/setup_package.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2023-11-14 18:45:22.000000 image_registration-0.2.8/image_registration/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2023-11-14 18:45:33.000000 image_registration-0.2.8/image_registration/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 18:45:33.358924 image_registration-0.2.8/image_registration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2023-11-14 18:45:33.000000 image_registration-0.2.8/image_registration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2023-11-14 18:45:33.000000 image_registration-0.2.8/image_registration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 18:45:33.000000 image_registration-0.2.8/image_registration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-11-14 18:45:33.000000 image_registration-0.2.8/image_registration.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 18:45:33.000000 image_registration-0.2.8/image_registration.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-11-14 18:45:33.000000 image_registration-0.2.8/image_registration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-11-14 18:45:33.000000 image_registration-0.2.8/image_registration.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      219 2023-11-14 18:45:22.000000 image_registration-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2023-11-14 18:45:33.362923 image_registration-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2023-11-14 18:45:22.000000 image_registration-0.2.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2023-11-14 18:45:22.000000 image_registration-0.2.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:18:53.682082 image_registration-0.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:18:53.658082 image_registration-0.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:18:53.666082 image_registration-0.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-14 15:18:47.000000 image_registration-0.2.9/.github/workflows/ci_cron_weekly.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-14 15:18:47.000000 image_registration-0.2.9/.github/workflows/ci_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-14 15:18:47.000000 image_registration-0.2.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-14 15:18:47.000000 image_registration-0.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-14 15:18:47.000000 image_registration-0.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-14 15:18:47.000000 image_registration-0.2.9/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-14 15:18:47.000000 image_registration-0.2.9/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-14 15:18:47.000000 image_registration-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-14 15:18:47.000000 image_registration-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-14 15:18:53.682082 image_registration-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-14 15:18:47.000000 image_registration-0.2.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-14 15:18:47.000000 image_registration-0.2.9/REQUIREMENTS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:18:53.670082 image_registration-0.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)   446999 2024-04-14 15:18:47.000000 image_registration-0.2.9/docs/CrossCorrelationSimulation.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)  2093536 2024-04-14 15:18:47.000000 image_registration-0.2.9/docs/Fourier Scaling = Zooming = Similarity.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   665023 2024-04-14 15:18:47.000000 image_registration-0.2.9/docs/Image Registration Debugging.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-04-14 15:18:47.000000 image_registration-0.2.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-14 15:18:47.000000 image_registration-0.2.9/docs/REQUIREMENTS
+-rw-r--r--   0 runner    (1001) docker     (127)    63148 2024-04-14 15:18:47.000000 image_registration-0.2.9/docs/SpectralXCorr.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:18:53.658082 image_registration-0.2.9/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:18:53.670082 image_registration-0.2.9/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-14 15:18:47.000000 image_registration-0.2.9/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-14 15:18:47.000000 image_registration-0.2.9/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-14 15:18:47.000000 image_registration-0.2.9/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6679 2024-04-14 15:18:47.000000 image_registration-0.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-14 15:18:47.000000 image_registration-0.2.9/docs/fourier_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    45043 2024-04-14 15:18:47.000000 image_registration-0.2.9/docs/image.png
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-14 15:18:47.000000 image_registration-0.2.9/docs/image_registration.FITS_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-14 15:18:47.000000 image_registration-0.2.9/docs/image_registration.fft_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-04-14 15:18:47.000000 image_registration-0.2.9/docs/image_registration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    52277 2024-04-14 15:18:47.000000 image_registration-0.2.9/docs/image_shifted_corrupted.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6499 2024-04-14 15:18:47.000000 image_registration-0.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-14 15:18:47.000000 image_registration-0.2.9/docs/spectral_xcorr.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:18:53.670082 image_registration-0.2.9/docs/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (127)     5864 2024-04-14 15:18:47.000000 image_registration-0.2.9/docs/sphinxext/edit_on_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-14 15:18:47.000000 image_registration-0.2.9/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:18:53.674082 image_registration-0.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)   209960 2024-04-14 15:18:47.000000 image_registration-0.2.9/examples/Cross Correlation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6057 2024-04-14 15:18:47.000000 image_registration-0.2.9/examples/benchmarks_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-04-14 15:18:47.000000 image_registration-0.2.9/examples/benchmarks_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-14 15:18:47.000000 image_registration-0.2.9/examples/demo_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12155 2024-04-14 15:18:47.000000 image_registration-0.2.9/ez_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:18:53.674082 image_registration-0.2.9/image_registration/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:18:53.678082 image_registration-0.2.9/image_registration/FITS_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/FITS_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/FITS_tools/fits_overlap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/FITS_tools/hcongrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/FITS_tools/load_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6703 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/FITS_tools/match_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/_astropy_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25022 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/chi2_shifts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10225 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/cross_correlation_shifts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:18:53.678082 image_registration-0.2.9/image_registration/fft_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/fft_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13881 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/fft_tools/convolve_nd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/fft_tools/correlate2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/fft_tools/downsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/fft_tools/fast_ffts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6303 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/fft_tools/scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/fft_tools/shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8034 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/fft_tools/smooth_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:18:53.678082 image_registration-0.2.9/image_registration/fft_tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/fft_tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/fft_tools/tests/measure_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/fft_tools/tests/test_downsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/fft_tools/tests/test_shift.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13842 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/fft_tools/tests/test_upsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/fft_tools/tests/test_upsample_1d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5352 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/fft_tools/tests/test_zoomnd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/fft_tools/upsample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/fft_tools/zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/iterative_zoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14087 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/register_images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:18:53.682082 image_registration-0.2.9/image_registration/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/tests/coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)     6748 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/tests/debug_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8564 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/tests/measure_expected_offsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24331 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/tests/registration_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/tests/setup_package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-14 15:18:47.000000 image_registration-0.2.9/image_registration/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-14 15:18:53.000000 image_registration-0.2.9/image_registration/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 15:18:53.682082 image_registration-0.2.9/image_registration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-14 15:18:53.000000 image_registration-0.2.9/image_registration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-04-14 15:18:53.000000 image_registration-0.2.9/image_registration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 15:18:53.000000 image_registration-0.2.9/image_registration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-14 15:18:53.000000 image_registration-0.2.9/image_registration.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 15:18:53.000000 image_registration-0.2.9/image_registration.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-14 15:18:53.000000 image_registration-0.2.9/image_registration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-14 15:18:53.000000 image_registration-0.2.9/image_registration.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-14 15:18:47.000000 image_registration-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-14 15:18:53.682082 image_registration-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-14 15:18:47.000000 image_registration-0.2.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-14 15:18:47.000000 image_registration-0.2.9/tox.ini
```

### Comparing `image_registration-0.2.8/.github/workflows/ci_cron_weekly.yml` & `image_registration-0.2.9/.github/workflows/ci_cron_weekly.yml`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/.github/workflows/ci_tests.yml` & `image_registration-0.2.9/.github/workflows/ci_tests.yml`

 * *Files 5% similar despite different names*

```diff
@@ -26,40 +26,45 @@
             os: ubuntu-latest
             python: 3.x
             toxenv: codestyle
 
           - name: Python 3.10 with minimal dependencies
             os: ubuntu-latest
             python: 3.10
-            toxenv: py37-test
+            toxenv: py310-test
+
+          - name: Python 3.12 with minimal dependencies
+            os: ubuntu-latest
+            python: 3.12
+            toxenv: py312-test
 
           - name: Python 3.11 with all optional dependencies and coverage checking
             os: ubuntu-latest
             python: 3.11
-            toxenv: py38-test-alldeps-cov
+            toxenv: py311-test-alldeps-cov
 
           - name: macOS - Python 3.11 with all optional dependencies
             os: macos-latest
             python: 3.11
-            toxenv: py38-test-alldeps
+            toxenv: py311-test-alldeps
 
           - name: Windows - Python 3.11 with all optional dependencies
             os: windows-latest
             python: 3.11
-            toxenv: py38-test-alldeps
+            toxenv: py311-test-alldeps
 
           # - name: Python 3.10 with oldest supported version of all dependencies
           #   os: ubuntu-16.04
           #   python: 3.10
           #   toxenv: py37-test-oldestdeps
 
           # - name: Python 3.11 with latest dev versions of key dependencies
           #   os: ubuntu-latest
           #   python: 3.11
-          #   toxenv: py38-test-devdeps
+          #   toxenv: py311-test-devdeps
 
           # - name: Test building of Sphinx docs
           #   os: ubuntu-latest
           #   python: 3.x
           #   toxenv: build_docs
 
     steps:
```

### Comparing `image_registration-0.2.8/.github/workflows/publish.yml` & `image_registration-0.2.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/.gitignore` & `image_registration-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/.travis.yml` & `image_registration-0.2.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/LICENSE` & `image_registration-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/PKG-INFO` & `image_registration-0.2.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: image_registration
-Version: 0.2.8
+Version: 0.2.9
 Summary: Package for registering images with extended emission
 Home-page: https://image-registration.readthedocs.io/en/latest/
 Author: Adam Ginsburg
 Author-email: adam.g.ginsburg@gmail.com
 License: BSD
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: astropy
+Requires-Dist: matplotlib
+Requires-Dist: pytest
 Provides-Extra: test
 Requires-Dist: pytest-astropy; extra == "test"
 Requires-Dist: matplotlib; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx-astropy; extra == "docs"
 Requires-Dist: matplotlib; extra == "docs"
 Requires-Dist: FITS_tools; extra == "docs"
```

### Comparing `image_registration-0.2.8/README.md` & `image_registration-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/docs/CrossCorrelationSimulation.pdf` & `image_registration-0.2.9/docs/CrossCorrelationSimulation.pdf`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/docs/Fourier Scaling = Zooming = Similarity.ipynb` & `image_registration-0.2.9/docs/Fourier Scaling = Zooming = Similarity.ipynb`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/docs/Image Registration Debugging.ipynb` & `image_registration-0.2.9/docs/Image Registration Debugging.ipynb`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/docs/Makefile` & `image_registration-0.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/docs/SpectralXCorr.ipynb` & `image_registration-0.2.9/docs/SpectralXCorr.ipynb`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/docs/conf.py` & `image_registration-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/docs/fourier_tools.rst` & `image_registration-0.2.9/docs/fourier_tools.rst`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/docs/image.png` & `image_registration-0.2.9/docs/image.png`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/docs/image_registration.fft_tools.rst` & `image_registration-0.2.9/docs/image_registration.fft_tools.rst`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/docs/image_registration.rst` & `image_registration-0.2.9/docs/image_registration.rst`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/docs/image_shifted_corrupted.png` & `image_registration-0.2.9/docs/image_shifted_corrupted.png`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/docs/index.rst` & `image_registration-0.2.9/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -53,17 +53,17 @@
    :doc:`image_registration.fft_tools` (and a description of the :doc:`fourier_tools`)
 
 
    The most successful of the methods implemented here is
    :obj:`~image_registration.chi2_shifts.chi2_shift`
 
    There is an ipython notebook demonstration of the code `here
-   <http://nbviewer.ipython.org/urls/raw.github.com/keflavich/image_registration/master/examples/Cross%2520Correlation.ipynb>`__
+   <https://nbviewer.org/github/keflavich/image_registration/blob/master/examples/Cross%20Correlation.ipynb>`__
    and in pdf `here
-   <https://github.com/keflavich/image_registration/blob/master/doc/CrossCorrelationSimulation.pdf?raw=true>`__
+   <https://github.com/keflavich/image_registration/blob/master/docs/CrossCorrelationSimulation.pdf?raw=true>`__
 
 Related Methods
 ---------------
 There are many other approaches to performing image registration.  Some are
 summarized here.  Note that this package is intended for image registration
 where the brightness is "extended" or "spread out" - stellar images are best to
 register by treating the stars as control points.
```

### Comparing `image_registration-0.2.8/docs/sphinxext/edit_on_github.py` & `image_registration-0.2.9/docs/sphinxext/edit_on_github.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/examples/benchmarks_shift.py` & `image_registration-0.2.9/examples/benchmarks_shift.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/examples/benchmarks_zoom.py` & `image_registration-0.2.9/examples/benchmarks_zoom.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/examples/demo_gaussian.py` & `image_registration-0.2.9/examples/demo_gaussian.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/ez_setup.py` & `image_registration-0.2.9/ez_setup.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/FITS_tools/fits_overlap.py` & `image_registration-0.2.9/image_registration/FITS_tools/fits_overlap.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/FITS_tools/load_header.py` & `image_registration-0.2.9/image_registration/FITS_tools/load_header.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/FITS_tools/match_images.py` & `image_registration-0.2.9/image_registration/FITS_tools/match_images.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/__init__.py` & `image_registration-0.2.9/image_registration/__init__.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/chi2_shifts.py` & `image_registration-0.2.9/image_registration/chi2_shifts.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/conftest.py` & `image_registration-0.2.9/image_registration/conftest.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/cross_correlation_shifts.py` & `image_registration-0.2.9/image_registration/cross_correlation_shifts.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/fft_tools/convolve_nd.py` & `image_registration-0.2.9/image_registration/fft_tools/convolve_nd.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/fft_tools/correlate2d.py` & `image_registration-0.2.9/image_registration/fft_tools/correlate2d.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/fft_tools/downsample.py` & `image_registration-0.2.9/image_registration/fft_tools/downsample.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/fft_tools/fast_ffts.py` & `image_registration-0.2.9/image_registration/fft_tools/fast_ffts.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/fft_tools/scale.py` & `image_registration-0.2.9/image_registration/fft_tools/scale.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/fft_tools/shift.py` & `image_registration-0.2.9/image_registration/fft_tools/shift.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,22 +93,22 @@
     """
 
     fftn,ifftn = fast_ffts.get_ffts(nthreads=nthreads, use_numpy_fft=use_numpy_fft)
 
     if np.any(np.isnan(data)):
         data = np.nan_to_num(data)
 
-    freq_grid = np.sum(
-        [off*np.fft.fftfreq(nx)[
+    freq_grid = sum(
+            [off*np.fft.fftfreq(nx)[
             tuple(
                 [np.newaxis]*dim + [slice(None)] + [np.newaxis]*(data.ndim-dim-1)
                 )
             ]
-            for dim,(off,nx) in enumerate(zip(offset,data.shape))],
-        axis=0)
+            for dim,(off,nx) in enumerate(zip(offset,data.shape))]
+    )
 
     kernel = np.exp(-1j*2*np.pi*freq_grid-1j*phase)
 
     result = ifftn( fftn(data) * kernel )
 
     if return_real:
         return np.real(result)
```

### Comparing `image_registration-0.2.8/image_registration/fft_tools/smooth_tools.py` & `image_registration-0.2.9/image_registration/fft_tools/smooth_tools.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/fft_tools/tests/measure_accuracy.py` & `image_registration-0.2.9/image_registration/fft_tools/tests/measure_accuracy.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/fft_tools/tests/test_downsample.py` & `image_registration-0.2.9/image_registration/fft_tools/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/fft_tools/tests/test_shift.py` & `image_registration-0.2.9/image_registration/fft_tools/tests/test_shift.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/fft_tools/tests/test_upsample.py` & `image_registration-0.2.9/image_registration/fft_tools/tests/test_upsample.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/fft_tools/tests/test_upsample_1d.py` & `image_registration-0.2.9/image_registration/fft_tools/tests/test_upsample_1d.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/fft_tools/tests/test_zoomnd.py` & `image_registration-0.2.9/image_registration/fft_tools/tests/test_zoomnd.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/fft_tools/upsample.py` & `image_registration-0.2.9/image_registration/fft_tools/upsample.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/fft_tools/zoom.py` & `image_registration-0.2.9/image_registration/fft_tools/zoom.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/iterative_zoom.py` & `image_registration-0.2.9/image_registration/iterative_zoom.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/register_images.py` & `image_registration-0.2.9/image_registration/register_images.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/tests/coveragerc` & `image_registration-0.2.9/image_registration/tests/coveragerc`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/tests/debug_test.py` & `image_registration-0.2.9/image_registration/tests/debug_test.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/tests/measure_expected_offsets.py` & `image_registration-0.2.9/image_registration/tests/measure_expected_offsets.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration/tests/registration_testing.py` & `image_registration-0.2.9/image_registration/tests/registration_testing.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/image_registration.egg-info/PKG-INFO` & `image_registration-0.2.9/image_registration.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
-Name: image-registration
-Version: 0.2.8
+Name: image_registration
+Version: 0.2.9
 Summary: Package for registering images with extended emission
 Home-page: https://image-registration.readthedocs.io/en/latest/
 Author: Adam Ginsburg
 Author-email: adam.g.ginsburg@gmail.com
 License: BSD
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: astropy
+Requires-Dist: matplotlib
+Requires-Dist: pytest
 Provides-Extra: test
 Requires-Dist: pytest-astropy; extra == "test"
 Requires-Dist: matplotlib; extra == "test"
 Provides-Extra: docs
 Requires-Dist: sphinx-astropy; extra == "docs"
 Requires-Dist: matplotlib; extra == "docs"
 Requires-Dist: FITS_tools; extra == "docs"
```

### Comparing `image_registration-0.2.8/image_registration.egg-info/SOURCES.txt` & `image_registration-0.2.9/image_registration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/setup.cfg` & `image_registration-0.2.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 [options]
 zip_safe = False
 packages = find:
 python_requires = >=3.7
 setup_requires = setuptools_scm
 install_requires = 
 	astropy
+	matplotlib
+	pytest
 
 [options.entry_points]
 console_scripts = 
 	astropy-package-template-example = packagename.example_mod:main
 
 [options.extras_require]
 test =
```

### Comparing `image_registration-0.2.8/setup.py` & `image_registration-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `image_registration-0.2.8/tox.ini` & `image_registration-0.2.9/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tox]
 envlist =
-    py{36,37,38}-test{,-alldeps,-devdeps}{,-cov}
-    py{36,37,38}-test-numpy{116,117,118}
-    py{36,37,38}-test-astropy{30,40,lts}
+    py{310,311,312}-test{,-alldeps,-devdeps}{,-cov}
+    py{310,311,312}-test-numpy{116,117,118,120,126,200}
+    py{310,311,312}-test-astropy{30,40,lts}
     build_docs
     linkcheck
     codestyle
 requires =
     setuptools >= 30.3.0
     pip >= 19.3.1
     matplotlib
@@ -39,29 +39,35 @@
     alldeps: with all optional dependencies
     devdeps: with the latest developer version of key dependencies
     oldestdeps: with the oldest supported version of key dependencies
     cov: and test coverage
     numpy116: with numpy 1.16.*
     numpy117: with numpy 1.17.*
     numpy118: with numpy 1.18.*
+    numpy120: with numpy 1.20.*
+    numpy126: with numpy 1.26.*
+    numpy200: with numpy 200.*
     astropy30: with astropy 3.0.*
     astropy40: with astropy 4.0.*
     astropylts: with the latest astropy LTS
 
 # The following provides some specific pinnings for key packages
 deps =
 
     cov: coverage
     numpy116: numpy==1.16.*
     numpy117: numpy==1.17.*
     numpy118: numpy==1.18.*
+    numpy120: numpy==1.20.*
+    numpy126: numpy==1.26.*
+    numpy200: numpy==2.00.*
 
     astropy30: astropy==3.0.*
     astropy40: astropy==4.0.*
-    astropylts: astropy==4.0.*
+    astropylts: astropy==6.0.*
 
     devdeps: :NIGHTLY:numpy
     devdeps: git+https://github.com/astropy/astropy.git#egg=astropy
 
 # The following indicates which extras_require from setup.cfg will be installed
 extras =
     test
```

