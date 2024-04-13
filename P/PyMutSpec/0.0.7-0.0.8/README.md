# Comparing `tmp/PyMutSpec-0.0.7.tar.gz` & `tmp/PyMutSpec-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyMutSpec-0.0.7.tar", last modified: Mon Oct 16 15:17:09 2023, max compression
+gzip compressed data, was "PyMutSpec-0.0.8.tar", last modified: Mon Nov 13 12:47:37 2023, max compression
```

## Comparing `PyMutSpec-0.0.7.tar` & `PyMutSpec-0.0.8.tar`

### file list

```diff
@@ -1,62 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 15:17:09.418735 PyMutSpec-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2023-10-16 15:17:09.418735 PyMutSpec-0.0.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 15:17:09.410735 PyMutSpec-0.0.7/PyMutSpec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2023-10-16 15:17:09.000000 PyMutSpec-0.0.7/PyMutSpec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-10-16 15:17:09.000000 PyMutSpec-0.0.7/PyMutSpec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-16 15:17:09.000000 PyMutSpec-0.0.7/PyMutSpec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-10-16 15:17:09.000000 PyMutSpec-0.0.7/PyMutSpec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-16 15:17:09.000000 PyMutSpec-0.0.7/PyMutSpec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 15:17:09.410735 PyMutSpec-0.0.7/pymutspec/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/pymutspec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 15:17:09.414735 PyMutSpec-0.0.7/pymutspec/annotation/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/pymutspec/annotation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/pymutspec/annotation/auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (127)    31436 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/pymutspec/annotation/mut.py
--rw-r--r--   0 runner    (1001) docker     (127)     9669 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/pymutspec/annotation/spectra.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/pymutspec/annotation/tree.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 15:17:09.414735 PyMutSpec-0.0.7/pymutspec/constants/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/pymutspec/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/pymutspec/constants/sbs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 15:17:09.414735 PyMutSpec-0.0.7/pymutspec/draw/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/pymutspec/draw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/pymutspec/draw/sbs_orders.py
--rw-r--r--   0 runner    (1001) docker     (127)     9833 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/pymutspec/draw/spectra.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 15:17:09.414735 PyMutSpec-0.0.7/pymutspec/io/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/pymutspec/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3212 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/pymutspec/io/auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (127)    11972 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/pymutspec/io/states.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 15:17:09.414735 PyMutSpec-0.0.7/pymutspec/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/pymutspec/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 15:17:09.414735 PyMutSpec-0.0.7/pymutspec/utils/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/pymutspec/utils/configs/log_settings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      701 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/pymutspec/utils/custom_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/pymutspec/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      179 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 15:17:09.418735 PyMutSpec-0.0.7/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2866 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/scripts/1.terminal_genomes2iqtree_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/scripts/2.iqtree_states2custom_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/scripts/2.iqtree_states_parted2custom_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/scripts/alignment2iqtree_states.py
--rw-r--r--   0 runner    (1001) docker     (127)    11839 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/scripts/calculate_mutspec.py
--rw-r--r--   0 runner    (1001) docker     (127)    19203 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/scripts/collect_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/scripts/concat_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)      906 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/scripts/filter_aln.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/scripts/iqtree_states_add_part.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/scripts/multifasta_coding.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/scripts/plot_spectra.py
--rw-r--r--   0 runner    (1001) docker     (127)     6278 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/scripts/pyvolve_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/scripts/qc_aln.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/scripts/raxml_states2iqtree_states.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/scripts/rename_internal_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/scripts/select_records.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-16 15:17:09.418735 PyMutSpec-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 15:17:09.418735 PyMutSpec-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/tests/test_codon_ann.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/tests/test_collect_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2023-10-16 15:16:57.000000 PyMutSpec-0.0.7/tests/test_mutspec_calc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 12:47:37.569058 PyMutSpec-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2023-11-13 12:47:37.565058 PyMutSpec-0.0.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 12:47:37.561058 PyMutSpec-0.0.8/PyMutSpec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2023-11-13 12:47:37.000000 PyMutSpec-0.0.8/PyMutSpec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2023-11-13 12:47:37.000000 PyMutSpec-0.0.8/PyMutSpec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-13 12:47:37.000000 PyMutSpec-0.0.8/PyMutSpec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2023-11-13 12:47:37.000000 PyMutSpec-0.0.8/PyMutSpec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-13 12:47:37.000000 PyMutSpec-0.0.8/PyMutSpec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 12:47:37.561058 PyMutSpec-0.0.8/pymutspec/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/pymutspec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 12:47:37.561058 PyMutSpec-0.0.8/pymutspec/annotation/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/pymutspec/annotation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/pymutspec/annotation/auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31437 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/pymutspec/annotation/mut.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10075 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/pymutspec/annotation/spectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/pymutspec/annotation/tree.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 12:47:37.561058 PyMutSpec-0.0.8/pymutspec/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/pymutspec/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/pymutspec/constants/sbs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 12:47:37.561058 PyMutSpec-0.0.8/pymutspec/draw/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/pymutspec/draw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/pymutspec/draw/sbs_orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9861 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/pymutspec/draw/spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 12:47:37.561058 PyMutSpec-0.0.8/pymutspec/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/pymutspec/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3212 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/pymutspec/io/auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11972 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/pymutspec/io/states.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 12:47:37.561058 PyMutSpec-0.0.8/pymutspec/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/pymutspec/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 12:47:37.565058 PyMutSpec-0.0.8/pymutspec/utils/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/pymutspec/utils/configs/log_settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/pymutspec/utils/custom_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/pymutspec/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 12:47:37.565058 PyMutSpec-0.0.8/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2866 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/scripts/1.terminal_genomes2iqtree_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/scripts/2.iqtree_states2custom_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/scripts/2.iqtree_states_parted2custom_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/scripts/alignment2iqtree_states.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11839 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/scripts/calculate_mutspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19211 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/scripts/collect_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/scripts/concat_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/scripts/filter_aln.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/scripts/iqtree_states_add_part.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/scripts/multifasta_coding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/scripts/plot_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6278 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/scripts/pyvolve_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/scripts/qc_aln.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/scripts/raxml_states2iqtree_states.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/scripts/rename_internal_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/scripts/select_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-13 12:47:37.569058 PyMutSpec-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-13 12:47:37.565058 PyMutSpec-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3318 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/tests/test_codon_ann.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/tests/test_collect_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/tests/test_mutspec_calc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/tests/test_plot_spectrum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/tests/test_run_main_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2023-11-13 12:47:28.000000 PyMutSpec-0.0.8/tests/test_tree_annotation.py
```

### Comparing `PyMutSpec-0.0.7/LICENSE` & `PyMutSpec-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/PyMutSpec.egg-info/SOURCES.txt` & `PyMutSpec-0.0.8/PyMutSpec.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -42,8 +42,11 @@
 scripts/qc_aln.py
 scripts/raxml_states2iqtree_states.py
 scripts/rename_internal_nodes.py
 scripts/select_records.py
 tests/test_codon_ann.py
 tests/test_collect_mutations.py
 tests/test_io.py
