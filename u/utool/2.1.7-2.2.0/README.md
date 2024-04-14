# Comparing `tmp/utool-2.1.7.tar.gz` & `tmp/utool-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utool-2.1.7.tar", last modified: Sun Jan 29 02:45:58 2023, max compression
+gzip compressed data, was "utool-2.2.0.tar", last modified: Sun Apr 14 00:30:20 2024, max compression
```

## Comparing `utool-2.1.7.tar` & `utool-2.2.0.tar`

### file list

```diff
@@ -1,103 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 02:45:58.689964 utool-2.1.7/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11323 2023-01-29 02:45:50.000000 utool-2.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-01-29 02:45:58.689964 utool-2.1.7/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-01-29 02:45:50.000000 utool-2.1.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-01-29 02:45:50.000000 utool-2.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-01-29 02:45:58.689964 utool-2.1.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     8911 2023-01-29 02:45:50.000000 utool-2.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 02:45:58.689964 utool-2.1.7/utool/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3404 2023-01-29 02:45:50.000000 utool-2.1.7/utool/DynamicStruct.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25215 2023-01-29 02:45:50.000000 utool-2.1.7/utool/Preferences.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6657 2023-01-29 02:45:50.000000 utool-2.1.7/utool/Printable.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    62834 2023-01-29 02:45:50.000000 utool-2.1.7/utool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-01-29 02:45:50.000000 utool-2.1.7/utool/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 02:45:58.689964 utool-2.1.7/utool/_internal/
--rwxr-xr-x   0 runner    (1001) docker     (123)      292 2023-01-29 02:45:50.000000 utool-2.1.7/utool/_internal/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4165 2023-01-29 02:45:50.000000 utool-2.1.7/utool/_internal/meta_util_arg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1202 2023-01-29 02:45:50.000000 utool-2.1.7/utool/_internal/meta_util_cache.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      252 2023-01-29 02:45:50.000000 utool-2.1.7/utool/_internal/meta_util_constants.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1220 2023-01-29 02:45:50.000000 utool-2.1.7/utool/_internal/meta_util_cplat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-01-29 02:45:50.000000 utool-2.1.7/utool/_internal/meta_util_dbg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1417 2023-01-29 02:45:50.000000 utool-2.1.7/utool/_internal/meta_util_git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-01-29 02:45:50.000000 utool-2.1.7/utool/_internal/meta_util_iter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      919 2023-01-29 02:45:50.000000 utool-2.1.7/utool/_internal/meta_util_path.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4613 2023-01-29 02:45:50.000000 utool-2.1.7/utool/_internal/meta_util_six.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-01-29 02:45:50.000000 utool-2.1.7/utool/_internal/py2_syntax_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-01-29 02:45:50.000000 utool-2.1.7/utool/_internal/randomwrap.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17542 2023-01-29 02:45:50.000000 utool-2.1.7/utool/_internal/util_importer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18854 2023-01-29 02:45:50.000000 utool-2.1.7/utool/_internal/win32_send_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 02:45:58.689964 utool-2.1.7/utool/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-29 02:45:50.000000 utool-2.1.7/utool/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-01-29 02:45:50.000000 utool-2.1.7/utool/experimental/bytecode_optimizations.py
--rw-r--r--   0 runner    (1001) docker     (123)    32280 2023-01-29 02:45:50.000000 utool-2.1.7/utool/experimental/dynamic_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (123)    37862 2023-01-29 02:45:50.000000 utool-2.1.7/utool/experimental/euler_tour_tree_avl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-01-29 02:45:50.000000 utool-2.1.7/utool/experimental/pandas_highlight.py
--rw-r--r--   0 runner    (1001) docker     (123)    16691 2023-01-29 02:45:50.000000 utool-2.1.7/utool/oldalg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-01-29 02:45:50.000000 utool-2.1.7/utool/sandbox.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 02:45:58.689964 utool-2.1.7/utool/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-29 02:45:50.000000 utool-2.1.7/utool/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-01-29 02:45:50.000000 utool-2.1.7/utool/tests/_oldtest_decor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4521 2023-01-29 02:45:50.000000 utool-2.1.7/utool/tests/_oldtest_hash.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2233 2023-01-29 02:45:50.000000 utool-2.1.7/utool/tests/_oldtest_logging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1651 2023-01-29 02:45:50.000000 utool-2.1.7/utool/tests/_oldtest_reloading.py
--rw-r--r--   0 runner    (1001) docker     (123)     5637 2023-01-29 02:45:50.000000 utool-2.1.7/utool/tests/run_tests.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    95826 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_alg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      421 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_aliases.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    45463 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_arg.py
--rw-r--r--   0 runner    (1001) docker     (123)    11090 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_assert.py
--rw-r--r--   0 runner    (1001) docker     (123)    38063 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_autogen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    56184 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_cache.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    35896 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_const.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49053 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_cplat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13720 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_csv.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    48758 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_dbg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    35228 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_decor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_depricated.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   115719 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_dev.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    68893 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_dict.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1424 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_func.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    38083 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_git.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    44394 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_grabdata.py
--rw-r--r--   0 runner    (1001) docker     (123)    85924 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    88494 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_gridsearch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    40343 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    21078 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_import.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22140 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_inject.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   120460 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28576 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    11812 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_ipynb.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20577 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_iter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34213 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_latex.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   104674 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_list.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20556 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_logging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4259 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_num.py
--rw-r--r--   0 runner    (1001) docker     (123)    12783 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_numpy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    37497 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_parallel.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    94079 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_path.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11426 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_print.py
--rw-r--r--   0 runner    (1001) docker     (123)     7738 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_profile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36286 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)    34438 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_project.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14759 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_regex.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9459 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_set.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24831 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_setup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_six.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_sqlite.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   119632 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_str.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8166 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_sysreq.py
--rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_tags.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    78781 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_tests.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    37718 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_time.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15865 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    25927 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_ubuntu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-01-29 02:45:50.000000 utool-2.1.7/utool/util_win32.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 02:45:58.689964 utool-2.1.7/utool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-01-29 02:45:58.000000 utool-2.1.7/utool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-01-29 02:45:58.000000 utool-2.1.7/utool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-29 02:45:58.000000 utool-2.1.7/utool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14149 2023-01-29 02:45:58.000000 utool-2.1.7/utool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-29 02:45:58.000000 utool-2.1.7/utool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:30:20.708495 utool-2.2.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11323 2024-04-14 00:29:51.000000 utool-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    45440 2024-04-14 00:30:20.708495 utool-2.2.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3023 2024-04-14 00:29:51.000000 utool-2.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-14 00:29:51.000000 utool-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-14 00:30:20.708495 utool-2.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9162 2024-04-14 00:29:51.000000 utool-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:30:20.628495 utool-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-14 00:29:51.000000 utool-2.2.0/tests/test_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:30:20.640495 utool-2.2.0/utool/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3404 2024-04-14 00:29:51.000000 utool-2.2.0/utool/DynamicStruct.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25225 2024-04-14 00:29:51.000000 utool-2.2.0/utool/Preferences.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6657 2024-04-14 00:29:51.000000 utool-2.2.0/utool/Printable.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    62834 2024-04-14 00:29:51.000000 utool-2.2.0/utool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-14 00:29:51.000000 utool-2.2.0/utool/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:30:20.640495 utool-2.2.0/utool/_internal/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      292 2024-04-14 00:29:51.000000 utool-2.2.0/utool/_internal/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4165 2024-04-14 00:29:51.000000 utool-2.2.0/utool/_internal/meta_util_arg.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1202 2024-04-14 00:29:51.000000 utool-2.2.0/utool/_internal/meta_util_cache.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      252 2024-04-14 00:29:51.000000 utool-2.2.0/utool/_internal/meta_util_constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1220 2024-04-14 00:29:51.000000 utool-2.2.0/utool/_internal/meta_util_cplat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-14 00:29:51.000000 utool-2.2.0/utool/_internal/meta_util_dbg.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1417 2024-04-14 00:29:51.000000 utool-2.2.0/utool/_internal/meta_util_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-14 00:29:51.000000 utool-2.2.0/utool/_internal/meta_util_iter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      919 2024-04-14 00:29:51.000000 utool-2.2.0/utool/_internal/meta_util_path.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1798 2024-04-14 00:29:51.000000 utool-2.2.0/utool/_internal/meta_util_six.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-04-14 00:29:51.000000 utool-2.2.0/utool/_internal/py2_syntax_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5537 2024-04-14 00:29:51.000000 utool-2.2.0/utool/_internal/randomwrap.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17542 2024-04-14 00:29:51.000000 utool-2.2.0/utool/_internal/util_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18854 2024-04-14 00:29:51.000000 utool-2.2.0/utool/_internal/win32_send_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18176 2024-04-14 00:29:51.000000 utool-2.2.0/utool/_kwimage_im_demodata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:30:20.644495 utool-2.2.0/utool/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 00:29:51.000000 utool-2.2.0/utool/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12988 2024-04-14 00:29:51.000000 utool-2.2.0/utool/experimental/bytecode_optimizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32280 2024-04-14 00:29:51.000000 utool-2.2.0/utool/experimental/dynamic_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37862 2024-04-14 00:29:51.000000 utool-2.2.0/utool/experimental/euler_tour_tree_avl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9050 2024-04-14 00:29:51.000000 utool-2.2.0/utool/experimental/pandas_highlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16691 2024-04-14 00:29:51.000000 utool-2.2.0/utool/oldalg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-14 00:29:51.000000 utool-2.2.0/utool/sandbox.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    95826 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_alg.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_aliases.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    45463 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_arg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11090 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_assert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38063 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_autogen.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    56184 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_cache.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35896 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_const.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    48971 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_cplat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13720 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_csv.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    48758 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_dbg.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    32317 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_decor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_depricated.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   115719 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_dev.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    68893 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_dict.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1424 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_func.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    38083 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_git.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    44812 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_grabdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85924 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88494 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_gridsearch.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    40343 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21078 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_import.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22140 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_inject.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   120460 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    28576 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11812 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_ipynb.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20577 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_iter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34213 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_latex.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   104674 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20556 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4259 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_num.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12783 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_numpy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    37497 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_parallel.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    94046 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_path.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11426 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_profile.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    36286 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34438 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_project.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14759 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_regex.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9459 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_set.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24831 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_six.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7338 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_sqlite.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   119681 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_str.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8166 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_sysreq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10873 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_tags.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    78781 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_tests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    35169 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_time.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15865 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25927 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_ubuntu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-14 00:29:51.000000 utool-2.2.0/utool/util_win32.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 00:30:20.644495 utool-2.2.0/utool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    45440 2024-04-14 00:30:20.000000 utool-2.2.0/utool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-14 00:30:20.000000 utool-2.2.0/utool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 00:30:20.000000 utool-2.2.0/utool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18724 2024-04-14 00:30:20.000000 utool-2.2.0/utool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-14 00:30:20.000000 utool-2.2.0/utool.egg-info/top_level.txt
```

### Comparing `utool-2.1.7/LICENSE` & `utool-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/README.rst` & `utool-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/pyproject.toml` & `utool-2.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -9,27 +9,34 @@
 tags = ["github", "erotemic", "purepy", "notypes"]
 mod_name = "utool"
 repo_name = "utool"
 rel_mod_parent_dpath = "."
 ci_pypy_versions = []
 os = [ "linux", "osx", "win",]
 url = 'https://github.com/Erotemic/utool'
