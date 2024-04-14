# Comparing `tmp/psyke-0.8.2.dev4.tar.gz` & `tmp/psyke-0.8.2.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psyke-0.8.2.dev4.tar", last modified: Thu Apr 11 01:01:42 2024, max compression
+gzip compressed data, was "psyke-0.8.2.dev8.tar", last modified: Sat Apr 13 13:12:41 2024, max compression
```

## Comparing `psyke-0.8.2.dev4.tar` & `psyke-0.8.2.dev8.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.329067 psyke-0.8.2.dev4/
--rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-11 01:01:42.329067 psyke-0.8.2.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 01:01:42.000000 psyke-0.8.2.dev4/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.313067 psyke-0.8.2.dev4/psyke/
--rw-r--r--   0 runner    (1001) docker     (127)    18155 2024-04-11 01:01:40.000000 psyke-0.8.2.dev4/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.317067 psyke-0.8.2.dev4/psyke/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.317067 psyke-0.8.2.dev4/psyke/clustering/cream/
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/clustering/cream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.317067 psyke-0.8.2.dev4/psyke/clustering/exact/
--rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/clustering/exact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/clustering/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.317067 psyke-0.8.2.dev4/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.317067 psyke-0.8.2.dev4/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/extraction/cart/predictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.317067 psyke-0.8.2.dev4/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (127)    10451 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.317067 psyke-0.8.2.dev4/psyke/extraction/hypercubic/cosmik/
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/extraction/hypercubic/cosmik/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.317067 psyke-0.8.2.dev4/psyke/extraction/hypercubic/creepy/
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/extraction/hypercubic/creepy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.317067 psyke-0.8.2.dev4/psyke/extraction/hypercubic/divine/
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/extraction/hypercubic/divine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.317067 psyke-0.8.2.dev4/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/extraction/hypercubic/gridex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.321067 psyke-0.8.2.dev4/psyke/extraction/hypercubic/gridrex/
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/extraction/hypercubic/gridrex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.321067 psyke-0.8.2.dev4/psyke/extraction/hypercubic/hex/
--rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/extraction/hypercubic/hex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22322 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/extraction/hypercubic/hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.321067 psyke-0.8.2.dev4/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/extraction/hypercubic/iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/extraction/hypercubic/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/extraction/hypercubic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.321067 psyke-0.8.2.dev4/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/extraction/real/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.321067 psyke-0.8.2.dev4/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/extraction/trepan/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/hypercubepredictor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.321067 psyke-0.8.2.dev4/psyke/schema/
--rw-r--r--   0 runner    (1001) docker     (127)    15760 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.321067 psyke-0.8.2.dev4/psyke/tuning/
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/tuning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.321067 psyke-0.8.2.dev4/psyke/tuning/crash/
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/tuning/crash/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.321067 psyke-0.8.2.dev4/psyke/tuning/orchid/
--rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/tuning/orchid/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.321067 psyke-0.8.2.dev4/psyke/tuning/pedro/
--rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/tuning/pedro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.321067 psyke-0.8.2.dev4/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/utils/logic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/psyke/utils/sorted.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.325067 psyke-0.8.2.dev4/psyke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-11 01:01:42.000000 psyke-0.8.2.dev4/psyke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-11 01:01:42.000000 psyke-0.8.2.dev4/psyke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:01:42.000000 psyke-0.8.2.dev4/psyke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:01:42.000000 psyke-0.8.2.dev4/psyke.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-11 01:01:42.000000 psyke-0.8.2.dev4/psyke.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-11 01:01:42.000000 psyke-0.8.2.dev4/psyke.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 01:01:42.329067 psyke-0.8.2.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.313067 psyke-0.8.2.dev4/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.321067 psyke-0.8.2.dev4/test/psyke/
--rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/test/psyke/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.321067 psyke-0.8.2.dev4/test/psyke/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/test/psyke/clustering/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.321067 psyke-0.8.2.dev4/test/psyke/extraction/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/test/psyke/extraction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.325067 psyke-0.8.2.dev4/test/psyke/extraction/cart/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/test/psyke/extraction/cart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/test/psyke/extraction/cart/test_cart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/test/psyke/extraction/cart/test_simplified_cart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.325067 psyke-0.8.2.dev4/test/psyke/extraction/hypercubic/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/test/psyke/extraction/hypercubic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.325067 psyke-0.8.2.dev4/test/psyke/extraction/hypercubic/gridex/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/test/psyke/extraction/hypercubic/gridex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/test/psyke/extraction/hypercubic/gridex/test_gridex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.325067 psyke-0.8.2.dev4/test/psyke/extraction/hypercubic/iter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/test/psyke/extraction/hypercubic/iter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/test/psyke/extraction/hypercubic/iter/test_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14266 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/test/psyke/extraction/hypercubic/test_hypercube.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.325067 psyke-0.8.2.dev4/test/psyke/extraction/real/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/test/psyke/extraction/real/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/test/psyke/extraction/real/test_real.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/test/psyke/extraction/real/test_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.325067 psyke-0.8.2.dev4/test/psyke/extraction/trepan/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/test/psyke/extraction/trepan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/test/psyke/extraction/trepan/test_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/test/psyke/extraction/trepan/test_split.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/test/psyke/extraction/trepan/test_trepan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.325067 psyke-0.8.2.dev4/test/psyke/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/test/psyke/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/test/psyke/utils/test_prune.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/test/psyke/utils/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-11 01:00:34.000000 psyke-0.8.2.dev4/test/psyke/utils/test_simplify_formatter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.325067 psyke-0.8.2.dev4/test/resources/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-11 01:00:35.000000 psyke-0.8.2.dev4/test/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.325067 psyke-0.8.2.dev4/test/resources/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-11 01:00:35.000000 psyke-0.8.2.dev4/test/resources/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.325067 psyke-0.8.2.dev4/test/resources/predictors/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-11 01:00:35.000000 psyke-0.8.2.dev4/test/resources/predictors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 01:01:42.325067 psyke-0.8.2.dev4/test/resources/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-11 01:00:36.000000 psyke-0.8.2.dev4/test/resources/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.994426 psyke-0.8.2.dev8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11354 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-13 13:12:41.994426 psyke-0.8.2.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6843 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-13 13:12:41.000000 psyke-0.8.2.dev8/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.982426 psyke-0.8.2.dev8/psyke/
+-rw-r--r--   0 runner    (1001) docker     (127)    18155 2024-04-13 13:12:40.000000 psyke-0.8.2.dev8/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.982426 psyke-0.8.2.dev8/psyke/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.982426 psyke-0.8.2.dev8/psyke/clustering/cream/
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/clustering/cream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.982426 psyke-0.8.2.dev8/psyke/clustering/exact/
+-rw-r--r--   0 runner    (1001) docker     (127)     5243 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/clustering/exact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/clustering/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.982426 psyke-0.8.2.dev8/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.982426 psyke-0.8.2.dev8/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/extraction/cart/predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.982426 psyke-0.8.2.dev8/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (127)    10368 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.982426 psyke-0.8.2.dev8/psyke/extraction/hypercubic/cosmik/
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/extraction/hypercubic/cosmik/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.986426 psyke-0.8.2.dev8/psyke/extraction/hypercubic/creepy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/extraction/hypercubic/creepy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.986426 psyke-0.8.2.dev8/psyke/extraction/hypercubic/divine/
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/extraction/hypercubic/divine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.986426 psyke-0.8.2.dev8/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/extraction/hypercubic/gridex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.986426 psyke-0.8.2.dev8/psyke/extraction/hypercubic/gridrex/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/extraction/hypercubic/gridrex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.986426 psyke-0.8.2.dev8/psyke/extraction/hypercubic/hex/
+-rw-r--r--   0 runner    (1001) docker     (127)     4562 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/extraction/hypercubic/hex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22754 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/extraction/hypercubic/hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.986426 psyke-0.8.2.dev8/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (127)    10084 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/extraction/hypercubic/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/extraction/hypercubic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.986426 psyke-0.8.2.dev8/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/extraction/real/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.986426 psyke-0.8.2.dev8/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/extraction/trepan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/hypercubepredictor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.986426 psyke-0.8.2.dev8/psyke/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)    15760 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.986426 psyke-0.8.2.dev8/psyke/tuning/
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/tuning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.986426 psyke-0.8.2.dev8/psyke/tuning/crash/
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/tuning/crash/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.986426 psyke-0.8.2.dev8/psyke/tuning/orchid/
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/tuning/orchid/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.986426 psyke-0.8.2.dev8/psyke/tuning/pedro/
+-rw-r--r--   0 runner    (1001) docker     (127)     6395 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/tuning/pedro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.986426 psyke-0.8.2.dev8/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12419 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/utils/logic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/psyke/utils/sorted.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.994426 psyke-0.8.2.dev8/psyke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-13 13:12:41.000000 psyke-0.8.2.dev8/psyke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-13 13:12:41.000000 psyke-0.8.2.dev8/psyke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:12:41.000000 psyke-0.8.2.dev8/psyke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:12:41.000000 psyke-0.8.2.dev8/psyke.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-13 13:12:41.000000 psyke-0.8.2.dev8/psyke.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-13 13:12:41.000000 psyke-0.8.2.dev8/psyke.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 13:12:41.994426 psyke-0.8.2.dev8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8400 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.978426 psyke-0.8.2.dev8/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.990426 psyke-0.8.2.dev8/test/psyke/
+-rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/test/psyke/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.990426 psyke-0.8.2.dev8/test/psyke/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/test/psyke/clustering/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.990426 psyke-0.8.2.dev8/test/psyke/extraction/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/test/psyke/extraction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.990426 psyke-0.8.2.dev8/test/psyke/extraction/cart/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/test/psyke/extraction/cart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/test/psyke/extraction/cart/test_cart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/test/psyke/extraction/cart/test_simplified_cart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.990426 psyke-0.8.2.dev8/test/psyke/extraction/hypercubic/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/test/psyke/extraction/hypercubic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.990426 psyke-0.8.2.dev8/test/psyke/extraction/hypercubic/gridex/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/test/psyke/extraction/hypercubic/gridex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/test/psyke/extraction/hypercubic/gridex/test_gridex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.990426 psyke-0.8.2.dev8/test/psyke/extraction/hypercubic/iter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/test/psyke/extraction/hypercubic/iter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/test/psyke/extraction/hypercubic/iter/test_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14266 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/test/psyke/extraction/hypercubic/test_hypercube.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.990426 psyke-0.8.2.dev8/test/psyke/extraction/real/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/test/psyke/extraction/real/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/test/psyke/extraction/real/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/test/psyke/extraction/real/test_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.990426 psyke-0.8.2.dev8/test/psyke/extraction/trepan/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/test/psyke/extraction/trepan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/test/psyke/extraction/trepan/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/test/psyke/extraction/trepan/test_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/test/psyke/extraction/trepan/test_trepan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.990426 psyke-0.8.2.dev8/test/psyke/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/test/psyke/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/test/psyke/utils/test_prune.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/test/psyke/utils/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-13 13:11:36.000000 psyke-0.8.2.dev8/test/psyke/utils/test_simplify_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.994426 psyke-0.8.2.dev8/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-13 13:11:37.000000 psyke-0.8.2.dev8/test/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.994426 psyke-0.8.2.dev8/test/resources/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-13 13:11:37.000000 psyke-0.8.2.dev8/test/resources/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.994426 psyke-0.8.2.dev8/test/resources/predictors/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-13 13:11:37.000000 psyke-0.8.2.dev8/test/resources/predictors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 13:12:41.994426 psyke-0.8.2.dev8/test/resources/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-13 13:11:38.000000 psyke-0.8.2.dev8/test/resources/tests/__init__.py
```

### Comparing `psyke-0.8.2.dev4/LICENSE` & `psyke-0.8.2.dev8/LICENSE`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/PKG-INFO` & `psyke-0.8.2.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.8.2.dev4
+Version: 0.8.2.dev8
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.8.2.dev4/README.md` & `psyke-0.8.2.dev8/README.md`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/__init__.py` & `psyke-0.8.2.dev8/psyke/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/clustering/__init__.py` & `psyke-0.8.2.dev8/psyke/clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/clustering/cream/__init__.py` & `psyke-0.8.2.dev8/psyke/clustering/cream/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/clustering/exact/__init__.py` & `psyke-0.8.2.dev8/psyke/clustering/exact/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/clustering/utils.py` & `psyke-0.8.2.dev8/psyke/clustering/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/extraction/__init__.py` & `psyke-0.8.2.dev8/psyke/extraction/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/extraction/cart/__init__.py` & `psyke-0.8.2.dev8/psyke/extraction/cart/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/extraction/cart/predictor.py` & `psyke-0.8.2.dev8/psyke/extraction/cart/predictor.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/extraction/hypercubic/__init__.py` & `psyke-0.8.2.dev8/psyke/extraction/hypercubic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from __future__ import annotations
 
 from abc import ABC