-tests/test_mutspec_calc.py
+tests/test_mutspec_calc.py
+tests/test_plot_spectrum.py
+tests/test_run_main_scripts.py
+tests/test_tree_annotation.py
```

### Comparing `PyMutSpec-0.0.7/pymutspec/annotation/auxiliary.py` & `PyMutSpec-0.0.8/pymutspec/annotation/auxiliary.py`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/pymutspec/annotation/mut.py` & `PyMutSpec-0.0.8/pymutspec/annotation/mut.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class CodonAnnotation:
     nucl_order = possible_nucls
 
     def __init__(self, gencode: Union[NCBICodonTableDNA, int]):
         self.codontable = self._prepare_codontable(gencode)
         self._syn_codons, self._ff_codons = self.__extract_syn_codons()
-        self.possible_ff_contexts = self.__extract_possible_ff_contexts()
+        self.possible_ff_contexts  = self.__extract_possible_ff_contexts()
         self.possible_syn_contexts = self.__extract_possible_syn_contexts()
         self.startcodons, self.stopcodons = self.read_start_stop_codons(gencode)
 
     def is_fourfold(self, cdn: str):
         """Check if codon is neutral in 3rd position"""
         return cdn in self._ff_codons
```

### Comparing `PyMutSpec-0.0.7/pymutspec/annotation/spectra.py` & `PyMutSpec-0.0.8/pymutspec/annotation/spectra.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,28 +110,47 @@
     if len(df.columns) != 192:
         for sbs192 in set(possible_sbs192).difference(df.columns.values):
             df[sbs192] = 0.
     df = df[possible_sbs192]
     return df
 
 