-min_python = 3.6
+min_python = 3.8
+max_python = 3.11
 version = "{mod_dpath}/__init__.py::__version__"
 author = "Jon Crall"
 author_email = "erotemic@gmail.com"
 description = "Useful utilities and the kitchen sink"
 license = "Apache 2"
 dev_status = "alpha"
 
 
 [tool.pytest.ini_options]
 addopts = "-p no:doctest --xdoctest --xdoctest-style=google --ignore-glob=setup.py --ignore-glob=docs"
-norecursedirs = ".git ignore build __pycache__ dev _skbuild utool/tests utool/experimental docs"
-filterwarnings = [ "default", "ignore:.*No cfgstr given in Cacher constructor or call.*:Warning", "ignore:.*Define the __nice__ method for.*:Warning", "ignore:.*private pytest class or function.*:Warning",]
+norecursedirs = ".git ignore build __pycache__ dev _skbuild docs"
+filterwarnings = [
+    "default",
+    "ignore:.*No cfgstr given in Cacher constructor or call.*:Warning",
+    "ignore:.*Define the __nice__ method for.*:Warning",
+    "ignore:.*private pytest class or function.*:Warning",
+]
+
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 exclude_lines = [ "pragma: no cover", ".*  # pragma: no cover", ".*  # nocover", "def __repr__", "raise AssertionError", "raise NotImplementedError", "if 0:", "if trace is not None", "verbose = .*", "^ *raise", "^ *pass *$", "if _debug:", "if __name__ == .__main__.:", ".*if six.PY2:",]
 omit = [ "utool/__main__.py", "*/setup.py",]
```

### Comparing `utool-2.1.7/setup.py` & `utool-2.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # Generated by ~/code/xcookie/xcookie/builders/setup.py
 # based on part ~/code/xcookie/xcookie/rc/setup.py.in
 import sys
-from os.path import exists
+import re
+from os.path import exists, dirname, join
 from setuptools import find_packages
 from setuptools import setup
 
 
 def parse_version(fpath):
     """
     Statically parse the version number from a python file
@@ -49,16 +50,14 @@
     """
     Parse the description in the README file
 
     CommandLine:
         pandoc --from=markdown --to=rst --output=README.rst README.md
         python -c "import setup; print(setup.parse_description())"
     """
-    from os.path import dirname, join, exists
-
     readme_fpath = join(dirname(__file__), "README.rst")
     # This breaks on pip install, so check that it exists.
     if exists(readme_fpath):
         with open(readme_fpath, "r") as f:
             text = f.read()
         return text
     return ""
@@ -73,18 +72,18 @@
         fname (str): path to requirements file
         versions (bool | str, default=False):
             If true include version specs.
             If strict, then pin to the minimum version.
 
     Returns:
         List[str]: list of requirements items
-    """
-    from os.path import exists, dirname, join
-    import re
 
+    CommandLine:
+        python -c "import setup, ubelt; print(ubelt.urepr(setup.parse_requirements()))"
+    """
     require_fpath = fname
 
     def parse_line(line, dpath=""):
         """
         Parse information from a line in a requirements text file
 
         line = 'git+https://a.com/somedep@sometag#egg=SomeDep'
@@ -194,52 +193,54 @@
 #             raise KeyError(versions)
 #     requirements = [r.replace(' ', '') for r in requirements]
 #     return requirements
 
 
 NAME = "utool"
 INIT_PATH = "utool/__init__.py"
-VERSION = parse_version("utool/__init__.py")
+VERSION = parse_version(INIT_PATH)
 
 if __name__ == "__main__":
     setupkw = {}
 
-    setupkw["install_requires"] = parse_requirements("requirements/runtime.txt")
+    setupkw["install_requires"] = parse_requirements(
+        "requirements/runtime.txt", versions="loose"
+    )
     setupkw["extras_require"] = {
-        "all": parse_requirements("requirements.txt"),
-        "tests": parse_requirements("requirements/tests.txt"),
-        "optional": parse_requirements("requirements/optional.txt"),
+        "all": parse_requirements("requirements.txt", versions="loose"),
+        "runtime": parse_requirements("requirements/runtime.txt", versions="loose"),
+        "tests": parse_requirements("requirements/tests.txt", versions="loose"),
+        "optional": parse_requirements("requirements/optional.txt", versions="loose"),
+        "docs": parse_requirements("requirements/docs.txt", versions="loose"),
         "all-strict": parse_requirements("requirements.txt", versions="strict"),
         "runtime-strict": parse_requirements(
             "requirements/runtime.txt", versions="strict"
         ),
         "tests-strict": parse_requirements("requirements/tests.txt", versions="strict"),
         "optional-strict": parse_requirements(
             "requirements/optional.txt", versions="strict"
         ),
+        "docs-strict": parse_requirements("requirements/docs.txt", versions="strict"),
     }
-
     setupkw["name"] = NAME
     setupkw["version"] = VERSION
     setupkw["author"] = "Jon Crall"
     setupkw["author_email"] = "erotemic@gmail.com"
     setupkw["url"] = "https://github.com/Erotemic/utool"
     setupkw["description"] = "Useful utilities and the kitchen sink"
     setupkw["long_description"] = parse_description()
     setupkw["long_description_content_type"] = "text/x-rst"
     setupkw["license"] = "Apache 2"
     setupkw["packages"] = find_packages(".")
