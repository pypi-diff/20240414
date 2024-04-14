# Comparing `tmp/pyphetools-0.9.8.tar.gz` & `tmp/pyphetools-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyphetools-0.9.8.tar", last modified: Tue Dec  5 14:07:22 2023, max compression
+gzip compressed data, was "pyphetools-0.9.9.tar", last modified: Wed Dec  6 13:56:54 2023, max compression
```

## Comparing `pyphetools-0.9.8.tar` & `pyphetools-0.9.9.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-05 14:07:22.579669 pyphetools-0.9.8/
--rw-r--r--   0 robinp   (904623974) 1088672553     1079 2023-01-08 15:20:15.000000 pyphetools-0.9.8/LICENSE
--rw-r--r--   0 robinp   (904623974) 1088672553        0 2023-01-05 13:57:40.000000 pyphetools-0.9.8/MANIFEST.in
--rw-r--r--   0 robinp   (904623974) 1088672553     3109 2023-12-05 14:07:22.579073 pyphetools-0.9.8/PKG-INFO
--rw-r--r--   0 robinp   (904623974) 1088672553      791 2023-09-30 00:15:51.000000 pyphetools-0.9.8/README.md
-drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-05 14:07:22.036158 pyphetools-0.9.8/ppt_venv/
-drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-05 14:07:22.166044 pyphetools-0.9.8/ppt_venv/bin/
--rwxr-xr-x   0 robinp   (904623974) 1088672553      630 2023-08-28 06:42:13.000000 pyphetools-0.9.8/ppt_venv/bin/rst2html.py
--rwxr-xr-x   0 robinp   (904623974) 1088672553      750 2023-08-28 06:42:13.000000 pyphetools-0.9.8/ppt_venv/bin/rst2html4.py
--rwxr-xr-x   0 robinp   (904623974) 1088672553     1118 2023-08-28 06:42:13.000000 pyphetools-0.9.8/ppt_venv/bin/rst2html5.py
--rwxr-xr-x   0 robinp   (904623974) 1088672553      827 2023-08-28 06:42:13.000000 pyphetools-0.9.8/ppt_venv/bin/rst2latex.py
--rwxr-xr-x   0 robinp   (904623974) 1088672553      635 2023-08-28 06:42:13.000000 pyphetools-0.9.8/ppt_venv/bin/rst2man.py
--rwxr-xr-x   0 robinp   (904623974) 1088672553      800 2023-08-28 06:42:13.000000 pyphetools-0.9.8/ppt_venv/bin/rst2odt.py
--rwxr-xr-x   0 robinp   (904623974) 1088672553     1762 2023-08-28 06:42:13.000000 pyphetools-0.9.8/ppt_venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 robinp   (904623974) 1088672553      637 2023-08-28 06:42:13.000000 pyphetools-0.9.8/ppt_venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 robinp   (904623974) 1088672553      673 2023-08-28 06:42:13.000000 pyphetools-0.9.8/ppt_venv/bin/rst2s5.py
--rwxr-xr-x   0 robinp   (904623974) 1088672553      907 2023-08-28 06:42:13.000000 pyphetools-0.9.8/ppt_venv/bin/rst2xetex.py
--rwxr-xr-x   0 robinp   (904623974) 1088672553      638 2023-08-28 06:42:13.000000 pyphetools-0.9.8/ppt_venv/bin/rst2xml.py
--rwxr-xr-x   0 robinp   (904623974) 1088672553      706 2023-08-28 06:42:13.000000 pyphetools-0.9.8/ppt_venv/bin/rstpep2html.py
-drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-05 14:07:22.577993 pyphetools-0.9.8/pyphetools.egg-info/
--rw-r--r--   0 robinp   (904623974) 1088672553     3109 2023-12-05 14:07:21.000000 pyphetools-0.9.8/pyphetools.egg-info/PKG-INFO
--rw-r--r--   0 robinp   (904623974) 1088672553     5557 2023-12-05 14:07:22.000000 pyphetools-0.9.8/pyphetools.egg-info/SOURCES.txt
--rw-r--r--   0 robinp   (904623974) 1088672553        1 2023-12-05 14:07:21.000000 pyphetools-0.9.8/pyphetools.egg-info/dependency_links.txt
--rw-r--r--   0 robinp   (904623974) 1088672553        1 2023-08-30 08:37:05.000000 pyphetools-0.9.8/pyphetools.egg-info/not-zip-safe
--rw-r--r--   0 robinp   (904623974) 1088672553       81 2023-12-05 14:07:21.000000 pyphetools-0.9.8/pyphetools.egg-info/requires.txt
--rw-r--r--   0 robinp   (904623974) 1088672553       71 2023-12-05 14:07:21.000000 pyphetools-0.9.8/pyphetools.egg-info/top_level.txt
--rw-r--r--   0 robinp   (904623974) 1088672553     1833 2023-10-12 20:14:59.000000 pyphetools-0.9.8/pyproject.toml
--rw-r--r--   0 robinp   (904623974) 1088672553       38 2023-12-05 14:07:22.579744 pyphetools-0.9.8/setup.cfg
-drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-05 14:07:22.036708 pyphetools-0.9.8/src/
-drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-05 14:07:22.462026 pyphetools-0.9.8/src/pyphetools/
--rw-r--r--   0 robinp   (904623974) 1088672553      180 2023-12-05 14:06:57.000000 pyphetools-0.9.8/src/pyphetools/__init__.py
-drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-05 14:07:22.513299 pyphetools-0.9.8/src/pyphetools/creation/
--rw-r--r--   0 robinp   (904623974) 1088672553     1835 2023-11-27 11:53:57.000000 pyphetools-0.9.8/src/pyphetools/creation/__init__.py
--rw-r--r--   0 robinp   (904623974) 1088672553     1905 2023-12-02 13:48:44.000000 pyphetools-0.9.8/src/pyphetools/creation/abstract_encoder.py
--rw-r--r--   0 robinp   (904623974) 1088672553     7296 2023-11-19 07:48:16.000000 pyphetools-0.9.8/src/pyphetools/creation/age_column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553     3249 2023-10-25 06:40:55.000000 pyphetools-0.9.8/src/pyphetools/creation/age_isoformater.py
--rw-r--r--   0 robinp   (904623974) 1088672553      117 2023-11-16 08:39:03.000000 pyphetools-0.9.8/src/pyphetools/creation/allelic_requirement.py
--rw-r--r--   0 robinp   (904623974) 1088672553    12272 2023-11-27 12:05:13.000000 pyphetools-0.9.8/src/pyphetools/creation/case_encoder.py
--rw-r--r--   0 robinp   (904623974) 1088672553      577 2023-11-27 12:00:38.000000 pyphetools-0.9.8/src/pyphetools/creation/citation.py
--rw-r--r--   0 robinp   (904623974) 1088672553    10738 2023-12-02 13:37:26.000000 pyphetools-0.9.8/src/pyphetools/creation/cohort_encoder.py
--rw-r--r--   0 robinp   (904623974) 1088672553      679 2023-10-15 12:30:42.000000 pyphetools-0.9.8/src/pyphetools/creation/column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553     2401 2023-11-19 06:55:43.000000 pyphetools-0.9.8/src/pyphetools/creation/constant_column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553      310 2023-11-16 08:22:53.000000 pyphetools-0.9.8/src/pyphetools/creation/constants.py
--rw-r--r--   0 robinp   (904623974) 1088672553      745 2023-11-13 14:50:53.000000 pyphetools-0.9.8/src/pyphetools/creation/disease.py
--rw-r--r--   0 robinp   (904623974) 1088672553     1083 2023-10-16 07:36:08.000000 pyphetools-0.9.8/src/pyphetools/creation/disease_id_column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553     5966 2023-11-19 07:48:16.000000 pyphetools-0.9.8/src/pyphetools/creation/hgvs_variant.py
--rw-r--r--   0 robinp   (904623974) 1088672553     6073 2023-11-24 08:23:43.000000 pyphetools-0.9.8/src/pyphetools/creation/hp_term.py
--rw-r--r--   0 robinp   (904623974) 1088672553     2228 2023-11-29 08:07:02.000000 pyphetools-0.9.8/src/pyphetools/creation/hpo_cr.py
--rw-r--r--   0 robinp   (904623974) 1088672553    11557 2023-11-29 09:06:11.000000 pyphetools-0.9.8/src/pyphetools/creation/hpo_exact_cr.py
--rw-r--r--   0 robinp   (904623974) 1088672553     2875 2023-10-15 12:52:45.000000 pyphetools-0.9.8/src/pyphetools/creation/hpo_parser.py
--rw-r--r--   0 robinp   (904623974) 1088672553    16110 2023-12-05 13:28:07.000000 pyphetools-0.9.8/src/pyphetools/creation/individual.py
--rw-r--r--   0 robinp   (904623974) 1088672553     9134 2023-12-03 14:38:15.000000 pyphetools-0.9.8/src/pyphetools/creation/metadata.py
--rw-r--r--   0 robinp   (904623974) 1088672553     8280 2023-11-19 07:48:16.000000 pyphetools-0.9.8/src/pyphetools/creation/mixed_cohort_encoder.py
--rw-r--r--   0 robinp   (904623974) 1088672553     9130 2023-11-29 09:16:36.000000 pyphetools-0.9.8/src/pyphetools/creation/option_column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553     2902 2023-10-15 13:02:16.000000 pyphetools-0.9.8/src/pyphetools/creation/sex_column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553     6567 2023-12-05 07:36:33.000000 pyphetools-0.9.8/src/pyphetools/creation/simple_column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553     9179 2023-11-19 06:53:20.000000 pyphetools-0.9.8/src/pyphetools/creation/structural_variant.py
--rw-r--r--   0 robinp   (904623974) 1088672553     2949 2023-11-11 21:18:43.000000 pyphetools-0.9.8/src/pyphetools/creation/thresholded_column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553     1841 2023-09-28 17:50:55.000000 pyphetools-0.9.8/src/pyphetools/creation/variant.py
--rw-r--r--   0 robinp   (904623974) 1088672553     4902 2023-10-14 17:25:22.000000 pyphetools-0.9.8/src/pyphetools/creation/variant_column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553     4153 2023-09-28 17:51:00.000000 pyphetools-0.9.8/src/pyphetools/creation/variant_validator.py
-drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-05 14:07:22.526351 pyphetools-0.9.8/src/pyphetools/validation/
--rw-r--r--   0 robinp   (904623974) 1088672553      421 2023-11-23 07:21:16.000000 pyphetools-0.9.8/src/pyphetools/validation/__init__.py
--rw-r--r--   0 robinp   (904623974) 1088672553     2586 2023-12-02 13:38:25.000000 pyphetools-0.9.8/src/pyphetools/validation/cohort_validator.py
--rw-r--r--   0 robinp   (904623974) 1088672553     7274 2023-11-25 16:19:51.000000 pyphetools-0.9.8/src/pyphetools/validation/content_validator.py
--rw-r--r--   0 robinp   (904623974) 1088672553     9158 2023-12-05 07:42:45.000000 pyphetools-0.9.8/src/pyphetools/validation/ontology_qc.py
--rw-r--r--   0 robinp   (904623974) 1088672553      267 2023-10-25 07:05:50.000000 pyphetools-0.9.8/src/pyphetools/validation/phenopacket_validator.py
--rw-r--r--   0 robinp   (904623974) 1088672553     2735 2023-12-05 13:38:24.000000 pyphetools-0.9.8/src/pyphetools/validation/validated_individual.py
--rw-r--r--   0 robinp   (904623974) 1088672553    10081 2023-12-05 14:01:30.000000 pyphetools-0.9.8/src/pyphetools/validation/validation_result.py
-drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-05 14:07:22.541526 pyphetools-0.9.8/src/pyphetools/visualization/
--rw-r--r--   0 robinp   (904623974) 1088672553      416 2023-11-14 11:38:23.000000 pyphetools-0.9.8/src/pyphetools/visualization/__init__.py
--rw-r--r--   0 robinp   (904623974) 1088672553     7040 2023-11-19 07:48:16.000000 pyphetools-0.9.8/src/pyphetools/visualization/detailed_suppl_table.py
--rw-r--r--   0 robinp   (904623974) 1088672553     5693 2023-11-19 07:48:16.000000 pyphetools-0.9.8/src/pyphetools/visualization/focus_count_table.py
--rw-r--r--   0 robinp   (904623974) 1088672553     2980 2023-09-18 21:32:39.000000 pyphetools-0.9.8/src/pyphetools/visualization/hpo_category.py
--rw-r--r--   0 robinp   (904623974) 1088672553     7303 2023-11-19 07:48:16.000000 pyphetools-0.9.8/src/pyphetools/visualization/hpoa_table_creator.py
--rw-r--r--   0 robinp   (904623974) 1088672553     1366 2023-11-20 07:10:51.000000 pyphetools-0.9.8/src/pyphetools/visualization/html_table_generator.py
--rw-r--r--   0 robinp   (904623974) 1088672553     1694 2023-11-19 06:46:01.000000 pyphetools-0.9.8/src/pyphetools/visualization/phenopacket_ingestor.py
--rw-r--r--   0 robinp   (904623974) 1088672553     9526 2023-12-02 12:27:50.000000 pyphetools-0.9.8/src/pyphetools/visualization/phenopacket_table.py
--rw-r--r--   0 robinp   (904623974) 1088672553     9620 2023-12-05 13:29:54.000000 pyphetools-0.9.8/src/pyphetools/visualization/qc_visualizer.py
--rw-r--r--   0 robinp   (904623974) 1088672553     6987 2023-11-19 09:19:38.000000 pyphetools-0.9.8/src/pyphetools/visualization/simple_patient.py
--rw-r--r--   0 robinp   (904623974) 1088672553     5840 2023-11-19 07:48:16.000000 pyphetools-0.9.8/src/pyphetools/visualization/simple_variant.py
--rw-r--r--   0 robinp   (904623974) 1088672553      569 2023-09-18 21:32:39.000000 pyphetools-0.9.8/src/pyphetools/visualization/term_count.py
-drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-05 14:07:22.576882 pyphetools-0.9.8/test/
--rw-r--r--   0 robinp   (904623974) 1088672553     4766 2023-11-12 16:12:40.000000 pyphetools-0.9.8/test/test_age_column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553     2003 2023-10-25 06:44:57.000000 pyphetools-0.9.8/test/test_age_isoformater.py
--rw-r--r--   0 robinp   (904623974) 1088672553     3026 2023-11-14 10:48:33.000000 pyphetools-0.9.8/test/test_assume_excluded.py
--rw-r--r--   0 robinp   (904623974) 1088672553     4522 2023-11-27 12:05:56.000000 pyphetools-0.9.8/test/test_case_encoder.py
--rw-r--r--   0 robinp   (904623974) 1088672553     4075 2023-12-05 09:09:58.000000 pyphetools-0.9.8/test/test_cohort_validator.py
--rw-r--r--   0 robinp   (904623974) 1088672553     1160 2023-11-19 06:54:43.000000 pyphetools-0.9.8/test/test_constant_column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553     1415 2023-11-19 07:48:16.000000 pyphetools-0.9.8/test/test_hp_term.py
--rw-r--r--   0 robinp   (904623974) 1088672553      925 2023-09-18 21:32:39.000000 pyphetools-0.9.8/test/test_hpo_category.py
--rw-r--r--   0 robinp   (904623974) 1088672553     6687 2023-11-29 08:47:33.000000 pyphetools-0.9.8/test/test_hpo_cr.py
--rw-r--r--   0 robinp   (904623974) 1088672553      839 2023-09-18 00:23:19.000000 pyphetools-0.9.8/test/test_hpo_parser.py
--rw-r--r--   0 robinp   (904623974) 1088672553     2749 2023-11-27 12:08:08.000000 pyphetools-0.9.8/test/test_metadata.py
--rw-r--r--   0 robinp   (904623974) 1088672553     5355 2023-12-05 09:07:49.000000 pyphetools-0.9.8/test/test_ontology_qc.py
--rw-r--r--   0 robinp   (904623974) 1088672553     7443 2023-11-19 07:48:16.000000 pyphetools-0.9.8/test/test_option_column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553     9551 2023-11-29 09:12:50.000000 pyphetools-0.9.8/test/test_option_column_mapper2.py
--rw-r--r--   0 robinp   (904623974) 1088672553      848 2023-11-20 21:20:20.000000 pyphetools-0.9.8/test/test_phenopacket_table.py
--rw-r--r--   0 robinp   (904623974) 1088672553     1164 2023-10-02 00:47:18.000000 pyphetools-0.9.8/test/test_simple_variant.py
--rw-r--r--   0 robinp   (904623974) 1088672553     1478 2023-11-19 06:41:10.000000 pyphetools-0.9.8/test/test_structural_variant.py
--rw-r--r--   0 robinp   (904623974) 1088672553     1860 2023-09-18 00:23:19.000000 pyphetools-0.9.8/test/test_threshold_column_mapper.py
--rw-r--r--   0 robinp   (904623974) 1088672553     3229 2023-12-05 14:03:30.000000 pyphetools-0.9.8/test/test_validation_result.py
--rw-r--r--   0 robinp   (904623974) 1088672553     1395 2023-11-12 16:02:14.000000 pyphetools-0.9.8/test/test_variant.py
+drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-06 13:56:54.420699 pyphetools-0.9.9/
+-rw-r--r--   0 robinp   (904623974) 1088672553     1079 2023-01-08 15:20:15.000000 pyphetools-0.9.9/LICENSE
+-rw-r--r--   0 robinp   (904623974) 1088672553        0 2023-01-05 13:57:40.000000 pyphetools-0.9.9/MANIFEST.in
+-rw-r--r--   0 robinp   (904623974) 1088672553     3109 2023-12-06 13:56:54.420028 pyphetools-0.9.9/PKG-INFO
+-rw-r--r--   0 robinp   (904623974) 1088672553      791 2023-09-30 00:15:51.000000 pyphetools-0.9.9/README.md
+drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-06 13:56:54.017914 pyphetools-0.9.9/ppt_venv/
+drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-06 13:56:54.100066 pyphetools-0.9.9/ppt_venv/bin/
+-rwxr-xr-x   0 robinp   (904623974) 1088672553      630 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rst2html.py
+-rwxr-xr-x   0 robinp   (904623974) 1088672553      750 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rst2html4.py
+-rwxr-xr-x   0 robinp   (904623974) 1088672553     1118 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rst2html5.py
+-rwxr-xr-x   0 robinp   (904623974) 1088672553      827 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rst2latex.py
+-rwxr-xr-x   0 robinp   (904623974) 1088672553      635 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rst2man.py
+-rwxr-xr-x   0 robinp   (904623974) 1088672553      800 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rst2odt.py
+-rwxr-xr-x   0 robinp   (904623974) 1088672553     1762 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 robinp   (904623974) 1088672553      637 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 robinp   (904623974) 1088672553      673 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rst2s5.py
+-rwxr-xr-x   0 robinp   (904623974) 1088672553      907 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rst2xetex.py
+-rwxr-xr-x   0 robinp   (904623974) 1088672553      638 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rst2xml.py
+-rwxr-xr-x   0 robinp   (904623974) 1088672553      706 2023-08-28 06:42:13.000000 pyphetools-0.9.9/ppt_venv/bin/rstpep2html.py
+drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-06 13:56:54.419213 pyphetools-0.9.9/pyphetools.egg-info/
+-rw-r--r--   0 robinp   (904623974) 1088672553     3109 2023-12-06 13:56:53.000000 pyphetools-0.9.9/pyphetools.egg-info/PKG-INFO
+-rw-r--r--   0 robinp   (904623974) 1088672553     5557 2023-12-06 13:56:54.000000 pyphetools-0.9.9/pyphetools.egg-info/SOURCES.txt
+-rw-r--r--   0 robinp   (904623974) 1088672553        1 2023-12-06 13:56:53.000000 pyphetools-0.9.9/pyphetools.egg-info/dependency_links.txt
+-rw-r--r--   0 robinp   (904623974) 1088672553        1 2023-08-30 08:37:05.000000 pyphetools-0.9.9/pyphetools.egg-info/not-zip-safe
+-rw-r--r--   0 robinp   (904623974) 1088672553       81 2023-12-06 13:56:53.000000 pyphetools-0.9.9/pyphetools.egg-info/requires.txt
+-rw-r--r--   0 robinp   (904623974) 1088672553       71 2023-12-06 13:56:53.000000 pyphetools-0.9.9/pyphetools.egg-info/top_level.txt
+-rw-r--r--   0 robinp   (904623974) 1088672553     1833 2023-10-12 20:14:59.000000 pyphetools-0.9.9/pyproject.toml
+-rw-r--r--   0 robinp   (904623974) 1088672553       38 2023-12-06 13:56:54.420772 pyphetools-0.9.9/setup.cfg
+drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-06 13:56:54.019189 pyphetools-0.9.9/src/
+drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-06 13:56:54.337929 pyphetools-0.9.9/src/pyphetools/
+-rw-r--r--   0 robinp   (904623974) 1088672553      180 2023-12-06 13:56:07.000000 pyphetools-0.9.9/src/pyphetools/__init__.py
+drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-06 13:56:54.379289 pyphetools-0.9.9/src/pyphetools/creation/
+-rw-r--r--   0 robinp   (904623974) 1088672553     1871 2023-12-05 15:45:33.000000 pyphetools-0.9.9/src/pyphetools/creation/__init__.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     1905 2023-12-02 13:48:44.000000 pyphetools-0.9.9/src/pyphetools/creation/abstract_encoder.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     7296 2023-11-19 07:48:16.000000 pyphetools-0.9.9/src/pyphetools/creation/age_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     3249 2023-10-25 06:40:55.000000 pyphetools-0.9.9/src/pyphetools/creation/age_isoformater.py
+-rw-r--r--   0 robinp   (904623974) 1088672553      117 2023-11-16 08:39:03.000000 pyphetools-0.9.9/src/pyphetools/creation/allelic_requirement.py
+-rw-r--r--   0 robinp   (904623974) 1088672553    12272 2023-11-27 12:05:13.000000 pyphetools-0.9.9/src/pyphetools/creation/case_encoder.py
+-rw-r--r--   0 robinp   (904623974) 1088672553      577 2023-11-27 12:00:38.000000 pyphetools-0.9.9/src/pyphetools/creation/citation.py
+-rw-r--r--   0 robinp   (904623974) 1088672553    10738 2023-12-02 13:37:26.000000 pyphetools-0.9.9/src/pyphetools/creation/cohort_encoder.py
+-rw-r--r--   0 robinp   (904623974) 1088672553      679 2023-10-15 12:30:42.000000 pyphetools-0.9.9/src/pyphetools/creation/column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     2401 2023-11-19 06:55:43.000000 pyphetools-0.9.9/src/pyphetools/creation/constant_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553      310 2023-11-16 08:22:53.000000 pyphetools-0.9.9/src/pyphetools/creation/constants.py
+-rw-r--r--   0 robinp   (904623974) 1088672553      745 2023-11-13 14:50:53.000000 pyphetools-0.9.9/src/pyphetools/creation/disease.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     1083 2023-10-16 07:36:08.000000 pyphetools-0.9.9/src/pyphetools/creation/disease_id_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     5966 2023-11-19 07:48:16.000000 pyphetools-0.9.9/src/pyphetools/creation/hgvs_variant.py
+-rw-r--r--   0 robinp   (904623974) 1088672553    10732 2023-12-05 15:58:54.000000 pyphetools-0.9.9/src/pyphetools/creation/hp_term.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     2228 2023-11-29 08:07:02.000000 pyphetools-0.9.9/src/pyphetools/creation/hpo_cr.py
+-rw-r--r--   0 robinp   (904623974) 1088672553    11557 2023-11-29 09:06:11.000000 pyphetools-0.9.9/src/pyphetools/creation/hpo_exact_cr.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     2875 2023-10-15 12:52:45.000000 pyphetools-0.9.9/src/pyphetools/creation/hpo_parser.py
+-rw-r--r--   0 robinp   (904623974) 1088672553    16116 2023-12-05 15:58:54.000000 pyphetools-0.9.9/src/pyphetools/creation/individual.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     9134 2023-12-03 14:38:15.000000 pyphetools-0.9.9/src/pyphetools/creation/metadata.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     8320 2023-12-06 13:02:45.000000 pyphetools-0.9.9/src/pyphetools/creation/mixed_cohort_encoder.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     9130 2023-11-29 09:16:36.000000 pyphetools-0.9.9/src/pyphetools/creation/option_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     2902 2023-10-15 13:02:16.000000 pyphetools-0.9.9/src/pyphetools/creation/sex_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     6567 2023-12-05 07:36:33.000000 pyphetools-0.9.9/src/pyphetools/creation/simple_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     9179 2023-11-19 06:53:20.000000 pyphetools-0.9.9/src/pyphetools/creation/structural_variant.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     2949 2023-11-11 21:18:43.000000 pyphetools-0.9.9/src/pyphetools/creation/thresholded_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     1841 2023-09-28 17:50:55.000000 pyphetools-0.9.9/src/pyphetools/creation/variant.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     4902 2023-10-14 17:25:22.000000 pyphetools-0.9.9/src/pyphetools/creation/variant_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     4122 2023-12-06 12:56:24.000000 pyphetools-0.9.9/src/pyphetools/creation/variant_validator.py
+drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-06 13:56:54.386571 pyphetools-0.9.9/src/pyphetools/validation/
+-rw-r--r--   0 robinp   (904623974) 1088672553      421 2023-11-23 07:21:16.000000 pyphetools-0.9.9/src/pyphetools/validation/__init__.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     2586 2023-12-02 13:38:25.000000 pyphetools-0.9.9/src/pyphetools/validation/cohort_validator.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     7274 2023-11-25 16:19:51.000000 pyphetools-0.9.9/src/pyphetools/validation/content_validator.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     9158 2023-12-05 07:42:45.000000 pyphetools-0.9.9/src/pyphetools/validation/ontology_qc.py
+-rw-r--r--   0 robinp   (904623974) 1088672553      267 2023-10-25 07:05:50.000000 pyphetools-0.9.9/src/pyphetools/validation/phenopacket_validator.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     2735 2023-12-05 13:38:24.000000 pyphetools-0.9.9/src/pyphetools/validation/validated_individual.py
+-rw-r--r--   0 robinp   (904623974) 1088672553    10081 2023-12-05 14:01:30.000000 pyphetools-0.9.9/src/pyphetools/validation/validation_result.py
+drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-06 13:56:54.393993 pyphetools-0.9.9/src/pyphetools/visualization/
+-rw-r--r--   0 robinp   (904623974) 1088672553      416 2023-11-14 11:38:23.000000 pyphetools-0.9.9/src/pyphetools/visualization/__init__.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     7040 2023-11-19 07:48:16.000000 pyphetools-0.9.9/src/pyphetools/visualization/detailed_suppl_table.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     5693 2023-11-19 07:48:16.000000 pyphetools-0.9.9/src/pyphetools/visualization/focus_count_table.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     2980 2023-09-18 21:32:39.000000 pyphetools-0.9.9/src/pyphetools/visualization/hpo_category.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     7303 2023-11-19 07:48:16.000000 pyphetools-0.9.9/src/pyphetools/visualization/hpoa_table_creator.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     1366 2023-11-20 07:10:51.000000 pyphetools-0.9.9/src/pyphetools/visualization/html_table_generator.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     1694 2023-11-19 06:46:01.000000 pyphetools-0.9.9/src/pyphetools/visualization/phenopacket_ingestor.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     9526 2023-12-02 12:27:50.000000 pyphetools-0.9.9/src/pyphetools/visualization/phenopacket_table.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     9620 2023-12-05 13:29:54.000000 pyphetools-0.9.9/src/pyphetools/visualization/qc_visualizer.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     6987 2023-11-19 09:19:38.000000 pyphetools-0.9.9/src/pyphetools/visualization/simple_patient.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     5840 2023-11-19 07:48:16.000000 pyphetools-0.9.9/src/pyphetools/visualization/simple_variant.py
+-rw-r--r--   0 robinp   (904623974) 1088672553      569 2023-09-18 21:32:39.000000 pyphetools-0.9.9/src/pyphetools/visualization/term_count.py
+drwxr-xr-x   0 robinp   (904623974) 1088672553        0 2023-12-06 13:56:54.418473 pyphetools-0.9.9/test/
+-rw-r--r--   0 robinp   (904623974) 1088672553     4766 2023-11-12 16:12:40.000000 pyphetools-0.9.9/test/test_age_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     2003 2023-10-25 06:44:57.000000 pyphetools-0.9.9/test/test_age_isoformater.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     3026 2023-11-14 10:48:33.000000 pyphetools-0.9.9/test/test_assume_excluded.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     4522 2023-11-27 12:05:56.000000 pyphetools-0.9.9/test/test_case_encoder.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     4075 2023-12-05 09:09:58.000000 pyphetools-0.9.9/test/test_cohort_validator.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     1160 2023-11-19 06:54:43.000000 pyphetools-0.9.9/test/test_constant_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     3879 2023-12-05 16:11:01.000000 pyphetools-0.9.9/test/test_hp_term.py
+-rw-r--r--   0 robinp   (904623974) 1088672553      925 2023-09-18 21:32:39.000000 pyphetools-0.9.9/test/test_hpo_category.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     6687 2023-11-29 08:47:33.000000 pyphetools-0.9.9/test/test_hpo_cr.py
+-rw-r--r--   0 robinp   (904623974) 1088672553      839 2023-09-18 00:23:19.000000 pyphetools-0.9.9/test/test_hpo_parser.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     2749 2023-11-27 12:08:08.000000 pyphetools-0.9.9/test/test_metadata.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     5355 2023-12-05 09:07:49.000000 pyphetools-0.9.9/test/test_ontology_qc.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     7443 2023-11-19 07:48:16.000000 pyphetools-0.9.9/test/test_option_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     9551 2023-11-29 09:12:50.000000 pyphetools-0.9.9/test/test_option_column_mapper2.py
+-rw-r--r--   0 robinp   (904623974) 1088672553      848 2023-11-20 21:20:20.000000 pyphetools-0.9.9/test/test_phenopacket_table.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     1164 2023-10-02 00:47:18.000000 pyphetools-0.9.9/test/test_simple_variant.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     1478 2023-11-19 06:41:10.000000 pyphetools-0.9.9/test/test_structural_variant.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     1860 2023-09-18 00:23:19.000000 pyphetools-0.9.9/test/test_threshold_column_mapper.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     3229 2023-12-05 14:03:30.000000 pyphetools-0.9.9/test/test_validation_result.py
+-rw-r--r--   0 robinp   (904623974) 1088672553     1395 2023-11-12 16:02:14.000000 pyphetools-0.9.9/test/test_variant.py
```

### Comparing `pyphetools-0.9.8/LICENSE` & `pyphetools-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/PKG-INFO` & `pyphetools-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphetools
-Version: 0.9.8
+Version: 0.9.9
 Summary: Generate and work with GA4GH phenopackets
 Author-email: Peter Robinson <peter.robinson@jax.org>
 License: MIT License
         
         Copyright (c) 2023, The Monarch Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyphetools-0.9.8/README.md` & `pyphetools-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/ppt_venv/bin/rst2html.py` & `pyphetools-0.9.9/ppt_venv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/ppt_venv/bin/rst2html4.py` & `pyphetools-0.9.9/ppt_venv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/ppt_venv/bin/rst2html5.py` & `pyphetools-0.9.9/ppt_venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/ppt_venv/bin/rst2latex.py` & `pyphetools-0.9.9/ppt_venv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/ppt_venv/bin/rst2man.py` & `pyphetools-0.9.9/ppt_venv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/ppt_venv/bin/rst2odt.py` & `pyphetools-0.9.9/ppt_venv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/ppt_venv/bin/rst2odt_prepstyles.py` & `pyphetools-0.9.9/ppt_venv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/ppt_venv/bin/rst2pseudoxml.py` & `pyphetools-0.9.9/ppt_venv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/ppt_venv/bin/rst2s5.py` & `pyphetools-0.9.9/ppt_venv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/ppt_venv/bin/rst2xetex.py` & `pyphetools-0.9.9/ppt_venv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/ppt_venv/bin/rst2xml.py` & `pyphetools-0.9.9/ppt_venv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/ppt_venv/bin/rstpep2html.py` & `pyphetools-0.9.9/ppt_venv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/pyphetools.egg-info/PKG-INFO` & `pyphetools-0.9.9/pyphetools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyphetools
-Version: 0.9.8
+Version: 0.9.9
 Summary: Generate and work with GA4GH phenopackets
 Author-email: Peter Robinson <peter.robinson@jax.org>
 License: MIT License
         
         Copyright (c) 2023, The Monarch Initiative
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyphetools-0.9.8/pyphetools.egg-info/SOURCES.txt` & `pyphetools-0.9.9/pyphetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/pyproject.toml` & `pyphetools-0.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/__init__.py` & `pyphetools-0.9.9/src/pyphetools/creation/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .constant_column_mapper import ConstantColumnMapper
 from .disease import Disease
 from .disease_id_column_mapper import DiseaseIdColumnMapper
 from .hgvs_variant import HgvsVariant
 from .hpo_cr import HpoConceptRecognizer
 from .hpo_exact_cr import HpoExactConceptRecognizer
 from .hpo_parser import HpoParser
-from .hp_term import HpTerm
+from .hp_term import HpTerm, HpTermBuilder
 from .individual import Individual
 from .metadata import MetaData
 from .mixed_cohort_encoder import MixedCohortEncoder
 from .option_column_mapper import OptionColumnMapper
 from .sex_column_mapper import SexColumnMapper
 from .simple_column_mapper import SimpleColumnMapper, SimpleColumnMapperGenerator
 from .structural_variant import StructuralVariant