+def collapse_sbs192(df: pd.DataFrame, to=12):
+    assert (df.columns == possible_sbs192).all()
+    df = df.copy()
+    if to == 12:
+        for sbs192 in possible_sbs192:
+            sbs12 = sbs192[2:5]
+            if sbs12 in df.columns.values:
+                df[sbs12] += df[sbs192]
+            else:
+                df[sbs12] = df[sbs192]
+
+        return df[possible_sbs12]
+    else:
+        raise NotImplementedError()
+
+
 def jackknife_spectra_sampling(obs: pd.DataFrame, exp: pd.DataFrame, frac=0.5, n=1000):
-    if len(obs.columns) == 192 and (obs.columns == possible_sbs192).all() and (exp.columns == possible_sbs192).all():
+    if len(obs.columns) == 192 and \
+            (obs.columns == possible_sbs192).all() and \
+                (exp.columns == possible_sbs192).all():
         assert obs.index.names == ["RefNode", "AltNode"]
         assert exp.index.names == ["Node"]
         altnodes  = obs.index.get_level_values(1).values
         obs_edges = obs
         freqs_nodes = exp
         obs_edges.index = obs_edges.index.reorder_levels(order=["AltNode", "RefNode"])
         freqs_nodes.index.name = "RefNode"
     else:
         altnodes = obs.AltNode.unique()
         obs_edges = obs.groupby(["AltNode", "RefNode", "Mut"]).ProbaFull.sum().unstack()
         obs_edges = complete_sbs192_columns(obs_edges)
-        freqs_nodes = exp.rename(columns={"Node": "RefNode"}).groupby(["RefNode", "Mut"]).Proba.sum().unstack()
+        freqs_nodes = exp.rename(columns={"Node": "RefNode"})\
+            .groupby(["RefNode", "Mut"]).Proba.sum().unstack()
         freqs_nodes = complete_sbs192_columns(freqs_nodes)
 
     edges_sample_size = int(len(altnodes) * frac)
     spectra = []
     for _ in range(n):
         altnodes_sample = np.random.choice(altnodes, edges_sample_size, False)
         obs_sample = obs_edges.loc[altnodes_sample].reset_index(0, drop=True)
@@ -160,37 +179,47 @@
                 df[sbs12] = df[sbs192]
 
         return df[possible_sbs12]
     else:
         raise NotImplementedError()
 
 