-from itertools import groupby
-from typing import Iterable
 import numpy as np
 import pandas as pd
 from sklearn.base import ClassifierMixin
 from sklearn.feature_selection import SelectKBest, f_regression, f_classif
 from sklearn.linear_model import LinearRegression
 from tuprolog.core import Var, Struct, clause
 from tuprolog.theory import Theory, mutable_theory
 from psyke import logger
 from psyke.extraction import PedagogicalExtractor
 from psyke.extraction.hypercubic.hypercube import HyperCube, RegressionCube, ClassificationCube, ClosedCube, Point, \
     GenericCube
 from psyke.hypercubepredictor import HyperCubePredictor
 from psyke.schema import Between, Outside, Value
-from psyke.utils.logic import create_variable_list, create_head, to_var, Simplifier, last_in_body, PRECISION
+from psyke.utils.logic import create_variable_list, create_head, to_var, Simplifier
 from psyke.utils import Target
 from psyke.extraction.hypercubic.strategy import Strategy, FixedStrategy
 
 
 class HyperCubeExtractor(HyperCubePredictor, PedagogicalExtractor, ABC):
     def __init__(self, predictor, output, discretization=None, normalization=None):
         HyperCubePredictor.__init__(self, output=output, normalization=normalization)
```

### Comparing `psyke-0.8.2.dev4/psyke/extraction/hypercubic/cosmik/__init__.py` & `psyke-0.8.2.dev8/psyke/extraction/hypercubic/cosmik/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/extraction/hypercubic/creepy/__init__.py` & `psyke-0.8.2.dev8/psyke/extraction/hypercubic/creepy/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/extraction/hypercubic/divine/__init__.py` & `psyke-0.8.2.dev8/psyke/extraction/hypercubic/divine/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/extraction/hypercubic/gridex/__init__.py` & `psyke-0.8.2.dev8/psyke/extraction/hypercubic/gridex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/extraction/hypercubic/gridrex/__init__.py` & `psyke-0.8.2.dev8/psyke/extraction/hypercubic/gridrex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/extraction/hypercubic/hex/__init__.py` & `psyke-0.8.2.dev8/psyke/extraction/hypercubic/hex/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/extraction/hypercubic/hypercube.py` & `psyke-0.8.2.dev8/psyke/extraction/hypercubic/hypercube.py`

 * *Files 2% similar despite different names*

```diff
@@ -411,28 +411,34 @@
 
     # TODO: why this is not a property?
     def init_diversity(self, std: float) -> None:
         self._diversity = std
 
 
 class RegressionCube(HyperCube):