@@ -39,14 +39,15 @@
     "Disease",
     "DiseaseIdColumnMapper",
     "HgvsVariant",
     "HpoConceptRecognizer",
     "HpoExactConceptRecognizer",
     "HpoParser",
     "HpTerm",
+    "HpTermBuilder",
     "Individual",
     "MetaData",
     "MixedCohortEncoder",
     "OptionColumnMapper",
     "SexColumnMapper",
     "SimpleColumnMapper",
     "SimpleColumnMapperGenerator",
```

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/abstract_encoder.py` & `pyphetools-0.9.9/src/pyphetools/creation/abstract_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/age_column_mapper.py` & `pyphetools-0.9.9/src/pyphetools/creation/age_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/age_isoformater.py` & `pyphetools-0.9.9/src/pyphetools/creation/age_isoformater.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/case_encoder.py` & `pyphetools-0.9.9/src/pyphetools/creation/case_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/citation.py` & `pyphetools-0.9.9/src/pyphetools/creation/citation.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/cohort_encoder.py` & `pyphetools-0.9.9/src/pyphetools/creation/cohort_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/column_mapper.py` & `pyphetools-0.9.9/src/pyphetools/creation/column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/constant_column_mapper.py` & `pyphetools-0.9.9/src/pyphetools/creation/constant_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/disease.py` & `pyphetools-0.9.9/src/pyphetools/creation/disease.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/disease_id_column_mapper.py` & `pyphetools-0.9.9/src/pyphetools/creation/disease_id_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/hgvs_variant.py` & `pyphetools-0.9.9/src/pyphetools/creation/hgvs_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/hp_term.py` & `pyphetools-0.9.9/src/pyphetools/creation/hp_term.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pandas as pd
-import phenopackets
+import phenopackets as PPKt
 from .constants import Constants
 import hpotk
 
 class HpTerm:
     """
     Class to represent a phenotypic observation as an HPO term with optional modifiers
 
@@ -16,27 +16,28 @@
     :param measured: a boolean that indicates whether the HPO was measured (True) or not explicitly measured (False)
     :type measured: bool
     :param onset: an ISO8601 string representing the age of onset, optional
     :type onset: str
     :param resolution: an ISO8601 string representing the age of resolution, optional
     :type resolution: str
     """
-    def __init__(self, hpo_id, label, observed=True, measured=True, onset=Constants.NOT_PROVIDED, resolution=None):
+    def __init__(self, hpo_id, label, observed=True, measured=True, onset=Constants.NOT_PROVIDED, onset_term=None, resolution=None):
         if hpo_id is None or len(hpo_id) == 0 or not hpo_id.startswith("HP"):
             raise ValueError(f"invalid id argument: '{hpo_id}'")
         if label is None or len(label) == 0:
             raise ValueError(f"invalid label argument: '{label}'")
         self._id = hpo_id
         self._label = label
         self._observed = observed
         self._measured = measured
         if onset is None:
             self._onset = Constants.NOT_PROVIDED
         else:
             self._onset = onset
+        self._onset_term = onset_term
         if resolution is None:
             self._resolution = Constants.NOT_PROVIDED
         else:
             self._resolution = resolution
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
@@ -83,14 +84,18 @@
         """
         return self._onset
 
     def set_onset(self, onset):
         self._onset = onset
 
     @property
+    def onset_term(self):
+        return self._onset_term
+
+    @property
     def resolution(self):
         """
         :returns: iso8601 string representing the age this abnormality resolved
         :rtype: str, optional
         """
         return self._resolution
 
@@ -128,26 +133,31 @@
 
     def excluded(self):
         """
         Sets the current term to excluded (i.e., the abnormality was sought but explicitly ruled out clinically)
         """
         self._observed = False
 
-    def to_phenotypic_feature(self):
+    def to_ga4gh_phenotypic_feature(self):
         """
         :returns: A GA4GH PhenotypcFeature corresponding to this HpTerm
         :rtype: phenopackets.PhenotypicFeature
         """
-        pf = phenopackets.PhenotypicFeature()
+        pf = PPKt.PhenotypicFeature()
         pf.type.id = self._id
         pf.type.label = self._label
         if not self._observed:
             pf.excluded = True
         if self._onset != Constants.NOT_PROVIDED:
             pf.onset.age.iso8601duration = self._onset
+        elif self.onset_term is not None:
+            oclass = PPKt.OntologyClass()
+            oclass.id = self._onset_term[1]
+            oclass.label = self._onset_term[0]
+            pf.onset.ontology_class.CopyFrom(oclass)
         if self._resolution != Constants.NOT_PROVIDED:
             pf.resolution.age.iso8601duration = self._resolution
         return pf
 
 
     @staticmethod
     def term_list_to_dataframe(hpo_list):
@@ -174,7 +184,133 @@
         :returns: The corresponding HpTerm object
         :rtype: HpTerm
         """
         hpo_id = hpotk_term.identifier.value
         hpo_label = hpotk_term.name
         return HpTerm(hpo_id=hpo_id, label=hpo_label)
 
+
+class HpTermBuilder:
+
+    def __init__(self, hpo_id:str, hpo_label:str):
+        if not hpo_id.startswith("HP:"):
+            raise ValueError(f"Malformed HPO id {hpo_id}")
+        if not len(hpo_id) == 10:
+            length = len(hpo_id)
+            raise ValueError(f"Malformed HPO id with length {len(hpo_id)}: {hpo_id}")
+        self._hpo_id = hpo_id
+        if hpo_label is None or len(hpo_label) < 3:
+            raise ValueError(f"Malformed HPO label \"{hpo_label}\"")
+        self._hpo_label = hpo_label
+        self._observed=True
+        self._measured=True
+        self._onset=None
+        self._onsetTerm=None
+
+    def excluded(self):
+        self._observed = False
+        return self
+
+    def not_measured(self):
+        self._measured = False
+        return self
+
+    def iso8601_onset(self, onset):
+        self._onset = onset
+        return self
+
+    def embryonal_onset(self):
+        """Onset of disease at up to 8 weeks following fertilization (corresponding to 10 weeks of gestation).
+        """
+        self._onsetTerm = ["Embryonal onset", "HP:0011460"]
+        return self
+
+    def fetal_onset(self):
+        """Onset prior to birth but after 8 weeks of embryonic development (corresponding to a gestational age of 10 weeks).
+        """
+        self._onsetTerm = ["Fetal onset", "HP:0011461"]
+        return self
+
+    def second_trimester_onset(self):
+        """second trimester, which comprises the range of gestational ages from 14 0/7 weeks to 27 6/7 (inclusive)
+        """
+        self._onsetTerm = ["Second trimester onset", "HP:0034198"]
+        return self
+
+    def late_first_trimester_onset(self):
+        """late first trimester during the early fetal period, which is defined as 11 0/7 to 13 6/7 weeks of gestation (inclusive).
+        """
+        self._onsetTerm = ["Late first trimester onset", "HP:0034199"]
+        return self
+
+    def third_trimester_onset(self):
+        """third trimester, which is defined as 28 weeks and zero days (28+0) of gestation and beyond.
+        """
+        self._onsetTerm = ["Third trimester onset", "HP:0034197"]
+        return self
+
+    def antenatal_onset(self):
+        """onset prior to birth
+        """
+        self._onsetTerm = ["Antenatal onset", "HP:0030674"]
+        return self
+
+    def congenital_onset(self):
+        """A phenotypic abnormality that is present at birth.
+        """
+        self._onsetTerm = ["Congenital onset", "HP:0003577"]
+        return self
+
+    def neonatal_onset(self):
+        """Onset of signs or symptoms of disease within the first 28 days of life.
+        """
+        self._onsetTerm = ["Neonatal onset", "HP:0003623"]
+        return self
+
+
+    def infantile_onset(self):
+        """Onset of signs or symptoms of disease between 28 days to one year of life.
+        """
+        self._onsetTerm = ["Infantile onset", "HP:0003593"]
+        return self
+
+    def childhood_onset(self):
+        """Onset of disease at the age of between 1 and 5 years.
+        """
+        self._onsetTerm = ["Childhood onset", "HP:0011463"]
+        return self
+
+    def juvenile_onset(self):
+        """Onset of signs or symptoms of disease between the age of 5 and 15 years.
+        """
+        self._onsetTerm = ["Juvenile onset", "HP:0003621"]
+        return self
+
+    def young_adult_onset(self):
+        """Onset of disease at the age of between 16 and 40 years.
+        """
+        self._onsetTerm = ["Young adult onset", "HP:0011462"]
+        return self
+
+    def middle_age_onset(self):
+        """onset of symptoms at the age of 40 to 60 years.
+        """
+        self._onsetTerm = ["Middle age onset", "HP:0003596"]
+        return self
+
+    def late_onset(self):
+        """Onset of symptoms after the age of 60 years.
+        """
+        self._onsetTerm = ["Late onset", "HP:0003584"]
+        return self
+
+    def build(self) -> HpTerm:
+        if self._onset is not None and self._onsetTerm is not None:
+            raise ValueError("Both onset and onsetTerm were set but only a maximum of one of them may be not None")
+        return HpTerm(hpo_id=self._hpo_id,
+                    label=self._hpo_label,
+                    observed=self._observed,
+                    measured=self._measured,
+                    onset=self._onset,
+                    onset_term=self._onsetTerm)
+
+
```

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/hpo_cr.py` & `pyphetools-0.9.9/src/pyphetools/creation/hpo_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/hpo_exact_cr.py` & `pyphetools-0.9.9/src/pyphetools/creation/hpo_exact_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/hpo_parser.py` & `pyphetools-0.9.9/src/pyphetools/creation/hpo_parser.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/individual.py` & `pyphetools-0.9.9/src/pyphetools/creation/individual.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
             php.subject.sex = PPKt.Sex.UNKNOWN_SEX
         if self._age is not None and self._age != Constants.NOT_PROVIDED:
             php.subject.time_at_last_encounter.age.iso8601duration = self._age
         if isinstance(self._hpo_terms, list):
             for hp in self._hpo_terms:
                 if not hp.measured:
                     continue