-def calc_edgewise_spectra(obs: pd.DataFrame, exp: pd.DataFrame, nmtypes_cutoff=16, nobs_cuttof=20, collapse_to_12=False, scale=True, both_12_and_192=False):
-    if len(obs.columns) == 192 and (obs.columns == possible_sbs192).all() and (exp.columns == possible_sbs192).all():
+def calc_edgewise_spectra(
+        obs: pd.DataFrame, exp: pd.DataFrame, 
+        nmtypes_cutoff=10, nobs_cuttof=10, 
+        collapse_to_12=False, scale=True, 
+        both_12_and_192=False
+    ):
+    if len(obs.columns) == 192 and \
+            (obs.columns == possible_sbs192).all() and \
+                (exp.columns == possible_sbs192).all():
         assert obs.index.names == ["RefNode", "AltNode"]
         assert exp.index.names == ["Node"]
         obs_edges = obs
         freqs_nodes = exp
         freqs_nodes.index.name = "RefNode"
     else:
         obs_edges = obs.groupby(["RefNode", "AltNode", "Mut"]).ProbaFull.sum().unstack()
         obs_edges = complete_sbs192_columns(obs_edges)
         freqs_nodes = exp.groupby(["Node", "Mut"]).Proba.sum().unstack()
         freqs_nodes.index.name = "RefNode"
         freqs_nodes = complete_sbs192_columns(freqs_nodes)
 
     if not collapse_to_12:
-        obs_edges = obs_edges[((obs_edges > 0).sum(axis=1) >= nmtypes_cutoff) & (obs_edges.sum(axis=1) > nobs_cuttof)]
+        obs_edges = obs_edges[((obs_edges > 0).sum(axis=1) >= nmtypes_cutoff) & \
+                               (obs_edges.sum(axis=1) >= nobs_cuttof)]
     
     edges_df = obs_edges.index.to_frame(False)
 
     freqs_edges = edges_df.merge(freqs_nodes, on="RefNode")\
         .set_index(["RefNode", "AltNode"])[possible_sbs192]
-    
-    
+
+    # some indexes can be deleted from freqs, so we must delete them from obs
+    obs_edges = obs_edges.loc[freqs_edges.index]
+
     assert (obs_edges.columns == freqs_edges.columns).all()
     assert (obs_edges.index == freqs_edges.index).all()
 
     if both_12_and_192:
         obs_edges12   = collapse_sbs192(obs_edges.fillna(0.),   to=12)
         freqs_edges12 = collapse_sbs192(freqs_edges.fillna(0.), to=12)
 
@@ -219,26 +248,14 @@
 
     spectra = spectra.fillna(0)
     assert not (spectra == np.inf).any().any()
     assert not (spectra.isna()).any().any()
     return spectra
 
 
-def assign_cat(p: float, interval=0.1):
-    if interval < 0.01:
-        raise NotImplementedError
-    
-    left = p // interval / (1 / interval)
-    right = left + interval
-    if interval >= 0.1:
-        return f"{left:.1f}_{right:.1f}"
-    else:
-        return f"{left:.2f}_{right:.2f}"
-
-
 def get_cossim(a: pd.DataFrame, b: pd.DataFrame):
     assert (a.columns == b.columns).all()
     
     common_index = a.index.intersection(b.index)
     if len(common_index) == 0:
         return pd.Series()
```

### Comparing `PyMutSpec-0.0.7/pymutspec/constants/sbs.py` & `PyMutSpec-0.0.8/pymutspec/constants/sbs.py`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/pymutspec/draw/sbs_orders.py` & `PyMutSpec-0.0.8/pymutspec/draw/sbs_orders.py`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/pymutspec/draw/spectra.py` & `PyMutSpec-0.0.8/pymutspec/draw/spectra.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,14 +186,15 @@
 
     if savepath is not None:
         plt.savefig(savepath, dpi=300, bbox_inches="tight")
     if show:
         plt.show()
     else:
         plt.close()