-    setupkw["python_requires"] = ">=3.6"
+    setupkw["python_requires"] = ">=3.8"
     setupkw["classifiers"] = [
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Utilities",
         "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ]
     setup(**setupkw)
```

### Comparing `utool-2.1.7/utool/DynamicStruct.py` & `utool-2.2.0/utool/DynamicStruct.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/Preferences.py` & `utool-2.2.0/utool/Preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         # Try to select by index
         if isinstance(new_val, int):
             self.sel = new_val
         # Try to select by value
         elif isinstance(new_val, six.string_types):
             self.sel = self.choices.index(new_val)
         else:
-            raise('Exception: Unknown newval=%r' % new_val)
+            raise Exception('Exception: Unknown newval=%r' % new_val)
         if self.sel < 0 or self.sel > len(self.choices):
             raise Exception('self.sel=%r is not in the self.choices=%r '
                             % (self.sel, self.choices))
 
     def combo_val(self):
         return self.choices[self.sel]
```

### Comparing `utool-2.1.7/utool/Printable.py` & `utool-2.2.0/utool/Printable.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/__init__.py` & `utool-2.2.0/utool/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 pip install git+https://github.com/Erotemic/utool.git@next
 """
 # Utool is released under the Apache License Version 2.0
 
 import sys
 
-__version__ = '2.1.7'
+__version__ = '2.2.0'
 
 __DYNAMIC__ = True
 if __DYNAMIC__:
     __DYNAMIC__ = '--nodyn' not in sys.argv
 else:
     __DYNAMIC__ = '--dyn' in sys.argv
 # THESE COMMANDS WILL WRITE THE IMPORT FILE
```

### Comparing `utool-2.1.7/utool/_internal/meta_util_arg.py` & `utool-2.2.0/utool/_internal/meta_util_arg.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/_internal/meta_util_cache.py` & `utool-2.2.0/utool/_internal/meta_util_cache.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/_internal/meta_util_cplat.py` & `utool-2.2.0/utool/_internal/meta_util_cplat.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/_internal/meta_util_dbg.py` & `utool-2.2.0/utool/_internal/meta_util_dbg.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/_internal/meta_util_git.py` & `utool-2.2.0/utool/_internal/meta_util_git.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/_internal/meta_util_iter.py` & `utool-2.2.0/utool/_internal/meta_util_iter.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def ensure_iterable(obj):
     r"""
     Args:
         obj (scalar or iterable):
 
     Returns:
-        it3erable: obj if it was iterable otherwise [obj]
+        iterable: obj if it was iterable otherwise [obj]
 
     CommandLine:
         python -m utool._internal.meta_util_iter --test-ensure_iterable
 
     Timeit:
         %timeit ut.ensure_iterable([1])
         %timeit ut.ensure_iterable(1)
@@ -41,14 +41,16 @@
 
 
 def isiterable(obj):
     """
     Returns if the object can be iterated over and is NOT a string
     # TODO: implement isscalar similar to numpy
 
+    Use ubelt.iterable instead
+
     Args:
         obj (scalar or iterable):
 
     Returns:
         bool:
 
     CommandLine:
```

### Comparing `utool-2.1.7/utool/_internal/meta_util_path.py` & `utool-2.2.0/utool/_internal/meta_util_path.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/_internal/py2_syntax_funcs.py` & `utool-2.2.0/utool/_internal/py2_syntax_funcs.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/_internal/randomwrap.py` & `utool-2.2.0/utool/_internal/randomwrap.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/_internal/util_importer.py` & `utool-2.2.0/utool/_internal/util_importer.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/_internal/win32_send_keys.py` & `utool-2.2.0/utool/_internal/win32_send_keys.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/experimental/bytecode_optimizations.py` & `utool-2.2.0/utool/experimental/bytecode_optimizations.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/experimental/dynamic_connectivity.py` & `utool-2.2.0/utool/experimental/dynamic_connectivity.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/experimental/euler_tour_tree_avl.py` & `utool-2.2.0/utool/experimental/euler_tour_tree_avl.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/experimental/pandas_highlight.py` & `utool-2.2.0/utool/experimental/pandas_highlight.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/oldalg.py` & `utool-2.2.0/utool/oldalg.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/sandbox.py` & `utool-2.2.0/utool/sandbox.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_alg.py` & `utool-2.2.0/utool/util_alg.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_arg.py` & `utool-2.2.0/utool/util_arg.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_assert.py` & `utool-2.2.0/utool/util_assert.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_autogen.py` & `utool-2.2.0/utool/util_autogen.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_cache.py` & `utool-2.2.0/utool/util_cache.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_class.py` & `utool-2.2.0/utool/util_class.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_config.py` & `utool-2.2.0/utool/util_config.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_const.py` & `utool-2.2.0/utool/util_const.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_cplat.py` & `utool-2.2.0/utool/util_cplat.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 cross platform utilities
 """
 from __future__ import absolute_import, division, print_function, unicode_literals
 import os
-import pipes
 import six
 import sys
 import platform
 import subprocess
 import shlex
 from os.path import exists, normpath, basename, dirname, join, expanduser
 from utool import util_inject
@@ -467,21 +466,19 @@
 
     References:
         http://stackoverflow.com/questions/2692873/quote-posix-shell-special-characters-in-python-output
 
     """
     print('[cplat] startfile(%r)' % fpath)
     fpath = normpath(fpath)
-    # print('[cplat] fpath=%s' % fpath)
     if not exists(fpath):
         raise Exception('Cannot start nonexistant file: %r' % fpath)
-    #if quote:
-    #    fpath = '"%s"' % (fpath,)
     if not WIN32:
-        fpath = pipes.quote(fpath)
+        import shlex
+        fpath = shlex.quote(fpath)
     if LINUX:
         #out, err, ret = cmd(['xdg-open', fpath], detatch=True)
         outtup = cmd(('xdg-open', fpath), detatch=detatch, verbose=verbose, quiet=quiet)
         #outtup = cmd('xdg-open', fpath, detatch=detatch)
     elif DARWIN:
         outtup = cmd(('open', fpath), detatch=detatch, verbose=verbose, quiet=quiet)
     elif WIN32:
```

### Comparing `utool-2.1.7/utool/util_csv.py` & `utool-2.2.0/utool/util_csv.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_dbg.py` & `utool-2.2.0/utool/util_dbg.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_decor.py` & `utool-2.2.0/utool/util_decor.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,78 +70,72 @@
         #import sys
         #exc_type, exc_value, exc_traceback = sys.exc_info()
         #print(exc_traceback)
         # TODO: ensure decorators are not printed in stack trace
         ut.printex(ex, 'There is no error. This is a test', tb=True)
 
 
-if six.PY2:
-    # Use version that has special python2 only syntax.
-    # can not include it here for that reason
-    from utool._internal import py2_syntax_funcs
-    ignores_exc_tb = py2_syntax_funcs.ignores_exc_tb
-else:
-    def ignores_exc_tb(*args, **kwargs):
-        """
-        PYTHON 3 VERSION
-
-        ignore_exc_tb decorates a function and remove both itself
-        and the function from any exception traceback that occurs.
-
-        This is useful to decorate other trivial decorators
-        which are polluting your stacktrace.
-
-        if IGNORE_TRACEBACK is False then this decorator does nothing
-        (and it should do nothing in production code!)
-
-        References:
-            https://github.com/jcrocholl/pep8/issues/34  # NOQA
-            http://legacy.python.org/dev/peps/pep-3109/
-        """
-        outer_wrapper = kwargs.get('outer_wrapper', True)
-        def ignores_exc_tb_closure(func):
-            # HACK JUST TURN THIS OFF
-            return func
+def ignores_exc_tb(*args, **kwargs):
+    """
+    PYTHON 3 VERSION
 
-            if not IGNORE_TRACEBACK:
-                # if the global enforces that we should not ignore anytracebacks
-                # then just return the original function without any modifcation
-                return func
-            #@wraps(func)
-            def wrp_noexectb(*args, **kwargs):
+    ignore_exc_tb decorates a function and remove both itself
+    and the function from any exception traceback that occurs.
+
+    This is useful to decorate other trivial decorators
+    which are polluting your stacktrace.
+
+    if IGNORE_TRACEBACK is False then this decorator does nothing
+    (and it should do nothing in production code!)
+
+    References:
+        https://github.com/jcrocholl/pep8/issues/34  # NOQA
+        http://legacy.python.org/dev/peps/pep-3109/
+    """
+    outer_wrapper = kwargs.get('outer_wrapper', True)
+    def ignores_exc_tb_closure(func):
+        # HACK JUST TURN THIS OFF
+        return func
+
+        if not IGNORE_TRACEBACK:
+            # if the global enforces that we should not ignore anytracebacks
+            # then just return the original function without any modifcation
+            return func
+        #@wraps(func)
+        def wrp_noexectb(*args, **kwargs):
+            try:
+                #import utool
+                #if utool.DEBUG:
+                #    print('[IN IGNORETB] args=%r' % (args,))
+                #    print('[IN IGNORETB] kwargs=%r' % (kwargs,))
+                return func(*args, **kwargs)
+            except Exception:
+                # PYTHON 3.3 NEW METHODS
+                exc_type, exc_value, exc_traceback = sys.exc_info()
+                # Code to remove this decorator from traceback
+                # Remove two levels to remove this one as well
+                exc_type, exc_value, exc_traceback = sys.exc_info()
                 try:
-                    #import utool
-                    #if utool.DEBUG:
-                    #    print('[IN IGNORETB] args=%r' % (args,))
-                    #    print('[IN IGNORETB] kwargs=%r' % (kwargs,))
-                    return func(*args, **kwargs)
+                    exc_traceback = exc_traceback.tb_next
+                    exc_traceback = exc_traceback.tb_next
                 except Exception:
-                    # PYTHON 3.3 NEW METHODS
-                    exc_type, exc_value, exc_traceback = sys.exc_info()
-                    # Code to remove this decorator from traceback
-                    # Remove two levels to remove this one as well
-                    exc_type, exc_value, exc_traceback = sys.exc_info()
-                    try:
-                        exc_traceback = exc_traceback.tb_next
-                        exc_traceback = exc_traceback.tb_next
-                    except Exception:
-                        pass
-                    ex = exc_type(exc_value)
-                    ex.__traceback__ = exc_traceback
-                    raise ex
-            if outer_wrapper:
-                wrp_noexectb = preserve_sig(wrp_noexectb, func)
-            return wrp_noexectb
-        if len(args) == 1:
-            # called with one arg means its a function call
-            func = args[0]
-            return ignores_exc_tb_closure(func)
-        else:
-            # called with no args means kwargs as specified
-            return ignores_exc_tb_closure
+                    pass
+                ex = exc_type(exc_value)
+                ex.__traceback__ = exc_traceback
+                raise ex
+        if outer_wrapper:
+            wrp_noexectb = preserve_sig(wrp_noexectb, func)
+        return wrp_noexectb
+    if len(args) == 1:
+        # called with one arg means its a function call
+        func = args[0]
+        return ignores_exc_tb_closure(func)
+    else:
+        # called with no args means kwargs as specified
+        return ignores_exc_tb_closure
 
 
 # NEW PYTHON 2.7/3 VERSION
 #def ignores_exc_tb(*args, **kwargs):
 #    """
 #    ignore_exc_tb decorates a function and remove both itself
 #    and the function from any exception traceback that occurs.
@@ -674,85 +668,29 @@
         print(lbl + ' L___ EXIT ____')
         return ret
     return wrp_tracefunc
 
 
 def show_return_value(func):
     from utool.util_str import func_str
-    #@wraps(func)
     def wrp_show_return_value(*args, **kwargs):
         ret = func(*args, **kwargs)
-        #print('%s(*%r, **%r) returns %r' % (meta_util_six.get_funcname(func), args, kwargs, rv))
         print(func_str(func, args, kwargs)  + ' -> ret=%r' % (ret,))
         return ret
     return wrp_show_return_value
 
 
 def time_func(func):
-    #@wraps(func)
     def wrp_time(*args, **kwargs):
         with util_time.Timer(meta_util_six.get_funcname(func)):
             return func(*args, **kwargs)
     wrp_time = preserve_sig(wrp_time, func)
     return wrp_time
 
 
-#def rename_func(newname):
-#    import utool as ut
-#    return ut.partial(ut.set_funcname, newname=newname)
-
-
-#class copy_argspec(object):
-#    """
-#    copy_argspec is a signature modifying decorator.
-#    Specifically, it copies the signature from `source_func` to the wrapper, and
-#    the wrapper will call the original function (which should be using *args,
-#    **kwds).  The argspec, docstring, and default values are copied from
-#    src_func, and __module__ and __dict__ from tgt_func.
-#    .. References
-#    http://stackoverflow.com/questions/18625510/how-can-i-programmatically-change-the-argspec-of-a-function-not-in-a-python-de
-#    """
-#    def __init__(self, src_func):
-#        self.argspec = inspect.getargspec(src_func)
-#        self.src_doc = src_func.__doc__
-#        self.src_defaults = src_func.func_defaults
-#    def __call__(self, tgt_func):
-#        try:
-#            tgt_argspec = inspect.getargspec(tgt_func)
-#            need_self = False
-#            if len(tgt_argspec) > 0 and len(tgt_argspec[0]) > 0 and tgt_argspec[0][0] == 'self':
-#                need_self = True
-#            name = tgt_func.__name__
-#            argspec = self.argspec
-#            if len(argspec) > 0 and len(argspec[0]) > 0 and argspec[0][0] == 'self':
-#                need_self = False
-#            if need_self:
-#                newargspec = (['self'] + argspec[0],) + argspec[1:]
-#            else:
-#                newargspec = argspec
-#            signature = inspect.formatargspec(formatvalue=lambda val: "",
-#                                              *newargspec)[1:-1]
-#            new_func = (
-#                'def _wrapper_({signature}):\n'
-#                '    return {tgt_func}({signature})'
-#            ).format(signature=signature, tgt_func='tgt_func')
-#            evaldict = {'tgt_func' : tgt_func}
-#            exec new_func in evaldict
-#            wrapped = evaldict['_wrapper_']
-#            wrapped.__name__ = name
-#            wrapped.__doc__ = self.src_doc
-#            wrapped.func_defaults = self.src_defaults
-#            wrapped.__module__ = tgt_func.__module__
-#            wrapped.__dict__ = tgt_func.__dict__
-#            return wrapped
-#        except Exception as ex:
-#            util_dbg.printex(ex, 'error wrapping: %r' % (tgt_func,))
-#            raise
-
-
 def lazyfunc(func):
     """
     Returns a memcached version of a function
     """
     closuremem_ = [{}]
     def wrapper(*args, **kwargs):
         mem = closuremem_[0]
@@ -831,15 +769,15 @@
 
     if wrapper is orig_func:
         # nothing to do
         return orig_func
     orig_docstr = meta_util_six.get_funcdoc(orig_func)
     orig_docstr = '' if orig_docstr is None else orig_docstr
     orig_argspec = util_inspect.get_func_argspec(orig_func)
-    wrap_name = meta_util_six.get_funccode(wrapper).co_name
+    wrap_name = wrapper.__code__.co_name
     orig_name = meta_util_six.get_funcname(orig_func)
 
     # At the very least preserve info in a dictionary
     _utinfo = {}
     _utinfo['orig_func'] = orig_func
     _utinfo['wrap_name'] = wrap_name
     _utinfo['orig_name'] = orig_name
@@ -921,15 +859,15 @@
             '''
             {orig_docstr}
             '''
         )
     new_docstr = new_docstr_fmtstr.format(
         wrap_name=wrap_name, orig_name=orig_name, orig_docstr=orig_docstr,
         orig_argspec=orig_argspec)