-                pf = hp.to_phenotypic_feature()
+                pf = hp.to_ga4gh_phenotypic_feature()
                 if pf.onset.age.iso8601duration is None and self._age != Constants.NOT_PROVIDED:
                     pf.onset.age.iso8601duration = self._age
                 php.phenotypic_features.append(pf)
         elif isinstance(self._hpo_terms, dict):
             for age_key, hpoterm_list in self._hpo_terms.items():
                 for hp in hpoterm_list:
                     if not hp.measured:
```

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/metadata.py` & `pyphetools-0.9.9/src/pyphetools/creation/metadata.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/mixed_cohort_encoder.py` & `pyphetools-0.9.9/src/pyphetools/creation/mixed_cohort_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import List, Dict
 
 import pandas as pd
 
 from . import Individual
 from .abstract_encoder import AbstractEncoder
 from .age_column_mapper import AgeColumnMapper
+from .citation import Citation
 from .constants import Constants
 from .hpo_cr import HpoConceptRecognizer
 from .sex_column_mapper import SexColumnMapper
 
 
 class MixedCohortEncoder(AbstractEncoder):
     """Map a table of data to Individual/GA4GH Phenopacket Schema objects. This class should be used instead of CohortMapper
@@ -148,17 +149,17 @@
                     interpretation_list = []
             else:
                 interpretation_list = []
             disease_cell_contents = row[disease_column_name]
             if disease_cell_contents is None:
                 raise ValueError(f"Could not extract disease identifier for row {row}")
             disease = self._disease_id_mapper.map_cell(disease_cell_contents)
+            cite = Citation(pmid=pmid, title=title)
             indi = Individual(individual_id=individual_id,
                                   sex=sex,
                                   age=age,
                                   hpo_terms=hpo_terms,
-                                  pmid=pmid,
-                                  title=title,
+                                  citation=cite,
                                   interpretation_list=interpretation_list,
                                   disease=disease)
             individuals.append(indi)
         return individuals
```

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/option_column_mapper.py` & `pyphetools-0.9.9/src/pyphetools/creation/option_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/sex_column_mapper.py` & `pyphetools-0.9.9/src/pyphetools/creation/sex_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/simple_column_mapper.py` & `pyphetools-0.9.9/src/pyphetools/creation/simple_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/structural_variant.py` & `pyphetools-0.9.9/src/pyphetools/creation/structural_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/thresholded_column_mapper.py` & `pyphetools-0.9.9/src/pyphetools/creation/thresholded_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/variant.py` & `pyphetools-0.9.9/src/pyphetools/creation/variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/variant_column_mapper.py` & `pyphetools-0.9.9/src/pyphetools/creation/variant_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/creation/variant_validator.py` & `pyphetools-0.9.9/src/pyphetools/creation/variant_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,24 +15,24 @@
     encode_hgvs method.
 
     :param genome_build: The genome assembly, one of "GRCh37", "GRCh38", "hg19", "hg38"
     :type genome_build: str
     :param transcript: An mRNA transcript that is the reference for the HGVS string, opt
     :type transcript: str
     """
-    
+
     def __init__(self, genome_build, transcript=None):
         """
         Constructor
         """
         if genome_build not in ACCEPTABLE_GENOMES:
             raise ValueError(f"genome_build \"{genome_build}\" not recognized")
         self._genome_assembly = genome_build
         self._transcript = transcript
-        
+
     def encode_hgvs(self, hgvs, custom_transcript=None):
         """
         Encode an HGVS string as a pyphetools Variant object
 
         :param hgvs: Human Genome Variation Society (HGVS) representation of a variant, e.g., c.36613706dup
         :type hgvs: str
         :param custom_transcript: a transcript (e.g., NM_001848.2), if different from the default transcript, optional