-    def __init__(self, dimension: dict[str, tuple] = None, output=LinearRegression()):
-        super().__init__(dimension=dimension, output=output)
+    def __init__(self, dimension: dict[str, tuple] = None, output=None):
+        super().__init__(dimension=dimension, output=LinearRegression() if output is None else output)
 
     def update(self, dataset: pd.DataFrame, predictor) -> None:
         filtered = self.filter_dataframe(dataset.iloc[:, :-1])
         if len(filtered > 0):
             predictions = predictor.predict(filtered)
             self._output.fit(filtered, predictions)
             self._diversity = self._error = (abs(self._output.predict(filtered) - predictions)).mean()
             means = filtered.describe().loc['mean']
             self._barycenter = Point(means.index.values, means.values)
 
     def copy(self) -> RegressionCube:
-        return RegressionCube(self.dimensions.copy(), output=self._output)
+        output = LinearRegression()
+        try:
+            output.coef_ = self.output.coef_.copy()
+            output.intercept_ = self.output.intercept_
+        except AttributeError:
+            pass
+        return RegressionCube(self.dimensions.copy(), output=output)
 
     def body(self, variables: dict[str, Var], ignore: list[str], unscale=None, normalization=None) -> Iterable[Struct]:
         intercept = self.output.intercept_ if normalization is None else unscale(sum(
             [-self.output.coef_[i] * normalization[name][0] / normalization[name][1] for i, name in
              enumerate(self.dimensions.keys())], self.output.intercept_), list(normalization.keys())[-1])
         coefs = self.output.coef_ if normalization is None else [
             self.output.coef_[i] / normalization[name][1] * normalization[list(normalization.keys())[-1]][1] for
@@ -485,19 +491,25 @@
         return np.all((v[:, 0] <= ds) & (ds <= v[:, 1]), axis=1)
 
     def copy(self) -> ClosedCube:
         return ClosedCube(self.dimensions.copy(), output=self._output)
 
 
 class ClosedRegressionCube(ClosedCube, RegressionCube):
-    def __init__(self, dimension: dict[str, tuple] = None, output: LinearRegression = LinearRegression()):
-        super().__init__(dimension=dimension, output=output)
+    def __init__(self, dimension: dict[str, tuple] = None, output=None):
+        super().__init__(dimension=dimension, output=LinearRegression() if output is None else output)
 
     def copy(self) -> ClosedRegressionCube:
-        return ClosedRegressionCube(self.dimensions.copy(), output=self._output)
+        output = LinearRegression()
+        try:
+            output.coef_ = self.output.coef_.copy()
+            output.intercept_ = self.output.intercept_
+        except AttributeError:
+            pass
+        return ClosedRegressionCube(self.dimensions.copy(), output=output)
 
 
 class ClosedClassificationCube(ClosedCube, ClassificationCube):
     def __init__(self, dimension: dict[str, tuple] = None, output: str = None):
         super().__init__(dimension=dimension, output=output)
 
     def copy(self) -> ClosedClassificationCube:
```

### Comparing `psyke-0.8.2.dev4/psyke/extraction/hypercubic/iter/__init__.py` & `psyke-0.8.2.dev8/psyke/extraction/hypercubic/iter/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/extraction/hypercubic/strategy.py` & `psyke-0.8.2.dev8/psyke/extraction/hypercubic/strategy.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/extraction/hypercubic/utils.py` & `psyke-0.8.2.dev8/psyke/extraction/hypercubic/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/extraction/real/__init__.py` & `psyke-0.8.2.dev8/psyke/extraction/real/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/extraction/real/utils.py` & `psyke-0.8.2.dev8/psyke/extraction/real/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/extraction/trepan/__init__.py` & `psyke-0.8.2.dev8/psyke/extraction/trepan/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/extraction/trepan/utils.py` & `psyke-0.8.2.dev8/psyke/extraction/trepan/utils.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/hypercubepredictor.py` & `psyke-0.8.2.dev8/psyke/hypercubepredictor.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/schema/__init__.py` & `psyke-0.8.2.dev8/psyke/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/tuning/__init__.py` & `psyke-0.8.2.dev8/psyke/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/tuning/crash/__init__.py` & `psyke-0.8.2.dev8/psyke/tuning/crash/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/tuning/orchid/__init__.py` & `psyke-0.8.2.dev8/psyke/tuning/orchid/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/tuning/pedro/__init__.py` & `psyke-0.8.2.dev8/psyke/tuning/pedro/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/utils/__init__.py` & `psyke-0.8.2.dev8/psyke/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/utils/dataframe.py` & `psyke-0.8.2.dev8/psyke/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/utils/logic.py` & `psyke-0.8.2.dev8/psyke/utils/logic.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/utils/metrics.py` & `psyke-0.8.2.dev8/psyke/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/utils/plot.py` & `psyke-0.8.2.dev8/psyke/utils/plot.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke/utils/sorted.py` & `psyke-0.8.2.dev8/psyke/utils/sorted.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/psyke.egg-info/PKG-INFO` & `psyke-0.8.2.dev8/psyke.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psyke
-Version: 0.8.2.dev4
+Version: 0.8.2.dev8
 Summary: Python-based implementation of PSyKE, i.e. a Platform for Symbolic Knowledge Extraction
 Home-page: https://github.com/psykei/psyke-python
 Author: Matteo Magnini
 Author-email: matteo.magnini@unibo.it
 License: Apache 2.0 License
 Project-URL: Bug Reports, https://github.com/psykei/psyke-python/issues
 Project-URL: Source, https://github.com/psykei/psyke-python
```

### Comparing `psyke-0.8.2.dev4/psyke.egg-info/SOURCES.txt` & `psyke-0.8.2.dev8/psyke.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/setup.py` & `psyke-0.8.2.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/test/psyke/__init__.py` & `psyke-0.8.2.dev8/test/psyke/__init__.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/test/psyke/extraction/cart/test_cart.py` & `psyke-0.8.2.dev8/test/psyke/extraction/cart/test_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/test/psyke/extraction/cart/test_simplified_cart.py` & `psyke-0.8.2.dev8/test/psyke/extraction/cart/test_simplified_cart.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/test/psyke/extraction/hypercubic/gridex/test_gridex.py` & `psyke-0.8.2.dev8/test/psyke/extraction/hypercubic/gridex/test_gridex.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/test/psyke/extraction/hypercubic/iter/test_iter.py` & `psyke-0.8.2.dev8/test/psyke/extraction/hypercubic/iter/test_iter.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/test/psyke/extraction/hypercubic/test_hypercube.py` & `psyke-0.8.2.dev8/test/psyke/extraction/hypercubic/test_hypercube.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/test/psyke/extraction/real/test_real.py` & `psyke-0.8.2.dev8/test/psyke/extraction/real/test_real.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/test/psyke/extraction/real/test_rule.py` & `psyke-0.8.2.dev8/test/psyke/extraction/real/test_rule.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/test/psyke/extraction/trepan/test_node.py` & `psyke-0.8.2.dev8/test/psyke/extraction/trepan/test_node.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/test/psyke/extraction/trepan/test_split.py` & `psyke-0.8.2.dev8/test/psyke/extraction/trepan/test_split.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/test/psyke/extraction/trepan/test_trepan.py` & `psyke-0.8.2.dev8/test/psyke/extraction/trepan/test_trepan.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/test/psyke/utils/test_prune.py` & `psyke-0.8.2.dev8/test/psyke/utils/test_prune.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/test/psyke/utils/test_simplify.py` & `psyke-0.8.2.dev8/test/psyke/utils/test_simplify.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/test/psyke/utils/test_simplify_formatter.py` & `psyke-0.8.2.dev8/test/psyke/utils/test_simplify_formatter.py`

 * *Files identical despite different names*

### Comparing `psyke-0.8.2.dev4/test/resources/tests/__init__.py` & `psyke-0.8.2.dev8/test/resources/tests/__init__.py`

 * *Files identical despite different names*