-    meta_util_six.set_funcdoc(_wrp_preserve, new_docstr)
+    _wrp_preserve.__doc__ = new_docstr
     _wrp_preserve._utinfo = _utinfo
     return _wrp_preserve
 
 
 def dummy_args_decor(*args, **kwargs):
     def dummy_args_closure(func):
         return func
```

### Comparing `utool-2.1.7/utool/util_depricated.py` & `utool-2.2.0/utool/util_depricated.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_dev.py` & `utool-2.2.0/utool/util_dev.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_dict.py` & `utool-2.2.0/utool/util_dict.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_func.py` & `utool-2.2.0/utool/util_func.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_git.py` & `utool-2.2.0/utool/util_git.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_grabdata.py` & `utool-2.2.0/utool/util_grabdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -509,16 +509,15 @@
 
 
 TESTIMG_URL_DICT = {
     'grace.jpg' : 'http://i.imgur.com/rgQyu7r.jpg',
     'jeff.png'  : 'http://i.imgur.com/l00rECD.png',
     'ada2.jpg'  : 'http://i.imgur.com/zHOpTCb.jpg',
     'ada.jpg'   : 'http://i.imgur.com/iXNf4Me.jpg',
-    'lena.png'  : 'http://i.imgur.com/JGrqMnV.png',  # depricate lena
-    'astro.png' : 'https://i.imgur.com/KXhKM72.png',  # Use instead of lena
+    'astro.png' : 'https://i.imgur.com/KXhKM72.png',
     'carl.jpg'  : 'http://i.imgur.com/flTHWFD.jpg',
     'easy1.png' : 'http://i.imgur.com/Qqd0VNq.png',
     'easy2.png' : 'http://i.imgur.com/BDP8MIu.png',
     'easy3.png' : 'http://i.imgur.com/zBcm5mS.png',
     'hard3.png' : 'http://i.imgur.com/ST91yBf.png',
     'zebra.png' : 'http://i.imgur.com/58hbGcd.png',
     'star.png'  : 'http://i.imgur.com/d2FHuIU.png',
@@ -547,21 +546,21 @@
     import utool as ut
     download_dir = util_cplat.get_app_cache_dir('utool')
     for key in TESTIMG_URL_DICT:
         fpath = join(download_dir, key)
         ut.delete(fpath)
 
 
-def grab_test_imgpath(key='lena.png', allow_external=True, verbose=True):
+def grab_test_imgpath(key='astro.png', allow_external=True, verbose=True):
     r"""
     Gets paths to standard / fun test images.
     Downloads them if they dont exits
 
     Args:
-        key (str): one of the standard test images, e.g. lena.png, carl.jpg, ...
+        key (str): one of the standard test images, e.g. astro.png, carl.jpg, ...
         allow_external (bool): if True you can specify existing fpaths
 
     Returns:
         str: testimg_fpath - filepath to the downloaded or cached test image.
 
     SeeAlso:
         ut.get_valid_test_imgkeys
@@ -576,26 +575,39 @@
         >>> # build test data
         >>> key = 'carl.jpg'
         >>> # execute function
         >>> testimg_fpath = grab_test_imgpath(key)
         >>> # verify results
         >>> ut.assertpath(testimg_fpath)
     """
-    if allow_external and key not in TESTIMG_URL_DICT:
-        testimg_fpath = key
-        if not util_path.checkpath(testimg_fpath, verbose=True):
-            import utool as ut
-            raise AssertionError(
-                'testimg_fpath=%r not found did you mean %s' % (
-                    testimg_fpath,
-                    ut.conj_phrase(get_valid_test_imgkeys(), 'or')))
-    else:
-        testimg_fname = key
-        testimg_url = TESTIMG_URL_DICT[key]
-        testimg_fpath = grab_file_url(testimg_url, fname=testimg_fname, verbose=verbose)
+    try:
+        # Original utool implementation
+        if allow_external and key not in TESTIMG_URL_DICT:
+            testimg_fpath = key
+            if not util_path.checkpath(testimg_fpath, verbose=True):
+                import utool as ut
+                raise AssertionError(
+                    'testimg_fpath=%r not found did you mean %s' % (
+                        testimg_fpath,
+                        ut.conj_phrase(get_valid_test_imgkeys(), 'or')))
+        else:
+            testimg_fname = key
+            # raise Exception
+            testimg_url = TESTIMG_URL_DICT[key]
+            testimg_fpath = grab_file_url(testimg_url, fname=testimg_fname, verbose=verbose)
+    except Exception:
+        # Use the kwimage implementation if utool fails
+        from utool import _kwimage_im_demodata
+        import os
+        if key == 'carl.jpg':
+            key = 'carl'
+        elif key == 'astro.png':
+            key = 'astro'
+        testimg_fpath = _kwimage_im_demodata.grab_test_image_fpath(key)
+        testimg_fpath = os.fspath(testimg_fpath)
     return testimg_fpath
 
 
 def grab_selenium_chromedriver(redownload=False):
     r"""
     Automatically download selenium chrome driver if needed
 
@@ -787,20 +799,20 @@
         >>> # ENABLE_DOCTEST
         >>> from utool.util_grabdata import *  # NOQA
         >>> import utool as ut  # NOQA
         >>> from os.path import basename
         >>> ut.exec_funckw(ut.grab_file_url, locals())
         >>> file_url = 'http://i.imgur.com/JGrqMnV.png'
         >>> redownload = True
-        >>> fname = 'lena.png'
-        >>> lena_fpath = ut.grab_file_url(file_url, fname=fname,
+        >>> fname = 'astro.png'
+        >>> astro_fpath = ut.grab_file_url(file_url, fname=fname,
         >>>                               redownload=redownload)
-        >>> result = basename(lena_fpath)
+        >>> result = basename(astro_fpath)
         >>> print(result)
-        lena.png
+        astro.png
 
     Ignore:
         >>> # ENABLE_DOCTEST
         >>> from utool.util_grabdata import *  # NOQA
         >>> import utool as ut  # NOQA
         >>> ut.exec_funckw(ut.grab_file_url, locals())
         >>> file_url = 'https://lev.cs.rpi.edu/public/models/detect.yolo.12.classes'
```

### Comparing `utool-2.1.7/utool/util_graph.py` & `utool-2.2.0/utool/util_graph.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_gridsearch.py` & `utool-2.2.0/utool/util_gridsearch.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_hash.py` & `utool-2.2.0/utool/util_hash.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_import.py` & `utool-2.2.0/utool/util_import.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_inject.py` & `utool-2.2.0/utool/util_inject.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_inspect.py` & `utool-2.2.0/utool/util_inspect.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_io.py` & `utool-2.2.0/utool/util_io.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_ipynb.py` & `utool-2.2.0/utool/util_ipynb.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_iter.py` & `utool-2.2.0/utool/util_iter.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_latex.py` & `utool-2.2.0/utool/util_latex.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_list.py` & `utool-2.2.0/utool/util_list.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_logging.py` & `utool-2.2.0/utool/util_logging.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_num.py` & `utool-2.2.0/utool/util_num.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_numpy.py` & `utool-2.2.0/utool/util_numpy.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_parallel.py` & `utool-2.2.0/utool/util_parallel.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_path.py` & `utool-2.2.0/utool/util_path.py`

 * *Files 0% similar despite different names*

```diff
@@ -1002,15 +1002,14 @@
         >>> result = ('path_list = %s' % (ut.repr3(path_list),))
         >>> result = result.replace(r'\\', '/')
         >>> # xdoctest: +REQUIRES(POSIX)
         >>> print(result)
         path_list = [
             '__init__.py',
             '__main__.py',
-            'tests/__init__.py',
         ]
 
     Example:
         >>> # DISABLE_DOCTEST
         >>> from utool.util_path import *  # NOQA
         >>> import utool as ut
         >>> dpath = dirname(ut.__file__) + '/__*.py'
```

### Comparing `utool-2.1.7/utool/util_print.py` & `utool-2.2.0/utool/util_print.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_profile.py` & `utool-2.2.0/utool/util_profile.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_progress.py` & `utool-2.2.0/utool/util_progress.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_project.py` & `utool-2.2.0/utool/util_project.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_regex.py` & `utool-2.2.0/utool/util_regex.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_resources.py` & `utool-2.2.0/utool/util_resources.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_set.py` & `utool-2.2.0/utool/util_set.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_setup.py` & `utool-2.2.0/utool/util_setup.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_sqlite.py` & `utool-2.2.0/utool/util_sqlite.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_str.py` & `utool-2.2.0/utool/util_str.py`

 * *Files 0% similar despite different names*

```diff
@@ -2562,27 +2562,30 @@
     Args:
         font (str): default=cybermedium, other fonts include: cybersmall and
             cyberlarge.
 
     References:
         http://www.figlet.org/
 
+    CommandLine:
+        xdoctest -m utool.util_str bubbletext
+
     Example:
         >>> # ENABLE_DOCTEST
         >>> import utool as ut
         >>> bubble_text = ut.bubbletext('TESTING BUBBLE TEXT', font='cybermedium')
         >>> print(bubble_text)
     """
-    import utool as ut
-    pyfiglet = ut.tryimport('pyfiglet', 'git+https://github.com/pwaller/pyfiglet')
-    if pyfiglet is None:
-        return text
-    else:
+    try:
+        import pyfiglet
         bubble_text = pyfiglet.figlet_format(text, font=font)
         return bubble_text
+    except Exception:
+        # On any issue, import or font based, just return regular text
+        return text
 
 
 def closet_words(query, options, num=1, subset=False):
     import utool as ut
     ranked_list = []
     if subset:
         query_ = query.lower()
```

### Comparing `utool-2.1.7/utool/util_sysreq.py` & `utool-2.2.0/utool/util_sysreq.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_tags.py` & `utool-2.2.0/utool/util_tags.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_tests.py` & `utool-2.2.0/utool/util_tests.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_time.py` & `utool-2.2.0/utool/util_time.py`

 * *Files 4% similar despite different names*

```diff
@@ -267,76 +267,21 @@
         >>> for _ in ut.Timerit(num, 'inprecise'):
         >>>     ut.get_nth_prime_bruteforce(n)
         >>> # Using the timer object results in the most precise timeings
         >>> for timer in ut.Timerit(num, 'precise'):
         >>>     with timer:
         >>>         ut.get_nth_prime_bruteforce(n)
     """
-    ...
-    # def __init__(self, num, label=None, unit=None, verbose=1):
-    #     self.num = num
-    #     self.label = label
-    #     self.times = []
-    #     self.verbose = verbose
-    #     self.total_time = None
-    #     self.n_loops = None
-    #     self.unit = unit
-
-    # def __iter__(self):
-    #     import utool as ut
-    #     if self.verbose > 1:
-    #         if self.label is None:
-    #             print('Timing for %d loops' % self.num)
-    #         else:
-    #             print('Timing %s for %d loops.' % (self.label, self.num,))
-    #     self.n_loops = 0
-    #     self.total_time = 0
-    #     # Create a foreground and background timer
-    #     bg_timer = ut.Timer(verbose=0)   # (ideally this is unused)
-    #     fg_timer = ut.Timer(verbose=0)   # (used directly by user)
-    #     # Core timing loop
-    #     for i in range(self.num):
-    #         # Start background timer (in case the user doesnt use fg_timer)
-    #         # Yield foreground timer to let the user run a block of code
-    #         # When we return from yield the user code will have just finishec
-    #         # Then record background time + loop overhead
-    #         bg_timer.tic()
-    #         yield fg_timer
-    #         bg_time = bg_timer.toc()
-    #         # Check if the fg_timer object was used, but fallback on bg_timer
-    #         if fg_timer.ellapsed >= 0:
-    #             block_time = fg_timer.ellapsed  # high precision
-    #         else:
-    #             block_time = bg_time  # low precision
-    #         # record timeings
-    #         self.times.append(block_time)
-    #         self.total_time += block_time
-    #         self.n_loops += 1
-    #     # Timeing complete, print results
-    #     assert len(self.times) == self.num, 'incorrectly recorded times'
-    #     if self.verbose > 0:
-    #         self._print_report(self.verbose)
-
-    # @property
-    # def ave_secs(self):
-    #     return self.total_time / self.n_loops
-
-    # def _print_report(self, verbose=1):
-    #     import utool as ut
-    #     ave_secs = self.ave_secs
-    #     if self.label is None:
-    #         print('Timing complete, %d loops' % (self.n_loops,))
-    #     else:
-    #         print('Timing complete for: %s, %d loops' % (self.label,
-    #                                                      self.n_loops))
-    #     if verbose > 2:
-    #         body = ut.second_str(self.total_time, unit=self.unit, precision=4)
-    #         print('    body took: %s' % body)
-    #     perloop = ut.second_str(ave_secs, unit=self.unit, precision=4)
-    #     print('    time per loop : %s' % (perloop,))
+    @property
+    def ave_secs(self):
+        return self.mean()
+        # return self.total_time / self.n_loops
+
+    def _print_report(self, verbose=1):
+        self.print(verbose=verbose)
 
 
 def determine_timestamp_format(datetime_str, warn=True):
     r"""
     Args:
         datetime_str (str):
 
@@ -524,18 +469,14 @@
         timestamp_ = timestamp[:19].strip(';').strip()
         utc_offset = timestamp[19:]
     else:
         timestamp_ = timestamp
 
     dt_ = datetime.datetime.strptime(timestamp_, timefmt)
     if use_delorean:
-        #if utc and utc_offset is not None:
-        #if utc:
-        #    dn_ = delorean.Delorean(dt_, 'UTC')
-        #else:
         if zone is None:
             zone = time.tzname[0]
         if zone == 'local':
             zone = time.tzname[0]
         dn_ = delorean.Delorean(dt_, zone)
     else:
         dn_ = dt_
```

### Comparing `utool-2.1.7/utool/util_type.py` & `utool-2.2.0/utool/util_type.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_ubuntu.py` & `utool-2.2.0/utool/util_ubuntu.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_web.py` & `utool-2.2.0/utool/util_web.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool/util_win32.py` & `utool-2.2.0/utool/util_win32.py`

 * *Files identical despite different names*

### Comparing `utool-2.1.7/utool.egg-info/SOURCES.txt` & `utool-2.2.0/utool.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 LICENSE
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
+tests/test_import.py
 utool/DynamicStruct.py
 utool/Preferences.py
 utool/Printable.py
 utool/__init__.py
 utool/__main__.py
+utool/_kwimage_im_demodata.py
 utool/oldalg.py
 utool/sandbox.py
 utool/util_alg.py
 utool/util_aliases.py
 utool/util_arg.py
 utool/util_assert.py
 utool/util_autogen.py
@@ -83,14 +85,8 @@
 utool/_internal/randomwrap.py
 utool/_internal/util_importer.py
 utool/_internal/win32_send_keys.py
 utool/experimental/__init__.py
 utool/experimental/bytecode_optimizations.py
 utool/experimental/dynamic_connectivity.py
 utool/experimental/euler_tour_tree_avl.py
-utool/experimental/pandas_highlight.py
-utool/tests/__init__.py
-utool/tests/_oldtest_decor.py
-utool/tests/_oldtest_hash.py
-utool/tests/_oldtest_logging.py
-utool/tests/_oldtest_reloading.py
-utool/tests/run_tests.py
+utool/experimental/pandas_highlight.py
```

### Comparing `utool-2.1.7/utool.egg-info/requires.txt` & `utool-2.2.0/utool.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,530 +1,580 @@
-delorean
-parse
-pyparsing
-requests
-six
-timerit
+six>=1.10.0
+parse>=1.6.6
+requests>=2.27.1
+pyparsing>=3.0.7
+delorean>=1.0.0
+timerit>=1.0.1
 
 [:python_version < "2.7" and python_version >= "2.6"]
-gitpython
+gitpython>=2.1.8
 
 [:python_version < "3.0"]
-futures
-lockfile
+lockfile>=0.10.2
+futures>=1.0.0
 
 [:python_version < "3.0" and python_version >= "2.7"]
-gitpython
+gitpython>=2.1.4
 
 [:python_version < "3.10" and python_version >= "3.9"]
-numpy
-pandas
+numpy>=1.19.3
+pandas>=1.4.0
 
 [:python_version < "3.11" and python_version >= "3.10"]
-numpy
-pandas
+numpy>=1.21.6
+pandas>=1.3.5
 
 [:python_version < "3.4" and python_version >= "2.7"]
-numpy
-pandas
+numpy>=1.11.1
+pandas>=0.20.1
 
 [:python_version < "3.4" and python_version >= "3.0"]
-gitpython
+gitpython>=2.1.12
 
 [:python_version < "3.5" and python_version >= "2.7"]
-networkx
+networkx>=1.11
 
 [:python_version < "3.5" and python_version >= "3.4"]
-numpy
-pandas
+numpy>=1.11.1
+pandas>=0.18.1
 
 [:python_version < "3.5.3" and python_version >= "3.5"]
-pandas
+pandas>=0.18.1
 
 [:python_version < "3.6" and python_version >= "2.7"]
-ubelt
+ubelt>=0.8.1
 
 [:python_version < "3.6" and python_version >= "3.4"]
-gitpython
+gitpython>=3.0.7
 
 [:python_version < "3.6" and python_version >= "3.5"]
-networkx
-numpy
+numpy>=1.11.1
+networkx>=2.3
 
 [:python_version < "3.6" and python_version >= "3.5.3"]
-pandas
+pandas>=0.25.0
 
 [:python_version < "3.6.1" and python_version >= "3.6"]
-pandas
+pandas>=0.20.3
 
 [:python_version < "3.7" and python_version >= "3.6"]
-gitpython
-networkx
-numpy
+numpy>=1.12.0
+gitpython>=3.1.18
+networkx>=2.5
 
 [:python_version < "3.7" and python_version >= "3.6.1"]
-pandas
+pandas>=1.0.0
 
 [:python_version < "3.7.1" and python_version >= "3.7"]
-pandas
+pandas>=1.1.3
 
 [:python_version < "3.8" and python_version >= "3.7"]
-networkx
-numpy
+numpy>=1.14.5
+networkx>=2.6.2
 
 [:python_version < "3.8" and python_version >= "3.7.1"]
-pandas
+pandas>=1.2.0
 
 [:python_version < "3.9" and python_version >= "3.8"]
-numpy
-pandas
+numpy>=1.19.2
+pandas>=1.4.0
 
 [:python_version < "4.0" and python_version >= "3.11"]
-numpy
-pandas
+numpy>=1.24.0
+pandas>=1.5.0
 
 [:python_version >= "3.6"]
-ubelt
+ubelt>=1.0.0
 
 [:python_version >= "3.7"]
-gitpython
+gitpython>=3.1.24
 
 [:python_version >= "3.8"]
-networkx
+networkx>=2.7
 
 [all]
-Pygments
-astor
-autopep8
-boto
-codecov
-delorean
-objgraph
-parse
-pint
-pyfiglet
-pyparsing
-pyperclip
-pytest-timeout
-requests
-setproctitle
-six
-sphinx
-timerit
-xdoctest
+six>=1.10.0
+parse>=1.6.6
+requests>=2.27.1
+pyparsing>=3.0.7
+delorean>=1.0.0
+timerit>=1.0.1
+xdoctest>=1.1.3
+pytest-timeout>=1.4.2
+Pygments>=2.2.0
+autopep8>=1.6.0
+astor>=0.8.1
+pyperclip>=1.5.7
+pyfiglet>=0.7.2
+boto>=2.49.0
+sphinx>=5.0.1
+setproctitle>=1.2.3
+objgraph>=3.5.0
+pint>=0.18
 
 [all-strict]
+six==1.10.0
+parse==1.6.6
+requests==2.27.1
+pyparsing==3.0.7
+delorean==1.0.0
+timerit==1.0.1
+xdoctest==1.1.3
+pytest-timeout==1.4.2
 Pygments==2.2.0
-astor==0.8.1
 autopep8==1.6.0
+astor==0.8.1
+pyperclip==1.5.7
+pyfiglet==0.7.2
 boto==2.49.0
-codecov==2.0.15
-delorean==1.0.0
+sphinx==5.0.1
+setproctitle==1.2.3
 objgraph==3.5.0
-parse==1.6.6
 pint==0.18
-pyfiglet==0.7.2
-pyparsing==3.0.7
-pyperclip==1.5.7
-pytest-timeout==1.4.2
-requests==2.27.1
-setproctitle==1.2.3
-six==1.10.0
-sphinx==5.0.1
-timerit==1.0.1
-xdoctest==0.14.0
 
 [all-strict:python_version < "2.7" and python_version >= "2.6"]
-coverage==4.5
 gitpython==2.1.8
+coverage==4.5
 
 [all-strict:python_version < "2.8.0" and python_version >= "2.7.0"]
-pytest-cov==2.8.1
 pytest<=4.6.11,==4.6.0
+pytest-cov==2.8.1
 
 [all-strict:python_version < "3.0"]
-futures==1.0.0
 lockfile==0.10.2
+futures==1.0.0
 
 [all-strict:python_version < "3.0" and python_version >= "2.7"]
 gitpython==2.1.4
 
 [all-strict:python_version < "3.10" and python_version >= "3.9"]
-coverage==5.3.1
-h5py==3.7.0
-lru-dict==1.1.8
 numpy==1.19.3
 pandas==1.4.0
+pytest==8.1.1
+coverage==5.3.1
 xxhash==2.0.2
-
-[all-strict:python_version < "3.10.0" and python_version >= "3.7.0"]
-pytest==4.6.0
+lru-dict==1.1.8
+h5py==3.7.0
 
 [all-strict:python_version < "3.11" and python_version >= "3.10"]
-h5py==3.7.0
 numpy==1.21.6
 pandas==1.3.5
+pytest==8.1.1
 xxhash==3.0.0
+h5py==3.7.0
+
+[all-strict:python_version < "3.12" and python_version >= "3.11"]
+pytest==8.1.1
+xxhash==3.2.0
+h5py==3.8.0
+
+[all-strict:python_version < "3.13" and python_version >= "3.12"]
+pytest==8.1.1
 
 [all-strict:python_version < "3.4" and python_version >= "2.7"]
-coverage==5.3.1
 numpy==1.11.1
 pandas==0.20.1
+coverage==5.3.1
 
 [all-strict:python_version < "3.4" and python_version >= "3.0"]
 gitpython==2.1.12
 
 [all-strict:python_version < "3.5" and python_version >= "2.7"]
 networkx==1.11
 
 [all-strict:python_version < "3.5" and python_version >= "3.4"]
-coverage==4.3.4
 numpy==1.11.1
 pandas==0.18.1
+coverage==4.3.4
 
 [all-strict:python_version < "3.5.0" and python_version >= "3.4.0"]
-pytest-cov==2.8.1
 pytest<=4.6.11,==4.6.0
+pytest-cov==2.8.1
 
 [all-strict:python_version < "3.5.3" and python_version >= "3.5"]
 pandas==0.18.1
 
 [all-strict:python_version < "3.6" and python_version >= "2.7"]
 ubelt==0.8.1
 
 [all-strict:python_version < "3.6" and python_version >= "3.4"]
 gitpython==3.0.7
 
 [all-strict:python_version < "3.6" and python_version >= "3.5"]
+numpy==1.11.1
+networkx==2.3
 coverage==5.3.1
 h5py==3.7.0
-networkx==2.3
-numpy==1.11.1
 
 [all-strict:python_version < "3.6" and python_version >= "3.5.3"]
 pandas==0.25.0
 
 [all-strict:python_version < "3.6.0" and python_version >= "3.5.0"]
-pytest-cov==2.9.0
 pytest<=6.1.2,==4.6.0
+pytest-cov==2.9.0
 
 [all-strict:python_version < "3.6.1" and python_version >= "3.6"]
 pandas==0.20.3
 
 [all-strict:python_version < "3.7" and python_version >= "3.6"]
-coverage==6.1.1
+numpy==1.12.0
 gitpython==3.1.18
-h5py==3.7.0
-lru-dict==1.1.8
 networkx==2.5
-numpy==1.12.0
+coverage==6.1.1
 xxhash==1.3.0
+lru-dict==1.1.8
+h5py==3.7.0
 
 [all-strict:python_version < "3.7" and python_version >= "3.6.1"]
 pandas==1.0.0
 
-[all-strict:python_version < "3.7.0" and python_version >= "3.6.0"]
-pytest==4.6.0
-
 [all-strict:python_version < "3.7.1" and python_version >= "3.7"]
 pandas==1.1.3
 
 [all-strict:python_version < "3.8" and python_version >= "3.7"]
-coverage==6.1.1
-h5py==3.7.0
-lru-dict==1.1.8
-networkx==2.6.2
 numpy==1.14.5
+networkx==2.6.2
+pytest==4.6.0
+coverage==6.1.1
 xxhash==1.3.0
+lru-dict==1.1.8
+h5py==3.7.0
 
 [all-strict:python_version < "3.8" and python_version >= "3.7.1"]
 pandas==1.2.0
 
 [all-strict:python_version < "3.9" and python_version >= "3.8"]
-coverage==6.1.1
-h5py==3.7.0
-lru-dict==1.1.8
 numpy==1.19.2
 pandas==1.4.0
+pytest==8.1.1
+coverage==6.1.1
 xxhash==1.4.3
+lru-dict==1.1.8
+h5py==3.7.0
 
 [all-strict:python_version < "4.0" and python_version >= "3.10"]
 lru-dict==1.1.8
 
 [all-strict:python_version < "4.0" and python_version >= "3.11"]
-h5py==3.8.0
 numpy==1.24.0
 pandas==1.5.0
-xxhash==3.0.0
+
+[all-strict:python_version < "4.0" and python_version >= "3.12"]
+xxhash==3.4.1
+h5py==3.10.0
+
+[all-strict:python_version < "4.0" and python_version >= "3.13"]
+pytest==8.1.1
 
 [all-strict:python_version >= "3.10"]
 coverage==6.1.1
 
-[all-strict:python_version >= "3.10.0"]
-pytest==6.2.5
-
 [all-strict:python_version >= "3.6"]
 ubelt==1.0.0
 
 [all-strict:python_version >= "3.6.0"]
 pytest-cov==3.0.0
 
 [all-strict:python_version >= "3.7"]
 gitpython==3.1.24
 
 [all-strict:python_version >= "3.8"]
 networkx==2.7
 
 [all:python_version < "2.7" and python_version >= "2.6"]
-coverage
-gitpython
+gitpython>=2.1.8
+coverage>=4.5
 
 [all:python_version < "2.8.0" and python_version >= "2.7.0"]
-pytest
-pytest-cov
+pytest<=4.6.11,>=4.6.0
+pytest-cov>=2.8.1
 
 [all:python_version < "3.0"]
-futures
-lockfile
+lockfile>=0.10.2
+futures>=1.0.0
 
 [all:python_version < "3.0" and python_version >= "2.7"]
-gitpython
+gitpython>=2.1.4
 
 [all:python_version < "3.10" and python_version >= "3.9"]
-coverage
-h5py
-lru-dict
-numpy
-pandas
-xxhash
-
-[all:python_version < "3.10.0" and python_version >= "3.7.0"]
-pytest
+numpy>=1.19.3
+pandas>=1.4.0
+pytest>=8.1.1
+coverage>=5.3.1
+xxhash>=2.0.2
+lru-dict>=1.1.8
+h5py>=3.7.0
 
 [all:python_version < "3.11" and python_version >= "3.10"]
-h5py
-numpy
-pandas
-xxhash
+numpy>=1.21.6
+pandas>=1.3.5
+pytest>=8.1.1
+xxhash>=3.0.0
+h5py>=3.7.0
+
+[all:python_version < "3.12" and python_version >= "3.11"]
+pytest>=8.1.1
+xxhash>=3.2.0
+h5py>=3.8.0
+
+[all:python_version < "3.13" and python_version >= "3.12"]
+pytest>=8.1.1
 
 [all:python_version < "3.4" and python_version >= "2.7"]
-coverage
-numpy
-pandas
+numpy>=1.11.1
+pandas>=0.20.1
+coverage>=5.3.1
 
 [all:python_version < "3.4" and python_version >= "3.0"]
-gitpython
+gitpython>=2.1.12
 
 [all:python_version < "3.5" and python_version >= "2.7"]
-networkx
+networkx>=1.11
 
 [all:python_version < "3.5" and python_version >= "3.4"]
-coverage
-numpy
-pandas
+numpy>=1.11.1
+pandas>=0.18.1
+coverage>=4.3.4
 
 [all:python_version < "3.5.0" and python_version >= "3.4.0"]
-pytest
-pytest-cov
+pytest<=4.6.11,>=4.6.0
+pytest-cov>=2.8.1
 
 [all:python_version < "3.5.3" and python_version >= "3.5"]
-pandas
+pandas>=0.18.1
 
 [all:python_version < "3.6" and python_version >= "2.7"]
-ubelt
+ubelt>=0.8.1
 
 [all:python_version < "3.6" and python_version >= "3.4"]
-gitpython
+gitpython>=3.0.7
 
 [all:python_version < "3.6" and python_version >= "3.5"]
-coverage
-h5py
-networkx
-numpy
+numpy>=1.11.1
+networkx>=2.3
+coverage>=5.3.1
+h5py>=3.7.0
 
 [all:python_version < "3.6" and python_version >= "3.5.3"]
-pandas
+pandas>=0.25.0
 
 [all:python_version < "3.6.0" and python_version >= "3.5.0"]
-pytest
-pytest-cov
+pytest<=6.1.2,>=4.6.0
+pytest-cov>=2.9.0
 
 [all:python_version < "3.6.1" and python_version >= "3.6"]
-pandas
+pandas>=0.20.3
 
 [all:python_version < "3.7" and python_version >= "3.6"]
-coverage
-gitpython
-h5py
-lru-dict
-networkx
-numpy
-xxhash
+numpy>=1.12.0
+gitpython>=3.1.18
+networkx>=2.5
+coverage>=6.1.1
+xxhash>=1.3.0
+lru-dict>=1.1.8
+h5py>=3.7.0
 
 [all:python_version < "3.7" and python_version >= "3.6.1"]
-pandas
-
-[all:python_version < "3.7.0" and python_version >= "3.6.0"]
-pytest
+pandas>=1.0.0
 
 [all:python_version < "3.7.1" and python_version >= "3.7"]
-pandas
+pandas>=1.1.3
 
 [all:python_version < "3.8" and python_version >= "3.7"]
-coverage
-h5py
-lru-dict
-networkx
-numpy
-xxhash
+numpy>=1.14.5
+networkx>=2.6.2
+pytest>=4.6.0
+coverage>=6.1.1
+xxhash>=1.3.0
+lru-dict>=1.1.8
+h5py>=3.7.0
 
 [all:python_version < "3.8" and python_version >= "3.7.1"]
-pandas
+pandas>=1.2.0
 
 [all:python_version < "3.9" and python_version >= "3.8"]
-coverage
-h5py
-lru-dict
-numpy
-pandas
-xxhash
+numpy>=1.19.2
+pandas>=1.4.0
+pytest>=8.1.1
+coverage>=6.1.1
+xxhash>=1.4.3
+lru-dict>=1.1.8
+h5py>=3.7.0
 
 [all:python_version < "4.0" and python_version >= "3.10"]
-lru-dict
+lru-dict>=1.1.8
 
 [all:python_version < "4.0" and python_version >= "3.11"]
-h5py
-numpy
-pandas
-xxhash
+numpy>=1.24.0
+pandas>=1.5.0
 
-[all:python_version >= "3.10"]
-coverage
+[all:python_version < "4.0" and python_version >= "3.12"]
+xxhash>=3.4.1
+h5py>=3.10.0
+
+[all:python_version < "4.0" and python_version >= "3.13"]
+pytest>=8.1.1
 
-[all:python_version >= "3.10.0"]
-pytest
+[all:python_version >= "3.10"]
+coverage>=6.1.1
 
 [all:python_version >= "3.6"]
-ubelt
+ubelt>=1.0.0
 
 [all:python_version >= "3.6.0"]
-pytest-cov
+pytest-cov>=3.0.0
 
 [all:python_version >= "3.7"]
-gitpython
+gitpython>=3.1.24
 
 [all:python_version >= "3.8"]
-networkx
+networkx>=2.7
+
+[docs]
+sphinx>=5.0.1
+sphinx-autobuild>=2021.3.14
+sphinx_rtd_theme>=1.0.0
+sphinxcontrib-napoleon>=0.7
+sphinx-autoapi>=1.8.4
+Pygments>=2.9.0
+myst_parser>=0.16.1
+sphinx-reredirects>=0.0.1
+
+[docs-strict]
+sphinx==5.0.1
+sphinx-autobuild==2021.3.14
+sphinx_rtd_theme==1.0.0
+sphinxcontrib-napoleon==0.7
+sphinx-autoapi==1.8.4
+Pygments==2.9.0
+myst_parser==0.16.1
+sphinx-reredirects==0.0.1
 
 [optional]
-Pygments
-astor
-autopep8
-boto
-objgraph
-pint
-pyfiglet
-pyperclip
-setproctitle
-sphinx
+Pygments>=2.2.0
+autopep8>=1.6.0
+astor>=0.8.1
+pyperclip>=1.5.7
+pyfiglet>=0.7.2
+boto>=2.49.0
+sphinx>=5.0.1
+setproctitle>=1.2.3
+objgraph>=3.5.0
+pint>=0.18
 
 [optional-strict]
 Pygments==2.2.0
-astor==0.8.1
 autopep8==1.6.0
+astor==0.8.1
+pyperclip==1.5.7
+pyfiglet==0.7.2
 boto==2.49.0
+sphinx==5.0.1
+setproctitle==1.2.3
 objgraph==3.5.0
 pint==0.18
-pyfiglet==0.7.2
-pyperclip==1.5.7
-setproctitle==1.2.3
-sphinx==5.0.1
 
 [optional-strict:python_version < "3.10" and python_version >= "3.9"]
-h5py==3.7.0
-lru-dict==1.1.8
 xxhash==2.0.2
+lru-dict==1.1.8
+h5py==3.7.0
 
 [optional-strict:python_version < "3.11" and python_version >= "3.10"]
-h5py==3.7.0
 xxhash==3.0.0
+h5py==3.7.0
+
+[optional-strict:python_version < "3.12" and python_version >= "3.11"]
+xxhash==3.2.0
+h5py==3.8.0
 
 [optional-strict:python_version < "3.6" and python_version >= "3.5"]
 h5py==3.7.0
 
 [optional-strict:python_version < "3.7" and python_version >= "3.6"]
-h5py==3.7.0
-lru-dict==1.1.8
 xxhash==1.3.0
+lru-dict==1.1.8
+h5py==3.7.0
 
 [optional-strict:python_version < "3.8" and python_version >= "3.7"]
-h5py==3.7.0
-lru-dict==1.1.8
 xxhash==1.3.0
+lru-dict==1.1.8
+h5py==3.7.0
 
 [optional-strict:python_version < "3.9" and python_version >= "3.8"]
-h5py==3.7.0
-lru-dict==1.1.8
 xxhash==1.4.3
+lru-dict==1.1.8
+h5py==3.7.0
 
 [optional-strict:python_version < "4.0" and python_version >= "3.10"]
 lru-dict==1.1.8
 
-[optional-strict:python_version < "4.0" and python_version >= "3.11"]
-h5py==3.8.0
-xxhash==3.0.0
+[optional-strict:python_version < "4.0" and python_version >= "3.12"]
+xxhash==3.4.1
+h5py==3.10.0
 
 [optional:python_version < "3.10" and python_version >= "3.9"]
-h5py
-lru-dict
-xxhash
+xxhash>=2.0.2
+lru-dict>=1.1.8
+h5py>=3.7.0
 
 [optional:python_version < "3.11" and python_version >= "3.10"]
-h5py
-xxhash
+xxhash>=3.0.0
+h5py>=3.7.0
+
+[optional:python_version < "3.12" and python_version >= "3.11"]
+xxhash>=3.2.0
+h5py>=3.8.0
 
 [optional:python_version < "3.6" and python_version >= "3.5"]
-h5py
+h5py>=3.7.0
 
 [optional:python_version < "3.7" and python_version >= "3.6"]
-h5py
-lru-dict
-xxhash
+xxhash>=1.3.0
+lru-dict>=1.1.8
+h5py>=3.7.0
 
 [optional:python_version < "3.8" and python_version >= "3.7"]
-h5py
-lru-dict
-xxhash
+xxhash>=1.3.0
+lru-dict>=1.1.8
+h5py>=3.7.0
 
 [optional:python_version < "3.9" and python_version >= "3.8"]
-h5py
-lru-dict
-xxhash
+xxhash>=1.4.3
+lru-dict>=1.1.8
+h5py>=3.7.0
 
 [optional:python_version < "4.0" and python_version >= "3.10"]
-lru-dict
+lru-dict>=1.1.8
 
-[optional:python_version < "4.0" and python_version >= "3.11"]
-h5py
-xxhash
+[optional:python_version < "4.0" and python_version >= "3.12"]
+xxhash>=3.4.1
+h5py>=3.10.0
+
+[runtime]
+six>=1.10.0
+parse>=1.6.6
+requests>=2.27.1
+pyparsing>=3.0.7
+delorean>=1.0.0
+timerit>=1.0.1
 
 [runtime-strict]
-delorean==1.0.0
+six==1.10.0
 parse==1.6.6
-pyparsing==3.0.7
 requests==2.27.1
-six==1.10.0
+pyparsing==3.0.7
+delorean==1.0.0
 timerit==1.0.1
 
 [runtime-strict:python_version < "2.7" and python_version >= "2.6"]
 gitpython==2.1.8
 
 [runtime-strict:python_version < "3.0"]
-futures==1.0.0
 lockfile==0.10.2
+futures==1.0.0
 
 [runtime-strict:python_version < "3.0" and python_version >= "2.7"]
 gitpython==2.1.4
 
 [runtime-strict:python_version < "3.10" and python_version >= "3.9"]
 numpy==1.19.3
 pandas==1.4.0
@@ -553,37 +603,37 @@
 [runtime-strict:python_version < "3.6" and python_version >= "2.7"]
 ubelt==0.8.1
 
 [runtime-strict:python_version < "3.6" and python_version >= "3.4"]
 gitpython==3.0.7
 
 [runtime-strict:python_version < "3.6" and python_version >= "3.5"]
-networkx==2.3
 numpy==1.11.1
+networkx==2.3
 
 [runtime-strict:python_version < "3.6" and python_version >= "3.5.3"]
 pandas==0.25.0
 
 [runtime-strict:python_version < "3.6.1" and python_version >= "3.6"]
 pandas==0.20.3
 
 [runtime-strict:python_version < "3.7" and python_version >= "3.6"]
+numpy==1.12.0
 gitpython==3.1.18
 networkx==2.5
-numpy==1.12.0
 
 [runtime-strict:python_version < "3.7" and python_version >= "3.6.1"]
 pandas==1.0.0
 
 [runtime-strict:python_version < "3.7.1" and python_version >= "3.7"]
 pandas==1.1.3
 
 [runtime-strict:python_version < "3.8" and python_version >= "3.7"]
-networkx==2.6.2
 numpy==1.14.5
+networkx==2.6.2
 
 [runtime-strict:python_version < "3.8" and python_version >= "3.7.1"]
 pandas==1.2.0
 
 [runtime-strict:python_version < "3.9" and python_version >= "3.8"]
 numpy==1.19.2
 pandas==1.4.0
@@ -597,118 +647,214 @@
 
 [runtime-strict:python_version >= "3.7"]
 gitpython==3.1.24
 
 [runtime-strict:python_version >= "3.8"]
 networkx==2.7
 
+[runtime:python_version < "2.7" and python_version >= "2.6"]
+gitpython>=2.1.8
+
+[runtime:python_version < "3.0"]
+lockfile>=0.10.2
+futures>=1.0.0
+
+[runtime:python_version < "3.0" and python_version >= "2.7"]
+gitpython>=2.1.4
+
+[runtime:python_version < "3.10" and python_version >= "3.9"]
+numpy>=1.19.3
+pandas>=1.4.0
+
+[runtime:python_version < "3.11" and python_version >= "3.10"]
+numpy>=1.21.6
+pandas>=1.3.5
+
+[runtime:python_version < "3.4" and python_version >= "2.7"]
+numpy>=1.11.1
+pandas>=0.20.1
+
+[runtime:python_version < "3.4" and python_version >= "3.0"]
+gitpython>=2.1.12
+
+[runtime:python_version < "3.5" and python_version >= "2.7"]
+networkx>=1.11
+
+[runtime:python_version < "3.5" and python_version >= "3.4"]
+numpy>=1.11.1
+pandas>=0.18.1
+
+[runtime:python_version < "3.5.3" and python_version >= "3.5"]
+pandas>=0.18.1
+
+[runtime:python_version < "3.6" and python_version >= "2.7"]
+ubelt>=0.8.1
+
+[runtime:python_version < "3.6" and python_version >= "3.4"]
+gitpython>=3.0.7
+
+[runtime:python_version < "3.6" and python_version >= "3.5"]
+numpy>=1.11.1
+networkx>=2.3
+
+[runtime:python_version < "3.6" and python_version >= "3.5.3"]
+pandas>=0.25.0
+
+[runtime:python_version < "3.6.1" and python_version >= "3.6"]
+pandas>=0.20.3
+
+[runtime:python_version < "3.7" and python_version >= "3.6"]
+numpy>=1.12.0
+gitpython>=3.1.18
+networkx>=2.5
+
+[runtime:python_version < "3.7" and python_version >= "3.6.1"]
+pandas>=1.0.0
+
+[runtime:python_version < "3.7.1" and python_version >= "3.7"]
+pandas>=1.1.3
+
+[runtime:python_version < "3.8" and python_version >= "3.7"]
+numpy>=1.14.5
+networkx>=2.6.2
+
+[runtime:python_version < "3.8" and python_version >= "3.7.1"]
+pandas>=1.2.0
+
+[runtime:python_version < "3.9" and python_version >= "3.8"]
+numpy>=1.19.2
+pandas>=1.4.0
+
+[runtime:python_version < "4.0" and python_version >= "3.11"]
+numpy>=1.24.0
+pandas>=1.5.0
+
+[runtime:python_version >= "3.6"]
+ubelt>=1.0.0
+
+[runtime:python_version >= "3.7"]
+gitpython>=3.1.24
+
+[runtime:python_version >= "3.8"]
+networkx>=2.7
+
 [tests]
-codecov
-pytest-timeout
-xdoctest
+xdoctest>=1.1.3
+pytest-timeout>=1.4.2
 
 [tests-strict]
-codecov==2.0.15
+xdoctest==1.1.3
 pytest-timeout==1.4.2
-xdoctest==0.14.0
 
 [tests-strict:python_version < "2.7" and python_version >= "2.6"]
 coverage==4.5
 
 [tests-strict:python_version < "2.8.0" and python_version >= "2.7.0"]
-pytest-cov==2.8.1
 pytest<=4.6.11,==4.6.0
+pytest-cov==2.8.1
 
 [tests-strict:python_version < "3.10" and python_version >= "3.9"]
+pytest==8.1.1
 coverage==5.3.1
 
-[tests-strict:python_version < "3.10.0" and python_version >= "3.7.0"]
-pytest==4.6.0
+[tests-strict:python_version < "3.11" and python_version >= "3.10"]
+pytest==8.1.1
+
+[tests-strict:python_version < "3.12" and python_version >= "3.11"]
+pytest==8.1.1
+
+[tests-strict:python_version < "3.13" and python_version >= "3.12"]
+pytest==8.1.1
 
 [tests-strict:python_version < "3.4" and python_version >= "2.7"]
 coverage==5.3.1
 
 [tests-strict:python_version < "3.5" and python_version >= "3.4"]
 coverage==4.3.4
 
 [tests-strict:python_version < "3.5.0" and python_version >= "3.4.0"]
-pytest-cov==2.8.1
 pytest<=4.6.11,==4.6.0
+pytest-cov==2.8.1
 
 [tests-strict:python_version < "3.6" and python_version >= "3.5"]
 coverage==5.3.1
 
 [tests-strict:python_version < "3.6.0" and python_version >= "3.5.0"]
-pytest-cov==2.9.0
 pytest<=6.1.2,==4.6.0
+pytest-cov==2.9.0
 
 [tests-strict:python_version < "3.7" and python_version >= "3.6"]
 coverage==6.1.1
 
-[tests-strict:python_version < "3.7.0" and python_version >= "3.6.0"]
-pytest==4.6.0
-
 [tests-strict:python_version < "3.8" and python_version >= "3.7"]
+pytest==4.6.0
 coverage==6.1.1
 
 [tests-strict:python_version < "3.9" and python_version >= "3.8"]
+pytest==8.1.1
 coverage==6.1.1
 
+[tests-strict:python_version < "4.0" and python_version >= "3.13"]
+pytest==8.1.1
+
 [tests-strict:python_version >= "3.10"]
 coverage==6.1.1
 
-[tests-strict:python_version >= "3.10.0"]
-pytest==6.2.5
-
 [tests-strict:python_version >= "3.6.0"]
 pytest-cov==3.0.0
 
 [tests:python_version < "2.7" and python_version >= "2.6"]
-coverage
+coverage>=4.5
 
 [tests:python_version < "2.8.0" and python_version >= "2.7.0"]
-pytest
-pytest-cov
+pytest<=4.6.11,>=4.6.0
+pytest-cov>=2.8.1
 
 [tests:python_version < "3.10" and python_version >= "3.9"]
-coverage
+pytest>=8.1.1
+coverage>=5.3.1
 
-[tests:python_version < "3.10.0" and python_version >= "3.7.0"]
-pytest
+[tests:python_version < "3.11" and python_version >= "3.10"]
+pytest>=8.1.1
+
+[tests:python_version < "3.12" and python_version >= "3.11"]
+pytest>=8.1.1
+
+[tests:python_version < "3.13" and python_version >= "3.12"]
+pytest>=8.1.1
 
 [tests:python_version < "3.4" and python_version >= "2.7"]
-coverage
+coverage>=5.3.1
 
 [tests:python_version < "3.5" and python_version >= "3.4"]
-coverage
+coverage>=4.3.4
 
 [tests:python_version < "3.5.0" and python_version >= "3.4.0"]
-pytest
-pytest-cov
+pytest<=4.6.11,>=4.6.0
+pytest-cov>=2.8.1
 
 [tests:python_version < "3.6" and python_version >= "3.5"]
-coverage
+coverage>=5.3.1
 
 [tests:python_version < "3.6.0" and python_version >= "3.5.0"]
-pytest
-pytest-cov
+pytest<=6.1.2,>=4.6.0
+pytest-cov>=2.9.0
 
 [tests:python_version < "3.7" and python_version >= "3.6"]
-coverage
-
-[tests:python_version < "3.7.0" and python_version >= "3.6.0"]
-pytest
+coverage>=6.1.1
 
 [tests:python_version < "3.8" and python_version >= "3.7"]
-coverage
+pytest>=4.6.0
+coverage>=6.1.1
 
 [tests:python_version < "3.9" and python_version >= "3.8"]
-coverage
+pytest>=8.1.1
+coverage>=6.1.1
 
-[tests:python_version >= "3.10"]
-coverage
+[tests:python_version < "4.0" and python_version >= "3.13"]
+pytest>=8.1.1
 
-[tests:python_version >= "3.10.0"]
-pytest
+[tests:python_version >= "3.10"]
+coverage>=6.1.1
 
 [tests:python_version >= "3.6.0"]
-pytest-cov
+pytest-cov>=3.0.0
```