@@ -49,15 +49,15 @@
         api_url = URL_SCHEME % (self._genome_assembly, transcript, hgvs, transcript)
         #f"https://rest.variantvalidator.org/VariantValidator/variantvalidator/{self._genome_assembly}/{transcript}%3A{hgvs}/{transcript}"
         #
         print(api_url)
         response = requests.get(api_url)
         # We expect to get a dictionary with three keys. The first is the name of the variant, e.g., ACC:HGVS, then we
         # get flag and metadata
-        vv_dict = response.json() 
+        vv_dict = response.json()
         if 'flag' in vv_dict:
             if vv_dict['flag'] != 'gene_variant':
                 flag = vv_dict['flag']
                 raise ValueError(f"Expecting to get a gene_variant from Variant Validator but got {flag}")
         # This is the easiest way to get the variant key, which may contain difficult characters
         variant_key = [k for k in vv_dict.keys() if k not in {'flag', 'metadata'}][0]
         var = vv_dict[variant_key]
@@ -76,16 +76,14 @@
         reference_sequence_records = var.get('reference_sequence_records', None)
         if reference_sequence_records is not None:
             transcript = reference_sequence_records['transcript']
             if transcript.startswith('https://www.ncbi.nlm.nih.gov/nuccore/'):
                 transcript = transcript[37:]
         else:
             transcript = None