+    return ax
 
 
 def plot_mutspec96(
         spectra: pd.DataFrame, 
         ylabel="MutSpec", 
         title="Mutational spectrum", 
         figsize=(15, 5), 
@@ -269,14 +270,15 @@
 
     if savepath is not None:
         plt.savefig(savepath, dpi=300, bbox_inches="tight")
     if show:
         plt.show()
     else:
         plt.close()
+    return ax
 
 
 def plot_mutspec192kk(mutspec192: pd.DataFrame, ylabel="MutSpec", title="Mutational spectrum", show=True, figsize=(24, 6), filepath=None):
     ms192 = mutspec192.copy()
     ms192["long_lbl"] = ms192.Mut.str.get(2) + ms192.Mut.str.get(4) + ": " + ms192.Mut.str.get(0) + ms192.Mut.str.get(2) + ms192.Mut.str.get(-1)
     fig = plt.figure(figsize=figsize)
     ax = fig.add_subplot(111)
```

### Comparing `PyMutSpec-0.0.7/pymutspec/io/auxiliary.py` & `PyMutSpec-0.0.8/pymutspec/io/auxiliary.py`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/pymutspec/io/states.py` & `PyMutSpec-0.0.8/pymutspec/io/states.py`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/pymutspec/utils/configs/log_settings.yaml` & `PyMutSpec-0.0.8/pymutspec/utils/configs/log_settings.yaml`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/pymutspec/utils/custom_profile.py` & `PyMutSpec-0.0.8/pymutspec/utils/custom_profile.py`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/scripts/1.terminal_genomes2iqtree_format.py` & `PyMutSpec-0.0.8/scripts/1.terminal_genomes2iqtree_format.py`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/scripts/2.iqtree_states2custom_format.py` & `PyMutSpec-0.0.8/scripts/2.iqtree_states2custom_format.py`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/scripts/2.iqtree_states_parted2custom_format.py` & `PyMutSpec-0.0.8/scripts/2.iqtree_states_parted2custom_format.py`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/scripts/alignment2iqtree_states.py` & `PyMutSpec-0.0.8/scripts/alignment2iqtree_states.py`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/scripts/calculate_mutspec.py` & `PyMutSpec-0.0.8/scripts/calculate_mutspec.py`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/scripts/collect_mutations.py` & `PyMutSpec-0.0.8/scripts/collect_mutations.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,50 +3,57 @@
 pic is position in codon
 
 """
 
 import os
 import sys
 from collections import defaultdict
+from collections.abc import Iterable
 from shutil import rmtree
-from typing import Iterable, Union
 
 import click
 import numpy as np
 import pandas as pd
 from ete3 import PhyloTree
 
-from pymutspec.annotation import (CodonAnnotation, calculate_mutspec,
-                                      get_farthest_leaf, iter_tree_edges,
-                                      lbl2lbl_id)
+from pymutspec.annotation import (
+    CodonAnnotation, calculate_mutspec, 
+    iter_tree_edges, lbl2lbl_id, calc_phylocoefs, get_tree_outgrp_name,
+)
 from pymutspec.constants import possible_sbs12, possible_sbs192
 from pymutspec.io import GenesStates
-from pymutspec.utils import load_logger
+from pymutspec.utils import load_logger, basic_logger
 
-logger = None
+logger = basic_logger()
 
 
 class MutSpec(CodonAnnotation, GenesStates):    
     def __init__(
-            self, path_to_tree, path_to_states, outdir, 
+            self, path_to_tree, path_to_states, outdir,
             gcode=2, db_mode="dict", path_to_db=None, states_fmt="table",
-            rewrite_db=None, use_proba=False, proba_cutoff=0.05, 
-            use_phylocoef=False, syn=False, syn_c=False, syn4f=False, derive_spectra=True,
-            path_to_rates=None, cat_cutoff=0, save_exp_muts=False,
+            rewrite_db=None, use_proba=False, proba_cutoff=0.05,
+            use_phylocoef=False, syn=False, syn_c=False, syn4f=False,
+            derive_spectra=True, save_exp_muts=False,
+            path_to_rates=None, cat_cutoff=0,
             mnum192=16,
         ):
-        for path in list(path_to_states) + [path_to_tree]:
+        if not os.path.exists(path_to_tree):
+            raise ValueError(f"Path to tree doesn't exist: '{path_to_tree}'")
+
+        if not isinstance(path_to_states, Iterable):
+            raise ValueError(f"path_to_states must be Iterable of paths; got: '{type(path_to_states)}'")
+        for path in list(path_to_states):
             if not os.path.exists(path):
-                raise ValueError(f"Path doesn't exist: {path}")
+                raise ValueError(f"Path to states doesn't exist: '{path}'")
 
         CodonAnnotation.__init__(self, gencode=gcode)
         GenesStates.__init__(
-            self, path_states=path_to_states, path_to_db=path_to_db, 
-            mode=db_mode, rewrite=rewrite_db, use_proba=use_proba, 
-            path_to_rates=path_to_rates, cat_cutoff=cat_cutoff, 
+            self, path_states=path_to_states, path_to_db=path_to_db,
+            mode=db_mode, rewrite=rewrite_db, use_proba=use_proba,
+            path_to_rates=path_to_rates, cat_cutoff=cat_cutoff,
             states_fmt=states_fmt,
         )
         self.gcode = gcode
         self.use_proba = use_proba
         self.proba_cutoff = proba_cutoff
         self.use_phylocoef = use_phylocoef if use_proba else False
         self.derive_spectra = derive_spectra
@@ -65,19 +72,19 @@
         if syn_c:
             self.MUT_LABELS.append("syn_c")
         if syn4f:
             self.MUT_LABELS.append("ff")
         logger.info(f"Types of mutations to collect and process: {self.MUT_LABELS}")
         self.fp_format = np.float32
         self.tree = PhyloTree(path_to_tree, format=1)
-        self.max_dist = self.fp_format(get_farthest_leaf(self.tree, 0.95))
+        self.outgrp_name = get_tree_outgrp_name(self.tree)
         logger.info(
             f"Tree loaded, number of leaf nodes: {len(self.tree)}, "
             f"total number of nodes: {len(self.tree.get_cached_content())}, "
-            f"distance to farthest leaf: {self.max_dist: .2f}"
+            f"outgroup name: {self.outgrp_name}"
         )
         rnd_genome = self.get_random_genome()
         logger.info(f"Number of genes: {len(rnd_genome)}, number of sites: {[len(x) for x in rnd_genome.values()]}")
         if self.mask:
             logger.info(f"Number of invariable sites: {[len(x) - sum(x) for x in self.mask.values()]}")
 
     def open_handles(self, outdir):
@@ -101,41 +108,38 @@
 
     def extract_mutspec_from_tree(self):
         self.open_handles(self.outdir)
 
         logger.info("Start mutation extraction from tree")
         add_header = defaultdict(lambda: True)
         aln_size = self.genome_size
-        dists_to_leafs = dict()
         visited_nodes = set()
         total_mut_num = 0
+
+        # calculate phylogenetic uncertainty correction
+        if self.use_phylocoef:
+            phylocoefs = calc_phylocoefs(self.tree, self.outgrp_name)
+
         for ei, (ref_node, alt_node) in enumerate(iter_tree_edges(self.tree), 1):
             if alt_node.name not in self.nodes:
                 logger.warning(f"Skip edge '{ref_node.name}'-'{alt_node.name}' due to absence of '{alt_node.name}' genome")
                 continue
             if ref_node.name not in self.nodes:
                 logger.warning(f"Skip edge '{ref_node.name}'-'{alt_node.name}' due to absence of '{ref_node.name}' genome")
                 continue
 
             # get genomes from storage
             ref_genome = self.get_genome(ref_node.name)
             alt_genome = self.get_genome(alt_node.name)
 
             # calculate phylogenetic uncertainty correction
             if self.use_phylocoef:
-                if ref_node.name in dists_to_leafs:
-                    dist_to_closest_leaf = dists_to_leafs[ref_node.name]
-                else:
-                    _, dist_to_closest_leaf = ref_node.get_closest_leaf()
-                    dists_to_leafs[ref_node.name] = dist_to_closest_leaf
-
-                dist_to_closest_leaf = self.fp_format(dist_to_closest_leaf)
-                phylocoef = self.fp_format(1 - min(0.9999, dist_to_closest_leaf / self.max_dist))
+                phylocoef = self.fp_format(phylocoefs[ref_node.name] * phylocoefs[alt_node.name])
             else:
-                phylocoef = 1
+                phylocoef = self.fp_format(1)
 
             genome_nucl_freqs = {lbl: defaultdict(self.fp_format) for lbl in self.MUT_LABELS}
             genome_cxt_freqs  = {lbl: defaultdict(self.fp_format) for lbl in self.MUT_LABELS}
             genome_mutations = []
             for gene in ref_genome:
                 mask = self.mask[gene] if self.mask is not None else None
```

### Comparing `PyMutSpec-0.0.7/scripts/concat_mutations.py` & `PyMutSpec-0.0.8/scripts/concat_mutations.py`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/scripts/filter_aln.py` & `PyMutSpec-0.0.8/scripts/filter_aln.py`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/scripts/iqtree_states_add_part.py` & `PyMutSpec-0.0.8/scripts/iqtree_states_add_part.py`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/scripts/multifasta_coding.py` & `PyMutSpec-0.0.8/scripts/multifasta_coding.py`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/scripts/plot_spectra.py` & `PyMutSpec-0.0.8/scripts/plot_spectra.py`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/scripts/pyvolve_process.py` & `PyMutSpec-0.0.8/scripts/pyvolve_process.py`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/scripts/qc_aln.py` & `PyMutSpec-0.0.8/scripts/qc_aln.py`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/scripts/raxml_states2iqtree_states.py` & `PyMutSpec-0.0.8/scripts/raxml_states2iqtree_states.py`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/scripts/rename_internal_nodes.py` & `PyMutSpec-0.0.8/scripts/rename_internal_nodes.py`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/scripts/select_records.py` & `PyMutSpec-0.0.8/scripts/select_records.py`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/setup.py` & `PyMutSpec-0.0.8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,30 @@
 import os
+import re
 from setuptools import setup, find_packages
 
+path_to_pyproject = 'pyproject.toml'
+
+
+def read_specs(path: str):
+    specs = dict()
+    with open(path, 'r') as fin:
+        for line in fin:
+            if line.startswith('name'):
+                specs['name'] = re.match('name = "(.+)"', line).group(1)
+            elif line.startswith('version'):
+                specs['version'] = re.match('version = "(.+)"', line).group(1)
+            elif line.startswith('description'):
+                specs['description'] = re.match('description = "(.+)"', line).group(1)
+            elif line.startswith('requires-python'):
+                specs['python_requires'] = re.match('requires-python = "(.+)"', line).group(1)
+                break
+    return specs
+
+
 extra_index_urls = []
 packages = []
 scripts = []
 
 with open("requirements.txt", encoding="utf-8") as file:
     for line in map(str.strip, file):
         if line:
@@ -19,23 +39,21 @@
     for file in os.listdir("scripts"):
         if file.endswith(".py") and not file.startswith("_"):
             fp = os.path.join("scripts", file)
             with open(fp) as fin:
                 if "python" in fin.readline():
                     scripts.append(fp)
 
+specs = read_specs(path_to_pyproject)
+
 setup(
-    name="PyMutSpec",
-    version="0.0.7",
     author="kpotoh",
-    description="Utilities for advanced analysis of mutational spectra",
+    author_email="axepon@mail.ru",
     url="https://github.com/mitoclub/PyMutSpec",
-    author_email="None",
     license="MIT",
     install_requires=packages,
     dependency_links=extra_index_urls,
     scripts=scripts,
     packages=find_packages(),
-    # include_package_data=True,
     package_data={'pymutspec': ['utils/configs/log_settings.yaml']},
-    python_requires=">=3.8",
+    **specs
 )
```

### Comparing `PyMutSpec-0.0.7/tests/test_codon_ann.py` & `PyMutSpec-0.0.8/tests/test_codon_ann.py`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/tests/test_io.py` & `PyMutSpec-0.0.8/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `PyMutSpec-0.0.7/tests/test_mutspec_calc.py` & `PyMutSpec-0.0.8/tests/test_mutspec_calc.py`

 * *Files identical despite different names*