-       
         # 'vcf': {'alt': 'C', 'chr': '16', 'pos': '1756403', 'ref': 'CG'}},
         if not 'vcf' in assembly:
             raise ValueError(f"Could not identify vcf element in Variant Validator genome assembly response")
-        return HgvsVariant(assembly=self._genome_assembly, vcf_d=assembly['vcf'], symbol=symbol, 
-                       hgnc=hgnc, transcript=transcript, hgvs=hgvs_transcript_var, g_hgvs=genomic_hgvs)
-  
+        return HgvsVariant(assembly=self._genome_assembly, vcf_d=assembly['vcf'], symbol=symbol,
+                        hgnc=hgnc, transcript=transcript, hgvs=hgvs_transcript_var, g_hgvs=genomic_hgvs)
+
 
-
```

### Comparing `pyphetools-0.9.8/src/pyphetools/validation/cohort_validator.py` & `pyphetools-0.9.9/src/pyphetools/validation/cohort_validator.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/validation/content_validator.py` & `pyphetools-0.9.9/src/pyphetools/validation/content_validator.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/validation/ontology_qc.py` & `pyphetools-0.9.9/src/pyphetools/validation/ontology_qc.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/validation/validated_individual.py` & `pyphetools-0.9.9/src/pyphetools/validation/validated_individual.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/validation/validation_result.py` & `pyphetools-0.9.9/src/pyphetools/validation/validation_result.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/visualization/detailed_suppl_table.py` & `pyphetools-0.9.9/src/pyphetools/visualization/detailed_suppl_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/visualization/focus_count_table.py` & `pyphetools-0.9.9/src/pyphetools/visualization/focus_count_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/visualization/hpo_category.py` & `pyphetools-0.9.9/src/pyphetools/visualization/hpo_category.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/visualization/hpoa_table_creator.py` & `pyphetools-0.9.9/src/pyphetools/visualization/hpoa_table_creator.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/visualization/html_table_generator.py` & `pyphetools-0.9.9/src/pyphetools/visualization/html_table_generator.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/visualization/phenopacket_ingestor.py` & `pyphetools-0.9.9/src/pyphetools/visualization/phenopacket_ingestor.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/visualization/phenopacket_table.py` & `pyphetools-0.9.9/src/pyphetools/visualization/phenopacket_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/visualization/qc_visualizer.py` & `pyphetools-0.9.9/src/pyphetools/visualization/qc_visualizer.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/visualization/simple_patient.py` & `pyphetools-0.9.9/src/pyphetools/visualization/simple_patient.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/visualization/simple_variant.py` & `pyphetools-0.9.9/src/pyphetools/visualization/simple_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/src/pyphetools/visualization/term_count.py` & `pyphetools-0.9.9/src/pyphetools/visualization/term_count.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/test/test_age_column_mapper.py` & `pyphetools-0.9.9/test/test_age_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/test/test_age_isoformater.py` & `pyphetools-0.9.9/test/test_age_isoformater.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/test/test_assume_excluded.py` & `pyphetools-0.9.9/test/test_assume_excluded.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/test/test_case_encoder.py` & `pyphetools-0.9.9/test/test_case_encoder.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/test/test_cohort_validator.py` & `pyphetools-0.9.9/test/test_cohort_validator.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/test/test_constant_column_mapper.py` & `pyphetools-0.9.9/test/test_constant_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/test/test_hpo_category.py` & `pyphetools-0.9.9/test/test_hpo_category.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/test/test_hpo_cr.py` & `pyphetools-0.9.9/test/test_hpo_cr.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/test/test_hpo_parser.py` & `pyphetools-0.9.9/test/test_hpo_parser.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/test/test_metadata.py` & `pyphetools-0.9.9/test/test_metadata.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/test/test_ontology_qc.py` & `pyphetools-0.9.9/test/test_ontology_qc.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/test/test_option_column_mapper.py` & `pyphetools-0.9.9/test/test_option_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/test/test_option_column_mapper2.py` & `pyphetools-0.9.9/test/test_option_column_mapper2.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/test/test_phenopacket_table.py` & `pyphetools-0.9.9/test/test_phenopacket_table.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/test/test_simple_variant.py` & `pyphetools-0.9.9/test/test_simple_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/test/test_structural_variant.py` & `pyphetools-0.9.9/test/test_structural_variant.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/test/test_threshold_column_mapper.py` & `pyphetools-0.9.9/test/test_threshold_column_mapper.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/test/test_validation_result.py` & `pyphetools-0.9.9/test/test_validation_result.py`

 * *Files identical despite different names*

### Comparing `pyphetools-0.9.8/test/test_variant.py` & `pyphetools-0.9.9/test/test_variant.py`

 * *Files identical despite different names*

